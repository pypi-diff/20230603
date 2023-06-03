# Comparing `tmp/install-pybci-0.2.2b1.tar.gz` & `tmp/install-pybci-0.2.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.2b1.tar", last modified: Mon May 29 00:08:06 2023, max compression
+gzip compressed data, was "install-pybci-0.2.3b0.tar", last modified: Sat Jun  3 16:51:21 2023, max compression
```

## Comparing `install-pybci-0.2.2b1.tar` & `install-pybci-0.2.3b0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.765080 install-pybci-0.2.2b1/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 00:08:06.000000 install-pybci-0.2.2b1/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7779 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:08:06.769081 install-pybci-0.2.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-29 00:07:14.000000 install-pybci-0.2.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 16:51:21.000000 install-pybci-0.2.3b0/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/OptimisedDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 16:51:21.528853 install-pybci-0.2.3b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-03 16:50:48.000000 install-pybci-0.2.3b0/setup.py
```

### Comparing `install-pybci-0.2.2b1/LICENSE` & `install-pybci-0.2.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b1/PKG-INFO` & `install-pybci-0.2.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.2b1
+Version: 0.2.3b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `install-pybci-0.2.2b1/README.md` & `install-pybci-0.2.3b0/README.md`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b1/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.3b0/install_pybci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.2b1
+Version: 0.2.3b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
```

### Comparing `install-pybci-0.2.2b1/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.3b0/install_pybci.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 pybci/Configuration/FeatureSettings.py
 pybci/Configuration/__init__.py
 pybci/ThreadClasses/AsyncDataReceiverThread.py
 pybci/ThreadClasses/ClassifierThread.py
 pybci/ThreadClasses/DataReceiverThread.py
 pybci/ThreadClasses/FeatureProcessorThread.py
 pybci/ThreadClasses/MarkerThread.py
+pybci/ThreadClasses/OptimisedDataReceiverThread.py
 pybci/ThreadClasses/__init__.py
 pybci/Utils/Classifier.py
 pybci/Utils/FeatureExtractor.py
 pybci/Utils/LSLScanner.py
 pybci/Utils/Logger.py
 pybci/Utils/__init__.py
```

### Comparing `install-pybci-0.2.2b1/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.3b0/pybci/Configuration/EpochSettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class GlobalEpochSettings:
-    splitCheck = False  # checks whether or not subdivide epochs
+    splitCheck = True  # checks whether or not subdivide epochs
     tmin = 0      # time in seconds to capture samples before trigger
     tmax = 1      # time in seconds to capture samples after trigger
     windowLength = 0.5    # if splitcheck true - time in seconds to split epoch
     windowOverlap = 0.5 #if splitcheck true  percentage value > 0 and < 1, example if epoch has tmin of 0 and tmax of 1 with window 
     # length of 0.5 we have 1 epoch between t 0 and t0.5 another at 0.25 to 0.75, 0.5 to 1
 
 # customWindowSettings should be dict with marker name and IndividualEpochSetting
 class IndividualEpochSetting:
-    splitCheck = False  # checks whether or not subdivide epochs
+    splitCheck = True  # checks whether or not subdivide epochs
     tmin = 0      # time in seconds to capture samples before trigger
     tmax=  1      # time in seconds to capture samples after trigger
```

### Comparing `install-pybci-0.2.2b1/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.3b0/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b1/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.3b0/pybci/ThreadClasses/ClassifierThread.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ..Utils.Logger import Logger
 import queue,threading, time
 
 class ClassifierThread(threading.Thread):
     features = []
     targets = []
     mode = "train"
-    guess = None
+    guess = " "
     epochCounts = {} 
     def __init__(self, closeEvent,trainTestEvent, featureQueueTest,featureQueueTrain, classifierInfoQueue, classifierInfoRetrieveEvent, 
                  classifierGuessMarkerQueue, classifierGuessMarkerEvent, queryFeaturesQueue, queryFeaturesEvent,
                  logger = Logger(Logger.INFO), numStreamDevices = 1,
                  minRequiredEpochs = 10, clf = None, model = None, torchModel = None):
         super().__init__()
         self.trainTestEvent = trainTestEvent # responsible for tolling between train and test mode
@@ -47,67 +47,68 @@
                             if len(self.epochCounts) > 1: # check if there is more then one test condition
                                 minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                                 if minNumKeyEpochs < self.minRequiredEpochs:
                                     pass
                                 else: 
                                     start = time.time()
                                     self.classifier.TrainModel(self.features, self.targets)
-                                    if (self.logger.level == Logger.INFO):
+                                    if (self.logger.level == Logger.TIMING):
                                         end = time.time()
-                                        self.logger.log(Logger.INFO, f" classifier training time {end - start}")
+                                        self.logger.log(Logger.TIMING, f" classifier training time {end - start}")
                             if self.classifierGuessMarkerEvent.is_set():
-                                self.classifierGuessMarkerQueue.put(None)
+                                self.classifierGuessMarkerQueue.put(self.guess)
                     else: # Only one device to collect from
                         self.targets.append(target)
                         self.features.append(featuresSingle)
                         if len(self.epochCounts) > 1: # check if there is more then one test condition
                             minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                             if minNumKeyEpochs < self.minRequiredEpochs:
                                 pass
                             else: 
                                 start = time.time()
                                 self.classifier.TrainModel(self.features, self.targets)
-                                if (self.logger.level == Logger.INFO):
+                                if (self.logger.level == Logger.TIMING):
                                     end = time.time()
-                                    self.logger.log(Logger.INFO, f" classifier training time {end - start}")
+                                    self.logger.log(Logger.TIMING, f" classifier training time {end - start}")
                         if self.classifierGuessMarkerEvent.is_set():
-                            self.classifierGuessMarkerQueue.put(None)
+                            self.classifierGuessMarkerQueue.put(self.guess)
                 except queue.Empty:
                     pass
             else: # We're testing!
                 try:
                     featuresSingle, devCount = self.featureQueueTest.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
                     if self.numStreamDevices > 1:
                         tempdatatest[devCount] = featuresSingle
                         if len(tempdatatest) == self.numStreamDevices:
                             flattened_list = []
                             for value in tempdatatest.values():
                                 flattened_list.extend(value)
                             tempdatatest = {}
                             start = time.time()
                             self.guess = self.classifier.TestModel(flattened_list)
-                            if (self.logger.level == Logger.INFO):
+                            if (self.logger.level == Logger.TIMING):
                                 end = time.time()
-                                self.logger.log(Logger.INFO, f" classifier testing time {end - start}")
+                                self.logger.log(Logger.TIMING, f" classifier testing time {end - start}")
                     else:
                         start = time.time()
                         self.guess = self.classifier.TestModel(featuresSingle)
-                        if (self.logger.level == Logger.INFO):
+                        if (self.logger.level == Logger.TIMING):
                             end = time.time()
-                            self.logger.log(Logger.INFO, f" classifier testing time {end - start}")
+                            self.logger.log(Logger.TIMING, f" classifier testing time {end - start}")
                     if self.classifierGuessMarkerEvent.is_set():
                         self.classifierGuessMarkerQueue.put(self.guess)
                 except queue.Empty:
                     pass
             if self.classifierInfoRetrieveEvent.is_set():
+                a = self.classifier.accuracy
                 classdata = {
                     "clf":self.classifier.clf,
                     "model":self.classifier.model,
                     "torchModel":self.classifier.torchModel,
-                    "accuracy":self.classifier.accuracy
+                    "accuracy":a
                     }
                 self.classifierInfoQueue.put(classdata) 
             if self.queryFeaturesEvent.is_set():
                 featureData = {
                     "features":self.features,
                     "targets":self.targets
                 }
```

### Comparing `install-pybci-0.2.2b1/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.3b0/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b1/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.2.3b0/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b1/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.3b0/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b1/pybci/Utils/Classifier.py` & `install-pybci-0.2.3b0/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.2b1/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.3b0/pybci/Utils/FeatureExtractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import antropy as ant
 import numpy as np
 from scipy.signal import welch
 from scipy.integrate import simps
-import warnings
+import warnings, time
+from ..Utils.Logger import Logger
 from ..Configuration.FeatureSettings import GeneralFeatureChoices
 # Filter out UserWarning messages from the scipy package, could be worth moving to init and applying printdebug print levels? (typically nans, 0 and infs causing errors)
 warnings.filterwarnings("ignore", category=UserWarning, module="scipy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=UserWarning, module="antropy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=RuntimeWarning, module="antropy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=RuntimeWarning, module="numpy") # used to reduce print statements from constant signals being applied
 #warnings.filterwarnings("ignore", category=RuntimeWarning, module="pybci") # used to reduce print statements from constant signals being applied
 
 class GenericFeatureExtractor():
+    logger = Logger(Logger.INFO)
 
-    def __init__(self, freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()):
+    def __init__(self, logger = Logger(Logger.INFO), freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()):
         super().__init__()
         self.freqbands = freqbands
         self.featureChoices = featureChoices
         #for key, value in self.featureChoices.__dict__.items():
         #    print(f"{key} = {value}")
+        self.logger = logger
         selFeats = sum([self.featureChoices.appr_entropy,
             self.featureChoices.perm_entropy,
             self.featureChoices.spec_entropy,
             self.featureChoices.svd_entropy,
             self.featureChoices.samp_entropy,
             self.featureChoices.rms,
             self.featureChoices.meanPSD,
@@ -46,80 +49,86 @@
             sr = samplerate of current device
         Returns:
             features = 2D numpy array of size (chs, (len(freqbands) + sum(True in self.featureChoices)))
             target = same as input target, can be useful for using a baseline number differently
         NOTE: Any channels with a constant value will generate warnings in any frequency based features (constant level == no frequency components).
         """
         #print(np.array(epoch).shape)
-        numchs = len(epoch)
+        #print(epoch)
+        start = time.time()
+        numchs = epoch.shape[1]
         features = np.zeros(numchs * self.numFeatures)
-        for k, ch in enumerate(epoch):
+
+        for ch in range(epoch.shape[1]):
             #ch = np.isnan(ch)
             if self.featureChoices.psdBand: # get custom average power within given frequency band from freqbands
-                freqs, psd = welch(ch, sr)
+                freqs, psd = welch(epoch[:,ch], sr)
                 for l, band in enumerate(self.freqbands):
                     if len(freqs) > 0: # len(freqs) can be 0 if signal is all DC
                         idx_band = np.logical_and(freqs >= band[0], freqs <= band[1])
                         #if len(psd[idx_band]) == 1: # if freq band is only in one field just pass single value instead of calculating average
                         #print(ch)
                         bp = np.mean(psd[idx_band])
                         #else:
                         #    bp = simps(psd[idx_band], dx=(freqs[1]-freqs[0])) / (band[1] - band[0])
                             #bp = simpson(psd[idx_band], dx=freq_res)
-                        features[(k* self.numFeatures)+l] = bp
+                        features[(ch* self.numFeatures)+l] = bp
                     else:
-                        features[(k* self.numFeatures)+l] = 0
+                        features[(ch* self.numFeatures)+l] = 0
             else:
-                freqs, psd = welch(ch, sr)# calculate for mean and median
+                freqs, psd = welch(epoch[:,ch], sr)# calculate for mean and median
                 l = -1 # accounts for no freqbands being selected
             if self.featureChoices.meanPSD: # mean power
                 l += 1
-                if len(freqs) > 0: features[(k* self.numFeatures)+l] = np.mean(psd) # len(freqs) can be 0 if signal is all DC
-                else: features[(k* self.numFeatures)+l] = 0
+                if len(freqs) > 0: features[(ch* self.numFeatures)+l] = np.mean(psd) # len(freqs) can be 0 if signal is all DC
+                else: features[(ch* self.numFeatures)+l] = 0
             if self.featureChoices.medianPSD: # median Power
                 l += 1   
-                if len(freqs) > 0: features[(k* self.numFeatures)+l] = np.median(psd) # len(freqs) can be 0 if signal is all DC
-                else: features[(k* self.numFeatures)+l] = 0
-            if self.featureChoices.appr_entropy:  # Approximate entorpy(X,M,R) X = data, M is , R is 30% standard deviation of X 
+                if len(freqs) > 0: features[(ch* self.numFeatures)+l] = np.median(psd) # len(freqs) can be 0 if signal is all DC
+                else: features[(ch* self.numFeatures)+l] = 0
+            if self.featureChoices.appr_entropy:  # Approximate entropy(X,M,R) X = data, M is , R is 30% standard deviation of X 
                 l += 1
-                features[(k* self.numFeatures)+l] = ant.app_entropy(ch) 
+                features[(ch* self.numFeatures)+l] = ant.app_entropy(epoch[:,ch]) 
             if self.featureChoices.perm_entropy: # permutation_entropy
                 l += 1
-                features[(k* self.numFeatures)+l] = ant.perm_entropy(ch,normalize=True)
+                features[(ch* self.numFeatures)+l] = ant.perm_entropy(epoch[:,ch],normalize=True)
             if self.featureChoices.spec_entropy:  # spectral Entropy
                 l += 1
-                features[(k* self.numFeatures)+l] = ant.spectral_entropy(ch, sf=sr, method='welch', nperseg = len(ch), normalize=True)
+                features[(ch* self.numFeatures)+l] = ant.spectral_entropy(epoch[:,ch], sf=sr, method='welch', nperseg = len(epoch[:,ch]), normalize=True)
             if self.featureChoices.svd_entropy:# svd Entropy
                 l += 1
-                features[(k* self.numFeatures)+l] = ant.svd_entropy(ch, normalize=True)
+                features[(ch* self.numFeatures)+l] = ant.svd_entropy(epoch[:,ch], normalize=True)
             if self.featureChoices.samp_entropy: # sample Entropy
                 l += 1
-                features[(k* self.numFeatures)+l] = ant.sample_entropy(ch)
+                features[(ch* self.numFeatures)+l] = ant.sample_entropy(epoch[:,ch])
             if self.featureChoices.rms: # rms
                 l += 1
-                features[(k* self.numFeatures)+l] = np.sqrt(np.mean(np.array(ch)**2))
+                features[(ch* self.numFeatures)+l] = np.sqrt(np.mean(np.array(epoch[:,ch])**2))
             if self.featureChoices.variance: # variance
                 l += 1    
-                features[(k* self.numFeatures)+l] =  np.var(ch)
+                features[(ch* self.numFeatures)+l] =  np.var(epoch[:,ch])
             if self.featureChoices.meanAbs: # Mean Absolute Value 
                 l += 1
-                features[(k* self.numFeatures)+l] = sum([np.linalg.norm(c) for c in ch])/len(ch)
+                features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c) for c in epoch[:,ch]])/len(epoch[:,ch])
             #if self.featureChoices.waveformLength: # waveformLength
             #    l += 1
-            #    features[(k* self.numFeatures)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
+            #    features[(ch* self.numFeatures)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
             if self.featureChoices.zeroCross: # zeroCross
                 l += 1
-                features[(k* self.numFeatures)+l] = sum([1 if c*ch[inum+1]<0 else 0 for inum, c in enumerate(ch[:-1])])
+                features[(ch* self.numFeatures)+l] = sum([1 if c*epoch[:,ch][inum+1]<0 else 0 for inum, c in enumerate(epoch[:,ch][:-1])])
             #if self.featureChoices.slopeSignChange: # slopeSignChange
             #    l += 1    
             #    ssc = sum([1 if (c-ch[inum+1])*(c-ch[inum+1])>=0.1 else 0 for inum, c in enumerate(ch[:-1])])
-            #    features[(k* self.numFeatures)+l] = ssc
-        #features[np.isnan(features)] = 0 # checks for nans
-        #features[features == np.inf] = 0 # checks for infs
+            #    features[(ch self.numFeatures)+l] = ssc
+        features[np.isnan(features)] = 0 # checks for nans
+        features[features == np.inf] = 0#np.iinfo(np.int32).max
         #print(features)
+        if (self.logger.level == Logger.TIMING):
+            end = time.time()
+            self.logger.log(Logger.TIMING, f" Generic Feature Extraction time {end - start}")
         return features
     
 class GazeFeatureExtractor():
     def __init__(self):
         super().__init__()
 
 '''pupil channels in order
```

### Comparing `install-pybci-0.2.2b1/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.3b0/pybci/Utils/LSLScanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,16 +49,16 @@
         for stream in streams:
             if stream.type() in self.streamTypes:
                 dataStreams.append(StreamInlet(stream))
         if self.dataStreamPredefined:
             for s in dataStreams:
                 name = s.info().name()
                 if name not in self.dataStreamsNames:
-                    self.logger.log(Logger.WARNING,"Predefined LSL Data Stream name not present.")
-                    self.logger.log(Logger.WARNING, "Available Streams: "+str([s.info().name() for s in dataStreams]))
+                    self.logger.log(Logger.WARNING," Predefined LSL Data Stream name not present.")
+                    self.logger.log(Logger.WARNING, " Available Streams: "+str([s.info().name() for s in dataStreams]))
                 else:
                     self.dataStreams.append(s)
         else: # just add all datastreams as none were specified
             self.dataStreams = dataStreams
     
     def ScanMarkerStreams(self):
         """Scans available LSL streams and appends inlet to self.markerStreams"""
@@ -70,34 +70,37 @@
                 markerStreams.append(StreamInlet(stream))
         if self.markerStreamPredefined:
             if len(markerStreams) > 1:
                 self.logger.log(Logger.WARNING," Too many Marker streams available, set single desired markerStream in  bci.lslScanner.markerStream correctly.")
             for s in markerStreams:
                 name = s.info().name()
                 if name != self.markerStreamName:
-                    self.logger.log(Logger.WARNING,"Predefined LSL Marker Stream name not present.")
-                    self.logger.log(Logger.WARNING, "Available Streams: "+str([s.info().name() for s in markerStreams]))
+                    self.logger.log(Logger.WARNING," Predefined LSL Marker Stream name not present.")
+                    self.logger.log(Logger.WARNING, " Available Streams: "+str([s.info().name() for s in markerStreams]))
                 else:
                     self.markerStream = s
         else:
             if len(markerStreams) > 0:   
                 self.markerStream = markerStreams[0] # if none specified grabs first avaialble marker stream
 
     def CheckAvailableLSL(self):
         """Checks streaminlets available, 
-        Returns:
-            True = 1 marker stream present and available datastreams are present
-            False = If no datastreams are present and/or more or less then one marker stream is present, requires hard selection or markser stream if too many.
+        Returns
+        -------
+        bool :
+            True if 1 marker stream present and available datastreams are present.
+            False if no datastreams are present and/or more or less then one marker stream is present, requires hard selection or markser stream if too many.
         """
         self.ScanStreams()
         if self.markerStream == None:
-            self.logger.log(Logger.WARNING,"No Marker streams available, make sure your accepted marker data Type have been set in bci.lslScanner.markerTypes correctly.")
+            self.logger.log(Logger.WARNING," No Marker streams available, make sure your accepted marker data Type have been set in bci.lslScanner.markerTypes correctly.")
         if len(self.dataStreams) == 0:
-            self.logger.log(Logger.WARNING,"No data streams available, make sure your streamTypes have been set in bci.lslScanner.dataStream correctly.")
+            self.logger.log(Logger.WARNING," No data streams available, make sure your streamTypes have been set in bci.lslScanner.dataStream correctly.")
         if len(self.dataStreams) > 0 and self.markerStream !=None:
-            self.logger.log(Logger.INFO,"Success - "+str(len(self.dataStreams))+" data stream(s) found, 1 marker stream found")
+            self.logger.log(Logger.INFO," Success - "+str(len(self.dataStreams))+" data stream(s) found, 1 marker stream found")
+        
         if len(self.dataStreams) > 0 and self.markerStream != None:
             self.parent.dataStreams = self.dataStreams
             self.parent.markerStream = self.markerStream
             return True
         else:
             return False
```

### Comparing `install-pybci-0.2.2b1/pybci/Utils/Logger.py` & `install-pybci-0.2.3b0/pybci/Utils/Logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 class Logger:
     INFO = "info"
     WARNING = "warning"
     NONE = "none"
+    TIMING = "timing"
 
     def __init__(self, level=INFO):
         self.level = level
         self.check_level(level)
 
     def set_level(self, level):
         self.level = level
         self.check_level(level)
 
     def check_level(self,level):
-        if level != self.WARNING or level != self.INFO or level != self.NONE:
-            print("PyBCI: [WARNING] - Invalid log level selected, defaulted to info. (options: info, warning, none)")
+        if level != self.WARNING and level != self.INFO and level != self.NONE and level != self.TIMING :
+            print("PyBCI: [INFO] - Invalid or no log level selected, defaulting to info. (options: info, warning, none)")
             level = self.INFO
             self.level = level
 
     def log(self, level, message):
         if self.level == 'none':
-            return
-
+            return None
         if level == 'info':
-            if self.level != 'none':
+            if self.level != 'none' and self.level != 'warning':
                 print('PyBCI: [INFO] -' + message)
         elif level == 'warning':
-            if self.level == 'warning':
-                print('PyBCI: [WARNING] -' + message)
+            if self.level != 'none':
+                print('PyBCI: [WARNING] -' + message)
+        elif level == 'timing':
+            if self.level == 'timing':
+                print('PyBCI: [TIMING] -' + message)
```

### Comparing `install-pybci-0.2.2b1/pybci/pybci.py` & `install-pybci-0.2.3b0/pybci/pybci.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .Utils.LSLScanner import LSLScanner
 from .Utils.Logger import Logger
 from .ThreadClasses.FeatureProcessorThread import FeatureProcessorThread
 from .ThreadClasses.DataReceiverThread import DataReceiverThread
 from .ThreadClasses.AsyncDataReceiverThread import AsyncDataReceiverThread
+from .ThreadClasses.OptimisedDataReceiverThread import OptimisedDataReceiverThread
 from .ThreadClasses.MarkerThread import MarkerThread
 from .ThreadClasses.ClassifierThread import ClassifierThread
 from .Configuration.EpochSettings import GlobalEpochSettings, IndividualEpochSetting
 from .Configuration.FeatureSettings import GeneralFeatureChoices
 import queue, threading, copy
 import tensorflow as tf
 #import torch
@@ -22,54 +23,70 @@
     dataThreads = []
     streamChsDropDict= {}
     dataStreams = []
     markerStream = None
     connected = False
     epochCounts = {} # holds markers received, their target ids and number received of each
     classifierInformation = []
-
+    clf= None
+    model = None 
+    torchModel = None
     def __init__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, loggingLevel = Logger.INFO,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
                  streamCustomFeatureExtract = {},
                  minimumEpochsRequired = 10, clf= None, model = None, torchModel = None):
         """
         The PyBCI object stores data from available lsl time series data streams (EEG, pupilometry, EMG, etc.)
         and holds a configurable number of samples based on lsl marker strings.
         If no marker strings are available on the LSL the class will close and return an error.
-        Parameters:
-        dataStreams (List of strings): Allows user to set custom acceptable EEG stream definitions, if None defaults to streamTypes scan
-        markerStream (List of strings): Allows user to set custom acceptable Marker stream definitions, if None defaults to markerTypes scan
-        streamTypes (List of strings): Allows user to set custom acceptable EEG type definitions, ignored if dataStreams not None
-        markerTypes (List of strings): Allows user to set custom acceptable Marker type definitions, ignored if markerStream not None
-        loggingLevel (string): Sets PyBCI print level, ('info' prints all statements, 'warning' is only warning messages, and 'none' is no prints from PyBCI)
-        globalEpochSettings (GlobalEpochSettings): Sets global timing settings for epochs.
-        customEpochSettings (dict {marker name string:IndividualEpochSettings()}): Sets individual timing settings for epochs.
-        streamChsDropDict (dict {datastream name string: list(ints)}): Keys for dict should be respective datastreams with corresponding list of which channels to drop.
-        streamCustomFeatureExtract (dict {datastream type string: customClass()}): allows dict to be passed of datastream type with custom feature extractor class for analysing data.
-        minimumEpochsRequired (Int): minimm number of required epochs before model fitting begins, must be of each type of received markers and mroe then 1 type of marker to classify.
-        clf (ClassifierMixin): Allows custom Sklearn model to be passed.
-        model (model):Allows custom tensorflow model to be passed.
-        torchmodel ([torchModel(), torch.nn.Module] ): Currently a list where first item is torchmodel analysis function, second is torch model, check pytorch example - likely to change
+        Parameters
+        ----------
+        dataStreams: List[str] 
+            Allows user to set custom acceptable EEG stream definitions, if None defaults to streamTypes scan
+        markerStream: List[str] 
+            Allows user to set custom acceptable Marker stream definitions, if None defaults to markerTypes scan
+        streamTypes: List[str] 
+            Allows user to set custom acceptable EEG type definitions, ignored if dataStreams not None
+        markerTypes: List[str] 
+            Allows user to set custom acceptable Marker type definitions, ignored if markerStream not None
+        loggingLevel: string 
+            Sets PyBCI print level, ('info' prints all statements, 'warning' is only warning messages, and 'none' is no prints from PyBCI)
+        globalEpochSettings (GlobalEpochSettings): 
+            Sets global timing settings for epochs.
+        customEpochSettings: dict 
+            Sets individual timing settings for epochs. {markerstring1:IndividualEpochSettings(),markerstring2:IndividualEpochSettings()}
+        streamChsDropDict: dict 
+            Keys for dict should be respective datastreams with corresponding list of which channels to drop.  {datastreamstring1: list(ints), datastreamstring2: list(ints)}
+        streamCustomFeatureExtract: dict
+            Allows dict to be passed of datastream with custom feature extractor class for analysing data.  {datastreamstring1: customClass1(), datastreamstring2: customClass1(),}
+        minimumEpochsRequired: int 
+            Minimm number of required epochs before model fitting begins, must be of each type of received markers and mroe then 1 type of marker to classify.
+        clf: sklearn.base.ClassifierMixin 
+            Allows custom Sklearn model to be passed.
+        model: tf.keras.model
+            Allows custom tensorflow model to be passed.
+        torchmodel:  [torchModel(), torch.nn.Module]
+            Currently a list where first item is torchmodel analysis function, second is torch model, check pytorch example - likely to change in future updates.
         """
         self.streamCustomFeatureExtract = streamCustomFeatureExtract
         self.globalEpochSettings = globalEpochSettings
         self.customEpochSettings = customEpochSettings
         self.streamChsDropDict = streamChsDropDict
-        self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes)
         self.loggingLevel = loggingLevel
         self.logger = Logger(self.loggingLevel)
+        self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes, logger =self.logger)
         self.ConfigureMachineLearning(minimumEpochsRequired,  clf, model, torchModel) # configure first, connect second
         self.Connect()
        
     def __enter__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, loggingLevel = Logger.INFO,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
                  streamCustomFeatureExtract = {},
                  minimumEpochsRequired = 10, clf= None, model = None, torchModel = None): # with bci
         """
-        Please look at PyBCI.__init__ (same setup and description)
+        Please look at PyBCI.__init__ (same parameters, setup and description)
         """
         self.streamCustomFeatureExtract = streamCustomFeatureExtract
         self.globalEpochSettings = globalEpochSettings
         self.customEpochSettings = customEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes)
         self.loggingLevel = loggingLevel
@@ -90,34 +107,39 @@
 
     # set test and train boolean for changing  thread operation 
     def TrainMode(self):
         """
          Starts BCI training If PyBCI is connected to valid LSL data and marker streams, if not tries to scan and connect.
         """
         if self.connected:
-            self.logger.log(Logger.INFO,"Started training...")
+            self.logger.log(Logger.INFO," Started training...")
             self.trainTestEvent.set()
         else:
             self.Connect()
 
     def TestMode(self):
         """
          Starts BCI testing If PyBCI is connected to valid LSL data and marker streams, if not tries to scan and connect.
          (Need to check if invalid number of epochs are obtained and this is set)
         """
         if self.connected:
-            self.logger.log(Logger.INFO,"Started testing...")
+            self.logger.log(Logger.INFO," Started testing...")
             self.trainTestEvent.clear()
         else:
             self.Connect()
 
     # Get data from threads
     def CurrentClassifierInfo(self):
         """
-        
+        Gets dict with current clf, model, torchModel and accuracy. Accuracy will be 0 if not fiting has occurred.
+        Returns
+        -------
+        classInfo: dict
+            dict of "clf", "model, "torchModel"" and "accuracy" where accuracy is 0 if no model training/fitting has occurred. If mode not used corresponding value is None.
+            If not connected returns {"Not Connected": None}
         """
         if self.connected:
             self.classifierInfoRetrieveEvent.set()
             classInfo = self.classifierInfoQueue.get()
             self.classifierInfoRetrieveEvent.clear()
             return classInfo
         else:
@@ -125,34 +147,34 @@
             return {"Not Connected": None}
 
     def CurrentClassifierMarkerGuess(self):
         """
         Gets classifier current marker guess and targets.
         Returns
         -------
-        int
+        classGuess: int | None
             Returned int correlates to value of key from dict from ReceivedMarkerCount() when in testmode. 
             If in trainmode returns None.
         """
         if self.connected:
             # probably needs check that we're in test mode, maybe debu print if not?
             self.classifierGuessMarkerEvent.set()
             classGuess = self.classifierGuessMarkerQueue.get()
             self.classifierGuessMarkerEvent.clear()
             return classGuess
         else:
             self.Connect()
-            return {"Not Connected": None}
+            return None
 
     def CurrentFeaturesTargets(self):
         """
         Gets classifier current features and targets.
         Returns
         -------
-        dict
+        featureTargets: dict
             dict of "features" and "targets" where features is 2d list of feature data and targets is a 1d list of epoch targets as ints.
             If not connected returns {"Not Connected": None}
         """
         if self.connected:
             self.queryFeaturesEvent.set()
             featureTargets = self.queryFeaturesQueue.get()
             self.queryFeaturesEvent.clear() # still needs coding
@@ -162,17 +184,17 @@
             return {"Not Connected": None}
 
     def ReceivedMarkerCount(self):
         """
         Gets number of received training marker, their strings and their respective values to correlate with CurrentClassifierMarkerGuess().
         Returns
         -------
-        dict
+        markers: dict
             Every key is a string received on the selected LSL marker stream, the value is a list where the first item is the marker id value, 
-            use with CurrentClassifierMarkerGuess() the second value is a received count for that marker type.
+            use with CurrentClassifierMarkerGuess() the second value is a received count for that marker type. Will be empty if no markers received.
         """
         if self.connected:
             self.markerCountRetrieveEvent.set()
             markers = self.markerCountQueue.get()
             self.markerCountRetrieveEvent.clear()
             return markers
         else:
@@ -198,29 +220,38 @@
         # setup data thread
         self.dataThreads = []
         self.featureThreads = []
         for stream in self.dataStreams:
             self.dataQueueTrain = queue.Queue()
             self.dataQueueTest = queue.Queue()
 
+            #if stream.info().nominal_srate() == 0:
+            #    if stream.info().name() in self.streamChsDropDict.keys():
+            #        dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+            #                                self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
+            #    else:
+            #        dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+            #                                self.globalEpochSettings, len(self.dataThreads))
+            #else: # cold be desirable to capture samples only relative to timestammps with async, so maybe make this configurable?
             if stream.info().nominal_srate() == 0:
-                if stream.info().name() in self.streamChsDropDict.keys():
-                    dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+                if stream.info().name() in self.streamChsDropDict.keys(): ## all use optimised now (pull_chunk and timestamp relative)
+                    #print(self.streamChsDropDict[stream.info().name()])
+                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
                                             self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
                 else:
-                    dt = AsyncDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
                                             self.globalEpochSettings, len(self.dataThreads))
-            else: # cold be desirable to capture samples only relative to timestammps with async, so maybe make this configurable?
-                if stream.info().name() in self.streamChsDropDict.keys():
-                    dt = DataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()])
+            else:
+                if stream.info().name() in self.streamChsDropDict.keys(): ## all use optimised now (pull_chunk and timestamp relative)
+                    #print(self.streamChsDropDict[stream.info().name()])
+                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+                                            self.globalEpochSettings, len(self.dataThreads), streamChsDropDict=self.streamChsDropDict[stream.info().name()], maxExpectedSampleRate = stream.info().nominal_srate())
                 else:
-                    dt = DataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
-                                            self.globalEpochSettings, len(self.dataThreads))
-
+                    dt = OptimisedDataReceiverThread(self.closeEvent, self.trainTestEvent, self.dataQueueTrain,self.dataQueueTest, stream,  self.customEpochSettings, 
+                                            self.globalEpochSettings, len(self.dataThreads),maxExpectedSampleRate = stream.info().nominal_srate())
             dt.start()
             self.dataThreads.append(dt)
             if stream.info().name() in self.streamCustomFeatureExtract.keys():
                 self.ft = FeatureProcessorThread(self.closeEvent,self.trainTestEvent, self.dataQueueTrain, self.dataQueueTest,
                                                 self.featureQueueTest,self.featureQueueTrain, len(self.dataStreams),
                                                 self.markerCountRetrieveEvent, self.markerCountQueue,
                                                 featureExtractor = self.streamCustomFeatureExtract[stream.info().name()],
@@ -234,16 +265,16 @@
             self.featureThreads.append(dt)
         # marker thread requires data and feature threads to push new markers too
         self.markerThread = MarkerThread(self.closeEvent,self.trainTestEvent, self.markerStream,self.dataThreads, self.featureThreads)
         self.markerThread.start()
         self.classifierThread = ClassifierThread(self.closeEvent,self.trainTestEvent, self.featureQueueTest,self.featureQueueTrain,
                                                  self.classifierInfoQueue, self.classifierInfoRetrieveEvent,
                                                  self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, self.queryFeaturesQueue, self.queryFeaturesEvent,
-                                                 self.logger,len(self.dataThreads),
-                                                self.minimumEpochsRequired, clf = self.clf, model = self.model, torchModel = self.torchModel)
+                                                 logger = self.logger, numStreamDevices = len(self.dataThreads), minRequiredEpochs = self.minimumEpochsRequired,
+                                                clf = self.clf, model = self.model, torchModel = self.torchModel)
         self.classifierThread.start()
 
     def StopThreads(self):
         """
         Stops all PyBCI threads.
         """
         self.closeEvent.set()
@@ -256,15 +287,15 @@
         self.classifierThread.join()
         self.connected = False
         self.logger.log(Logger.INFO," Threads stopped.")
 
     def ConfigureMachineLearning(self, minimumEpochsRequired = 10, clf = None, model = None, torchModel = None):
         from sklearn.base import ClassifierMixin
         self.minimumEpochsRequired = minimumEpochsRequired
-
+        
         if isinstance(clf, ClassifierMixin):
             self.clf = clf
         else:
             self.clf = None
             self.logger.log(Logger.INFO," Invalid or no sklearn classifier passed to clf. Checking tensorflow model... ")
             if isinstance(model, tf.keras.Model):
                 self.model = model
@@ -276,15 +307,17 @@
                 else:
                     self.torchModel = None
                     self.logger.log(Logger.INFO," Invalid or no PyTorch model passed to model. Defaulting to SVM by SkLearn")
     
 
     # Could move all configures to a configuration class, might make options into more descriptive classes?
     def ConfigureEpochWindowSettings(self, globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}):
-        """allows globalWindowSettings to be modified, customWindowSettings is a dict with value names for marker strings which will appear on avalable markerStreams """
+        """
+        Allows globalWindowSettings to be modified, customWindowSettings is a dict with value names for marker strings which will appear on avalable markerStreams. 
+        """
         valid = False
         for key in customEpochSettings.keys():
             if isinstance(customEpochSettings[key], IndividualEpochSetting):
                 valid = True
             else:
                 valid = False
                 self.logger.log(Logger.WARNING," Invalid datatype passed for customWindowSettings, create dict of wanted markers \
```

### Comparing `install-pybci-0.2.2b1/setup.py` & `install-pybci-0.2.3b0/setup.py`

 * *Files identical despite different names*

