# Comparing `tmp/gitlab-ci-generator-1.0.6.tar.gz` & `tmp/gitlab-ci-generator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-ci-generator-1.0.6.tar", last modified: Fri Jun  2 18:47:23 2023, max compression
+gzip compressed data, was "gitlab-ci-generator-1.0.7.tar", last modified: Sat Jun  3 04:57:02 2023, max compression
```

## Comparing `gitlab-ci-generator-1.0.6.tar` & `gitlab-ci-generator-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/
--rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/MANIFEST.in
--rw-r--r--   0 developer  (9999) developer  (9999)     9571 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/PKG-INFO
--rw-rw-rw-   0 developer  (9999) developer  (9999)     9222 2023-06-02 18:47:08.000000 gitlab-ci-generator-1.0.6/README.md
--rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/VERSION.txt
--rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/setup.cfg
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/setup.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/
--rw-r--r--   0 developer  (9999) developer  (9999)     9571 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/PKG-INFO
--rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/entry_points.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/requires.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-06-02 18:47:23.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/
--rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/__init__.py
--rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/gitlab_ci_generator.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-02 18:47:23.319160 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/templates/
--rw-rw-rw-   0 developer  (9999) developer  (9999)     2045 2023-06-02 18:47:08.000000 gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/MANIFEST.in
+-rw-r--r--   0 developer  (9999) developer  (9999)     9703 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/PKG-INFO
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     9354 2023-06-03 04:56:48.000000 gitlab-ci-generator-1.0.7/README.md
+-rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/VERSION.txt
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/setup.cfg
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/setup.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/
+-rw-r--r--   0 developer  (9999) developer  (9999)     9703 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/requires.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-06-03 04:57:02.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/__init__.py
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/gitlab_ci_generator.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-06-03 04:57:02.882576 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/templates/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     2133 2023-06-03 04:56:48.000000 gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
```

### Comparing `gitlab-ci-generator-1.0.6/PKG-INFO` & `gitlab-ci-generator-1.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: gitlab-ci-generator
-Version: 1.0.6
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
@@ -147,14 +136,16 @@
       when: manual
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,schedule-rule-if]
   trigger:
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
+    forward:
+      pipeline_variables: true
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
     MYVAR: MYVAR_VALUE
@@ -171,28 +162,32 @@
     - if: !reference [.job_changes_rules,schedule-rule-if]
   needs: 
     - job: example-1
       optional: true 
   trigger:
     include: example/example-folder-2/.gitlab-example.yml    
     strategy: depend
+    forward:
+      pipeline_variables: true
  
 cut-tag:
   stage: post-deploy
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
         - example/example-folder-2/**/*
   trigger:
     include: 
       - project: 'gary.schaetz/private/pipelines'
         ref: 'main'
         file: '/path/to/child-pipeline.yml' 
     strategy: depend
+    forward:
+      pipeline_variables: true
 ```
 
 ## How to use in your pipeline
 A variable is passed into your pipeline that you can see in the previous section called PROJECT_SUBDIR.  Use this in before scripts to cd into the active project.  
 
 Here is an example of a pipeline that will use this program in one job to generate the ci file and then trigger it in the next job.  Notice how we set PARENT_PIPELINE_SOURCE variable so that you can use this in your downstream rules as a trigger overrides the original CI_PIPELINE_SOURCE.
 ```
@@ -235,8 +230,8 @@
     strategy: depend
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
-MIT License
+MIT License
```

### Comparing `gitlab-ci-generator-1.0.6/README.md` & `gitlab-ci-generator-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: gitlab-ci-generator
+Version: 1.0.7
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
@@ -136,14 +147,16 @@
       when: manual
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,schedule-rule-if]
   trigger:
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
+    forward:
+      pipeline_variables: true
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
     MYVAR: MYVAR_VALUE
@@ -160,28 +173,32 @@
     - if: !reference [.job_changes_rules,schedule-rule-if]
   needs: 
     - job: example-1
       optional: true 
   trigger:
     include: example/example-folder-2/.gitlab-example.yml    
     strategy: depend
+    forward:
+      pipeline_variables: true
  
 cut-tag:
   stage: post-deploy
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
         - example/example-folder-2/**/*
   trigger:
     include: 
       - project: 'gary.schaetz/private/pipelines'
         ref: 'main'
         file: '/path/to/child-pipeline.yml' 
     strategy: depend
+    forward:
+      pipeline_variables: true
 ```
 
 ## How to use in your pipeline
 A variable is passed into your pipeline that you can see in the previous section called PROJECT_SUBDIR.  Use this in before scripts to cd into the active project.  
 
 Here is an example of a pipeline that will use this program in one job to generate the ci file and then trigger it in the next job.  Notice how we set PARENT_PIPELINE_SOURCE variable so that you can use this in your downstream rules as a trigger overrides the original CI_PIPELINE_SOURCE.
 ```
@@ -224,8 +241,8 @@
     strategy: depend
   variables:
     PARENT_PIPELINE_ID: $CI_PIPELINE_ID
     PARENT_PIPELINE_SOURCE: $CI_PIPELINE_SOURCE
 ```
 
 ## License
-MIT License
+MIT License
```

### Comparing `gitlab-ci-generator-1.0.6/setup.py` & `gitlab-ci-generator-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.6/src/gitlab_ci_generator.egg-info/PKG-INFO` & `gitlab-ci-generator-1.0.7/src/gitlab_ci_generator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.6
+Version: 1.0.7
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
 Description-Content-Type: text/markdown
@@ -147,14 +147,16 @@
       when: manual
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,schedule-rule-if]
   trigger:
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
+    forward:
+      pipeline_variables: true
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
     PROJECT_JOB_NAME: example-2
     MYVAR: MYVAR_VALUE
@@ -171,28 +173,32 @@
     - if: !reference [.job_changes_rules,schedule-rule-if]
   needs: 
     - job: example-1
       optional: true 
   trigger:
     include: example/example-folder-2/.gitlab-example.yml    
     strategy: depend
+    forward:
+      pipeline_variables: true
  
 cut-tag:
   stage: post-deploy
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
         - example/example-folder-2/**/*
   trigger:
     include: 
       - project: 'gary.schaetz/private/pipelines'
         ref: 'main'
         file: '/path/to/child-pipeline.yml' 
     strategy: depend
+    forward:
+      pipeline_variables: true
 ```
 
 ## How to use in your pipeline
 A variable is passed into your pipeline that you can see in the previous section called PROJECT_SUBDIR.  Use this in before scripts to cd into the active project.  
 
 Here is an example of a pipeline that will use this program in one job to generate the ci file and then trigger it in the next job.  Notice how we set PARENT_PIPELINE_SOURCE variable so that you can use this in your downstream rules as a trigger overrides the original CI_PIPELINE_SOURCE.
 ```
```

### Comparing `gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/gitlab_ci_generator.py` & `gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/gitlab_ci_generator.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.6/src/gitlab_ci_generator_package/templates/gitlab-template.jinja` & `gitlab-ci-generator-1.0.7/src/gitlab_ci_generator_package/templates/gitlab-template.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 {% for parent in job.parents %}
     - job: {{ parent.name }}
       optional: true 
 {% endfor %}
   trigger:
     include: {{ job.folder }}/{{ job.gitlab_yml_file }}    
     strategy: depend
+    forward:
+      pipeline_variables: true
  
 {% endfor %}
 {% if pipeline_info.final_job %}
 {{ pipeline_info.final_job.name }}:
   stage: {{ pipeline_info.final_job.stage }}
   rules:
 {% for rule in pipeline_info.final_job.rules %}
@@ -72,9 +74,11 @@
 {% endfor %}
   trigger:
     include: 
       - project: '{{ pipeline_info.final_job.trigger_job_info.project }}'
         ref: '{{ pipeline_info.final_job.trigger_job_info.ref }}'
         file: '{{ pipeline_info.final_job.trigger_job_info.file }}' 
     strategy: depend
+    forward:
+      pipeline_variables: true
 {% endif %}
```

