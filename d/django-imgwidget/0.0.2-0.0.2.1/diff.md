# Comparing `tmp/django-imgwidget-0.0.2.tar.gz` & `tmp/django-imgwidget-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-imgwidget-0.0.2.tar", last modified: Sat Jun  3 04:38:17 2023, max compression
+gzip compressed data, was "django-imgwidget-0.0.2.1.tar", last modified: Sat Jun  3 05:18:39 2023, max compression
```

## Comparing `django-imgwidget-0.0.2.tar` & `django-imgwidget-0.0.2.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.071663 django-imgwidget-0.0.2/
--rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2/MANIFEST.in
--rw-r--r--   0 donghao    (501) staff       (20)     2107 2023-06-03 04:38:17.071523 django-imgwidget-0.0.2/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)     1682 2023-06-03 04:35:42.000000 django-imgwidget-0.0.2/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068310 django-imgwidget-0.0.2/django_imguploder/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/admin.py
--rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2/django_imguploder/apps.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068525 django-imgwidget-0.0.2/django_imguploder/forms/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2/django_imguploder/forms/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      865 2023-06-03 04:00:39.000000 django-imgwidget-0.0.2/django_imguploder/forms/widget.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068768 django-imgwidget-0.0.2/django_imguploder/migrations/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/migrations/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/models.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.065878 django-imgwidget-0.0.2/django_imguploder/static/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068851 django-imgwidget-0.0.2/django_imguploder/static/css/
--rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.2/django_imguploder/static/css/imgwidget.css
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.069143 django-imgwidget-0.0.2/django_imguploder/static/imgs/
--rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2/django_imguploder/static/imgs/add.png
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.069416 django-imgwidget-0.0.2/django_imguploder/static/js/
--rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2/django_imguploder/static/js/jquery.min.js
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.065974 django-imgwidget-0.0.2/django_imguploder/templates/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.066011 django-imgwidget-0.0.2/django_imguploder/templates/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.070260 django-imgwidget-0.0.2/django_imguploder/templates/admin/widgets/
--rw-r--r--   0 donghao    (501) staff       (20)     5778 2023-06-03 03:38:18.000000 django-imgwidget-0.0.2/django_imguploder/templates/admin/widgets/img_multi_upload.html
--rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/tests.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/views.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.071301 django-imgwidget-0.0.2/django_imgwidget.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)     2107 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      731 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/not-zip-safe
--rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 04:38:17.071704 django-imgwidget-0.0.2/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      876 2023-06-03 04:36:48.000000 django-imgwidget-0.0.2/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.565789 django-imgwidget-0.0.2.1/
+-rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2.1/MANIFEST.in
+-rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 05:18:39.565623 django-imgwidget-0.0.2.1/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)     1747 2023-06-03 04:43:52.000000 django-imgwidget-0.0.2.1/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.562956 django-imgwidget-0.0.2.1/django_imguploder/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/admin.py
+-rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2.1/django_imguploder/apps.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563177 django-imgwidget-0.0.2.1/django_imguploder/forms/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2.1/django_imguploder/forms/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      871 2023-06-03 05:18:17.000000 django-imgwidget-0.0.2.1/django_imguploder/forms/widget.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563406 django-imgwidget-0.0.2.1/django_imguploder/migrations/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/migrations/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/models.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561152 django-imgwidget-0.0.2.1/django_imguploder/static/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561298 django-imgwidget-0.0.2.1/django_imguploder/static/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563490 django-imgwidget-0.0.2.1/django_imguploder/static/admin/css/
+-rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.2.1/django_imguploder/static/admin/css/imgwidget.css
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563729 django-imgwidget-0.0.2.1/django_imguploder/static/admin/imgs/
+-rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2.1/django_imguploder/static/admin/imgs/add.png
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563976 django-imgwidget-0.0.2.1/django_imguploder/static/admin/js/
+-rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2.1/django_imguploder/static/admin/js/jquery.min.js
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561396 django-imgwidget-0.0.2.1/django_imguploder/templates/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561434 django-imgwidget-0.0.2.1/django_imguploder/templates/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.564645 django-imgwidget-0.0.2.1/django_imguploder/templates/admin/widgets/
+-rw-r--r--   0 donghao    (501) staff       (20)     5790 2023-06-03 05:18:17.000000 django-imgwidget-0.0.2.1/django_imguploder/templates/admin/widgets/img_multi_upload.html
+-rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/tests.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/views.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.565464 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      749 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/not-zip-safe
+-rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 05:18:39.565838 django-imgwidget-0.0.2.1/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      878 2023-06-03 05:18:38.000000 django-imgwidget-0.0.2.1/setup.py
```

### Comparing `django-imgwidget-0.0.2/PKG-INFO` & `django-imgwidget-0.0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
@@ -16,14 +16,18 @@
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+🌈 效果图片
+
+![这是图片](example.png "Magic Gardens")
+
 安装
 -----
 `pip install django-imgwidget`
 
 `主页: https://pypi.org/project/django-imgwidget`
 
 步骤
```

### Comparing `django-imgwidget-0.0.2/README.md` & `django-imgwidget-0.0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+🌈 效果图片
+
+![这是图片](example.png "Magic Gardens")
+
 安装
 -----
 `pip install django-imgwidget`
 
 `主页: https://pypi.org/project/django-imgwidget`
 
 步骤
```

### Comparing `django-imgwidget-0.0.2/django_imguploder/forms/widget.py` & `django-imgwidget-0.0.2.1/django_imguploder/forms/widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class MultiImagesInputWidget(Input):
     template_name = 'admin/widgets/img_multi_upload.html'
     input_type = "file"
 
     class Media:
         css = {
             "all": (
-                "css/imgwidget.css",
+                "admin/css/imgwidget.css",
             )
         }
 
     def render(self, name, value, attrs=None, renderer=None):
         context = self.get_context(name, value, attrs)
         try:
             context["widget"]['widget_img_urls'] = ",".join(json.loads(value))
```

### Comparing `django-imgwidget-0.0.2/django_imguploder/static/css/imgwidget.css` & `django-imgwidget-0.0.2.1/django_imguploder/static/admin/css/imgwidget.css`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2/django_imguploder/static/imgs/add.png` & `django-imgwidget-0.0.2.1/django_imguploder/static/admin/imgs/add.png`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2/django_imguploder/static/js/jquery.min.js` & `django-imgwidget-0.0.2.1/django_imguploder/static/admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2/django_imguploder/templates/admin/widgets/img_multi_upload.html` & `django-imgwidget-0.0.2.1/django_imguploder/templates/admin/widgets/img_multi_upload.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load static %}
 <html>
 <head>
-    <script src="{% static 'js/jquery.min.js' %}"></script>
+    <script src="{% static 'admin/js/jquery.min.js' %}"></script>
 </head>
 <body>
 <div class="file-button" id="upload_image_{{ widget.name }}"
-     style="background-image:  url('{% static 'imgs/add.png' %}');">
+     style="background-image:  url('{% static 'admin/imgs/add.png' %}');">
     <input type="{{ widget.type }}"
            data-widgetname="{{ widget.name }}"
            onchange="uploadImage(this)"
            accept="image/*"
            multiple>
     <textarea id="{{ widget.name }}" name="{{ widget.name }}" style="display: none"></textarea>
     <div id="outerdiv" class="big-img-box">
```

### Comparing `django-imgwidget-0.0.2/django_imgwidget.egg-info/PKG-INFO` & `django-imgwidget-0.0.2.1/django_imgwidget.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
@@ -16,14 +16,18 @@
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+🌈 效果图片
+
+![这是图片](example.png "Magic Gardens")
+
 安装
 -----
 `pip install django-imgwidget`
 
 `主页: https://pypi.org/project/django-imgwidget`
 
 步骤
```

### Comparing `django-imgwidget-0.0.2/django_imgwidget.egg-info/SOURCES.txt` & `django-imgwidget-0.0.2.1/django_imgwidget.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 django_imguploder/apps.py
 django_imguploder/models.py
 django_imguploder/tests.py
 django_imguploder/views.py
 django_imguploder/forms/__init__.py
 django_imguploder/forms/widget.py
 django_imguploder/migrations/__init__.py
-django_imguploder/static/css/imgwidget.css
-django_imguploder/static/imgs/add.png
-django_imguploder/static/js/jquery.min.js
+django_imguploder/static/admin/css/imgwidget.css
+django_imguploder/static/admin/imgs/add.png
+django_imguploder/static/admin/js/jquery.min.js
 django_imguploder/templates/admin/widgets/img_multi_upload.html
 django_imgwidget.egg-info/PKG-INFO
 django_imgwidget.egg-info/SOURCES.txt
 django_imgwidget.egg-info/dependency_links.txt
 django_imgwidget.egg-info/not-zip-safe
 django_imgwidget.egg-info/requires.txt
 django_imgwidget.egg-info/top_level.txt
```

### Comparing `django-imgwidget-0.0.2/setup.py` & `django-imgwidget-0.0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 long_description = "\n".join([
     open('README.md', 'r', encoding='utf-8').read(),
 ])
 
 NAME = 'django-imgwidget'
-VERSION = '0.0.2'
+VERSION = '0.0.2.1'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=()
     ),
```

