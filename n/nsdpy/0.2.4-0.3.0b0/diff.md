# Comparing `tmp/nsdpy-0.2.4.tar.gz` & `tmp/nsdpy-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdpy-0.2.4.tar", max compression
+gzip compressed data, was "nsdpy-0.3.0b0.tar", max compression
```

## Comparing `nsdpy-0.2.4.tar` & `nsdpy-0.3.0b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-27 13:47:59.346367 nsdpy-0.2.4/LICENSE
--rw-r--r--   0        0        0     2720 2023-05-27 13:47:59.346590 nsdpy-0.2.4/README.md
--rw-r--r--   0        0        0    35687 2023-05-27 13:47:59.386545 nsdpy-0.2.4/functions.py
--rw-r--r--   0        0        0    12577 2023-05-27 15:10:50.380161 nsdpy-0.2.4/nsdpy.py
--rw-r--r--   0        0        0      836 2023-05-27 15:10:50.297755 nsdpy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 nsdpy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.0b0/LICENSE
+-rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.0b0/README.md
+-rw-r--r--   0        0        0    34827 2023-06-03 12:39:19.745531 nsdpy-0.3.0b0/functions.py
+-rw-r--r--   0        0        0    12984 2023-06-03 12:47:07.435767 nsdpy-0.3.0b0/nsdpy.py
+-rw-r--r--   0        0        0      841 2023-06-03 12:47:07.238777 nsdpy-0.3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.0b0/PKG-INFO
```

### Comparing `nsdpy-0.2.4/LICENSE` & `nsdpy-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsdpy-0.2.4/README.md` & `nsdpy-0.3.0b0/README.md`

 * *Files identical despite different names*

### Comparing `nsdpy-0.2.4/functions.py` & `nsdpy-0.3.0b0/functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-#import from standard library
+ #import from standard library
 import os
 import re
 import csv
 from collections import Counter
-
+from constants import ESEARCH_URL, ESUMMARY_URL, EFETCH_URL, PLANTAE, FUNGI, METAZOA
 #third party imports
 import requests             #https://requests.readthedocs.io/en/master/
 
     
-
 def countDown(iteration, total, message=''):
     """
     Take the number of iteration, the range of a forloop and a message and output a message with the percent of job done
 
     INPUTS: countDown(iteration, total, message='')
     iteration:  positive INT
     total: positive INT
@@ -77,80 +76,76 @@
             print(f'An exception occurred:\n{e}')
             continue
 
     return result
 
 
 def esearchquery(QUERY):
-    ##unpack QUERY:
+    ## unpack QUERY:
     (query, api_key) = QUERY
 
-    ##build api address
-    esearchaddress = 'https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi'
-    #parameters
+    # parameters
     parameters = {}
     if api_key:
         parameters["api_key"] = str(api_key)
     parameters["db"] = "nucleotide"
     parameters["idtype"] = "acc"
     parameters["retmode"] = "json"
     parameters["retmax"] = "0"
     parameters["usehistory"] = "y"    
-    #user's query
+    # user's query
     parameters["term"] = query
     
-    ###send request to the API
-    y = download(parameters, esearchaddress)
+    ### send request to the API
+    y = download(parameters, ESEARCH_URL)
     if y == 1:
         return ({"error": "wrong address for esearch"})  
     return (y.json())
 
 
 def taxids(params, path, OPTIONS=None):
 
     if OPTIONS is None:
         OPTIONS = ("","","","","","")
 
-    ##unpack parameters
+    ## unpack parameters
     (querykey, webenv, count) = params
     (verb, _, _, fileoutput, _, _) = OPTIONS
 
     dict_ids = {}
     taxid = ''
     seqnb = ''
 
-    ##retreive the taxids sending batches of accession numbers to esummary
+    ## retreive the taxids sending batches of accession numbers to esummary
     retmax = 200 
     if count < retmax:
         retmax = count
 
     if count % retmax == 0:
         nb = count//retmax
     else: 
         nb = (count//retmax) + 1
 
     for x in range(nb):
-        ##build the API address
-        esummaryaddress = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esummary.fcgi"
-        #parameters 
+        # parameters 
         parameters = {}
         parameters['db'] = "taxonomy"
         parameters['query_key'] = querykey
         parameters['WebEnv'] = webenv
         parameters['retstart'] = str(x * retmax)
         parameters['retmax'] = str(retmax)
         parameters['rettype'] = "uilist"
         parameters['retmode'] = "text"
-        result = download(parameters, esummaryaddress)
+        result = download(parameters, ESUMMARY_URL)
 
-        #comments
+        # comments
         if verb and verb > 1:
             print(countDown(x, nb, "Downloading TaxIDs"))
             
-        ###extract the TaxIDs and accession numbers (record in text file and in dict_ids)
+        ### extract the TaxIDs and accession numbers (record in text file and in dict_ids)
         f = result.text.splitlines()
         for line in f:
             if len(line.split('<DocSum>')) > 1:
                 taxid = ''
                 seqnb = ''
             else:
                 try:
@@ -163,17 +158,17 @@
                 if len(TaxId) > 1:
                     taxid = TaxId[1].split("<")[0].strip()
                 
                 if seqnb:
                     dict_ids[seqnb] = taxid 
 
     if fileoutput:
-        ##filename
+        ## filename
         filename = "TaxIDs.txt"
-        ##path to filename
+        ## path to filename
         path = path + "/" + filename
         with open(path, 'a') as summary:
             [summary.write(f'{key}  {value}\n') for key, value in dict_ids.items()]
 
     return dict_ids
 
 
@@ -182,66 +177,55 @@
         take the lineage of a sequence and the classification option and return the base name of the file to store 
         the sequence.
 
         INPUTS: dispatch(lineage, classif) 
             lineage: LIST
             classif: INT or LIST
     """
-    ###Phylums
-    Plantae = ['Chlorophyta', 'Charophyta', 'Bryophyta', 'Marchantiophyta', 'Lycopodiophyta', 'Ophioglossophyta', 'Pteridophyta',\
-    'Cycadophyta', 'Ginkgophyta', 'Gnetophyta', 'Pinophyta', 'Magnoliophyta', 'Equisetidae', 'Psilophyta', 'Bacillariophyta',\
-    'Cyanidiophyta', 'Glaucophyta', 'Prasinophyceae','Rhodophyta']
-    Fungi = ['Chytridiomycota', 'Zygomycota', 'Ascomycota', 'Basidiomycota', 'Glomeromycota']
-    Metazoa = ['Acanthocephala', 'Acoelomorpha', 'Annelida', 'Arthropoda', 'Brachiopoda', 'Ectoprocta', 'Bryozoa', 'Chaetognatha',\
-    'Chordata', 'Cnidaria', 'Ctenophora', 'Cycliophora', 'Echinodermata', 'Echiura', 'Entoprocta', 'Gastrotricha', 'Gnathostomulida',\
-    'Hemichordata', 'Kinorhyncha', 'Loricifera', 'Micrognathozoa', 'Mollusca', 'Nematoda', 'Nematomorpha', 'Nemertea', 'Onychophora'\
-    'Orthonectida', 'Phoronida', 'Placozoa', 'Plathelminthes', 'Porifera', 'Priapulida', 'Rhombozoa', 'Rotifera', 'Sipuncula',\
-    'Tardigrada', 'Xenoturbella']
-
-    ##no option selected
+    ## no option selected
     if classif == 2:
         return "sequences"
-    ##user gave list of taxonomic levels
+    ## user gave list of taxonomic levels (option -l --levels)
     if isinstance(classif, list):
         try:
             other = [rank for rank in lineage if rank in classif][0]
         except IndexError:
             other = "OTHERS"
         return other
-    ##phylums
+    ## phylums
     if classif == 0:
         try:
-            Phylum = [phy for phy in lineage if phy in Metazoa or phy in Fungi or phy in Plantae][0]
+            Phylum = [phy for phy in lineage if phy in METAZOA or phy in FUNGI or phy in PLANTAE][0]
         except IndexError:
             Phylum = 'OTHERS'
         return Phylum
-    ##kingdoms
+    ## kingdoms
     if classif == 1:
-        if 'Metazoa' in lineage or len(list(set(lineage) & set(Metazoa))) > 0:
+        if 'METAZOA' in lineage or len(list(set(lineage) & set(METAZOA))) > 0:
             kingdom = "METAZOA"
-        elif "Viridiplantae" in lineage or len(list(set(lineage) & set(Plantae))) > 0:
+        elif "ViridiPLANTAE" in lineage or len(list(set(lineage) & set(PLANTAE))) > 0:
             kingdom = "PLANTAE" 
-        elif "Fungi" in  lineage or len(list(set(lineage) & set(Fungi))) > 0:
+        elif "FUNGI" in  lineage or len(list(set(lineage) & set(FUNGI))) > 0:
             kingdom = "FUNGI" 
         else:
             kingdom = "OTHERS"
         return kingdom
-    ##if the users choose to make groupe n rank higher than species (classif >= 3)
+    ## if the users choose to make groupe n rank higher than species (classif >= 3)
     classif = -(int(classif) - 2)
     try:
         rank = lineage[classif]
     except IndexError:
         rank = "OTHERS"
     return rank
 
 
-#query taxonomy with efetch, returns a dict with taxid as key and info in a dict as value
+# query taxonomy with efetch, returns a dict with taxid as key and info in a dict as value
 def completetaxo(idlist, QUERY, OPTIONS):
 
-    ##unpack parameters
+    ## unpack parameters
     (_, api_key) = QUERY
     (verb, _, classif, _, _, _) = OPTIONS
 
     if verb and verb > 0:
         print("retrieving taxonomy...")
 
     ##dictionnary that will be returned
@@ -253,36 +237,35 @@
     count = len(idlist)
     if count % retmax == 0:                                    
         nb = count//retmax
     else: 
         nb = (count//retmax) + 1
 
     for x in range(nb):
-        ##slice the idlist
+        ## slice the idlist
         retstart = x * retmax
         idsublist = idlist[retstart:(retstart+retmax)]
         idsublist = ','.join(idsublist)
 
-        ##build API address
-        efetchaddress = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi"
+        ## build API address
         parameters = {}
         #parameters 
         parameters['db'] = "taxonomy"
         parameters['id'] = idsublist
         if api_key:
             parameters['api_key'] = api_key
 
-        ##loop until download is correct
-        result = download(parameters, efetchaddress)
+        ## loop until download is correct
+        result = download(parameters, EFETCH_URL)
 
-        #comments
+        # comments
         if verb > 1:
             print(f'{round((int(retstart)/count)*100, 1)} % of the taxonomy found')
 
-        ##analyse the results from efetch
+        ## analyse the results from efetch
         result = result.text.split('</Taxon>\n<Taxon>')
 
         for seq in result:
             dicttemp = {}
             try:
                 TaxId, _ = seq.split('</TaxId>', 1)
                 _, TaxId = TaxId.split('<TaxId>', 1)
@@ -305,23 +288,38 @@
                 Lineage , _ = seq.split('</Lineage>', 1)
                 _, Lineage = Lineage.split('<Lineage>', 1)    
             except ValueError:
                 Lineage = 'not found'
             lineage = Lineage.split('; ')
             dicttemp['Lineage'] = lineage
 
-            ##dispatch
+            ## dispatch
             dicttemp['dispatch'] = dispatch(lineage, classif)
 
             data[TaxId] = dicttemp
 
-    #comments
+    # comments
     if verb and verb > 0:
         print(f'number of taxids:\t{len(data.keys())}')
 
+    if verb and verb > 0:
+        dup = {}
+        duplicate = 0
+        for TaxId in data.keys():
+            if data[TaxId]['dispatch'] in dup.keys():
+                duplicate = duplicate + 1
+                dup[data[TaxId]['dispatch']] = dup[data[TaxId]['dispatch']] + [TaxId]
+            else: 
+                dup[data[TaxId]['dispatch']] = [TaxId]
+        print('--------------- DUPLICATES ---------------')
+        print(f'Number of taxa for which more than one TaxId has been found: {duplicate}')
+        for key in dup.keys():
+            if len(dup[key]) > 1:
+                print(f'{key}: {dup[key]}')
+        print('------------------------------------------')
     return data
 
 
 ## Download the CDS fasta files by batch of 'retmax' for the seq access found by an esearch request returning a querykey and a webenv variable
 def cds_fasta(path, dict_ids, dict_taxo, QUERY, list_of_ids, OPTIONS=None):
 
     if OPTIONS is None:
@@ -350,27 +348,25 @@
         nb = (count//retmax) + 1
 
     for x in range(nb):
         ## Split the list of ids
         ids = list_of_ids[x * retmax : (x * retmax) + retmax]
         ## Check that id parameters is not empty
         ids = [i for i in ids if i]
-        ## Build API address
-        efetchaddress = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi"
-        parameters = {}
         # Parameters 
+        parameters = {}
         parameters['id'] = ",".join(ids)
         parameters['db'] = "nuccore"
         if api_key:
             parameters["api_key"] = api_key
         parameters['rettype'] = "fasta_cds_na"
         parameters['retmode'] = "text"
 
         ## Download
-        raw_result = download(parameters, efetchaddress)
+        raw_result = download(parameters, EFETCH_URL)
         raw_result = raw_result.text
 
         ## Extract available information
         if not information and not genelist and classif == 3:
             result_fasta = raw_result.split(">lcl|")[1:]
             sublist = [r.split("_cds")[0] for r in result_fasta]
 
@@ -426,15 +422,15 @@
         Name = "no info"
 
     #dispatch
     try:
         dispatch = dict_taxo[TaxId]['dispatch']
     except KeyError:
         dispatch = "others"
-    if classif == 3:
+    if classif == 2:
         dispatch = "sequences"
 
     ##check if genes
     check = [1 for reg_exp in genelist if len(re.split(reg_exp, seq, flags=re.IGNORECASE)) > 1]
     if 1 in check or not genelist:
         ##get the Sequence
         _, dna = seq.split('\n', 1)
@@ -543,27 +539,25 @@
         nb = (count//retmax) + 1
 
     for x in range(nb):
         ## Split the list of ids
         ids = list_of_ids[x * retmax : (x * retmax) + retmax]
         ## Check that id parameters is not empty
         ids = [i for i in ids if i]
-        ## Build API address
-        efetchaddress = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi"
-        parameters = {}
         # Parameters 
+        parameters = {}
         parameters['db'] = "nuccore"
         parameters['id'] = ",".join(ids)
         if api_key:
             parameters["api_key"] = api_key
         parameters['rettype'] = "fasta"
         parameters['retmode'] = "text"
 
         ## Download
-        raw_result = download(parameters, efetchaddress)
+        raw_result = download(parameters, EFETCH_URL)
         raw_result = raw_result.text
 
         ## Extract available informations
         result = raw_result.split('>')
 
         ## Store analyzed Accession version numbers
         for seq in result:
@@ -596,15 +590,15 @@
                 name = 'not found'
             
             try:
                 dispatch = dict_taxo[taxid]['dispatch']
             except KeyError:
                 name = 'others'
             
-            if classif == 3:
+            if classif == 2:
                 dispatch = "sequences"
             
             data = (name, key, taxid, lineage, dna)
 
             # Create folders for .tsv files and .fasta files
             if tsv:
                 if not os.path.exists(path + "/fasta"):
@@ -689,28 +683,25 @@
         ##slice the list of ids passed to the function
         ids = list_of_ids[x * retmax:(x+1) * retmax]
         ##if some ids haven't been dl at the last call add them to this call
         if remain:
             ids = ids + remain
         ids1 = ",".join(ids)
         retstart = str(x * retmax)
-
-        ##build API address
-        efetchaddress = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi"
-        parameters = {}
         #parameters 
+        parameters = {}
         parameters['db'] = "nuccore"
         parameters['id'] = ids1
         parameters['rettype'] = "gb"
         parameters['retmode'] = "text"
         if api_key:
             parameters["api_key"] = api_key
         
         ##loop until dl is correct
-        result = download(parameters, efetchaddress)
+        result = download(parameters, EFETCH_URL)
         result = result.text
 
 
         ########################################################################
         #######################   ANALYZING RESULTS   ##########################
         ########################################################################
```

### Comparing `nsdpy-0.2.4/nsdpy.py` & `nsdpy-0.3.0b0/nsdpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,94 +1,103 @@
-__version__ = '0.2.4'
+__version__ = '0.3.0-beta'
 __author__ = "Raphael Hebert, Emese Meglecz"
 __email__ = "raphaelhebert18@gmail.com, emese.meglecz@imbe.fr"
 __license__ = "MIT"
 
-from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
 import sys
 import os
-import argparse             #parsing command line arguments
+import argparse                     #parsing command line arguments
 from datetime import datetime    
 
+# local imports
+from constants import ESEARCH_URL
+from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
+
 
 def main():
 ############################################
 ###### CHECK COMMAND LINE ARGUMENTS ########
 ############################################
 
     parser = argparse.ArgumentParser()
 
-    ##VERSION
+    ## VERSION
     parser.add_argument('-V', '--version', action='version', version=__version__)
 
-    ##POSITIONAL ARGUMENTS
+    ## POSITIONAL ARGUMENTS
     parser.add_argument("-r", "--request", required=True, help="The request to the NCBI database")
 
-    ##OPTIONAL ARGUMENTS
-    #api key
+    ## OPTIONAL ARGUMENTS
+    # api key
     parser.add_argument("-a", "--apikey", default=None, help="API key (register to NCBI to get an API key)")
-    #verbose
+    # verbose
     group = parser.add_mutually_exclusive_group()
     group.add_argument("-v", "--verbose", help="Diplays downloads progress and actions", action="store_true")
     group.add_argument("-q", "--quiet", help="No verbose output", action="store_true")
-    #gene selection
-    parser.add_argument("-c", "--cds", help="search for a given list of gene, exp: COX1 COX2 COX3, accepts regex", nargs="*")
-    #file input
+    # Sequence types
+    group2 = parser.add_mutually_exclusive_group()
+    # Gene selection
+    group2.add_argument("-c", "--cds", help="search for a given list of gene, exp: COX1 COX2 COX3, accepts regex", nargs="*")
+    # Gene Features format
+    group2.add_argument("-g", "--gene", help="download sequences in gene feature format // NOT FUNCTIONAL YET", nargs="*")
+    # file input
     parser.add_argument("-L", "--list", help='input one or more .txt file as an external list of taxa: path/to/file.txt', nargs="*")
-    #file output
+    # file output
     parser.add_argument("-T", "--taxids", help='write a text file listing all the accession numbers and their related TaxIDs', action="store_true")
     parser.add_argument("-t", "--tsv", default=None, help="create a tsv file based on fasta file output", action="store_true")
-    #Taxonomy
+    # Taxonomy
     group3 = parser.add_mutually_exclusive_group()
     group3.add_argument("-k", "--kingdom", help="output four different text files file: Plantae and Fungi, Metazoa and  Others", action="store_true" )
     group3.add_argument("-p", "--phylum", help="output one file text per phylum", action="store_true" )
     group3.add_argument("-l", "--levels", help="find only the taxon given by user", nargs="+")
     group3.add_argument("-s", "--species",\
         help="classify the results in different text file one for each (specie + n) level found, exp: -s correspond to lowest levels, -ss 2nd lowest, -sssss 5th lowest and so on",\
         action="count", default=2)
 
-    #information line
+    # information line
     parser.add_argument("-i", "--information", help="just add the taxonomic information in the information line of the output file(s)", action="store_true" )
 
     args = parser.parse_args()
 
     #################################################
     #############   GLOBAL VARIABLES    #############
     #################################################
 
     # list the selected option to make it appear in report.txt
     options_report = []
 
-    #taxa list
+    # taxa list
     if args.list:
         input_files = ' '.join(args.list)
         options_report.append(f" -list (-L) {input_files}")
         # Check that a file is provided
         if len(args.list) == 0:
             sys.exit("The --list (-L) requires at list one .txt file")
 
         # Check if files exists
         for file in args.list:
             if not os.path.exists(file):
                 sys.exit(f"The file {file} cannot be found")
             if file[-4:] != ".txt":
-                sys.exit(f"The list of taxa {file} must be a .txt file")
+                sys.exit(f"The list of taxa {file} must be a file with a .txt extension")
 
-    #list of chosen options to display in the report.tsv
-    ##parse options
+    # list of chosen options to display in the report.tsv
+    ## parse options
     if args.tsv:
         options_report.append("--tsv (-t)")
     if args.information:
         options_report.append("--information (-i)")
     if args.taxids:
         options_report.append("--taxids (-T)")
     if args.cds is not None:
         options_report.append(f"--cds (-c) {' '.join(args.cds)}")
     if args.apikey:
         options_report.append(f"--apikey (-a) {args.apikey[0]}")
+    if args.gene:
+        options_report.append(f"--gene (-g) {' '.join(args.gene)}")
 
     #verbose
     if args.verbose:
         verb = 2
         options_report.append("--verbose (-v)")
     elif args.quiet:
         verb = 0
@@ -100,19 +109,20 @@
     if args.kingdom:
         classif = 1
         options_report.append("--kingdom (-k)")
     elif args.phylum:
         classif = 0
         options_report.append("--phylum (-p)")
     elif args.levels:
+        # here isinstance(classif, list) == true
         classif = args.levels
         options_report.append(f"--levels (-l) {args.levels[0]}")
     elif args.species:
         classif = args.species
-        if args.species > 2:
+        if args.species != 2:
             options_report.append("--species (-" + "s" * ( args.species - 2 ) + ")")
     else:
         classif = 2
 
     OPTIONS = (verb, args.cds, classif, args.taxids, args.tsv, args.information)
 
     ##foldername and path
@@ -137,15 +147,15 @@
             with open(file, "r") as data:
                 taxa_list = taxa_list + data.read().splitlines()
         
         # Add the taxa to the query
         taxa_list = [ taxon + "[ORGN] OR " for taxon in taxa_list]
 
         # Base URL with params
-        esearch_address = 'https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi'
+        esearch_address = ESEARCH_URL
         base_URL_length = len(esearch_address) + 100 # Keep 100 chars for params
 
         # Base query
         base_query = args.request + " AND ("
         
         # Remaining space for the taxa list 
         taxa_max_length = 2048 - ( len(base_query) + base_URL_length )
@@ -183,58 +193,57 @@
         QUERY = (query, args.apikey)
         if verb != 0:
             print(f"retrieving results for {query} ....")        
 
         ## esearchquery
         y = esearchquery(QUERY)
 
-        ##check errors (if bad API key etc) errors returned by the Entrez API
+        ## check errors (if bad API key etc) errors returned by the Entrez API
         if "error" in y.keys():
             errors = y["error"]
             sys.exit(errors)
 
         count = int(y["esearchresult"]["count"])
-        #comments
+        # comments
         if verb > 0:    
             print(f'Number of results found: {count}')
 
         if count < 1:
             continue
         webenv =  str(y["esearchresult"]["webenv"])
         querykey = str(y["esearchresult"]["querykey"])
         params = (querykey, webenv, count)
 
-        ###Taxids
+        ### Taxids
         if verb != 0:
             print("retreiving the corresponding TaxIDs...")
    
         subdictids = taxids(params, path, OPTIONS)
         dict_ids = {**dict_ids, **subdictids}
 
         total_number_of_results = len(set(dict_ids.keys()))
 
     if total_number_of_results < 1: 
         sys.exit("No results found")
 
     if verb != 0:
         print(f"Total number of results: {total_number_of_results}")
 
-    #make a set of TaxIDs
+    # make a set of TaxIDs
     list_of_ids = list(dict_ids.keys())
     reverse = set(dict_ids.values())
     list_of_TaxIDs = list(reverse)
 
 
     ### completetaxo (call EFETCH to query the taxonomy database)
     # Check that an option that requires the taxonomic information has been selected
     dict_taxo = {}
-    if classif != 3 or args.information:
+    if classif != 2 or args.information:
         dict_taxo = completetaxo(list_of_TaxIDs, QUERY, OPTIONS)
 
-
     ### Download the sequences (call to EFETCH to query the nuccore database)
     if args.cds is None:
         found = fasta(path, dict_ids, dict_taxo, QUERY, list_of_ids, OPTIONS)
     else:
         found = cds_fasta(path, dict_ids, dict_taxo, QUERY, list_of_ids, OPTIONS)
 
     ### List the remaining access ids:
@@ -246,15 +255,15 @@
         print(f'number of remaining accession numbers with sequence to be found in GenBank files: {len(remaining)}')
 
 
     ### taxo (call EFETCH to query the nuccore database to get the .gb files) 
     analyse, sequences = taxo(path, remaining, dict_ids, QUERY, dict_taxo, OPTIONS)
 
 
-    ### summarise
+    ### Summurize
     # Get the ending time of the run
     ending_time= str(datetime.now())
     ending_time= '_'.join(ending_time.split())[:19]
     ending_time= ending_time.replace(":", "-")        
 
     ### Comments
     genes = found + sequences
@@ -280,15 +289,15 @@
             print(f'number with more than one sequences:                                {duplicates(genes, path)}')
             print(f'total number of accession version identifiers analysed:             {len(total)}')
             print(f'ended:                                                              {ending_time}')
             print(f'number of accession version identifiers analysed with no sequences downloaded:             {len(notfound)}')
             if len(notfound) > 0:
                 print(f'see "notfound.txt"')
 
-    ##write summary
+    ## Write summary
     if args.cds is None:
         filters = ""
         filetype = "fasta"
     else:
         filters = ",".join(args.cds)
         filetype = "cds_fasta"
```

### Comparing `nsdpy-0.2.4/pyproject.toml` & `nsdpy-0.3.0b0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdpy"
-version = "0.2.4"
+version = "0.3.0-beta"
 description = "Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)"
 authors = ["RaphaelHebert <raphaelhebert18@gmail.com>", "Emese Meglecz <emese.meglecz@imbe.fr>"]
 include = ["functions.py"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RaphaelHebert/nsdpy"
 homepage = "https://github.com/RaphaelHebert/nsdpy"
```

### Comparing `nsdpy-0.2.4/PKG-INFO` & `nsdpy-0.3.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdpy
-Version: 0.2.4
+Version: 0.3.0b0
 Summary: Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)
 Home-page: https://github.com/RaphaelHebert/nsdpy
 License: MIT
 Keywords: NCBI,Taxonomy,DNA
 Author: RaphaelHebert
 Author-email: raphaelhebert18@gmail.com
 Requires-Python: >=3.8,<4.0
```

