# Comparing `tmp/uium-0.3.6.tar.gz` & `tmp/uium-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uium-0.3.6.tar", max compression
+gzip compressed data, was "uium-0.3.7.tar", max compression
```

## Comparing `uium-0.3.6.tar` & `uium-0.3.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.6/LICENSE
--rw-r--r--   0        0        0     1478 2023-06-02 07:32:58.819073 uium-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.6/README.md
--rw-r--r--   0        0        0     1035 2023-06-02 07:33:26.354098 uium-0.3.6/uium/__init__.py
--rw-r--r--   0        0        0     1579 2023-05-30 16:23:02.395487 uium-0.3.6/uium/_auto_electron.py
--rw-r--r--   0        0        0     3242 2023-05-31 14:22:37.155376 uium-0.3.6/uium/_install_driver.py
--rw-r--r--   0        0        0       14 2023-05-30 15:45:01.782811 uium-0.3.6/uium/_mirror.py
--rw-r--r--   0        0        0      137 2023-05-30 16:24:23.007397 uium-0.3.6/uium/_uium.py
--rw-r--r--   0        0        0       14 2023-05-30 15:44:58.897076 uium-0.3.6/uium/_webdriver_manager.py
--rw-r--r--   0        0        0      914 2023-05-31 14:23:25.829837 uium-0.3.6/uium/selenium.py
--rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 uium-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1478 2023-06-03 15:21:44.902705 uium-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.7/README.md
+-rw-r--r--   0        0        0     1034 2023-06-03 15:21:29.251114 uium-0.3.7/uium/__init__.py
+-rw-r--r--   0        0        0     1561 2023-06-03 15:21:11.254690 uium-0.3.7/uium/auto_electron.py
+-rw-r--r--   0        0        0     3224 2023-06-03 15:21:02.272034 uium-0.3.7/uium/install_driver.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:20:53.730427 uium-0.3.7/uium/mirror.py
+-rw-r--r--   0        0        0      884 2023-06-03 15:20:45.343139 uium-0.3.7/uium/selenium.py
+-rw-r--r--   0        0        0       94 2023-06-03 15:20:33.402600 uium-0.3.7/uium/uium.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:20:18.883480 uium-0.3.7/uium/webdriver_manager.py
+-rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 uium-0.3.7/PKG-INFO
```

### Comparing `uium-0.3.6/LICENSE` & `uium-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uium-0.3.6/pyproject.toml` & `uium-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uium"
-version = "0.3.6"
+version = "0.3.7"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/uium"
 repository = "https://github.com/MarkHoo/uium"
 classifiers = [
```

### Comparing `uium-0.3.6/README.md` & `uium-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `uium-0.3.6/uium/__init__.py` & `uium-0.3.7/uium/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from selenium.webdriver.chrome.service import Service as ChromiumService
 # webdriver manager modules
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 
 __all__ = ["Chrome", "ChromeOptions", "webdriver", "Options", "ChromiumService", "ChromeDriverManager", "ChromeType"]
-__version__ = "v0.3.6"
+__version__ = "0.3.7"
 
 
 """
 TODO:
 - 集成Chrome驱动管理
 - 集成隐藏Chrome指纹防反爬
 - 根据ip来自动选择最近的ChromeDriver镜像点
```

### Comparing `uium-0.3.6/uium/_auto_electron.py` & `uium-0.3.7/uium/auto_electron.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,10 +30,7 @@
 
     wait = WebDriverWait(browser, 5)
     print("browser.title:", browser.title)
     print("browser.current_url:", browser.current_url)
     print("创建新的请求，即将点击 new 按钮")
     new_tab = browser.find_element(By.XPATH, '//*[@id="app-root"]/div/div/div[6]/div[1]/div[1]/div/div/div/div[1]/div[1]/div/div/div[1]/div[2]/div/div[1]')
     new_tab.click()
-
-
-__all__ = []
```

### Comparing `uium-0.3.6/uium/_install_driver.py` & `uium-0.3.7/uium/install_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,10 +76,7 @@
                 f'The downloaded ChromeDriver version {latest_version} may not be compatible with your Chrome browser version. Local version: {local_version}')
 
         driver.quit()
 
     else:
         print(f'Failed to download ChromeDriver. Status code: {response.status_code}')
 
-
-
-__all__ = []
```

### Comparing `uium-0.3.6/uium/selenium.py` & `uium-0.3.7/uium/selenium.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,10 +18,7 @@
         browser = webdriver.Chrome(service=service, options=options)
         browser.get(page)
         return browser
 
 
     browser = simple_chrome("https://sogou.com")
     browser2 = simple_chrome("https://bing.com")
-
-
-__all__ = ["ChromeType"]
```

### Comparing `uium-0.3.6/PKG-INFO` & `uium-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uium
-Version: 0.3.6
+Version: 0.3.7
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/uium
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

