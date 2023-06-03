# Comparing `tmp/SecuriPy-1.1.0.tar.gz` & `tmp/SecuriPy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecuriPy-1.1.0.tar", last modified: Fri Jun  2 16:43:24 2023, max compression
+gzip compressed data, was "SecuriPy-1.1.1.tar", last modified: Sat Jun  3 17:22:05 2023, max compression
```

## Comparing `SecuriPy-1.1.0.tar` & `SecuriPy-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 16:43:24.351083 SecuriPy-1.1.0/
--rw-rw-rw-   0        0        0     3594 2023-06-02 16:43:24.346246 SecuriPy-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 16:43:24.340091 SecuriPy-1.1.0/SecuriPy.egg-info/
--rw-rw-rw-   0        0        0     3594 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 16:43:23.000000 SecuriPy-1.1.0/SecuriPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7336 2023-06-02 16:02:30.000000 SecuriPy-1.1.0/SecuriPy.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 16:43:24.351506 SecuriPy-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      879 2023-06-02 16:42:57.000000 SecuriPy-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 17:22:05.068348 SecuriPy-1.1.1/
+-rw-rw-rw-   0        0        0     3594 2023-06-03 17:22:05.066551 SecuriPy-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2998 2023-05-27 06:04:44.000000 SecuriPy-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 17:22:05.065042 SecuriPy-1.1.1/SecuriPy.egg-info/
+-rw-rw-rw-   0        0        0     3594 2023-06-03 17:22:04.000000 SecuriPy-1.1.1/SecuriPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      173 2023-06-03 17:22:04.000000 SecuriPy-1.1.1/SecuriPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 17:22:04.000000 SecuriPy-1.1.1/SecuriPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-03 17:22:04.000000 SecuriPy-1.1.1/SecuriPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6857 2023-06-03 17:21:28.000000 SecuriPy-1.1.1/SecuriPy.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 SecuriPy-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 17:22:05.068348 SecuriPy-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-06-03 17:21:37.000000 SecuriPy-1.1.1/setup.py
```

### Comparing `SecuriPy-1.1.0/PKG-INFO` & `SecuriPy-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.1.0/README.md` & `SecuriPy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `SecuriPy-1.1.0/SecuriPy.egg-info/PKG-INFO` & `SecuriPy-1.1.1/SecuriPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SecuriPy
-Version: 1.1.0
+Version: 1.1.1
 Summary: Encrypter and Decrypter of Readable messages Using Python
 Home-page: https://pypi.org/project/SecuriPy
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `SecuriPy-1.1.0/SecuriPy.py` & `SecuriPy-1.1.1/SecuriPy.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,99 +48,92 @@
             return "Message is corrupt or Password is incorrect"
 
 class Image:
     @staticmethod
     def Key():
         from cryptography.fernet import Fernet
         
+        key_value = Fernet.generate_key()
+        
         with open("key.txt","wb") as k:
-            k.write(Fernet.generate_key())
+            k.write(key_value)
+
+        with open("temp","wb") as k:
+            k.write(key_value)
             
     @staticmethod
-    def Encrypt(image_path):
-        import base64
+    def Encrypt(image_path, key_path):
         from cryptography.fernet import Fernet
         from PIL import Image
         from io import BytesIO
 
-        def image_to_base64(image_path):
-            with Image.open(image_path) as img:
-                buffer = BytesIO()
-                img.save(buffer, format=((image_path.split("."))[1].upper()))
-                img_data = buffer.getvalue()
-                base64_str = base64.b64encode(img_data).decode('utf-8')
-            return base64_str
-
         def encrypt_data(data, key):
             fernet = Fernet(key)
             encrypted_data = fernet.encrypt(data)
             return encrypted_data
 
         def image_to_encrypted_image(image_path, output_path):
             with Image.open(image_path) as img:
                 buffer = BytesIO()
                 img.save(buffer, format=((image_path.split("."))[1].upper()))
                 img_data = buffer.getvalue()
-            with open("key.txt","rb") as k:
+                
+            with open(key_path,"rb") as k:
                 key = k.read()
+                    
             encrypted_data = encrypt_data(img_data, key)
             with open(output_path, 'wb') as f:
                 f.write(encrypted_data)
 
-        # Replace 'path/to/your/image.jpg' with the actual path to your image file
-
-        # Convert the image to an encrypted image
-        # Replace 'path/to/your/new_image.jpg' with the desired path for the new image
-        new_image_path = image_path
-        encryption_key = image_to_encrypted_image(image_path, new_image_path)
+        encrypted_image_path = image_path
+        image_to_encrypted_image(image_path, encrypted_image_path)
         
     @staticmethod
-    def Decrypt(encrypted_image_path):
-        import base64
+    def Decrypt(encrypted_image_path, key_path):
         from cryptography.fernet import Fernet
-        from PIL import Image
-        from io import BytesIO
 
         def decrypt_data(encrypted_data, key):
             fernet = Fernet(key)
             decrypted_data = fernet.decrypt(encrypted_data)
             return decrypted_data
 
-        # Decrypt the encrypted image
-        with open("key.txt","rb") as k:
-            encryption_key = k.read()
-        with open(encrypted_image_path, 'rb') as f:
-            encrypted_data = f.read()
-        decrypted_data = decrypt_data(encrypted_data, encryption_key)
+        def encrypted_image_to_image(image_path, output_path):
+            with open(key_path,"rb") as k:
+                encryption_key = k.read()
+                    
+            with open(image_path, 'rb') as f:
+                encrypted_data = f.read()
+                
+            decrypted_data = decrypt_data(encrypted_data, encryption_key)
+            with open(output_path, 'wb') as f:
+                f.write(decrypted_data)
 
-        # Save the decrypted image as a new image
-        # Replace 'path/to/your/decrypted_image.jpg' with the desired path for the decrypted image
-        decrypted_image_path = encrypted_image_path
-        with open(decrypted_image_path, 'wb') as f:
-            f.write(decrypted_data)
+        
 
+        decrypted_image_path = encrypted_image_path
+        encrypted_image_to_image(encrypted_image_path, decrypted_image_path)
     @staticmethod
-    def EncryptAll():
+    def EncryptAll(key_path):
         import os
         images = os.listdir()
 
         for image in images:
             try:
-                Image.Encrypt(image)
+                Image.Encrypt(image, key_path)
             except:
                 pass
 
     @staticmethod
-    def DecryptAll():
+    def DecryptAll(key_path):
             import os
             images = os.listdir()
 
             for image in images:
                 try:
-                    Image.Decrypt(image)
+                    Image.Decrypt(image, key_path)
                 except:
                     pass
 
 class File:
     @staticmethod
     def Key():
         from cryptography.fernet import Fernet
```

### Comparing `SecuriPy-1.1.0/setup.py` & `SecuriPy-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SecuriPy",
-    version="1.1.0",
+    version="1.1.1",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Encrypter and Decrypter of Readable messages Using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/project/SecuriPy",
     project_urls={
```

