# Comparing `tmp/implicit_globals-1.0.0-py3-none-any.whl.zip` & `tmp/implicit_globals-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6403 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     6276 b- defN 20-Aug-31 18:22 implicit_globals.py
--rw-rw-rw-  2.0 fat     1102 b- defN 20-Aug-31 18:25 implicit_globals-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4389 b- defN 20-Aug-31 18:25 implicit_globals-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 20-Aug-31 18:25 implicit_globals-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 20-Aug-31 18:25 implicit_globals-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      507 b- defN 20-Aug-31 18:25 implicit_globals-1.0.0.dist-info/RECORD
-6 files, 12388 bytes uncompressed, 5479 bytes compressed:  55.8%
+Zip file size: 6451 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     5983 b- defN 23-Jun-03 13:44 implicit_globals.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-Jun-03 13:48 implicit_globals-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5009 b- defN 23-Jun-03 13:48 implicit_globals-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 13:48 implicit_globals-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-03 13:48 implicit_globals-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      507 b- defN 23-Jun-03 13:48 implicit_globals-1.0.1.dist-info/RECORD
+6 files, 12690 bytes uncompressed, 5527 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: implicit_globals.py
 Comment: 
 
-Filename: implicit_globals-1.0.0.dist-info/LICENSE
+Filename: implicit_globals-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: implicit_globals-1.0.0.dist-info/METADATA
+Filename: implicit_globals-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: implicit_globals-1.0.0.dist-info/WHEEL
+Filename: implicit_globals-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: implicit_globals-1.0.0.dist-info/top_level.txt
+Filename: implicit_globals-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: implicit_globals-1.0.0.dist-info/RECORD
+Filename: implicit_globals-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## implicit_globals.py

```diff
@@ -1,184 +1,186 @@
-# -*- coding: utf-8 -*-
-# module implicit_globals.py
-#
-# Copyright (c) 2020 Sebastien Devine
-#
-# Permission is hereby granted, free of charge, to any person obtaining
-# a copy of this software and associated documentation files (the
-# "Software"), to deal in the Software without restriction, including
-# without limitation the rights to use, copy, modify, merge, publish,
-# distribute, sublicense, and/or sell copies of the Software, and to
-# permit persons to whom the Software is furnished to do so, subject to
-# the following conditions:
-#
-# The above copyright notice and this permission notice shall be
-# included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
-# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
-# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-#
-__version__ = "1.0.0"
-__author__ = "Sebastien Devine"
-__email__ = "sebdevine@users.noreply.github.com"
-__github__ = "https://github.com/sebdevine/implicit_globals"
-
-__doc__ = """A decorator that provides a way to override a function/method 's global and default variables
-
-Those global/default variables can be overriden using a dict-like api.
-
-Notes:
-    - Inspired from Scala's implicits
-    - Chain functions and manage interwined function with global
-      / default variables hanging around
-    - Another way to monkey patch with an explicit mechanism to override
-    - Easy for non-experts to just import and decorate functions/methods
-
-Warnings:
-    - NO thread-safety
-    - NO async/coroutine support (yet)
-    - You must instanciate another `Implicit` decorator if you want
-      to keep things separate (per class / module etc)
-
-Usage:
-    You can use either the default decorator, or instanciate you own
-
-    >>> import sys
-    >>> from implicit_globals import implicit
-    >>>
-    >>> AAA = "FRE"
-    >>>
-    >>> def load():
-    ...     return "Hello"
-    >>>
-    >>> @implicit
-    >>> def foo(a, b, c=1, *, d=None):
-    ...     print("foo : ", a, b, c, d, AAA, load())
-
-    >>> foo(3, 4)
-    foo :  3 4 1 None FRE Hello
-
-    >>> # Override a global variable
-    >>> implicit["AAA"] = "BAZ"
-    >>> # Override builtin function
-    >>> implicit["print"] = lambda *_: sys.stdout.write("YO-- %s\\n" % ', '.join(map(str, _)))
-    >>> # Override global function
-    >>> implicit["load"] = lambda: "New Hello"
-    >>> # Override default parameter
-    >>> implicit["d"] = 333
-
-    >>> foo(3, 4)
-    YO-- foo : , 7, 8, 1, 333, BAZ, New Hello
-
-    Function can also be changed, with above definitions :
-    >>> @implicit
-    >>> def bar(a, b):
-    ...     print("bar : ", a, b, AAA)
-    ...     foo(a, b)
-
-    >>> bar(3, 4)
-    YO-- bar : , 3, 4, BAZ
-    YO-- foo : , 3, 4, 1, 333, BAZ, New Hello
-"""
-
-import copy
-import functools
-import inspect
-import types
-from typing import MutableMapping
-
-__all__ = ['ImplicitGlobals', 'implicit']
-
-
-def islambda(func: callable) -> bool:
-    def lmb():
-        return lambda: None
-
-    return isinstance(func, type(lmb())) and func.__name__ == lmb().__name__
-
-
-class ImplicitGlobals(MutableMapping):
-    """Dict-like object that stores global variables, its instances can be used as decorators
-    """
-
-    def __init__(self, **overrides):
-        self._overrides = overrides
-
-    def __len__(self):
-        return len(self._overrides)
-
-    def __iter__(self):
-        return iter(self._overrides)
-
-    def __delitem__(self, key):
-        del self._overrides[key]
-
-    def __getitem__(self, item):
-        return self._overrides[item]
-
-    def __setitem__(self, key, value):
-        self._overrides[key] = value
-
-    # noinspection PyMethodParameters
-    def __call__(this, func: callable) -> callable:
-        """Called upon function decoration
-        """
-        if not inspect.isfunction(func):
-            raise TypeError("Expecting a function, got: " + type(func).__name__)
-
-        if islambda(func):
-            raise TypeError("Cannot work on lambda functions")
-
-        # Poor man's class function detector
-        is_method = func.__qualname__.count('.') > 0
-
-        def new_func() -> types.FunctionType:
-            # Make a copy to avoid side effect the original function
-            __globals__: dict = copy.copy(func.__globals__)
-            # Then add our overrides
-            __globals__.update(this._overrides)
-
-            # noinspection PyTypeChecker
-            new_f: types.FunctionType = functools.update_wrapper(
-                wrapped=func,
-                wrapper=types.FunctionType(
-                    func.__code__,
-                    __globals__,
-                    name=func.__name__,
-                    argdefs=func.__defaults__,
-                    closure=func.__closure__))
-
-            # Reconstruct the keyword arguments' defaults
-            fa: inspect.FullArgSpec = inspect.getfullargspec(func)
-            func_args = fa.args or tuple()
-            func_defaults = fa.defaults or tuple()
-            func_kwdefaults = fa.kwonlydefaults or dict()
-
-            __kwdefaults__ = dict(zip(func_defaults[::-1], func_args[::-1]), **func_kwdefaults)
-            for k, v in __kwdefaults__.items():
-                if k in this._overrides:
-                    __kwdefaults__[k] = this._overrides[k]
-
-            new_f.__kwdefaults__ = __kwdefaults__
-            return new_f
-
-        if not is_method:
-            # Pure function
-            def wrapper(*args, **kwargs):
-                return new_func()(*args, **kwargs)
-
-        else:
-            # Method => must have self as first argument
-            def wrapper(self, *args, **kwargs):
-                return new_func()(self, *args, **kwargs)
-
-        functools.update_wrapper(wrapped=func, wrapper=wrapper)
-        return wrapper
-
-
-#: Default globals implicits decorator
-implicit = ImplicitGlobals()
+# -*- coding: utf-8 -*-
+# module implicit_globals.py
+#
+# Copyright (c) 2020 Sebastien Devine
+#
+# Permission is hereby granted, free of charge, to any person obtaining
+# a copy of this software and associated documentation files (the
+# "Software"), to deal in the Software without restriction, including
+# without limitation the rights to use, copy, modify, merge, publish,
+# distribute, sublicense, and/or sell copies of the Software, and to
+# permit persons to whom the Software is furnished to do so, subject to
+# the following conditions:
+#
+# The above copyright notice and this permission notice shall be
+# included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+# IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+# CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+# TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+# SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+#
+__version__ = "1.0.1"
+__author__ = "Sebastien Devine"
+__email__ = "sebdevine@users.noreply.github.com"
+__github__ = "https://github.com/sebdevine/implicit_globals"
+
+__doc__ = """A decorator that provides a way to override a function's global variables
+
+Those global/default variables can be overriden using a dict-like api.
+
+Notes:
+    - Inspired from Scala's implicits
+    - Chain functions and manage interwined function with global
+      / default variables hanging around
+    - Another way to monkey patch with an explicit mechanism to override
+    - Easy for non-experts to just import and decorate functions/methods
+
+Warnings:
+    - NO thread-safety
+    - NO async/coroutine support (yet)
+    - You must instanciate another `Implicit` decorator if you want
+      to keep things separate (per class / module etc)
+
+Usage:
+    You can use either the default decorator, or instanciate you own
+
+    >>> import sys
+    >>> from implicit_globals import implicit
+    >>>
+    >>> AAA = "FRE"
+    >>>
+    >>> def load():
+    ...     return "Hello"
+    >>>
+    >>> @implicit
+    >>> def foo(a, b, c=1, *, d=None):
+    ...     print("foo : ", a, b, c, d, AAA, load())
+
+    >>> foo(3, 4)
+    foo :  3 4 1 None FRE Hello
+
+    >>> # Override a global variable
+    >>> implicit["AAA"] = "BAZ"
+    >>> # Override builtin function
+    >>> implicit["print"] = \
+    ...     lambda *_: sys.stdout.write("YO-- %s\\n" % ', '.join(map(str, _)))
+    >>> # Override global function
+    >>> implicit["load"] = lambda: "New Hello"
+    >>> # Override default parameter
+    >>> implicit["d"] = 333
+
+    >>> foo(3, 4)
+    YO-- foo : , 7, 8, 1, 333, BAZ, New Hello
+
+    Function can also be changed, with above definitions :
+    >>> @implicit
+    >>> def bar(a, b):
+    ...     print("bar : ", a, b, AAA)
+    ...     foo(a, b)
+
+    >>> bar(3, 4)
+    YO-- bar : , 3, 4, BAZ
+    YO-- foo : , 3, 4, 1, 333, BAZ, New Hello
+"""
+
+import copy
+import functools
+import inspect
+import types
+from typing import MutableMapping
+
+__all__ = ["ImplicitGlobals", "implicit"]
+
+
+def islambda(func: callable) -> bool:
+    def lmb():
+        return lambda: None
+
+    return isinstance(func, type(lmb())) and func.__name__ == lmb().__name__
+
+
+class ImplicitGlobals(MutableMapping):
+    """Dict-like object that stores global variables, its instances can be used as decorators
+    """
+
+    def __init__(self, **overrides):
+        self._overrides = overrides
+
+    def __len__(self):
+        return len(self._overrides)
+
+    def __iter__(self):
+        return iter(self._overrides)
+
+    def __delitem__(self, key):
+        del self._overrides[key]
+
+    def __getitem__(self, item):
+        return self._overrides[item]
+
+    def __setitem__(self, key, value):
+        self._overrides[key] = value
+
+    # noinspection PyMethodParameters
+    def __call__(this, func: callable) -> callable:
+        """Called upon function decoration
+        """
+        if not inspect.isfunction(func):
+            raise TypeError("Expecting a function, got: " + type(func).__name__)
+
+        if islambda(func):
+            raise TypeError("Cannot work on lambda functions")
+
+        is_method = inspect.ismethod(func)
+
+        def new_func() -> types.FunctionType:
+            __globals__: dict = dict(func.__globals__)
+            __globals__.update(this._overrides)
+
+            # noinspection PyTypeChecker
+            new_f: types.FunctionType = functools.update_wrapper(
+                wrapped=func,
+                wrapper=types.FunctionType(
+                    func.__code__,
+                    __globals__,
+                    name=func.__name__,
+                    argdefs=func.__defaults__,
+                    closure=func.__closure__,
+                ),
+            )
+
+            # Reconstruct the keyword arguments' defaults
+            fa: inspect.FullArgSpec = inspect.getfullargspec(func)
+            func_args = fa.args or tuple()
+            func_defaults = fa.defaults or tuple()
+            func_kwdefaults = fa.kwonlydefaults or dict()
+
+            __kwdefaults__ = dict(
+                zip(func_args[::-1], func_defaults[::-1],), **func_kwdefaults
+            )
+            for k, v in __kwdefaults__.items():
+                if k in this._overrides:
+                    __kwdefaults__[k] = this._overrides[k]
+
+            new_f.__kwdefaults__ = __kwdefaults__
+            return new_f
+
+        if not is_method:
+            # Pure function
+            def wrapper(*args, **kwargs):
+                return new_func()(*args, **kwargs)
+
+        else:
+            # Method => must have self as first argument
+            def wrapper(self, *args, **kwargs):
+                return new_func()(self, *args, **kwargs)
+
+        functools.update_wrapper(wrapped=func, wrapper=wrapper)
+        return wrapper
+
+
+#: Default globals implicits decorator
+implicit = ImplicitGlobals()
```

## Comparing `implicit_globals-1.0.0.dist-info/LICENSE` & `implicit_globals-1.0.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2020 Sebastien Devine
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+The MIT License (MIT)
+
+Copyright (c) 2020 Sebastien Devine
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

## Comparing `implicit_globals-1.0.0.dist-info/METADATA` & `implicit_globals-1.0.1.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: implicit-globals
-Version: 1.0.0
-Summary: A decorator that provides a way to override a function/method 's global and default variables
+Version: 1.0.1
+Summary: A decorator that provides a way to override a function's global variables
 Home-page: https://github.com/sebdevine/implicit_globals
 Author: Sebastien Devine
 Author-email: sebdevine@users.noreply.github.com
 License: MIT
 Keywords: implicit globals decorator functional
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
+Classifier: Topic :: Software Development
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # implicit-globals
+[![Build Status](https://travis-ci.com/sebdevine/implicit_globals.svg?branch=master)](https://travis-ci.com/sebdevine/implicit_globals)
+[![codecov](https://codecov.io/gh/sebdevine/implicit_globals/branch/master/graph/badge.svg)](https://codecov.io/gh/sebdevine/implicit_globals)
+[![PyPI license](https://img.shields.io/pypi/l/implicit-globals.svg)](https://pypi.python.org/pypi/implicit-globals/)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/implicit-globals.svg)](https://pypi.python.org/pypi/implicit-globals/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/implicit-globals.svg)](https://pypi.python.org/pypi/implicit-globals/)
+
 
 **TL;DR: A Python decorator that allow you to modify at runtime a function's 
 implicit global variables or default variables.**
 
 ## Goals
 The _implicit_ adjective refers to all variables that are not explicit to a function call,
 either from the function (or method) 's global variables or any parameter with a default value.
```

