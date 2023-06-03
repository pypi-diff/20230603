# Comparing `tmp/lesscode_database-0.0.2.tar.gz` & `tmp/lesscode_database-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_database-0.0.2.tar", last modified: Fri Jun  2 01:24:03 2023, max compression
+gzip compressed data, was "dist/lesscode_database-0.0.3.tar", last modified: Sat Jun  3 07:13:07 2023, max compression
```

## Comparing `lesscode_database-0.0.2.tar` & `lesscode_database-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/
--rw-r--r--   0 baai       (501) staff       (20)    11357 2023-06-01 01:18:51.000000 lesscode_database-0.0.2/LICENSE
--rw-r--r--   0 baai       (501) staff       (20)     6062 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)     5696 2023-06-02 01:23:39.000000 lesscode_database-0.0.2/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-01 01:20:17.000000 lesscode_database-0.0.2/lesscode_database/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)    23749 2023-06-02 00:50:57.000000 lesscode_database-0.0.2/lesscode_database/connect_pool.py
--rw-r--r--   0 baai       (501) staff       (20)     1109 2023-06-02 00:50:57.000000 lesscode_database-0.0.2/lesscode_database/connection_info.py
--rw-r--r--   0 baai       (501) staff       (20)     1900 2023-06-02 00:50:57.000000 lesscode_database-0.0.2/lesscode_database/options.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-06-02 01:23:39.000000 lesscode_database-0.0.2/lesscode_database/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)     6062 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      349 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       18 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/lesscode_database.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-06-02 01:24:03.000000 lesscode_database-0.0.2/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1194 2023-06-01 01:27:32.000000 lesscode_database-0.0.2/setup.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/
+-rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-06-01 13:04:22.000000 lesscode_database-0.0.3/LICENSE
+-rw-r--r--   0 navy      (1000) navy      (1000)     6933 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)     6567 2023-06-03 07:09:07.000000 lesscode_database-0.0.3/README.md
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database/
+-rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-06-01 13:04:45.000000 lesscode_database-0.0.3/lesscode_database/__init__.py
+-rw-r--r--   0 navy      (1000) navy      (1000)    26428 2023-06-03 06:57:13.000000 lesscode_database-0.0.3/lesscode_database/connect_pool.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     1194 2023-06-03 05:01:48.000000 lesscode_database-0.0.3/lesscode_database/connection_info.py
+-rw-r--r--   0 navy      (1000) navy      (1000)     1900 2023-06-01 13:32:42.000000 lesscode_database-0.0.3/lesscode_database/options.py
+-rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-06-03 07:10:39.000000 lesscode_database-0.0.3/lesscode_database/version.py
+drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/
+-rw-r--r--   0 navy      (1000) navy      (1000)     6933 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/PKG-INFO
+-rw-r--r--   0 navy      (1000) navy      (1000)      349 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/SOURCES.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/dependency_links.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       18 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/lesscode_database.egg-info/top_level.txt
+-rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-06-03 07:13:07.000000 lesscode_database-0.0.3/setup.cfg
+-rw-r--r--   0 navy      (1000) navy      (1000)     1194 2023-06-01 13:04:45.000000 lesscode_database-0.0.3/setup.py
```

### Comparing `lesscode_database-0.0.2/LICENSE` & `lesscode_database-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.2/PKG-INFO` & `lesscode_database-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,47 @@
-Metadata-Version: 2.1
-Name: lesscode_database
-Version: 0.0.2
-Summary: lesscode_database是数据库连接工具包
-Author: navysummer
-Author-email: navysummer@yeah.net
-Platform: python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # lesscode_database
 
 数据库连接工具包
 
 示例代码
+
 ```python
 import asyncio
 
 from sqlalchemy import MetaData, Table, Column, VARCHAR, INTEGER, select
-from sqlalchemy.orm import scoped_session, sessionmaker
+from sqlalchemy.ext.asyncio import async_sessionmaker
+from sqlalchemy.orm import sessionmaker
 
 from lesscode_database.connection_info import ConnectionInfo
 from lesscode_database.options import options
 
 options.conn_list = [
     ConnectionInfo(dialect="mysql", name="mysql", host="127.0.0.1", port=3306, user="root",
                    password="root", db_name="test", enable=True, params={"pool_recycle": 3600},
                    async_enable=True),
     ConnectionInfo(dialect="elasticsearch", name="es", host="127.0.0.1", port=9210, user="root",
                    password="root", enable=True, async_enable=True),
     ConnectionInfo(dialect="mongo", name="mongo", host="127.0.0.1", port=27027, user="root",
                    password="root", enable=True, async_enable=True),
-    ConnectionInfo(dialect="nebula3", name="nebula", host="127.0.0.1", port=9669, user="root",
+    ConnectionInfo(dialect="nebula", name="nebula", host="127.0.0.1", port=9669, user="root",
                    password="nebula", db_name="nebula", enable=True),
     ConnectionInfo(dialect="postgresql", host="127.0.0.1", port=5454, user="root", password="root",
                    db_name="root", enable=True, async_enable=True),
     ConnectionInfo(dialect="redis", name="redis", host="127.0.0.1", port=6379, user=None,
                    password=None, db_name=1, enable=True, async_enable=True),
     ConnectionInfo(dialect="sqlalchemy", name="sqlalchemy", host="127.0.0.1", port=3306, user="root",
                    password="root", db_name="test", enable=True, async_enable=True),
     ConnectionInfo(dialect="neo4j", name="neo4j", host="127.0.0.1", port=7687, user="neo4j",
                    password="neo4j", db_name=None, enable=True, async_enable=True),
+    ConnectionInfo(dialect="clickhouse", name="clickhouse", dsn="clickhouse://localhost", host="127.0.0.1", port=9000,
+                   user="default", password="", db_name='', enable=True, async_enable=False),
 
 ]
+# 获取数据库连接池的方式
+## options.name    name是ConnectionInfo的name，options.conn_list里所有的name不可重复
 
 # mysql 同步测试，async_enable=False
 with options.mysql.dedicated_connection() as conn:
     conn.ping(reconnect=True)
     with conn.cursor() as cursor:
         cursor.execute("select 1")
         description = cursor.description
@@ -106,21 +99,21 @@
     resp = await options.mongo.test.test.find_one()
     print(resp)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_mongo_test())
 
-# nebula3同步测试，async_enable=False
+# nebula同步测试，async_enable=False
 with options.nebula.session_context("root", "nebula") as session:
     session.execute(f'USE test')
     result = session.execute("match (t:Test) return t limit 1")
     print(result)
 
-# nebula3暂不支持异步
+# nebula暂不支持异步
 
 # postgresql同步测试，async_enable=False
 with options.postgresql.connection() as conn:
     with conn.cursor() as cursor:
         cursor.execute("select 1")
         rs = cursor.fetchone()
         print(rs)
@@ -154,26 +147,25 @@
 # sqlalchemy table
 meta = MetaData()
 t1 = Table("test", meta, Column("name", VARCHAR(collation='utf8mb3_bin', length=255)),
            Column(name='id', comment=None, nullable=False, autoincrement=False, primary_key=True, type_=INTEGER(),
                   server_default=None))
 
 # sqlalchemy同步测试，async_enable=False
-db_session = scoped_session(sessionmaker(bind=options.internal_capability))
-session = db_session()
-cur = session.execute(select(t1))
-print(cur.fetchall())
+with sessionmaker(bind=options.sqlalchemy)() as session:
+    cur = session.execute(select(t1))
+    print(cur.fetchall())
 
 
 # sqlalchemy异步测试，async_enable=True
 async def async_sqlalchemy_test():
-    async with options.internal_capability.connect() as conn:
-        result = await conn.execute(select(t1))
+    async with async_sessionmaker(options.sqlalchemy)() as session:
+        cur = await session.execute(select(t1))
 
-        print(result.fetchall())
+        print(cur.fetchall())
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_sqlalchemy_test())
 
 
 # neo4j同步测试
@@ -199,8 +191,27 @@
     async with options.neo4j.session(database="test") as session:
         await session.execute_read(query)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_neo4j_test())
 
+# clickhouse 同步测试
+with options.clickhouse as conn:
+    with conn.cursor() as cursor:
+        cursor.execute('SELECT 1')
+        print(cursor.fetchall())
+
+
+# clickhouse 异步测试测试
+async def async_clickhouse_test():
+    async with options.clickhouse.acquire() as conn:
+        async with conn.cursor() as cursor:
+            await cursor.execute("SELECT 1")
+            ret = await cursor.fetchone()
+            print(ret)
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(async_clickhouse_test())
+
 ```
```

### Comparing `lesscode_database-0.0.2/README.md` & `lesscode_database-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,60 @@
+Metadata-Version: 2.1
+Name: lesscode_database
+Version: 0.0.3
+Summary: lesscode_database是数据库连接工具包
+Author: navysummer
+Author-email: navysummer@yeah.net
+Platform: python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # lesscode_database
 
 数据库连接工具包
 
 示例代码
+
 ```python
 import asyncio
 
 from sqlalchemy import MetaData, Table, Column, VARCHAR, INTEGER, select
-from sqlalchemy.orm import scoped_session, sessionmaker
+from sqlalchemy.ext.asyncio import async_sessionmaker
+from sqlalchemy.orm import sessionmaker
 
 from lesscode_database.connection_info import ConnectionInfo
 from lesscode_database.options import options
 
 options.conn_list = [
     ConnectionInfo(dialect="mysql", name="mysql", host="127.0.0.1", port=3306, user="root",
                    password="root", db_name="test", enable=True, params={"pool_recycle": 3600},
                    async_enable=True),
     ConnectionInfo(dialect="elasticsearch", name="es", host="127.0.0.1", port=9210, user="root",
                    password="root", enable=True, async_enable=True),
     ConnectionInfo(dialect="mongo", name="mongo", host="127.0.0.1", port=27027, user="root",
                    password="root", enable=True, async_enable=True),
-    ConnectionInfo(dialect="nebula3", name="nebula", host="127.0.0.1", port=9669, user="root",
+    ConnectionInfo(dialect="nebula", name="nebula", host="127.0.0.1", port=9669, user="root",
                    password="nebula", db_name="nebula", enable=True),
     ConnectionInfo(dialect="postgresql", host="127.0.0.1", port=5454, user="root", password="root",
                    db_name="root", enable=True, async_enable=True),
     ConnectionInfo(dialect="redis", name="redis", host="127.0.0.1", port=6379, user=None,
                    password=None, db_name=1, enable=True, async_enable=True),
     ConnectionInfo(dialect="sqlalchemy", name="sqlalchemy", host="127.0.0.1", port=3306, user="root",
                    password="root", db_name="test", enable=True, async_enable=True),
     ConnectionInfo(dialect="neo4j", name="neo4j", host="127.0.0.1", port=7687, user="neo4j",
                    password="neo4j", db_name=None, enable=True, async_enable=True),
+    ConnectionInfo(dialect="clickhouse", name="clickhouse", dsn="clickhouse://localhost", host="127.0.0.1", port=9000,
+                   user="default", password="", db_name='', enable=True, async_enable=False),
 
 ]
+# 获取数据库连接池的方式
+## options.name    name是ConnectionInfo的name，options.conn_list里所有的name不可重复
 
 # mysql 同步测试，async_enable=False
 with options.mysql.dedicated_connection() as conn:
     conn.ping(reconnect=True)
     with conn.cursor() as cursor:
         cursor.execute("select 1")
         description = cursor.description
@@ -93,21 +112,21 @@
     resp = await options.mongo.test.test.find_one()
     print(resp)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_mongo_test())
 
-# nebula3同步测试，async_enable=False
+# nebula同步测试，async_enable=False
 with options.nebula.session_context("root", "nebula") as session:
     session.execute(f'USE test')
     result = session.execute("match (t:Test) return t limit 1")
     print(result)
 
-# nebula3暂不支持异步
+# nebula暂不支持异步
 
 # postgresql同步测试，async_enable=False
 with options.postgresql.connection() as conn:
     with conn.cursor() as cursor:
         cursor.execute("select 1")
         rs = cursor.fetchone()
         print(rs)
@@ -141,26 +160,25 @@
 # sqlalchemy table
 meta = MetaData()
 t1 = Table("test", meta, Column("name", VARCHAR(collation='utf8mb3_bin', length=255)),
            Column(name='id', comment=None, nullable=False, autoincrement=False, primary_key=True, type_=INTEGER(),
                   server_default=None))
 
 # sqlalchemy同步测试，async_enable=False
-db_session = scoped_session(sessionmaker(bind=options.internal_capability))
-session = db_session()
-cur = session.execute(select(t1))
-print(cur.fetchall())
+with sessionmaker(bind=options.sqlalchemy)() as session:
+    cur = session.execute(select(t1))
+    print(cur.fetchall())
 
 
 # sqlalchemy异步测试，async_enable=True
 async def async_sqlalchemy_test():
-    async with options.internal_capability.connect() as conn:
-        result = await conn.execute(select(t1))
+    async with async_sessionmaker(options.sqlalchemy)() as session:
+        cur = await session.execute(select(t1))
 
-        print(result.fetchall())
+        print(cur.fetchall())
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_sqlalchemy_test())
 
 
 # neo4j同步测试
@@ -186,8 +204,27 @@
     async with options.neo4j.session(database="test") as session:
         await session.execute_read(query)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_neo4j_test())
 
+# clickhouse 同步测试
+with options.clickhouse as conn:
+    with conn.cursor() as cursor:
+        cursor.execute('SELECT 1')
+        print(cursor.fetchall())
+
+
+# clickhouse 异步测试测试
+async def async_clickhouse_test():
+    async with options.clickhouse.acquire() as conn:
+        async with conn.cursor() as cursor:
+            await cursor.execute("SELECT 1")
+            ret = await cursor.fetchone()
+            print(ret)
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(async_clickhouse_test())
+
 ```
```

### Comparing `lesscode_database-0.0.2/lesscode_database/connect_pool.py` & `lesscode_database-0.0.3/lesscode_database/connect_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,106 +9,117 @@
 
 class Pool:
     """
     Elasticsearch 数据库链接创建类
     """
 
     @staticmethod
-    async def create_es_pool(conn_info):
+    async def create_es_pool(conn_info: ConnectionInfo):
         """
         创建elasticsearch 异步连接池
         :param conn_info: 连接对象信息
         :return:
         """
-
-        host_arr = conn_info.host.split(",")
-        protocol = "http"
-        if conn_info.params:
-            if conn_info.params.get('protocol', 'http'):
-                protocol = conn_info.params.get('protocol', 'http')
-        hosts = [f"{protocol}://{conn_info.user}:{conn_info.password}@{host}:{conn_info.port}" for host in host_arr]
+        if conn_info.dsn:
+            hosts = conn_info.dsn
+        else:
+            host_arr = conn_info.host.split(",")
+            protocol = "http"
+            if conn_info.params:
+                if conn_info.params.get('protocol', 'http'):
+                    protocol = conn_info.params.get('protocol', 'http')
+            hosts = [f"{protocol}://{conn_info.user}:{conn_info.password}@{host}:{conn_info.port}" for host in host_arr]
         try:
             elasticsearch = importlib.import_module("elasticsearch")
         except ImportError:
             raise Exception(f"elasticsearch is not exist,run:pip install elasticsearch[async]")
         pool = elasticsearch.AsyncElasticsearch(hosts=hosts)
         return pool
 
     @staticmethod
-    def sync_create_es_pool(conn_info):
+    def sync_create_es_pool(conn_info: ConnectionInfo):
         """
         创建elasticsearch 同步连接池
         :param conn_info: 连接对象信息
         :return:
         """
-        host_arr = conn_info.host.split(",")
-        protocol = "http"
-        if conn_info.params:
-            if conn_info.params.get('protocol', 'http'):
-                protocol = conn_info.params.get('protocol', 'http')
-        hosts = [f"{protocol}://{conn_info.user}:{conn_info.password}@{host}:{conn_info.port}" for host in host_arr]
+        if conn_info.dsn:
+            hosts = conn_info.dsn
+        else:
+            host_arr = conn_info.host.split(",")
+            protocol = "http"
+            if conn_info.params:
+                if conn_info.params.get('protocol', 'http'):
+                    protocol = conn_info.params.get('protocol', 'http')
+            hosts = [f"{protocol}://{conn_info.user}:{conn_info.password}@{host}:{conn_info.port}" for host in host_arr]
         try:
             elasticsearch = importlib.import_module("elasticsearch")
         except ImportError:
             raise Exception(f"elasticsearch is not exist,run:pip install elasticsearch")
         pool = elasticsearch.Elasticsearch(hosts)
         return pool
 
     @staticmethod
-    def create_mongo_pool(conn_info):
+    def create_mongo_pool(conn_info: ConnectionInfo):
         """
         创建mongodb 异步连接池
         :param conn_info: 连接信息
         :return:
         """
         try:
             motor_asyncio = importlib.import_module("motor.motor_asyncio")
         except ImportError:
             raise Exception(f"motor is not exist,run:pip install motor")
-        host_str = conn_info.host.split(",")
-        hosts = ",".join([f"{host}:{conn_info.port}" for host in host_str])
-        conn_info_string = f"mongodb://{conn_info.user}:{conn_info.password}@{hosts}"
-        if conn_info.params:
-            auth_type = conn_info.params.get("type")
-            if auth_type == "LDAP":
-                conn_info_string += "/?authMechanism=PLAIN"
-            elif auth_type == "Password":
-                conn_info_string += "/?authSource=admin"
-            elif auth_type == "X509":
-                conn_info_string += "/?authMechanism=MONGODB-X509"
-        pool = motor_asyncio.AsyncIOMotorClient(conn_info_string)
+        if conn_info.dsn:
+            uri = conn_info.dsn
+        else:
+            host_str = conn_info.host.split(",")
+            hosts = ",".join([f"{host}:{conn_info.port}" for host in host_str])
+            uri = f"mongodb://{conn_info.user}:{conn_info.password}@{hosts}"
+            if conn_info.params:
+                auth_type = conn_info.params.get("type")
+                if auth_type == "LDAP":
+                    uri += "/?authMechanism=PLAIN"
+                elif auth_type == "Password":
+                    uri += "/?authSource=admin"
+                elif auth_type == "X509":
+                    uri += "/?authMechanism=MONGODB-X509"
+        pool = motor_asyncio.AsyncIOMotorClient(uri)
         return pool
 
     @staticmethod
-    def sync_create_mongo_pool(conn_info):
+    def sync_create_mongo_pool(conn_info: ConnectionInfo):
         """
         创建mongodb 同步连接池
         :param conn_info: 连接信息
         :return:
         """
         try:
             pymongo = importlib.import_module("pymongo")
         except ImportError:
             raise Exception(f"pymongo is not exist,run:pip install pymongo")
-        host_str = conn_info.host.split(",")
-        hosts = ",".join([f"{host}:{conn_info.port}" for host in host_str])
-        conn_info_string = f"mongodb://{conn_info.user}:{conn_info.password}@{hosts}"
-        if conn_info.params:
-            auth_type = conn_info.params.get("type")
-            if auth_type == "LDAP":
-                conn_info_string += "/?authMechanism=PLAIN"
-            elif auth_type == "Password":
-                conn_info_string += "/?authSource=admin"
-            elif auth_type == "X509":
-                conn_info_string += "/?authMechanism=MONGODB-X509"
-        pool = pymongo.MongoClient(conn_info_string)
+        if conn_info.dsn:
+            uri = conn_info.dsn
+        else:
+            host_str = conn_info.host.split(",")
+            hosts = ",".join([f"{host}:{conn_info.port}" for host in host_str])
+            uri = f"mongodb://{conn_info.user}:{conn_info.password}@{hosts}"
+            if conn_info.params:
+                auth_type = conn_info.params.get("type")
+                if auth_type == "LDAP":
+                    uri += "/?authMechanism=PLAIN"
+                elif auth_type == "Password":
+                    uri += "/?authSource=admin"
+                elif auth_type == "X509":
+                    uri += "/?authMechanism=MONGODB-X509"
+        pool = pymongo.MongoClient(uri)
         return pool
 
     @staticmethod
-    async def create_mysql_pool(conn_info):
+    async def create_mysql_pool(conn_info: ConnectionInfo):
         """
         创建mysql 异步连接池
         :param conn_info: 连接信息
         :return:
         """
         try:
             aiomysql = importlib.import_module("aiomysql")
@@ -121,15 +132,15 @@
                                           if conn_info.params else 3600,
                                           db=conn_info.db_name, autocommit=True,
                                           minsize=conn_info.min_size,
                                           maxsize=conn_info.max_size)
         return pool
 
     @staticmethod
-    def sync_create_mysql_pool(conn_info):
+    def sync_create_mysql_pool(conn_info: ConnectionInfo):
         """
         创建mysql 同步连接池
         :param conn_info: 连接信息
         :return: 
         """
         try:
             pymysql = importlib.import_module("pymysql")
@@ -145,15 +156,15 @@
                                   mincached=conn_info.min_size, blocking=True, maxusage=conn_info.min_size,
                                   maxshared=conn_info.max_size, maxcached=conn_info.max_size,
                                   ping=1, maxconnections=conn_info.max_size, charset="utf8mb4", autocommit=True,
                                   read_timeout=30)
         return pool
 
     @staticmethod
-    def sync_create_nebula3_pool(conn_info):
+    def sync_create_nebula_pool(conn_info: ConnectionInfo):
         """
         创建nebula3连接池
         :param conn_info: 连接信息
         :return: 
         """
         try:
             nebula3_gclient_net = importlib.import_module("nebula3.gclient.net")
@@ -180,61 +191,67 @@
                 ssl_conf.certfile = ssl_config.get("certfile", None)
                 ssl_conf.allow_weak_ssl_versions = ssl_config.get("allow_weak_ssl_versions", None)
         pool = nebula3_gclient_net.ConnectionPool()
         pool.init([(conn_info.host, conn_info.port)], config, ssl_conf)
         return pool
 
     @staticmethod
-    async def create_neo4j_pool(conn_info):
+    async def create_neo4j_pool(conn_info: ConnectionInfo):
         """
         创建Neo4j异步连接池
         :param conn_info: 连接信息
         :return:
         """
         try:
             neo4j = importlib.import_module("neo4j")
         except ImportError:
             raise Exception(f"neo4j is not exist,run:pip install neo4j")
-        driver = neo4j.AsyncGraphDatabase.driver(f"bolt://{conn_info.host}:{conn_info.port}",
-                                                 auth=(conn_info.user, conn_info.password))
+        if conn_info.dsn:
+            uri = conn_info.dsn
+        else:
+            uri = f"bolt://{conn_info.host}:{conn_info.port}"
+        driver = neo4j.AsyncGraphDatabase.driver(uri, auth=(conn_info.user, conn_info.password))
         return driver
 
     @staticmethod
-    def sync_create_neo4j_pool(conn_info):
+    def sync_create_neo4j_pool(conn_info: ConnectionInfo):
         """
         创建Neo4j同步连接池
         :param conn_info: 连接信息
         :return:
         """
         try:
             neo4j = importlib.import_module("neo4j")
         except ImportError:
             raise Exception(f"neo4j is not exist,run:pip install neo4j")
-        driver = neo4j.GraphDatabase.driver(f"bolt://{conn_info.host}:{conn_info.port}",
-                                            auth=(conn_info.user, conn_info.password))
+        if conn_info.dsn:
+            uri = conn_info.dsn
+        else:
+            uri = f"bolt://{conn_info.host}:{conn_info.port}"
+        driver = neo4j.GraphDatabase.driver(uri, auth=(conn_info.user, conn_info.password))
         return driver
 
     @staticmethod
-    async def create_postgresql_pool(conn_info):
+    async def create_postgresql_pool(conn_info: ConnectionInfo):
         """
         创建postgresql 异步连接池
         :param conn_info: 连接信息
         :return: 
         """
         try:
             aiopg = importlib.import_module("aiopg")
         except ImportError:
             raise Exception(f"aiopg is not exist,run:pip install aiopg")
-        pool = await aiopg.create_pool(host=conn_info.host, port=conn_info.port, user=conn_info.user,
+        pool = await aiopg.create_pool(dsn=conn_info.dsn, host=conn_info.host, port=conn_info.port, user=conn_info.user,
                                        password=conn_info.password,
                                        database=conn_info.db_name)
         return pool
 
     @staticmethod
-    def sync_create_postgresql_pool(conn_info):
+    def sync_create_postgresql_pool(conn_info: ConnectionInfo):
         """
         创建postgresql 同步连接池
         :param conn_info: 连接信息
         :return: 
         """
         try:
             psycopg2 = importlib.import_module("psycopg2")
@@ -246,47 +263,51 @@
             raise Exception(f"DBUtils is not exist,run:pip install DBUtils")
         pool = pooled_db.PooledDB(psycopg2, host=conn_info.host, port=conn_info.port,
                                   user=conn_info.user,
                                   password=conn_info.password, database=conn_info.db_name)
         return pool
 
     @staticmethod
-    def create_redis_pool(conn_info):
+    def create_redis_pool(conn_info: ConnectionInfo):
         """
         创建redis异步连接池
         :param conn_info: 连接信息
         :return:
         """
         try:
             aioredis = importlib.import_module("aioredis")
         except ImportError:
             raise Exception(f"aioredis is not exist,run:pip install aioredis")
-        pool = aioredis.ConnectionPool.from_url(f"redis://{conn_info.host}", port=conn_info.port,
-                                                password=conn_info.password,
+        if not conn_info.dsn:
+            conn_info.dsn = "redis://"
+        pool = aioredis.ConnectionPool.from_url(url=conn_info.dsn, host=conn_info.host, port=conn_info.port,
+                                                username=conn_info.user, password=conn_info.password,
                                                 db=conn_info.db_name, encoding="utf-8", decode_responses=True)
         return aioredis.Redis(connection_pool=pool, decode_responses=True)
 
     @staticmethod
-    def sync_create_redis_pool(conn_info):
+    def sync_create_redis_pool(conn_info: ConnectionInfo):
         """
         创建redis同步连接池
         :param conn_info:连接信息
         :return:
         """
         try:
             redis = importlib.import_module("redis")
         except ImportError:
             raise Exception(f"redis is not exist,run:pip install redis")
-        pool = redis.ConnectionPool.from_url(f"redis://{conn_info.host}", port=conn_info.port,
-                                             password=conn_info.password,
+        if not conn_info.dsn:
+            conn_info.dsn = "redis://"
+        pool = redis.ConnectionPool.from_url(url=conn_info.dsn, host=conn_info.host, port=conn_info.port,
+                                             username=conn_info.user, password=conn_info.password,
                                              db=conn_info.db_name, encoding="utf-8", decode_responses=True)
         return redis.Redis(connection_pool=pool, decode_responses=True)
 
     @staticmethod
-    async def create_redis_cluster_pool(conn_info):
+    async def create_redis_cluster_pool(conn_info: ConnectionInfo):
         """
         创建redis cluster异步连接池
         :param conn_info:连接信息
         :return:
         """
         try:
             aioredis_cluster = importlib.import_module("aioredis_cluster")
@@ -301,15 +322,15 @@
         idle_connection_timeout = params.get("idle_connection_timeout")
         username = params.get("username")
         password = conn_info.password
         encoding = params.get("encoding")
         connect_timeout = params.get("connect_timeout")
         attempt_timeout = params.get("attempt_timeout")
         ssl_info = params.get("ssl")
-        pool = await aioredis_cluster.create_redis_cluster(startup_nodes=conn_info.host,
+        pool = await aioredis_cluster.create_redis_cluster(startup_nodes=conn_info.dsn,
                                                            retry_min_delay=retry_min_delay,
                                                            retry_max_delay=retry_max_delay,
                                                            max_attempts=max_attempts,
                                                            state_reload_interval=state_reload_interval,
                                                            follow_cluster=follow_cluster,
                                                            idle_connection_timeout=idle_connection_timeout,
                                                            username=username,
@@ -319,15 +340,15 @@
                                                            pool_maxsize=conn_info.max_size,
                                                            connect_timeout=connect_timeout,
                                                            attempt_timeout=attempt_timeout,
                                                            ssl=ssl_info)
         return pool
 
     @staticmethod
-    def sync_create_redis_cluster_pool(conn_info):
+    def sync_create_redis_cluster_pool(conn_info: ConnectionInfo):
         """
         创建redis cluster同步连接池
         :param conn_info:连接信息
         :return:
         """
         try:
             rediscluster = importlib.import_module("rediscluster")
@@ -340,52 +361,78 @@
 
         skip_full_coverage_check = params.get("skip_full_coverage_check",
                                               False) if params else False
         nodemanager_follow_cluster = params.get("nodemanager_follow_cluster",
                                                 False) if params else False
         host_port_remap = params.get("nodemanager_follow_cluster",
                                      None) if params else None
-        pool = rediscluster.ClusterConnectionPool(startup_nodes=conn_info.host, init_slot_cache=init_slot_cache,
+        pool = rediscluster.ClusterConnectionPool(startup_nodes=conn_info.dsn, init_slot_cache=init_slot_cache,
                                                   max_connections=conn_info.max_size,
                                                   max_connections_per_node=max_connections_per_node,
                                                   skip_full_coverage_check=skip_full_coverage_check,
                                                   nodemanager_follow_cluster=nodemanager_follow_cluster,
                                                   host_port_remap=host_port_remap, db=conn_info.db_name,
                                                   username=conn_info.user, password=conn_info.password)
         return pool
 
     @staticmethod
-    def create_sqlalchemy_pool(conn_info):
+    async def create_clickhouse_pool(conn_info: ConnectionInfo):
+        try:
+            asynch = importlib.import_module("asynch")
+        except ImportError:
+            raise Exception(f"asynch is not exist,run:pip install asynch")
+        pool = await asynch.create_pool(minsize=conn_info.min_size, maxsize=conn_info.max_size,
+                                        dsn=conn_info.dsn, host=conn_info.host,
+                                        user=conn_info.user, password=conn_info.password,
+                                        port=conn_info.port, database=conn_info.db_name)
+        return pool
+
+    @staticmethod
+    def sync_create_clickhouse_pool(conn_info: ConnectionInfo):
+        try:
+            clickhouse_driver_dbapi = importlib.import_module("clickhouse_driver.dbapi")
+        except ImportError:
+            raise Exception(f"clickhouse-driver is not exist,run:pip install clickhouse-driver")
+        con = clickhouse_driver_dbapi.connect(dsn=conn_info.dsn, host=conn_info.host,
+                                              user=conn_info.user, password=conn_info.password,
+                                              port=conn_info.port, database=conn_info.db_name)
+        return con
+
+    @staticmethod
+    def create_sqlalchemy_pool(conn_info: ConnectionInfo):
         """
         创建sqlalchemy同步连接池
         :param conn_info: 连接信息
         :return:
         """
-        db_type = "mysql"
-        if conn_info.params:
-            if conn_info.params.get("db_type"):
-                db_type = conn_info.params.pop("db_type")
-        if db_type == "mysql":
-            url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
-        elif db_type == "postgresql":
-            url = 'postgresql+aiopg://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
-        elif db_type == "tidb":
-            url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
-        elif db_type == "ocean_base":
-            url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
+        if conn_info.dsn:
+            url = conn_info.dsn
         else:
-            raise Exception("UNSUPPORTED DB TYPE")
+            db_type = "mysql"
+            if conn_info.params:
+                if conn_info.params.get("db_type"):
+                    db_type = conn_info.params.pop("db_type")
+            if db_type == "mysql":
+                url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "postgresql":
+                url = 'postgresql+aiopg://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "tidb":
+                url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "ocean_base":
+                url = 'mysql+aiomysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            else:
+                raise Exception("UNSUPPORTED DB TYPE")
         try:
             sqlalchemy = importlib.import_module("sqlalchemy.ext.asyncio")
         except ImportError:
             raise Exception(f"sqlalchemy is not exist,run:pip install sqlalchemy")
         engine = sqlalchemy.create_async_engine(url, echo=conn_info.params.get("echo",
                                                                                True) if conn_info.params else True,
                                                 pool_size=conn_info.min_size,
@@ -396,42 +443,45 @@
                                                 pool_timeout=conn_info.params.get("pool_timeout",
                                                                                   10) if conn_info.params else 10,
                                                 pool_pre_ping=conn_info.params.get("pool_pre_ping",
                                                                                    True) if conn_info.params else True)
         return engine
 
     @staticmethod
-    def sync_create_sqlalchemy_pool(conn_info):
+    def sync_create_sqlalchemy_pool(conn_info: ConnectionInfo):
         """
         创建sqlalchemy同步连接池
         :param conn_info: 连接信息
         :return:
         """
-        db_type = "mysql"
-        if conn_info.params:
-            if conn_info.params.get("db_type"):
-                db_type = conn_info.params.pop("db_type")
-        if db_type == "mysql":
-            url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
-        elif db_type == "postgresql":
-            url = 'postgresql+psycopg2://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
-        elif db_type == "tidb":
-            url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
-        elif db_type == "ocean_base":
-            url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
-                conn_info.user, conn_info.password, conn_info.host, conn_info.port,
-                conn_info.db_name)
+        if conn_info.dsn:
+            url = conn_info.dsn
         else:
-            raise Exception("UNSUPPORTED DB TYPE")
+            db_type = "mysql"
+            if conn_info.params:
+                if conn_info.params.get("db_type"):
+                    db_type = conn_info.params.pop("db_type")
+            if db_type == "mysql":
+                url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "postgresql":
+                url = 'postgresql+psycopg2://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "tidb":
+                url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            elif db_type == "ocean_base":
+                url = 'mysql+pymysql://{}:{}@{}:{}/{}?charset=utf8mb4'.format(
+                    conn_info.user, conn_info.password, conn_info.host, conn_info.port,
+                    conn_info.db_name)
+            else:
+                raise Exception("UNSUPPORTED DB TYPE")
         try:
             sqlalchemy = importlib.import_module("sqlalchemy")
         except ImportError:
             raise Exception(f"sqlalchemy is not exist,run:pip install sqlalchemy")
         engine = sqlalchemy.create_engine(url, echo=conn_info.params.get("echo",
                                                                          True) if conn_info.params else True,
                                           pool_size=conn_info.min_size,
@@ -471,16 +521,16 @@
 
     elif conn_info.dialect == "mysql":
         if conn_info.async_enable:
             return run_sync(Pool.create_mysql_pool(conn_info))
         else:
             return run_sync(Pool.sync_create_mysql_pool(conn_info))
 
-    elif conn_info.dialect == "nebula3":
-        return run_sync(Pool.sync_create_nebula3_pool(conn_info))
+    elif conn_info.dialect == "nebula":
+        return run_sync(Pool.sync_create_nebula_pool(conn_info))
 
     elif conn_info.dialect == "neo4j":
         if conn_info.async_enable:
             return run_sync(Pool.create_neo4j_pool(conn_info))
         else:
             return run_sync(Pool.sync_create_neo4j_pool(conn_info))
 
@@ -498,14 +548,20 @@
 
     elif conn_info.dialect == "redis_cluster":
         if conn_info.async_enable:
             return run_sync(Pool.create_redis_cluster_pool(conn_info))
         else:
             return run_sync(Pool.sync_create_redis_cluster_pool(conn_info))
 
+    elif conn_info.dialect == "clickhouse":
+        if conn_info.async_enable:
+            return run_sync(Pool.create_clickhouse_pool(conn_info))
+        else:
+            return run_sync(Pool.sync_create_clickhouse_pool(conn_info))
+
     elif conn_info.dialect == "sqlalchemy":
         if conn_info.async_enable:
             return run_sync(Pool.create_sqlalchemy_pool(conn_info))
         else:
             return run_sync(Pool.sync_create_sqlalchemy_pool(conn_info))
 
     else:
```

### Comparing `lesscode_database-0.0.2/lesscode_database/connection_info.py` & `lesscode_database-0.0.3/lesscode_database/connection_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,27 @@
 
 
 class ConnectionInfo:
     """
     数据库连接信息对象
     """
 
-    def __init__(self, dialect: str, host: str, port: int, user: str = None, password: str = None,
+    def __init__(self, dialect: str, dsn: str = None, host: str = None, port: int = None, user: str = None,
+                 password: str = None,
                  db_name: Any = None, name: str = None, params: dict = None, min_size: int = 3, max_size: int = 10,
                  enable: bool = True, async_enable: bool = False):
         # 数据库dialect类型
         self.dialect = dialect
         # 连接池名称
         if name:
             self.name = name
         else:
             self.name = dialect
+        # dsn
+        self.dsn = dsn
         # 主机地址
         self.host = host
         # 端口号
         self.port = port
         # 用户名
         self.user = user
         # 密码
```

### Comparing `lesscode_database-0.0.2/lesscode_database/options.py` & `lesscode_database-0.0.3/lesscode_database/options.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.2/lesscode_database.egg-info/PKG-INFO` & `lesscode_database-0.0.3/lesscode_database.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesscode-database
-Version: 0.0.2
+Version: 0.0.3
 Summary: lesscode_database是数据库连接工具包
 Author: navysummer
 Author-email: navysummer@yeah.net
 Platform: python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -12,43 +12,49 @@
 License-File: LICENSE
 
 # lesscode_database
 
 数据库连接工具包
 
 示例代码
+
 ```python
 import asyncio
 
 from sqlalchemy import MetaData, Table, Column, VARCHAR, INTEGER, select
-from sqlalchemy.orm import scoped_session, sessionmaker
+from sqlalchemy.ext.asyncio import async_sessionmaker
+from sqlalchemy.orm import sessionmaker
 
 from lesscode_database.connection_info import ConnectionInfo
 from lesscode_database.options import options
 
 options.conn_list = [
     ConnectionInfo(dialect="mysql", name="mysql", host="127.0.0.1", port=3306, user="root",
                    password="root", db_name="test", enable=True, params={"pool_recycle": 3600},
                    async_enable=True),
     ConnectionInfo(dialect="elasticsearch", name="es", host="127.0.0.1", port=9210, user="root",
                    password="root", enable=True, async_enable=True),
     ConnectionInfo(dialect="mongo", name="mongo", host="127.0.0.1", port=27027, user="root",
                    password="root", enable=True, async_enable=True),
-    ConnectionInfo(dialect="nebula3", name="nebula", host="127.0.0.1", port=9669, user="root",
+    ConnectionInfo(dialect="nebula", name="nebula", host="127.0.0.1", port=9669, user="root",
                    password="nebula", db_name="nebula", enable=True),
     ConnectionInfo(dialect="postgresql", host="127.0.0.1", port=5454, user="root", password="root",
                    db_name="root", enable=True, async_enable=True),
     ConnectionInfo(dialect="redis", name="redis", host="127.0.0.1", port=6379, user=None,
                    password=None, db_name=1, enable=True, async_enable=True),
     ConnectionInfo(dialect="sqlalchemy", name="sqlalchemy", host="127.0.0.1", port=3306, user="root",
                    password="root", db_name="test", enable=True, async_enable=True),
     ConnectionInfo(dialect="neo4j", name="neo4j", host="127.0.0.1", port=7687, user="neo4j",
                    password="neo4j", db_name=None, enable=True, async_enable=True),
+    ConnectionInfo(dialect="clickhouse", name="clickhouse", dsn="clickhouse://localhost", host="127.0.0.1", port=9000,
+                   user="default", password="", db_name='', enable=True, async_enable=False),
 
 ]
+# 获取数据库连接池的方式
+## options.name    name是ConnectionInfo的name，options.conn_list里所有的name不可重复
 
 # mysql 同步测试，async_enable=False
 with options.mysql.dedicated_connection() as conn:
     conn.ping(reconnect=True)
     with conn.cursor() as cursor:
         cursor.execute("select 1")
         description = cursor.description
@@ -106,21 +112,21 @@
     resp = await options.mongo.test.test.find_one()
     print(resp)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_mongo_test())
 
-# nebula3同步测试，async_enable=False
+# nebula同步测试，async_enable=False
 with options.nebula.session_context("root", "nebula") as session:
     session.execute(f'USE test')
     result = session.execute("match (t:Test) return t limit 1")
     print(result)
 
-# nebula3暂不支持异步
+# nebula暂不支持异步
 
 # postgresql同步测试，async_enable=False
 with options.postgresql.connection() as conn:
     with conn.cursor() as cursor:
         cursor.execute("select 1")
         rs = cursor.fetchone()
         print(rs)
@@ -154,26 +160,25 @@
 # sqlalchemy table
 meta = MetaData()
 t1 = Table("test", meta, Column("name", VARCHAR(collation='utf8mb3_bin', length=255)),
            Column(name='id', comment=None, nullable=False, autoincrement=False, primary_key=True, type_=INTEGER(),
                   server_default=None))
 
 # sqlalchemy同步测试，async_enable=False
-db_session = scoped_session(sessionmaker(bind=options.internal_capability))
-session = db_session()
-cur = session.execute(select(t1))
-print(cur.fetchall())
+with sessionmaker(bind=options.sqlalchemy)() as session:
+    cur = session.execute(select(t1))
+    print(cur.fetchall())
 
 
 # sqlalchemy异步测试，async_enable=True
 async def async_sqlalchemy_test():
-    async with options.internal_capability.connect() as conn:
-        result = await conn.execute(select(t1))
+    async with async_sessionmaker(options.sqlalchemy)() as session:
+        cur = await session.execute(select(t1))
 
-        print(result.fetchall())
+        print(cur.fetchall())
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_sqlalchemy_test())
 
 
 # neo4j同步测试
@@ -199,8 +204,27 @@
     async with options.neo4j.session(database="test") as session:
         await session.execute_read(query)
 
 
 loop = asyncio.get_event_loop()
 loop.run_until_complete(async_neo4j_test())
 
+# clickhouse 同步测试
+with options.clickhouse as conn:
+    with conn.cursor() as cursor:
+        cursor.execute('SELECT 1')
+        print(cursor.fetchall())
+
+
+# clickhouse 异步测试测试
+async def async_clickhouse_test():
+    async with options.clickhouse.acquire() as conn:
+        async with conn.cursor() as cursor:
+            await cursor.execute("SELECT 1")
+            ret = await cursor.fetchone()
+            print(ret)
+
+
+loop = asyncio.get_event_loop()
+loop.run_until_complete(async_clickhouse_test())
+
 ```
```

### Comparing `lesscode_database-0.0.2/setup.py` & `lesscode_database-0.0.3/setup.py`

 * *Files identical despite different names*

