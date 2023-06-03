# Comparing `tmp/django-imgwidget-0.0.1.tar.gz` & `tmp/django-imgwidget-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-imgwidget-0.0.1.tar", last modified: Sat Jun  3 04:33:57 2023, max compression
+gzip compressed data, was "django-imgwidget-0.0.2.tar", last modified: Sat Jun  3 04:38:17 2023, max compression
```

## Comparing `django-imgwidget-0.0.1.tar` & `django-imgwidget-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.207205 django-imgwidget-0.0.1/
--rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.1/MANIFEST.in
--rw-r--r--   0 donghao    (501) staff       (20)     2001 2023-06-03 04:33:57.207044 django-imgwidget-0.0.1/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)     1585 2023-06-03 03:51:37.000000 django-imgwidget-0.0.1/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.202109 django-imgwidget-0.0.1/django_imguploder/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.1/django_imguploder/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.1/django_imguploder/admin.py
--rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.1/django_imguploder/apps.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.202311 django-imgwidget-0.0.1/django_imguploder/forms/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.1/django_imguploder/forms/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      865 2023-06-03 04:00:39.000000 django-imgwidget-0.0.1/django_imguploder/forms/widget.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.202522 django-imgwidget-0.0.1/django_imguploder/migrations/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.1/django_imguploder/migrations/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.1/django_imguploder/models.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.200319 django-imgwidget-0.0.1/django_imguploder/static/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.202598 django-imgwidget-0.0.1/django_imguploder/static/css/
--rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.1/django_imguploder/static/css/imgwidget.css
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.203853 django-imgwidget-0.0.1/django_imguploder/static/imgs/
--rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.1/django_imguploder/static/imgs/add.png
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.204134 django-imgwidget-0.0.1/django_imguploder/static/js/
--rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.1/django_imguploder/static/js/jquery.min.js
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.200412 django-imgwidget-0.0.1/django_imguploder/templates/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.200448 django-imgwidget-0.0.1/django_imguploder/templates/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.204812 django-imgwidget-0.0.1/django_imguploder/templates/admin/widgets/
--rw-r--r--   0 donghao    (501) staff       (20)     5778 2023-06-03 03:38:18.000000 django-imgwidget-0.0.1/django_imguploder/templates/admin/widgets/img_multi_upload.html
--rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.1/django_imguploder/tests.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.1/django_imguploder/views.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:33:57.206749 django-imgwidget-0.0.1/django_imgwidget.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)     2001 2023-06-03 04:33:57.000000 django-imgwidget-0.0.1/django_imgwidget.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      731 2023-06-03 04:33:57.000000 django-imgwidget-0.0.1/django_imgwidget.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 04:33:57.000000 django-imgwidget-0.0.1/django_imgwidget.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.1/django_imgwidget.egg-info/not-zip-safe
--rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 04:33:57.000000 django-imgwidget-0.0.1/django_imgwidget.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 04:33:57.000000 django-imgwidget-0.0.1/django_imgwidget.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 04:33:57.207320 django-imgwidget-0.0.1/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      867 2023-06-03 04:33:51.000000 django-imgwidget-0.0.1/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.071663 django-imgwidget-0.0.2/
+-rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2/MANIFEST.in
+-rw-r--r--   0 donghao    (501) staff       (20)     2107 2023-06-03 04:38:17.071523 django-imgwidget-0.0.2/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)     1682 2023-06-03 04:35:42.000000 django-imgwidget-0.0.2/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068310 django-imgwidget-0.0.2/django_imguploder/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/admin.py
+-rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2/django_imguploder/apps.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068525 django-imgwidget-0.0.2/django_imguploder/forms/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2/django_imguploder/forms/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      865 2023-06-03 04:00:39.000000 django-imgwidget-0.0.2/django_imguploder/forms/widget.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068768 django-imgwidget-0.0.2/django_imguploder/migrations/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/migrations/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/models.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.065878 django-imgwidget-0.0.2/django_imguploder/static/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.068851 django-imgwidget-0.0.2/django_imguploder/static/css/
+-rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.2/django_imguploder/static/css/imgwidget.css
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.069143 django-imgwidget-0.0.2/django_imguploder/static/imgs/
+-rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2/django_imguploder/static/imgs/add.png
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.069416 django-imgwidget-0.0.2/django_imguploder/static/js/
+-rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2/django_imguploder/static/js/jquery.min.js
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.065974 django-imgwidget-0.0.2/django_imguploder/templates/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.066011 django-imgwidget-0.0.2/django_imguploder/templates/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.070260 django-imgwidget-0.0.2/django_imguploder/templates/admin/widgets/
+-rw-r--r--   0 donghao    (501) staff       (20)     5778 2023-06-03 03:38:18.000000 django-imgwidget-0.0.2/django_imguploder/templates/admin/widgets/img_multi_upload.html
+-rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/tests.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2/django_imguploder/views.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 04:38:17.071301 django-imgwidget-0.0.2/django_imgwidget.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)     2107 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      731 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/not-zip-safe
+-rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 04:38:17.000000 django-imgwidget-0.0.2/django_imgwidget.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 04:38:17.071704 django-imgwidget-0.0.2/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      876 2023-06-03 04:36:48.000000 django-imgwidget-0.0.2/setup.py
```

### Comparing `django-imgwidget-0.0.1/PKG-INFO` & `django-imgwidget-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,20 @@
-Metadata-Version: 2.1
-Name: django-imgwidget
-Version: 0.0.1
-Summary: 上传图片组件
-Home-page: https://github.com/RelaxedDong/simpleui
-Author: donghao
-Author-email: 1417766861@qq.com
-License: Apache License 2.0
-Keywords: django,admin,widget,image,uploader
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 django_imguploder
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+安装
+-----
+`pip install django-imgwidget`
+
+`主页: https://pypi.org/project/django-imgwidget`
 
 步骤
 -----
 - 在settings.py中加入 `django_imguploder`
 
 - 配置上传图片路由
 ```python
@@ -66,9 +57,8 @@
 
 - 如果想保存为json格式，例如：['111.jpg', '222.jpg']
 ```
 def save_model(self, request, obj, form, change):
     for img in ['imgs', 'certificate_imgs']:
         setattr(obj, img, json.dumps(get_imgs_value(form.cleaned_data.get(img))))
     return super(MyAdmin, self).save_model(request, obj, form, change)
-```
-
+```
```

### Comparing `django-imgwidget-0.0.1/django_imguploder/forms/widget.py` & `django-imgwidget-0.0.2/django_imguploder/forms/widget.py`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.1/django_imguploder/static/css/imgwidget.css` & `django-imgwidget-0.0.2/django_imguploder/static/css/imgwidget.css`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.1/django_imguploder/static/imgs/add.png` & `django-imgwidget-0.0.2/django_imguploder/static/imgs/add.png`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.1/django_imguploder/static/js/jquery.min.js` & `django-imgwidget-0.0.2/django_imguploder/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.1/django_imguploder/templates/admin/widgets/img_multi_upload.html` & `django-imgwidget-0.0.2/django_imguploder/templates/admin/widgets/img_multi_upload.html`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.1/django_imgwidget.egg-info/PKG-INFO` & `django-imgwidget-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.1
+Version: 0.0.2
 Summary: 上传图片组件
-Home-page: https://github.com/RelaxedDong/simpleui
+Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,19 @@
 -----
 👍 后台上传图片
 
 ⚡️ 单图片、多图片批量上传
 
 ✨ 图片大图预览、删除
 
+安装
+-----
+`pip install django-imgwidget`
+
+`主页: https://pypi.org/project/django-imgwidget`
 
 步骤
 -----
 - 在settings.py中加入 `django_imguploder`
 
 - 配置上传图片路由
 ```python
```

### Comparing `django-imgwidget-0.0.1/django_imgwidget.egg-info/SOURCES.txt` & `django-imgwidget-0.0.2/django_imgwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.1/setup.py` & `django-imgwidget-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from setuptools import setup, find_packages
 
 long_description = "\n".join([
     open('README.md', 'r', encoding='utf-8').read(),
 ])
 
 NAME = 'django-imgwidget'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=()
     ),
     zip_safe=False,
     include_package_data=True,
     keywords='django,admin,widget,image,uploader',
-    url='https://github.com/RelaxedDong/simpleui',
+    url='https://github.com/RelaxedDong/django_imguploder',
     license='Apache License 2.0',
     author='donghao',
     long_description=long_description,
     long_description_content_type="text/markdown",  # 描述文档README的格式 一般md
     author_email='1417766861@qq.com',
     description='上传图片组件',
     install_requires=['django'],
```

