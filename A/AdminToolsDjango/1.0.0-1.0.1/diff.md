# Comparing `tmp/AdminToolsDjango-1.0.0.tar.gz` & `tmp/AdminToolsDjango-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdminToolsDjango-1.0.0.tar", last modified: Fri Jun  2 18:45:13 2023, max compression
+gzip compressed data, was "AdminToolsDjango-1.0.1.tar", last modified: Sat Jun  3 04:02:51 2023, max compression
```

## Comparing `AdminToolsDjango-1.0.0.tar` & `AdminToolsDjango-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 18:45:13.231821 AdminToolsDjango-1.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-02 18:45:13.225841 AdminToolsDjango-1.0.0/AdminToolsDjango/
--rw-rw-rw-   0        0        0     7710 2023-06-02 17:58:47.000000 AdminToolsDjango-1.0.0/AdminToolsDjango/CreateProject.py
--rw-rw-rw-   0        0        0       28 2023-06-02 17:28:25.000000 AdminToolsDjango-1.0.0/AdminToolsDjango/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:45:13.230798 AdminToolsDjango-1.0.0/AdminToolsDjango.egg-info/
--rw-rw-rw-   0        0        0      921 2023-06-02 18:45:13.000000 AdminToolsDjango-1.0.0/AdminToolsDjango.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-06-02 18:45:13.000000 AdminToolsDjango-1.0.0/AdminToolsDjango.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 18:45:13.000000 AdminToolsDjango-1.0.0/AdminToolsDjango.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-02 18:45:13.000000 AdminToolsDjango-1.0.0/AdminToolsDjango.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      921 2023-06-02 18:45:13.231821 AdminToolsDjango-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-06-02 18:38:25.000000 AdminToolsDjango-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 18:45:13.231821 AdminToolsDjango-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      433 2023-06-02 18:44:10.000000 AdminToolsDjango-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 04:02:51.759521 AdminToolsDjango-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-03 04:02:51.753500 AdminToolsDjango-1.0.1/AdminToolsDjango/
+-rw-rw-rw-   0        0        0     7710 2023-06-02 17:58:47.000000 AdminToolsDjango-1.0.1/AdminToolsDjango/CreateProject.py
+-rw-rw-rw-   0        0        0       28 2023-06-02 17:28:25.000000 AdminToolsDjango-1.0.1/AdminToolsDjango/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 04:02:51.757490 AdminToolsDjango-1.0.1/AdminToolsDjango.egg-info/
+-rw-rw-rw-   0        0        0     1111 2023-06-03 04:02:51.000000 AdminToolsDjango-1.0.1/AdminToolsDjango.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-06-03 04:02:51.000000 AdminToolsDjango-1.0.1/AdminToolsDjango.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 04:02:51.000000 AdminToolsDjango-1.0.1/AdminToolsDjango.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-03 04:02:51.000000 AdminToolsDjango-1.0.1/AdminToolsDjango.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2023-06-03 04:02:51.758521 AdminToolsDjango-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2023-06-03 03:57:19.000000 AdminToolsDjango-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 04:02:51.759521 AdminToolsDjango-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-06-03 04:02:38.000000 AdminToolsDjango-1.0.1/setup.py
```

### Comparing `AdminToolsDjango-1.0.0/AdminToolsDjango/CreateProject.py` & `AdminToolsDjango-1.0.1/AdminToolsDjango/CreateProject.py`

 * *Files identical despite different names*

### Comparing `AdminToolsDjango-1.0.0/AdminToolsDjango.egg-info/PKG-INFO` & `AdminToolsDjango-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-Metadata-Version: 2.1
-Name: AdminToolsDjango
-Version: 1.0.0
-Author: 孙亮
-Description-Content-Type: text/markdown
-
 # DjangoAdminTools
 
 使用模板 自动创建Django项目
-## 介绍
+## 介绍：
     兼容 linux windows 系统 
     创建虚拟环境后 安装djano==3.2.11 然后用模板创建项目，
     可以自定义模板： 模板路径 建议使用绝对路径
     可以自定义项目上级文件夹，project_parent_dir， 建议使用绝对路径
+## 使用示例：
 ```python
-import DjangoAdminTools
+import AdminToolsDjango
 # 创建一个对象
-django_project = DjangoAdminTools.ProjectManager(project_parent_dir='/obj_test/new_obj_parent',
+django_project = AdminToolsDjango.ProjectManager(project_parent_dir='/obj_test/new_obj_parent',
                                             project_name='new_obj',
                                             )
 print(django_project.cmd_activate_venv)
+# 创建项目
 django_project.create_project()
+# 配置生产环境 会自动配置nginx反向代理 要确保linux系统 有 nginx 服务器
+django_project.configure_production_environment() 
 ```
 
-## 安装
-使用以下命令安装 DjangoAdminTools：
+## 安装：
+使用以下命令安装 AdminToolsDjango：
 ```shell
-pip install DjangoAdminTools
+pip install AdminToolsDjango
 ```
```

