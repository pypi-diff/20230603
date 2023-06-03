# Comparing `tmp/python-canvas-0.3.5.tar.gz` & `tmp/python-canvas-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-canvas-0.3.5.tar", last modified: Sat Jun  3 14:57:29 2023, max compression
+gzip compressed data, was "python-canvas-0.3.6.tar", last modified: Sat Jun  3 15:03:13 2023, max compression
```

## Comparing `python-canvas-0.3.5.tar` & `python-canvas-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 14:57:29.179999 python-canvas-0.3.5/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-06-03 14:39:28.000000 python-canvas-0.3.5/LICENSE
--rw-r--r--   0 user      (1000) user      (1001)      949 2023-06-03 14:57:29.179999 python-canvas-0.3.5/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      422 2023-06-03 14:39:28.000000 python-canvas-0.3.5/README.md
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 14:57:29.179999 python-canvas-0.3.5/canvas_db/
--rw-r--r--   0 user      (1000) user      (1001)        0 2023-06-03 14:39:28.000000 python-canvas-0.3.5/canvas_db/__init__.py
--rw-r--r--   0 user      (1000) user      (1001)      214 2023-06-03 14:39:28.000000 python-canvas-0.3.5/canvas_db/config.py
--rw-r--r--   0 user      (1000) user      (1001)    73935 2023-06-03 14:55:16.000000 python-canvas-0.3.5/canvas_db/models.py
--rw-r--r--   0 user      (1000) user      (1001)      501 2023-06-03 14:39:28.000000 python-canvas-0.3.5/canvas_db/orm.py
-drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 14:57:29.179999 python-canvas-0.3.5/python_canvas.egg-info/
--rw-r--r--   0 user      (1000) user      (1001)      949 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1001)      289 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1001)        1 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1001)       20 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1001)       10 2023-06-03 14:57:29.000000 python-canvas-0.3.5/python_canvas.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1001)       38 2023-06-03 14:57:29.179999 python-canvas-0.3.5/setup.cfg
--rw-r--r--   0 user      (1000) user      (1001)      815 2023-06-03 14:55:30.000000 python-canvas-0.3.5/setup.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 15:03:13.133333 python-canvas-0.3.6/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-06-03 14:39:28.000000 python-canvas-0.3.6/LICENSE
+-rw-r--r--   0 user      (1000) user      (1001)      949 2023-06-03 15:03:13.133333 python-canvas-0.3.6/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      422 2023-06-03 14:39:28.000000 python-canvas-0.3.6/README.md
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 15:03:13.133333 python-canvas-0.3.6/canvas_db/
+-rw-r--r--   0 user      (1000) user      (1001)        0 2023-06-03 14:39:28.000000 python-canvas-0.3.6/canvas_db/__init__.py
+-rw-r--r--   0 user      (1000) user      (1001)      214 2023-06-03 14:39:28.000000 python-canvas-0.3.6/canvas_db/config.py
+-rw-r--r--   0 user      (1000) user      (1001)    73935 2023-06-03 15:02:40.000000 python-canvas-0.3.6/canvas_db/models.py
+-rw-r--r--   0 user      (1000) user      (1001)      501 2023-06-03 14:39:28.000000 python-canvas-0.3.6/canvas_db/orm.py
+drwxr-xr-x   0 user      (1000) user      (1001)        0 2023-06-03 15:03:13.133333 python-canvas-0.3.6/python_canvas.egg-info/
+-rw-r--r--   0 user      (1000) user      (1001)      949 2023-06-03 15:03:13.000000 python-canvas-0.3.6/python_canvas.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1001)      289 2023-06-03 15:03:13.000000 python-canvas-0.3.6/python_canvas.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1001)        1 2023-06-03 15:03:13.000000 python-canvas-0.3.6/python_canvas.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1001)       20 2023-06-03 15:03:13.000000 python-canvas-0.3.6/python_canvas.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1001)       10 2023-06-03 15:03:13.000000 python-canvas-0.3.6/python_canvas.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1001)       38 2023-06-03 15:03:13.133333 python-canvas-0.3.6/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1001)      815 2023-06-03 15:02:52.000000 python-canvas-0.3.6/setup.py
```

### Comparing `python-canvas-0.3.5/PKG-INFO` & `python-canvas-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-canvas
-Version: 0.3.5
+Version: 0.3.6
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Canvas
 Home-page: https://github.com/yessenovuniversity/python_canvas
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-canvas-0.3.5/canvas_db/models.py` & `python-canvas-0.3.6/canvas_db/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -855,15 +855,15 @@
     # Статус работы
     workflow_state = Column(String)
 
     # Дата и время создания
     created_at = Column(DateTime, server_default=func.now())
 
     # Дата и время изменения
-    updated_at = Column(DateTIme, onupdate=func.now())
+    updated_at = Column(DateTime, onupdate=func.now())
 
     # Неизвестное значение
     fudge_points = Column(Integer)
 
     # Неизвестное значение (Возможно сколько максимум студент может набрать баллов)
     quiz_points_possible = Column(Integer)
```

### Comparing `python-canvas-0.3.5/python_canvas.egg-info/PKG-INFO` & `python-canvas-0.3.6/python_canvas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-canvas
-Version: 0.3.5
+Version: 0.3.6
 Summary: Данная библиотека содержить SqlAlchemy ORM для системы Canvas
 Home-page: https://github.com/yessenovuniversity/python_canvas
 Author: Nauryzbek Aitbayev
 Author-email: nauryzbek.aitbayev@yu.edu.kz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-canvas-0.3.5/setup.py` & `python-canvas-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="python-canvas",
-    version="0.3.5",
+    version="0.3.6",
     author="Nauryzbek Aitbayev",
     author_email="nauryzbek.aitbayev@yu.edu.kz",
     description="Данная библиотека содержить SqlAlchemy ORM для системы Canvas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yessenovuniversity/python_canvas",
     packages=setuptools.find_packages(),
```

