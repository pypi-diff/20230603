# Comparing `tmp/read_rapidpe-0.5.4.tar.gz` & `tmp/read_rapidpe-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_rapidpe-0.5.4.tar", max compression
+gzip compressed data, was "read_rapidpe-0.5.5.tar", max compression
```

## Comparing `read_rapidpe-0.5.4.tar` & `read_rapidpe-0.5.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.5.4/README.md
--rw-r--r--   0        0        0      627 2023-06-03 11:55:30.000242 read_rapidpe-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      303 2023-05-17 02:31:18.161235 read_rapidpe-0.5.4/read_rapidpe/__init__.py
--rw-r--r--   0        0        0    11295 2023-05-13 16:31:51.989559 read_rapidpe-0.5.4/read_rapidpe/grid_point.py
--rw-r--r--   0        0        0     3445 2023-05-16 05:02:30.343719 read_rapidpe-0.5.4/read_rapidpe/io.py
--rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.5.4/read_rapidpe/p_astro.py
--rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.5.4/read_rapidpe/parser.py
--rw-r--r--   0        0        0     1802 2023-05-17 02:28:36.535926 read_rapidpe-0.5.4/read_rapidpe/plot.py
--rw-r--r--   0        0        0    27705 2023-06-03 11:51:35.256470 read_rapidpe-0.5.4/read_rapidpe/result.py
--rw-r--r--   0        0        0     8222 2023-06-02 21:48:32.317059 read_rapidpe-0.5.4/read_rapidpe/transform.py
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-04-17 13:15:50.969962 read_rapidpe-0.5.5/README.md
+-rw-r--r--   0        0        0      627 2023-06-03 21:07:18.540968 read_rapidpe-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      303 2023-05-17 02:31:18.161235 read_rapidpe-0.5.5/read_rapidpe/__init__.py
+-rw-r--r--   0        0        0    11295 2023-05-13 16:31:51.989559 read_rapidpe-0.5.5/read_rapidpe/grid_point.py
+-rw-r--r--   0        0        0     3620 2023-06-03 15:19:21.433555 read_rapidpe-0.5.5/read_rapidpe/io.py
+-rw-r--r--   0        0        0     6083 2023-04-16 13:20:01.614285 read_rapidpe-0.5.5/read_rapidpe/p_astro.py
+-rw-r--r--   0        0        0     9718 2023-04-07 15:04:09.805939 read_rapidpe-0.5.5/read_rapidpe/parser.py
+-rw-r--r--   0        0        0     1802 2023-05-17 02:28:36.535926 read_rapidpe-0.5.5/read_rapidpe/plot.py
+-rw-r--r--   0        0        0    33017 2023-06-03 21:05:24.917487 read_rapidpe-0.5.5/read_rapidpe/result.py
+-rw-r--r--   0        0        0     8855 2023-06-03 14:39:22.849276 read_rapidpe-0.5.5/read_rapidpe/transform.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 read_rapidpe-0.5.5/PKG-INFO
```

### Comparing `read_rapidpe-0.5.4/README.md` & `read_rapidpe-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.4/pyproject.toml` & `read_rapidpe-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "read-rapidpe"
-version = "0.5.4"
+version = "0.5.5"
 description = "Read and analyse results generated by rapidpe-rift-pipe"
 authors = ["Cory Chu <cory@gwlab.page>"]
 readme = "README.md"
 packages = [{include = "read_rapidpe"}]
 homepage = "https://github.com/c0rychu/read-rapidpe"
 repository = "https://git.ligo.org/yu-kuang.chu/read-rapidpe"
```

### Comparing `read_rapidpe-0.5.4/read_rapidpe/grid_point.py` & `read_rapidpe-0.5.5/read_rapidpe/grid_point.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.4/read_rapidpe/io.py` & `read_rapidpe-0.5.5/read_rapidpe/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,14 +101,21 @@
     keys = dict_of_ndarray.keys()
     names = ", ".join(keys)
     return np.core.records.fromarrays(
         [dict_of_ndarray[key] for key in keys], names=names
         )
 
 
+def recarray_to_dict_of_ndarray(recarray):
+    """
+    Convert numpy record-array to dict of ndarray
+    """
+    return {key: recarray[key] for key in recarray.dtype.names}
+
+
 def dict_to_hdf_group(input_dict, hdf_group):
     """
     Save nested python dict to existing hdf5 group
     """
     for key, val in input_dict.items():
         if isinstance(val, dict):
             g = hdf_group.create_group(key)
```

### Comparing `read_rapidpe-0.5.4/read_rapidpe/p_astro.py` & `read_rapidpe-0.5.5/read_rapidpe/p_astro.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.4/read_rapidpe/parser.py` & `read_rapidpe-0.5.5/read_rapidpe/parser.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.4/read_rapidpe/plot.py` & `read_rapidpe-0.5.5/read_rapidpe/plot.py`

 * *Files identical despite different names*

### Comparing `read_rapidpe-0.5.4/read_rapidpe/result.py` & `read_rapidpe-0.5.5/read_rapidpe/result.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 import h5py
 # import pandas as pd
 from .grid_point import RapidPE_grid_point
 from .io import load_event_info_dict_txt
 from .io import load_injection_info_txt
 from .io import dict_of_ndarray_to_recarray
+from .io import recarray_to_dict_of_ndarray
 from .io import dict_from_hdf_group
 from .io import dict_to_hdf_group
 
 from .transform import transform_m1m2_to_mceta, transform_mceta_to_m1m2
 from .transform import jacobian_mceta_by_m1m2
 from .transform import Mass_Spin
 
@@ -91,15 +92,16 @@
             self._keys = []
         else:
             self.grid_points = result.grid_points
             self._keys = result._keys
 
             for attr in result._keys + ["event_info",
                                         "injection_info",
-                                        "config_info"]:
+                                        "config_info",
+                                        "posterior_samples"]:
                 try:
                     setattr(self, attr, getattr(result, attr))
                 except AttributeError:
                     pass
             # Try:
             # self.mass_1 = result.mass_1
             # self.mass_2 = result.mass_2
@@ -198,45 +200,55 @@
 
         extrinsic_table : bool
             Whether loading extrinsic_table as well
 
         """
         result = cls()
         with h5py.File(hdf_file, "r") as f:
-            # Load grid_points
-            gps = f["grid_points"]
-            N = len(gps)
-            result.grid_points = np.empty(N, dtype=object)
-            for i, gp in enumerate(gps.values()):
-                result.grid_points[i] = \
-                    RapidPE_grid_point.from_hdf_grid_point_group(
-                        hdf_gp_group=gp,
-                        extrinsic_table=extrinsic_table
-                        )
-
-            # Load intrinsic_table
-            it = f["intrinsic_table"]
-            result.intrinsic_table = {key: it[key] for key in it.dtype.names}
+            try:
+                # Load grid_points
+                gps = f["grid_points"]
+                N = len(gps)
+                result.grid_points = np.empty(N, dtype=object)
+                for i, gp in enumerate(gps.values()):
+                    result.grid_points[i] = \
+                        RapidPE_grid_point.from_hdf_grid_point_group(
+                            hdf_gp_group=gp,
+                            extrinsic_table=extrinsic_table
+                            )
+
+                # Load intrinsic_table
+                it = f["intrinsic_table"]
+                result.intrinsic_table = {key: it[key] for key in it.dtype.names}  # noqa E501
+                result._keys = list(it.dtype.names)
+            except KeyError:
+                pass
 
             # Load other attributes
-            result._keys = list(it.dtype.names)
             for attr in result._keys:
                 try:
                     setattr(result, attr, result.intrinsic_table[attr])
                 except KeyError:
                     pass
 
             # Load event_info and injection_info
             for attr in ["event_info", "injection_info", "config_info"]:
                 try:
                     x = dict_from_hdf_group(f[attr])
                     setattr(result, attr, x)
                 except KeyError:
                     pass
 
+            # Load posterior samples
+            try:
+                result.posterior_samples = \
+                     recarray_to_dict_of_ndarray(f["posterior_samples"])
+            except KeyError:
+                pass
+
         return cls(result)
 
     @classmethod
     def from_run_dir(cls,
                      run_dir,
                      use_numpy=True,
                      use_ligolw=True,
@@ -420,69 +432,79 @@
 
         compression : str, optional (default: None)
             The compression method, e.g., "gzip", "lzf".
         """
 
         with h5py.File(hdf_filename, 'w', track_order=True) as f:
 
-            # Check if there is extrinsic_table
-            gp = self.grid_points[0]
-            extrinsic_table &= len(gp.extrinsic_table) > 0
-
-            # Create "grid_points" group to hold self.grid_points
-            group_grid_points_raw = \
-                f.create_group("grid_points", track_order=True)
-
-            for i, gp in enumerate(self.grid_points):
-                group_gp = group_grid_points_raw.create_group(str(i))
-
-                # Add intrinsic_table
-                it = dict_of_ndarray_to_recarray(gp.intrinsic_table)
-                group_gp.create_dataset("intrinsic_table", data=it)
+            # Check if there are results
+            if len(self.grid_points) != 0:
 
-                # Add extrinsic_table
-                if extrinsic_table:
-                    et = dict_of_ndarray_to_recarray(gp.extrinsic_table)
-                    group_gp.create_dataset("extrinsic_table",
-                                            data=et,
-                                            compression=compression)
-
-                # Add xml_filename
-                group_gp.attrs["xml_filename"] = gp.xml_filename
-
-            # Combine intrinsic parameters into "intrinsic_table" dataset
-            result_np = dict_of_ndarray_to_recarray(self.intrinsic_table)
-            f.create_dataset("intrinsic_table", data=result_np)
+                # Check if there is extrinsic_table
+                gp = self.grid_points[0]
+                extrinsic_table &= len(gp.extrinsic_table) > 0
+
+                # Create "grid_points" group to hold self.grid_points
+                group_grid_points_raw = \
+                    f.create_group("grid_points", track_order=True)
+
+                for i, gp in enumerate(self.grid_points):
+                    group_gp = group_grid_points_raw.create_group(str(i))
+
+                    # Add intrinsic_table
+                    it = dict_of_ndarray_to_recarray(gp.intrinsic_table)
+                    group_gp.create_dataset("intrinsic_table", data=it)
+
+                    # Add extrinsic_table
+                    if extrinsic_table:
+                        et = dict_of_ndarray_to_recarray(gp.extrinsic_table)
+                        group_gp.create_dataset("extrinsic_table",
+                                                data=et,
+                                                compression=compression)
+
+                    # Add xml_filename
+                    group_gp.attrs["xml_filename"] = gp.xml_filename
+
+                # Combine intrinsic parameters into "intrinsic_table" dataset
+                result_np = dict_of_ndarray_to_recarray(self.intrinsic_table)
+                f.create_dataset("intrinsic_table", data=result_np)
 
-            # Create virtual dataset for "extrinsic_samples"
-            if extrinsic_table:
-                gps = f["grid_points"]
-                ds0 = f["grid_points/0/extrinsic_table"]
-                n_samples = np.array(
-                    [gp["extrinsic_table"].shape[0] for gp in gps.values()])
-                n_samples = np.cumsum(n_samples)
-                n_samples = np.concatenate([[0], n_samples])
-                layout = h5py.VirtualLayout(shape=(n_samples[-1], ),
-                                            dtype=ds0.dtype)
-
-                for i, gp in enumerate(gps.values()):
-                    vsource = h5py.VirtualSource(gp["extrinsic_table"])
-                    layout[n_samples[i]:n_samples[i+1]] = vsource
+                # Create virtual dataset for "extrinsic_samples"
+                if extrinsic_table:
+                    gps = f["grid_points"]
+                    ds0 = f["grid_points/0/extrinsic_table"]
+                    n_samples = np.array(
+                        [gp["extrinsic_table"].shape[0] for gp in gps.values()])  # noqa: E501
+                    n_samples = np.cumsum(n_samples)
+                    n_samples = np.concatenate([[0], n_samples])
+                    layout = h5py.VirtualLayout(shape=(n_samples[-1], ),
+                                                dtype=ds0.dtype)
+
+                    for i, gp in enumerate(gps.values()):
+                        vsource = h5py.VirtualSource(gp["extrinsic_table"])
+                        layout[n_samples[i]:n_samples[i+1]] = vsource
 
-                f.create_virtual_dataset('extrinsic_samples', layout)
+                    f.create_virtual_dataset('extrinsic_samples', layout)
 
-            # Save event_info and injection_info
+            # Save event_info, injection_info, and config_info
             for attr in ["event_info", "injection_info", "config_info"]:
                 try:
                     x = getattr(self, attr)
                     g = f.create_group(attr)
                     dict_to_hdf_group(x, g)
                 except AttributeError:
                     pass
 
+            # Save posterior_samples
+            try:
+                data = dict_of_ndarray_to_recarray(self.posterior_samples)
+                f.create_dataset("posterior_samples", data=data)
+            except AttributeError:
+                pass
+
     def do_interpolate_marg_log_likelihood_m1m2(
             self,
             method="linear-scipy",
             gaussian_sigma_to_grid_size_ratio=0.5
             ):
         """
         Perfom triangular interpolation of marg_log_likelihood in
@@ -735,7 +757,123 @@
             prob /= np.sum(prob)
 
             m = [{"m1": m1[i], "m2": m2[i]} for i in range(len(m1))]
             # m_samples = np.random.choice(m, size=N, p=prob)
             m_samples = np.random.choice(m, size=N, p=prob, replace=False)
             m1, m2 = np.array([[x["m1"], x["m2"]] for x in m_samples]).T
             self.samples = {"mass_1": m1, "mass_2": m2}
+
+    def generate_posterior_samples(self,
+                                   N=5000,
+                                   method="gaussian",
+                                   gaussian_sigma_to_grid_size_ratio=1.0,
+                                   em_bright_compatible=True):
+        """
+        Generate posterior samples.
+        The generated samples are saved in self.samples
+
+        Parameters
+        ----------
+        N: int
+            Number of samples to generate
+            Default: 5000
+
+        method: str
+            Method to generate samples
+            Default: "gaussian"
+
+        gaussian_sigma_to_grid_size_ratio: float
+            Ratio of sigma to grid size
+            Default: 1.0
+
+        em_bright_compatible: bool
+            If True, generate samples compatible with EM_BRIGHT
+            Default: True
+
+        """
+        if method == "gaussian":
+            grid_levels = np.unique(self.iteration)
+            cov = {}
+            for gl in grid_levels:
+                mask = self.iteration == gl
+                sigma_x1 = grid_separation_min(
+                    self.x1[mask]) * gaussian_sigma_to_grid_size_ratio
+                sigma_x2 = grid_separation_min(
+                    self.x2[mask]) * gaussian_sigma_to_grid_size_ratio
+                cov[gl] = np.diag([sigma_x1**2, sigma_x2**2])
+
+            # Compute likelihood at each grid point
+            likelihood = np.exp(self.marg_log_likelihood)
+            sum_likelihood = np.sum(likelihood)
+
+            # Compute number of samples for each grid point
+            N_multinomial = multinomial(N*20, likelihood/sum_likelihood)
+            N_per_grid_point = N_multinomial.rvs(1)[0]
+
+            # Generate samples
+            samples = np.zeros([0, 2])
+            for x1, x2, lh, gl, n in zip(self.x1,
+                                         self.x2,
+                                         likelihood,
+                                         self.iteration,
+                                         N_per_grid_point):
+                samples = np.concatenate([
+                    samples,
+                    np.random.multivariate_normal([x1, x2], cov[gl], n)
+                    ])
+            x1, x2 = samples.T
+
+            # Mask out the samples outside the region of interest
+            if self.grid_coordinates[0] == "chirp_mass":
+                x1_min = 0.0
+            else:
+                raise ValueError("Unknown grid coordinate x1")
+
+            if self.grid_coordinates[1] == "mass_ratio":
+                x2_max = 1.0
+                x2_min = 0.0
+            elif self.grid_coordinates[1] == "symmetric_mass_ratio":
+                x2_max = 0.25
+                x2_min = 0.0
+            else:
+                raise ValueError("Unknown grid coordinate x2")
+
+            mask = x2 <= x2_max
+            mask &= x2 > x2_min
+            mask &= x1 > x1_min
+
+            x1, x2 = x1[mask], x2[mask]
+
+            x = Mass_Spin.from_x1x2(x1,
+                                    x2,
+                                    grid_coordinates=self.grid_coordinates)
+
+            # An ad-hoc cut on the mass_1
+            mask_m1_max = x.mass_1 < 500
+
+            # Re-weight the samples according to the Jacobian such that
+            # it has a uniform prior in m1-m2 space
+            # Reference: https://dcc.ligo.org/LIGO-T2300198
+            weight = x.jacobian_m1m2_by_x1x2[mask_m1_max]
+            weight /= np.sum(weight)
+
+            m = {"mass_1": x.mass_1[mask_m1_max],
+                 "mass_2": x.mass_2[mask_m1_max]}
+
+            m = dict_of_ndarray_to_recarray(m)
+            samples = np.random.choice(m, size=N, p=weight, replace=False)
+            samples = recarray_to_dict_of_ndarray(samples)
+
+            if em_bright_compatible:
+                shape = samples["mass_1"].shape
+                event_spin = self.event_info["event_spin"]
+                spin_1z = np.broadcast_to(event_spin["spin_1z"], shape)
+                spin_2z = np.broadcast_to(event_spin["spin_2z"], shape)
+
+                samples["mass_1_source"] = samples["mass_1"]
+                samples["mass_2_source"] = samples["mass_2"]
+                samples["spin_1z"] = spin_1z
+                samples["spin_2z"] = spin_2z
+
+                self.posterior_samples = samples
+            else:
+                self.posterior_samples = samples
```

### Comparing `read_rapidpe-0.5.4/read_rapidpe/transform.py` & `read_rapidpe-0.5.5/read_rapidpe/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,14 +161,30 @@
     def m1m2(self):
         return self._mass_1, self._mass_2
 
     @property
     def mcq(self):
         return self.chirp_mass, self.mass_ratio
 
+    @property
+    def jacobian_x1x2_by_m1m2(self):
+        if self.grid_coordinates[0] == "chirp_mass":
+            if self.grid_coordinates[1] == "mass_ratio":
+                return self.jacobian_mcq_by_m1m2(self._mass_1, self._mass_2)
+            elif self.grid_coordinates[1] == "symmetric_mass_ratio":
+                return self.jacobian_mceta_by_m1m2(self._mass_1, self._mass_2)
+            else:
+                raise ValueError("Invalid grid_coordinates")
+        else:
+            raise ValueError("Invalid grid_coordinates")
+
+    @property
+    def jacobian_m1m2_by_x1x2(self):
+        return 1/self.jacobian_x1x2_by_m1m2
+
     @classmethod
     def _norm_sym_ratio(cls, eta):
         """
         Copied from https://git.ligo.org/rapidpe-rift/rapidpe/-/blob/master/rapid_pe/lalsimutils.py
         """  # noqa E501
         # Assert phyisicality
         assert np.all(eta <= 0.25)
```

### Comparing `read_rapidpe-0.5.4/PKG-INFO` & `read_rapidpe-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read-rapidpe
-Version: 0.5.4
+Version: 0.5.5
 Summary: Read and analyse results generated by rapidpe-rift-pipe
 Home-page: https://github.com/c0rychu/read-rapidpe
 Author: Cory Chu
 Author-email: cory@gwlab.page
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

