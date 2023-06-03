# Comparing `tmp/CheckSSLCert-0.0.1.tar.gz` & `tmp/CheckSSLCert-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CheckSSLCert-0.0.1.tar", last modified: Fri Jun  2 13:55:27 2023, max compression
+gzip compressed data, was "CheckSSLCert-0.1.0.tar", last modified: Sat Jun  3 08:39:23 2023, max compression
```

## Comparing `CheckSSLCert-0.0.1.tar` & `CheckSSLCert-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 13:55:27.757342 CheckSSLCert-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-01 13:49:19.000000 CheckSSLCert-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4412 2023-06-02 13:55:27.755704 CheckSSLCert-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3812 2023-06-02 13:45:52.000000 CheckSSLCert-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-06-02 05:24:56.000000 CheckSSLCert-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 13:55:27.757342 CheckSSLCert-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      821 2023-06-02 13:52:47.000000 CheckSSLCert-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:55:27.741742 CheckSSLCert-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 13:55:27.744734 CheckSSLCert-0.0.1/src/CheckSSLCert/
--rw-rw-rw-   0        0        0       35 2023-06-01 08:02:33.000000 CheckSSLCert-0.0.1/src/CheckSSLCert/__init__.py
--rw-rw-rw-   0        0        0    11419 2023-06-02 13:55:06.000000 CheckSSLCert-0.0.1/src/CheckSSLCert/validate.py
-drwxrwxrwx   0        0        0        0 2023-06-02 13:55:27.755704 CheckSSLCert-0.0.1/src/CheckSSLCert.egg-info/
--rw-rw-rw-   0        0        0     4412 2023-06-02 13:55:27.000000 CheckSSLCert-0.0.1/src/CheckSSLCert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-02 13:55:27.000000 CheckSSLCert-0.0.1/src/CheckSSLCert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 13:55:27.000000 CheckSSLCert-0.0.1/src/CheckSSLCert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-02 13:55:27.000000 CheckSSLCert-0.0.1/src/CheckSSLCert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.324526 CheckSSLCert-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 13:49:19.000000 CheckSSLCert-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4763 2023-06-03 08:39:23.277628 CheckSSLCert-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4074 2023-06-03 07:51:20.000000 CheckSSLCert-0.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-06-02 05:24:56.000000 CheckSSLCert-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 08:39:23.324526 CheckSSLCert-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      908 2023-06-03 08:38:48.000000 CheckSSLCert-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.262007 CheckSSLCert-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.262007 CheckSSLCert-0.1.0/src/CheckSSLCert/
+-rw-rw-rw-   0        0        0       35 2023-06-01 08:02:33.000000 CheckSSLCert-0.1.0/src/CheckSSLCert/__init__.py
+-rw-rw-rw-   0        0        0    11419 2023-06-02 13:55:06.000000 CheckSSLCert-0.1.0/src/CheckSSLCert/validate.py
+drwxrwxrwx   0        0        0        0 2023-06-03 08:39:23.277628 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/
+-rw-rw-rw-   0        0        0     4763 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-03 08:39:23.000000 CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/top_level.txt
```

### Comparing `CheckSSLCert-0.0.1/LICENSE` & `CheckSSLCert-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CheckSSLCert-0.0.1/PKG-INFO` & `CheckSSLCert-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: CheckSSLCert
-Version: 0.0.1
-Summary: CheckSSLCert is a Python library that allows you to check the SSL certificate status.
-Home-page: https://github.com/Huntroid-India/CheckSSLCert
-Author: Huntriod
-Author-email: srimath8@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/Huntroid-India/CheckSSLCert/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CheckSSLCert
 [![Made with Python](https://img.shields.io/badge/Python->=3.6-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 
 
 [![Huntroid-India - SSLCheckerr](https://img.shields.io/static/v1?label=Huntroid-India&message=CheckSSLCert&color=blue&logo=github)](https://github.com/Huntroid-India/CheckSSLCert "Go to GitHub repo")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 [![stars - SSLChecker](https://img.shields.io/github/stars/Huntroid-India/CheckSSLCert?style=social)](https://github.com/Huntroid-India/CheckSSLCert)
@@ -63,14 +47,18 @@
 
 # Create a bulksslchecker object with the path to the domain list file (CSV format)
 checker = validate.from_file("domain_list.csv")
 
 # Print the SSL certificate status report to the console
 checker.print_report()
 
+# Send the SSL certificate status report to an email address
+checker.send_report("sender_address", "sender_password", "receiver_address", "Subject")
+# Note: It is recommended to use an app password for the sender password. It only works with Gmail(Sender).
+
 # Save the SSL certificate status report to a file (HTML format)
 checker.save_report("C:\Users\YourUsername\Desktop") # By default HTML is selected
 checker.save_report("C:\Users\YourUsername\Desktop", "html")
 
 # Save the SSL certificate status report to a file (CSV format)
 checker.save_report("C:\Users\YourUsername\Desktop", "csv")
 ```
```

### Comparing `CheckSSLCert-0.0.1/README.md` & `CheckSSLCert-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: CheckSSLCert
+Version: 0.1.0
+Summary: CheckSSLCert is a Python library that allows you to check the SSL certificate status.
+Home-page: https://github.com/Huntroid-India/CheckSSLCert
+Author: Srimath
+Author-email: srimath8@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/Huntroid-India/CheckSSLCert/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CheckSSLCert
 [![Made with Python](https://img.shields.io/badge/Python->=3.6-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 
 
 [![Huntroid-India - SSLCheckerr](https://img.shields.io/static/v1?label=Huntroid-India&message=CheckSSLCert&color=blue&logo=github)](https://github.com/Huntroid-India/CheckSSLCert "Go to GitHub repo")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 [![stars - SSLChecker](https://img.shields.io/github/stars/Huntroid-India/CheckSSLCert?style=social)](https://github.com/Huntroid-India/CheckSSLCert)
@@ -47,14 +65,18 @@
 
 # Create a bulksslchecker object with the path to the domain list file (CSV format)
 checker = validate.from_file("domain_list.csv")
 
 # Print the SSL certificate status report to the console
 checker.print_report()
 
+# Send the SSL certificate status report to an email address
+checker.send_report("sender_address", "sender_password", "receiver_address", "Subject")
+# Note: It is recommended to use an app password for the sender password. It only works with Gmail(Sender).
+
 # Save the SSL certificate status report to a file (HTML format)
 checker.save_report("C:\Users\YourUsername\Desktop") # By default HTML is selected
 checker.save_report("C:\Users\YourUsername\Desktop", "html")
 
 # Save the SSL certificate status report to a file (CSV format)
 checker.save_report("C:\Users\YourUsername\Desktop", "csv")
 ```
```

### Comparing `CheckSSLCert-0.0.1/setup.py` & `CheckSSLCert-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import setuptools
 
 setuptools.setup(
     name='CheckSSLCert',
-    version='0.0.1',
+    version='0.1.0',
     url='https://github.com/Huntroid-India/CheckSSLCert',
     project_urls={
         "Bug Tracker": "https://github.com/Huntroid-India/CheckSSLCert/issues",
     },
     license='MIT',
-    author='Huntriod',
+    author='Srimath',
     author_email='srimath8@gmail.com',
     description='CheckSSLCert is a Python library that allows you to check the SSL certificate status.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     package_dir={'': "src"},
     packages=setuptools.find_packages("src"),
     classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"],
     python_requires='>=3.6'
 )
```

### Comparing `CheckSSLCert-0.0.1/src/CheckSSLCert/validate.py` & `CheckSSLCert-0.1.0/src/CheckSSLCert/validate.py`

 * *Files identical despite different names*

### Comparing `CheckSSLCert-0.0.1/src/CheckSSLCert.egg-info/PKG-INFO` & `CheckSSLCert-0.1.0/src/CheckSSLCert.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: CheckSSLCert
-Version: 0.0.1
+Version: 0.1.0
 Summary: CheckSSLCert is a Python library that allows you to check the SSL certificate status.
 Home-page: https://github.com/Huntroid-India/CheckSSLCert
-Author: Huntriod
+Author: Srimath
 Author-email: srimath8@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Huntroid-India/CheckSSLCert/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -63,14 +65,18 @@
 
 # Create a bulksslchecker object with the path to the domain list file (CSV format)
 checker = validate.from_file("domain_list.csv")
 
 # Print the SSL certificate status report to the console
 checker.print_report()
 
+# Send the SSL certificate status report to an email address
+checker.send_report("sender_address", "sender_password", "receiver_address", "Subject")
+# Note: It is recommended to use an app password for the sender password. It only works with Gmail(Sender).
+
 # Save the SSL certificate status report to a file (HTML format)
 checker.save_report("C:\Users\YourUsername\Desktop") # By default HTML is selected
 checker.save_report("C:\Users\YourUsername\Desktop", "html")
 
 # Save the SSL certificate status report to a file (CSV format)
 checker.save_report("C:\Users\YourUsername\Desktop", "csv")
 ```
```

