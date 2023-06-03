# Comparing `tmp/arkprts-0.1.4.tar.gz` & `tmp/arkprts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.1.4.tar", last modified: Fri May 26 14:45:21 2023, max compression
+gzip compressed data, was "arkprts-0.1.5.tar", last modified: Sat Jun  3 10:38:45 2023, max compression
```

## Comparing `arkprts-0.1.4.tar` & `arkprts-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.628323 arkprts-0.1.4/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1748 2023-05-26 14:45:21.616330 arkprts-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.482407 arkprts-0.1.4/arkprts/
--rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.4/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1925 2023-05-26 13:50:36.000000 arkprts-0.1.4/arkprts/__main__.py
--rw-rw-rw-   0        0        0    12518 2023-05-26 14:00:15.000000 arkprts-0.1.4/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.4/arkprts/errors.py
--rw-rw-rw-   0        0        0     6994 2023-05-26 14:35:04.000000 arkprts-0.1.4/arkprts/gamedata.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.591352 arkprts-0.1.4/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.4/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     3012 2023-05-21 13:53:11.000000 arkprts-0.1.4/arkprts/models/base.py
--rw-rw-rw-   0        0        0    11504 2023-05-26 14:36:53.000000 arkprts-0.1.4/arkprts/models/data.py
--rw-rw-rw-   0        0        0     7120 2023-05-26 13:50:27.000000 arkprts-0.1.4/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.4/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.554367 arkprts-0.1.4/arkprts.egg-info/
--rw-rw-rw-   0        0        0     1748 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 14:45:21.000000 arkprts-0.1.4/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 14:45:21.628323 arkprts-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-05-26 14:38:54.000000 arkprts-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:45:21.606339 arkprts-0.1.4/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.4/tests/test_config.py
--rw-rw-rw-   0        0        0      360 2023-05-26 14:03:38.000000 arkprts-0.1.4/tests/test_gamedata.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.899198 arkprts-0.1.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1748 2023-06-03 10:38:45.898198 arkprts-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.820244 arkprts-0.1.5/arkprts/
+-rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.5/arkprts/__init__.py
+-rw-rw-rw-   0        0        0     1925 2023-06-02 18:37:27.000000 arkprts-0.1.5/arkprts/__main__.py
+-rw-rw-rw-   0        0        0    13028 2023-06-03 10:35:52.000000 arkprts-0.1.5/arkprts/client.py
+-rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.5/arkprts/errors.py
+-rw-rw-rw-   0        0        0     7011 2023-06-02 19:22:21.000000 arkprts-0.1.5/arkprts/gamedata.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.888214 arkprts-0.1.5/arkprts/models/
+-rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.5/arkprts/models/__init__.py
+-rw-rw-rw-   0        0        0     3489 2023-06-03 10:30:47.000000 arkprts-0.1.5/arkprts/models/base.py
+-rw-rw-rw-   0        0        0    11504 2023-05-26 14:36:53.000000 arkprts-0.1.5/arkprts/models/data.py
+-rw-rw-rw-   0        0        0     7120 2023-05-26 13:50:27.000000 arkprts-0.1.5/arkprts/models/social.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.5/arkprts/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.873219 arkprts-0.1.5/arkprts.egg-info/
+-rw-rw-rw-   0        0        0     1748 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 10:38:45.899198 arkprts-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-06-03 10:37:23.000000 arkprts-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.896200 arkprts-0.1.5/tests/
+-rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.5/tests/test_config.py
+-rw-rw-rw-   0        0        0      360 2023-05-26 14:03:38.000000 arkprts-0.1.5/tests/test_gamedata.py
```

### Comparing `arkprts-0.1.4/LICENSE` & `arkprts-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.4/PKG-INFO` & `arkprts-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.4
+Version: 0.1.5
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.4/README.md` & `arkprts-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.4/arkprts/__main__.py` & `arkprts-0.1.5/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.4/arkprts/client.py` & `arkprts-0.1.5/arkprts/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     gamedata: GameData
     proxy: str | None = None
 
     uid: str | None
     secret: str | None
 
     _seqnum: int
+    _seqnum_lock: asyncio.Lock
 
     def __init__(
         self,
         *,
         config: Config | None = None,
         gamedata: GameData | None = None,
         pure: bool = False,
@@ -75,14 +76,15 @@
         self.config = config or Config()
         self.gamedata = gamedata or GameData()
         self.pure = pure
 
         self.uid = None
         self.secret = None
         self._seqnum = 1
+        self._seqnum_lock = asyncio.Lock()
 
     async def _request(
         self,
         method: str,
         url: str,
         *,
         headers: typing.Mapping[str, str] | None = None,
@@ -107,23 +109,24 @@
                 return data
 
     async def request(self, endpoint: str, *, method: str = "POST", **kwargs: typing.Any) -> typing.Any:
         """Make a request towards the game server."""
         if self.uid is None or self.secret is None:
             raise errors.NotLoggedInError("Not logged in.")
 
-        logger.debug("[%s] Sending request #%d to %s.", self.uid, self._seqnum, endpoint)
-        headers = {
-            "secret": self.secret,
-            "seqnum": str(self._seqnum),
-            "uid": self.uid,
-        }
-        self._seqnum += 1  # tfw no x++
+        async with self._seqnum_lock:
+            logger.debug("[%s] Sending request #%d to %s.", self.uid, self._seqnum, endpoint)
+            headers = {
+                "secret": self.secret,
+                "seqnum": str(self._seqnum),
+                "uid": self.uid,
+            }
+            self._seqnum += 1  # tfw no x++
 
-        return await self._request(method, f"{GAME_SERVER}/{endpoint}", headers=headers, **kwargs)
+            return await self._request(method, f"{GAME_SERVER}/{endpoint}", headers=headers, **kwargs)
 
     async def _load_network_config(self) -> None:
         """Get network config."""
         logger.debug("Loading network config.")
         data = await self._request("GET", f"{CONF_SERVER}/config/prod/official/network_config")
         content = json.loads(data["content"])
         self.config.sign = data["sign"]
@@ -270,18 +273,21 @@
     async def _get_social_sort_list(
         self,
         type: int,
         sort_key: typing.Sequence[str] = ["level"],
         param: typing.Mapping[str, str] = {},
     ) -> typing.Any:
         """Request sortedusers."""
-        return await self.request(
+        data = await self.request(
             "social/getSortListInfo",
             json={"type": type, "sortKeyList": sort_key, "param": param},
         )
+        data["result"].sort(key=lambda x: tuple(x[key] for key in sort_key), reverse=True)  # pyright: ignore
+
+        return data
 
     async def get_raw_friend_info(self, ids: typing.Sequence[str]) -> typing.Any:
         """Get detailed player info. You don't need to be friends actually."""
         return await self.request("social/getFriendList", json={"idList": ids})
 
     async def get_raw_player_info(self, ids: typing.Sequence[str]) -> typing.Any:
         """Get player info."""
@@ -299,23 +305,29 @@
         self,
         nickname: str,
         nicknumber: str = "",
         *,
         limit: int | None = None,
     ) -> typing.Sequence[models.Player]:
         """Search for a player and return a model."""
+        if "#" in nickname:
+            nickname, nicknumber = nickname.split("#", 1)
+
         uid_data = await self.get_raw_nicknamed(nickname, nicknumber)
-        uids = sorted(uid_data["result"], key=lambda x: x["level"], reverse=True)[:limit]
-        data = await self.get_raw_friend_info([uid["uid"] for uid in uids])
+        data = await self.get_raw_friend_info([uid["uid"] for uid in uid_data["result"][:limit]])
         return [models.Player(client=self, **i) for i in data["friends"]]
 
+    async def get_players(self, ids: typing.MutableSequence[str]) -> typing.Sequence[models.Player]:
+        """Get players and return a model."""
+        data = await self.get_raw_player_info(ids)
+        return [models.Player(client=self, **i) for i in data["result"]]
+
     async def get_friends(self, *, limit: int | None = None) -> typing.Sequence[models.Player]:
         """Get friends and return a model."""
         uid_data = await self.get_raw_friends()
-        uids = sorted(uid_data["result"], key=lambda x: x["level"], reverse=True)[:limit]
-        data = await self.get_raw_friend_info([uid["uid"] for uid in uids])
+        data = await self.get_raw_friend_info([uid["uid"] for uid in uid_data["result"][:limit]])
         return [models.Player(client=self, **i) for i in data["friends"]]
 
     async def get_data(self) -> models.User:
         """Get user sync data and return a model. Use raw data for more info."""
         data = await self.get_raw_data()
         return models.User(client=self, **data["user"])
```

### Comparing `arkprts-0.1.4/arkprts/errors.py` & `arkprts-0.1.5/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.4/arkprts/gamedata.py` & `arkprts-0.1.5/arkprts/gamedata.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         allow = allow or RELEVANT_FILES
 
         with tarfile.open(self.tarball_file) as tar:
             top_directory = os.path.commonprefix(tar.getnames())
 
             members: list[tarfile.TarInfo] = []
             for member in tar.getmembers():
-                if not re.search(allow, member.name):
+                if allow != "*" and not re.search(allow, member.name):
                     continue
 
                 member.name = member.name[len(top_directory + "/") :]
                 members.append(member)
 
             tar.extractall(self.directory, members=members)
```

### Comparing `arkprts-0.1.4/arkprts/models/base.py` & `arkprts-0.1.5/arkprts/models/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Modified pydantic base model."""
 import collections
+import datetime
 import typing
 
 import pydantic
 
 from arkprts.client import Client
 
 __all__ = ("BaseModel", "DDict")
@@ -42,14 +43,23 @@
 
     def __init__(self, client: typing.Optional[Client] = None, **kwargs: typing.Any) -> None:
         """Init."""
         super().__init__(client=_fake_client, **kwargs)
         if client:
             _set_recursively(self, "client", client)
 
+    @pydantic.root_validator  # pyright: ignore[reportUnknownMemberType]
+    def _fix_timestamps(cls, values: typing.Dict[str, typing.Any]) -> typing.Dict[str, typing.Any]:
+        """Arknights provides timestamps not with UTC but with the client's timezone."""
+        for key, value in values.items():
+            if isinstance(value, datetime.datetime):
+                values[key] = value.replace(tzinfo=None).astimezone()
+
+        return values
+
     class Config:
         """Config."""
 
         arbitrary_types_allowed = True
 
 
 class DList(collections.UserList[typing.Any]):
```

### Comparing `arkprts-0.1.4/arkprts/models/data.py` & `arkprts-0.1.5/arkprts/models/data.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.4/arkprts/models/social.py` & `arkprts-0.1.5/arkprts/models/social.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.4/arkprts.egg-info/PKG-INFO` & `arkprts-0.1.5/arkprts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.4
+Version: 0.1.5
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `arkprts-0.1.4/pyproject.toml` & `arkprts-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.4/setup.py` & `arkprts-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.1.4",
+    version="0.1.5",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic"],
     extras_require={
```

