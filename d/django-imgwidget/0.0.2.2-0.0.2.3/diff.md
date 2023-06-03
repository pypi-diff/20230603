# Comparing `tmp/django-imgwidget-0.0.2.2.tar.gz` & `tmp/django-imgwidget-0.0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-imgwidget-0.0.2.2.tar", last modified: Sat Jun  3 07:14:21 2023, max compression
+gzip compressed data, was "django-imgwidget-0.0.2.3.tar", last modified: Sat Jun  3 12:10:19 2023, max compression
```

## Comparing `django-imgwidget-0.0.2.2.tar` & `django-imgwidget-0.0.2.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.930136 django-imgwidget-0.0.2.2/
--rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2.2/MANIFEST.in
--rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 07:14:21.930006 django-imgwidget-0.0.2.2/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)     1747 2023-06-03 04:43:52.000000 django-imgwidget-0.0.2.2/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927404 django-imgwidget-0.0.2.2/django_imguploder/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/admin.py
--rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2.2/django_imguploder/apps.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927599 django-imgwidget-0.0.2.2/django_imguploder/forms/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2.2/django_imguploder/forms/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      871 2023-06-03 05:18:17.000000 django-imgwidget-0.0.2.2/django_imguploder/forms/widget.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927809 django-imgwidget-0.0.2.2/django_imguploder/migrations/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/migrations/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/models.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925678 django-imgwidget-0.0.2.2/django_imguploder/static/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925820 django-imgwidget-0.0.2.2/django_imguploder/static/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927894 django-imgwidget-0.0.2.2/django_imguploder/static/admin/css/
--rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.2.2/django_imguploder/static/admin/css/imgwidget.css
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.928113 django-imgwidget-0.0.2.2/django_imguploder/static/admin/imgs/
--rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2.2/django_imguploder/static/admin/imgs/add.png
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.928338 django-imgwidget-0.0.2.2/django_imguploder/static/admin/js/
--rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2.2/django_imguploder/static/admin/js/jquery.min.js
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925915 django-imgwidget-0.0.2.2/django_imguploder/templates/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925954 django-imgwidget-0.0.2.2/django_imguploder/templates/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.929001 django-imgwidget-0.0.2.2/django_imguploder/templates/admin/widgets/
--rw-r--r--   0 donghao    (501) staff       (20)     6300 2023-06-03 07:14:17.000000 django-imgwidget-0.0.2.2/django_imguploder/templates/admin/widgets/img_multi_upload.html
--rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/tests.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/views.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.929832 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      749 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/not-zip-safe
--rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 07:14:21.930174 django-imgwidget-0.0.2.2/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      878 2023-06-03 07:14:17.000000 django-imgwidget-0.0.2.2/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.705743 django-imgwidget-0.0.2.3/
+-rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2.3/MANIFEST.in
+-rw-r--r--   0 donghao    (501) staff       (20)     2199 2023-06-03 12:10:19.705584 django-imgwidget-0.0.2.3/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)     1772 2023-06-03 07:16:25.000000 django-imgwidget-0.0.2.3/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.702631 django-imgwidget-0.0.2.3/django_imguploder/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.3/django_imguploder/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.3/django_imguploder/admin.py
+-rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2.3/django_imguploder/apps.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.702855 django-imgwidget-0.0.2.3/django_imguploder/forms/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2.3/django_imguploder/forms/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      940 2023-06-03 12:07:49.000000 django-imgwidget-0.0.2.3/django_imguploder/forms/widget.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.703081 django-imgwidget-0.0.2.3/django_imguploder/migrations/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.3/django_imguploder/migrations/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.3/django_imguploder/models.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.700787 django-imgwidget-0.0.2.3/django_imguploder/static/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.700935 django-imgwidget-0.0.2.3/django_imguploder/static/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.703165 django-imgwidget-0.0.2.3/django_imguploder/static/admin/css/
+-rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.2.3/django_imguploder/static/admin/css/imgwidget.css
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.703379 django-imgwidget-0.0.2.3/django_imguploder/static/admin/imgs/
+-rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2.3/django_imguploder/static/admin/imgs/add.png
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.703859 django-imgwidget-0.0.2.3/django_imguploder/static/admin/js/
+-rw-r--r--   0 donghao    (501) staff       (20)     5318 2023-06-03 12:06:56.000000 django-imgwidget-0.0.2.3/django_imguploder/static/admin/js/img_multi_upload.js
+-rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2.3/django_imguploder/static/admin/js/jquery.min.js
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.701032 django-imgwidget-0.0.2.3/django_imguploder/templates/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.701068 django-imgwidget-0.0.2.3/django_imguploder/templates/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.704562 django-imgwidget-0.0.2.3/django_imguploder/templates/admin/widgets/
+-rw-r--r--   0 donghao    (501) staff       (20)     2677 2023-06-03 12:07:49.000000 django-imgwidget-0.0.2.3/django_imguploder/templates/admin/widgets/img_multi_upload.html
+-rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.3/django_imguploder/tests.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.3/django_imguploder/views.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 12:10:19.705408 django-imgwidget-0.0.2.3/django_imgwidget.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)     2199 2023-06-03 12:10:19.000000 django-imgwidget-0.0.2.3/django_imgwidget.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      803 2023-06-03 12:10:19.000000 django-imgwidget-0.0.2.3/django_imgwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 12:10:19.000000 django-imgwidget-0.0.2.3/django_imgwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2.3/django_imgwidget.egg-info/not-zip-safe
+-rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 12:10:19.000000 django-imgwidget-0.0.2.3/django_imgwidget.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 12:10:19.000000 django-imgwidget-0.0.2.3/django_imgwidget.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 12:10:19.705793 django-imgwidget-0.0.2.3/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      878 2023-06-03 12:07:49.000000 django-imgwidget-0.0.2.3/setup.py
```

### Comparing `django-imgwidget-0.0.2.2/PKG-INFO` & `django-imgwidget-0.0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
@@ -16,14 +16,16 @@
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+🐰 图片旋转预览
+
 🌈 效果图片
 
 ![这是图片](example.png "Magic Gardens")
 
 安装
 -----
 `pip install django-imgwidget`
```

### Comparing `django-imgwidget-0.0.2.2/README.md` & `django-imgwidget-0.0.2.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+🐰 图片旋转预览
+
 🌈 效果图片
 
 ![这是图片](example.png "Magic Gardens")
 
 安装
 -----
 `pip install django-imgwidget`
```

### Comparing `django-imgwidget-0.0.2.2/django_imguploder/forms/widget.py` & `django-imgwidget-0.0.2.3/django_imguploder/forms/widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
     class Media:
         css = {
             "all": (
                 "admin/css/imgwidget.css",
             )
         }
+        js = (
+            "admin/js/img_multi_upload.js",
+        )
 
     def render(self, name, value, attrs=None, renderer=None):
         context = self.get_context(name, value, attrs)
         try:
             context["widget"]['widget_img_urls'] = ",".join(json.loads(value))
         except:
             pass
```

### Comparing `django-imgwidget-0.0.2.2/django_imguploder/static/admin/css/imgwidget.css` & `django-imgwidget-0.0.2.3/django_imguploder/static/admin/css/imgwidget.css`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.2/django_imguploder/static/admin/imgs/add.png` & `django-imgwidget-0.0.2.3/django_imguploder/static/admin/imgs/add.png`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.2/django_imguploder/static/admin/js/jquery.min.js` & `django-imgwidget-0.0.2.3/django_imguploder/static/admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.2/django_imgwidget.egg-info/PKG-INFO` & `django-imgwidget-0.0.2.3/django_imgwidget.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
@@ -16,14 +16,16 @@
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+🐰 图片旋转预览
+
 🌈 效果图片
 
 ![这是图片](example.png "Magic Gardens")
 
 安装
 -----
 `pip install django-imgwidget`
```

### Comparing `django-imgwidget-0.0.2.2/django_imgwidget.egg-info/SOURCES.txt` & `django-imgwidget-0.0.2.3/django_imgwidget.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 django_imguploder/tests.py
 django_imguploder/views.py
 django_imguploder/forms/__init__.py
 django_imguploder/forms/widget.py
 django_imguploder/migrations/__init__.py
 django_imguploder/static/admin/css/imgwidget.css
 django_imguploder/static/admin/imgs/add.png
+django_imguploder/static/admin/js/img_multi_upload.js
 django_imguploder/static/admin/js/jquery.min.js
 django_imguploder/templates/admin/widgets/img_multi_upload.html
 django_imgwidget.egg-info/PKG-INFO
 django_imgwidget.egg-info/SOURCES.txt
 django_imgwidget.egg-info/dependency_links.txt
 django_imgwidget.egg-info/not-zip-safe
 django_imgwidget.egg-info/requires.txt
```

### Comparing `django-imgwidget-0.0.2.2/setup.py` & `django-imgwidget-0.0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 long_description = "\n".join([
     open('README.md', 'r', encoding='utf-8').read(),
 ])
 
 NAME = 'django-imgwidget'
-VERSION = '0.0.2.2'
+VERSION = '0.0.2.3'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=()
     ),
```

