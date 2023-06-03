# Comparing `tmp/webint_editor-0.0.158.tar.gz` & `tmp/webint_editor-0.0.159.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_editor-0.0.158.tar", max compression
+gzip compressed data, was "webint_editor-0.0.159.tar", max compression
```

## Comparing `webint_editor-0.0.158.tar` & `webint_editor-0.0.159.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      892 2023-06-03 07:09:27.296511 webint_editor-0.0.158/pyproject.toml
--rw-r--r--   0        0        0     4929 2023-06-03 02:55:47.150152 webint_editor-0.0.158/webint_editor/__init__.py
--rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.158/webint_editor/templates/__init__.py
--rw-r--r--   0        0        0    17455 2023-06-03 07:09:24.940454 webint_editor-0.0.158/webint_editor/templates/draft.html
--rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.158/webint_editor/templates/editor.html
--rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.158/webint_editor/templates/template.html
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.158/setup.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.158/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-03 07:13:45.646566 webint_editor-0.0.159/pyproject.toml
+-rw-r--r--   0        0        0     4929 2023-06-03 02:55:47.150152 webint_editor-0.0.159/webint_editor/__init__.py
+-rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.159/webint_editor/templates/__init__.py
+-rw-r--r--   0        0        0    17490 2023-06-03 07:13:40.086439 webint_editor-0.0.159/webint_editor/templates/draft.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.159/webint_editor/templates/editor.html
+-rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.159/webint_editor/templates/template.html
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.159/setup.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.159/PKG-INFO
```

### Comparing `webint_editor-0.0.158/pyproject.toml` & `webint_editor-0.0.159/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-editor"
-version = "0.0.158"
+version = "0.0.159"
 description = "Edit posts on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 keywords = ["Micropub"]
 packages = [{include="webint_editor"}]
 
 [tool.poetry.plugins.webapps]
```

### Comparing `webint_editor-0.0.158/webint_editor/__init__.py` & `webint_editor-0.0.159/webint_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `webint_editor-0.0.158/webint_editor/templates/draft.html` & `webint_editor-0.0.159/webint_editor/templates/draft.html`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,15 @@
 
   const getContent = () => {
     // XXX monaco.getValue()
     // return document.querySelector('#content-editor').value
     const request = new XMLHttpRequest()
     request.open("GET", '/pads/p/$pad_id/export/etherpad', false)
     request.send(null);
+    console.log(request.status)
     if (request.status === 200) {
       response = JSON.stringify(request.responseText)
       console.log(response)
       return response['pad:$pad_id'].atext.text
     }
   }
 
@@ -370,15 +371,15 @@
   $#   $#   },
   $#   $#   '$(tx.user.session["uid"][0] if tx.user.session else tx.user.ip)',
   $#   $#   true
   $#   $# )
   $#   $# monaco.onKeyUp(updatePreview)
   $# })
 
-  document.querySelector('#content-editor').addEventListener('keyup', updatePreview)
+  // document.querySelector('#content-editor').addEventListener('keyup', updatePreview)
   document.querySelector('#in_reply_to input[type=text]').addEventListener('blur', ev => {
     previewReplyContext(ev.target.value)
   })
 
   addEventListener('beforeunload', ev => {
     ev.stopPropagation()
     ev.preventDefault()
```

### Comparing `webint_editor-0.0.158/setup.py` & `webint_editor-0.0.159/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['editor = webint_editor:app']}
 
 setup_kwargs = {
     'name': 'webint-editor',
-    'version': '0.0.158',
+    'version': '0.0.159',
     'description': 'Edit posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

