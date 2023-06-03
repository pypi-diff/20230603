# Comparing `tmp/rs_distances-0.2.0.tar.gz` & `tmp/rs_distances-0.4.0.tar.gz`

## Comparing `rs_distances-0.2.0.tar` & `rs_distances-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 rs_distances-0.2.0/Cargo.toml
--rw-r--r--   0        0        0      915 2023-06-03 16:17:28.000000 rs_distances-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1164 2023-06-03 15:45:21.000000 rs_distances-0.2.0/src/lib.rs
--rw-r--r--   0        0        0    65812 2023-06-03 16:17:30.000000 rs_distances-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 rs_distances-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 rs_distances-0.4.0/Cargo.toml
+-rw-r--r--   0        0        0     2807 2023-06-03 05:19:15.000000 rs_distances-0.4.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      764 2023-06-03 16:25:17.000000 rs_distances-0.4.0/.gitignore
+-rw-r--r--   0        0        0     2313 2023-06-03 16:58:44.000000 rs_distances-0.4.0/README.md
+-rw-r--r--   0        0        0      914 2023-06-03 18:38:08.000000 rs_distances-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1433 2023-06-03 18:37:49.000000 rs_distances-0.4.0/src/lib.rs
+-rw-r--r--   0        0        0    65812 2023-06-03 18:39:05.000000 rs_distances-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 rs_distances-0.4.0/PKG-INFO
```

### Comparing `rs_distances-0.2.0/pyproject.toml` & `rs_distances-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rs-distances"
 description = "A Python module implemented in Rust for efficient calculations"
 authors = [{name = "Flynn OConnell", email = "flynnoconnell@gmail.com"}]
-#readme = "readme.md"
+readme = "README.md"
 homepage = "https://github.com/NeuroPyPy/rs-distances"
 license = "MIT"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [package]
-version = "0.1.0"
-edition = "2018"
+version = "0.4.0"
+edition = "2023"
 
 [package.metadata.maturin]
 rust-version = "1.56.0"
 requires-dist = ["numpy"]
 
 [package.metadata.maturin.dependencies]
 ndarray = "0.15.4"
```

### Comparing `rs_distances-0.2.0/src/lib.rs` & `rs_distances-0.4.0/src/lib.rs`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,25 @@
                 scr[[q, xii, xjj]] = a.min(b.min(c));
             }
         }
     }
 }
 
 #[pyfunction]
+/// Perform iteration on spike trains.
+///
+/// Rust implimentation of spike-train array iteration.
+///
+/// Args:
+///   scr: Array of spike train data.
+///   sd: Array of additional data.
+///
+/// Returns:
+///   Array: The resulting array after iteration.
+///
 fn iterate_spiketrains_impl(py: Python, scr: &PyArray3<f64>, sd: &PyArray3<f64>) -> PyResult<PyObject> {
     let mut scr: Array3<f64> = scr.to_owned_array();
     let sd: Array3<f64> = sd.to_owned_array();
 
     iterate_spiketrains(&mut scr, &sd);
 
     // Convert the result to a PyArray
```

### Comparing `rs_distances-0.2.0/Cargo.lock` & `rs_distances-0.4.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1632,15 +1632,15 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rs-distances"
-version = "0.2.0"
+version = "0.4.0"
 dependencies = [
  "maturin",
  "ndarray",
  "numpy",
  "pyo3",
 ]
```

