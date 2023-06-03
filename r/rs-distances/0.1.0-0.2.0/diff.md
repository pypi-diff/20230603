# Comparing `tmp/rs_distances-0.1.0.tar.gz` & `tmp/rs_distances-0.2.0.tar.gz`

## Comparing `rs_distances-0.1.0.tar` & `rs_distances-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 rs_distances-0.1.0/Cargo.toml
--rw-r--r--   0        0        0      388 2023-06-03 05:19:15.000000 rs_distances-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1207 2023-06-03 06:24:08.000000 rs_distances-0.1.0/src/lib.rs
--rw-r--r--   0        0        0    65812 2023-06-03 05:41:50.000000 rs_distances-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 rs_distances-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 rs_distances-0.2.0/Cargo.toml
+-rw-r--r--   0        0        0      915 2023-06-03 16:17:28.000000 rs_distances-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1164 2023-06-03 15:45:21.000000 rs_distances-0.2.0/src/lib.rs
+-rw-r--r--   0        0        0    65812 2023-06-03 16:17:30.000000 rs_distances-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 rs_distances-0.2.0/PKG-INFO
```

### Comparing `rs_distances-0.1.0/src/lib.rs` & `rs_distances-0.2.0/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 use ndarray::{Array3};
 use pyo3::prelude::*;
 use numpy::{PyArray3, IntoPyArray};
 
 
-fn iterate_spiketrains(scr: &mut Array3<f64>, sd: &Array3<f64>) -> Array3<f64> {
+fn iterate_spiketrains(scr: &mut Array3<f64>, sd: &Array3<f64>)  {
     let (num_qvals, num_spikes_xii, num_spikes_xjj) = scr.dim();
-
     for xii in 1..num_spikes_xii {
         for xjj in 1..num_spikes_xjj {
             for q in 0..num_qvals {
                 let a = scr[[q, xii - 1, xjj]] + 1.0;
                 let b = scr[[q, xii, xjj - 1]] + 1.0;
                 let c = scr[[q, xii - 1, xjj - 1]] + sd[[q, xii - 1, xjj - 1]];
 
                 scr[[q, xii, xjj]] = a.min(b.min(c));
             }
         }
     }
-    scr.clone()
 }
 
 #[pyfunction]
 fn iterate_spiketrains_impl(py: Python, scr: &PyArray3<f64>, sd: &PyArray3<f64>) -> PyResult<PyObject> {
     let mut scr: Array3<f64> = scr.to_owned_array();
     let sd: Array3<f64> = sd.to_owned_array();
 
-    let res = iterate_spiketrains(&mut scr, &sd);
+    iterate_spiketrains(&mut scr, &sd);
 
     // Convert the result to a PyArray
-    let res = res.into_pyarray(py).to_owned();
+    let res = scr.into_pyarray(py).to_owned();
     Ok(res.into())
 }
 
 
 #[pymodule]
 fn rs_distances(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(iterate_spiketrains_impl, m)?)?;
```

### Comparing `rs_distances-0.1.0/Cargo.lock` & `rs_distances-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1632,15 +1632,15 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rs-distances"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "maturin",
  "ndarray",
  "numpy",
  "pyo3",
 ]
```

