# Comparing `tmp/fenjing-0.3.7.tar.gz` & `tmp/fenjing-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.7.tar", last modified: Mon May 29 05:54:01 2023, max compression
+gzip compressed data, was "fenjing-0.3.8.tar", last modified: Sat Jun  3 01:27:23 2023, max compression
```

## Comparing `fenjing-0.3.7.tar` & `fenjing-0.3.8.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 05:53:44.000000 fenjing-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 05:53:44.000000 fenjing-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-29 05:54:01.587361 fenjing-0.3.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-05-29 05:53:44.000000 fenjing-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 05:53:44.000000 fenjing-0.3.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4184 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    30746 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-29 05:53:44.000000 fenjing-0.3.7/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:54:01.587361 fenjing-0.3.7/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 05:54:01.000000 fenjing-0.3.7/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 05:53:44.000000 fenjing-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 05:54:01.587361 fenjing-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-29 05:53:44.000000 fenjing-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.940680 fenjing-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-03 01:27:14.000000 fenjing-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 01:27:14.000000 fenjing-0.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-03 01:27:23.936680 fenjing-0.3.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-06-03 01:27:14.000000 fenjing-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 01:27:14.000000 fenjing-0.3.8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.936680 fenjing-0.3.8/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5080 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30746 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.936680 fenjing-0.3.8/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.936680 fenjing-0.3.8/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-03 01:27:14.000000 fenjing-0.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 01:27:23.940680 fenjing-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-03 01:27:14.000000 fenjing-0.3.8/setup.py
```

### Comparing `fenjing-0.3.7/LICENSE` & `fenjing-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/PKG-INFO` & `fenjing-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.7/README.md` & `fenjing-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/cli.py` & `fenjing-0.3.8/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/colorize.py` & `fenjing-0.3.8/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/config_payload.py` & `fenjing-0.3.8/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/const.py` & `fenjing-0.3.8/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/form.py` & `fenjing-0.3.8/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/form_cracker.py` & `fenjing-0.3.8/fenjing/form_cracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,21 @@
 from .full_payload_gen import FullPayloadGen
 
 logger = logging.getLogger("form_cracker")
 Result = namedtuple("Result", "full_payload_gen input_field")
 
 
 class FormCracker:
+    """对指定的文档进行攻击
+    其接受一个表格及其对应的URL，还有一个用于发送请求的requester。
+    其会根据一系列危险的关键字获取被WAF时页面的hash, 据此生成一个waf函数用于生成payload
     """
-    对指定的文档进行攻击
-    """
-    dangerous_keywords = [
-        "config", "self", "os", "class", "mro", "base", "request",
-        "attr", "open", "system",
-        "[", '"', "'", "_", ".", "+", "{{", "|",
-        "0", "1", "2",
-    ]
     test_cmd = "echo f3n  j1ng;"
     test_result = "f3n j1ng"
+    test_vulunable_inputs_times = 5
 
     def __init__(
             self,
             url: str,
             form: Dict[str, Any],
             requester: Requester,
             callback: Union[Callable[[str, Dict], None], None] = None
@@ -58,25 +54,28 @@
 
     def vulunable_inputs(self) -> List[str]:
         """解析出form中有回显的input
 
         Returns:
             List[str]: 所有有回显的input name
         """
-        fill_dict = random_fill(self.form)
-        r = self.req.request(
-            **fill_form(
-                self.url,
-                self.form,
-                form_inputs=fill_dict))
-        assert r is not None
-        return [
-            k for k, v in fill_dict.items()
-            if v in r.text
-        ]
+        answers = []
+        for _ in range(self.test_vulunable_inputs_times):
+            fill_dict = random_fill(self.form)
+            r = self.req.request(
+                **fill_form(
+                    self.url,
+                    self.form,
+                    form_inputs=fill_dict))
+            assert r is not None
+            answers += [
+                k for k, v in fill_dict.items()
+                if v in r.text
+            ]
+        return list(set(answers))
 
     def submit(self, inputs: dict):
         """根据inputs提交form
 
         Args:
             inputs (dict): 需要提交的input
```

### Comparing `fenjing-0.3.7/fenjing/full_payload_gen.py` & `fenjing-0.3.8/fenjing/full_payload_gen.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,21 @@
             return outer_pattern, will_print
     else:
         logger.warning("LOTS OF THINGS is being waf, NOTHING FOR YOU!")
         return None, None
 
 
 class FullPayloadGen:
-    def __init__(self, waf_func, callback: Union[Callable[[str, Dict], None], None] = None):
+    """接受一个waf函数并负责生成payload
+    waf函数接受一个字符串并返回这个字符串是否可以通过WAF
+    payload由两部分组成：
+        - 前方提供变量等上下文的上下文payload（一般为{%set xxx=xxx%}的形式）
+        - 以及后方实际发挥作用的作用payload（一般被双花括号{{}}包裹）
+    """
+    def __init__(self, waf_func: Callable[[str, ], bool], callback: Union[Callable[[str, Dict], None], None] = None):
         self.waf_func = waf_func
         self.prepared = False
         self._callback: Callable[[str, Dict], None] = callback if callback else (lambda x, y: None)
 
     @property
     def callback(self):
         return self._callback
@@ -57,15 +63,19 @@
     @callback.setter
     def callback(self, callback):
         self._callback = callback
         if self.payload_gen:
             self.payload_gen.callback = callback
 
     def do_prepare(self) -> bool:
+        """生成上下文payload，并准备作用payload的最外层（一般为双花括号{{}}）
 
+        Returns:
+            bool: 是否生成成功，失败则无法生成payload。有时生成的
+        """
         if self.prepared:
             return True
 
         int_payload, int_context = get_int_context(self.waf_func)
         str_payload, str_context = get_str_context(self.waf_func)
 
         self.context_payload, self.context = int_payload + \
@@ -86,15 +96,22 @@
             "context": self.context,
             "outer_pattern": self.outer_pattern,
             "will_print": self.will_print,
         })
         return True
 
     def generate(self, gen_type, *args) -> Tuple[Union[str, None], Union[bool, None]]:
+        """根据要求生成payload
 
+        Args:
+            gen_type (str): 生成payload的类型，应传入如OS_POPEN_READ等在const.py中定义的类型
+
+        Returns:
+            Tuple[Union[str, None], Union[bool, None]]: payload, 以及payload是否会有回显
+        """
         if not self.prepared and not self.do_prepare():
             return None, None
 
         inner_payload = self.payload_gen.generate(gen_type, *args)
 
         if inner_payload is None:
             logger.warning("Bypassing WAF Failed.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fenjing-0.3.7/fenjing/int_vars.py` & `fenjing-0.3.8/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/payload_gen.py` & `fenjing-0.3.8/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/requester.py` & `fenjing-0.3.8/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/scan_url.py` & `fenjing-0.3.8/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/shell_payload.py` & `fenjing-0.3.8/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/templates/index.html` & `fenjing-0.3.8/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/waf_func_gen.py` & `fenjing-0.3.8/fenjing/waf_func_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing/webui.py` & `fenjing-0.3.8/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.7/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.8/fenjing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.7
+Version: 0.3.8
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.7/fenjing.egg-info/SOURCES.txt` & `fenjing-0.3.8/fenjing.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 setup.py
 fenjing/__init__.py
 fenjing/__main__.py
 fenjing/cli.py
 fenjing/colorize.py
 fenjing/config_payload.py
 fenjing/const.py
-fenjing/exceptions.py
 fenjing/form.py
 fenjing/form_cracker.py
 fenjing/full_payload_gen.py
 fenjing/int_vars.py
 fenjing/payload_gen.py
 fenjing/requester.py
 fenjing/scan_url.py
```

### Comparing `fenjing-0.3.7/setup.py` & `fenjing-0.3.8/setup.py`

 * *Files identical despite different names*

