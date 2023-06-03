# Comparing `tmp/persist-queue-0.8.0b0.tar.gz` & `tmp/persist-queue-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/persist-queue-0.8.0b0.tar", last modified: Tue Apr 26 11:08:02 2022, max compression
+gzip compressed data, was "persist-queue-0.8.1.tar", last modified: Sat Jun  3 10:59:51 2023, max compression
```

## Comparing `persist-queue-0.8.0b0.tar` & `persist-queue-0.8.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 yuzhi.wx   (501) staff       (20)        0 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    25601 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/PKG-INFO
-drwxr-xr-x   0 yuzhi.wx   (501) staff       (20)        0 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persistqueue/
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    10970 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/queue.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     5167 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/mysqlqueue.py
-drwxr-xr-x   0 yuzhi.wx   (501) staff       (20)        0 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persistqueue/tests/
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)       15 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/tests/__init__.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     2719 2021-08-12 06:27:32.000000 persist-queue-0.8.0b0/persistqueue/tests/test_pdict.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    10340 2019-11-07 05:26:42.000000 persist-queue-0.8.0b0/persistqueue/tests/test_queue.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    14322 2022-04-25 02:08:52.000000 persist-queue-0.8.0b0/persistqueue/tests/test_sqlqueue.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     8965 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/tests/test_mysqlqueue.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    15828 2022-04-25 02:08:52.000000 persist-queue-0.8.0b0/persistqueue/tests/test_sqlackqueue.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    15386 2022-04-25 02:08:52.000000 persist-queue-0.8.0b0/persistqueue/sqlbase.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)      785 2022-04-25 02:08:52.000000 persist-queue-0.8.0b0/persistqueue/__init__.py
-drwxr-xr-x   0 yuzhi.wx   (501) staff       (20)        0 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persistqueue/serializers/
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     1229 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/serializers/msgpack.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)       15 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/serializers/__init__.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)      938 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/serializers/pickle.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)      760 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/serializers/json.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)      318 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/common.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    12898 2022-04-25 02:08:52.000000 persist-queue-0.8.0b0/persistqueue/sqlackqueue.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)      268 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/exceptions.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     3012 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/sqlqueue.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     2235 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/persistqueue/pdict.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     1551 2018-05-19 06:56:15.000000 persist-queue-0.8.0b0/LICENSE
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)        0 2022-02-15 06:32:16.000000 persist-queue-0.8.0b0/requirements.txt
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)      210 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/test-requirements.txt
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)       79 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/extra-requirements.txt
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)       49 2020-11-09 05:32:56.000000 persist-queue-0.8.0b0/MANIFEST.in
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)     1599 2022-02-20 15:55:07.000000 persist-queue-0.8.0b0/setup.py
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)       67 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/setup.cfg
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    19632 2022-04-25 02:08:52.000000 persist-queue-0.8.0b0/README.rst
-drwxr-xr-x   0 yuzhi.wx   (501) staff       (20)        0 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persist_queue.egg-info/
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)    25601 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persist_queue.egg-info/PKG-INFO
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)      869 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persist_queue.egg-info/SOURCES.txt
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)       46 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persist_queue.egg-info/requires.txt
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)       13 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persist_queue.egg-info/top_level.txt
--rw-r--r--   0 yuzhi.wx   (501) staff       (20)        1 2022-04-26 11:08:02.000000 persist-queue-0.8.0b0/persist_queue.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 10:59:51.096334 persist-queue-0.8.1/
+-rw-rw-rw-   0        0        0     1579 2022-04-16 04:39:22.000000 persist-queue-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0       52 2022-04-16 04:39:22.000000 persist-queue-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    22438 2023-06-03 10:59:51.096334 persist-queue-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0    21264 2023-06-03 10:42:58.000000 persist-queue-0.8.1/README.rst
+-rw-rw-rw-   0        0        0       97 2023-06-03 10:42:58.000000 persist-queue-0.8.1/extra-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 10:59:51.087335 persist-queue-0.8.1/persist_queue.egg-info/
+-rw-rw-rw-   0        0        0    22438 2023-06-03 10:59:51.000000 persist-queue-0.8.1/persist_queue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      903 2023-06-03 10:59:51.000000 persist-queue-0.8.1/persist_queue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 10:59:51.000000 persist-queue-0.8.1/persist_queue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-03 10:59:51.000000 persist-queue-0.8.1/persist_queue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 10:59:51.000000 persist-queue-0.8.1/persist_queue.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 10:59:51.091335 persist-queue-0.8.1/persistqueue/
+-rw-rw-rw-   0        0        0      940 2023-06-03 10:56:57.000000 persist-queue-0.8.1/persistqueue/__init__.py
+-rw-rw-rw-   0        0        0      318 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/common.py
+-rw-rw-rw-   0        0        0      287 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/exceptions.py
+-rw-rw-rw-   0        0        0     5329 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/mysqlqueue.py
+-rw-rw-rw-   0        0        0     2312 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/pdict.py
+-rw-rw-rw-   0        0        0    11357 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/queue.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:59:51.093335 persist-queue-0.8.1/persistqueue/serializers/
+-rw-rw-rw-   0        0        0       16 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1161 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/serializers/cbor2.py
+-rw-rw-rw-   0        0        0      760 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/serializers/json.py
+-rw-rw-rw-   0        0        0     1229 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/serializers/msgpack.py
+-rw-rw-rw-   0        0        0      938 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/serializers/pickle.py
+-rw-rw-rw-   0        0        0    13327 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/sqlackqueue.py
+-rw-rw-rw-   0        0        0    15882 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/sqlbase.py
+-rw-rw-rw-   0        0        0     3117 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/sqlqueue.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:59:51.095335 persist-queue-0.8.1/persistqueue/tests/
+-rw-rw-rw-   0        0        0       16 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/tests/__init__.py
+-rw-rw-rw-   0        0        0     9561 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/tests/test_mysqlqueue.py
+-rw-rw-rw-   0        0        0     2795 2022-04-16 04:39:22.000000 persist-queue-0.8.1/persistqueue/tests/test_pdict.py
+-rw-rw-rw-   0        0        0    11129 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/tests/test_queue.py
+-rw-rw-rw-   0        0        0    16668 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/tests/test_sqlackqueue.py
+-rw-rw-rw-   0        0        0    15595 2023-06-03 10:42:58.000000 persist-queue-0.8.1/persistqueue/tests/test_sqlqueue.py
+-rw-rw-rw-   0        0        0        0 2022-04-16 04:39:22.000000 persist-queue-0.8.1/requirements.txt
+-rw-rw-rw-   0        0        0       74 2023-06-03 10:59:51.096334 persist-queue-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1646 2022-04-16 04:39:22.000000 persist-queue-0.8.1/setup.py
+-rw-rw-rw-   0        0        0      234 2023-06-03 10:42:58.000000 persist-queue-0.8.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `persist-queue-0.8.0b0/persistqueue/mysqlqueue.py` & `persist-queue-0.8.1/persistqueue/mysqlqueue.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-# coding=utf-8
-from dbutils.pooled_db import PooledDB
-import threading
-import time as _time
-
-import persistqueue
-from .sqlbase import SQLBase
-
-
-class MySQLQueue(SQLBase):
-    """Mysql(or future standard dbms) based FIFO queue."""
-    _TABLE_NAME = 'queue'
-    _KEY_COLUMN = '_id'  # the name of the key column, used in DB CRUD
-    # SQL to create a table
-    _SQL_CREATE = (
-        'CREATE TABLE IF NOT EXISTS {table_name} ('
-        '{key_column} INTEGER PRIMARY KEY AUTO_INCREMENT, '
-        'data BLOB, timestamp FLOAT)')
-    # SQL to insert a record
-    _SQL_INSERT = 'INSERT INTO {table_name} (data, timestamp) VALUES (%s, %s)'
-    # SQL to select a record
-    _SQL_SELECT_ID = (
-        'SELECT {key_column}, data, timestamp FROM {table_name} WHERE'
-        ' {key_column} = {rowid}'
-    )
-    _SQL_SELECT = (
-        'SELECT {key_column}, data, timestamp FROM {table_name} '
-        'ORDER BY {key_column} ASC LIMIT 1'
-    )
-    _SQL_SELECT_WHERE = (
-        'SELECT {key_column}, data, timestamp FROM {table_name} WHERE'
-        ' {column} {op} %s ORDER BY {key_column} ASC LIMIT 1 '
-    )
-    _SQL_UPDATE = 'UPDATE {table_name} SET data = %s WHERE {key_column} = %s'
-
-    _SQL_DELETE = 'DELETE FROM {table_name} WHERE {key_column} {op} %s'
-
-    def __init__(self, host, user, passwd, db_name, name=None,
-                 port=3306,
-                 charset='utf8mb4',
-                 auto_commit=True,
-                 serializer=persistqueue.serializers.pickle,
-                 ):
-        self.name = name if name else "sql"
-        self.host = host
-        self.user = user
-        self.passwd = passwd
-        self.db_name = db_name
-        self.name = name
-        self.port = port
-        self.charset = charset
-        self._serializer = serializer
-        self.auto_commit = auto_commit
-
-        # SQLite3 transaction lock
-        self.tran_lock = threading.Lock()
-        self.put_event = threading.Event()
-        # Action lock to assure multiple action to be *atomic*
-        self.action_lock = threading.Lock()
-
-        self._connection_pool = None
-        self._getter = None
-        self._putter = None
-        self._new_db_connection()
-        self._init()
-
-    def _new_db_connection(self):
-        try:
-            import pymysql
-        except ImportError:
-            print(
-                "Please install mysql library via "
-                "'pip install PyMySQL'")
-            raise
-        db_pool = PooledDB(pymysql, 2, 10, 5, 10, True,
-                           host=self.host, port=self.port, user=self.user,
-                           passwd=self.passwd, database=self.db_name,
-                           charset=self.charset
-                           )
-        self._connection_pool = db_pool
-        conn = db_pool.connection()
-        cursor = conn.cursor()
-        cursor.execute("SELECT VERSION()")
-        _ = cursor.fetchone()
-        # create table automatically
-        cursor.execute(self._sql_create)
-        conn.commit()
-        # switch to the desired db
-        cursor.execute("use %s" % self.db_name)
-        self._putter = MySQLConn(queue=self)
-        self._getter = self._putter
-
-    def put(self, item, block=True):
-        # block kwarg is noop and only here to align with python's queue
-        obj = self._serializer.dumps(item)
-        _id = self._insert_into(obj, _time.time())
-        self.total += 1
-        self.put_event.set()
-        return _id
-
-    def put_nowait(self, item):
-        return self.put(item, block=False)
-
-    def _init(self):
-        # super(SQLBase, self)._init()
-        # Action lock to assure multiple action to be *atomic*
-        self.action_lock = threading.Lock()
-        if not self.auto_commit:
-            # Refresh current cursor after restart
-            head = self._select()
-            if head:
-                self.cursor = head[0] - 1
-            else:
-                self.cursor = 0
-        self.total = self._count()
-
-    def get_pooled_conn(self):
-        return self._connection_pool.connection()
-
-
-class MySQLConn(object):
-    """MySqlConn defines a common structure for
-    both mysql and sqlite3 connections.
-
-    used to mitigate the interface differences between drivers/db
-    """
-
-    def __init__(self, queue=None, conn=None):
-        if queue is not None:
-            self._conn = queue.get_pooled_conn()
-        else:
-            self._conn = conn
-        self._queue = queue
-        self._cursor = None
-        self.closed = False
-
-    def __enter__(self):
-        self._cursor = self._conn.cursor()
-        return self._conn
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        # do not commit() but to close() , keep same behavior
-        # with dbutils
-        self._cursor.close()
-
-    def execute(self, *args, **kwargs):
-        if self._queue is not None:
-            conn = self._queue.get_pooled_conn()
-        else:
-            conn = self._conn
-        cursor = conn.cursor()
-        cursor.execute(*args, **kwargs)
-        return cursor
-
-    def close(self):
-        if not self.closed:
-            self._conn.close()
-        self.closed = True
-
-    def commit(self):
-        if not self.closed:
-            self._conn.commit()
+# coding=utf-8
+from dbutils.pooled_db import PooledDB
+import threading
+import time as _time
+
+import persistqueue
+from .sqlbase import SQLBase
+
+
+class MySQLQueue(SQLBase):
+    """Mysql(or future standard dbms) based FIFO queue."""
+    _TABLE_NAME = 'queue'
+    _KEY_COLUMN = '_id'  # the name of the key column, used in DB CRUD
+    # SQL to create a table
+    _SQL_CREATE = (
+        'CREATE TABLE IF NOT EXISTS {table_name} ('
+        '{key_column} INTEGER PRIMARY KEY AUTO_INCREMENT, '
+        'data BLOB, timestamp FLOAT)')
+    # SQL to insert a record
+    _SQL_INSERT = 'INSERT INTO {table_name} (data, timestamp) VALUES (%s, %s)'
+    # SQL to select a record
+    _SQL_SELECT_ID = (
+        'SELECT {key_column}, data, timestamp FROM {table_name} WHERE'
+        ' {key_column} = {rowid}'
+    )
+    _SQL_SELECT = (
+        'SELECT {key_column}, data, timestamp FROM {table_name} '
+        'ORDER BY {key_column} ASC LIMIT 1'
+    )
+    _SQL_SELECT_WHERE = (
+        'SELECT {key_column}, data, timestamp FROM {table_name} WHERE'
+        ' {column} {op} %s ORDER BY {key_column} ASC LIMIT 1 '
+    )
+    _SQL_UPDATE = 'UPDATE {table_name} SET data = %s WHERE {key_column} = %s'
+
+    _SQL_DELETE = 'DELETE FROM {table_name} WHERE {key_column} {op} %s'
+
+    def __init__(self, host, user, passwd, db_name, name=None,
+                 port=3306,
+                 charset='utf8mb4',
+                 auto_commit=True,
+                 serializer=persistqueue.serializers.pickle,
+                 ):
+        self.name = name if name else "sql"
+        self.host = host
+        self.user = user
+        self.passwd = passwd
+        self.db_name = db_name
+        self.name = name
+        self.port = port
+        self.charset = charset
+        self._serializer = serializer
+        self.auto_commit = auto_commit
+
+        # SQLite3 transaction lock
+        self.tran_lock = threading.Lock()
+        self.put_event = threading.Event()
+        # Action lock to assure multiple action to be *atomic*
+        self.action_lock = threading.Lock()
+
+        self._connection_pool = None
+        self._getter = None
+        self._putter = None
+        self._new_db_connection()
+        self._init()
+
+    def _new_db_connection(self):
+        try:
+            import pymysql
+        except ImportError:
+            print(
+                "Please install mysql library via "
+                "'pip install PyMySQL'")
+            raise
+        db_pool = PooledDB(pymysql, 2, 10, 5, 10, True,
+                           host=self.host, port=self.port, user=self.user,
+                           passwd=self.passwd, database=self.db_name,
+                           charset=self.charset
+                           )
+        self._connection_pool = db_pool
+        conn = db_pool.connection()
+        cursor = conn.cursor()
+        cursor.execute("SELECT VERSION()")
+        _ = cursor.fetchone()
+        # create table automatically
+        cursor.execute(self._sql_create)
+        conn.commit()
+        # switch to the desired db
+        cursor.execute("use %s" % self.db_name)
+        self._putter = MySQLConn(queue=self)
+        self._getter = self._putter
+
+    def put(self, item, block=True):
+        # block kwarg is noop and only here to align with python's queue
+        obj = self._serializer.dumps(item)
+        _id = self._insert_into(obj, _time.time())
+        self.total += 1
+        self.put_event.set()
+        return _id
+
+    def put_nowait(self, item):
+        return self.put(item, block=False)
+
+    def _init(self):
+        # super(SQLBase, self)._init()
+        # Action lock to assure multiple action to be *atomic*
+        self.action_lock = threading.Lock()
+        if not self.auto_commit:
+            # Refresh current cursor after restart
+            head = self._select()
+            if head:
+                self.cursor = head[0] - 1
+            else:
+                self.cursor = 0
+        self.total = self._count()
+
+    def get_pooled_conn(self):
+        return self._connection_pool.connection()
+
+
+class MySQLConn(object):
+    """MySqlConn defines a common structure for
+    both mysql and sqlite3 connections.
+
+    used to mitigate the interface differences between drivers/db
+    """
+
+    def __init__(self, queue=None, conn=None):
+        if queue is not None:
+            self._conn = queue.get_pooled_conn()
+        else:
+            self._conn = conn
+        self._queue = queue
+        self._cursor = None
+        self.closed = False
+
+    def __enter__(self):
+        self._cursor = self._conn.cursor()
+        return self._conn
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        # do not commit() but to close() , keep same behavior
+        # with dbutils
+        self._cursor.close()
+
+    def execute(self, *args, **kwargs):
+        if self._queue is not None:
+            conn = self._queue.get_pooled_conn()
+        else:
+            conn = self._conn
+        cursor = conn.cursor()
+        cursor.execute(*args, **kwargs)
+        return cursor
+
+    def close(self):
+        if not self.closed:
+            self._conn.close()
+        self.closed = True
+
+    def commit(self):
+        if not self.closed:
+            self._conn.commit()
```

### Comparing `persist-queue-0.8.0b0/persistqueue/tests/test_pdict.py` & `persist-queue-0.8.1/persistqueue/tests/test_pdict.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-
-import shutil
-import tempfile
-import unittest
-
-from persistqueue import pdict
-
-
-class PDictTest(unittest.TestCase):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='pdict')
-
-    def tearDown(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-
-    def test_unsupported(self):
-        pd = pdict.PDict(self.path, 'pd')
-        pd['key_a'] = 'value_a'
-        self.assertRaises(NotImplementedError, pd.keys)
-        self.assertRaises(NotImplementedError, pd.iterkeys)
-        self.assertRaises(NotImplementedError, pd.values)
-        self.assertRaises(NotImplementedError, pd.itervalues)
-        self.assertRaises(NotImplementedError, pd.items)
-        self.assertRaises(NotImplementedError, pd.iteritems)
-
-        def _for():
-            for _ in pd:
-                pass
-        self.assertRaises(NotImplementedError, _for)
-
-    def test_add(self):
-        pd = pdict.PDict(self.path, 'pd')
-        pd['key_a'] = 'value_a'
-        self.assertEqual(pd['key_a'], 'value_a')
-        self.assertTrue('key_a' in pd)
-        self.assertFalse('key_b' in pd)
-        self.assertEqual(pd.get('key_a'), 'value_a')
-        self.assertEqual(pd.get('key_b'), None)
-        self.assertEqual(pd.get('key_b', 'absent'), 'absent')
-        self.assertRaises(KeyError, lambda: pd['key_b'])
-        pd['key_b'] = 'value_b'
-        self.assertEqual(pd['key_a'], 'value_a')
-        self.assertEqual(pd['key_b'], 'value_b')
-
-    def test_set(self):
-        pd = pdict.PDict(self.path, 'pd')
-        pd['key_a'] = 'value_a'
-        pd['key_b'] = 'value_b'
-        self.assertEqual(pd['key_a'], 'value_a')
-        self.assertEqual(pd['key_b'], 'value_b')
-        self.assertEqual(pd.get('key_a'), 'value_a')
-        self.assertEqual(pd.get('key_b', 'absent'), 'value_b')
-        pd['key_a'] = 'value_aaaaaa'
-        self.assertEqual(pd['key_a'], 'value_aaaaaa')
-        self.assertEqual(pd['key_b'], 'value_b')
-
-    def test_delete(self):
-        pd = pdict.PDict(self.path, 'pd')
-        pd['key_a'] = 'value_a'
-        pd['key_b'] = 'value_b'
-        self.assertEqual(pd['key_a'], 'value_a')
-        self.assertEqual(pd['key_b'], 'value_b')
-        del pd['key_a']
-        self.assertFalse('key_a' in pd)
-        self.assertRaises(KeyError, lambda: pd['key_a'])
-        self.assertEqual(pd['key_b'], 'value_b')
-
-    def test_two_dicts(self):
-        pd_1 = pdict.PDict(self.path, '1')
-        pd_2 = pdict.PDict(self.path, '2')
-        pd_1['key_a'] = 'value_a'
-        pd_2['key_b'] = 'value_b'
-        self.assertEqual(pd_1['key_a'], 'value_a')
-        self.assertEqual(pd_2['key_b'], 'value_b')
-        self.assertRaises(KeyError, lambda: pd_1['key_b'])
-        self.assertRaises(KeyError, lambda: pd_2['key_a'])
+
+import shutil
+import tempfile
+import unittest
+
+from persistqueue import pdict
+
+
+class PDictTest(unittest.TestCase):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='pdict')
+
+    def tearDown(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+
+    def test_unsupported(self):
+        pd = pdict.PDict(self.path, 'pd')
+        pd['key_a'] = 'value_a'
+        self.assertRaises(NotImplementedError, pd.keys)
+        self.assertRaises(NotImplementedError, pd.iterkeys)
+        self.assertRaises(NotImplementedError, pd.values)
+        self.assertRaises(NotImplementedError, pd.itervalues)
+        self.assertRaises(NotImplementedError, pd.items)
+        self.assertRaises(NotImplementedError, pd.iteritems)
+
+        def _for():
+            for _ in pd:
+                pass
+        self.assertRaises(NotImplementedError, _for)
+
+    def test_add(self):
+        pd = pdict.PDict(self.path, 'pd')
+        pd['key_a'] = 'value_a'
+        self.assertEqual(pd['key_a'], 'value_a')
+        self.assertTrue('key_a' in pd)
+        self.assertFalse('key_b' in pd)
+        self.assertEqual(pd.get('key_a'), 'value_a')
+        self.assertEqual(pd.get('key_b'), None)
+        self.assertEqual(pd.get('key_b', 'absent'), 'absent')
+        self.assertRaises(KeyError, lambda: pd['key_b'])
+        pd['key_b'] = 'value_b'
+        self.assertEqual(pd['key_a'], 'value_a')
+        self.assertEqual(pd['key_b'], 'value_b')
+
+    def test_set(self):
+        pd = pdict.PDict(self.path, 'pd')
+        pd['key_a'] = 'value_a'
+        pd['key_b'] = 'value_b'
+        self.assertEqual(pd['key_a'], 'value_a')
+        self.assertEqual(pd['key_b'], 'value_b')
+        self.assertEqual(pd.get('key_a'), 'value_a')
+        self.assertEqual(pd.get('key_b', 'absent'), 'value_b')
+        pd['key_a'] = 'value_aaaaaa'
+        self.assertEqual(pd['key_a'], 'value_aaaaaa')
+        self.assertEqual(pd['key_b'], 'value_b')
+
+    def test_delete(self):
+        pd = pdict.PDict(self.path, 'pd')
+        pd['key_a'] = 'value_a'
+        pd['key_b'] = 'value_b'
+        self.assertEqual(pd['key_a'], 'value_a')
+        self.assertEqual(pd['key_b'], 'value_b')
+        del pd['key_a']
+        self.assertFalse('key_a' in pd)
+        self.assertRaises(KeyError, lambda: pd['key_a'])
+        self.assertEqual(pd['key_b'], 'value_b')
+
+    def test_two_dicts(self):
+        pd_1 = pdict.PDict(self.path, '1')
+        pd_2 = pdict.PDict(self.path, '2')
+        pd_1['key_a'] = 'value_a'
+        pd_2['key_b'] = 'value_b'
+        self.assertEqual(pd_1['key_a'], 'value_a')
+        self.assertEqual(pd_2['key_b'], 'value_b')
+        self.assertRaises(KeyError, lambda: pd_1['key_b'])
+        self.assertRaises(KeyError, lambda: pd_2['key_a'])
```

### Comparing `persist-queue-0.8.0b0/persistqueue/tests/test_queue.py` & `persist-queue-0.8.1/persistqueue/tests/test_queue.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,325 +1,340 @@
-# coding=utf-8
-
-import os
-import pickle
-import random
-import shutil
-import sys
-import tempfile
-import unittest
-from collections import namedtuple
-from nose2.tools import params
-from threading import Thread
-
-from persistqueue.serializers import json as serializers_json
-from persistqueue.serializers import pickle as serializers_pickle
-from persistqueue.serializers import msgpack as serializers_msgpack
-
-from persistqueue import Queue, Empty, Full
-
-# map keys as params for readable errors from nose
-serializer_params = {
-    "serializer=default": {},
-    "serializer=json": {"serializer": serializers_json},
-    "serializer=msgpack": {"serializer": serializers_msgpack},
-    "serializer=pickle": {"serializer": serializers_pickle},
-}
-
-
-class PersistTest(unittest.TestCase):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='queue')
-
-    def tearDown(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-
-    @params(*serializer_params)
-    def test_open_close_single(self, serializer):
-        """Write 1 item, close, reopen checking if same item is there"""
-
-        q = Queue(self.path, **serializer_params[serializer])
-        q.put('var1')
-        del q
-        q = Queue(self.path, **serializer_params[serializer])
-        self.assertEqual(1, q.qsize())
-        self.assertEqual('var1', q.get())
-        q.task_done()
-        del q
-
-    def test_empty(self):
-        q = Queue(self.path)
-        self.assertEqual(q.empty(), True)
-
-        q.put('var1')
-        self.assertEqual(q.empty(), False)
-
-        q.get()
-        self.assertEqual(q.empty(), True)
-
-    @params(*serializer_params)
-    def test_open_close_1000(self, serializer):
-        """Write 1000 items, close, reopen checking if all items are there"""
-
-        q = Queue(self.path, **serializer_params[serializer])
-        for i in range(1000):
-            q.put('var%d' % i)
-        self.assertEqual(1000, q.qsize())
-        del q
-        q = Queue(self.path, **serializer_params[serializer])
-        self.assertEqual(1000, q.qsize())
-        for i in range(1000):
-            data = q.get()
-            self.assertEqual('var%d' % i, data)
-            q.task_done()
-        with self.assertRaises(Empty):
-            q.get_nowait()
-        # assert adding another one still works
-        q.put('foobar')
-        data = q.get()
-
-    @params(*serializer_params)
-    def test_partial_write(self, serializer):
-        """Test recovery from previous crash w/ partial write"""
-
-        q = Queue(self.path, **serializer_params[serializer])
-        for i in range(100):
-            q.put('var%d' % i)
-        del q
-        with open(os.path.join(self.path, 'q00000'), 'ab') as f:
-            pickle.dump('文字化け', f)
-        q = Queue(self.path, **serializer_params[serializer])
-        self.assertEqual(100, q.qsize())
-        for i in range(100):
-            self.assertEqual('var%d' % i, q.get())
-            q.task_done()
-        with self.assertRaises(Empty):
-            q.get_nowait()
-
-    @params(*serializer_params)
-    def test_random_read_write(self, serializer):
-        """Test random read/write"""
-
-        q = Queue(self.path, **serializer_params[serializer])
-        n = 0
-        for i in range(1000):
-            if random.random() < 0.5:
-                if n > 0:
-                    q.get_nowait()
-                    q.task_done()
-                    n -= 1
-                else:
-                    with self.assertRaises(Empty):
-                        q.get_nowait()
-            else:
-                q.put('var%d' % random.getrandbits(16))
-                n += 1
-
-    @params(*serializer_params)
-    def test_multi_threaded(self, serializer):
-        """Create consumer and producer threads, check parallelism"""
-
-        q = Queue(self.path, **serializer_params[serializer])
-
-        def producer():
-            for i in range(1000):
-                q.put('var%d' % i)
-
-        def consumer():
-            for i in range(1000):
-                q.get()
-                q.task_done()
-
-        c = Thread(target=consumer)
-        c.start()
-        p = Thread(target=producer)
-        p.start()
-        c.join()
-        p.join()
-
-        q.join()
-        with self.assertRaises(Empty):
-            q.get_nowait()
-
-    @params(*serializer_params)
-    def test_garbage_on_head(self, serializer):
-        """Adds garbage to the queue head and let the internal integrity
-        checks fix it"""
-
-        q = Queue(self.path, **serializer_params[serializer])
-        q.put('var1')
-        del q
-
-        with open(os.path.join(self.path, 'q00000'), 'ab') as f:
-            f.write(b'garbage')
-        q = Queue(self.path, **serializer_params[serializer])
-        q.put('var2')
-
-        self.assertEqual(2, q.qsize())
-        self.assertEqual('var1', q.get())
-        q.task_done()
-
-    @params(*serializer_params)
-    def test_task_done_too_many_times(self, serializer):
-        """Test too many task_done called."""
-        q = Queue(self.path, **serializer_params[serializer])
-        q.put('var1')
-        q.get()
-        q.task_done()
-
-        with self.assertRaises(ValueError):
-            q.task_done()
-
-    @params(*serializer_params)
-    def test_get_timeout_negative(self, serializer):
-        q = Queue(self.path, **serializer_params[serializer])
-        q.put('var1')
-        with self.assertRaises(ValueError):
-            q.get(timeout=-1)
-
-    @params(*serializer_params)
-    def test_get_timeout(self, serializer):
-        """Test when get failed within timeout."""
-        q = Queue(self.path, **serializer_params[serializer])
-        q.put('var1')
-        q.get()
-        with self.assertRaises(Empty):
-            q.get(timeout=1)
-
-    @params(*serializer_params)
-    def test_put_nowait(self, serializer):
-        """Tests the put_nowait interface."""
-        q = Queue(self.path, **serializer_params[serializer])
-        q.put_nowait('var1')
-        self.assertEqual('var1', q.get())
-        q.task_done()
-
-    @params(*serializer_params)
-    def test_put_maxsize_reached(self, serializer):
-        """Test that maxsize reached."""
-        q = Queue(self.path, maxsize=10, **serializer_params[serializer])
-        for x in range(10):
-            q.put(x)
-
-        with self.assertRaises(Full):
-            q.put('full_now', block=False)
-
-    @params(*serializer_params)
-    def test_put_timeout_reached(self, serializer):
-        """Test put with block and timeout."""
-        q = Queue(self.path, maxsize=2, **serializer_params[serializer])
-        for x in range(2):
-            q.put(x)
-
-        with self.assertRaises(Full):
-            q.put('full_and_timeout', block=True, timeout=1)
-
-    @params(*serializer_params)
-    def test_put_timeout_negative(self, serializer):
-        """Test and put with timeout < 0"""
-        q = Queue(self.path, maxsize=1, **serializer_params[serializer])
-        with self.assertRaises(ValueError):
-            q.put('var1', timeout=-1)
-
-    @params(*serializer_params)
-    def test_put_block_and_wait(self, serializer):
-        """Test block until queue is not full."""
-        q = Queue(self.path, maxsize=10, **serializer_params[serializer])
-
-        def consumer():
-            for i in range(5):
-                q.get()
-                q.task_done()
-
-        def producer():
-            for j in range(16):
-                q.put('var%d' % j)
-
-        p = Thread(target=producer)
-        p.start()
-        c = Thread(target=consumer)
-        c.start()
-        c.join()
-        val = q.get_nowait()
-        p.join()
-        self.assertEqual('var5', val)
-
-    @params(*serializer_params)
-    def test_clear_tail_file(self, serializer):
-        """Test that only remove tail file when calling task_done."""
-        q = Queue(self.path, chunksize=10, **serializer_params[serializer])
-        for i in range(35):
-            q.put('var%d' % i)
-
-        for _ in range(15):
-            q.get()
-
-        q = Queue(self.path, chunksize=10, **serializer_params[serializer])
-        self.assertEqual(q.qsize(), 35)
-
-        for _ in range(15):
-            q.get()
-        # the first tail file gets removed after task_done
-        q.task_done()
-        for _ in range(16):
-            q.get()
-        # the second and third files get removed after task_done
-        q.task_done()
-        self.assertEqual(q.qsize(), 4)
-
-    def test_protocol(self):
-        # test that protocol is set properly
-        expect_protocol = 2 if sys.version_info[0] == 2 else 4
-        self.assertEqual(
-            serializers_pickle.protocol,
-            expect_protocol,
-        )
-
-        # test that protocol is used properly
-        serializer = namedtuple("Serializer", ["dump", "load"])(
-                serializers_pickle.dump, lambda fp: fp.read())
-
-        q = Queue(path=self.path, serializer=serializer)
-        q.put(b'a')
-        self.assertEqual(q.get(), pickle.dumps(b'a', protocol=expect_protocol))
-
-    @params(*serializer_params)
-    def test_del(self, serializer):
-        """test that __del__ can be called successfully"""
-        q = Queue(self.path, **serializer_params[serializer])
-        q.__del__()
-        self.assertTrue(q.headf.closed)
-        self.assertTrue(q.tailf.closed)
-
-    @params(*serializer_params)
-    def test_autosave_get(self, serializer):
-        """test the autosave feature saves on get()"""
-        q = Queue(self.path, autosave=True, **serializer_params[serializer])
-        q.put('var1')
-        q.put('var2')
-        self.assertEqual('var1', q.get())
-        del q
-        # queue should save on get(), only one item should remain
-        q = Queue(self.path, autosave=True, **serializer_params[serializer])
-        self.assertEqual(1, q.qsize())
-        self.assertEqual('var2', q.get())
-        del q
-
-    @params(*serializer_params)
-    def test_autosave_join(self, serializer):
-        """Enabling autosave should still allow task_done/join behavior"""
-        q = Queue(self.path, autosave=True, **serializer_params[serializer])
-        for i in range(10):
-            q.put('var%d' % i)
-
-        def consumer():
-            for i in range(10):
-                q.get()
-                # this should still 'count down' properly and allow q.join()
-                # to finish
-                q.task_done()
-
-        c = Thread(target=consumer)
-        c.start()
-        q.join()
-        with self.assertRaises(Empty):
-            q.get_nowait()
+# coding=utf-8
+
+import os
+import pickle
+import random
+import shutil
+import sys
+import tempfile
+import unittest
+from collections import namedtuple
+from nose2.tools import params
+from threading import Thread
+
+from persistqueue.serializers import json as serializers_json
+from persistqueue.serializers import pickle as serializers_pickle
+from persistqueue.serializers import msgpack as serializers_msgpack
+from persistqueue.serializers import cbor2 as serializers_cbor2
+
+from persistqueue import Queue, Empty, Full
+
+# map keys as params for readable errors from nose
+serializer_params = {
+    "serializer=default": {},
+    "serializer=json": {"serializer": serializers_json},
+    "serializer=msgpack": {"serializer": serializers_msgpack},
+    "serializer=cbor2": {"serializer": serializers_cbor2},
+    "serializer=pickle": {"serializer": serializers_pickle},
+}
+
+
+class PersistTest(unittest.TestCase):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='queue')
+
+    def tearDown(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+
+    @params(*serializer_params)
+    def test_open_close_single(self, serializer):
+        """Write 1 item, close, reopen checking if same item is there"""
+
+        q = Queue(self.path, **serializer_params[serializer])
+        q.put('var1')
+        del q
+        q = Queue(self.path, **serializer_params[serializer])
+        self.assertEqual(1, q.qsize())
+        self.assertEqual('var1', q.get())
+        q.task_done()
+        del q
+
+    def test_empty(self):
+        q = Queue(self.path)
+        self.assertEqual(q.empty(), True)
+
+        q.put('var1')
+        self.assertEqual(q.empty(), False)
+
+        q.get()
+        self.assertEqual(q.empty(), True)
+
+    def test_full(self):
+        q = Queue(self.path, maxsize=3)
+
+        for i in range(1, q.maxsize):
+            q.put('var{}'.format(i))
+        self.assertEqual(q.full(), False)
+
+        q.put('var{}'.format(q.maxsize))
+        self.assertEqual(q.full(), True)
+
+        q.get()
+        self.assertEqual(q.full(), False)
+
+    @params(*serializer_params)
+    def test_open_close_1000(self, serializer):
+        """Write 1000 items, close, reopen checking if all items are there"""
+
+        q = Queue(self.path, **serializer_params[serializer])
+        for i in range(1000):
+            q.put('var%d' % i)
+        self.assertEqual(1000, q.qsize())
+        del q
+        q = Queue(self.path, **serializer_params[serializer])
+        self.assertEqual(1000, q.qsize())
+        for i in range(1000):
+            data = q.get()
+            self.assertEqual('var%d' % i, data)
+            q.task_done()
+        with self.assertRaises(Empty):
+            q.get_nowait()
+        # assert adding another one still works
+        q.put('foobar')
+        data = q.get()
+
+    @params(*serializer_params)
+    def test_partial_write(self, serializer):
+        """Test recovery from previous crash w/ partial write"""
+
+        q = Queue(self.path, **serializer_params[serializer])
+        for i in range(100):
+            q.put('var%d' % i)
+        del q
+        with open(os.path.join(self.path, 'q00000'), 'ab') as f:
+            pickle.dump('文字化け', f)
+        q = Queue(self.path, **serializer_params[serializer])
+        self.assertEqual(100, q.qsize())
+        for i in range(100):
+            self.assertEqual('var%d' % i, q.get())
+            q.task_done()
+        with self.assertRaises(Empty):
+            q.get_nowait()
+
+    @params(*serializer_params)
+    def test_random_read_write(self, serializer):
+        """Test random read/write"""
+
+        q = Queue(self.path, **serializer_params[serializer])
+        n = 0
+        for i in range(1000):
+            if random.random() < 0.5:
+                if n > 0:
+                    q.get_nowait()
+                    q.task_done()
+                    n -= 1
+                else:
+                    with self.assertRaises(Empty):
+                        q.get_nowait()
+            else:
+                q.put('var%d' % random.getrandbits(16))
+                n += 1
+
+    @params(*serializer_params)
+    def test_multi_threaded(self, serializer):
+        """Create consumer and producer threads, check parallelism"""
+
+        q = Queue(self.path, **serializer_params[serializer])
+
+        def producer():
+            for i in range(1000):
+                q.put('var%d' % i)
+
+        def consumer():
+            for i in range(1000):
+                q.get()
+                q.task_done()
+
+        c = Thread(target=consumer)
+        c.start()
+        p = Thread(target=producer)
+        p.start()
+        c.join()
+        p.join()
+
+        q.join()
+        with self.assertRaises(Empty):
+            q.get_nowait()
+
+    @params(*serializer_params)
+    def test_garbage_on_head(self, serializer):
+        """Adds garbage to the queue head and let the internal integrity
+        checks fix it"""
+
+        q = Queue(self.path, **serializer_params[serializer])
+        q.put('var1')
+        del q
+
+        with open(os.path.join(self.path, 'q00000'), 'ab') as f:
+            f.write(b'garbage')
+        q = Queue(self.path, **serializer_params[serializer])
+        q.put('var2')
+
+        self.assertEqual(2, q.qsize())
+        self.assertEqual('var1', q.get())
+        q.task_done()
+
+    @params(*serializer_params)
+    def test_task_done_too_many_times(self, serializer):
+        """Test too many task_done called."""
+        q = Queue(self.path, **serializer_params[serializer])
+        q.put('var1')
+        q.get()
+        q.task_done()
+
+        with self.assertRaises(ValueError):
+            q.task_done()
+
+    @params(*serializer_params)
+    def test_get_timeout_negative(self, serializer):
+        q = Queue(self.path, **serializer_params[serializer])
+        q.put('var1')
+        with self.assertRaises(ValueError):
+            q.get(timeout=-1)
+
+    @params(*serializer_params)
+    def test_get_timeout(self, serializer):
+        """Test when get failed within timeout."""
+        q = Queue(self.path, **serializer_params[serializer])
+        q.put('var1')
+        q.get()
+        with self.assertRaises(Empty):
+            q.get(timeout=1)
+
+    @params(*serializer_params)
+    def test_put_nowait(self, serializer):
+        """Tests the put_nowait interface."""
+        q = Queue(self.path, **serializer_params[serializer])
+        q.put_nowait('var1')
+        self.assertEqual('var1', q.get())
+        q.task_done()
+
+    @params(*serializer_params)
+    def test_put_maxsize_reached(self, serializer):
+        """Test that maxsize reached."""
+        q = Queue(self.path, maxsize=10, **serializer_params[serializer])
+        for x in range(10):
+            q.put(x)
+
+        with self.assertRaises(Full):
+            q.put('full_now', block=False)
+
+    @params(*serializer_params)
+    def test_put_timeout_reached(self, serializer):
+        """Test put with block and timeout."""
+        q = Queue(self.path, maxsize=2, **serializer_params[serializer])
+        for x in range(2):
+            q.put(x)
+
+        with self.assertRaises(Full):
+            q.put('full_and_timeout', block=True, timeout=1)
+
+    @params(*serializer_params)
+    def test_put_timeout_negative(self, serializer):
+        """Test and put with timeout < 0"""
+        q = Queue(self.path, maxsize=1, **serializer_params[serializer])
+        with self.assertRaises(ValueError):
+            q.put('var1', timeout=-1)
+
+    @params(*serializer_params)
+    def test_put_block_and_wait(self, serializer):
+        """Test block until queue is not full."""
+        q = Queue(self.path, maxsize=10, **serializer_params[serializer])
+
+        def consumer():
+            for i in range(5):
+                q.get()
+                q.task_done()
+
+        def producer():
+            for j in range(16):
+                q.put('var%d' % j)
+
+        p = Thread(target=producer)
+        p.start()
+        c = Thread(target=consumer)
+        c.start()
+        c.join()
+        val = q.get_nowait()
+        p.join()
+        self.assertEqual('var5', val)
+
+    @params(*serializer_params)
+    def test_clear_tail_file(self, serializer):
+        """Test that only remove tail file when calling task_done."""
+        q = Queue(self.path, chunksize=10, **serializer_params[serializer])
+        for i in range(35):
+            q.put('var%d' % i)
+
+        for _ in range(15):
+            q.get()
+
+        q = Queue(self.path, chunksize=10, **serializer_params[serializer])
+        self.assertEqual(q.qsize(), 35)
+
+        for _ in range(15):
+            q.get()
+        # the first tail file gets removed after task_done
+        q.task_done()
+        for _ in range(16):
+            q.get()
+        # the second and third files get removed after task_done
+        q.task_done()
+        self.assertEqual(q.qsize(), 4)
+
+    def test_protocol(self):
+        # test that protocol is set properly
+        expect_protocol = 2 if sys.version_info[0] == 2 else 4
+        self.assertEqual(
+            serializers_pickle.protocol,
+            expect_protocol,
+        )
+
+        # test that protocol is used properly
+        serializer = namedtuple("Serializer", ["dump", "load"])(
+                serializers_pickle.dump, lambda fp: fp.read())
+
+        q = Queue(path=self.path, serializer=serializer)
+        q.put(b'a')
+        self.assertEqual(q.get(), pickle.dumps(b'a', protocol=expect_protocol))
+
+    @params(*serializer_params)
+    def test_del(self, serializer):
+        """test that __del__ can be called successfully"""
+        q = Queue(self.path, **serializer_params[serializer])
+        q.__del__()
+        self.assertTrue(q.headf.closed)
+        self.assertTrue(q.tailf.closed)
+
+    @params(*serializer_params)
+    def test_autosave_get(self, serializer):
+        """test the autosave feature saves on get()"""
+        q = Queue(self.path, autosave=True, **serializer_params[serializer])
+        q.put('var1')
+        q.put('var2')
+        self.assertEqual('var1', q.get())
+        del q
+        # queue should save on get(), only one item should remain
+        q = Queue(self.path, autosave=True, **serializer_params[serializer])
+        self.assertEqual(1, q.qsize())
+        self.assertEqual('var2', q.get())
+        del q
+
+    @params(*serializer_params)
+    def test_autosave_join(self, serializer):
+        """Enabling autosave should still allow task_done/join behavior"""
+        q = Queue(self.path, autosave=True, **serializer_params[serializer])
+        for i in range(10):
+            q.put('var%d' % i)
+
+        def consumer():
+            for i in range(10):
+                q.get()
+                # this should still 'count down' properly and allow q.join()
+                # to finish
+                q.task_done()
+
+        c = Thread(target=consumer)
+        c.start()
+        q.join()
+        with self.assertRaises(Empty):
+            q.get_nowait()
```

### Comparing `persist-queue-0.8.0b0/persistqueue/tests/test_sqlqueue.py` & `persist-queue-0.8.1/persistqueue/tests/test_sqlqueue.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,467 +1,491 @@
-# coding=utf-8
-
-import random
-import shutil
-import sys
-import tempfile
-import unittest
-from threading import Thread
-
-from persistqueue import SQLiteQueue, FILOSQLiteQueue, UniqueQ
-from persistqueue import Empty
-from persistqueue.serializers import json as serializers_json
-from persistqueue.serializers import pickle as serializers_pickle
-from persistqueue.serializers import msgpack as serializers_msgpack
-
-
-class SQLite3QueueTest(unittest.TestCase):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='sqlqueue')
-        self.auto_commit = True
-        self.queue_class = SQLiteQueue
-
-    def tearDown(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-
-    def test_raise_empty(self):
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-
-        q.put('first')
-        d = q.get()
-        self.assertEqual('first', d)
-        self.assertRaises(Empty, q.get, block=False)
-        self.assertRaises(Empty, q.get_nowait)
-
-        # assert with timeout
-        self.assertRaises(Empty, q.get, block=True, timeout=1.0)
-        # assert with negative timeout
-        self.assertRaises(ValueError, q.get, block=True, timeout=-1.0)
-        del q
-
-    def test_empty(self):
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        self.assertEqual(q.empty(), True)
-
-        q.put('first')
-        self.assertEqual(q.empty(), False)
-
-        q.get()
-        self.assertEqual(q.empty(), True)
-
-    def test_open_close_single(self):
-        """Write 1 item, close, reopen checking if same item is there"""
-
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        q.put(b'var1')
-        del q
-        q = SQLiteQueue(self.path)
-        self.assertEqual(1, q.qsize())
-        self.assertEqual(b'var1', q.get())
-
-    def test_open_close_1000(self):
-        """Write 1000 items, close, reopen checking if all items are there"""
-
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        for i in range(1000):
-            q.put('var%d' % i)
-
-        self.assertEqual(1000, q.qsize())
-        del q
-        q = SQLiteQueue(self.path)
-        self.assertEqual(1000, q.qsize())
-        for i in range(1000):
-            data = q.get()
-            self.assertEqual('var%d' % i, data)
-        # assert adding another one still works
-        q.put('foobar')
-        data = q.get()
-        q.shrink_disk_usage()
-        self.assertEqual('foobar', data)
-
-    def test_random_read_write(self):
-        """Test random read/write"""
-
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        n = 0
-        for _ in range(1000):
-            if random.random() < 0.5:
-                if n > 0:
-                    q.get()
-                    n -= 1
-                else:
-                    self.assertRaises(Empty, q.get, block=False)
-            else:
-                q.put('var%d' % random.getrandbits(16))
-                n += 1
-
-    def test_multi_threaded_parallel(self):
-        """Create consumer and producer threads, check parallelism"""
-
-        # self.skipTest("Not supported multi-thread.")
-
-        m_queue = SQLiteQueue(path=self.path, multithreading=True,
-                              auto_commit=self.auto_commit)
-
-        def producer():
-            for i in range(1000):
-                m_queue.put('var%d' % i)
-
-        def consumer():
-            for i in range(1000):
-                x = m_queue.get(block=True)
-                self.assertEqual('var%d' % i, x)
-
-        c = Thread(target=consumer)
-        c.start()
-        p = Thread(target=producer)
-        p.start()
-        p.join()
-        c.join()
-        self.assertEqual(0, m_queue.size)
-        self.assertEqual(0, len(m_queue))
-        self.assertRaises(Empty, m_queue.get, block=False)
-
-    def test_multi_threaded_multi_producer(self):
-        """Test sqlqueue can be used by multiple producers."""
-        queue = self.queue_class(path=self.path, multithreading=True,
-                                 auto_commit=self.auto_commit)
-
-        def producer(seq):
-            for i in range(10):
-                queue.put('var%d' % (i + (seq * 10)))
-
-        def consumer():
-            for _ in range(100):
-                data = queue.get(block=True)
-                self.assertTrue('var' in data)
-
-        c = Thread(target=consumer)
-        c.start()
-        producers = []
-        for seq in range(10):
-            t = Thread(target=producer, args=(seq,))
-            t.start()
-            producers.append(t)
-
-        for t in producers:
-            t.join()
-
-        c.join()
-
-    def test_multiple_consumers(self):
-        """Test sqlqueue can be used by multiple consumers."""
-
-        queue = self.queue_class(path=self.path, multithreading=True,
-                                 auto_commit=self.auto_commit)
-
-        def producer():
-            for x in range(1000):
-                queue.put('var%d' % x)
-
-        counter = []
-        # Set all to 0
-        for _ in range(1000):
-            counter.append(0)
-
-        def consumer(index):
-            for i in range(200):
-                data = queue.get(block=True)
-                self.assertTrue('var' in data)
-                counter[index * 200 + i] = data
-
-        p = Thread(target=producer)
-        p.start()
-        consumers = []
-        for index in range(5):
-            t = Thread(target=consumer, args=(index,))
-            t.start()
-            consumers.append(t)
-
-        p.join()
-        for t in consumers:
-            t.join()
-
-        self.assertEqual(0, queue.qsize())
-        for x in range(1000):
-            self.assertNotEqual(0, counter[x],
-                                "not 0 for counter's index %s" % x)
-
-        self.assertEqual(len(set(counter)), len(counter))
-
-    def test_task_done_with_restart(self):
-        """Test that items are not deleted before task_done."""
-
-        q = self.queue_class(path=self.path, auto_commit=False)
-
-        for i in range(1, 11):
-            q.put(i)
-
-        self.assertEqual(1, q.get())
-        self.assertEqual(2, q.get())
-        # size is correct before task_done
-        self.assertEqual(8, q.qsize())
-        q.task_done()
-        # make sure the size still correct
-        self.assertEqual(8, q.qsize())
-
-        self.assertEqual(3, q.get())
-        # without task done
-        del q
-        q = SQLiteQueue(path=self.path, auto_commit=False)
-        # After restart, the qsize and head item are the same
-        self.assertEqual(8, q.qsize())
-        # After restart, the queue still works
-        self.assertEqual(3, q.get())
-        self.assertEqual(7, q.qsize())
-
-    def test_protocol_1(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-        q = self.queue_class(path=self.path)
-        self.assertEqual(q._serializer.protocol,
-                         2 if sys.version_info[0] == 2 else 4)
-
-    def test_protocol_2(self):
-        q = self.queue_class(path=self.path)
-        self.assertEqual(q._serializer.protocol,
-                         2 if sys.version_info[0] == 2 else 4)
-
-    def test_json_serializer(self):
-        q = self.queue_class(
-            path=self.path,
-            serializer=serializers_json)
-        x = dict(
-            a=1,
-            b=2,
-            c=dict(
-                d=list(range(5)),
-                e=[1]
-            ))
-        q.put(x)
-        self.assertEqual(q.get(), x)
-
-    def test_put_0(self):
-        q = self.queue_class(path=self.path)
-        q.put(0)
-        d = q.get(block=False)
-        self.assertIsNotNone(d)
-
-    def test_get_id(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        val2_id = q.put("val2")
-        q.put("val3")
-        item = q.get(id=val2_id)
-        # item id should be 2
-        self.assertEqual(val2_id, 2)
-        # item should get val2
-        self.assertEqual(item, 'val2')
-
-    def test_get_raw(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        item = q.get(raw=True)
-        # item should get val2
-        self.assertEqual(True, "pqid" in item)
-        self.assertEqual(item.get("data"), 'val1')
-
-    def test_queue(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        q.put("val2")
-        q.put("val3")
-        # queue should get the three items
-        d = q.queue()
-        self.assertEqual(len(d), 3)
-        self.assertEqual(d[1].get("data"), "val2")
-
-    def test_update(self):
-        q = self.queue_class(path=self.path)
-        qid = q.put("val1")
-        q.update(item="val2", id=qid)
-        item = q.get(id=qid)
-        self.assertEqual(item, "val2")
-
-
-class SQLite3QueueNoAutoCommitTest(SQLite3QueueTest):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='sqlqueue_auto_commit')
-        self.auto_commit = False
-        self.queue_class = SQLiteQueue
-
-    def test_multiple_consumers(self):
-        """
-        FAIL: test_multiple_consumers (
-        -tests.test_sqlqueue.SQLite3QueueNoAutoCommitTest)
-        Test sqlqueue can be used by multiple consumers.
-        ----------------------------------------------------------------------
-        Traceback (most recent call last):
-        File "persist-queue\tests\test_sqlqueue.py", line 183,
-        -in test_multiple_consumers
-        self.assertEqual(0, queue.qsize())
-        AssertionError: 0 != 72
-        :return:
-        """
-        self.skipTest('Skipped due to a known bug above.')
-
-
-class SQLite3QueueInMemory(SQLite3QueueTest):
-    skipstr = 'Skipped due to occasional crash during multithreading mode.'
-
-    def setUp(self):
-        self.path = ":memory:"
-        self.auto_commit = True
-        self.queue_class = SQLiteQueue
-
-    def test_open_close_1000(self):
-        self.skipTest('Memory based sqlite is not persistent.')
-
-    def test_open_close_single(self):
-        self.skipTest('Memory based sqlite is not persistent.')
-
-    def test_multiple_consumers(self):
-        self.skipTest(self.skipstr)
-
-    def test_multi_threaded_multi_producer(self):
-        self.skipTest(self.skipstr)
-
-    def test_multi_threaded_parallel(self):
-        self.skipTest(self.skipstr)
-
-    def test_task_done_with_restart(self):
-        self.skipTest('Skipped due to not persistent.')
-
-    def test_protocol_2(self):
-        self.skipTest('In memory queue is always new.')
-
-
-class FILOSQLite3QueueTest(unittest.TestCase):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='filo_sqlqueue')
-        self.auto_commit = True
-        self.queue_class = SQLiteQueue
-
-    def tearDown(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-
-    def test_open_close_1000(self):
-        """Write 1000 items, close, reopen checking if all items are there"""
-
-        q = FILOSQLiteQueue(self.path, auto_commit=self.auto_commit)
-        for i in range(1000):
-            q.put('var%d' % i)
-        self.assertEqual(1000, q.qsize())
-        del q
-        q = FILOSQLiteQueue(self.path)
-        self.assertEqual(1000, q.qsize())
-        for i in range(1000):
-            data = q.get()
-            self.assertEqual('var%d' % (999 - i), data)
-        # assert adding another one still works
-        q.put('foobar')
-        data = q.get()
-        self.assertEqual('foobar', data)
-
-
-class FILOSQLite3QueueNoAutoCommitTest(FILOSQLite3QueueTest):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='filo_sqlqueue_auto_commit')
-        self.auto_commit = False
-        self.queue_class = FILOSQLiteQueue
-
-
-class SQLite3UniqueQueueTest(unittest.TestCase):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='sqlqueue')
-        self.auto_commit = True
-        self.queue_class = UniqueQ
-
-    def test_add_duplicate_item(self):
-        q = UniqueQ(self.path)
-        q.put(1111)
-        self.assertEqual(1, q.size)
-        # put duplicate item
-        q.put(1111)
-        self.assertEqual(1, q.size)
-
-        q.put(2222)
-        self.assertEqual(2, q.size)
-
-        del q
-        q = UniqueQ(self.path)
-        self.assertEqual(2, q.size)
-
-    def test_multiple_consumers(self):
-        """Test UniqueQ can be used by multiple consumers."""
-
-        queue = UniqueQ(path=self.path, multithreading=True,
-                        auto_commit=self.auto_commit)
-
-        def producer():
-            for x in range(1000):
-                queue.put('var%d' % x)
-
-        counter = []
-        # Set all to 0
-        for _ in range(1000):
-            counter.append(0)
-
-        def consumer(index):
-            for i in range(200):
-                data = queue.get(block=True)
-                self.assertTrue('var' in data)
-                counter[index * 200 + i] = data
-
-        p = Thread(target=producer)
-        p.start()
-        consumers = []
-        for index in range(5):
-            t = Thread(target=consumer, args=(index,))
-            t.start()
-            consumers.append(t)
-
-        p.join()
-        for t in consumers:
-            t.join()
-
-        self.assertEqual(0, queue.qsize())
-        for x in range(1000):
-            self.assertNotEqual(0, counter[x],
-                                "not 0 for counter's index %s" % x)
-
-        self.assertEqual(len(set(counter)), len(counter))
-
-    def test_unique_dictionary_serialization_pickle(self):
-        queue = UniqueQ(
-            path=self.path,
-            multithreading=True,
-            auto_commit=self.auto_commit,
-            serializer=serializers_pickle,
-        )
-        queue.put({"foo": 1, "bar": 2})
-        self.assertEqual(queue.total, 1)
-        queue.put({"bar": 2, "foo": 1})
-        self.assertEqual(queue.total, 1)
-
-    def test_unique_dictionary_serialization_msgpack(self):
-        queue = UniqueQ(
-            path=self.path,
-            multithreading=True,
-            auto_commit=self.auto_commit,
-            serializer=serializers_msgpack
-        )
-        queue.put({"foo": 1, "bar": 2})
-        self.assertEqual(queue.total, 1)
-        queue.put({"bar": 2, "foo": 1})
-        self.assertEqual(queue.total, 1)
-
-    def test_unique_dictionary_serialization_json(self):
-        queue = UniqueQ(
-            path=self.path,
-            multithreading=True,
-            auto_commit=self.auto_commit,
-            serializer=serializers_json
-        )
-        queue.put({"foo": 1, "bar": 2})
-        self.assertEqual(queue.total, 1)
-        queue.put({"bar": 2, "foo": 1})
-        self.assertEqual(queue.total, 1)
+# coding=utf-8
+
+import random
+import shutil
+import sys
+import tempfile
+import unittest
+from threading import Thread
+
+from persistqueue import SQLiteQueue, FILOSQLiteQueue, UniqueQ
+from persistqueue import Empty
+from persistqueue.serializers import json as serializers_json
+from persistqueue.serializers import pickle as serializers_pickle
+from persistqueue.serializers import msgpack as serializers_msgpack
+from persistqueue.serializers import cbor2 as serializers_cbor2
+
+
+class SQLite3QueueTest(unittest.TestCase):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='sqlqueue')
+        self.auto_commit = True
+        self.queue_class = SQLiteQueue
+
+    def tearDown(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+
+    def test_raise_empty(self):
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+
+        q.put('first')
+        d = q.get()
+        self.assertEqual('first', d)
+        self.assertRaises(Empty, q.get, block=False)
+        self.assertRaises(Empty, q.get_nowait)
+
+        # assert with timeout
+        self.assertRaises(Empty, q.get, block=True, timeout=1.0)
+        # assert with negative timeout
+        self.assertRaises(ValueError, q.get, block=True, timeout=-1.0)
+        del q
+
+    def test_empty(self):
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        self.assertEqual(q.empty(), True)
+
+        q.put('first')
+        self.assertEqual(q.empty(), False)
+
+        q.get()
+        self.assertEqual(q.empty(), True)
+
+    def test_full(self):
+        # SQL queue `full()` always returns `False` !!
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        self.assertEqual(q.full(), False)
+
+        q.put('first')
+        self.assertEqual(q.full(), False)
+
+        q.get()
+        self.assertEqual(q.full(), False)
+
+    def test_open_close_single(self):
+        """Write 1 item, close, reopen checking if same item is there"""
+
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        q.put(b'var1')
+        del q
+        q = SQLiteQueue(self.path)
+        self.assertEqual(1, q.qsize())
+        self.assertEqual(b'var1', q.get())
+
+    def test_open_close_1000(self):
+        """Write 1000 items, close, reopen checking if all items are there"""
+
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        for i in range(1000):
+            q.put('var%d' % i)
+
+        self.assertEqual(1000, q.qsize())
+        del q
+        q = SQLiteQueue(self.path)
+        self.assertEqual(1000, q.qsize())
+        for i in range(1000):
+            data = q.get()
+            self.assertEqual('var%d' % i, data)
+        # assert adding another one still works
+        q.put('foobar')
+        data = q.get()
+        q.shrink_disk_usage()
+        self.assertEqual('foobar', data)
+
+    def test_random_read_write(self):
+        """Test random read/write"""
+
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        n = 0
+        for _ in range(1000):
+            if random.random() < 0.5:
+                if n > 0:
+                    q.get()
+                    n -= 1
+                else:
+                    self.assertRaises(Empty, q.get, block=False)
+            else:
+                q.put('var%d' % random.getrandbits(16))
+                n += 1
+
+    def test_multi_threaded_parallel(self):
+        """Create consumer and producer threads, check parallelism"""
+
+        # self.skipTest("Not supported multi-thread.")
+
+        m_queue = SQLiteQueue(path=self.path, multithreading=True,
+                              auto_commit=self.auto_commit)
+
+        def producer():
+            for i in range(1000):
+                m_queue.put('var%d' % i)
+
+        def consumer():
+            for i in range(1000):
+                x = m_queue.get(block=True)
+                self.assertEqual('var%d' % i, x)
+
+        c = Thread(target=consumer)
+        c.start()
+        p = Thread(target=producer)
+        p.start()
+        p.join()
+        c.join()
+        self.assertEqual(0, m_queue.size)
+        self.assertEqual(0, len(m_queue))
+        self.assertRaises(Empty, m_queue.get, block=False)
+
+    def test_multi_threaded_multi_producer(self):
+        """Test sqlqueue can be used by multiple producers."""
+        queue = self.queue_class(path=self.path, multithreading=True,
+                                 auto_commit=self.auto_commit)
+
+        def producer(seq):
+            for i in range(10):
+                queue.put('var%d' % (i + (seq * 10)))
+
+        def consumer():
+            for _ in range(100):
+                data = queue.get(block=True)
+                self.assertTrue('var' in data)
+
+        c = Thread(target=consumer)
+        c.start()
+        producers = []
+        for seq in range(10):
+            t = Thread(target=producer, args=(seq,))
+            t.start()
+            producers.append(t)
+
+        for t in producers:
+            t.join()
+
+        c.join()
+
+    def test_multiple_consumers(self):
+        """Test sqlqueue can be used by multiple consumers."""
+
+        queue = self.queue_class(path=self.path, multithreading=True,
+                                 auto_commit=self.auto_commit)
+
+        def producer():
+            for x in range(1000):
+                queue.put('var%d' % x)
+
+        counter = []
+        # Set all to 0
+        for _ in range(1000):
+            counter.append(0)
+
+        def consumer(index):
+            for i in range(200):
+                data = queue.get(block=True)
+                self.assertTrue('var' in data)
+                counter[index * 200 + i] = data
+
+        p = Thread(target=producer)
+        p.start()
+        consumers = []
+        for index in range(5):
+            t = Thread(target=consumer, args=(index,))
+            t.start()
+            consumers.append(t)
+
+        p.join()
+        for t in consumers:
+            t.join()
+
+        self.assertEqual(0, queue.qsize())
+        for x in range(1000):
+            self.assertNotEqual(0, counter[x],
+                                "not 0 for counter's index %s" % x)
+
+        self.assertEqual(len(set(counter)), len(counter))
+
+    def test_task_done_with_restart(self):
+        """Test that items are not deleted before task_done."""
+
+        q = self.queue_class(path=self.path, auto_commit=False)
+
+        for i in range(1, 11):
+            q.put(i)
+
+        self.assertEqual(1, q.get())
+        self.assertEqual(2, q.get())
+        # size is correct before task_done
+        self.assertEqual(8, q.qsize())
+        q.task_done()
+        # make sure the size still correct
+        self.assertEqual(8, q.qsize())
+
+        self.assertEqual(3, q.get())
+        # without task done
+        del q
+        q = SQLiteQueue(path=self.path, auto_commit=False)
+        # After restart, the qsize and head item are the same
+        self.assertEqual(8, q.qsize())
+        # After restart, the queue still works
+        self.assertEqual(3, q.get())
+        self.assertEqual(7, q.qsize())
+
+    def test_protocol_1(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+        q = self.queue_class(path=self.path)
+        self.assertEqual(q._serializer.protocol,
+                         2 if sys.version_info[0] == 2 else 4)
+
+    def test_protocol_2(self):
+        q = self.queue_class(path=self.path)
+        self.assertEqual(q._serializer.protocol,
+                         2 if sys.version_info[0] == 2 else 4)
+
+    def test_json_serializer(self):
+        q = self.queue_class(
+            path=self.path,
+            serializer=serializers_json)
+        x = dict(
+            a=1,
+            b=2,
+            c=dict(
+                d=list(range(5)),
+                e=[1]
+            ))
+        q.put(x)
+        self.assertEqual(q.get(), x)
+
+    def test_put_0(self):
+        q = self.queue_class(path=self.path)
+        q.put(0)
+        d = q.get(block=False)
+        self.assertIsNotNone(d)
+
+    def test_get_id(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        val2_id = q.put("val2")
+        q.put("val3")
+        item = q.get(id=val2_id)
+        # item id should be 2
+        self.assertEqual(val2_id, 2)
+        # item should get val2
+        self.assertEqual(item, 'val2')
+
+    def test_get_raw(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        item = q.get(raw=True)
+        # item should get val2
+        self.assertEqual(True, "pqid" in item)
+        self.assertEqual(item.get("data"), 'val1')
+
+    def test_queue(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        q.put("val2")
+        q.put("val3")
+        # queue should get the three items
+        d = q.queue()
+        self.assertEqual(len(d), 3)
+        self.assertEqual(d[1].get("data"), "val2")
+
+    def test_update(self):
+        q = self.queue_class(path=self.path)
+        qid = q.put("val1")
+        q.update(item="val2", id=qid)
+        item = q.get(id=qid)
+        self.assertEqual(item, "val2")
+
+
+class SQLite3QueueNoAutoCommitTest(SQLite3QueueTest):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='sqlqueue_auto_commit')
+        self.auto_commit = False
+        self.queue_class = SQLiteQueue
+
+    def test_multiple_consumers(self):
+        """
+        FAIL: test_multiple_consumers (
+        -tests.test_sqlqueue.SQLite3QueueNoAutoCommitTest)
+        Test sqlqueue can be used by multiple consumers.
+        ----------------------------------------------------------------------
+        Traceback (most recent call last):
+        File "persist-queue\tests\test_sqlqueue.py", line 183,
+        -in test_multiple_consumers
+        self.assertEqual(0, queue.qsize())
+        AssertionError: 0 != 72
+        :return:
+        """
+        self.skipTest('Skipped due to a known bug above.')
+
+
+class SQLite3QueueInMemory(SQLite3QueueTest):
+    skipstr = 'Skipped due to occasional crash during multithreading mode.'
+
+    def setUp(self):
+        self.path = ":memory:"
+        self.auto_commit = True
+        self.queue_class = SQLiteQueue
+
+    def test_open_close_1000(self):
+        self.skipTest('Memory based sqlite is not persistent.')
+
+    def test_open_close_single(self):
+        self.skipTest('Memory based sqlite is not persistent.')
+
+    def test_multiple_consumers(self):
+        self.skipTest(self.skipstr)
+
+    def test_multi_threaded_multi_producer(self):
+        self.skipTest(self.skipstr)
+
+    def test_multi_threaded_parallel(self):
+        self.skipTest(self.skipstr)
+
+    def test_task_done_with_restart(self):
+        self.skipTest('Skipped due to not persistent.')
+
+    def test_protocol_2(self):
+        self.skipTest('In memory queue is always new.')
+
+
+class FILOSQLite3QueueTest(unittest.TestCase):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='filo_sqlqueue')
+        self.auto_commit = True
+        self.queue_class = SQLiteQueue
+
+    def tearDown(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+
+    def test_open_close_1000(self):
+        """Write 1000 items, close, reopen checking if all items are there"""
+
+        q = FILOSQLiteQueue(self.path, auto_commit=self.auto_commit)
+        for i in range(1000):
+            q.put('var%d' % i)
+        self.assertEqual(1000, q.qsize())
+        del q
+        q = FILOSQLiteQueue(self.path)
+        self.assertEqual(1000, q.qsize())
+        for i in range(1000):
+            data = q.get()
+            self.assertEqual('var%d' % (999 - i), data)
+        # assert adding another one still works
+        q.put('foobar')
+        data = q.get()
+        self.assertEqual('foobar', data)
+
+
+class FILOSQLite3QueueNoAutoCommitTest(FILOSQLite3QueueTest):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='filo_sqlqueue_auto_commit')
+        self.auto_commit = False
+        self.queue_class = FILOSQLiteQueue
+
+
+class SQLite3UniqueQueueTest(unittest.TestCase):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='sqlqueue')
+        self.auto_commit = True
+        self.queue_class = UniqueQ
+
+    def test_add_duplicate_item(self):
+        q = UniqueQ(self.path)
+        q.put(1111)
+        self.assertEqual(1, q.size)
+        # put duplicate item
+        q.put(1111)
+        self.assertEqual(1, q.size)
+
+        q.put(2222)
+        self.assertEqual(2, q.size)
+
+        del q
+        q = UniqueQ(self.path)
+        self.assertEqual(2, q.size)
+
+    def test_multiple_consumers(self):
+        """Test UniqueQ can be used by multiple consumers."""
+
+        queue = UniqueQ(path=self.path, multithreading=True,
+                        auto_commit=self.auto_commit)
+
+        def producer():
+            for x in range(1000):
+                queue.put('var%d' % x)
+
+        counter = []
+        # Set all to 0
+        for _ in range(1000):
+            counter.append(0)
+
+        def consumer(index):
+            for i in range(200):
+                data = queue.get(block=True)
+                self.assertTrue('var' in data)
+                counter[index * 200 + i] = data
+
+        p = Thread(target=producer)
+        p.start()
+        consumers = []
+        for index in range(5):
+            t = Thread(target=consumer, args=(index,))
+            t.start()
+            consumers.append(t)
+
+        p.join()
+        for t in consumers:
+            t.join()
+
+        self.assertEqual(0, queue.qsize())
+        for x in range(1000):
+            self.assertNotEqual(0, counter[x],
+                                "not 0 for counter's index %s" % x)
+
+        self.assertEqual(len(set(counter)), len(counter))
+
+    def test_unique_dictionary_serialization_pickle(self):
+        queue = UniqueQ(
+            path=self.path,
+            multithreading=True,
+            auto_commit=self.auto_commit,
+            serializer=serializers_pickle,
+        )
+        queue.put({"foo": 1, "bar": 2})
+        self.assertEqual(queue.total, 1)
+        queue.put({"bar": 2, "foo": 1})
+        self.assertEqual(queue.total, 1)
+
+    def test_unique_dictionary_serialization_msgpack(self):
+        queue = UniqueQ(
+            path=self.path,
+            multithreading=True,
+            auto_commit=self.auto_commit,
+            serializer=serializers_msgpack
+        )
+        queue.put({"foo": 1, "bar": 2})
+        self.assertEqual(queue.total, 1)
+        queue.put({"bar": 2, "foo": 1})
+        self.assertEqual(queue.total, 1)
+
+    def test_unique_dictionary_serialization_cbor2(self):
+        queue = UniqueQ(
+            path=self.path,
+            multithreading=True,
+            auto_commit=self.auto_commit,
+            serializer=serializers_cbor2
+        )
+        queue.put({"foo": 1, "bar": 2})
+        self.assertEqual(queue.total, 1)
+        queue.put({"bar": 2, "foo": 1})
+        self.assertEqual(queue.total, 1)
+
+    def test_unique_dictionary_serialization_json(self):
+        queue = UniqueQ(
+            path=self.path,
+            multithreading=True,
+            auto_commit=self.auto_commit,
+            serializer=serializers_json
+        )
+        queue.put({"foo": 1, "bar": 2})
+        self.assertEqual(queue.total, 1)
+        queue.put({"bar": 2, "foo": 1})
+        self.assertEqual(queue.total, 1)
```

### Comparing `persist-queue-0.8.0b0/persistqueue/tests/test_sqlackqueue.py` & `persist-queue-0.8.1/persistqueue/tests/test_sqlackqueue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,511 +1,522 @@
-# coding=utf-8
-
-import random
-import shutil
-import sys
-import tempfile
-import unittest
-from threading import Thread
-import uuid
-
-from persistqueue.sqlackqueue import (
-    SQLiteAckQueue,
-    FILOSQLiteAckQueue,
-    UniqueAckQ,
-)
-from persistqueue import Empty
-
-
-class SQLite3AckQueueTest(unittest.TestCase):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='sqlackqueue')
-        self.auto_commit = True
-        self.queue_class = SQLiteAckQueue
-
-    def tearDown(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-
-    def test_raise_empty(self):
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-
-        q.put('first')
-        d = q.get()
-        self.assertEqual('first', d)
-        self.assertRaises(Empty, q.get, block=False)
-
-        # assert with timeout
-        self.assertRaises(Empty, q.get, block=True, timeout=1.0)
-        # assert with negative timeout
-        self.assertRaises(ValueError, q.get, block=True, timeout=-1.0)
-
-    def test_empty(self):
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        self.assertEqual(q.empty(), True)
-
-        q.put('first')
-        self.assertEqual(q.empty(), False)
-
-        q.get()
-        self.assertEqual(q.empty(), True)
-
-    def test_open_close_single(self):
-        """Write 1 item, close, reopen checking if same item is there"""
-
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        q.put(b'var1')
-        del q
-        q = self.queue_class(self.path)
-        self.assertEqual(1, q.qsize())
-        self.assertEqual(b'var1', q.get())
-
-    def test_open_close_1000(self):
-        """Write 1000 items, close, reopen checking if all items are there"""
-
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        for i in range(1000):
-            q.put('var%d' % i)
-
-        self.assertEqual(1000, q.qsize())
-        del q
-        q = self.queue_class(self.path)
-        self.assertEqual(1000, q.qsize())
-        for i in range(1000):
-            data = q.get()
-            self.assertEqual('var%d' % i, data)
-        # assert adding another one still works
-        q.put('foobar')
-        data = q.get()
-        q.shrink_disk_usage()
-        self.assertEqual('foobar', data)
-
-    def test_random_read_write(self):
-        """Test random read/write"""
-
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        n = 0
-        for _ in range(1000):
-            if random.random() < 0.5:
-                if n > 0:
-                    q.get()
-                    n -= 1
-                else:
-                    self.assertRaises(Empty, q.get, block=False)
-            else:
-                # UniqueQueue will block at get() if this is not unique
-                # uuid.uuid4() should be unique
-                q.put('var%s' % uuid.uuid4())
-                n += 1
-
-    def test_multi_threaded_parallel(self):
-        """Create consumer and producer threads, check parallelism"""
-
-        # self.skipTest("Not supported multi-thread.")
-
-        m_queue = self.queue_class(
-            path=self.path, multithreading=True, auto_commit=self.auto_commit
-        )
-
-        def producer():
-            for i in range(1000):
-                m_queue.put('var%d' % i)
-
-        def consumer():
-            for i in range(1000):
-                x = m_queue.get(block=True)
-                self.assertEqual('var%d' % i, x)
-
-        c = Thread(target=consumer)
-        c.start()
-        p = Thread(target=producer)
-        p.start()
-        p.join()
-        c.join()
-        self.assertEqual(0, m_queue.size)
-        self.assertEqual(0, len(m_queue))
-        self.assertRaises(Empty, m_queue.get, block=False)
-
-    def test_multi_threaded_multi_producer(self):
-        """Test sqlqueue can be used by multiple producers."""
-        queue = self.queue_class(
-            path=self.path, multithreading=True, auto_commit=self.auto_commit
-        )
-
-        def producer(seq):
-            for i in range(10):
-                queue.put('var%d' % (i + (seq * 10)))
-
-        def consumer():
-            for _ in range(100):
-                data = queue.get(block=True)
-                self.assertTrue('var' in data)
-
-        c = Thread(target=consumer)
-        c.start()
-        producers = []
-        for seq in range(10):
-            t = Thread(target=producer, args=(seq,))
-            t.start()
-            producers.append(t)
-
-        for t in producers:
-            t.join()
-
-        c.join()
-
-    def test_multiple_consumers(self):
-        """Test sqlqueue can be used by multiple consumers."""
-
-        queue = self.queue_class(
-            path=self.path, multithreading=True, auto_commit=self.auto_commit
-        )
-
-        def producer():
-            for x in range(1000):
-                queue.put('var%d' % x)
-
-        counter = []
-        # Set all to 0
-        for _ in range(1000):
-            counter.append(0)
-
-        def consumer(index):
-            for i in range(200):
-                data = queue.get(block=True)
-                self.assertTrue('var' in data)
-                counter[index * 200 + i] = data
-
-        p = Thread(target=producer)
-        p.start()
-        consumers = []
-        for index in range(5):
-            t = Thread(target=consumer, args=(index,))
-            t.start()
-            consumers.append(t)
-
-        p.join()
-        for t in consumers:
-            t.join()
-
-        self.assertEqual(0, queue.qsize())
-        for x in range(1000):
-            self.assertNotEqual(
-                0, counter[x], "not 0 for counter's index %s" % x
-            )
-
-    def test_protocol_1(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-        q = self.queue_class(path=self.path)
-        self.assertEqual(
-            q._serializer.protocol, 2 if sys.version_info[0] == 2 else 4
-        )
-
-    def test_protocol_2(self):
-        q = self.queue_class(path=self.path)
-        self.assertEqual(
-            q._serializer.protocol, 2 if sys.version_info[0] == 2 else 4
-        )
-
-    def test_ack_and_clear(self):
-        q = self.queue_class(path=self.path)
-        ret_list = []
-        for _ in range(100):
-            q.put("val%s" % _)
-        for _ in range(100):
-            ret_list.append(q.get())
-        for ret in ret_list:
-            q.ack(ret)
-        self.assertEqual(q.acked_count(), 100)
-        q.clear_acked_data(keep_latest=10)
-        self.assertEqual(q.acked_count(), 10)
-        q.shrink_disk_usage()
-
-    def test_ack_unknown_item(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        val1 = q.get()
-        q.ack("val2")
-        q.nack("val3")
-        q.ack_failed("val4")
-        self.assertEqual(q.qsize(), 0)
-        self.assertEqual(q.unack_count(), 1)
-        q.ack(val1)
-        self.assertEqual(q.unack_count(), 0)
-
-    def test_resume_unack(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        val1 = q.get()
-        self.assertEqual(q.empty(), True)
-        self.assertEqual(q.qsize(), 0)
-        self.assertEqual(q.unack_count(), 1)
-        self.assertEqual(q.ready_count(), 0)
-        del q
-
-        q = self.queue_class(path=self.path, auto_resume=False)
-        self.assertEqual(q.empty(), True)
-        self.assertEqual(q.qsize(), 0)
-        self.assertEqual(q.unack_count(), 1)
-        self.assertEqual(q.ready_count(), 0)
-        q.resume_unack_tasks()
-        self.assertEqual(q.empty(), False)
-        self.assertEqual(q.qsize(), 1)
-        self.assertEqual(q.unack_count(), 0)
-        self.assertEqual(q.ready_count(), 1)
-        self.assertEqual(val1, q.get())
-        del q
-
-        q = self.queue_class(path=self.path, auto_resume=True)
-        self.assertEqual(q.empty(), False)
-        self.assertEqual(q.qsize(), 1)
-        self.assertEqual(q.unack_count(), 0)
-        self.assertEqual(q.ready_count(), 1)
-        self.assertEqual(val1, q.get())
-
-    def test_ack_unack_ack_failed(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        q.put("val2")
-        q.put("val3")
-        val1 = q.get()
-        val2 = q.get()
-        val3 = q.get()
-        # qsize should be zero when all item is getted from q
-        self.assertEqual(q.qsize(), 0)
-        self.assertEqual(q.unack_count(), 3)
-        # active size should be equal to qsize + unack_count
-        self.assertEqual(q.active_size(), 3)
-        # nack will let the item requeued as ready status
-        q.nack(val1)
-        self.assertEqual(q.qsize(), 1)
-        self.assertEqual(q.ready_count(), 1)
-        # ack failed is just mark item as ack failed
-        q.ack_failed(val3)
-        self.assertEqual(q.ack_failed_count(), 1)
-        # ack should not effect qsize
-        q.ack(val2)
-        self.assertEqual(q.acked_count(), 1)
-        self.assertEqual(q.qsize(), 1)
-        # all ack* related action will reduce unack count
-        self.assertEqual(q.unack_count(), 0)
-        # reget the nacked item
-        ready_val = q.get()
-        self.assertEqual(ready_val, val1)
-        q.ack(ready_val)
-        self.assertEqual(q.qsize(), 0)
-        self.assertEqual(q.acked_count(), 2)
-        self.assertEqual(q.ready_count(), 0)
-
-    def test_put_0(self):
-        q = self.queue_class(path=self.path)
-        q.put(0)
-        d = q.get(block=False)
-        self.assertIsNotNone(d)
-
-    def test_get_id(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        val2_id = q.put("val2")
-        q.put("val3")
-        item = q.get(id=val2_id)
-        # item id should be 2
-        self.assertEqual(val2_id, 2)
-        # item should get val2
-        self.assertEqual(item, 'val2')
-
-    def test_get_next_in_order(self):
-        q = self.queue_class(path=self.path)
-        val1_id = q.put("val1")
-        q.put("val2")
-        q.put("val3")
-        item = q.get(id=val1_id, next_in_order=True)
-        # item id should be 1
-        self.assertEqual(val1_id, 1)
-        # item should get val2
-        self.assertEqual(item, 'val2')
-        q.nack(item)
-        # queue should roll over to begining if next > end
-        item = q.get(id=3, next_in_order=True, raw=True)
-        q.nack(item)
-        self.assertEqual(item.get("pqid"), 1)
-
-    def test_get_raw(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        item = q.get(raw=True)
-        q.nack(item)
-        # item should get val2
-        self.assertEqual(True, "pqid" in item)
-        self.assertEqual(item.get("data"), 'val1')
-
-    def test_nack_raw(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        item = q.get(raw=True)
-        # nack a raw return
-        q.nack(item)
-        # size should be 1 after nack
-        self.assertEqual(q.qsize(), 1)
-
-    def test_ack_active_size(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        item = q.get(raw=True)
-        # active_size should be 1 as it hasn't been acked
-        self.assertEqual(q.active_size(), 1)
-        q.ack(item)
-        # active_size should be 0 after ack
-        self.assertEqual(q.active_size(), 0)
-
-    def test_queue(self):
-        q = self.queue_class(path=self.path)
-        q.put("val1")
-        q.put("val2")
-        q.put("val3")
-        # queue should get the three items
-        d = q.queue()
-        self.assertEqual(len(d), 3)
-        self.assertEqual(d[1].get("data"), "val2")
-
-    def test_update(self):
-        q = self.queue_class(path=self.path)
-        qid = q.put("val1")
-        q.update(id=qid, item="val2")
-        item = q.get(id=qid)
-        q.nack(item)
-        self.assertEqual(item, "val2")
-
-
-class SQLite3QueueInMemory(SQLite3AckQueueTest):
-    def setUp(self):
-        self.path = ":memory:"
-        self.auto_commit = True
-        self.queue_class = SQLiteAckQueue
-
-    def test_open_close_1000(self):
-        self.skipTest('Memory based sqlite is not persistent.')
-
-    def test_open_close_single(self):
-        self.skipTest('Memory based sqlite is not persistent.')
-
-    def test_multiple_consumers(self):
-        self.skipTest(
-            'Skipped due to occasional crash during multithreading mode.'
-        )
-
-    def test_multi_threaded_multi_producer(self):
-        self.skipTest(
-            'Skipped due to occasional crash during multithreading mode.'
-        )
-
-    def test_multi_threaded_parallel(self):
-        self.skipTest(
-            'Skipped due to occasional crash during multithreading mode.'
-        )
-
-    def test_task_done_with_restart(self):
-        self.skipTest('Skipped due to not persistent.')
-
-    def test_protocol_2(self):
-        self.skipTest('In memory queue is always new.')
-
-    def test_resume_unack(self):
-        self.skipTest('Memory based sqlite is not persistent.')
-
-
-class FILOSQLite3AckQueueTest(SQLite3AckQueueTest):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='filo_sqlackqueue')
-        self.auto_commit = True
-        self.queue_class = FILOSQLiteAckQueue
-
-    def tearDown(self):
-        shutil.rmtree(self.path, ignore_errors=True)
-
-    def test_open_close_1000(self):
-        """Write 1000 items, close, reopen checking if all items are there"""
-
-        q = self.queue_class(self.path, auto_commit=self.auto_commit)
-        for i in range(1000):
-            q.put('var%d' % i)
-        self.assertEqual(1000, q.qsize())
-        del q
-        q = self.queue_class(self.path)
-        self.assertEqual(1000, q.qsize())
-        for i in range(1000):
-            data = q.get()
-            self.assertEqual('var%d' % (999 - i), data)
-        # assert adding another one still works
-        q.put('foobar')
-        data = q.get()
-        q.nack(data)
-        self.assertEqual('foobar', data)
-
-    def test_multi_threaded_parallel(self):
-        """Create consumer and producer threads, check parallelism"""
-
-        # self.skipTest("Not supported multi-thread.")
-
-        m_queue = self.queue_class(
-            path=self.path, multithreading=True, auto_commit=self.auto_commit
-        )
-
-        def producer():
-            for i in range(1000):
-                m_queue.put('var%d' % i)
-
-        def consumer():
-            # We cannot quarantee what next number will be like in FIFO
-            for _ in range(1000):
-                x = m_queue.get(block=True)
-                self.assertTrue('var' in x)
-
-        c = Thread(target=consumer)
-        c.start()
-        p = Thread(target=producer)
-        p.start()
-        p.join()
-        c.join()
-        self.assertEqual(0, m_queue.size)
-        self.assertEqual(0, len(m_queue))
-        self.assertRaises(Empty, m_queue.get, block=False)
-
-    def test_get_next_in_order(self):
-        q = self.queue_class(path=self.path)
-        val1_id = q.put("val1")
-        q.put("val2")
-        q.put("val3")
-        item = q.get(id=val1_id, next_in_order=True)
-        q.nack(item)
-        # item id should be 1
-        self.assertEqual(val1_id, 1)
-        # item should get val2
-        self.assertEqual(item, 'val3')
-        # queue should roll over to end if next < begining
-        item = q.get(id=1, next_in_order=True, raw=True)
-        q.nack(item)
-        self.assertEqual(item.get("pqid"), 3)
-
-
-# Note
-# We have to be carefull to avoid test cases from SQLite3AckQueueTest having
-# duplicate values in their q.put()'s. This could block the test indefinitely
-class SQLite3UniqueAckQueueTest(SQLite3AckQueueTest):
-    def setUp(self):
-        self.path = tempfile.mkdtemp(suffix='sqlackqueue')
-        self.auto_commit = True
-        self.queue_class = UniqueAckQ
-
-    def test_add_duplicate_item(self):
-        q = self.queue_class(self.path)
-        q.put(1111)
-        self.assertEqual(1, q.size)
-        # put duplicate item
-        q.put(1111)
-        self.assertEqual(1, q.size)
-
-        q.put(2222)
-        self.assertEqual(2, q.size)
-
-        del q
-        q = self.queue_class(self.path)
-        self.assertEqual(2, q.size)
+# coding=utf-8
+
+import random
+import shutil
+import sys
+import tempfile
+import unittest
+from threading import Thread
+import uuid
+
+from persistqueue.sqlackqueue import (
+    SQLiteAckQueue,
+    FILOSQLiteAckQueue,
+    UniqueAckQ,
+)
+from persistqueue import Empty
+
+
+class SQLite3AckQueueTest(unittest.TestCase):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='sqlackqueue')
+        self.auto_commit = True
+        self.queue_class = SQLiteAckQueue
+
+    def tearDown(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+
+    def test_raise_empty(self):
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+
+        q.put('first')
+        d = q.get()
+        self.assertEqual('first', d)
+        self.assertRaises(Empty, q.get, block=False)
+
+        # assert with timeout
+        self.assertRaises(Empty, q.get, block=True, timeout=1.0)
+        # assert with negative timeout
+        self.assertRaises(ValueError, q.get, block=True, timeout=-1.0)
+
+    def test_empty(self):
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        self.assertEqual(q.empty(), True)
+
+        q.put('first')
+        self.assertEqual(q.empty(), False)
+
+        q.get()
+        self.assertEqual(q.empty(), True)
+
+    def test_full(self):
+        # SQL queue `full()` always returns `False` !!
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        self.assertEqual(q.full(), False)
+
+        q.put('first')
+        self.assertEqual(q.full(), False)
+
+        q.get()
+        self.assertEqual(q.full(), False)
+
+    def test_open_close_single(self):
+        """Write 1 item, close, reopen checking if same item is there"""
+
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        q.put(b'var1')
+        del q
+        q = self.queue_class(self.path)
+        self.assertEqual(1, q.qsize())
+        self.assertEqual(b'var1', q.get())
+
+    def test_open_close_1000(self):
+        """Write 1000 items, close, reopen checking if all items are there"""
+
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        for i in range(1000):
+            q.put('var%d' % i)
+
+        self.assertEqual(1000, q.qsize())
+        del q
+        q = self.queue_class(self.path)
+        self.assertEqual(1000, q.qsize())
+        for i in range(1000):
+            data = q.get()
+            self.assertEqual('var%d' % i, data)
+        # assert adding another one still works
+        q.put('foobar')
+        data = q.get()
+        q.shrink_disk_usage()
+        self.assertEqual('foobar', data)
+
+    def test_random_read_write(self):
+        """Test random read/write"""
+
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        n = 0
+        for _ in range(1000):
+            if random.random() < 0.5:
+                if n > 0:
+                    q.get()
+                    n -= 1
+                else:
+                    self.assertRaises(Empty, q.get, block=False)
+            else:
+                # UniqueQueue will block at get() if this is not unique
+                # uuid.uuid4() should be unique
+                q.put('var%s' % uuid.uuid4())
+                n += 1
+
+    def test_multi_threaded_parallel(self):
+        """Create consumer and producer threads, check parallelism"""
+
+        # self.skipTest("Not supported multi-thread.")
+
+        m_queue = self.queue_class(
+            path=self.path, multithreading=True, auto_commit=self.auto_commit
+        )
+
+        def producer():
+            for i in range(1000):
+                m_queue.put('var%d' % i)
+
+        def consumer():
+            for i in range(1000):
+                x = m_queue.get(block=True)
+                self.assertEqual('var%d' % i, x)
+
+        c = Thread(target=consumer)
+        c.start()
+        p = Thread(target=producer)
+        p.start()
+        p.join()
+        c.join()
+        self.assertEqual(0, m_queue.size)
+        self.assertEqual(0, len(m_queue))
+        self.assertRaises(Empty, m_queue.get, block=False)
+
+    def test_multi_threaded_multi_producer(self):
+        """Test sqlqueue can be used by multiple producers."""
+        queue = self.queue_class(
+            path=self.path, multithreading=True, auto_commit=self.auto_commit
+        )
+
+        def producer(seq):
+            for i in range(10):
+                queue.put('var%d' % (i + (seq * 10)))
+
+        def consumer():
+            for _ in range(100):
+                data = queue.get(block=True)
+                self.assertTrue('var' in data)
+
+        c = Thread(target=consumer)
+        c.start()
+        producers = []
+        for seq in range(10):
+            t = Thread(target=producer, args=(seq,))
+            t.start()
+            producers.append(t)
+
+        for t in producers:
+            t.join()
+
+        c.join()
+
+    def test_multiple_consumers(self):
+        """Test sqlqueue can be used by multiple consumers."""
+
+        queue = self.queue_class(
+            path=self.path, multithreading=True, auto_commit=self.auto_commit
+        )
+
+        def producer():
+            for x in range(1000):
+                queue.put('var%d' % x)
+
+        counter = []
+        # Set all to 0
+        for _ in range(1000):
+            counter.append(0)
+
+        def consumer(index):
+            for i in range(200):
+                data = queue.get(block=True)
+                self.assertTrue('var' in data)
+                counter[index * 200 + i] = data
+
+        p = Thread(target=producer)
+        p.start()
+        consumers = []
+        for index in range(5):
+            t = Thread(target=consumer, args=(index,))
+            t.start()
+            consumers.append(t)
+
+        p.join()
+        for t in consumers:
+            t.join()
+
+        self.assertEqual(0, queue.qsize())
+        for x in range(1000):
+            self.assertNotEqual(
+                0, counter[x], "not 0 for counter's index %s" % x
+            )
+
+    def test_protocol_1(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+        q = self.queue_class(path=self.path)
+        self.assertEqual(
+            q._serializer.protocol, 2 if sys.version_info[0] == 2 else 4
+        )
+
+    def test_protocol_2(self):
+        q = self.queue_class(path=self.path)
+        self.assertEqual(
+            q._serializer.protocol, 2 if sys.version_info[0] == 2 else 4
+        )
+
+    def test_ack_and_clear(self):
+        q = self.queue_class(path=self.path)
+        ret_list = []
+        for _ in range(100):
+            q.put("val%s" % _)
+        for _ in range(100):
+            ret_list.append(q.get())
+        for ret in ret_list:
+            q.ack(ret)
+        self.assertEqual(q.acked_count(), 100)
+        q.clear_acked_data(keep_latest=10)
+        self.assertEqual(q.acked_count(), 10)
+        q.shrink_disk_usage()
+
+    def test_ack_unknown_item(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        val1 = q.get()
+        q.ack("val2")
+        q.nack("val3")
+        q.ack_failed("val4")
+        self.assertEqual(q.qsize(), 0)
+        self.assertEqual(q.unack_count(), 1)
+        q.ack(val1)
+        self.assertEqual(q.unack_count(), 0)
+
+    def test_resume_unack(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        val1 = q.get()
+        self.assertEqual(q.empty(), True)
+        self.assertEqual(q.qsize(), 0)
+        self.assertEqual(q.unack_count(), 1)
+        self.assertEqual(q.ready_count(), 0)
+        del q
+
+        q = self.queue_class(path=self.path, auto_resume=False)
+        self.assertEqual(q.empty(), True)
+        self.assertEqual(q.qsize(), 0)
+        self.assertEqual(q.unack_count(), 1)
+        self.assertEqual(q.ready_count(), 0)
+        q.resume_unack_tasks()
+        self.assertEqual(q.empty(), False)
+        self.assertEqual(q.qsize(), 1)
+        self.assertEqual(q.unack_count(), 0)
+        self.assertEqual(q.ready_count(), 1)
+        self.assertEqual(val1, q.get())
+        del q
+
+        q = self.queue_class(path=self.path, auto_resume=True)
+        self.assertEqual(q.empty(), False)
+        self.assertEqual(q.qsize(), 1)
+        self.assertEqual(q.unack_count(), 0)
+        self.assertEqual(q.ready_count(), 1)
+        self.assertEqual(val1, q.get())
+
+    def test_ack_unack_ack_failed(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        q.put("val2")
+        q.put("val3")
+        val1 = q.get()
+        val2 = q.get()
+        val3 = q.get()
+        # qsize should be zero when all item is getted from q
+        self.assertEqual(q.qsize(), 0)
+        self.assertEqual(q.unack_count(), 3)
+        # active size should be equal to qsize + unack_count
+        self.assertEqual(q.active_size(), 3)
+        # nack will let the item requeued as ready status
+        q.nack(val1)
+        self.assertEqual(q.qsize(), 1)
+        self.assertEqual(q.ready_count(), 1)
+        # ack failed is just mark item as ack failed
+        q.ack_failed(val3)
+        self.assertEqual(q.ack_failed_count(), 1)
+        # ack should not effect qsize
+        q.ack(val2)
+        self.assertEqual(q.acked_count(), 1)
+        self.assertEqual(q.qsize(), 1)
+        # all ack* related action will reduce unack count
+        self.assertEqual(q.unack_count(), 0)
+        # reget the nacked item
+        ready_val = q.get()
+        self.assertEqual(ready_val, val1)
+        q.ack(ready_val)
+        self.assertEqual(q.qsize(), 0)
+        self.assertEqual(q.acked_count(), 2)
+        self.assertEqual(q.ready_count(), 0)
+
+    def test_put_0(self):
+        q = self.queue_class(path=self.path)
+        q.put(0)
+        d = q.get(block=False)
+        self.assertIsNotNone(d)
+
+    def test_get_id(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        val2_id = q.put("val2")
+        q.put("val3")
+        item = q.get(id=val2_id)
+        # item id should be 2
+        self.assertEqual(val2_id, 2)
+        # item should get val2
+        self.assertEqual(item, 'val2')
+
+    def test_get_next_in_order(self):
+        q = self.queue_class(path=self.path)
+        val1_id = q.put("val1")
+        q.put("val2")
+        q.put("val3")
+        item = q.get(id=val1_id, next_in_order=True)
+        # item id should be 1
+        self.assertEqual(val1_id, 1)
+        # item should get val2
+        self.assertEqual(item, 'val2')
+        q.nack(item)
+        # queue should roll over to begining if next > end
+        item = q.get(id=3, next_in_order=True, raw=True)
+        q.nack(item)
+        self.assertEqual(item.get("pqid"), 1)
+
+    def test_get_raw(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        item = q.get(raw=True)
+        q.nack(item)
+        # item should get val2
+        self.assertEqual(True, "pqid" in item)
+        self.assertEqual(item.get("data"), 'val1')
+
+    def test_nack_raw(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        item = q.get(raw=True)
+        # nack a raw return
+        q.nack(item)
+        # size should be 1 after nack
+        self.assertEqual(q.qsize(), 1)
+
+    def test_ack_active_size(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        item = q.get(raw=True)
+        # active_size should be 1 as it hasn't been acked
+        self.assertEqual(q.active_size(), 1)
+        q.ack(item)
+        # active_size should be 0 after ack
+        self.assertEqual(q.active_size(), 0)
+
+    def test_queue(self):
+        q = self.queue_class(path=self.path)
+        q.put("val1")
+        q.put("val2")
+        q.put("val3")
+        # queue should get the three items
+        d = q.queue()
+        self.assertEqual(len(d), 3)
+        self.assertEqual(d[1].get("data"), "val2")
+
+    def test_update(self):
+        q = self.queue_class(path=self.path)
+        qid = q.put("val1")
+        q.update(id=qid, item="val2")
+        item = q.get(id=qid)
+        q.nack(item)
+        self.assertEqual(item, "val2")
+
+
+class SQLite3QueueInMemory(SQLite3AckQueueTest):
+    def setUp(self):
+        self.path = ":memory:"
+        self.auto_commit = True
+        self.queue_class = SQLiteAckQueue
+
+    def test_open_close_1000(self):
+        self.skipTest('Memory based sqlite is not persistent.')
+
+    def test_open_close_single(self):
+        self.skipTest('Memory based sqlite is not persistent.')
+
+    def test_multiple_consumers(self):
+        self.skipTest(
+            'Skipped due to occasional crash during multithreading mode.'
+        )
+
+    def test_multi_threaded_multi_producer(self):
+        self.skipTest(
+            'Skipped due to occasional crash during multithreading mode.'
+        )
+
+    def test_multi_threaded_parallel(self):
+        self.skipTest(
+            'Skipped due to occasional crash during multithreading mode.'
+        )
+
+    def test_task_done_with_restart(self):
+        self.skipTest('Skipped due to not persistent.')
+
+    def test_protocol_2(self):
+        self.skipTest('In memory queue is always new.')
+
+    def test_resume_unack(self):
+        self.skipTest('Memory based sqlite is not persistent.')
+
+
+class FILOSQLite3AckQueueTest(SQLite3AckQueueTest):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='filo_sqlackqueue')
+        self.auto_commit = True
+        self.queue_class = FILOSQLiteAckQueue
+
+    def tearDown(self):
+        shutil.rmtree(self.path, ignore_errors=True)
+
+    def test_open_close_1000(self):
+        """Write 1000 items, close, reopen checking if all items are there"""
+
+        q = self.queue_class(self.path, auto_commit=self.auto_commit)
+        for i in range(1000):
+            q.put('var%d' % i)
+        self.assertEqual(1000, q.qsize())
+        del q
+        q = self.queue_class(self.path)
+        self.assertEqual(1000, q.qsize())
+        for i in range(1000):
+            data = q.get()
+            self.assertEqual('var%d' % (999 - i), data)
+        # assert adding another one still works
+        q.put('foobar')
+        data = q.get()
+        q.nack(data)
+        self.assertEqual('foobar', data)
+
+    def test_multi_threaded_parallel(self):
+        """Create consumer and producer threads, check parallelism"""
+
+        # self.skipTest("Not supported multi-thread.")
+
+        m_queue = self.queue_class(
+            path=self.path, multithreading=True, auto_commit=self.auto_commit
+        )
+
+        def producer():
+            for i in range(1000):
+                m_queue.put('var%d' % i)
+
+        def consumer():
+            # We cannot quarantee what next number will be like in FIFO
+            for _ in range(1000):
+                x = m_queue.get(block=True)
+                self.assertTrue('var' in x)
+
+        c = Thread(target=consumer)
+        c.start()
+        p = Thread(target=producer)
+        p.start()
+        p.join()
+        c.join()
+        self.assertEqual(0, m_queue.size)
+        self.assertEqual(0, len(m_queue))
+        self.assertRaises(Empty, m_queue.get, block=False)
+
+    def test_get_next_in_order(self):
+        q = self.queue_class(path=self.path)
+        val1_id = q.put("val1")
+        q.put("val2")
+        q.put("val3")
+        item = q.get(id=val1_id, next_in_order=True)
+        q.nack(item)
+        # item id should be 1
+        self.assertEqual(val1_id, 1)
+        # item should get val2
+        self.assertEqual(item, 'val3')
+        # queue should roll over to end if next < begining
+        item = q.get(id=1, next_in_order=True, raw=True)
+        q.nack(item)
+        self.assertEqual(item.get("pqid"), 3)
+
+
+# Note
+# We have to be carefull to avoid test cases from SQLite3AckQueueTest having
+# duplicate values in their q.put()'s. This could block the test indefinitely
+class SQLite3UniqueAckQueueTest(SQLite3AckQueueTest):
+    def setUp(self):
+        self.path = tempfile.mkdtemp(suffix='sqlackqueue')
+        self.auto_commit = True
+        self.queue_class = UniqueAckQ
+
+    def test_add_duplicate_item(self):
+        q = self.queue_class(self.path)
+        q.put(1111)
+        self.assertEqual(1, q.size)
+        # put duplicate item
+        q.put(1111)
+        self.assertEqual(1, q.size)
+
+        q.put(2222)
+        self.assertEqual(2, q.size)
+
+        del q
+        q = self.queue_class(self.path)
+        self.assertEqual(2, q.size)
```

### Comparing `persist-queue-0.8.0b0/persistqueue/sqlbase.py` & `persist-queue-0.8.1/persistqueue/sqlbase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,451 +1,454 @@
-# coding=utf-8
-import logging
-import os
-import time as _time
-import sqlite3
-import threading
-
-from persistqueue.exceptions import Empty
-
-import persistqueue.serializers.pickle
-
-sqlite3.enable_callback_tracebacks(True)
-
-log = logging.getLogger(__name__)
-
-# 10 seconds internal for `wait` of event
-TICK_FOR_WAIT = 10
-
-
-def with_conditional_transaction(func):
-    def _execute(obj, *args, **kwargs):
-        # for MySQL, connection pool should be used since db connection is
-        # basically not thread-safe
-        _putter = obj._putter
-        if str(type(obj)).find("MySQLQueue") > 0:
-            # use fresh connection from pool not the shared one
-            _putter = obj.get_pooled_conn()
-        with obj.tran_lock:
-            with _putter as tran:
-                # For sqlite3, commit() is called automatically afterwards
-                # but for other db API, this is not TRUE!
-                stat, param = func(obj, *args, **kwargs)
-                s = str(type(tran))
-                if s.find("Cursor") > 0:
-                    cur = tran
-                    cur.execute(stat, param)
-                else:
-                    cur = tran.cursor()
-                    cur.execute(stat, param)
-                    cur.close()
-                    tran.commit()
-                return cur.lastrowid
-
-    return _execute
-
-
-def commit_ignore_error(conn):
-    """Ignore the error of no transaction is active.
-
-    The transaction may be already committed by user's task_done call.
-    It's safe to ignore all errors of this kind.
-    """
-    try:
-        conn.commit()
-    except sqlite3.OperationalError as ex:
-        if 'no transaction is active' in str(ex):
-            log.debug(
-                'Not able to commit the transaction, '
-                'may already be committed.'
-            )
-        else:
-            raise
-
-
-class SQLBase(object):
-    """SQL base class."""
-
-    _TABLE_NAME = 'base'  # DB table name
-    _KEY_COLUMN = ''  # the name of the key column, used in DB CRUD
-    _SQL_CREATE = ''  # SQL to create a table
-    _SQL_UPDATE = ''  # SQL to update a record
-    _SQL_INSERT = ''  # SQL to insert a record
-    _SQL_SELECT = ''  # SQL to select a record
-    _SQL_SELECT_ID = ''  # SQL to select a record with criteria
-    _SQL_SELECT_WHERE = ''  # SQL to select a record with criteria
-    _SQL_DELETE = ''  # SQL to delete a record
-    # _MEMORY = ':memory:'  # flag indicating store DB in memory
-
-    def __init__(self):
-        """Initiate a queue in db.
-        """
-        self._serializer = None
-        self.auto_commit = None
-
-        # SQL transaction lock
-        self.tran_lock = threading.Lock()
-        self.put_event = threading.Event()
-        # Action lock to assure multiple action to be *atomic*
-        self.action_lock = threading.Lock()
-        self.total = 0
-        self.cursor = 0
-        self._getter = None
-        self._putter = None
-
-    @with_conditional_transaction
-    def _insert_into(self, *record):
-        return self._sql_insert, record
-
-    @with_conditional_transaction
-    def _update(self, key, *args):
-        args = list(args) + [key]
-        return self._sql_update, args
-
-    @with_conditional_transaction
-    def _delete(self, key, op='='):
-
-        sql = self._SQL_DELETE.format(
-            table_name=self._table_name, key_column=self._key_column, op=op)
-        return sql, (key,)
-
-    def _pop(self, rowid=None, raw=False):
-        with self.action_lock:
-            if self.auto_commit:
-                row = self._select(rowid=rowid)
-                # Perhaps a sqlite3 bug, sometimes (None, None) is returned
-                # by select, below can avoid these invalid records.
-                if row and row[0] is not None:
-                    self._delete(row[0])
-                    self.total -= 1
-                    item = self._serializer.loads(row[1])
-                    if raw:
-                        return {
-                            'pqid': row[0],
-                            'data': item,
-                            'timestamp': row[2],
-                        }
-                    else:
-                        return item
-            else:
-                row = self._select(
-                    self.cursor, op=">", column=self._KEY_COLUMN, rowid=rowid
-                )
-                if row and row[0] is not None:
-                    self.cursor = row[0]
-                    self.total -= 1
-                    item = self._serializer.loads(row[1])
-                    if raw:
-                        return {
-                            'pqid': row[0],
-                            'data': item,
-                            'timestamp': row[2],
-                        }
-                    else:
-                        return item
-            return None
-
-    def update(self, item, id=None):
-        if isinstance(item, dict) and "pqid" in item:
-            _id = item.get("pqid")
-            item = item.get("data")
-        if id is not None:
-            _id = id
-        if _id is None:
-            raise ValueError("Provide an id or raw item")
-        obj = self._serializer.dumps(item)
-        self._update(_id, obj)
-        return _id
-
-    def get(self, block=True, timeout=None, id=None, raw=False):
-        if isinstance(id, dict) and "pqid" in id:
-            rowid = id.get("pqid")
-        elif isinstance(id, int):
-            rowid = id
-        else:
-            rowid = None
-        if not block:
-            serialized = self._pop(raw=raw, rowid=rowid)
-            if serialized is None:
-                raise Empty
-        elif timeout is None:
-            # block until a put event.
-            serialized = self._pop(raw=raw, rowid=rowid)
-            while serialized is None:
-                self.put_event.clear()
-                self.put_event.wait(TICK_FOR_WAIT)
-                serialized = self._pop(raw=raw, rowid=rowid)
-        elif timeout < 0:
-            raise ValueError("'timeout' must be a non-negative number")
-        else:
-            # block until the timeout reached
-            endtime = _time.time() + timeout
-            serialized = self._pop(raw=raw, rowid=rowid)
-            while serialized is None:
-                self.put_event.clear()
-                remaining = endtime - _time.time()
-                if remaining <= 0.0:
-                    raise Empty
-                self.put_event.wait(
-                    TICK_FOR_WAIT if TICK_FOR_WAIT < remaining else remaining
-                )
-                serialized = self._pop(raw=raw, rowid=rowid)
-        return serialized
-
-    def get_nowait(self, id=None, raw=False):
-        return self.get(block=False, id=id, raw=raw)
-
-    def task_done(self):
-        """Persist the current state if auto_commit=False."""
-        if not self.auto_commit:
-            self._delete(self.cursor, op='<=')
-            self._task_done()
-
-    def queue(self):
-        rows = self._sql_queue().fetchall()
-        datarows = []
-        for row in rows:
-            item = {
-                'id': row[0],
-                'data': self._serializer.loads(row[1]),
-                'timestamp': row[2],
-            }
-            datarows.append(item)
-        return datarows
-
-    @with_conditional_transaction
-    def shrink_disk_usage(self):
-        sql = """VACUUM"""
-        return sql, ()
-
-    @property
-    def size(self):
-        return self.total
-
-    def qsize(self):
-        return max(0, self.size)
-
-    def empty(self):
-        return self.size == 0
-
-    def __len__(self):
-        return self.size
-
-    def _select(self, *args, **kwargs):
-        start_key = self._start_key()
-        op = kwargs.get('op', None)
-        column = kwargs.get('column', None)
-        next_in_order = kwargs.get('next_in_order', False)
-        rowid = kwargs.get('rowid') if kwargs.get('rowid', None) else start_key
-        if not next_in_order and rowid != start_key:
-            # Get the record by the id
-            result = self._getter.execute(
-                self._sql_select_id(rowid), args
-            ).fetchone()
-        elif op and column:
-            # Get the next record with criteria
-            rowid = rowid if next_in_order else start_key
-            result = self._getter.execute(
-                self._sql_select_where(rowid, op, column), args
-            ).fetchone()
-        else:
-            # Get the next record
-            rowid = rowid if next_in_order else start_key
-            result = self._getter.execute(
-                self._sql_select(rowid), args
-            ).fetchone()
-        if (
-                next_in_order
-                and rowid != start_key
-                and (not result or len(result) == 0)
-        ):
-            # sqlackqueue: if we're at the end, start over
-            kwargs['rowid'] = start_key
-            result = self._select(*args, **kwargs)
-        return result
-
-    def _count(self):
-        sql = 'SELECT COUNT({}) FROM {}'.format(
-            self._key_column, self._table_name
-        )
-        row = self._getter.execute(sql).fetchone()
-        return row[0] if row else 0
-
-    def _start_key(self):
-        if self._TABLE_NAME == 'ack_filo_queue':
-            return 9223372036854775807  # maxsize
-        else:
-            return 0
-
-    def _task_done(self):
-        """Only required if auto-commit is set as False."""
-        commit_ignore_error(self._putter)
-
-    def _sql_queue(self):
-        sql = 'SELECT * FROM {}'.format(self._table_name)
-        return self._getter.execute(sql)
-
-    @property
-    def _table_name(self):
-        return '`{}_{}`'.format(self._TABLE_NAME, self.name)
-
-    @property
-    def _key_column(self):
-        return self._KEY_COLUMN
-
-    @property
-    def _sql_create(self):
-        return self._SQL_CREATE.format(
-            table_name=self._table_name, key_column=self._key_column
-        )
-
-    @property
-    def _sql_insert(self):
-        return self._SQL_INSERT.format(
-            table_name=self._table_name, key_column=self._key_column
-        )
-
-    @property
-    def _sql_update(self):
-        return self._SQL_UPDATE.format(
-            table_name=self._table_name, key_column=self._key_column
-        )
-
-    def _sql_select_id(self, rowid):
-        return self._SQL_SELECT_ID.format(
-            table_name=self._table_name,
-            key_column=self._key_column,
-            rowid=rowid,
-        )
-
-    def _sql_select(self, rowid):
-        return self._SQL_SELECT.format(
-            table_name=self._table_name,
-            key_column=self._key_column,
-            rowid=rowid,
-        )
-
-    def _sql_select_where(self, rowid, op, column):
-        return self._SQL_SELECT_WHERE.format(
-            table_name=self._table_name,
-            key_column=self._key_column,
-            rowid=rowid,
-            op=op,
-            column=column,
-        )
-
-    def __del__(self):
-        """Handles sqlite connection when queue was deleted"""
-        if self._getter:
-            self._getter.close()
-        if self._putter:
-            self._putter.close()
-
-
-class SQLiteBase(SQLBase):
-    """SQLite3 base class."""
-
-    _TABLE_NAME = 'base'  # DB table name
-    _KEY_COLUMN = ''  # the name of the key column, used in DB CRUD
-    _SQL_CREATE = ''  # SQL to create a table
-    _SQL_UPDATE = ''  # SQL to update a record
-    _SQL_INSERT = ''  # SQL to insert a record
-    _SQL_SELECT = ''  # SQL to select a record
-    _SQL_SELECT_ID = ''  # SQL to select a record with criteria
-    _SQL_SELECT_WHERE = ''  # SQL to select a record with criteria
-    _SQL_DELETE = ''  # SQL to delete a record
-    _MEMORY = ':memory:'  # flag indicating store DB in memory
-
-    def __init__(
-            self,
-            path,
-            name='default',
-            multithreading=False,
-            timeout=10.0,
-            auto_commit=True,
-            serializer=persistqueue.serializers.pickle,
-            db_file_name=None,
-    ):
-        """Initiate a queue in sqlite3 or memory.
-
-        :param path: path for storing DB file.
-        :param name: the suffix for the table name,
-                     table name would be ${_TABLE_NAME}_${name}
-        :param multithreading: if set to True, two db connections will be,
-                               one for **put** and one for **get**.
-        :param timeout: timeout in second waiting for the database lock.
-        :param auto_commit: Set to True, if commit is required on every
-                            INSERT/UPDATE action, otherwise False, whereas
-                            a **task_done** is required to persist changes
-                            after **put**.
-        :param serializer: The serializer parameter controls how enqueued data
-                           is serialized. It must have methods dump(value, fp)
-                           and load(fp). The dump method must serialize the
-                           value and write it to fp, and may be called for
-                           multiple values with the same fp. The load method
-                           must deserialize and return one value from fp,
-                           and may be called multiple times with the same fp
-                           to read multiple values.
-        :param db_file_name: set the db file name of the queue data, otherwise
-                             default to `data.db`
-        """
-        super(SQLiteBase, self).__init__()
-        self.memory_sql = False
-        self.path = path
-        self.name = name
-        self.timeout = timeout
-        self.multithreading = multithreading
-        self.auto_commit = auto_commit
-        self._serializer = serializer
-        self.db_file_name = "data.db"
-        if db_file_name:
-            self.db_file_name = db_file_name
-        self._init()
-
-    def _init(self):
-        """Initialize the tables in DB."""
-        if self.path == self._MEMORY:
-            self.memory_sql = True
-            log.debug("Initializing Sqlite3 Queue in memory.")
-        elif not os.path.exists(self.path):
-            os.makedirs(self.path)
-            log.debug(
-                'Initializing Sqlite3 Queue with path {}'.format(self.path)
-            )
-        self._conn = self._new_db_connection(
-            self.path, self.multithreading, self.timeout
-        )
-        self._getter = self._conn
-        self._putter = self._conn
-
-        self._conn.execute(self._sql_create)
-        self._conn.commit()
-        # Setup another session only for disk-based queue.
-        if self.multithreading:
-            if not self.memory_sql:
-                self._putter = self._new_db_connection(
-                    self.path, self.multithreading, self.timeout
-                )
-        self._conn.text_factory = str
-        self._putter.text_factory = str
-
-        # SQLite3 transaction lock
-        self.tran_lock = threading.Lock()
-        self.put_event = threading.Event()
-
-    def _new_db_connection(self, path, multithreading, timeout):
-        conn = None
-        if path == self._MEMORY:
-            conn = sqlite3.connect(path, check_same_thread=not multithreading)
-        else:
-            conn = sqlite3.connect(
-                '{}/{}'.format(path, self.db_file_name),
-                timeout=timeout,
-                check_same_thread=not multithreading,
-            )
-        conn.execute('PRAGMA journal_mode=WAL;')
-        return conn
-
-    def __del__(self):
-        """Handles sqlite connection when queue was deleted"""
-        self._getter.close()
-        self._putter.close()
+# coding=utf-8
+import logging
+import os
+import time as _time
+import sqlite3
+import threading
+
+from persistqueue.exceptions import Empty
+
+import persistqueue.serializers.pickle
+
+sqlite3.enable_callback_tracebacks(True)
+
+log = logging.getLogger(__name__)
+
+# 10 seconds internal for `wait` of event
+TICK_FOR_WAIT = 10
+
+
+def with_conditional_transaction(func):
+    def _execute(obj, *args, **kwargs):
+        # for MySQL, connection pool should be used since db connection is
+        # basically not thread-safe
+        _putter = obj._putter
+        if str(type(obj)).find("MySQLQueue") > 0:
+            # use fresh connection from pool not the shared one
+            _putter = obj.get_pooled_conn()
+        with obj.tran_lock:
+            with _putter as tran:
+                # For sqlite3, commit() is called automatically afterwards
+                # but for other db API, this is not TRUE!
+                stat, param = func(obj, *args, **kwargs)
+                s = str(type(tran))
+                if s.find("Cursor") > 0:
+                    cur = tran
+                    cur.execute(stat, param)
+                else:
+                    cur = tran.cursor()
+                    cur.execute(stat, param)
+                    cur.close()
+                    tran.commit()
+                return cur.lastrowid
+
+    return _execute
+
+
+def commit_ignore_error(conn):
+    """Ignore the error of no transaction is active.
+
+    The transaction may be already committed by user's task_done call.
+    It's safe to ignore all errors of this kind.
+    """
+    try:
+        conn.commit()
+    except sqlite3.OperationalError as ex:
+        if 'no transaction is active' in str(ex):
+            log.debug(
+                'Not able to commit the transaction, '
+                'may already be committed.'
+            )
+        else:
+            raise
+
+
+class SQLBase(object):
+    """SQL base class."""
+
+    _TABLE_NAME = 'base'  # DB table name
+    _KEY_COLUMN = ''  # the name of the key column, used in DB CRUD
+    _SQL_CREATE = ''  # SQL to create a table
+    _SQL_UPDATE = ''  # SQL to update a record
+    _SQL_INSERT = ''  # SQL to insert a record
+    _SQL_SELECT = ''  # SQL to select a record
+    _SQL_SELECT_ID = ''  # SQL to select a record with criteria
+    _SQL_SELECT_WHERE = ''  # SQL to select a record with criteria
+    _SQL_DELETE = ''  # SQL to delete a record
+    # _MEMORY = ':memory:'  # flag indicating store DB in memory
+
+    def __init__(self):
+        """Initiate a queue in db.
+        """
+        self._serializer = None
+        self.auto_commit = None
+
+        # SQL transaction lock
+        self.tran_lock = threading.Lock()
+        self.put_event = threading.Event()
+        # Action lock to assure multiple action to be *atomic*
+        self.action_lock = threading.Lock()
+        self.total = 0
+        self.cursor = 0
+        self._getter = None
+        self._putter = None
+
+    @with_conditional_transaction
+    def _insert_into(self, *record):
+        return self._sql_insert, record
+
+    @with_conditional_transaction
+    def _update(self, key, *args):
+        args = list(args) + [key]
+        return self._sql_update, args
+
+    @with_conditional_transaction
+    def _delete(self, key, op='='):
+
+        sql = self._SQL_DELETE.format(
+            table_name=self._table_name, key_column=self._key_column, op=op)
+        return sql, (key,)
+
+    def _pop(self, rowid=None, raw=False):
+        with self.action_lock:
+            if self.auto_commit:
+                row = self._select(rowid=rowid)
+                # Perhaps a sqlite3 bug, sometimes (None, None) is returned
+                # by select, below can avoid these invalid records.
+                if row and row[0] is not None:
+                    self._delete(row[0])
+                    self.total -= 1
+                    item = self._serializer.loads(row[1])
+                    if raw:
+                        return {
+                            'pqid': row[0],
+                            'data': item,
+                            'timestamp': row[2],
+                        }
+                    else:
+                        return item
+            else:
+                row = self._select(
+                    self.cursor, op=">", column=self._KEY_COLUMN, rowid=rowid
+                )
+                if row and row[0] is not None:
+                    self.cursor = row[0]
+                    self.total -= 1
+                    item = self._serializer.loads(row[1])
+                    if raw:
+                        return {
+                            'pqid': row[0],
+                            'data': item,
+                            'timestamp': row[2],
+                        }
+                    else:
+                        return item
+            return None
+
+    def update(self, item, id=None):
+        if isinstance(item, dict) and "pqid" in item:
+            _id = item.get("pqid")
+            item = item.get("data")
+        if id is not None:
+            _id = id
+        if _id is None:
+            raise ValueError("Provide an id or raw item")
+        obj = self._serializer.dumps(item)
+        self._update(_id, obj)
+        return _id
+
+    def get(self, block=True, timeout=None, id=None, raw=False):
+        if isinstance(id, dict) and "pqid" in id:
+            rowid = id.get("pqid")
+        elif isinstance(id, int):
+            rowid = id
+        else:
+            rowid = None
+        if not block:
+            serialized = self._pop(raw=raw, rowid=rowid)
+            if serialized is None:
+                raise Empty
+        elif timeout is None:
+            # block until a put event.
+            serialized = self._pop(raw=raw, rowid=rowid)
+            while serialized is None:
+                self.put_event.clear()
+                self.put_event.wait(TICK_FOR_WAIT)
+                serialized = self._pop(raw=raw, rowid=rowid)
+        elif timeout < 0:
+            raise ValueError("'timeout' must be a non-negative number")
+        else:
+            # block until the timeout reached
+            endtime = _time.time() + timeout
+            serialized = self._pop(raw=raw, rowid=rowid)
+            while serialized is None:
+                self.put_event.clear()
+                remaining = endtime - _time.time()
+                if remaining <= 0.0:
+                    raise Empty
+                self.put_event.wait(
+                    TICK_FOR_WAIT if TICK_FOR_WAIT < remaining else remaining
+                )
+                serialized = self._pop(raw=raw, rowid=rowid)
+        return serialized
+
+    def get_nowait(self, id=None, raw=False):
+        return self.get(block=False, id=id, raw=raw)
+
+    def task_done(self):
+        """Persist the current state if auto_commit=False."""
+        if not self.auto_commit:
+            self._delete(self.cursor, op='<=')
+            self._task_done()
+
+    def queue(self):
+        rows = self._sql_queue().fetchall()
+        datarows = []
+        for row in rows:
+            item = {
+                'id': row[0],
+                'data': self._serializer.loads(row[1]),
+                'timestamp': row[2],
+            }
+            datarows.append(item)
+        return datarows
+
+    @with_conditional_transaction
+    def shrink_disk_usage(self):
+        sql = """VACUUM"""
+        return sql, ()
+
+    @property
+    def size(self):
+        return self.total
+
+    def qsize(self):
+        return max(0, self.size)
+
+    def empty(self):
+        return self.size == 0
+
+    def full(self):
+        return False
+
+    def __len__(self):
+        return self.size
+
+    def _select(self, *args, **kwargs):
+        start_key = self._start_key()
+        op = kwargs.get('op', None)
+        column = kwargs.get('column', None)
+        next_in_order = kwargs.get('next_in_order', False)
+        rowid = kwargs.get('rowid') if kwargs.get('rowid', None) else start_key
+        if not next_in_order and rowid != start_key:
+            # Get the record by the id
+            result = self._getter.execute(
+                self._sql_select_id(rowid), args
+            ).fetchone()
+        elif op and column:
+            # Get the next record with criteria
+            rowid = rowid if next_in_order else start_key
+            result = self._getter.execute(
+                self._sql_select_where(rowid, op, column), args
+            ).fetchone()
+        else:
+            # Get the next record
+            rowid = rowid if next_in_order else start_key
+            result = self._getter.execute(
+                self._sql_select(rowid), args
+            ).fetchone()
+        if (
+                next_in_order
+                and rowid != start_key
+                and (not result or len(result) == 0)
+        ):
+            # sqlackqueue: if we're at the end, start over
+            kwargs['rowid'] = start_key
+            result = self._select(*args, **kwargs)
+        return result
+
+    def _count(self):
+        sql = 'SELECT COUNT({}) FROM {}'.format(
+            self._key_column, self._table_name
+        )
+        row = self._getter.execute(sql).fetchone()
+        return row[0] if row else 0
+
+    def _start_key(self):
+        if self._TABLE_NAME == 'ack_filo_queue':
+            return 9223372036854775807  # maxsize
+        else:
+            return 0
+
+    def _task_done(self):
+        """Only required if auto-commit is set as False."""
+        commit_ignore_error(self._putter)
+
+    def _sql_queue(self):
+        sql = 'SELECT * FROM {}'.format(self._table_name)
+        return self._getter.execute(sql)
+
+    @property
+    def _table_name(self):
+        return '`{}_{}`'.format(self._TABLE_NAME, self.name)
+
+    @property
+    def _key_column(self):
+        return self._KEY_COLUMN
+
+    @property
+    def _sql_create(self):
+        return self._SQL_CREATE.format(
+            table_name=self._table_name, key_column=self._key_column
+        )
+
+    @property
+    def _sql_insert(self):
+        return self._SQL_INSERT.format(
+            table_name=self._table_name, key_column=self._key_column
+        )
+
+    @property
+    def _sql_update(self):
+        return self._SQL_UPDATE.format(
+            table_name=self._table_name, key_column=self._key_column
+        )
+
+    def _sql_select_id(self, rowid):
+        return self._SQL_SELECT_ID.format(
+            table_name=self._table_name,
+            key_column=self._key_column,
+            rowid=rowid,
+        )
+
+    def _sql_select(self, rowid):
+        return self._SQL_SELECT.format(
+            table_name=self._table_name,
+            key_column=self._key_column,
+            rowid=rowid,
+        )
+
+    def _sql_select_where(self, rowid, op, column):
+        return self._SQL_SELECT_WHERE.format(
+            table_name=self._table_name,
+            key_column=self._key_column,
+            rowid=rowid,
+            op=op,
+            column=column,
+        )
+
+    def __del__(self):
+        """Handles sqlite connection when queue was deleted"""
+        if self._getter:
+            self._getter.close()
+        if self._putter:
+            self._putter.close()
+
+
+class SQLiteBase(SQLBase):
+    """SQLite3 base class."""
+
+    _TABLE_NAME = 'base'  # DB table name
+    _KEY_COLUMN = ''  # the name of the key column, used in DB CRUD
+    _SQL_CREATE = ''  # SQL to create a table
+    _SQL_UPDATE = ''  # SQL to update a record
+    _SQL_INSERT = ''  # SQL to insert a record
+    _SQL_SELECT = ''  # SQL to select a record
+    _SQL_SELECT_ID = ''  # SQL to select a record with criteria
+    _SQL_SELECT_WHERE = ''  # SQL to select a record with criteria
+    _SQL_DELETE = ''  # SQL to delete a record
+    _MEMORY = ':memory:'  # flag indicating store DB in memory
+
+    def __init__(
+            self,
+            path,
+            name='default',
+            multithreading=False,
+            timeout=10.0,
+            auto_commit=True,
+            serializer=persistqueue.serializers.pickle,
+            db_file_name=None,
+    ):
+        """Initiate a queue in sqlite3 or memory.
+
+        :param path: path for storing DB file.
+        :param name: the suffix for the table name,
+                     table name would be ${_TABLE_NAME}_${name}
+        :param multithreading: if set to True, two db connections will be,
+                               one for **put** and one for **get**.
+        :param timeout: timeout in second waiting for the database lock.
+        :param auto_commit: Set to True, if commit is required on every
+                            INSERT/UPDATE action, otherwise False, whereas
+                            a **task_done** is required to persist changes
+                            after **put**.
+        :param serializer: The serializer parameter controls how enqueued data
+                           is serialized. It must have methods dump(value, fp)
+                           and load(fp). The dump method must serialize the
+                           value and write it to fp, and may be called for
+                           multiple values with the same fp. The load method
+                           must deserialize and return one value from fp,
+                           and may be called multiple times with the same fp
+                           to read multiple values.
+        :param db_file_name: set the db file name of the queue data, otherwise
+                             default to `data.db`
+        """
+        super(SQLiteBase, self).__init__()
+        self.memory_sql = False
+        self.path = path
+        self.name = name
+        self.timeout = timeout
+        self.multithreading = multithreading
+        self.auto_commit = auto_commit
+        self._serializer = serializer
+        self.db_file_name = "data.db"
+        if db_file_name:
+            self.db_file_name = db_file_name
+        self._init()
+
+    def _init(self):
+        """Initialize the tables in DB."""
+        if self.path == self._MEMORY:
+            self.memory_sql = True
+            log.debug("Initializing Sqlite3 Queue in memory.")
+        elif not os.path.exists(self.path):
+            os.makedirs(self.path)
+            log.debug(
+                'Initializing Sqlite3 Queue with path {}'.format(self.path)
+            )
+        self._conn = self._new_db_connection(
+            self.path, self.multithreading, self.timeout
+        )
+        self._getter = self._conn
+        self._putter = self._conn
+
+        self._conn.execute(self._sql_create)
+        self._conn.commit()
+        # Setup another session only for disk-based queue.
+        if self.multithreading:
+            if not self.memory_sql:
+                self._putter = self._new_db_connection(
+                    self.path, self.multithreading, self.timeout
+                )
+        self._conn.text_factory = str
+        self._putter.text_factory = str
+
+        # SQLite3 transaction lock
+        self.tran_lock = threading.Lock()
+        self.put_event = threading.Event()
+
+    def _new_db_connection(self, path, multithreading, timeout):
+        conn = None
+        if path == self._MEMORY:
+            conn = sqlite3.connect(path, check_same_thread=not multithreading)
+        else:
+            conn = sqlite3.connect(
+                '{}/{}'.format(path, self.db_file_name),
+                timeout=timeout,
+                check_same_thread=not multithreading,
+            )
+        conn.execute('PRAGMA journal_mode=WAL;')
+        return conn
+
+    def __del__(self):
+        """Handles sqlite connection when queue was deleted"""
+        self._getter.close()
+        self._putter.close()
```

### Comparing `persist-queue-0.8.0b0/persistqueue/__init__.py` & `persist-queue-0.8.1/persistqueue/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# coding=utf-8
-__author__ = 'Peter Wang'
-__license__ = 'BSD'
-__version__ = '0.8.0-beta0'
-
-from .exceptions import Empty, Full  # noqa
-from .queue import Queue  # noqa
-
-try:
-    from .pdict import PDict  # noqa
-    from .sqlqueue import SQLiteQueue, FIFOSQLiteQueue, FILOSQLiteQueue, \
-        UniqueQ  # noqa
-    from .sqlackqueue import SQLiteAckQueue, UniqueAckQ
-    from .mysqlqueue import MySQLQueue
-except ImportError:
-    import logging
-
-    log = logging.getLogger(__name__)
-    log.info("No sqlite3 module found, sqlite3 based queues are not available")
-
-__all__ = ["Queue", "SQLiteQueue", "FIFOSQLiteQueue", "FILOSQLiteQueue",
-           "UniqueQ", "PDict", "SQLiteAckQueue", "UniqueAckQ", "MySQLQueue",
-           "Empty", "Full", "__author__", "__license__", "__version__"]
+# coding=utf-8
+__author__ = 'Peter Wang'
+__license__ = 'BSD'
+__version__ = '0.8.1'
+
+from .exceptions import Empty, Full  # noqa
+from .queue import Queue  # noqa
+
+try:
+    from .pdict import PDict  # noqa
+    from .sqlqueue import SQLiteQueue, FIFOSQLiteQueue, FILOSQLiteQueue, \
+        UniqueQ  # noqa
+    from .sqlackqueue import SQLiteAckQueue, FIFOSQLiteAckQueue, \
+        FILOSQLiteAckQueue, UniqueAckQ, AckStatus # noqa
+    from .mysqlqueue import MySQLQueue
+except ImportError:
+    import logging
+
+    log = logging.getLogger(__name__)
+    log.info("No sqlite3 module found, sqlite3 based queues are not available")
+
+__all__ = ["Queue", "SQLiteQueue", "FIFOSQLiteQueue", "FILOSQLiteQueue",
+           "UniqueQ", "PDict", "SQLiteAckQueue", "FIFOSQLiteAckQueue",
+           "FILOSQLiteAckQueue", "UniqueAckQ", "AckStatus", "MySQLQueue",
+           "Empty", "Full", "__author__", "__license__", "__version__"]
```

### Comparing `persist-queue-0.8.0b0/persistqueue/serializers/msgpack.py` & `persist-queue-0.8.1/persistqueue/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `persist-queue-0.8.0b0/persistqueue/serializers/pickle.py` & `persist-queue-0.8.1/persistqueue/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `persist-queue-0.8.0b0/persistqueue/serializers/json.py` & `persist-queue-0.8.1/persistqueue/serializers/json.py`

 * *Files identical despite different names*

### Comparing `persist-queue-0.8.0b0/persistqueue/sqlackqueue.py` & `persist-queue-0.8.1/persistqueue/sqlackqueue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,384 +1,387 @@
-# coding=utf-8
-from __future__ import absolute_import
-from __future__ import unicode_literals
-
-import logging
-import sqlite3
-import time as _time
-import threading
-import warnings
-
-from . import sqlbase
-from .exceptions import Empty
-
-sqlite3.enable_callback_tracebacks(True)
-
-log = logging.getLogger(__name__)
-
-# 10 seconds internal for `wait` of event
-TICK_FOR_WAIT = 10
-
-
-class AckStatus(object):
-    inited = '0'
-    ready = '1'
-    unack = '2'
-    acked = '5'
-    ack_failed = '9'
-
-
-class SQLiteAckQueue(sqlbase.SQLiteBase):
-    """SQLite3 based FIFO queue with ack support."""
-
-    _TABLE_NAME = 'ack_queue'
-    _KEY_COLUMN = '_id'  # the name of the key column, used in DB CRUD
-    _MAX_ACKED_LENGTH = 1000  # deprecated
-    # SQL to create a table
-    _SQL_CREATE = (
-        'CREATE TABLE IF NOT EXISTS {table_name} ('
-        '{key_column} INTEGER PRIMARY KEY AUTOINCREMENT, '
-        'data BLOB, timestamp FLOAT, status INTEGER)'
-    )
-    # SQL to insert a record
-    _SQL_INSERT = (
-        'INSERT INTO {table_name} (data, timestamp, status)'
-        ' VALUES (?, ?, %s)' % AckStatus.inited
-    )
-    # SQL to select a record
-    _SQL_SELECT_ID = (
-        'SELECT {key_column}, data, timestamp, status FROM {table_name} WHERE'
-        ' {key_column} = {rowid}'
-    )
-    _SQL_SELECT = (
-        'SELECT {key_column}, data, timestamp, status FROM {table_name} '
-        'WHERE {key_column} > {rowid} AND status < %s '
-        'ORDER BY {key_column} ASC LIMIT 1' % AckStatus.unack
-    )
-    _SQL_MARK_ACK_UPDATE = (
-        'UPDATE {table_name} SET status = ? WHERE {key_column} = ?'
-    )
-    _SQL_SELECT_WHERE = (
-        'SELECT {key_column}, data, timestamp FROM {table_name}'
-        ' WHERE {key_column} > {rowid} AND status < %s AND'
-        ' {column} {op} ? ORDER BY {key_column} ASC'
-        ' LIMIT 1 ' % AckStatus.unack
-    )
-    _SQL_UPDATE = 'UPDATE {table_name} SET data = ? WHERE {key_column} = ?'
-
-    def __init__(self, path, auto_resume=True, **kwargs):
-        super(SQLiteAckQueue, self).__init__(path, **kwargs)
-        if not self.auto_commit:
-            warnings.warn("disable auto commit is not support in ack queue")
-            self.auto_commit = True
-        self._unack_cache = {}
-        if auto_resume:
-            self.resume_unack_tasks()
-
-    def resume_unack_tasks(self):
-        unack_count = self.unack_count()
-        if unack_count:
-            log.info("resume %d unack tasks", unack_count)
-        sql = 'UPDATE {} set status = ?' \
-              ' WHERE status = ?'.format(self._table_name)
-        with self.tran_lock:
-            with self._putter as tran:
-                tran.execute(sql, (AckStatus.ready, AckStatus.unack,))
-            self.total = self._count()
-
-    def put(self, item):
-        obj = self._serializer.dumps(item)
-        _id = self._insert_into(obj, _time.time())
-        self.total += 1
-        self.put_event.set()
-        return _id
-
-    def _init(self):
-        super(SQLiteAckQueue, self)._init()
-        # Action lock to assure multiple action to be *atomic*
-        self.action_lock = threading.Lock()
-        self.total = self._count()
-
-    def _count(self):
-        sql = 'SELECT COUNT({}) FROM {} WHERE status < ?'.format(
-            self._key_column, self._table_name
-        )
-        row = self._getter.execute(sql, (AckStatus.unack,)).fetchone()
-        return row[0] if row else 0
-
-    def _ack_count_via_status(self, status):
-        sql = 'SELECT COUNT({}) FROM {} WHERE status = ?'.format(
-            self._key_column, self._table_name
-        )
-        row = self._getter.execute(sql, (status,)).fetchone()
-        return row[0] if row else 0
-
-    def unack_count(self):
-        return self._ack_count_via_status(AckStatus.unack)
-
-    def acked_count(self):
-        return self._ack_count_via_status(AckStatus.acked)
-
-    def ready_count(self):
-        return self._ack_count_via_status(AckStatus.ready)
-
-    def ack_failed_count(self):
-        return self._ack_count_via_status(AckStatus.ack_failed)
-
-    @sqlbase.with_conditional_transaction
-    def _mark_ack_status(self, key, status):
-        return self._sql_mark_ack_status, (
-            status,
-            key,
-        )
-
-    @sqlbase.with_conditional_transaction
-    def clear_acked_data(
-        self, max_delete=1000, keep_latest=1000, clear_ack_failed=False
-    ):
-        acked_clear_all = ''
-        acked_to_delete = ''
-        acked_to_keep = ''
-        if self._MAX_ACKED_LENGTH != 1000 and not max_delete:
-            # Added for backward compatibility for
-            # those that set the _MAX_ACKED_LENGTH
-            print(
-                "_MAX_ACKED_LENGTH has been deprecated.  \
-                    Use clear_acked_data(keep_latest=1000, max_delete=1000)"
-            )
-            keep_latest = self._MAX_ACKED_LENGTH
-        if clear_ack_failed:
-            acked_clear_all = 'OR status = %s' % AckStatus.ack_failed
-        if max_delete and max_delete > 0:
-            acked_to_delete = 'LIMIT %d' % max_delete
-        if keep_latest and keep_latest > 0:
-            acked_to_keep = 'OFFSET %d' % keep_latest
-        sql = """DELETE FROM {table_name}
-            WHERE {key_column} IN (
-                SELECT _id FROM {table_name}
-                WHERE status = ? {clear_ack_failed}
-                ORDER BY {key_column}
-                DESC {acked_to_delete} {acked_to_keep}
-            )""".format(
-            table_name=self._table_name,
-            key_column=self._key_column,
-            acked_to_delete=acked_to_delete,
-            acked_to_keep=acked_to_keep,
-            clear_ack_failed=acked_clear_all,
-        )
-        return sql, AckStatus.acked
-
-    @property
-    def _sql_mark_ack_status(self):
-        return self._SQL_MARK_ACK_UPDATE.format(
-            table_name=self._table_name, key_column=self._key_column
-        )
-
-    def _pop(self, rowid=None, next_in_order=False, raw=False):
-        with self.action_lock:
-            row = self._select(next_in_order=next_in_order, rowid=rowid)
-            # Perhaps a sqlite3 bug, sometimes (None, None) is returned
-            # by select, below can avoid these invalid records.
-            if row and row[0] is not None:
-                self._mark_ack_status(row[0], AckStatus.unack)
-                serialized_data = row[1]
-                item = self._serializer.loads(serialized_data)
-                self._unack_cache[row[0]] = item
-                self.total -= 1
-                if raw:
-                    return {'pqid': row[0], 'data': item, 'timestamp': row[2]}
-                else:
-                    return item
-            return None
-
-    def _find_item_id(self, item, search=True):
-        if item is None:
-            return None
-        elif isinstance(item, dict) and "pqid" in item:
-            return item.get("pqid")
-        elif search:
-            for key, value in self._unack_cache.items():
-                if value is item:
-                    return key
-        elif isinstance(item, int) or (
-            isinstance(item, str) and item.isnumeric()
-        ):
-            return int(item)
-        log.warning("Item id not Interger and can't find item in unack cache.")
-        return None
-
-    def _check_id(self, item, id):
-        if id is not None and item is not None:
-            raise ValueError("Specify an id or an item, not both.")
-        elif id is None and item is None:
-            raise ValueError("Specify an id or an item.")
-        elif id is not None:
-            search = False
-            item = id
-        else:
-            search = True
-        return item, search
-
-    def ack(self, item=None, id=None):
-        item, search = self._check_id(item, id)
-        with self.action_lock:
-            _id = self._find_item_id(item, search)
-            if _id is None:
-                return None
-            self._mark_ack_status(_id, AckStatus.acked)
-            if _id in self._unack_cache:
-                self._unack_cache.pop(_id)
-        return _id
-
-    def ack_failed(self, item=None, id=None):
-        item, search = self._check_id(item, id)
-        with self.action_lock:
-            _id = self._find_item_id(item, search)
-            if _id is None:
-                return None
-            self._mark_ack_status(_id, AckStatus.ack_failed)
-            if _id in self._unack_cache:
-                self._unack_cache.pop(_id)
-        return _id
-
-    def nack(self, item=None, id=None):
-        item, search = self._check_id(item, id)
-        with self.action_lock:
-            _id = self._find_item_id(item, search)
-            if _id is None:
-                return None
-            self._mark_ack_status(_id, AckStatus.ready)
-            if _id in self._unack_cache:
-                self._unack_cache.pop(_id)
-            self.total += 1
-        return _id
-
-    def update(self, item, id=None):
-        _id = None
-        if isinstance(item, dict) and "pqid" in item:
-            _id = item.get("pqid")
-            item = item.get("data")
-        if id is not None:
-            _id = id
-        if _id is None:
-            raise ValueError("Provide an id or raw item")
-        obj = self._serializer.dumps(item)
-        self._update(_id, obj)
-        return _id
-
-    def get(
-        self, block=True, timeout=None, id=None, next_in_order=False, raw=False
-    ):
-        rowid = self._find_item_id(id, search=False)
-        if rowid is None and next_in_order:
-            raise ValueError(
-                "'next_in_order' requires the preceding 'id' be specified."
-            )
-        if next_in_order and not isinstance(next_in_order, bool):
-            raise ValueError("'next_in_order' must be a boolean (True/False)")
-        if not block:
-            serialized = self._pop(
-                next_in_order=next_in_order, raw=raw, rowid=rowid
-            )
-            if serialized is None:
-                raise Empty
-        elif timeout is None:
-            # block until a put event.
-            serialized = self._pop(
-                next_in_order=next_in_order, raw=raw, rowid=rowid
-            )
-            while serialized is None:
-                self.put_event.clear()
-                self.put_event.wait(TICK_FOR_WAIT)
-                serialized = self._pop(
-                    next_in_order=next_in_order, raw=raw, rowid=rowid
-                )
-        elif timeout < 0:
-            raise ValueError("'timeout' must be a non-negative number")
-        else:
-            # block until the timeout reached
-            endtime = _time.time() + timeout
-            serialized = self._pop(
-                next_in_order=next_in_order, raw=raw, rowid=rowid
-            )
-            while serialized is None:
-                self.put_event.clear()
-                remaining = endtime - _time.time()
-                if remaining <= 0.0:
-                    raise Empty
-                self.put_event.wait(
-                    TICK_FOR_WAIT if TICK_FOR_WAIT < remaining else remaining
-                )
-                serialized = self._pop(
-                    next_in_order=next_in_order, raw=raw, rowid=rowid
-                )
-        return serialized
-
-    def task_done(self):
-        """Persist the current state if auto_commit=False."""
-        if not self.auto_commit:
-            self._task_done()
-
-    def queue(self):
-        rows = self._sql_queue()
-        datarows = []
-        for row in rows:
-            item = {
-                'id': row[0],
-                'data': self._serializer.loads(row[1]),
-                'timestamp': row[2],
-                'status': row[3],
-            }
-            datarows.append(item)
-        return datarows
-
-    @property
-    def size(self):
-        return self.total
-
-    def qsize(self):
-        return max(0, self.size)
-
-    def active_size(self):
-        return max(0, self.size + len(self._unack_cache))
-
-    def empty(self):
-        return self.size == 0
-
-    def __len__(self):
-        return self.size
-
-
-FIFOSQLiteAckQueue = SQLiteAckQueue
-
-
-class FILOSQLiteAckQueue(SQLiteAckQueue):
-    """SQLite3 based FILO queue with ack support."""
-
-    _TABLE_NAME = 'ack_filo_queue'
-    # SQL to select a record
-    _SQL_SELECT = (
-        'SELECT {key_column}, data, timestamp, status FROM {table_name} '
-        'WHERE {key_column} < {rowid} and status < %s '
-        'ORDER BY {key_column} DESC LIMIT 1' % AckStatus.unack
-    )
-
-
-class UniqueAckQ(SQLiteAckQueue):
-    _TABLE_NAME = 'ack_unique_queue'
-    _SQL_CREATE = (
-        'CREATE TABLE IF NOT EXISTS {table_name} ('
-        '{key_column} INTEGER PRIMARY KEY AUTOINCREMENT, '
-        'data BLOB, timestamp FLOAT, status INTEGER, UNIQUE (data))'
-    )
-
-    def put(self, item):
-        obj = self._serializer.dumps(item, sort_keys=True)
-        _id = None
-        try:
-            _id = self._insert_into(obj, _time.time())
-        except sqlite3.IntegrityError:
-            pass
-        else:
-            self.total += 1
-            self.put_event.set()
-        return _id
+# coding=utf-8
+from __future__ import absolute_import
+from __future__ import unicode_literals
+
+import logging
+import sqlite3
+import time as _time
+import threading
+import warnings
+
+from . import sqlbase
+from .exceptions import Empty
+
+sqlite3.enable_callback_tracebacks(True)
+
+log = logging.getLogger(__name__)
+
+# 10 seconds internal for `wait` of event
+TICK_FOR_WAIT = 10
+
+
+class AckStatus(object):
+    inited = '0'
+    ready = '1'
+    unack = '2'
+    acked = '5'
+    ack_failed = '9'
+
+
+class SQLiteAckQueue(sqlbase.SQLiteBase):
+    """SQLite3 based FIFO queue with ack support."""
+
+    _TABLE_NAME = 'ack_queue'
+    _KEY_COLUMN = '_id'  # the name of the key column, used in DB CRUD
+    _MAX_ACKED_LENGTH = 1000  # deprecated
+    # SQL to create a table
+    _SQL_CREATE = (
+        'CREATE TABLE IF NOT EXISTS {table_name} ('
+        '{key_column} INTEGER PRIMARY KEY AUTOINCREMENT, '
+        'data BLOB, timestamp FLOAT, status INTEGER)'
+    )
+    # SQL to insert a record
+    _SQL_INSERT = (
+        'INSERT INTO {table_name} (data, timestamp, status)'
+        ' VALUES (?, ?, %s)' % AckStatus.inited
+    )
+    # SQL to select a record
+    _SQL_SELECT_ID = (
+        'SELECT {key_column}, data, timestamp, status FROM {table_name} WHERE'
+        ' {key_column} = {rowid}'
+    )
+    _SQL_SELECT = (
+        'SELECT {key_column}, data, timestamp, status FROM {table_name} '
+        'WHERE {key_column} > {rowid} AND status < %s '
+        'ORDER BY {key_column} ASC LIMIT 1' % AckStatus.unack
+    )
+    _SQL_MARK_ACK_UPDATE = (
+        'UPDATE {table_name} SET status = ? WHERE {key_column} = ?'
+    )
+    _SQL_SELECT_WHERE = (
+        'SELECT {key_column}, data, timestamp FROM {table_name}'
+        ' WHERE {key_column} > {rowid} AND status < %s AND'
+        ' {column} {op} ? ORDER BY {key_column} ASC'
+        ' LIMIT 1 ' % AckStatus.unack
+    )
+    _SQL_UPDATE = 'UPDATE {table_name} SET data = ? WHERE {key_column} = ?'
+
+    def __init__(self, path, auto_resume=True, **kwargs):
+        super(SQLiteAckQueue, self).__init__(path, **kwargs)
+        if not self.auto_commit:
+            warnings.warn("disable auto commit is not support in ack queue")
+            self.auto_commit = True
+        self._unack_cache = {}
+        if auto_resume:
+            self.resume_unack_tasks()
+
+    def resume_unack_tasks(self):
+        unack_count = self.unack_count()
+        if unack_count:
+            log.info("resume %d unack tasks", unack_count)
+        sql = 'UPDATE {} set status = ?' \
+              ' WHERE status = ?'.format(self._table_name)
+        with self.tran_lock:
+            with self._putter as tran:
+                tran.execute(sql, (AckStatus.ready, AckStatus.unack,))
+            self.total = self._count()
+
+    def put(self, item):
+        obj = self._serializer.dumps(item)
+        _id = self._insert_into(obj, _time.time())
+        self.total += 1
+        self.put_event.set()
+        return _id
+
+    def _init(self):
+        super(SQLiteAckQueue, self)._init()
+        # Action lock to assure multiple action to be *atomic*
+        self.action_lock = threading.Lock()
+        self.total = self._count()
+
+    def _count(self):
+        sql = 'SELECT COUNT({}) FROM {} WHERE status < ?'.format(
+            self._key_column, self._table_name
+        )
+        row = self._getter.execute(sql, (AckStatus.unack,)).fetchone()
+        return row[0] if row else 0
+
+    def _ack_count_via_status(self, status):
+        sql = 'SELECT COUNT({}) FROM {} WHERE status = ?'.format(
+            self._key_column, self._table_name
+        )
+        row = self._getter.execute(sql, (status,)).fetchone()
+        return row[0] if row else 0
+
+    def unack_count(self):
+        return self._ack_count_via_status(AckStatus.unack)
+
+    def acked_count(self):
+        return self._ack_count_via_status(AckStatus.acked)
+
+    def ready_count(self):
+        return self._ack_count_via_status(AckStatus.ready)
+
+    def ack_failed_count(self):
+        return self._ack_count_via_status(AckStatus.ack_failed)
+
+    @sqlbase.with_conditional_transaction
+    def _mark_ack_status(self, key, status):
+        return self._sql_mark_ack_status, (
+            status,
+            key,
+        )
+
+    @sqlbase.with_conditional_transaction
+    def clear_acked_data(
+        self, max_delete=1000, keep_latest=1000, clear_ack_failed=False
+    ):
+        acked_clear_all = ''
+        acked_to_delete = ''
+        acked_to_keep = ''
+        if self._MAX_ACKED_LENGTH != 1000 and not max_delete:
+            # Added for backward compatibility for
+            # those that set the _MAX_ACKED_LENGTH
+            print(
+                "_MAX_ACKED_LENGTH has been deprecated.  \
+                    Use clear_acked_data(keep_latest=1000, max_delete=1000)"
+            )
+            keep_latest = self._MAX_ACKED_LENGTH
+        if clear_ack_failed:
+            acked_clear_all = 'OR status = %s' % AckStatus.ack_failed
+        if max_delete and max_delete > 0:
+            acked_to_delete = 'LIMIT %d' % max_delete
+        if keep_latest and keep_latest > 0:
+            acked_to_keep = 'OFFSET %d' % keep_latest
+        sql = """DELETE FROM {table_name}
+            WHERE {key_column} IN (
+                SELECT _id FROM {table_name}
+                WHERE status = ? {clear_ack_failed}
+                ORDER BY {key_column}
+                DESC {acked_to_delete} {acked_to_keep}
+            )""".format(
+            table_name=self._table_name,
+            key_column=self._key_column,
+            acked_to_delete=acked_to_delete,
+            acked_to_keep=acked_to_keep,
+            clear_ack_failed=acked_clear_all,
+        )
+        return sql, AckStatus.acked
+
+    @property
+    def _sql_mark_ack_status(self):
+        return self._SQL_MARK_ACK_UPDATE.format(
+            table_name=self._table_name, key_column=self._key_column
+        )
+
+    def _pop(self, rowid=None, next_in_order=False, raw=False):
+        with self.action_lock:
+            row = self._select(next_in_order=next_in_order, rowid=rowid)
+            # Perhaps a sqlite3 bug, sometimes (None, None) is returned
+            # by select, below can avoid these invalid records.
+            if row and row[0] is not None:
+                self._mark_ack_status(row[0], AckStatus.unack)
+                serialized_data = row[1]
+                item = self._serializer.loads(serialized_data)
+                self._unack_cache[row[0]] = item
+                self.total -= 1
+                if raw:
+                    return {'pqid': row[0], 'data': item, 'timestamp': row[2]}
+                else:
+                    return item
+            return None
+
+    def _find_item_id(self, item, search=True):
+        if item is None:
+            return None
+        elif isinstance(item, dict) and "pqid" in item:
+            return item.get("pqid")
+        elif search:
+            for key, value in self._unack_cache.items():
+                if value is item:
+                    return key
+        elif isinstance(item, int) or (
+            isinstance(item, str) and item.isnumeric()
+        ):
+            return int(item)
+        log.warning("Item id not Interger and can't find item in unack cache.")
+        return None
+
+    def _check_id(self, item, id):
+        if id is not None and item is not None:
+            raise ValueError("Specify an id or an item, not both.")
+        elif id is None and item is None:
+            raise ValueError("Specify an id or an item.")
+        elif id is not None:
+            search = False
+            item = id
+        else:
+            search = True
+        return item, search
+
+    def ack(self, item=None, id=None):
+        item, search = self._check_id(item, id)
+        with self.action_lock:
+            _id = self._find_item_id(item, search)
+            if _id is None:
+                return None
+            self._mark_ack_status(_id, AckStatus.acked)
+            if _id in self._unack_cache:
+                self._unack_cache.pop(_id)
+        return _id
+
+    def ack_failed(self, item=None, id=None):
+        item, search = self._check_id(item, id)
+        with self.action_lock:
+            _id = self._find_item_id(item, search)
+            if _id is None:
+                return None
+            self._mark_ack_status(_id, AckStatus.ack_failed)
+            if _id in self._unack_cache:
+                self._unack_cache.pop(_id)
+        return _id
+
+    def nack(self, item=None, id=None):
+        item, search = self._check_id(item, id)
+        with self.action_lock:
+            _id = self._find_item_id(item, search)
+            if _id is None:
+                return None
+            self._mark_ack_status(_id, AckStatus.ready)
+            if _id in self._unack_cache:
+                self._unack_cache.pop(_id)
+            self.total += 1
+        return _id
+
+    def update(self, item, id=None):
+        _id = None
+        if isinstance(item, dict) and "pqid" in item:
+            _id = item.get("pqid")
+            item = item.get("data")
+        if id is not None:
+            _id = id
+        if _id is None:
+            raise ValueError("Provide an id or raw item")
+        obj = self._serializer.dumps(item)
+        self._update(_id, obj)
+        return _id
+
+    def get(
+        self, block=True, timeout=None, id=None, next_in_order=False, raw=False
+    ):
+        rowid = self._find_item_id(id, search=False)
+        if rowid is None and next_in_order:
+            raise ValueError(
+                "'next_in_order' requires the preceding 'id' be specified."
+            )
+        if next_in_order and not isinstance(next_in_order, bool):
+            raise ValueError("'next_in_order' must be a boolean (True/False)")
+        if not block:
+            serialized = self._pop(
+                next_in_order=next_in_order, raw=raw, rowid=rowid
+            )
+            if serialized is None:
+                raise Empty
+        elif timeout is None:
+            # block until a put event.
+            serialized = self._pop(
+                next_in_order=next_in_order, raw=raw, rowid=rowid
+            )
+            while serialized is None:
+                self.put_event.clear()
+                self.put_event.wait(TICK_FOR_WAIT)
+                serialized = self._pop(
+                    next_in_order=next_in_order, raw=raw, rowid=rowid
+                )
+        elif timeout < 0:
+            raise ValueError("'timeout' must be a non-negative number")
+        else:
+            # block until the timeout reached
+            endtime = _time.time() + timeout
+            serialized = self._pop(
+                next_in_order=next_in_order, raw=raw, rowid=rowid
+            )
+            while serialized is None:
+                self.put_event.clear()
+                remaining = endtime - _time.time()
+                if remaining <= 0.0:
+                    raise Empty
+                self.put_event.wait(
+                    TICK_FOR_WAIT if TICK_FOR_WAIT < remaining else remaining
+                )
+                serialized = self._pop(
+                    next_in_order=next_in_order, raw=raw, rowid=rowid
+                )
+        return serialized
+
+    def task_done(self):
+        """Persist the current state if auto_commit=False."""
+        if not self.auto_commit:
+            self._task_done()
+
+    def queue(self):
+        rows = self._sql_queue()
+        datarows = []
+        for row in rows:
+            item = {
+                'id': row[0],
+                'data': self._serializer.loads(row[1]),
+                'timestamp': row[2],
+                'status': row[3],
+            }
+            datarows.append(item)
+        return datarows
+
+    @property
+    def size(self):
+        return self.total
+
+    def qsize(self):
+        return max(0, self.size)
+
+    def active_size(self):
+        return max(0, self.size + len(self._unack_cache))
+
+    def empty(self):
+        return self.size == 0
+
+    def full(self):
+        return False
+
+    def __len__(self):
+        return self.size
+
+
+FIFOSQLiteAckQueue = SQLiteAckQueue
+
+
+class FILOSQLiteAckQueue(SQLiteAckQueue):
+    """SQLite3 based FILO queue with ack support."""
+
+    _TABLE_NAME = 'ack_filo_queue'
+    # SQL to select a record
+    _SQL_SELECT = (
+        'SELECT {key_column}, data, timestamp, status FROM {table_name} '
+        'WHERE {key_column} < {rowid} and status < %s '
+        'ORDER BY {key_column} DESC LIMIT 1' % AckStatus.unack
+    )
+
+
+class UniqueAckQ(SQLiteAckQueue):
+    _TABLE_NAME = 'ack_unique_queue'
+    _SQL_CREATE = (
+        'CREATE TABLE IF NOT EXISTS {table_name} ('
+        '{key_column} INTEGER PRIMARY KEY AUTOINCREMENT, '
+        'data BLOB, timestamp FLOAT, status INTEGER, UNIQUE (data))'
+    )
+
+    def put(self, item):
+        obj = self._serializer.dumps(item, sort_keys=True)
+        _id = None
+        try:
+            _id = self._insert_into(obj, _time.time())
+        except sqlite3.IntegrityError:
+            pass
+        else:
+            self.total += 1
+            self.put_event.set()
+        return _id
```

### Comparing `persist-queue-0.8.0b0/LICENSE` & `persist-queue-0.8.1/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-Copyright (c) G. B. Versiani.
-Copyright (c) Peter Wang.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification,
-are permitted provided that the following conditions are met:
-
-    1. Redistributions of source code must retain the above copyright notice, 
-       this list of conditions and the following disclaimer.
-    
-    2. Redistributions in binary form must reproduce the above copyright 
-       notice, this list of conditions and the following disclaimer in the
-       documentation and/or other materials provided with the distribution.
-
-    3. Neither the name of python-pqueue nor the names of its contributors may be used
-       to endorse or promote products derived from this software without
-       specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
-ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Copyright (c) G. B. Versiani.
+Copyright (c) Peter Wang.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without modification,
+are permitted provided that the following conditions are met:
+
+    1. Redistributions of source code must retain the above copyright notice, 
+       this list of conditions and the following disclaimer.
+    
+    2. Redistributions in binary form must reproduce the above copyright 
+       notice, this list of conditions and the following disclaimer in the
+       documentation and/or other materials provided with the distribution.
+
+    3. Neither the name of python-pqueue nor the names of its contributors may be used
+       to endorse or promote products derived from this software without
+       specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
+ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `persist-queue-0.8.0b0/setup.py` & `persist-queue-0.8.1/setup.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-#!/usr/bin/env python
-# coding=utf-8
-
-from setuptools import setup, find_packages
-
-
-def get_extras():
-    return {
-        "extra": open("extra-requirements.txt").read().splitlines()
-    }
-
-
-setup(
-    name='persist-queue',
-    version=__import__('persistqueue').__version__,
-    description=(
-        'A thread-safe disk based persistent queue in Python.'
-    ),
-    long_description=open('README.rst').read(),
-    long_description_content_type='text/x-rst',
-    author=__import__('persistqueue').__author__,
-    author_email='wangxu198709@gmail.com',
-    maintainer=__import__('persistqueue').__author__,
-    maintainer_email='wangxu198709@gmail.com',
-    license=__import__('persistqueue').__license__,
-    packages=find_packages(),
-    extras_require=get_extras(),
-    platforms=["all"],
-    url='http://github.com/peter-wangxu/persist-queue',
-    classifiers=[
-        'Development Status :: 4 - Beta',
-        'Operating System :: OS Independent',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: Implementation',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Topic :: Software Development :: Libraries'
-    ],
-)
+#!/usr/bin/env python
+# coding=utf-8
+
+from setuptools import setup, find_packages
+
+
+def get_extras():
+    return {
+        "extra": open("extra-requirements.txt").read().splitlines()
+    }
+
+
+setup(
+    name='persist-queue',
+    version=__import__('persistqueue').__version__,
+    description=(
+        'A thread-safe disk based persistent queue in Python.'
+    ),
+    long_description=open('README.rst').read(),
+    long_description_content_type='text/x-rst',
+    author=__import__('persistqueue').__author__,
+    author_email='wangxu198709@gmail.com',
+    maintainer=__import__('persistqueue').__author__,
+    maintainer_email='wangxu198709@gmail.com',
+    license=__import__('persistqueue').__license__,
+    packages=find_packages(),
+    extras_require=get_extras(),
+    platforms=["all"],
+    url='http://github.com/peter-wangxu/persist-queue',
+    classifiers=[
+        'Development Status :: 4 - Beta',
+        'Operating System :: OS Independent',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: BSD License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: Implementation',
+        'Programming Language :: Python :: 2',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Topic :: Software Development :: Libraries'
+    ],
+)
```

### Comparing `persist-queue-0.8.0b0/README.rst` & `persist-queue-0.8.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,604 +1,645 @@
-persist-queue - A thread-safe, disk-based queue for Python
-==========================================================
-
-.. image:: https://img.shields.io/circleci/project/github/peter-wangxu/persist-queue/master.svg?label=Linux%20%26%20Mac
-    :target: https://circleci.com/gh/peter-wangxu/persist-queue
-
-.. image:: https://img.shields.io/appveyor/ci/peter-wangxu/persist-queue/master.svg?label=Windows
-    :target: https://ci.appveyor.com/project/peter-wangxu/persist-queue
-
-.. image:: https://img.shields.io/codecov/c/github/peter-wangxu/persist-queue/master.svg
-    :target: https://codecov.io/gh/peter-wangxu/persist-queue
-
-.. image:: https://img.shields.io/pypi/v/persist-queue.svg
-    :target: https://pypi.python.org/pypi/persist-queue
-
-``persist-queue`` implements a file-based queue and a serial of sqlite3-based queues. The goals is to achieve following requirements:
-
-* Disk-based: each queued item should be stored in disk in case of any crash.
-* Thread-safe: can be used by multi-threaded producers and multi-threaded consumers.
-* Recoverable: Items can be read after process restart.
-* Green-compatible: can be used in ``greenlet`` or ``eventlet`` environment.
-
-While *queuelib* and *python-pqueue* cannot fulfil all of above. After some try, I found it's hard to achieve based on their current
-implementation without huge code change. this is the motivation to start this project.
-
-By default, *persist-queue* use *pickle* object serialization module to support object instances.
-Most built-in type, like `int`, `dict`, `list` are able to be persisted by `persist-queue` directly, to support customized objects,
-please refer to `Pickling and unpickling extension types(Python2) <https://docs.python.org/2/library/pickle.html#pickling-and-unpickling-normal-class-instances>`_
-and `Pickling Class Instances(Python3) <https://docs.python.org/3/library/pickle.html#pickling-class-instances>`_
-
-This project is based on the achievements of `python-pqueue <https://github.com/balena/python-pqueue>`_
-and `queuelib <https://github.com/scrapy/queuelib>`_
-
-Slack channels
-^^^^^^^^^^^^^^
-
-Join `persist-queue <https://join.slack
-.com/t/persist-queue/shared_invite
-/enQtOTM0MDgzNTQ0MDg3LTNmN2IzYjQ1MDc0MDYzMjI4OGJmNmVkNWE3ZDBjYzg5MDc0OWUzZDJkYTkwODdkZmYwODdjNjUzMTk3MWExNDE>`_ channel
-
-
-Requirements
-------------
-* Python 2.7 or Python 3.x (refer to `Deprecation`_ for future plan)
-* Full support for Linux.
-* Windows support (with `Caution`_ if ``persistqueue.Queue`` is used).
-
-Features
---------
-
-- Multiple platforms support: Linux, macOS, Windows
-- Pure python
-- Both filed based queues and sqlite3 based queues are supported
-- Filed based queue: multiple serialization protocol support: pickle(default), msgpack, json
-
-Deprecation
------------
-- `Python 3.4 release has reached end of life <https://www.python.org/downloads/release/python-3410/>`_ and
-  `DBUtils <https://webwareforpython.github.io/DBUtils/changelog.html>`_ ceased support for `Python 3.4`, `persist queue` drops the support for python 3.4 since version 0.8.0.
-  other queue implementations such as file based queue and sqlite3 based queue are still workable.
-- `Python 2 was sunset on January 1, 2020 <https://www.python.org/doc/sunset-python-2/>`_, `persist-queue` will drop any Python 2 support in future version `1.0.0`, no new feature will be developed under Python 2.
-
-Installation
-------------
-
-from pypi
-^^^^^^^^^
-
-.. code-block:: console
-
-    pip install persist-queue
-    # for msgpack and mysql support, use following command
-    pip install persist-queue[extra]
-
-
-from source code
-^^^^^^^^^^^^^^^^
-
-.. code-block:: console
-
-    git clone https://github.com/peter-wangxu/persist-queue
-    cd persist-queue
-    # for msgpack support, run 'pip install -r extra-requirements.txt' first
-    python setup.py install
-
-
-Benchmark
----------
-
-Here are the time spent(in seconds) for writing/reading **1000** items to the
-disk comparing the sqlite3 and file queue.
-
-- Windows
-    - OS: Windows 10
-    - Disk: SATA3 SSD
-    - RAM: 16 GiB
-
-+---------------+---------+-------------------------+----------------------------+
-|               | Write   | Write/Read(1 task_done) | Write/Read(many task_done) |
-+---------------+---------+-------------------------+----------------------------+
-| SQLite3 Queue | 1.8880  | 2.0290                  | 3.5940                     |
-+---------------+---------+-------------------------+----------------------------+
-| File Queue    | 4.9520  | 5.0560                  | 8.4900                     |
-+---------------+---------+-------------------------+----------------------------+
-
-**windows note**
-Performance of Windows File Queue has dramatic improvement since `v0.4.1` due to the
-atomic renaming support(3-4X faster)
-
-- Linux
-    - OS: Ubuntu 16.04 (VM)
-    - Disk: SATA3 SSD
-    - RAM:  4 GiB
-
-+---------------+--------+-------------------------+----------------------------+
-|               | Write  | Write/Read(1 task_done) | Write/Read(many task_done) |
-+---------------+--------+-------------------------+----------------------------+
-| SQLite3 Queue | 1.8282 | 1.8075                  | 2.8639                     |
-+---------------+--------+-------------------------+----------------------------+
-| File Queue    | 0.9123 | 1.0411                  | 2.5104                     |
-+---------------+--------+-------------------------+----------------------------+
-
-- Mac OS
-    - OS: 10.14 (macOS Mojave)
-    - Disk: PCIe SSD
-    - RAM:  16 GiB
-
-+---------------+--------+-------------------------+----------------------------+
-|               | Write  | Write/Read(1 task_done) | Write/Read(many task_done) |
-+---------------+--------+-------------------------+----------------------------+
-| SQLite3 Queue | 0.1879 | 0.2115                  | 0.3147                     |
-+---------------+--------+-------------------------+----------------------------+
-| File Queue    | 0.5158 | 0.5357                  | 1.0446                     |
-+---------------+--------+-------------------------+----------------------------+
-
-**note**
-
-- The value above is in seconds for reading/writing *1000* items, the less
-  the better
-- Above result was got from:
-
-.. code-block:: console
-
-    python benchmark/run_benchmark.py 1000
-
-
-To see the real performance on your host, run the script under ``benchmark/run_benchmark.py``:
-
-.. code-block:: console
-
-    python benchmark/run_benchmark.py <COUNT, default to 100>
-
-
-Examples
---------
-
-
-Example usage with a SQLite3 based queue
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code-block:: python
-
-    >>> import persistqueue
-    >>> q = persistqueue.SQLiteQueue('mypath', auto_commit=True)
-    >>> q.put('str1')
-    >>> q.put('str2')
-    >>> q.put('str3')
-    >>> q.get()
-    'str1'
-    >>> del q
-
-
-Close the console, and then recreate the queue:
-
-.. code-block:: python
-
-   >>> import persistqueue
-   >>> q = persistqueue.SQLiteQueue('mypath', auto_commit=True)
-   >>> q.get()
-   'str2'
-   >>>
-
-New functions:
-*Available since v0.8.0*
-
-- ``shrink_disk_usage`` perform a ``VACUUM`` against the sqlite, and rebuild the database file, this usually takes long time and frees a lot of disk space after ``get()``
-
-
-Example usage of SQLite3 based ``UniqueQ``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-This queue does not allow duplicate items.
-
-.. code-block:: python
-
-   >>> import persistqueue
-   >>> q = persistqueue.UniqueQ('mypath')
-   >>> q.put('str1')
-   >>> q.put('str1')
-   >>> q.size
-   1
-   >>> q.put('str2')
-   >>> q.size
-   2
-   >>>
-
-Example usage of SQLite3 based ``SQLiteAckQueue``/``UniqueAckQ``
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-The core functions:
-
-- ``put``: add item to the queue. Returns ``id``
-- ``get``: get item from queue and mark as unack.  Returns ``item``, Optional paramaters (``block``, ``timeout``, ``id``, ``next_in_order``, ``raw``)
-- ``update``: update an item. Returns ``id``, Paramaters (``item``), Optional parameter if item not in raw format (``id``)
-- ``ack``: mark item as acked. Returns ``id``, Parameters (``item`` or ``id``)
-- ``nack``: there might be something wrong with current consumer, so mark item as ready and new consumer will get it.  Returns ``id``, Parameters (``item`` or ``id``)
-- ``ack_failed``: there might be something wrong during process, so just mark item as failed. Returns ``id``, Parameters (``item`` or ``id``)
-- ``clear_acked_data``: perform a sql delete agaist sqlite. It removes 1000 items, while keeping 1000 of the most recent, whose status is ``AckStatus.acked`` (note: this does not shrink the file size on disk) Optional paramters (``max_delete``, ``keep_latest``, ``clear_ack_failed``)
-- ``shrink_disk_usage`` perform a ``VACUUM`` against the sqlite, and rebuild the database file, this usually takes long time and frees a lot of disk space after ``clear_acked_data``
-- ``queue``: returns the database contents as a Python List[Dict]
-- ``active_size``: The active size changes when an item is added (put) and completed (ack/ack_failed) unlike ``qsize`` which changes when an item is pulled (get) or returned (nack).
-
-.. code-block:: python
-
-   >>> import persistqueue
-   >>> ackq = persistqueue.SQLiteAckQueue('path')
-   >>> ackq.put('str1')
-   >>> item = ackq.get()
-   >>> # Do something with the item
-   >>> ackq.ack(item) # If done with the item
-   >>> ackq.nack(item) # Else mark item as `nack` so that it can be proceeded again by any worker
-   >>> ackq.ack_failed(item) # Or else mark item as `ack_failed` to discard this item
-
-Paramaters:
-
-- ``clear_acked_data``
-    - ``max_delete`` (defaults to 1000): This is the LIMIT.  How many items to delete.
-    - ``keep_latest`` (defaults to 1000): This is the OFFSET.  How many recent items to keep.
-    - ``clear_ack_failed`` (defaults to False): Clears the ``AckStatus.ack_failed`` in addition to the ``AckStatus.ack``.
-
-- ``get``
-    - ``raw`` (defaults to False): Returns the metadata along with the record, which includes the id (``pqid``) and timestamp.  On the SQLiteAckQueue, the raw results can be ack, nack, ack_failed similar to the normal return.
-    -  ``id`` (defaults to None): Accepts an `id` or a raw item containing ``pqid``.  Will select the item based on the row id.
-    -  ``next_in_order`` (defaults to False): Requires the ``id`` attribute.  This option tells the SQLiteAckQueue/UniqueAckQ to get the next item based on  ``id``, not the first available.  This allows the user to get, nack, get, nack and progress down the queue, instead of continuing to get the same nack'd item over again.
-
-``raw`` example:
-
-.. code-block:: python
-
-   >>> q.put('val1')
-   >>> d = q.get(raw=True)
-   >>> print(d)
-   >>> {'pqid': 1, 'data': 'val1', 'timestamp': 1616719225.012912}
-   >>> q.ack(d)
-
-``next_in_order`` example:
-
-.. code-block:: python
-
-   >>> q.put("val1")
-   >>> q.put("val2")
-   >>> q.put("val3")
-   >>> item = q.get()
-   >>> id = q.nack(item)
-   >>> item = q.get(id=id, next_in_order=True)
-   >>> print(item)
-   >>> val2
-
-
-Note:
-
-1. The SQLiteAckQueue always uses "auto_commit=True".
-2. The Queue could be set in non-block style, e.g. "SQLiteAckQueue.get(block=False, timeout=5)".
-3. ``UniqueAckQ`` only allows for unique items
-
-Example usage with a file based queue
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code-block:: python
-
-    >>> from persistqueue import Queue
-    >>> q = Queue("mypath")
-    >>> q.put('a')
-    >>> q.put('b')
-    >>> q.put('c')
-    >>> q.get()
-    'a'
-    >>> q.task_done()
-
-Close the python console, and then we restart the queue from the same path,
-
-.. code-block:: python
-
-    >>> from persistqueue import Queue
-    >>> q = Queue('mypath')
-    >>> q.get()
-    'b'
-    >>> q.task_done()
-
-Example usage with an auto-saving file based queue
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-*Available since: v0.5.0*
-
-By default, items added to the queue are persisted during the ``put()`` call,
-and items removed from a queue are only persisted when ``task_done()`` is
-called.
-
-.. code-block:: python
-
-    >>> from persistqueue import Queue
-    >>> q = Queue("mypath")
-    >>> q.put('a')
-    >>> q.put('b')
-    >>> q.get()
-    'a'
-    >>> q.get()
-    'b'
-
-After exiting and restarting the queue from the same path, we see the items
-remain in the queue, because ``task_done()`` wasn't called before.
-
-.. code-block:: python
-
-    >>> from persistqueue import Queue
-    >>> q = Queue('mypath')
-    >>> q.get()
-    'a'
-    >>> q.get()
-    'b'
-
-This can be advantageous. For example, if your program crashes before finishing
-processing an item, it will remain in the queue after restarting. You can also
-spread out the ``task_done()`` calls for performance reasons to avoid lots of
-individual writes.
-
-Using ``autosave=True`` on a file based queue will automatically save on every
-call to ``get()``. Calling ``task_done()`` is not necessary, but may still be
-used to ``join()`` against the queue.
-
-.. code-block:: python
-
-    >>> from persistqueue import Queue
-    >>> q = Queue("mypath", autosave=True)
-    >>> q.put('a')
-    >>> q.put('b')
-    >>> q.get()
-    'a'
-
-After exiting and restarting the queue from the same path, only the second item
-remains:
-
-.. code-block:: python
-
-    >>> from persistqueue import Queue
-    >>> q = Queue('mypath', autosave=True)
-    >>> q.get()
-    'b'
-
-
-Example usage with a SQLite3 based dict
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code-block:: python
-
-    >>> from persisitqueue import PDict
-    >>> q = PDict("testpath", "testname")
-    >>> q['key1'] = 123
-    >>> q['key2'] = 321
-    >>> q['key1']
-    123
-    >>> len(q)
-    2
-    >>> del q['key1']
-    >>> q['key1']
-    Traceback (most recent call last):
-      File "<stdin>", line 1, in <module>
-      File "persistqueue\pdict.py", line 58, in __getitem__
-        raise KeyError('Key: {} not exists.'.format(item))
-    KeyError: 'Key: key1 not exists.'
-
-Close the console and restart the PDict
-
-
-.. code-block:: python
-
-    >>> from persisitqueue import PDict
-    >>> q = PDict("testpath", "testname")
-    >>> q['key2']
-    321
-
-
-Multi-thread usage for **SQLite3** based queue
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code-block:: python
-
-    from persistqueue import FIFOSQLiteQueue
-
-    q = FIFOSQLiteQueue(path="./test", multithreading=True)
-
-    def worker():
-        while True:
-            item = q.get()
-            do_work(item)
-
-    for i in range(num_worker_threads):
-         t = Thread(target=worker)
-         t.daemon = True
-         t.start()
-
-    for item in source():
-        q.put(item)
-
-
-multi-thread usage for **Queue**
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code-block:: python
-
-    from persistqueue import Queue
-
-    q = Queue()
-
-    def worker():
-        while True:
-            item = q.get()
-            do_work(item)
-            q.task_done()
-
-    for i in range(num_worker_threads):
-         t = Thread(target=worker)
-         t.daemon = True
-         t.start()
-
-    for item in source():
-        q.put(item)
-
-    q.join()       # block until all tasks are done
-
-Example usage with a MySQL based queue
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-*Available since: v0.8.0*
-
-.. code-block:: python
-
-    >>> import persistqueue
-    >>> db_conf = {
-    >>>     "host": "127.0.0.1",
-    >>>     "user": "user",
-    >>>     "passwd": "passw0rd",
-    >>>     "db_name": "testqueue",
-    >>>     # "name": "",
-    >>>     "port": 3306
-    >>> }
-    >>> q = persistqueue.MySQLQueue(name="testtable", **db_conf)
-    >>> q.put('str1')
-    >>> q.put('str2')
-    >>> q.put('str3')
-    >>> q.get()
-    'str1'
-    >>> del q
-
-
-Close the console, and then recreate the queue:
-
-.. code-block:: python
-
-   >>> import persistqueue
-   >>> q = persistqueue.MySQLQueue(name="testtable", **db_conf)
-   >>> q.get()
-   'str2'
-   >>>
-
-
-
-**note**
-
-Due to the limitation of file queue described in issue `#89 <https://github.com/peter-wangxu/persist-queue/issues/89>`_,
-`task_done` in one thread may acknowledge items in other threads which should not be. Considering the `SQLiteAckQueue` if you have such requirement.
-
-
-Serialization via msgpack/json
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-- v0.4.1: Currently only available for file based Queue
-- v0.4.2: Also available for SQLite3 based Queues
-
-.. code-block:: python
-
-    >>> from persistqueue
-    >>> q = persistqueue.Queue('mypath', serializer=persistqueue.serializers.msgpack)
-    >>> # via json
-    >>> # q = Queue('mypath', serializer=persistqueue.serializers.json)
-    >>> q.get()
-    'b'
-    >>> q.task_done()
-
-Explicit resource reclaim
-^^^^^^^^^^^^^^^^^^^^^^^^^
-
-For some reasons, an application may require explicit reclamation for file
-handles or sql connections before end of execution. In these cases, user can
-simply call:
-.. code-block:: python
-
-    q = Queue() # or q = persistqueue.SQLiteQueue('mypath', auto_commit=True)
-    del q
-
-
-to reclaim related file handles or sql connections.
-
-Tips
-----
-
-``task_done`` is required both for file based queue and SQLite3 based queue (when ``auto_commit=False``)
-to persist the cursor of next ``get`` to the disk.
-
-
-Performance impact
-------------------
-
-- **WAL**
-
-  Starting on v0.3.2, the ``persistqueue`` is leveraging the sqlite3 builtin feature
-  `WAL <https://www.sqlite.org/wal.html>`_ which can improve the performance
-  significantly, a general testing indicates that ``persistqueue`` is 2-4 times
-  faster than previous version.
-
-- **auto_commit=False**
-
-  Since persistqueue v0.3.0, a new parameter ``auto_commit`` is introduced to tweak
-  the performance for sqlite3 based queues as needed. When specify ``auto_commit=False``, user
-  needs to perform ``queue.task_done()`` to persist the changes made to the disk since
-  last ``task_done`` invocation.
-
-- **pickle protocol selection**
-
-  From v0.3.6, the ``persistqueue`` will select ``Protocol version 2`` for python2 and ``Protocol version 4`` for python3
-  respectively. This selection only happens when the directory is not present when initializing the queue.
-
-Tests
------
-
-*persist-queue* use ``tox`` to trigger tests.
-
-- Unit test
-
-.. code-block:: console
-
-    tox -e <PYTHON_VERSION>
-
-Available ``<PYTHON_VERSION>``: ``py27``, ``py34``, ``py35``, ``py36``, ``py37``
-
-
-- PEP8 check
-
-.. code-block:: console
-
-   tox -e pep8
-
-
-`pyenv <https://github.com/pyenv/pyenv>`_ is usually a helpful tool to manage multiple versions of Python.
-
-Caution
--------
-
-Currently, the atomic operation is supported on Windows while still in experimental,
-That's saying, the data in ``persistqueue.Queue`` could be in unreadable state when an incidental failure occurs during ``Queue.task_done``.
-
-**DO NOT put any critical data on persistqueue.queue on Windows**.
-
-
-Contribution
-------------
-
-Simply fork this repo and send PR for your code change(also tests to cover your change), remember to give a title and description of your PR. I am willing to
-enhance this project with you :).
-
-
-License
--------
-
-`BSD <LICENSE>`_
-
-Contributors
-------------
-
-`Contributors <https://github.com/peter-wangxu/persist-queue/graphs/contributors>`_
-
-FAQ
----
-
-* ``sqlite3.OperationalError: database is locked`` is raised.
-
-persistqueue open 2 connections for the db if ``multithreading=True``, the
-SQLite database is locked until that transaction is committed. The ``timeout``
-parameter specifies how long the connection should wait for the lock to go away
-until raising an exception. Default time is **10**, increase ``timeout``
-when creating the queue if above error occurs.
-
-* sqlite3 based queues are not thread-safe.
-
-The sqlite3 queues are heavily tested under multi-threading environment, if you find it's not thread-safe, please
-make sure you set the ``multithreading=True`` when initializing the queue before submitting new issue:).
-
+Metadata-Version: 2.1
+Name: persist-queue
+Version: 0.8.1
+Summary: A thread-safe disk based persistent queue in Python.
+Home-page: http://github.com/peter-wangxu/persist-queue
+Author: Peter Wang
+Author-email: wangxu198709@gmail.com
+Maintainer: Peter Wang
+Maintainer-email: wangxu198709@gmail.com
+License: BSD
+Platform: all
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries
+Description-Content-Type: text/x-rst
+Provides-Extra: extra
+License-File: LICENSE
+
+persist-queue - A thread-safe, disk-based queue for Python
+==========================================================
+
+.. image:: https://img.shields.io/circleci/project/github/peter-wangxu/persist-queue/master.svg?label=Linux%20%26%20Mac
+    :target: https://circleci.com/gh/peter-wangxu/persist-queue
+
+.. image:: https://img.shields.io/appveyor/ci/peter-wangxu/persist-queue/master.svg?label=Windows
+    :target: https://ci.appveyor.com/project/peter-wangxu/persist-queue
+
+.. image:: https://img.shields.io/codecov/c/github/peter-wangxu/persist-queue/master.svg
+    :target: https://codecov.io/gh/peter-wangxu/persist-queue
+
+.. image:: https://img.shields.io/pypi/v/persist-queue.svg
+    :target: https://pypi.python.org/pypi/persist-queue
+
+``persist-queue`` implements a file-based queue and a serial of sqlite3-based queues. The goals is to achieve following requirements:
+
+* Disk-based: each queued item should be stored in disk in case of any crash.
+* Thread-safe: can be used by multi-threaded producers and multi-threaded consumers.
+* Recoverable: Items can be read after process restart.
+* Green-compatible: can be used in ``greenlet`` or ``eventlet`` environment.
+
+While *queuelib* and *python-pqueue* cannot fulfil all of above. After some try, I found it's hard to achieve based on their current
+implementation without huge code change. this is the motivation to start this project.
+
+By default, *persist-queue* use *pickle* object serialization module to support object instances.
+Most built-in type, like `int`, `dict`, `list` are able to be persisted by `persist-queue` directly, to support customized objects,
+please refer to `Pickling and unpickling extension types(Python2) <https://docs.python.org/2/library/pickle.html#pickling-and-unpickling-normal-class-instances>`_
+and `Pickling Class Instances(Python3) <https://docs.python.org/3/library/pickle.html#pickling-class-instances>`_
+
+This project is based on the achievements of `python-pqueue <https://github.com/balena/python-pqueue>`_
+and `queuelib <https://github.com/scrapy/queuelib>`_
+
+Slack channels
+^^^^^^^^^^^^^^
+
+Join `persist-queue <https://join.slack
+.com/t/persist-queue/shared_invite
+/enQtOTM0MDgzNTQ0MDg3LTNmN2IzYjQ1MDc0MDYzMjI4OGJmNmVkNWE3ZDBjYzg5MDc0OWUzZDJkYTkwODdkZmYwODdjNjUzMTk3MWExNDE>`_ channel
+
+
+Requirements
+------------
+* Python 2.7 or Python 3.x (refer to `Deprecation`_ for future plan)
+* Full support for Linux.
+* Windows support (with `Caution`_ if ``persistqueue.Queue`` is used).
+
+Features
+--------
+
+- Multiple platforms support: Linux, macOS, Windows
+- Pure python
+- Both filed based queues and sqlite3 based queues are supported
+- Filed based queue: multiple serialization protocol support: pickle(default), msgpack, cbor, json
+
+Deprecation
+-----------
+- `Python 3.4 release has reached end of life <https://www.python.org/downloads/release/python-3410/>`_ and
+  `DBUtils <https://webwareforpython.github.io/DBUtils/changelog.html>`_ ceased support for `Python 3.4`, `persist queue` drops the support for python 3.4 since version 0.8.0.
+  other queue implementations such as file based queue and sqlite3 based queue are still workable.
+- `Python 2 was sunset on January 1, 2020 <https://www.python.org/doc/sunset-python-2/>`_, `persist-queue` will drop any Python 2 support in future version `1.0.0`, no new feature will be developed under Python 2.
+
+Installation
+------------
+
+from pypi
+^^^^^^^^^
+
+.. code-block:: console
+
+    pip install persist-queue
+    # for msgpack, cbor and mysql support, use following command
+    pip install persist-queue[extra]
+
+
+from source code
+^^^^^^^^^^^^^^^^
+
+.. code-block:: console
+
+    git clone https://github.com/peter-wangxu/persist-queue
+    cd persist-queue
+    # for msgpack and cbor support, run 'pip install -r extra-requirements.txt' first
+    python setup.py install
+
+
+Benchmark
+---------
+
+Here are the time spent(in seconds) for writing/reading **1000** items to the
+disk comparing the sqlite3 and file queue.
+
+- Windows
+    - OS: Windows 10
+    - Disk: SATA3 SSD
+    - RAM: 16 GiB
+
++---------------+---------+-------------------------+----------------------------+
+|               | Write   | Write/Read(1 task_done) | Write/Read(many task_done) |
++---------------+---------+-------------------------+----------------------------+
+| SQLite3 Queue | 1.8880  | 2.0290                  | 3.5940                     |
++---------------+---------+-------------------------+----------------------------+
+| File Queue    | 4.9520  | 5.0560                  | 8.4900                     |
++---------------+---------+-------------------------+----------------------------+
+
+**windows note**
+Performance of Windows File Queue has dramatic improvement since `v0.4.1` due to the
+atomic renaming support(3-4X faster)
+
+- Linux
+    - OS: Ubuntu 16.04 (VM)
+    - Disk: SATA3 SSD
+    - RAM:  4 GiB
+
++---------------+--------+-------------------------+----------------------------+
+|               | Write  | Write/Read(1 task_done) | Write/Read(many task_done) |
++---------------+--------+-------------------------+----------------------------+
+| SQLite3 Queue | 1.8282 | 1.8075                  | 2.8639                     |
++---------------+--------+-------------------------+----------------------------+
+| File Queue    | 0.9123 | 1.0411                  | 2.5104                     |
++---------------+--------+-------------------------+----------------------------+
+
+- Mac OS
+    - OS: 10.14 (macOS Mojave)
+    - Disk: PCIe SSD
+    - RAM:  16 GiB
+
++---------------+--------+-------------------------+----------------------------+
+|               | Write  | Write/Read(1 task_done) | Write/Read(many task_done) |
++---------------+--------+-------------------------+----------------------------+
+| SQLite3 Queue | 0.1879 | 0.2115                  | 0.3147                     |
++---------------+--------+-------------------------+----------------------------+
+| File Queue    | 0.5158 | 0.5357                  | 1.0446                     |
++---------------+--------+-------------------------+----------------------------+
+
+**note**
+
+- The value above is in seconds for reading/writing *1000* items, the less
+  the better
+- Above result was got from:
+
+.. code-block:: console
+
+    python benchmark/run_benchmark.py 1000
+
+
+To see the real performance on your host, run the script under ``benchmark/run_benchmark.py``:
+
+.. code-block:: console
+
+    python benchmark/run_benchmark.py <COUNT, default to 100>
+
+
+Examples
+--------
+
+
+Example usage with a SQLite3 based queue
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: python
+
+    >>> import persistqueue
+    >>> q = persistqueue.SQLiteQueue('mypath', auto_commit=True)
+    >>> q.put('str1')
+    >>> q.put('str2')
+    >>> q.put('str3')
+    >>> q.get()
+    'str1'
+    >>> del q
+
+
+Close the console, and then recreate the queue:
+
+.. code-block:: python
+
+   >>> import persistqueue
+   >>> q = persistqueue.SQLiteQueue('mypath', auto_commit=True)
+   >>> q.get()
+   'str2'
+   >>>
+
+New functions:
+*Available since v0.8.0*
+
+- ``shrink_disk_usage`` perform a ``VACUUM`` against the sqlite, and rebuild the database file, this usually takes long time and frees a lot of disk space after ``get()``
+
+
+Example usage of SQLite3 based ``UniqueQ``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+This queue does not allow duplicate items.
+
+.. code-block:: python
+
+   >>> import persistqueue
+   >>> q = persistqueue.UniqueQ('mypath')
+   >>> q.put('str1')
+   >>> q.put('str1')
+   >>> q.size
+   1
+   >>> q.put('str2')
+   >>> q.size
+   2
+   >>>
+
+Example usage of SQLite3 based ``SQLiteAckQueue``/``UniqueAckQ``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+The core functions:
+
+- ``put``: add item to the queue. Returns ``id``
+- ``get``: get item from queue and mark as unack.  Returns ``item``, Optional paramaters (``block``, ``timeout``, ``id``, ``next_in_order``, ``raw``)
+- ``update``: update an item. Returns ``id``, Paramaters (``item``), Optional parameter if item not in raw format (``id``)
+- ``ack``: mark item as acked. Returns ``id``, Parameters (``item`` or ``id``)
+- ``nack``: there might be something wrong with current consumer, so mark item as ready and new consumer will get it.  Returns ``id``, Parameters (``item`` or ``id``)
+- ``ack_failed``: there might be something wrong during process, so just mark item as failed. Returns ``id``, Parameters (``item`` or ``id``)
+- ``clear_acked_data``: perform a sql delete agaist sqlite. It removes 1000 items, while keeping 1000 of the most recent, whose status is ``AckStatus.acked`` (note: this does not shrink the file size on disk) Optional paramters (``max_delete``, ``keep_latest``, ``clear_ack_failed``)
+- ``shrink_disk_usage`` perform a ``VACUUM`` against the sqlite, and rebuild the database file, this usually takes long time and frees a lot of disk space after ``clear_acked_data``
+- ``queue``: returns the database contents as a Python List[Dict]
+- ``active_size``: The active size changes when an item is added (put) and completed (ack/ack_failed) unlike ``qsize`` which changes when an item is pulled (get) or returned (nack).
+
+.. code-block:: python
+
+   >>> import persistqueue
+   >>> ackq = persistqueue.SQLiteAckQueue('path')
+   >>> ackq.put('str1')
+   >>> item = ackq.get()
+   >>> # Do something with the item
+   >>> ackq.ack(item) # If done with the item
+   >>> ackq.nack(item) # Else mark item as `nack` so that it can be proceeded again by any worker
+   >>> ackq.ack_failed(item) # Or else mark item as `ack_failed` to discard this item
+
+Parameters:
+
+- ``clear_acked_data``
+    - ``max_delete`` (defaults to 1000): This is the LIMIT.  How many items to delete.
+    - ``keep_latest`` (defaults to 1000): This is the OFFSET.  How many recent items to keep.
+    - ``clear_ack_failed`` (defaults to False): Clears the ``AckStatus.ack_failed`` in addition to the ``AckStatus.ack``.
+
+- ``get``
+    - ``raw`` (defaults to False): Returns the metadata along with the record, which includes the id (``pqid``) and timestamp.  On the SQLiteAckQueue, the raw results can be ack, nack, ack_failed similar to the normal return.
+    -  ``id`` (defaults to None): Accepts an `id` or a raw item containing ``pqid``.  Will select the item based on the row id.
+    -  ``next_in_order`` (defaults to False): Requires the ``id`` attribute.  This option tells the SQLiteAckQueue/UniqueAckQ to get the next item based on  ``id``, not the first available.  This allows the user to get, nack, get, nack and progress down the queue, instead of continuing to get the same nack'd item over again.
+
+``raw`` example:
+
+.. code-block:: python
+
+   >>> q.put('val1')
+   >>> d = q.get(raw=True)
+   >>> print(d)
+   >>> {'pqid': 1, 'data': 'val1', 'timestamp': 1616719225.012912}
+   >>> q.ack(d)
+
+``next_in_order`` example:
+
+.. code-block:: python
+
+   >>> q.put("val1")
+   >>> q.put("val2")
+   >>> q.put("val3")
+   >>> item = q.get()
+   >>> id = q.nack(item)
+   >>> item = q.get(id=id, next_in_order=True)
+   >>> print(item)
+   >>> val2
+
+
+Note:
+
+1. The SQLiteAckQueue always uses "auto_commit=True".
+2. The Queue could be set in non-block style, e.g. "SQLiteAckQueue.get(block=False, timeout=5)".
+3. ``UniqueAckQ`` only allows for unique items
+
+Example usage with a file based queue
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Parameters:
+
+- ``path``: specifies the directory wher enqueued data persisted.
+- ``maxsize``: indicates the maximum size stored in the queue, if maxsize<=0 the queue is unlimited.
+- ``chunksize``: indicates how many entries should exist in each chunk file on disk. When a all entries in a chunk file was dequeued by get(), the file would be removed from filesystem.
+- ``tempdir``: indicates where temporary files should be stored. The tempdir has to be located on the same disk as the enqueued data in order to obtain atomic operations.
+- ``serializer``: controls how enqueued data is serialized.
+- ``auto_save``: `True` or `False`. By default, the change is only persisted when task_done() is called. If autosave is enabled, info data is persisted immediately when get() is called. Adding data to the queue with put() will always persist immediately regardless of this setting.
+
+.. code-block:: python
+
+    >>> from persistqueue import Queue
+    >>> q = Queue("mypath")
+    >>> q.put('a')
+    >>> q.put('b')
+    >>> q.put('c')
+    >>> q.get()
+    'a'
+    >>> q.task_done()
+
+
+Close the python console, and then we restart the queue from the same path,
+
+.. code-block:: python
+
+    >>> from persistqueue import Queue
+    >>> q = Queue('mypath')
+    >>> q.get()
+    'b'
+    >>> q.task_done()
+
+Example usage with an auto-saving file based queue
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+*Available since: v0.5.0*
+
+By default, items added to the queue are persisted during the ``put()`` call,
+and items removed from a queue are only persisted when ``task_done()`` is
+called.
+
+.. code-block:: python
+
+    >>> from persistqueue import Queue
+    >>> q = Queue("mypath")
+    >>> q.put('a')
+    >>> q.put('b')
+    >>> q.get()
+    'a'
+    >>> q.get()
+    'b'
+
+After exiting and restarting the queue from the same path, we see the items
+remain in the queue, because ``task_done()`` wasn't called before.
+
+.. code-block:: python
+
+    >>> from persistqueue import Queue
+    >>> q = Queue('mypath')
+    >>> q.get()
+    'a'
+    >>> q.get()
+    'b'
+
+This can be advantageous. For example, if your program crashes before finishing
+processing an item, it will remain in the queue after restarting. You can also
+spread out the ``task_done()`` calls for performance reasons to avoid lots of
+individual writes.
+
+Using ``autosave=True`` on a file based queue will automatically save on every
+call to ``get()``. Calling ``task_done()`` is not necessary, but may still be
+used to ``join()`` against the queue.
+
+.. code-block:: python
+
+    >>> from persistqueue import Queue
+    >>> q = Queue("mypath", autosave=True)
+    >>> q.put('a')
+    >>> q.put('b')
+    >>> q.get()
+    'a'
+
+After exiting and restarting the queue from the same path, only the second item
+remains:
+
+.. code-block:: python
+
+    >>> from persistqueue import Queue
+    >>> q = Queue('mypath', autosave=True)
+    >>> q.get()
+    'b'
+
+
+Example usage with a SQLite3 based dict
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: python
+
+    >>> from persisitqueue import PDict
+    >>> q = PDict("testpath", "testname")
+    >>> q['key1'] = 123
+    >>> q['key2'] = 321
+    >>> q['key1']
+    123
+    >>> len(q)
+    2
+    >>> del q['key1']
+    >>> q['key1']
+    Traceback (most recent call last):
+      File "<stdin>", line 1, in <module>
+      File "persistqueue\pdict.py", line 58, in __getitem__
+        raise KeyError('Key: {} not exists.'.format(item))
+    KeyError: 'Key: key1 not exists.'
+
+Close the console and restart the PDict
+
+
+.. code-block:: python
+
+    >>> from persisitqueue import PDict
+    >>> q = PDict("testpath", "testname")
+    >>> q['key2']
+    321
+
+
+Multi-thread usage for **SQLite3** based queue
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: python
+
+    from persistqueue import FIFOSQLiteQueue
+
+    q = FIFOSQLiteQueue(path="./test", multithreading=True)
+
+    def worker():
+        while True:
+            item = q.get()
+            do_work(item)
+
+    for i in range(num_worker_threads):
+         t = Thread(target=worker)
+         t.daemon = True
+         t.start()
+
+    for item in source():
+        q.put(item)
+
+
+multi-thread usage for **Queue**
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code-block:: python
+
+    from persistqueue import Queue
+
+    q = Queue()
+
+    def worker():
+        while True:
+            item = q.get()
+            do_work(item)
+            q.task_done()
+
+    for i in range(num_worker_threads):
+         t = Thread(target=worker)
+         t.daemon = True
+         t.start()
+
+    for item in source():
+        q.put(item)
+
+    q.join()       # block until all tasks are done
+
+Example usage with a MySQL based queue
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+*Available since: v0.8.0*
+
+.. code-block:: python
+
+    >>> import persistqueue
+    >>> db_conf = {
+    >>>     "host": "127.0.0.1",
+    >>>     "user": "user",
+    >>>     "passwd": "passw0rd",
+    >>>     "db_name": "testqueue",
+    >>>     # "name": "",
+    >>>     "port": 3306
+    >>> }
+    >>> q = persistqueue.MySQLQueue(name="testtable", **db_conf)
+    >>> q.put('str1')
+    >>> q.put('str2')
+    >>> q.put('str3')
+    >>> q.get()
+    'str1'
+    >>> del q
+
+
+Close the console, and then recreate the queue:
+
+.. code-block:: python
+
+   >>> import persistqueue
+   >>> q = persistqueue.MySQLQueue(name="testtable", **db_conf)
+   >>> q.get()
+   'str2'
+   >>>
+
+
+
+**note**
+
+Due to the limitation of file queue described in issue `#89 <https://github.com/peter-wangxu/persist-queue/issues/89>`_,
+`task_done` in one thread may acknowledge items in other threads which should not be. Considering the `SQLiteAckQueue` if you have such requirement.
+
+
+Serialization via msgpack/cbor/json
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+- v0.4.1: Currently only available for file based Queue
+- v0.4.2: Also available for SQLite3 based Queues
+
+.. code-block:: python
+
+    >>> from persistqueue
+    >>> q = persistqueue.Queue('mypath', serializer=persistqueue.serializers.msgpack)
+    >>> # via cbor2
+    >>> # q = persistqueue.Queue('mypath', serializer=persistqueue.serializers.cbor2)
+    >>> # via json
+    >>> # q = Queue('mypath', serializer=persistqueue.serializers.json)
+    >>> q.get()
+    'b'
+    >>> q.task_done()
+
+Explicit resource reclaim
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+For some reasons, an application may require explicit reclamation for file
+handles or sql connections before end of execution. In these cases, user can
+simply call:
+.. code-block:: python
+
+    q = Queue() # or q = persistqueue.SQLiteQueue('mypath', auto_commit=True)
+    del q
+
+
+to reclaim related file handles or sql connections.
+
+Tips
+----
+
+``task_done`` is required both for file based queue and SQLite3 based queue (when ``auto_commit=False``)
+to persist the cursor of next ``get`` to the disk.
+
+
+Performance impact
+------------------
+
+- **WAL**
+
+  Starting on v0.3.2, the ``persistqueue`` is leveraging the sqlite3 builtin feature
+  `WAL <https://www.sqlite.org/wal.html>`_ which can improve the performance
+  significantly, a general testing indicates that ``persistqueue`` is 2-4 times
+  faster than previous version.
+
+- **auto_commit=False**
+
+  Since persistqueue v0.3.0, a new parameter ``auto_commit`` is introduced to tweak
+  the performance for sqlite3 based queues as needed. When specify ``auto_commit=False``, user
+  needs to perform ``queue.task_done()`` to persist the changes made to the disk since
+  last ``task_done`` invocation.
+
+- **pickle protocol selection**
+
+  From v0.3.6, the ``persistqueue`` will select ``Protocol version 2`` for python2 and ``Protocol version 4`` for python3
+  respectively. This selection only happens when the directory is not present when initializing the queue.
+
+Tests
+-----
+
+*persist-queue* use ``tox`` to trigger tests.
+
+- Unit test
+
+.. code-block:: console
+
+    tox -e <PYTHON_VERSION>
+
+Available ``<PYTHON_VERSION>``: ``py27``, ``py34``, ``py35``, ``py36``, ``py37``
+
+
+- PEP8 check
+
+.. code-block:: console
+
+   tox -e pep8
+
+
+`pyenv <https://github.com/pyenv/pyenv>`_ is usually a helpful tool to manage multiple versions of Python.
+
+Caution
+-------
+
+Currently, the atomic operation is supported on Windows while still in experimental,
+That's saying, the data in ``persistqueue.Queue`` could be in unreadable state when an incidental failure occurs during ``Queue.task_done``.
+
+**DO NOT put any critical data on persistqueue.queue on Windows**.
+
+
+Contribution
+------------
+
+Simply fork this repo and send PR for your code change(also tests to cover your change), remember to give a title and description of your PR. I am willing to
+enhance this project with you :).
+
+
+License
+-------
+
+`BSD <LICENSE>`_
+
+Contributors
+------------
+
+`Contributors <https://github.com/peter-wangxu/persist-queue/graphs/contributors>`_
+
+FAQ
+---
+
+* ``sqlite3.OperationalError: database is locked`` is raised.
+
+persistqueue open 2 connections for the db if ``multithreading=True``, the
+SQLite database is locked until that transaction is committed. The ``timeout``
+parameter specifies how long the connection should wait for the lock to go away
+until raising an exception. Default time is **10**, increase ``timeout``
+when creating the queue if above error occurs.
+
+* sqlite3 based queues are not thread-safe.
+
+The sqlite3 queues are heavily tested under multi-threading environment, if you find it's not thread-safe, please
+make sure you set the ``multithreading=True`` when initializing the queue before submitting new issue:).
```

### Comparing `persist-queue-0.8.0b0/persist_queue.egg-info/SOURCES.txt` & `persist-queue-0.8.1/persist_queue.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 persistqueue/mysqlqueue.py
 persistqueue/pdict.py
 persistqueue/queue.py
 persistqueue/sqlackqueue.py
 persistqueue/sqlbase.py
 persistqueue/sqlqueue.py
 persistqueue/serializers/__init__.py
+persistqueue/serializers/cbor2.py
 persistqueue/serializers/json.py
 persistqueue/serializers/msgpack.py
 persistqueue/serializers/pickle.py
 persistqueue/tests/__init__.py
 persistqueue/tests/test_mysqlqueue.py
 persistqueue/tests/test_pdict.py
 persistqueue/tests/test_queue.py
```

