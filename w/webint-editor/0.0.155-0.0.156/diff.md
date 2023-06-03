# Comparing `tmp/webint_editor-0.0.155.tar.gz` & `tmp/webint_editor-0.0.156.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_editor-0.0.155.tar", max compression
+gzip compressed data, was "webint_editor-0.0.156.tar", max compression
```

## Comparing `webint_editor-0.0.155.tar` & `webint_editor-0.0.156.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      892 2023-02-24 02:05:46.286781 webint_editor-0.0.155/pyproject.toml
--rw-r--r--   0        0        0     4534 2023-01-27 00:43:44.024128 webint_editor-0.0.155/webint_editor/__init__.py
--rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.155/webint_editor/templates/__init__.py
--rw-r--r--   0        0        0    16930 2023-02-21 00:31:31.801886 webint_editor-0.0.155/webint_editor/templates/editor.html
--rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.155/webint_editor/templates/template.html
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.155/setup.py
--rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.155/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-06-03 06:57:04.371558 webint_editor-0.0.156/pyproject.toml
+-rw-r--r--   0        0        0     4929 2023-06-03 02:55:47.150152 webint_editor-0.0.156/webint_editor/__init__.py
+-rw-r--r--   0        0        0      104 2023-01-27 00:43:44.028128 webint_editor-0.0.156/webint_editor/templates/__init__.py
+-rw-r--r--   0        0        0    17245 2023-06-03 06:56:57.015302 webint_editor-0.0.156/webint_editor/templates/draft.html
+-rw-r--r--   0        0        0       44 2023-03-08 03:45:25.484536 webint_editor-0.0.156/webint_editor/templates/editor.html
+-rw-r--r--   0        0        0       54 2023-01-27 00:43:44.024128 webint_editor-0.0.156/webint_editor/templates/template.html
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 webint_editor-0.0.156/setup.py
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 webint_editor-0.0.156/PKG-INFO
```

### Comparing `webint_editor-0.0.155/pyproject.toml` & `webint_editor-0.0.156/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-editor"
-version = "0.0.155"
+version = "0.0.156"
 description = "Edit posts on your website"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "AGPL-3.0-or-later"
 keywords = ["Micropub"]
 packages = [{include="webint_editor"}]
 
 [tool.poetry.plugins.webapps]
```

### Comparing `webint_editor-0.0.155/webint_editor/__init__.py` & `webint_editor-0.0.156/webint_editor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,39 @@
 
 @app.control("")
 class Editor:
     """The editor."""
 
     def get(self):
         """Return the editor."""
+        return app.view.editor()
+
+    def post(self):
+        return "requires javascript"
+        # form = web.form("content")
+        # web.application("understory.posts").model.create(
+        #     "entry", {"content": form.content}
+        # )
+        # return "entry created"
+
+
+@app.control("draft")
+class Draft:
+    """A draft."""
+
+    def get(self):
+        """Return the draft."""
         permalink = web.form(permalink=None).permalink
         post = {}
         if permalink:
             post = web.application("webint_posts").model.read(permalink)["resource"]
         else:
             permalink, _ = web.application("webint_posts").model.create("entry")
-            raise web.SeeOther(f"/editor?permalink={permalink}")
-        return app.view.editor(
+            raise web.SeeOther(f"/editor/draft?permalink={permalink}")
+        return app.view.draft(
             post,
             web.application("webint_owner").model.get_identities(),
             [],  # web.application("webint_guests").model.get_guests(),
         )
 
     def post(self):
         return "requires javascript"
```

### Comparing `webint_editor-0.0.155/webint_editor/templates/editor.html` & `webint_editor-0.0.156/webint_editor/templates/draft.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 $var body_classes = ["widescreen"]
 
 $code:
     def get_property(prop):
         return post.pop(prop, [""])[0]
 
 $ permalink = get_property("url")
+$ pad_id = permalink.lstrip('/').replace('/', '--')
 $var title: Editing $permalink
 $var show_title = False
 $var hide_footer = True
 
 <form id=editor method=post action=$tx.origin/editor>
 <div id=preview>
     <div id=replyContext></div>
@@ -150,15 +151,17 @@
         </div>
         <div id=econtent>
             <label><small>Content</small><br>
             <label class=bounding>
             $# XXX <div id=editor></div>
             $# XXX <div id=editorStatus></div>
             $# TODO FIXME <textarea id=content-editor name=content>$get_property('content')["html"]</textarea>
-            <textarea id=content-editor name=content>$get_property('content')</textarea>
+            <!--textarea id=content-editor name=content>$get_property('content')</textarea-->
+            <iframe src="$tx.origin/pads/p/$pad_id"
+                frameborder=0 style=height:30em;width:100%></iframe>
             </label></label>
             $# XXX <div id=connection></div>
             $# XXX <div id=version></div>
         </div>
     </div>
     <div id=event_properties>
         <div id=name>
@@ -219,27 +222,27 @@
     </div>
 </form>
 
 $if post:
     <pre>$pformat(post)</pre>
 
 <style>
-form {
+form#editor {
   column-gap: 2em;
   display: grid;
   grid-template-columns: auto 30em; }
-input[type=text], textarea {
+form#editor input[type=text], textarea {
   background-color: #ddd;
   border: 0;
   padding: 0;
   width: 100%; }
-textarea {
+form#editor textarea {
   height: 20em;
   width: 100%; }
-input[type=text] {
+form#editor input[type=text] {
   height: 1.5em; }
 #categories ul {
   list-style: none;
   padding-left: 0; }
 .bounding {
   background-color: #ddd;
   border: .1em solid #333;
@@ -309,15 +312,17 @@
   enlivenOptionalProperty('entry', 'name')
   enlivenOptionalProperty('entry', 'summary')
   enlivenOptionalProperty('entry', 'photo')
   enlivenOptionalProperty('entry', 'econtent')
 
   const getContent = () => {
     // XXX monaco.getValue()
-    return document.querySelector('#content-editor').value
+    // return document.querySelector('#content-editor').value
+    const response = await fetch(url)
+    return response.json()['pad:$pad_id'].atext.text
   }
 
   var frequency = 1.5;  // seconds
   var count = 0;
   var clean = true;
   const tick = () => {
     setTimeout(() => {
```

### Comparing `webint_editor-0.0.155/setup.py` & `webint_editor-0.0.156/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['webint>=0.0']
 
 entry_points = \
 {'webapps': ['editor = webint_editor:app']}
 
 setup_kwargs = {
     'name': 'webint-editor',
-    'version': '0.0.155',
+    'version': '0.0.156',
     'description': 'Edit posts on your website',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

