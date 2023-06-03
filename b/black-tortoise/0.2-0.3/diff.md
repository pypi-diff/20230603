# Comparing `tmp/black_tortoise-0.2.tar.gz` & `tmp/black_tortoise-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "black_tortoise-0.2.tar", last modified: Sat Jun  3 11:44:09 2023, max compression
+gzip compressed data, was "black_tortoise-0.3.tar", last modified: Sat Jun  3 12:11:42 2023, max compression
```

## Comparing `black_tortoise-0.2.tar` & `black_tortoise-0.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 11:44:09.055546 black_tortoise-0.2/
--rw-r--r--   0 lambert    (501) staff       (20)     1431 2023-06-03 11:44:09.055340 black_tortoise-0.2/PKG-INFO
--rw-rw-r--   0 lambert    (501) staff       (20)      741 2023-06-03 10:14:00.000000 black_tortoise-0.2/README.md
-drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 11:44:09.054376 black_tortoise-0.2/black_tortoise.egg-info/
--rw-r--r--   0 lambert    (501) staff       (20)     1431 2023-06-03 11:44:09.000000 black_tortoise-0.2/black_tortoise.egg-info/PKG-INFO
--rw-r--r--   0 lambert    (501) staff       (20)      327 2023-06-03 11:44:09.000000 black_tortoise-0.2/black_tortoise.egg-info/SOURCES.txt
--rw-r--r--   0 lambert    (501) staff       (20)        1 2023-06-03 11:44:09.000000 black_tortoise-0.2/black_tortoise.egg-info/dependency_links.txt
--rw-r--r--   0 lambert    (501) staff       (20)       59 2023-06-03 11:44:09.000000 black_tortoise-0.2/black_tortoise.egg-info/requires.txt
--rw-r--r--   0 lambert    (501) staff       (20)       22 2023-06-03 11:44:09.000000 black_tortoise-0.2/black_tortoise.egg-info/top_level.txt
-drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 11:44:09.054507 black_tortoise-0.2/mock_data/
--rw-rw-r--   0 lambert    (501) staff       (20)      166 2023-04-16 02:37:48.000000 black_tortoise-0.2/mock_data/__init__.py
-drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 11:44:09.054641 black_tortoise-0.2/mock_data/user/
--rw-rw-r--   0 lambert    (501) staff       (20)      166 2023-04-16 02:37:48.000000 black_tortoise-0.2/mock_data/user/__init__.py
--rw-r--r--   0 lambert    (501) staff       (20)       38 2023-06-03 11:44:09.055606 black_tortoise-0.2/setup.cfg
--rw-rw-r--   0 lambert    (501) staff       (20)     1542 2023-06-03 11:42:56.000000 black_tortoise-0.2/setup.py
-drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 11:44:09.054776 black_tortoise-0.2/tests/
--rw-rw-r--   0 lambert    (501) staff       (20)      166 2023-04-16 02:25:42.000000 black_tortoise-0.2/tests/__init__.py
-drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 11:44:09.055153 black_tortoise-0.2/utils/
--rw-r--r--   0 lambert    (501) staff       (20)     3486 2023-06-03 09:51:52.000000 black_tortoise-0.2/utils/FileUtils.py
--rw-rw-r--   0 lambert    (501) staff       (20)      161 2023-04-26 01:00:52.000000 black_tortoise-0.2/utils/__init__.py
--rw-rw-r--   0 lambert    (501) staff       (20)     3084 2023-04-25 14:02:58.000000 black_tortoise-0.2/utils/logger.py
+drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 12:11:42.858207 black_tortoise-0.3/
+-rw-r--r--   0 lambert    (501) staff       (20)       48 2023-06-03 12:04:08.000000 black_tortoise-0.3/MANIFEST.in
+-rw-r--r--   0 lambert    (501) staff       (20)     1446 2023-06-03 12:11:42.858023 black_tortoise-0.3/PKG-INFO
+-rw-r--r--   0 lambert    (501) staff       (20)      756 2023-06-03 11:58:28.000000 black_tortoise-0.3/README.md
+drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 12:11:42.856092 black_tortoise-0.3/black_tortoise.egg-info/
+-rw-r--r--   0 lambert    (501) staff       (20)     1446 2023-06-03 12:11:42.000000 black_tortoise-0.3/black_tortoise.egg-info/PKG-INFO
+-rw-r--r--   0 lambert    (501) staff       (20)      356 2023-06-03 12:11:42.000000 black_tortoise-0.3/black_tortoise.egg-info/SOURCES.txt
+-rw-r--r--   0 lambert    (501) staff       (20)        1 2023-06-03 12:11:42.000000 black_tortoise-0.3/black_tortoise.egg-info/dependency_links.txt
+-rw-r--r--   0 lambert    (501) staff       (20)       59 2023-06-03 12:11:42.000000 black_tortoise-0.3/black_tortoise.egg-info/requires.txt
+-rw-r--r--   0 lambert    (501) staff       (20)       22 2023-06-03 12:11:42.000000 black_tortoise-0.3/black_tortoise.egg-info/top_level.txt
+drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 12:11:42.856228 black_tortoise-0.3/mock_data/
+-rw-r--r--   0 lambert    (501) staff       (20)      166 2023-06-03 11:46:11.000000 black_tortoise-0.3/mock_data/__init__.py
+drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 12:11:42.856807 black_tortoise-0.3/mock_data/user/
+-rw-r--r--   0 lambert    (501) staff       (20)      166 2023-06-03 11:46:11.000000 black_tortoise-0.3/mock_data/user/__init__.py
+-rw-r--r--   0 lambert    (501) staff       (20)       27 2023-06-03 11:46:11.000000 black_tortoise-0.3/requirements.txt
+-rw-r--r--   0 lambert    (501) staff       (20)       38 2023-06-03 12:11:42.858263 black_tortoise-0.3/setup.cfg
+-rw-r--r--   0 lambert    (501) staff       (20)     1542 2023-06-03 12:04:51.000000 black_tortoise-0.3/setup.py
+drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 12:11:42.857057 black_tortoise-0.3/tests/
+-rw-r--r--   0 lambert    (501) staff       (20)      166 2023-06-03 11:46:11.000000 black_tortoise-0.3/tests/__init__.py
+drwxr-xr-x   0 lambert    (501) staff       (20)        0 2023-06-03 12:11:42.857759 black_tortoise-0.3/utils/
+-rw-r--r--   0 lambert    (501) staff       (20)     3486 2023-06-03 11:46:11.000000 black_tortoise-0.3/utils/FileUtils.py
+-rw-r--r--   0 lambert    (501) staff       (20)      161 2023-06-03 11:46:11.000000 black_tortoise-0.3/utils/__init__.py
+-rw-r--r--   0 lambert    (501) staff       (20)     3084 2023-06-03 11:46:11.000000 black_tortoise-0.3/utils/logger.py
```

### Comparing `black_tortoise-0.2/PKG-INFO` & `black_tortoise-0.3/black_tortoise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: black_tortoise
-Version: 0.2
+Name: black-tortoise
+Version: 0.3
 Summary: 玄武 SDK 是一个提供底层工具级的项目，类似于hutool 一样，提供很多的工具类
 Home-page: https://github.com/lizhen1412/black_tortoise
 Author: Lambert
 Author-email: 595265454@qq.com
 License: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,16 @@
 ##### 项目结构 #####
 1. 源码查看项目结构 tree 方法
 ```shell
 tree -I "venv|__pycache__|*.pyc|*.pyo|*.so|*.egg-info|*.egg|*.log|*.txt|*.md|*.json|*.yaml|*.yml|*.ini|*.cfg|*.conf|*.xml|*.html|*.rst|*.rst.txt|*.rst"
 ```
 2. 项目结构说明
 ```shell
- dosc
+black_tortoise
+|dosc
 │   └── deployment -- 发布相关文档介绍 
 ├── mock_data  -- mock 数据
 │   ├── __init__.py
 │   └── user
 │       └── __init__.py
 ├── setup.py -- 项目打包配置文件
 ├── tests -- 测试用例
```

### Comparing `black_tortoise-0.2/README.md` & `black_tortoise-0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 ##### 项目结构 #####
 1. 源码查看项目结构 tree 方法
 ```shell
 tree -I "venv|__pycache__|*.pyc|*.pyo|*.so|*.egg-info|*.egg|*.log|*.txt|*.md|*.json|*.yaml|*.yml|*.ini|*.cfg|*.conf|*.xml|*.html|*.rst|*.rst.txt|*.rst"
 ```
 2. 项目结构说明
 ```shell
- dosc
+black_tortoise
+|dosc
 │   └── deployment -- 发布相关文档介绍 
 ├── mock_data  -- mock 数据
 │   ├── __init__.py
 │   └── user
 │       └── __init__.py
 ├── setup.py -- 项目打包配置文件
 ├── tests -- 测试用例
```

### Comparing `black_tortoise-0.2/black_tortoise.egg-info/PKG-INFO` & `black_tortoise-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: black-tortoise
-Version: 0.2
+Name: black_tortoise
+Version: 0.3
 Summary: 玄武 SDK 是一个提供底层工具级的项目，类似于hutool 一样，提供很多的工具类
 Home-page: https://github.com/lizhen1412/black_tortoise
 Author: Lambert
 Author-email: 595265454@qq.com
 License: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -24,15 +24,16 @@
 ##### 项目结构 #####
 1. 源码查看项目结构 tree 方法
 ```shell
 tree -I "venv|__pycache__|*.pyc|*.pyo|*.so|*.egg-info|*.egg|*.log|*.txt|*.md|*.json|*.yaml|*.yml|*.ini|*.cfg|*.conf|*.xml|*.html|*.rst|*.rst.txt|*.rst"
 ```
 2. 项目结构说明
 ```shell
- dosc
+black_tortoise
+|dosc
 │   └── deployment -- 发布相关文档介绍 
 ├── mock_data  -- mock 数据
 │   ├── __init__.py
 │   └── user
 │       └── __init__.py
 ├── setup.py -- 项目打包配置文件
 ├── tests -- 测试用例
```

### Comparing `black_tortoise-0.2/setup.py` & `black_tortoise-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @Description: 
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name='black_tortoise',  # 应用名
-    version='0.2',  # 版本号
+    version='0.3',  # 版本号
     packages=find_packages(),  # 包括在安装包内的Python包
     include_package_data=True,  # 启用清单文件MANIFEST.in
     install_requires=[
         'faker >= 18.10.1',
         'loguru >= 0.7.0',
         'requests >= 2.31.0',
         'gmssl >= 3.2.2',
```

### Comparing `black_tortoise-0.2/utils/FileUtils.py` & `black_tortoise-0.3/utils/FileUtils.py`

 * *Files identical despite different names*

### Comparing `black_tortoise-0.2/utils/logger.py` & `black_tortoise-0.3/utils/logger.py`

 * *Files identical despite different names*

