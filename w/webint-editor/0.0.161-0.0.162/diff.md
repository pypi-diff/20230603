# Comparing `tmp/webint_editor-0.0.161.tar.gz` & `tmp/webint_editor-0.0.162.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_editor-0.0.161.tar", max compression
+gzip compressed data, was "webint_editor-0.0.162.tar", max compression
```

## Comparing `webint_editor-0.0.161.tar` & `webint_editor-0.0.162.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      892 2023-06-03 07:19:32.974316 webint_editor-0.0.161/pyproject.toml
--rw-r--r--   0        0        0     4929 2023-06-03 02:55:47.150152 webint_editor-0.0.161/webint_editor/__init__.py
--rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.161/webint_editor/templates/__init__.py
--rw-r--r--   0        0        0    17460 2023-06-03 07:19:30.754267 webint_editor-0.0.161/webint_editor/templates/draft.html
--rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.161/webint_editor/templates/editor.html
--rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.161/webint_editor/templates/template.html
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.161/setup.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.161/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-03 07:26:15.676582 webint_editor-0.0.162/pyproject.toml
+-rw-r--r--   0        0        0     4929 2023-06-03 02:55:47.150152 webint_editor-0.0.162/webint_editor/__init__.py
+-rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.162/webint_editor/templates/__init__.py
+-rw-r--r--   0        0        0    17434 2023-06-03 07:26:12.856578 webint_editor-0.0.162/webint_editor/templates/draft.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.162/webint_editor/templates/editor.html
+-rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.162/webint_editor/templates/template.html
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.162/setup.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.162/PKG-INFO
```

### Comparing `webint_editor-0.0.161/pyproject.toml` & `webint_editor-0.0.162/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-editor"
-version = "0.0.161"
+version = "0.0.162"
 description = "Edit posts on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 keywords = ["Micropub"]
 packages = [{include="webint_editor"}]
 
 [tool.poetry.plugins.webapps]
```

### Comparing `webint_editor-0.0.161/webint_editor/__init__.py` & `webint_editor-0.0.162/webint_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_editor-0.0.161/webint_editor/templates/draft.html` & `webint_editor-0.0.162/webint_editor/templates/draft.html`

 * *Files 1% similar despite different names*

```diff
@@ -318,25 +318,24 @@
     // XXX monaco.getValue()
     // return document.querySelector('#content-editor').value
     const request = new XMLHttpRequest()
     request.open("GET", '/pads/p/$pad_id/export/etherpad', false)
     request.send(null);
     if (request.status === 200) {
       const response = JSON.parse(request.responseText)
-      console.log(response)
       return response['pad:$pad_id'].atext.text
     }
   }
 
-  var frequency = 1.5;  // seconds
+  var frequency = 1;  // seconds
   var count = 0;
   var clean = true;
   const tick = () => {
     setTimeout(() => {
-      if (count++ > frequency * 10 && !clean)
+      if (count++ > frequency * 10) // && !clean)
         updatePreview();
       tick();
     }, 100);
   }
   tick();
   const updatePreview = () => {
     clean = false;
```

### Comparing `webint_editor-0.0.161/setup.py` & `webint_editor-0.0.162/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['editor = webint_editor:app']}
 
 setup_kwargs = {
     'name': 'webint-editor',
-    'version': '0.0.161',
+    'version': '0.0.162',
     'description': 'Edit posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

