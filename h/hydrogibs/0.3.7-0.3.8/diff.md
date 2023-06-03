# Comparing `tmp/hydrogibs-0.3.7.tar.gz` & `tmp/hydrogibs-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.3.7.tar", last modified: Tue May 23 16:57:37 2023, max compression
+gzip compressed data, was "hydrogibs-0.3.8.tar", last modified: Sat Jun  3 17:09:21 2023, max compression
```

## Comparing `hydrogibs-0.3.7.tar` & `hydrogibs-0.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.7/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)     1558 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.3.7/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    15081 2023-05-23 16:49:06.000000 hydrogibs-0.3.7/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5176 2023-05-16 12:38:08.000000 hydrogibs-0.3.7/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.7/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     9762 2023-05-22 14:18:40.000000 hydrogibs-0.3.7/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.7/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.3.7/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.3.7/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.7/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1558 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-05-23 16:57:37.000000 hydrogibs-0.3.7/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      535 2023-05-23 16:57:08.000000 hydrogibs-0.3.7/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-05-23 16:57:37.954574 hydrogibs-0.3.7/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:09:21.517545 hydrogibs-0.3.8/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.8/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1615 2023-06-03 17:09:21.517545 hydrogibs-0.3.8/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.3.8/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:09:21.513545 hydrogibs-0.3.8/hydrogibs/
+-rwxrwxr-x   0 axel      (1000) axel      (1000)    14055 2023-06-03 17:07:49.000000 hydrogibs-0.3.8/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     5176 2023-06-03 17:06:24.000000 hydrogibs-0.3.8/hydrogibs/ModelApp.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.8/hydrogibs/ModelTemplate.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     7892 2023-06-03 17:08:00.000000 hydrogibs-0.3.8/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.8/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-05-24 13:52:28.000000 hydrogibs-0.3.8/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      121 2023-06-03 17:06:41.000000 hydrogibs-0.3.8/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.8/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:09:21.513545 hydrogibs-0.3.8/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1615 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      592 2023-06-03 17:05:24.000000 hydrogibs-0.3.8/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-06-03 17:09:21.517545 hydrogibs-0.3.8/setup.cfg
```

### Comparing `hydrogibs-0.3.7/LICENSE` & `hydrogibs-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.7/PKG-INFO` & `hydrogibs-0.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.7
-Summary: A small hydrology package created for a class project with Christophe Ancey
+Version: 0.3.8
+Summary: A small hydrology package created for a class project with Christophe Ancey: http://fr.ancey.ch/cours/masterGC/cours-hydraulique.pdf
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `hydrogibs-0.3.7/README.md` & `hydrogibs-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.7/hydrogibs/GR4.py` & `hydrogibs-0.3.8/hydrogibs/GR4.py`

 * *Files 19% similar despite different names*

```diff
@@ -117,22 +117,32 @@
         X1 (float)  [-] : dQ = X1 * dPrecipitations
         X2 (float)  [mm]: Initial abstraction (vegetation interception)
         X3 (float) [1/h]: Sub-surface water volume emptying rate dQs = X3*V*dt
         X4 (float)  [h] : the hydrogram's raising time
     """
 
     def __init__(self,
-                 X1: float,
-                 X2: float,
-                 X3: float,
-                 X4: float,
+                 X1: float = ...,
+                 X2: float = ...,
+                 X3: float = ...,
+                 X4: float = ...,
                  surface: float = 1,
                  initial_volume: float = 0,
                  transfer_function: Callable = None) -> None:
 
+        if isinstance(X1, str):
+            preset = X1
+            if preset in preset_params:
+                X1, X2, X3, X4 = preset_params[preset].values()
+            else:
+                raise KeyError(
+                    f"{preset} does not match an available preset catchment."
+                    f"\nAvailable presets: {set(preset_params.keys())}"
+                )
+
         assert 0 <= X1 <= 1, "Runoff coefficient must be within [0 : 1]"
         assert 0 <= X2, "Initial abstraction must be positive"
         assert 0 <= X3 <= 1, "Emptying rate must be within [0 : 1]"
         assert 0 <= X4, "Raising time must be positive"
 
         self.X1 = X1
         self.X2 = X2
@@ -145,88 +155,48 @@
                                   else _transfer_func)
         self.initial_volume = initial_volume
 
     def __matmul__(self, rain):
         return rain @ self
 
 
-class Laval(Catchment):
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(57.6/100, 7.8, 2.4/100, 0.38,
-                         *args, **kwargs)
-
-
-class Erlenbach(Catchment):
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(46.5/100, 13.6, 16.2/100, 0.63,
-                         *args, **kwargs)
-
-
-class Rimbaud(Catchment):
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(35.4/100, 40, 2.28/100, 1.07,
-                         *args, **kwargs)
-
-
-class Latte(Catchment):
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(14.4/100, 75.4, 3.96/100, 0.78,
-                         *args, **kwargs)
+def _read_presets():
 
+    presets = dict()
 
-class Sapine(Catchment):
+    with open("hydrogibs/data/GR4presets.csv") as file:
+        lines = file.readlines()
 
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(15.7/100, 71.1, 0.90/100, 1.03,
-                         *args, **kwargs)
-
-
-class Rietholzbach(Catchment):
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(26.5/100, 17, 2.82/100, 1.11,
-                         *args, **kwargs)
-
-
-class Lumpenenbach(Catchment):
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(22.6/100, 12.2, 9.6/100, 0.5,
-                         *args, **kwargs)
-
-
-class Vogelbach(Catchment):
-
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(31.4/100, 11.5, 5.88/100, 0.64,
-                         *args, **kwargs)
+    for line in lines[2:]:
+        line = line.replace('\n', '')
+        data = [
+            float(d) if d.replace('.', '', 1).isdigit()
+            else d
+            for d in line.split(',')
+        ]
+        name, _, _, x1, x2, x3, x4, _, _ = data
+        presets[name] = dict(X1=x1/100, X2=x2, X3=x3/100, X4=x4)
 
+    return presets
 
-class Brusquet(Catchment):
 
-    def __init__(self, *args, **kwargs) -> None:
-        super().__init__(13.8/100, 22.4, 0.72/100, 1.63,
-                         *args, **kwargs)
+preset_params = _read_presets()
 
 
-presets = dict(
-    Laval=Laval,
-    Erlenbach=Erlenbach,
-    Rimbaud=Rimbaud,
-    Latte=Latte,
-    Sapine=Sapine,
-    Rietholzbach=Rietholzbach,
-    Lumpenenbach=Lumpenenbach,
-    Vogelbach=Vogelbach,
-    Brusquet=Brusquet
-)
+# preset = dict(
+#     Laval=Laval,
+#     Erlenbach=Erlenbach,
+#     Rimbaud=Rimbaud,
+#     Latte=Latte,
+#     Sapine=Sapine,
+#     Rietholzbach=Rietholzbach,
+#     Lumpenenbach=Lumpenenbach,
+#     Vogelbach=Vogelbach,
+#     Brusquet=Brusquet
+# )
 
 
 class Event(ModelTemplate.Event):
     """
     Stores all relevant results of a GR4h calculation
 
     basic class instead of dataclass, namedtuple or dataframe is used
@@ -326,15 +296,15 @@
                 lw=1,
                 ls='-.',
                 color=c5,
                 label="Écoulements hypodermiques",
                 zorder=9
             )
             ax1.set_ylabel("$Q$ (m³/s)", color=c1)
-            ax1.set_xlabel("Temps (h)")
+            ax1.set_xlabel("t (h)")
             ax1.set_xlim((0, tmax if tmax else 1))
             ax1.set_ylim((0, Qmax*1.1 if Qmax else 1))
             ax1.tick_params(colors=c1, axis='y')
 
             lineP, = ax2.step(
                 time,
                 rain,
@@ -501,26 +471,17 @@
             f"\tInitial  abstraction: {X2v:.2e}\n"
             f"Precipitation volume: {Ptot:.2e}\n\n"
         )
 
     return Event(time, dP, V, dTp+dTv, Qp, Qv, Qp+Qv)
 
 
-def GR4_demo(kind: Literal["array", "block"] = "array"):
+def GR4_demo():
 
-    if kind == "block":
-        rain = BlockRain(50, duration=1.8, observation_span=5.8)
-    else:
-        time = np.linspace(0, 10, 1000)
-        rainfall = np.full_like(time, 50)
-        rainfall[(3 <= time) & (time <= 7) | (time >= 9)] = 0
-        rain = Rain(
-            time=time,
-            rainfall=rainfall
-        )
-    Catchment(8/100, 40, 0.1, 1) @ rain
-    # GR4h(Catchment(8/100, 40, 0.1, 1), rain).App()
-    App(Catchment(8/100, 40, 0.1, 1), rain)
+    rain = BlockRain(50, duration=1.8, observation_span=5.8)
+    catchment = Catchment("Rimbaud")
+    # event = catchment @ rain
+    App(catchment, rain)
 
 
 if __name__ == "__main__":
-    GR4_demo("block")
+    GR4_demo()
```

### Comparing `hydrogibs-0.3.7/hydrogibs/ModelApp.py` & `hydrogibs-0.3.8/hydrogibs/ModelApp.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.7/hydrogibs/ModelTemplate.py` & `hydrogibs-0.3.8/hydrogibs/ModelTemplate.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.7/hydrogibs/QDF.py` & `hydrogibs-0.3.8/hydrogibs/QDF.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,36 @@
 from typing import Literal, Union
 from matplotlib import pyplot as plt
 from hydrogibs.ModelApp import ModelApp, Entry
 from warnings import warn
 from scipy.optimize import least_squares
 
 
+def _read_coeficients(kind="mean"):
+
+    with open(f"hydrogibs/data/QDFcoefs_{kind}.csv") as file:
+        lines = file.readlines()
+
+    coefs = dict()
+    for line in lines[2:]:
+        name, *values = line.split(',')
+        values = [float(v) for v in values]
+        coefs[name] = dict(
+            A=values[:3],
+            B=values[3:6],
+            C=values[6:]
+        )
+
+    return coefs
+
+
+coefs_mean = _read_coeficients('mean')
+coefs_threshold = _read_coeficients('threshold')
+
+
 class Catchment:
     """
     Stores a QDF catchment's parameters.
 
     Creates a QDF event object when called with a QDF Rain object:
     >>> qdf = QDF(catchment, rain)
     Creates an Event object when applied to a Rain object
@@ -23,50 +45,14 @@
                                     - 'vandenesse'
         specific_duration (float) [h]:    Specific duration
         surface           (float) [km]:   Length of the thalweg
         length            (float) [%]:    Mean slope of the thalweg
         mean_slope        (float) [km^2]: Catchment surface
     """
 
-    _coefs_threshold = dict(
-
-        soyans=dict(
-            A=(2.57, 4.86, 0),
-            B=(2.10, 2.10, 0.050),
-            C=(1.49, 0.660, 0.017)),
-
-        florac=dict(
-            A=(3.05, 3.53, 0),
-            B=(2.13, 2.96, 0.010),
-            C=(2.78, 1.77, 0.040)),
-
-        vandenesse=dict(
-            A=(3.970, 6.48, 0.010),
-            B=(1.910, 1.910, 0.097),
-            C=(3.674, 1.774, 0.013))
-    )
-
-    _coefs_mean = dict(
-
-        soyans=dict(
-            A=(0.87, 4.60, 0),
-            B=(1.07, 2.50, 0.099),
-            C=(0.569, 0.690, 0.046)),
-
-        florac=dict(
-            A=(1.12, 3.56, 0),
-            B=(0.95, 3.18, 0.039),
-            C=(1.56, 1.91, 0.085)),
-
-        vandenesse=dict(
-            A=(2.635, 6.19, 0.016),
-            B=(1.045, 2.385, 0.172),
-            C=(1.083, 1.75, 0))
-    )
-
     def __init__(self,
                  model: Literal["soyans", "florac", "vandenesse"],
                  specific_duration: float = None,
                  surface: float = None,
                  length: float = None,
                  mean_slope: float = None) -> None:
 
@@ -96,27 +82,26 @@
     >>> event = rain @ catchment
 
     Args:
 
     """
 
     def __init__(self,
-                 duration: Union[float, np.ndarray],
+                 duration: float,
                  return_period: float,
                  specific_discharge: float,
                  discharge_Q10: float,
-                 dt: float = None,
+                 dt: float = .0,
                  observation_time: float = None):
 
         self.duration = duration
         self.return_period = return_period
         self.specific_discharge = specific_discharge
         self.discharge_Q10 = discharge_Q10
-
-        self.dt = dt if dt is not None else duration/100
+        self.dt = dt if dt else duration/100
         self.tf = (observation_time if observation_time is not None
                    else 5 * duration)
 
         assert 0 <= return_period
         assert 0 <= specific_discharge
         assert 0 <= discharge_Q10
 
@@ -181,15 +166,15 @@
     if catchment is None:
         catchment = Catchment("soyans",
                               specific_duration=1,
                               surface=1.8,
                               length=2,
                               mean_slope=9.83/100)
     if rain is None:
-        rain = Rain(np.linspace(0, 24), 100, 0.3, 0.3)
+        rain = Rain(1, 100, 0.3, 0.3)
 
     if hasattr(catchment, "specific_duration"):
         entries = [("catchment", "specific_duration", "h", "ds")]
     else:
         entries = [
             ("catchment", "surface", "km^2", "S"),
             ("catchment", "length", "km", "L"),
@@ -209,18 +194,18 @@
         entries=entries
     )
 
 
 def qdf(catchment, rain):
 
     constants_threshold = list(
-        catchment._coefs_threshold[catchment.model].values()
+        coefs_threshold[catchment.model.capitalize()].values()
     )
     constants_mean = list(
-        catchment._coefs_mean[catchment.model].values()
+        coefs_mean[catchment.model.capitalize()].values()
     )
 
     if hasattr(catchment, "specific_duration"):
         ds = catchment.specific_duration
     else:
         ds = Turraza(
             catchment.surface,
@@ -230,49 +215,14 @@
 
     discharge_peak = discharge(Q10=rain.discharge_Q10,
                                Qsp=rain.specific_discharge,
                                T=rain.return_period,
                                constants=constants_mean,
                                d=rain.duration,
                                ds=ds)
-    _d = np.linspace(0, 5)
-    print(f"{rain.discharge_Q10 = }")
-    print(f"{rain.specific_discharge = }")
-    print(f"{rain.return_period = }")
-    print(f"{ds = }")
-    with plt.style.context("ggplot"):
-        plt.figure(figsize=(3, 3))
-        plt.plot(_d, discharge(Q10=rain.discharge_Q10,
-                               Qsp=rain.specific_discharge,
-                               T=rain.return_period,
-                               constants=constants_mean,
-                               d=_d,
-                               ds=ds), label="Q$_{10}$ = 1.3 m$^3$/s")
-        print(discharge(Q10=rain.discharge_Q10,
-                        Qsp=rain.specific_discharge,
-                        T=rain.return_period,
-                        constants=constants_mean,
-                        d=1,
-                        ds=ds))
-        print(discharge(Q10=2,
-                        Qsp=2,
-                        T=rain.return_period,
-                        constants=constants_mean,
-                        d=1,
-                        ds=ds))
-        plt.plot(_d, discharge(Q10=2,
-                               Qsp=2,
-                               T=rain.return_period,
-                               constants=constants_mean,
-                               d=_d,
-                               ds=ds), label="Q$_{10}$ = 2.0 m$^3$/s")
-        plt.xlabel("Durée de la pluie (h)")
-        plt.ylabel("Débit de pointe (m$^3$/s)")
-        plt.legend()
-        plt.show()
 
     dt = rain.dt
     time = np.arange(0, rain.tf, step=rain.dt)
     Q = np.full_like(time, discharge_peak)
 
     ds = catchment.specific_duration
     i = time <= ds
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hydrogibs-0.3.7/hydrogibs/RationalMethod.py` & `hydrogibs-0.3.8/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.7/hydrogibs/SoCoSe.py` & `hydrogibs-0.3.8/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.7/hydrogibs/misc.py` & `hydrogibs-0.3.8/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.7/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.3.8/hydrogibs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.7
-Summary: A small hydrology package created for a class project with Christophe Ancey
+Version: 0.3.8
+Summary: A small hydrology package created for a class project with Christophe Ancey: http://fr.ancey.ch/cours/masterGC/cours-hydraulique.pdf
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `hydrogibs-0.3.7/pyproject.toml` & `hydrogibs-0.3.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "hydrogibs"
-version = "0.3.7"
+version = "0.3.8"
 authors = [
   { name="axel Giboulot", email="axel.giboulot@epfl.ch" },
 ]
-description = "A small hydrology package created for a class project with Christophe Ancey"
+description = "A small hydrology package created for a class project with Christophe Ancey: http://fr.ancey.ch/cours/masterGC/cours-hydraulique.pdf"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

