# Comparing `tmp/gqylpy_exception-2.0.3.tar.gz` & `tmp/gqylpy_exception-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_exception-2.0.3.tar", last modified: Sat May 13 02:44:00 2023, max compression
+gzip compressed data, was "gqylpy_exception-2.0.4.tar", last modified: Sat Jun  3 05:58:56 2023, max compression
```

## Comparing `gqylpy_exception-2.0.3.tar` & `gqylpy_exception-2.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:44:00.619649 gqylpy_exception-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-13 02:43:46.000000 gqylpy_exception-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-13 02:44:00.619649 gqylpy_exception-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-13 02:43:46.000000 gqylpy_exception-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:44:00.615649 gqylpy_exception-2.0.3/gqylpy_exception/
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-13 02:43:46.000000 gqylpy_exception-2.0.3/gqylpy_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-05-13 02:43:46.000000 gqylpy_exception-2.0.3/gqylpy_exception/g exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 02:44:00.619649 gqylpy_exception-2.0.3/gqylpy_exception.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-13 02:44:00.000000 gqylpy_exception-2.0.3/gqylpy_exception.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-13 02:44:00.000000 gqylpy_exception-2.0.3/gqylpy_exception.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 02:44:00.000000 gqylpy_exception-2.0.3/gqylpy_exception.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 02:44:00.000000 gqylpy_exception-2.0.3/gqylpy_exception.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 02:44:00.619649 gqylpy_exception-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-13 02:43:46.000000 gqylpy_exception-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:58:56.183187 gqylpy_exception-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-03 05:58:46.000000 gqylpy_exception-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-03 05:58:56.183187 gqylpy_exception-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-03 05:58:46.000000 gqylpy_exception-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:58:56.183187 gqylpy_exception-2.0.4/gqylpy_exception/
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-06-03 05:58:46.000000 gqylpy_exception-2.0.4/gqylpy_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-06-03 05:58:46.000000 gqylpy_exception-2.0.4/gqylpy_exception/g exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 05:58:56.183187 gqylpy_exception-2.0.4/gqylpy_exception.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-03 05:58:56.000000 gqylpy_exception-2.0.4/gqylpy_exception.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-03 05:58:56.000000 gqylpy_exception-2.0.4/gqylpy_exception.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 05:58:56.000000 gqylpy_exception-2.0.4/gqylpy_exception.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-03 05:58:56.000000 gqylpy_exception-2.0.4/gqylpy_exception.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 05:58:56.183187 gqylpy_exception-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-03 05:58:46.000000 gqylpy_exception-2.0.4/setup.py
```

### Comparing `gqylpy_exception-2.0.3/LICENSE` & `gqylpy_exception-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_exception-2.0.3/PKG-INFO` & `gqylpy_exception-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gqylpy_exception
-Version: 2.0.3
+Version: 2.0.4
 Summary: 在执行 raise 语句的同时创建异常类，无需事先定义异常类，方便快捷。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Artistic Software
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `gqylpy_exception-2.0.3/README.md` & `gqylpy_exception-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gqylpy_exception-2.0.3/gqylpy_exception/__init__.py` & `gqylpy_exception-2.0.4/gqylpy_exception/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Create the exception class while executing the `raise` statement, you no longer
 need to define an exception class in advance, Convenient and Fast.
 
     >>> import gqylpy_exception as ge
     >>> raise ge.AnError(...)
 
-    @version: 2.0.3
+    @version: 2.0.4
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-exception
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -31,17 +31,15 @@
 
 ExceptionTypes    = Union[Type[Exception], Tuple[Type[Exception], ...]]
 ExceptionLogger   = Union[logging.Logger, 'gqylpy_log']
 ExceptionCallback = Callable[[Exception, Callable, '...'], None]
 
 
 def __getattr__(ename: str) -> Type['GqylpyError']:
-    if ename not in __history__[ename]:
-        __history__[ename] = type(ename, (GqylpyError,), {})
-    return __history__[ename]
+    return __history__.setdefault(ename, type(ename, (GqylpyError,), {}))
 
 
 def __getitem__(ename: str) -> Type['GqylpyError']:
     return __getattr__(ename)
 
 
 __history__: Dict[str, Type['GqylpyError']]
@@ -184,33 +182,36 @@
         logger    =logger
     )
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
     import sys
 
-    gpack = globals()
-    gpath = f'{__name__}.g {__name__[7:]}'
-    gcode = __import__(gpath, fromlist=...)
-
-    ge = gcode.GqylpyException()
-
-    for gname in gpack:
-        if gname[0] != '_':
-            try:
-                gfunc = getattr(gcode, gname)
-                assert gfunc.__module__ in (gpath, __package__)
-            except (AttributeError, AssertionError):
-                continue
-            gfunc.__module__ = __package__
-            setattr(ge, gname, gfunc)
-        elif not hasattr(ge, gname):
-            setattr(ge.__class__, gname, gpack[gname])
-
-    setattr(ge, __package__, ge.__class__)
-
-    ge.__doc__                = __doc__
-    ge.__name__               = __package__
-    ge.__class__.__qualname__ = __package__
-    ge.__class__.__module__   = __package__
+    if sys.platform != 'linux' or \
+            logging.__file__[:-20] == __file__[:-len(__name__) - 27]:
+        gpack = globals()
+        gpath = f'{__name__}.g {__name__[7:]}'
+        gcode = __import__(gpath, fromlist=...)
+
+        ge = gcode.GqylpyException()
+
+        for gname in gpack:
+            if gname[0] != '_':
+                try:
+                    gfunc = getattr(gcode, gname)
+                    assert gfunc.__module__ in (gpath, __package__)
+                except (AttributeError, AssertionError):
+                    continue
+                gfunc.__module__ = __package__
+                setattr(ge, gname, gfunc)
+            elif not hasattr(ge, gname):
+                setattr(ge.__class__, gname, gpack[gname])
+
+        setattr(ge, __package__, ge.__class__)
 
-    sys.modules[__name__] = ge
+        ge.__doc__  = __doc__
+        ge.__name__ = __package__
+
+        ge.__class__.__qualname__ = __package__
+        ge.__class__.__module__   = __package__
+
+        sys.modules[__name__] = ge
```

### Comparing `gqylpy_exception-2.0.3/gqylpy_exception/g exception.py` & `gqylpy_exception-2.0.4/gqylpy_exception/g exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 
 Function = Closure = TypeVar('Function', bound=Callable)
 
 ExceptionTypes    = Union[Type[Exception], Tuple[Type[Exception], ...]]
 ExceptionLogger   = Union[logging.Logger, 'gqylpy_log']
 ExceptionCallback = Callable[[Exception, Function, '...'], None]
 
-warnings.filterwarnings('once', category=DeprecationWarning)
-
 
 class GqylpyException:
     __history__ = {}
 
     def __getattr__(self, ename: str) -> Type['GqylpyError']:
         try:
             eclass = self.__history__[ename]
@@ -51,15 +49,15 @@
             if hasattr(builtins, ename):
                 raise self.ExceptionClassIsBuiltinsError(
                     f'exception class "{ename}" is builtins.'
                 ) from None
             if ename[-5:] != 'Error':
                 warnings.warn(
                     f'strange exception class "{ename}", exception class name '
-                    'should end with "Error".', UserWarning, stacklevel=2
+                    'should end with "Error".', stacklevel=2
                 )
             eclass = self.__history__[ename] = type(
                 ename, (self.GqylpyError,), {'__module__': 'builtins'}
             )
             # Compatible with object serialization.
             setattr(builtins, ename, eclass)
         return eclass
@@ -71,17 +69,20 @@
         __module__ = 'builtins'
 
         @property
         def msg(self) -> Any:
             return self.args[0] if len(self.args) == 1 else \
                 self.args if self.args else None
 
+
 # Compatible with object serialization, for `GqylpyException.GqylpyError`.
 builtins.GqylpyException = GqylpyException
 
+ParameterError = GqylpyException().ParameterError
+
 
 def stderr(einfo: str) -> None:
     now: str = time.strftime('%F %T', time.localtime())
     sys.stderr.write(f'[{now}] {einfo}\n')
 
 
 def get_logger(logger: logging.Logger) -> Callable[[str], None]:
@@ -101,25 +102,14 @@
         return logger.warning
 
     return logger.error
 
 
 class TryExcept:
 
-    def __new__(cls, *a, **kw):
-        if 'ignore' in kw:
-            warnings.warn(DeprecationWarning(
-                'parameter "ignore" deprecated, replaced to "silent_exc".'
-            ), stacklevel=2)
-        if 'output_raw_exc' in kw:
-            warnings.warn(DeprecationWarning(
-                'parameter "output_raw_exc" deprecated, replaced to "raw_exc".'
-            ), stacklevel=2)
-        return object.__new__(cls)
-
     def __init__(
             self,
             etype:      ExceptionTypes,
             *,
             silent_exc: bool                        = False,
             raw_exc:    bool                        = False,
             logger:     Optional[ExceptionLogger]   = None,
@@ -189,27 +179,36 @@
 
     def exception_analysis(self, func: Function, e: Exception) -> str:
         einfo: str = traceback.format_exc()
 
         if self.raw_exc:
             return einfo
 
-        filepath: str = func.__globals__['__file__']
-        funcpath: str = f'{func.__module__}.{func.__qualname__}'
+        if isinstance(func, type):
+            filepath: str = sys.modules[func.__module__].__file__
+        else:
+            try:
+                filepath: str = func.__globals__['__file__']
+            except AttributeError:
+                filepath = None
 
-        for line in reversed(einfo.split('\n')[1:-3]):
-            if filepath in line:
-                eline: str = re.search(
-                    r'line \d+', line
-                ).group().replace(' ', '')
-                break
+        if filepath is None:
+            eline = 'lineX'
         else:
-            eline: str = 'lineX'
+            for line in reversed(einfo.split('\n')[1:-3]):
+                if filepath in line:
+                    eline: str = re.search(
+                        r'line \d+', line
+                    ).group().replace(' ', '')
+                    break
+            else:
+                eline = 'lineX'
 
-        return f'[{funcpath}.{eline}.{e.__class__.__name__}] {e}'
+        return f'[{func.__module__}.{func.__qualname__}.{eline}.' \
+               f'{e.__class__.__name__}] {e}'
 
 
 class Retry(TryExcept):
 
     def __init__(
             self,
             etype:      ExceptionTypes            = Exception,
@@ -277,9 +276,7 @@
                 if count == self.count:
                     raise e
 
             await asyncio.sleep(self.cycle)
 
 
 TryExceptAsync, RetryAsync = TryExcept, Retry
-
-ParameterError = GqylpyException().ParameterError
```

### Comparing `gqylpy_exception-2.0.3/gqylpy_exception.egg-info/PKG-INFO` & `gqylpy_exception-2.0.4/gqylpy_exception.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gqylpy-exception
-Version: 2.0.3
+Version: 2.0.4
 Summary: 在执行 raise 语句的同时创建异常类，无需事先定义异常类，方便快捷。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Artistic Software
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `gqylpy_exception-2.0.3/setup.py` & `gqylpy_exception-2.0.4/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=[g.__name__],
     python_requires='>=3.6, <4',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
+        'License :: OSI Approved :: Apache Software License',
         'Natural Language :: Chinese (Simplified)',
         'Natural Language :: English',
-        'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Bug Tracking',
         'Topic :: Software Development :: Widget Sets',
         'Topic :: Artistic Software',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

