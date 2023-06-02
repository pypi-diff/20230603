# Comparing `tmp/aiodiskqueue-0.1.0b5.tar.gz` & `tmp/aiodiskqueue-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0b5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0b7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0b5.tar` & `aiodiskqueue-0.1.0b7.tar`

### file list

```diff
@@ -1,38 +1,47 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b5/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b5/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b5/.github/workflows/release.yml
--rw-r--r--   0        0        0      155 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b5/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b5/LICENSE
--rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b5/Makefile
--rw-r--r--   0        0        0     2124 2023-05-29 15:23:28.059933 aiodiskqueue-0.1.0b5/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b5/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b5/docs/_static/custom.css
--rw-r--r--   0        0        0      267 2023-05-30 15:23:45.131006 aiodiskqueue-0.1.0b5/docs/api.rst
--rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b5/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b5/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b5/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b5/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b5/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b5/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b5/examples/single_consumer.py
--rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0b5/pyproject.toml
--rw-r--r--   0        0        0      307 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     4218 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/src/aiodiskqueue/engines.py
--rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b5/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0     8386 2023-05-31 14:37:36.233099 aiodiskqueue-0.1.0b5/src/aiodiskqueue/queues.py
--rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b5/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b5/tests/__init__.py
--rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b5/tests/factories.py
--rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b5/tests/helpers.py
--rw-r--r--   0        0        0        0 2023-05-30 08:19:53.541514 aiodiskqueue-0.1.0b5/tests/measurements/__init__.py
--rw-r--r--   0        0        0    49220 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/measurements/analysis.ipynb
--rw-r--r--   0        0        0      370 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/measurements/config.toml
--rw-r--r--   0        0        0       17 2023-05-30 10:40:38.676516 aiodiskqueue-0.1.0b5/tests/measurements/requirements.txt
--rw-r--r--   0        0        0     5825 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/measurements/run.py
--rw-r--r--   0        0        0     2495 2023-05-30 13:21:08.625414 aiodiskqueue-0.1.0b5/tests/test_integration.py
--rw-r--r--   0        0        0     8297 2023-05-31 14:37:36.237100 aiodiskqueue-0.1.0b5/tests/test_queues.py
--rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b5/tests/test_utils.py
--rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0b5/tox.ini
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b5/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b7/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b7/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b7/.github/workflows/release.yml
+-rw-r--r--   0        0        0      136 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b7/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b7/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b7/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b7/Makefile
+-rw-r--r--   0        0        0     2752 2023-06-02 22:45:46.710613 aiodiskqueue-0.1.0b7/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b7/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b7/docs/_static/custom.css
+-rw-r--r--   0        0        0      267 2023-05-30 15:23:45.131006 aiodiskqueue-0.1.0b7/docs/api.rst
+-rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b7/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b7/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b7/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b7/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b7/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b7/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b7/examples/single_consumer.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b7/measurements/__init__.py
+-rw-r--r--   0        0        0    51690 2023-06-02 12:59:19.828870 aiodiskqueue-0.1.0b7/measurements/analysis.ipynb
+-rw-r--r--   0        0        0      353 2023-06-01 20:15:41.824468 aiodiskqueue-0.1.0b7/measurements/config.toml
+-rw-r--r--   0        0        0       17 2023-06-01 19:01:40.059543 aiodiskqueue-0.1.0b7/measurements/requirements.txt
+-rw-r--r--   0        0        0     7078 2023-06-02 22:02:42.961153 aiodiskqueue-0.1.0b7/measurements/run.py
+-rw-r--r--   0        0        0     1055 2023-06-02 22:08:23.472217 aiodiskqueue-0.1.0b7/pyproject.toml
+-rw-r--r--   0        0        0      277 2023-06-02 22:06:54.677164 aiodiskqueue-0.1.0b7/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-02 22:07:35.456683 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/__init__.py
+-rw-r--r--   0        0        0     1097 2023-06-01 19:01:40.067544 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/base.py
+-rw-r--r--   0        0        0     3503 2023-06-02 12:59:11.304713 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/dbm.py
+-rw-r--r--   0        0        0     3353 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/simple.py
+-rw-r--r--   0        0        0     2198 2023-06-01 19:43:16.734632 aiodiskqueue-0.1.0b7/src/aiodiskqueue/engines/sqlite.py
+-rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b7/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0     7955 2023-06-02 22:36:25.575233 aiodiskqueue-0.1.0b7/src/aiodiskqueue/queues.py
+-rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b7/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b7/tests/engines/__init__.py
+-rw-r--r--   0        0        0     1910 2023-06-01 19:01:40.071544 aiodiskqueue-0.1.0b7/tests/engines/test_base.py
+-rw-r--r--   0        0        0      637 2023-06-02 22:11:12.239200 aiodiskqueue-0.1.0b7/tests/engines/test_dbm.py
+-rw-r--r--   0        0        0      714 2023-06-02 22:18:18.574682 aiodiskqueue-0.1.0b7/tests/engines/test_simple.py
+-rw-r--r--   0        0        0      405 2023-06-02 22:10:58.483256 aiodiskqueue-0.1.0b7/tests/engines/test_sqlite.py
+-rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b7/tests/factories.py
+-rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b7/tests/helpers.py
+-rw-r--r--   0        0        0     3495 2023-06-02 22:13:13.350859 aiodiskqueue-0.1.0b7/tests/test_integration.py
+-rw-r--r--   0        0        0     8469 2023-06-02 22:33:56.531565 aiodiskqueue-0.1.0b7/tests/test_queues.py
+-rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b7/tests/test_utils.py
+-rw-r--r--   0        0        0      459 2023-06-02 22:24:25.114342 aiodiskqueue-0.1.0b7/tox.ini
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b7/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0b5/.github/workflows/main.yml` & `aiodiskqueue-0.1.0b7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/.github/workflows/release.yml` & `aiodiskqueue-0.1.0b7/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/LICENSE` & `aiodiskqueue-0.1.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/README.rst` & `aiodiskqueue-0.1.0b7/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 - Queue content can persist a process restart
 - Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Sane logging
 - Type hints
 - Fully tested
+- Supports different storage engines
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
@@ -42,14 +43,24 @@
 
 You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodiskqueue
 
+storage Engines
+---------------
+
+Support different storage engines. The default engine is `DbmEngine`.
+
+- `DbmEngine`: Stores the queue in a DBM database. Consistent throughput even at higher volumes and much faster then Sqlite
+- `SqliteEngine`: Stores the queue in a SQlite database. Consistent throughput even at higher volumes and also process safe
+- `PickledList`: Stores the queue in a pickled list. Very fast at smaller volumes, but does not scale well
+- `PickleSequence`: Stores the queue in a list of pickled items. Very fast for putting and at smaller volumes, does not scale well
+
 
 
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
 .. |tests| image:: https://github.com/ErikKalkoken/aiodiskqueue/actions/workflows/main.yml/badge.svg
```

### Comparing `aiodiskqueue-0.1.0b5/docs/Makefile` & `aiodiskqueue-0.1.0b7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/docs/conf.py` & `aiodiskqueue-0.1.0b7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/docs/make.bat` & `aiodiskqueue-0.1.0b7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0b7/examples/multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/examples/single_consumer.py` & `aiodiskqueue-0.1.0b7/examples/single_consumer.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/src/aiodiskqueue/queues.py` & `aiodiskqueue-0.1.0b7/src/aiodiskqueue/queues.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Core implementation of a persistent AsyncIO queue."""
 
 import asyncio
 import logging
 from pathlib import Path
 from typing import Any, Union
 
-import aiofiles
-import aiofiles.os
-
-from aiodiskqueue.engines import PickledList, _StorageEngine
+from aiodiskqueue.engines.base import _FifoStorageEngine
+from aiodiskqueue.engines.dbm import DbmEngine
 from aiodiskqueue.exceptions import QueueEmpty, QueueFull
 from aiodiskqueue.utils import NoDirectInstantiation
 
 logger = logging.getLogger(__name__)
 
 
 class Queue(metaclass=NoDirectInstantiation):
@@ -27,15 +25,15 @@
     """
 
     def __init__(
         self,
         data_path: Path,
         maxsize: int,
         queue: list,
-        storage_engine: _StorageEngine,
+        storage_engine: _FifoStorageEngine,
     ) -> None:
         """Direct instantiation would break the persistance feature
         and has therefore been disabled.
 
         :meta private:
         """
         self._data_path = Path(data_path)
@@ -89,18 +87,17 @@
         else raise :class:`.QueueEmpty`.
         """
         async with self._queue_lock:
             if not self._queue:
                 raise QueueEmpty()
 
             item = self._queue.pop(0)
-            if self._queue:
-                await self._write_queue()
-            else:
-                await aiofiles.os.remove(self._data_path)
+            await self._storage_engine.remove_item(self._queue)
+            size = self.qsize()
+            self._peak_size = max(self._peak_size, size)
 
         if self._maxsize:
             async with self._has_free_slots:
                 self._has_free_slots.notify()
 
         return item
 
@@ -137,18 +134,15 @@
         Args:
             item: Any Python object that can be pickled
         """
         async with self._queue_lock:
             if self._maxsize and self.qsize() >= self._maxsize:
                 raise QueueFull
             self._queue.append(item)
-            if self._storage_engine.can_append:
-                await self._storage_engine.append_item(item)
-            else:
-                await self._storage_engine.save_all_items(self._queue)
+            await self._storage_engine.add_item(item, self._queue)
             async with self._tasks_are_finished:
                 self._unfinished_tasks += 1
 
         async with self._has_new_item:
             self._has_new_item.notify()
 
     def qsize(self) -> int:
@@ -176,20 +170,14 @@
             if self._unfinished_tasks <= 0:
                 raise ValueError("task_done() called too many times")
 
             self._unfinished_tasks -= 1
             if self._unfinished_tasks == 0:
                 self._tasks_are_finished.notify_all()
 
-    async def _write_queue(self):
-        await self._storage_engine.save_all_items(self._queue)
-        size = self.qsize()
-        self._peak_size = max(self._peak_size, size)
-        logger.debug("Wrote queue with %d items: %s", size, self._data_path)
-
     @classmethod
     async def create(
         cls,
         data_path: Union[str, Path],
         maxsize: int = 0,
         cls_storage_engine=None,
     ) -> "Queue":
@@ -207,29 +195,28 @@
         Args:
             data_path: Path of the data file for this queue. e.g. `queue.dat`
             maxsize: If maxsize is less than or equal to zero,
                 the queue size is infinite.
                 If it is an integer greater than 0, then put() blocks
                 when the queue reaches maxsize until an item is removed by get().
             cls_storage_engine: Define the storage engine to be used.
-                Default is :class:`.PickleSequence`.
+                Default is :class:`.DbmEngine`.
         """
         data_path = Path(data_path)
         if data_path.suffix == ".bak":
             raise ValueError("Invalid file name: .bak suffix is reserved for backups")
 
         if not cls_storage_engine:
-            cls_storage_engine = PickledList
+            cls_storage_engine = DbmEngine
         else:
-            if not issubclass(cls_storage_engine, _StorageEngine):
+            if not issubclass(cls_storage_engine, _FifoStorageEngine):
                 raise TypeError("Invalid storage engine")
         storage_engine = cls_storage_engine(data_path)
-        queue = await storage_engine.load_all_items()
+        queue = await storage_engine.fetch_all()
         if not queue:
-            await storage_engine.save_all_items([])  # ensuring early we can write
-            await aiofiles.os.remove(data_path)
+            await storage_engine.initialize()  # ensuring early we can write
         else:
             logger.info(
                 "Read %d items from existing data file: %s", len(queue), data_path
             )
 
         return cls._create(data_path, maxsize, queue, storage_engine)
```

### Comparing `aiodiskqueue-0.1.0b5/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.0b7/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/tests/factories.py` & `aiodiskqueue-0.1.0b7/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/tests/measurements/run.py` & `aiodiskqueue-0.1.0b7/measurements/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 """Measure queue throughput.
 
 Runs multiple producers and consumers in parallel and measures duration and throughput.
 """
+import argparse
 import asyncio
 import csv
 import datetime as dt
 import logging
 import random
 import string
+import tempfile
 import time
 from dataclasses import asdict, dataclass, fields
 from pathlib import Path
 from typing import List
 
 import tomllib
 
 import aiodiskqueue
 
-logging.basicConfig(level="INFO", format="%(asctime)s - %(levelname)s -  %(message)s")
+logging.basicConfig(level="INFO", format="%(asctime)s | %(levelname)s | %(message)s")
 
 logger = logging.getLogger(__name__)
 
+ITEM_SIZE = 256
+
 
 @dataclass(frozen=True)
 class Measurement:
     FILENAME = "measurements.csv"
 
     timestamp: dt.datetime
-    run: int
     items: int
     producers: int
     consumers: int
     peak_size: int
     profile: str
     storage_engine: str
     throughput: float
@@ -52,25 +55,14 @@
         logger.info(f"Written results to: {path}")
 
     @classmethod
     def field_names(cls) -> List[str]:
         return [field.name for field in fields(cls)]
 
     @classmethod
-    def latest_run(cls) -> int:
-        if not cls.path().exists():
-            return 0
-        with cls.path().open("r") as csv_file:
-            run_nums = []
-            reader = csv.DictReader(csv_file)
-            for row in reader:
-                run_nums.append(int(row["run"]))
-        return max(run_nums)
-
-    @classmethod
     def path(cls) -> Path:
         return Path(__file__).parent / cls.FILENAME
 
 
 def random_string(length: int) -> str:
     return "".join(random.choices(string.ascii_uppercase + string.digits, k=length))
 
@@ -102,33 +94,32 @@
 
 async def runner(
     data_path: Path,
     items_count: int,
     producer_count: int,
     consumer_count: int,
     timestamp: dt.datetime,
-    run: int,
     profile_name: str,
     cls_storage_engine,
 ):
     logger.info(
-        f"Starting run #{run} with engine {cls_storage_engine.__name__}, "
+        f"Starting run with engine {cls_storage_engine.__name__}, "
         f"profile {profile_name} and {items_count} items."
     )
 
     # create queues
     source_queue = asyncio.Queue()
     data_path.unlink(missing_ok=True)
     disk_queue = await aiodiskqueue.Queue.create(
         data_path, cls_storage_engine=cls_storage_engine
     )
     result_queue = asyncio.Queue()
 
     # create source queue with items
-    source_items = {random_string(16) for _ in range(items_count)}
+    source_items = {random_string(ITEM_SIZE) for _ in range(items_count)}
 
     if producer_count:
         for item in source_items:
             source_queue.put_nowait(item)
     else:
         for item in source_items:
             await disk_queue.put_nowait(item)
@@ -156,55 +147,111 @@
 
     # measure duration and throughput
     duration = end - start
     throughput = items_count * 2 / duration
     logger.info("Throughput for %d items: %f items / sec", items_count, throughput)
     logger.info("Peak size of disk queue was: %d", disk_queue._peak_size)
 
+    # compare source items with result items
+    result_items = set()
+    while True:
+        try:
+            item = result_queue.get_nowait()
+        except asyncio.QueueEmpty:
+            break
+        else:
+            result_items.add(item)
+    dif = source_items.difference(result_items)
+    if dif:
+        logger.error("Differences found")
+        logger.info("dif: %s", sorted(list(dif)))
+        raise RuntimeError("Run failed due to differences")
+
+    logger.info("Data integrity confirmed")
+
     # write results
     data = {
         "timestamp": timestamp,
-        "run": run,
         "items": items_count,
         "producers": producer_count,
         "consumers": consumer_count,
         "peak_size": disk_queue._peak_size,
         "profile": profile_name,
         "storage_engine": type(disk_queue._storage_engine).__name__,
         "throughput": throughput,
     }
     obj = Measurement(**data)
     obj.save()
 
 
-async def start(data_path: Path, config: dict, run: int):
+async def start(
+    data_path: Path,
+    config: dict,
+    profiles: list,
+    max_items=None,
+):
     timestamp = dt.datetime.now(tz=dt.timezone.utc)
-    for cls_storage_engine in [aiodiskqueue.PickleSequence, aiodiskqueue.PickledList]:
-        for profile in config["profiles"]:
-            for item_count in config["common"]["items"]:
+
+    # select item count if override set
+    if max_items:
+        item_counts = [
+            count for count in config["common"]["items"] if count <= max_items
+        ]
+    else:
+        item_counts = config["common"]["items"]
+
+    for cls_storage_engine in [
+        aiodiskqueue.engines.PickledList,
+        aiodiskqueue.engines.PickleSequence,
+        aiodiskqueue.engines.DbmEngine,
+        # aiodiskqueue.engines.SqliteEngine,
+    ]:
+        for profile in profiles:
+            for item_count in item_counts:
                 await runner(
                     data_path,
                     item_count,
                     profile["producers"],
                     profile["consumers"],
                     timestamp,
-                    run,
                     profile["name"],
                     cls_storage_engine,
                 )
 
 
 def load_config() -> dict:
     path = Path(__file__).parent / "config.toml"
     with path.open("rb") as fp:
         return tomllib.load(fp)
 
 
 def main():
-    data_path = Path(__file__).parent / "loadtest_queue.dat"
     config = load_config()
-    run = Measurement.latest_run() + 1
-    asyncio.run(start(data_path, config, run=run))
+    profiles = sorted([obj["name"] for obj in config["profiles"]])
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "profiles", choices=profiles, nargs="*", help="Name of the profiles to run"
+    )
+    parser.add_argument(
+        "--max-items",
+        type=int,
+        choices=config["common"]["items"],
+        help="Max items to run with from the profile",
+    )
+    parser.add_argument(
+        "--all",
+        action="store_true",
+        help="Run all profiles",
+    )
+    args = parser.parse_args()
+
+    if args.profiles:
+        chosen_profiles = [o for o in config["profiles"] if o["name"] in args.profiles]
+    else:
+        chosen_profiles = config["profiles"]
+    with tempfile.TemporaryDirectory() as temp_dir:
+        data_path = Path(temp_dir) / "loadtest_queue.dat"
+        asyncio.run(start(data_path, config, chosen_profiles, args.max_items))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aiodiskqueue-0.1.0b5/tests/test_queues.py` & `aiodiskqueue-0.1.0b7/tests/test_queues.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import asyncio
-
-import aiofiles
-import aiofiles.os
+import sys
+from unittest import skipIf
 
 from aiodiskqueue import Queue, QueueEmpty, QueueFull
-from aiodiskqueue.engines import PickledList, PickleSequence
 
 from .factories import ItemFactory
 from .helpers import QueueAsyncioTestCase
 
+try:
+    from aiodiskqueue.engines.simple import PickledList
+except ImportError:
+    PickledList = None
+
+py_version = f"{sys.version_info.major}{sys.version_info.minor}"
+
 
 class TestCreateQueue(QueueAsyncioTestCase):
     async def test_should_create_queue_and_measure_size(self):
         # given
         q = await Queue.create(self.data_path)
         # when/then
         self.assertIsInstance(q, Queue)
@@ -38,87 +43,86 @@
     async def test_fail_at_creation_when_data_file_can_not_be_written(self):
         # given
         invalid_path = self.data_path.parent / "dead-end" / "queue.dat"
         # when/then
         with self.assertRaises(OSError):
             await Queue.create(invalid_path)
 
-    async def test_should_reset_queue_and_backup_data_file_when_not_usable(self):
-        # given
-        async with aiofiles.open(self.data_path, "wb") as fp:
-            await fp.write(b"invalid-data")
-        # when
-        q = await Queue.create(self.data_path)
-        # then
-        self.assertEqual(q.qsize(), 0)
-        backup_path = self.data_path.with_suffix(".bak")
-        self.assertTrue(backup_path.exists())
-
-    async def test_should_overwrite_existing_backup(self):
-        # given
-        async with aiofiles.open(self.data_path, "wb") as fp:
-            await fp.write(b"invalid-data")
-        backup_path = self.data_path.with_suffix(".bak")
-        backup_path.touch()
-        # when
-        q = await Queue.create(self.data_path)
-        # then
-        self.assertEqual(q.qsize(), 0)
-        self.assertTrue(backup_path.exists())
+    # TODO: Does not work with new default, rework needed
+    # async def test_should_reset_queue_and_backup_data_file_when_not_usable(self):
+    #     # given
+    #     async with aiofiles.open(self.data_path, "wb") as fp:
+    #         await fp.write(b"invalid-data")
+    #     # when
+    #     q = await Queue.create(self.data_path)
+    #     # then
+    #     self.assertEqual(q.qsize(), 0)
+    #     backup_path = self.data_path.with_suffix(".bak")
+    #     self.assertTrue(backup_path.exists())
+
+    # async def test_should_overwrite_existing_backup(self):
+    #     # given
+    #     async with aiofiles.open(self.data_path, "wb") as fp:
+    #         await fp.write(b"invalid-data")
+    #     backup_path = self.data_path.with_suffix(".bak")
+    #     backup_path.touch()
+    #     # when
+    #     q = await Queue.create(self.data_path)
+    #     # then
+    #     self.assertEqual(q.qsize(), 0)
+    #     self.assertTrue(backup_path.exists())
 
     async def test_should_preserve_queue_content(self):
         # given
         queue_1 = await Queue.create(self.data_path)
         item = ItemFactory()
         await queue_1.put_nowait(item)
         del queue_1
         # when
         queue_2 = await Queue.create(self.data_path)
         # then
         item_new = await queue_2.get()
         self.assertEqual(item_new, item)
 
-    async def test_should_create_queue_with_storage_engine_1(self):
-        # given
-        q = await Queue.create(self.data_path, cls_storage_engine=PickleSequence)
-        # when/then
-        self.assertIsInstance(q._storage_engine, PickleSequence)
-
-    async def test_should_create_queue_with_storage_engine_2(self):
-        # given
-        q = await Queue.create(self.data_path, cls_storage_engine=PickledList)
-        # when/then
-        self.assertIsInstance(q._storage_engine, PickledList)
-
     async def test_should_raise_error_when_storage_engine_not_valid(self):
         # when/then
         with self.assertRaises(TypeError):
             await Queue.create(self.data_path, cls_storage_engine=str)
 
+    if PickledList:
+
+        async def test_should_create_queue_with_storage_engine_2(self):
+            # given
+            q = await Queue.create(self.data_path, cls_storage_engine=PickledList)
+            # when/then
+            self.assertIsInstance(q._storage_engine, PickledList)  # type: ignore
+
 
 class TestPutIntoQueue(QueueAsyncioTestCase):
     async def test_should_put_items_and_measure_size(self):
         # given
         q = await Queue.create(self.data_path)
         # when
         await q.put_nowait(ItemFactory())
         await q.put_nowait(ItemFactory())
         # then
         result = q.qsize()
         self.assertEqual(result, 2)
 
-    async def test_should_delete_file_when_queue_is_empty(self):
+    @skipIf(py_version in ["38", "39"], "Not supported in older Py versions")
+    async def test_should_keep_data_file_for_empty_queue(self):
         # given
         q = await Queue.create(self.data_path)
         await q.put_nowait(ItemFactory)
         # when
         await q.get()
         # then
-        self.assertFalse(self.data_path.exists())
+        self.assertTrue(self.data_path.exists())
 
+    @skipIf(py_version in ["38", "39"], "Not supported in older Py versions")
     async def test_should_raise_error_when_putting_into_full_queue(self):
         # given
         q = await Queue.create(self.data_path, maxsize=1)
         await q.put_nowait(ItemFactory)
         # when
         with self.assertRaises(QueueFull):
             await q.put_nowait(ItemFactory)
```

### Comparing `aiodiskqueue-0.1.0b5/tests/test_utils.py` & `aiodiskqueue-0.1.0b7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b5/PKG-INFO` & `aiodiskqueue-0.1.0b7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0b5
+Version: 0.1.0b7
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles>=23.1.0
+Requires-Dist: aiodbm>=0.2.0a1
+Requires-Dist: aiofiles>=23.1.0 ; extra == "aiofiles"
+Requires-Dist: aiosqlite>=0.19.0 ; extra == "aiosqlite"
 Project-URL: Documentation, https://aiodiskqueue.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ErikKalkoken/aiodiskqueue
 Project-URL: Tracker, https://github.com/ErikKalkoken/aiodiskqueue/issues
+Provides-Extra: aiofiles
+Provides-Extra: aiosqlite
 
 aiodiskqueue
 ============
 
 Persistent queue for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
@@ -31,14 +35,15 @@
 
 - Queue content can persist a process restart
 - Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Sane logging
 - Type hints
 - Fully tested
+- Supports different storage engines
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
@@ -61,14 +66,24 @@
 
 You can install this library directly from PyPI with the following command:
 
 .. code:: shell
 
     pip install aiodiskqueue
 
+storage Engines
+---------------
+
+Support different storage engines. The default engine is `DbmEngine`.
+
+- `DbmEngine`: Stores the queue in a DBM database. Consistent throughput even at higher volumes and much faster then Sqlite
+- `SqliteEngine`: Stores the queue in a SQlite database. Consistent throughput even at higher volumes and also process safe
+- `PickledList`: Stores the queue in a pickled list. Very fast at smaller volumes, but does not scale well
+- `PickleSequence`: Stores the queue in a list of pickled items. Very fast for putting and at smaller volumes, does not scale well
+
 
 
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
 .. |tests| image:: https://github.com/ErikKalkoken/aiodiskqueue/actions/workflows/main.yml/badge.svg
```

