# Comparing `tmp/git2vec-0.1.1.tar.gz` & `tmp/git2vec-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2vec-0.1.1.tar", last modified: Sat Jun  3 01:37:19 2023, max compression
+gzip compressed data, was "git2vec-0.1.2.tar", last modified: Sat Jun  3 12:00:22 2023, max compression
```

## Comparing `git2vec-0.1.1.tar` & `git2vec-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 01:37:19.001129 git2vec-0.1.1/
--rw-rw-rw-   0        0        0     2422 2023-06-03 01:37:19.001129 git2vec-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1768 2023-06-03 01:36:21.000000 git2vec-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 01:37:18.988987 git2vec-0.1.1/git2vec/
--rw-rw-rw-   0        0        0        0 2023-06-03 01:26:04.000000 git2vec-0.1.1/git2vec/__init__.py
--rw-rw-rw-   0        0        0     4594 2023-06-03 00:41:21.000000 git2vec-0.1.1/git2vec/loader.py
--rw-rw-rw-   0        0        0     3996 2023-06-03 00:41:21.000000 git2vec-0.1.1/git2vec/vectordb.py
-drwxrwxrwx   0        0        0        0 2023-06-03 01:37:18.999133 git2vec-0.1.1/git2vec.egg-info/
--rw-rw-rw-   0        0        0     2422 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 01:37:18.000000 git2vec-0.1.1/git2vec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 01:37:19.002126 git2vec-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-06-03 01:37:01.000000 git2vec-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:00:22.236302 git2vec-0.1.2/
+-rw-rw-rw-   0        0        0     2805 2023-06-03 12:00:22.235303 git2vec-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2151 2023-06-03 11:58:52.000000 git2vec-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 12:00:22.224911 git2vec-0.1.2/git2vec/
+-rw-rw-rw-   0        0        0        0 2023-06-03 01:26:04.000000 git2vec-0.1.2/git2vec/__init__.py
+-rw-rw-rw-   0        0        0     4660 2023-06-03 11:42:33.000000 git2vec-0.1.2/git2vec/loader.py
+-rw-rw-rw-   0        0        0     3996 2023-06-03 00:41:21.000000 git2vec-0.1.2/git2vec/vectordb.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:00:22.234304 git2vec-0.1.2/git2vec.egg-info/
+-rw-rw-rw-   0        0        0     2805 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 12:00:22.000000 git2vec-0.1.2/git2vec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:00:22.236302 git2vec-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-06-03 11:59:12.000000 git2vec-0.1.2/setup.py
```

### Comparing `git2vec-0.1.1/PKG-INFO` & `git2vec-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.1
+Version: 0.1.2
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Git2Vec
+# Git2Vec Repo
 
-Git2Vec is a text analysis tool that loads files from a Git repository, processes and embeds the text using OpenAI, and stores the embeddings in a Pinecone index for efficient retrieval and analysis.
+Git2Vec is a Python module that allows you to load text files from a Git repository and create a searchable vector database using Langchain, Pinecone, and OpenAI.
 
-## Dependencies
+## Installation
 
-The following packages are required to use Git2Vec:
+Install from https://pypi.org/project/git2vec/ using pip
 
-- langchain
-- pinecone-client
-- tiktoken
-- gitpython
-- turbo_docs
-- toml
-- setuptools
-- wheel
-- twine
+```bash
+pip install git2vec
+```
 
-Install them with the following commands:
+If cloned, you will need to install the following packages:
 
-```
+```bash
 pip install -r requirements.txt
-pip install -r requirements.dev.txt
 ```
 
-## Repo Structure
+If you are a developer, you will need to install the development requirements:
 
-- `exclude.toml`: Configuration file for excluding specific files for the `turbo_docs` package.
-- `requirements.dev.txt`: Development dependencies.
-- `requirements.txt`: Main dependencies.
-- `git2vec/loader.py`: Functions for loading documents from a Git repository using the TurboGitLoader class.
-- `git2vec/vectordb.py`: Functions for creating a Pinecone index, embedding documents and upserting them in the index.
+```bash
+pip install -r requirements.dev.txt
+```
 
 ## Usage
 
-1. First, create a Pinecone API key and save it as the `PINECONE_API_KEY` environment variable in your `.env` file.
-2. Create an OpenAI API key and save it as the `OPENAI_API_KEY` environment variable in your `.env` file.
-3. Load the Git repository data:
+### Loading a Git repository
+
+To load a Git repository, use the `git2vec.loader.load()` function:
 
 ```python
-from git2vec.loader import load
+from git2vec import loader
+
+repo_name = "https://github.com/voynow/turbo-docs"
 
-repo_data = load(repo="https://github.com/your/repository.git", branch="main")
+# Returns a list of Document objects
+repo_data = loader.load(repo_name)
+
+# Or return a string of all the raw text
+raw_repo = loader.load(repo_name, return_str=True)
 ```
 
-4. Create and insert embeddings into the Pinecone index:
+### Creating and managing a vector database
+
+To create a vector database from the loaded Git repository, use the following functions:
 
 ```python
-from git2vec.vectordb import create_vectorstore
+from git2vec import vectordb
 
-create_vectorstore(repo_data)
+# Create a vector store from the Git repo
+vectorstore = vectordb.create_vectorstore(repo_name)
+
+# Retrieve the vector store from Pinecone index
+vectorstore = vectordb.get_vectorstore()
 ```
 
-5. Get the Pinecone vector store instance for text retrieval:
+## Modules
 
-```python
-from git2vec.vectordb import get_vectorstore
+### loader.py
 
-vector_store = get_vectorstore()
-```
+The `loader.py` module contains the `TurboGitLoader` class which can be used to load text files from a Git repository. The `load()` function takes a repository URL and returns a list of `Document` objects or a string containing all the raw text.
+
+### vectordb.py
+
+The `vectordb.py` module provides functions to create and manage a vector database using Langchain, Pinecone, and OpenAI. It contains functions for initializing Pinecone, upserting data, processing data, embedding and upserting, creating a vectorstore, and retrieving a vectorstore.
+
+## Contributing
+
+If you find any issues or have any suggestions, feel free to open an issue or submit a pull request. We welcome any contributions!
+
+## License
 
-6. Use the vector store for information retrieval and analysis.
+This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `git2vec-0.1.1/git2vec/loader.py` & `git2vec-0.1.2/git2vec/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,32 +117,34 @@
             future_to_item = {executor.submit(self._load_file, item): item for item in repo.tree().traverse()}
             for future in concurrent.futures.as_completed(future_to_item):
                 doc = future.result()
                 if doc is not None:
                     docs.append(doc)
 
         return docs
+    
+
+def docs_to_str(repo_data):
+    """ Convert repo data to raw text """
+    raw_repo = ""
+    for item in repo_data:
+        if item.page_content:
+            raw_repo += f"{item.metadata['file_path']}:\n\n{item.page_content}\n\n"
+    return raw_repo
 
 
-def load(repo, branch="main"):
-    """ Load the git repo data using TurboGitLoader
-    """
-    print("Fetching data from git repo...")
+def load(repo, branch="main", return_str=False):
+    """ Load the git repo data using TurboGitLoader """
     folder_name = repo.split("/")[-1]
     filter_fn = lambda x: not any([x.endswith(t) for t in UNWANTED_TYPES])
 
-    gitdata = TurboGitLoader(
+    repo_docs = TurboGitLoader(
         clone_url=repo,
-        repo_path=f"./data/{folder_name}/",
+        repo_path=f"./repo_loader_data/{folder_name}/",
         branch=branch,
         file_filter=filter_fn,
     ).load()
 
-    return gitdata
-
-def repo_to_raw(repo_data):
-    """ Convert repo data to raw text """
-    raw_repo = ""
-    for item in repo_data:
-        if item.page_content:
-            raw_repo += f"{item.metadata['file_path']}:\n{item.page_content}\n\n"
-    return raw_repo
+    if return_str:
+        return docs_to_str(repo_docs)
+    else:
+        return repo_docs
```

### Comparing `git2vec-0.1.1/git2vec/vectordb.py` & `git2vec-0.1.2/git2vec/vectordb.py`

 * *Files identical despite different names*

### Comparing `git2vec-0.1.1/git2vec.egg-info/PKG-INFO` & `git2vec-0.1.2/git2vec.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 Metadata-Version: 2.1
 Name: git2vec
-Version: 0.1.1
+Version: 0.1.2
 Summary: A useful module for handling Git data.
 Home-page: https://github.com/voynow/git2vec
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Git2Vec
+# Git2Vec Repo
 
-Git2Vec is a text analysis tool that loads files from a Git repository, processes and embeds the text using OpenAI, and stores the embeddings in a Pinecone index for efficient retrieval and analysis.
+Git2Vec is a Python module that allows you to load text files from a Git repository and create a searchable vector database using Langchain, Pinecone, and OpenAI.
 
-## Dependencies
+## Installation
 
-The following packages are required to use Git2Vec:
+Install from https://pypi.org/project/git2vec/ using pip
 
-- langchain
-- pinecone-client
-- tiktoken
-- gitpython
-- turbo_docs
-- toml
-- setuptools
-- wheel
-- twine
+```bash
+pip install git2vec
+```
 
-Install them with the following commands:
+If cloned, you will need to install the following packages:
 
-```
+```bash
 pip install -r requirements.txt
-pip install -r requirements.dev.txt
 ```
 
-## Repo Structure
+If you are a developer, you will need to install the development requirements:
 
-- `exclude.toml`: Configuration file for excluding specific files for the `turbo_docs` package.
-- `requirements.dev.txt`: Development dependencies.
-- `requirements.txt`: Main dependencies.
-- `git2vec/loader.py`: Functions for loading documents from a Git repository using the TurboGitLoader class.
-- `git2vec/vectordb.py`: Functions for creating a Pinecone index, embedding documents and upserting them in the index.
+```bash
+pip install -r requirements.dev.txt
+```
 
 ## Usage
 
-1. First, create a Pinecone API key and save it as the `PINECONE_API_KEY` environment variable in your `.env` file.
-2. Create an OpenAI API key and save it as the `OPENAI_API_KEY` environment variable in your `.env` file.
-3. Load the Git repository data:
+### Loading a Git repository
+
+To load a Git repository, use the `git2vec.loader.load()` function:
 
 ```python
-from git2vec.loader import load
+from git2vec import loader
+
+repo_name = "https://github.com/voynow/turbo-docs"
 
-repo_data = load(repo="https://github.com/your/repository.git", branch="main")
+# Returns a list of Document objects
+repo_data = loader.load(repo_name)
+
+# Or return a string of all the raw text
+raw_repo = loader.load(repo_name, return_str=True)
 ```
 
-4. Create and insert embeddings into the Pinecone index:
+### Creating and managing a vector database
+
+To create a vector database from the loaded Git repository, use the following functions:
 
 ```python
-from git2vec.vectordb import create_vectorstore
+from git2vec import vectordb
 
-create_vectorstore(repo_data)
+# Create a vector store from the Git repo
+vectorstore = vectordb.create_vectorstore(repo_name)
+
+# Retrieve the vector store from Pinecone index
+vectorstore = vectordb.get_vectorstore()
 ```
 
-5. Get the Pinecone vector store instance for text retrieval:
+## Modules
 
-```python
-from git2vec.vectordb import get_vectorstore
+### loader.py
 
-vector_store = get_vectorstore()
-```
+The `loader.py` module contains the `TurboGitLoader` class which can be used to load text files from a Git repository. The `load()` function takes a repository URL and returns a list of `Document` objects or a string containing all the raw text.
+
+### vectordb.py
+
+The `vectordb.py` module provides functions to create and manage a vector database using Langchain, Pinecone, and OpenAI. It contains functions for initializing Pinecone, upserting data, processing data, embedding and upserting, creating a vectorstore, and retrieving a vectorstore.
+
+## Contributing
+
+If you find any issues or have any suggestions, feel free to open an issue or submit a pull request. We welcome any contributions!
+
+## License
 
-6. Use the vector store for information retrieval and analysis.
+This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `git2vec-0.1.1/setup.py` & `git2vec-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2vec',
-    version='0.1.1',
+    version='0.1.2',
     description='A useful module for handling Git data.',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2vec',
     packages=find_packages(),
     install_requires=[
         'langchain',
```

