# Comparing `tmp/slixmppbot-2.0.3.tar.gz` & `tmp/slixmppbot-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slixmppbot-2.0.3.tar", max compression
+gzip compressed data, was "slixmppbot-2.0.4.tar", max compression
```

## Comparing `slixmppbot-2.0.3.tar` & `slixmppbot-2.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35141 2017-03-12 18:31:56.511032 slixmppbot-2.0.3/LICENSE
--rw-r--r--   0        0        0      504 2023-06-02 15:29:47.872743 slixmppbot-2.0.3/README.md
--rw-r--r--   0        0        0      787 2023-06-02 16:28:51.941340 slixmppbot-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      159 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/__init__.py
--rw-r--r--   0        0        0     2205 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/basebot.py
--rw-r--r--   0        0        0     4673 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/cmdbot.py
--rw-r--r--   0        0        0      294 2023-06-02 15:29:47.884743 slixmppbot-2.0.3/xmppbot/common.py
--rw-r--r--   0        0        0     3920 2023-06-02 15:46:26.508820 slixmppbot-2.0.3/xmppbot/configbot.py
--rw-r--r--   0        0        0      475 2023-06-02 15:29:47.888743 slixmppbot-2.0.3/xmppbot/timeout.py
--rw-r--r--   0        0        0     7691 2023-06-02 15:46:01.156829 slixmppbot-2.0.3/xmppbot/xmppbot.py
--rw-r--r--   0        0        0     2730 2023-06-02 16:28:09.277379 slixmppbot-2.0.3/xmppbot/xmppmsg.py
--rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 slixmppbot-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35141 2017-03-12 18:31:56.511032 slixmppbot-2.0.4/LICENSE
+-rw-r--r--   0        0        0      504 2023-06-02 15:29:47.872743 slixmppbot-2.0.4/README.md
+-rw-r--r--   0        0        0      787 2023-06-02 22:17:54.257498 slixmppbot-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-06-02 15:29:47.884743 slixmppbot-2.0.4/xmppbot/__init__.py
+-rw-r--r--   0        0        0     2205 2023-06-02 15:29:47.884743 slixmppbot-2.0.4/xmppbot/basebot.py
+-rw-r--r--   0        0        0     4673 2023-06-02 15:29:47.884743 slixmppbot-2.0.4/xmppbot/cmdbot.py
+-rw-r--r--   0        0        0      294 2023-06-02 15:29:47.884743 slixmppbot-2.0.4/xmppbot/common.py
+-rw-r--r--   0        0        0     3920 2023-06-02 15:46:26.508820 slixmppbot-2.0.4/xmppbot/configbot.py
+-rw-r--r--   0        0        0      475 2023-06-02 15:29:47.888743 slixmppbot-2.0.4/xmppbot/timeout.py
+-rw-r--r--   0        0        0     7691 2023-06-02 15:46:01.156829 slixmppbot-2.0.4/xmppbot/xmppbot.py
+-rw-r--r--   0        0        0     2784 2023-06-02 22:17:23.501432 slixmppbot-2.0.4/xmppbot/xmppmsg.py
+-rw-r--r--   0        0        0     1302 1970-01-01 00:00:00.000000 slixmppbot-2.0.4/PKG-INFO
```

### Comparing `slixmppbot-2.0.3/LICENSE` & `slixmppbot-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.3/pyproject.toml` & `slixmppbot-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slixmppbot"
-version = "2.0.3"
+version = "2.0.4"
 description = "A framework for writing Jabber/XMPP bots"
 authors = ["s-nt-s <santos82h@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 include = ["LICENSE"]
 homepage = "https://github.com/s-nt-s/XmppBot"
 keywords = ["xmpp", "bot"]
```

### Comparing `slixmppbot-2.0.3/xmppbot/basebot.py` & `slixmppbot-2.0.4/xmppbot/basebot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.3/xmppbot/cmdbot.py` & `slixmppbot-2.0.4/xmppbot/cmdbot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.3/xmppbot/configbot.py` & `slixmppbot-2.0.4/xmppbot/configbot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.3/xmppbot/xmppbot.py` & `slixmppbot-2.0.4/xmppbot/xmppbot.py`

 * *Files identical despite different names*

### Comparing `slixmppbot-2.0.3/xmppbot/xmppmsg.py` & `slixmppbot-2.0.4/xmppbot/xmppmsg.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,21 @@
             self.register_plugin('xep_0045')  # Multi-User Chat
         self.messages = []
         self.add_event_handler("session_start", self.start)
 
     async def start(self, event):
         await self.get_roster()
         self.send_presence()
-        rooms = set(self.config.rooms).intersection(tm[0] for tm in self.messages)
+        rooms = set(
+            self.config.rooms).intersection(
+            tm[0] for tm in self.messages)
 
         for room in rooms:
             await self.xep_0045.join_muc(room, self.config.user.split("@")[0])
+            time.sleep(0.1)
         while self.messages:
             to, msg = self.messages.pop(0)
             mtype = 'chat'
             if to in rooms:
                 mtype = 'groupchat'
             self.send_message(mto=to,
                               mbody=msg,
```

### Comparing `slixmppbot-2.0.3/PKG-INFO` & `slixmppbot-2.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slixmppbot
-Version: 2.0.3
+Version: 2.0.4
 Summary: A framework for writing Jabber/XMPP bots
 Home-page: https://github.com/s-nt-s/XmppBot
 License: GPLv3
 Keywords: xmpp,bot
 Author: s-nt-s
 Author-email: santos82h@gmail.com
 Requires-Python: >=3.9,<4.0
```

