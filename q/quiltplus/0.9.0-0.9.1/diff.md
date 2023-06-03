# Comparing `tmp/quiltplus-0.9.0.tar.gz` & `tmp/quiltplus-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltplus-0.9.0.tar", max compression
+gzip compressed data, was "quiltplus-0.9.1.tar", max compression
```

## Comparing `quiltplus-0.9.0.tar` & `quiltplus-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.0/LICENSE.md
--rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.0/README.md
--rw-r--r--   0        0        0      837 2023-05-31 14:03:42.570360 quiltplus-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      631 2023-05-31 14:03:42.572187 quiltplus-0.9.0/quiltplus/__init__.py
--rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.0/quiltplus/ignore.py
--rw-r--r--   0        0        0     2059 2023-05-31 14:03:42.573471 quiltplus-0.9.0/quiltplus/local.py
--rw-r--r--   0        0        0     3805 2023-05-31 14:03:42.575123 quiltplus-0.9.0/quiltplus/package.py
--rw-r--r--   0        0        0      457 2023-05-31 14:03:42.576091 quiltplus-0.9.0/quiltplus/path.py
--rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.0/quiltplus/property.py
--rw-r--r--   0        0        0      593 2023-05-31 14:03:42.577524 quiltplus-0.9.0/quiltplus/registry.py
--rw-r--r--   0        0        0      606 2023-05-31 14:03:42.578377 quiltplus-0.9.0/quiltplus/resource.py
--rw-r--r--   0        0        0      366 2023-05-31 14:03:42.579049 quiltplus-0.9.0/quiltplus/root.py
--rw-r--r--   0        0        0     1176 2023-05-31 14:03:42.579492 quiltplus-0.9.0/quiltplus/type.py
--rw-r--r--   0        0        0     1483 2023-05-31 14:03:42.579909 quiltplus-0.9.0/quiltplus/uri.py
--rw-r--r--   0        0        0      573 2023-05-31 14:03:42.580666 quiltplus-0.9.0/quiltplus/versions.py
--rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 quiltplus-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.1/LICENSE.md
+-rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.1/README.md
+-rw-r--r--   0        0        0      908 2023-06-03 15:47:57.984367 quiltplus-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-06-03 22:59:04.000000 quiltplus-0.9.1/quiltplus/__init__.py
+-rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.1/quiltplus/ignore.py
+-rw-r--r--   0        0        0     2219 2023-06-03 15:46:39.662073 quiltplus-0.9.1/quiltplus/local.py
+-rw-r--r--   0        0        0     3189 2023-06-03 15:46:39.662850 quiltplus-0.9.1/quiltplus/package.py
+-rw-r--r--   0        0        0      523 2023-06-03 15:46:39.663694 quiltplus-0.9.1/quiltplus/path.py
+-rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.1/quiltplus/property.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:46:39.663802 quiltplus-0.9.1/quiltplus/py.typed
+-rw-r--r--   0        0        0      609 2023-06-03 15:46:39.664625 quiltplus-0.9.1/quiltplus/registry.py
+-rw-r--r--   0        0        0      708 2023-06-03 15:46:39.666292 quiltplus-0.9.1/quiltplus/resource.py
+-rw-r--r--   0        0        0      366 2023-05-31 14:03:42.579049 quiltplus-0.9.1/quiltplus/root.py
+-rw-r--r--   0        0        0     1186 2023-06-03 15:46:39.667587 quiltplus-0.9.1/quiltplus/type.py
+-rw-r--r--   0        0        0     1459 2023-06-03 15:46:39.668475 quiltplus-0.9.1/quiltplus/uri.py
+-rw-r--r--   0        0        0      589 2023-06-03 15:46:39.669427 quiltplus-0.9.1/quiltplus/versions.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 quiltplus-0.9.1/PKG-INFO
```

### Comparing `quiltplus-0.9.0/LICENSE.md` & `quiltplus-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.0/README.md` & `quiltplus-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.0/pyproject.toml` & `quiltplus-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltplus"
-version = "0.9.0"
+version = "0.9.1"
 description = "Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["yaml", "api", "resource", "quilt"]
 packages = [
    { include = "quiltplus" }
@@ -15,21 +15,23 @@
 urllib3 = "<2"
 quilt3 = "^5.1.0"
 trio = "^0.22.0"
 isort = "^5.12.0"
 asyncclick = "^8.1.3.4"
 pytest-cov = "^4.0.0"
 anyio = "^3.7.0"
-typing-extensions = "^4.5.0"
-un-yaml = ">0.0.0"
+typing-extensions = "^4.6.3"
+un-yaml = ">=0.2.0"
 # udc = {git = "https://github.com/data-yaml/udc.git", rev = "main"}
 tzlocal = "^5.0.1"
 
-
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest-trio = "^0.8.0"
-pytest-watcher = "^0.2.6"
+pytest-watcher = "^0.3.1"
+mypy = "^1.3.0"
+types-pyyaml = "^6.0.12.10"
+types-tzlocal = "^5.0.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `quiltplus-0.9.0/quiltplus/ignore.py` & `quiltplus-0.9.1/quiltplus/ignore.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.0/quiltplus/local.py` & `quiltplus-0.9.1/quiltplus/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,38 +16,43 @@
             tmpdir = Path(tmpdirname)
             yield (tmpdir)
             logging.debug(f"Removing {tmpdirname} on {platform.system()}")
 
     @staticmethod
     def OpenDesktop(dest: str):
         if platform.system() == "Windows":
-            os.startfile(dest)
+            os.startfile(dest)  # type: ignore
         elif platform.system() == "Darwin":
             subprocess.Popen(["open", "-R", dest])
         else:
             subprocess.Popen(["xdg-open", dest])
         return dest
 
     def __init__(self, attrs: dict):
         super().__init__(attrs)
         for tmp in QuiltLocal.TempDir():
             self.last_path = tmp
 
-    def check_dir(self, path: Path = None):
+    def check_dir(self, path: Path | None = None):
         if not path:
             return self.last_path
 
         self.last_path = path
         if not path.exists():
             logging.warn(f"Path does not exist: {path}")
             path.mkdir(parents=True, exist_ok=True)
         elif not path.is_dir():
             raise ValueError(f"Path is not a directory: {path}")
         return path
 
+    def check_path(self, opts: dict):
+        path = opts.get(QuiltLocal.K_PTH)
+        print(path)
+        return self.check_dir(path)
+
     def local_path(self, *paths: str):
         p = self.check_dir()
         for path in paths:
             p = p / path
 
         p.mkdir(parents=True, exist_ok=True)
         return p
```

### Comparing `quiltplus-0.9.0/quiltplus/package.py` & `quiltplus-0.9.1/quiltplus/package.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Resource-oriented version of a Quilt Package
 
 import logging
 import shutil
 
-from quilt3 import Package
-from typing_extensions import Self
+from quilt3 import Package  # type: ignore
+from typing_extensions import Self, Type
 
 from .local import QuiltLocal
 from .uri import QuiltUri
 
 
 class QuiltPackage(QuiltLocal):
     METHOD_NAMES = "get list diff patch put".split(" ")
 
     @classmethod
-    def FromURI(cls: Self, uri: str):
+    def FromURI(cls: Type[Self], uri: str):
         attrs = QuiltUri.AttrsFromUri(uri)
         return cls(attrs)
 
     def __init__(self, attrs: dict):
         super().__init__(attrs)
         self.hash = self.attrs.get(QuiltUri.K_HASH)
 
@@ -47,69 +47,53 @@
             return [x for sub in diffs.values() for x in sub]
         q = await self.remote_pkg()
         return list(q.keys())
 
     async def list(self, opts: dict = {}):
         return [self.path_uri(k) for k in await self.child()]
 
-    async def diff(self):
+    async def diff(self, opts: dict = {}):
         logging.debug(f"\ndiff.local_files\n{self.local_files()}")
         q_remote = await self.remote_pkg()
         logging.debug(f"diff.remote_keys {q_remote.keys()}")
         q_local = await self.local_pkg()
         logging.debug(f"diff.local_keys {q_local.keys()}")
         diffs = q_remote.diff(q_local)
         logging.debug(f"diff: {diffs}")
         return {"added": diffs[0], "modified": diffs[1], "deleted": diffs[2]}
 
-    def check_path(self, opts: dict):
-        if QuiltUri.K_PTH in opts:
-            self.check_dir(opts[QuiltUri.K_PTH])
-        return self.dest()
-
     async def get(self, opts: dict = {}):
         dest = self.check_path(opts)
         q = await self.remote_pkg()
         q.fetch(dest=dest)
         return dest
 
-    async def push_args(self, opts: dict) -> dict:
+    async def commit(self, opts: dict = {}):  # create new empty package
+        pass
+
+    async def push(self, q: Package, opts: dict):
+        """Generic handler for all push methods"""
         kwargs = {
             "registry": self.registry,
-            "force": opts.get("force", False),
+            "force": True,
             "message": opts.get("message", f"{__name__} {QuiltUri.Now()} @ {opts}"),
         }
-        if "commit" in opts:
-            await self.commit(opts)
-        return kwargs
-
-    async def commit(self, opts: dict = {}):  # create new empty package
-        q = await self.local_pkg()
-        [q.set(f) for f in self.config.get_stage(adds=True)]
-        [q.delete(f) for f in self.config.get_stage(adds=False)]
-        result = q.build(self.package)
-        return result
-
-    async def push(self, opts: dict, put=True):
-        """Generic handler for all push methods"""
-        q = await self.remote_pkg()  # reset to latest
-        if put:
-            [q.delete(f) for f in await self.child()]  # clean slate; replace with dest
         q.set_dir(".", self.check_path(opts))
         q.build(self.package)
-        args = await self.push_args(opts)
-        result = q.push(self.package, **args)
+        result = q.push(self.package, **kwargs)
         return result
 
     async def put(self, opts: dict = {}):
-        return await self.push(opts, put=True)
+        q = Package()
+        return await self.push(q, opts)
 
     async def patch(self, opts: dict = {}):
-        """Update the latest version of the remote package with the latest commit"""
-        return await self.push(opts, put=False)
+        """Use contents of directory to (merge) update the remote package"""
+        q = await self.remote_pkg()  # reset to latest
+        return await self.push(q, opts)
 
     def delete(self):  # remove local cache
         return shutil.rmtree(self.last_path)
 
     async def call(self, method: str = "get", opts={}):
         attr_method = getattr(self, method)
         return await attr_method(opts)
```

### Comparing `quiltplus-0.9.0/quiltplus/registry.py` & `quiltplus-0.9.1/quiltplus/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quilt3 import list_packages
+from quilt3 import list_packages  # type: ignore
 
 from .root import QuiltRoot
 
 
 class QuiltRegistry(QuiltRoot):
     """Creates registry object from QuiltID."""
```

### Comparing `quiltplus-0.9.0/quiltplus/resource.py` & `quiltplus-0.9.1/quiltplus/resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import logging
+
+import yaml
+
 from .package import QuiltPackage
 from .path import QuiltPath
 from .property import QuiltProperty
 from .registry import QuiltRegistry
 from .uri import QuiltUri
 from .versions import QuiltVersions
 
@@ -12,14 +16,15 @@
     QuiltUri.K_BKT: QuiltRegistry,
     QuiltUri.K_VER: QuiltVersions,
 }
 
 
 def QuiltResource(attrs: dict):
     type = QuiltUri.Type(attrs)
+    logging.debug(f"QuiltResource: type={type} for\n{yaml.dump(attrs)}")
     klass = KLASS_MAP[type]
     return klass(attrs)
 
 
 def QuiltResourceURI(uri: str):
     attrs = QuiltUri.AttrsFromUri(uri)
     return QuiltResource(attrs)
```

### Comparing `quiltplus-0.9.0/quiltplus/type.py` & `quiltplus-0.9.1/quiltplus/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     @staticmethod
     def Type(attrs: dict) -> str:
         type = QuiltType.BaseType(attrs)
         if type != QuiltType.K_PKG:
             return type
         pkg = attrs.get(QuiltType.K_PKG)
-        if QuiltType.SEP_HASH in pkg or QuiltType.SEP_TAG in pkg:
+        if pkg and (QuiltType.SEP_HASH in pkg or QuiltType.SEP_TAG in pkg):
             return QuiltType.K_PKG
         return QuiltType.K_VER
 
     @staticmethod
     def Now() -> str:
         tz = get_localzone()
         dt = datetime.now(tz)
```

### Comparing `quiltplus-0.9.0/quiltplus/uri.py` & `quiltplus-0.9.1/quiltplus/uri.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Create Quilt URI from UnURI attributes
 
-from typing_extensions import Self
-from un_yaml import UnUri
+from un_yaml.un_uri import UnUri
 
 from .type import QuiltType
 
 
 class QuiltUri(QuiltType):
-    @staticmethod
-    def FromUnUri(un: UnUri) -> Self:
-        return QuiltUri(un.attrs)
+    @classmethod
+    def FromUnUri(cls, un: UnUri) -> "QuiltUri":
+        return cls(un.attrs)
 
-    @staticmethod
-    def FromUri(uri: str) -> Self:
+    @classmethod
+    def FromUri(cls, uri: str) -> "QuiltUri":
         un = UnUri(uri)
-        return QuiltUri.FromUnUri(un)
+        return cls.FromUnUri(un)
 
     @staticmethod
     def AttrsFromUri(uri: str) -> dict:
         un = UnUri(uri)
         return un.attrs
 
     def __init__(self, attrs: dict):
@@ -26,20 +25,18 @@
         self.uri = attrs.get(UnUri.K_URI)
         self.registry = f"{attrs.get(UnUri.K_PROT)}://{attrs.get(UnUri.K_HOST)}"
         self.package = self.parse_package()
 
     def __repr__(self):
         return f"QuiltUri({self.uri})"
 
-    def __eq__(self, other: Self):
-        return (
-            self.registry == other.registry
-            and self.package == other.package
-            and self.__class__ == other.__class__
-        )
+    def __eq__(self, other: object):
+        if not isinstance(other, QuiltUri):
+            return NotImplemented
+        return self.registry == other.registry and self.package == other.package
 
     def full_package(self):
         return self.attrs.get(QuiltUri.K_PKG)
 
     def split_package(self, key):
         sep = QuiltUri.SEP.get(key)
         pkg = self.full_package()
```

### Comparing `quiltplus-0.9.0/quiltplus/versions.py` & `quiltplus-0.9.1/quiltplus/versions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from quilt3 import list_package_versions
+from quilt3 import list_package_versions  # type: ignore
 
 from .root import QuiltRoot
 
 
 class QuiltVersions(QuiltRoot):
     """Creates versions manager for a package."""
```

### Comparing `quiltplus-0.9.0/PKG-INFO` & `quiltplus-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltplus
-Version: 0.9.0
+Version: 0.9.1
 Summary: Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform
 License: MIT
 Keywords: yaml,api,resource,quilt
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: quilt3 (>=5.1.0,<6.0.0)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
 Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
-Requires-Dist: un-yaml (>0.0.0)
+Requires-Dist: un-yaml (>=0.2.0)
 Requires-Dist: urllib3 (<2)
 Description-Content-Type: text/markdown
 
 # QuiltPlus
 
 ## Next-generation API for Quilt Universal Data Collections
```

