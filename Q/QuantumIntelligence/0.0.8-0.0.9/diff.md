# Comparing `tmp/QuantumIntelligence-0.0.8.tar.gz` & `tmp/QuantumIntelligence-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumIntelligence-0.0.8.tar", last modified: Mon May 15 01:27:36 2023, max compression
+gzip compressed data, was "QuantumIntelligence-0.0.9.tar", last modified: Sat Jun  3 00:31:03 2023, max compression
```

## Comparing `QuantumIntelligence-0.0.8.tar` & `QuantumIntelligence-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.260228 QuantumIntelligence-0.0.8/
--rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1763 2023-05-15 01:27:36.260228 QuantumIntelligence-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-15 01:27:36.260228 QuantumIntelligence-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     8844 2023-05-15 01:27:15.000000 QuantumIntelligence-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.173317 QuantumIntelligence-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.180697 QuantumIntelligence-0.0.8/src/QuantumIntelligence/
-drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.231709 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/
--rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
--rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/__init__.py
--rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
--rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
--rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.253903 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/
--rw-rw-rw-   0        0        0    49591 2023-05-15 01:21:09.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Circuit.py
--rw-rw-rw-   0        0        0     9960 2023-04-28 05:24:32.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Gate.py
--rw-rw-rw-   0        0        0    18277 2023-05-04 19:49:53.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Simulator.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.259991 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/
--rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/MPSclass.py
--rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TEBD.py
--rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TNclass.py
--rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/__init__.py
--rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 01:27:36.203683 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/
--rw-rw-rw-   0        0        0     1763 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      977 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-15 01:27:36.000000 QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 00:31:03.304450 QuantumIntelligence-0.0.9/
+-rw-rw-rw-   0        0        0    35149 2022-08-31 04:58:38.000000 QuantumIntelligence-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1763 2023-06-03 00:31:03.304450 QuantumIntelligence-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      911 2022-10-04 09:52:33.000000 QuantumIntelligence-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 00:31:03.304450 QuantumIntelligence-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     8854 2023-06-03 00:26:35.000000 QuantumIntelligence-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:31:03.241655 QuantumIntelligence-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 00:31:03.251352 QuantumIntelligence-0.0.9/src/QuantumIntelligence/
+drwxrwxrwx   0        0        0        0 2023-06-03 00:31:03.284068 QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/
+-rw-rw-rw-   0        0        0     1393 2023-04-25 03:54:04.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py
+-rw-rw-rw-   0        0        0     7075 2023-04-25 12:46:20.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/__init__.py
+-rw-rw-rw-   0        0        0     3648 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py
+-rw-rw-rw-   0        0        0     1607 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py
+-rw-rw-rw-   0        0        0     5084 2022-10-20 02:41:17.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:31:03.294804 QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/
+-rw-rw-rw-   0        0        0    50619 2023-05-24 08:16:22.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/Circuit.py
+-rw-rw-rw-   0        0        0    10422 2023-05-26 07:07:27.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/Gate.py
+-rw-rw-rw-   0        0        0    20534 2023-05-29 12:16:02.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/Simulator.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:31:03.301714 QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/
+-rw-rw-rw-   0        0        0     4335 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/MPSclass.py
+-rw-rw-rw-   0        0        0    13521 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/TEBD.py
+-rw-rw-rw-   0        0        0     1023 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/TNclass.py
+-rw-rw-rw-   0        0        0        0 2022-10-06 02:25:06.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-10-04 10:08:04.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 00:31:03.261046 QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/
+-rw-rw-rw-   0        0        0     1763 2023-06-03 00:31:03.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      977 2023-06-03 00:31:03.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 00:31:03.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-03 00:31:03.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-03 00:31:03.000000 QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/top_level.txt
```

### Comparing `QuantumIntelligence-0.0.8/LICENSE` & `QuantumIntelligence-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/PKG-INFO` & `QuantumIntelligence-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.8
+Version: 0.0.9
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.8/README.md` & `QuantumIntelligence-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/setup.py` & `QuantumIntelligence-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     name="QuantumIntelligence",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.0.8",  # Required
+    version="0.0.9",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Developing quantum intelligence.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -124,15 +124,15 @@
     python_requires=">=3.7, <4",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
-    install_requires=["torch", "numpy", "scipy", "matplotlib", "pynvml", "stim"],  # Optional
+    install_requires=["torch", "numpy", "scipy", "matplotlib", "pynvml", "stim", "qiskit"],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
```

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/BasicClass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/BasicFunctions_szz.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/physical_fun.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/tensor_trick.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/BasicFunSZZ/wheel_function.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Circuit.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/Circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from QuantumIntelligence.QuantumSimulator import Gate
 from QuantumIntelligence.BasicFunSZZ import tensor_trick as tt
 from cirq.contrib.qasm_import import circuit_from_qasm
 from cirq.circuits.qasm_output import QasmUGate
 from qiskit.quantum_info import Operator
 
 
+
 # [1, 0] is |0>, [0, 1] is |1>
 # do not use fake functions, it will be removed soon
 # please apply gate on position as list(range(?)) as much as possible, this will make it faster
 # please control gate on position as list(range(?, n_qubit)) as much as possible, this will make it faster
 
 class Circuit:
 
@@ -48,14 +49,15 @@
         if qubit_position is None:
             self.qubit_position = list()
             for ii in range(self.n_qubit):
                 self.qubit_position.append((ii // self.size[1], ii % self.size[1]))
         else:
             self.qubit_position = qubit_position
 
+
     @property
     def requires_grad(self):
         flag = list()
         for gg in self.gate_list:
             flag.append(gg.requires_grad)
         return flag
 
@@ -106,15 +108,15 @@
                     new_c.append(position[oo])
                 for oo in control:
                     new_c.append(oo)
                 self.append(gate=cc[0], position=new_p.copy(), control=new_c.copy())
         else:
             raise ValueError('error in extend, check position')
 
-    def add_single_gate(self, gate: Gate, position, control=None, inverse=False):
+    def add_single_gate(self, gate:Gate, position, control=None, inverse=False):
         # gate can be sparse, but there seems to be no speedup
         # one should be careful when add inverse gates
         # the gate will be cloned and detached by default
 
         # do not change the following code, or some bugs would occur in circuit.ch
         gate = Gate.Gate(gate, independent=True)
         # gate = Gate.Gate(gate, independent=True).to(self.device).to(self.dtype)
@@ -196,19 +198,25 @@
         self.position_list.pop(index)
         self.control_list.pop(index)
 
     def clear(self):
         while len(self) > 0:
             self.pop(0)
 
+
     def add_noise_gate(self, strength=0.01):
-        for ii in range(len(self)):
-            if self.control_list[ii] is not None:
-                tmp_noise = Gate.noise_gate_single_gaussian(strength=strength, device=self.device, dtype=self.dtype)
-                self.gate_list[ii].tensor = self.gate_list[ii].tensor.mm(tmp_noise.tensor)
+        old_circuit = copy.deepcopy(self)
+        self.clear()
+        for ii in range(len(old_circuit)):
+            self.append(old_circuit.gate_list[ii], old_circuit.position_list[ii], old_circuit.control_list[ii])
+            combined_position = old_circuit.position_list[ii] + old_circuit.control_list[ii]
+            if len(combined_position) > 0:
+                for pp in combined_position:
+                    tmp_noise = Gate.noise_gate_single_gaussian(strength=strength, device=self.device, dtype=self.dtype)
+                    self.append(gate=tmp_noise, position=[pp])
 
     def cal_barrier(self):
         self.regularize_all_position()
         position_list = list(range(self.n_qubit))
         flag = False
         for ii in range(len(self)):
             for nn in self.position_list[ii]:
@@ -270,19 +278,20 @@
                         if nn in index_list_strict:
                             index_list_strict.remove(nn)
                     ii = ii + 1
         self.gate_list = new_gate_list
         self.position_list = new_position_list
         self.control_list = new_control_list
 
-    def map_qubits(self, qubit_map: dict):
+    def map_qubits(self, qubit_map:dict):
         for ii in range(len(self)):
             self.position_list[ii] = [qubit_map[pp] for pp in self.position_list[ii]]
             self.control_list[ii] = [qubit_map[pp] for pp in self.control_list[ii]]
         self.qubit_position = [self.qubit_position[ii] for ii in qubit_map.keys()]
+        self.n_qubit = len(qubit_map.keys())
 
     def using_qubits(self):
         using_qubits = list()
         for _, position, control in self:
             using_qubits.extend(position)
             using_qubits.extend(control)
         using_qubits = sorted(list(set(using_qubits)))
@@ -351,171 +360,172 @@
                 elif len(tmp_control) == 1:
                     raise ValueError('Waiting to support controlled ', tmp_label)
             elif tmp_label in supported_label:
                 if tmp_label == 'Z':
                     if len(tmp_control) == 0:
                         self.rz_gate(position=tmp_position, theta=np.pi)
                     elif len(tmp_control) == 1:
-                        self.cz_gate(position=[tmp_position + tmp_control])
+                        self.cz_gate(position=[tmp_position+tmp_control])
                 elif tmp_label == 'X':
                     if len(tmp_control) == 0:
                         self.rx_gate(position=tmp_position, theta=np.pi)
                     elif len(tmp_control) == 1:
                         self.rz_gate(position=tmp_position, theta=np.pi)
-                        self.ry_gate(position=tmp_position, theta=np.pi / 2)
-                        self.cz_gate(position=[tmp_position + tmp_control])
+                        self.ry_gate(position=tmp_position, theta=np.pi/2)
+                        self.cz_gate(position=[tmp_position+tmp_control])
                         self.ry_gate(position=tmp_position, theta=-np.pi / 2)
                         self.rz_gate(position=tmp_position, theta=-np.pi)
                 elif tmp_label == 'Y':
                     if len(tmp_control) == 0:
                         self.ry_gate(position=tmp_position, theta=np.pi)
                     elif len(tmp_control) == 1:
-                        self.rz_gate(position=tmp_position, theta=-np.pi / 2)
-                        self.ry_gate(position=tmp_position, theta=-np.pi / 2)
-                        self.cz_gate(position=[tmp_position + tmp_control])
-                        self.ry_gate(position=tmp_position, theta=np.pi / 2)
-                        self.rz_gate(position=tmp_position, theta=np.pi / 2)
+                        self.rz_gate(position=tmp_position, theta=-np.pi/2)
+                        self.ry_gate(position=tmp_position, theta=-np.pi/2)
+                        self.cz_gate(position=[tmp_position+tmp_control])
+                        self.ry_gate(position=tmp_position, theta=np.pi/2)
+                        self.rz_gate(position=tmp_position, theta=np.pi/2)
                 elif tmp_label == 'H':
                     if len(tmp_control) > 1:
                         raise ValueError('Do not support controlled ', tmp_label)
                     self.rz_gate(position=tmp_position, theta=np.pi)
-                    self.ry_gate(position=tmp_position, theta=np.pi / 2)
+                    self.ry_gate(position=tmp_position, theta=np.pi/2)
                 else:
                     raise ValueError('tired')
             else:
                 raise ValueError('The unsupported label is', tmp_label)
 
     def cancel_rz_clifford_exp(self):
         rz_index = len(self) - 1
-        while rz_index >= 0:
+        while rz_index >=0:
             if self.gate_list[rz_index].label[0] == 'RZ':
                 walk_index = rz_index
                 walk_label = self.gate_list[walk_index].label
                 walk_position = self.position_list[walk_index][0]
                 self.pop(walk_index)
                 while walk_index > 0:
                     check_index = walk_index - 1
-                    if walk_position in self.position_list[check_index]:
+                    if  walk_position in self.position_list[check_index]:
                         check_label = self.gate_list[check_index].label
                         if check_label == 'CZ':
                             pass
                         elif check_label[0] == 'RZ':
                             new_theta = walk_label[1] + check_label[1]
-                            new_theta = ((new_theta / np.pi) % 2) * np.pi
+                            new_theta = ((new_theta/np.pi) % 2) * np.pi
                             walk_label = ('RZ', new_theta)
                             self.pop(check_index)
                             walk_index = walk_index - 1
                             rz_index = rz_index - 1
-                            if ((new_theta / np.pi) % 2) == 0:
+                            if ((new_theta/np.pi) % 2) == 0:
                                 walk_index = -1
-                        elif check_label[0] == 'RX':
-                            if np.isclose((walk_label[1] / np.pi) % 2, 0.5):
+                        elif check_label[0] =='RX':
+                            if np.isclose((walk_label[1]/np.pi) % 2, 0.5):
                                 self.gate_list[check_index] = Gate.ry_gate(theta=check_label[1])
-                            elif np.isclose((walk_label[1] / np.pi) % 2, 1):
+                            elif np.isclose((walk_label[1]/np.pi) % 2, 1):
                                 self.gate_list[check_index] = Gate.rx_gate(theta=-check_label[1])
-                            elif np.isclose((walk_label[1] / np.pi) % 2, 1.5):
+                            elif np.isclose((walk_label[1]/np.pi) % 2, 1.5):
                                 self.gate_list[check_index] = Gate.ry_gate(theta=-check_label[1])
                             else:
-                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1] / np.pi)
-                        elif check_label[0] == 'RY':
-                            if (walk_label[1] / np.pi) % 2 == 0.5:
+                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1]/np.pi)
+                        elif check_label[0] =='RY':
+                            if (walk_label[1]/np.pi) % 2 == 0.5:
                                 self.gate_list[check_index] = Gate.rx_gate(theta=-check_label[1])
-                            elif (walk_label[1] / np.pi) % 2 == 1:
+                            elif (walk_label[1]/np.pi) % 2 == 1:
                                 self.gate_list[check_index] = Gate.ry_gate(theta=-check_label[1])
-                            elif (walk_label[1] / np.pi) % 2 == 1.5:
+                            elif (walk_label[1]/np.pi) % 2 == 1.5:
                                 self.gate_list[check_index] = Gate.rx_gate(theta=check_label[1])
                             else:
-                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1] / np.pi)
+                                raise ValueError('tired', 'walk_label[1]/np.pi is', walk_label[1]/np.pi)
                         else:
                             raise ValueError('tired')
                     walk_index = walk_index - 1
             rz_index = rz_index - 1
         self.to(self.device).to(self.dtype)
 
     def cancel_rxy_clifford_exp(self):
         rxy_index = len(self) - 1
-        while rxy_index > 0:
+        while rxy_index >0:
             if self.gate_list[rxy_index].label[0] in ('RX', 'RY'):
                 walk_index = rxy_index
                 walk_label = self.gate_list[walk_index].label
                 walk_position = self.position_list[walk_index][0]
-                if (walk_label[1] / np.pi) % 2 == 0:
+                if (walk_label[1]/np.pi) % 2 ==0:
                     walk_index = -1
                 while walk_index > 0:
                     check_index = walk_index - 1
-                    if walk_position in self.position_list[check_index]:
+                    if  walk_position in self.position_list[check_index]:
                         check_label = self.gate_list[check_index].label
                         if check_label == 'CZ':
                             walk_index = 1
                         elif check_label[0] == 'RZ':
                             raise ValueError('cancel rz first')
                         elif check_label[0] == walk_label[0]:
                             new_theta = walk_label[1] + check_label[1]
-                            new_theta = ((new_theta / np.pi) % 2) * np.pi
+                            new_theta = ((new_theta/np.pi) % 2) * np.pi
                             walk_label = (walk_label[0], new_theta)
                             self.pop(check_index)
                             rxy_index = rxy_index - 1
-                            if ((new_theta / np.pi) % 2) == 0:
+                            if ((new_theta/np.pi) % 2) == 0:
                                 walk_index = -1
                         elif check_label[0] in ('RX', 'RY'):
-                            if (check_label[1] / np.pi) % 2 == 0:
+                            if (check_label[1]/np.pi) % 2 == 0:
                                 self.pop(check_index)
                                 walk_index = walk_index - 1
                                 rxy_index = rxy_index - 1
-                            elif (check_label[1] / np.pi) % 2 == 1:
+                            elif (check_label[1]/np.pi) % 2 == 1:
                                 walk_label = (walk_label[0], -walk_label[1])
                             else:
-                                if (walk_label[1] / np.pi) % 2 == 1:
-                                    self.gate_list[check_index] = Gate.r_gate(theta=-check_label[1],
-                                                                              label=check_label[0])
+                                if (walk_label[1]/np.pi) % 2 == 1:
+                                    self.gate_list[check_index] = Gate.r_gate(theta=-check_label[1], label=check_label[0])
                                 else:
                                     walk_index = 1
                         else:
                             raise ValueError('tired')
                     walk_index = walk_index - 1
                 if walk_index <= 0:
                     self.pop(rxy_index)
-                if walk_index == 0:
+                if walk_index  == 0:
                     self.gate_list.insert(check_index + 1, Gate.r_gate(theta=walk_label[1], label=walk_label[0]))
                     self.position_list.insert(check_index + 1, [walk_position])
                     self.control_list.insert(check_index + 1, [])
             rxy_index = rxy_index - 1
         self.to(self.device).to(self.dtype)
-
+            
     def cancel_xyz_surface_code_abandoned(self):
         walk_index = 0
         xyz_list = ['X', 'Y', 'Z']
         rxyz_list = ['RX', 'RY', 'RZ']
         while walk_index < len(self):
             pop_flag = False
             tmp_label = self.gate_list[walk_index].label
             tmp_control = self.control_list[walk_index]
             if tmp_label in xyz_list:
                 if len(tmp_control) == 0:
                     pop_flag = True
             elif tmp_label[0] in rxyz_list:
                 if len(tmp_control) == 0:
-                    if (tmp_label[1] / np.pi) % 1 == 0:
+                    if (tmp_label[1]/np.pi) % 1 == 0:
                         pop_flag = True
 
             if pop_flag:
                 self.pop(walk_index)
             else:
                 walk_index = walk_index + 1
         self.to(self.device).to(self.dtype)
 
+
     # useful gates and circuits
 
     def labelled_gate(self, name, position, control=None, params=None):
         tmp_gate = Gate.labelled_simple_gate(name=name, params=params)
         for pp in position:
             if not isinstance(pp, list):
                 pp = [pp]
             self.add_single_gate(tmp_gate, position=pp, control=control)
 
+
     def x_gate(self, position, control=None):
         tmp_gate = Gate.x_gate()
         for pp in position:
             self.add_single_gate(tmp_gate, position=[pp], control=control)
 
     def y_gate(self, position, control=None):
         tmp_gate = Gate.y_gate()
@@ -560,26 +570,23 @@
     def time_evolution(self, hamiltonian, time, position, control=None):
         tmp_gate = Gate.time_evolution(hamiltonian, time, device=self.device, dtype=self.dtype)
         self.add_single_gate(tmp_gate, position=position, control=control)
 
     def qft(self, position, control=None, inverse=False):
         if control is None:
             control = []
-        tmp_circuit = qft(self.n_qubit, position=position, control=control, inverse=inverse, device=self.device,
-                          dtype=self.dtype)
+        tmp_circuit = qft(self.n_qubit, position=position, control=control, inverse=inverse, device=self.device, dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def ch(self, unitary, position_phi, position_c, control=None, inverse=False):
-        tmp_circuit = ch(self.n_qubit, unitary, position_phi, position_c, control, inverse, device=self.device,
-                         dtype=self.dtype)
+        tmp_circuit = ch(self.n_qubit, unitary, position_phi, position_c, control, inverse, device=self.device, dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def qpe(self, unitary, position_phi, position_qpe, control=None, inverse=False):
-        tmp_circuit = qpe(self.n_qubit, unitary, position_phi, position_qpe, control, inverse, device=self.device,
-                          dtype=self.dtype)
+        tmp_circuit = qpe(self.n_qubit, unitary, position_phi, position_qpe, control, inverse, device=self.device, dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def add_one(self, position=None, control=None, inverse=False):
         tmp_circuit = add_one(self.n_qubit, position, control, inverse, device=self.device, dtype=self.dtype)
         self.__extend(tmp_circuit)
 
     def qhc(self, unitary, position_phi, position_qpe, position_f, n_f=None,
@@ -701,25 +708,28 @@
                         qiskit_circuit.cu(*theta, gamma=theta3, control_qubit=c_position, target_qubit=q_position)
                     else:
                         raise ValueError('tired')
             else:
                 raise ValueError('Do not support the label of', str(ii), 'th gate, which is', old_label)
         return qiskit_circuit
 
+
     def to_qasm(self):
         # this is achieved by qiskit
         qiskit_circuit = self.to_qiskit()
         qasm_circuit = qiskit_circuit.qasm()
         return qasm_circuit
-
+    
+    
     def to_tensor(self):
         qiskit_circuit = self.to_qiskit()
         out_tensor = Operator(qiskit_circuit.reverse_bits()).data
         out_tensor = tc.from_numpy(out_tensor).to(self.device).to(self.dtype)
         return out_tensor
+        
 
     def from_qasm(self, qasm_circuit, replace=False, from_file=False):
         if from_file:
             qiskit_circuit = qiskit.QuantumCircuit.from_qasm_file(qasm_circuit)
         else:
             qiskit_circuit = qiskit.QuantumCircuit.from_qasm_str(qasm_circuit)
         circuit = self.from_qiskit(qiskit_circuit=qiskit_circuit, replace=replace)
@@ -780,33 +790,34 @@
             return circuit
 
     def positive_theta(self):
         for ii in range(len(self)):
             old_label = self.gate_list[ii].label
             if old_label[0] in ('RX', 'RY', 'RZ'):
                 while self.gate_list[ii].label[1] <= 0:
-                    self.gate_list[ii].label = (old_label[0], self.gate_list[ii].label[1] + 4 * np.pi)
+                    self.gate_list[ii].label = (old_label[0], self.gate_list[ii].label[1] + 4*np.pi)
+
 
     def zx_optimize(self, replace=False):
         self.positive_theta()
         qiskit_circuit = self.to_qiskit()
         zx_circuit = zx.Circuit.from_qasm(self.to_qasm())
         # print(zx_circuit)
         new_zx_circuit = zx.optimize.basic_optimization(zx_circuit.split_phase_gates(), do_swaps=False)
         # new_zx_circuit = zx_circuit
         new_qasm_circuit = new_zx_circuit.to_qasm()
         new_qiskit_circuit = qiskit.QuantumCircuit.from_qasm_str(new_qasm_circuit)
-        new_qiskit_circuit = qiskit.transpile(new_qiskit_circuit, basis_gates=['cz', 'rx', 'rz'], optimization_level=3)
+        new_qiskit_circuit = qiskit.transpile(new_qiskit_circuit,basis_gates=['cz', 'rx', 'rz'],optimization_level=3)
         circuit = self.from_qiskit(new_qiskit_circuit, replace=True)
         # circuit = self.from_qasm(new_qasm_circuit, replace=replace)
         if not replace:
             return circuit
 
     def qiskit_transpile(self, replace=True, **kwargs):
-        qiskit_circuit = qiskit.transpile(self.to_qiskit(), **kwargs)
+        qiskit_circuit = qiskit.transpile(self.to_qiskit(),**kwargs)
         circuit = self.from_qiskit(qiskit_circuit=qiskit_circuit, replace=replace)
         if not replace:
             return circuit
 
     def to_stim(self):
         stim_circuit = stim.Circuit()
         same_label_control0_list = ['CX', 'CY', 'CZ', 'H']
@@ -843,37 +854,38 @@
                     raise ValueError('Do not support multi control.')
             elif old_label[0] in tuple_RD_list:
                 if len(self.control_list[ii]) > 0:
                     raise ValueError('Do not support control for RD gate.')
                 new_label = old_label[0][1]
                 if self.gate_list[ii].inverse:
                     old_label = (old_label[0], -old_label[1])
-                while old_label[1] / np.pi > 1:
-                    old_label = (old_label[0], old_label[1] - 2 * np.pi)
+                while old_label[1]/np.pi > 1:
+                    old_label = (old_label[0], old_label[1] - 2*np.pi)
                 while old_label[1] / np.pi < -1:
                     old_label = (old_label[0], old_label[1] + 2 * np.pi)
-                if np.abs(old_label[1] / np.pi) == 1:
+                if np.abs(old_label[1]/np.pi) == 1:
                     new_label = new_label
                 elif old_label[1] / np.pi == 0.5:
                     new_label = 'SQRT_' + new_label
                 elif old_label[1] / np.pi == -0.5:
                     new_label = 'SQRT_' + new_label + '_DAG'
                 else:
-                    raise ValueError('Do not support theta/np.pi = ', str(old_label[1] / np.pi))
+                    raise ValueError('Do not support theta/np.pi = ', str(old_label[1]/np.pi))
                 new_position = self.position_list[ii]
             else:
                 raise ValueError('Do not support the label of', str(ii), 'th gate, which is', old_label)
             stim_circuit.append(new_label, new_position)
         return stim_circuit
 
+
     def to_cirq(self):
-        supported_gates_C = {'CZ': cirq.CZ, 'CX': cirq.CX}
-        supported_gates_R = {'RX': cirq.rx, 'RY': cirq.ry, 'RZ': cirq.rz}
-        supported_gates_CC = {'CCX': cirq.CCX, }
-        supported_gates_U = {'U3': QasmUGate}
+        supported_gates_C = {'CZ':cirq.CZ, 'CX':cirq.CX}
+        supported_gates_R = {'RX':cirq.rx, 'RY':cirq.ry, 'RZ':cirq.rz}
+        supported_gates_CC = {'CCX':cirq.CCX, }
+        supported_gates_U = {'U3':QasmUGate}
         cirq_citcuit = cirq.Circuit()
         for ii in range(len(self)):
             if len(self.control_list[ii]) > 0:
                 raise ValueError('does not support controlled gates')
             tmp_label = self.gate_list[ii].label
             if tmp_label in supported_gates_C.keys():
                 position0 = self.qubit_position[self.position_list[ii][0]]
@@ -893,15 +905,15 @@
                 position0 = self.qubit_position[self.position_list[ii][0]]
                 qubit0 = cirq.GridQubit(position0[0], position0[1])
                 cirq_citcuit.append(supported_gates_R[tmp_label[0]](tmp_label[1])(qubit0))
             elif tmp_label[0] in supported_gates_U.keys():
                 position0 = self.qubit_position[self.position_list[ii][0]]
                 qubit0 = cirq.GridQubit(position0[0], position0[1])
                 theta, phi, lmda = tmp_label[1]
-                cirq_citcuit.append(supported_gates_U[tmp_label[0]](theta / np.pi, phi / np.pi, lmda / np.pi)(qubit0))
+                cirq_citcuit.append(supported_gates_U[tmp_label[0]](theta/np.pi, phi/np.pi, lmda/np.pi)(qubit0))
             else:
                 raise ValueError(tmp_label, 'is not supported')
         return cirq_citcuit
 
     def cirq_qubit_order(self):
         cirq_order_list = []
 
@@ -914,14 +926,32 @@
         cirq_circuit = self.to_cirq()
         c3d = cirq_web.Circuit3D(cirq_circuit)
         c3d.generate_html_file(file_name=save_path)
 
     def qiskit_draw(self, **kwargs):
         return self.to_qiskit().draw(**kwargs)
 
+    def check_connectivity(self):
+        error_list = []
+        for _, pp, pp_c in self:
+            position_combined = pp + pp_c
+            if len(position_combined) > 2:
+                raise ValueError('reduce all gate to one- or two- qubit gates before check connectivity')
+            if len(position_combined) == 2:
+                dis_row = self.qubit_position[position_combined[0]][0] - self.qubit_position[position_combined[1]][0]
+                dis_col = self.qubit_position[position_combined[0]][1] - self.qubit_position[position_combined[1]][1]
+                ab_dis = np.abs(dis_row) + np.abs(dis_col)
+                if ab_dis > 1:
+                    error_list.append((pp, pp_c))
+        if len(error_list) > 0:
+            error_str = 'check connectivity fails. Error list is ' +  str(error_list)
+            raise ValueError(error_str)
+
+
+
 
 def qft(n_qubit, position, control=None, inverse=False, device='cpu', dtype=tc.complex64):
     if control is None:
         control = []
     tmp_circuit = Circuit(n_qubit, device, dtype)
     m_qft = len(position)
     perm = list(range(m_qft))
```

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Gate.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/Gate.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     @grad.setter
     def grad(self, value):
         self._tensor.grad = value
 
     # core functions start
 
     def check_unitary(self, acc=1e-6):
-        identity_matrix = tc.eye(self._tensor.shape[0], device=self._tensor.device, dtype=self._tensor.dtype)
-        diff = tc.dist(self._tensor.mm(self._tensor.conj().t()), identity_matrix)
+        identity_matrix = tc.eye(self.tensor.shape[0], device=self.tensor.device, dtype=self.tensor.dtype)
+        diff = tc.dist(self.tensor.mm(self.tensor.conj().t()), identity_matrix)
         flag = (diff > acc)
         if flag:
             raise ValueError('the gate is not unitary. distance is ', diff)
 
     def inv(self):
         self.inverse = not self.inverse
 
@@ -172,16 +172,15 @@
         elif self.label[0] in ('T'):
             self.tensor = tc.tensor([[1, 0], [0, np.exp(1j*np.pi/4)]])
         else:
             raise ValueError('The label', self.label, 'is not supported')
         if self.inverse:
             self.tensor = self.tensor.T.conj()
 
-
-    # core function end
+# core function end
 
 # labelled gate
 
 def labelled_simple_gate(name, params=None):
     if params is None:
         return Gate(unitary=None, label=name)
     else:
@@ -222,17 +221,31 @@
     return Gate(unitary=None, label='CCX')
 
 # practical gates with label
 
 def u3(theta:tuple):
     return Gate(unitary=None, label=('U3', theta))
 
-def u4(theta:tuple, device='cpu', dtype=tc.complex64):
+def u4(theta:tuple):
     return Gate(unitary=None, label=('U4', theta))
 
+def u3_from_tensor(tensor, acc=1e-6):
+    assert tensor.shape == (2, 2)
+    tensor = tensor.to(tc.complex64)
+    tensor = tensor * np.sqrt(2) / tensor.norm()
+    phase = tensor[0, 0] / tensor[0, 0].norm()
+    tensor = tensor / phase
+    theta0 = 2*tc.arccos(tensor[0, 0])
+    theta1 = tensor[1, 0].angle()
+    theta2 = tensor[1, 0].angle() + np.pi
+    gate = Gate(unitary=None, label=('U3', (float(theta0), float(theta1), float(theta2))))
+    gate.check_unitary(acc=acc)
+    return gate
+    
+
 def hadamard():
     return Gate(unitary=None, label='H')
 
 
 def phase_shift(theta, device='cpu', dtype=tc.complex64):
     gate = tc.eye(2, device=device, dtype=dtype)
     gate[1, 1] = tc.exp(tc.tensor(theta * 1j))
```

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/QuantumSimulator/Simulator.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/QuantumSimulator/Simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -421,7 +421,65 @@
         if if_print:
             for key in res.keys():
                 print(key, res[key])
         if return_weight:
             return res, weight
         else:
             return res
+
+
+# temporary program
+class SimulatorOperator:
+    def __init__(self, n_qubit, device='cuda:0', dtype=tc.complex64,
+                 rand_seed=1, operator_acc=1e-5, circuit_size=None, qubit_position=None):
+        self.n_qubit = n_qubit
+        self.device = device
+        self.dtype = dtype
+        self.rand_seed = rand_seed
+        self.shape = 2*n_qubit*(2, )
+        self.operator = tc.eye(2**n_qubit, device=device, dtype=dtype).reshape(self.shape)
+        self.chi = 2 ** self.n_qubit
+        self.operator_acc = operator_acc
+        self.circuit_size = circuit_size
+        self.circuit = Circuit(n_qubit, device=device, dtype=dtype, size=circuit_size, qubit_position=qubit_position)
+
+
+
+    def simulate(self, clear_circuit=True, method=None, fast_mode=None, operator_acc=None):
+        self.operator_simulate(clear_circuit=clear_circuit, operator_acc=operator_acc)
+
+
+    def operator_simulate(self, clear_circuit=True, operator_acc=None):
+        self.circuit.regularize_all_position()
+
+
+        if operator_acc is None:
+            operator_acc = self.operator_acc
+
+        for ii in range(len(self.circuit)):
+            cc = self.circuit[ii]
+            self.act_single_gate(gate=cc[0], position=cc[1], control=cc[2])
+
+        if clear_circuit:
+            self.circuit.clear()
+
+    def act_single_gate(self, gate, position, control=None,):
+        # the position and control need to be canonized
+
+        if control is None:
+            control = []
+        # gate can be sparse, but there seems to be no speedup
+        # one should be careful when add inverse gates
+        m_p = len(position)
+        m_c = len(control)
+        old_position = position + control
+        new_position = list(range(m_p)) + list(range(-m_c, 0))
+        if gate.inverse:
+            tmp_gate = gate.tensor.conj().t()
+        else:
+            tmp_gate = gate.tensor
+        tmp_gate = tmp_gate.to(self.device).to(self.dtype)
+        self.operator = self.operator.movedim(old_position, new_position).contiguous().view(2 ** m_p, -1, 2 ** m_c)
+
+        self.operator[:, :, -1] = tmp_gate.mm(self.operator[:, :, -1])
+
+        self.operator = self.operator.view(self.shape).movedim(new_position, old_position)
```

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/MPSclass.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/MPSclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TEBD.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/TEBD.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence/TEBD/TNclass.py` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence/TEBD/TNclass.py`

 * *Files identical despite different names*

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/PKG-INFO` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumIntelligence
-Version: 0.0.8
+Version: 0.0.9
 Summary: Developing quantum intelligence.
 Author: Zheng-Zhi Sun
 Author-email: sunzhengzhi.work@gmail.com
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `QuantumIntelligence-0.0.8/src/QuantumIntelligence.egg-info/SOURCES.txt` & `QuantumIntelligence-0.0.9/src/QuantumIntelligence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

