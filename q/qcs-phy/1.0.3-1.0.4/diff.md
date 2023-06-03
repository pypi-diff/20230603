# Comparing `tmp/qcs_phy-1.0.3.tar.gz` & `tmp/qcs_phy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcs_phy-1.0.3.tar", last modified: Fri Jun  2 03:01:41 2023, max compression
+gzip compressed data, was "qcs_phy-1.0.4.tar", last modified: Sat Jun  3 18:36:35 2023, max compression
```

## Comparing `qcs_phy-1.0.3.tar` & `qcs_phy-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 03:01:41.112188 qcs_phy-1.0.3/
--rw-rw-rw-   0        0        0     1011 2023-06-02 03:01:41.111119 qcs_phy-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 03:01:41.106132 qcs_phy-1.0.3/qcs_phy/
--rw-rw-rw-   0        0        0    55725 2023-06-02 02:51:05.000000 qcs_phy-1.0.3/qcs_phy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 03:01:41.110122 qcs_phy-1.0.3/qcs_phy.egg-info/
--rw-rw-rw-   0        0        0     1011 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-02 03:01:41.000000 qcs_phy-1.0.3/qcs_phy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 03:01:40.000000 qcs_phy-1.0.3/qcs_phy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 03:01:41.112188 qcs_phy-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1696 2023-06-02 03:01:19.000000 qcs_phy-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 18:36:35.727476 qcs_phy-1.0.4/
+-rw-rw-rw-   0        0        0     1011 2023-06-03 18:36:35.727476 qcs_phy-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 18:36:35.722489 qcs_phy-1.0.4/qcs_phy/
+-rw-rw-rw-   0        0        0    56060 2023-06-03 18:35:52.000000 qcs_phy-1.0.4/qcs_phy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 18:36:35.726478 qcs_phy-1.0.4/qcs_phy.egg-info/
+-rw-rw-rw-   0        0        0     1011 2023-06-03 18:36:35.000000 qcs_phy-1.0.4/qcs_phy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-06-03 18:36:35.000000 qcs_phy-1.0.4/qcs_phy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 18:36:35.000000 qcs_phy-1.0.4/qcs_phy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-03 18:36:35.000000 qcs_phy-1.0.4/qcs_phy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 18:36:35.000000 qcs_phy-1.0.4/qcs_phy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 18:36:35.727476 qcs_phy-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1696 2023-06-03 18:31:11.000000 qcs_phy-1.0.4/setup.py
```

### Comparing `qcs_phy-1.0.3/PKG-INFO` & `qcs_phy-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs_phy
-Version: 1.0.3
+Version: 1.0.4
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.3/qcs_phy/__init__.py` & `qcs_phy-1.0.4/qcs_phy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -962,58 +962,68 @@
                 return G[0, 0]
 
         elif label == -4:  # many-to-many-different
             print("This function is not yet available")
         else:  # many-to-many-same
             print("This function is not yet available")
 
-    def calculate_2nd_uETCF(self, channel_name: str, tau=0, zp=0):
+    def calculate_2nd_uETCF(self, Quantity: str, tau=0, zp=0):
         """Calculating the 2nd-order unequal-time coreelation function . For example,
                 \-----------------------------------------------------------------------------------------------\
-                channel_name = "c1" ==>
+                Quantity = "c1c1" ==>
 
                 g^{(2)}(\\\ tau) = <c1^{\\\dagger}(0)c1^{\\\dagger}(\\\ tau)c1(\\\ tau) c1(0)> / <c1^{\\\dagger} c1>^2
 
                 \-----------------------------------------------------------------------------------------------\
-                :param channel_name: the name of output channel
+                :param Quantity: physical quantity
                 :param tau: the delay time
                 :param zp: an infinitely small quantity
                 :return: the 2nd-order unequal-time coreelation function (uETCF)
         """
         inv, abs, expm = nlg.inv, np.abs, slg.expm  # Assign to a local variable
-        key_out = [channel_name for _ in range(2)]
+        photons = {}
+        for mode in self.__Output.keys():
+            photons[mode] = Quantity.count(mode)
+        key_out = [key for key in photons for _ in range(photons[key])]
         label = self.__classification(key_out)
+        if len(set(key_out)) == 1:
+            key_out = key_out[0]
         self.__excitation_number()
         if self.__Heff_v != qcs.__Judge_Heff:
-            qcs.__BasisList.clear()
+            qcs.__HeffList.clear()
             qcs.__Judge_Heff = self.__Heff_v
             qcs.__Judge_InOut = dict(self.__Input, **self.__Output)
             for n in range(0, 3):
                 self.__basis(n)
                 if n != 0:
                     self.__prestore_HeffList(n)
                     self.__prestore_InOutList(n)
         elif compare_dicts(self.__Input, qcs.__Judge_InOut) and compare_dicts(self.__Output, qcs.__Judge_InOut):
             pass
         else:
+            qcs.__InOutList.clear()
             qcs.__Judge_InOut = dict(self.__Input, **self.__Output)
             for n in range(1, 3):
                 self.__prestore_InOutList(n)
         for n in range(1, 3):
-            if n not in list(qcs.__BasisList.keys()):
+            if n not in list(qcs.__HeffList.keys()):
                 self.__basis(n)
                 self.__prestore_HeffList(n)
                 self.__prestore_InOutList(n)
+            elif n not in list(qcs.__InOutList.keys()):
+                self.__basis(n)
+                self.__prestore_InOutList(n)
             else:
                 pass
+
         if label == -1:  # one-to-one-differnt
             key_in = list(self.__Input.keys())[0]
             ome = self.__Frequency[key_in]
             B = [self.__Input_Matrix(n)[key_in].conj().T for n in range(1, 3)]
-            C = [self.__Output_Matrix(n)[channel_name] for n in range(1, 3)]
+            C = [self.__Output_Matrix(n)[key_out] for n in range(1, 3)]
             I = [np.eye(qcs.__Dim[n]) for n in range(1, 3)]
             Heff = [self.__Heff_Matrix(n) - (n * ome + zp) * I[n - 1] for n in range(1, 3)]
             P1 = C[0] @ inv(Heff[0]) @ B[0]
             P1_R = inv(Heff[0]) @ B[0]
             P2_R = C[1] @ inv(Heff[1]) @ B[1] @ P1_R
             if type(tau) not in number_type:
                 g2_t = []
@@ -1026,15 +1036,15 @@
                 P1_t = expm(-1j * Heff[0] * abs(tau))
                 return (abs(P1 ** 2 + C[0] @ P1_t @ P2_R - C[0] @ P1_t @ P1_R * P1) ** 2 / abs(P1) ** 4)[0, 0]
 
         elif label == 1:  # one-to-one-same
             key_in = list(self.__Input.keys())[0]
             ome = self.__Frequency[key_in]
             B = [self.__Input_Matrix(n)[key_in].conj().T for n in range(1, 3)]
-            C = [self.__Output_Matrix(n)[channel_name] for n in range(1, 3)]
+            C = [self.__Output_Matrix(n)[key_out] for n in range(1, 3)]
             I = [np.eye(qcs.__Dim[n]) for n in range(1, 3)]
             Heff = [self.__Heff_Matrix(n) - (n * ome + zp) * I[n - 1] for n in range(1, 3)]
             P1 = C[0] @ inv(Heff[0]) @ B[0]
             P1_R = inv(Heff[0]) @ B[0]
             P2_R = C[1] @ inv(Heff[1]) @ B[1] @ P1_R
             if type(tau) not in number_type:
                 g2_t = []
@@ -1047,15 +1057,15 @@
                 P1_t = expm(-1j * Heff[0] * abs(tau))
                 return (abs((1 + 1j * P1) ** 2 - C[0] @ P1_t @ P2_R + C[0] @ P1_t @ P1_R * P1) ** 2 / abs(1 + 1j * P1) ** 4)[0, 0]
 
         elif label == -2:  # many-to-one-differnt
             key_in = list(self.__Input.keys())
             ome = list(self.__Frequency.values())[0]
             B = [sum([self.__ratio[key] * self.__Input_Matrix(n)[key].conj().T for key in key_in]) for n in range(1, 3)]
-            C = [self.__Output_Matrix(n)[channel_name] for n in range(1, 3)]
+            C = [self.__Output_Matrix(n)[key_out] for n in range(1, 3)]
             I = [np.eye(qcs.__Dim[n]) for n in range(1, 3)]
             Heff = [self.__Heff_Matrix(n) - (n * ome + zp) * I[n - 1] for n in range(1, 3)]
             P1 = C[0] @ inv(Heff[0]) @ B[0]
             P1_R = inv(Heff[0]) @ B[0]
             P2_R = C[1] @ inv(Heff[1]) @ B[1] @ P1_R
             if type(tau) not in number_type:
                 g2_t = []
@@ -1068,21 +1078,21 @@
                 P1_t = expm(-1j * Heff[0] * abs(tau))
                 return (abs(P1 ** 2 + C[0] @ P1_t @ P2_R - C[0] @ P1_t @ P1_R * P1) ** 2 / abs(P1) ** 4)[0, 0]
 
         elif label == 2:  # many-to-one-same
             key_in = list(self.__Input.keys())
             ome = list(self.__Frequency.values())[0]
             B = [sum([self.__ratio[key] * self.__Input_Matrix(n)[key].conj().T for key in key_in]) for n in range(1, 3)]
-            C = [self.__Output_Matrix(n)[channel_name] for n in range(1, 3)]
+            C = [self.__Output_Matrix(n)[key_out] for n in range(1, 3)]
             I = [np.eye(qcs.__Dim[n]) for n in range(1, 3)]
             Heff = [self.__Heff_Matrix(n) - (n * ome + zp) * I[n - 1] for n in range(1, 3)]
             P1 = C[0] @ inv(Heff[0]) @ B[0]
             P1_R = inv(Heff[0]) @ B[0]
             P2_R = C[1] @ inv(Heff[1]) @ B[1] @ P1_R
-            ratio_c = self.__ratio[channel_name]
+            ratio_c = self.__ratio[key_out]
             if type(tau) not in number_type:
                 g2_t = []
                 append = g2_t.append
                 for t in tau:
                     P1_t = expm(-1j * Heff[0] * abs(t))
                     append((abs((ratio_c + 1j * P1) ** 2 - C[0] @ P1_t @ P2_R + C[0] @ P1_t @ P1_R * P1) ** 2 / abs(ratio_c + 1j * P1) ** 4)[0, 0])
                 return g2_t
```

### Comparing `qcs_phy-1.0.3/qcs_phy.egg-info/PKG-INFO` & `qcs_phy-1.0.4/qcs_phy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs-phy
-Version: 1.0.3
+Version: 1.0.4
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.3/setup.py` & `qcs_phy-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # # these things are needed for the README.md show on pypi
 # here = os.path.abspath(os.path.dirname(__file__))
 #
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'QCS: Quantum Correlation Solver'
 LONG_DESCRIPTION = 'QCS is an open-source Python code that allows to study the single-photon transmission and reflection, ' \
                    'as well as the nth-order equal-time correlation functions (ETCFs) in driven-dissipative quantum systems.'
 REQUIRES = ['numpy (>=1.8)', 'scipy (>=0.15)']
 INSTALL_REQUIRES = ['numpy>=1.8', 'scipy>=0.15']
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "quantum physics higher-order equal-time correlation function"
```

