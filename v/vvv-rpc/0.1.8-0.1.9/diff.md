# Comparing `tmp/vvv_rpc-0.1.8-py3-none-any.whl.zip` & `tmp/vvv_rpc-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3643 bytes, number of entries: 7
+Zip file size: 3664 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       34 b- defN 23-Feb-15 04:16 vvv_rpc/__init__.py
--rw-rw-rw-  2.0 fat     8583 b- defN 23-Mar-23 14:49 vvv_rpc/client.py
+-rw-rw-rw-  2.0 fat     8751 b- defN 23-Apr-04 11:25 vvv_rpc/client.py
 -rw-rw-rw-  2.0 fat      103 b- defN 19-Sep-25 12:29 vvv_rpc/xx.py
--rw-rw-rw-  2.0 fat      424 b- defN 23-Mar-23 15:01 vvv_rpc-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-23 15:01 vvv_rpc-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Mar-23 15:01 vvv_rpc-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      513 b- defN 23-Mar-23 15:01 vvv_rpc-0.1.8.dist-info/RECORD
-7 files, 9757 bytes uncompressed, 2735 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat      424 b- defN 23-Apr-04 11:25 vvv_rpc-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-04 11:25 vvv_rpc-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-04 11:25 vvv_rpc-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      513 b- defN 23-Apr-04 11:25 vvv_rpc-0.1.9.dist-info/RECORD
+7 files, 9925 bytes uncompressed, 2756 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: vvv_rpc/client.py
 Comment: 
 
 Filename: vvv_rpc/xx.py
 Comment: 
 
-Filename: vvv_rpc-0.1.8.dist-info/METADATA
+Filename: vvv_rpc-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: vvv_rpc-0.1.8.dist-info/WHEEL
+Filename: vvv_rpc-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: vvv_rpc-0.1.8.dist-info/top_level.txt
+Filename: vvv_rpc-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: vvv_rpc-0.1.8.dist-info/RECORD
+Filename: vvv_rpc-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vvv_rpc/client.py

```diff
@@ -106,14 +106,17 @@
         return self.post_interface(self.config_url, self.make_post_data({"size": "{},{}".format(w, h)}))
 
     def restart(self, auto_change_sec=None):
         data = self.make_post_data({"is_restart": True})
         if auto_change_sec: data['auto_change_sec'] = auto_change_sec
         return self.post_interface(self.config_url, data)
 
+    def auto_change_finger(self, auto_change_sec):
+        return self.post_interface(self.config_url, self.make_post_data({ "auto_change_sec": auto_change_sec }))
+
     def disabled_http_only(self, enable=True):
         return self.post_interface(self.config_url, self.make_post_data({ "disabled_http_only": enable }))
 
     def is_debugger(self, enable=True):
         return self.post_interface(self.config_url, self.make_post_data({ "is_debugger": enable }))
 
     def log_debugger(self, enable=True):
```

## Comparing `vvv_rpc-0.1.8.dist-info/RECORD` & `vvv_rpc-0.1.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 vvv_rpc/__init__.py,sha256=dpu61SgozWHF24eKa6v-dxc2uka0iROzBGbcOWjaPeo,34
-vvv_rpc/client.py,sha256=v4Yot54_qJGXpga6dTnJMOqKru-DshyCHklVsCH0CLc,8583
+vvv_rpc/client.py,sha256=QFF_19F6giU3B2OLStww55GY-jWULbHtusqMdJ9tabA,8751
 vvv_rpc/xx.py,sha256=X0esnw6KFoZ5KxGon9m4py39zrCofIjKng7pLScwOh4,103
-vvv_rpc-0.1.8.dist-info/METADATA,sha256=-I3zS96kpWAVlnHvtgmb5sudOVF8hGgvqu7DhYa8qCA,424
-vvv_rpc-0.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-vvv_rpc-0.1.8.dist-info/top_level.txt,sha256=vqJ765OgwBIgAg1qneB-jDZM0FQdNyd7MN-UzQmybP8,8
-vvv_rpc-0.1.8.dist-info/RECORD,,
+vvv_rpc-0.1.9.dist-info/METADATA,sha256=qtH7xJE69Fi1tdUKAkTwOBoeqGs5pvM0Sk64PLiJkts,424
+vvv_rpc-0.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+vvv_rpc-0.1.9.dist-info/top_level.txt,sha256=vqJ765OgwBIgAg1qneB-jDZM0FQdNyd7MN-UzQmybP8,8
+vvv_rpc-0.1.9.dist-info/RECORD,,
```

