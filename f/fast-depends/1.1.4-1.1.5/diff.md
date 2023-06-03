# Comparing `tmp/fast_depends-1.1.4.tar.gz` & `tmp/fast_depends-1.1.5.tar.gz`

## Comparing `fast_depends-1.1.4.tar` & `fast_depends-1.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/__about__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/__init__.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/construct.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/injector.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/model.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/provider.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/types.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/usage.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.4/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.4/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.4/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.4/README.md
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-1.1.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-1.1.5/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-1.1.5/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-1.1.5/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-1.1.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/__about__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/__init__.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/construct.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/injector.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/model.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/provider.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/types.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/usage.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fast_depends-1.1.5/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-1.1.5/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-1.1.5/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-1.1.5/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-1.1.5/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-1.1.5/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-1.1.5/LICENSE
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-1.1.5/README.md
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 fast_depends-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 fast_depends-1.1.5/PKG-INFO
```

### Comparing `fast_depends-1.1.4/CONTRIBUTING.md` & `fast_depends-1.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/.github/workflows/documentation.yml` & `fast_depends-1.1.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/.github/workflows/publish_coverage.yml` & `fast_depends-1.1.5/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/.github/workflows/publish_pypi.yml` & `fast_depends-1.1.5/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/.github/workflows/tests.yml` & `fast_depends-1.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/fast_depends/construct.py` & `fast_depends-1.1.5/fast_depends/construct.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/fast_depends/injector.py` & `fast_depends-1.1.5/fast_depends/injector.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/fast_depends/model.py` & `fast_depends-1.1.5/fast_depends/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple, List
 
 from pydantic import create_model
 from pydantic.error_wrappers import ErrorList
 from pydantic.fields import ModelField
 
 from fast_depends.library import CustomField
 from fast_depends.types import AnyCallable
@@ -33,14 +33,32 @@
         self.name = name
         # Store the path to be able to re-generate a dependable from it in overrides
         self.path = path
         # Save the cache key at creation to optimize performance
         self.cache_key = (self.call,)
         self.error_model = create_model(getattr(call, "__name__", str(call)))
 
+    @property
+    def real_params(self) -> List[ModelField]:
+        custom = tuple(c.param_name for c in self.custom)
+        return list(filter(lambda x: x.name not in custom, self.params))
+
+    @property
+    def flat_params(self) -> List[ModelField]:
+        params = self.real_params
+        for d in self.dependencies:
+            params.extend(d.flat_params)
+
+        params_unique = []
+        for p in params:
+            if p not in params_unique:
+                params_unique.append(p)
+
+        return params_unique
+
     def cast_response(self, response: Any) -> Tuple[Optional[Any], Optional[ErrorList]]:
         if self.return_field is None:
             return response, []
         return self.return_field.validate(response, {}, loc=RETURN_FIELD)
 
 
 class Depends:
```

### Comparing `fast_depends-1.1.4/fast_depends/usage.py` & `fast_depends-1.1.5/fast_depends/usage.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/fast_depends/utils.py` & `fast_depends-1.1.5/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/fast_depends/library/model.py` & `fast_depends-1.1.5/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/LICENSE` & `fast_depends-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/README.md` & `fast_depends-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/pyproject.toml` & `fast_depends-1.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-1.1.4/PKG-INFO` & `fast_depends-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 1.1.4
+Version: 1.1.5
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

