# Comparing `tmp/pyDictStore-1.0.1.tar.gz` & `tmp/pyDictStore-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDictStore-1.0.1.tar", last modified: Fri Jun  2 19:34:49 2023, max compression
+gzip compressed data, was "pyDictStore-1.0.2.tar", last modified: Sat Jun  3 01:15:02 2023, max compression
```

## Comparing `pyDictStore-1.0.1.tar` & `pyDictStore-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.537985 pyDictStore-1.0.1/
--rw-rw-rw-   0        0        0     1090 2022-05-31 23:42:26.000000 pyDictStore-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4494 2023-06-02 19:34:49.537006 pyDictStore-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3654 2022-08-06 00:15:10.000000 pyDictStore-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 19:34:49.538958 pyDictStore-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2158 2023-06-02 18:25:43.000000 pyDictStore-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.463784 pyDictStore-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.478429 pyDictStore-1.0.1/src/pyDictStore/
--rw-rw-rw-   0        0        0     2780 2022-06-06 01:53:10.000000 pyDictStore-1.0.1/src/pyDictStore/__decorators__.py
--rw-rw-rw-   0        0        0      974 2022-06-05 20:49:49.000000 pyDictStore-1.0.1/src/pyDictStore/__events__.py
--rw-rw-rw-   0        0        0      545 2023-06-02 19:05:36.000000 pyDictStore-1.0.1/src/pyDictStore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.534081 pyDictStore-1.0.1/src/pyDictStore.egg-info/
--rw-rw-rw-   0        0        0     4494 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.145612 pyDictStore-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2022-05-31 23:42:26.000000 pyDictStore-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4494 2023-06-03 01:15:02.143663 pyDictStore-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3654 2022-08-06 00:15:10.000000 pyDictStore-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 01:15:02.145612 pyDictStore-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2158 2023-06-02 18:25:43.000000 pyDictStore-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.089964 pyDictStore-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.112420 pyDictStore-1.0.2/src/pyDictStore/
+-rw-rw-rw-   0        0        0     2794 2023-06-03 01:13:50.000000 pyDictStore-1.0.2/src/pyDictStore/__decorators__.py
+-rw-rw-rw-   0        0        0      974 2022-06-05 20:49:49.000000 pyDictStore-1.0.2/src/pyDictStore/__events__.py
+-rw-rw-rw-   0        0        0      545 2023-06-03 01:14:15.000000 pyDictStore-1.0.2/src/pyDictStore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 01:15:02.141708 pyDictStore-1.0.2/src/pyDictStore.egg-info/
+-rw-rw-rw-   0        0        0     4494 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 01:15:01.000000 pyDictStore-1.0.2/src/pyDictStore.egg-info/top_level.txt
```

### Comparing `pyDictStore-1.0.1/LICENSE` & `pyDictStore-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.1/PKG-INFO` & `pyDictStore-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDictStore
-Version: 1.0.1
+Version: 1.0.2
 Summary: pyDictStore adds automated dictionary storage to properties eliminating the need for code bodies, property getters and setters. It also provides a property change event.
 Home-page: https://OpenWayside.org
 Author: Peter Varney, OpenWayside
 Author-email: pyDictStore@OpenWayside.org
 License: UNKNOWN
 Project-URL: Documentation, https://openwayside.org/rtm/pyDictStore/
 Project-URL: Source, https://github.com/OpenWayside/pyDictStore
```

### Comparing `pyDictStore-1.0.1/README.md` & `pyDictStore-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.1/setup.py` & `pyDictStore-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.1/src/pyDictStore/__decorators__.py` & `pyDictStore-1.0.2/src/pyDictStore/__decorators__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                     )
             fset = (prop.fset 
                     #if prop.fset.__qualname__ == 'storageSetter.<locals>.wrapper'
                     if isinstance(prop.fset,storageSetter)
                     else storageSetter(prop.fset)
                     )
             setattr(self.cls, name, property(fget, fset, prop.fdel))  
-        return self.cls()
+        return self.cls(*args,**kwargs)
 
 class default:
     def __init__(self, value=None) -> None:
         self.value = value
 
     def __call__(self, function):
         def wrapper(*args, **kwargs):
```

### Comparing `pyDictStore-1.0.1/src/pyDictStore/__events__.py` & `pyDictStore-1.0.2/src/pyDictStore/__events__.py`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.1/src/pyDictStore/__init__.py` & `pyDictStore-1.0.2/src/pyDictStore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 .. include:: ../../README.md
 
 # Library functions
 '''
 
 __PROJECT__ = 'pyDictStore'
-__VERSION__ = '1.0.1'
+__VERSION__ = '1.0.2'
 
 from .__decorators__ import default, storageSetter, storage
 
 def isDefault(obj:object,prop:str) -> bool:
     '''
     Checks if an objects property is equal to its default value
     '''
```

### Comparing `pyDictStore-1.0.1/src/pyDictStore.egg-info/PKG-INFO` & `pyDictStore-1.0.2/src/pyDictStore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDictStore
-Version: 1.0.1
+Version: 1.0.2
 Summary: pyDictStore adds automated dictionary storage to properties eliminating the need for code bodies, property getters and setters. It also provides a property change event.
 Home-page: https://OpenWayside.org
 Author: Peter Varney, OpenWayside
 Author-email: pyDictStore@OpenWayside.org
 License: UNKNOWN
 Project-URL: Documentation, https://openwayside.org/rtm/pyDictStore/
 Project-URL: Source, https://github.com/OpenWayside/pyDictStore
```

