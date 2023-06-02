# Comparing `tmp/easel-cli-1.0.5.tar.gz` & `tmp/easel-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easel-cli-1.0.5.tar", last modified: Fri Dec 30 22:12:17 2022, max compression
+gzip compressed data, was "easel-cli-1.1.0.tar", last modified: Fri Jun  2 22:54:52 2023, max compression
```

## Comparing `easel-cli-1.0.5.tar` & `easel-cli-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2022-12-30 22:12:17.069493 easel-cli-1.0.5/
--rw-rw-r--   0 ren       (1000) ren       (1000)    35149 2021-05-25 20:29:14.000000 easel-cli-1.0.5/LICENSE
--rw-rw-r--   0 ren       (1000) ren       (1000)    12476 2022-12-30 22:12:17.069493 easel-cli-1.0.5/PKG-INFO
--rw-rw-r--   0 ren       (1000) ren       (1000)    11988 2022-12-30 21:52:26.000000 easel-cli-1.0.5/README.md
-drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2022-12-30 22:12:17.069493 easel-cli-1.0.5/easel/
--rw-rw-r--   0 ren       (1000) ren       (1000)        0 2021-05-25 20:29:14.000000 easel-cli-1.0.5/easel/__init__.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     3296 2021-12-23 02:25:55.000000 easel-cli-1.0.5/easel/__main__.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     7942 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/assignment.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     1906 2022-12-29 01:56:16.000000 easel-cli-1.0.5/easel/assignment_group.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     1560 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/canvas_id.py
--rw-rw-r--   0 ren       (1000) ren       (1000)    14741 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/commands.py
--rw-rw-r--   0 ren       (1000) ren       (1000)    13294 2022-12-29 01:56:16.000000 easel-cli-1.0.5/easel/component.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     4653 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/course.py
--rw-rw-r--   0 ren       (1000) ren       (1000)      860 2021-12-21 17:09:32.000000 easel-cli-1.0.5/easel/external_tool.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     5249 2021-12-21 17:09:32.000000 easel-cli-1.0.5/easel/files.py
--rw-rw-r--   0 ren       (1000) ren       (1000)      831 2021-12-21 22:23:01.000000 easel-cli-1.0.5/easel/grading_scheme.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     7021 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/helpers.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     2746 2022-12-29 01:56:16.000000 easel-cli-1.0.5/easel/helpers_yaml.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     8831 2022-12-29 01:56:16.000000 easel-cli-1.0.5/easel/module.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     4978 2021-12-21 17:09:32.000000 easel-cli-1.0.5/easel/module_item.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     5047 2022-08-17 20:54:23.000000 easel-cli-1.0.5/easel/navigation_tab.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     2730 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/page.py
--rw-rw-r--   0 ren       (1000) ren       (1000)    15704 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/quiz.py
--rw-rw-r--   0 ren       (1000) ren       (1000)     5033 2022-12-30 21:26:27.000000 easel-cli-1.0.5/easel/quiz_question.py
-drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2022-12-30 22:12:17.069493 easel-cli-1.0.5/easel_cli.egg-info/
--rw-rw-r--   0 ren       (1000) ren       (1000)    12476 2022-12-30 22:12:17.000000 easel-cli-1.0.5/easel_cli.egg-info/PKG-INFO
--rw-rw-r--   0 ren       (1000) ren       (1000)      593 2022-12-30 22:12:17.000000 easel-cli-1.0.5/easel_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 ren       (1000) ren       (1000)        1 2022-12-30 22:12:17.000000 easel-cli-1.0.5/easel_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 ren       (1000) ren       (1000)       47 2022-12-30 22:12:17.000000 easel-cli-1.0.5/easel_cli.egg-info/entry_points.txt
--rw-rw-r--   0 ren       (1000) ren       (1000)       61 2022-12-30 22:12:17.000000 easel-cli-1.0.5/easel_cli.egg-info/requires.txt
--rw-rw-r--   0 ren       (1000) ren       (1000)        6 2022-12-30 22:12:17.000000 easel-cli-1.0.5/easel_cli.egg-info/top_level.txt
--rw-rw-r--   0 ren       (1000) ren       (1000)       38 2022-12-30 22:12:17.069493 easel-cli-1.0.5/setup.cfg
--rw-rw-r--   0 ren       (1000) ren       (1000)      898 2022-12-30 22:00:26.000000 easel-cli-1.0.5/setup.py
+drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2023-06-02 22:54:52.760911 easel-cli-1.1.0/
+-rw-rw-r--   0 ren       (1000) ren       (1000)    35149 2021-01-02 17:06:05.000000 easel-cli-1.1.0/LICENSE
+-rw-rw-r--   0 ren       (1000) ren       (1000)    12476 2023-06-02 22:54:52.760911 easel-cli-1.1.0/PKG-INFO
+-rw-rw-r--   0 ren       (1000) ren       (1000)    11988 2023-06-02 22:53:58.000000 easel-cli-1.1.0/README.md
+drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2023-06-02 22:54:52.760911 easel-cli-1.1.0/easel/
+-rw-rw-r--   0 ren       (1000) ren       (1000)        0 2021-01-04 17:58:25.000000 easel-cli-1.1.0/easel/__init__.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     3296 2022-01-11 01:25:26.000000 easel-cli-1.1.0/easel/__main__.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     8244 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/assignment.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     1954 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/assignment_group.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     1799 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/canvas_id.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)    14901 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/commands.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)    13294 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/component.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     6204 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/course.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)      860 2021-12-20 23:38:30.000000 easel-cli-1.1.0/easel/external_tool.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     5249 2021-12-20 23:38:30.000000 easel-cli-1.1.0/easel/files.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)      831 2022-01-11 01:25:26.000000 easel-cli-1.1.0/easel/grading_scheme.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     8526 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/helpers.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     2746 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/helpers_yaml.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     8829 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/module.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     4978 2021-12-20 23:38:30.000000 easel-cli-1.1.0/easel/module_item.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     5047 2022-01-11 01:25:26.000000 easel-cli-1.1.0/easel/navigation_tab.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     3049 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/page.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)    15998 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/quiz.py
+-rw-rw-r--   0 ren       (1000) ren       (1000)     5397 2023-06-02 22:53:58.000000 easel-cli-1.1.0/easel/quiz_question.py
+drwxrwxr-x   0 ren       (1000) ren       (1000)        0 2023-06-02 22:54:52.760911 easel-cli-1.1.0/easel_cli.egg-info/
+-rw-rw-r--   0 ren       (1000) ren       (1000)    12476 2023-06-02 22:54:52.000000 easel-cli-1.1.0/easel_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 ren       (1000) ren       (1000)      593 2023-06-02 22:54:52.000000 easel-cli-1.1.0/easel_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 ren       (1000) ren       (1000)        1 2023-06-02 22:54:52.000000 easel-cli-1.1.0/easel_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 ren       (1000) ren       (1000)       47 2023-06-02 22:54:52.000000 easel-cli-1.1.0/easel_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 ren       (1000) ren       (1000)       61 2023-06-02 22:54:52.000000 easel-cli-1.1.0/easel_cli.egg-info/requires.txt
+-rw-rw-r--   0 ren       (1000) ren       (1000)        6 2023-06-02 22:54:52.000000 easel-cli-1.1.0/easel_cli.egg-info/top_level.txt
+-rw-rw-r--   0 ren       (1000) ren       (1000)       38 2023-06-02 22:54:52.760911 easel-cli-1.1.0/setup.cfg
+-rw-rw-r--   0 ren       (1000) ren       (1000)      898 2023-06-02 22:54:07.000000 easel-cli-1.1.0/setup.py
```

### Comparing `easel-cli-1.0.5/LICENSE` & `easel-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/PKG-INFO` & `easel-cli-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easel-cli
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Canvas course management tool
 Home-page: https://github.com/renquinn/easel-py
 Author: Ren Quinn
 Author-email: renquinn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easel-cli-1.0.5/README.md` & `easel-cli-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/__main__.py` & `easel-cli-1.1.0/easel/__main__.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/assignment.py` & `easel-cli-1.1.0/easel/assignment.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,18 +73,26 @@
                 raise ValueError(f"failed to find AssignmentGroup called '{self.assignment_group}'")
             # assumes assignment group names will be unique
             fname = assignment_group_.AssignmentGroup(**dict(results[0])).filename
             cid = canvas_id.CanvasID(fname, course_id)
             cid.find_id(db)
             self.assignment_group_id = cid.canvas_id
 
+    def md(self, db, course_):
+        if self.description:
+            fields = helpers.get_global_template_fields()
+            course_fields = helpers.get_course_template_fields(db, course_)
+            fields.update(course_fields)
+            return helpers.md2html(self.description.strip(), fields)
+        return ''
+
     def preprocess(self, db, course_, dry_run):
         self.get_assignment_group_id(db, course_.canvas_id)
         if self.description:
-            self.description = helpers.md2html(self.description.strip())
+            self.description = self.md(db, course_)
 
     # TODO: originally, pulling a new component vs pulling an existing one to
     # update it was a different operation. Since then, I've added extra
     # processing to some of the operations for pulling a new component that I
     # need to use that for updating now, which is why I wrote this function.
     # Seems like this could use a better design to reuse some of the
     # functionality while taking advantage of inheriting from the Component
```

### Comparing `easel-cli-1.0.5/easel/assignment_group.py` & `easel-cli-1.1.0/easel/assignment_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         if cid:
             ag['filename'] = cid.filename
         else:
             ag['filename'] = component.gen_filename(ASSIGN_GROUPS_DIR, ag.get('name',''))
             cid = canvas_id.CanvasID(ag['filename'], course_.canvas_id)
             cid.canvas_id = ag.get('id')
             cid.save(db)
-        ags.append(AssignmentGroup.build(ag))
+        new_ag = AssignmentGroup.build(ag)
+        new_ag.save(db)
+        ags.append(new_ag)
     return ags
 
 # Needed for custom yaml tag
 def constructor(loader, node):
     fields = helpers_yaml.construct_ordered_mapping(loader, node)
     return AssignmentGroup(**fields)
```

### Comparing `easel-cli-1.0.5/easel/canvas_id.py` & `easel-cli-1.1.0/easel/canvas_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,7 +43,15 @@
 def find_by_prefix(db, course_id, prefix):
     table = db.table(TABLE)
     CID = tinydb.Query()
     results = table.search((CID.filename.matches("^"+prefix)) & (CID.course_id == course_id))
     for result in results:
         if result:
             yield CanvasID(**result)
+
+def find_all_course_components(db, course_id):
+    table = db.table(TABLE)
+    CID = tinydb.Query()
+    results = table.search(CID.course_id == course_id)
+    for result in results:
+        if result:
+            yield CanvasID(**result)
```

### Comparing `easel-cli-1.0.5/easel/commands.py` & `easel-cli-1.1.0/easel/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -305,37 +305,39 @@
                     else:
                         # not a yaml file so assume it's a file/dir to upload
                         files.push(db, course_, component_filepath,
                                 args.hidden, args.dry_run)
 
 def cmd_md(db, args):
     if not args.components:
-        args.components = ["syllabus.md", "assignment_groups", "assignments",
-                "files", "pages", "quizzes", "modules"]
+        args.components = ["syllabus.md", "assignments", "pages", "quizzes"]
 
+    courses = course.find_all(db)
     for component_filepath in args.components:
         if component_filepath.endswith("*"):
             component_filepath = component_filepath[:-1]
         if component_filepath.endswith("/"):
             component_filepath = component_filepath[:-1]
 
         if os.path.isdir(component_filepath) and not component_filepath.startswith("files"):
             if component_filepath not in helpers.DIRS:
                 logging.error("Invalid directory: "+component_filepath)
                 continue
 
-            for child_path in os.listdir(component_filepath):
-                full_child_path = component_filepath + '/' + child_path
-                component = helpers_yaml.read(full_child_path)
-                print(component.md())
+            for course_ in courses:
+                for child_path in os.listdir(component_filepath):
+                    full_child_path = component_filepath + '/' + child_path
+                    component = helpers_yaml.read(full_child_path)
+                    print(component.md(db, course_))
         else:
             if component_filepath == "syllabus.md":
-                f = open("syllabus.md")
-                print(helpers.md2html(f.read()))
-                f.close()
+                for course_ in courses:
+                    print(course.format_syllabus(db, course_.canvas_id))
             else:
                 component = helpers_yaml.read(component_filepath)
                 if isinstance(component, list):
-                    for obj in component:
-                        print("\n\n*****\n", obj.md())
+                    for course_ in courses:
+                        for obj in component:
+                            print("\n\n*****\n", obj.md(db, course_))
                 else:
-                    print(component.md())
+                    for course_ in courses:
+                        print(component.md(db, course_))
```

### Comparing `easel-cli-1.0.5/easel/component.py` & `easel-cli-1.1.0/easel/component.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/external_tool.py` & `easel-cli-1.1.0/easel/external_tool.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/files.py` & `easel-cli-1.1.0/easel/files.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/grading_scheme.py` & `easel-cli-1.1.0/easel/grading_scheme.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/helpers.py` & `easel-cli-1.1.0/easel/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import re
 from tqdm import tqdm
 import urllib.parse
 
 import markdown
 import requests
 import tinydb
+import yaml
 
+from easel import canvas_id
 
 API="/api/v1"
 HTTPS="https://"
 DIRS = { # maps a directory name to its easel module name
         "assignment_groups": "assignment_group",
         "assignments": "assignment",
         "external_tools": "external_tool",
@@ -22,14 +24,48 @@
         "modules": "module",
         "pages": "page",
         "quiz_questions": "quiz_question",
         "quizzes": "quiz",
         "local": "",
         }
 
+def get_course_template_fields(db, course_):
+    '''Take a course and produce relevant info to be formatted into the
+    markdown of various components (e.g., syllabus, pages, assignment
+    descriptions). TODO: At some point there may be a collision with an
+    assignment name and the course info key names (e.g., an assignment named
+    "semester").'''
+    fields = {}
+
+    # 1. course info
+    # NOTE: Canvas may change the format of these fields in the future
+    fields['code'] = course_.code[:7]
+    fields['crn'] = course_.name[-6:-1]
+    fields['semester'] = ' '.join(course_.name.split()[1:3])
+    fields["course_id"] = course_.canvas_id
+
+    # 2. all assignment/quiz ids ("{root_filename}" => canvas_id)
+    # root_filename: w/o parent dirs and extension
+    for cid in canvas_id.find_all_course_components(db, course_.canvas_id):
+        if '/' in cid.filename:
+            filename = cid.filename.split('/')[1].split('.')[0]
+            fields[filename] = cid.canvas_id
+
+    return fields
+
+def get_global_template_fields():
+    '''Produce custom info from template_fields.yaml to be formatted into the
+    markdown of various components (e.g., syllabus, pages, assignment
+    descriptions)'''
+    template_fields_fname = "template_fields.yaml"
+    if os.path.isfile(template_fields_fname):
+        with open(template_fields_fname) as f:
+            return yaml.load(f, Loader=yaml.FullLoader)
+    return {}
+
 def isurl(url):
     # requires protocol in addition to hostname
     try:
         parsed = urllib.parse.urlparse(url)
         return all([parsed.scheme, parsed.netloc])
     except:
         return False
@@ -46,17 +82,18 @@
             html = html.replace(lt, '')
     scripttags = re.findall("<script.*?><\/script>", html)
     for st in scripttags:
         if 'canvas_global_app' in st:
             html = html.replace(st, '')
     return html
 
-def md2html(mdtext):
+def md2html(mdtext, args={}):
     extensions = ['fenced_code', 'codehilite', 'tables', 'attr_list']
     config = {'codehilite': {'noclasses': True}}
+    mdtext = mdtext.format(**args)
     return markdown.markdown(mdtext, extensions=extensions,
             extension_configs=config)
 
 def write_config(hostname, token, dry_run):
     home = Path.home()
     if home == "":
         raise ValueError("home directory is not set")
```

### Comparing `easel-cli-1.0.5/easel/helpers_yaml.py` & `easel-cli-1.1.0/easel/helpers_yaml.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/module.py` & `easel-cli-1.1.0/easel/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 MODULES_DIR="modules"
 WRAPPER="module"
 
 class Module(component.Component):
 
     def __init__(self, name=None, published=None, position=None,
             unlock_at=None, require_sequential_progress=None,
-            prerequisite_module_ids=None, items=None, filename="",
+            prerequisite_module_ids=None, items=[], filename="",
             yaml_order=[]):
         super().__init__(create_path=MODULES_PATH, update_path=MODULE_PATH,
                 db_table=MODULES_TABLE, canvas_wrapper=WRAPPER,
                 filename=filename, yaml_order=yaml_order)
         self.name = name
         self.published = published
         self.position = position
```

### Comparing `easel-cli-1.0.5/easel/module_item.py` & `easel-cli-1.1.0/easel/module_item.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/navigation_tab.py` & `easel-cli-1.1.0/easel/navigation_tab.py`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/easel/page.py` & `easel-cli-1.1.0/easel/page.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,30 @@
         self.student_todo_at = todo_date
         if student_todo_at:
             self.student_todo_at = student_todo_at
         self.editing_roles = editing_roles
         self.notify_of_update = notify_of_update
         self.body = body
 
-    def preprocess(self, db, course_, dry_run):
+    def md(self, db, course_):
         if self.body:
-            self.body = helpers.md2html(self.body.strip())
+            body = self.body
+            fields = helpers.get_global_template_fields()
+            course_fields = helpers.get_course_template_fields(db, course_)
+            fields.update(course_fields)
+            return helpers.md2html(body.strip(), fields)
+        return ''
 
     def __repr__(self):
         return f"Page(title={self.title}, published={self.published})"
 
+    def preprocess(self, db, course_, dry_run):
+        if self.body:
+            self.body = self.md(db, course_)
+
     @classmethod
     def build(cls, fields):
         defaults = {
                 "front_page": False,
                 "editing_roles": "teachers",
                 }
         desired_fields = cls.__init__.__code__.co_varnames[1:]
```

### Comparing `easel-cli-1.0.5/easel/quiz.py` & `easel-cli-1.1.0/easel/quiz.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,17 +170,25 @@
                 raise ValueError(f"failed to find AssignmentGroup called '{self.assignment_group}'")
             # assumes assignment group names will be unique
             fname = assignment_group.AssignmentGroup(**dict(results[0])).filename
             cid = canvas_id.CanvasID(fname, course_id)
             cid.find_id(db)
             self.assignment_group_id = cid.canvas_id
 
+    def md(self, db, course_):
+        if self.description:
+            fields = helpers.get_global_template_fields()
+            course_fields = helpers.get_course_template_fields(db, course_)
+            fields.update(course_fields)
+            return helpers.md2html(self.description.strip())
+        return ''
+
     def preprocess(self, db, course_, dry_run):
         if self.description:
-            self.description = helpers.md2html(self.description.strip())
+            self.description = self.md(db, course_)
         self.get_assignment_group_id(db, course_.canvas_id)
         self.remember_published = self.published
         self.published = False
 
     def postprocess(self, db, course_, dry_run):
         course_id = course_.canvas_id
         cid = canvas_id.CanvasID(self.filename, course_id)
```

### Comparing `easel-cli-1.0.5/easel/quiz_question.py` & `easel-cli-1.1.0/easel/quiz_question.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,15 +79,20 @@
 
     def __repr__(self):
         return f"QuizQuestion(id={self.id}, question_name={self.question_name}, " \
                 f"question_type={self.question_type}, " \
                 f"points_possible={self.points_possible}, "\
                 f"answers_count={len(self.answers)})"
 
-    def md(self):
+    def md(self, db, course_):
+        '''TODO: was originally meant for debugging only, but now I'm using it
+        in other components as the operation used for converting markdown to
+        html in potentially multiple places. QuizQuestion is the only component
+        that needs a custom display for debugging so I need to think through a
+        different approach here.'''
         out = self.question_text
         for answer in self.answers:
             for key in ['answer_html', 'answer_text']:
                 if key in answer:
                     out += "\n- A: " + answer[key]
         return out
```

### Comparing `easel-cli-1.0.5/easel_cli.egg-info/PKG-INFO` & `easel-cli-1.1.0/easel_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easel-cli
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Canvas course management tool
 Home-page: https://github.com/renquinn/easel-py
 Author: Ren Quinn
 Author-email: renquinn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easel-cli-1.0.5/easel_cli.egg-info/SOURCES.txt` & `easel-cli-1.1.0/easel_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easel-cli-1.0.5/setup.py` & `easel-cli-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read().splitlines()
 
 setuptools.setup(
     name="easel-cli",
-    version="1.0.5",
+    version="1.1.0",
     author="Ren Quinn",
     author_email="renquinn@gmail.com",
     description="A Canvas course management tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/renquinn/easel-py",
     install_requires=install_requires,
```

