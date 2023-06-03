# Comparing `tmp/aiodbm-0.2.0a1.tar.gz` & `tmp/aiodbm-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodbm-0.2.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodbm-0.2.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodbm-0.2.0a1.tar` & `aiodbm-0.2.0b1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      221 2023-05-31 12:59:34.028365 aiodbm-0.2.0a1/.coveragerc
--rw-r--r--   0        0        0      964 2023-06-01 00:00:49.918153 aiodbm-0.2.0a1/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-06-01 00:00:49.918153 aiodbm-0.2.0a1/.github/workflows/release.yml
--rw-r--r--   0        0        0      110 2023-05-31 01:31:26.803876 aiodbm-0.2.0a1/.gitignore
--rw-r--r--   0        0        0      477 2023-05-31 13:13:07.581265 aiodbm-0.2.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-06-02 17:34:44.178645 aiodbm-0.2.0a1/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-31 00:53:23.248884 aiodbm-0.2.0a1/LICENSE
--rw-r--r--   0        0        0      121 2023-05-31 13:00:10.815989 aiodbm-0.2.0a1/Makefile
--rw-r--r--   0        0        0     2287 2023-06-02 17:30:00.580465 aiodbm-0.2.0a1/README.rst
--rw-r--r--   0        0        0      634 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/Makefile
--rw-r--r--   0        0        0       37 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/_static/custom.css
--rw-r--r--   0        0        0       97 2023-06-02 17:31:54.543635 aiodbm-0.2.0a1/docs/api.rst
--rw-r--r--   0        0        0     1856 2023-06-02 17:19:55.420980 aiodbm-0.2.0a1/docs/conf.py
--rw-r--r--   0        0        0      347 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-06-02 17:04:23.375256 aiodbm-0.2.0a1/docs/make.bat
--rw-r--r--   0        0        0      378 2023-06-01 00:51:11.106230 aiodbm-0.2.0a1/examples/basic_usage.py
--rw-r--r--   0        0        0      736 2023-06-01 00:58:32.392882 aiodbm-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0      144 2023-06-02 17:19:55.424980 aiodbm-0.2.0a1/src/aiodbm/__init__.py
--rw-r--r--   0        0        0     8076 2023-06-02 17:27:04.806092 aiodbm-0.2.0a1/src/aiodbm/core.py
--rw-r--r--   0        0        0        0 2023-05-31 00:55:46.532853 aiodbm-0.2.0a1/tests/__init__.py
--rw-r--r--   0        0        0     2044 2023-06-02 17:03:15.638929 aiodbm-0.2.0a1/tests/measurements.py
--rw-r--r--   0        0        0     8303 2023-06-02 17:03:15.638929 aiodbm-0.2.0a1/tests/test_core.py
--rw-r--r--   0        0        0      397 2023-05-31 12:58:42.736904 aiodbm-0.2.0a1/tox.ini
--rw-r--r--   0        0        0     2912 1970-01-01 00:00:00.000000 aiodbm-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0      221 2023-05-31 12:59:34.028365 aiodbm-0.2.0b1/.coveragerc
+-rw-r--r--   0        0        0      964 2023-06-01 00:00:49.918153 aiodbm-0.2.0b1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-06-01 00:00:49.918153 aiodbm-0.2.0b1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      110 2023-05-31 01:31:26.803876 aiodbm-0.2.0b1/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-31 13:13:07.581265 aiodbm-0.2.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-06-02 17:34:44.178645 aiodbm-0.2.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-31 00:53:23.248884 aiodbm-0.2.0b1/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-31 13:00:10.815989 aiodbm-0.2.0b1/Makefile
+-rw-r--r--   0        0        0     3771 2023-06-03 11:55:58.452751 aiodbm-0.2.0b1/README.rst
+-rw-r--r--   0        0        0      634 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/_static/custom.css
+-rw-r--r--   0        0        0       97 2023-06-02 17:31:54.543635 aiodbm-0.2.0b1/docs/api.rst
+-rw-r--r--   0        0        0     1856 2023-06-02 17:19:55.420980 aiodbm-0.2.0b1/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-06-02 17:04:23.375256 aiodbm-0.2.0b1/docs/make.bat
+-rw-r--r--   0        0        0      378 2023-06-01 00:51:11.106230 aiodbm-0.2.0b1/examples/basic_usage.py
+-rw-r--r--   0        0        0      795 2023-06-02 17:51:19.099511 aiodbm-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0      144 2023-06-03 11:55:22.932910 aiodbm-0.2.0b1/src/aiodbm/__init__.py
+-rw-r--r--   0        0        0     8179 2023-06-03 10:28:02.047201 aiodbm-0.2.0b1/src/aiodbm/core.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:55:46.532853 aiodbm-0.2.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     2044 2023-06-02 17:03:15.638929 aiodbm-0.2.0b1/tests/measurements.py
+-rw-r--r--   0        0        0     9197 2023-06-03 10:44:24.394360 aiodbm-0.2.0b1/tests/test_core.py
+-rw-r--r--   0        0        0      397 2023-05-31 12:58:42.736904 aiodbm-0.2.0b1/tox.ini
+-rw-r--r--   0        0        0     4465 1970-01-01 00:00:00.000000 aiodbm-0.2.0b1/PKG-INFO
```

### Comparing `aiodbm-0.2.0a1/.github/workflows/main.yml` & `aiodbm-0.2.0b1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0a1/.github/workflows/release.yml` & `aiodbm-0.2.0b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0a1/LICENSE` & `aiodbm-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0a1/docs/Makefile` & `aiodbm-0.2.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0a1/docs/conf.py` & `aiodbm-0.2.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0a1/docs/make.bat` & `aiodbm-0.2.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0a1/pyproject.toml` & `aiodbm-0.2.0b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -15,12 +15,13 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 [project.urls]
+Documentation = "https://aiodbm.readthedocs.io/en/latest/"
 Source = "https://github.com/ErikKalkoken/aiodbm"
 Tracker = "https://github.com/ErikKalkoken/aiodbm/issues"
 
 [tool.isort]
 profile = "black"
```

### Comparing `aiodbm-0.2.0a1/src/aiodbm/core.py` & `aiodbm-0.2.0b1/src/aiodbm/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,56 +42,57 @@
 
 
 class Database(threading.Thread):
     """A proxy for a DBM database."""
 
     def __init__(self, connector: Callable) -> None:
         super().__init__()
-        self._database = None
+        self._db = None
         self._connector = connector
         self._message_queue = queue.Queue()
 
     def __await__(self) -> Generator[Any, None, "Database"]:
         return self._connect().__await__()
 
     async def __aenter__(self) -> "Database":
         return await self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         await self.close()
 
     @property
-    def _db(self):
-        """Return current database if one exists, else raise exception."""
-        if self._database is None:
+    def _db_strict(self):
+        """Return current database if one is active, else raise exception."""
+        if self._db is None:
             raise ValueError("no active database")
 
-        return self._database
+        return self._db
 
     @property
     def _dbm_type_name(self) -> str:
-        return type(self._db).__name__
+        """Return name of the currently active DBM variant."""
+        return type(self._db_strict).__name__
 
     @property
     def is_gdbm(self) -> bool:
         """Return True if this is a GDBM database."""
         return self._dbm_type_name == "gdbm"
 
     async def _connect(self) -> "Database":
         """Connect to the actual DBM database."""
-        if self._database is not None:
+        if self._db is not None:
             raise RuntimeError("Already connected")
 
         self.start()
         try:
             future = asyncio.get_running_loop().create_future()
             self._message_queue.put_nowait(Message(future, self._connector))
-            self._database = await future
+            self._db = await future
         except Exception:
-            self._database = None
+            self._db = None
             self._stop_runner()
             raise
 
         return self
 
     def run(self) -> None:
         """
@@ -132,116 +133,116 @@
     def _stop_runner(self):
         """Stop the thread runner."""
         stop_signal = Message.create_stop_signal()
         self._message_queue.put_nowait(stop_signal)
 
     async def _execute(self, fn, *args, **kwargs) -> Any:
         """Queue a function with the given arguments for execution in the runner."""
-        if self._database is None:
+        if self._db is None:
             raise ValueError("Database closed")
 
         func = partial(fn, *args, **kwargs)
         future = asyncio.get_running_loop().create_future()
 
         self._message_queue.put_nowait(Message(future, func))
 
         return await future
 
     # DBM API
 
     async def close(self) -> None:
         """Complete queued operations and close the database."""
 
-        if self._database is None:
+        if self._db is None:
             return
 
         try:
-            await self._execute(self._db.close)
+            await self._execute(self._db_strict.close)
         except Exception:
             logger.warning("exception occurred while closing database")
             raise
         finally:
-            self._database = None
+            self._db = None
             self._stop_runner()
 
     async def delete(self, key: Union[str, bytes]) -> None:
         """Delete given key."""
 
         def _func():
             try:
-                del self._db[key]
+                del self._db_strict[key]
             except KeyError as ex:
                 raise KeyError(f"Key {key} does not exist") from ex
 
         return await self._execute(_func)
 
     async def exists(self, key: Union[str, bytes]) -> bool:
         """Return True when the given key exists, else False."""
 
         def _func():
-            return key in self._db
+            return key in self._db_strict
 
         return await self._execute(_func)
 
     async def get(
         self, key: Union[str, bytes], default: Optional[bytes] = None
     ) -> Optional[bytes]:
         """Get the value of key. If the key does not exist, return default."""
 
-        return await self._execute(self._db.get, key, default)
+        return await self._execute(self._db_strict.get, key, default)
 
     async def keys(self) -> List[bytes]:
         """Return existing keys."""
 
-        return await self._execute(self._db.keys)
+        return await self._execute(self._db_strict.keys)
 
     async def set(self, key: Union[str, bytes], value: Union[str, bytes]) -> None:
         """Set key to hold the value.
         If key already holds a value, it is overwritten.
         """
 
         def _set():
-            self._db[key] = value
+            self._db_strict[key] = value
 
         await self._execute(_set)
 
     async def setdefault(self, key: Union[str, bytes], default: bytes) -> bytes:
         """Set key to hold the default value, if it does not yet exist.
         Or return current value of existing key.
         """
 
-        return await self._execute(self._db.setdefault, key, default)
+        return await self._execute(self._db_strict.setdefault, key, default)
 
     # GDBM only API
 
     async def firstkey(self) -> bytes:
         """Return the first key for looping over all keys. GDBM only."""
 
-        return await self._execute(self._db.firstkey)
+        return await self._execute(self._db_strict.firstkey)
 
     async def nextkey(self, key: Union[str, bytes]) -> Optional[bytes]:
         """Return the next key, when looping over all keys.
         Or return None, when the end of the loop has been reached.
         GDBM only.
         """
 
-        return await self._execute(self._db.nextkey, key)
+        return await self._execute(self._db_strict.nextkey, key)
 
     async def reorganize(self) -> None:
         """Reorganize the database. GDBM only."""
 
-        await self._execute(self._db.reorganize)
+        await self._execute(self._db_strict.reorganize)
 
     async def sync(self) -> None:
         """When the database has been opened in fast mode,
         this method forces any unwritten data to be written to the disk.
         GDBM only.
         """
 
-        await self._execute(self._db.sync)
+        await self._execute(self._db_strict.sync)
 
 
 def open(file: Union[str, Path], *args, **kwargs) -> Database:
     """Create and return a proxy to the DBM database.
 
     Example:
```

### Comparing `aiodbm-0.2.0a1/tests/measurements.py` & `aiodbm-0.2.0b1/tests/measurements.py`

 * *Files identical despite different names*

### Comparing `aiodbm-0.2.0a1/tests/test_core.py` & `aiodbm-0.2.0b1/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import dbm
 import shutil
 import sys
 import tempfile
 import time
 import unittest
 from pathlib import Path
+from unittest.mock import Mock
 
 import aiodbm
 from aiodbm.core import Message
 
 python_version = f"{sys.version_info.major}{sys.version_info.minor}"
 
 
@@ -44,15 +45,15 @@
         with self.assertRaises(ValueError):
             message.func_strict
 
 
 class DbmAsyncioTestCase(unittest.IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         self.temp_dir = Path(tempfile.mkdtemp())
-        self.data_path = str(self.temp_dir / "data.dbm")
+        self.data_path = str(self.temp_dir / "data.dat")
 
     def tearDown(self) -> None:
         shutil.rmtree(self.temp_dir, ignore_errors=True)
 
 
 class TestDbmFunctions(DbmAsyncioTestCase):
     async def test_whichdbm_should_return_name(self):
@@ -62,14 +63,23 @@
 
         # when
         result = await aiodbm.whichdb(self.data_path)
         # then
         self.assertIn(result, ["dbm.gnu", "dbm.ndbm", "dbm.dumb"])
 
 
+class TestDatabase(unittest.TestCase):
+    def test_should_raise_error_when_no_database_configured(self):
+        # given
+        db = aiodbm.Database(Mock())
+        # when/then
+        with self.assertRaises(ValueError):
+            db._db_strict
+
+
 class TestDatabaseAsync(DbmAsyncioTestCase):
     async def test_get_should_return_none_when_key_does_not_exists(self):
         async with aiodbm.open(self.data_path, "c") as db:
             # when
             result = await db.get("alpha")
             # then
             self.assertIsNone(result)
@@ -198,21 +208,27 @@
         await db.get("dummy")
         await db.close()
 
     async def test_open_raises_exception_when_opening_fails(self):
         with self.assertRaises(dbm.error):
             await aiodbm.open(self.data_path, "r")
 
-    async def test_can_call_close_multiple_timers(self):
+    async def test_can_call_close_multiple_times(self):
         # given
         db = await aiodbm.open(self.data_path, "c")
         await db.close()
         # when/then
         await db.close()
 
+    async def test_should_raise_error_when_trying_to_connect_again(self):
+        async with aiodbm.open(self.data_path, "c") as db:
+            # when/then
+            with self.assertRaises(RuntimeError):
+                await db._connect()
+
 
 @unittest.skipIf(python_version in ["38", "39"], reason="Unsupported Python")
 class TestGdbmFunctions(DbmAsyncioTestCase):
     async def test_firstkey_should_return_first_key(self):
         async with aiodbm.open(self.data_path, "c") as db:
             # given
             await db.set("alpha", "green")
@@ -242,7 +258,17 @@
             await db.reorganize()
 
     async def test_can_sync(self):
         async with aiodbm.open(self.data_path, "cf") as db:
             # when/then
             await db.set("alpha", "green")
             await db.sync()
+
+    async def test_can_detect_gdbm(self):
+        # given
+        async with aiodbm.open(self.data_path, "c") as db:
+            await db.set("alpha", "green")
+        result = await aiodbm.whichdb(self.data_path)
+        assert result == "dbm.gnu"
+        # when/then
+        async with aiodbm.open(self.data_path, "c") as db:
+            self.assertTrue(db.is_gdbm)
```

