# Comparing `tmp/genbank-0.81.tar.gz` & `tmp/genbank-0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genbank-0.81.tar", last modified: Fri May 12 23:04:20 2023, max compression
+gzip compressed data, was "genbank-0.96.tar", last modified: Sat Jun  3 00:42:27 2023, max compression
```

## Comparing `genbank-0.81.tar` & `genbank-0.96.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-05-12 23:04:20.889831 genbank-0.81/
--rw-r--r--   0 katelyn    (501) staff       (20)    35149 2022-02-15 23:16:16.000000 genbank-0.81/LICENSE
--rw-r--r--   0 katelyn    (501) staff       (20)       51 2022-12-13 21:12:02.000000 genbank-0.81/MANIFEST.in
--rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-05-12 23:04:20.889557 genbank-0.81/PKG-INFO
--rw-r--r--   0 katelyn    (501) staff       (20)     2744 2022-12-13 21:12:02.000000 genbank-0.81/README.md
--rw-r--r--   0 katelyn    (501) staff       (20)        5 2023-05-12 22:17:30.000000 genbank-0.81/VERSION
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-05-12 23:04:20.886922 genbank-0.81/genbank/
--rw-r--r--   0 katelyn    (501) staff       (20)        0 2022-02-15 23:20:41.000000 genbank-0.81/genbank/__init__.py
--rw-r--r--   0 katelyn    (501) staff       (20)     3235 2022-03-01 21:08:53.000000 genbank-0.81/genbank/codons.py
--rw-r--r--   0 katelyn    (501) staff       (20)     6086 2023-05-12 22:39:31.000000 genbank-0.81/genbank/feature.py
--rw-r--r--   0 katelyn    (501) staff       (20)     2918 2023-02-07 21:33:49.000000 genbank-0.81/genbank/file.py
--rw-r--r--   0 katelyn    (501) staff       (20)    13299 2023-05-12 22:26:53.000000 genbank-0.81/genbank/locus.py
--rw-r--r--   0 katelyn    (501) staff       (20)      371 2023-04-11 20:58:21.000000 genbank-0.81/genbank/sequence.py
--rw-r--r--   0 katelyn    (501) staff       (20)     2726 2022-03-08 22:07:42.000000 genbank-0.81/genbank/translate.py
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-05-12 23:04:20.888557 genbank-0.81/genbank.egg-info/
--rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-05-12 23:04:20.000000 genbank-0.81/genbank.egg-info/PKG-INFO
--rw-r--r--   0 katelyn    (501) staff       (20)      330 2023-05-12 23:04:20.000000 genbank-0.81/genbank.egg-info/SOURCES.txt
--rw-r--r--   0 katelyn    (501) staff       (20)        1 2023-05-12 23:04:20.000000 genbank-0.81/genbank.egg-info/dependency_links.txt
--rw-r--r--   0 katelyn    (501) staff       (20)        8 2023-05-12 23:04:20.000000 genbank-0.81/genbank.egg-info/top_level.txt
--rw-r--r--   0 katelyn    (501) staff       (20)     8793 2023-05-05 23:42:46.000000 genbank-0.81/genbank.py
--rw-r--r--   0 katelyn    (501) staff       (20)       38 2023-05-12 23:04:20.889903 genbank-0.81/setup.cfg
--rw-r--r--   0 katelyn    (501) staff       (20)     1397 2023-04-12 22:59:11.000000 genbank-0.81/setup.py
-drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-05-12 23:04:20.888842 genbank-0.81/tests/
--rw-r--r--   0 katelyn    (501) staff       (20)      126 2022-04-07 22:19:14.000000 genbank-0.81/tests/small.fasta
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-03 00:42:27.243462 genbank-0.96/
+-rw-r--r--   0 katelyn    (501) staff       (20)    35149 2022-02-15 23:16:16.000000 genbank-0.96/LICENSE
+-rw-r--r--   0 katelyn    (501) staff       (20)       51 2022-12-13 21:12:02.000000 genbank-0.96/MANIFEST.in
+-rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-06-03 00:42:27.243164 genbank-0.96/PKG-INFO
+-rw-r--r--   0 katelyn    (501) staff       (20)     2744 2022-12-13 21:12:02.000000 genbank-0.96/README.md
+-rw-r--r--   0 katelyn    (501) staff       (20)        5 2023-06-02 21:37:41.000000 genbank-0.96/VERSION
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-03 00:42:27.239805 genbank-0.96/genbank/
+-rw-r--r--   0 katelyn    (501) staff       (20)        0 2022-02-15 23:20:41.000000 genbank-0.96/genbank/__init__.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     3235 2022-03-01 21:08:53.000000 genbank-0.96/genbank/codons.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     7231 2023-05-31 21:20:09.000000 genbank-0.96/genbank/feature.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     2963 2023-05-30 19:17:51.000000 genbank-0.96/genbank/file.py
+-rw-r--r--   0 katelyn    (501) staff       (20)    13397 2023-05-31 21:54:27.000000 genbank-0.96/genbank/locus.py
+-rw-r--r--   0 katelyn    (501) staff       (20)      491 2023-05-17 21:07:28.000000 genbank-0.96/genbank/sequence.py
+-rw-r--r--   0 katelyn    (501) staff       (20)     2724 2023-05-26 01:58:53.000000 genbank-0.96/genbank/translate.py
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-03 00:42:27.241502 genbank-0.96/genbank.egg-info/
+-rw-r--r--   0 katelyn    (501) staff       (20)     3209 2023-06-03 00:42:27.000000 genbank-0.96/genbank.egg-info/PKG-INFO
+-rw-r--r--   0 katelyn    (501) staff       (20)      330 2023-06-03 00:42:27.000000 genbank-0.96/genbank.egg-info/SOURCES.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)        1 2023-06-03 00:42:27.000000 genbank-0.96/genbank.egg-info/dependency_links.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)        8 2023-06-03 00:42:27.000000 genbank-0.96/genbank.egg-info/top_level.txt
+-rw-r--r--   0 katelyn    (501) staff       (20)     8678 2023-06-03 00:42:16.000000 genbank-0.96/genbank.py
+-rw-r--r--   0 katelyn    (501) staff       (20)       38 2023-06-03 00:42:27.243547 genbank-0.96/setup.cfg
+-rw-r--r--   0 katelyn    (501) staff       (20)     1397 2023-04-12 22:59:11.000000 genbank-0.96/setup.py
+drwxr-xr-x   0 katelyn    (501) staff       (20)        0 2023-06-03 00:42:27.241812 genbank-0.96/tests/
+-rw-r--r--   0 katelyn    (501) staff       (20)      126 2022-04-07 22:19:14.000000 genbank-0.96/tests/small.fasta
```

### Comparing `genbank-0.81/LICENSE` & `genbank-0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `genbank-0.81/PKG-INFO` & `genbank-0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genbank
-Version: 0.81
+Version: 0.96
 Summary: Code to work with Genbank files
 Home-page: https://github.com/deprekate/genbank
 Author: Katelyn McNair
 Author-email: deprekate@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `genbank-0.81/README.md` & `genbank-0.96/README.md`

 * *Files identical despite different names*

### Comparing `genbank-0.81/genbank/codons.py` & `genbank-0.96/genbank/codons.py`

 * *Files identical despite different names*

### Comparing `genbank-0.81/genbank/feature.py` & `genbank-0.96/genbank/feature.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,44 +46,80 @@
 	def right(self):
 		# convert genbank 1-based indexing to standard 0-based
 		return nint(self.pairs[-1][-1]) - 3
 	
 	def length(self):
 		return len(self.seq())
 
+	'''
 	def seq(self):
 		seq = list()
 		for pair in self.pairs:
 			left,right = map(nint, pair)
 			seq.append(self.locus.seq(left-1,right, self.strand))
 		if self.strand > 0:
 			return ''.join(seq)
 		else:
 			return ''.join(seq[::-1])
+	'''
 
-	def codons(self):
+	def seq(self):
+		# lol this is chatgpts more optimized version
+		seq = [self.locus.seq(nint(pair[0]) - 1, nint(pair[-1]), self.strand) for pair in self.pairs]
+		return ''.join(seq) if self.strand > 0 else ''.join(seq[::-1])
+
+	'''
+	def loc(self):
+		loc = list()
+		for pair in self.pairs:
+			left,right = map(nint, pair)
+			loc.extend(list(range(left-1,right)))
+		return loc
+	'''
+	def loc(self):
+		# lol this is chatgpts more optimized version
+		return [val for pair in self.pairs for val in range(nint(pair[0])-1, nint(pair[-1]))]
+	
+	def codons(self, loc=False):
 		assert self.type == 'CDS'
 		dna = self.seq()
 		# should I return partial codons?
-		if self.partial() == 'left':
-			remainder = len(dna) % 3
-			if self.strand > 0:
-				dna = dna[remainder:]
-			else:
-				dna = dna[:-remainder]
-		if self.partial() == 'right':
-			remainder = len(dna) % 3
-			if self.strand > 0:
-				dna = dna[:-remainder]
-			else:
-				dna = dna[remainder:]
+		partial_type = self.partial()
+		remainder = len(dna) % 3
+		if partial_type == 'left':
+			dna = dna[remainder:] if self.strand > 0 else dna[:-remainder]
+		elif partial_type == 'right':
+			dna = dna[:-remainder] if self.strand > 0 else dna[remainder:]
+		if len(dna) % 3:
+			# not sure how to handle bad features
+			dna = ''
 		for triplet in grouper(dna, 3):
 			yield ''.join(triplet)
 		return
 
+	def codon_locations(self):
+		assert self.type == 'CDS'
+		loc = self.loc()
+		if self.strand < 0:
+			loc.reverse()
+		# should I return partial codons?
+		partial_type = self.partial()
+		remainder = len(loc) % 3
+		if partial_type == 'left':
+			loc = loc[remainder:] if self.strand > 0 else loc[:-remainder]
+		elif partial_type == 'right':
+			loc = loc[:-remainder] if self.strand > 0 else loc[remainder:]
+		if len(loc) % 3:
+			# not sure how to handle bad features
+			loc = []
+		for locs in grouper(loc, 3):
+			yield locs
+		return
+
+
 	def fna(self):
 		return self.header() + self.seq() + "\n"
 
 	def faa(self):
 		return self.header() + self.translation() + "\n"
 	
 	def header(self):
@@ -94,15 +130,15 @@
 					if value:
 						header += " [" + tag + "=" + value +"]"
 					else:
 						header += " [" + tag +"]"
 		return header + "\n"
 
 	def hypothetical(self):
-		function = self.tags['product'] if 'product' in self.tags else ''
+		function = ''.join(self.tags['product']).lower() if 'product' in self.tags else ''
 		if 'hypot'  in function or \
 		   'etical' in function or \
 		   'unchar' in function or \
 		   ('orf' in function and 'orfb' not in function):
 			return True
 		else:
 			return False
@@ -127,22 +163,23 @@
 			return False
 
 	def is_joined(self):
 		if len(self.pairs) > 1:
 			return True
 		return False
 
+	'''
 	def __iter__(self):
 		for left,*right in self.pairs:
 			if right:
 				right = right[0]
 			else:
 				right = left
 			yield nint(left)-1 , nint(right)-1
-
+	'''
 	def __str__(self):
 		"""Compute the string representation of the feature."""
 		return "%s\t%s\t%s\t%s" % (
 				repr(self.locus.name()),
 				repr(self.type),
 				repr(self.pairs),
 				repr(self.tags))
```

### Comparing `genbank-0.81/genbank/file.py` & `genbank-0.96/genbank/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,47 +15,45 @@
 		
 		lib = gzip if filename.endswith(".gz") else io
 		with lib.open(filename, mode="rb") as fp:
 			for line in chain(fp, [b'>']):
 				# FASTA
 				if line.startswith(b'>') and temp.tell() > 1:
 					locus = self.parse_locus(temp)
-					self[locus.name()] = locus
+					self[locus] = True
 				temp.write(line)
 				# GENBANK
 				if line.startswith(b'//'):
 					locus = self.parse_locus(temp)
-					self[locus.name()] = locus
+					self[locus] = True 
 		temp.close()
 	
 	def __init_subclass__(cls, locus, **kwargs):
 		'''this method allows for a Locus class to be modified through inheritance in other code '''
 		super().__init_subclass__(**kwargs)
 		cls.locus = locus
 
+	'''
 	def __iter__(self):
 		# hopefully this doesnt break stuff
 		return iter(self.values())
+	'''
 
 	def features(self, include=None, exclude=None):
 		for locus in self.values():
 			for feature in locus.features(include=include):
 				yield feature
 	
 	def dna(self):
-		dna = ""
-		for locus in self.values():
-			dna += locus.dna
-		return dna
+		dna = [locus.dna for locus in self.values()]
+		return "".join(dna)
 
 	def parse_locus(self, fp):
 		locus = self.locus()
-		current = None
-		field = None
-		fasta = False
+		current = fasta = False
 		dna = []	
 		fp.seek(0)
 		for line in fp:
 			line = line.decode("utf-8")
 			if line.startswith('\n'):
 				pass
 			elif not line.startswith(' '):
@@ -65,18 +63,19 @@
 					locus.groups['LOCUS'] = [group[1:]]
 					fasta = True
 				elif fasta:
 					dna.append( line.rstrip().replace(' ','').lower() )
 				elif line.startswith('//'):
 					break
 				else:
-					if group in locus.groups and locus.groups[group][-1]:
-						locus.groups[group].append(''.join(map(str,value)))
-					else:
-						locus.groups[group] = [''.join(map(str,value))]
+					locus.groups.setdefault(group, []).append(''.join(map(str, value)))
+					#if group in locus.groups and locus.groups[group][-1]:
+					#	locus.groups[group].append(''.join(map(str,value)))
+					#else:
+					#	locus.groups[group] = [''.join(map(str,value))]
 			elif group == 'ORIGIN':
 				#locus.dna += line.split(maxsplit=1)[1].rstrip().replace(' ','').lower()
 				dna.append( line.split(maxsplit=1)[1].rstrip().replace(' ','').lower() )
 			elif group == 'FEATURES':
 				line = line.rstrip()
 				if not line.startswith(' ' * 21):
 					while line.endswith(','):
```

### Comparing `genbank-0.81/genbank/locus.py` & `genbank-0.96/genbank/locus.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,35 +39,38 @@
 			self.feature = Feature
 		#self.name = name
 		self.dna = dna.lower()
 		#self.codons = dict()
 		self.translate = Translate()
 		self.strand = 1
 		self.groups = dict()
-		self.groups['LOCUS'] = [name.replace(' ','')]
+		self.groups['LOCUS'] = [name.replace(' ','')] if name else []
 		#self.groups['FEATURES'] = ['']
 		#self.groups['ORIGIN'] = ['']
+		
+	def __eq__(self, other):
+		return (self == other)
+
+	def __hash__(self):
+		return id(self)
 
 	def __init_subclass__(cls, feature=Feature, **kwargs):
 		'''this method allows for a Feature class to be modified through inheritance in other code '''
 		super().__init_subclass__(**kwargs)
 		cls.feature = feature
 
 	def name(self):
-		#return self.groups['LOCUS'][0].split()[0]
 		return self.groups['LOCUS'][0].split(' ')[0]
 
 	def molecule(self):
 		if len(locus) > 2:
 			return locus[3]
 		else:
 			return 'DNA'
 
-		
-
 	def fasta(self):
 		return ">" + self.name() + "\n" + self.seq() + "\n"
 
 	def seq(self, left=0, right=None, strand=None):
 		# this should always refer to zero based indexing
 		#if strand is None:
 		#	strand = self.strand
@@ -425,25 +428,23 @@
 			return self.rarity
 
 	def slice(self, left, right):
 		if left > right:
 			left,right = right+1,left+1
 			self.strand = -1
 		self.dna = self.seq(left,right)
-		for feature in list(self.keys()):
-			if feature.right() - 1 < left:
-				del self[feature]
-			elif feature.left() > right:
-				del self[feature]
+		to_delete = list()
+		for feature in self.keys():
+			if feature.right() - 1 < left or feature.left() > right:
+				to_delete.append(feature)
 			else:
 				# whew there is a lot going on here
 				f0 = lambda x : int(x.replace('<','').replace('>',''))
 				f1 = lambda x : '<1' if f0(x) - left < 1 else ('>'+str(self.length()) if f0(x) - left > self.length() else f0(x) - left)
 				f2 = lambda x : str(f1(x))
 				feature.pairs = rmap(f2, feature.pairs)
+		for feature in to_delete:
+			del self[feature]
 		return self
-		
-
 
 
-
```

### Comparing `genbank-0.81/genbank/translate.py` & `genbank-0.96/genbank/translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 					   }
 
 	def rev_comp(self, seq):
 		seq_dict = {'a':'t','t':'a','g':'c','c':'g',
 					'n':'n',
 					'r':'y','y':'r','s':'s','w':'w','k':'m','m':'k',
 					'b':'v','v':'b','d':'h','h':'d'}
-		return "".join([seq_dict[base] for base in reversed(seq)])
+		return "".join(seq_dict[base] for base in reversed(seq))
 
 	def codon(self, codon):
 		if len(codon) == 3:
 			return self.translate.get(codon.lower(), 'X')
 		else:
 			return ''
```

### Comparing `genbank-0.81/genbank.egg-info/PKG-INFO` & `genbank-0.96/genbank.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genbank
-Version: 0.81
+Version: 0.96
 Summary: Code to work with Genbank files
 Home-page: https://github.com/deprekate/genbank
 Author: Katelyn McNair
 Author-email: deprekate@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `genbank-0.81/genbank.py` & `genbank-0.96/genbank.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import io
 import sys
 import gzip
 import re
 import argparse
 import tempfile
 from collections import Counter
-from argparse import RawTextHelpFormatter
 from itertools import zip_longest, chain
 import shutil
 import tempfile
 import urllib.request
 import fileinput
 
 sys.path.pop(0)
@@ -35,15 +34,15 @@
         self.write(item)
     else:
         self.write(str(item))
 
 if __name__ == "__main__":
 	choices = 	['tabular','genbank','fasta', 'fna','faa', 'coverage','rarity','bases','gc','gcfp', 'taxonomy','part', 'gff', 'gff3', 'testcode']
 	usage = '%s [-opt1, [-opt2, ...]] infile' % __file__
-	parser = argparse.ArgumentParser(description='', formatter_class=RawTextHelpFormatter, usage=usage)
+	parser = argparse.ArgumentParser(description='', formatter_class=argparse.RawTextHelpFormatter, usage=usage)
 	parser.add_argument('infile', type=is_valid_file, help='input file in genbank format')
 	parser.add_argument('-o', '--outfile', action="store", default=sys.stdout, type=argparse.FileType('w'), help='where to write output [stdout]')
 	parser.add_argument('-f', '--format', help='Output the features in the specified format', type=str, default='genbank', choices=choices)
 	parser.add_argument('-s', '--slice', help='This slices the infile at the specified coordinates. \nThe range can be in one of three different formats:\n    -s 0-99      (zero based string indexing)\n    -s 1..100    (one based GenBank indexing)\n    -s 50:+10    (an index and size of slice)', type=str, default=None)
 	parser.add_argument('-g', '--get', action="store_true")
 	parser.add_argument('-r', '--revcomp', action="store_true")
 	parser.add_argument('-a', '--add', help='This adds features the shell input via < features.txt', type=str, default=None)
@@ -64,50 +63,40 @@
 			with tempfile.NamedTemporaryFile() as tmp:
 				shutil.copyfileobj(response, tmp)
 				genbank = File(tmp.name)
 		
 	if args.compare:
 		perfect = partial = total = 0
 		compare = File(args.compare)
-		for (name,locus),( _ ,other) in zip(genbank.items(),compare.items()):
+		for locus,other in zip(genbank,compare):
 			pairs = dict()
 			for feature in locus.features(include='CDS'):
 				if feature.strand > 0:
 					pairs[feature.pairs[-1][-1]] = feature.pairs[ 0][ 0]
 				else:
 					pairs[feature.pairs[ 0][ 0]] = feature.pairs[-1][-1]
 			total += len(pairs)
 			for feature in other.features(include='CDS'):
 				if feature.strand > 0:
 					if feature.pairs[-1][-1] in pairs:
 						partial += 1
 						if feature.pairs[ 0][ 0] == pairs[feature.pairs[-1][-1]]:
 							perfect += 1
+						del pairs[feature.pairs[-1][-1]]
 				else:
 					if feature.pairs[ 0][ 0] in pairs:
 						partial += 1
 						if feature.pairs[-1][-1] == pairs[feature.pairs[ 0][ 0]]:
 							perfect += 1
-		args.outfile.print(partial)
-		args.outfile.print('\t')
-		args.outfile.print('(')
-		args.outfile.print(partial/total)
-		args.outfile.print(')')
-		args.outfile.print('\t')
-		args.outfile.print(perfect)
-		args.outfile.print('\t')
-		args.outfile.print('(')
-		args.outfile.print(perfect/total)
-		args.outfile.print(')')
-		args.outfile.print('\t')
-		args.outfile.print(total)
-		args.outfile.print('\n')
+						del pairs[feature.pairs[ 0][ 0]]
+		args.outfile.write(f"{partial}\t({partial/total})\t{perfect}\t({perfect/total})\t{total}\n")
 		exit()
 	if args.add:
 		# this only works for single sequence files
+		stdin = []
 		if not sys.stdin.isatty():
 			stdin = sys.stdin.readlines()
 		for locus in genbank:
 			for line in stdin:
 				if args.add == 'genbank':
 					pass
 				elif args.add == 'genemark':
@@ -115,124 +104,131 @@
 						key = 'CDS'
 						n,strand,left,right,*_ = line.split()
 						locus.add_feature(key,strand,[[left,right]],{'note':['genemarkS']})
 				elif args.add == 'glimmer':
 					if not line.startswith('>'):
 						key = 'CDS'
 						n,left,right,(strand,*_),*_ = line.split()
-						locus.add_feature(key,strand,[[left,right]],{'note':['glimmer3']})
+						if strand == '-':
+							left, right = right, left
+							pairs = [[left, right]] if int(left) > int(right) else [[left, str(locus.length())], ['1', right]]
+						else:
+							pairs = [[left, right]] if int(left) > int(right) else [[left, right]]
+						locus.add_feature(key,strand,pairs,{'note':['glimmer3']})
 				elif args.add == 'gff':
 					if not line.startswith('#'):
 						name,other,key,left,right,_,strand,_,tags = line.rstrip('\n').split('\t')
-						tags = dict((key,value) for tag in tags.split(';') for key,*value in [tag.split('=')])
+						tags = {key:val for tag in tags.split(';') for key,*val in [tag.split('=')]}
 						locus.add_feature(key,strand,[[left,right]],tags)
 	elif args.edit:
 		if not sys.stdin.isatty():
 			stdin = sys.stdin.readlines()
 			#sys.stdin = open('/dev/tty')
 		key,qualifier = args.edit.replace('/',':').split(':')
 		for feature,values in zip(genbank.features(include=[key]), stdin):
 			feature.tags[qualifier] = list()
 			for value in values.rstrip().split('\t'):
 				feature.tags[qualifier].append(value)
 	if args.slice:
 		if '..' in args.slice:
 			left,right = map(int, args.slice.split('..'))
-			left = left - 1
+			left -= 1
 		elif ':' in args.slice:
 			left,right = args.slice.split(':')
 			if '+' in right and '-' in right:
 				left = eval(left + right)
 				right = eval(left + right)
 			elif '+' in right:
 				right = eval(left + right)
 			elif '-' in right:
 				left,right = eval(left + right) , left
 			left,right = map(int, [left,right])
 		elif '-' in args.slice:
 			left,right = map(int, args.slice.split('-'))
-			right = right + 1
+			right += 1
 		else:
 			raise Exception("re-circularization not implemented yet")
 			left = int(args.slice)
 			right = left+1
-		for name,locus in genbank.items():
+		for locus in genbank:
 			locus = locus.slice(left,right)
 	if args.key:
 		key,qualifier = args.key.replace('/',':').split(':')
 		for feature in genbank.features(include=key):
 			args.outfile.print('\t'.join(feature.tags[qualifier]))
 			args.outfile.print("\n")
 	elif args.format == 'genbank':
+		if args.revcomp:
+			raise Exception("not implemented yet")
 		genbank.write(args.outfile)	
 	elif args.format == 'tabular':
 		for feature in genbank.features(include=['CDS']):
 			args.outfile.print(feature)
 			args.outfile.print("\t")
 			args.outfile.print(feature.seq())
 			args.outfile.print("\n")
 	elif args.format in ['gff', 'gff3']:
 		for locus in genbank:
 			locus.write(args.outfile, args)
 	elif args.format in ['fna','faa']:
-		for name,locus in genbank.items():
+		for locus in genbank:
 			for feature in locus.features(include=['CDS']):
 				args.outfile.print( getattr(feature, args.format)() )
 	elif args.format in ['fasta']:
-		for name,locus in genbank.items():
+		for locus in genbank:
 			if args.revcomp:
 				locus.dna = locus.seq(strand=-1)
 			args.outfile.print( getattr(locus, args.format)() )
 	elif args.format == 'coverage':
 		cbases = tbases = 0
-		for name,locus in genbank.items():
+		for locus in genbank:
 			c,t = locus.gene_coverage()
 			cbases += c
 			tbases += t
 		#args.outfile.print( name )
 		#args.outfile.print( '\t' )
 		args.outfile.print( cbases / tbases )
 		args.outfile.print( '\n' )
 	elif args.format == 'rarity':
 		rarity = dict()
-		for name,locus in genbank.items():
+		for locus in genbank:
 			for codon,freq in sorted(locus.codon_rarity().items(), key=lambda item: item[1]):
 				args.outfile.print(codon)
 				args.outfile.print('\t')
 				args.outfile.print(round(freq,5))
 				args.outfile.print('\n')
 	elif args.format == 'bases':
 		strand = -1 if args.revcomp else +1
-		for name,locus in genbank.items():
+		for locus in genbank:
 			args.outfile.print(locus.seq(strand=strand))
 			args.outfile.print('\n')
 	elif args.format in ['gc','gcfp']:
-		for name,locus in genbank.items():
+		for locus in genbank:
 			args.outfile.print(locus.name())
 			args.outfile.print('\t')
 			if args.format == 'gc':
 				args.outfile.print(locus.gc_content())
 			else:
 				args.outfile.print(locus.gc_fp())
 			args.outfile.print('\n')
 	elif args.format == 'taxonomy':
-		for name,locus in genbank.items():
+		for locus in genbank:
 			args.outfile.print(locus.groups['SOURCE'][0].replace('\n','\t').replace('            ','').replace(';\t','; ') )
 			args.outfile.print('\n')
 	elif args.format in ['part']:
 		folder = args.outfile.name if args.outfile.name != '<stdout>' else ''
-		for name,locus in genbank.items():
+		for locus in genbank:
 			with open(os.path.join(folder,name + '.fna'), 'w') as f:
 				f.write('>')
-				f.write(name)
+				f.write(locus.name())
 				f.write('\n')
 				f.write(locus.seq())
 				f.write('\n')
 	elif args.format == 'testcode':
-		for name,locus in genbank.items():
+		for locus in genbank:
 			args.outfile.print(locus.name())
 			args.outfile.print('\t')
 			args.outfile.print(locus.testcode())
 			args.outfile.print('\n')
```

### Comparing `genbank-0.81/setup.py` & `genbank-0.96/setup.py`

 * *Files identical despite different names*

