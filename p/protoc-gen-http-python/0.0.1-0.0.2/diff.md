# Comparing `tmp/protoc_gen_http_python-0.0.1-py3-none-any.whl.zip` & `tmp/protoc_gen_http_python-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10601 bytes, number of entries: 11
+Zip file size: 10550 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-02 16:17 protoc_gen_http_python/__init__.py
--rw-rw-rw-  2.0 fat     7253 b- defN 23-Jun-02 18:45 protoc_gen_http_python/http.py
--rw-rw-rw-  2.0 fat      952 b- defN 23-Jun-02 19:12 protoc_gen_http_python/main.py
+-rw-rw-rw-  2.0 fat     7008 b- defN 23-Jun-03 07:02 protoc_gen_http_python/http.py
+-rw-rw-rw-  2.0 fat      952 b- defN 23-Jun-03 07:16 protoc_gen_http_python/main.py
 -rw-rw-rw-  2.0 fat     4247 b- defN 23-Jun-02 18:54 protoc_gen_http_python/template.py
 -rw-rw-rw-  2.0 fat      688 b- defN 23-May-30 12:30 protoc_gen_http_python/util.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Jun-02 19:13 protoc_gen_http_python-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      495 b- defN 23-Jun-02 19:13 protoc_gen_http_python-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 19:13 protoc_gen_http_python-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       76 b- defN 23-Jun-02 19:13 protoc_gen_http_python-0.0.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-02 19:13 protoc_gen_http_python-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1009 b- defN 23-Jun-02 19:13 protoc_gen_http_python-0.0.1.dist-info/RECORD
-11 files, 26192 bytes uncompressed, 8849 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Jun-03 07:17 protoc_gen_http_python-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      495 b- defN 23-Jun-03 07:17 protoc_gen_http_python-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 07:17 protoc_gen_http_python-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       76 b- defN 23-Jun-03 07:17 protoc_gen_http_python-0.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-03 07:17 protoc_gen_http_python-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1009 b- defN 23-Jun-03 07:17 protoc_gen_http_python-0.0.2.dist-info/RECORD
+11 files, 25947 bytes uncompressed, 8798 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: protoc_gen_http_python/template.py
 Comment: 
 
 Filename: protoc_gen_http_python/util.py
 Comment: 
 
-Filename: protoc_gen_http_python-0.0.1.dist-info/LICENSE
+Filename: protoc_gen_http_python-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: protoc_gen_http_python-0.0.1.dist-info/METADATA
+Filename: protoc_gen_http_python-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: protoc_gen_http_python-0.0.1.dist-info/WHEEL
+Filename: protoc_gen_http_python-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: protoc_gen_http_python-0.0.1.dist-info/entry_points.txt
+Filename: protoc_gen_http_python-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: protoc_gen_http_python-0.0.1.dist-info/top_level.txt
+Filename: protoc_gen_http_python-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: protoc_gen_http_python-0.0.1.dist-info/RECORD
+Filename: protoc_gen_http_python-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## protoc_gen_http_python/http.py

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import List, Dict
+from typing import List, Dict, Union
 
 import google.api.annotations_pb2
 from google.protobuf.compiler.plugin_pb2 import CodeGeneratorResponse
 from google.protobuf.descriptor_pb2 import FileDescriptorProto, ServiceDescriptorProto, MethodDescriptorProto
 from google.protobuf.descriptor_pool import DescriptorPool
 from google.protobuf.descriptor import FileDescriptor
 from google.api.http_pb2 import HttpRule
@@ -103,22 +103,18 @@
 
     for method_desc in service_desc.methods:
         service_desc.uses.add(method_desc.request.use)
         service_desc.uses.add(method_desc.reply.use)
         if method_desc.body_type is not None:
             service_desc.uses.add(method_desc.body_type.use)
 
-    # if len(service_desc.methods) > 0:
-    #     s = {tuple(location.path): location for location in proto_file.source_code_info.location}
-    #     raise AttributeError(f'{s}')
-
     return service_desc
 
 
-def build_method(pool: DescriptorPool, m: MethodDescriptorProto) -> MethodDesc | None:
+def build_method(pool: DescriptorPool, m: MethodDescriptorProto) -> Union[MethodDesc, None]:
     http = m.options.Extensions[google.api.annotations_pb2.http]
     if http is {}:
         return None
 
     assert isinstance(http, HttpRule)
 
     method_desc = MethodDesc()
@@ -153,15 +149,14 @@
         path = http.patch
     else:
         if http.custom and http.custom.kind:
             method = http.custom.kind
             path = http.custom.path
         else:
             return None
-            # raise AttributeError(f'no http type in method {m.name}')
 
     method_desc.method = method
     method_desc.path = path
 
     body = http.body
     method_desc.body_type = None
     has_body = False
@@ -178,15 +173,14 @@
     if http.get or http.delete:
         if has_body:
             raise AttributeError(f'{method} {path} body should not be declared')
     else:
         if not has_body:
             raise AttributeError(f'{method} {path} does not declare a body')
 
-
     return method_desc
 
 
 def build_type(pool: DescriptorPool, type_full_name: str) -> TypeDesc:
     file_descriptor = pool.FindFileContainingSymbol(type_full_name)
     assert isinstance(file_descriptor, FileDescriptor)
```

## protoc_gen_http_python/main.py

```diff
@@ -4,15 +4,15 @@
 from google.protobuf.descriptor_pool import DescriptorPool
 
 if __package__ is None and not hasattr(sys, "frozen"):
     path = os.path.realpath(os.path.abspath(__file__))
     sys.path.insert(0, os.path.dirname(os.path.dirname(path)))
 from protoc_gen_http_python import http
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 def main() -> None:
     request = plugin.CodeGeneratorRequest.FromString(sys.stdin.buffer.read())
 
     response = plugin.CodeGeneratorResponse()
     response.supported_features = plugin.CodeGeneratorResponse.FEATURE_PROTO3_OPTIONAL
```

## Comparing `protoc_gen_http_python-0.0.1.dist-info/LICENSE` & `protoc_gen_http_python-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `protoc_gen_http_python-0.0.1.dist-info/RECORD` & `protoc_gen_http_python-0.0.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 protoc_gen_http_python/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-protoc_gen_http_python/http.py,sha256=kFVopFTSJ77DycMvmqTdscQ1HtnZsF2RDG9nMAqyo9w,7253
-protoc_gen_http_python/main.py,sha256=m_laIhD0cY4iNfcSeZK6ZPoIgQIlb5WQvGByji9OGnE,952
+protoc_gen_http_python/http.py,sha256=r18YUHvBnMBEt4teoiozZiH_cDHM3LEv4V_wNI4rqxE,7008
+protoc_gen_http_python/main.py,sha256=AF3lhzg_3HsubN2ExZYrPeZ-dKzT_85n01Ilk_sVrZA,952
 protoc_gen_http_python/template.py,sha256=4BBomDa_5uMhsALlz3lF2t3zQ475jYrucp9oPN57c80,4247
 protoc_gen_http_python/util.py,sha256=uJ6yPw3X4QNw8o9OFhpcdhQd23y681mjtAefHHwK3mM,688
-protoc_gen_http_python-0.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-protoc_gen_http_python-0.0.1.dist-info/METADATA,sha256=95t9j4CSrms-HmcdiZD1WRY5vozT62GQSwk9FMAvm4k,495
-protoc_gen_http_python-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-protoc_gen_http_python-0.0.1.dist-info/entry_points.txt,sha256=NhGgREmeCzfi_3n81KNxHUHQ9wXa0pPKZIKLdDr3i1w,76
-protoc_gen_http_python-0.0.1.dist-info/top_level.txt,sha256=nLRSViUlcCpKj02MpsM9KMizsBEzjuiMQjhz07aMA-4,23
-protoc_gen_http_python-0.0.1.dist-info/RECORD,,
+protoc_gen_http_python-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+protoc_gen_http_python-0.0.2.dist-info/METADATA,sha256=uNrp0GyhHVh560uO8i7cLBkPTtnEo5L5hy7Okkd2RIM,495
+protoc_gen_http_python-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+protoc_gen_http_python-0.0.2.dist-info/entry_points.txt,sha256=NhGgREmeCzfi_3n81KNxHUHQ9wXa0pPKZIKLdDr3i1w,76
+protoc_gen_http_python-0.0.2.dist-info/top_level.txt,sha256=nLRSViUlcCpKj02MpsM9KMizsBEzjuiMQjhz07aMA-4,23
+protoc_gen_http_python-0.0.2.dist-info/RECORD,,
```

