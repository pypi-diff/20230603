# Comparing `tmp/taskhawk-4.2.0.tar.gz` & `tmp/taskhawk-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskhawk-4.2.0.tar", last modified: Wed Nov 30 05:34:06 2022, max compression
+gzip compressed data, was "taskhawk-4.2.1.tar", last modified: Sat Jun  3 00:17:03 2023, max compression
```

## Comparing `taskhawk-4.2.0.tar` & `taskhawk-4.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-11-30 05:34:06.504150 taskhawk-4.2.0/
--rw-r--r--   0 maru       (501) staff       (20)      348 2020-03-12 19:54:19.000000 taskhawk-4.2.0/CONTRIBUTORS.txt
--rw-r--r--   0 maru       (501) staff       (20)    11342 2021-07-30 00:29:32.000000 taskhawk-4.2.0/LICENSE.md
--rw-r--r--   0 maru       (501) staff       (20)      162 2020-03-12 19:54:19.000000 taskhawk-4.2.0/MANIFEST.in
--rw-r--r--   0 maru       (501) staff       (20)     5395 2022-11-30 05:34:06.504380 taskhawk-4.2.0/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)     4432 2021-07-30 00:29:32.000000 taskhawk-4.2.0/README.rst
--rw-r--r--   0 maru       (501) staff       (20)      244 2020-03-12 19:54:19.000000 taskhawk-4.2.0/pyproject.toml
--rw-r--r--   0 maru       (501) staff       (20)      316 2022-11-30 05:34:06.505489 taskhawk-4.2.0/setup.cfg
--rw-r--r--   0 maru       (501) staff       (20)     3197 2022-11-29 05:20:56.000000 taskhawk-4.2.0/setup.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-11-30 05:34:06.485310 taskhawk-4.2.0/taskhawk/
--rw-r--r--   0 maru       (501) staff       (20)      632 2022-11-30 05:33:57.000000 taskhawk-4.2.0/taskhawk/__init__.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-11-30 05:34:06.491360 taskhawk-4.2.0/taskhawk/backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.0/taskhawk/backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     9887 2022-11-29 05:20:56.000000 taskhawk-4.2.0/taskhawk/backends/aws.py
--rw-r--r--   0 maru       (501) staff       (20)     6872 2022-11-30 05:33:20.000000 taskhawk-4.2.0/taskhawk/backends/base.py
--rw-r--r--   0 maru       (501) staff       (20)      343 2020-03-12 19:54:19.000000 taskhawk-4.2.0/taskhawk/backends/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)    10881 2022-11-30 05:33:20.000000 taskhawk-4.2.0/taskhawk/backends/gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      567 2020-03-12 19:54:19.000000 taskhawk-4.2.0/taskhawk/backends/import_utils.py
--rw-r--r--   0 maru       (501) staff       (20)     1121 2020-03-12 19:54:19.000000 taskhawk-4.2.0/taskhawk/backends/utils.py
--rw-r--r--   0 maru       (501) staff       (20)      809 2022-11-29 05:20:56.000000 taskhawk-4.2.0/taskhawk/commands.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-11-30 05:34:06.492090 taskhawk-4.2.0/taskhawk/conf/
--rw-r--r--   0 maru       (501) staff       (20)     6930 2022-04-12 21:04:16.000000 taskhawk-4.2.0/taskhawk/conf/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     2983 2022-11-29 05:20:56.000000 taskhawk-4.2.0/taskhawk/consumer.py
--rw-r--r--   0 maru       (501) staff       (20)      980 2022-11-28 19:50:36.000000 taskhawk-4.2.0/taskhawk/exceptions.py
--rw-r--r--   0 maru       (501) staff       (20)     9359 2022-11-29 05:20:56.000000 taskhawk-4.2.0/taskhawk/models.py
--rw-r--r--   0 maru       (501) staff       (20)      525 2022-11-29 05:20:56.000000 taskhawk-4.2.0/taskhawk/publisher.py
--rw-r--r--   0 maru       (501) staff       (20)     7975 2022-04-13 05:43:22.000000 taskhawk-4.2.0/taskhawk/task_manager.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-11-30 05:34:06.487424 taskhawk-4.2.0/taskhawk.egg-info/
--rw-r--r--   0 maru       (501) staff       (20)     5395 2022-11-30 05:34:06.000000 taskhawk-4.2.0/taskhawk.egg-info/PKG-INFO
--rw-r--r--   0 maru       (501) staff       (20)      959 2022-11-30 05:34:06.000000 taskhawk-4.2.0/taskhawk.egg-info/SOURCES.txt
--rw-r--r--   0 maru       (501) staff       (20)        1 2022-11-30 05:34:06.000000 taskhawk-4.2.0/taskhawk.egg-info/dependency_links.txt
--rw-r--r--   0 maru       (501) staff       (20)      478 2022-11-30 05:34:06.000000 taskhawk-4.2.0/taskhawk.egg-info/requires.txt
--rw-r--r--   0 maru       (501) staff       (20)        9 2022-11-30 05:34:06.000000 taskhawk-4.2.0/taskhawk.egg-info/top_level.txt
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-11-30 05:34:06.500491 taskhawk-4.2.0/tests/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)     4363 2022-11-29 05:20:56.000000 taskhawk-4.2.0/tests/conftest.py
--rw-r--r--   0 maru       (501) staff       (20)      201 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/settings.py
--rw-r--r--   0 maru       (501) staff       (20)      661 2021-07-06 19:19:15.000000 taskhawk-4.2.0/tests/tasks.py
-drwxr-xr-x   0 maru       (501) staff       (20)        0 2022-11-30 05:34:06.503446 taskhawk-4.2.0/tests/test_backends/
--rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/test_backends/__init__.py
--rw-r--r--   0 maru       (501) staff       (20)    12649 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/test_backends/test_aws.py
--rw-r--r--   0 maru       (501) staff       (20)    10558 2021-07-06 19:19:15.000000 taskhawk-4.2.0/tests/test_backends/test_base.py
--rw-r--r--   0 maru       (501) staff       (20)    12496 2022-11-30 05:33:20.000000 taskhawk-4.2.0/tests/test_backends/test_gcp.py
--rw-r--r--   0 maru       (501) staff       (20)      481 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/test_commands.py
--rw-r--r--   0 maru       (501) staff       (20)     1101 2022-11-28 19:50:36.000000 taskhawk-4.2.0/tests/test_consumer.py
--rw-r--r--   0 maru       (501) staff       (20)     5851 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/test_models.py
--rw-r--r--   0 maru       (501) staff       (20)      383 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/test_publisher.py
--rw-r--r--   0 maru       (501) staff       (20)      607 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/test_settings.py
--rw-r--r--   0 maru       (501) staff       (20)     8474 2020-03-12 19:54:19.000000 taskhawk-4.2.0/tests/test_task_manager.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.070654 taskhawk-4.2.1/
+-rw-r--r--   0 maru       (501) staff       (20)      348 2020-03-12 19:54:19.000000 taskhawk-4.2.1/CONTRIBUTORS.txt
+-rw-r--r--   0 maru       (501) staff       (20)    11342 2021-07-30 00:29:32.000000 taskhawk-4.2.1/LICENSE.md
+-rw-r--r--   0 maru       (501) staff       (20)      162 2020-03-12 19:54:19.000000 taskhawk-4.2.1/MANIFEST.in
+-rw-r--r--   0 maru       (501) staff       (20)     5395 2023-06-03 00:17:03.070708 taskhawk-4.2.1/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)     4432 2021-07-30 00:29:32.000000 taskhawk-4.2.1/README.rst
+-rw-r--r--   0 maru       (501) staff       (20)      244 2020-03-12 19:54:19.000000 taskhawk-4.2.1/pyproject.toml
+-rw-r--r--   0 maru       (501) staff       (20)      316 2023-06-03 00:17:03.070920 taskhawk-4.2.1/setup.cfg
+-rw-r--r--   0 maru       (501) staff       (20)     3197 2022-11-29 05:20:56.000000 taskhawk-4.2.1/setup.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.067542 taskhawk-4.2.1/taskhawk/
+-rw-r--r--   0 maru       (501) staff       (20)      632 2023-06-03 00:17:01.000000 taskhawk-4.2.1/taskhawk/__init__.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.068911 taskhawk-4.2.1/taskhawk/backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     9886 2023-06-03 00:08:40.000000 taskhawk-4.2.1/taskhawk/backends/aws.py
+-rw-r--r--   0 maru       (501) staff       (20)     6872 2022-11-30 05:33:20.000000 taskhawk-4.2.1/taskhawk/backends/base.py
+-rw-r--r--   0 maru       (501) staff       (20)      343 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)    11346 2023-06-03 00:08:40.000000 taskhawk-4.2.1/taskhawk/backends/gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      567 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/import_utils.py
+-rw-r--r--   0 maru       (501) staff       (20)     1121 2020-03-12 19:54:19.000000 taskhawk-4.2.1/taskhawk/backends/utils.py
+-rw-r--r--   0 maru       (501) staff       (20)      809 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/commands.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.069021 taskhawk-4.2.1/taskhawk/conf/
+-rw-r--r--   0 maru       (501) staff       (20)     6931 2023-06-03 00:08:40.000000 taskhawk-4.2.1/taskhawk/conf/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     2983 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/consumer.py
+-rw-r--r--   0 maru       (501) staff       (20)      980 2022-11-28 19:50:36.000000 taskhawk-4.2.1/taskhawk/exceptions.py
+-rw-r--r--   0 maru       (501) staff       (20)     9359 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/models.py
+-rw-r--r--   0 maru       (501) staff       (20)      525 2022-11-29 05:20:56.000000 taskhawk-4.2.1/taskhawk/publisher.py
+-rw-r--r--   0 maru       (501) staff       (20)     7975 2022-04-13 05:43:22.000000 taskhawk-4.2.1/taskhawk/task_manager.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.068164 taskhawk-4.2.1/taskhawk.egg-info/
+-rw-r--r--   0 maru       (501) staff       (20)     5395 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/PKG-INFO
+-rw-r--r--   0 maru       (501) staff       (20)      959 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/SOURCES.txt
+-rw-r--r--   0 maru       (501) staff       (20)        1 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/dependency_links.txt
+-rw-r--r--   0 maru       (501) staff       (20)      478 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/requires.txt
+-rw-r--r--   0 maru       (501) staff       (20)        9 2023-06-03 00:17:03.000000 taskhawk-4.2.1/taskhawk.egg-info/top_level.txt
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.070083 taskhawk-4.2.1/tests/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)     4363 2022-11-29 05:20:56.000000 taskhawk-4.2.1/tests/conftest.py
+-rw-r--r--   0 maru       (501) staff       (20)      201 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/settings.py
+-rw-r--r--   0 maru       (501) staff       (20)      661 2021-07-06 19:19:15.000000 taskhawk-4.2.1/tests/tasks.py
+drwxr-xr-x   0 maru       (501) staff       (20)        0 2023-06-03 00:17:03.070535 taskhawk-4.2.1/tests/test_backends/
+-rw-r--r--   0 maru       (501) staff       (20)        0 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_backends/__init__.py
+-rw-r--r--   0 maru       (501) staff       (20)    12649 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_backends/test_aws.py
+-rw-r--r--   0 maru       (501) staff       (20)    10558 2021-07-06 19:19:15.000000 taskhawk-4.2.1/tests/test_backends/test_base.py
+-rw-r--r--   0 maru       (501) staff       (20)    12496 2022-11-30 05:33:20.000000 taskhawk-4.2.1/tests/test_backends/test_gcp.py
+-rw-r--r--   0 maru       (501) staff       (20)      481 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_commands.py
+-rw-r--r--   0 maru       (501) staff       (20)     1101 2022-11-28 19:50:36.000000 taskhawk-4.2.1/tests/test_consumer.py
+-rw-r--r--   0 maru       (501) staff       (20)     5851 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_models.py
+-rw-r--r--   0 maru       (501) staff       (20)      383 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_publisher.py
+-rw-r--r--   0 maru       (501) staff       (20)      607 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_settings.py
+-rw-r--r--   0 maru       (501) staff       (20)     8474 2020-03-12 19:54:19.000000 taskhawk-4.2.1/tests/test_task_manager.py
```

### Comparing `taskhawk-4.2.0/LICENSE.md` & `taskhawk-4.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/PKG-INFO` & `taskhawk-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskhawk
-Version: 4.2.0
+Version: 4.2.1
 Summary: Taskhawk Python Library
 Home-page: https://github.com/cloudchacho/taskhawk-python
 Author: Automatic Labs
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: python taskhawk
```

### Comparing `taskhawk-4.2.0/README.rst` & `taskhawk-4.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/setup.py` & `taskhawk-4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/__init__.py` & `taskhawk-4.2.1/taskhawk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ~~~~~~~~
 
 :copyright: (c) 2013-2017 by the Automatic Labs.
 """
 
 
 # semantic versioning (http://semver.org/)
-VERSION = '4.2.0'
+VERSION = '4.2.1'
 
 
 try:
     from .backends.aws import AWSMetadata  # noqa
 except ImportError:
     pass
 try:
```

### Comparing `taskhawk-4.2.0/taskhawk/backends/aws.py` & `taskhawk-4.2.1/taskhawk/backends/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         return self._publish_over_sns(self.topic_name, payload, headers or {})
 
 
 class AWSSQSConsumerBackend(TaskhawkConsumerBaseBackend):
     WAIT_TIME_SECONDS = 20
 
     def __init__(self, priority: Priority, dlq=False):
-
         self._sqs_resource: Optional[SQSServiceResource] = None
         self._sqs_client: Optional[SQSClient] = None
         self.queue_name = (
             f'TASKHAWK-{settings.TASKHAWK_QUEUE.upper()}{self.get_priority_suffix(priority)}{"-DLQ" if dlq else ""}'
         )
 
     @property
```

### Comparing `taskhawk-4.2.0/taskhawk/backends/base.py` & `taskhawk-4.2.1/taskhawk/backends/base.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/backends/gcp.py` & `taskhawk-4.2.1/taskhawk/backends/gcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import json
 import logging
 import typing
 from contextlib import contextmanager, ExitStack
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import cast, Generator, Optional
 from unittest import mock
 
 from google.api_core.exceptions import DeadlineExceeded, ServiceUnavailable
 from google.auth import environment_vars as google_env_vars, default as google_auth_default
 from google.cloud import pubsub_v1
 from google.cloud.pubsub_v1.futures import Future
@@ -145,14 +145,15 @@
 
 
 class GooglePubSubConsumerBackend(TaskhawkConsumerBaseBackend):
     def __init__(self, priority: Priority, dlq=False) -> None:
         self._error_count = 0
         self._publisher = None
         self._subscriber = None
+        self.last_log_time = datetime(1970, 1, 1)
         if not settings.TASKHAWK_SYNC:
             cloud_project = get_google_cloud_project()
             self._subscription_path: str = pubsub_v1.SubscriberClient.subscription_path(
                 cloud_project,
                 f'taskhawk-{settings.TASKHAWK_QUEUE.lower()}{get_priority_suffix(priority)}{"-dlq" if dlq else ""}',
             )
             self._dlq_topic_path: str = pubsub_v1.PublisherClient.topic_path(
@@ -185,14 +186,19 @@
         """
         return self._error_count
 
     def pull_messages(
         self, num_messages: int = 1, visibility_timeout: Optional[int] = None
     ) -> typing.List[ReceivedMessage]:
         try:
+            # Only log that we're pulling messages every 1 minute so we know the process is ready and not hung but not on every message pull to keep it from being spammy
+            time_since_last_log = datetime.now() - self.last_log_time
+            if time_since_last_log > timedelta(minutes=1):
+                logging.info("Pulling new messages")
+                self.last_log_time = datetime.now()
             messages = self.subscriber.pull(
                 subscription=self._subscription_path,
                 max_messages=num_messages,
                 retry=None,
                 timeout=settings.GOOGLE_PUBSUB_READ_TIMEOUT_S,
             ).received_messages
```

### Comparing `taskhawk-4.2.0/taskhawk/backends/import_utils.py` & `taskhawk-4.2.1/taskhawk/backends/import_utils.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/backends/utils.py` & `taskhawk-4.2.1/taskhawk/backends/utils.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/commands.py` & `taskhawk-4.2.1/taskhawk/commands.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/conf/__init__.py` & `taskhawk-4.2.1/taskhawk/conf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'AWS_ENDPOINT_SNS': None,
     'AWS_ENDPOINT_SQS': None,
     'AWS_READ_TIMEOUT_S': 2,
     'AWS_SECRET_KEY': None,
     'AWS_SESSION_TOKEN': None,
     'GOOGLE_APPLICATION_CREDENTIALS': None,
     'GOOGLE_CLOUD_PROJECT': None,
-    'GOOGLE_PUBSUB_READ_TIMEOUT_S': 5,
+    'GOOGLE_PUBSUB_READ_TIMEOUT_S': 20,
     'IS_LAMBDA_APP': False,
     'TASKHAWK_CONSUMER_BACKEND': None,
     'TASKHAWK_DEFAULT_HEADERS': 'taskhawk.conf.default_headers_hook',
     'TASKHAWK_PRE_PROCESS_HOOK': 'taskhawk.conf.noop_hook',
     'TASKHAWK_POST_PROCESS_HOOK': 'taskhawk.conf.noop_hook',
     'TASKHAWK_PUBLISHER_BACKEND': None,
     'TASKHAWK_PUBLISHER_GCP_BATCH_SETTINGS': (),
```

### Comparing `taskhawk-4.2.0/taskhawk/consumer.py` & `taskhawk-4.2.1/taskhawk/consumer.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/exceptions.py` & `taskhawk-4.2.1/taskhawk/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/models.py` & `taskhawk-4.2.1/taskhawk/models.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/publisher.py` & `taskhawk-4.2.1/taskhawk/publisher.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk/task_manager.py` & `taskhawk-4.2.1/taskhawk/task_manager.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/taskhawk.egg-info/PKG-INFO` & `taskhawk-4.2.1/taskhawk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskhawk
-Version: 4.2.0
+Version: 4.2.1
 Summary: Taskhawk Python Library
 Home-page: https://github.com/cloudchacho/taskhawk-python
 Author: Automatic Labs
 Maintainer: Aniruddha Maru
 Maintainer-email: aniruddhamaru@gmail.com
 License: Apache Software License (Apache License 2.0)
 Keywords: python taskhawk
```

### Comparing `taskhawk-4.2.0/taskhawk.egg-info/SOURCES.txt` & `taskhawk-4.2.1/taskhawk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/conftest.py` & `taskhawk-4.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/tasks.py` & `taskhawk-4.2.1/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/test_backends/test_aws.py` & `taskhawk-4.2.1/tests/test_backends/test_aws.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/test_backends/test_base.py` & `taskhawk-4.2.1/tests/test_backends/test_base.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/test_backends/test_gcp.py` & `taskhawk-4.2.1/tests/test_backends/test_gcp.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/test_consumer.py` & `taskhawk-4.2.1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/test_models.py` & `taskhawk-4.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/test_settings.py` & `taskhawk-4.2.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `taskhawk-4.2.0/tests/test_task_manager.py` & `taskhawk-4.2.1/tests/test_task_manager.py`

 * *Files identical despite different names*

