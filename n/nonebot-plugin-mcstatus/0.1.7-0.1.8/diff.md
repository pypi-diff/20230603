# Comparing `tmp/nonebot_plugin_mcstatus-0.1.7.tar.gz` & `tmp/nonebot-plugin-mcstatus-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mcstatus-0.1.7.tar", max compression
+gzip compressed data, was "nonebot-plugin-mcstatus-0.1.8.tar", last modified: Sat Jun  3 07:30:24 2023, max compression
```

## Comparing `nonebot_plugin_mcstatus-0.1.7.tar` & `nonebot-plugin-mcstatus-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1063 2022-12-08 07:37:22.556748 nonebot_plugin_mcstatus-0.1.7/LICENSE
--rw-r--r--   0        0        0     1428 2022-12-08 08:44:05.880199 nonebot_plugin_mcstatus-0.1.7/README.md
--rw-r--r--   0        0        0     2993 2022-12-08 08:18:15.066820 nonebot_plugin_mcstatus-0.1.7/nonebot_plugin_mcstatus/__init__.py
--rw-r--r--   0        0        0     3243 2022-12-08 07:37:22.556748 nonebot_plugin_mcstatus-0.1.7/nonebot_plugin_mcstatus/data.py
--rw-r--r--   0        0        0     1676 2022-12-08 08:16:16.440150 nonebot_plugin_mcstatus-0.1.7/nonebot_plugin_mcstatus/handle.py
--rw-r--r--   0        0        0      635 2022-12-08 07:37:22.556748 nonebot_plugin_mcstatus-0.1.7/nonebot_plugin_mcstatus/parser.py
--rw-r--r--   0        0        0      640 2022-12-08 08:21:36.183493 nonebot_plugin_mcstatus-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 nonebot_plugin_mcstatus-0.1.7/setup.py
--rw-r--r--   0        0        0     2305 1970-01-01 00:00:00.000000 nonebot_plugin_mcstatus-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-03 07:30:00.967070 nonebot-plugin-mcstatus-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1428 2023-06-03 07:30:00.967070 nonebot-plugin-mcstatus-0.1.8/README.md
+-rw-r--r--   0        0        0     3557 2023-06-03 07:30:00.967070 nonebot-plugin-mcstatus-0.1.8/nonebot_plugin_mcstatus/__init__.py
+-rw-r--r--   0        0        0     3241 2023-06-03 07:30:00.967070 nonebot-plugin-mcstatus-0.1.8/nonebot_plugin_mcstatus/data.py
+-rw-r--r--   0        0        0     1676 2023-06-03 07:30:00.967070 nonebot-plugin-mcstatus-0.1.8/nonebot_plugin_mcstatus/handle.py
+-rw-r--r--   0        0        0      635 2023-06-03 07:30:00.967070 nonebot-plugin-mcstatus-0.1.8/nonebot_plugin_mcstatus/parser.py
+-rw-r--r--   0        0        0     1349 2023-06-03 07:30:00.967070 nonebot-plugin-mcstatus-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1793 1970-01-01 00:00:00.000000 nonebot-plugin-mcstatus-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_mcstatus-0.1.7/LICENSE` & `nonebot-plugin-mcstatus-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcstatus-0.1.7/README.md` & `nonebot-plugin-mcstatus-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcstatus-0.1.7/nonebot_plugin_mcstatus/data.py` & `nonebot-plugin-mcstatus-0.1.8/nonebot_plugin_mcstatus/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Dict, List, Optional, Union, cast
+from typing import Dict, List, Union, Optional, cast
 
 import yaml
 from pydantic import BaseModel
 
 
 class Server(BaseModel):
     name: str
@@ -21,15 +21,14 @@
     def __init__(self, path: Path = Path() / "data" / "mcstatus" / "server_list.yml"):
         self.__path = path
         self.__load()
 
     def get_server_list(
         self, user_id: Optional[int] = None, group_id: Optional[int] = None
     ) -> Union[ServerList, List[Server]]:
-
         server_list = self.__server_list
 
         if user_id:
             if user_id not in server_list["user"]:
                 server_list["user"][user_id] = []
             return server_list["user"][user_id]
         elif group_id:
@@ -58,15 +57,14 @@
 
     def remove_server(
         self,
         name: str,
         user_id: Optional[int] = None,
         group_id: Optional[int] = None,
     ):
-
         server_list = list(
             filter(
                 lambda server: server.name != name,
                 cast(List[Server], self.get_server_list(user_id, group_id)),
             )
         )
```

### Comparing `nonebot_plugin_mcstatus-0.1.7/nonebot_plugin_mcstatus/handle.py` & `nonebot-plugin-mcstatus-0.1.8/nonebot_plugin_mcstatus/handle.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, cast
 
 from mcstatus import JavaServer
 
-from nonebot_plugin_mcstatus.data import Data, Server
 from nonebot_plugin_mcstatus.parser import Namespace
+from nonebot_plugin_mcstatus.data import Data, Server
 
 
 class Handle:
     @classmethod
     async def check(cls, args: Namespace) -> str:
         try:
             ping = await JavaServer.lookup(args.address).async_ping()
```

### Comparing `nonebot_plugin_mcstatus-0.1.7/nonebot_plugin_mcstatus/parser.py` & `nonebot-plugin-mcstatus-0.1.8/nonebot_plugin_mcstatus/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mcstatus-0.1.7/setup.py` & `nonebot-plugin-mcstatus-0.1.8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,65 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-mcstatus
+Version: 0.1.8
+Summary: Check Minecraft server status
+License: MIT
+Author-email: Jigsaw <j1g5aw@foxmail.com>
+Requires-Python: >=3.8,<4.0
+Project-URL: homepage, https://github.com/nonepkg/plugin-mcstatus
+Project-URL: repository, https://github.com/nonepkg/plugin-mcstatus
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_mcstatus']
+# Nonebot Plugin MCStatus
 
-package_data = \
-{'': ['*']}
+基于 [nonebot2](https://github.com/nonebot/nonebot2) 和 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) 的 Minecraft 服务器状态查询插件
 
-install_requires = \
-['mcstatus>=10.0.1,<11.0.0',
- 'nonebot-adapter-onebot>=2.1.5,<3.0.0',
- 'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
- 'nonebot2>=2.0.0rc1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-mcstatus',
-    'version': '0.1.7',
-    'description': 'Check Minecraft server status',
-    'long_description': '# Nonebot Plugin MCStatus\n\n基于 [nonebot2](https://github.com/nonebot/nonebot2) 和 [go-cqhttp](https://github.com/Mrs4s/go-cqhttp) 的 Minecraft 服务器状态查询插件\n\n**目前仅能查询 Java 服务器，且非官方 Java 服务端则请自行测试。**\n\n[![License](https://img.shields.io/github/license/Jigsaw111/nonebot_plugin_mcstatus)](LICENSE)\n![Python Version](https://img.shields.io/badge/python-3.7.3+-blue.svg)\n![NoneBot Version](https://img.shields.io/badge/nonebot-2.0.0a11+-red.svg)\n![Pypi Version](https://img.shields.io/pypi/v/nonebot-plugin-mcstatus.svg)\n\n### 安装\n\n#### 从 PyPI 安装（推荐）\n\n- 使用 nb-cli  \n\n```\nnb plugin install nonebot_plugin_mcstatus\n```\n\n- 使用 poetry\n\n```\npoetry add nonebot_plugin_mcstatus\n```\n\n- 使用 pip\n\n```\npip install nonebot_plugin_mcstatus\n```\n\n#### 从 GitHub 安装（不推荐）\n\n```\ngit clone https://github.com/Jigsaw111/nonebot_plugin_mcstatus.git\n```\n\n### 使用\n\n**使用前请先确保命令前缀为空，否则请在以下命令前加上命令前缀 (默认为 `/` )。**\n\n- `mc list` 查看当前会话（群/私聊）的关注服务器列表\n- `mc add server address` 添加服务器到当前会话（群/私聊）的关注服务器列表\n- `mc remove server` 从当前会话（群/私聊）的关注服务器列表移除服务器\n- `mc check address` 查看指定地址的服务器状态（一次性）\n\n### Bug\n\n### To Do\n\n### Changelog\n',
-    'author': 'Jigsaw',
-    'author_email': 'j1g5aw@foxmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nonepkg/nonebot-plugin-mcstatus',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+**目前仅能查询 Java 服务器，且非官方 Java 服务端则请自行测试。**
 
+[![License](https://img.shields.io/github/license/Jigsaw111/nonebot_plugin_mcstatus)](LICENSE)
+![Python Version](https://img.shields.io/badge/python-3.7.3+-blue.svg)
+![NoneBot Version](https://img.shields.io/badge/nonebot-2.0.0a11+-red.svg)
+![Pypi Version](https://img.shields.io/pypi/v/nonebot-plugin-mcstatus.svg)
+
+### 安装
+
+#### 从 PyPI 安装（推荐）
+
+- 使用 nb-cli  
+
+```
+nb plugin install nonebot_plugin_mcstatus
+```
+
+- 使用 poetry
+
+```
+poetry add nonebot_plugin_mcstatus
+```
+
+- 使用 pip
+
+```
+pip install nonebot_plugin_mcstatus
+```
+
+#### 从 GitHub 安装（不推荐）
+
+```
+git clone https://github.com/Jigsaw111/nonebot_plugin_mcstatus.git
+```
+
+### 使用
+
+**使用前请先确保命令前缀为空，否则请在以下命令前加上命令前缀 (默认为 `/` )。**
+
+- `mc list` 查看当前会话（群/私聊）的关注服务器列表
+- `mc add server address` 添加服务器到当前会话（群/私聊）的关注服务器列表
+- `mc remove server` 从当前会话（群/私聊）的关注服务器列表移除服务器
+- `mc check address` 查看指定地址的服务器状态（一次性）
+
+### Bug
+
+### To Do
+
+### Changelog
 
-setup(**setup_kwargs)
```

