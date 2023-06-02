# Comparing `tmp/datajoint-0.8.2.tar.gz` & `tmp/datajoint-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datajoint-0.8.2.tar", last modified: Wed Oct 25 16:26:26 2017, max compression
+gzip compressed data, was "dist/datajoint-0.9.0.tar", last modified: Wed Nov 15 17:36:06 2017, max compression
```

## Comparing `datajoint-0.8.2.tar` & `datajoint-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 eywalker   (501) staff       (20)        0 2017-10-25 16:26:26.000000 datajoint-0.8.2/
-drwxr-xr-x   0 eywalker   (501) staff       (20)        0 2017-10-25 16:26:26.000000 datajoint-0.8.2/datajoint/
--rw-r--r--   0 eywalker   (501) staff       (20)     3260 2017-10-24 02:19:05.000000 datajoint-0.8.2/datajoint/__init__.py
--rw-r--r--   0 eywalker   (501) staff       (20)     2252 2017-07-27 02:20:07.000000 datajoint-0.8.2/datajoint/admin.py
--rw-r--r--   0 eywalker   (501) staff       (20)     6841 2017-07-27 02:20:07.000000 datajoint-0.8.2/datajoint/autopopulate.py
--rw-r--r--   0 eywalker   (501) staff       (20)    29129 2017-10-24 17:29:24.000000 datajoint-0.8.2/datajoint/base_relation.py
--rw-r--r--   0 eywalker   (501) staff       (20)     9600 2017-07-27 02:19:45.000000 datajoint-0.8.2/datajoint/blob.py
--rw-r--r--   0 eywalker   (501) staff       (20)     7803 2017-10-24 03:09:54.000000 datajoint-0.8.2/datajoint/connection.py
--rw-r--r--   0 eywalker   (501) staff       (20)     8341 2017-10-24 02:19:05.000000 datajoint-0.8.2/datajoint/declare.py
--rw-r--r--   0 eywalker   (501) staff       (20)     6091 2017-10-24 02:19:05.000000 datajoint-0.8.2/datajoint/dependencies.py
--rw-r--r--   0 eywalker   (501) staff       (20)    12580 2017-07-28 03:12:48.000000 datajoint-0.8.2/datajoint/erd.py
--rw-r--r--   0 eywalker   (501) staff       (20)    13512 2017-07-27 02:20:07.000000 datajoint-0.8.2/datajoint/fetch.py
--rw-r--r--   0 eywalker   (501) staff       (20)      887 2017-07-27 02:20:07.000000 datajoint-0.8.2/datajoint/hash.py
--rw-r--r--   0 eywalker   (501) staff       (20)    11683 2017-07-27 02:19:45.000000 datajoint-0.8.2/datajoint/heading.py
--rw-r--r--   0 eywalker   (501) staff       (20)     4916 2017-10-24 04:39:47.000000 datajoint-0.8.2/datajoint/jobs.py
--rw-r--r--   0 eywalker   (501) staff       (20)    33968 2017-10-24 02:19:05.000000 datajoint-0.8.2/datajoint/relational_operand.py
--rw-r--r--   0 eywalker   (501) staff       (20)     4939 2017-10-24 02:19:05.000000 datajoint-0.8.2/datajoint/s3.py
--rw-r--r--   0 eywalker   (501) staff       (20)     9635 2017-10-24 02:19:05.000000 datajoint-0.8.2/datajoint/schema.py
--rw-r--r--   0 eywalker   (501) staff       (20)     5542 2017-10-24 04:02:43.000000 datajoint-0.8.2/datajoint/settings.py
--rw-r--r--   0 eywalker   (501) staff       (20)     5183 2017-10-24 02:19:05.000000 datajoint-0.8.2/datajoint/user_relations.py
--rw-r--r--   0 eywalker   (501) staff       (20)     1827 2017-07-27 02:19:45.000000 datajoint-0.8.2/datajoint/utils.py
--rw-r--r--   0 eywalker   (501) staff       (20)       22 2017-10-24 17:26:12.000000 datajoint-0.8.2/datajoint/version.py
-drwxr-xr-x   0 eywalker   (501) staff       (20)        0 2017-10-25 16:26:26.000000 datajoint-0.8.2/datajoint.egg-info/
--rw-r--r--   0 eywalker   (501) staff       (20)        1 2017-10-25 16:26:26.000000 datajoint-0.8.2/datajoint.egg-info/dependency_links.txt
--rw-r--r--   0 eywalker   (501) staff       (20)      428 2017-10-25 16:26:26.000000 datajoint-0.8.2/datajoint.egg-info/PKG-INFO
--rw-r--r--   0 eywalker   (501) staff       (20)       70 2017-10-25 16:26:26.000000 datajoint-0.8.2/datajoint.egg-info/requires.txt
--rw-r--r--   0 eywalker   (501) staff       (20)      669 2017-10-25 16:26:26.000000 datajoint-0.8.2/datajoint.egg-info/SOURCES.txt
--rw-r--r--   0 eywalker   (501) staff       (20)       10 2017-10-25 16:26:26.000000 datajoint-0.8.2/datajoint.egg-info/top_level.txt
--rw-r--r--   0 eywalker   (501) staff       (20)    26444 2017-07-27 02:19:45.000000 datajoint-0.8.2/LICENSE.txt
--rw-r--r--   0 eywalker   (501) staff       (20)       14 2017-10-24 02:19:05.000000 datajoint-0.8.2/MANIFEST.in
--rw-r--r--   0 eywalker   (501) staff       (20)      428 2017-10-25 16:26:26.000000 datajoint-0.8.2/PKG-INFO
--rw-r--r--   0 eywalker   (501) staff       (20)       70 2017-10-24 02:19:05.000000 datajoint-0.8.2/requirements.txt
--rw-r--r--   0 eywalker   (501) staff       (20)       59 2017-10-25 16:26:26.000000 datajoint-0.8.2/setup.cfg
--rw-r--r--   0 eywalker   (501) staff       (20)     1033 2017-07-28 01:19:41.000000 datajoint-0.8.2/setup.py
--rw-r--r--   0 eywalker   (501) staff       (20)       27 2017-10-24 02:19:05.000000 datajoint-0.8.2/test_requirements.txt
+drwxr-xr-x   0 eywalker   (501) staff       (20)        0 2017-11-15 17:36:06.000000 datajoint-0.9.0/
+drwxr-xr-x   0 eywalker   (501) staff       (20)        0 2017-11-15 17:36:06.000000 datajoint-0.9.0/datajoint/
+-rw-r--r--   0 eywalker   (501) staff       (20)     3260 2017-10-24 02:19:05.000000 datajoint-0.9.0/datajoint/__init__.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     2252 2017-07-27 02:20:07.000000 datajoint-0.9.0/datajoint/admin.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     7977 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/autopopulate.py
+-rw-r--r--   0 eywalker   (501) staff       (20)    28333 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/base_relation.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     9600 2017-07-27 02:19:45.000000 datajoint-0.9.0/datajoint/blob.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     7988 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/connection.py
+-rw-r--r--   0 eywalker   (501) staff       (20)    10257 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/declare.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     6237 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/dependencies.py
+-rw-r--r--   0 eywalker   (501) staff       (20)    12574 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/erd.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     3683 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/external.py
+-rw-r--r--   0 eywalker   (501) staff       (20)    15443 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/fetch.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     1046 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/hash.py
+-rw-r--r--   0 eywalker   (501) staff       (20)    12302 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/heading.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     4433 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/jobs.py
+-rw-r--r--   0 eywalker   (501) staff       (20)    37883 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/relational_operand.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     4939 2017-10-24 02:19:05.000000 datajoint-0.9.0/datajoint/s3.py
+-rw-r--r--   0 eywalker   (501) staff       (20)    10131 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/schema.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     5415 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/settings.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     5183 2017-10-24 02:19:05.000000 datajoint-0.9.0/datajoint/user_relations.py
+-rw-r--r--   0 eywalker   (501) staff       (20)     1827 2017-07-27 02:19:45.000000 datajoint-0.9.0/datajoint/utils.py
+-rw-r--r--   0 eywalker   (501) staff       (20)       22 2017-11-15 17:35:05.000000 datajoint-0.9.0/datajoint/version.py
+drwxr-xr-x   0 eywalker   (501) staff       (20)        0 2017-11-15 17:36:06.000000 datajoint-0.9.0/datajoint.egg-info/
+-rw-r--r--   0 eywalker   (501) staff       (20)        1 2017-11-15 17:36:06.000000 datajoint-0.9.0/datajoint.egg-info/dependency_links.txt
+-rw-r--r--   0 eywalker   (501) staff       (20)      428 2017-11-15 17:36:06.000000 datajoint-0.9.0/datajoint.egg-info/PKG-INFO
+-rw-r--r--   0 eywalker   (501) staff       (20)       75 2017-11-15 17:36:06.000000 datajoint-0.9.0/datajoint.egg-info/requires.txt
+-rw-r--r--   0 eywalker   (501) staff       (20)      691 2017-11-15 17:36:06.000000 datajoint-0.9.0/datajoint.egg-info/SOURCES.txt
+-rw-r--r--   0 eywalker   (501) staff       (20)       10 2017-11-15 17:36:06.000000 datajoint-0.9.0/datajoint.egg-info/top_level.txt
+-rw-r--r--   0 eywalker   (501) staff       (20)    26444 2017-07-27 02:19:45.000000 datajoint-0.9.0/LICENSE.txt
+-rw-r--r--   0 eywalker   (501) staff       (20)       14 2017-10-24 02:19:05.000000 datajoint-0.9.0/MANIFEST.in
+-rw-r--r--   0 eywalker   (501) staff       (20)      428 2017-11-15 17:36:06.000000 datajoint-0.9.0/PKG-INFO
+-rw-r--r--   0 eywalker   (501) staff       (20)       75 2017-11-15 17:35:05.000000 datajoint-0.9.0/requirements.txt
+-rw-r--r--   0 eywalker   (501) staff       (20)       59 2017-11-15 17:36:06.000000 datajoint-0.9.0/setup.cfg
+-rw-r--r--   0 eywalker   (501) staff       (20)     1033 2017-07-28 01:19:41.000000 datajoint-0.9.0/setup.py
+-rw-r--r--   0 eywalker   (501) staff       (20)       26 2017-11-15 17:35:05.000000 datajoint-0.9.0/test_requirements.txt
```

### Comparing `datajoint-0.8.2/datajoint/__init__.py` & `datajoint-0.9.0/datajoint/__init__.py`

 * *Files identical despite different names*

### Comparing `datajoint-0.8.2/datajoint/admin.py` & `datajoint-0.9.0/datajoint/admin.py`

 * *Files identical despite different names*

### Comparing `datajoint-0.8.2/datajoint/autopopulate.py` & `datajoint-0.9.0/datajoint/autopopulate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 """autopopulate containing the dj.AutoPopulate class. See `dj.AutoPopulate` for more info."""
 import logging
 import datetime
+import traceback
 import random
+from tqdm import tqdm
+from itertools import count
 from pymysql import OperationalError
-from .relational_operand import RelationalOperand, AndList
+from .relational_operand import RelationalOperand, AndList, U
 from . import DataJointError
 from . import key as KEY
 from .base_relation import FreeRelation
 import signal
 
 # noinspection PyExceptionInherit,PyCallingNonCallable
 
 logger = logging.getLogger(__name__)
 
 
 class AutoPopulate:
     """
     AutoPopulate is a mixin class that adds the method populate() to a Relation class.
     Auto-populated relations must inherit from both Relation and AutoPopulate,
-    must define the property `key_source`, and must define the callback method _make_tuples.
+    must define the property `key_source`, and must define the callback method `make`.
     """
     _key_source = None
 
     @property
     def key_source(self):
         """
         :return: the relation whose primary key values are passed, sequentially, to the
-                `_make_tuples` method when populate() is called.The default value is the
+                ``make`` method when populate() is called.The default value is the
                 join of the parent relations. Users may override to change the granularity
                 or the scope of populate() calls.
         """
         if self._key_source is None:
             self.connection.dependencies.load(self.full_table_name)
             parents = list(self.target.parents(primary=True))
             if not parents:
                 raise DataJointError('A relation must have parent relations to be able to be populated')
             self._key_source = FreeRelation(self.connection, parents.pop(0)).proj()
             while parents:
                 self._key_source *= FreeRelation(self.connection, parents.pop(0)).proj()
         return self._key_source
 
-    def _make_tuples(self, key):
+
+    def make(self, key):
         """
-        Derived classes must implement method _make_tuples that fetches data from tables that are
+        Derived classes must implement method `make` that fetches data from tables that are
         above them in the dependency hierarchy, restricting by the given key, computes dependent
         attributes, and inserts the new tuples into self.
         """
-        raise NotImplementedError('Subclasses of AutoPopulate must implement the method "_make_tuples"')
+        raise NotImplementedError('Subclasses of AutoPopulate must implement the method `make`')
+
 
     @property
     def target(self):
         """
         relation to be populated.
         Typically, AutoPopulate are mixed into a Relation object and the target is self.
         """
@@ -59,100 +64,120 @@
     def _job_key(self, key):
         """
         :param key:  they key returned for the job from the key source
         :return: the dict to use to generate the job reservation hash
         """
         return key
 
-    def populate(self, *restrictions, suppress_errors=False, reserve_jobs=False, order="original", limit=None):
+    def populate(self, *restrictions, suppress_errors=False, reserve_jobs=False,
+                 order="original", limit=None, max_calls=None, display_progress=False):
         """
-        rel.populate() calls rel._make_tuples(key) for every primary key in self.key_source
+        rel.populate() calls rel.make(key) for every primary key in self.key_source
         for which there is not already a tuple in rel.
 
         :param restrictions: a list of restrictions each restrict (rel.key_source - target.proj())
         :param suppress_errors: suppresses error if true
         :param reserve_jobs: if true, reserves job to populate in asynchronous fashion
         :param order: "original"|"reverse"|"random"  - the order of execution
-        :param limit: if not None, populates at max that many keys
+        :param display_progress: if True, report progress_bar
+        :param limit: if not None, checks at most that many keys
+        :param max_calls: if not None, populates at max that many keys
         """
         if self.connection.in_transaction:
             raise DataJointError('Populate cannot be called during a transaction.')
 
         valid_order = ['original', 'reverse', 'random']
         if order not in valid_order:
             raise DataJointError('The order argument must be one of %s' % str(valid_order))
 
         todo = self.key_source
         if not isinstance(todo, RelationalOperand):
             raise DataJointError('Invalid key_source value')
-        todo = todo.proj() & AndList(restrictions)
+        todo = (todo & AndList(restrictions)).proj()
 
-        error_list = [] if suppress_errors else None
+        # raise error if the populated target lacks any attributes from the primary key of key_source
+        try:
+            raise DataJointError(
+                    'The populate target lacks attribute %s from the primary key of key_source' % next(
+                        name for name in todo.heading if name not in self.target.heading))
+        except StopIteration:
+            pass
+
+        todo -= self.target
 
-        jobs = self.connection.jobs[self.target.database] if reserve_jobs else None
+        error_list = [] if suppress_errors else None
+        jobs = self.connection.schemas[self.target.database].jobs if reserve_jobs else None
 
         # define and setup signal handler for SIGTERM
         if reserve_jobs:
             def handler(signum, frame):
                 logger.info('Populate terminated by SIGTERM')
                 raise SystemExit('SIGTERM received')
             old_handler = signal.signal(signal.SIGTERM, handler)
 
-        todo -= self.target
         keys = todo.fetch(KEY, limit=limit)
         if order == "reverse":
             keys.reverse()
         elif order == "random":
             random.shuffle(keys)
 
+        call_count = count()
         logger.info('Found %d keys to populate' % len(keys))
-        for key in keys:
+
+        make = self._make_tuples if hasattr(self, '_make_tuples') else self.make
+
+        for key in (tqdm(keys) if display_progress else keys):
+            if max_calls is not None and call_count >= max_calls:
+                break
             if not reserve_jobs or jobs.reserve(self.target.table_name, self._job_key(key)):
                 self.connection.start_transaction()
                 if key in self.target:  # already populated
                     self.connection.cancel_transaction()
                     if reserve_jobs:
                         jobs.complete(self.target.table_name, self._job_key(key))
                 else:
                     logger.info('Populating: ' + str(key))
+                    next(call_count)
                     try:
-                        self._make_tuples(dict(key))
+                        make(dict(key))
                     except (KeyboardInterrupt, SystemExit, Exception) as error:
                         try:
                             self.connection.cancel_transaction()
                         except OperationalError:
                             pass
                         if reserve_jobs:
                             # show error name and error message (if any)
                             error_message = ': '.join([error.__class__.__name__, str(error)]).strip(': ')
-                            jobs.error(self.target.table_name, self._job_key(key), error_message=error_message)
+                            jobs.error(self.target.table_name, self._job_key(key),
+                                       error_message=error_message, error_stack=traceback.format_exc())
 
                         if not suppress_errors or isinstance(error, SystemExit):
                             raise
                         else:
                             logger.error(error)
                             error_list.append((key, error))
                     else:
                         self.connection.commit_transaction()
                         if reserve_jobs:
                             jobs.complete(self.target.table_name, self._job_key(key))
 
         # place back the original signal handler
         if reserve_jobs:
             signal.signal(signal.SIGTERM, old_handler)
-
         return error_list
 
     def progress(self, *restrictions, display=True):
         """
         report progress of populating this table
         :return: remaining, total -- tuples to be populated
         """
-        todo = self.key_source & AndList(restrictions)
+        todo = (self.key_source & AndList(restrictions)).proj()
+        if any(name not in self.target.heading for name in todo.heading):
+            raise DataJointError('The populated target must have all the attributes of the key source')
         total = len(todo)
-        remaining = len(todo.proj() - self.target)
+        remaining = len(todo - self.target)
         if display:
             print('%-20s' % self.__class__.__name__,
                   'Completed %d of %d (%2.1f%%)   %s' % (
                       total - remaining, total, 100 - 100 * remaining / (total+1e-12),
                       datetime.datetime.strftime(datetime.datetime.now(), '%Y-%m-%d %H:%M:%S')), flush=True)
         return remaining, total
```

### Comparing `datajoint-0.8.2/datajoint/base_relation.py` & `datajoint-0.9.0/datajoint/base_relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     table name, database, context, and definition.
     A Relation implements insert and delete methods in addition to inherited relational operators.
     """
     _heading = None
     _context = None
     database = None
     _log_ = None
+    _external_table = None
 
     # -------------- required by RelationalOperand ----------------- #
     @property
     def heading(self):
         """
         Returns the table heading. If the table is not declared, attempts to declare it and return heading.
         :return: table heading
@@ -46,22 +47,29 @@
 
     @property
     def context(self):
         return self._context
 
     def declare(self):
         """
-        Loads the table heading. If the table is not declared, use self.definition to declare
+        Use self.definition to declare the table in the database
         """
         try:
-            self.connection.query(
-                declare(self.full_table_name, self.definition, self._context))
+            sql, uses_external = declare(self.full_table_name, self.definition, self._context)
+            if uses_external:
+                # trigger the creation of the external hash lookup for the current schema
+                external_table = self.connection.schemas[self.database].external_table
+                sql = sql.format(external_table=external_table.full_table_name)
+            self.connection.query(sql)
         except pymysql.OperationalError as error:
+            # skip if no create privilege
             if error.args[0] == server_error_codes['command denied']:
                 logger.warning(error.args[1])
+            else:
+                raise
         else:
             self._log('Declared ' + self.full_table_name)
 
     @property
     def from_clause(self):
         """
         :return: the FROM clause of SQL SELECT statements.
@@ -110,14 +118,20 @@
 
     @property
     def _log(self):
         if self._log_ is None:
             self._log_ = Log(self.connection, database=self.database)
         return self._log_
 
+    @property
+    def external_table(self):
+        if self._external_table is None:
+            self._external_table = self.connection.schemas[self.database].external_table
+        return self._external_table
+
     def insert1(self, row, **kwargs):
         """
         Insert one data record or one Mapping (like a dict).
         :param row: a numpy record, a dict-like object, or an ordered sequence to be inserted as one row.
         For kwargs, see insert()
         """
         self.insert((row,), **kwargs)
@@ -138,68 +152,37 @@
         >>>     dict(subject_id=8, species="mouse", date_of_birth="2014-09-02")])
         """
 
         if ignore_errors:
             warnings.warn('Use of `ignore_errors` in `insert` and `insert1` is deprecated. Use try...except... '
                           'to explicitly handle any errors', stacklevel=2)
 
-        # handle query safely - if skip_duplicates=True, wraps the query with transaction and checks for warning
-        def safe_query(*args, **kwargs):
-            if skip_duplicates:
-                # check if there is already an open transaction
-                open_transaction = self.connection.in_transaction
-                if not open_transaction:
-                    self.connection.start_transaction()
-                try:
-                    with warnings.catch_warnings(record=True) as ws:
-                        warnings.simplefilter('always')
-                        self.connection.query(*args, suppress_warnings=False, **kwargs)
-                        for w in ws:
-                            if w.message.args[0] != server_error_codes['duplicate entry']:
-                                raise InternalError(w.message.args)
-                except:
-                    if not open_transaction:
-                        try:
-                            self.connection.cancel_transaction()
-                        except OperationalError:
-                            pass
-                    raise
-                else:
-                    if not open_transaction:
-                        self.connection.commit_transaction()
-            else:
-                self.connection.query(*args, **kwargs)
-
+        heading = self.heading
         if isinstance(rows, RelationalOperand):
-            # INSERT FROM SELECT - build alternate field-narrowing query (only) when needed
-            if ignore_extra_fields and not all(name in self.heading.names for name in rows.heading.names):
-                query = 'INSERT{ignore} INTO {table} ({fields}) SELECT {fields} FROM ({select}) as `__alias`'.format(
-                ignore=" IGNORE" if skip_duplicates else "",
-                table=self.full_table_name,
-                fields='`'+'`,`'.join(self.heading.names)+'`',
-                select=rows.make_sql())
-            else:
-                query = 'INSERT{ignore} INTO {table} ({fields}) {select}'.format(
-                ignore=" IGNORE" if skip_duplicates else "",
+            # insert from select
+            if not ignore_extra_fields:
+                try:
+                    raise DataJointError(
+                        "Attribute %s not found.  To ignore extra attributes in insert, set ignore_extra_fields=True." %
+                        next(name for name in rows.heading if name not in heading))
+                except StopIteration:
+                    pass
+            fields = list(name for name in heading if name in rows.heading)
+
+            query = '{command} INTO {table} ({fields}) {select}{duplicate}'.format(
+                command='REPLACE' if replace else 'INSERT',
+                fields='`' + '`,`'.join(fields) + '`',
                 table=self.full_table_name,
-                fields='`'+'`,`'.join(rows.heading.names)+'`',
-                select=rows.make_sql())
-            try:
-                safe_query(query)
-            except (InternalError, IntegrityError) as err:
-                if err.args[0] == server_error_codes['unknown column']:
-                    # args[1] -> Unknown column 'extra' in 'field list'
-                    raise DataJointError('{} : To ignore extra fields, set ignore_extra_fields=True in insert.'.format(err.args[1]))
-                elif err.args[0] == server_error_codes['duplicate entry']:
-                    raise DataJointError('{} : To ignore duplicate entries, set skip_duplicates=True in insert.'.format(err.args[1]))
-                else:
-                    raise
+                select=rows.make_sql(select_fields=fields),
+                duplicate=(' ON DUPLICATE KEY UPDATE `{pk}`=`{pk}`'.format(pk=self.primary_key[0])
+                           if skip_duplicates else '')
+            )
+            self.connection.query(query)
             return
 
-        heading = self.heading
         if heading.attributes is None:
             logger.warning('Could not access table {table}'.format(table=self.full_table_name))
             return
 
         field_list = None  # ensures that all rows have the same attributes in the same order as the first row.
 
         def make_row_to_insert(row):
@@ -214,24 +197,26 @@
                 as a string to be included in the query and the value, if any, to be submitted for
                 processing by mysql API.
                 :param name:
                 :param value:
                 """
                 if ignore_extra_fields and name not in heading:
                     return None
-                if heading[name].is_blob:
-                    value = pack(value)
-                    placeholder = '%s'
+                if heading[name].is_external:
+                    placeholder, value = '%s', self.external_table.put(heading[name].type, value)
+                elif heading[name].is_blob:
+                    if value is None:
+                        placeholder, value = 'NULL', None
+                    else:
+                        placeholder, value = '%s', pack(value)
                 elif heading[name].numeric:
                     if value is None or value == '' or np.isnan(np.float(value)):  # nans are turned into NULLs
-                        placeholder = 'NULL'
-                        value = None
+                        placeholder, value = 'NULL', None
                     else:
-                        placeholder = '%s'
-                        value = str(int(value) if isinstance(value, bool) else value)
+                        placeholder, value = '%s', (str(int(value) if isinstance(value, bool) else value))
                 else:
                     placeholder = '%s'
                 return name, placeholder, value
 
             def check_fields(fields):
                 """
                 Validates that all items in `fields` are valid attributes in the heading
@@ -280,35 +265,36 @@
                 row_to_insert['values'] = list(row_to_insert['values'][i] for i in order)
 
             return row_to_insert
 
         rows = list(make_row_to_insert(row) for row in rows)
         if rows:
             try:
-                safe_query(
-                    "{command} INTO {destination}(`{fields}`) VALUES {placeholders}".format(
-                        command='REPLACE' if replace else 'INSERT IGNORE' if skip_duplicates else 'INSERT',
-                        destination=self.from_clause,
-                        fields='`,`'.join(field_list),
-                        placeholders=','.join('(' + ','.join(row['placeholders']) + ')' for row in rows)),
-                    args=list(itertools.chain.from_iterable((v for v in r['values'] if v is not None) for r in rows)))
+                query = "{command} INTO {destination}(`{fields}`) VALUES {placeholders}{duplicate}".format(
+                    command='REPLACE' if replace else 'INSERT',
+                    destination=self.from_clause,
+                    fields='`,`'.join(field_list),
+                    placeholders=','.join('(' + ','.join(row['placeholders']) + ')' for row in rows),
+                    duplicate=(' ON DUPLICATE KEY UPDATE `{pk}`=`{pk}`'.format(pk=self.primary_key[0])
+                               if skip_duplicates else ''))
+                self.connection.query(query, args=list(
+                    itertools.chain.from_iterable((v for v in r['values'] if v is not None) for r in rows)))
             except (OperationalError, InternalError, IntegrityError) as err:
                 if err.args[0] == server_error_codes['command denied']:
                     raise DataJointError('Command denied:  %s' % err.args[1]) from None
                 elif err.args[0] == server_error_codes['unknown column']:
                     # args[1] -> Unknown column 'extra' in 'field list'
                     raise DataJointError(
                         '{} : To ignore extra fields, set ignore_extra_fields=True in insert.'.format(err.args[1])) from None
                 elif err.args[0] == server_error_codes['duplicate entry']:
                     raise DataJointError(
                         '{} : To ignore duplicate entries, set skip_duplicates=True in insert.'.format(err.args[1])) from None
                 else:
                     raise
 
-
     def delete_quick(self):
         """
         Deletes the table without cascading and without user prompt. If this table has any dependent
         table(s), this will fail.
         """
         query = 'DELETE FROM ' + self.full_table_name + self.where_clause
         self.connection.query(query)
@@ -334,15 +320,15 @@
 
         # construct restrictions for each relation
         restrict_by_me = set()
         restrictions = collections.defaultdict(list)
         # restrict by self
         if self.restrictions:
             restrict_by_me.add(self.full_table_name)
-            restrictions[self.full_table_name].append(self.restrictions.simplify())  # copy own restrictions
+            restrictions[self.full_table_name].append(self.restrictions)  # copy own restrictions
         # restrict by renamed nodes
         restrict_by_me.update(table for table in delete_list if table.isdigit())  # restrict by all renamed nodes
         # restrict by tables restricted by a non-primary semijoin
         for table in delete_list:
             restrict_by_me.update(graph.children(table, primary=False))   # restrict by any non-primary dependents
 
         # compile restriction lists
@@ -450,15 +436,15 @@
                 in_key = False
             attributes_thus_far.add(attr.name)
             do_include = True
             for parent_name, fk_props in list(parents.items()):  # need list() to force a copy
                 if attr.name in fk_props['referencing_attributes']:
                     do_include = False
                     if attributes_thus_far.issuperset(fk_props['referencing_attributes']):
-                        # simple foreign keys
+                        # simple foreign key
                         parents.pop(parent_name)
                         if not parent_name.isdigit():
                             definition += '-> {class_name}\n'.format(
                                 class_name=lookup_class_name(parent_name, self.context) or parent_name)
                         else:
                             # aliased foreign key
                             parent_name = self.connection.dependencies.in_edges(parent_name)[0][0]
@@ -469,17 +455,18 @@
                                 attr_list=','.join(r[0] for r in lst),
                                 class_name=lookup_class_name(parent_name, self.context) or parent_name,
                                 ref_list=('' if len(attributes_thus_far) - len(attributes_declared) == 1
                                           else '(%s)' % ','.join(r[1] for r in lst)))
                             attributes_declared.update(fk_props['referencing_attributes'])
             if do_include:
                 attributes_declared.add(attr.name)
+                name = attr.name.lstrip('_')  # for external
                 definition += '%-20s : %-28s # %s\n' % (
-                    attr.name if attr.default is None else '%s=%s' % (attr.name, attr.default),
-                    '%s%s' % (attr.type, 'auto_increment' if attr.autoincrement else ''), attr.comment)
+                    name if attr.default is None else '%s=%s' % (name, attr.default),
+                    '%s%s' % (attr.type, ' auto_increment' if attr.autoincrement else ''), attr.comment)
         print(definition)
         return definition
 
     def _update(self, attrname, value=None):
         """
             Updates a field in an existing tuple. This is not a datajoyous operation and should not be used
             routinely. Relational database maintain referential integrity on the level of a tuple. Therefore,
@@ -543,15 +530,15 @@
                 if member.full_table_name == name:   # found it!
                     return '.'.join([node['context_name'],  member_name]).lstrip('.')
                 try:  # look for part tables
                     parts = member._ordered_class_members
                 except AttributeError:
                     pass  # not a UserRelation -- cannot have part tables.
                 else:
-                    for part in (getattr(member, p) for p in parts):
+                    for part in (getattr(member, p) for p in parts if hasattr(member, p)):
                         if inspect.isclass(part) and issubclass(part, BaseRelation) and part.full_table_name == name:
                             return '.'.join([node['context_name'], member_name, part.__name__]).lstrip('.')
             elif node['depth'] > 0 and inspect.ismodule(member) and member.__name__ != 'datajoint':
                 try:
                     nodes.append(
                         dict(context=dict(inspect.getmembers(member)),
                              context_name=node['context_name'] + '.' + member_name,
```

### Comparing `datajoint-0.8.2/datajoint/blob.py` & `datajoint-0.9.0/datajoint/blob.py`

 * *Files identical despite different names*

### Comparing `datajoint-0.8.2/datajoint/connection.py` & `datajoint-0.9.0/datajoint/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pymysql as client
 import logging
 from getpass import getpass
 
 from . import config
 from . import DataJointError
 from .dependencies import Dependencies
-from .jobs import JobManager
 from pymysql import err
 
 logger = logging.getLogger(__name__)
 
 
 def conn(host=None, user=None, password=None, init_fun=None, reset=False):
     """
@@ -71,15 +70,14 @@
         if self.is_connected:
             logger.info("Connected {user}@{host}:{port}".format(**self.conn_info))
             self.connection_id = self.query('SELECT connection_id()').fetchone()[0]
         else:
             raise DataJointError('Connection failed.')
         self._conn.autocommit(True)
         self._in_transaction = False
-        self.jobs = JobManager(self)
         self.schemas = dict()
         self.dependencies = Dependencies(self)
 
     def __eq__(self, other):
         return self.conn_info == other.conn_info
 
     def __repr__(self):
@@ -87,15 +85,18 @@
         return "DataJoint connection ({connected}) {user}@{host}:{port}".format(
             connected=connected, **self.conn_info)
 
     def connect(self):
         """
         Connects to the database server.
         """
-        self._conn = client.connect(init_command=self.init_fun, **self.conn_info)
+        self._conn = client.connect(init_command=self.init_fun,
+                                    sql_mode="NO_ZERO_DATE,NO_ZERO_IN_DATE,ERROR_FOR_DIVISION_BY_ZERO,"
+                                             "STRICT_TRANS_TABLES,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION",
+                                    **self.conn_info)
 
     def register(self, schema):
         self.schemas[schema.database] = schema
 
     @property
     def is_connected(self):
         """
```

### Comparing `datajoint-0.8.2/datajoint/declare.py` & `datajoint-0.9.0/datajoint/declare.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 This module hosts functions to convert DataJoint table definitions into mysql table definitions, and to
 declare the corresponding mysql tables.
 """
 import re
 import pyparsing as pp
 import logging
 
-from . import DataJointError
+from . import DataJointError, config
+
+STORE_NAME_LENGTH = 8
+STORE_HASH_LENGTH = 43
+HASH_DATA_TYPE = 'char(51)'
 
 logger = logging.getLogger(__name__)
 
 
 def build_foreign_key_parser():
     left = pp.Literal('(').suppress()
     right = pp.Literal(')').suppress()
@@ -59,15 +63,15 @@
     :param attr_sql: a list of sql statements defining attributes -- to be updated by this function.
     :param foreign_key_sql: a list of sql statements specifying foreign key constraints -- to be updated by this function.
     """
     from .base_relation import BaseRelation
     try:
         result = foreign_key_parser.parseString(line)
     except pp.ParseException as err:
-        raise DataJointError('Parsing error in line "%s". %s.' % line, err)
+        raise DataJointError('Parsing error in line "%s". %s.' % (line, err))
     try:
         referenced_class = eval(result.ref_table, context)
     except NameError:
         raise DataJointError('Foreign key reference %s could not be resolved' % result.ref_table)
     if not issubclass(referenced_class, BaseRelation):
         raise DataJointError('Foreign key reference %s must be a subclass of UserRelation' % result.ref_table)
     ref = referenced_class()
@@ -110,51 +114,54 @@
     table_comment = definition.pop(0)[1:].strip() if definition[0].startswith('#') else ''
     in_key = True  # parse primary keys
     primary_key = []
     attributes = []
     attribute_sql = []
     foreign_key_sql = []
     index_sql = []
+    uses_external = False
 
     for line in definition:
         if line.startswith('#'):  # additional comments are ignored
             pass
         elif line.startswith('---') or line.startswith('___'):
             in_key = False  # start parsing dependent attributes
         elif is_foreign_key(line):
             compile_foreign_key(line, context, attributes,
                                 primary_key if in_key else None,
                                 attribute_sql, foreign_key_sql)
         elif re.match(r'^(unique\s+)?index[^:]*$', line, re.I):   # index
             index_sql.append(line)  # the SQL syntax is identical to DataJoint's
         else:
-            name, sql = compile_attribute(line, in_key)
+            name, sql, is_external = compile_attribute(line, in_key, foreign_key_sql)
+            uses_external = uses_external or is_external
             if in_key and name not in primary_key:
                 primary_key.append(name)
             if name not in attributes:
                 attributes.append(name)
                 attribute_sql.append(sql)
     # compile SQL
     if not primary_key:
         raise DataJointError('Table must have a primary key')
     return ('CREATE TABLE IF NOT EXISTS %s (\n' % full_table_name +
             ',\n'.join(attribute_sql +
                        ['PRIMARY KEY (`' + '`,`'.join(primary_key) + '`)'] +
                        foreign_key_sql +
                        index_sql) +
-            '\n) ENGINE=InnoDB, COMMENT "%s"' % table_comment)
+            '\n) ENGINE=InnoDB, COMMENT "%s"' % table_comment), uses_external
 
 
-def compile_attribute(line, in_key=False):
+def compile_attribute(line, in_key, foreign_key_sql):
     """
     Convert attribute definition from DataJoint format to SQL
 
     :param line: attribution line
     :param in_key: set to True if attribute is in primary key set
-    :returns: (name, sql) -- attribute name and sql code for its declaration
+    :param foreign_key_sql:
+    :returns: (name, sql, is_external) -- attribute name and sql code for its declaration
     """
 
     try:
         match = attribute_parser.parseString(line+'#', parseAll=True)
     except pp.ParseException as err:
         raise DataJointError('Declaration error in position {pos} in line:\n  {line}\n{msg}'.format(
             line=err.args[0], pos=err.args[1], msg=err.args[2]))
@@ -173,9 +180,39 @@
         if match['default']:
             quote = match['default'].upper() not in literals and match['default'][0] not in '"\''
             match['default'] = ('NOT NULL DEFAULT ' +
                                 ('"%s"' if quote else "%s") % match['default'])
         else:
             match['default'] = 'NOT NULL'
     match['comment'] = match['comment'].replace('"', '\\"')   # escape double quotes in comment
-    sql = ('`{name}` {type} {default}' + (' COMMENT "{comment}"' if match['comment'] else '')).format(**match)
-    return match['name'], sql
+
+    is_external = match['type'].startswith('external')
+    if not is_external:
+        sql = ('`{name}` {type} {default}' + (' COMMENT "{comment}"' if match['comment'] else '')).format(**match)
+    else:
+        # process externally stored attribute
+        if in_key:
+            raise DataJointError('External attributes cannot be primary in:\n%s' % line)
+        store_name = match['type'].split('-')
+        if store_name[0] != 'external':
+            raise DataJointError('External store types must be specified as "external" or "external-<name>"')
+        store_name = '-'.join(store_name[1:])
+        if store_name != '' and not store_name.isidentifier():
+            raise DataJointError(
+                'The external store name `{type}` is invalid. Make like a python identifier.'.format(**match))
+        if len(store_name)>STORE_NAME_LENGTH:
+            raise DataJointError(
+                'The external store name `{type}` is too long. Must be <={max_len} characters.'.format(
+                    max_len=STORE_NAME_LENGTH, **match))
+        if not match['default'] in ('DEFAULT NULL', 'NOT NULL'):
+            raise DataJointError('The only acceptable default value for an external field is null in:\n%s' % line)
+        if match['type'] not in config:
+            raise DataJointError('The external store `{type}` is not configured.'.format(**match))
+
+        # append external configuration name to the end of the comment
+        sql = '`{name}` {hash_type} {default} COMMENT ":{type}:{comment}"'.format(
+            hash_type=HASH_DATA_TYPE, **match)
+        foreign_key_sql.append(
+            "FOREIGN KEY (`{name}`) REFERENCES {{external_table}} (`hash`) "
+            "ON UPDATE RESTRICT ON DELETE RESTRICT".format(**match))
+
+    return match['name'], sql, is_external
```

### Comparing `datajoint-0.8.2/datajoint/dependencies.py` & `datajoint-0.9.0/datajoint/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,30 +54,31 @@
                 else:
                     primary_key = [s.strip(' `') for s in result.primary_key.split(',')]
             try:
                 result = fk_parser.parseString(line)
             except pp.ParseException:
                 pass
             else:
-                referencing_attributes = [r.strip('` ') for r in result.attributes.split(',')]
-                referenced_attributes = [r.strip('` ') for r in result.referenced_attributes.split(',')]
-                props = dict(
-                    primary=all(a in primary_key for a in referencing_attributes),
-                    referencing_attributes=referencing_attributes,
-                    referenced_attributes=referenced_attributes,
-                    aliased=not all(a == b for a, b in zip(referencing_attributes, referenced_attributes)),
-                    multi=not all(a in referencing_attributes for a in primary_key))
-                if not props['aliased']:
-                    self.add_edge(result.referenced_table, table_name, **props)
-                else:
-                    # for aliased dependencies, add an extra node in the format '1', '2', etc
-                    alias_node = '%d' % next(self._node_alias_count)
-                    self.add_node(alias_node)
-                    self.add_edge(result.referenced_table, alias_node, **props)
-                    self.add_edge(alias_node, table_name, **props)
+                if '`.`~' not in result.referenced_table:  # omit external tables
+                    referencing_attributes = [r.strip('` ') for r in result.attributes.split(',')]
+                    referenced_attributes = [r.strip('` ') for r in result.referenced_attributes.split(',')]
+                    props = dict(
+                        primary=all(a in primary_key for a in referencing_attributes),
+                        referencing_attributes=referencing_attributes,
+                        referenced_attributes=referenced_attributes,
+                        aliased=not all(a == b for a, b in zip(referencing_attributes, referenced_attributes)),
+                        multi=not all(a in referencing_attributes for a in primary_key))
+                    if not props['aliased']:
+                        self.add_edge(result.referenced_table, table_name, **props)
+                    else:
+                        # for aliased dependencies, add an extra node in the format '1', '2', etc
+                        alias_node = '%d' % next(self._node_alias_count)
+                        self.add_node(alias_node)
+                        self.add_edge(result.referenced_table, alias_node, **props)
+                        self.add_edge(alias_node, table_name, **props)
 
     def load(self, target=None):
         """
         Load dependencies for all loaded schemas.
         This method gets called before any operation that requires dependencies: delete, drop, populate, progress.
         """
         if target is not None and '.' in target:  # `database`.`table`
```

### Comparing `datajoint-0.8.2/datajoint/erd.py` & `datajoint-0.9.0/datajoint/erd.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import functools
 import io
 import warnings
 
 try:
     from matplotlib import pyplot as plt
-    from networkx.drawing.nx_agraph import graphviz_layout
+    from networkx.drawing.nx_pydot import pydot_layout
     erd_active = True
 except:
     erd_active = False
 
 from . import Manual, Imported, Computed, Lookup, Part, DataJointError
 from .base_relation import lookup_class_name
 
@@ -31,14 +31,15 @@
     else:
         try:
             return next(tier for tier in user_relation_classes
                         if re.fullmatch(tier.tier_regexp, table_name.split('`')[-2]))
         except StopIteration:
             return None
 
+
 if not erd_active:
     class ERD:
         """
         Entity relationship diagram, currently disabled due to the lack of required packages: matplotlib and pygraphviz.
 
         To enable ERD feature, please install both matplotlib and pygraphviz. For instructions on how to install
         these two packages, refer to http://docs.datajoint.io/setup/Install-and-connect.html#python and
@@ -226,15 +227,15 @@
                            size=0.4*scale, fixed=False),
                 _AliasNode: dict(shape='circle', color="#FF880080", fontcolor='white', fontsize=round(scale*6),
                                  size=0.15*scale, fixed=True),
                 Manual: dict(shape='box', color="#00FF0030", fontcolor='darkgreen', fontsize=round(scale*10),
                              size=0.4*scale, fixed=False),
                 Lookup: dict(shape='plaintext', color='#00000020', fontcolor='black', fontsize=round(scale*8),
                              size=0.4*scale, fixed=False),
-                Computed: dict(shape='circle', color='#FF000020', fontcolor='#7F0000A0', fontsize=round(scale*10),
+                Computed: dict(shape='ellipse', color='#FF000020', fontcolor='#7F0000A0', fontsize=round(scale*10),
                                size=0.3*scale, fixed=True),
                 Imported: dict(shape='ellipse', color='#00007F40', fontcolor='#00007FA0', fontsize=round(scale*10),
                                size=0.4*scale, fixed=False),
                 Part: dict(shape='plaintext', color='#0000000', fontcolor='black', fontsize=round(scale*8),
                            size=0.1*scale, fixed=False)}
             node_props = {node: label_props[d['node_type']] for node, d in dict(graph.nodes(data=True)).items()}
 
@@ -300,9 +301,8 @@
                 with open(filename, 'w') as f:
                     f.write(self.make_svg().data)
             else:
                 raise DataJointError('Unsupported file format')
 
         @staticmethod
         def _layout(graph, **kwargs):
-            return graphviz_layout(graph, prog='dot', **kwargs)
-
+            return pydot_layout(graph, prog='dot', **kwargs)
```

### Comparing `datajoint-0.8.2/datajoint/fetch.py` & `datajoint-0.9.0/datajoint/fetch.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     def squeeze(self):
         """
         DEPRECATED
 
         Changes the state of the fetch object to squeeze the returned values as much as possible.
         :return: a copy of the fetch object
         """
-
         warnings.warn('Use of `squeeze` on `fetch` object is deprecated. Please use `squeeze=True` keyword arguments '
                       'in the call to `fetch`/`keys` instead', stacklevel=2)
 
         ret = self.copy()
         ret.ext_behavior['squeeze'] = True
         return ret
 
@@ -109,17 +108,15 @@
     def as_dict(self):
         """
         DEPRECATED
 
         Changes the state of the fetch object to return dictionaries.
         :return: a copy of the fetch object
         Example:
-
         >>> my_relation.fetch.as_dict()
-
         """
         warnings.warn('Use of `as_dict` on `fetch` object is deprecated. Please use `as_dict` keyword arguments in the '
                       'call to `fetch`/`keys` instead', stacklevel=2)
         ret = Fetch(self)
         ret.sql_behavior['as_dict'] = True
         return ret
 
@@ -154,33 +151,47 @@
         if ret.sql_behavior['limit'] is None:
             warnings.warn('Fetch offset should be used with a limit.')
         ret.sql_behavior['offset'] = offset
         return ret
 
     def __call__(self, *attrs, **kwargs):
         """
-        Fetches the relation from the database table into an np.array and unpacks blob attributes.
+        Fetches the query results from the database into an np.array or list of dictionaries and unpacks blob attributes.
 
         :param attrs: OPTIONAL. one or more attributes to fetch. If not provided, the call will return
         all attributes of this relation. If provided, returns tuples with an entry for each attribute.
         :param offset: the number of tuples to skip in the returned result
         :param limit: the maximum number of tuples to return
         :param order_by: the list of attributes to order the results. No ordering should be assumed if order_by=None.
         :param as_dict: returns a list of dictionaries instead of a record array
-        :return: the contents of the relation in the form of a structured numpy.array
+        :param squeeze:  if True, remove extra dimensions from arrays
+        :return: the contents of the relation in the form of a structured numpy.array or a dict list
         """
+
+        # check unexpected arguments
+        try:
+            raise TypeError("fetch() got an unexpected argument '%s'" % next(
+                k for k in kwargs if k not in {'offset', 'limit', 'as_dict', 'squeeze', 'order_by'}))
+        except StopIteration:
+            pass   # arguments are okay
+
         # if 'order_by' passed in a string, make into list
         if isinstance(kwargs.get('order_by'), str):
             kwargs['order_by'] = [kwargs['order_by']]
 
         sql_behavior = update_dict(self.sql_behavior, kwargs)
         ext_behavior = update_dict(self.ext_behavior, kwargs)
         total_behavior = dict(sql_behavior)
         total_behavior.update(ext_behavior)
 
+        # if attrs are specified then as_dict cannot be true
+        if attrs and sql_behavior['as_dict']:
+            raise DataJointError('Cannot specify attributes to return when as_dict=True. '
+                                 'Use proj() to select attributes or set as_dict=False')
+
         unpack_ = partial(unpack, squeeze=ext_behavior['squeeze'])
 
         if sql_behavior['limit'] is None and sql_behavior['offset'] is not None:
             warnings.warn('Offset set, but no limit. Setting limit to a large number. '
                           'Consider setting a limit explicitly.')
             sql_behavior['limit'] = 2 * len(self._relation)
 
@@ -190,16 +201,20 @@
             if sql_behavior['as_dict']:
                 ret = [OrderedDict((name, unpack_(d[name]) if heading[name].is_blob else d[name])
                                    for name in heading.names)
                        for d in cur.fetchall()]
             else:
                 ret = list(cur.fetchall())
                 ret = np.array(ret, dtype=heading.as_dtype)
-                for blob_name in heading.blobs:
-                    ret[blob_name] = list(map(unpack_, ret[blob_name]))
+                for name in heading:
+                    if heading[name].is_external:
+                        external_table = self._relation.connection.schemas[heading[name].database].external_table
+                        ret[name] = list(map(external_table.get, ret[name]))
+                    elif heading[name].is_blob:
+                        ret[name] = list(map(unpack_, ret[name]))
 
         else:  # if list of attributes provided
             attributes = [a for a in attrs if a is not PRIMARY_KEY]
             result = self._relation.proj(*attributes).fetch(**total_behavior)
             return_values = [
                 list(to_dicts(result[self._relation.primary_key]))
                 if attribute is PRIMARY_KEY else result[attribute]
@@ -208,14 +223,17 @@
 
         return ret
 
     def __iter__(self):
         """
         Iterator that returns the contents of the database.
         """
+        warnings.warn('Iteration on the fetch object is deprecated.  '
+                      'Iterate over the result of fetch() or fetch.keys() instead')
+
         sql_behavior = dict(self.sql_behavior)
         ext_behavior = dict(self.ext_behavior)
 
         unpack_ = partial(unpack, squeeze=ext_behavior['squeeze'])
 
         cur = self._relation.cursor(**sql_behavior)
 
@@ -246,17 +264,16 @@
         datajoint.key is a special value that requests the entire primary key
         :return: tuple with an entry for each element of item
 
         Examples:
         >>> a, b = relation['a', 'b']
         >>> a, b, key = relation['a', 'b', datajoint.key]
         """
-
-        warnings.warn('Use of `rel.fetch[a, b]` notation is deprecated. Please use `rel.fetch(a, b) for equivalent '
-                      'result', stacklevel=2)
+        warnings.warn('Use of `rel.fetch[a, b]` notation is deprecated. '
+                      'Please use `rel.fetch(a, b) for equivalent result', stacklevel=2)
 
         behavior = dict(self.sql_behavior)
         behavior.update(self.ext_behavior)
 
         single_output = isinstance(item, str) or item is PRIMARY_KEY or isinstance(item, int)
         item, attributes = self._prepare_attributes(item)
         result = self._relation.proj(*attributes).fetch(**behavior)
@@ -279,33 +296,50 @@
 class Fetch1(FetchBase, Callable):
     """
     Fetch object for fetching exactly one row.
 
     :param relation: relation the fetch object fetches data from
     """
 
-    def __call__(self, *attrs, **kwargs):
+    def __call__(self, *attrs, squeeze=False):
         """
-        This version of fetch is called when self is expected to contain exactly one tuple.
+        Fetches the query results from the database when the query is known to contain only one entry.
+
+        If no attributes are specified, returns the result as a dict.
+        If attributes are specified returns the corresponding results as a tuple.
+
+        Examples:
+        d = rel.fetch1()   # as a dictionary
+        a, b = rel.fetch1('a', 'b')   # as a tuple
+
+        :params *attrs: attributes to return when expanding into a tuple. If empty, the return result is a dict
+        :param squeeze:  When true, remove extra dimensions from arrays in attributes
         :return: the one tuple in the relation in the form of a dict
         """
+
         heading = self._relation.heading
-        ext_behavior = update_dict(self.ext_behavior, kwargs)
-        unpack_ = partial(unpack, squeeze=ext_behavior['squeeze'])
+        squeeze = squeeze or self.ext_behavior['squeeze']  # for backward compatibility
+        unpack_ = partial(unpack, squeeze=squeeze)
 
-        if len(attrs) == 0:  # fetch all attributes
+        if not attrs:  # fetch all attributes, return as ordered dict
             cur = self._relation.cursor(as_dict=True)
             ret = cur.fetchone()
             if not ret or cur.fetchone():
                 raise DataJointError('fetch1 should only be used for relations with exactly one tuple')
-            ret = OrderedDict((name, unpack_(ret[name]) if heading[name].is_blob else ret[name])
-                               for name in heading.names)
-        else:
+
+            def get_external(attr, _hash):
+                return self._relation.connection.schemas[attr.database].external_table.get(_hash)
+
+            ret = OrderedDict((name, get_external(heading[name], ret[name])) if heading[name].is_external
+                              else (name, unpack_(ret[name]) if heading[name].is_blob else ret[name])
+                              for name in heading.names)
+
+        else:  # fetch some attributes, return as tuple
             attributes = [a for a in attrs if a is not PRIMARY_KEY]
-            result = self._relation.proj(*attributes).fetch(**ext_behavior)
+            result = self._relation.proj(*attributes).fetch(squeeze=squeeze)
             if len(result) != 1:
                 raise DataJointError('fetch1 should only return one tuple. %d tuples were found' % len(result))
             return_values = tuple(
                 next(to_dicts(result[self._relation.primary_key]))
                 if attribute is PRIMARY_KEY else result[attribute][0]
                 for attribute in attrs)
             ret = return_values[0] if len(attrs) == 1 else return_values
```

### Comparing `datajoint-0.8.2/datajoint/heading.py` & `datajoint-0.9.0/datajoint/heading.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import logging
 from . import DataJointError
 
 logger = logging.getLogger(__name__)
 
 default_attribute_properties = dict(    # these default values are set in computed attributes
     name=None, type='expression', in_key=False, nullable=False, default=None, comment='calculated attribute',
-    autoincrement=False, numeric=None, string=None, is_blob=False, sql_expression=None, dtype=object)
+    autoincrement=False, numeric=None, string=None, is_blob=False, is_external=False, sql_expression=None,
+    database=None, dtype=object)
 
 
 class Attribute(namedtuple('_Attribute', default_attribute_properties.keys())):
     """
     Properties of a table column (attribute)
     """
     def todict(self):
@@ -20,14 +21,15 @@
         return OrderedDict((name, self[i]) for i, name in enumerate(self._fields))
 
     @property
     def sql(self):
         """
         Convert primary key attribute tuple into its SQL CREATE TABLE clause.
         Default values are not reflected.
+        This is used for declaring foreign keys in referencing tables
         :return: SQL code
         """
         assert self.in_key and not self.nullable   # primary key attributes are never nullable
         return '`{name}` {type} NOT NULL COMMENT "{comment}"'.format(
             name=self.name, type=self.type, comment=self.comment)
 
 
@@ -78,14 +80,17 @@
         return [k for k, v in self.attributes.items() if v.sql_expression is not None]
 
     def __getitem__(self, name):
         """shortcut to the attribute"""
         return self.attributes[name]
 
     def __repr__(self):
+        """
+        :return:  heading representation in DataJoint declaration format but without foreign key expansion
+        """
         if self.attributes is None:
             return 'heading not loaded'
         in_key = True
         ret = ''
         if self.table_info:
             ret += '# ' + self.table_info['comment'] + '\n'
         for v in self.attributes.values():
@@ -111,18 +116,17 @@
             formats=[v.dtype for v in self.attributes.values()]))
 
     @property
     def as_sql(self):
         """
         represent heading as SQL field list
         """
-        return ','.join(['`%s`' % name
-                         if self.attributes[name].sql_expression is None
-                         else '%s as `%s`' % (self.attributes[name].sql_expression, name)
-                         for name in self.names])
+        return ','.join('`%s`' % name if self.attributes[name].sql_expression is None
+                        else '%s as `%s`' % (self.attributes[name].sql_expression, name)
+                        for name in self.names)
 
     def __iter__(self):
         return iter(self.attributes)
 
     def init_from_database(self, conn, database, table_name):
         """
         initialize heading from a database table.  The table must exist already.
@@ -176,21 +180,29 @@
             ('bigint', True): np.uint64
             }
 
         sql_literals = ['CURRENT_TIMESTAMP']
 
         # additional attribute properties
         for attr in attributes:
+            # process external attributes
+            split_comment = attr['comment'].split(':')
+            attr['is_external'] = len(split_comment) >= 3 and split_comment[1].startswith('external')
+            if attr['is_external']:
+                attr['comment'] = ':'.join(split_comment[2:])
+                attr['type'] = split_comment[1]
+
             attr['nullable'] = (attr['nullable'] == 'YES')
             attr['in_key'] = (attr['in_key'] == 'PRI')
             attr['autoincrement'] = bool(re.search(r'auto_increment', attr['Extra'], flags=re.IGNORECASE))
             attr['type'] = re.sub(r'int\(\d+\)', 'int', attr['type'], count=1)   # strip size off integers
             attr['numeric'] = bool(re.match(r'(tiny|small|medium|big)?int|decimal|double|float', attr['type']))
             attr['string'] = bool(re.match(r'(var)?char|enum|date|year|time|timestamp', attr['type']))
-            attr['is_blob'] = bool(re.match(r'(tiny|medium|long)?blob', attr['type']))
+            attr['is_blob'] = attr['is_external'] or bool(re.match(r'(tiny|medium|long)?blob', attr['type']))
+            attr['database'] = database
 
             if attr['string'] and attr['default'] is not None and attr['default'] not in sql_literals:
                 attr['default'] = '"%s"' % attr['default']
 
             if attr['nullable']:   # nullable fields always default to null
                 attr['default'] = 'null'
```

### Comparing `datajoint-0.8.2/datajoint/jobs.py` & `datajoint-0.9.0/datajoint/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-import hashlib
+from .hash import key_hash
 import os
 import pymysql
 from .base_relation import BaseRelation
 from . import DataJointError
 
 ERROR_MESSAGE_LENGTH = 2047
 TRUNCATION_APPENDIX = '...truncated'
 
 
-def key_hash(key):
-    """
-    32-byte hash used for lookup of primary keys of jobs
-    """
-    hashed = hashlib.md5()
-    for k, v in sorted(key.items()):
-        hashed.update(str(v).encode())
-    return hashed.hexdigest()
-
-
 class JobTable(BaseRelation):
     """
     A base relation with no definition. Allows reserving jobs
     """
     def __init__(self, arg, database=None):
         if isinstance(arg, JobTable):
             super().__init__(arg)
@@ -96,41 +86,30 @@
         Log a completed job.  When a job is completed, its reservation entry is deleted.
         :param table_name: `database`.`table_name`
         :param key: the dict of the job's primary key
         """
         job_key = dict(table_name=table_name, key_hash=key_hash(key))
         (self & job_key).delete_quick()
 
-    def error(self, table_name, key, error_message):
+    def error(self, table_name, key, error_message, error_stack=None):
         """
         Log an error message.  The job reservation is replaced with an error entry.
         if an error occurs, leave an entry describing the problem
         :param table_name: `database`.`table_name`
         :param key: the dict of the job's primary key
         :param error_message: string error message
+        :param error_stack: stack trace
         """
         if len(error_message) > ERROR_MESSAGE_LENGTH:
             error_message = error_message[:ERROR_MESSAGE_LENGTH-len(TRUNCATION_APPENDIX)] + TRUNCATION_APPENDIX
         job_key = dict(table_name=table_name, key_hash=key_hash(key))
         self.insert1(
             dict(job_key,
                  status="error",
                  host=os.uname().nodename,
                  pid=os.getpid(),
                  connection_id=self.connection.connection_id,
                  user=self._user,
                  key=key,
-                 error_message=error_message), replace=True, ignore_extra_fields=True)
-
-
-class JobManager:
-    """
-    A container for all job tables (one job table per schema).
-    """
-    def __init__(self, connection):
-        self.connection = connection
-        self._jobs = {}
-
-    def __getitem__(self, database):
-        if database not in self._jobs:
-            self._jobs[database] = JobTable(self.connection, database)
-        return self._jobs[database]
+                 error_message=error_message,
+                 error_stack=error_stack),
+            replace=True, ignore_extra_fields=True)
```

### Comparing `datajoint-0.8.2/datajoint/relational_operand.py` & `datajoint-0.9.0/datajoint/relational_operand.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import collections
-from itertools import zip_longest
+from itertools import zip_longest, count
 import logging
 import numpy as np
 import re
 import datetime
 import decimal
 from . import DataJointError, config
 from .fetch import Fetch, Fetch1
@@ -33,45 +33,79 @@
     or_lists = (list, set, tuple, np.ndarray)
     return (arg is None or (isinstance(arg, AndList) and any(restricts_to_empty(r) for r in arg)) or
             arg is None or arg is False or equal_ignore_case(arg, "FALSE") or
             isinstance(arg, or_lists) and len(arg) == 0 or  # empty OR-list equals FALSE
             isinstance(arg, Not) and restricts_to_same(arg.restriction))
 
 
-class AndList(list):
+class OrList(list):
     """
-    A list of restrictions to by applied to a relation.  The restrictions are AND-ed.
-    Each restriction can be a list or set or a relation whose elements are OR-ed.
-    But the elements that are lists can contain other AndLists.
+    A list of conditions to restrict a relation.  The conditions are OR-ed.
+    If any restriction is True, then the overall condition is True.
+    Each condition can be a AndList.
 
     Example:
-    rel2 = rel & dj.AndList((cond1, cond2, cond3))
+    rel2 = rel & dj.ORList((cond1, cond2, cond3))
     is equivalent to
-    rel2 = rel & cond1 & cond2 & cond3
+    rel2 = rel & [cond1, cond2, cond3]
     """
 
-    def simplify(self):
-        return self[0] if len(self) == 1 else self
+    @staticmethod
+    def _recurse(other):
+        for item in other:
+            if isinstance(item, OrList):
+                yield from OrList._recurse(item)  # flatten list
+            else:
+                if not isinstance(item, AndList):
+                    yield item
+                elif len(item) == 0:
+                    yield True
+                elif len(item) == 1:
+                    if isinstance(item[0], OrList):
+                        OrList._recurse(item[0])
+                    else:
+                        yield item[0]
+                else:
+                    yield item
 
+    def __init__(self, other):
+        lst = list(self._recurse(other))
+        super().__init__([True] if any(i is True for i in lst) else lst)
 
-class OrList(list):
+
+class AndList(list):
     """
-    A list of restrictions to by applied to a relation.  The restrictions are OR-ed.
-    If any restriction is .
+    A list of restrictions to by applied to a relation.  The restrictions are AND-ed.
+    Each restriction can be a list or set or a relation whose elements are OR-ed.
     But the elements that are lists can contain other AndLists.
 
     Example:
-    rel2 = rel & dj.ORList((cond1, cond2, cond3))
+    rel2 = rel & dj.AndList((cond1, cond2, cond3))
     is equivalent to
-    rel2 = rel & [cond1, cond2, cond3]
-
-    Since ORList is just an alias for list, it is not necessary and is only provided
-    for consistency with AndList.
+    rel2 = rel & cond1 & cond2 & cond3
     """
-    pass
+
+    def set(self, items):
+        self.clear()
+        self.append(items)
+
+    def append(self, item):
+        # append item, reducing nesting
+        if isinstance(item, AndList):
+            self.extend(item)
+        elif isinstance(item, OrList):
+            if not item:  # an empty OrList is equivalent to False
+                super().append(False)
+            else:  # an OrList with one element is equivalent to the element
+                super().append(item[0] if len(item) == 1 else item)
+        else:
+            super().append(item)
+        # an AndList with a False in it is False
+        if len(self) > 1 and any(i is False for i in self):
+            self.set(False)
 
 
 class RelationalOperand:
     """
     RelationalOperand implements the relational algebra.
     RelationalOperand objects link other relational operands with relational operators.
     The leaves of this tree of objects are base relations.
@@ -138,14 +172,16 @@
         """
 
         def make_condition(arg, _negate=False):
             if isinstance(arg, str):
                 return arg, _negate
             elif isinstance(arg, AndList):
                 return '(' + ' AND '.join([make_condition(element)[0] for element in arg]) + ')', _negate
+            elif isinstance(arg, bool):
+                return 'FALSE' if _negate == arg else 'TRUE', False
             # semijoin or antijoin
             elif isinstance(arg, RelationalOperand):
                 common_attributes = [q for q in self.heading.names if q in arg.heading.names]
                 if not common_attributes:
                     condition = 'FALSE' if _negate else 'TRUE'
                 else:
                     condition = '({fields}) {not_}in ({subquery})'.format(
@@ -197,14 +233,20 @@
 
     def __mul__(self, other):
         """
         natural join of relations self and other
         """
         return other * self if isinstance(other, U) else Join.create(self, other)
 
+    def __add__(self, other):
+        """
+        union of relations
+        """
+        return Union.create(self, other)
+
     def proj(self, *attributes, **named_attributes):
         """
         Relational projection operator.
         :param attributes:  attributes to be included in the result. (The primary key is already included).
         :param named_attributes: new attributes computed or renamed from existing attributes.
         :return: the projected relation.
         Primary key attributes are always cannot be excluded but may be renamed.
@@ -309,21 +351,30 @@
 
         relational_operand.restrict is the only access point that modifies restrictions. All other operators must
         ultimately call restrict()
 
         :param restriction: a sequence or an array (treated as OR list), another relation, an SQL condition string, or
             an AndList.
         """
+        assert not self.heading.expressions or isinstance(self, GroupBy), "Cannot restrict in place" \
+                                                                          " a projection with renamed attributes."
         if not restricts_to_same(restriction):
-            assert not self.heading.expressions or isinstance(self, GroupBy), \
-                "Cannot restrict in place a projection with renamed attributes."
-            if isinstance(restriction, AndList):
-                self.restrictions.extend(restriction)
+            self.restrictions.append(restriction)
+        elif restricts_to_empty(restriction):
+            self.restrictions.set(False)
+        return self
+
+    def allow(self, arg):
+        assert not self.heading.expressions or isinstance(self, GroupBy), "Cannot restrict in place" \
+                                                                          " a projection with renamed attributes."
+        if self.restrictions:
+            if restricts_to_same(arg):
+                self.restrictions.clear()
             else:
-                self.restrictions.append(restriction)
+                self.restrictions.set(OrList([self.restrictions, arg]))
         return self
 
     @property
     def fetch1(self):
         return Fetch1(self)
 
     @property
@@ -556,17 +607,66 @@
     def from_clause(self):
         return '{from1} NATURAL{left} JOIN {from2}'.format(
             from1=self._arg1.from_clause,
             left=" LEFT" if self._left else "",
             from2=self._arg2.from_clause)
 
 
+class Union(RelationalOperand):
+    """
+    Union is a private DataJoint class that implements relational union.
+    """
+
+    __count = count()
+
+    def __init__(self, arg=None):
+        super().__init__(arg)
+        if arg is not None:
+            assert isinstance(arg, Union), "Union copy constructore requires a Union object"
+            self._connection = arg.connection
+            self._heading = arg.heading
+            self._arg1 = arg._arg1
+            self._arg2 = arg._arg2
+
+    @classmethod
+    def create(cls, arg1, arg2):
+        obj = cls()
+        if not isinstance(arg1, RelationalOperand) or not isinstance(arg2, RelationalOperand):
+            raise DataJointError('a relation can only be unioned with another relation')
+        if arg1.connection != arg2.connection:
+            raise DataJointError("Cannot operate on relations from different connections.")
+        if set(arg1.heading.names) != set(arg2.heading.names):
+            raise DataJointError('Union requires the same attributes in both arguments')
+        if any(not v.in_key for v in arg1.heading.attributes.values()) or \
+                all(not v.in_key for v in arg2.heading.attributes.values()):
+            raise DataJointError('Union arguments must not have any secondary attributes.')
+        obj._connection = arg1.connection
+        obj._heading = arg1.heading
+        obj._arg1 = arg1
+        obj._arg2 = arg2
+        return obj
+
+    def make_sql(self, select_fields=None):
+        return "SELECT {_fields} FROM {_from}{_where}".format(
+            _fields=self.get_select_fields(select_fields),
+            _from=self.from_clause,
+            _where=self.where_clause)
+
+    @property
+    def from_clause(self):
+        return ("(SELECT {fields} FROM {from1}{where1} UNION SELECT {fields} FROM {from2}{where2}) as `_u%x`".format(
+            fields=self.get_select_fields(None), from1=self._arg1.from_clause,
+            where1=self._arg1.where_clause,
+            from2=self._arg2.from_clause,
+            where2=self._arg2.where_clause)) % next(self.__count)
+
+
 class Projection(RelationalOperand):
     """
-    Projection is an private DataJoint class that implements relational projection.
+    Projection is a private DataJoint class that implements relational projection.
     See RelationalOperand.proj() for user interface.
     """
 
     def __init__(self, arg=None):
         super().__init__(arg)
         if arg is not None:
             assert isinstance(arg, Projection), "Projection copy constructor requires a Projection object."
@@ -673,15 +773,15 @@
 
 class Subquery(RelationalOperand):
     """
     A Subquery encapsulates its argument in a SELECT statement, enabling its use as a subquery.
     The attribute list and the WHERE clause are resolved.  Thus, a subquery no longer has any renamed attributes.
     A subquery of a subquery is a just a copy of the subquery with no change in SQL.
     """
-    __counter = 0
+    __count = count()
 
     def __init__(self, arg=None):
         super().__init__(arg)
         if arg is not None:
             # copy constructor
             assert isinstance(arg, Subquery)
             self._connection = arg.connection
@@ -696,21 +796,16 @@
         obj = cls()
         obj._connection = arg.connection
         obj._heading = arg.heading.make_subquery_heading()
         obj._arg = arg
         return obj
 
     @property
-    def counter(self):
-        Subquery.__counter += 1
-        return Subquery.__counter
-
-    @property
     def from_clause(self):
-        return '(' + self._arg.make_sql() + ') as `_s%x`' % self.counter
+        return '(' + self._arg.make_sql() + ') as `_s%x`' % next(self.__count)
 
     def get_select_fields(self, select_fields=None):
         return '*' if select_fields is None else self.heading.project(select_fields).as_sql
 
 
 class U:
     """
```

### Comparing `datajoint-0.8.2/datajoint/s3.py` & `datajoint-0.9.0/datajoint/s3.py`

 * *Files identical despite different names*

### Comparing `datajoint-0.8.2/datajoint/schema.py` & `datajoint-0.9.0/datajoint/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import warnings
 import pymysql
 import logging
 import inspect
 import re
 from . import conn, DataJointError, config
 from .erd import ERD
+from .jobs import JobTable
+from .external import ExternalTable
 from .heading import Heading
 from .utils import user_choice, to_camel_case
 from .user_relations import Part, Computed, Imported, Manual, Lookup
 from .base_relation import lookup_class_name, Log
 
 logger = logging.getLogger(__name__)
 
@@ -16,23 +18,20 @@
 def ordered_dir(klass):
     """
     List (most) attributes of the class including inherited ones, similar to `dir` build-in function,
     but respects order of attribute declaration as much as possible.
     :param klass: class to list members for
     :return: a list of attributes declared in klass and its superclasses
     """
-    m = []
-    mro = klass.mro()
-    for c in mro:
-        if hasattr(c, '_ordered_class_members'):
-            elements = c._ordered_class_members
-        else:
-            elements = c.__dict__.keys()
-        m = [e for e in elements if e not in m] + m
-    return m
+    attr_list = list()
+    for c in reversed(klass.mro()):
+        attr_list.extend(e for e in (
+            c._ordered_class_members if hasattr(c, '_ordered_class_members') else
+            c.__dict__.keys()) if e not in attr_list)
+    return attr_list
 
 
 class Schema:
     """
     A schema object is a decorator for UserRelation classes that binds them to their database.
     It also specifies the namespace `context` in which other UserRelation classes are defined.
     """
@@ -49,14 +48,16 @@
         if connection is None:
             connection = conn()
         self._log = None
         self.database = database
         self.connection = connection
         self.context = context
         self.create_tables = create_tables
+        self._jobs = None
+        self._external = None
         if not self.exists:
             if not self.create_tables:
                 raise DataJointError("Database named `{database}` was not defined. "
                                      "Set the create_tables flag to create it.".format(database=database))
             else:
                 # create database
                 logger.info("Database `{database}` could not be found. "
@@ -209,18 +210,29 @@
                     self.process_relation_class(part, context=dict(self.context, **ext))
         return cls
 
     @property
     def jobs(self):
         """
         schema.jobs provides a view of the job reservation table for the schema
-        :return: jobs relation
+        :return: jobs table
         """
-        return self.connection.jobs[self.database]
+        if self._jobs is None:
+            self._jobs = JobTable(self.connection, self.database)
+        return self._jobs
+
+    @property
+    def external_table(self):
+        """
+        schema.external provides a view of the external hash table for the schema
+        :return: external table
+        """
+        if self._external is None:
+            self._external = ExternalTable(self.connection, self.database)
+        return self._external
 
     def erd(self):
         # get the caller's locals()
         import inspect
         frame = inspect.currentframe()
         context = frame.f_back.f_locals
         return ERD(self, context=context)
-
```

### Comparing `datajoint-0.8.2/datajoint/settings.py` & `datajoint-0.9.0/datajoint/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 }
 prefix_to_role = dict(zip(role_to_prefix.values(), role_to_prefix.keys()))
 
 
 server_error_codes = {
     'unknown column': 1054,
     'command denied': 1142,
-    'tables does not exist': 1146,
+    'table does not exist': 1146,
     'syntax error': 1149,
     'duplicate entry': 1062,
 }
 
 
 default = OrderedDict({
     'database.host': 'localhost',
@@ -172,13 +172,11 @@
             self._conf.update(dict(*args, **kwargs))  # use the free update to set keys
 
         def __getitem__(self, key):
             return self._conf[key]
 
         def __setitem__(self, key, value):
             logger.log(logging.INFO, u"Setting {0:s} to {1:s}".format(str(key), str(value)))
-            if isinstance(value, collections.Mapping):
-                raise ValueError("Nested settings are not supported!")
             if validators[key](value):
                 self._conf[key] = value
             else:
                 raise DataJointError(u'Validator for {0:s} did not pass'.format(key, ))
```

### Comparing `datajoint-0.8.2/datajoint/user_relations.py` & `datajoint-0.9.0/datajoint/user_relations.py`

 * *Files identical despite different names*

### Comparing `datajoint-0.8.2/datajoint/utils.py` & `datajoint-0.9.0/datajoint/utils.py`

 * *Files identical despite different names*

### Comparing `datajoint-0.8.2/datajoint.egg-info/SOURCES.txt` & `datajoint-0.9.0/datajoint.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 datajoint/autopopulate.py
 datajoint/base_relation.py
 datajoint/blob.py
 datajoint/connection.py
 datajoint/declare.py
 datajoint/dependencies.py
 datajoint/erd.py
+datajoint/external.py
 datajoint/fetch.py
 datajoint/hash.py
 datajoint/heading.py
 datajoint/jobs.py
 datajoint/relational_operand.py
 datajoint/s3.py
 datajoint/schema.py
```

### Comparing `datajoint-0.8.2/LICENSE.txt` & `datajoint-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datajoint-0.8.2/setup.py` & `datajoint-0.9.0/setup.py`

 * *Files identical despite different names*

