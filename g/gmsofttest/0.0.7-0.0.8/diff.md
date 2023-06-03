# Comparing `tmp/gmsofttest-0.0.7.tar.gz` & `tmp/gmsofttest-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gmsofttest-0.0.7.tar", last modified: Fri May 26 06:02:06 2023, max compression
+gzip compressed data, was "dist\gmsofttest-0.0.8.tar", last modified: Sat Jun  3 03:57:19 2023, max compression
```

## Comparing `gmsofttest-0.0.7.tar` & `gmsofttest-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1271 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      777 2023-05-24 02:45:32.000000 gmsofttest-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      803 2023-05-26 06:01:45.000000 gmsofttest-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/gmsofttest/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.7/src/gmsofttest/__init__.py
--rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.7/src/gmsofttest/china_address.py
--rw-rw-rw-   0        0        0     3327 2023-05-24 03:07:23.000000 gmsofttest-0.0.7/src/gmsofttest/gm_assert_utils.py
--rw-rw-rw-   0        0        0     4867 2023-05-23 08:36:05.000000 gmsofttest-0.0.7/src/gmsofttest/gm_excel_utils.py
--rw-rw-rw-   0        0        0     3369 2023-05-26 05:38:26.000000 gmsofttest-0.0.7/src/gmsofttest/gm_parse_response_utils.py
--rw-rw-rw-   0        0        0     2197 2023-05-20 08:15:01.000000 gmsofttest-0.0.7/src/gmsofttest/gm_randomdata_utils.py
--rw-rw-rw-   0        0        0     1806 2023-05-24 02:44:27.000000 gmsofttest-0.0.7/src/gmsofttest/gm_request_utils.py
--rw-rw-rw-   0        0        0    11797 2023-05-23 08:03:00.000000 gmsofttest-0.0.7/src/gmsofttest/gm_sqlconn_utils.py
--rw-rw-rw-   0        0        0      877 2023-05-23 08:40:42.000000 gmsofttest-0.0.7/src/gmsofttest/gm_stock_enum.py
--rw-rw-rw-   0        0        0     3109 2023-05-20 08:15:01.000000 gmsofttest-0.0.7/src/gmsofttest/gm_timestamp_utils.py
--rw-rw-rw-   0        0        0     2196 2023-05-23 08:01:45.000000 gmsofttest-0.0.7/src/gmsofttest/gm_yaml_process_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-05-26 06:02:05.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-05-26 06:02:06.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 06:02:05.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 06:02:05.000000 gmsofttest-0.0.7/src/gmsofttest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1407 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2023-06-03 03:57:15.000000 gmsofttest-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-06-03 03:55:43.000000 gmsofttest-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.8/src/gmsofttest/__init__.py
+-rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.8/src/gmsofttest/china_address.py
+-rw-rw-rw-   0        0        0     3327 2023-05-24 03:07:23.000000 gmsofttest-0.0.8/src/gmsofttest/gm_assert_utils.py
+-rw-rw-rw-   0        0        0     4867 2023-05-23 08:36:05.000000 gmsofttest-0.0.8/src/gmsofttest/gm_excel_utils.py
+-rw-rw-rw-   0        0        0     3382 2023-06-03 03:54:28.000000 gmsofttest-0.0.8/src/gmsofttest/gm_parse_response_utils.py
+-rw-rw-rw-   0        0        0     2170 2023-06-02 00:58:44.000000 gmsofttest-0.0.8/src/gmsofttest/gm_randomdata_utils.py
+-rw-rw-rw-   0        0        0     1806 2023-05-24 02:44:27.000000 gmsofttest-0.0.8/src/gmsofttest/gm_request_utils.py
+-rw-rw-rw-   0        0        0    11797 2023-05-23 08:03:00.000000 gmsofttest-0.0.8/src/gmsofttest/gm_sqlconn_utils.py
+-rw-rw-rw-   0        0        0      877 2023-05-23 08:40:42.000000 gmsofttest-0.0.8/src/gmsofttest/gm_stock_enum.py
+-rw-rw-rw-   0        0        0     4322 2023-06-02 06:56:24.000000 gmsofttest-0.0.8/src/gmsofttest/gm_sucreditcode_utils.py
+-rw-rw-rw-   0        0        0     3109 2023-05-20 08:15:01.000000 gmsofttest-0.0.8/src/gmsofttest/gm_timestamp_utils.py
+-rw-rw-rw-   0        0        0     2196 2023-05-23 08:01:45.000000 gmsofttest-0.0.8/src/gmsofttest/gm_yaml_process_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/
+-rw-rw-rw-   0        0        0     1407 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 03:57:19.000000 gmsofttest-0.0.8/src/gmsofttest.egg-info/top_level.txt
```

### Comparing `gmsofttest-0.0.7/LICENSE` & `gmsofttest-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/PKG-INFO` & `gmsofttest-0.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.7
+Version: 0.0.8
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 License-File: LICENSE
 
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
+v0.0.8
+ 修改gm_prase_response的调用名称为gm_extract_json
+ 增加gm_sucreditcode_utils，用于生成企业社会信用代码
 
 v0.0.6 
  修改gm_request_utils的请求参数verfiy的默认值,由NONE调整成False
 
 v0.0.5
 
  增加gm_assert_utils：assert验证封装
```

### Comparing `gmsofttest-0.0.7/README.md` & `gmsofttest-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
+v0.0.8
+ 修改gm_prase_response的调用名称为gm_extract_json
+ 增加gm_sucreditcode_utils，用于生成企业社会信用代码
 
 v0.0.6 
  修改gm_request_utils的请求参数verfiy的默认值,由NONE调整成False
 
 v0.0.5
 
  增加gm_assert_utils：assert验证封装
```

### Comparing `gmsofttest-0.0.7/setup.py` & `gmsofttest-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gmsofttest",
-    version="0.0.7",
+    version="0.0.8",
     author="ronaldsu",
     author_email="uph4rmt@dingtalk.com",
     description="大家软件内部测试技术线支撑工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.gec123.com",
     project_urls={
```

### Comparing `gmsofttest-0.0.7/src/gmsofttest/china_address.py` & `gmsofttest-0.0.8/src/gmsofttest/china_address.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_assert_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_assert_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_excel_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_excel_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_parse_response_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_parse_response_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 Time    : 2023-05-16 9:33
 Desc:  快速解析请求返回text，并获取自己想要的数据。需学习jsonpath插件
 """
 
 import json
 from jsonpath import jsonpath
 
-def extract_json_data(text, jsonpath_expression):
+def gm_extract_json(text, jsonpath_expression):
     """使用jsonpath工具类解析请求返回值"""
     try:
         # 判断是否
         if isinstance(text, dict):
             data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
         elif isinstance(text, str):
             data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
         elif isinstance(text, list):
             data = jsonpath(text, jsonpath_expression)  # 使用jsonpath进行解析
         else:
-            json_text = json.loads(text)  # 转换requests请求返回string为python对象
+            json_text = json.loads(text)  # 如果是非dict、str、list类型，则转换成python对象
             data = jsonpath(json_text, jsonpath_expression)  # 使用jsonpath进行解析
         return data
     except TypeError as e:
         print("入参{}的类型错误，请检查,{}".format(text, e))
 
 
 if __name__ == '__main__':
```

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_randomdata_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_randomdata_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     """省份"""
     return fake.province()
 
 def getIDcard():
     """身份证号"""
     return fake.ssn()
 
+
 def getProfile():
     """生成一串用户数据"""
     return fake.profile()
 
 def getInt(min_value=0, max_value=10000, step=1):
     """生成长度在min_chars到max_chars之间整数"""
     return fake.pyint(min_value=min_value, max_value=max_value, step=step)
@@ -85,11 +86,10 @@
     return st
 
 
 if __name__ == '__main__':
     print(getMobile())
     print(getCityName())
     print(getInt())
-    print(getInt().__str__)
     print(getCompany())
     print(getProfile())
     print(getIDcard())
```

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_request_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_request_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_sqlconn_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_sqlconn_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_stock_enum.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_stock_enum.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_timestamp_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest/gm_yaml_process_utils.py` & `gmsofttest-0.0.8/src/gmsofttest/gm_yaml_process_utils.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.7/src/gmsofttest.egg-info/PKG-INFO` & `gmsofttest-0.0.8/src/gmsofttest.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmsofttest
-Version: 0.0.7
+Version: 0.0.8
 Summary: 大家软件内部测试技术线支撑工具
 Home-page: https://www.gec123.com
 Author: ronaldsu
 Author-email: uph4rmt@dingtalk.com
 Project-URL: Bug Tracker, https://www.gpwbeta.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 License-File: LICENSE
 
 # Gmtestplugin
 
     大家软件Python插件定制私有库开发项目
 
 ## change logs
+v0.0.8
+ 修改gm_prase_response的调用名称为gm_extract_json
+ 增加gm_sucreditcode_utils，用于生成企业社会信用代码
 
 v0.0.6 
  修改gm_request_utils的请求参数verfiy的默认值,由NONE调整成False
 
 v0.0.5
 
  增加gm_assert_utils：assert验证封装
```

### Comparing `gmsofttest-0.0.7/src/gmsofttest.egg-info/SOURCES.txt` & `gmsofttest-0.0.8/src/gmsofttest.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 src/gmsofttest/gm_assert_utils.py
 src/gmsofttest/gm_excel_utils.py
 src/gmsofttest/gm_parse_response_utils.py
 src/gmsofttest/gm_randomdata_utils.py
 src/gmsofttest/gm_request_utils.py
 src/gmsofttest/gm_sqlconn_utils.py
 src/gmsofttest/gm_stock_enum.py
+src/gmsofttest/gm_sucreditcode_utils.py
 src/gmsofttest/gm_timestamp_utils.py
 src/gmsofttest/gm_yaml_process_utils.py
 src/gmsofttest.egg-info/PKG-INFO
 src/gmsofttest.egg-info/SOURCES.txt
 src/gmsofttest.egg-info/dependency_links.txt
 src/gmsofttest.egg-info/top_level.txt
```

