# Comparing `tmp/ofscraper-2.1.tar.gz` & `tmp/ofscraper-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-2.1.tar", max compression
+gzip compressed data, was "ofscraper-2.2.tar", max compression
```

## Comparing `ofscraper-2.1.tar` & `ofscraper-2.2.tar`

### file list

```diff
@@ -1,41 +1,44 @@
--rw-r--r--   0        0        0     1067 2023-05-27 02:37:19.645984 ofscraper-2.1/LICENSE
--rw-r--r--   0        0        0     5192 2023-05-27 02:37:19.645984 ofscraper-2.1/README.md
--rw-r--r--   0        0        0      607 2023-05-27 02:37:20.529999 ofscraper-2.1/ofscraper/__init__.py
--rw-r--r--   0        0        0      999 2023-05-27 02:37:20.529999 ofscraper-2.1/ofscraper/__version__.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/highlights.py
--rw-r--r--   0        0        0      979 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/init.py
--rw-r--r--   0        0        0     2264 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/me.py
--rw-r--r--   0        0        0     5599 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/messages.py
--rw-r--r--   0        0        0     1884 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/paid.py
--rw-r--r--   0        0        0     9037 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/posts.py
--rw-r--r--   0        0        0     2841 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1867 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     7882 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     5033 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/__init__.py
--rw-r--r--   0        0        0     6759 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3199 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4028 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/interaction/like.py
--rw-r--r--   0        0        0     5477 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    20976 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/prompts/prompts.py
--rwxr-xr-x   0        0        0    25673 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/scraper.py
--rw-r--r--   0        0        0        1 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     4373 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/args.py
--rw-r--r--   0        0        0     8996 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/auth.py
--rw-r--r--   0        0        0    10857 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/config.py
--rw-r--r--   0        0        0      257 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/console.py
--rw-r--r--   0        0        0      993 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    18388 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     2865 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     2381 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/filters.py
--rw-r--r--   0        0        0     5105 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/logger.py
--rw-r--r--   0        0        0     5220 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     3060 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      674 2023-05-27 02:37:20.533999 ofscraper-2.1/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     1509 2023-05-27 02:37:53.298575 ofscraper-2.1/pyproject.toml
--rw-r--r--   0        0        0     6554 1970-01-01 00:00:00.000000 ofscraper-2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-02 22:49:16.032687 ofscraper-2.2/LICENSE
+-rw-r--r--   0        0        0     5192 2023-06-02 22:49:16.032687 ofscraper-2.2/README.md
+-rw-r--r--   0        0        0      607 2023-06-02 22:49:16.036687 ofscraper-2.2/ofscraper/__init__.py
+-rw-r--r--   0        0        0      999 2023-06-02 22:49:16.036687 ofscraper-2.2/ofscraper/__version__.py
+-rw-r--r--   0        0        0        1 2023-06-02 22:49:16.036687 ofscraper-2.2/ofscraper/api/__init__.py
+-rw-r--r--   0        0        0     2015 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1067 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/init.py
+-rw-r--r--   0        0        0     2343 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/me.py
+-rw-r--r--   0        0        0     6524 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     2205 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     9663 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/posts.py
+-rw-r--r--   0        0        0     3256 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1936 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9094 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0    22926 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/commands/check.py
+-rwxr-xr-x   0        0        0    25489 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     5551 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0     8082 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3252 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4028 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0     5477 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    21642 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      609 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     7056 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/args.py
+-rw-r--r--   0        0        0     9035 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     5987 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    11158 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      257 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      993 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    18420 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     2865 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     2713 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0     5541 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0     5316 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     3060 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      674 2023-06-02 22:49:16.040687 ofscraper-2.2/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     1488 2023-06-02 22:49:50.532864 ofscraper-2.2/pyproject.toml
+-rw-r--r--   0        0        0     6596 1970-01-01 00:00:00.000000 ofscraper-2.2/PKG-INFO
```

### Comparing `ofscraper-2.1/LICENSE` & `ofscraper-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/README.md` & `ofscraper-2.2/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/__init__.py` & `ofscraper-2.2/ofscraper/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/__version__.py` & `ofscraper-2.2/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/api/highlights.py` & `ofscraper-2.2/ofscraper/api/highlights.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import ofscraper.constants as constants
 import ofscraper.utils.auth as auth
 log=logging.getLogger(__package__)
 
 
 
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def scrape_highlights(headers, user_id) -> list:
     with httpx.Client(http2=True, headers=headers) as c:
         url_stories = constants.highlightsWithStoriesEP.format(user_id)
         url_story = constants.highlightsWithAStoryEP.format(user_id)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url_stories, headers))
```

### Comparing `ofscraper-2.1/ofscraper/api/init.py` & `ofscraper-2.2/ofscraper/api/init.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,14 +5,15 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
 from . import me
+import traceback
 from rich.console import Console
 import ofscraper.utils.stdout as stdout
 import logging
 
 log=logging.getLogger(__package__)
 
 
@@ -27,8 +28,10 @@
 
 
 def getstatus(headers):
     try:
         resp = me.scrape_user(headers)
         return "UP"
     except Exception as e:
+        log.traceback(e)
+        log.traceback(traceback.format_exc())
         return "DOWN"
```

### Comparing `ofscraper-2.1/ofscraper/api/me.py` & `ofscraper-2.2/ofscraper/api/me.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import ofscraper.utils.auth as auth
 import ofscraper.utils.encoding as encoding
 import ofscraper.utils.stdout as stdout
 from ofscraper.utils.logger import updateSenstiveDict
 log=logging.getLogger(__package__)
 console=Console()
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=2, max=6),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/5")) 
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MAX, max=constants.OF_MAX),reraise=True,after=lambda retry_state:print(f"Attempting to login attempt:{retry_state.attempt_number}/{constants.NUM_TRIES}")) 
 def scrape_user(headers):
     with httpx.Client(http2=True, headers=headers) as c:
         url = constants.meEP
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
@@ -43,15 +43,15 @@
 
     return (name, username)
 
 
 def print_user(name, username):
     with stdout.lowstdout():
         console.print(f'Welcome, {name} | {username}')
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def parse_subscriber_count(headers):
     with httpx.Client(http2=True, headers=headers) as c:
         url = constants.subscribeCountEP
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
         r = c.get(url, timeout=None)
         if not r.is_error:
```

### Comparing `ofscraper-2.1/ofscraper/api/messages.py` & `ofscraper-2.2/ofscraper/api/messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,33 +43,34 @@
     sem = asyncio.Semaphore(8)
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue"),),TextColumn("Getting Messages...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
     with Live(progress_group, refresh_per_second=constants.refreshScreen,console=console.shared_console): 
-
         oldmessages=cache.get(f"messages_{model_id}",default=[]) 
         oldmsgset=set(map(lambda x:x.get("id"),oldmessages))
         log.debug(f"[bold]Messages Cache[/bold] {len(oldmessages)} found")
         oldmessages=list(filter(lambda x:x.get("createdAt")!=None,oldmessages))
         postedAtArray=list(map(lambda x:x["id"],sorted(oldmessages,key=lambda x:arrow.get(x["createdAt"]).float_timestamp,reverse=True)))
         global tasks
         tasks=[]
         
-        #split and interval can't match because of breakpoints
-        split=40
-        interval=30
-        if len(postedAtArray)>split:
-            splitArrays=[postedAtArray[i:i+split] for i in range(0, len(postedAtArray), interval)]
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress)))
-            tasks.extend(list(map(lambda x:asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=x[0])),splitArrays[1:-1])))
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=splitArrays[-1][0],recursive=True)))
+        #require a min num of posts to be returned
+        min_posts=50
+        if len(postedAtArray)>min_posts:
+            splitArrays=[postedAtArray[i:i+min_posts] for i in range(0, len(postedAtArray), min_posts)]
+            #use the previous split for message_id
+            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,required_ids=set(splitArrays[0]))))
+            [tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,required_ids=set(splitArrays[i]),message_id=splitArrays[i-1][-1])))
+            for i in range(1,len(splitArrays)-1)]
+            # keeping grabbing until nothign left
+            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,message_id=splitArrays[-2][-1])))
         else:
-            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress,recursive=True)))
+            tasks.append(asyncio.create_task(scrape_messages(headers,model_id,job_progress)))
     
     
         
         
         responseArray=[]
         page_count=0 
         page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
@@ -90,47 +91,59 @@
         if message["id"] in dupeSet:
             continue
         dupeSet.add(message["id"])
         oldmsgset.discard(message["id"])       
         unduped.append(message)
     if len(oldmsgset)==0:
         cache.set(f"messages_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"message_check_{model_id}",oldmessages,expire=constants.CHECK_EXPIRY)
+
         cache.close()
     else:
         cache.set(f"messages_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"message_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
         cache.close()
         log.debug("Some messages where not retrived resetting cache")
 
     return unduped    
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-async def scrape_messages(headers, user_id, progress,message_id=None,recursive=False) -> list:
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+async def scrape_messages(headers, model_id, progress,message_id=None,required_ids=None) -> list:
     global sem
+    global tasks
     attempt.set(attempt.get(0) + 1)
     ep = constants.messagesNextEP if message_id else constants.messagesEP
-    url = ep.format(user_id, message_id)
+    url = ep.format(model_id, message_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Message ID-> {message_id if message_id else 'initial'}")
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url, timeout=None)
             if not r.is_error:
                 progress.remove_task(task)
                 messages = r.json()['list']
                 if not messages:
                     return []
                 elif len(messages)==0:
-                    return messages
-                elif not recursive:
-                    return messages
-                global tasks
-                attempt.set(0)
-                tasks.append(asyncio.create_task(scrape_messages(headers, user_id,progress, recursive=True,message_id=messages[-1]['id'])))
+                    return []
+                elif required_ids==None:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'])))
+                else:
+                    [required_ids.discard(ele["id"]) for ele in messages]
+                    #try once more to grab, else quit
+                    if len(required_ids)==1:
+                        attempt.set(0)
+                        tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'],required_ids=set())))
+
+                    elif len(required_ids)>0:
+                        attempt.set(0)
+                        tasks.append(asyncio.create_task(scrape_messages(headers, model_id,progress,message_id=messages[-1]['id'],required_ids=required_ids)))
                 return messages
             log.debug(f"[bold]message request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]message response:[/bold] {r.content.decode()}")
             r.raise_for_status()
```

### Comparing `ofscraper-2.1/ofscraper/api/paid.py` & `ofscraper-2.2/ofscraper/api/paid.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 """
 from urllib.request import urlopen
 from rich.console import Console
 import httpx
 import logging
 import ofscraper.utils.auth as auth
 import ofscraper.constants as constants
+import ofscraper.api.profile as profile
+from diskcache import Cache
+from ..utils.paths import getcachepath
+cache = Cache(getcachepath())
+
 paid_content_list_name = 'list'
 log=logging.getLogger(__package__)
 console=Console()
 
 
 
 
@@ -50,14 +55,17 @@
             if not r.is_error:
                 log.info(f"Scraping paid content, Scraping isn't frozen. It takes time.\nScraped Page: {count}")
                 if "hasMore" in r.json():
                     hasMore = r.json()['hasMore']
                     count=count+1
                 media_to_download.extend(list(filter(lambda x:isinstance(x,list),r.json().values()))[0])
     log.debug(f"[bold]Paid Post count without Dupes[/bold] {len(media_to_download)} found")
+    model_id=profile.get_id(headers,username)
+    # set purchash check values during scan
+    cache.set(f"purchased_check_{model_id}",media_to_download,expire=constants.CHECK_EXPIRY)
     return media_to_download
```

### Comparing `ofscraper-2.1/ofscraper/api/posts.py` & `ofscraper-2.2/ofscraper/api/posts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import re
 import logging
 import httpx
+import arrow
 from ..constants import LICENCE_URL
 import ofscraper.utils.args as args_
 import ofscraper.utils.auth as auth
 from mpegdash.parser import MPEGDASHParser
 import ofscraper.utils.config as config
 
+
 log=logging.getLogger(__package__)
 
 class Post():
     def __init__(self, post, model_id, username, responsetype=None):
         self._post = post
         self._model_id = model_id
         self._username = username
         self._responsetype_ = responsetype or post.get("responseType")
 
     @property
-    def allmedia(self):
+    def post_media(self):
         if self._responsetype_ == "highlights":
             return [{"url": self.post["cover"], "type":"photo"}]
         return self._post.get("media") or []
 
     @property
     def post(self):
         return self._post
@@ -63,17 +65,17 @@
             if config.get_archived_responsetype(config.read_config()) == "":
                 return "achived"
             return config.get_archived_responsetype(config.read_config())
 
         else:
             response=config.read_config().get("responsetype", {}).get(self._responsetype_) 
             if  response == "":
-                return self._responsetype_
+                return self._responsetype_.capitalize()
             elif  response == None:
-                return self._responsetype_
+                return self._responsetype_.capitalize()
             elif  response != "":
                 return  response
 
     @property
     def id(self):
         return self._post["id"]
 
@@ -111,32 +113,53 @@
 
     @property
     def media(self):
         if (self.fromuser != self.model_id):
             return []
         else:
             media = map(lambda x: Media(
-                x[1], x[0], self), enumerate(self.allmedia))
+                x[1], x[0], self), enumerate(self.post_media))
             return list(filter(lambda x: x.canview == True, media))
-
-
+    @property
+    def all_media(self):
+        return list(map(lambda x: Media(
+            x[1], x[0], self), enumerate(self.post_media)))
+    @property
+    def expires(self):
+        return (self._post.get("expiredAt",{}) or self._post.get("expiresAt",None))!=None
 class Media():
     def __init__(self, media, count, post):
         self._media = media
         self._count = count
         self._post = post
 
     @property
+    def expires(self):
+        return self._post.expires
+
+    @property
     def mediatype(self):
         if self.responsetype_ == "highlights":
             return "images"
         if self._media["type"] == "gif" or self._media["type"] == "photo":
             return "images"
         else:
             return f"{self._media['type']}s"
+    @property
+    def length(self):
+        return self._media.get("duration")
+    @property
+    def length_(self):
+        if not self.length:
+            return "N/A"
+        return str((arrow.get(self.length)-arrow.get(0)))
+
+
+
+      
 
     @property
     def url(self):
         if self.responsetype_ == "stories":
             return self._media.get("files", {}).get("source", {}).get("url")
         elif self.responsetype_ == "highlights":
             return self._media.get("url")
@@ -151,16 +174,16 @@
 
     @property
     def id(self):
         return self._media["id"]
 
     # ID for use in dynamic names
     @property
-    def id_(self):
-        if self.count != None and len(self._post.allmedia) > 1:
+    def postid_(self):
+        if self.count != None and len(self._post.post_media) > 1:
             return f"{self._post._post['id']}_{self.count}"
         return self._post._post['id']
 
     @property
     def canview(self):
         if self.responsetype_ == "highlights":
             return True
@@ -318,10 +341,10 @@
         responsetype=self.post.post["responseType"]
         if responsetype in ["timeline","archived","pinned"]:
             responsetype="post"
         return LICENCE_URL.format(self.id,responsetype,self.postid)
 
     # for use in dynamic names
     def _addcount(self):
-        if len(self._post.allmedia) > 1 or self.responsetype_ in ["stories", "highlights"]:
+        if len(self._post.post_media) > 1 or self.responsetype_ in ["stories", "highlights"]:
             return True
         return False
```

### Comparing `ofscraper-2.1/ofscraper/api/profile.py` & `ofscraper-2.2/ofscraper/api/profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,33 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 import logging
+from typing import Union
 import httpx
 from rich.console import Console
 from tenacity import retry,stop_after_attempt,wait_random
-from ..constants import profileEP,NUM_TRIES
+from ..constants import profileEP,NUM_TRIES,DAILY_EXPIRY
 from ..utils import auth, encoding
 from xxhash import xxh32
+from diskcache import Cache
+from ..utils.paths import getcachepath
+import ofscraper.constants as constants
+cache = Cache(getcachepath())
+
 
 log=logging.getLogger(__package__)
 console=Console()
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-def scrape_profile(headers, username) -> dict:
+
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+def scrape_profile(headers, username:Union[int, str]) -> dict:
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(profileEP.format(username), timeout=None)
@@ -64,22 +71,28 @@
 def print_profile_info(info):
     header_fmt = 'Name: {} | Username: {} | ID: {} | Joined: {}\n'
     info_fmt = '- {} posts\n -- {} photos\n -- {} videos\n -- {} audios\n- {} archived posts'
     final_fmt = header_fmt + info_fmt
     log.info(final_fmt.format(*info))
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def get_id(headers, username):
+    id=cache.get(f"model_id_{username}",None)
+    if id:
+        return id
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = c.get(url, timeout=None)
         if not r.is_error:
-            return r.json()['id']
+            id=r.json()['id']
+            cache.set(f"model_id_{username}",id,DAILY_EXPIRY)
+            return id
+        
         r.raise_for_status()
```

### Comparing `ofscraper-2.1/ofscraper/api/subscriptions.py` & `ofscraper-2.2/ofscraper/api/subscriptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 import logging
 import httpx
 from rich.console import Console
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import subscriptionsEP,NUM_TRIES
 from ..utils import auth, dates
+import ofscraper.constants as constants
 log=logging.getLogger(__package__)
 
 
 async def get_subscriptions(headers, subscribe_count):
     offsets = range(0, subscribe_count, 10)
     tasks = [scrape_subscriptions(headers, offset) for offset in offsets]
     subscriptions = await asyncio.gather(*tasks)
     return list(chain.from_iterable(subscriptions))
 
 
-@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 async def scrape_subscriptions(headers, offset=500) -> list:
     async with httpx.AsyncClient(http2=True, headers=headers) as c:
         url = subscriptionsEP.format(offset)
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
         r = await c.get(subscriptionsEP.format(offset), timeout=None)
```

### Comparing `ofscraper-2.1/ofscraper/api/timeline.py` & `ofscraper-2.2/ofscraper/api/timeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from ..utils.paths import getcachepath
 import ofscraper.utils.console as console
 
 from diskcache import Cache
 cache = Cache(getcachepath())
 log=logging.getLogger(__package__)
 attempt = contextvars.ContextVar("attempt")
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def scrape_pinned_posts(headers, model_id,timestamp=0) -> list:
     with httpx.Client(http2=True, headers=headers) as c:
         ep = constants.timelinePinnedNextEP if timestamp else constants.timelinePinnedEP
         url = ep.format(model_id, timestamp)
         # url = timelinePinnedEP.format(model_id)
 
         auth.add_cookies(c)
@@ -46,51 +46,58 @@
         r = c.get(url, timeout=None)
         if not r.is_error:
             return r.json()['list']
         r.raise_for_status()
         log.debug(f"[bold]pinned request status code:[/bold]{r.status_code}")
         log.debug(f"[bold]pinned response:[/bold] {r.content.decode()}")
 
-def get_pinned_post(headers,model_id,username):
+def get_pinned_post(headers,model_id):
     return scrape_pinned_posts(headers,model_id)
    
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
-async def scrape_timeline_posts(headers, model_id,progress, timestamp=None,recursive=False) -> list:
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
+async def scrape_timeline_posts(headers, model_id,progress, timestamp=None,required_ids=None) -> list:
     global sem 
+    global tasks
     attempt.set(attempt.get(0) + 1)
     if timestamp:
         log.debug(arrow.get(math.trunc(float(timestamp))))
         timestamp=str(timestamp)
         ep = constants.timelineNextEP
         url = ep.format(model_id, timestamp)
     else:
         ep=constants.timelineEP
         url=ep.format(model_id)
     log.debug(url)
     async with sem:
         task=progress.add_task(f"Attempt {attempt.get()}/{constants.NUM_TRIES}: Timestamp -> {arrow.get(math.trunc(float(timestamp))) if timestamp!=None  else 'initial'}",visible=True)
-
         async with httpx.AsyncClient(http2=True, headers=headers) as c:
             auth.add_cookies(c)
             c.headers.update(auth.create_sign(url, headers))
             r = await c.get(url , timeout=None)
             if not r.is_error:
                 progress.remove_task(task)
                 posts = r.json()['list']
-    
                 if not posts:
                     return []
                 elif len(posts)==0:
-                    return posts
-                elif not recursive:
-                    return posts
-                # recursive search for posts
-                attempt.set(0)
-                global tasks
-                tasks.append(asyncio.create_task( scrape_timeline_posts(headers, model_id,progress,posts[-1]['postedAtPrecise'],recursive=True)))
+                    return []
+                elif required_ids==None:
+                    attempt.set(0)
+                    tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'])))
+                else:
+                    [required_ids.discard(float(ele["postedAtPrecise"])) for ele in posts]
+
+                    #try once more to get id if only 1 left
+                    if len(required_ids)==1:
+                        attempt.set(0)
+                        tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=set())))
+
+                    elif len(required_ids)>0:
+                        attempt.set(0)
+                        tasks.append(asyncio.create_task(scrape_timeline_posts(headers, model_id,progress,timestamp=posts[-1]['postedAtPrecise'],required_ids=required_ids)))
                 return posts
             log.debug(f"[bold]timeline request status code:[/bold]{r.status_code}")
             log.debug(f"[bold]timeline response:[/bold] {r.content.decode()}")
             r.raise_for_status()
 
 async def get_timeline_post(headers,model_id):
     global sem
@@ -98,37 +105,35 @@
     overall_progress=Progress(SpinnerColumn(style=Style(color="blue")),TextColumn("Getting timeline media...\n{task.description}"))
     job_progress=Progress("{task.description}")
     progress_group = Group(
     overall_progress,
     Panel(Group(job_progress)))
     with Live(progress_group, refresh_per_second=5,console=console.shared_console): 
 
-        oldtimeline=cache.get(f"timeline_{model_id}",default=[]) 
+        oldtimeline=cache.get(f"timeline_{model_id}",default=[])
         oldtimeset=set(map(lambda x:x.get("id"),oldtimeline))
         log.debug(f"[bold]Timeline Cache[/bold] {len(oldtimeline)} found")
         oldtimeline=list(filter(lambda x:x.get("postedAtPrecise")!=None,oldtimeline))
         postedAtArray=sorted(list(map(lambda x:float(x["postedAtPrecise"]),oldtimeline)))
         global tasks
         tasks=[]
-        #max result is 50, try to get 40 in each async task for leeway
-        # Also need to grab new posts
-        #add differing splits and interval for inclusivity and potential breakpoints
-        split=40
-        interval=30
-        if len(postedAtArray)>split:
-            split=40
-            interval=30
-            splitArrays=[postedAtArray[i:i+split] for i in range(0, len(postedAtArray), interval)]
-            
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress)))
-            tasks.extend(list(map(lambda x:asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=x[0]-100)),splitArrays[1:-1])))
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=splitArrays[-1][0],recursive=True)))
+        min_posts=50
+        if len(postedAtArray)>min_posts:
+            splitArrays=[postedAtArray[i:i+min_posts] for i in range(0, len(postedAtArray), min_posts)]
+            #use the previous split for timesamp
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[0]))))
+            [tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,required_ids=set(splitArrays[i]),timestamp=splitArrays[i-1][-1])))
+            for i in range(1,len(splitArrays)-1)]
+            # keeping grabbing until nothign left
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,timestamp=splitArrays[-2][-1])))
         else:
-            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress,recursive=True)))
-
+            tasks.append(asyncio.create_task(scrape_timeline_posts(headers,model_id,job_progress)))
+    
+    
+       
         responseArray=[]
     
     
         page_count=0 
         page_task = overall_progress.add_task(f' Pages Progress: {page_count}',visible=True)
         while len(tasks)!=0:
             for coro in asyncio.as_completed(tasks):
@@ -147,27 +152,31 @@
             continue
         dupeSet.add(post["id"])
         oldtimeset.discard(post["id"])
         unduped.append(post)
     log.debug(f"[bold]Timeline Count without Dupes[/bold] {len(unduped)} found")
     if len(oldtimeset)==0:
         cache.set(f"timeline_{model_id}",unduped,expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"timeline_check_{model_id}",unduped,expire=constants.CHECK_EXPIRY)
+
         cache.close()
     else:
         cache.set(f"timeline_{model_id}",[],expire=constants.RESPONSE_EXPIRY)
+        cache.set(f"timeline_check_{model_id}",[],expire=constants.CHECK_EXPIRY)
+
         cache.close()
         log.debug("Some post where not retrived resetting cache")
 
     return unduped                                
 
 def get_archive_post(headers,model_id):
     return scrape_archived_posts(headers,model_id)
    
 
-@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=5, max=20),reraise=True)   
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True)   
 def scrape_archived_posts(headers, model_id, timestamp=0) -> list:
     ep = constants.archivedNextEP if timestamp else constants.archivedEP
     url = ep.format(model_id, timestamp)
     with httpx.Client(http2=True, headers=headers) as c:
         auth.add_cookies(c)
         c.headers.update(auth.create_sign(url, headers))
 
@@ -179,11 +188,19 @@
             posts += scrape_archived_posts(
                 headers, model_id, posts[-1]['postedAtPrecise'])
             return posts
         r.raise_for_status()
         log.debug(f"[bold]archived request status code:[/bold]{r.status_code}")
         log.debug(f"[bold]archived response:[/bold] {r.content.decode()}")
 
-
-
-               
+def get_individual_post(id,client=None):
+    headers = auth.make_headers(auth.read_auth())
+    with client or httpx.Client(http2=True, headers=headers) as c:
+        url=f"https://onlyfans.com/api2/v2/posts/{id}?skip_users=all"
+        auth.add_cookies(c)
+        c.headers.update(auth.create_sign(url, headers))
+        r=c.get(url)
+        if not r.is_error:
+            return r.json()
+        log.debug(f"{r.status_code}")
+        log.debug(f"{r.content.decode()}")
```

### Comparing `ofscraper-2.1/ofscraper/constants.py` & `ofscraper-2.2/ofscraper/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 messagesEP = 'https://onlyfans.com/api2/v2/chats/{}/messages?limit=100&offset=0&order=desc&skip_users=all&skip_users_dups=1'
 messagesNextEP = 'https://onlyfans.com/api2/v2/chats/{}/messages?limit=100&offset=0&id={}&order=desc&skip_users=all&skip_users_dups=1'
 
 favoriteEP = 'https://onlyfans.com/api2/v2/posts/{}/favorites/{}'
 postURL = 'https://onlyfans.com/{}/{}'
 
-DC_EP = 'https://raw.githubusercontent.com/DATAHOARDERS/dynamic-rules/main/onlyfans.json'
+DYNAMIC = 'https://raw.githubusercontent.com/deviint/onlyfans-dynamic-rules/main/dynamicRules.json'
 
 donateEP = "https://www.buymeacoffee.com/excludedBittern"
 
 purchased_contentEP = "https://onlyfans.com/api2/v2/posts/paid?limit=100&skip_users=all&format=infinite&offset={}&user_id={}"
 
 mainPromptChoices = {
     'Download content from a user': 0,
@@ -92,22 +92,35 @@
 PROFILE_DEFAULT="main_profile"
 PREMIUM_DEFAULT="Premium"
 MP4DECRYPT_DEFAULT=""
 FFMPEG_DEFAULT =""
 DISCORD_DEFAULT =""
 SUPPRESS_LOG_LEVEL=21
 RESPONSE_TYPE_DEFAULT= {
-            "message":"messages",
-            "timeline":"posts",
-            "archived":"archived",
-            "paid":"messages",
-            "stories":"stories",
-            "highlights":"stories",
-            "profile":"profile",
-            "pinned":"posts"
+            "message":"Messages",
+            "timeline":"Posts",
+            "archived":"Archived",
+            "paid":"Messages",
+            "stories":"Stories",
+            "highlights":"Stories",
+            "profile":"Profile",
+            "pinned":"Posts"
         }
-NUM_TRIES=5
+NUM_TRIES=10
 RESPONSE_EXPIRY=5000000
+CHECK_EXPIRY=86400
+DAILY_EXPIRY=86400
+DISCORDWAIT=5
+OF_MIN=15
+OF_MAX=50
 LICENCE_URL="https://onlyfans.com/api2/v2/users/media/{}/drm/{}/{}?type=widevine"
 logname="ofscraper"
 PATH_STR_MAX=200
-refreshScreen=20
+TABLE_STR_MAX=100
+
+refreshScreen=20
+
+MP4DECRYPT_LINUX="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-unknown-linux.zip"
+MP4DECRYPT_WINDOWS="https://www.bok.net/Bento4/binaries/Bento4-SDK-1-6-0-640.x86_64-microsoft-win32.zip"
+FFMPEG_LINUX="https://johnvansickle.com/ffmpeg/releases/ffmpeg-release-amd64-static.tar.xz"
+FFMPEG_WINDOWS="https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-gpl.zip"
+
```

### Comparing `ofscraper-2.1/ofscraper/db/queries.py` & `ofscraper-2.2/ofscraper/db/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,21 @@
 """
 
 allIDCheck=\
 """
 SELECT media_id FROM medias
 """
 
+
+allPOSTCheck=\
+"""
+SELECT post_id FROM medias
+"""
+
+
 mediaInsert=\
 f"""INSERT INTO 'medias'(
 media_id,post_id,link,directory,filename,size,api_type,media_type,preview,linked,downloaded,created_at)
             VALUES (?, ?,?,?,?,?,?,?,?,?,?,?);"""
 
 mediaDupeCheck=\
 """
```

### Comparing `ofscraper-2.1/ofscraper/interaction/like.py` & `ofscraper-2.2/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/prompts/prompt_functions.py` & `ofscraper-2.2/ofscraper/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/prompts/prompts.py` & `ofscraper-2.2/ofscraper/prompts/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -556,14 +556,41 @@
 """,
 "default":config.get_ffmpeg(config_)
         },
     ]
 
     answer = prompt(questions)
     return answer["ffmpeg"] 
+def auto_download_mp4_decrypt()-> bool:
+    name = 'manual download'
+    questions = [
+        {
+            'type': 'list',
+            'name': name,
+            'message': "mp4decrypt not found would you like to auto install?",
+            'choices':["Yes","No"]
+        }
+    ]
+
+    answer = prompt(questions)
+    return answer[name]
+
+def auto_download_ffmpeg()-> bool:
+    name = 'manual download'
+    questions = [
+        {
+            'type': 'list',
+            'name': name,
+            'message': "ffmpeg not found would you like to auto install?",
+            'choices':["Yes","No"]
+        }
+    ]
+
+    answer = prompt(questions)
+    return answer[name]
 
 def continue_prompt() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
             'name': name,
```

### Comparing `ofscraper-2.1/ofscraper/scraper.py` & `ofscraper-2.2/ofscraper/commands/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,38 +55,38 @@
 import ofscraper.interaction.like as like
 import ofscraper.utils.logger as logger
 import ofscraper.utils.args as args_
 import ofscraper.utils.filters as filters
 import ofscraper.utils.stdout as stdout
 import ofscraper.utils.console as console
 
-log=logger.init_logger(logging.getLogger(__package__))
+log=logging.getLogger(__package__)
 args=args_.getargs()
 log.debug(args)
 def process_messages(headers, model_id,username):
     with stdout.lowstdout():
         with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
 
             messages_ =asyncio.run(messages.get_messages(headers,  model_id)) 
             messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
-            log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),messages_))}")
+            log.debug(f"[bold]Messages Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}")
             log.debug("Removing locked messages media")
             for message in messages_:
                 operations.write_messages_table(message)
             output=[]
             [ output.extend(message.media) for message in messages_]
             return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_paid_post(model_id,username):
     with stdout.lowstdout():
         with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
             task1=progress.add_task("Getting Paid Media....")
             paid_content=paid.scrape_paid(username)
             paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
-            log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),paid_content))}")
+            log.debug(f"[bold]Paid Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),paid_content))}")
             log.debug("Removing locked paid media")
             for post in paid_content:
                 operations.write_post_table(post,model_id,username)
             output=[]
             [output.extend(post.media) for post in paid_content]
             progress.remove_task(task1)
             return list(filter(lambda x:isinstance(x,posts_.Media),output))
@@ -96,15 +96,15 @@
 def process_highlights(headers, model_id,username):
     with stdout.lowstdout():
         with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
             task1=progress.add_task("Highlights and Stories....")
             highlights_, stories = highlights.scrape_highlights(headers, model_id)
             highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
             list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
-            log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.allmedia), highlights_))+sum(map(lambda x:len(x.allmedia), stories))}")
+            log.debug(f"[bold]Combined Story and Highlight Media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))+sum(map(lambda x:len(x.post_media), stories))}")
             for post in highlights_:
                 operations.write_stories_table(post,model_id,username)
             for post in stories:
                 operations.write_stories_table(post,model_id,username)   
             output=[]
             output2=[]
             [ output.extend(highlight.media) for highlight in highlights_]
@@ -120,29 +120,29 @@
 
 
 def process_timeline_posts(headers, model_id,username):
     with stdout.lowstdout():
         with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
             timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id))
             timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
-            log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),timeline_posts))}")
+            log.debug(f"[bold]Timeline Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_posts))}")
             log.debug("Removing locked timeline media")
             for post in timeline_posts:
                 operations.write_post_table(post,model_id,username)
             output=[]
             [output.extend(post.media) for post in  timeline_posts ]
             return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_archived_posts(headers, model_id,username):
     with stdout.lowstdout():
         with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
             task1=progress.add_task("Getting Archived Media....")
             archived_posts = timeline.get_archive_post(headers, model_id)
             archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
-            log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),archived_posts))}")
+            log.debug(f"[bold]Archived Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),archived_posts))}")
             log.debug("Removing locked archived media")
 
             for post in archived_posts:
                 operations.write_post_table(post,model_id,username)
             output=[]
             [ output.extend(post.media) for post in archived_posts ]
             progress.remove_task(task1)
@@ -151,17 +151,17 @@
 
 
 
 def process_pinned_posts(headers, model_id,username):
     with stdout.lowstdout():
         with Progress(  SpinnerColumn(style=Style(color="blue")),TextColumn("{task.description}")) as progress:
             task1=progress.add_task("Getting Pinned Media....")
-            pinned_posts = timeline.get_pinned_post(headers, model_id,username)
+            pinned_posts = timeline.get_pinned_post(headers, model_id)
             pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
-            log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.allmedia),pinned_posts))}")
+            log.debug(f"[bold]Pinned Media Count with locked[/bold] {sum(map(lambda x:len(x.post_media),pinned_posts))}")
             log.debug("Removing locked pinned media")
             for post in  pinned_posts:
                 operations.write_post_table(post,model_id,username)
             output=[]
             [ output.extend(post.media) for post in pinned_posts ]
             progress.remove_task(task1)
             return list(filter(lambda x:isinstance(x,posts_.Media),output))
@@ -360,15 +360,15 @@
                 eleDict[key]["name"]=ele['name']
                 log.debug(f"getting content for {count+1}/{length} model")
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id(headers, ele["name"])
                     eleDict[key]["id"]=model_id
-                    create_tables(model_id,ele['name'])
+                    operations.create_tables(model_id,ele['name'])
                     operations.write_profile_table(model_id,ele['name'])
                     eleDict[key]["combined"]=process_areas(headers, ele, model_id)
                 
                 except Exception as e:
                     log.traceback(f"failed with exception: {e}")
                     log.traceback(traceback.format_exc())      
             for key in eleDict.keys():
@@ -386,15 +386,15 @@
             for count,ele in enumerate(userdata):
                 log.debug(f"Getting content+downloading {count+1}/{length} model")
 
                 if args.posts:
                     log.info(f"Getting {','.join(args.posts)} for [bold]{ele['name']}[/bold]\n[bold]Subscription Active:[/bold] {ele['active']}")
                 try:
                     model_id = profile.get_id(headers, ele["name"])
-                    create_tables(model_id,ele['name'])
+                    operations.create_tables(model_id,ele['name'])
                     operations.write_profile_table(model_id,ele['name'])
                     combined_urls=process_areas(headers, ele, model_id)
                     asyncio.run(download.process_dicts(
                     ele["name"],
                     model_id,
                     combined_urls,
                     forced=args.dupe,
@@ -502,36 +502,40 @@
     scraper_bool=len(args.posts)>0 or args.action
     #always return with correct args
     if selectedusers and scraper_bool:
             return selectedusers
     if scraper_bool:
         selectedusers=selectuserhelper()
     #create in these situations
+    #set at least once
+    elif args.username and not selectedusers:
+        selectedusers=selectuserhelper()
     elif not selectedusers and not scraper_bool:
         setfilter()
         selectedusers=selectuserhelper()
     elif selectedusers and not scraper_bool:
-        if prompts.reset_username_prompt()=="Yes":
+        if prompts.reset_username_prompt()=="Yes":  
             setfilter()
             selectedusers=selectuserhelper()
     return selectedusers
 
 def selectuserhelper():
     headers = auth.make_headers(auth.read_auth())
     subscribe_count = process_me(headers)
     parsed_subscriptions = get_models(headers, subscribe_count)
-    filter_subscriptions=filteruserHelper(parsed_subscriptions )
     if args.username and "ALL" in args.username:
+        filter_subscriptions=filteruserHelper(parsed_subscriptions )
         selectedusers=filter_subscriptions
         
     elif args.username:
         userSelect=set(args.username)
-        selectedusers=list(filter(lambda x:x["name"] in userSelect,filter_subscriptions))
+        selectedusers=list(filter(lambda x:x["name"] in userSelect,parsed_subscriptions))
     #manually select usernames
     else:
+        filter_subscriptions=filteruserHelper(parsed_subscriptions )
         selectedusers= get_model(filter_subscriptions)
     return selectedusers
 
         
 
         
 
@@ -557,22 +561,15 @@
     if args.sub_status=="active":
         filterusername=list(filter(lambda x:x["data"]["subscribedIsExpiredNow"]==False,filterusername))     
     if args.sub_status=="expired":
         filterusername=list(filter(lambda x:x["data"]["subscribedIsExpiredNow"]==True,filterusername))      
     return filterusername
 
 
-def create_tables(model_id,username):
-    operations.create_post_table(model_id,username)
-    operations.create_message_table(model_id,username)
-    operations.create_media_table(model_id,username)
-    operations.create_products_table(model_id,username)
-    operations.create_others_table(model_id,username)
-    operations.create_profile_table(model_id,username)
-    operations.create_stories_table(model_id,username)
+
 
 
 
 @contextmanager
 def scrape_context_manager():
         
         # Before yield as the enter method
@@ -600,14 +597,15 @@
         console.shared_console.print(
             f"[bold green]Welcome to OF-Scraper Version {args.version}[/bold green]"
         )                
 def main():
  
         try:
             print_start()
+            logger.start_discord_queue()
             scrapper()
             paths.cleanup()
             logger.discord_cleanup()
         except KeyboardInterrupt as E:
             try:
                 with exit.DelayedKeyboardInterrupt():
                     paths.cleanup()
```

### Comparing `ofscraper-2.1/ofscraper/utils/auth.py` & `ofscraper-2.2/ofscraper/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 import httpx
 import browser_cookie3
 from .profiles import get_current_profile
 from ..prompts.prompts import *
-from ..constants import configPath, authFile, DC_EP, requestAuth
+from ..constants import configPath, authFile, DYNAMIC, requestAuth
 
 console=Console()
 
 
 
 def read_auth():
     make_request_auth()
@@ -211,14 +211,15 @@
 
     checksum_indexes = content['checksum_indexes']
     checksum_constant = content['checksum_constant']
     checksum = sum(sha_1_b[i] for i in checksum_indexes) + checksum_constant
 
     final_sign = content['format'].format(sha_1_sign, abs(checksum))
 
+
     headers.update(
         {
             'sign': final_sign,
             'time': time2
         }
     )
     return headers
@@ -255,17 +256,17 @@
 
         with open(p / requestAuth, 'w') as f:
             f.write(json.dumps(request_auth, indent=4))
 
 
 def get_request_auth():
     with httpx.Client(http2=True) as c:
-        r = c.get(DC_EP)
+        r = c.get(DYNAMIC)
     if not r.is_error:
         content = r.json()
         static_param = content['static_param']
-        fmt = content['format']
+        fmt = f"{content['start']}:{{}}:{{:x}}:{content['end']}" 
         checksum_indexes = content['checksum_indexes']
         checksum_constant = content['checksum_constant']
         return (static_param, fmt, checksum_indexes, checksum_constant)
     else:
         return []
```

### Comparing `ofscraper-2.1/ofscraper/utils/config.py` & `ofscraper-2.2/ofscraper/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import json
 import pathlib
 import logging
 from rich.console import Console
 import ofscraper.constants as constants
 import ofscraper.prompts.prompts as prompts 
+import ofscraper.utils.binaries as binaries
 
 console=Console()
 log=logging.getLogger(__package__)
 
 def read_config():
     p = pathlib.Path.home() / constants.configPath
     if not p.is_dir():
@@ -172,22 +173,28 @@
                         config = json.loads(configText)
                     break
                 except:
                     continue
 
 def update_mp4decrypt():
     config={"config":read_config()}
-    config["config"]["mp4decrypt"]=prompts.mp4_prompt(config)
+    if prompts.auto_download_mp4_decrypt()=="Yes":
+        config["config"]["mp4decrypt"]=binaries.mp4decrypt_download()
+    else:
+        config["config"]["mp4decrypt"]=prompts.mp4_prompt(config)
     p = pathlib.Path.home() / constants.configPath / constants.configFile
     with open(p, 'w') as f:
         f.write(json.dumps(config, indent=4))
 
 def update_ffmpeg():
     config={"config":read_config()}
-    config["config"]["ffmpeg"]=prompts.ffmpeg_prompt(config)
+    if prompts.auto_download_ffmpeg()=="Yes":
+        config["config"]["ffmpeg"]=binaries.ffmpeg_download()
+    else:
+        config["config"]["ffmpeg"]=prompts.ffmpeg_prompt(config)
     p = pathlib.Path.home() / constants.configPath / constants.configFile
     with open(p, 'w') as f:
         f.write(json.dumps(config, indent=4))
 
     
 def get_save_location(config=None):
     if config==None:
```

### Comparing `ofscraper-2.1/ofscraper/utils/dates.py` & `ofscraper-2.2/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/download.py` & `ofscraper-2.2/ofscraper/utils/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                         overall_progress.update(task1,description=desc.format(
                                     p_count=photo_count, v_count=video_count, a_count=audio_count,skipped=skipped, data=data,mediacount=len(medialist), sumcount=video_count+audio_count+photo_count+skipped), refresh=True, advance=1)
         overall_progress.remove_task(task1)
     log.error(f'[bold]{username}[/bold] ({photo_count} photos, {video_count} videos, {audio_count} audios,  {skipped} skipped)' )
 def retry_required(value):
     return value == ('skipped', 1)
 
-@retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=20, max=40),reraise=True) 
+@retry(retry=retry_if_result(retry_required),stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_random(min=constants.OF_MIN, max=constants.OF_MAX),reraise=True) 
 async def download(ele,path,model_id,username,file_size_limit,progress):
     attempt.set(attempt.get(0) + 1)
     
     try:
         if ele.url:
            return await main_download_helper(ele,path,file_size_limit,username,model_id,progress)
         elif ele.mpd:  
@@ -341,13 +341,13 @@
     try:
         return error_content.get('message', 'No error message available')
     except AttributeError:
         return error_content
 def createfilename(ele,username,model_id,ext):
     if ele.responsetype =="profile":
         return "{filename}.{ext}".format(ext=ext,filename=ele.filename)
-    return (config_.get_fileformat(config_.read_config())).format(filename=ele.filename,sitename="Onlyfans",site_name="Onlyfans",post_id=ele.id_,media_id=ele.id,first_letter=username[0],mediatype=ele.mediatype,value=ele.value,text=ele.text_,date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config())),ext=ext,model_username=username,model_id=model_id,responsetype=ele.responsetype) 
+    return (config_.get_fileformat(config_.read_config())).format(filename=ele.filename,sitename="Onlyfans",site_name="Onlyfans",post_id=ele.postid_,media_id=ele.id,first_letter=username[0],mediatype=ele.mediatype,value=ele.value,text=ele.text_,date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config())),ext=ext,model_username=username,model_id=model_id,responsetype=ele.responsetype)
```

### Comparing `ofscraper-2.1/ofscraper/utils/encoding.py` & `ofscraper-2.2/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/exit.py` & `ofscraper-2.2/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/filters.py` & `ofscraper-2.2/ofscraper/utils/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,23 @@
 args=args_.getargs()
 log=logging.getLogger(__package__)
 def filterMedia(media):
     media=dupefilter(media)
     media=post_datesorter(media)
     media=posts_type_filter(media)
     media=posts_date_filter(media)
+    media=post_promo_filter(media)
+    # if args.manual_download():
+    #     args.dupe=True
+    #     args_.changeargs(args)
+    #     media=post_manual_filter(media)
     return media
 
+def post_manual_filter():
+    None
 
 def dupefilter(media):
     output=[]
     ids=set()
     log.info("Removing duplicate media")
     log.debug(f"[bold]Combined Media Count with dupes[/bold]  {len(media)}")
     for item in media:
@@ -61,7 +68,12 @@
 
 def posts_date_filter(media):
     if args.before:
         media=filter(lambda x:x.postdate==None or arrow.get(x.postdate)<=args.before,media)
     if args.after:
         media=filter(lambda x:x.postdate==None or arrow.get(x.postdate)>=args.after,media)
     return list(media)
+
+def post_promo_filter(media):
+    if args.skip_promo:
+        return list(filter(lambda x:not x.expires,media))
+    return media
```

### Comparing `ofscraper-2.1/ofscraper/utils/logger.py` & `ofscraper-2.2/ofscraper/utils/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import re
 import httpx
 import logging
 import threading
 import time
 import queue
 from rich.logging import RichHandler
+from tenacity import retry,stop_after_attempt,wait_fixed
+
 import ofscraper.utils.paths as paths
 import ofscraper.utils.config as config_
 import ofscraper.utils.args as args
 import ofscraper.utils.console as console
-
+import ofscraper.constants as constants
 senstiveDict={}
 discord_queue=queue.Queue()
 
 
 class DebugOnly(logging.Filter):
     def filter(self, record):
         if record.levelname=="DEBUG" or record.levelname=="TRACEBACK":
@@ -37,31 +39,40 @@
         #convert markup
         log_entry=re.sub("\[bold\]|\[/bold\]","**",log_entry)
         discord_queue.put((url,log_entry))
 
 def discord_messenger():
     with httpx.Client() as c:
         while True:
-            url,entry=discord_queue.get()   
+            url,message=discord_queue.get()   
             if url=="exit":
-                return 
-            c.post(url, headers={"Content-type": "application/json"},json={"content":entry})
+                return
+            try:
+                discord_pusher(url,message,c)
+            except httpx.HTTPError as E:
+                console.shared_console.print("Discord Error")
+
+@retry(stop=stop_after_attempt(constants.NUM_TRIES),wait=wait_fixed(constants.DISCORDWAIT),reraise=True) 
+def discord_pusher(url,message,c):
+    c.post(url, headers={"Content-type": "application/json"},json={"content":message})
+
+
+
 def discord_cleanup():
     logging.getLogger("ofscraper").info("Pushing Discord Queue")
     with httpx.Client() as c:
         while True:
             if discord_queue.empty:
                 discord_queue.put(("exit",None))
                 break
             time.sleep(.5)
              
-
-
-worker_thread = threading.Thread(target=discord_messenger)
-worker_thread.start()
+def start_discord_queue():
+    worker_thread = threading.Thread(target=discord_messenger)
+    worker_thread.start()
 class SensitiveFormatter(logging.Formatter):
     """Formatter that removes sensitive information in logs."""
     @staticmethod
     def _filter(s):
         s=re.sub("&Policy=[^&\"]+", "&Policy={hidden}", s)
         s=re.sub("&Signature=[^&\"]+", "&Signature={hidden}", s)
         s=re.sub("&Key-Pair-Id=[^&\"]+", "&Key-Pair-Id={hidden}", s)
```

### Comparing `ofscraper-2.1/ofscraper/utils/paths.py` & `ofscraper-2.2/ofscraper/utils/paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import subprocess
 import logging
 from rich.console import Console
 import arrow
 import ofscraper.constants as constants
 import ofscraper.utils.profiles as profiles
 import ofscraper.utils.config as config_
+import ofscraper.utils.args as args_
 
 console=Console()
 homeDir=pathlib.Path.home()
 log=logging.getLogger(__package__)
 
 
 @contextmanager
@@ -46,15 +47,15 @@
 def databasePathHelper(model_id,username):
     formatStr=config_.get_metadata(config_.read_config())
     return pathlib.Path(formatStr.format(configpath=homeDir / constants.configPath,profile=profiles.get_current_profile(),model_username=username,username=username,model_id=model_id,sitename="Onlyfans",site_name="Onlyfans",first_letter=username[0],save_location=config_.get_save_location(config_.read_config())),"user_data.db")
 
 def getmediadir(ele,username,model_id):
     root= pathlib.Path((config_.get_save_location(config_.read_config())))
     downloadDir=config_.get_dirformat(config_.read_config())\
-    .format(sitename="onlyfans",first_letter=username[0].capitalize(),model_id=model_id,model_username=username,responsetype=ele.responsetype.capitalize(),mediatype=ele.mediatype.capitalize(),value=ele.value.capitalize(),date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config())))
+    .format(post_id=ele.postid,sitename="onlyfans",first_letter=username[0].capitalize(),model_id=model_id,model_username=username,responsetype=ele.responsetype,mediatype=ele.mediatype.capitalize(),value=ele.value.capitalize(),date=arrow.get(ele.postdate).format(config_.get_date(config_.read_config())))
     return root /downloadDir   
 
 
 def messageResponsePathHelper(model_id,username):
     profile = profiles.get_current_profile()
     return homeDir / constants.configPath / profile / ".data"/f"{username}_{model_id}"/"messages.json"
 
@@ -80,14 +81,16 @@
 
 def getcachepath():
     profile = profiles.get_current_profile()
     path=pathlib.Path.home() / constants.configPath / profile/"cache"
     createDir(path.parent)
     return path
 def trunicate(path):
+    if args_.getargs().original:
+        return path
     if platform.system() == 'Windows' and len(str(path))>256:
         return _windows_trunicateHelper(path)
     elif platform.system() == 'Linux':
         return _linux_trunicateHelper(path)
     else:
         return pathlib.Path(path)
 def _windows_trunicateHelper(path):
```

### Comparing `ofscraper-2.1/ofscraper/utils/profiles.py` & `ofscraper-2.2/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/separate.py` & `ofscraper-2.2/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/ofscraper/utils/stdout.py` & `ofscraper-2.2/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-2.1/pyproject.toml` & `ofscraper-2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "ofscraper"
-version = "2.1"
+version = "2.2"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
-packages = [{include = "ofscraper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 httpx = {extras = ["http2"], version = "^0.23.3"}
 inquirerpy = "^0.3.4"
 setuptools = "^67.6.0"
 schedule = "^1.1.0"
@@ -22,14 +21,15 @@
 pathvalidate = "^2.5.2"
 xxhash = "^3.2.0"
 mpegdash = "^0.3.1"
 diskcache = "^5.6.1"
 ffmpeg-python = "^0.2.0"
 dunamai = "^1.17.0"
 poetry-dynamic-versioning = "^0.22.0"
+textual = "^0.27.0"
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 
 
 [tool.poetry.group.test]
@@ -43,18 +43,18 @@
 pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.scripts]
-ofscraper = "ofscraper.scraper:main"
+ofscraper = "ofscraper.start:main"
 
 [project.scripts]
-ofscraper = "ofscraper.scraper:main"
+ofscraper = "ofscraper.start:main"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/datawhores/OF-Scraper"
 
 # pyproject.toml
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `ofscraper-2.1/PKG-INFO` & `ofscraper-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 2.1
+Version: 2.2
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +23,15 @@
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry-dynamic-versioning (>=0.22.0,<0.23.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
+Requires-Dist: textual (>=0.27.0,<0.28.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Project-URL: Homepage, https://github.com/datawhores/OF-Scraper
 Description-Content-Type: text/markdown
 
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with digitalcriminal's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
```

