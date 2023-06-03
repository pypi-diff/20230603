# Comparing `tmp/arkprts-0.1.5.tar.gz` & `tmp/arkprts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkprts-0.1.5.tar", last modified: Sat Jun  3 10:38:45 2023, max compression
+gzip compressed data, was "arkprts-0.1.6.tar", last modified: Sat Jun  3 19:20:34 2023, max compression
```

## Comparing `arkprts-0.1.5.tar` & `arkprts-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.899198 arkprts-0.1.5/
--rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1748 2023-06-03 10:38:45.898198 arkprts-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1462 2023-05-19 17:49:21.000000 arkprts-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.820244 arkprts-0.1.5/arkprts/
--rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.5/arkprts/__init__.py
--rw-rw-rw-   0        0        0     1925 2023-06-02 18:37:27.000000 arkprts-0.1.5/arkprts/__main__.py
--rw-rw-rw-   0        0        0    13028 2023-06-03 10:35:52.000000 arkprts-0.1.5/arkprts/client.py
--rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.5/arkprts/errors.py
--rw-rw-rw-   0        0        0     7011 2023-06-02 19:22:21.000000 arkprts-0.1.5/arkprts/gamedata.py
-drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.888214 arkprts-0.1.5/arkprts/models/
--rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.5/arkprts/models/__init__.py
--rw-rw-rw-   0        0        0     3489 2023-06-03 10:30:47.000000 arkprts-0.1.5/arkprts/models/base.py
--rw-rw-rw-   0        0        0    11504 2023-05-26 14:36:53.000000 arkprts-0.1.5/arkprts/models/data.py
--rw-rw-rw-   0        0        0     7120 2023-05-26 13:50:27.000000 arkprts-0.1.5/arkprts/models/social.py
--rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.5/arkprts/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.873219 arkprts-0.1.5/arkprts.egg-info/
--rw-rw-rw-   0        0        0     1748 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 10:38:45.000000 arkprts-0.1.5/arkprts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 10:38:45.899198 arkprts-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      623 2023-06-03 10:37:23.000000 arkprts-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 10:38:45.896200 arkprts-0.1.5/tests/
--rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.5/tests/test_config.py
--rw-rw-rw-   0        0        0      360 2023-05-26 14:03:38.000000 arkprts-0.1.5/tests/test_gamedata.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.646733 arkprts-0.1.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-30 21:01:40.000000 arkprts-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3019 2023-06-03 19:20:34.642736 arkprts-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2687 2023-06-03 19:10:54.000000 arkprts-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.556785 arkprts-0.1.6/arkprts/
+-rw-rw-rw-   0        0        0      111 2023-05-19 17:48:39.000000 arkprts-0.1.6/arkprts/__init__.py
+-rw-rw-rw-   0        0        0     1925 2023-06-02 18:37:27.000000 arkprts-0.1.6/arkprts/__main__.py
+-rw-rw-rw-   0        0        0    13911 2023-06-03 18:46:42.000000 arkprts-0.1.6/arkprts/client.py
+-rw-rw-rw-   0        0        0     1356 2023-05-07 16:47:55.000000 arkprts-0.1.6/arkprts/errors.py
+-rw-rw-rw-   0        0        0     7295 2023-06-03 19:11:28.000000 arkprts-0.1.6/arkprts/gamedata.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.634742 arkprts-0.1.6/arkprts/models/
+-rw-rw-rw-   0        0        0       75 2023-05-07 15:46:44.000000 arkprts-0.1.6/arkprts/models/__init__.py
+-rw-rw-rw-   0        0        0     3631 2023-06-03 18:45:01.000000 arkprts-0.1.6/arkprts/models/base.py
+-rw-rw-rw-   0        0        0    11643 2023-06-03 18:59:38.000000 arkprts-0.1.6/arkprts/models/data.py
+-rw-rw-rw-   0        0        0     7056 2023-06-03 19:00:31.000000 arkprts-0.1.6/arkprts/models/social.py
+-rw-rw-rw-   0        0        0        0 2023-04-30 21:01:40.000000 arkprts-0.1.6/arkprts/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.611754 arkprts-0.1.6/arkprts.egg-info/
+-rw-rw-rw-   0        0        0     3019 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 19:20:34.000000 arkprts-0.1.6/arkprts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2569 2023-05-19 18:44:52.000000 arkprts-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 19:20:34.646733 arkprts-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      623 2023-06-03 19:19:53.000000 arkprts-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 19:20:34.640737 arkprts-0.1.6/tests/
+-rw-rw-rw-   0        0        0      282 2023-05-01 00:20:38.000000 arkprts-0.1.6/tests/test_config.py
+-rw-rw-rw-   0        0        0      360 2023-05-26 14:03:38.000000 arkprts-0.1.6/tests/test_gamedata.py
```

### Comparing `arkprts-0.1.5/LICENSE` & `arkprts-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.5/PKG-INFO` & `arkprts-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkprts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Arknights python wrapper.
 Home-page: https://github.com/thesadru/arkprts
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
@@ -47,11 +47,57 @@
 users = await client.search_user("UserName")
 operator = users[0].assist_char_list[0]  # type: arkprts.models.Character
 print(f"Assist operator {operator.static.name} is level {operator.level}")
 ```
 
 To disable downloading static data use `arkprts.Client(pure=True)`. To choose the data download location set `client.gamedata = akprts.GameData("/path/to/data")`.
 
+If you do not trust logging in with your account but still wish to request public game data you may log in as a guest.
+Remember to save the generated credentials to not spam Arknights servers.
+
+```py
+client = arkprts.Client()
+uid, token = await client.login_as_guest()
+print(f"Please save uid {uid} and token {token}")
+
+users = await client.search_user("Doctor")
+
+# and later if you wish to use the same guest account again
+client = arkprts.Client()
+await client.login_with_token(uid, token)
+
+users = await client.search_user("Doctor")
+```
+
+### Frequent usage cases
+
+Get all of my operators.
+
+```py
+data = await client.get_data()
+for char in data.troop.chars.values():
+    print(char.char_id)
+```
+
+Get my inventory.
+
+```py
+data = await client.get_data()
+# normal inventory items
+for item_id, count in user.inventory.items():
+    if count > 0:
+        print(item_id, count)
+# basic items like originium or green certificates
+for item_id, count in user.status.basic_item_inventory.items():
+    if count > 0:
+        print(item_id, count)
+# consumable expirable items
+for item_id, subitems in user.consumable.items():
+    for item in subitems.values():
+        if count > 0:
+            print(item_id, item.ts, item.count)
+```
+
 ## Contributing
 
 Any kind of contribution is welcome.
 Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
```

### Comparing `arkprts-0.1.5/README.md` & `arkprts-0.1.6/arkprts.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,103 @@
-# ArkPRTS
-
-Arknights python wrapper.
-
-This project aims to purely allow for data collection, no account automation is planned.
-
----
-
-Source Code: <https://github.com/thesadru/arkprts>
-
----
-
-## Usage
-
-```py
-import arkprts
-
-async def main() -> None:
-    client = arkprts.Client()
-    await client.login_with_email("user@gmail.com")
-    # or client.login_with_token("123456", "abcdefg")
-
-    # get logged-in user data
-    data = await client.get_data()
-    print("Level: ", data.status.level)
-
-    # get data of other users
-    users = await client.search_user("UserName")
-    print("Level: ", users[0].level)
-```
-
-Returned data is in the form of pydantic models, however you can also request raw json with `client.get_raw_data()` to access even untyped data.
-
-For convenience, static game data is automatically downloaded and updated on login. You can access the static data directly or through the models. This is useful for getting names and descriptions of objects.
-
-```py
-users = await client.search_user("UserName")
-operator = users[0].assist_char_list[0]  # type: arkprts.models.Character
-print(f"Assist operator {operator.static.name} is level {operator.level}")
-```
-
-To disable downloading static data use `arkprts.Client(pure=True)`. To choose the data download location set `client.gamedata = akprts.GameData("/path/to/data")`.
-
-## Contributing
-
-Any kind of contribution is welcome.
-Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
+Metadata-Version: 2.1
+Name: arkprts
+Version: 0.1.6
+Summary: Arknights python wrapper.
+Home-page: https://github.com/thesadru/arkprts
+License: MIT
+Description-Content-Type: text/markdown
+Provides-Extra: all
+License-File: LICENSE
+
+# ArkPRTS
+
+Arknights python wrapper.
+
+This project aims to purely allow for data collection, no account automation is planned.
+
+---
+
+Source Code: <https://github.com/thesadru/arkprts>
+
+---
+
+## Usage
+
+```py
+import arkprts
+
+async def main() -> None:
+    client = arkprts.Client()
+    await client.login_with_email("user@gmail.com")
+    # or client.login_with_token("123456", "abcdefg")
+
+    # get logged-in user data
+    data = await client.get_data()
+    print("Level: ", data.status.level)
+
+    # get data of other users
+    users = await client.search_user("UserName")
+    print("Level: ", users[0].level)
+```
+
+Returned data is in the form of pydantic models, however you can also request raw json with `client.get_raw_data()` to access even untyped data.
+
+For convenience, static game data is automatically downloaded and updated on login. You can access the static data directly or through the models. This is useful for getting names and descriptions of objects.
+
+```py
+users = await client.search_user("UserName")
+operator = users[0].assist_char_list[0]  # type: arkprts.models.Character
+print(f"Assist operator {operator.static.name} is level {operator.level}")
+```
+
+To disable downloading static data use `arkprts.Client(pure=True)`. To choose the data download location set `client.gamedata = akprts.GameData("/path/to/data")`.
+
+If you do not trust logging in with your account but still wish to request public game data you may log in as a guest.
+Remember to save the generated credentials to not spam Arknights servers.
+
+```py
+client = arkprts.Client()
+uid, token = await client.login_as_guest()
+print(f"Please save uid {uid} and token {token}")
+
+users = await client.search_user("Doctor")
+
+# and later if you wish to use the same guest account again
+client = arkprts.Client()
+await client.login_with_token(uid, token)
+
+users = await client.search_user("Doctor")
+```
+
+### Frequent usage cases
+
+Get all of my operators.
+
+```py
+data = await client.get_data()
+for char in data.troop.chars.values():
+    print(char.char_id)
+```
+
+Get my inventory.
+
+```py
+data = await client.get_data()
+# normal inventory items
+for item_id, count in user.inventory.items():
+    if count > 0:
+        print(item_id, count)
+# basic items like originium or green certificates
+for item_id, count in user.status.basic_item_inventory.items():
+    if count > 0:
+        print(item_id, count)
+# consumable expirable items
+for item_id, subitems in user.consumable.items():
+    for item in subitems.values():
+        if count > 0:
+            print(item_id, item.ts, item.count)
+```
+
+## Contributing
+
+Any kind of contribution is welcome.
+Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for more information.
```

### Comparing `arkprts-0.1.5/arkprts/__main__.py` & `arkprts-0.1.6/arkprts/__main__.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.5/arkprts/client.py` & `arkprts-0.1.6/arkprts/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,17 +159,28 @@
         body = {
             "platform": "android",
             "uid": channel_uid,
             "token": yostar_token,
             "deviceId": self.config.device_id,
         }
         data = await self._request("POST", f"{PASSPORT_SERVER}/user/login", json=body)
-        # print(data["yostar_username"])
         return data["accessToken"]
 
+    async def _create_guest_account(self, device_id: str | None = None) -> tuple[str, str]:
+        """Create a new guest account."""
+        if device_id:
+            self.config.device_id = device_id
+
+        logger.debug("Creating guest account.")
+        body = {
+            "deviceId": self.config.device_id,
+        }
+        data = await self._request("POST", f"{PASSPORT_SERVER}/user/create", json=body)
+        return data["uid"], data["token"]
+
     async def _get_u8_token(self, channel_uid: str, access_token: str) -> str:
         """Get an arknights uid and u8 token from a channel uid and access token."""
         logger.debug("Getting u8 token.")
         body = {
             "appId": "1",
             "channelId": "3",
             "extension": json.dumps({"uid": channel_uid, "token": access_token}),
@@ -258,14 +269,26 @@
         yostar_uid, yostar_token = await self._submit_yostar_auth(email, code)
         channel_uid, token = await self._get_yostar_token(email, yostar_uid, yostar_token)
         await self.login_with_token(channel_uid, token)
 
         print(f"Channel UID: {channel_uid} Token: {token}")  # noqa: T201
         print(f'Usage: client.login_with_token("{channel_uid}", "{token}")')  # noqa: T201
 
+    async def login_as_guest(
+        self,
+        nickname: str | None = None,
+        *,
+        device_id: str | None = None,
+    ) -> tuple[str, str]:
+        """Login as guest and return tokens."""
+        channel_uid, yostar_token = await self._create_guest_account(device_id)
+        await self.login_with_token(channel_uid, yostar_token)
+        await self._bind_nickname(nickname or "Doctor")
+        return channel_uid, yostar_token
+
     async def _bind_nickname(self, nickname: str) -> typing.Any:
         """Bind a nickname. Required for new accounts."""
         return await self.request("user/bindNickName", json={"nickName": nickname})
 
     async def get_raw_data(self) -> typing.Any:
         """Get user data."""
         return await self.request("account/syncData", json={"platform": 1})
```

### Comparing `arkprts-0.1.5/arkprts/errors.py` & `arkprts-0.1.6/arkprts/errors.py`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.5/arkprts/gamedata.py` & `arkprts-0.1.6/arkprts/gamedata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Gamedata client. Fetches from github and such."""
 from __future__ import annotations
 
+import bisect
 import json
 import logging
 import os
 import os.path
 import pathlib
 import re
 import tarfile
@@ -183,7 +184,12 @@
         data = self.get_excel("skill_table", server=server)
         return data[id]
 
     def get_module(self, id: str, *, server: str | None = None) -> models.DDict:
         """Get a module."""
         data = self.get_excel("uniequip_table", server=server)
         return data["equipDict"][id]
+
+    def calculate_trust_level(self, trust: int) -> int:
+        """Calculate trust level from trust points."""
+        frames = self.get_excel("favor_table")["favor_frames"]
+        return bisect.bisect_left(frames, trust, key=lambda x: x["data"]["favor_point"])
```

### Comparing `arkprts-0.1.5/arkprts/models/base.py` & `arkprts-0.1.6/arkprts/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,19 @@
             _set_recursively(self, "client", client)
 
     @pydantic.root_validator  # pyright: ignore[reportUnknownMemberType]
     def _fix_timestamps(cls, values: typing.Dict[str, typing.Any]) -> typing.Dict[str, typing.Any]:
         """Arknights provides timestamps not with UTC but with the client's timezone."""
         for key, value in values.items():
             if isinstance(value, datetime.datetime):
-                values[key] = value.replace(tzinfo=None).astimezone()
+                ts = value.timestamp()
+                if ts in (0, -1):
+                    values[key] = None
+                else:
+                    values[key] = value.replace(tzinfo=None).astimezone()
 
         return values
 
     class Config:
         """Config."""
 
         arbitrary_types_allowed = True
```

### Comparing `arkprts-0.1.5/arkprts/models/data.py` & `arkprts-0.1.6/arkprts/models/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,22 +152,15 @@
     unlock: bool
     """Whether the skill is unlocked."""
     state: bool = pydantic.Field(repr=False)
     """IDK. Always false."""
     specialize_level: int = pydantic.Field(alias="specializeLevel")
     """Skill mastery level."""
     complete_upgrade_time: typing.Optional[datetime.datetime] = pydantic.Field(alias="completeUpgradeTime")
-    """IDK. Time left until skill upgrade is complete. Is -1 if not upgrading."""
-
-    @pydantic.validator("complete_upgrade_time", pre=True)  # pyright: ignore[reportUnknownMemberType]
-    def _complete_upgrade_time(cls, v: int) -> typing.Optional[int]:
-        if v == -1:
-            return None
-
-        return v
+    """IDK. Time left until skill upgrade is complete. Is raw -1 if not upgrading."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this skill."""
         return self.client.gamedata.skill_table[self.skill_id]
 
 
@@ -186,15 +179,15 @@
     """Operator data."""
 
     inst_id: int = pydantic.Field(alias="instId")
     """Index of the operator."""
     char_id: str = pydantic.Field(alias="charId")
     """Operator ID."""
     favor_point: int = pydantic.Field(alias="favorPoint")
-    """Operator trust."""
+    """Operator trust points."""
     potential_rank: int = pydantic.Field(alias="potentialRank")
     """Operator potential. Starts at 0."""
     main_skill_lvl: int = pydantic.Field(alias="mainSkillLvl")
     """Operator skill level."""
     skin: str
     """Operator skin ID."""
     level: int
@@ -217,14 +210,19 @@
     """Whether the operator is marked as favorite."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this operator."""
         return self.client.gamedata.character_table[self.char_id]
 
+    @property
+    def trust(self) -> int:
+        """Trust calculated from favor_point."""
+        return self.client.gamedata.calculate_trust_level(self.favor_point)
+
     @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
     def _fix_amiya(cls, values: typing.Any) -> typing.Any:
         """Flatten Amiya to only keep her guard form."""
         if values and values.get("tmpl"):
             current = values["tmpl"][values["currentTmpl"]]
             values.update(current)
             values["skin"] = current["skinId"]  # why even?
@@ -232,15 +230,20 @@
         return values
 
 
 class CharGroup(base.BaseModel):
     """Additional operator data."""
 
     favor_point: int = pydantic.Field(alias="favorPoint")
-    """Operator trust."""
+    """Operator trust points."""
+
+    @property
+    def trust(self) -> int:
+        """Trust calculated from favor_point."""
+        return self.client.gamedata.calculate_trust_level(self.favor_point)
 
 
 class Troops(base.BaseModel):
     """Operator data."""
 
     cur_char_inst_id: int = pydantic.Field(alias="curCharInstId")
     """Amount of owned operators."""
@@ -290,15 +293,15 @@
     medal_board: base.DDict = pydantic.Field(default_factory=base.DDict, alias="medalBoard")
     """Medal board."""
 
 
 class ConsumableExpire(base.BaseModel):
     """Consumable expiration data."""
 
-    ts: datetime.datetime
+    ts: typing.Optional[datetime.datetime]
     """When the consumable expires."""
     count: int
     """Amount of consumables."""
 
 
 class User(base.BaseModel):
     """User sync data. Not fully modeled."""
```

### Comparing `arkprts-0.1.5/arkprts/models/social.py` & `arkprts-0.1.6/arkprts/models/social.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,22 +27,15 @@
     unlock: bool
     """Whether the skill is unlocked."""
     state: bool = pydantic.Field(repr=False)
     """IDK. Always false."""
     specialize_level: int = pydantic.Field(alias="specializeLevel")
     """Skill mastery level."""
     complete_upgrade_time: typing.Optional[datetime.datetime] = pydantic.Field(alias="completeUpgradeTime")
-    """IDK. Time left until skill upgrade is complete. Is -1 if not upgrading."""
-
-    @pydantic.validator("complete_upgrade_time", pre=True)  # pyright: ignore[reportUnknownMemberType]
-    def _complete_upgrade_time(cls, v: int) -> typing.Optional[int]:
-        if v == -1:
-            return None
-
-        return v
+    """IDK. Time left until skill upgrade is complete. Is raw -1 if not upgrading."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this skill."""
         return self.client.gamedata.skill_table[self.skill_id]
 
 
@@ -69,15 +62,15 @@
     main_skill_lvl: int = pydantic.Field(alias="mainSkillLvl")
     """Level of the equipped skill."""
     skill_index: int = pydantic.Field(alias="skillIndex")
     """Index of the equipped skill."""
     evolve_phase: int = pydantic.Field(alias="evolvePhase")
     """Elite phase."""
     favor_point: int = pydantic.Field(alias="favorPoint")
-    """Raw trust points (25570 is 200% Trust)"""
+    """Operator trust points."""
     potential_rank: int = pydantic.Field(alias="potentialRank")
     """Operator potential. Starts at 0."""
     level: int
     """Operator level."""
     crisis_record: base.DDict = pydantic.Field(alias="crisisRecord", repr=False)
     """IDK. selectedCrisis is used for contingency contracts elsewhere."""
     current_equip: typing.Optional[str] = pydantic.Field(alias="currentEquip")
@@ -86,14 +79,19 @@
     """Equipped modules. Module ID to module info."""
 
     @property
     def static(self) -> base.DDict:
         """Static data for this operator."""
         return self.client.gamedata.character_table[self.char_id]
 
+    @property
+    def trust(self) -> int:
+        """Trust calculated from favor_point."""
+        return self.client.gamedata.calculate_trust_level(self.favor_point)
+
     @pydantic.root_validator(pre=True)  # pyright: ignore[reportUnknownMemberType]
     def _fix_amiya(cls, values: typing.Any) -> typing.Any:
         """Flatten Amiya to only keep her guard form."""
         if values and values.get("tmpl"):
             current = values["tmpl"][values["currentTmpl"]]
             values.update(current)
 
@@ -191,13 +189,13 @@
     """ID of the secretary operator's skin."""
     resume: str
     """Player display bio."""
     team_v2: typing.Mapping[str, int] = pydantic.Field(alias="teamV2")
     """Amount of characters owned in each faction."""
     board: typing.Sequence[str]
     """Factions with full trust. Shows up blue in-game."""
-    info_share: datetime.datetime = pydantic.Field(alias="infoShare")
+    info_share: typing.Optional[datetime.datetime] = pydantic.Field(alias="infoShare")
     """IDK."""
     recent_visited: bool = pydantic.Field(alias="recentVisited")
     """IDK."""
     info_share_visited: typing.Optional[int] = pydantic.Field(None, alias="infoShareVisited")
     """IDK."""
```

### Comparing `arkprts-0.1.5/pyproject.toml` & `arkprts-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkprts-0.1.5/setup.py` & `arkprts-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Run setuptools."""
 import pathlib
 
 from setuptools import find_packages, setup
 
 setup(
     name="arkprts",
-    version="0.1.5",
+    version="0.1.6",
     description="Arknights python wrapper.",
     url="https://github.com/thesadru/arkprts",
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     package_data={"arkprts": ["py.typed"]},
     install_requires=["aiohttp", "pydantic"],
     extras_require={
```

