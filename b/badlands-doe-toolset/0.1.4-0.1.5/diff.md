# Comparing `tmp/badlands_doe_toolset-0.1.4.tar.gz` & `tmp/badlands_doe_toolset-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badlands_doe_toolset-0.1.4.tar", last modified: Sun Jun 12 01:11:42 2022, max compression
+gzip compressed data, was "badlands_doe_toolset-0.1.5.tar", last modified: Sat Jun  3 01:26:54 2023, max compression
```

## Comparing `badlands_doe_toolset-0.1.4.tar` & `badlands_doe_toolset-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-12 01:11:42.234159 badlands_doe_toolset-0.1.4/
--rwxrwxrwx   0 root         (0) root         (0)    35184 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      383 2022-06-12 01:11:42.233159 badlands_doe_toolset-0.1.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      759 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-12 01:11:42.174680 badlands_doe_toolset-0.1.4/badlands_doe_toolset/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8301 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset/badlands_multiproc_run.py
--rwxrwxrwx   0 root         (0) root         (0)    19656 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset/csv_to_badlands.py
--rwxrwxrwx   0 root         (0) root         (0)    36149 2022-06-05 04:52:52.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset/postproc_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     8007 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset/postproc_xmf_update.py
--rwxrwxrwx   0 root         (0) root         (0)    16458 2022-06-08 08:11:12.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset/well_doe_similarity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-12 01:11:42.222160 badlands_doe_toolset-0.1.4/badlands_doe_toolset.egg-info/
--rw-r--r--   0 root         (0) root         (0)      383 2022-06-12 01:11:41.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      507 2022-06-12 01:11:42.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-12 01:11:41.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2022-06-12 01:11:41.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-12 01:11:42.000000 badlands_doe_toolset-0.1.4/badlands_doe_toolset.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      108 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-12 01:11:42.235159 badlands_doe_toolset-0.1.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1214 2022-06-12 01:06:36.000000 badlands_doe_toolset-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 01:26:54.103223 badlands_doe_toolset-0.1.5/
+-rwxrwxrwx   0 root         (0) root         (0)    35184 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-03 01:26:54.101221 badlands_doe_toolset-0.1.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      741 2022-09-26 02:36:28.000000 badlands_doe_toolset-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 01:26:54.032220 badlands_doe_toolset-0.1.5/badlands_doe_toolset/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8301 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset/badlands_multiproc_run.py
+-rwxrwxrwx   0 root         (0) root         (0)    19656 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset/csv_to_badlands.py
+-rwxrwxrwx   0 root         (0) root         (0)    43825 2023-02-19 03:39:06.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset/postproc_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    11276 2023-03-28 07:05:04.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset/postproc_xmf_update.py
+-rwxrwxrwx   0 root         (0) root         (0)    16458 2022-06-08 08:11:12.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset/well_doe_similarity.py
+-rwxrwxrwx   0 root         (0) root         (0)    17829 2023-01-29 01:59:19.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset/well_doe_similarity_experimental.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-03 01:26:54.089222 badlands_doe_toolset-0.1.5/badlands_doe_toolset.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-03 01:26:53.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-03 01:26:53.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-03 01:26:53.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-03 01:26:53.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-03 01:26:53.000000 badlands_doe_toolset-0.1.5/badlands_doe_toolset.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      108 2022-06-01 23:13:39.000000 badlands_doe_toolset-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-03 01:26:54.104222 badlands_doe_toolset-0.1.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1214 2023-06-03 01:20:08.000000 badlands_doe_toolset-0.1.5/setup.py
```

### Comparing `badlands_doe_toolset-0.1.4/LICENSE` & `badlands_doe_toolset-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `badlands_doe_toolset-0.1.4/README.md` & `badlands_doe_toolset-0.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # badlands_doe_toolset
-a set of tools to simply combine the setup and analysis of Badlands using Design of Experiments (DoEgen) python software.
+A set of tools that combines the setup and analysis of Badlands using Design of Experiments (DoEgen) python software.
 see 
 https://badlands.readthedocs.io/
 and
 https://github.com/sebhaan/DoEgen
 
 
-This repository is also available on pip testing, to install:
+This repository is also available on pip, to install:
 
-pip install -i https://test.pypi.org/simple/ badlands-doe-toolset
+pip install badlands-doe-toolset
 
 
 An example on the functionality and description of how to use this is available here:
 
 https://github.com/GeoMattB/Badlands_DOE_examples
 
 
-This research was supported by the Sydney Informatics Hub, a Core Research Facility of the University of Sydney.
+The DoEgen component of this research was supported by the Sydney Informatics Hub, a Core Research Facility of the University of Sydney.
 
 It is an extension/implementaton of :
 
 https://github.com/sebhaan/DoEgen
 
 https://github.com/Sydney-Informatics-Hub/DoEgen-Geo
+
```

### Comparing `badlands_doe_toolset-0.1.4/badlands_doe_toolset/badlands_multiproc_run.py` & `badlands_doe_toolset-0.1.5/badlands_doe_toolset/badlands_multiproc_run.py`

 * *Files identical despite different names*

### Comparing `badlands_doe_toolset-0.1.4/badlands_doe_toolset/csv_to_badlands.py` & `badlands_doe_toolset-0.1.5/badlands_doe_toolset/csv_to_badlands.py`

 * *Files identical despite different names*

### Comparing `badlands_doe_toolset-0.1.4/badlands_doe_toolset/postproc_utils.py` & `badlands_doe_toolset-0.1.5/badlands_doe_toolset/postproc_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import sys
 import time
 import badlands_doe_toolset.badlands_multiproc_run as mpr
 import ntpath
 from functools import partial
 import matplotlib.pyplot as plt
 from pyevtk.hl import gridToVTK
+from pathlib import Path
 
 """ this Stratdata class might be removed and the Stratigraphy class from StratalMesh used instead, however I don't need to reshape the arrays here"""
 class Stratadata:
     """
     Class for loading data from stratal files.
     """
     def __init__(self):
@@ -159,14 +160,51 @@
         #attrib_temp = interp.griddata((tin.x, tin.y), getattr(tin,attribs[i]) , (X, Y), method='nearest') #
         attrib_temp = interp.griddata((tin.x, tin.y), tin.tin_layer[i][:] , (X, Y), method='nearest')
         attrib_temp = attrib_temp.flatten()
         attribs_inter.append(attrib_temp)
     return(attribs_inter)
 
 
+#This function writes the instdiff parameter to the tin.time files. Useful for time-step visualisation in paraview, 
+# could probably be done entirely in PV as a filter but I couldn't work out how to do it dynamically for animations in paraview.
+# to do use multiproc to speed this up
+def tin_write_instdiff(modelfile):
+    model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
+    modelh5dir=model.outDir+'/h5'
+    maxSteps=int(model.tEnd/model.tDisplay)
+
+    #loop through the tin.timeXX loading each as we go.
+    for i in range(0,maxSteps):
+        tin_N=TINfile()
+        tin_N1=TINfile()
+        tin_N.loadTIN(modelh5dir+'/tin.time'+str(i)+'.hdf5')
+        #return(tin_N)
+        tin_N1.loadTIN(modelh5dir+'/tin.time'+str(i+1)+'.hdf5')
+        
+        #this is a bit not-that-useful, it just adds an attribute to the first (zero) layer to keep outputs consistent / tidy.
+        if i==0:
+            instdiff=tin_N.tin_layer['cumdiff'][:]
+            with h5py.File((modelh5dir+'/tin.time'+str(i)+'.hdf5'), 'a') as t:
+                print('tin.time'+str(i))
+                if ('instdiff') in t.keys():
+                    del t['instdiff'] # if the value exists already remove it
+                t.require_dataset('instdiff', data=instdiff, shape=instdiff.shape, dtype="f",compression="gzip" )
+                t.close()
+        
+        # subtracts (layer N) from (layer N+1) and adds it to the tin file, this is the main bit.
+        else:
+            instdiff=(tin_N1.tin_layer['cumdiff'][:])-(tin_N.tin_layer['cumdiff'][:])
+        with h5py.File((modelh5dir+'/tin.time'+str(i+1)+'.hdf5'), 'a') as t:
+            print('tin.time'+str(i+1))
+            if ('instdiff') in t.keys():
+                del t['instdiff'] # if the value exists already remove it
+            t.require_dataset('instdiff', data=instdiff, shape=instdiff.shape, dtype="f",compression="gzip" )
+            t.close()
+
+
 #This function writes the list of supplied parameters in a models tin.time files to the final sed.time file.
 def strat_tin_write(attribs,modelfile):
     model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
     modelh5dir=model.outDir+'/h5'
     maxSteps=int(model.tEnd/model.tDisplay)
     strat_file=modelh5dir+'/sed.time'+str(maxSteps)+'.hdf5'
     
@@ -186,27 +224,40 @@
     for i in range(0,maxSteps+1):
         attributes_interpolate_results=interp_from_tin(X,Y,nx,ny,modelh5dir+'/tin.time'+str(i)+'.hdf5',attribs)
         # loop over the results to populate the dict/dataframes
         for j in range(0,len(attributes_interpolate_results)):       
             dataout[attribs[j]][i]=attributes_interpolate_results[j]
     
     # dataout now needs to be written to the final sed.time file, open the strat file, append each attribute
-    # note, this is an append function and if the attribute already exists it won't be overwritten.    
+    # note, the require_dataset function won't overwrite the attribute if it already exists, so the attribute is first removed if it exists using the if / in statement for each.     
     with h5py.File(strat_file, 'a') as g:
         print('writing to file')
         for i in attribs:
             if i =='cumdiff': 
+                if ('layinstdiff') in g.keys():
+                    del g['layinstdiff'] # if the value exists already remove it
                 print('cumdiff specified, generating instdiff as well')
                 dataout['instdiff']=np.copy(dataout['cumdiff'])
                 dataout['instdiff'][:, 1:] -= dataout['instdiff'][:, :-1]  #cumdiff is more useful as a rate of depostion for that step, subtract previous column (timestep) to get deposition/erosion per step.
                 dataout['instdiff'][:, 0] = 0
                 g.require_dataset(str('layinstdiff'), data=dataout['instdiff'], shape=dataout['instdiff'].shape, dtype="f",compression="gzip" )
-            elif ('lay'+str(i)) in g.keys():
-                del g['lay'+str(i)] # if the value exists already remove it
-            g.require_dataset('lay'+str(i), data=dataout[i], shape=dataout[i].shape, dtype="f",compression="gzip" )
+
+            if i =='cumhill': 
+                if ('layinsthill') in g.keys():
+                    del g['layinsthill'] # if the value exists already remove it
+                print('cumhill specified, generating insthill as well')
+                dataout['insthill']=np.copy(dataout['cumhill'])
+                dataout['insthill'][:, 1:] -= dataout['insthill'][:, :-1]  #cumhill is more useful as a rate of depostion for that step, subtract previous column (timestep) to get deposition/erosion per step.
+                dataout['insthill'][:, 0] = 0
+                g.require_dataset(str('layinsthill'), data=dataout['insthill'], shape=dataout['insthill'].shape, dtype="f",compression="gzip" )
+
+            else:
+                if ('lay'+str(i)) in g.keys():
+                    del g['lay'+str(i)] # if the value exists already remove it
+                g.require_dataset('lay'+str(i), data=dataout[i], shape=dataout[i].shape, dtype="f",compression="gzip" )
         g.close()
         print('completed '+strat_file)
 
 
 #This function writes the specified attributes from tin files to the final strata output in a set of DoEgen experiments
 def strat_tin_write_doegen(xml_dir,attribs,proc=None):
 #    import lib.badlands_multiproc_run as mpr
@@ -242,16 +293,48 @@
     #interpolate the data onto the strata array
     for i in attribs:
         #attrib_temp = interp.griddata((flow.x, flow.y), getattr(flow,attribs[i]) , (X, Y), method='nearest') #
         attrib_temp = interp.griddata((flow.x, flow.y), flow.flw_layer[i][:] , (X, Y), method='nearest')
         attrib_temp = attrib_temp.flatten()
         attribs_inter.append(attrib_temp)
     return(attribs_inter)
+    
+# Interpolates a flow files attributes onto a TIN file to make it easy to compare stuff.
+def interp_flow_to_tin(flow_file,tin_file,attribs):
+    #use the Flow class to load the flow array
+    flow=Flowfile()
+    flow.loadFlow(flow_file)
+    attribs_inter=[]
+    tin=TINfile()
+    tin.loadTIN(tin_file)
+    
+    #interpolate the data onto the strata array
+    for i in attribs:
+        attrib_temp = interp.griddata((flow.x, flow.y), flow.flw_layer[i][:] , (tin.x, tin.y), method='nearest')
+        attrib_temp = attrib_temp.flatten()
+        attribs_inter.append(attrib_temp)
+    return(attribs_inter)
 
-#This writes the interp onto the final stratal file for all of flow files in a model.
+#write the flow.time attributes to the tin.tin attributes by interpolation for an entire experiment/model
+def tin_write_flow_experiment(modelfile,attribs):
+    model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
+    modelh5dir=model.outDir+'/h5'
+    maxSteps=int(model.tEnd/model.tDisplay)
+    for i in range(0,maxSteps):
+        tin_file=(modelh5dir+'/tin.time'+str(i)+'.hdf5')
+        flow_file=(modelh5dir+'/flow.time'+str(i)+'.hdf5')
+        attribs_inter=interp_flow_to_tin(flow_file,tin_file,attribs)
+        with h5py.File(tin_file, 'a') as t:
+            for i in range(len(attribs)):
+                if (attribs[i]) in t.keys():
+                    del t[attribs[i]] # if the attribute exists already remove it (possible errors check so we don't remove x/y
+                t.require_dataset(attribs[i], data=attribs_inter[i], shape=attribs_inter[i].shape, dtype="f",compression="gzip" )
+            t.close()
+        
+ #This writes the interp onto the final stratal file for all of flow files in a model.
 def strat_flow_write(attribs,modelfile):
     model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
     modelh5dir=model.outDir+'/h5'
     maxSteps=int(model.tEnd/model.tDisplay)
     strat_file=modelh5dir+'/sed.time'+str(maxSteps)+'.hdf5'
     
     #load in the XY coords from the stratal file.
@@ -401,14 +484,91 @@
     with h5py.File(strat_file, 'r+') as g:
         if 'layTerrRough' in g.keys():
             del g['layTerrRough'] # if the value exists already remove it
         g.require_dataset('layTerrRough', data=TRI, shape=TRI.shape, dtype="f", compression="gzip" )
         g.close()
         print(str(model.outDir) + '  final strat file written')
 
+#Writes a QGIS compatible TIN mesh ascii file, 
+# write the header and then the triangle cell / node index values
+#assign an index to the cells as well, this is required for the format
+def TIN_hdf_to_2dm(outpath,hdf5_input):
+    g=TINfile()
+    g.loadTIN(hdf5_input)
+    outname=Path(hdf5_input).stem
+    #print(outname)
+    outfile2dm=outpath+'/'+(Path(hdf5_input).stem)+'.2dm'
+
+    with open (outfile2dm,'w') as f:
+            f.write('MESH2D')
+            f.write('\n')
+            f.write(f"MESHNAME, {outname}")
+            f.write('\n')
+            for i in range(0,len(g.cells)):
+                f.write('E3T')
+                f.write(' ')
+                f.write(str(i))
+                f.write(' ')
+                f.write(str(g.cells[i][0]))
+                f.write(' ')
+                f.write(str(g.cells[i][1]))
+                f.write(' ')
+                f.write(str(g.cells[i][2]))
+                f.write('\n')
+            f.close()
+    #append coordinate values to the text file (round XY coords to cm / 2 decimal places)
+    with open(outfile2dm,'a') as f:
+        for i in range(0,len(g.x)):
+            f.write('ND')
+            f.write(' ')
+            f.write(str(i))
+            f.write(' ')
+            f.write(str(round(g.x[i],2)))
+            f.write(' ')
+            f.write(str(round(g.y[i],2)))
+            f.write(' ')
+            f.write(str(round(g.z[i],2)))
+            f.write('\n')
+        f.close()
+
+def experiment_TIN_hdf_to_2dm(modelfile):
+    model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
+    modelh5dir=model.outDir+'/h5'
+    maxSteps=int(model.tEnd/model.tDisplay)
+    model2dmdir=model.outDir+'/2dm'
+    isExist = os.path.exists(model2dmdir)
+    if not isExist:
+        os.makedirs(model2dmdir)
+    #loop through the hdf5 tin files creating the output for each
+    for i in range(0,maxSteps+1):
+        hdf5_input=modelh5dir+'/tin.time'+str(i)+'.hdf5'
+        TIN_hdf_to_2dm(model2dmdir,hdf5_input)
+        
+## multiproc version of the experiment level conversion
+def MP_TIN_hdf_to_2dm(modelfile):
+#    import lib.badlands_multiproc_run as mpr
+    model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
+    modelh5dir=model.outDir+'/h5/'
+    maxSteps=int(model.tEnd/model.tDisplay)
+    model2dmdir=model.outDir+'/2dm/'
+    isExist = os.path.exists(model2dmdir)
+    if not isExist:
+        os.makedirs(model2dmdir)
+    TINlist=[]
+    for i in range(0,maxSteps+1):
+        TINlist.append(modelh5dir+'tin.time'+str(i)+'.hdf5')
+    print (str(len(TINlist))+' surfaces to convert from hdf5 to 2dm for QGIS')
+    cpuCount = os.cpu_count() #lets use all the threads
+    print ("number of threads available here: "+str(cpuCount)) 
+    with Pool(processes = cpuCount) as p:
+        async_result = p.map_async(partial(TIN_hdf_to_2dm,model2dmdir),TINlist)
+        p.close()
+        p.join()
+        print('All outputs written')
+#################
 
 class Welldata:
     """
     Class for loading data from well csv file.
     """
     def __init__(self):
         self.well_name = None
@@ -506,16 +666,16 @@
         h5file.close()
         return('data written to '+str(outfile_loc))
         
         
     
     def extractWellsExperiment(self,modelfile,wellfile,outfile_loc): #was extractWellsModel
         """
-        Get the well locations from the wellfile then extract the 
-        Then extract the properties at the well
+        Get the well locations from the wellfile
+        and extract the properties at the well for all of the layers
         """
         h5file=h5py.File(str(outfile_loc),'a')
         
         model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
         modelh5dir=model.outDir+'/h5'
         maxSteps=int(model.tEnd/model.tDisplay)
         strat_file=modelh5dir+'/sed.time'+str(maxSteps)+'.hdf5'
```

### Comparing `badlands_doe_toolset-0.1.4/badlands_doe_toolset/postproc_xmf_update.py` & `badlands_doe_toolset-0.1.5/badlands_doe_toolset/postproc_xmf_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -87,59 +87,143 @@
         print ('reading '+hdf_file)
         xmf_file=str(modelXmfdir)+'/tin.time'+str(i)+'.xmf'
         print ('output will be '+xmf_file)
         f=h5py.File(hdf_file, 'r')
         tmstep=float(i*model.tDisplay)
         cells=len(f['cells'])
         geom=len(f['coords'])
-#        row=pd.DataFrame()
-#        row['cells']=cells,
-#        row['geom']=geom,
+        row=pd.DataFrame()
+        row['cells']=cells,
+        row['geom']=geom,
         texfile=open(xmf_file,'w')
         texfile.write(f"""<?xml version="1.0" encoding="UTF-8"?>
 <!DOCTYPE Xdmf SYSTEM "Xdmf.dtd">
 <Xdmf Version="2.0" xmlns:xi="http://www.w3.org/2001/XInclude">
  <Domain>
     <Grid GridType="Collection" CollectionType="Spatial">
       <Time Type="Single" Value="{tmstep}"/>
       <Grid Name="Block.0">
          <Topology Type="Triangle" NumberOfElements="{(int(row['cells']))}" BaseOffset="1">
-          <DataItem Format="HDF" DataType="Int" Dimensions="{int(cells)} 2">h5/tin.time{i}.hdf5:/cells</DataItem>
+          <DataItem Format="HDF" DataType="Int" Dimensions="{int(cells)} 3">h5/tin.time{i}.hdf5:/cells</DataItem>
          </Topology>
          <Geometry Type="XYZ">
           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 3">h5/tin.time{i}.hdf5:/coords</DataItem>
          </Geometry>
          <Attribute Type="Scalar" Center="Node" Name="lake">
-          <DataItem Format="HDF" NumberType="Integer" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/lake</DataItem>
+          <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/lake</DataItem>
          </Attribute>
-         <Attribute Type="Scalar" Center="Node" Name="Discharge [m3/s]">
+         <Attribute Type="Scalar" Center="Node" Name="Discharge">
           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/discharge</DataItem>
          </Attribute>
-         <Attribute Type="Scalar" Center="Node" Name="cumdiff">
+         <Attribute Type="Scalar" Center="Node" Name="EroDep">
           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/cumdiff</DataItem>
          </Attribute>
-         <Attribute Type="Scalar" Center="Node" Name="cumhill [m3/s]">
+         <Attribute Type="Scalar" Center="Node" Name="EroDep hillslope">
           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/cumhill</DataItem>
          </Attribute>
-         <Attribute Type="Scalar" Center="Node" Name="cumfail adim">
+         <Attribute Type="Scalar" Center="Node" Name="EroDep failure">
           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/cumfail</DataItem>
          </Attribute>
          <Attribute Type="Scalar" Center="Node" Name="Sealevel">
           <DataItem ItemType="Function" Function="$0 * 0.00000000001 + {SeaLvl}" Dimensions="{int(geom)} 1">
-           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time1.hdf5:/cumdiff</DataItem>
+           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/cumdiff</DataItem>
           </DataItem>
          </Attribute>
          """)
         for g in (f.keys()): ## if there are any new parameters add them to the xmf for paraview.
-            if g !='coords' and g !='cells' and g !='lake' and g !='discharge' and g !='cumdiff' and g !='cumhill' and g !='cumhill' and g !='cumfail' and g !='lake':
+            if g !='coords' and g !='area' and g !='cells' and g !='lake' and g !='discharge' and g !='cumdiff' and g !='cumhill' and g !='cumfail' and g !='lake':
                 texfile.write(f"""
          <Attribute Type="Scalar" Center="Node" Name="{str(g)}">
           <DataItem Format="HDF" NumberType="Float" Precision="4" Dimensions="{int(geom)} 1">h5/tin.time{i}.hdf5:/{str(g)}</DataItem>
          </Attribute>""")
         texfile.write(f""" 
       </Grid>
     </Grid>
  </Domain>
 </Xdmf>
 """)
     texfile.close()
+ 
+# XMF for sed time strat files
+# single xmf build write the xmf to view in paraview
+def sedfile_xmf(hdf_file,modelinc,tDisplay=100000)  
+        print ('load '+hdf_file)
+        strat=ppu.Stratadata()
+        strat.loadStrat(hdf_file)
+        f=h5py.File(hdf_file, 'r')
+        tmstep=modelinc*tDisplay
+        NumberOfElements=str(strat.ny)+' ' +str(strat.nx) + ' ' +str(strat.nz)
+        Dimensions= str(len(strat.x))+' '+ str(strat.nz)
+        print(Dimensions)
+        xmf_file='xmf/sed.time'+str(modelinc)+'.xmf'
+        print ('output will be '+xmf_file)
+        
+        texfile=open(xmf_file,'w')
+        texfile.write(f"""<?xml version="1.0" encoding="UTF-8"?>
+<!DOCTYPE Xdmf SYSTEM "Xdmf.dtd">
+<Xdmf Version="2.0" xmlns:xi="http://www.w3.org/2001/XInclude">
+ <Domain>
+  <Grid GridType="Collection" CollectionType="Spatial">
+  <Time Type="Single" Value="{tmstep}"/>
+    <Grid Name="Block.0" GridType="Uniform">
+     <Topology TopologyType="3DSMesh" Format="HDF" NumberOfElements="{NumberOfElements}" BaseOffset="1">
+     </Topology>
+      <Geometry GeometryType="X_Y_Z">
+        <DataItem Name="X" Dimensions="{Dimensions}" NumberType="Float" Precision="4" Format="HDF"> {hdf_file}:/X </DataItem>
+        <DataItem Name="Y" Dimensions="{Dimensions}" NumberType="Float" Precision="4" Format="HDF"> {hdf_file}:/Y </DataItem>
+        <DataItem Name="Z" Dimensions="{Dimensions}" NumberType="Float" Precision="4" Format="HDF"> {hdf_file}:/layDepth </DataItem>
+      </Geometry>
+""")
+        for g in (f.keys()): ## if there are any other attributes add them to the xmf for paraview.
+            if g !='X' and g !='Y' and g !='coords':
+                texfile.write(f"""
+      <Attribute Type="Scalar" Center="Node" Name="{str(g)}">
+        <DataItem Dimensions="{NumberOfElements}" Format="HDF" NumberType="Float" Precision="4"> {hdf_file}:/{str(g)} </DataItem>
+      </Attribute>""")
+        texfile.write(f""" 
+    
+    </Grid>
+   </Grid>
+ </Domain>
+</Xdmf>
+""")
+    texfile.close()
+
+
+#write all of the xmf files and then the XDMF for a time series. 
+def sedfile_xdmf(modelfile):
+    model=xmlParser.xmlParser(modelfile,'False') #just read in the xml 'False' stops it writing output directories'
+    modelh5dir=model.outDir+'/h5'
+    maxSteps=int(model.tEnd/model.tDisplay)
+    modelXmfdir=model.outDir+'/xmf'
+    SeaLvl=model.seapos
+    
+    ## send to xmf function
+    for i in range(1,maxSteps+1):
+        hdf_file=modelh5dir+'/sed.time'+str(i)+'.hdf5'
+        sedfile_xmf(hdf_file,i)
+  
+##XMDF part
+#Write the xdmf time series file to tie this all together
+    xdmf_file=model.outDir+'/sedtime_series.xdmf'
+    texfile=open(xdmf_file,'w')
+    texfile.write(f"""<?xml version="1.0" encoding="UTF-8"?>
+<!DOCTYPE Xdmf SYSTEM "Xdmf.dtd">
+<Xdmf Version="2.0" xmlns:xi="http://www.w3.org/2001/XInclude">
+ <Domain>
+    <Grid GridType="Collection" CollectionType="Temporal">
+""")
+    for i in range(1,maxSteps+1):
+        xmf_file=str(modelXmfdir)+'/sed.time'+str(i)+'.xmf'
+        texfile.write(f"""     <xi:include href="xmf/sed.time{i}.xmf" xpointer="xpointer(//Xdmf/Domain/Grid)"/>
+""")
+    
+    texfile.write(f"""  </Grid>
+ </Domain>
+</Xdmf>
+""")
+    texfile.close()   
+    
+    
+
     
+
```

### Comparing `badlands_doe_toolset-0.1.4/badlands_doe_toolset/well_doe_similarity.py` & `badlands_doe_toolset-0.1.5/badlands_doe_toolset/well_doe_similarity.py`

 * *Files identical despite different names*

### Comparing `badlands_doe_toolset-0.1.4/setup.py` & `badlands_doe_toolset-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 if __name__ == "__main__":
     setup(
         name="badlands_doe_toolset",
         author="Matt Boyd",
         author_email="mboyd@sydney.edu.au",
         url="https://github.com/GeoMattB",
-        version="0.1.4",
+        version="0.1.5",
         description="badlands_doe_toolset is a set of tools to help build and analyse Design of Experiment configurations for badlands modelling",
         ext_modules = [],
         packages=['badlands_doe_toolset'],
         package_data={'badlands_doe_toolset':sys_includes},
         data_files=[('badlands_doe_toolset',sys_includes)],
         include_package_data=True,
         install_requires=[
```

