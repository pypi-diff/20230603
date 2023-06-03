# Comparing `tmp/git-debranch-0.1.5.tar.gz` & `tmp/git-debranch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-debranch-0.1.5.tar", last modified: Sat May 27 12:59:01 2023, max compression
+gzip compressed data, was "git-debranch-0.1.6.tar", last modified: Sat Jun  3 13:01:20 2023, max compression
```

## Comparing `git-debranch-0.1.5.tar` & `git-debranch-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-27 12:58:51.000000 git-debranch-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-27 12:59:01.539928 git-debranch-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-27 12:58:51.000000 git-debranch-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 12:59:01.539928 git-debranch-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-27 12:58:51.000000 git-debranch-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.535928 git-debranch-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.535928 git-debranch-0.1.5/src/git_debranch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/src/git_debranch/bpmn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/process_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/spawn.bpmn
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/bpmn/process_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/script_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 12:58:51.000000 git-debranch-0.1.5/src/git_debranch/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:59:01.539928 git-debranch-0.1.5/src/git_debranch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-27 12:59:01.000000 git-debranch-0.1.5/src/git_debranch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-06-03 13:01:06.000000 git-debranch-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-03 13:01:20.817450 git-debranch-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-03 13:01:06.000000 git-debranch-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 13:01:20.817450 git-debranch-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-03 13:01:06.000000 git-debranch-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.813450 git-debranch-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.813450 git-debranch-0.1.6/src/git_debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/src/git_debranch/bpmn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/all_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/confirm_deletion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/git-debranch.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/process_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/spawn.bpmn
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/bpmn/process_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/script_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-03 13:01:06.000000 git-debranch-0.1.6/src/git_debranch/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:01:20.817450 git-debranch-0.1.6/src/git_debranch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 13:01:20.000000 git-debranch-0.1.6/src/git_debranch.egg-info/top_level.txt
```

### Comparing `git-debranch-0.1.5/LICENSE` & `git-debranch-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.5/PKG-INFO` & `git-debranch-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-debranch
-Version: 0.1.5
+Version: 0.1.6
 Summary: Remove git branches
 Author: Jon Herron
 Author-email: jon.herron@yahoo.com
 License: lGPLv2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,25 +15,39 @@
 
 ## Installation
 
 ```
 pip install git-debranch
 ```
 
-## Usage
+## Running
 
 ```
 git debranch
 ```
 
 From inside a git repository, running `git debranch` will present you with a list of branches that could 
 be deleted. This list is presented using `$EDITOR`. If the environment variable is not set `vi` is used 
 as the fallback.
 
-*Please note `git fetch -p` is run before the branch list is presented.*
+*Please note `git fetch -p` is run before the branch list is presented. This can be disabled by providing
+the --offline switch.*
+
+## Usage
+
+```
+usage: git debranch [-h] [--offline] [--dry-run]
+
+Delete local git branches
+
+options:
+  -h          show this help message and exit
+  --offline   Do not run online operations such as fetch and prune
+  --dry-run   Do not actually delete branches
+```
 
 ## Editing the Branch List
 
 When `$EDITOR` is invoked, it will contain a series of lines. Comment lines begin with `#` and any line that 
 is not empty or a comment is assumed to be the name of a branch to delete locally. You can update this list 
 by either removing or commenting branches that you want to keep. Branches that appear safe to delete are 
 uncommented by default. Branches that may not be safe to delete are left commented by default. When you save
```

### Comparing `git-debranch-0.1.5/README.md` & `git-debranch-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,39 @@
 
 ## Installation
 
 ```
 pip install git-debranch
 ```
 
-## Usage
+## Running
 
 ```
 git debranch
 ```
 
 From inside a git repository, running `git debranch` will present you with a list of branches that could 
 be deleted. This list is presented using `$EDITOR`. If the environment variable is not set `vi` is used 
 as the fallback.
 
-*Please note `git fetch -p` is run before the branch list is presented.*
+*Please note `git fetch -p` is run before the branch list is presented. This can be disabled by providing
+the --offline switch.*
+
+## Usage
+
+```
+usage: git debranch [-h] [--offline] [--dry-run]
+
+Delete local git branches
+
+options:
+  -h          show this help message and exit
+  --offline   Do not run online operations such as fetch and prune
+  --dry-run   Do not actually delete branches
+```
 
 ## Editing the Branch List
 
 When `$EDITOR` is invoked, it will contain a series of lines. Comment lines begin with `#` and any line that 
 is not empty or a comment is assumed to be the name of a branch to delete locally. You can update this list 
 by either removing or commenting branches that you want to keep. Branches that appear safe to delete are 
 uncommented by default. Branches that may not be safe to delete are left commented by default. When you save
```

### Comparing `git-debranch-0.1.5/setup.py` & `git-debranch-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def contents_of(filename):
     with open(filename) as f:
         return f.read()
 
 setup(
     name = "git-debranch",
-    version = "0.1.5",
+    version = contents_of("VERSION"),
     description = "Remove git branches",
     long_description = contents_of("README.md"),
     long_description_content_type = "text/markdown",
 
     license = "lGPLv2",
     author = "Jon Herron",
     author_email = "jon.herron@yahoo.com",
```

### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/all_branches.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/all_branches.bpmn`

 * *Files 10% similar despite different names*

#### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/all_branches.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/all_branches.bpmn`

```diff
@@ -1,16 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
   <bpmn:process id="get_all_branches" name="Get all branches" isExecutable="true">
     <bpmn:startEvent id="StartEvent_1">
       <bpmn:outgoing>Flow_0hezl4t</bpmn:outgoing>
     </bpmn:startEvent>
-    <bpmn:sequenceFlow id="Flow_0hezl4t" sourceRef="StartEvent_1" targetRef="Activity_0lb6dii"/>
+    <bpmn:sequenceFlow id="Flow_0hezl4t" sourceRef="StartEvent_1" targetRef="Gateway_0jfksvo"/>
     <bpmn:parallelGateway id="Gateway_07vk4jr">
-      <bpmn:incoming>Flow_1ogqfb8</bpmn:incoming>
+      <bpmn:incoming>Flow_1c6aokx</bpmn:incoming>
       <bpmn:outgoing>Flow_0889ozu</bpmn:outgoing>
       <bpmn:outgoing>Flow_05auvqd</bpmn:outgoing>
       <bpmn:outgoing>Flow_1nxzhsg</bpmn:outgoing>
       <bpmn:outgoing>Flow_02avd0d</bpmn:outgoing>
     </bpmn:parallelGateway>
     <bpmn:sequenceFlow id="Flow_0889ozu" sourceRef="Gateway_07vk4jr" targetRef="Activity_09d782o"/>
     <bpmn:parallelGateway id="Gateway_0gmspex">
@@ -78,15 +78,15 @@
 del(current_branch_result)
 del(spawn_args)</bpmn:script>
     </bpmn:scriptTask>
     <bpmn:sequenceFlow id="Flow_04ggq0k" sourceRef="Activity_1rwssw3" targetRef="Event_1y1qa7g"/>
     <bpmn:endEvent id="Event_1y1qa7g">
       <bpmn:incoming>Flow_04ggq0k</bpmn:incoming>
     </bpmn:endEvent>
-    <bpmn:sequenceFlow id="Flow_1ogqfb8" sourceRef="Activity_0lb6dii" targetRef="Gateway_07vk4jr"/>
+    <bpmn:sequenceFlow id="Flow_1ogqfb8" sourceRef="Activity_0lb6dii" targetRef="Gateway_0te47lu"/>
     <bpmn:sequenceFlow id="Flow_0plnctp" sourceRef="Gateway_0gmspex" targetRef="Activity_1rwssw3"/>
     <bpmn:callActivity id="Activity_09d782o" name="Get merged branches" calledElement="spawn_process">
       <bpmn:extensionElements>
         <spiffworkflow:preScript>spawn_args = [&quot;git&quot;, &quot;branch&quot;, &quot;--merged&quot;]</spiffworkflow:preScript>
         <spiffworkflow:postScript>merged_branches_result = result</spiffworkflow:postScript>
       </bpmn:extensionElements>
       <bpmn:incoming>Flow_0889ozu</bpmn:incoming>
@@ -128,31 +128,45 @@
         <spiffworkflow:serviceTaskOperator id="os/SpawnProcess" resultVariable="result">
           <spiffworkflow:parameters>
             <spiffworkflow:parameter id="args" type="any" value="[&quot;git&quot;, &quot;fetch&quot;, &quot;-p&quot;]"/>
           </spiffworkflow:parameters>
         </spiffworkflow:serviceTaskOperator>
         <spiffworkflow:preScript>spawn_args = [&quot;git&quot;, &quot;fetch&quot;, &quot;-p&quot;]</spiffworkflow:preScript>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_0hezl4t</bpmn:incoming>
+      <bpmn:incoming>Flow_1pz1noe</bpmn:incoming>
       <bpmn:outgoing>Flow_1ogqfb8</bpmn:outgoing>
     </bpmn:callActivity>
+    <bpmn:exclusiveGateway id="Gateway_0jfksvo" default="Flow_1pz1noe">
+      <bpmn:incoming>Flow_0hezl4t</bpmn:incoming>
+      <bpmn:outgoing>Flow_1pz1noe</bpmn:outgoing>
+      <bpmn:outgoing>Flow_10267z6</bpmn:outgoing>
+    </bpmn:exclusiveGateway>
+    <bpmn:sequenceFlow id="Flow_1pz1noe" sourceRef="Gateway_0jfksvo" targetRef="Activity_0lb6dii"/>
+    <bpmn:exclusiveGateway id="Gateway_0te47lu">
+      <bpmn:incoming>Flow_1ogqfb8</bpmn:incoming>
+      <bpmn:incoming>Flow_0zq7ab2</bpmn:incoming>
+      <bpmn:outgoing>Flow_1c6aokx</bpmn:outgoing>
+    </bpmn:exclusiveGateway>
+    <bpmn:sequenceFlow id="Flow_1c6aokx" sourceRef="Gateway_0te47lu" targetRef="Gateway_07vk4jr"/>
+    <bpmn:sequenceFlow id="Flow_10267z6" sourceRef="Gateway_0jfksvo" targetRef="Activity_11bxwa4">
+      <bpmn:conditionExpression>offline</bpmn:conditionExpression>
+    </bpmn:sequenceFlow>
+    <bpmn:sequenceFlow id="Flow_0zq7ab2" sourceRef="Activity_11bxwa4" targetRef="Gateway_0te47lu"/>
+    <bpmn:scriptTask id="Activity_11bxwa4" name="Show offline">
+      <bpmn:incoming>Flow_10267z6</bpmn:incoming>
+      <bpmn:outgoing>Flow_0zq7ab2</bpmn:outgoing>
+      <bpmn:script>print(&quot;Skipping fetch -p because --offline&quot;)</bpmn:script>
+    </bpmn:scriptTask>
     <bpmn:textAnnotation id="TextAnnotation_1b81gty">
       <bpmn:text>Would like to look at making this a multi-instance once things are merged.</bpmn:text>
     </bpmn:textAnnotation>
     <bpmn:association id="Association_06jn47e" sourceRef="Gateway_07vk4jr" targetRef="TextAnnotation_1b81gty"/>
-    <bpmn:textAnnotation id="TextAnnotation_1wtp9ek">
-      <bpmn:text>Before checking local branches we want to fetch and prune branches. This will be arg driven soon.</bpmn:text>
-    </bpmn:textAnnotation>
-    <bpmn:association id="Association_1uty3t0" sourceRef="Activity_0lb6dii" targetRef="TextAnnotation_1wtp9ek"/>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
     <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="get_all_branches">
-      <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
-        <dc:Bounds x="32" y="159" width="36" height="36"/>
-      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Gateway_120o0l4_di" bpmnElement="Gateway_07vk4jr">
         <dc:Bounds x="265" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Gateway_1v3pb50_di" bpmnElement="Gateway_0gmspex">
         <dc:Bounds x="525" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_097d5gt_di" bpmnElement="Activity_1rwssw3">
@@ -162,71 +176,72 @@
       <bpmndi:BPMNShape id="Event_1y1qa7g_di" bpmnElement="Event_1y1qa7g">
         <dc:Bounds x="752" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_1lc0i0u_di" bpmnElement="Activity_09d782o">
         <dc:Bounds x="370" y="-20" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="TextAnnotation_1b81gty_di" bpmnElement="TextAnnotation_1b81gty">
-        <dc:Bounds x="160" y="-63" width="100" height="98"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="TextAnnotation_1wtp9ek_di" bpmnElement="TextAnnotation_1wtp9ek">
-        <dc:Bounds x="-30" y="-63" width="100" height="127"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="BPMNShape_0apvxkl" bpmnElement="Activity_1qlm0jm">
         <dc:Bounds x="370" y="80" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="BPMNShape_0w43oon" bpmnElement="Activity_1ntduty">
         <dc:Bounds x="370" y="190" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="BPMNShape_10pp7pw" bpmnElement="Activity_0wtw0rj">
         <dc:Bounds x="370" y="290" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="TextAnnotation_1b81gty_di" bpmnElement="TextAnnotation_1b81gty">
+        <dc:Bounds x="160" y="-63" width="100" height="98"/>
+        <bpmndi:BPMNLabel/>
+      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_0gv5hia_di" bpmnElement="Activity_0lb6dii">
-        <dc:Bounds x="120" y="137" width="100" height="80"/>
+        <dc:Bounds x="70" y="137" width="100" height="80"/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Gateway_0te47lu_di" bpmnElement="Gateway_0te47lu" isMarkerVisible="true">
+        <dc:Bounds x="195" y="152" width="50" height="50"/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
+        <dc:Bounds x="-88" y="159" width="36" height="36"/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Gateway_0jfksvo_di" bpmnElement="Gateway_0jfksvo" isMarkerVisible="true">
+        <dc:Bounds x="-25" y="152" width="50" height="50"/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Activity_1pi1x08_di" bpmnElement="Activity_11bxwa4">
+        <dc:Bounds x="70" y="250" width="100" height="80"/>
+        <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNEdge id="Flow_0hezl4t_di" bpmnElement="Flow_0hezl4t">
-        <di:waypoint x="68" y="177"/>
-        <di:waypoint x="120" y="177"/>
+        <di:waypoint x="-52" y="177"/>
+        <di:waypoint x="-25" y="177"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_0889ozu_di" bpmnElement="Flow_0889ozu">
         <di:waypoint x="290" y="152"/>
         <di:waypoint x="290" y="20"/>
         <di:waypoint x="370" y="20"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_04ggq0k_di" bpmnElement="Flow_04ggq0k">
         <di:waypoint x="710" y="177"/>
         <di:waypoint x="752" y="177"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_1ogqfb8_di" bpmnElement="Flow_1ogqfb8">
-        <di:waypoint x="220" y="177"/>
-        <di:waypoint x="265" y="177"/>
+        <di:waypoint x="170" y="177"/>
+        <di:waypoint x="195" y="177"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_0plnctp_di" bpmnElement="Flow_0plnctp">
         <di:waypoint x="575" y="177"/>
         <di:waypoint x="610" y="177"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_02q163a_di" bpmnElement="Flow_02q163a">
         <di:waypoint x="470" y="20"/>
         <di:waypoint x="550" y="20"/>
         <di:waypoint x="550" y="152"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Association_06jn47e_di" bpmnElement="Association_06jn47e">
-        <di:waypoint x="283" y="159"/>
-        <di:waypoint x="239" y="35"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Association_1uty3t0_di" bpmnElement="Association_1uty3t0">
-        <di:waypoint x="137" y="137"/>
-        <di:waypoint x="70" y="52"/>
-      </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_05auvqd_di" bpmnElement="Flow_05auvqd">
         <di:waypoint x="290" y="152"/>
         <di:waypoint x="290" y="120"/>
         <di:waypoint x="370" y="120"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_1msiwsx_di" bpmnElement="Flow_1msiwsx">
         <di:waypoint x="470" y="120"/>
@@ -249,10 +264,32 @@
         <di:waypoint x="370" y="330"/>
       </bpmndi:BPMNEdge>
       <bpmndi:BPMNEdge id="Flow_0ua7und_di" bpmnElement="Flow_0ua7und">
         <di:waypoint x="470" y="330"/>
         <di:waypoint x="550" y="330"/>
         <di:waypoint x="550" y="202"/>
       </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Association_06jn47e_di" bpmnElement="Association_06jn47e">
+        <di:waypoint x="283" y="159"/>
+        <di:waypoint x="239" y="35"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1pz1noe_di" bpmnElement="Flow_1pz1noe">
+        <di:waypoint x="25" y="177"/>
+        <di:waypoint x="70" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1c6aokx_di" bpmnElement="Flow_1c6aokx">
+        <di:waypoint x="245" y="177"/>
+        <di:waypoint x="265" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_10267z6_di" bpmnElement="Flow_10267z6">
+        <di:waypoint x="0" y="202"/>
+        <di:waypoint x="0" y="290"/>
+        <di:waypoint x="70" y="290"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_0zq7ab2_di" bpmnElement="Flow_0zq7ab2">
+        <di:waypoint x="170" y="290"/>
+        <di:waypoint x="220" y="290"/>
+        <di:waypoint x="220" y="202"/>
+      </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/branch_parser.bpmn`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/spawn.bpmn`

 * *Files 16% similar despite different names*

#### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/spawn.bpmn`

```diff
@@ -1,81 +1,102 @@
 <?xml version="1.0" encoding="utf-8"?>
-<bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
-  <bpmn:process id="delete_branches" isExecutable="true">
+<bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
+  <bpmn:process id="spawn_process" name="Spawn a New Process" isExecutable="true">
     <bpmn:startEvent id="StartEvent_1">
-      <bpmn:outgoing>Flow_0ecta24</bpmn:outgoing>
+      <bpmn:outgoing>Flow_090xnqj</bpmn:outgoing>
     </bpmn:startEvent>
-    <bpmn:sequenceFlow id="Flow_0ecta24" sourceRef="StartEvent_1" targetRef="Gateway_1ltog1i"/>
-    <bpmn:endEvent id="Event_1bsl2ov">
-      <bpmn:incoming>Flow_0v4mach</bpmn:incoming>
-    </bpmn:endEvent>
-    <bpmn:exclusiveGateway id="Gateway_1ltog1i" default="Flow_1lxcorc">
-      <bpmn:incoming>Flow_0ecta24</bpmn:incoming>
-      <bpmn:outgoing>Flow_1lxcorc</bpmn:outgoing>
-      <bpmn:outgoing>Flow_1cn71yy</bpmn:outgoing>
+    <bpmn:sequenceFlow id="Flow_090xnqj" sourceRef="StartEvent_1" targetRef="Activity_1wobbp0"/>
+    <bpmn:exclusiveGateway id="Gateway_0o5auw6" default="Flow_1gimdqy">
+      <bpmn:incoming>Flow_1cl2vgj</bpmn:incoming>
+      <bpmn:outgoing>Flow_1gimdqy</bpmn:outgoing>
+      <bpmn:outgoing>Flow_1msh4mr</bpmn:outgoing>
     </bpmn:exclusiveGateway>
-    <bpmn:sequenceFlow id="Flow_1lxcorc" sourceRef="Gateway_1ltog1i" targetRef="Activity_1yt24dj"/>
-    <bpmn:sequenceFlow id="Flow_1cn71yy" sourceRef="Gateway_1ltog1i" targetRef="Gateway_0w96sv3">
-      <bpmn:conditionExpression>len(branches_to_delete) == 0</bpmn:conditionExpression>
+    <bpmn:sequenceFlow id="Flow_1cl2vgj" sourceRef="Activity_1wobbp0" targetRef="Gateway_0o5auw6"/>
+    <bpmn:endEvent id="Event_1vc03l8">
+      <bpmn:incoming>Flow_1gimdqy</bpmn:incoming>
+    </bpmn:endEvent>
+    <bpmn:sequenceFlow id="Flow_1gimdqy" sourceRef="Gateway_0o5auw6" targetRef="Event_1vc03l8"/>
+    <bpmn:sequenceFlow id="Flow_1msh4mr" sourceRef="Gateway_0o5auw6" targetRef="Activity_1ufh8x7">
+      <bpmn:conditionExpression>result[&quot;returncode&quot;] != 0</bpmn:conditionExpression>
     </bpmn:sequenceFlow>
-    <bpmn:exclusiveGateway id="Gateway_0w96sv3">
-      <bpmn:incoming>Flow_1cn71yy</bpmn:incoming>
-      <bpmn:incoming>Flow_1iyvi2c</bpmn:incoming>
-      <bpmn:outgoing>Flow_0v4mach</bpmn:outgoing>
-    </bpmn:exclusiveGateway>
-    <bpmn:sequenceFlow id="Flow_0v4mach" sourceRef="Gateway_0w96sv3" targetRef="Event_1bsl2ov"/>
-    <bpmn:sequenceFlow id="Flow_1iyvi2c" sourceRef="Activity_1yt24dj" targetRef="Gateway_0w96sv3"/>
-    <bpmn:serviceTask id="Activity_1yt24dj" name="Delete selected branches">
+    <bpmn:serviceTask id="Activity_1wobbp0" name="Spawn a process">
       <bpmn:extensionElements>
         <spiffworkflow:serviceTaskOperator id="os/SpawnProcess" resultVariable="result">
           <spiffworkflow:parameters>
-            <spiffworkflow:parameter id="args" type="any" value="[&quot;git&quot;, &quot;branch&quot;, &quot;-D&quot;] + branches_to_delete"/>
+            <spiffworkflow:parameter id="args" type="any" value="spawn_args"/>
           </spiffworkflow:parameters>
         </spiffworkflow:serviceTaskOperator>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_1lxcorc</bpmn:incoming>
-      <bpmn:outgoing>Flow_1iyvi2c</bpmn:outgoing>
+      <bpmn:incoming>Flow_090xnqj</bpmn:incoming>
+      <bpmn:outgoing>Flow_1cl2vgj</bpmn:outgoing>
     </bpmn:serviceTask>
+    <bpmn:sequenceFlow id="Flow_0utbnx3" sourceRef="Activity_1ufh8x7" targetRef="Event_08pdzal"/>
+    <bpmn:endEvent id="Event_08pdzal">
+      <bpmn:incoming>Flow_0utbnx3</bpmn:incoming>
+    </bpmn:endEvent>
+    <bpmn:scriptTask id="Activity_1ufh8x7" name="unwrap">
+      <bpmn:incoming>Flow_1msh4mr</bpmn:incoming>
+      <bpmn:outgoing>Flow_0utbnx3</bpmn:outgoing>
+      <bpmn:script>import sys
+
+print(result[&quot;stderr&quot;], file=sys.stderr)
+exit(result[&quot;returncode&quot;])</bpmn:script>
+    </bpmn:scriptTask>
+    <bpmn:textAnnotation id="TextAnnotation_1gt83ai">
+      <bpmn:text>Not how i want to handle this but I might be in too deep with the subprocesses and what is supported.</bpmn:text>
+    </bpmn:textAnnotation>
+    <bpmn:association id="Association_1hdvgtw" sourceRef="Activity_1ufh8x7" targetRef="TextAnnotation_1gt83ai"/>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
-    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="delete_branches">
+    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="spawn_process">
+      <bpmndi:BPMNShape id="TextAnnotation_1gt83ai_di" bpmnElement="TextAnnotation_1gt83ai">
+        <dc:Bounds x="500" y="370" width="100" height="142"/>
+        <bpmndi:BPMNLabel/>
+      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
         <dc:Bounds x="179" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_1bsl2ov_di" bpmnElement="Event_1bsl2ov">
-        <dc:Bounds x="612" y="159" width="36" height="36"/>
+      <bpmndi:BPMNShape id="Gateway_0o5auw6_di" bpmnElement="Gateway_0o5auw6" isMarkerVisible="true">
+        <dc:Bounds x="425" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Gateway_1ltog1i_di" bpmnElement="Gateway_1ltog1i" isMarkerVisible="true">
-        <dc:Bounds x="245" y="152" width="50" height="50"/>
+      <bpmndi:BPMNShape id="Event_1vc03l8_di" bpmnElement="Event_1vc03l8">
+        <dc:Bounds x="532" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Gateway_0w96sv3_di" bpmnElement="Gateway_0w96sv3" isMarkerVisible="true">
-        <dc:Bounds x="535" y="152" width="50" height="50"/>
+      <bpmndi:BPMNShape id="Activity_1qk1mwi_di" bpmnElement="Activity_1wobbp0">
+        <dc:Bounds x="270" y="137" width="100" height="80"/>
+        <bpmndi:BPMNLabel/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Event_12c7q1f_di" bpmnElement="Event_08pdzal">
+        <dc:Bounds x="622" y="272" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_080uqjc_di" bpmnElement="Activity_1yt24dj">
-        <dc:Bounds x="360" y="200" width="100" height="80"/>
+      <bpmndi:BPMNShape id="Activity_1hcqe3e_di" bpmnElement="Activity_1ufh8x7">
+        <dc:Bounds x="480" y="250" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNEdge id="Flow_0ecta24_di" bpmnElement="Flow_0ecta24">
+      <bpmndi:BPMNEdge id="Association_1hdvgtw_di" bpmnElement="Association_1hdvgtw">
+        <di:waypoint x="538" y="330"/>
+        <di:waypoint x="547" y="370"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_090xnqj_di" bpmnElement="Flow_090xnqj">
         <di:waypoint x="215" y="177"/>
-        <di:waypoint x="245" y="177"/>
+        <di:waypoint x="270" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1cl2vgj_di" bpmnElement="Flow_1cl2vgj">
+        <di:waypoint x="370" y="177"/>
+        <di:waypoint x="425" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1gimdqy_di" bpmnElement="Flow_1gimdqy">
+        <di:waypoint x="475" y="177"/>
+        <di:waypoint x="532" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1msh4mr_di" bpmnElement="Flow_1msh4mr">
+        <di:waypoint x="450" y="202"/>
+        <di:waypoint x="450" y="290"/>
+        <di:waypoint x="480" y="290"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1lxcorc_di" bpmnElement="Flow_1lxcorc">
-        <di:waypoint x="270" y="202"/>
-        <di:waypoint x="270" y="240"/>
-        <di:waypoint x="360" y="240"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1cn71yy_di" bpmnElement="Flow_1cn71yy">
-        <di:waypoint x="295" y="177"/>
-        <di:waypoint x="535" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_0v4mach_di" bpmnElement="Flow_0v4mach">
-        <di:waypoint x="585" y="177"/>
-        <di:waypoint x="612" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1iyvi2c_di" bpmnElement="Flow_1iyvi2c">
-        <di:waypoint x="460" y="240"/>
-        <di:waypoint x="560" y="240"/>
-        <di:waypoint x="560" y="202"/>
+      <bpmndi:BPMNEdge id="Flow_0utbnx3_di" bpmnElement="Flow_0utbnx3">
+        <di:waypoint x="580" y="290"/>
+        <di:waypoint x="622" y="290"/>
       </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn`

 * *Files 2% similar despite different names*

#### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/deletion_prompt.bpmn`

```diff
@@ -44,27 +44,15 @@
     lines.append(&quot;&quot;)
     if comment:
         section_lines = map(lambda l: f&quot;# {l}&quot;, section_lines)
     lines.extend(section_lines)
     lines.append(&quot;&quot;)
 
 def build_branch_report():
-    if len(merged) == 0 and len(unmerged) == 0:
-        return &quot;&quot;
-    
-    lines = [
-        &quot;## git debranch&quot;,
-        &quot;##&quot;,
-        &quot;## Select branches to delete.&quot;,
-        &quot;##&quot;,
-        &quot;## Any lines that are non empty and do not start with a # are assumed to &quot;,
-        &quot;## be branch names, one per line. Each uncommented branch name will be &quot;,
-        &quot;## marked for deletion. HEAD and current branches are not shown.&quot;,
-        &quot;&quot;,
-    ]
+    lines = []
 
     merged_local_only = local_only(merged)
 
     add_section(lines, merged_local_only, False, [
         &quot;## The following branches appear safe to delete. They exist locally &quot;,
         &quot;## but not on any remote and have been merged:&quot;,
     ])
@@ -86,14 +74,26 @@
     unmerged_has_remote_branch = has_remote(unmerged)
 
     add_section(lines, unmerged_has_remote_branch, True, [
         &quot;## The following branches exist locally as well as on a remote and &quot;,
         &quot;## may not have been merged:&quot;,
     ])
 
+    if len(lines) &gt; 0:
+        lines = [
+            &quot;## git debranch&quot;,
+            &quot;##&quot;,
+            &quot;## Select branches to delete.&quot;,
+            &quot;##&quot;,
+            &quot;## Any lines that are non empty and do not start with a # are assumed to &quot;,
+            &quot;## be branch names, one per line. Each uncommented branch name will be &quot;,
+            &quot;## marked for deletion. HEAD and current branches are not shown.&quot;,
+            &quot;&quot;,
+        ] + lines
+
     return &quot;\n&quot;.join(lines)
 
 branch_report = build_branch_report()</bpmn:script>
     </bpmn:scriptTask>
     <bpmn:sequenceFlow id="Flow_0povx4i" sourceRef="confirm_deletion" targetRef="Gateway_1rx5xww"/>
     <bpmn:userTask id="confirm_deletion" name="Prompt for confirmation">
       <bpmn:incoming>Flow_0g02i6z</bpmn:incoming>
@@ -163,35 +163,35 @@
     </bpmn:scriptTask>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
     <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="deletion_prompt">
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
         <dc:Bounds x="179" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Event_185zs44_di" bpmnElement="Event_185zs44">
+        <dc:Bounds x="872" y="159" width="36" height="36"/>
+      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_0wzugcm_di" bpmnElement="Activity_1sjkjk0">
         <dc:Bounds x="270" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_185zs44_di" bpmnElement="Event_185zs44">
-        <dc:Bounds x="872" y="159" width="36" height="36"/>
+      <bpmndi:BPMNShape id="Activity_18aapsf_di" bpmnElement="confirm_deletion">
+        <dc:Bounds x="500" y="60" width="100" height="80"/>
+        <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_14dv693_di" bpmnElement="Activity_0a61ymz">
         <dc:Bounds x="730" y="137" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Gateway_008evke_di" bpmnElement="Gateway_008evke" isMarkerVisible="true">
         <dc:Bounds x="405" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Gateway_1rx5xww_di" bpmnElement="Gateway_1rx5xww" isMarkerVisible="true">
         <dc:Bounds x="635" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_18aapsf_di" bpmnElement="confirm_deletion">
-        <dc:Bounds x="500" y="60" width="100" height="80"/>
-        <bpmndi:BPMNLabel/>
-      </bpmndi:BPMNShape>
       <bpmndi:BPMNShape id="Activity_1lqxs1e_di" bpmnElement="Activity_00hkuxb">
         <dc:Bounds x="500" y="220" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
       <bpmndi:BPMNEdge id="Flow_0p7er6v_di" bpmnElement="Flow_0p7er6v">
         <di:waypoint x="215" y="177"/>
         <di:waypoint x="270" y="177"/>
```

### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/spawn.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn`

 * *Files 22% similar despite different names*

#### Comparing `git-debranch-0.1.5/src/git_debranch/bpmn/git-debranch/spawn.bpmn` & `git-debranch-0.1.6/src/git_debranch/bpmn/git-debranch/delete_branches.bpmn`

```diff
@@ -1,86 +1,135 @@
 <?xml version="1.0" encoding="utf-8"?>
-<bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
-  <bpmn:process id="spawn_process" name="Spawn a New Process" isExecutable="true">
+<bpmn:definitions xmlns:bpmn="http://www.omg.org/spec/BPMN/20100524/MODEL" xmlns:bpmndi="http://www.omg.org/spec/BPMN/20100524/DI" xmlns:dc="http://www.omg.org/spec/DD/20100524/DC" xmlns:di="http://www.omg.org/spec/DD/20100524/DI" xmlns:spiffworkflow="http://spiffworkflow.org/bpmn/schema/1.0/core" id="Definitions_96f6665" targetNamespace="http://bpmn.io/schema/bpmn" exporter="Camunda Modeler" exporterVersion="3.0.0-dev">
+  <bpmn:process id="delete_branches" isExecutable="true">
     <bpmn:startEvent id="StartEvent_1">
-      <bpmn:outgoing>Flow_090xnqj</bpmn:outgoing>
+      <bpmn:outgoing>Flow_0ecta24</bpmn:outgoing>
     </bpmn:startEvent>
-    <bpmn:sequenceFlow id="Flow_090xnqj" sourceRef="StartEvent_1" targetRef="Activity_1wobbp0"/>
-    <bpmn:exclusiveGateway id="Gateway_0o5auw6" default="Flow_1gimdqy">
-      <bpmn:incoming>Flow_1cl2vgj</bpmn:incoming>
-      <bpmn:outgoing>Flow_1gimdqy</bpmn:outgoing>
-      <bpmn:outgoing>Flow_1msh4mr</bpmn:outgoing>
-    </bpmn:exclusiveGateway>
-    <bpmn:sequenceFlow id="Flow_1cl2vgj" sourceRef="Activity_1wobbp0" targetRef="Gateway_0o5auw6"/>
-    <bpmn:endEvent id="Event_1vc03l8">
-      <bpmn:incoming>Flow_1gimdqy</bpmn:incoming>
+    <bpmn:sequenceFlow id="Flow_0ecta24" sourceRef="StartEvent_1" targetRef="Gateway_1ltog1i"/>
+    <bpmn:endEvent id="Event_1bsl2ov">
+      <bpmn:incoming>Flow_0v4mach</bpmn:incoming>
     </bpmn:endEvent>
-    <bpmn:sequenceFlow id="Flow_1gimdqy" sourceRef="Gateway_0o5auw6" targetRef="Event_1vc03l8"/>
-    <bpmn:sequenceFlow id="Flow_1msh4mr" sourceRef="Gateway_0o5auw6" targetRef="Event_08pdzal">
-      <bpmn:conditionExpression>result[&quot;returncode&quot;] != 0</bpmn:conditionExpression>
+    <bpmn:exclusiveGateway id="Gateway_1ltog1i" default="Flow_1lxcorc">
+      <bpmn:incoming>Flow_0ecta24</bpmn:incoming>
+      <bpmn:outgoing>Flow_1lxcorc</bpmn:outgoing>
+      <bpmn:outgoing>Flow_1cn71yy</bpmn:outgoing>
+    </bpmn:exclusiveGateway>
+    <bpmn:sequenceFlow id="Flow_1lxcorc" sourceRef="Gateway_1ltog1i" targetRef="Gateway_07vqtbt"/>
+    <bpmn:sequenceFlow id="Flow_1cn71yy" sourceRef="Gateway_1ltog1i" targetRef="Gateway_0w96sv3">
+      <bpmn:conditionExpression>len(branches_to_delete) == 0</bpmn:conditionExpression>
     </bpmn:sequenceFlow>
-    <bpmn:endEvent id="Event_08pdzal">
-      <bpmn:incoming>Flow_1msh4mr</bpmn:incoming>
-      <bpmn:terminateEventDefinition id="TerminateEventDefinition_16l45dq"/>
-    </bpmn:endEvent>
-    <bpmn:serviceTask id="Activity_1wobbp0" name="Spawn a process">
+    <bpmn:exclusiveGateway id="Gateway_0w96sv3">
+      <bpmn:incoming>Flow_1cn71yy</bpmn:incoming>
+      <bpmn:incoming>Flow_0b6k53w</bpmn:incoming>
+      <bpmn:outgoing>Flow_0v4mach</bpmn:outgoing>
+    </bpmn:exclusiveGateway>
+    <bpmn:sequenceFlow id="Flow_0v4mach" sourceRef="Gateway_0w96sv3" targetRef="Event_1bsl2ov"/>
+    <bpmn:sequenceFlow id="Flow_1iyvi2c" sourceRef="Activity_1yt24dj" targetRef="Gateway_1jb67dn"/>
+    <bpmn:serviceTask id="Activity_1yt24dj" name="Delete selected branches">
       <bpmn:extensionElements>
         <spiffworkflow:serviceTaskOperator id="os/SpawnProcess" resultVariable="result">
           <spiffworkflow:parameters>
-            <spiffworkflow:parameter id="args" type="any" value="spawn_args"/>
+            <spiffworkflow:parameter id="args" type="any" value="[&quot;git&quot;, &quot;branch&quot;, &quot;-D&quot;] + branches_to_delete"/>
           </spiffworkflow:parameters>
         </spiffworkflow:serviceTaskOperator>
       </bpmn:extensionElements>
-      <bpmn:incoming>Flow_090xnqj</bpmn:incoming>
-      <bpmn:outgoing>Flow_1cl2vgj</bpmn:outgoing>
+      <bpmn:incoming>Flow_0w5mz6n</bpmn:incoming>
+      <bpmn:outgoing>Flow_1iyvi2c</bpmn:outgoing>
     </bpmn:serviceTask>
-    <bpmn:textAnnotation id="TextAnnotation_0kuplex">
-      <bpmn:text>This behaves like spawn+unwrap. Maybe rename if reusing or make spawn_unwrap.bpmn</bpmn:text>
-    </bpmn:textAnnotation>
-    <bpmn:association id="Association_06bmaew" sourceRef="Gateway_0o5auw6" targetRef="TextAnnotation_0kuplex"/>
+    <bpmn:exclusiveGateway id="Gateway_07vqtbt" default="Flow_0w5mz6n">
+      <bpmn:incoming>Flow_1lxcorc</bpmn:incoming>
+      <bpmn:outgoing>Flow_0w5mz6n</bpmn:outgoing>
+      <bpmn:outgoing>Flow_00p4mau</bpmn:outgoing>
+    </bpmn:exclusiveGateway>
+    <bpmn:sequenceFlow id="Flow_0w5mz6n" sourceRef="Gateway_07vqtbt" targetRef="Activity_1yt24dj"/>
+    <bpmn:exclusiveGateway id="Gateway_1jb67dn">
+      <bpmn:incoming>Flow_1iyvi2c</bpmn:incoming>
+      <bpmn:incoming>Flow_12z8ned</bpmn:incoming>
+      <bpmn:outgoing>Flow_0b6k53w</bpmn:outgoing>
+    </bpmn:exclusiveGateway>
+    <bpmn:sequenceFlow id="Flow_0b6k53w" sourceRef="Gateway_1jb67dn" targetRef="Gateway_0w96sv3"/>
+    <bpmn:sequenceFlow id="Flow_00p4mau" sourceRef="Gateway_07vqtbt" targetRef="Activity_1n96cpz">
+      <bpmn:conditionExpression>dry_run</bpmn:conditionExpression>
+    </bpmn:sequenceFlow>
+    <bpmn:sequenceFlow id="Flow_12z8ned" sourceRef="Activity_1n96cpz" targetRef="Gateway_1jb67dn"/>
+    <bpmn:scriptTask id="Activity_1n96cpz" name="Show dry run results">
+      <bpmn:incoming>Flow_00p4mau</bpmn:incoming>
+      <bpmn:outgoing>Flow_12z8ned</bpmn:outgoing>
+      <bpmn:script>print(&quot;Skipping branch -D because --dry-run.\n\nWould have deleted:&quot;)
+
+for branch in branches_to_delete:
+    print(f&quot;\t{branch}&quot;)</bpmn:script>
+    </bpmn:scriptTask>
   </bpmn:process>
   <bpmndi:BPMNDiagram id="BPMNDiagram_1">
-    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="spawn_process">
+    <bpmndi:BPMNPlane id="BPMNPlane_1" bpmnElement="delete_branches">
       <bpmndi:BPMNShape id="_BPMNShape_StartEvent_2" bpmnElement="StartEvent_1">
         <dc:Bounds x="179" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Gateway_0o5auw6_di" bpmnElement="Gateway_0o5auw6" isMarkerVisible="true">
-        <dc:Bounds x="425" y="152" width="50" height="50"/>
+      <bpmndi:BPMNShape id="Event_1bsl2ov_di" bpmnElement="Event_1bsl2ov">
+        <dc:Bounds x="612" y="159" width="36" height="36"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_1vc03l8_di" bpmnElement="Event_1vc03l8">
-        <dc:Bounds x="532" y="159" width="36" height="36"/>
+      <bpmndi:BPMNShape id="Gateway_1ltog1i_di" bpmnElement="Gateway_1ltog1i" isMarkerVisible="true">
+        <dc:Bounds x="245" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Event_1vzcyjv_di" bpmnElement="Event_08pdzal">
-        <dc:Bounds x="532" y="272" width="36" height="36"/>
+      <bpmndi:BPMNShape id="Gateway_0w96sv3_di" bpmnElement="Gateway_0w96sv3" isMarkerVisible="true">
+        <dc:Bounds x="535" y="152" width="50" height="50"/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="Activity_1qk1mwi_di" bpmnElement="Activity_1wobbp0">
-        <dc:Bounds x="270" y="137" width="100" height="80"/>
+      <bpmndi:BPMNShape id="Activity_080uqjc_di" bpmnElement="Activity_1yt24dj">
+        <dc:Bounds x="370" y="210" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNShape id="TextAnnotation_0kuplex_di" bpmnElement="TextAnnotation_0kuplex">
-        <dc:Bounds x="480" y="-20" width="100" height="127"/>
+      <bpmndi:BPMNShape id="Gateway_07vqtbt_di" bpmnElement="Gateway_07vqtbt" isMarkerVisible="true">
+        <dc:Bounds x="295" y="285" width="50" height="50"/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Gateway_1jb67dn_di" bpmnElement="Gateway_1jb67dn" isMarkerVisible="true">
+        <dc:Bounds x="495" y="285" width="50" height="50"/>
+      </bpmndi:BPMNShape>
+      <bpmndi:BPMNShape id="Activity_15tqjgt_di" bpmnElement="Activity_1n96cpz">
+        <dc:Bounds x="370" y="330" width="100" height="80"/>
         <bpmndi:BPMNLabel/>
       </bpmndi:BPMNShape>
-      <bpmndi:BPMNEdge id="Flow_090xnqj_di" bpmnElement="Flow_090xnqj">
+      <bpmndi:BPMNEdge id="Flow_0ecta24_di" bpmnElement="Flow_0ecta24">
         <di:waypoint x="215" y="177"/>
-        <di:waypoint x="270" y="177"/>
+        <di:waypoint x="245" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1lxcorc_di" bpmnElement="Flow_1lxcorc">
+        <di:waypoint x="270" y="202"/>
+        <di:waypoint x="270" y="310"/>
+        <di:waypoint x="295" y="310"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1cn71yy_di" bpmnElement="Flow_1cn71yy">
+        <di:waypoint x="295" y="177"/>
+        <di:waypoint x="535" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_0v4mach_di" bpmnElement="Flow_0v4mach">
+        <di:waypoint x="585" y="177"/>
+        <di:waypoint x="612" y="177"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_1iyvi2c_di" bpmnElement="Flow_1iyvi2c">
+        <di:waypoint x="470" y="250"/>
+        <di:waypoint x="520" y="250"/>
+        <di:waypoint x="520" y="285"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_0w5mz6n_di" bpmnElement="Flow_0w5mz6n">
+        <di:waypoint x="320" y="285"/>
+        <di:waypoint x="320" y="250"/>
+        <di:waypoint x="370" y="250"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_0b6k53w_di" bpmnElement="Flow_0b6k53w">
+        <di:waypoint x="545" y="310"/>
+        <di:waypoint x="560" y="310"/>
+        <di:waypoint x="560" y="202"/>
+      </bpmndi:BPMNEdge>
+      <bpmndi:BPMNEdge id="Flow_00p4mau_di" bpmnElement="Flow_00p4mau">
+        <di:waypoint x="320" y="335"/>
+        <di:waypoint x="320" y="370"/>
+        <di:waypoint x="370" y="370"/>
       </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1cl2vgj_di" bpmnElement="Flow_1cl2vgj">
-        <di:waypoint x="370" y="177"/>
-        <di:waypoint x="425" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1gimdqy_di" bpmnElement="Flow_1gimdqy">
-        <di:waypoint x="475" y="177"/>
-        <di:waypoint x="532" y="177"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Flow_1msh4mr_di" bpmnElement="Flow_1msh4mr">
-        <di:waypoint x="450" y="202"/>
-        <di:waypoint x="450" y="290"/>
-        <di:waypoint x="532" y="290"/>
-      </bpmndi:BPMNEdge>
-      <bpmndi:BPMNEdge id="Association_06bmaew_di" bpmnElement="Association_06bmaew">
-        <di:waypoint x="458" y="160"/>
-        <di:waypoint x="480" y="107"/>
+      <bpmndi:BPMNEdge id="Flow_12z8ned_di" bpmnElement="Flow_12z8ned">
+        <di:waypoint x="470" y="370"/>
+        <di:waypoint x="520" y="370"/>
+        <di:waypoint x="520" y="335"/>
       </bpmndi:BPMNEdge>
     </bpmndi:BPMNPlane>
   </bpmndi:BPMNDiagram>
 </bpmn:definitions>
```

### Comparing `git-debranch-0.1.5/src/git_debranch/loader.py` & `git-debranch-0.1.6/src/git_debranch/loader.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.5/src/git_debranch/runner.py` & `git-debranch-0.1.6/src/git_debranch/runner.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.5/src/git_debranch/script_engine.py` & `git-debranch-0.1.6/src/git_debranch/script_engine.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.5/src/git_debranch/workflow.py` & `git-debranch-0.1.6/src/git_debranch/workflow.py`

 * *Files identical despite different names*

### Comparing `git-debranch-0.1.5/src/git_debranch.egg-info/PKG-INFO` & `git-debranch-0.1.6/src/git_debranch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-debranch
-Version: 0.1.5
+Version: 0.1.6
 Summary: Remove git branches
 Author: Jon Herron
 Author-email: jon.herron@yahoo.com
 License: lGPLv2
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,25 +15,39 @@
 
 ## Installation
 
 ```
 pip install git-debranch
 ```
 
-## Usage
+## Running
 
 ```
 git debranch
 ```
 
 From inside a git repository, running `git debranch` will present you with a list of branches that could 
 be deleted. This list is presented using `$EDITOR`. If the environment variable is not set `vi` is used 
 as the fallback.
 
-*Please note `git fetch -p` is run before the branch list is presented.*
+*Please note `git fetch -p` is run before the branch list is presented. This can be disabled by providing
+the --offline switch.*
+
+## Usage
+
+```
+usage: git debranch [-h] [--offline] [--dry-run]
+
+Delete local git branches
+
+options:
+  -h          show this help message and exit
+  --offline   Do not run online operations such as fetch and prune
+  --dry-run   Do not actually delete branches
+```
 
 ## Editing the Branch List
 
 When `$EDITOR` is invoked, it will contain a series of lines. Comment lines begin with `#` and any line that 
 is not empty or a comment is assumed to be the name of a branch to delete locally. You can update this list 
 by either removing or commenting branches that you want to keep. Branches that appear safe to delete are 
 uncommented by default. Branches that may not be safe to delete are left commented by default. When you save
```

### Comparing `git-debranch-0.1.5/src/git_debranch.egg-info/SOURCES.txt` & `git-debranch-0.1.6/src/git_debranch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

