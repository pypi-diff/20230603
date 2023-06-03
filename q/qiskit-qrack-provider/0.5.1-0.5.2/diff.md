# Comparing `tmp/qiskit-qrack-provider-0.5.1.tar.gz` & `tmp/qiskit-qrack-provider-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-qrack-provider-0.5.1.tar", last modified: Thu Mar 23 19:29:24 2023, max compression
+gzip compressed data, was "qiskit-qrack-provider-0.5.2.tar", last modified: Sat Jun  3 15:46:52 2023, max compression
```

## Comparing `qiskit-qrack-provider-0.5.1.tar` & `qiskit-qrack-provider-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.5.1/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2021-12-03 23:15:01.000000 qiskit-qrack-provider-0.5.1/README.md
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/qiskit/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/qiskit/providers/
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1135 2021-10-08 01:17:38.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/__init__.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/backends/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      665 2022-08-31 13:41:07.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/backends/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    31978 2022-09-05 16:13:51.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/backends/noisy_clifford_t_simulator.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    34184 2022-09-05 16:13:24.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/backends/noisy_qasm_simulator.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    36525 2023-03-23 19:09:47.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/backends/qasm_simulator.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/qrackerror.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2021-10-09 18:55:08.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/qrackjob.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1633 2022-08-31 13:44:00.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/qrackprovider.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      507 2022-08-15 16:14:46.000000 qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/version.py
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-03-23 19:29:24.000000 qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      643 2023-03-23 19:29:24.000000 qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-03-23 19:29:24.000000 qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       29 2023-03-23 19:29:24.000000 qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2023-03-23 19:29:24.000000 qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/top_level.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-03-23 19:29:24.042656 qiskit-qrack-provider-0.5.1/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1642 2023-03-23 19:09:34.000000 qiskit-qrack-provider-0.5.1/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.521543 qiskit-qrack-provider-0.5.2/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.5.2/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1671 2021-12-03 23:15:01.000000 qiskit-qrack-provider-0.5.2/README.md
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/providers/
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1135 2021-10-08 01:17:38.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/__init__.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      548 2023-06-03 15:41:45.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    36664 2023-06-03 15:45:18.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/qasm_simulator.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      914 2021-05-14 12:44:18.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackerror.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1903 2021-10-09 18:55:08.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackjob.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1449 2023-06-03 15:42:03.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackprovider.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      506 2023-06-03 15:42:26.000000 qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/version.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-06-03 15:46:52.517543 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     2691 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      525 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       29 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        7 2023-06-03 15:46:52.000000 qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/top_level.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-06-03 15:46:52.521543 qiskit-qrack-provider-0.5.2/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1642 2023-06-03 15:41:06.000000 qiskit-qrack-provider-0.5.2/setup.py
```

### Comparing `qiskit-qrack-provider-0.5.1/LICENSE` & `qiskit-qrack-provider-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.1/PKG-INFO` & `qiskit-qrack-provider-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.5.1
+Version: 0.5.2
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.5.1/README.md` & `qiskit-qrack-provider-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/__init__.py` & `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/backends/__init__.py` & `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Qrack Backends."""
 
 from .qasm_simulator import QasmSimulator
-from .noisy_clifford_t_simulator import NoisyCliffordTSimulator
-from .noisy_qasm_simulator import NoisyQasmSimulator
```

### Comparing `qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/backends/noisy_clifford_t_simulator.py` & `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/backends/qasm_simulator.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,19 +9,16 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 # pylint: disable=invalid-name
 
 
-import os
-import math
 import uuid
 import time
-import random
 import numpy as np
 import pandas as pd
 from datetime import datetime
 from collections import Counter
 from qiskit.providers.models import BackendConfiguration
 
 from ..version import __version__
@@ -83,24 +80,23 @@
         self.header = header
         self.meta_data = meta_data,
         self.time_taken = time_taken
 
     def to_dict(self):
         return vars(self)
 
-class NoisyCliffordTSimulator(BackendV1):
+
+class QasmSimulator(BackendV1):
     """
-    A very efficient Clifford+T simulator with an intrinsically noisy T gate (and inverse).
+    Contains an OpenCL based backend
     """
 
     DEFAULT_OPTIONS = {
         'method': 'automatic',
         'shots': 1024,
-        'noise': 0.0001,
-        'is_strong_simulation': False,
         'is_schmidt_decompose_multi': True,
         'is_schmidt_decompose': True,
         'is_stabilizer_hybrid': True,
         'is_binary_decision_tree': False,
         'is_paged': True,
         'is_cpu_gpu_hybrid': True,
         'is_host_pointer': False,
@@ -116,24 +112,76 @@
         'local': True,
         'open_pulse': False,
         'memory': True,
         'max_shots': 65536,
         'description': 'An OpenCL based qasm simulator',
         'coupling_map': None,
         'basis_gates': [
-            'id', 'h', 'x', 'y', 'z', 's', 'sdg', 'sx', 'sxdg', 't', 'tdg', 'rz', 'u1', 'p'
-            'cx', 'cy', 'cz', 'swap', 'iswap', 'reset', 'measure', 'barrier'
+            'id', 'u', 'u1', 'u2', 'u3', 'r', 'rx', 'ry', 'rz',
+            'h', 'x', 'y', 'z', 's', 'sdg', 'sx', 'sxdg', 'p', 't', 'tdg',
+            'cu', 'cu1', 'cu2', 'cu3', 'cx', 'cy', 'cz', 'ch', 'cp', 'csx', 'csxdg', 'dcx',
+            'ccx', 'ccy', 'ccz', 'mcx', 'mcy', 'mcz', 'mcu', 'mcu1', 'mcu2', 'mcu3',
+            'swap', 'iswap', 'cswap', 'mcswap', 'reset', 'measure', 'barrier'
         ],
         'gates': [{
             'name': 'id',
             'parameters': [],
             'conditional': True,
             'description': 'Single-qubit identity gate',
             'qasm_def': 'gate id a { U(0,0,0) a; }'
         }, {
+            'name': 'u',
+            'parameters': ['theta', 'phi', 'lam'],
+            'conditional': True,
+            'description': 'Single-qubit gate with three rotation angles',
+            'qasm_def': 'gate u(theta,phi,lam) q { U(theta,phi,lam) q; }'
+        }, {
+            'name': 'u1',
+            'parameters': ['lam'],
+            'conditional': True,
+            'description': 'Single-qubit gate [[1, 0], [0, exp(1j*lam)]]',
+            'qasm_def': 'gate u1(lam) q { U(0,0,lam) q; }'
+        }, {
+            'name': 'u2',
+            'parameters': ['phi', 'lam'],
+            'conditional': True,
+            'description':
+            'Single-qubit gate [[1, -exp(1j*lam)], [exp(1j*phi), exp(1j*(phi+lam))]]/sqrt(2)',
+            'qasm_def': 'gate u2(phi,lam) q { U(pi/2,phi,lam) q; }'
+        }, {
+            'name': 'u3',
+            'parameters': ['theta', 'phi', 'lam'],
+            'conditional': True,
+            'description': 'Single-qubit gate with three rotation angles',
+            'qasm_def': 'gate u3(theta,phi,lam) q { U(theta,phi,lam) q; }'
+        }, {
+            'name': 'r',
+            'parameters': ['lam'],
+            'conditional': True,
+            'description': 'Single-qubit gate [[1, 0], [0, exp(1j*lam)]]',
+            'qasm_def': 'gate p(lam) q { U(0,0,lam) q; }'
+        }, {
+            'name': 'rx',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Single-qubit Pauli-X axis rotation gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'ry',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Single-qubit Pauli-Y axis rotation gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'rz',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Single-qubit Pauli-Z axis rotation gate',
+            'qasm_def': 'TODO'
+        }, {
             'name': 'h',
             'parameters': [],
             'conditional': True,
             'description': 'Single-qubit Hadamard gate',
             'qasm_def': 'TODO'
         }, {
             'name': 'x',
@@ -174,43 +222,55 @@
         }, {
             'name': 'sxdg',
             'parameters': [],
             'conditional': True,
             'description': 'Single-qubit inverse square root of Pauli-X gate',
             'qasm_def': 'TODO'
         }, {
+            'name': 'p',
+            'parameters': ['theta', 'phi'],
+            'conditional': True,
+            'description': 'Single-qubit gate [[cos(theta), -1j*exp(-1j*phi)], [sin(theta), -1j*exp(1j *phi)*sin(theta), cos(theta)]]',
+            'qasm_def': 'gate r(theta, phi) q { U(theta, phi - pi/2, -phi + pi/2) q;}'
+        }, {
             'name': 't',
             'parameters': [],
             'conditional': True,
             'description': 'Single-qubit T gate',
             'qasm_def': 'TODO'
         }, {
             'name': 'tdg',
             'parameters': [],
             'conditional': True,
             'description': 'Single-qubit adjoint T gate',
             'qasm_def': 'TODO'
         }, {
-            'name': 'rz',
-            'parameters': [],
+            'name': 'cu',
+            'parameters': ['theta', 'phi', 'lam'],
             'conditional': True,
-            'description': 'Single-qubit Pauli-Z axis rotation gate',
+            'description': 'Two-qubit Controlled-u gate',
             'qasm_def': 'TODO'
         }, {
-            'name': 'u1',
+            'name': 'cu1',
             'parameters': ['lam'],
             'conditional': True,
-            'description': 'Single-qubit gate [[1, 0], [0, exp(1j*lam)]]',
-            'qasm_def': 'gate u1(lam) q { U(0,0,lam) q; }'
+            'description': 'Two-qubit Controlled-u1 gate',
+            'qasm_def': 'TODO'
         }, {
-            'name': 'p',
-            'parameters': ['theta', 'phi'],
+            'name': 'cu2',
+            'parameters': ['phi', 'lam'],
             'conditional': True,
-            'description': 'Single-qubit gate [[cos(theta), -1j*exp(-1j*phi)], [sin(theta), -1j*exp(1j *phi)*sin(theta), cos(theta)]]',
-            'qasm_def': 'gate r(theta, phi) q { U(theta, phi - pi/2, -phi + pi/2) q;}'
+            'description': 'Two-qubit Controlled-u2 gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'cu3',
+            'parameters': ['theta', 'phi', 'lam'],
+            'conditional': True,
+            'description': 'Two-qubit Controlled-u3 gate',
+            'qasm_def': 'TODO'
         }, {
             'name': 'cx',
             'parameters': [],
             'conditional': True,
             'description': 'Two-qubit Controlled-NOT gate',
             'qasm_def': 'gate cx c,t { CX c,t; }'
         }, {
@@ -222,26 +282,128 @@
         }, {
             'name': 'cz',
             'parameters': [],
             'conditional': True,
             'description': 'Two-qubit Controlled-Z gate',
             'qasm_def': 'gate cz a,b { h b; cx a,b; h b; }'
         }, {
+            'name': 'ch',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Two-qubit Controlled-H gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'cp',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Controlled-Phase gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'csx',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Two-qubit Controlled square root of Pauli-X gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'csxdg',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Two-qubit controlled inverse square root of Pauli-X gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'dcx',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Double-CNOT gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'ccx',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Three-qubit Toffoli gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'ccy',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Three-qubit controlled-Y gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'ccz',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Three-qubit controlled-Z gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcx',
+            'parameters': [],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-X gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcy',
+            'parameters': [],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-Y gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcz',
+            'parameters': [],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-Z gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcu',
+            'parameters': ['theta', 'phi', 'lam'],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-u3 gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcu1',
+            'parameters': ['lam'],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-u1 gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcu2',
+            'parameters': ['phi', 'lam'],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-u2 gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcu3',
+            'parameters': ['theta', 'phi', 'lam'],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-u3 gate',
+            'qasm_def': 'TODO'
+        }, {
             'name': 'swap',
             'parameters': [],
             'conditional': True,
             'description': 'Two-qubit SWAP gate',
             'qasm_def': 'TODO'
         }, {
             'name': 'iswap',
             'parameters': [],
             'conditional': True,
             'description': 'Two-qubit ISWAP gate',
             'qasm_def': 'TODO'
         }, {
+            'name': 'cswap',
+            'parameters': [],
+            'conditional': True,
+            'description': 'Three-qubit Fredkin (controlled-SWAP) gate',
+            'qasm_def': 'TODO'
+        }, {
+            'name': 'mcswap',
+            'parameters': [],
+            'conditional': True,
+            'description': 'N-qubit multi-controlled-SWAP gate',
+            'qasm_def': 'TODO'
+        }, {
             'name': 'measure',
             'parameters': [],
             'conditional': True,
             'description': 'Measure qubit',
             'qasm_def': 'TODO'
         }, {
             'name': 'reset',
@@ -352,32 +514,24 @@
             'isStabilizerHybrid': options.is_stabilizer_hybrid if hasattr(options, 'is_stabilizer_hybrid') else self._options.get('is_stabilizer_hybrid'),
             'isBinaryDecisionTree': options.is_binary_decision_tree if hasattr(options, 'is_binary_decision_tree') else self._options.get('is_binary_decision_tree'),
             'isPaged': options.is_paged if hasattr(options, 'is_paged') else self._options.get('is_paged'),
             'isCpuGpuHybrid': options.is_cpu_gpu_hybrid if hasattr(options, 'is_cpu_gpu_hybrid') else self._options.get('is_cpu_gpu_hybrid'),
             'isHostPointer': options.is_host_pointer if hasattr(options, 'is_host_pointer') else self._options.get('is_host_pointer'),
         }
 
-        # In the ideal, if the user isn't demanding a specific separability threshold, this is a well-motivated choice.
-        is_strong_simulation = options.noise if hasattr(options, 'is_strong_simulation') else self._options.get('is_strong_simulation')
-        noise = options.noise if hasattr(options, 'noise') else self._options.get('noise')
-        self._reset_separability_threshold = False
-        if "QRACK_QUNIT_SEPARABILITY_THRESHOLD" not in os.environ:
-            self._reset_separability_threshold = True
-            os.environ["QRACK_QUNIT_SEPARABILITY_THRESHOLD"] = str(noise / 2)
-
         data = run_input.config.memory if hasattr(run_input, 'config') else []
         self._shots = options['shots'] if 'shots' in options else (run_input.config.shots if hasattr(run_input, 'config') else self._options.get('shots'))
         qobj_id = options['qobj_id'] if 'qobj_id' in options else (run_input.qobj_id if hasattr(run_input, 'config') else '')
         qobj_header = options['qobj_header'] if 'qobj_header' in options else (run_input.header if hasattr(run_input, 'config') else {})
         job_id = str(uuid.uuid4())
 
-        job = QrackJob(self, job_id, self._run_job(job_id, run_input, data, qobj_id, qobj_header, noise, is_strong_simulation, **qrack_options), run_input)
+        job = QrackJob(self, job_id, self._run_job(job_id, run_input, data, qobj_id, qobj_header, **qrack_options), run_input)
         return job
 
-    def _run_job(self, job_id, run_input, data, qobj_id, qobj_header, noise, is_strong_simulation, **options):
+    def _run_job(self, job_id, run_input, data, qobj_id, qobj_header, **options):
         """Run experiments in run_input
         Args:
             job_id (str): unique id for the job.
             run_input (QuantumCircuit or Schedule or list): job description
         Returns:
             Result: Result object
         """
@@ -387,34 +541,30 @@
 
         experiments = run_input.experiments if hasattr(run_input, 'config') else run_input
         if isinstance(experiments, QuantumCircuit):
             experiments = [experiments]
         results = []
 
         for experiment in experiments:
-            results.append(self.run_experiment(experiment, noise, is_strong_simulation, **options))
-
-        if self._reset_separability_threshold:
-            # If the separability threshold is auto-default, clear its automatically assigned environment variable.
-            del os.environ["QRACK_QUNIT_SEPARABILITY_THRESHOLD"]
+            results.append(self.run_experiment(experiment, **options))
 
         return Result(
             backend_name = self.name(),
             backend_version = self._configuration.backend_version,
             qobj_id = qobj_id,
             job_id = job_id,
             success = True,
             results = results,
             date = datetime.now(),
             status = 'COMPLETED',
             header = QrackExperimentHeader(qobj_header) if type(qobj_header) is dict else qobj_header,
             time_taken = (time.time() - start)
         )
 
-    def run_experiment(self, experiment, noise, is_strong_simulation, **options):
+    def run_experiment(self, experiment, **options):
         """Run an experiment (circuit) and return a single experiment result.
         Args:
             experiment (QobjExperiment): experiment from qobj experiments list
         Returns:
             dict: A dictionary of results.
             dict: A result dictionary
         Raises:
@@ -485,28 +635,14 @@
                 continue
 
             if is_initializing and ((operation.name == 'measure') or (operation.name == 'reset')):
                 continue
 
             is_initializing = False
 
-            if (noise > 0) and (not is_strong_simulation):
-                if (operation.name == 't') or (operation.name == 'tdg'):
-                    if boundary_start == -1:
-                        boundary_start = opcount
-                elif (operation.name == 'rz') or (operation.name == 'u1') or (operation.name == 'p'):
-                    angle = operation.params[0]
-                    while float(angle) < 0.:
-                        angle = angle + 2. * math.pi
-                    while float(angle) >= 2. * math.pi:
-                        angle = angle - 2. * math.pi
-                    if not (math.isclose(angle, 0.) or math.isclose(angle, math.pi) or math.isclose(angle, math.pi / 2.) or math.isclose(angle, -math.pi / 2.)):
-                        if boundary_start == -1:
-                            boundary_start = opcount
-
             if (operation.name == 'measure') or (operation.name == 'reset'):
                 if boundary_start == -1:
                     boundary_start = opcount
 
             if (boundary_start != -1) and (operation.name != 'measure'):
                 shotsPerLoop = 1
                 shotLoopMax = self._shots
@@ -526,15 +662,15 @@
             boundary_start -= 1
             if boundary_start > 0:
                 self._sim = QrackSimulator(qubitCount = self._number_of_qubits, **options)
                 self._classical_memory = 0
                 self._classical_register = 0
 
                 for operation in instructions[:boundary_start]:
-                    self._apply_op(operation, noise, is_strong_simulation)
+                    self._apply_op(operation)
 
                 preamble_memory = self._classical_memory
                 preamble_register = self._classical_register
                 preamble_sim = self._sim
 
         for shot in range(shotLoopMax):
             if preamble_sim is None:
@@ -543,15 +679,15 @@
                 self._classical_register = 0
             else:
                 self._sim = QrackSimulator(cloneSid = preamble_sim.sid)
                 self._classical_memory = preamble_memory
                 self._classical_register = preamble_register
 
             for operation in instructions[boundary_start:]:
-                self._apply_op(operation, noise, is_strong_simulation)
+                self._apply_op(operation)
 
             if not self._sample_measure and (len(self._sample_qubits) > 0):
                 self._data += [hex(int(bin(self._classical_memory)[2:], 2))]
                 self._sample_qubits = []
                 self._sample_clbits = []
                 self._sample_cregbits = []
 
@@ -576,60 +712,17 @@
             status = 'DONE',
             success = True,
             header = experiment.header if isinstance(experiment, QasmQobjExperiment) else QrackExperimentResultHeader(name = experiment.name),
             meta_data = metadata,
             time_taken = (time.time() - start)
         )
 
-    def inject_depolarizing_1qb_noise(self, qubit, lam, is_strong_simulation=False):
-        if (lam <= 0.):
-            return
-
-        # Original qubit, Z->X basis
-        self._sim.h(qubit)
-
-        # Allocate an ancilla
-        ancilla = self._sim.num_qubits()
-        self._sim.allocate_qubit(ancilla)
-        # Partially entangle with the ancilla
-        lamAngle = 2. * math.asin(lam ** (1/4))
-        self._sim.mcr(Pauli.PauliY, lamAngle, [qubit], ancilla)
-
-        if not is_strong_simulation:
-            # Partially collapse the original state
-            self._sim.m(ancilla)
-            # The ancilla is fully separable, after measurement.
-            self._sim.release(ancilla)
-
-        # Uncompute
-        self._sim.h(qubit)
-
-        if not is_strong_simulation:
-            # The original qubit might be below separability threshold.
-            self._sim.try_separate_1qb(qubit)
-
-    def _apply_op(self, operation, noise, is_strong_simulation):
+    def _apply_op(self, operation):
         name = operation.name
 
-        # Divert variational phase gates to Clifford, when possible.
-        if name == 'rz' or name == 'u1' or name == 'p':
-            angle = operation.params[0]
-            while float(angle) < 0.:
-                angle = angle + 2. * math.pi
-            while float(angle) >= 2. * math.pi:
-                angle = angle - 2. * math.pi
-            if math.isclose(angle, 0.):
-                return
-            if math.isclose(angle, math.pi):
-                name = 'z'
-            elif math.isclose(angle, math.pi / 2.):
-                name = 's'
-            elif math.isclose(angle, -math.pi / 2.):
-                name = 'sdg'
-
         if (name == 'id') or (name == 'barrier'):
             # Skip measurement logic
             return
 
         conditional = getattr(operation, 'conditional', None)
         if isinstance(conditional, int):
             conditional_bit_set = (self._classical_register >> conditional) & 1
@@ -641,15 +734,29 @@
                 value = self._classical_memory & mask
                 while (mask & 0x1) == 0:
                     mask >>= 1
                     value >>= 1
                 if value != int(conditional.val, 16):
                     return
 
-        if name == 'h':
+        if (name == 'u1') or (name == 'p'):
+            self._sim.u(operation.qubits[0], 0, 0, float(operation.params[0]))
+        elif name == 'u2':
+            self._sim.u(operation.qubits[0], np.pi / 2, float(operation.params[0]), float(operation.params[1]))
+        elif (name == 'u3') or (name == 'u'):
+            self._sim.u(operation.qubits[0], float(operation.params[0]), float(operation.params[1]), float(operation.params[2]))
+        elif name == 'r':
+            self._sim.u(operation.qubits[0], float(operation.params[0]), float(operation.params[1]) - np.pi/2, (-1 * float(operation.params[1])) + np.pi/2)
+        elif name == 'rx':
+            self._sim.r(Pauli.PauliX, float(operation.params[0]), operation.qubits[0])
+        elif name == 'ry':
+            self._sim.r(Pauli.PauliY, float(operation.params[0]), operation.qubits[0])
+        elif name == 'rz':
+            self._sim.r(Pauli.PauliZ, float(operation.params[0]), operation.qubits[0])
+        elif name == 'h':
             self._sim.h(operation.qubits[0])
         elif name == 'x':
             self._sim.x(operation.qubits[0])
         elif name == 'y':
             self._sim.y(operation.qubits[0])
         elif name == 'z':
             self._sim.z(operation.qubits[0])
@@ -657,37 +764,61 @@
             self._sim.s(operation.qubits[0])
         elif name == 'sdg':
             self._sim.adjs(operation.qubits[0])
         elif name == 'sx':
             self._sim.mtrx([(1+1j)/2, (1-1j)/2, (1-1j)/2, (1+1j)/2], operation.qubits[0])
         elif name == 'sxdg':
             self._sim.mtrx([(1-1j)/2, (1+1j)/2, (1+1j)/2, (1-1j)/2], operation.qubits[0])
-        # See https://arxiv.org/abs/1810.03176 for suggestion of only non-Clifford noise.
         elif name == 't':
             self._sim.t(operation.qubits[0])
-            self.inject_depolarizing_1qb_noise(operation.qubits[0], noise, is_strong_simulation)
         elif name == 'tdg':
             self._sim.adjt(operation.qubits[0])
-            self.inject_depolarizing_1qb_noise(operation.qubits[0], noise, is_strong_simulation)
-        elif name == 'rz':
-            self._sim.r(Pauli.PauliZ, operation.params[0], operation.qubits[0])
-            self.inject_depolarizing_1qb_noise(operation.qubits[0], noise, is_strong_simulation)
-        elif (name == 'u1') or (name == 'p'):
-            self._sim.u(operation.qubits[0], 0, 0, operation.params[0])
-            self.inject_depolarizing_1qb_noise(operation.qubits[0], noise, is_strong_simulation)
+        elif name == 'cu1':
+            self._sim.mcu(operation.qubits[0:1], operation.qubits[1], 0, 0, float(operation.params[0]))
+        elif name == 'cu2':
+            self._sim.mcu(operation.qubits[0:1], operation.qubits[1], np.pi / 2, float(operation.params[0]), float(operation.params[1]))
+        elif (name == 'cu3') or (name == 'cu'):
+            self._sim.mcu(operation.qubits[0:1], operation.qubits[1], float(operation.params[0]), float(operation.params[1]), float(operation.params[2]))
         elif name == 'cx':
             self._sim.mcx(operation.qubits[0:1], operation.qubits[1])
         elif name == 'cy':
             self._sim.mcy(operation.qubits[0:1], operation.qubits[1])
         elif name == 'cz':
             self._sim.mcz(operation.qubits[0:1], operation.qubits[1])
+        elif name == 'ch':
+            self._sim.mch(operation.qubits[0:1], operation.qubits[1])
+        elif name == 'cp':
+            self._sim.mcmtrx(operation.qubits[0:1], [1, 0, 0, np.exp(1j * float(operation.params[0]))], operation.qubits[1])
+        elif name == 'csx':
+            self._sim.mcmtrx(operation.qubits[0:1], [(1+1j)/2, (1-1j)/2, (1-1j)/2, (1+1j)/2], operation.qubits[1])
+        elif name == 'csxdg':
+            self._sim.mcmtrx(operation.qubits[0:1], [(1-1j)/2, (1+1j)/2, (1+1j)/2, (1-1j)/2], operation.qubits[1])
+        elif name == 'dcx':
+            self._sim.mcx(operation.qubits[0:1], operation.qubits[1])
+            self._sim.mcx(operation.qubits[1:2], operation.qubits[0])
+        elif name == 'ccx':
+            self._sim.mcx(operation.qubits[0:2], operation.qubits[2])
+        elif name == 'ccy':
+            self._sim.mcy(operation.qubits[0:2], operation.qubits[2])
+        elif name == 'ccz':
+            self._sim.mcz(operation.qubits[0:2], operation.qubits[2])
+        elif name == 'mcx':
+            self._sim.mcx(operation.qubits[0:-1], operation.qubits[-1])
+        elif name == 'mcy':
+            self._sim.mcy(operation.qubits[0:-1], operation.qubits[-1])
+        elif name == 'mcz':
+            self._sim.mcz(operation.qubits[0:-1], operation.qubits[-1])
         elif name == 'swap':
             self._sim.swap(operation.qubits[0], operation.qubits[1])
         elif name == 'iswap':
             self._sim.iswap(operation.qubits[0], operation.qubits[1])
+        elif name == 'cswap':
+            self._sim.cswap(operation.qubits[0:1], operation.qubits[1], operation.qubits[2])
+        elif name == 'mcswap':
+            self._sim.cswap(operation.qubits[:-2], operation.qubits[-2], operation.qubits[-1])
         elif name == 'reset':
             qubits = operation.qubits
             for qubit in qubits:
                 if self._sim.m(qubit):
                     self._sim.x(qubit)
         elif name == 'measure':
             qubits = operation.qubits
@@ -787,8 +918,8 @@
 
             data.append(hex(int(bin(self._classical_memory)[2:], 2)))
 
         return data
 
     @staticmethod
     def name():
-        return 'noisy_clifford_t_simulator'
+        return 'qasm_simulator'
```

### Comparing `qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/qrackerror.py` & `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackerror.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/qrackjob.py` & `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackjob.py`

 * *Files identical despite different names*

### Comparing `qiskit-qrack-provider-0.5.1/qiskit/providers/qrack/qrackprovider.py` & `qiskit-qrack-provider-0.5.2/qiskit/providers/qrack/qrackprovider.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,28 +13,26 @@
 # pylint: disable=invalid-name, bad-continuation
 
 """Provider for Qrack backends."""
 
 from qiskit.providers.provider import ProviderV1
 from qiskit.providers.providerutils import filter_backends
 
-from .backends import QasmSimulator, NoisyCliffordTSimulator, NoisyQasmSimulator
+from .backends import QasmSimulator
 
 
 class QrackProvider(ProviderV1):
     """Provider for Qrack backends."""
 
     def __init__(self):
         super().__init__()
 
         # Populate the list of Qrack simulator providers.
         self._backends = [
-            QasmSimulator(configuration=None, provider=self),
-            NoisyCliffordTSimulator(configuration=None, provider=self),
-            NoisyQasmSimulator(configuration=None, provider=self)
+            QasmSimulator(configuration=None, provider=self)
         ]
 
     def backends(self, name=None, filters=None, **kwargs):
         # pylint: disable=arguments-differ
         backends = self._backends
         if name:
             backends = [backend for backend in backends if backend.name() == name]
```

### Comparing `qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/PKG-INFO` & `qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-qrack-provider
-Version: 0.5.1
+Version: 0.5.2
 Summary: Qiskit Qrack Provider - Qrack High-Performance GPU simulation for Qiskit
 Home-page: https://github.com/vm6502q/qiskit-qrack-provider
 Author: Daniel Strano
 Author-email: dan@unitary.fund
 License: Apache 2.0
 Keywords: qiskit qrack pyqrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `qiskit-qrack-provider-0.5.1/qiskit_qrack_provider.egg-info/SOURCES.txt` & `qiskit-qrack-provider-0.5.2/qiskit_qrack_provider.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,13 @@
 setup.py
 qiskit/providers/qrack/__init__.py
 qiskit/providers/qrack/qrackerror.py
 qiskit/providers/qrack/qrackjob.py
 qiskit/providers/qrack/qrackprovider.py
 qiskit/providers/qrack/version.py
 qiskit/providers/qrack/backends/__init__.py
-qiskit/providers/qrack/backends/noisy_clifford_t_simulator.py
-qiskit/providers/qrack/backends/noisy_qasm_simulator.py
 qiskit/providers/qrack/backends/qasm_simulator.py
 qiskit_qrack_provider.egg-info/PKG-INFO
 qiskit_qrack_provider.egg-info/SOURCES.txt
 qiskit_qrack_provider.egg-info/dependency_links.txt
 qiskit_qrack_provider.egg-info/requires.txt
 qiskit_qrack_provider.egg-info/top_level.txt
```

### Comparing `qiskit-qrack-provider-0.5.1/setup.py` & `qiskit-qrack-provider-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = [
     'numpy>=1.16.3',
     'pyqrack>=0.8.0'
 ]
 
 # Handle version.
-VERSION = "0.5.1"
+VERSION = "0.5.2"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                            'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
```

