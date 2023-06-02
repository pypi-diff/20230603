# Comparing `tmp/PyOdoo-0.5.8.tar.gz` & `tmp/PyOdoo-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOdoo-0.5.8.tar", last modified: Mon May 15 23:54:18 2023, max compression
+gzip compressed data, was "PyOdoo-0.5.9.tar", last modified: Wed May 17 21:33:39 2023, max compression
```

## Comparing `PyOdoo-0.5.8.tar` & `PyOdoo-0.5.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/
--rw-r--r--   0 muflone   (1000) users      (985)      613 2021-05-09 18:22:23.000000 PyOdoo-0.5.8/LICENSE
--rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/PKG-INFO
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/PyOdoo.egg-info/
--rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/PKG-INFO
--rw-r--r--   0 muflone   (1000) users      (985)      552 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/SOURCES.txt
--rw-r--r--   0 muflone   (1000) users      (985)        1 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/dependency_links.txt
--rw-r--r--   0 muflone   (1000) users      (985)        7 2023-05-15 23:54:18.000000 PyOdoo-0.5.8/PyOdoo.egg-info/top_level.txt
--rw-r--r--   0 muflone   (1000) users      (985)     1014 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/README.md
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/pyodoo/
--rw-r--r--   0 muflone   (1000) users      (985)     1306 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)     1004 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/active_status_choice.py
--rw-r--r--   0 muflone   (1000) users      (985)      956 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/boolean_operator.py
--rw-r--r--   0 muflone   (1000) users      (985)     1365 2023-05-15 23:49:57.000000 PyOdoo-0.5.8/pyodoo/compare_type.py
--rw-r--r--   0 muflone   (1000) users      (985)     1227 2023-05-13 15:49:56.000000 PyOdoo-0.5.8/pyodoo/constants.py
--rw-r--r--   0 muflone   (1000) users      (985)     1502 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/filter.py
--rw-r--r--   0 muflone   (1000) users      (985)     1008 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/message_subtype.py
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/pyodoo/samples/
--rw-r--r--   0 muflone   (1000) users      (985)        0 2022-09-23 22:59:11.000000 PyOdoo-0.5.8/pyodoo/samples/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)     1345 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/samples/awaitable.py
--rw-r--r--   0 muflone   (1000) users      (985)     5169 2023-03-19 10:57:46.000000 PyOdoo-0.5.8/pyodoo/samples/contacts.py
--rw-r--r--   0 muflone   (1000) users      (985)     3666 2023-02-05 16:20:33.000000 PyOdoo-0.5.8/pyodoo/samples/contacts_async.py
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.492088 PyOdoo-0.5.8/pyodoo/v12/
--rw-r--r--   0 muflone   (1000) users      (985)      986 2023-02-05 04:31:04.000000 PyOdoo-0.5.8/pyodoo/v12/__init__.py
--rw-r--r--   0 muflone   (1000) users      (985)    11089 2023-02-05 18:02:47.000000 PyOdoo-0.5.8/pyodoo/v12/api.py
--rw-r--r--   0 muflone   (1000) users      (985)    32118 2023-03-19 10:22:52.000000 PyOdoo-0.5.8/pyodoo/v12/model.py
--rw-r--r--   0 muflone   (1000) users      (985)       90 2022-01-06 22:44:31.000000 PyOdoo-0.5.8/pyproject.toml
--rw-r--r--   0 muflone   (1000) users      (985)      883 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/setup.cfg
-drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-15 23:54:18.495422 PyOdoo-0.5.8/tests/
--rw-r--r--   0 muflone   (1000) users      (985)    16600 2023-05-15 23:49:57.000000 PyOdoo-0.5.8/tests/test_compare_types.py
--rw-r--r--   0 muflone   (1000) users      (985)    33179 2023-05-13 16:57:45.000000 PyOdoo-0.5.8/tests/test_contacts.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/
+-rw-r--r--   0 muflone   (1000) users      (985)      613 2021-05-09 18:22:23.000000 PyOdoo-0.5.9/LICENSE
+-rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/PKG-INFO
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.660327 PyOdoo-0.5.9/PyOdoo.egg-info/
+-rw-r--r--   0 muflone   (1000) users      (985)     1762 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/PKG-INFO
+-rw-r--r--   0 muflone   (1000) users      (985)      552 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/SOURCES.txt
+-rw-r--r--   0 muflone   (1000) users      (985)        1 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/dependency_links.txt
+-rw-r--r--   0 muflone   (1000) users      (985)        7 2023-05-17 21:33:39.000000 PyOdoo-0.5.9/PyOdoo.egg-info/top_level.txt
+-rw-r--r--   0 muflone   (1000) users      (985)     1014 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/README.md
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.660327 PyOdoo-0.5.9/pyodoo/
+-rw-r--r--   0 muflone   (1000) users      (985)     1306 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1004 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/active_status_choice.py
+-rw-r--r--   0 muflone   (1000) users      (985)      956 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/boolean_operator.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1365 2023-05-15 23:49:57.000000 PyOdoo-0.5.9/pyodoo/compare_type.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1227 2023-05-17 21:21:43.000000 PyOdoo-0.5.9/pyodoo/constants.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1502 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/filter.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1008 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/message_subtype.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/pyodoo/samples/
+-rw-r--r--   0 muflone   (1000) users      (985)        0 2022-09-23 22:59:11.000000 PyOdoo-0.5.9/pyodoo/samples/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)     1345 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/samples/awaitable.py
+-rw-r--r--   0 muflone   (1000) users      (985)     5169 2023-03-19 10:57:46.000000 PyOdoo-0.5.9/pyodoo/samples/contacts.py
+-rw-r--r--   0 muflone   (1000) users      (985)     3666 2023-02-05 16:20:33.000000 PyOdoo-0.5.9/pyodoo/samples/contacts_async.py
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/pyodoo/v12/
+-rw-r--r--   0 muflone   (1000) users      (985)      986 2023-02-05 04:31:04.000000 PyOdoo-0.5.9/pyodoo/v12/__init__.py
+-rw-r--r--   0 muflone   (1000) users      (985)    11089 2023-02-05 18:02:47.000000 PyOdoo-0.5.9/pyodoo/v12/api.py
+-rw-r--r--   0 muflone   (1000) users      (985)    31145 2023-05-17 21:27:30.000000 PyOdoo-0.5.9/pyodoo/v12/model.py
+-rw-r--r--   0 muflone   (1000) users      (985)       90 2022-01-06 22:44:31.000000 PyOdoo-0.5.9/pyproject.toml
+-rw-r--r--   0 muflone   (1000) users      (985)      883 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/setup.cfg
+drwxr-xr-x   0 muflone   (1000) users      (985)        0 2023-05-17 21:33:39.663660 PyOdoo-0.5.9/tests/
+-rw-r--r--   0 muflone   (1000) users      (985)    16600 2023-05-15 23:49:57.000000 PyOdoo-0.5.9/tests/test_compare_types.py
+-rw-r--r--   0 muflone   (1000) users      (985)    33179 2023-05-17 21:28:14.000000 PyOdoo-0.5.9/tests/test_contacts.py
```

### Comparing `PyOdoo-0.5.8/LICENSE` & `PyOdoo-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/PKG-INFO` & `PyOdoo-0.5.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOdoo
-Version: 0.5.8
+Version: 0.5.9
 Summary: API for Odoo
 Home-page: http://www.muflone.com/pyodoo/
 Author: Fabio Castelli
 Author-email: muflone@muflone.com
 License: GPLv3+
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `PyOdoo-0.5.8/PyOdoo.egg-info/PKG-INFO` & `PyOdoo-0.5.9/PyOdoo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOdoo
-Version: 0.5.8
+Version: 0.5.9
 Summary: API for Odoo
 Home-page: http://www.muflone.com/pyodoo/
 Author: Fabio Castelli
 Author-email: muflone@muflone.com
 License: GPLv3+
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `PyOdoo-0.5.8/PyOdoo.egg-info/SOURCES.txt` & `PyOdoo-0.5.9/PyOdoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/README.md` & `PyOdoo-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/__init__.py` & `PyOdoo-0.5.9/pyodoo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/active_status_choice.py` & `PyOdoo-0.5.9/pyodoo/active_status_choice.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/boolean_operator.py` & `PyOdoo-0.5.9/pyodoo/boolean_operator.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/compare_type.py` & `PyOdoo-0.5.9/pyodoo/compare_type.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/constants.py` & `PyOdoo-0.5.9/pyodoo/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ##
 
 APP_NAME = 'PyOdoo'
-APP_VERSION = '0.5.8'
+APP_VERSION = '0.5.9'
 APP_DESCRIPTION = 'API for Odoo'
 APP_DOMAIN = 'pyodoo'
 APP_ID = f'{APP_DOMAIN}.muflone.com'
 APP_AUTHOR = 'Fabio Castelli'
 APP_AUTHOR_EMAIL = 'muflone@muflone.com'
 APP_COPYRIGHT = f'Copyright 2021-2023 {APP_AUTHOR}'
 URL_AUTHOR = 'http://www.muflone.com/'
```

### Comparing `PyOdoo-0.5.8/pyodoo/filter.py` & `PyOdoo-0.5.9/pyodoo/filter.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/message_subtype.py` & `PyOdoo-0.5.9/pyodoo/message_subtype.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/samples/awaitable.py` & `PyOdoo-0.5.9/pyodoo/samples/awaitable.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/samples/contacts.py` & `PyOdoo-0.5.9/pyodoo/samples/contacts.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/samples/contacts_async.py` & `PyOdoo-0.5.9/pyodoo/samples/contacts_async.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/v12/__init__.py` & `PyOdoo-0.5.9/pyodoo/v12/__init__.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/v12/api.py` & `PyOdoo-0.5.9/pyodoo/v12/api.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/pyodoo/v12/model.py` & `PyOdoo-0.5.9/pyodoo/v12/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,71 +135,49 @@
                                limit=1,
                                offset=0)
         return results[0] if results else None
 
     def get(self,
             entity_id: int,
             fields: tuple[str, ...] = None,
-            options: dict[str, Any] = None,
-            limit: Optional[int] = None,
-            offset: Optional[int] = None,
-            order: Optional[str] = None) -> Optional[dict[str, Any]]:
+            options: dict[str, Any] = None) -> Optional[dict[str, Any]]:
         """
         Get a row from a model using its ID
 
         :param entity_id: Object ID to query
         :param fields: Tuple with the fields to include in the response
         :param options: Dictionary with options to use
-        :param limit: Maximum number of results count
-        :param offset: Starting record number to fetch the data
-        :param order: Ordering clause
         :return: Dictionary with the requested fields
         """
         results = self.get_many(entity_ids=[entity_id],
                                 fields=fields,
-                                options=options,
-                                limit=limit,
-                                offset=offset,
-                                order=order)
+                                options=options)
         return results[0] if results else None
 
     def get_many(self,
                  entity_ids: list[int],
                  fields: tuple[str, ...] = None,
-                 options: dict[str, Any] = None,
-                 limit: Optional[int] = None,
-                 offset: Optional[int] = None,
-                 order: Optional[str] = None
+                 options: dict[str, Any] = None
                  ) -> Optional[list[dict[str, Any]]]:
         """
         Get a row from a model using its ID
 
         :param entity_ids: Object IDs to query
         :param fields: Tuple with the fields to include in the response
         :param options: Dictionary with options to use
-        :param limit: Maximum number of results count
-        :param offset: Starting record number to fetch the data
-        :param order: Ordering clause
         :return: List of dictionaries with the requested fields
         """
         # Set options
         if options is None:
             options = {}
         # Limit results only to selected fields
         if fields:
             options['fields'] = fields
         # Set language for translated fields
         self._set_options_language(options=options)
-        # Set pagination
-        self._set_pagination(options=options,
-                             limit=limit,
-                             offset=offset)
-        # Set order
-        self._set_order_by(options=options,
-                           order=order)
         # Request data and get results
         results = self.api.do_read_many(entity_ids=entity_ids,
                                         options=options)
         return results
 
     def all(self,
             is_active: ActiveStatusChoice = ActiveStatusChoice.NOT_SET,
```

### Comparing `PyOdoo-0.5.8/setup.cfg` & `PyOdoo-0.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/tests/test_compare_types.py` & `PyOdoo-0.5.9/tests/test_compare_types.py`

 * *Files identical despite different names*

### Comparing `PyOdoo-0.5.8/tests/test_contacts.py` & `PyOdoo-0.5.9/tests/test_contacts.py`

 * *Files identical despite different names*

