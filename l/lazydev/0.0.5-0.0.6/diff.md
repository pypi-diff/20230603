# Comparing `tmp/lazydev-0.0.5.tar.gz` & `tmp/lazydev-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.0.5.tar", last modified: Fri Jun  2 20:45:06 2023, max compression
+gzip compressed data, was "lazydev-0.0.6.tar", last modified: Fri Jun  2 22:13:42 2023, max compression
```

## Comparing `lazydev-0.0.5.tar` & `lazydev-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.456223 lazydev-0.0.5/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.5/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:45:06.456061 lazydev-0.0.5/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     3464 2023-06-02 18:29:53.000000 lazydev-0.0.5/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.453655 lazydev-0.0.5/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.5/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1247 2023-06-02 17:38:13.000000 lazydev-0.0.5/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.455689 lazydev-0.0.5/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.5/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     5694 2023-06-02 20:35:48.000000 lazydev-0.0.5/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     4520 2023-06-02 20:38:10.000000 lazydev-0.0.5/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.5/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.454790 lazydev-0.0.5/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 20:45:06.456260 lazydev-0.0.5/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 20:44:57.000000 lazydev-0.0.5/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.192264 lazydev-0.0.6/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.6/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4559 2023-06-02 22:13:42.192111 lazydev-0.0.6/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     3889 2023-06-02 22:13:23.000000 lazydev-0.0.6/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.189807 lazydev-0.0.6/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.6/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1280 2023-06-02 20:51:59.000000 lazydev-0.0.6/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.191686 lazydev-0.0.6/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.6/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     6177 2023-06-02 22:08:19.000000 lazydev-0.0.6/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4556 2023-06-02 21:07:12.000000 lazydev-0.0.6/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.6/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 22:13:42.190755 lazydev-0.0.6/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4559 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 22:13:42.000000 lazydev-0.0.6/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 22:13:42.192303 lazydev-0.0.6/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 22:09:23.000000 lazydev-0.0.6/setup.py
```

### Comparing `lazydev-0.0.5/LICENSE` & `lazydev-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.5/PKG-INFO` & `lazydev-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.5
+Version: 0.0.6
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,53 +12,68 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LazyDev: Automated Coding Project
+# LazyDev: Automating Coding Projects
 
-`Lazyness is the mother of invention`
+```
+Lazyness is the mother of invention 😉
+```
 
 LazyDev is a Python module that utilizes GPT models to create entire coding projects for you. With just a few simple commands, LazyDev can generate a project file tree, write the necessary code, and even test the project for you. Say goodbye to the hassle of setting up projects from scratch and let LazyDev do the heavy lifting for you.
 
 ## Features
 
 - **Effortless project initialization**: Simply use the `python -m lazydev.develop -r <what you want to do>` command to kickstart the project generation process.
 - **Interactive question-based approach**: LazyDev asks relevant questions to gather essential information before starting the coding process, ensuring that the generated project meets your specific requirements.
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
-```
+LazyDev requires Python 3.6 or above.
+```shell
 pip install lazydev
 ```
+### setup environment 
 
-LazyDev requires Python 3.6 or above.
+first setup your shell with openai api key in the environment. I would recommend  adding it to your ~/.bashrc
+```bash
+echo 'export OPENAI_API_KEY="your_openai_key"' >> ~/.bashrc && source ~/.bashrc
+```
+
+### for zsh users:
+```zsh
+echo 'export OPENAI_API_KEY="your_openai_key"' >> ~/.zshrc && source ~/.zshrc
+```
+
+Replace `your_openai_key` with your openai api key 
+ 
 
 ## Usage
 
 Using LazyDev is as simple as running a single command. Once installed, you can initiate the project generation process by executing the following command:
 
-```
-lazydev develop -r <what you want to do>
+```shell
+lazydev develop -r "what ever you want to do"
 ```
 
-Replace `<what you want to do>` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
+Replace `what ever you want to do` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
 
 After answering the questions, LazyDev will proceed to plan the project structure, create the appropriate file tree, generate the required code files, and even run tests to verify the functionality.
 
 ## Example
 
 Let's say you want to create a Python web application for managing a book library. You can use LazyDev to automate the project setup. Here's an example command:
 
-```
+```shell
 lazydev develop -r "Book Library Web App"
 ```
 
 LazyDev will ask you questions like:
 
 - What database system would you like to use?
 - What features would you like to include in your web app?
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lazydev-0.0.5/README.md` & `lazydev-0.0.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,61 @@
-# LazyDev: Automated Coding Project
+# LazyDev: Automating Coding Projects
 
-`Lazyness is the mother of invention`
+```
+Lazyness is the mother of invention 😉
+```
 
 LazyDev is a Python module that utilizes GPT models to create entire coding projects for you. With just a few simple commands, LazyDev can generate a project file tree, write the necessary code, and even test the project for you. Say goodbye to the hassle of setting up projects from scratch and let LazyDev do the heavy lifting for you.
 
 ## Features
 
 - **Effortless project initialization**: Simply use the `python -m lazydev.develop -r <what you want to do>` command to kickstart the project generation process.
 - **Interactive question-based approach**: LazyDev asks relevant questions to gather essential information before starting the coding process, ensuring that the generated project meets your specific requirements.
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
-```
+LazyDev requires Python 3.6 or above.
+```shell
 pip install lazydev
 ```
+### setup environment 
 
-LazyDev requires Python 3.6 or above.
+first setup your shell with openai api key in the environment. I would recommend  adding it to your ~/.bashrc
+```bash
+echo 'export OPENAI_API_KEY="your_openai_key"' >> ~/.bashrc && source ~/.bashrc
+```
+
+### for zsh users:
+```zsh
+echo 'export OPENAI_API_KEY="your_openai_key"' >> ~/.zshrc && source ~/.zshrc
+```
+
+Replace `your_openai_key` with your openai api key 
+ 
 
 ## Usage
 
 Using LazyDev is as simple as running a single command. Once installed, you can initiate the project generation process by executing the following command:
 
-```
-lazydev develop -r <what you want to do>
+```shell
+lazydev develop -r "what ever you want to do"
 ```
 
-Replace `<what you want to do>` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
+Replace `what ever you want to do` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
 
 After answering the questions, LazyDev will proceed to plan the project structure, create the appropriate file tree, generate the required code files, and even run tests to verify the functionality.
 
 ## Example
 
 Let's say you want to create a Python web application for managing a book library. You can use LazyDev to automate the project setup. Here's an example command:
 
-```
+```shell
 lazydev develop -r "Book Library Web App"
 ```
 
 LazyDev will ask you questions like:
 
 - What database system would you like to use?
 - What features would you like to include in your web app?
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lazydev-0.0.5/lazydev/develop.py` & `lazydev-0.0.6/lazydev/develop.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 
 def run(args):
 
     requirement = args.requirement
     directory= args.directory
     load_dotenv()
     api_key = os.environ.get('OPENAI_API_KEY')
-    developer =Developer(requirement=requirement,root_dir=directory,openai_api_key=api_key)
+    model=args.model
+    developer =Developer(requirement=requirement,root_dir=directory,openai_api_key=api_key,model=model)
     developer.develop()
```

### Comparing `lazydev-0.0.5/lazydev/modules/developer.py` & `lazydev-0.0.6/lazydev/modules/developer.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 )
 
 import json
 
 from .utils import Utilities
 
 class Developer():
-    def __init__(self, requirement:str,root_dir:str, openai_api_key:str):
+    def __init__(self, requirement:str,root_dir:str, openai_api_key:str,model:str):
         self.requirement=requirement
         self.root_dir=root_dir
         self.api_key=openai_api_key
         self.files_written=[]
         self.brain = ChatOpenAI(
-            model="gpt-3.5-turbo",
+            model=model,
             openai_api_key=self.api_key,
             temperature=0.1,
             streaming=False
             )
     
 
     def brain_storm(self,prompt:str,step_name="prompt")->str:
@@ -44,19 +44,31 @@
         if not os.path.exists("./thoughts"):
             os.makedirs("./thoughts")
         if os.path.exists(f"./thoughts/{step_name}.md"):
             os.remove(f"./thoughts/{step_name}.md")
         Utilities.write_to_file(f"{prompt}\n\n{aiMessage.content}",f"./thoughts/{step_name}.md")
         return aiMessage.content
     
-    def clear_doubts(self):
+    def get_doubts(self):
         prompt=PromptBook.expand_requirements(self.requirement)
         doubts=self.brain_storm(prompt,'clear-doubts')
         doubt_list:List[str]=doubts.split("\n")
         doubt_list=[doubt.strip() for doubt in doubt_list if doubt.strip()!=""]
+        return doubt_list
+    
+    def get_clarifications(self,doubts:List[str],answers:List[str]):
+        clarifications=""
+        for i in range(len(doubts)):
+            clarifications=f"{clarifications}\n\n{i+1}. {doubts[i]}\n Ans: {answers[i]}"
+        self.clarifications=clarifications
+        return clarifications
+    
+
+    def clear_doubts(self):
+        doubt_list=self.get_doubts()
         print("""
 Hey there! 😄 It's Lazy Dev, your friendly neighborhood programmer, here to make your awesome project's dreams come true! 🎉 
 But before I dive into coding magic, I have a few fun and important questions for you. 
 So, grab a cup of coffee ☕️, sit back, and let's clarify some details, shall we? Here we go! 🚀
         """)
         answer_list=[]
         for doubt in doubt_list:
@@ -69,41 +81,43 @@
 Sit back and relax while I work my coding magic for you! ✨✨✨
 
 🚀 I've got this! 🎉
 
 Cheers! 👨‍💻
         """)
         return doubt_list,answer_list
-
+    
     def plan_project(self):
         prompt=PromptBook.plan_project(self.requirement,self.clarifications)
         plannings:str=self.brain_storm(prompt,'plan-project')
+        self.plannings=plannings
         return plannings
     
     def generate_folder_structure(self):
         prompt=PromptBook.design_folder_structure(
             question=self.requirement,
             plan=self.plannings,
             clarifications=self.clarifications
             )
         retry_count=3
         while retry_count>0:
             try:
 
                 folder_tree_str:str=self.brain_storm(prompt,"generate-filders")
-                folder_tree:dict=json.loads(folder_tree_str)
+                folder_tree:dict=json.loads(folder_tree_str.strip().strip("`"))
                 break
             except:
                 print("Opps messed up the json format, let me try again")
                 retry_count=retry_count-1
         
         if retry_count==0:
             print("Sorry I was not able to create the folder structure in json correct format, check my instructions and try to refine it sothat i can understan the task better")
             sys.exit()       
         self.root_folder_name, self.file_paths = Utilities.generate_files_and_folders(structure=folder_tree,root_dir=self.root_dir)
+        return self.root_folder_name, self.file_paths
 
 
     def prioratize_files(self):
         prompt=PromptBook.prioritise_file_list(self.file_paths)
         retry_count=3
         while retry_count>0:
             try:
@@ -112,14 +126,15 @@
             except:
                 print("Opps messed up the json format, let me try again")
                 retry_count=retry_count-1
         if retry_count==0:
             print("Sorry I was not able to create the file list in correct format, check my instructions and try to refine it sothat i can understan the task better")
             sys.exit()       
         self.file_paths=file_paths_str.split("\n")
+        return self.file_paths
     
     def write_file_content(self,file_path):
         prompt=PromptBook.write_file(
             question=self.requirement,
             clarifications=self.clarifications,
             plan=self.plannings,
             files_written=self.files_written,
@@ -132,21 +147,20 @@
             file_path,
             code
         ))
 
     def develop(self):
         # clearing all doubts
         doubts,answers=self.clear_doubts()
-        self.clarifications:str=""
-        for i in range(len(doubts)):
-            self.clarifications=f"{self.clarifications}\n\n{i+1}. {doubts[i]}\n Ans: {answers[i]}"
-
+        self.clarifications=self.get_clarifications(doubts=doubts,answers=answers)
         # planning the project
         print("Planning...")
-        self.plannings=self.plan_project()
+        self.plan_project()
+        print(self.plannings)
+        print("\n\n")
         # creating files and folders for the project
         print("Creating files...")
         self.generate_folder_structure()
         self.prioratize_files()
         self.files_written=[]
         for file_path in self.file_paths:
             file_name=file_path.split("/")[-1]
```

### Comparing `lazydev-0.0.5/lazydev/modules/prompts.py` & `lazydev-0.0.6/lazydev/modules/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,9 +126,12 @@
 
 As your response will go to an automated parser, things to keep in mind all the time:
 * follow the exact format provided above without fail
 * only write the file content, no expiation, no pretext.
 * if the language support, add comments at steps, which expains what you are about to do, dont add comment if comment is not supported by the file type example json file
 * keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
 Begin!
+
+File:{file_path_to_write}
+Content:
 """
```

### Comparing `lazydev-0.0.5/lazydev/modules/utils.py` & `lazydev-0.0.6/lazydev/modules/utils.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.5/lazydev.egg-info/PKG-INFO` & `lazydev-0.0.6/lazydev.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.5
+Version: 0.0.6
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,53 +12,68 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# LazyDev: Automated Coding Project
+# LazyDev: Automating Coding Projects
 
-`Lazyness is the mother of invention`
+```
+Lazyness is the mother of invention 😉
+```
 
 LazyDev is a Python module that utilizes GPT models to create entire coding projects for you. With just a few simple commands, LazyDev can generate a project file tree, write the necessary code, and even test the project for you. Say goodbye to the hassle of setting up projects from scratch and let LazyDev do the heavy lifting for you.
 
 ## Features
 
 - **Effortless project initialization**: Simply use the `python -m lazydev.develop -r <what you want to do>` command to kickstart the project generation process.
 - **Interactive question-based approach**: LazyDev asks relevant questions to gather essential information before starting the coding process, ensuring that the generated project meets your specific requirements.
 - **Complete project planning**: LazyDev plans the entire project structure based on the gathered information, setting up the necessary directories and files for you.
 - **Automated code generation**: The module automatically generates the code based on the project plan, saving you time and effort.
 - **Built-in testing functionality**: LazyDev even includes an automated testing phase to ensure that the generated code performs as expected.
 
 ## Installation
 
-```
+LazyDev requires Python 3.6 or above.
+```shell
 pip install lazydev
 ```
+### setup environment 
 
-LazyDev requires Python 3.6 or above.
+first setup your shell with openai api key in the environment. I would recommend  adding it to your ~/.bashrc
+```bash
+echo 'export OPENAI_API_KEY="your_openai_key"' >> ~/.bashrc && source ~/.bashrc
+```
+
+### for zsh users:
+```zsh
+echo 'export OPENAI_API_KEY="your_openai_key"' >> ~/.zshrc && source ~/.zshrc
+```
+
+Replace `your_openai_key` with your openai api key 
+ 
 
 ## Usage
 
 Using LazyDev is as simple as running a single command. Once installed, you can initiate the project generation process by executing the following command:
 
-```
-lazydev develop -r <what you want to do>
+```shell
+lazydev develop -r "what ever you want to do"
 ```
 
-Replace `<what you want to do>` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
+Replace `what ever you want to do` with a brief description of your project's purpose or objective. LazyDev will then prompt you with a series of questions to gather the necessary information for project generation.
 
 After answering the questions, LazyDev will proceed to plan the project structure, create the appropriate file tree, generate the required code files, and even run tests to verify the functionality.
 
 ## Example
 
 Let's say you want to create a Python web application for managing a book library. You can use LazyDev to automate the project setup. Here's an example command:
 
-```
+```shell
 lazydev develop -r "Book Library Web App"
 ```
 
 LazyDev will ask you questions like:
 
 - What database system would you like to use?
 - What features would you like to include in your web app?
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lazydev-0.0.5/setup.py` & `lazydev-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
```

