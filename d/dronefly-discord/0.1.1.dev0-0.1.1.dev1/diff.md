# Comparing `tmp/dronefly_discord-0.1.1.dev0.tar.gz` & `tmp/dronefly_discord-0.1.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_discord-0.1.1.dev0.tar", max compression
+gzip compressed data, was "dronefly_discord-0.1.1.dev1.tar", max compression
```

## Comparing `dronefly_discord-0.1.1.dev0.tar` & `dronefly_discord-0.1.1.dev1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.1.dev0/LICENSE
--rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.1.dev0/README.md
--rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.1.dev0/dronefly/discord/__init__.py
--rw-r--r--   0        0        0     3430 2023-05-27 08:05:17.585923 dronefly_discord-0.1.1.dev0/dronefly/discord/embeds.py
--rw-r--r--   0        0        0      688 2023-06-02 15:47:25.548696 dronefly_discord-0.1.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev0/setup.py
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.1.dev1/LICENSE
+-rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.1.dev1/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.1.dev1/dronefly/discord/__init__.py
+-rw-r--r--   0        0        0     3430 2023-05-27 08:05:17.585923 dronefly_discord-0.1.1.dev1/dronefly/discord/embeds.py
+-rw-r--r--   0        0        0      700 2023-06-03 21:17:43.151019 dronefly_discord-0.1.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1640 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev1/setup.py
+-rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev1/PKG-INFO
```

### Comparing `dronefly_discord-0.1.1.dev0/LICENSE` & `dronefly_discord-0.1.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev0/README.md` & `dronefly_discord-0.1.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev0/dronefly/discord/embeds.py` & `dronefly_discord-0.1.1.dev1/dronefly/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.1.dev0/setup.py` & `dronefly_discord-0.1.1.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['discord']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['dronefly-core>=0.3.5,<0.4.0',
+['dronefly-core>=0.3.6.dev0,<0.4.0',
  'inflect>=5.3.0,<6.0.0',
- 'pyinaturalist>=0.18,<0.20']
+ 'pyinaturalist>=0.19.0.dev2,<0.20']
 
 setup_kwargs = {
     'name': 'dronefly-discord',
-    'version': '0.1.1.dev0',
+    'version': '0.1.1.dev1',
     'description': 'Dronefly Discord library',
     'long_description': "# Dronefly Discord\n\nThis library will support writing Discord cogs based on\n[dronefly-core](https://github.com/dronefly-garden/dronefly-core). It is\nderived from the Discord-specific code extracted from the original\n[Dronefly](https://dronefly.readthedocs.io) bot codebase. We aim to keep\nthe library general enough to work with any bot based on\n[discord.py](https://discordpy.readthedocs.io), as well as on bots using\nthe [Red-DiscordBot](https://docs.discord.red) framework.\n\n# Related packages\n\n## Dronefly core\n\nThe [dronefly-core](https://github.com/dronefly-garden/dronefly-core)\npackage is an incomplete rewrite of [Dronefly](https://dronefly.readthedocs.io/)\nDiscord bot's core components.\n\n## Dronefly Discord bot\n\nDronefly Discord bot brings [iNaturalist](https://www.inaturalist.org) taxa,\nobservations, and other data from the site into conversations on the\n[Discord](https://discord.com) chat platform.\n",
     'author': 'Ben Armstrong',
     'author_email': 'synrg@debian.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dronefly_discord-0.1.1.dev0/PKG-INFO` & `dronefly_discord-0.1.1.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dronefly-discord
-Version: 0.1.1.dev0
+Version: 0.1.1.dev1
 Summary: Dronefly Discord library
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dronefly-core (>=0.3.5,<0.4.0)
+Requires-Dist: dronefly-core (>=0.3.6.dev0,<0.4.0)
 Requires-Dist: inflect (>=5.3.0,<6.0.0)
-Requires-Dist: pyinaturalist (>=0.18,<0.20)
+Requires-Dist: pyinaturalist (>=0.19.0.dev2,<0.20)
 Description-Content-Type: text/markdown
 
 # Dronefly Discord
 
 This library will support writing Discord cogs based on
 [dronefly-core](https://github.com/dronefly-garden/dronefly-core). It is
 derived from the Discord-specific code extracted from the original
```

