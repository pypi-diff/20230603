# Comparing `tmp/AdminToolsDjango-1.0.3.tar.gz` & `tmp/AdminToolsDjango-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdminToolsDjango-1.0.3.tar", last modified: Sat Jun  3 04:49:04 2023, max compression
+gzip compressed data, was "AdminToolsDjango-1.0.5.tar", last modified: Sat Jun  3 12:29:14 2023, max compression
```

## Comparing `AdminToolsDjango-1.0.3.tar` & `AdminToolsDjango-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.821016 AdminToolsDjango-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.797830 AdminToolsDjango-1.0.3/AdminToolsDjango/
--rw-rw-rw-   0        0        0     7710 2023-06-02 17:58:47.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/CreateProject.py
--rw-rw-rw-   0        0        0       28 2023-06-02 17:28:25.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.803820 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/
--rw-rw-rw-   0        0        0     3956 2023-05-31 15:42:58.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/admin_script.py
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.810795 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/
--rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/__init__.py
--rw-rw-rw-   0        0        0       63 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/admin.py
--rw-rw-rw-   0        0        0      147 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.811792 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/migrations/
--rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/migrations/__init__.py
--rw-rw-rw-   0        0        0       57 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/models.py
--rw-rw-rw-   0        0        0      450 2023-05-31 09:51:36.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/tests.py
--rw-rw-rw-   0        0        0      142 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/urls.py
--rw-rw-rw-   0        0        0      148 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/app_test/views.py
--rw-rw-rw-   0        0        0      792 2023-05-31 08:06:12.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/manage.py
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.818773 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/
--rw-rw-rw-   0        0        0        0 2022-11-25 16:12:43.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/__init__.py
--rw-rw-rw-   0        0        0      411 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/asgi.py
--rw-rw-rw-   0        0        0     4298 2023-05-31 15:40:42.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/settings.py
--rw-rw-rw-   0        0        0      896 2023-05-31 15:40:42.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/urls.py
--rw-rw-rw-   0        0        0      177 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/uwsgi.ini
--rw-rw-rw-   0        0        0      419 2023-05-31 07:46:15.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.819985 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/static/
--rw-rw-rw-   0        0        0       22 2023-05-31 09:51:09.000000 AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/static/test.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 04:49:04.801819 AdminToolsDjango-1.0.3/AdminToolsDjango.egg-info/
--rw-rw-rw-   0        0        0     1111 2023-06-03 04:49:04.000000 AdminToolsDjango-1.0.3/AdminToolsDjango.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1089 2023-06-03 04:49:04.000000 AdminToolsDjango-1.0.3/AdminToolsDjango.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 04:49:04.000000 AdminToolsDjango-1.0.3/AdminToolsDjango.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-03 04:49:04.000000 AdminToolsDjango-1.0.3/AdminToolsDjango.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2023-06-03 04:49:04.821016 AdminToolsDjango-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      989 2023-06-03 03:57:19.000000 AdminToolsDjango-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 04:49:04.821982 AdminToolsDjango-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      750 2023-06-03 04:48:41.000000 AdminToolsDjango-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.661996 AdminToolsDjango-1.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.638040 AdminToolsDjango-1.0.5/AdminToolsDjango/
+-rw-rw-rw-   0        0        0     7761 2023-06-03 12:27:57.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/CreateProject.py
+-rw-rw-rw-   0        0        0       28 2023-06-02 17:28:25.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.644052 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/
+-rw-rw-rw-   0        0        0     3956 2023-05-31 15:42:58.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/admin_script.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.651004 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/
+-rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/admin.py
+-rw-rw-rw-   0        0        0      147 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.652002 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/migrations/
+-rw-rw-rw-   0        0        0        0 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/migrations/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-05-30 13:49:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/models.py
+-rw-rw-rw-   0        0        0      450 2023-05-31 09:51:36.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/tests.py
+-rw-rw-rw-   0        0        0      142 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/urls.py
+-rw-rw-rw-   0        0        0      148 2023-05-31 06:12:54.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/app_test/views.py
+-rw-rw-rw-   0        0        0      792 2023-05-31 08:06:12.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/manage.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.658982 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/
+-rw-rw-rw-   0        0        0        0 2022-11-25 16:12:43.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/__init__.py
+-rw-rw-rw-   0        0        0      411 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/asgi.py
+-rw-rw-rw-   0        0        0     4259 2023-06-03 12:26:07.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/settings.py
+-rw-rw-rw-   0        0        0      896 2023-05-31 15:40:42.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/urls.py
+-rw-rw-rw-   0        0        0      177 2023-05-31 07:34:39.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/uwsgi.ini
+-rw-rw-rw-   0        0        0      419 2023-05-31 07:46:15.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.659999 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/static/
+-rw-rw-rw-   0        0        0       22 2023-05-31 09:51:09.000000 AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/static/test.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 12:29:14.642029 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/
+-rw-rw-rw-   0        0        0     1112 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1089 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-03 12:29:14.000000 AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1112 2023-06-03 12:29:14.661001 AdminToolsDjango-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2023-06-03 12:28:33.000000 AdminToolsDjango-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:29:14.661996 AdminToolsDjango-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      750 2023-06-03 12:28:05.000000 AdminToolsDjango-1.0.5/setup.py
```

### Comparing `AdminToolsDjango-1.0.3/AdminToolsDjango/CreateProject.py` & `AdminToolsDjango-1.0.5/AdminToolsDjango/CreateProject.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,26 @@
         return f.read()
 
 
 def write(path, data):
     with open(path, mode='w', encoding='utf-8') as f:
         return f.write(data)
 
+
 class ProjectManager:
     def __init__(self, project_parent_dir=None, project_name=None, template_path=None, uwsgi_local_ip_port=None,
-                 nginx_port=None, nginx_conf_path=None):
+                 nginx_port=None, nginx_conf_path=None, python_environment=None):
         self.project_parent_dir = project_parent_dir or f'/django_par_{int(time.time())}'
         self.project_name = project_name or 'new_object'
         self.template_path = template_path or os.path.join(os.path.dirname(os.path.abspath(__file__)), 'template-1.0')
         self.uwsgi_local_ip_port = uwsgi_local_ip_port or '127.0.0.2:8000'
         self.nginx_port = nginx_port or '81'
         self.nginx_conf_path = nginx_conf_path or '/etc/nginx/nginx.conf'
         self.venv_name = f'{self.project_name}_venv'
-        self.python_environment = 'python3' if sys.platform == 'linux' else 'python'
+        self.python_environment = python_environment or ('python3' if sys.platform == 'linux' else 'python')
         self.cmd_activate_venv = f'source {self.venv_name}/bin/activate' if sys.platform == 'linux' else f'{self.venv_name}\\Scripts\\activate'
         self.last_result = 0
 
     def configure_production_environment(self):
         self.ide_uwsgi_ini()
         self.install_uwsgi()
         if sys.platform == 'linux':
```

### Comparing `AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/admin_script.py` & `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/admin_script.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/manage.py` & `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/manage.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/settings.py` & `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = get_random_secret_key()
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
-ALLOWED_HOSTS = ['43.139.189.169']   # 【2】 把公网ip增加到这里
+ALLOWED_HOSTS = ['43.139.189.169', '127.0.0.100']   # 【2】 把公网ip增加到这里
 
 # 应用在这个列表里面增加：
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
@@ -116,15 +116,15 @@
 
 # *** 后面每次增加新应用，应该在个列表里面增加新的静态目录。使用命令进行收集  ***
 
 DATA_UPLOAD_MAX_MEMORY_SIZE = None      # 【8】 新增
 
 # 【7】 新增用于收集给生产服务器
 
-if ('runserver' in sys.argv) and ('python3' in sys.argv or 'python' in sys.argv):
+if 'runserver' in sys.argv:
     STATICFILES_DIRS = [os.path.join(BASE_DIR, "static"), ]
     STATIC_ROOT = ''
 else:
     STATICFILES_DIRS = []  #
     STATIC_ROOT = os.path.join(BASE_DIR, "static")
 
 INSTALLED_APPS.append('app_test')
```

### Comparing `AdminToolsDjango-1.0.3/AdminToolsDjango/template-1.0/project_name/urls.py` & `AdminToolsDjango-1.0.5/AdminToolsDjango/template-1.0/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.3/AdminToolsDjango.egg-info/PKG-INFO` & `AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: AdminToolsDjango
-Version: 1.0.3
+Version: 1.0.5
 Author: 孙亮
 Description-Content-Type: text/markdown
 
-# DjangoAdminTools
+## AdminToolsDjango
 
 使用模板 自动创建Django项目
 ## 介绍：
     兼容 linux windows 系统 
     创建虚拟环境后 安装djano==3.2.11 然后用模板创建项目，
     可以自定义模板： 模板路径 建议使用绝对路径
     可以自定义项目上级文件夹，project_parent_dir， 建议使用绝对路径
```

### Comparing `AdminToolsDjango-1.0.3/AdminToolsDjango.egg-info/SOURCES.txt` & `AdminToolsDjango-1.0.5/AdminToolsDjango.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.3/PKG-INFO` & `AdminToolsDjango-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: AdminToolsDjango
-Version: 1.0.3
+Version: 1.0.5
 Author: 孙亮
 Description-Content-Type: text/markdown
 
-# DjangoAdminTools
+## AdminToolsDjango
 
 使用模板 自动创建Django项目
 ## 介绍：
     兼容 linux windows 系统 
     创建虚拟环境后 安装djano==3.2.11 然后用模板创建项目，
     可以自定义模板： 模板路径 建议使用绝对路径
     可以自定义项目上级文件夹，project_parent_dir， 建议使用绝对路径
```

### Comparing `AdminToolsDjango-1.0.3/README.md` & `AdminToolsDjango-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# DjangoAdminTools
+## AdminToolsDjango
 
 使用模板 自动创建Django项目
 ## 介绍：
     兼容 linux windows 系统 
     创建虚拟环境后 安装djano==3.2.11 然后用模板创建项目，
     可以自定义模板： 模板路径 建议使用绝对路径
     可以自定义项目上级文件夹，project_parent_dir， 建议使用绝对路径
```

### Comparing `AdminToolsDjango-1.0.3/setup.py` & `AdminToolsDjango-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='AdminToolsDjango',
-    version='1.0.3',
+    version='1.0.5',
     author='孙亮',
     packages=['AdminToolsDjango'],
     # install_requires=[
     #     # 'some_dependency>=1.0.0',
     # ],
     # package_data={'AdminToolsDjango': ['template-1.0/*', 'template-1.0/app_test', 'template-1.0/app_test/migrations',
     #                                    'template-1.0/project_name', 'template-1.0/static']},
```

