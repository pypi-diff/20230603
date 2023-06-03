# Comparing `tmp/mindmate-0.0.3.tar.gz` & `tmp/mindmate-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindmate-0.0.3.tar", last modified: Wed Apr 26 02:26:13 2023, max compression
+gzip compressed data, was "mindmate-0.0.4.tar", last modified: Sat Jun  3 16:23:23 2023, max compression
```

## Comparing `mindmate-0.0.3.tar` & `mindmate-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.738560 mindmate-0.0.3/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1328 2023-04-26 02:26:13.734371 mindmate-0.0.3/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      527 2023-04-26 02:15:41.000000 mindmate-0.0.3/README.md
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.199887 mindmate-0.0.3/mindmate/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      616 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/cli.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.571443 mindmate-0.0.3/mindmate/commands/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/commands/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3899 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/commands/ai.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3448 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/commands/chat.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.0.3/mindmate/commands/configure.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      381 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/commands/dropdb.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      301 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/commands/initdb.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.709369 mindmate-0.0.3/mindmate/utils/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.3/mindmate/utils/__init__.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1699 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/utils/conf.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.0.3/mindmate/utils/env.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.0.3/mindmate/utils/helper.py
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1679 2023-04-26 02:15:41.000000 mindmate-0.0.3/mindmate/utils/utils.py
-drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-26 02:26:13.382032 mindmate-0.0.3/mindmate.egg-info/
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1328 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/PKG-INFO
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      537 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/SOURCES.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/dependency_links.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/entry_points.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       40 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/requires.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-04-26 02:26:11.000000 mindmate-0.0.3/mindmate.egg-info/top_level.txt
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-04-26 02:26:13.740563 mindmate-0.0.3/setup.cfg
--rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1793 2023-04-26 02:15:41.000000 mindmate-0.0.3/setup.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:23.250839 mindmate-0.0.4/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:23:23.247839 mindmate-0.0.4/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      701 2023-06-03 15:12:40.000000 mindmate-0.0.4/README.md
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:22.631647 mindmate-0.0.4/mindmate/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.4/mindmate/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      551 2023-06-03 16:21:53.000000 mindmate-0.0.4/mindmate/cli.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:22.968992 mindmate-0.0.4/mindmate/commands/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.4/mindmate/commands/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3968 2023-06-03 15:08:35.000000 mindmate-0.0.4/mindmate/commands/ai.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3448 2023-05-15 20:38:34.000000 mindmate-0.0.4/mindmate/commands/chat.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      756 2023-04-26 02:15:41.000000 mindmate-0.0.4/mindmate/commands/configure.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      143 2023-06-03 16:17:26.000000 mindmate-0.0.4/mindmate/commands/version.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       17 2023-06-03 16:13:11.000000 mindmate-0.0.4/mindmate/meta.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:23.062337 mindmate-0.0.4/mindmate/services/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:05:22.000000 mindmate-0.0.4/mindmate/services/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1457 2023-06-03 15:10:29.000000 mindmate-0.0.4/mindmate/services/directory.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     3545 2023-06-03 15:09:47.000000 mindmate-0.0.4/mindmate/services/models.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:23.225838 mindmate-0.0.4/mindmate/utils/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-04-24 04:35:25.000000 mindmate-0.0.4/mindmate/utils/__init__.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      730 2023-06-03 15:21:23.000000 mindmate-0.0.4/mindmate/utils/conf.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      619 2023-04-24 05:58:07.000000 mindmate-0.0.4/mindmate/utils/env.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      312 2023-04-26 01:29:16.000000 mindmate-0.0.4/mindmate/utils/helper.py
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     1862 2023-06-03 14:53:12.000000 mindmate-0.0.4/mindmate/utils/utils.py
+drwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        0 2023-06-03 16:23:22.813302 mindmate-0.0.4/mindmate.egg-info/
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2010 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/PKG-INFO
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)      616 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        1 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       47 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/entry_points.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       41 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/requires.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)        9 2023-06-03 16:23:21.000000 mindmate-0.0.4/mindmate.egg-info/top_level.txt
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)       38 2023-06-03 16:23:23.251843 mindmate-0.0.4/setup.cfg
+-rwxrwxrwx   0 yalattas  (1000) yalattas  (1000)     2260 2023-06-03 16:13:54.000000 mindmate-0.0.4/setup.py
```

### Comparing `mindmate-0.0.3/mindmate/cli.py` & `mindmate-0.0.4/mindmate/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import click
 from mindmate.utils import helper
 from mindmate.commands.configure import configure
 from mindmate.commands.chat import chat
 from mindmate.commands.ai import ai
-from mindmate.commands.initdb import initdb
-from mindmate.commands.dropdb import dropdb
+from mindmate.commands.version import version
 
 CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli():
     """hi to mindmate cli, try option --help for more information"""
     pass
 
 cli.add_command(configure)
 cli.add_command(chat)
-cli.add_command(initdb)
-cli.add_command(dropdb)
 cli.add_command(ai)
+cli.add_command(version)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `mindmate-0.0.3/mindmate/commands/ai.py` & `mindmate-0.0.4/mindmate/commands/ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import click
-from mindmate.utils.conf import constants
+from mindmate.services.directory import manifest
 
 def _generate_output(content: dict) -> None:
     # Determine the maximum length of keys for formatting
     try:
         max_key_length = max(len(str(key)) for key in content.keys())
     except ValueError as e:
         max_key_length = 5
@@ -69,71 +69,71 @@
 def coding():
     """Returns related functionalities to code-based AI platforms"""
     pass
 
 @click.command(name='list')
 def list_chat():
     """a list of AI platforms that offer chat-based responses"""
-    click.echo_via_pager(_generate_output(constants.WRITING))
+    click.echo_via_pager(_generate_output(manifest.list_writing()))
 
 chat.add_command(list_chat)
 
 @click.command(name='list')
 def list_image():
     """a list of AI platforms that offer image-based responses"""
-    click.echo_via_pager(_generate_output(constants.IMAGES))
+    click.echo_via_pager(_generate_output(manifest.list_images()))
 
 image.add_command(list_image)
 
 @click.command(name='list')
 def list_video():
     """a list of AI platforms that offer video-based responses"""
-    click.echo_via_pager(_generate_output(constants.VIDEO))
+    click.echo_via_pager(_generate_output(manifest.list_videos()))
 
 video.add_command(list_video)
 
 @click.command(name='list')
 def list_prompting():
     """a list of AI platforms that offer image-based responses"""
-    click.echo_via_pager(_generate_output(constants.PROMPTING))
+    click.echo_via_pager(_generate_output(manifest.list_prompting()))
 
 prompting.add_command(list_prompting)
 
 @click.command(name='list')
 def list_design():
     """a list of AI platforms that offer design-based responses"""
-    click.echo_via_pager(_generate_output(constants.DESIGN))
+    click.echo_via_pager(_generate_output(manifest.list_designs()))
 
 design.add_command(list_design)
 
 @click.command(name='list')
 def list_presentation():
     """a list of AI platforms that offer presentation-based responses"""
-    click.echo_via_pager(_generate_output(constants.PRESENTATION))
+    click.echo_via_pager(_generate_output(manifest.list_presentations()))
 
 presentation.add_command(list_presentation)
 
 @click.command(name='list')
 def list_no_code_apps():
     """a list of AI platforms that offer no-code development platform"""
-    click.echo_via_pager(_generate_output(constants.NO_CODE))
+    click.echo_via_pager(_generate_output(manifest.list_no_code()))
 
 no_code.add_command(list_no_code_apps)
 
 @click.command(name='list')
 def list_data():
     """a list of AI platforms that offer data-based responses"""
-    click.echo_via_pager(_generate_output(constants.DATA))
+    click.echo_via_pager(_generate_output(manifest.list_data()))
 
 data.add_command(list_data)
 
 @click.command(name='list')
 def list_coding():
     """a list of AI platforms that offer code-based responses"""
-    click.echo_via_pager(_generate_output(constants.CODING))
+    click.echo_via_pager(_generate_output(manifest.list_development()))
 
 coding.add_command(list_coding)
 
 ai.add_command(chat)
 ai.add_command(image)
 ai.add_command(video)
 ai.add_command(prompting)
```

### Comparing `mindmate-0.0.3/mindmate/commands/chat.py` & `mindmate-0.0.4/mindmate/commands/chat.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.3/mindmate/commands/configure.py` & `mindmate-0.0.4/mindmate/commands/configure.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.3/mindmate/utils/env.py` & `mindmate-0.0.4/mindmate/utils/env.py`

 * *Files identical despite different names*

### Comparing `mindmate-0.0.3/mindmate/utils/utils.py` & `mindmate-0.0.4/mindmate/utils/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import yaml
 import os
-from mindmate.utils.conf import constants
+from mindmate.utils.conf import constants, mongo
 
 class utility:
     def create_yaml_state(file: str) -> dict:
         while not os.path.isfile(constants.FILE_PATH+'/'+constants.FILE_NAME):
-            try:
-                os.makedirs(constants.FILE_PATH)
-            except FileExistsError as f:
-                pass
+            os.makedirs(constants.FILE_PATH, exist_ok=True)
             data = {
                 'version':1,
                 'keys': {
                     'openai_token':'xxxx',
                     'openai_id':'xxxx',
                 }
             }
@@ -34,8 +31,16 @@
 
     #TODO: below implementation is not associated with any functionality yet, require implementation to be completed
     def override_with_environment_variables(data: dict) -> dict:
         """Override YAML data with environment variables."""
         for key in data:
             if key in os.environ:
                 data[key] = os.environ[key]
-        return data
+        return data
+
+    def extract_results(result: dict) -> dict:
+        final = {}
+        for object in result:
+            for key, value in object.items():
+                if key != '_id':
+                    final.update({key: value})
+        return final
```

### Comparing `mindmate-0.0.3/mindmate.egg-info/SOURCES.txt` & `mindmate-0.0.4/mindmate.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 README.md
 setup.py
 mindmate/__init__.py
 mindmate/cli.py
+mindmate/meta.py
 mindmate.egg-info/PKG-INFO
 mindmate.egg-info/SOURCES.txt
 mindmate.egg-info/dependency_links.txt
 mindmate.egg-info/entry_points.txt
 mindmate.egg-info/requires.txt
 mindmate.egg-info/top_level.txt
 mindmate/commands/__init__.py
 mindmate/commands/ai.py
 mindmate/commands/chat.py
 mindmate/commands/configure.py
-mindmate/commands/dropdb.py
-mindmate/commands/initdb.py
+mindmate/commands/version.py
+mindmate/services/__init__.py
+mindmate/services/directory.py
+mindmate/services/models.py
 mindmate/utils/__init__.py
 mindmate/utils/conf.py
 mindmate/utils/env.py
 mindmate/utils/helper.py
 mindmate/utils/utils.py
```

### Comparing `mindmate-0.0.3/setup.py` & `mindmate-0.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,49 @@
+from mindmate import meta
 from setuptools import setup, find_packages
+try:
+    # For pip >= 10
+    from pip._internal.req import parse_requirements
+except ImportError:
+    # For pip <= 9.0.3
+    from pip.req import parse_requirements
 
 GITHUB_REPO = 'https://github.com/yalattas/mindmate'
+
+# Function to parse requirements recursively
+def parse_requirements_file(file_path):
+    requirements = parse_requirements(file_path, session=False)
+    sub_requirements = []
+    for req in requirements:
+        if req.req:
+            sub_requirements.append(str(req.req))
+    return sub_requirements
+
+# Parsing requirements recursively from requirements.txt file
+install_packages = parse_requirements_file('requirements.txt')
+
+# Reading README.md file
+with open('README.md', 'r', encoding='utf-8') as readme_file:
+    readme_contents = readme_file.read()
+
 setup(
     name='mindmate',
-    version='0.0.3',
+    version=meta.VERSION,
     author='Yasser Alattas',
     author_email='y.alattas@gmail.com',
     description="MindMate is a command-line tool that leverages the power of AI platforms to offer different use-cases to developers",
-    long_description="MindMate is a powerful command-line tool that harnesses the capabilities of state-of-the-art artificial intelligence platforms to offer a wide range of use-cases to developers. With MindMate, developers can easily leverage advanced natural language processing (NLP) and machine learning (ML) functionalities to enable various applications",
+    long_description=readme_contents,
+    long_description_content_type='text/markdown',
     url=GITHUB_REPO,
     download_url=GITHUB_REPO,
     packages=find_packages(),
-    keywords=['cli', 'ai', 'nlp', 'ml', 'developers', 'productivity', 'openai'],
+    platforms='any',
+    keywords=['cli', 'ai', 'nlp', 'ml', 'developers', 'productivity', 'openai', 'directory', 'manifest'],
     install_requires=[
-        'wheel',
-        'click>=8.1',
-        'openai>=0.27',
-        'PyYAML==6',
+        install_packages
     ],
     entry_points={
         'console_scripts': [
             'mindmate = mindmate.cli:cli',  # Update with your CLI entry point
         ],
     },
     # reference: https://pypi.org/classifiers/
```

