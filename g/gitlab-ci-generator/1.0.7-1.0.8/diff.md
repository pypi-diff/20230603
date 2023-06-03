# Comparing `tmp/gitlab-ci-generator-1.0.7.tar.gz` & `tmp/gitlab-ci-generator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-ci-generator-1.0.7.tar", last modified: Sat Jun  3 04:57:02 2023, max compression
+gzip compressed data, was "gitlab-ci-generator-1.0.8.tar", last modified: Sat Jun  3 18:40:38 2023, max compression
```

## Comparing `gitlab-ci-generator-1.0.7.tar` & `gitlab-ci-generator-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/
--rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/MANIFEST.in
--rw-r--r--   0 developer  (9999) developer  (9999)     9703 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/PKG-INFO
--rw-rw-rw-   0 developer  (9999) developer  (9999)     9354 2023-06-03 04:56:48.000000 gitlab-ci-generator-1.0.7/README.md
--rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/VERSION.txt
--rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/setup.cfg
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/setup.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/
--rw-r--r--   0 developer  (9999) developer  (9999)     9703 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/PKG-INFO
--rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/entry_points.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/requires.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/
--rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/__init__.py
--rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/gitlab_ci_generator.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/templates/
--rw-rw-rw-   0 developer  (9999) developer  (9999)     2133 2023-06-03 04:56:48.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/MANIFEST.in
+-rw-r--r--   0 developer  (9999) developer  (9999)     9981 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/PKG-INFO
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     9632 2023-06-03 18:40:22.000000 gitlab-ci-generator-1.0.8/README.md
+-rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/VERSION.txt
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/setup.cfg
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/setup.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.949511 gitlab-ci-generator-1.0.8/src/
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/
+-rw-r--r--   0 developer  (9999) developer  (9999)     9981 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/requires.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-06-03 18:40:38.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/__init__.py
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/gitlab_ci_generator.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 18:40:38.953511 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/templates/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     2220 2023-06-03 18:40:22.000000 gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
```

### Comparing `gitlab-ci-generator-1.0.7/PKG-INFO` & `gitlab-ci-generator-1.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: gitlab-ci-generator
-Version: 1.0.7
-Summary: Generates a mono-repo ci file.
-Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
-Author: Gary Schaetz
-Author-email: gary@schaetzkc.com
-License: MIT
-Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
-Description-Content-Type: text/markdown
-
 # gitlab-ci-generator
 This project builds a dynamic gitlab ci file that is intended to be used for monorepos.  The concept is to simplify the amount of work that is needed to manage the monorepo.
 
 ## Installation
 You can download and run directly with python or install using:
 ```
 pip install gitlab-ci-generator
@@ -129,19 +118,21 @@
 include:
     - local: 'example/example-config/rules.yml'
 
 stages:
   - build
   - post-deploy
 
+
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
     PROJECT_JOB_NAME: example-1
+    PROJECT_SUBDIR_LAST_FOLDER: example-folder-1
     MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
@@ -150,19 +141,21 @@
     - if: !reference [.job_changes_rules,schedule-rule-if]
   trigger:
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
     forward:
       pipeline_variables: true
  
+
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
+    PROJECT_SUBDIR_LAST_FOLDER: example-folder-2
     MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
@@ -196,14 +189,18 @@
     forward:
       pipeline_variables: true
 ```
 
 ## How to use in your pipeline
 A variable is passed into your pipeline that you can see in the previous section called PROJECT_SUBDIR.  Use this in before scripts to cd into the active project.  
 
+Two other variables are exposed:
+* PROJECT_JOB_NAME which contains the value from the name tag in your input yaml
+* PROJECT_SUBDIR_LAST_FOLDER the last folder in PROJECT_SUBDIR
+
 Here is an example of a pipeline that will use this program in one job to generate the ci file and then trigger it in the next job.  Notice how we set PARENT_PIPELINE_SOURCE variable so that you can use this in your downstream rules as a trigger overrides the original CI_PIPELINE_SOURCE.
 ```
 include: 
   - project: "gary.schaetz/private/pipelines"
     ref: main
     file: 'templates/rules/rules.yml'
 
@@ -241,8 +238,8 @@
     strategy: depend
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
-MIT License
+MIT License
```

### Comparing `gitlab-ci-generator-1.0.7/README.md` & `gitlab-ci-generator-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: gitlab-ci-generator
+Version: 1.0.8
+Summary: Generates a mono-repo ci file.
+Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
+Author: Gary Schaetz
+Author-email: gary@schaetzkc.com
+License: MIT
+Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
+Description-Content-Type: text/markdown
+
 # gitlab-ci-generator
 This project builds a dynamic gitlab ci file that is intended to be used for monorepos.  The concept is to simplify the amount of work that is needed to manage the monorepo.
 
 ## Installation
 You can download and run directly with python or install using:
 ```
 pip install gitlab-ci-generator
@@ -118,19 +129,21 @@
 include:
     - local: 'example/example-config/rules.yml'
 
 stages:
   - build
   - post-deploy
 
+
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
     PROJECT_JOB_NAME: example-1
+    PROJECT_SUBDIR_LAST_FOLDER: example-folder-1
     MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
@@ -139,19 +152,21 @@
     - if: !reference [.job_changes_rules,schedule-rule-if]
   trigger:
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
     forward:
       pipeline_variables: true
  
+
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
+    PROJECT_SUBDIR_LAST_FOLDER: example-folder-2
     MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
@@ -185,14 +200,18 @@
     forward:
       pipeline_variables: true
 ```
 
 ## How to use in your pipeline
 A variable is passed into your pipeline that you can see in the previous section called PROJECT_SUBDIR.  Use this in before scripts to cd into the active project.  
 
+Two other variables are exposed:
+* PROJECT_JOB_NAME which contains the value from the name tag in your input yaml
+* PROJECT_SUBDIR_LAST_FOLDER the last folder in PROJECT_SUBDIR
+
 Here is an example of a pipeline that will use this program in one job to generate the ci file and then trigger it in the next job.  Notice how we set PARENT_PIPELINE_SOURCE variable so that you can use this in your downstream rules as a trigger overrides the original CI_PIPELINE_SOURCE.
 ```
 include: 
   - project: "gary.schaetz/private/pipelines"
     ref: main
     file: 'templates/rules/rules.yml'
 
@@ -230,8 +249,8 @@
     strategy: depend
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
-MIT License
+MIT License
```

### Comparing `gitlab-ci-generator-1.0.7/setup.py` & `gitlab-ci-generator-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/PKG-INFO` & `gitlab-ci-generator-1.0.8/src/gitlab_ci_generator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
 Description-Content-Type: text/markdown
@@ -129,19 +129,21 @@
 include:
     - local: 'example/example-config/rules.yml'
 
 stages:
   - build
   - post-deploy
 
+
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
     PROJECT_JOB_NAME: example-1
+    PROJECT_SUBDIR_LAST_FOLDER: example-folder-1
     MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
@@ -150,19 +152,21 @@
     - if: !reference [.job_changes_rules,schedule-rule-if]
   trigger:
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
     forward:
       pipeline_variables: true
  
+
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
+    PROJECT_SUBDIR_LAST_FOLDER: example-folder-2
     MYVAR: MYVAR_VALUE
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
@@ -196,14 +200,18 @@
     forward:
       pipeline_variables: true
 ```
 
 ## How to use in your pipeline
 A variable is passed into your pipeline that you can see in the previous section called PROJECT_SUBDIR.  Use this in before scripts to cd into the active project.  
 
+Two other variables are exposed:
+* PROJECT_JOB_NAME which contains the value from the name tag in your input yaml
+* PROJECT_SUBDIR_LAST_FOLDER the last folder in PROJECT_SUBDIR
+
 Here is an example of a pipeline that will use this program in one job to generate the ci file and then trigger it in the next job.  Notice how we set PARENT_PIPELINE_SOURCE variable so that you can use this in your downstream rules as a trigger overrides the original CI_PIPELINE_SOURCE.
 ```
 include: 
   - project: "gary.schaetz/private/pipelines"
     ref: main
     file: 'templates/rules/rules.yml'
```

### Comparing `gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/gitlab_ci_generator.py` & `gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/gitlab_ci_generator.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/templates/gitlab-template.jinja` & `gitlab-ci-generator-1.0.8/src/gitlab_ci_generator_package/templates/gitlab-template.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -16,19 +16,22 @@
 stages:
   - build
 {% if pipeline_info.final_job %}
   - {{ pipeline_info.final_job.stage }}
 {% endif %}
 
 {% for job in jobs %}
+{% set path = job.folder.split('/') %}
+
 {{ job.name }}:
   stage: build
   variables:
     PROJECT_SUBDIR: {{ job.folder }}
     PROJECT_JOB_NAME: {{ job.name }}
+    PROJECT_SUBDIR_LAST_FOLDER: {{ path[-1] }}
 {% for variable in pipeline_info.shared_variables %}
     {{ variable.name }}: {{ variable.value }}
 {% endfor %}
   rules:
 {% for rule in pipeline_info.shared_reference_rules %}
     - if: !reference [{{ rule.rule_source }},{{ rule.rule_name }}]
 {% if rule.when %}
```

