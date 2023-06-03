# Comparing `tmp/terratalk-0.2.2.tar.gz` & `tmp/terratalk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terratalk-0.2.2.tar", last modified: Thu Nov 11 21:08:33 2021, max compression
+gzip compressed data, was "terratalk-0.3.0.tar", last modified: Sat Jun  3 13:31:34 2023, max compression
```

## Comparing `terratalk-0.2.2.tar` & `terratalk-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-11 21:08:33.806215 terratalk-0.2.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2021-11-11 21:08:03.000000 terratalk-0.2.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2021-11-11 21:08:33.806215 terratalk-0.2.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2062 2021-11-11 21:08:03.000000 terratalk-0.2.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-11-11 21:08:33.806215 terratalk-0.2.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2021-11-11 21:08:03.000000 terratalk-0.2.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-11 21:08:33.806215 terratalk-0.2.2/terratalk/
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2021-11-11 21:08:03.000000 terratalk-0.2.2/terratalk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3099 2021-11-11 21:08:03.000000 terratalk-0.2.2/terratalk/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2546 2021-11-11 21:08:03.000000 terratalk-0.2.2/terratalk/bitbucket_server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2139 2021-11-11 21:08:03.000000 terratalk-0.2.2/terratalk/terraform_out.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-11 21:08:33.806215 terratalk-0.2.2/terratalk.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2554 2021-11-11 21:08:33.000000 terratalk-0.2.2/terratalk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2021-11-11 21:08:33.000000 terratalk-0.2.2/terratalk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-11 21:08:33.000000 terratalk-0.2.2/terratalk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       54 2021-11-11 21:08:33.000000 terratalk-0.2.2/terratalk.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2021-11-11 21:08:33.000000 terratalk-0.2.2/terratalk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2021-11-11 21:08:33.000000 terratalk-0.2.2/terratalk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:31:34.144892 terratalk-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 13:31:19.000000 terratalk-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-03 13:31:34.144892 terratalk-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-03 13:31:19.000000 terratalk-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 13:31:34.144892 terratalk-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-03 13:31:19.000000 terratalk-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:31:34.140892 terratalk-0.3.0/terratalk/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-03 13:31:19.000000 terratalk-0.3.0/terratalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-03 13:31:19.000000 terratalk-0.3.0/terratalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-03 13:31:19.000000 terratalk-0.3.0/terratalk/bitbucket_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-03 13:31:19.000000 terratalk-0.3.0/terratalk/bitbucket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-03 13:31:19.000000 terratalk-0.3.0/terratalk/terraform_out.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:31:34.144892 terratalk-0.3.0/terratalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-03 13:31:34.000000 terratalk-0.3.0/terratalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-03 13:31:34.000000 terratalk-0.3.0/terratalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:31:34.000000 terratalk-0.3.0/terratalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-03 13:31:34.000000 terratalk-0.3.0/terratalk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-03 13:31:34.000000 terratalk-0.3.0/terratalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-03 13:31:34.000000 terratalk-0.3.0/terratalk.egg-info/top_level.txt
```

### Comparing `terratalk-0.2.2/LICENSE` & `terratalk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terratalk-0.2.2/PKG-INFO` & `terratalk-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: terratalk
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Terraform commentator.
 Home-page: https://github.com/lifeofguenter/terratalk
 Author: Günter Grodotzki
 Author-email: gunter@grodotzki.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: GitHub
 License-File: LICENSE
 
 # terratalk
 
-[![Build Status](https://app.travis-ci.com/lifeofguenter/terratalk.svg?branch=main)](https://app.travis-ci.com/lifeofguenter/terratalk)
+[![build and publish](https://github.com/lifeofguenter/terratalk/actions/workflows/build-and-publish.yml/badge.svg)](https://github.com/lifeofguenter/terratalk/actions/workflows/build-and-publish.yml)
 [![Coverage Status](https://coveralls.io/repos/github/lifeofguenter/terratalk/badge.svg)](https://coveralls.io/github/lifeofguenter/terratalk)
 [![PyPI](https://img.shields.io/pypi/v/terratalk.svg)](https://pypi.org/project/terratalk/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/terratalk)
 [![License](https://img.shields.io/github/license/lifeofguenter/terratalk.svg)](LICENSE)
 
 **_Terratalk_** is a simple tool to add an opinionated terraform plan output
 into your pull-request as a comment. This allows you to have a quick feedback on
@@ -40,21 +38,21 @@
 allow `terratalk` to construct the proper API request to your SCM.
 
 ### Installation
 
 On the build agent, install `terratalk`:
 
 ```bash
-$ sudo -H pip install terratalk
+$ pip install --user terratalk
 ```
 
 If you are using GitHub you will additionally need to install the following:
 
 ```bash
-$ sudo -H pip install PyGithub
+$ pip install --user PyGithub
 ```
 
 ### Running
 
 Execute in the same directory, optionally with the same `TF_DATA_DIR` as you
 would normally run `terraform`. If you use
 [`tfenv`](https://github.com/tfutils/tfenv) that will work as well.
@@ -62,25 +60,28 @@
 ```bash
 $ terraform plan -out WORKSPACE.plan
 $ terratalk comment -w WORKSPACE
 ```
 
 ### Supported environment variables
 
-#### Bitbucket
+#### Bitbucket Server
 
 * `STASH_USER`
 * `STASH_PASS`
 
+#### Bitbucket Cloud
+
+* `BITBUCKET_USERNAME`
+* `BITBUCKET_APP_PASSWORD`
+
 #### GitHub
 
 * `GITHUB_TOKEN`
 
 ## Results
 
 ![terratalk on Bitbucket Server](https://raw.githubusercontent.com/lifeofguenter/terratalk/main/docs/images/terratalk-on-bitbucket-server.png "terratalk on Bitbucket Server")
 
 ## License
 
 [MIT](LICENSE)
-
-
```

### Comparing `terratalk-0.2.2/README.md` & `terratalk-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # terratalk
 
-[![Build Status](https://app.travis-ci.com/lifeofguenter/terratalk.svg?branch=main)](https://app.travis-ci.com/lifeofguenter/terratalk)
+[![build and publish](https://github.com/lifeofguenter/terratalk/actions/workflows/build-and-publish.yml/badge.svg)](https://github.com/lifeofguenter/terratalk/actions/workflows/build-and-publish.yml)
 [![Coverage Status](https://coveralls.io/repos/github/lifeofguenter/terratalk/badge.svg)](https://coveralls.io/github/lifeofguenter/terratalk)
 [![PyPI](https://img.shields.io/pypi/v/terratalk.svg)](https://pypi.org/project/terratalk/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/terratalk)
 [![License](https://img.shields.io/github/license/lifeofguenter/terratalk.svg)](LICENSE)
 
 **_Terratalk_** is a simple tool to add an opinionated terraform plan output
 into your pull-request as a comment. This allows you to have a quick feedback on
@@ -23,21 +23,21 @@
 allow `terratalk` to construct the proper API request to your SCM.
 
 ### Installation
 
 On the build agent, install `terratalk`:
 
 ```bash
-$ sudo -H pip install terratalk
+$ pip install --user terratalk
 ```
 
 If you are using GitHub you will additionally need to install the following:
 
 ```bash
-$ sudo -H pip install PyGithub
+$ pip install --user PyGithub
 ```
 
 ### Running
 
 Execute in the same directory, optionally with the same `TF_DATA_DIR` as you
 would normally run `terraform`. If you use
 [`tfenv`](https://github.com/tfutils/tfenv) that will work as well.
@@ -45,19 +45,24 @@
 ```bash
 $ terraform plan -out WORKSPACE.plan
 $ terratalk comment -w WORKSPACE
 ```
 
 ### Supported environment variables
 
-#### Bitbucket
+#### Bitbucket Server
 
 * `STASH_USER`
 * `STASH_PASS`
 
+#### Bitbucket Cloud
+
+* `BITBUCKET_USERNAME`
+* `BITBUCKET_APP_PASSWORD`
+
 #### GitHub
 
 * `GITHUB_TOKEN`
 
 ## Results
 
 ![terratalk on Bitbucket Server](https://raw.githubusercontent.com/lifeofguenter/terratalk/main/docs/images/terratalk-on-bitbucket-server.png "terratalk on Bitbucket Server")
```

### Comparing `terratalk-0.2.2/setup.py` & `terratalk-0.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,35 @@
-import re
-import setuptools
+from setuptools import setup, find_packages
 from distutils.util import convert_path
 
 
-def find_version():
-    with open(convert_path('terratalk/__init__.py')) as fh:
-        version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]",
-                                  fh.read(), re.M)
-
-        if version_match:
-            return version_match.group(1)
-
-    raise RuntimeError("Unable to find version string.")
-
-
 def find_description():
     with open(convert_path('README.md')) as fh:
         return fh.read()
 
 
-setuptools.setup(
+setup(
     name='terratalk',
-    version=find_version(),
+    version='0.3.0',
+    py_modules=['cli'],
     author='Günter Grodotzki',
     author_email='gunter@grodotzki.com',
     description='A Terraform commentator.',
     long_description=find_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/lifeofguenter/terratalk',
-    packages=setuptools.find_packages(exclude=['tests*']),
+    packages=find_packages(exclude=['tests*']),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3',
     install_requires=[
-        'click',
+        'Click',
         'requests',
     ],
     extras_require={
         'GitHub': ['PyGithub'],
     },
     entry_points={
         'console_scripts': [
```

### Comparing `terratalk-0.2.2/terratalk/__main__.py` & `terratalk-0.3.0/terratalk/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 import os
 import re
 
 import click
 
-from terratalk import __version__ as terratalk_version
 from terratalk.terraform_out import TerraformOut
 
 
 @click.group()
-@click.version_option(terratalk_version)
+@click.version_option()
 def cli():
     pass
 
 
 @cli.command()
 @click.option('-w', '--workspace')
 def comment(workspace):
 
     m = re.search(
-        r'\Ahttps://github.com/([^/]+)/([^/]+)/pull/(\d+)\Z',
+        r'\A(https?://.*?)/projects/([^/]+)/repos/([^/]+)/pull-requests/(\d+)',
         os.getenv('CHANGE_URL'),
         re.IGNORECASE,
     )
+
     if not m:
         m = re.search(
-            r'\A(https?://.*?)/projects/([^/]+)/repos/([^/]+)/'
-            r'pull-requests/(\d+)',
+            r'\Ahttps://(github\.com|bitbucket\.org)'
+            r'/([^/]+)/([^/]+)/(?:pull|pull-requests)/(\d+)\Z',
             os.getenv('CHANGE_URL'),
             re.IGNORECASE,
         )
 
-    if len(m.groups()) == 3:
-        server = 'github'
-        project_key = m.group(1)
-        repository_slug = m.group(2)
-        pull_request_id = int(m.group(3))
+    server = m.group(1)
+    project_key = m.group(2)
+    repository_slug = m.group(3)
+    pull_request_id = int(m.group(4))
 
-    else:
-        server = m.group(1)
-        project_key = m.group(2)
-        repository_slug = m.group(3)
-        pull_request_id = int(m.group(4))
+    # fetch terraform output
+    tf = TerraformOut(workspace + '.plan')
+
+    if tf.does_nothing():
+        click.echo('[terratalk] this plan does nothing')
 
-    if server == 'github':
+    if server == 'github.com':
         from github import Github
 
         gh = Github(os.getenv('GITHUB_TOKEN'))
 
         repo = gh.get_repo(f'{project_key}/{repository_slug}')
         issue = repo.get_issue(pull_request_id)
 
@@ -54,14 +53,52 @@
         for c in issue.get_comments():
             if c.body.lstrip().startswith(f'<!-- terratalk: {workspace} -->'):
                 click.echo(
                     f'[tf-comment-plan] deleting previous comment: {c.id}'
                 )
                 c.delete()
 
+        if not tf.does_nothing():
+            issue.create_comment(f'''
+<!-- terratalk: {workspace} -->
+### tf plan output: {workspace}
+```diff
+{tf.show()}
+```
+''')
+
+    elif server == 'bitbucket.org':
+        from terratalk.bitbucket_cloud import BitbucketCloud
+
+        bb = BitbucketCloud(
+            username=os.getenv('BITBUCKET_USERNAME'),
+            password=os.getenv('BITBUCKET_APP_PASSWORD'),
+        )
+
+        bb.pr(
+            project_key=project_key,
+            repository_slug=repository_slug,
+            pull_request_id=pull_request_id,
+        )
+
+        for c in bb.comments():
+            if c['content']['raw'].lstrip().startswith(
+                f'### tf plan output: {workspace}'
+            ):
+                click.echo(f"[terratalk] deleting previous comment {c['id']}")
+                bb.comment_delete(c['id'])
+
+        if not tf.does_nothing():
+            bb.comment_add(f'''
+### tf plan output: {workspace}
+```diff
+{tf.show()}
+```
+''')
+
     else:
         from terratalk.bitbucket_server import BitbucketServer
 
         bs = BitbucketServer(
             base_url=server,
             username=os.getenv('STASH_USER'),
             password=os.getenv('STASH_PASS'),
@@ -76,33 +113,17 @@
         for c in bs.comments():
             if c['comment']['text'].lstrip().startswith(
                 f'[comment]: # (terratalk: {workspace})'
             ):
                 click.echo(f"[terratalk] deleting previous comment {c['id']}")
                 bs.comment_delete(c['comment']['id'], c['comment']['version'])
 
-    # fetch terraform output
-    tf = TerraformOut(workspace + '.plan')
-
-    if tf.does_nothing():
-        click.echo('[terratalk] this plan does nothing')
-        exit()
-
-    if server == 'github':
-        issue.create_comment(f'''
-<!-- terratalk: {workspace} -->
-### tf plan output: {workspace}
-```diff
-{tf.show()}
-```
-''')
-
-    else:
-        # https://bitbucket.org/tutorials/markdowndemo/issues/15/how-can-you-insert-comments-in-the#comment-22433250
-        bs.comment_add(f'''
+        if not tf.does_nothing():
+            # https://bitbucket.org/tutorials/markdowndemo/issues/15/how-can-you-insert-comments-in-the#comment-22433250
+            bs.comment_add(f'''
 [comment]: # (terratalk: {workspace})
 ### tf plan output: {workspace}
 ```diff
 {tf.show()}
 ```
 ''')
```

### Comparing `terratalk-0.2.2/terratalk/bitbucket_server.py` & `terratalk-0.3.0/terratalk/bitbucket_server.py`

 * *Files identical despite different names*

### Comparing `terratalk-0.2.2/terratalk/terraform_out.py` & `terratalk-0.3.0/terratalk/terraform_out.py`

 * *Files identical despite different names*

### Comparing `terratalk-0.2.2/terratalk.egg-info/PKG-INFO` & `terratalk-0.3.0/terratalk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: terratalk
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Terraform commentator.
 Home-page: https://github.com/lifeofguenter/terratalk
 Author: Günter Grodotzki
 Author-email: gunter@grodotzki.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: GitHub
 License-File: LICENSE
 
 # terratalk
 
-[![Build Status](https://app.travis-ci.com/lifeofguenter/terratalk.svg?branch=main)](https://app.travis-ci.com/lifeofguenter/terratalk)
+[![build and publish](https://github.com/lifeofguenter/terratalk/actions/workflows/build-and-publish.yml/badge.svg)](https://github.com/lifeofguenter/terratalk/actions/workflows/build-and-publish.yml)
 [![Coverage Status](https://coveralls.io/repos/github/lifeofguenter/terratalk/badge.svg)](https://coveralls.io/github/lifeofguenter/terratalk)
 [![PyPI](https://img.shields.io/pypi/v/terratalk.svg)](https://pypi.org/project/terratalk/)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/terratalk)
 [![License](https://img.shields.io/github/license/lifeofguenter/terratalk.svg)](LICENSE)
 
 **_Terratalk_** is a simple tool to add an opinionated terraform plan output
 into your pull-request as a comment. This allows you to have a quick feedback on
@@ -40,21 +38,21 @@
 allow `terratalk` to construct the proper API request to your SCM.
 
 ### Installation
 
 On the build agent, install `terratalk`:
 
 ```bash
-$ sudo -H pip install terratalk
+$ pip install --user terratalk
 ```
 
 If you are using GitHub you will additionally need to install the following:
 
 ```bash
-$ sudo -H pip install PyGithub
+$ pip install --user PyGithub
 ```
 
 ### Running
 
 Execute in the same directory, optionally with the same `TF_DATA_DIR` as you
 would normally run `terraform`. If you use
 [`tfenv`](https://github.com/tfutils/tfenv) that will work as well.
@@ -62,25 +60,28 @@
 ```bash
 $ terraform plan -out WORKSPACE.plan
 $ terratalk comment -w WORKSPACE
 ```
 
 ### Supported environment variables
 
-#### Bitbucket
+#### Bitbucket Server
 
 * `STASH_USER`
 * `STASH_PASS`
 
+#### Bitbucket Cloud
+
+* `BITBUCKET_USERNAME`
+* `BITBUCKET_APP_PASSWORD`
+
 #### GitHub
 
 * `GITHUB_TOKEN`
 
 ## Results
 
 ![terratalk on Bitbucket Server](https://raw.githubusercontent.com/lifeofguenter/terratalk/main/docs/images/terratalk-on-bitbucket-server.png "terratalk on Bitbucket Server")
 
 ## License
 
 [MIT](LICENSE)
-
-
```

