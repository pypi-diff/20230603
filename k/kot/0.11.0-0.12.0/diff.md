# Comparing `tmp/kot-0.11.0.tar.gz` & `tmp/kot-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kot-0.11.0.tar", last modified: Thu Jun  1 14:59:59 2023, max compression
+gzip compressed data, was "kot-0.12.0.tar", last modified: Sat Jun  3 08:46:02 2023, max compression
```

## Comparing `kot-0.11.0.tar` & `kot-0.12.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:59:59.818257 kot-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-01 14:59:50.000000 kot-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-01 14:59:59.818257 kot-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-01 14:59:50.000000 kot-0.11.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:59:59.818257 kot-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-01 14:59:50.000000 kot-0.11.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:59:59.814257 kot-0.11.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:59:59.814257 kot-0.11.0/src/kot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 14:59:50.000000 kot-0.11.0/src/kot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-06-01 14:59:50.000000 kot-0.11.0/src/kot/kot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:59:59.818257 kot-0.11.0/src/kot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-01 14:59:59.000000 kot-0.11.0/src/kot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 14:59:59.000000 kot-0.11.0/src/kot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:59:59.000000 kot-0.11.0/src/kot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 14:59:59.000000 kot-0.11.0/src/kot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:59:59.000000 kot-0.11.0/src/kot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-01 14:59:59.000000 kot-0.11.0/src/kot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 14:59:59.000000 kot-0.11.0/src/kot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:46:02.250506 kot-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-03 08:45:49.000000 kot-0.12.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-03 08:46:02.250506 kot-0.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-03 08:45:49.000000 kot-0.12.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:46:02.250506 kot-0.12.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-03 08:45:49.000000 kot-0.12.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:46:02.246506 kot-0.12.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:46:02.250506 kot-0.12.0/src/kot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 08:45:49.000000 kot-0.12.0/src/kot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-03 08:45:49.000000 kot-0.12.0/src/kot/kot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 08:46:02.250506 kot-0.12.0/src/kot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-03 08:46:02.000000 kot-0.12.0/src/kot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-03 08:46:02.000000 kot-0.12.0/src/kot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:46:02.000000 kot-0.12.0/src/kot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 08:46:02.000000 kot-0.12.0/src/kot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 08:46:02.000000 kot-0.12.0/src/kot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-03 08:46:02.000000 kot-0.12.0/src/kot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-03 08:46:02.000000 kot-0.12.0/src/kot.egg-info/top_level.txt
```

### Comparing `kot-0.11.0/LICENSE` & `kot-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kot-0.11.0/PKG-INFO` & `kot-0.12.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.11.0
+Version: 0.12.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT | Multithreaded Simultaneous Writing Key-Value DB
         KOT is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -17,15 +17,15 @@
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
         - Able to encryption
         - Able to caching
         - Able to backup and restore
-        - Able to listing, deleting and deleting all databases
+        - Able to listing, deleting, deleting all and rename databases
         
         
         ## Installation
         You can install KOT by pip3:
         
         ```console
         pip3 install kot
```

### Comparing `kot-0.11.0/README.md` & `kot-0.12.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - Easy to deploy
 - Able to saving files
 - Able to compressing datas
 - Able to storing pyton objects (Pickle)
 - Able to encryption
 - Able to caching
 - Able to backup and restore
-- Able to listing, deleting and deleting all databases
+- Able to listing, deleting, deleting all and rename databases
 
 
 ## Installation
 You can install KOT by pip3:
 
 ```console
 pip3 install kot
```

### Comparing `kot-0.11.0/setup.py` & `kot-0.12.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='kot',
-version='0.11.0',
+version='0.12.0',
 description="""Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing""",
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 long_description_content_type='text/markdown',
 url='https://github.com/onuratakan/KOT',
 author='Onur Atakan ULUSOY',
 author_email='atadogan06@gmail.com',
 license='MIT',
@@ -14,11 +14,11 @@
 package_dir={'':'src'},
 install_requires=[
     "fire==0.5.0",
     "mgzip==0.2.1",
     "pycryptodome==3.18.0"
 ],
 entry_points = {
-    'console_scripts': ['kot=kot.kot:main'],
+    'console_scripts': ['KOT=kot.kot:main'],
 },
 python_requires=">= 3",
 zip_safe=False)
```

### Comparing `kot-0.11.0/src/kot/kot.py` & `kot-0.12.0/src/kot/kot.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,21 +20,68 @@
 from Crypto import Random
 from Crypto.Cipher import AES
 
 import traceback
 
 class KOT:
 
+
+    @staticmethod
+    def benchmark_set(number: int = 10000, compress: bool=False, encryption_key:str="") -> float:
+        my_db = KOT("KOT-benchmark", self_datas=True)
+        start = time.time()
+        for i in range(number):
+            my_db.set("key"+str(i), "value"+str(i), compress=compress, encryption_key=encryption_key)
+        end = time.time()
+        my_db.delete_all()
+        return end-start
+
+    @staticmethod
+    def benchmark_get(number: int = 10000, compress: bool=False, encryption_key:str="", dont_generate:bool=False) -> float:
+        my_db = KOT("KOT-benchmark", self_datas=True)
+        if not dont_generate:
+            for i in range(number):
+                my_db.set("key"+str(i), "value"+str(i), compress=compress, encryption_key=encryption_key)
+        start = time.time()
+        for i in range(number):
+            my_db.get("key"+str(i), encryption_key=encryption_key)
+        end = time.time()
+        my_db.delete_all()
+        return end-start    
+
+    @staticmethod
+    def benchmark_delete(number: int = 10000, compress: bool=False, encryption_key:str="", dont_generate:bool=False) -> float:
+        my_db = KOT("KOT-benchmark", self_datas=True)
+        if not dont_generate:
+            for i in range(number):
+                my_db.set("key"+str(i), "value"+str(i), compress=compress, encryption_key=encryption_key)
+        start = time.time()
+        for i in range(number):
+            my_db.delete("key"+str(i))
+        end = time.time()
+        my_db.delete_all()
+        return end-start   
+
+
+    @staticmethod
+    def benchmark(number: int = 10000, compress: bool=False, encryption_key:str="") -> float:
+        total_time = 0
+        total_time += KOT.benchmark_set(number, compress, encryption_key)
+        total_time += KOT.benchmark_get(number, compress, encryption_key, dont_generate=True)
+        total_time += KOT.benchmark_delete(number, compress, encryption_key, dont_generate=True)
+        return total_time
+
+
     @staticmethod
     def database_list() -> dict:
         database_index = KOT("KOT-database-index", self_datas=True)
         return database_index.dict()
     
     @staticmethod
-    def database_delete(name) -> bool:
+    def database_delete(name: str) -> bool:
         database_index = KOT("KOT-database-index", self_datas=True)
         try:
             rmtree(database_index.get(name))
         except:
             return False
         
         database_index.delete(name)
@@ -42,14 +89,31 @@
 
     @staticmethod
     def database_delete_all():
         database_index = KOT("KOT-database-index", self_datas=True)
         for each_database in database_index.dict():
             KOT.database_delete(each_database)
 
+
+    @staticmethod
+    def database_rename(name: str, new_name: str, force: bool=False) -> bool:
+        if new_name in KOT.database_list() and not force:
+            return False
+        try:
+            first_db = KOT(name)
+            location = first_db.backup(".")
+            KOT.database_delete(name)
+            second_db = KOT(new_name)
+            second_db.restore(location)
+            os.remove(location)
+        except:
+            traceback.print_exc()
+            return False
+        return True
+
     def __init__(self, name, self_datas: bool = False):
         self.name = name
         self.hashed_name = sha256(name.encode()).hexdigest()
         self.location = os.path.join(os.getcwd(), "KOT-" + self.hashed_name)
 
         if not self_datas:
             database_index = KOT("KOT-database-index", self_datas=True)
@@ -87,103 +151,121 @@
         def unpad(s):
             return s[:-ord(s[len(s)-1:])]
         message = base64.b64decode(message.encode())
         iv = message[:AES.block_size]
         cipher = AES.new(hashlib.sha256(key.encode()).digest(), AES.MODE_CBC, iv)
         return unpad(cipher.decrypt(message[AES.block_size:])).decode()
 
-    def set(self, key: str, value, type_of_value: str ="str", compress: bool=False, encryption_key:str="None", cache_policy: int = 0, dont_delete_cache: bool=False) -> str:
+    def set(self, key: str, value, type_of_value: str ="str", compress: bool=False, encryption_key:str="", cache_policy: int = 0, dont_delete_cache: bool=False) -> bool:
         self.counter += 1
         
-        
-
-
         if not isinstance(key, str):
             raise TypeError("Key must be a string")
 
-        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
-        key_location_loading = os.path.join(self.location, key_location+".l")
-        key_location_loading_indicator = os.path.join(self.location, key_location+".li")
+        try:
 
-        key_location_reading_indicator = os.path.join(self.location, key_location+".re")
-        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
-        if encryption_key != "None":
-            value = self.encrypt(encryption_key, value)
+            key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
+            key_location_loading = os.path.join(self.location, key_location+".l")
+            key_location_loading_indicator = os.path.join(self.location, key_location+".li")
 
-        the_dict = {"key":key,"value":value, "type":type}
+            key_location_reading_indicator = os.path.join(self.location, key_location+".re")
+            key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
-        if cache_policy != 0:
-            the_dict["cache_time"] = time.time()
-            the_dict["cache_policy"] = cache_policy
-        else:
-            if key in self.cache and not dont_delete_cache:
-                del self.cache[key]
+            if encryption_key != "":
+                value = self.encrypt(encryption_key, value)
 
+            the_dict = {"key":key,"value":value, "type":type_of_value}
 
-        if compress:
-            # create key_location_compress_indicator
-            with open(key_location_compress_indicator, "wb") as f:
-                f.write(b"1")
+            if cache_policy != 0:
+                the_dict["cache_time"] = time.time()
+                the_dict["cache_policy"] = cache_policy
+            else:
+                if key in self.cache and not dont_delete_cache:
+                    del self.cache[key]
 
-            with mgzip.open(key_location_loading, "wb") as f:
-                pickle.dump(the_dict, f)
-        
-        else:
-            with open(key_location_loading, "wb") as f:
-                pickle.dump(the_dict, f)
 
+            if compress:
+                # create key_location_compress_indicator
+                with open(key_location_compress_indicator, "wb") as f:
+                    f.write(b"1")
 
+                with mgzip.open(key_location_loading, "wb") as f:
+                    pickle.dump(the_dict, f)
+            
+            else:
+                with open(key_location_loading, "wb") as f:
+                    pickle.dump(the_dict, f)
 
 
-        #Create a file that inform is loading
-        with open(key_location_loading_indicator, "wb") as f:
-            f.write(b"1")
 
-        while os.path.exists(key_location_reading_indicator):
-                    time.sleep(0.25)
 
-        move(key_location_loading, key_location)
+            #Create a file that inform is loading
+            with open(key_location_loading_indicator, "wb") as f:
+                f.write(b"1")
 
-        #Remove the loading indicator
-        os.remove(key_location_loading_indicator)
+            while os.path.exists(key_location_reading_indicator):
+                        time.sleep(0.25)
 
-        return key
+            move(key_location_loading, key_location)
 
+            #Remove the loading indicator
+            os.remove(key_location_loading_indicator)
 
-    def set_withrkey(self, value, type_of_value="str") -> str:
-        key = str(self.counter) + str(time.time())
-        return self.set(key, value, type_of_value)
+        except:
+            traceback.print_exc()
+            return False
 
+        return True
 
-    def set_file(self, key: str, file, dont_remove: bool = False) -> str:
 
-        the_key = self.set(key, file, type_of_value="file")
-        key_name = self.get_file(key)
-        if not dont_remove:
-            move(file, os.path.join(self.location, key_name))
-        else:
-            copy(file, os.path.join(self.location, key_name))
+    def set_withrkey(self, value, type_of_value="str") -> str:
+        key = str(self.counter) + str(time.time())
+        try:
+            self.set(key, value, type_of_value)
+            return key
+        except:
+            traceback.print_exc()
+            return ""
+
 
-        return the_key
+    def set_file(self, key: str, file, dont_remove: bool = False) -> bool:
+        try:
+            the_key = self.set(key, file, type_of_value="file")
+            key_name = self.get_file(key)
+            if not dont_remove:
+                move(file, os.path.join(self.location, key_name))
+            else:
+                copy(file, os.path.join(self.location, key_name))
+        except:
+            traceback.print_exc()
+            return False
+        return True
 
 
     def set_file_withrkey(self, file, dont_remove: bool = False) -> str:
         key = str(self.counter) + str(time.time())
-        return self.set_file(key, file, dont_remove)
+        try:
+            self.set_file(key, file, dont_remove)
+            return key
+        except:
+            traceback.print_exc()
+            return ""
+
 
 
     def get_file(self, key: str, custom_key_location: str = ""):
         the_key = self.get(key,custom_key_location)
-        return the_key+the_key.split("/")[-1]
+        key_sha_256 = os.path.join(self.location, sha256(key.encode()).hexdigest())
+        return key_sha_256+"_"+the_key.split("/")[-1]
 
 
 
 
-    def get(self, key: str, custom_key_location: str = "", encryption_key:str="None", no_cache: bool = False):
+    def get(self, key: str, custom_key_location: str = "", encryption_key:str="", no_cache: bool = False, raw_dict:bool=False):
 
         if key in self.cache and not no_cache:
             cache_control = False
             currently = time.time()
             last_time = self.cache[key]["cache_time"]
             cache_policy = self.cache[key]["cache_policy"]
 
@@ -228,28 +310,40 @@
                     result = pickle.load(f)
                     total_result_standart = result
                     try:
                         total_result = result["value"]
                     except TypeError:
                         total_result = result
 
-            if encryption_key != "None":
+            if encryption_key != "":
                 total_result = self.decrypt(encryption_key, total_result)
 
             if "cache_time" in total_result_standart:
                 self.cache[key] = total_result_standart
 
         except EOFError or FileNotFoundError:
             pass
 
         if os.path.isfile(key_location_reading_indicator):
             os.remove(key_location_reading_indicator)
 
+        if raw_dict:
+            return total_result_standart
+
         return total_result
 
+
+    def get_key_type(self, key: str, custom_key_location: str = "") -> str:
+        result = self.get(key, custom_key_location, raw_dict=True)
+        if result is None:
+            return ""
+        if not "type" in result:
+            return ""
+        return result["type"]
+
     def get_key(self, key_location: str):
        
         key_location_compress_indicator = os.path.join(self.location, key_location+".co")
         if not os.path.isfile(os.path.join(self.location, key_location)):
             return None
         total_result = None
 
@@ -280,86 +374,132 @@
                         total_result = result["key"]
                     except TypeError:
                         total_result = False
         except EOFError or FileNotFoundError:
             pass            
         return total_result
 
-    def delete(self, key: str):
-        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
-
-        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
+    def delete(self, key: str) -> bool:
 
         try:
+            if key in self.cache:
+                del self.cache[key]            
+            key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
+            key_location_compress_indicator = os.path.join(self.location, key_location+".co")
+
             if os.path.exists(key_location_compress_indicator):
                 os.remove(os.path.join(self.location, key_location_compress_indicator))
-            os.remove(os.path.join(self.location, key_location))
-        except OSError:
-            pass
-
-    def delete_file(self, key: str):
+            if os.path.exists(os.path.join(self.location, key_location)):
+                os.remove(os.path.join(self.location, key_location))
+        except:
+            traceback.print_exc()
+            return False
         
+        return True
+
 
+    def delete_file(self, key: str) -> bool:
+        
+        
         try:
-            os.remove(os.path.join(self.location, self.get_file(key)))
-        except OSError:
-            pass
+            if os.path.exists(os.path.join(self.location, self.get_file(key))):
+                os.remove(os.path.join(self.location, self.get_file(key)))
+            
+        except:
+            traceback.print_exc()
+            return False
+
+
+        if self.delete(key):
+            return True
+        else:
+            return False
 
-        self.delete(key)
+        
         
 
-    def delete_all(self):
-        for key in self.dict():
-            self.delete(key)
+    def delete_all(self) -> bool:
+        try:
+            for key in self.dict():
+                self.delete(key)
+        except:
+            traceback.print_exc()
+            return False
+        return True
 
-    def dict(self, encryption_key:str="None"):
+    def dict(self, encryption_key:str=""):
         result ={}
         for key in os.listdir(self.location):
             if not "." in key:
                 the_key = self.get_key(key)
                 if not the_key is None:
                     if the_key != False:
                         result_of_key = self.get(the_key, encryption_key=encryption_key)
                         if not result_of_key is None:
                             result[the_key] = result_of_key
         return result
 
-    def size_all(self):
+    def size_all(self) -> int:
         #Calculate self.location size
         total_size = 0
 
         for dirpath, dirnames, filenames in os.walk(self.location):
             for f in filenames:
                 fp = os.path.join(dirpath, f)
                 total_size += os.path.getsize(fp)
 
         return total_size
     
-    def size(self, key: str):
-        key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
+    def size(self, key: str) -> int:
+        total_size = 0
+        try:
+            key_location = os.path.join(self.location, sha256(key.encode()).hexdigest())
+
+            key_location_compress_indicator = os.path.join(self.location, key_location+".co")
+
+            if os.path.exists(key_location_compress_indicator):
+                total_size += os.path.getsize(os.path.join(self.location, key_location+".co"))
+
+
+            total_size += os.path.getsize(os.path.join(self.location, key_location))
+        except:
+            traceback.print_exc()
+
+        return total_size
+
+
+    def size_file(self, key: str) -> int:
+        total_size = self.size(key)
+        try:
+            total_size += os.path.getsize(os.path.join(self.location, self.get_file(key)))
+        except:
+            traceback.print_exc()
+
+        return total_size
+    
 
-        key_location_compress_indicator = os.path.join(self.location, key_location+".co")
 
-        return os.path.getsize(os.path.join(self.location, key_location))
 
     def backup(self, backup_location: str) -> str:
         # create a name for backup that a date
         name = datetime.now().strftime("%Y_%m_%d_%H_%M_%S")
         location = os.path.join(backup_location, name)
         make_archive(location, 'zip', self.location)
         move(location+".zip", location+".KOT")
         return location+".KOT"
 
     def restore(self, backup_location: str) -> bool:
         try:
             move(backup_location, backup_location.replace(".KOT", ".zip"))
             backup_location = backup_location.replace(".KOT", ".zip")
             unpack_archive(backup_location, self.location)
+            move(backup_location, backup_location.replace(".zip", ".KOT"))
             return True
         except:
             traceback.print_exc()
             return False
 
 
 
+
 def main():
-    fire.Fire(KOT)    
+    fire.Fire(KOT)
```

### Comparing `kot-0.11.0/src/kot.egg-info/PKG-INFO` & `kot-0.12.0/src/kot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kot
-Version: 0.11.0
+Version: 0.12.0
 Summary: Efficient Key-Value Data Storage with Multithreaded Simultaneous Writing
 Home-page: https://github.com/onuratakan/KOT
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # KOT | Multithreaded Simultaneous Writing Key-Value DB
         KOT is an efficient key-value data storage system that aims to making simultaneous writing with multithreaded. 
@@ -17,15 +17,15 @@
         - Easy to deploy
         - Able to saving files
         - Able to compressing datas
         - Able to storing pyton objects (Pickle)
         - Able to encryption
         - Able to caching
         - Able to backup and restore
-        - Able to listing, deleting and deleting all databases
+        - Able to listing, deleting, deleting all and rename databases
         
         
         ## Installation
         You can install KOT by pip3:
         
         ```console
         pip3 install kot
```

