# Comparing `tmp/twitter-api-client-0.8.5.tar.gz` & `tmp/twitter-api-client-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.5.tar", last modified: Fri Jun  2 17:06:28 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.6.tar", last modified: Sat Jun  3 18:36:24 2023, max compression
```

## Comparing `twitter-api-client-0.8.5.tar` & `twitter-api-client-0.8.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.5/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    11223 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    13056 2023-06-02 17:03:22.000000 twitter-api-client-0.8.5/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-05-28 16:24:21.000000 twitter-api-client-0.8.5/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23264 2023-06-02 17:01:02.000000 twitter-api-client-0.8.5/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28454 2023-06-02 01:49:12.000000 twitter-api-client-0.8.5/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 17:01:01.000000 twitter-api-client-0.8.5/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    27552 2023-06-02 17:05:12.000000 twitter-api-client-0.8.5/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.5/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9348 2023-06-02 17:01:02.000000 twitter-api-client-0.8.5/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-02 17:06:28.543697 twitter-api-client-0.8.5/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    11223 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-02 17:06:28.000000 twitter-api-client-0.8.5/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.6/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-03 18:35:25.000000 twitter-api-client-0.8.6/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-03 18:36:24.064571 twitter-api-client-0.8.6/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.6/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23264 2023-06-02 20:06:40.000000 twitter-api-client-0.8.6/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28454 2023-06-02 01:49:12.000000 twitter-api-client-0.8.6/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.6/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    27547 2023-06-03 18:35:00.000000 twitter-api-client-0.8.6/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.6/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9348 2023-06-02 17:01:02.000000 twitter-api-client-0.8.6/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.5/LICENSE` & `twitter-api-client-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.5/PKG-INFO` & `twitter-api-client-0.8.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.5
+Version: 0.8.6
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 ## Implementation of Twitter's v1, v2, and GraphQL APIs
 
-Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
-
-Automated email challenge solvers are supported for **Proton Mail** accounts using [proton-python-client](https://github.com/ProtonMail/proton-python-client). See [here](#automated-solvers) for more information.
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Automation](#automation)
 * [Scraping](#scraping)
   * [Get all user/tweet data](#get-all-usertweet-data)
```

### Comparing `twitter-api-client-0.8.5/setup.py` & `twitter-api-client-0.8.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,21 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.5",
+    version="0.8.6",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
 
-    Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
-    
-    Automated email challenge solvers are supported for **Proton Mail** accounts using [proton-python-client](https://github.com/ProtonMail/proton-python-client). See [here](#automated-solvers) for more information.
     
     ## Table of Contents
     
     * [Installation](#installation)
     * [Automation](#automation)
     * [Scraping](#scraping)
       * [Get all user/tweet data](#get-all-usertweet-data)
```

### Comparing `twitter-api-client-0.8.5/twitter/account.py` & `twitter-api-client-0.8.6/twitter/account.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.5/twitter/constants.py` & `twitter-api-client-0.8.6/twitter/constants.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.5/twitter/login.py` & `twitter-api-client-0.8.6/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.5/twitter/scraper.py` & `twitter-api-client-0.8.6/twitter/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         Use the batched query `users_by_ids` instead if you wish to pull user profile data.
         """
         return self._run(Operation.UserByRestId, user_ids, **kwargs)
 
     def tweet_stats(self, user_ids: list[int], **kwargs) -> list[dict]:
         return self._run(Operation.TweetStats, user_ids, **kwargs)
 
-    def users_by_rest_ids(self, user_ids: list[int], **kwargs) -> list[dict]:
+    def users_by_ids(self, user_ids: list[int], **kwargs) -> list[dict]:
         return self._run(Operation.UsersByRestIds, batch_ids(user_ids), **kwargs)
 
     def recommended_users(self, user_ids: list[int] = None, **kwargs) -> dict:
         if user_ids:
             contexts = [{"context": orjson.dumps({"contextualUserId": x}).decode()} for x in user_ids]
         else:
             contexts = [{'context': None}]
```

### Comparing `twitter-api-client-0.8.5/twitter/search.py` & `twitter-api-client-0.8.6/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.5/twitter/util.py` & `twitter-api-client-0.8.6/twitter/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.5/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.6/twitter_api_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.5
+Version: 0.8.6
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 ## Implementation of Twitter's v1, v2, and GraphQL APIs
 
-Tools include: [Scraping](#scraping), [Account Automation](#automation), [Search](#search)
-
-Automated email challenge solvers are supported for **Proton Mail** accounts using [proton-python-client](https://github.com/ProtonMail/proton-python-client). See [here](#automated-solvers) for more information.
 
 ## Table of Contents
 
 * [Installation](#installation)
 * [Automation](#automation)
 * [Scraping](#scraping)
   * [Get all user/tweet data](#get-all-usertweet-data)
```

