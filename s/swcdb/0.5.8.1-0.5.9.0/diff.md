# Comparing `tmp/swcdb-0.5.8.1.tar.gz` & `tmp/swcdb-0.5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swcdb-0.5.8.1.tar", last modified: Thu Mar 17 14:41:23 2022, max compression
+gzip compressed data, was "dist/swcdb-0.5.9.0.tar", last modified: Sat May 21 21:29:01 2022, max compression
```

## Comparing `swcdb-0.5.8.1.tar` & `swcdb-0.5.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/
--rw-r--r--   0 root         (0) root         (0)      258 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1453 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/swcdb/
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-17 14:41:20.000000 swcdb-0.5.8.1/swcdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/swcdb/thrift/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/swcdb/thrift/native/
--rw-r--r--   0 root         (0) root         (0)   170353 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/native/Service.py
--rw-r--r--   0 root         (0) root         (0)       45 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/native/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/native/constants.py
--rw-r--r--   0 root         (0) root         (0)   188768 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/native/ttypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/swcdb/thrift/twisted/
--rw-r--r--   0 root         (0) root         (0)   194527 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/twisted/Service.py
--rw-r--r--   0 root         (0) root         (0)       45 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/twisted/__init__.py
--rw-r--r--   0 root         (0) root         (0)      384 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/twisted/constants.py
--rw-r--r--   0 root         (0) root         (0)   188776 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/twisted/ttypes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/swcdb/thrift/zopeif/
--rw-r--r--   0 root         (0) root         (0)   170331 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/zopeif/Service.py
--rw-r--r--   0 root         (0) root         (0)       45 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/zopeif/__init__.py
--rw-r--r--   0 root         (0) root         (0)      391 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/zopeif/constants.py
--rw-r--r--   0 root         (0) root         (0)   188783 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/zopeif/ttypes.py
--rw-r--r--   0 root         (0) root         (0)     7425 2022-03-17 14:41:20.000000 swcdb-0.5.8.1/swcdb/thrift/pool.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-17 14:41:20.000000 swcdb-0.5.8.1/swcdb/thrift/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1832 2022-03-17 14:41:20.000000 swcdb-0.5.8.1/swcdb/thrift/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-17 14:41:23.000000 swcdb-0.5.8.1/swcdb/thrift/tornado/
--rw-r--r--   0 root         (0) root         (0)   172513 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/tornado/Service.py
--rw-r--r--   0 root         (0) root         (0)       45 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/tornado/__init__.py
--rw-r--r--   0 root         (0) root         (0)      384 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/tornado/constants.py
--rw-r--r--   0 root         (0) root         (0)   188776 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/swcdb/thrift/tornado/ttypes.py
--rw-r--r--   0 root         (0) root         (0)     1102 2022-03-17 14:41:20.000000 swcdb-0.5.8.1/swcdb/serialization.py
--rw-r--r--   0 root         (0) root         (0)       71 2022-03-17 14:35:06.000000 swcdb-0.5.8.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     3811 2022-03-17 14:37:18.000000 swcdb-0.5.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/
+-rw-r--r--   0 root         (0) root         (0)      258 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1453 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/swcdb/
+-rw-r--r--   0 root         (0) root         (0)       38 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/swcdb/thrift/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/swcdb/thrift/native/
+-rw-r--r--   0 root         (0) root         (0)   170353 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/native/Service.py
+-rw-r--r--   0 root         (0) root         (0)       45 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/native/constants.py
+-rw-r--r--   0 root         (0) root         (0)   220391 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/native/ttypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/swcdb/thrift/twisted/
+-rw-r--r--   0 root         (0) root         (0)   194527 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/twisted/Service.py
+-rw-r--r--   0 root         (0) root         (0)       45 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/twisted/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      498 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/twisted/constants.py
+-rw-r--r--   0 root         (0) root         (0)   220399 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/twisted/ttypes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/swcdb/thrift/zopeif/
+-rw-r--r--   0 root         (0) root         (0)   170331 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/zopeif/Service.py
+-rw-r--r--   0 root         (0) root         (0)       45 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/zopeif/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      505 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/zopeif/constants.py
+-rw-r--r--   0 root         (0) root         (0)   220406 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/zopeif/ttypes.py
+-rw-r--r--   0 root         (0) root         (0)     7425 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/pool.py
+-rw-r--r--   0 root         (0) root         (0)       73 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-21 21:29:01.000000 swcdb-0.5.9.0/swcdb/thrift/tornado/
+-rw-r--r--   0 root         (0) root         (0)   172513 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/tornado/Service.py
+-rw-r--r--   0 root         (0) root         (0)       45 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/tornado/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      498 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/tornado/constants.py
+-rw-r--r--   0 root         (0) root         (0)   220399 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/thrift/tornado/ttypes.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/swcdb/serialization.py
+-rw-r--r--   0 root         (0) root         (0)       71 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     3948 2022-05-21 21:17:25.000000 swcdb-0.5.9.0/setup.py
```

### Comparing `swcdb-0.5.8.1/PKG-INFO` & `swcdb-0.5.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: swcdb
-Version: 0.5.8.1
+Version: 0.5.9.0
 Summary: The SWC-DB Python Package
 Home-page: https://github.com/kashirin-alex/swc-db
 Author: Kashirin Alex
 Author-email: kashirin.alex@gmail.com
 License: GPLv3
 Description:
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/native/Service.py` & `swcdb-0.5.9.0/swcdb/thrift/native/Service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1925,19 +1925,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype385, _size382) = iprot.readListBegin()
-                    for _i386 in range(_size382):
-                        _elem387 = Schema()
-                        _elem387.read(iprot)
-                        self.success.append(_elem387)
+                    (_etype413, _size410) = iprot.readListBegin()
+                    for _i414 in range(_size410):
+                        _elem415 = Schema()
+                        _elem415.read(iprot)
+                        self.success.append(_elem415)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -1951,16 +1951,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter388 in self.success:
-                iter388.write(oprot)
+            for iter416 in self.success:
+                iter416.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2092,19 +2092,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype392, _size389) = iprot.readListBegin()
-                    for _i393 in range(_size389):
-                        _elem394 = CompactResult()
-                        _elem394.read(iprot)
-                        self.success.append(_elem394)
+                    (_etype420, _size417) = iprot.readListBegin()
+                    for _i421 in range(_size417):
+                        _elem422 = CompactResult()
+                        _elem422.read(iprot)
+                        self.success.append(_elem422)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2118,16 +2118,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter395 in self.success:
-                iter395.write(oprot)
+            for iter423 in self.success:
+                iter423.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2418,20 +2418,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype397, _vtype398, _size396) = iprot.readMapBegin()
-                    for _i400 in range(_size396):
-                        _key401 = iprot.readString()
-                        _val402 = ColCells()
-                        _val402.read(iprot)
-                        self.success[_key401] = _val402
+                    (_ktype425, _vtype426, _size424) = iprot.readMapBegin()
+                    for _i428 in range(_size424):
+                        _key429 = iprot.readString()
+                        _val430 = ColCells()
+                        _val430.read(iprot)
+                        self.success[_key429] = _val430
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2445,17 +2445,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter403, viter404 in self.success.items():
-                oprot.writeString(kiter403)
-                viter404.write(oprot)
+            for kiter431, viter432 in self.success.items():
+                oprot.writeString(kiter431)
+                viter432.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2587,19 +2587,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype408, _size405) = iprot.readListBegin()
-                    for _i409 in range(_size405):
-                        _elem410 = kCells()
-                        _elem410.read(iprot)
-                        self.success.append(_elem410)
+                    (_etype436, _size433) = iprot.readListBegin()
+                    for _i437 in range(_size433):
+                        _elem438 = kCells()
+                        _elem438.read(iprot)
+                        self.success.append(_elem438)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2613,16 +2613,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter411 in self.success:
-                iter411.write(oprot)
+            for iter439 in self.success:
+                iter439.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3634,25 +3634,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype413, _vtype414, _size412) = iprot.readMapBegin()
-                    for _i416 in range(_size412):
-                        _key417 = iprot.readI64()
-                        _val418 = []
-                        (_etype422, _size419) = iprot.readListBegin()
-                        for _i423 in range(_size419):
-                            _elem424 = UCell()
-                            _elem424.read(iprot)
-                            _val418.append(_elem424)
+                    (_ktype441, _vtype442, _size440) = iprot.readMapBegin()
+                    for _i444 in range(_size440):
+                        _key445 = iprot.readI64()
+                        _val446 = []
+                        (_etype450, _size447) = iprot.readListBegin()
+                        for _i451 in range(_size447):
+                            _elem452 = UCell()
+                            _elem452.read(iprot)
+                            _val446.append(_elem452)
                         iprot.readListEnd()
-                        self.cells[_key417] = _val418
+                        self.cells[_key445] = _val446
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -3666,19 +3666,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter425, viter426 in self.cells.items():
-                oprot.writeI64(kiter425)
-                oprot.writeListBegin(TType.STRUCT, len(viter426))
-                for iter427 in viter426:
-                    iter427.write(oprot)
+            for kiter453, viter454 in self.cells.items():
+                oprot.writeI64(kiter453)
+                oprot.writeListBegin(TType.STRUCT, len(viter454))
+                for iter455 in viter454:
+                    iter455.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -3812,25 +3812,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype429, _vtype430, _size428) = iprot.readMapBegin()
-                    for _i432 in range(_size428):
-                        _key433 = iprot.readI64()
-                        _val434 = []
-                        (_etype438, _size435) = iprot.readListBegin()
-                        for _i439 in range(_size435):
-                            _elem440 = UCellSerial()
-                            _elem440.read(iprot)
-                            _val434.append(_elem440)
+                    (_ktype457, _vtype458, _size456) = iprot.readMapBegin()
+                    for _i460 in range(_size456):
+                        _key461 = iprot.readI64()
+                        _val462 = []
+                        (_etype466, _size463) = iprot.readListBegin()
+                        for _i467 in range(_size463):
+                            _elem468 = UCellSerial()
+                            _elem468.read(iprot)
+                            _val462.append(_elem468)
                         iprot.readListEnd()
-                        self.cells[_key433] = _val434
+                        self.cells[_key461] = _val462
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -3844,19 +3844,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_serial_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter441, viter442 in self.cells.items():
-                oprot.writeI64(kiter441)
-                oprot.writeListBegin(TType.STRUCT, len(viter442))
-                for iter443 in viter442:
-                    iter443.write(oprot)
+            for kiter469, viter470 in self.cells.items():
+                oprot.writeI64(kiter469)
+                oprot.writeListBegin(TType.STRUCT, len(viter470))
+                for iter471 in viter470:
+                    iter471.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -4224,19 +4224,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype447, _size444) = iprot.readListBegin()
-                    for _i448 in range(_size444):
-                        _elem449 = Schema()
-                        _elem449.read(iprot)
-                        self.success.append(_elem449)
+                    (_etype475, _size472) = iprot.readListBegin()
+                    for _i476 in range(_size472):
+                        _elem477 = Schema()
+                        _elem477.read(iprot)
+                        self.success.append(_elem477)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4250,16 +4250,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter450 in self.success:
-                iter450.write(oprot)
+            for iter478 in self.success:
+                iter478.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4392,19 +4392,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype454, _size451) = iprot.readListBegin()
-                    for _i455 in range(_size451):
-                        _elem456 = CompactResult()
-                        _elem456.read(iprot)
-                        self.success.append(_elem456)
+                    (_etype482, _size479) = iprot.readListBegin()
+                    for _i483 in range(_size479):
+                        _elem484 = CompactResult()
+                        _elem484.read(iprot)
+                        self.success.append(_elem484)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4418,16 +4418,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter457 in self.success:
-                iter457.write(oprot)
+            for iter485 in self.success:
+                iter485.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4720,20 +4720,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype459, _vtype460, _size458) = iprot.readMapBegin()
-                    for _i462 in range(_size458):
-                        _key463 = iprot.readString()
-                        _val464 = ColCells()
-                        _val464.read(iprot)
-                        self.success[_key463] = _val464
+                    (_ktype487, _vtype488, _size486) = iprot.readMapBegin()
+                    for _i490 in range(_size486):
+                        _key491 = iprot.readString()
+                        _val492 = ColCells()
+                        _val492.read(iprot)
+                        self.success[_key491] = _val492
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4747,17 +4747,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter465, viter466 in self.success.items():
-                oprot.writeString(kiter465)
-                viter466.write(oprot)
+            for kiter493, viter494 in self.success.items():
+                oprot.writeString(kiter493)
+                viter494.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4890,19 +4890,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype470, _size467) = iprot.readListBegin()
-                    for _i471 in range(_size467):
-                        _elem472 = kCells()
-                        _elem472.read(iprot)
-                        self.success.append(_elem472)
+                    (_etype498, _size495) = iprot.readListBegin()
+                    for _i499 in range(_size495):
+                        _elem500 = kCells()
+                        _elem500.read(iprot)
+                        self.success.append(_elem500)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4916,16 +4916,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter473 in self.success:
-                iter473.write(oprot)
+            for iter501 in self.success:
+                iter501.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/native/ttypes.py` & `swcdb-0.5.9.0/swcdb/thrift/native/ttypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,14 +246,41 @@
 
     _NAMES_TO_VALUES = {
         "UPDATING": 4,
         "DELETING": 8,
     }
 
 
+class UpdateOP(object):
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    SERIAL = 5
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "SERIAL",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "SERIAL": 5,
+    }
+
+
 class Flag(object):
     """
     The Cell Flag
 
     """
     NONE = 0
     INSERT = 1
@@ -271,14 +298,79 @@
         "NONE": 0,
         "INSERT": 1,
         "DELETE_LE": 2,
         "DELETE_EQ": 3,
     }
 
 
+class FU_MATH_OP(object):
+    """
+    MATH Operations for Serial Field Update of types INT64 and DOUBLE
+
+    """
+    EQUAL = 0
+    PLUS = 1
+    MULTIPLY = 2
+    DIVIDE = 3
+
+    _VALUES_TO_NAMES = {
+        0: "EQUAL",
+        1: "PLUS",
+        2: "MULTIPLY",
+        3: "DIVIDE",
+    }
+
+    _NAMES_TO_VALUES = {
+        "EQUAL": 0,
+        "PLUS": 1,
+        "MULTIPLY": 2,
+        "DIVIDE": 3,
+    }
+
+
+class FU_LIST_OP(object):
+    """
+    LIST Operations for Serial Field Update of array/list/bytes with LIST-op in the inner SERIAL fields
+
+    """
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    ERASE = 5
+    BY_UNIQUE = 6
+    BY_COND = 7
+    BY_INDEX = 8
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "ERASE",
+        6: "BY_UNIQUE",
+        7: "BY_COND",
+        8: "BY_INDEX",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "ERASE": 5,
+        "BY_UNIQUE": 6,
+        "BY_COND": 7,
+        "BY_INDEX": 8,
+    }
+
+
 class CellsResult(object):
     """
     The Cells Results types for using with CellsGroup requests
 
     """
     IN_LIST = 0
     ON_COLUMN = 1
@@ -1519,36 +1611,119 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class SpecUpdateOP(object):
+    """
+    Attributes:
+     - op: The Operation of update
+     - pos: The position/index of INSERT and OVERWRITE update operations
+
+    """
+
+    __slots__ = (
+        'op',
+        'pos',
+    )
+
+
+    def __init__(self, op=None, pos=None,):
+        self.op = op
+        self.pos = pos
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('SpecUpdateOP')
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 1)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 2)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class SpecIntervalUpdate(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecInterval
 
     Attributes:
      - v: The value for the updated cell
      - ts: The timestamp for the updated cell NULL: MIN_INT64+1, AUTO:MIN_INT64+2 (or not-set)
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'v',
         'ts',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, v=None, ts=None, encoder=None,):
+    def __init__(self, v=None, ts=None, encoder=None, update_op=None,):
         self.v = v
         self.ts = ts
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1566,14 +1741,20 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1588,14 +1769,18 @@
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 3)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 4)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1619,30 +1804,36 @@
 
 class SpecIntervalUpdateSerial(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecIntervalSerial
 
     Attributes:
      - ts: The timestamp for the updated cell NULL: MIN_INT64-1, AUTO:MIN_INT64-1
-     - v: The value for the updated cell
+     - v: The values of serial-fields for the updated cell
+     - v_op: The values of serial-fields for the the SERIAL operation update
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'ts',
         'v',
+        'v_op',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, ts=None, v=None, encoder=None,):
+    def __init__(self, ts=None, v=None, v_op=None, encoder=None, update_op=None,):
         self.ts = ts
         self.v = v
+        self.v_op = v_op
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1662,18 +1853,35 @@
                         _elem54 = CellValueSerial()
                         _elem54.read(iprot)
                         self.v.append(_elem54)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
+                if ftype == TType.LIST:
+                    self.v_op = []
+                    (_etype58, _size55) = iprot.readListBegin()
+                    for _i59 in range(_size55):
+                        _elem60 = CellValueSerialOp()
+                        _elem60.read(iprot)
+                        self.v_op.append(_elem60)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1683,22 +1891,33 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 1)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter55 in self.v:
-                iter55.write(oprot)
+            for iter61 in self.v:
+                iter61.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_op is not None:
+            oprot.writeFieldBegin('v_op', TType.LIST, 3)
+            oprot.writeListBegin(TType.STRUCT, len(self.v_op))
+            for iter62 in self.v_op:
+                iter62.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
-            oprot.writeFieldBegin('encoder', TType.I32, 3)
+            oprot.writeFieldBegin('encoder', TType.I32, 4)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 5)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1775,65 +1994,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype59, _size56) = iprot.readListBegin()
-                    for _i60 in range(_size56):
-                        _elem61 = iprot.readBinary()
-                        self.range_begin.append(_elem61)
+                    (_etype66, _size63) = iprot.readListBegin()
+                    for _i67 in range(_size63):
+                        _elem68 = iprot.readBinary()
+                        self.range_begin.append(_elem68)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype65, _size62) = iprot.readListBegin()
-                    for _i66 in range(_size62):
-                        _elem67 = iprot.readBinary()
-                        self.range_end.append(_elem67)
+                    (_etype72, _size69) = iprot.readListBegin()
+                    for _i73 in range(_size69):
+                        _elem74 = iprot.readBinary()
+                        self.range_end.append(_elem74)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype71, _size68) = iprot.readListBegin()
-                    for _i72 in range(_size68):
-                        _elem73 = iprot.readBinary()
-                        self.offset_key.append(_elem73)
+                    (_etype78, _size75) = iprot.readListBegin()
+                    for _i79 in range(_size75):
+                        _elem80 = iprot.readBinary()
+                        self.offset_key.append(_elem80)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype77, _size74) = iprot.readListBegin()
-                    for _i78 in range(_size74):
-                        _elem79 = SpecKeyInterval()
-                        _elem79.read(iprot)
-                        self.key_intervals.append(_elem79)
+                    (_etype84, _size81) = iprot.readListBegin()
+                    for _i85 in range(_size81):
+                        _elem86 = SpecKeyInterval()
+                        _elem86.read(iprot)
+                        self.key_intervals.append(_elem86)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype83, _size80) = iprot.readListBegin()
-                    for _i84 in range(_size80):
-                        _elem85 = SpecValue()
-                        _elem85.read(iprot)
-                        self.values.append(_elem85)
+                    (_etype90, _size87) = iprot.readListBegin()
+                    for _i91 in range(_size87):
+                        _elem92 = SpecValue()
+                        _elem92.read(iprot)
+                        self.values.append(_elem92)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -1871,48 +2090,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecInterval')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter86 in self.range_begin:
-                oprot.writeBinary(iter86)
+            for iter93 in self.range_begin:
+                oprot.writeBinary(iter93)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter87 in self.range_end:
-                oprot.writeBinary(iter87)
+            for iter94 in self.range_end:
+                oprot.writeBinary(iter94)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter88 in self.offset_key:
-                oprot.writeBinary(iter88)
+            for iter95 in self.offset_key:
+                oprot.writeBinary(iter95)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter89 in self.key_intervals:
-                iter89.write(oprot)
+            for iter96 in self.key_intervals:
+                iter96.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter90 in self.values:
-                iter90.write(oprot)
+            for iter97 in self.values:
+                iter97.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -1989,19 +2208,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype94, _size91) = iprot.readListBegin()
-                    for _i95 in range(_size91):
-                        _elem96 = SpecInterval()
-                        _elem96.read(iprot)
-                        self.intervals.append(_elem96)
+                    (_etype101, _size98) = iprot.readListBegin()
+                    for _i102 in range(_size98):
+                        _elem103 = SpecInterval()
+                        _elem103.read(iprot)
+                        self.intervals.append(_elem103)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2014,16 +2233,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter97 in self.intervals:
-                iter97.write(oprot)
+            for iter104 in self.intervals:
+                iter104.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2326,19 +2545,19 @@
                 if ftype == TType.I32:
                     self.seq = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype101, _size98) = iprot.readListBegin()
-                    for _i102 in range(_size98):
-                        _elem103 = SpecFraction()
-                        _elem103.read(iprot)
-                        self.v.append(_elem103)
+                    (_etype108, _size105) = iprot.readListBegin()
+                    for _i109 in range(_size105):
+                        _elem110 = SpecFraction()
+                        _elem110.read(iprot)
+                        self.v.append(_elem110)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2351,16 +2570,16 @@
         if self.seq is not None:
             oprot.writeFieldBegin('seq', TType.I32, 1)
             oprot.writeI32(self.seq)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter104 in self.v:
-                iter104.write(oprot)
+            for iter111 in self.v:
+                iter111.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2417,19 +2636,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype108, _size105) = iprot.readListBegin()
-                    for _i109 in range(_size105):
-                        _elem110 = SpecValueSerial_INT64()
-                        _elem110.read(iprot)
-                        self.v.append(_elem110)
+                    (_etype115, _size112) = iprot.readListBegin()
+                    for _i116 in range(_size112):
+                        _elem117 = SpecValueSerial_INT64()
+                        _elem117.read(iprot)
+                        self.v.append(_elem117)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2442,16 +2661,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter111 in self.v:
-                iter111.write(oprot)
+            for iter118 in self.v:
+                iter118.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2508,19 +2727,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype115, _size112) = iprot.readListBegin()
-                    for _i116 in range(_size112):
-                        _elem117 = SpecValueSerial_BYTES()
-                        _elem117.read(iprot)
-                        self.v.append(_elem117)
+                    (_etype122, _size119) = iprot.readListBegin()
+                    for _i123 in range(_size119):
+                        _elem124 = SpecValueSerial_BYTES()
+                        _elem124.read(iprot)
+                        self.v.append(_elem124)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2533,16 +2752,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter118 in self.v:
-                iter118.write(oprot)
+            for iter125 in self.v:
+                iter125.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2745,19 +2964,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.fields = []
-                    (_etype122, _size119) = iprot.readListBegin()
-                    for _i123 in range(_size119):
-                        _elem124 = SpecValueSerialField()
-                        _elem124.read(iprot)
-                        self.fields.append(_elem124)
+                    (_etype129, _size126) = iprot.readListBegin()
+                    for _i130 in range(_size126):
+                        _elem131 = SpecValueSerialField()
+                        _elem131.read(iprot)
+                        self.fields.append(_elem131)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2770,16 +2989,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.fields is not None:
             oprot.writeFieldBegin('fields', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.fields))
-            for iter125 in self.fields:
-                iter125.write(oprot)
+            for iter132 in self.fields:
+                iter132.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2858,65 +3077,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype129, _size126) = iprot.readListBegin()
-                    for _i130 in range(_size126):
-                        _elem131 = iprot.readBinary()
-                        self.range_begin.append(_elem131)
+                    (_etype136, _size133) = iprot.readListBegin()
+                    for _i137 in range(_size133):
+                        _elem138 = iprot.readBinary()
+                        self.range_begin.append(_elem138)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype135, _size132) = iprot.readListBegin()
-                    for _i136 in range(_size132):
-                        _elem137 = iprot.readBinary()
-                        self.range_end.append(_elem137)
+                    (_etype142, _size139) = iprot.readListBegin()
+                    for _i143 in range(_size139):
+                        _elem144 = iprot.readBinary()
+                        self.range_end.append(_elem144)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype141, _size138) = iprot.readListBegin()
-                    for _i142 in range(_size138):
-                        _elem143 = iprot.readBinary()
-                        self.offset_key.append(_elem143)
+                    (_etype148, _size145) = iprot.readListBegin()
+                    for _i149 in range(_size145):
+                        _elem150 = iprot.readBinary()
+                        self.offset_key.append(_elem150)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype147, _size144) = iprot.readListBegin()
-                    for _i148 in range(_size144):
-                        _elem149 = SpecKeyInterval()
-                        _elem149.read(iprot)
-                        self.key_intervals.append(_elem149)
+                    (_etype154, _size151) = iprot.readListBegin()
+                    for _i155 in range(_size151):
+                        _elem156 = SpecKeyInterval()
+                        _elem156.read(iprot)
+                        self.key_intervals.append(_elem156)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype153, _size150) = iprot.readListBegin()
-                    for _i154 in range(_size150):
-                        _elem155 = SpecValueSerial()
-                        _elem155.read(iprot)
-                        self.values.append(_elem155)
+                    (_etype160, _size157) = iprot.readListBegin()
+                    for _i161 in range(_size157):
+                        _elem162 = SpecValueSerial()
+                        _elem162.read(iprot)
+                        self.values.append(_elem162)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -2954,48 +3173,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecIntervalSerial')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter156 in self.range_begin:
-                oprot.writeBinary(iter156)
+            for iter163 in self.range_begin:
+                oprot.writeBinary(iter163)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter157 in self.range_end:
-                oprot.writeBinary(iter157)
+            for iter164 in self.range_end:
+                oprot.writeBinary(iter164)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter158 in self.offset_key:
-                oprot.writeBinary(iter158)
+            for iter165 in self.offset_key:
+                oprot.writeBinary(iter165)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter159 in self.key_intervals:
-                iter159.write(oprot)
+            for iter166 in self.key_intervals:
+                iter166.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter160 in self.values:
-                iter160.write(oprot)
+            for iter167 in self.values:
+                iter167.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -3072,19 +3291,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype164, _size161) = iprot.readListBegin()
-                    for _i165 in range(_size161):
-                        _elem166 = SpecIntervalSerial()
-                        _elem166.read(iprot)
-                        self.intervals.append(_elem166)
+                    (_etype171, _size168) = iprot.readListBegin()
+                    for _i172 in range(_size168):
+                        _elem173 = SpecIntervalSerial()
+                        _elem173.read(iprot)
+                        self.intervals.append(_elem173)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3097,16 +3316,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter167 in self.intervals:
-                iter167.write(oprot)
+            for iter174 in self.intervals:
+                iter174.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3161,30 +3380,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.columns = []
-                    (_etype171, _size168) = iprot.readListBegin()
-                    for _i172 in range(_size168):
-                        _elem173 = SpecColumn()
-                        _elem173.read(iprot)
-                        self.columns.append(_elem173)
+                    (_etype178, _size175) = iprot.readListBegin()
+                    for _i179 in range(_size175):
+                        _elem180 = SpecColumn()
+                        _elem180.read(iprot)
+                        self.columns.append(_elem180)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.columns_serial = []
-                    (_etype177, _size174) = iprot.readListBegin()
-                    for _i178 in range(_size174):
-                        _elem179 = SpecColumnSerial()
-                        _elem179.read(iprot)
-                        self.columns_serial.append(_elem179)
+                    (_etype184, _size181) = iprot.readListBegin()
+                    for _i185 in range(_size181):
+                        _elem186 = SpecColumnSerial()
+                        _elem186.read(iprot)
+                        self.columns_serial.append(_elem186)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRUCT:
                     self.flags = SpecFlags()
                     self.flags.read(iprot)
@@ -3199,23 +3418,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecScan')
         if self.columns is not None:
             oprot.writeFieldBegin('columns', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.columns))
-            for iter180 in self.columns:
-                iter180.write(oprot)
+            for iter187 in self.columns:
+                iter187.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columns_serial is not None:
             oprot.writeFieldBegin('columns_serial', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.columns_serial))
-            for iter181 in self.columns_serial:
-                iter181.write(oprot)
+            for iter188 in self.columns_serial:
+                iter188.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.flags is not None:
             oprot.writeFieldBegin('flags', TType.STRUCT, 3)
             self.flags.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3288,18 +3507,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype185, _size182) = iprot.readListBegin()
-                    for _i186 in range(_size182):
-                        _elem187 = iprot.readBinary()
-                        self.k.append(_elem187)
+                    (_etype192, _size189) = iprot.readListBegin()
+                    for _i193 in range(_size189):
+                        _elem194 = iprot.readBinary()
+                        self.k.append(_elem194)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3332,16 +3551,16 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter188 in self.k:
-                oprot.writeBinary(iter188)
+            for iter195 in self.k:
+                oprot.writeBinary(iter195)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
@@ -3444,38 +3663,38 @@
                 if ftype == TType.STRING:
                     self.v_bytes = iprot.readBinary()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v_key = []
-                    (_etype192, _size189) = iprot.readListBegin()
-                    for _i193 in range(_size189):
-                        _elem194 = iprot.readBinary()
-                        self.v_key.append(_elem194)
+                    (_etype199, _size196) = iprot.readListBegin()
+                    for _i200 in range(_size196):
+                        _elem201 = iprot.readBinary()
+                        self.v_key.append(_elem201)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.v_li = []
-                    (_etype198, _size195) = iprot.readListBegin()
-                    for _i199 in range(_size195):
-                        _elem200 = iprot.readI64()
-                        self.v_li.append(_elem200)
+                    (_etype205, _size202) = iprot.readListBegin()
+                    for _i206 in range(_size202):
+                        _elem207 = iprot.readI64()
+                        self.v_li.append(_elem207)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.v_lb = []
-                    (_etype204, _size201) = iprot.readListBegin()
-                    for _i205 in range(_size201):
-                        _elem206 = iprot.readBinary()
-                        self.v_lb.append(_elem206)
+                    (_etype211, _size208) = iprot.readListBegin()
+                    for _i212 in range(_size208):
+                        _elem213 = iprot.readBinary()
+                        self.v_lb.append(_elem213)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3500,30 +3719,499 @@
         if self.v_bytes is not None:
             oprot.writeFieldBegin('v_bytes', TType.STRING, 4)
             oprot.writeBinary(self.v_bytes)
             oprot.writeFieldEnd()
         if self.v_key is not None:
             oprot.writeFieldBegin('v_key', TType.LIST, 5)
             oprot.writeListBegin(TType.STRING, len(self.v_key))
-            for iter207 in self.v_key:
-                oprot.writeBinary(iter207)
+            for iter214 in self.v_key:
+                oprot.writeBinary(iter214)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_li is not None:
             oprot.writeFieldBegin('v_li', TType.LIST, 6)
             oprot.writeListBegin(TType.I64, len(self.v_li))
-            for iter208 in self.v_li:
-                oprot.writeI64(iter208)
+            for iter215 in self.v_li:
+                oprot.writeI64(iter215)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_lb is not None:
             oprot.writeFieldBegin('v_lb', TType.LIST, 7)
             oprot.writeListBegin(TType.STRING, len(self.v_lb))
-            for iter209 in self.v_lb:
-                oprot.writeBinary(iter209)
+            for iter216 in self.v_lb:
+                oprot.writeBinary(iter216)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_INT64(object):
+    """
+    Serial INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.I64:
+                    self.v = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_INT64')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.I64, 5)
+            oprot.writeI64(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_DOUBLE(object):
+    """
+    Serial DOUBLE Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.DOUBLE:
+                    self.v = iprot.readDouble()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_DOUBLE')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.DOUBLE, 5)
+            oprot.writeDouble(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_BYTES(object):
+    """
+    Serial BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRING:
+                    self.v = iprot.readBinary()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_BYTES')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.STRING, 5)
+            oprot.writeBinary(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_LI(object):
+    """
+    Serial LIST_INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype220, _size217) = iprot.readListBegin()
+                    for _i221 in range(_size217):
+                        _elem222 = FU_INT64()
+                        _elem222.read(iprot)
+                        self.v.append(_elem222)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LI')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter223 in self.v:
+                iter223.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3543,14 +4231,284 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class FU_LB(object):
+    """
+    Serial LIST_BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype227, _size224) = iprot.readListBegin()
+                    for _i228 in range(_size224):
+                        _elem229 = FU_BYTES()
+                        _elem229.read(iprot)
+                        self.v.append(_elem229)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LB')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter230 in self.v:
+                iter230.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class CellValueSerialOp(object):
+    """
+    The Serial Values Cell field with Update Operation
+
+    Attributes:
+     - field_id: The Field ID, a single ID can have any/all the field types
+     - v_int64: The INT64 type update-field
+     - v_double: The DOUBLE type update-field
+     - v_bytes: The BYTES type update-field
+     - v_key: The Cell KEY type update-field
+     - v_li: The LIST INT64 type update-field
+     - v_lb: The LIST BYTES type update-field
+
+    """
+
+    __slots__ = (
+        'field_id',
+        'v_int64',
+        'v_double',
+        'v_bytes',
+        'v_key',
+        'v_li',
+        'v_lb',
+    )
+
+
+    def __init__(self, field_id=None, v_int64=None, v_double=None, v_bytes=None, v_key=None, v_li=None, v_lb=None,):
+        self.field_id = field_id
+        self.v_int64 = v_int64
+        self.v_double = v_double
+        self.v_bytes = v_bytes
+        self.v_key = v_key
+        self.v_li = v_li
+        self.v_lb = v_lb
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.field_id = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.v_int64 = FU_INT64()
+                    self.v_int64.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRUCT:
+                    self.v_double = FU_DOUBLE()
+                    self.v_double.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.v_bytes = FU_BYTES()
+                    self.v_bytes.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.LIST:
+                    self.v_key = []
+                    (_etype234, _size231) = iprot.readListBegin()
+                    for _i235 in range(_size231):
+                        _elem236 = iprot.readBinary()
+                        self.v_key.append(_elem236)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.STRUCT:
+                    self.v_li = FU_LI()
+                    self.v_li.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 7:
+                if ftype == TType.STRUCT:
+                    self.v_lb = FU_LB()
+                    self.v_lb.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('CellValueSerialOp')
+        if self.field_id is not None:
+            oprot.writeFieldBegin('field_id', TType.I32, 1)
+            oprot.writeI32(self.field_id)
+            oprot.writeFieldEnd()
+        if self.v_int64 is not None:
+            oprot.writeFieldBegin('v_int64', TType.STRUCT, 2)
+            self.v_int64.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_double is not None:
+            oprot.writeFieldBegin('v_double', TType.STRUCT, 3)
+            self.v_double.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_bytes is not None:
+            oprot.writeFieldBegin('v_bytes', TType.STRUCT, 4)
+            self.v_bytes.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_key is not None:
+            oprot.writeFieldBegin('v_key', TType.LIST, 5)
+            oprot.writeListBegin(TType.STRING, len(self.v_key))
+            for iter237 in self.v_key:
+                oprot.writeBinary(iter237)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_li is not None:
+            oprot.writeFieldBegin('v_li', TType.STRUCT, 6)
+            self.v_li.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_lb is not None:
+            oprot.writeFieldBegin('v_lb', TType.STRUCT, 7)
+            self.v_lb.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class UCellSerial(object):
     """
     The Cell data for using with Update of SERIAL Column Type
 
     Attributes:
      - f: The Cell Flag
      - k: The Cell Key
@@ -3592,18 +4550,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype213, _size210) = iprot.readListBegin()
-                    for _i214 in range(_size210):
-                        _elem215 = iprot.readBinary()
-                        self.k.append(_elem215)
+                    (_etype241, _size238) = iprot.readListBegin()
+                    for _i242 in range(_size238):
+                        _elem243 = iprot.readBinary()
+                        self.k.append(_elem243)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3612,19 +4570,19 @@
                 if ftype == TType.BOOL:
                     self.ts_desc = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype219, _size216) = iprot.readListBegin()
-                    for _i220 in range(_size216):
-                        _elem221 = CellValueSerial()
-                        _elem221.read(iprot)
-                        self.v.append(_elem221)
+                    (_etype247, _size244) = iprot.readListBegin()
+                    for _i248 in range(_size244):
+                        _elem249 = CellValueSerial()
+                        _elem249.read(iprot)
+                        self.v.append(_elem249)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
@@ -3642,31 +4600,31 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter222 in self.k:
-                oprot.writeBinary(iter222)
+            for iter250 in self.k:
+                oprot.writeBinary(iter250)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
             oprot.writeFieldBegin('ts_desc', TType.BOOL, 4)
             oprot.writeBool(self.ts_desc)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter223 in self.v:
-                iter223.write(oprot)
+            for iter251 in self.v:
+                iter251.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 6)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3733,18 +4691,18 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype227, _size224) = iprot.readListBegin()
-                    for _i228 in range(_size224):
-                        _elem229 = iprot.readBinary()
-                        self.k.append(_elem229)
+                    (_etype255, _size252) = iprot.readListBegin()
+                    for _i256 in range(_size252):
+                        _elem257 = iprot.readBinary()
+                        self.k.append(_elem257)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3767,16 +4725,16 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter230 in self.k:
-                oprot.writeBinary(iter230)
+            for iter258 in self.k:
+                oprot.writeBinary(iter258)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -3847,34 +4805,34 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype234, _size231) = iprot.readListBegin()
-                    for _i235 in range(_size231):
-                        _elem236 = iprot.readBinary()
-                        self.k.append(_elem236)
+                    (_etype262, _size259) = iprot.readListBegin()
+                    for _i263 in range(_size259):
+                        _elem264 = iprot.readBinary()
+                        self.k.append(_elem264)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype240, _size237) = iprot.readListBegin()
-                    for _i241 in range(_size237):
-                        _elem242 = CellValueSerial()
-                        _elem242.read(iprot)
-                        self.v.append(_elem242)
+                    (_etype268, _size265) = iprot.readListBegin()
+                    for _i269 in range(_size265):
+                        _elem270 = CellValueSerial()
+                        _elem270.read(iprot)
+                        self.v.append(_elem270)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3887,27 +4845,27 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter243 in self.k:
-                oprot.writeBinary(iter243)
+            for iter271 in self.k:
+                oprot.writeBinary(iter271)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter244 in self.v:
-                iter244.write(oprot)
+            for iter272 in self.v:
+                iter272.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3959,30 +4917,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype248, _size245) = iprot.readListBegin()
-                    for _i249 in range(_size245):
-                        _elem250 = Cell()
-                        _elem250.read(iprot)
-                        self.cells.append(_elem250)
+                    (_etype276, _size273) = iprot.readListBegin()
+                    for _i277 in range(_size273):
+                        _elem278 = Cell()
+                        _elem278.read(iprot)
+                        self.cells.append(_elem278)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype254, _size251) = iprot.readListBegin()
-                    for _i255 in range(_size251):
-                        _elem256 = CellSerial()
-                        _elem256.read(iprot)
-                        self.serial_cells.append(_elem256)
+                    (_etype282, _size279) = iprot.readListBegin()
+                    for _i283 in range(_size279):
+                        _elem284 = CellSerial()
+                        _elem284.read(iprot)
+                        self.serial_cells.append(_elem284)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3991,23 +4949,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Cells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter257 in self.cells:
-                iter257.write(oprot)
+            for iter285 in self.cells:
+                iter285.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter258 in self.serial_cells:
-                iter258.write(oprot)
+            for iter286 in self.serial_cells:
+                iter286.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4062,18 +5020,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype262, _size259) = iprot.readListBegin()
-                    for _i263 in range(_size259):
-                        _elem264 = iprot.readBinary()
-                        self.k.append(_elem264)
+                    (_etype290, _size287) = iprot.readListBegin()
+                    for _i291 in range(_size287):
+                        _elem292 = iprot.readBinary()
+                        self.k.append(_elem292)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -4092,16 +5050,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCell')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter265 in self.k:
-                oprot.writeBinary(iter265)
+            for iter293 in self.k:
+                oprot.writeBinary(iter293)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -4164,34 +5122,34 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype269, _size266) = iprot.readListBegin()
-                    for _i270 in range(_size266):
-                        _elem271 = iprot.readBinary()
-                        self.k.append(_elem271)
+                    (_etype297, _size294) = iprot.readListBegin()
+                    for _i298 in range(_size294):
+                        _elem299 = iprot.readBinary()
+                        self.k.append(_elem299)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype275, _size272) = iprot.readListBegin()
-                    for _i276 in range(_size272):
-                        _elem277 = CellValueSerial()
-                        _elem277.read(iprot)
-                        self.v.append(_elem277)
+                    (_etype303, _size300) = iprot.readListBegin()
+                    for _i304 in range(_size300):
+                        _elem305 = CellValueSerial()
+                        _elem305.read(iprot)
+                        self.v.append(_elem305)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4200,27 +5158,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCellSerial')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter278 in self.k:
-                oprot.writeBinary(iter278)
+            for iter306 in self.k:
+                oprot.writeBinary(iter306)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter279 in self.v:
-                iter279.write(oprot)
+            for iter307 in self.v:
+                iter307.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4272,30 +5230,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype283, _size280) = iprot.readListBegin()
-                    for _i284 in range(_size280):
-                        _elem285 = CCell()
-                        _elem285.read(iprot)
-                        self.cells.append(_elem285)
+                    (_etype311, _size308) = iprot.readListBegin()
+                    for _i312 in range(_size308):
+                        _elem313 = CCell()
+                        _elem313.read(iprot)
+                        self.cells.append(_elem313)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype289, _size286) = iprot.readListBegin()
-                    for _i290 in range(_size286):
-                        _elem291 = CCellSerial()
-                        _elem291.read(iprot)
-                        self.serial_cells.append(_elem291)
+                    (_etype317, _size314) = iprot.readListBegin()
+                    for _i318 in range(_size314):
+                        _elem319 = CCellSerial()
+                        _elem319.read(iprot)
+                        self.serial_cells.append(_elem319)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4304,23 +5262,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ColCells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter292 in self.cells:
-                iter292.write(oprot)
+            for iter320 in self.cells:
+                iter320.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter293 in self.serial_cells:
-                iter293.write(oprot)
+            for iter321 in self.serial_cells:
+                iter321.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4479,19 +5437,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype297, _size294) = iprot.readListBegin()
-                    for _i298 in range(_size294):
-                        _elem299 = CellValueSerial()
-                        _elem299.read(iprot)
-                        self.v.append(_elem299)
+                    (_etype325, _size322) = iprot.readListBegin()
+                    for _i326 in range(_size322):
+                        _elem327 = CellValueSerial()
+                        _elem327.read(iprot)
+                        self.v.append(_elem327)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4508,16 +5466,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter300 in self.v:
-                iter300.write(oprot)
+            for iter328 in self.v:
+                iter328.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4572,40 +5530,40 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype304, _size301) = iprot.readListBegin()
-                    for _i305 in range(_size301):
-                        _elem306 = iprot.readBinary()
-                        self.k.append(_elem306)
+                    (_etype332, _size329) = iprot.readListBegin()
+                    for _i333 in range(_size329):
+                        _elem334 = iprot.readBinary()
+                        self.k.append(_elem334)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype310, _size307) = iprot.readListBegin()
-                    for _i311 in range(_size307):
-                        _elem312 = KCell()
-                        _elem312.read(iprot)
-                        self.cells.append(_elem312)
+                    (_etype338, _size335) = iprot.readListBegin()
+                    for _i339 in range(_size335):
+                        _elem340 = KCell()
+                        _elem340.read(iprot)
+                        self.cells.append(_elem340)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype316, _size313) = iprot.readListBegin()
-                    for _i317 in range(_size313):
-                        _elem318 = KCellSerial()
-                        _elem318.read(iprot)
-                        self.serial_cells.append(_elem318)
+                    (_etype344, _size341) = iprot.readListBegin()
+                    for _i345 in range(_size341):
+                        _elem346 = KCellSerial()
+                        _elem346.read(iprot)
+                        self.serial_cells.append(_elem346)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4614,30 +5572,30 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('kCells')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter319 in self.k:
-                oprot.writeBinary(iter319)
+            for iter347 in self.k:
+                oprot.writeBinary(iter347)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter320 in self.cells:
-                iter320.write(oprot)
+            for iter348 in self.cells:
+                iter348.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter321 in self.serial_cells:
-                iter321.write(oprot)
+            for iter349 in self.serial_cells:
+                iter349.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4796,19 +5754,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype325, _size322) = iprot.readListBegin()
-                    for _i326 in range(_size322):
-                        _elem327 = CellValueSerial()
-                        _elem327.read(iprot)
-                        self.v.append(_elem327)
+                    (_etype353, _size350) = iprot.readListBegin()
+                    for _i354 in range(_size350):
+                        _elem355 = CellValueSerial()
+                        _elem355.read(iprot)
+                        self.v.append(_elem355)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4825,16 +5783,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter328 in self.v:
-                iter328.write(oprot)
+            for iter356 in self.v:
+                iter356.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4889,42 +5847,42 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.f = {}
-                    (_ktype330, _vtype331, _size329) = iprot.readMapBegin()
-                    for _i333 in range(_size329):
-                        _key334 = iprot.readBinary()
-                        _val335 = FCells()
-                        _val335.read(iprot)
-                        self.f[_key334] = _val335
+                    (_ktype358, _vtype359, _size357) = iprot.readMapBegin()
+                    for _i361 in range(_size357):
+                        _key362 = iprot.readBinary()
+                        _val363 = FCells()
+                        _val363.read(iprot)
+                        self.f[_key362] = _val363
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype339, _size336) = iprot.readListBegin()
-                    for _i340 in range(_size336):
-                        _elem341 = FCell()
-                        _elem341.read(iprot)
-                        self.cells.append(_elem341)
+                    (_etype367, _size364) = iprot.readListBegin()
+                    for _i368 in range(_size364):
+                        _elem369 = FCell()
+                        _elem369.read(iprot)
+                        self.cells.append(_elem369)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype345, _size342) = iprot.readListBegin()
-                    for _i346 in range(_size342):
-                        _elem347 = FCellSerial()
-                        _elem347.read(iprot)
-                        self.serial_cells.append(_elem347)
+                    (_etype373, _size370) = iprot.readListBegin()
+                    for _i374 in range(_size370):
+                        _elem375 = FCellSerial()
+                        _elem375.read(iprot)
+                        self.serial_cells.append(_elem375)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4933,31 +5891,31 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('FCells')
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.MAP, 1)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.f))
-            for kiter348, viter349 in self.f.items():
-                oprot.writeBinary(kiter348)
-                viter349.write(oprot)
+            for kiter376, viter377 in self.f.items():
+                oprot.writeBinary(kiter376)
+                viter377.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter350 in self.cells:
-                iter350.write(oprot)
+            for iter378 in self.cells:
+                iter378.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter351 in self.serial_cells:
-                iter351.write(oprot)
+            for iter379 in self.serial_cells:
+                iter379.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5021,31 +5979,31 @@
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.ccells = {}
-                    (_ktype353, _vtype354, _size352) = iprot.readMapBegin()
-                    for _i356 in range(_size352):
-                        _key357 = iprot.readString()
-                        _val358 = ColCells()
-                        _val358.read(iprot)
-                        self.ccells[_key357] = _val358
+                    (_ktype381, _vtype382, _size380) = iprot.readMapBegin()
+                    for _i384 in range(_size380):
+                        _key385 = iprot.readString()
+                        _val386 = ColCells()
+                        _val386.read(iprot)
+                        self.ccells[_key385] = _val386
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.kcells = []
-                    (_etype362, _size359) = iprot.readListBegin()
-                    for _i363 in range(_size359):
-                        _elem364 = kCells()
-                        _elem364.read(iprot)
-                        self.kcells.append(_elem364)
+                    (_etype390, _size387) = iprot.readListBegin()
+                    for _i391 in range(_size387):
+                        _elem392 = kCells()
+                        _elem392.read(iprot)
+                        self.kcells.append(_elem392)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.fcells = FCells()
                     self.fcells.read(iprot)
@@ -5064,24 +6022,24 @@
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 1)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.ccells is not None:
             oprot.writeFieldBegin('ccells', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.ccells))
-            for kiter365, viter366 in self.ccells.items():
-                oprot.writeString(kiter365)
-                viter366.write(oprot)
+            for kiter393, viter394 in self.ccells.items():
+                oprot.writeString(kiter393)
+                viter394.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.kcells is not None:
             oprot.writeFieldBegin('kcells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.kcells))
-            for iter367 in self.kcells:
-                iter367.write(oprot)
+            for iter395 in self.kcells:
+                iter395.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.fcells is not None:
             oprot.writeFieldBegin('fcells', TType.STRUCT, 4)
             self.fcells.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5222,36 +6180,36 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemas = []
-                    (_etype371, _size368) = iprot.readListBegin()
-                    for _i372 in range(_size368):
-                        _elem373 = Schema()
-                        _elem373.read(iprot)
-                        self.schemas.append(_elem373)
+                    (_etype399, _size396) = iprot.readListBegin()
+                    for _i400 in range(_size396):
+                        _elem401 = Schema()
+                        _elem401.read(iprot)
+                        self.schemas.append(_elem401)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRUCT:
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.compact = []
-                    (_etype377, _size374) = iprot.readListBegin()
-                    for _i378 in range(_size374):
-                        _elem379 = CompactResult()
-                        _elem379.read(iprot)
-                        self.compact.append(_elem379)
+                    (_etype405, _size402) = iprot.readListBegin()
+                    for _i406 in range(_size402):
+                        _elem407 = CompactResult()
+                        _elem407.read(iprot)
+                        self.compact.append(_elem407)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5260,27 +6218,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Result')
         if self.schemas is not None:
             oprot.writeFieldBegin('schemas', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemas))
-            for iter380 in self.schemas:
-                iter380.write(oprot)
+            for iter408 in self.schemas:
+                iter408.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 2)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.compact is not None:
             oprot.writeFieldBegin('compact', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.compact))
-            for iter381 in self.compact:
-                iter381.write(oprot)
+            for iter409 in self.compact:
+                iter409.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5384,27 +6342,36 @@
 )
 all_structs.append(SpecValue)
 SpecValue.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'comp', None, None, ),  # 1
     (2, TType.STRING, 'v', 'BINARY', None, ),  # 2
 )
+all_structs.append(SpecUpdateOP)
+SpecUpdateOP.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'op', None, None, ),  # 1
+    (2, TType.I32, 'pos', None, None, ),  # 2
+)
 all_structs.append(SpecIntervalUpdate)
 SpecIntervalUpdate.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'v', 'BINARY', None, ),  # 1
     (2, TType.I64, 'ts', None, None, ),  # 2
     (3, TType.I32, 'encoder', None, None, ),  # 3
+    (4, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 4
 )
 all_structs.append(SpecIntervalUpdateSerial)
 SpecIntervalUpdateSerial.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'ts', None, None, ),  # 1
     (2, TType.LIST, 'v', (TType.STRUCT, [CellValueSerial, None], False), None, ),  # 2
-    (3, TType.I32, 'encoder', None, None, ),  # 3
+    (3, TType.LIST, 'v_op', (TType.STRUCT, [CellValueSerialOp, None], False), None, ),  # 3
+    (4, TType.I32, 'encoder', None, None, ),  # 4
+    (5, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 5
 )
 all_structs.append(SpecInterval)
 SpecInterval.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'range_begin', (TType.STRING, 'BINARY', False), None, ),  # 1
     (2, TType.LIST, 'range_end', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.LIST, 'offset_key', (TType.STRING, 'BINARY', False), None, ),  # 3
@@ -5521,14 +6488,68 @@
     (2, TType.I64, 'v_int64', None, None, ),  # 2
     (3, TType.DOUBLE, 'v_double', None, None, ),  # 3
     (4, TType.STRING, 'v_bytes', 'BINARY', None, ),  # 4
     (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
     (6, TType.LIST, 'v_li', (TType.I64, None, False), None, ),  # 6
     (7, TType.LIST, 'v_lb', (TType.STRING, 'BINARY', False), None, ),  # 7
 )
+all_structs.append(FU_INT64)
+FU_INT64.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.I64, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_DOUBLE)
+FU_DOUBLE.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.DOUBLE, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_BYTES)
+FU_BYTES.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.STRING, 'v', 'BINARY', None, ),  # 5
+)
+all_structs.append(FU_LI)
+FU_LI.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_INT64, None], False), None, ),  # 4
+)
+all_structs.append(FU_LB)
+FU_LB.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_BYTES, None], False), None, ),  # 4
+)
+all_structs.append(CellValueSerialOp)
+CellValueSerialOp.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'field_id', None, None, ),  # 1
+    (2, TType.STRUCT, 'v_int64', [FU_INT64, None], None, ),  # 2
+    (3, TType.STRUCT, 'v_double', [FU_DOUBLE, None], None, ),  # 3
+    (4, TType.STRUCT, 'v_bytes', [FU_BYTES, None], None, ),  # 4
+    (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
+    (6, TType.STRUCT, 'v_li', [FU_LI, None], None, ),  # 6
+    (7, TType.STRUCT, 'v_lb', [FU_LB, None], None, ),  # 7
+)
 all_structs.append(UCellSerial)
 UCellSerial.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'f', None, None, ),  # 1
     (2, TType.LIST, 'k', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.I64, 'ts', None, None, ),  # 3
     (4, TType.BOOL, 'ts_desc', None, None, ),  # 4
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/twisted/Service.py` & `swcdb-0.5.9.0/swcdb/thrift/twisted/Service.py`

 * *Files 0% similar despite different names*

```diff
@@ -2540,19 +2540,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype385, _size382) = iprot.readListBegin()
-                    for _i386 in range(_size382):
-                        _elem387 = Schema()
-                        _elem387.read(iprot)
-                        self.success.append(_elem387)
+                    (_etype413, _size410) = iprot.readListBegin()
+                    for _i414 in range(_size410):
+                        _elem415 = Schema()
+                        _elem415.read(iprot)
+                        self.success.append(_elem415)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2566,16 +2566,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter388 in self.success:
-                iter388.write(oprot)
+            for iter416 in self.success:
+                iter416.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2707,19 +2707,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype392, _size389) = iprot.readListBegin()
-                    for _i393 in range(_size389):
-                        _elem394 = CompactResult()
-                        _elem394.read(iprot)
-                        self.success.append(_elem394)
+                    (_etype420, _size417) = iprot.readListBegin()
+                    for _i421 in range(_size417):
+                        _elem422 = CompactResult()
+                        _elem422.read(iprot)
+                        self.success.append(_elem422)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2733,16 +2733,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter395 in self.success:
-                iter395.write(oprot)
+            for iter423 in self.success:
+                iter423.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3033,20 +3033,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype397, _vtype398, _size396) = iprot.readMapBegin()
-                    for _i400 in range(_size396):
-                        _key401 = iprot.readString()
-                        _val402 = ColCells()
-                        _val402.read(iprot)
-                        self.success[_key401] = _val402
+                    (_ktype425, _vtype426, _size424) = iprot.readMapBegin()
+                    for _i428 in range(_size424):
+                        _key429 = iprot.readString()
+                        _val430 = ColCells()
+                        _val430.read(iprot)
+                        self.success[_key429] = _val430
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -3060,17 +3060,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter403, viter404 in self.success.items():
-                oprot.writeString(kiter403)
-                viter404.write(oprot)
+            for kiter431, viter432 in self.success.items():
+                oprot.writeString(kiter431)
+                viter432.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3202,19 +3202,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype408, _size405) = iprot.readListBegin()
-                    for _i409 in range(_size405):
-                        _elem410 = kCells()
-                        _elem410.read(iprot)
-                        self.success.append(_elem410)
+                    (_etype436, _size433) = iprot.readListBegin()
+                    for _i437 in range(_size433):
+                        _elem438 = kCells()
+                        _elem438.read(iprot)
+                        self.success.append(_elem438)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -3228,16 +3228,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter411 in self.success:
-                iter411.write(oprot)
+            for iter439 in self.success:
+                iter439.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4249,25 +4249,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype413, _vtype414, _size412) = iprot.readMapBegin()
-                    for _i416 in range(_size412):
-                        _key417 = iprot.readI64()
-                        _val418 = []
-                        (_etype422, _size419) = iprot.readListBegin()
-                        for _i423 in range(_size419):
-                            _elem424 = UCell()
-                            _elem424.read(iprot)
-                            _val418.append(_elem424)
+                    (_ktype441, _vtype442, _size440) = iprot.readMapBegin()
+                    for _i444 in range(_size440):
+                        _key445 = iprot.readI64()
+                        _val446 = []
+                        (_etype450, _size447) = iprot.readListBegin()
+                        for _i451 in range(_size447):
+                            _elem452 = UCell()
+                            _elem452.read(iprot)
+                            _val446.append(_elem452)
                         iprot.readListEnd()
-                        self.cells[_key417] = _val418
+                        self.cells[_key445] = _val446
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -4281,19 +4281,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter425, viter426 in self.cells.items():
-                oprot.writeI64(kiter425)
-                oprot.writeListBegin(TType.STRUCT, len(viter426))
-                for iter427 in viter426:
-                    iter427.write(oprot)
+            for kiter453, viter454 in self.cells.items():
+                oprot.writeI64(kiter453)
+                oprot.writeListBegin(TType.STRUCT, len(viter454))
+                for iter455 in viter454:
+                    iter455.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -4427,25 +4427,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype429, _vtype430, _size428) = iprot.readMapBegin()
-                    for _i432 in range(_size428):
-                        _key433 = iprot.readI64()
-                        _val434 = []
-                        (_etype438, _size435) = iprot.readListBegin()
-                        for _i439 in range(_size435):
-                            _elem440 = UCellSerial()
-                            _elem440.read(iprot)
-                            _val434.append(_elem440)
+                    (_ktype457, _vtype458, _size456) = iprot.readMapBegin()
+                    for _i460 in range(_size456):
+                        _key461 = iprot.readI64()
+                        _val462 = []
+                        (_etype466, _size463) = iprot.readListBegin()
+                        for _i467 in range(_size463):
+                            _elem468 = UCellSerial()
+                            _elem468.read(iprot)
+                            _val462.append(_elem468)
                         iprot.readListEnd()
-                        self.cells[_key433] = _val434
+                        self.cells[_key461] = _val462
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -4459,19 +4459,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_serial_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter441, viter442 in self.cells.items():
-                oprot.writeI64(kiter441)
-                oprot.writeListBegin(TType.STRUCT, len(viter442))
-                for iter443 in viter442:
-                    iter443.write(oprot)
+            for kiter469, viter470 in self.cells.items():
+                oprot.writeI64(kiter469)
+                oprot.writeListBegin(TType.STRUCT, len(viter470))
+                for iter471 in viter470:
+                    iter471.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -4839,19 +4839,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype447, _size444) = iprot.readListBegin()
-                    for _i448 in range(_size444):
-                        _elem449 = Schema()
-                        _elem449.read(iprot)
-                        self.success.append(_elem449)
+                    (_etype475, _size472) = iprot.readListBegin()
+                    for _i476 in range(_size472):
+                        _elem477 = Schema()
+                        _elem477.read(iprot)
+                        self.success.append(_elem477)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4865,16 +4865,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter450 in self.success:
-                iter450.write(oprot)
+            for iter478 in self.success:
+                iter478.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5007,19 +5007,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype454, _size451) = iprot.readListBegin()
-                    for _i455 in range(_size451):
-                        _elem456 = CompactResult()
-                        _elem456.read(iprot)
-                        self.success.append(_elem456)
+                    (_etype482, _size479) = iprot.readListBegin()
+                    for _i483 in range(_size479):
+                        _elem484 = CompactResult()
+                        _elem484.read(iprot)
+                        self.success.append(_elem484)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -5033,16 +5033,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter457 in self.success:
-                iter457.write(oprot)
+            for iter485 in self.success:
+                iter485.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5335,20 +5335,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype459, _vtype460, _size458) = iprot.readMapBegin()
-                    for _i462 in range(_size458):
-                        _key463 = iprot.readString()
-                        _val464 = ColCells()
-                        _val464.read(iprot)
-                        self.success[_key463] = _val464
+                    (_ktype487, _vtype488, _size486) = iprot.readMapBegin()
+                    for _i490 in range(_size486):
+                        _key491 = iprot.readString()
+                        _val492 = ColCells()
+                        _val492.read(iprot)
+                        self.success[_key491] = _val492
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -5362,17 +5362,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter465, viter466 in self.success.items():
-                oprot.writeString(kiter465)
-                viter466.write(oprot)
+            for kiter493, viter494 in self.success.items():
+                oprot.writeString(kiter493)
+                viter494.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5505,19 +5505,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype470, _size467) = iprot.readListBegin()
-                    for _i471 in range(_size467):
-                        _elem472 = kCells()
-                        _elem472.read(iprot)
-                        self.success.append(_elem472)
+                    (_etype498, _size495) = iprot.readListBegin()
+                    for _i499 in range(_size495):
+                        _elem500 = kCells()
+                        _elem500.read(iprot)
+                        self.success.append(_elem500)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -5531,16 +5531,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter473 in self.success:
-                iter473.write(oprot)
+            for iter501 in self.success:
+                iter501.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/twisted/ttypes.py` & `swcdb-0.5.9.0/swcdb/thrift/twisted/ttypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,14 +246,41 @@
 
     _NAMES_TO_VALUES = {
         "UPDATING": 4,
         "DELETING": 8,
     }
 
 
+class UpdateOP(object):
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    SERIAL = 5
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "SERIAL",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "SERIAL": 5,
+    }
+
+
 class Flag(object):
     """
     The Cell Flag
 
     """
     NONE = 0
     INSERT = 1
@@ -271,14 +298,79 @@
         "NONE": 0,
         "INSERT": 1,
         "DELETE_LE": 2,
         "DELETE_EQ": 3,
     }
 
 
+class FU_MATH_OP(object):
+    """
+    MATH Operations for Serial Field Update of types INT64 and DOUBLE
+
+    """
+    EQUAL = 0
+    PLUS = 1
+    MULTIPLY = 2
+    DIVIDE = 3
+
+    _VALUES_TO_NAMES = {
+        0: "EQUAL",
+        1: "PLUS",
+        2: "MULTIPLY",
+        3: "DIVIDE",
+    }
+
+    _NAMES_TO_VALUES = {
+        "EQUAL": 0,
+        "PLUS": 1,
+        "MULTIPLY": 2,
+        "DIVIDE": 3,
+    }
+
+
+class FU_LIST_OP(object):
+    """
+    LIST Operations for Serial Field Update of array/list/bytes with LIST-op in the inner SERIAL fields
+
+    """
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    ERASE = 5
+    BY_UNIQUE = 6
+    BY_COND = 7
+    BY_INDEX = 8
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "ERASE",
+        6: "BY_UNIQUE",
+        7: "BY_COND",
+        8: "BY_INDEX",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "ERASE": 5,
+        "BY_UNIQUE": 6,
+        "BY_COND": 7,
+        "BY_INDEX": 8,
+    }
+
+
 class CellsResult(object):
     """
     The Cells Results types for using with CellsGroup requests
 
     """
     IN_LIST = 0
     ON_COLUMN = 1
@@ -1519,36 +1611,119 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class SpecUpdateOP(object):
+    """
+    Attributes:
+     - op: The Operation of update
+     - pos: The position/index of INSERT and OVERWRITE update operations
+
+    """
+
+    __slots__ = (
+        'op',
+        'pos',
+    )
+
+
+    def __init__(self, op=None, pos=None,):
+        self.op = op
+        self.pos = pos
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('SpecUpdateOP')
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 1)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 2)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class SpecIntervalUpdate(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecInterval
 
     Attributes:
      - v: The value for the updated cell
      - ts: The timestamp for the updated cell NULL: MIN_INT64+1, AUTO:MIN_INT64+2 (or not-set)
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'v',
         'ts',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, v=None, ts=None, encoder=None,):
+    def __init__(self, v=None, ts=None, encoder=None, update_op=None,):
         self.v = v
         self.ts = ts
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1566,14 +1741,20 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1588,14 +1769,18 @@
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 3)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 4)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1619,30 +1804,36 @@
 
 class SpecIntervalUpdateSerial(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecIntervalSerial
 
     Attributes:
      - ts: The timestamp for the updated cell NULL: MIN_INT64-1, AUTO:MIN_INT64-1
-     - v: The value for the updated cell
+     - v: The values of serial-fields for the updated cell
+     - v_op: The values of serial-fields for the the SERIAL operation update
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'ts',
         'v',
+        'v_op',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, ts=None, v=None, encoder=None,):
+    def __init__(self, ts=None, v=None, v_op=None, encoder=None, update_op=None,):
         self.ts = ts
         self.v = v
+        self.v_op = v_op
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1662,18 +1853,35 @@
                         _elem54 = CellValueSerial()
                         _elem54.read(iprot)
                         self.v.append(_elem54)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
+                if ftype == TType.LIST:
+                    self.v_op = []
+                    (_etype58, _size55) = iprot.readListBegin()
+                    for _i59 in range(_size55):
+                        _elem60 = CellValueSerialOp()
+                        _elem60.read(iprot)
+                        self.v_op.append(_elem60)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1683,22 +1891,33 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 1)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter55 in self.v:
-                iter55.write(oprot)
+            for iter61 in self.v:
+                iter61.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_op is not None:
+            oprot.writeFieldBegin('v_op', TType.LIST, 3)
+            oprot.writeListBegin(TType.STRUCT, len(self.v_op))
+            for iter62 in self.v_op:
+                iter62.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
-            oprot.writeFieldBegin('encoder', TType.I32, 3)
+            oprot.writeFieldBegin('encoder', TType.I32, 4)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 5)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1775,65 +1994,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype59, _size56) = iprot.readListBegin()
-                    for _i60 in range(_size56):
-                        _elem61 = iprot.readBinary()
-                        self.range_begin.append(_elem61)
+                    (_etype66, _size63) = iprot.readListBegin()
+                    for _i67 in range(_size63):
+                        _elem68 = iprot.readBinary()
+                        self.range_begin.append(_elem68)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype65, _size62) = iprot.readListBegin()
-                    for _i66 in range(_size62):
-                        _elem67 = iprot.readBinary()
-                        self.range_end.append(_elem67)
+                    (_etype72, _size69) = iprot.readListBegin()
+                    for _i73 in range(_size69):
+                        _elem74 = iprot.readBinary()
+                        self.range_end.append(_elem74)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype71, _size68) = iprot.readListBegin()
-                    for _i72 in range(_size68):
-                        _elem73 = iprot.readBinary()
-                        self.offset_key.append(_elem73)
+                    (_etype78, _size75) = iprot.readListBegin()
+                    for _i79 in range(_size75):
+                        _elem80 = iprot.readBinary()
+                        self.offset_key.append(_elem80)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype77, _size74) = iprot.readListBegin()
-                    for _i78 in range(_size74):
-                        _elem79 = SpecKeyInterval()
-                        _elem79.read(iprot)
-                        self.key_intervals.append(_elem79)
+                    (_etype84, _size81) = iprot.readListBegin()
+                    for _i85 in range(_size81):
+                        _elem86 = SpecKeyInterval()
+                        _elem86.read(iprot)
+                        self.key_intervals.append(_elem86)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype83, _size80) = iprot.readListBegin()
-                    for _i84 in range(_size80):
-                        _elem85 = SpecValue()
-                        _elem85.read(iprot)
-                        self.values.append(_elem85)
+                    (_etype90, _size87) = iprot.readListBegin()
+                    for _i91 in range(_size87):
+                        _elem92 = SpecValue()
+                        _elem92.read(iprot)
+                        self.values.append(_elem92)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -1871,48 +2090,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecInterval')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter86 in self.range_begin:
-                oprot.writeBinary(iter86)
+            for iter93 in self.range_begin:
+                oprot.writeBinary(iter93)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter87 in self.range_end:
-                oprot.writeBinary(iter87)
+            for iter94 in self.range_end:
+                oprot.writeBinary(iter94)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter88 in self.offset_key:
-                oprot.writeBinary(iter88)
+            for iter95 in self.offset_key:
+                oprot.writeBinary(iter95)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter89 in self.key_intervals:
-                iter89.write(oprot)
+            for iter96 in self.key_intervals:
+                iter96.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter90 in self.values:
-                iter90.write(oprot)
+            for iter97 in self.values:
+                iter97.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -1989,19 +2208,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype94, _size91) = iprot.readListBegin()
-                    for _i95 in range(_size91):
-                        _elem96 = SpecInterval()
-                        _elem96.read(iprot)
-                        self.intervals.append(_elem96)
+                    (_etype101, _size98) = iprot.readListBegin()
+                    for _i102 in range(_size98):
+                        _elem103 = SpecInterval()
+                        _elem103.read(iprot)
+                        self.intervals.append(_elem103)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2014,16 +2233,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter97 in self.intervals:
-                iter97.write(oprot)
+            for iter104 in self.intervals:
+                iter104.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2326,19 +2545,19 @@
                 if ftype == TType.I32:
                     self.seq = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype101, _size98) = iprot.readListBegin()
-                    for _i102 in range(_size98):
-                        _elem103 = SpecFraction()
-                        _elem103.read(iprot)
-                        self.v.append(_elem103)
+                    (_etype108, _size105) = iprot.readListBegin()
+                    for _i109 in range(_size105):
+                        _elem110 = SpecFraction()
+                        _elem110.read(iprot)
+                        self.v.append(_elem110)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2351,16 +2570,16 @@
         if self.seq is not None:
             oprot.writeFieldBegin('seq', TType.I32, 1)
             oprot.writeI32(self.seq)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter104 in self.v:
-                iter104.write(oprot)
+            for iter111 in self.v:
+                iter111.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2417,19 +2636,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype108, _size105) = iprot.readListBegin()
-                    for _i109 in range(_size105):
-                        _elem110 = SpecValueSerial_INT64()
-                        _elem110.read(iprot)
-                        self.v.append(_elem110)
+                    (_etype115, _size112) = iprot.readListBegin()
+                    for _i116 in range(_size112):
+                        _elem117 = SpecValueSerial_INT64()
+                        _elem117.read(iprot)
+                        self.v.append(_elem117)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2442,16 +2661,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter111 in self.v:
-                iter111.write(oprot)
+            for iter118 in self.v:
+                iter118.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2508,19 +2727,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype115, _size112) = iprot.readListBegin()
-                    for _i116 in range(_size112):
-                        _elem117 = SpecValueSerial_BYTES()
-                        _elem117.read(iprot)
-                        self.v.append(_elem117)
+                    (_etype122, _size119) = iprot.readListBegin()
+                    for _i123 in range(_size119):
+                        _elem124 = SpecValueSerial_BYTES()
+                        _elem124.read(iprot)
+                        self.v.append(_elem124)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2533,16 +2752,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter118 in self.v:
-                iter118.write(oprot)
+            for iter125 in self.v:
+                iter125.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2745,19 +2964,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.fields = []
-                    (_etype122, _size119) = iprot.readListBegin()
-                    for _i123 in range(_size119):
-                        _elem124 = SpecValueSerialField()
-                        _elem124.read(iprot)
-                        self.fields.append(_elem124)
+                    (_etype129, _size126) = iprot.readListBegin()
+                    for _i130 in range(_size126):
+                        _elem131 = SpecValueSerialField()
+                        _elem131.read(iprot)
+                        self.fields.append(_elem131)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2770,16 +2989,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.fields is not None:
             oprot.writeFieldBegin('fields', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.fields))
-            for iter125 in self.fields:
-                iter125.write(oprot)
+            for iter132 in self.fields:
+                iter132.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2858,65 +3077,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype129, _size126) = iprot.readListBegin()
-                    for _i130 in range(_size126):
-                        _elem131 = iprot.readBinary()
-                        self.range_begin.append(_elem131)
+                    (_etype136, _size133) = iprot.readListBegin()
+                    for _i137 in range(_size133):
+                        _elem138 = iprot.readBinary()
+                        self.range_begin.append(_elem138)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype135, _size132) = iprot.readListBegin()
-                    for _i136 in range(_size132):
-                        _elem137 = iprot.readBinary()
-                        self.range_end.append(_elem137)
+                    (_etype142, _size139) = iprot.readListBegin()
+                    for _i143 in range(_size139):
+                        _elem144 = iprot.readBinary()
+                        self.range_end.append(_elem144)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype141, _size138) = iprot.readListBegin()
-                    for _i142 in range(_size138):
-                        _elem143 = iprot.readBinary()
-                        self.offset_key.append(_elem143)
+                    (_etype148, _size145) = iprot.readListBegin()
+                    for _i149 in range(_size145):
+                        _elem150 = iprot.readBinary()
+                        self.offset_key.append(_elem150)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype147, _size144) = iprot.readListBegin()
-                    for _i148 in range(_size144):
-                        _elem149 = SpecKeyInterval()
-                        _elem149.read(iprot)
-                        self.key_intervals.append(_elem149)
+                    (_etype154, _size151) = iprot.readListBegin()
+                    for _i155 in range(_size151):
+                        _elem156 = SpecKeyInterval()
+                        _elem156.read(iprot)
+                        self.key_intervals.append(_elem156)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype153, _size150) = iprot.readListBegin()
-                    for _i154 in range(_size150):
-                        _elem155 = SpecValueSerial()
-                        _elem155.read(iprot)
-                        self.values.append(_elem155)
+                    (_etype160, _size157) = iprot.readListBegin()
+                    for _i161 in range(_size157):
+                        _elem162 = SpecValueSerial()
+                        _elem162.read(iprot)
+                        self.values.append(_elem162)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -2954,48 +3173,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecIntervalSerial')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter156 in self.range_begin:
-                oprot.writeBinary(iter156)
+            for iter163 in self.range_begin:
+                oprot.writeBinary(iter163)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter157 in self.range_end:
-                oprot.writeBinary(iter157)
+            for iter164 in self.range_end:
+                oprot.writeBinary(iter164)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter158 in self.offset_key:
-                oprot.writeBinary(iter158)
+            for iter165 in self.offset_key:
+                oprot.writeBinary(iter165)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter159 in self.key_intervals:
-                iter159.write(oprot)
+            for iter166 in self.key_intervals:
+                iter166.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter160 in self.values:
-                iter160.write(oprot)
+            for iter167 in self.values:
+                iter167.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -3072,19 +3291,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype164, _size161) = iprot.readListBegin()
-                    for _i165 in range(_size161):
-                        _elem166 = SpecIntervalSerial()
-                        _elem166.read(iprot)
-                        self.intervals.append(_elem166)
+                    (_etype171, _size168) = iprot.readListBegin()
+                    for _i172 in range(_size168):
+                        _elem173 = SpecIntervalSerial()
+                        _elem173.read(iprot)
+                        self.intervals.append(_elem173)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3097,16 +3316,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter167 in self.intervals:
-                iter167.write(oprot)
+            for iter174 in self.intervals:
+                iter174.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3161,30 +3380,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.columns = []
-                    (_etype171, _size168) = iprot.readListBegin()
-                    for _i172 in range(_size168):
-                        _elem173 = SpecColumn()
-                        _elem173.read(iprot)
-                        self.columns.append(_elem173)
+                    (_etype178, _size175) = iprot.readListBegin()
+                    for _i179 in range(_size175):
+                        _elem180 = SpecColumn()
+                        _elem180.read(iprot)
+                        self.columns.append(_elem180)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.columns_serial = []
-                    (_etype177, _size174) = iprot.readListBegin()
-                    for _i178 in range(_size174):
-                        _elem179 = SpecColumnSerial()
-                        _elem179.read(iprot)
-                        self.columns_serial.append(_elem179)
+                    (_etype184, _size181) = iprot.readListBegin()
+                    for _i185 in range(_size181):
+                        _elem186 = SpecColumnSerial()
+                        _elem186.read(iprot)
+                        self.columns_serial.append(_elem186)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRUCT:
                     self.flags = SpecFlags()
                     self.flags.read(iprot)
@@ -3199,23 +3418,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecScan')
         if self.columns is not None:
             oprot.writeFieldBegin('columns', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.columns))
-            for iter180 in self.columns:
-                iter180.write(oprot)
+            for iter187 in self.columns:
+                iter187.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columns_serial is not None:
             oprot.writeFieldBegin('columns_serial', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.columns_serial))
-            for iter181 in self.columns_serial:
-                iter181.write(oprot)
+            for iter188 in self.columns_serial:
+                iter188.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.flags is not None:
             oprot.writeFieldBegin('flags', TType.STRUCT, 3)
             self.flags.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3288,18 +3507,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype185, _size182) = iprot.readListBegin()
-                    for _i186 in range(_size182):
-                        _elem187 = iprot.readBinary()
-                        self.k.append(_elem187)
+                    (_etype192, _size189) = iprot.readListBegin()
+                    for _i193 in range(_size189):
+                        _elem194 = iprot.readBinary()
+                        self.k.append(_elem194)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3332,16 +3551,16 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter188 in self.k:
-                oprot.writeBinary(iter188)
+            for iter195 in self.k:
+                oprot.writeBinary(iter195)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
@@ -3444,38 +3663,38 @@
                 if ftype == TType.STRING:
                     self.v_bytes = iprot.readBinary()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v_key = []
-                    (_etype192, _size189) = iprot.readListBegin()
-                    for _i193 in range(_size189):
-                        _elem194 = iprot.readBinary()
-                        self.v_key.append(_elem194)
+                    (_etype199, _size196) = iprot.readListBegin()
+                    for _i200 in range(_size196):
+                        _elem201 = iprot.readBinary()
+                        self.v_key.append(_elem201)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.v_li = []
-                    (_etype198, _size195) = iprot.readListBegin()
-                    for _i199 in range(_size195):
-                        _elem200 = iprot.readI64()
-                        self.v_li.append(_elem200)
+                    (_etype205, _size202) = iprot.readListBegin()
+                    for _i206 in range(_size202):
+                        _elem207 = iprot.readI64()
+                        self.v_li.append(_elem207)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.v_lb = []
-                    (_etype204, _size201) = iprot.readListBegin()
-                    for _i205 in range(_size201):
-                        _elem206 = iprot.readBinary()
-                        self.v_lb.append(_elem206)
+                    (_etype211, _size208) = iprot.readListBegin()
+                    for _i212 in range(_size208):
+                        _elem213 = iprot.readBinary()
+                        self.v_lb.append(_elem213)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3500,30 +3719,499 @@
         if self.v_bytes is not None:
             oprot.writeFieldBegin('v_bytes', TType.STRING, 4)
             oprot.writeBinary(self.v_bytes)
             oprot.writeFieldEnd()
         if self.v_key is not None:
             oprot.writeFieldBegin('v_key', TType.LIST, 5)
             oprot.writeListBegin(TType.STRING, len(self.v_key))
-            for iter207 in self.v_key:
-                oprot.writeBinary(iter207)
+            for iter214 in self.v_key:
+                oprot.writeBinary(iter214)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_li is not None:
             oprot.writeFieldBegin('v_li', TType.LIST, 6)
             oprot.writeListBegin(TType.I64, len(self.v_li))
-            for iter208 in self.v_li:
-                oprot.writeI64(iter208)
+            for iter215 in self.v_li:
+                oprot.writeI64(iter215)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_lb is not None:
             oprot.writeFieldBegin('v_lb', TType.LIST, 7)
             oprot.writeListBegin(TType.STRING, len(self.v_lb))
-            for iter209 in self.v_lb:
-                oprot.writeBinary(iter209)
+            for iter216 in self.v_lb:
+                oprot.writeBinary(iter216)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_INT64(object):
+    """
+    Serial INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.I64:
+                    self.v = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_INT64')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.I64, 5)
+            oprot.writeI64(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_DOUBLE(object):
+    """
+    Serial DOUBLE Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.DOUBLE:
+                    self.v = iprot.readDouble()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_DOUBLE')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.DOUBLE, 5)
+            oprot.writeDouble(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_BYTES(object):
+    """
+    Serial BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRING:
+                    self.v = iprot.readBinary()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_BYTES')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.STRING, 5)
+            oprot.writeBinary(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_LI(object):
+    """
+    Serial LIST_INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype220, _size217) = iprot.readListBegin()
+                    for _i221 in range(_size217):
+                        _elem222 = FU_INT64()
+                        _elem222.read(iprot)
+                        self.v.append(_elem222)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LI')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter223 in self.v:
+                iter223.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3543,14 +4231,284 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class FU_LB(object):
+    """
+    Serial LIST_BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype227, _size224) = iprot.readListBegin()
+                    for _i228 in range(_size224):
+                        _elem229 = FU_BYTES()
+                        _elem229.read(iprot)
+                        self.v.append(_elem229)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LB')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter230 in self.v:
+                iter230.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class CellValueSerialOp(object):
+    """
+    The Serial Values Cell field with Update Operation
+
+    Attributes:
+     - field_id: The Field ID, a single ID can have any/all the field types
+     - v_int64: The INT64 type update-field
+     - v_double: The DOUBLE type update-field
+     - v_bytes: The BYTES type update-field
+     - v_key: The Cell KEY type update-field
+     - v_li: The LIST INT64 type update-field
+     - v_lb: The LIST BYTES type update-field
+
+    """
+
+    __slots__ = (
+        'field_id',
+        'v_int64',
+        'v_double',
+        'v_bytes',
+        'v_key',
+        'v_li',
+        'v_lb',
+    )
+
+
+    def __init__(self, field_id=None, v_int64=None, v_double=None, v_bytes=None, v_key=None, v_li=None, v_lb=None,):
+        self.field_id = field_id
+        self.v_int64 = v_int64
+        self.v_double = v_double
+        self.v_bytes = v_bytes
+        self.v_key = v_key
+        self.v_li = v_li
+        self.v_lb = v_lb
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.field_id = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.v_int64 = FU_INT64()
+                    self.v_int64.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRUCT:
+                    self.v_double = FU_DOUBLE()
+                    self.v_double.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.v_bytes = FU_BYTES()
+                    self.v_bytes.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.LIST:
+                    self.v_key = []
+                    (_etype234, _size231) = iprot.readListBegin()
+                    for _i235 in range(_size231):
+                        _elem236 = iprot.readBinary()
+                        self.v_key.append(_elem236)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.STRUCT:
+                    self.v_li = FU_LI()
+                    self.v_li.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 7:
+                if ftype == TType.STRUCT:
+                    self.v_lb = FU_LB()
+                    self.v_lb.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('CellValueSerialOp')
+        if self.field_id is not None:
+            oprot.writeFieldBegin('field_id', TType.I32, 1)
+            oprot.writeI32(self.field_id)
+            oprot.writeFieldEnd()
+        if self.v_int64 is not None:
+            oprot.writeFieldBegin('v_int64', TType.STRUCT, 2)
+            self.v_int64.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_double is not None:
+            oprot.writeFieldBegin('v_double', TType.STRUCT, 3)
+            self.v_double.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_bytes is not None:
+            oprot.writeFieldBegin('v_bytes', TType.STRUCT, 4)
+            self.v_bytes.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_key is not None:
+            oprot.writeFieldBegin('v_key', TType.LIST, 5)
+            oprot.writeListBegin(TType.STRING, len(self.v_key))
+            for iter237 in self.v_key:
+                oprot.writeBinary(iter237)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_li is not None:
+            oprot.writeFieldBegin('v_li', TType.STRUCT, 6)
+            self.v_li.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_lb is not None:
+            oprot.writeFieldBegin('v_lb', TType.STRUCT, 7)
+            self.v_lb.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class UCellSerial(object):
     """
     The Cell data for using with Update of SERIAL Column Type
 
     Attributes:
      - f: The Cell Flag
      - k: The Cell Key
@@ -3592,18 +4550,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype213, _size210) = iprot.readListBegin()
-                    for _i214 in range(_size210):
-                        _elem215 = iprot.readBinary()
-                        self.k.append(_elem215)
+                    (_etype241, _size238) = iprot.readListBegin()
+                    for _i242 in range(_size238):
+                        _elem243 = iprot.readBinary()
+                        self.k.append(_elem243)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3612,19 +4570,19 @@
                 if ftype == TType.BOOL:
                     self.ts_desc = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype219, _size216) = iprot.readListBegin()
-                    for _i220 in range(_size216):
-                        _elem221 = CellValueSerial()
-                        _elem221.read(iprot)
-                        self.v.append(_elem221)
+                    (_etype247, _size244) = iprot.readListBegin()
+                    for _i248 in range(_size244):
+                        _elem249 = CellValueSerial()
+                        _elem249.read(iprot)
+                        self.v.append(_elem249)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
@@ -3642,31 +4600,31 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter222 in self.k:
-                oprot.writeBinary(iter222)
+            for iter250 in self.k:
+                oprot.writeBinary(iter250)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
             oprot.writeFieldBegin('ts_desc', TType.BOOL, 4)
             oprot.writeBool(self.ts_desc)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter223 in self.v:
-                iter223.write(oprot)
+            for iter251 in self.v:
+                iter251.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 6)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3733,18 +4691,18 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype227, _size224) = iprot.readListBegin()
-                    for _i228 in range(_size224):
-                        _elem229 = iprot.readBinary()
-                        self.k.append(_elem229)
+                    (_etype255, _size252) = iprot.readListBegin()
+                    for _i256 in range(_size252):
+                        _elem257 = iprot.readBinary()
+                        self.k.append(_elem257)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3767,16 +4725,16 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter230 in self.k:
-                oprot.writeBinary(iter230)
+            for iter258 in self.k:
+                oprot.writeBinary(iter258)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -3847,34 +4805,34 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype234, _size231) = iprot.readListBegin()
-                    for _i235 in range(_size231):
-                        _elem236 = iprot.readBinary()
-                        self.k.append(_elem236)
+                    (_etype262, _size259) = iprot.readListBegin()
+                    for _i263 in range(_size259):
+                        _elem264 = iprot.readBinary()
+                        self.k.append(_elem264)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype240, _size237) = iprot.readListBegin()
-                    for _i241 in range(_size237):
-                        _elem242 = CellValueSerial()
-                        _elem242.read(iprot)
-                        self.v.append(_elem242)
+                    (_etype268, _size265) = iprot.readListBegin()
+                    for _i269 in range(_size265):
+                        _elem270 = CellValueSerial()
+                        _elem270.read(iprot)
+                        self.v.append(_elem270)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3887,27 +4845,27 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter243 in self.k:
-                oprot.writeBinary(iter243)
+            for iter271 in self.k:
+                oprot.writeBinary(iter271)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter244 in self.v:
-                iter244.write(oprot)
+            for iter272 in self.v:
+                iter272.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3959,30 +4917,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype248, _size245) = iprot.readListBegin()
-                    for _i249 in range(_size245):
-                        _elem250 = Cell()
-                        _elem250.read(iprot)
-                        self.cells.append(_elem250)
+                    (_etype276, _size273) = iprot.readListBegin()
+                    for _i277 in range(_size273):
+                        _elem278 = Cell()
+                        _elem278.read(iprot)
+                        self.cells.append(_elem278)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype254, _size251) = iprot.readListBegin()
-                    for _i255 in range(_size251):
-                        _elem256 = CellSerial()
-                        _elem256.read(iprot)
-                        self.serial_cells.append(_elem256)
+                    (_etype282, _size279) = iprot.readListBegin()
+                    for _i283 in range(_size279):
+                        _elem284 = CellSerial()
+                        _elem284.read(iprot)
+                        self.serial_cells.append(_elem284)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3991,23 +4949,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Cells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter257 in self.cells:
-                iter257.write(oprot)
+            for iter285 in self.cells:
+                iter285.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter258 in self.serial_cells:
-                iter258.write(oprot)
+            for iter286 in self.serial_cells:
+                iter286.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4062,18 +5020,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype262, _size259) = iprot.readListBegin()
-                    for _i263 in range(_size259):
-                        _elem264 = iprot.readBinary()
-                        self.k.append(_elem264)
+                    (_etype290, _size287) = iprot.readListBegin()
+                    for _i291 in range(_size287):
+                        _elem292 = iprot.readBinary()
+                        self.k.append(_elem292)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -4092,16 +5050,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCell')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter265 in self.k:
-                oprot.writeBinary(iter265)
+            for iter293 in self.k:
+                oprot.writeBinary(iter293)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -4164,34 +5122,34 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype269, _size266) = iprot.readListBegin()
-                    for _i270 in range(_size266):
-                        _elem271 = iprot.readBinary()
-                        self.k.append(_elem271)
+                    (_etype297, _size294) = iprot.readListBegin()
+                    for _i298 in range(_size294):
+                        _elem299 = iprot.readBinary()
+                        self.k.append(_elem299)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype275, _size272) = iprot.readListBegin()
-                    for _i276 in range(_size272):
-                        _elem277 = CellValueSerial()
-                        _elem277.read(iprot)
-                        self.v.append(_elem277)
+                    (_etype303, _size300) = iprot.readListBegin()
+                    for _i304 in range(_size300):
+                        _elem305 = CellValueSerial()
+                        _elem305.read(iprot)
+                        self.v.append(_elem305)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4200,27 +5158,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCellSerial')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter278 in self.k:
-                oprot.writeBinary(iter278)
+            for iter306 in self.k:
+                oprot.writeBinary(iter306)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter279 in self.v:
-                iter279.write(oprot)
+            for iter307 in self.v:
+                iter307.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4272,30 +5230,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype283, _size280) = iprot.readListBegin()
-                    for _i284 in range(_size280):
-                        _elem285 = CCell()
-                        _elem285.read(iprot)
-                        self.cells.append(_elem285)
+                    (_etype311, _size308) = iprot.readListBegin()
+                    for _i312 in range(_size308):
+                        _elem313 = CCell()
+                        _elem313.read(iprot)
+                        self.cells.append(_elem313)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype289, _size286) = iprot.readListBegin()
-                    for _i290 in range(_size286):
-                        _elem291 = CCellSerial()
-                        _elem291.read(iprot)
-                        self.serial_cells.append(_elem291)
+                    (_etype317, _size314) = iprot.readListBegin()
+                    for _i318 in range(_size314):
+                        _elem319 = CCellSerial()
+                        _elem319.read(iprot)
+                        self.serial_cells.append(_elem319)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4304,23 +5262,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ColCells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter292 in self.cells:
-                iter292.write(oprot)
+            for iter320 in self.cells:
+                iter320.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter293 in self.serial_cells:
-                iter293.write(oprot)
+            for iter321 in self.serial_cells:
+                iter321.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4479,19 +5437,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype297, _size294) = iprot.readListBegin()
-                    for _i298 in range(_size294):
-                        _elem299 = CellValueSerial()
-                        _elem299.read(iprot)
-                        self.v.append(_elem299)
+                    (_etype325, _size322) = iprot.readListBegin()
+                    for _i326 in range(_size322):
+                        _elem327 = CellValueSerial()
+                        _elem327.read(iprot)
+                        self.v.append(_elem327)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4508,16 +5466,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter300 in self.v:
-                iter300.write(oprot)
+            for iter328 in self.v:
+                iter328.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4572,40 +5530,40 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype304, _size301) = iprot.readListBegin()
-                    for _i305 in range(_size301):
-                        _elem306 = iprot.readBinary()
-                        self.k.append(_elem306)
+                    (_etype332, _size329) = iprot.readListBegin()
+                    for _i333 in range(_size329):
+                        _elem334 = iprot.readBinary()
+                        self.k.append(_elem334)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype310, _size307) = iprot.readListBegin()
-                    for _i311 in range(_size307):
-                        _elem312 = KCell()
-                        _elem312.read(iprot)
-                        self.cells.append(_elem312)
+                    (_etype338, _size335) = iprot.readListBegin()
+                    for _i339 in range(_size335):
+                        _elem340 = KCell()
+                        _elem340.read(iprot)
+                        self.cells.append(_elem340)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype316, _size313) = iprot.readListBegin()
-                    for _i317 in range(_size313):
-                        _elem318 = KCellSerial()
-                        _elem318.read(iprot)
-                        self.serial_cells.append(_elem318)
+                    (_etype344, _size341) = iprot.readListBegin()
+                    for _i345 in range(_size341):
+                        _elem346 = KCellSerial()
+                        _elem346.read(iprot)
+                        self.serial_cells.append(_elem346)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4614,30 +5572,30 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('kCells')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter319 in self.k:
-                oprot.writeBinary(iter319)
+            for iter347 in self.k:
+                oprot.writeBinary(iter347)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter320 in self.cells:
-                iter320.write(oprot)
+            for iter348 in self.cells:
+                iter348.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter321 in self.serial_cells:
-                iter321.write(oprot)
+            for iter349 in self.serial_cells:
+                iter349.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4796,19 +5754,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype325, _size322) = iprot.readListBegin()
-                    for _i326 in range(_size322):
-                        _elem327 = CellValueSerial()
-                        _elem327.read(iprot)
-                        self.v.append(_elem327)
+                    (_etype353, _size350) = iprot.readListBegin()
+                    for _i354 in range(_size350):
+                        _elem355 = CellValueSerial()
+                        _elem355.read(iprot)
+                        self.v.append(_elem355)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4825,16 +5783,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter328 in self.v:
-                iter328.write(oprot)
+            for iter356 in self.v:
+                iter356.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4889,42 +5847,42 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.f = {}
-                    (_ktype330, _vtype331, _size329) = iprot.readMapBegin()
-                    for _i333 in range(_size329):
-                        _key334 = iprot.readBinary()
-                        _val335 = FCells()
-                        _val335.read(iprot)
-                        self.f[_key334] = _val335
+                    (_ktype358, _vtype359, _size357) = iprot.readMapBegin()
+                    for _i361 in range(_size357):
+                        _key362 = iprot.readBinary()
+                        _val363 = FCells()
+                        _val363.read(iprot)
+                        self.f[_key362] = _val363
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype339, _size336) = iprot.readListBegin()
-                    for _i340 in range(_size336):
-                        _elem341 = FCell()
-                        _elem341.read(iprot)
-                        self.cells.append(_elem341)
+                    (_etype367, _size364) = iprot.readListBegin()
+                    for _i368 in range(_size364):
+                        _elem369 = FCell()
+                        _elem369.read(iprot)
+                        self.cells.append(_elem369)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype345, _size342) = iprot.readListBegin()
-                    for _i346 in range(_size342):
-                        _elem347 = FCellSerial()
-                        _elem347.read(iprot)
-                        self.serial_cells.append(_elem347)
+                    (_etype373, _size370) = iprot.readListBegin()
+                    for _i374 in range(_size370):
+                        _elem375 = FCellSerial()
+                        _elem375.read(iprot)
+                        self.serial_cells.append(_elem375)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4933,31 +5891,31 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('FCells')
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.MAP, 1)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.f))
-            for kiter348, viter349 in self.f.items():
-                oprot.writeBinary(kiter348)
-                viter349.write(oprot)
+            for kiter376, viter377 in self.f.items():
+                oprot.writeBinary(kiter376)
+                viter377.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter350 in self.cells:
-                iter350.write(oprot)
+            for iter378 in self.cells:
+                iter378.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter351 in self.serial_cells:
-                iter351.write(oprot)
+            for iter379 in self.serial_cells:
+                iter379.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5021,31 +5979,31 @@
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.ccells = {}
-                    (_ktype353, _vtype354, _size352) = iprot.readMapBegin()
-                    for _i356 in range(_size352):
-                        _key357 = iprot.readString()
-                        _val358 = ColCells()
-                        _val358.read(iprot)
-                        self.ccells[_key357] = _val358
+                    (_ktype381, _vtype382, _size380) = iprot.readMapBegin()
+                    for _i384 in range(_size380):
+                        _key385 = iprot.readString()
+                        _val386 = ColCells()
+                        _val386.read(iprot)
+                        self.ccells[_key385] = _val386
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.kcells = []
-                    (_etype362, _size359) = iprot.readListBegin()
-                    for _i363 in range(_size359):
-                        _elem364 = kCells()
-                        _elem364.read(iprot)
-                        self.kcells.append(_elem364)
+                    (_etype390, _size387) = iprot.readListBegin()
+                    for _i391 in range(_size387):
+                        _elem392 = kCells()
+                        _elem392.read(iprot)
+                        self.kcells.append(_elem392)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.fcells = FCells()
                     self.fcells.read(iprot)
@@ -5064,24 +6022,24 @@
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 1)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.ccells is not None:
             oprot.writeFieldBegin('ccells', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.ccells))
-            for kiter365, viter366 in self.ccells.items():
-                oprot.writeString(kiter365)
-                viter366.write(oprot)
+            for kiter393, viter394 in self.ccells.items():
+                oprot.writeString(kiter393)
+                viter394.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.kcells is not None:
             oprot.writeFieldBegin('kcells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.kcells))
-            for iter367 in self.kcells:
-                iter367.write(oprot)
+            for iter395 in self.kcells:
+                iter395.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.fcells is not None:
             oprot.writeFieldBegin('fcells', TType.STRUCT, 4)
             self.fcells.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5222,36 +6180,36 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemas = []
-                    (_etype371, _size368) = iprot.readListBegin()
-                    for _i372 in range(_size368):
-                        _elem373 = Schema()
-                        _elem373.read(iprot)
-                        self.schemas.append(_elem373)
+                    (_etype399, _size396) = iprot.readListBegin()
+                    for _i400 in range(_size396):
+                        _elem401 = Schema()
+                        _elem401.read(iprot)
+                        self.schemas.append(_elem401)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRUCT:
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.compact = []
-                    (_etype377, _size374) = iprot.readListBegin()
-                    for _i378 in range(_size374):
-                        _elem379 = CompactResult()
-                        _elem379.read(iprot)
-                        self.compact.append(_elem379)
+                    (_etype405, _size402) = iprot.readListBegin()
+                    for _i406 in range(_size402):
+                        _elem407 = CompactResult()
+                        _elem407.read(iprot)
+                        self.compact.append(_elem407)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5260,27 +6218,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Result')
         if self.schemas is not None:
             oprot.writeFieldBegin('schemas', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemas))
-            for iter380 in self.schemas:
-                iter380.write(oprot)
+            for iter408 in self.schemas:
+                iter408.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 2)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.compact is not None:
             oprot.writeFieldBegin('compact', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.compact))
-            for iter381 in self.compact:
-                iter381.write(oprot)
+            for iter409 in self.compact:
+                iter409.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5384,27 +6342,36 @@
 )
 all_structs.append(SpecValue)
 SpecValue.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'comp', None, None, ),  # 1
     (2, TType.STRING, 'v', 'BINARY', None, ),  # 2
 )
+all_structs.append(SpecUpdateOP)
+SpecUpdateOP.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'op', None, None, ),  # 1
+    (2, TType.I32, 'pos', None, None, ),  # 2
+)
 all_structs.append(SpecIntervalUpdate)
 SpecIntervalUpdate.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'v', 'BINARY', None, ),  # 1
     (2, TType.I64, 'ts', None, None, ),  # 2
     (3, TType.I32, 'encoder', None, None, ),  # 3
+    (4, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 4
 )
 all_structs.append(SpecIntervalUpdateSerial)
 SpecIntervalUpdateSerial.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'ts', None, None, ),  # 1
     (2, TType.LIST, 'v', (TType.STRUCT, [CellValueSerial, None], False), None, ),  # 2
-    (3, TType.I32, 'encoder', None, None, ),  # 3
+    (3, TType.LIST, 'v_op', (TType.STRUCT, [CellValueSerialOp, None], False), None, ),  # 3
+    (4, TType.I32, 'encoder', None, None, ),  # 4
+    (5, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 5
 )
 all_structs.append(SpecInterval)
 SpecInterval.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'range_begin', (TType.STRING, 'BINARY', False), None, ),  # 1
     (2, TType.LIST, 'range_end', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.LIST, 'offset_key', (TType.STRING, 'BINARY', False), None, ),  # 3
@@ -5521,14 +6488,68 @@
     (2, TType.I64, 'v_int64', None, None, ),  # 2
     (3, TType.DOUBLE, 'v_double', None, None, ),  # 3
     (4, TType.STRING, 'v_bytes', 'BINARY', None, ),  # 4
     (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
     (6, TType.LIST, 'v_li', (TType.I64, None, False), None, ),  # 6
     (7, TType.LIST, 'v_lb', (TType.STRING, 'BINARY', False), None, ),  # 7
 )
+all_structs.append(FU_INT64)
+FU_INT64.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.I64, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_DOUBLE)
+FU_DOUBLE.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.DOUBLE, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_BYTES)
+FU_BYTES.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.STRING, 'v', 'BINARY', None, ),  # 5
+)
+all_structs.append(FU_LI)
+FU_LI.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_INT64, None], False), None, ),  # 4
+)
+all_structs.append(FU_LB)
+FU_LB.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_BYTES, None], False), None, ),  # 4
+)
+all_structs.append(CellValueSerialOp)
+CellValueSerialOp.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'field_id', None, None, ),  # 1
+    (2, TType.STRUCT, 'v_int64', [FU_INT64, None], None, ),  # 2
+    (3, TType.STRUCT, 'v_double', [FU_DOUBLE, None], None, ),  # 3
+    (4, TType.STRUCT, 'v_bytes', [FU_BYTES, None], None, ),  # 4
+    (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
+    (6, TType.STRUCT, 'v_li', [FU_LI, None], None, ),  # 6
+    (7, TType.STRUCT, 'v_lb', [FU_LB, None], None, ),  # 7
+)
 all_structs.append(UCellSerial)
 UCellSerial.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'f', None, None, ),  # 1
     (2, TType.LIST, 'k', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.I64, 'ts', None, None, ),  # 3
     (4, TType.BOOL, 'ts_desc', None, None, ),  # 4
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/zopeif/Service.py` & `swcdb-0.5.9.0/swcdb/thrift/zopeif/Service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1929,19 +1929,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype385, _size382) = iprot.readListBegin()
-                    for _i386 in range(_size382):
-                        _elem387 = Schema()
-                        _elem387.read(iprot)
-                        self.success.append(_elem387)
+                    (_etype413, _size410) = iprot.readListBegin()
+                    for _i414 in range(_size410):
+                        _elem415 = Schema()
+                        _elem415.read(iprot)
+                        self.success.append(_elem415)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -1955,16 +1955,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter388 in self.success:
-                iter388.write(oprot)
+            for iter416 in self.success:
+                iter416.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2096,19 +2096,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype392, _size389) = iprot.readListBegin()
-                    for _i393 in range(_size389):
-                        _elem394 = CompactResult()
-                        _elem394.read(iprot)
-                        self.success.append(_elem394)
+                    (_etype420, _size417) = iprot.readListBegin()
+                    for _i421 in range(_size417):
+                        _elem422 = CompactResult()
+                        _elem422.read(iprot)
+                        self.success.append(_elem422)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2122,16 +2122,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter395 in self.success:
-                iter395.write(oprot)
+            for iter423 in self.success:
+                iter423.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2422,20 +2422,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype397, _vtype398, _size396) = iprot.readMapBegin()
-                    for _i400 in range(_size396):
-                        _key401 = iprot.readString()
-                        _val402 = ColCells()
-                        _val402.read(iprot)
-                        self.success[_key401] = _val402
+                    (_ktype425, _vtype426, _size424) = iprot.readMapBegin()
+                    for _i428 in range(_size424):
+                        _key429 = iprot.readString()
+                        _val430 = ColCells()
+                        _val430.read(iprot)
+                        self.success[_key429] = _val430
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2449,17 +2449,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter403, viter404 in self.success.items():
-                oprot.writeString(kiter403)
-                viter404.write(oprot)
+            for kiter431, viter432 in self.success.items():
+                oprot.writeString(kiter431)
+                viter432.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2591,19 +2591,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype408, _size405) = iprot.readListBegin()
-                    for _i409 in range(_size405):
-                        _elem410 = kCells()
-                        _elem410.read(iprot)
-                        self.success.append(_elem410)
+                    (_etype436, _size433) = iprot.readListBegin()
+                    for _i437 in range(_size433):
+                        _elem438 = kCells()
+                        _elem438.read(iprot)
+                        self.success.append(_elem438)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2617,16 +2617,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter411 in self.success:
-                iter411.write(oprot)
+            for iter439 in self.success:
+                iter439.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3638,25 +3638,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype413, _vtype414, _size412) = iprot.readMapBegin()
-                    for _i416 in range(_size412):
-                        _key417 = iprot.readI64()
-                        _val418 = []
-                        (_etype422, _size419) = iprot.readListBegin()
-                        for _i423 in range(_size419):
-                            _elem424 = UCell()
-                            _elem424.read(iprot)
-                            _val418.append(_elem424)
+                    (_ktype441, _vtype442, _size440) = iprot.readMapBegin()
+                    for _i444 in range(_size440):
+                        _key445 = iprot.readI64()
+                        _val446 = []
+                        (_etype450, _size447) = iprot.readListBegin()
+                        for _i451 in range(_size447):
+                            _elem452 = UCell()
+                            _elem452.read(iprot)
+                            _val446.append(_elem452)
                         iprot.readListEnd()
-                        self.cells[_key417] = _val418
+                        self.cells[_key445] = _val446
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -3670,19 +3670,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter425, viter426 in self.cells.items():
-                oprot.writeI64(kiter425)
-                oprot.writeListBegin(TType.STRUCT, len(viter426))
-                for iter427 in viter426:
-                    iter427.write(oprot)
+            for kiter453, viter454 in self.cells.items():
+                oprot.writeI64(kiter453)
+                oprot.writeListBegin(TType.STRUCT, len(viter454))
+                for iter455 in viter454:
+                    iter455.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -3816,25 +3816,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype429, _vtype430, _size428) = iprot.readMapBegin()
-                    for _i432 in range(_size428):
-                        _key433 = iprot.readI64()
-                        _val434 = []
-                        (_etype438, _size435) = iprot.readListBegin()
-                        for _i439 in range(_size435):
-                            _elem440 = UCellSerial()
-                            _elem440.read(iprot)
-                            _val434.append(_elem440)
+                    (_ktype457, _vtype458, _size456) = iprot.readMapBegin()
+                    for _i460 in range(_size456):
+                        _key461 = iprot.readI64()
+                        _val462 = []
+                        (_etype466, _size463) = iprot.readListBegin()
+                        for _i467 in range(_size463):
+                            _elem468 = UCellSerial()
+                            _elem468.read(iprot)
+                            _val462.append(_elem468)
                         iprot.readListEnd()
-                        self.cells[_key433] = _val434
+                        self.cells[_key461] = _val462
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -3848,19 +3848,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_serial_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter441, viter442 in self.cells.items():
-                oprot.writeI64(kiter441)
-                oprot.writeListBegin(TType.STRUCT, len(viter442))
-                for iter443 in viter442:
-                    iter443.write(oprot)
+            for kiter469, viter470 in self.cells.items():
+                oprot.writeI64(kiter469)
+                oprot.writeListBegin(TType.STRUCT, len(viter470))
+                for iter471 in viter470:
+                    iter471.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -4228,19 +4228,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype447, _size444) = iprot.readListBegin()
-                    for _i448 in range(_size444):
-                        _elem449 = Schema()
-                        _elem449.read(iprot)
-                        self.success.append(_elem449)
+                    (_etype475, _size472) = iprot.readListBegin()
+                    for _i476 in range(_size472):
+                        _elem477 = Schema()
+                        _elem477.read(iprot)
+                        self.success.append(_elem477)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4254,16 +4254,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter450 in self.success:
-                iter450.write(oprot)
+            for iter478 in self.success:
+                iter478.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4396,19 +4396,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype454, _size451) = iprot.readListBegin()
-                    for _i455 in range(_size451):
-                        _elem456 = CompactResult()
-                        _elem456.read(iprot)
-                        self.success.append(_elem456)
+                    (_etype482, _size479) = iprot.readListBegin()
+                    for _i483 in range(_size479):
+                        _elem484 = CompactResult()
+                        _elem484.read(iprot)
+                        self.success.append(_elem484)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4422,16 +4422,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter457 in self.success:
-                iter457.write(oprot)
+            for iter485 in self.success:
+                iter485.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4724,20 +4724,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype459, _vtype460, _size458) = iprot.readMapBegin()
-                    for _i462 in range(_size458):
-                        _key463 = iprot.readString()
-                        _val464 = ColCells()
-                        _val464.read(iprot)
-                        self.success[_key463] = _val464
+                    (_ktype487, _vtype488, _size486) = iprot.readMapBegin()
+                    for _i490 in range(_size486):
+                        _key491 = iprot.readString()
+                        _val492 = ColCells()
+                        _val492.read(iprot)
+                        self.success[_key491] = _val492
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4751,17 +4751,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter465, viter466 in self.success.items():
-                oprot.writeString(kiter465)
-                viter466.write(oprot)
+            for kiter493, viter494 in self.success.items():
+                oprot.writeString(kiter493)
+                viter494.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4894,19 +4894,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype470, _size467) = iprot.readListBegin()
-                    for _i471 in range(_size467):
-                        _elem472 = kCells()
-                        _elem472.read(iprot)
-                        self.success.append(_elem472)
+                    (_etype498, _size495) = iprot.readListBegin()
+                    for _i499 in range(_size495):
+                        _elem500 = kCells()
+                        _elem500.read(iprot)
+                        self.success.append(_elem500)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4920,16 +4920,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter473 in self.success:
-                iter473.write(oprot)
+            for iter501 in self.success:
+                iter501.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/zopeif/ttypes.py` & `swcdb-0.5.9.0/swcdb/thrift/zopeif/ttypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,14 +246,41 @@
 
     _NAMES_TO_VALUES = {
         "UPDATING": 4,
         "DELETING": 8,
     }
 
 
+class UpdateOP(object):
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    SERIAL = 5
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "SERIAL",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "SERIAL": 5,
+    }
+
+
 class Flag(object):
     """
     The Cell Flag
 
     """
     NONE = 0
     INSERT = 1
@@ -271,14 +298,79 @@
         "NONE": 0,
         "INSERT": 1,
         "DELETE_LE": 2,
         "DELETE_EQ": 3,
     }
 
 
+class FU_MATH_OP(object):
+    """
+    MATH Operations for Serial Field Update of types INT64 and DOUBLE
+
+    """
+    EQUAL = 0
+    PLUS = 1
+    MULTIPLY = 2
+    DIVIDE = 3
+
+    _VALUES_TO_NAMES = {
+        0: "EQUAL",
+        1: "PLUS",
+        2: "MULTIPLY",
+        3: "DIVIDE",
+    }
+
+    _NAMES_TO_VALUES = {
+        "EQUAL": 0,
+        "PLUS": 1,
+        "MULTIPLY": 2,
+        "DIVIDE": 3,
+    }
+
+
+class FU_LIST_OP(object):
+    """
+    LIST Operations for Serial Field Update of array/list/bytes with LIST-op in the inner SERIAL fields
+
+    """
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    ERASE = 5
+    BY_UNIQUE = 6
+    BY_COND = 7
+    BY_INDEX = 8
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "ERASE",
+        6: "BY_UNIQUE",
+        7: "BY_COND",
+        8: "BY_INDEX",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "ERASE": 5,
+        "BY_UNIQUE": 6,
+        "BY_COND": 7,
+        "BY_INDEX": 8,
+    }
+
+
 class CellsResult(object):
     """
     The Cells Results types for using with CellsGroup requests
 
     """
     IN_LIST = 0
     ON_COLUMN = 1
@@ -1519,36 +1611,119 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class SpecUpdateOP(object):
+    """
+    Attributes:
+     - op: The Operation of update
+     - pos: The position/index of INSERT and OVERWRITE update operations
+
+    """
+
+    __slots__ = (
+        'op',
+        'pos',
+    )
+
+
+    def __init__(self, op=None, pos=None,):
+        self.op = op
+        self.pos = pos
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('SpecUpdateOP')
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 1)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 2)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class SpecIntervalUpdate(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecInterval
 
     Attributes:
      - v: The value for the updated cell
      - ts: The timestamp for the updated cell NULL: MIN_INT64+1, AUTO:MIN_INT64+2 (or not-set)
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'v',
         'ts',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, v=None, ts=None, encoder=None,):
+    def __init__(self, v=None, ts=None, encoder=None, update_op=None,):
         self.v = v
         self.ts = ts
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1566,14 +1741,20 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1588,14 +1769,18 @@
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 3)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 4)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1619,30 +1804,36 @@
 
 class SpecIntervalUpdateSerial(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecIntervalSerial
 
     Attributes:
      - ts: The timestamp for the updated cell NULL: MIN_INT64-1, AUTO:MIN_INT64-1
-     - v: The value for the updated cell
+     - v: The values of serial-fields for the updated cell
+     - v_op: The values of serial-fields for the the SERIAL operation update
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'ts',
         'v',
+        'v_op',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, ts=None, v=None, encoder=None,):
+    def __init__(self, ts=None, v=None, v_op=None, encoder=None, update_op=None,):
         self.ts = ts
         self.v = v
+        self.v_op = v_op
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1662,18 +1853,35 @@
                         _elem54 = CellValueSerial()
                         _elem54.read(iprot)
                         self.v.append(_elem54)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
+                if ftype == TType.LIST:
+                    self.v_op = []
+                    (_etype58, _size55) = iprot.readListBegin()
+                    for _i59 in range(_size55):
+                        _elem60 = CellValueSerialOp()
+                        _elem60.read(iprot)
+                        self.v_op.append(_elem60)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1683,22 +1891,33 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 1)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter55 in self.v:
-                iter55.write(oprot)
+            for iter61 in self.v:
+                iter61.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_op is not None:
+            oprot.writeFieldBegin('v_op', TType.LIST, 3)
+            oprot.writeListBegin(TType.STRUCT, len(self.v_op))
+            for iter62 in self.v_op:
+                iter62.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
-            oprot.writeFieldBegin('encoder', TType.I32, 3)
+            oprot.writeFieldBegin('encoder', TType.I32, 4)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 5)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1775,65 +1994,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype59, _size56) = iprot.readListBegin()
-                    for _i60 in range(_size56):
-                        _elem61 = iprot.readBinary()
-                        self.range_begin.append(_elem61)
+                    (_etype66, _size63) = iprot.readListBegin()
+                    for _i67 in range(_size63):
+                        _elem68 = iprot.readBinary()
+                        self.range_begin.append(_elem68)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype65, _size62) = iprot.readListBegin()
-                    for _i66 in range(_size62):
-                        _elem67 = iprot.readBinary()
-                        self.range_end.append(_elem67)
+                    (_etype72, _size69) = iprot.readListBegin()
+                    for _i73 in range(_size69):
+                        _elem74 = iprot.readBinary()
+                        self.range_end.append(_elem74)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype71, _size68) = iprot.readListBegin()
-                    for _i72 in range(_size68):
-                        _elem73 = iprot.readBinary()
-                        self.offset_key.append(_elem73)
+                    (_etype78, _size75) = iprot.readListBegin()
+                    for _i79 in range(_size75):
+                        _elem80 = iprot.readBinary()
+                        self.offset_key.append(_elem80)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype77, _size74) = iprot.readListBegin()
-                    for _i78 in range(_size74):
-                        _elem79 = SpecKeyInterval()
-                        _elem79.read(iprot)
-                        self.key_intervals.append(_elem79)
+                    (_etype84, _size81) = iprot.readListBegin()
+                    for _i85 in range(_size81):
+                        _elem86 = SpecKeyInterval()
+                        _elem86.read(iprot)
+                        self.key_intervals.append(_elem86)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype83, _size80) = iprot.readListBegin()
-                    for _i84 in range(_size80):
-                        _elem85 = SpecValue()
-                        _elem85.read(iprot)
-                        self.values.append(_elem85)
+                    (_etype90, _size87) = iprot.readListBegin()
+                    for _i91 in range(_size87):
+                        _elem92 = SpecValue()
+                        _elem92.read(iprot)
+                        self.values.append(_elem92)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -1871,48 +2090,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecInterval')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter86 in self.range_begin:
-                oprot.writeBinary(iter86)
+            for iter93 in self.range_begin:
+                oprot.writeBinary(iter93)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter87 in self.range_end:
-                oprot.writeBinary(iter87)
+            for iter94 in self.range_end:
+                oprot.writeBinary(iter94)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter88 in self.offset_key:
-                oprot.writeBinary(iter88)
+            for iter95 in self.offset_key:
+                oprot.writeBinary(iter95)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter89 in self.key_intervals:
-                iter89.write(oprot)
+            for iter96 in self.key_intervals:
+                iter96.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter90 in self.values:
-                iter90.write(oprot)
+            for iter97 in self.values:
+                iter97.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -1989,19 +2208,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype94, _size91) = iprot.readListBegin()
-                    for _i95 in range(_size91):
-                        _elem96 = SpecInterval()
-                        _elem96.read(iprot)
-                        self.intervals.append(_elem96)
+                    (_etype101, _size98) = iprot.readListBegin()
+                    for _i102 in range(_size98):
+                        _elem103 = SpecInterval()
+                        _elem103.read(iprot)
+                        self.intervals.append(_elem103)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2014,16 +2233,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter97 in self.intervals:
-                iter97.write(oprot)
+            for iter104 in self.intervals:
+                iter104.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2326,19 +2545,19 @@
                 if ftype == TType.I32:
                     self.seq = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype101, _size98) = iprot.readListBegin()
-                    for _i102 in range(_size98):
-                        _elem103 = SpecFraction()
-                        _elem103.read(iprot)
-                        self.v.append(_elem103)
+                    (_etype108, _size105) = iprot.readListBegin()
+                    for _i109 in range(_size105):
+                        _elem110 = SpecFraction()
+                        _elem110.read(iprot)
+                        self.v.append(_elem110)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2351,16 +2570,16 @@
         if self.seq is not None:
             oprot.writeFieldBegin('seq', TType.I32, 1)
             oprot.writeI32(self.seq)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter104 in self.v:
-                iter104.write(oprot)
+            for iter111 in self.v:
+                iter111.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2417,19 +2636,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype108, _size105) = iprot.readListBegin()
-                    for _i109 in range(_size105):
-                        _elem110 = SpecValueSerial_INT64()
-                        _elem110.read(iprot)
-                        self.v.append(_elem110)
+                    (_etype115, _size112) = iprot.readListBegin()
+                    for _i116 in range(_size112):
+                        _elem117 = SpecValueSerial_INT64()
+                        _elem117.read(iprot)
+                        self.v.append(_elem117)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2442,16 +2661,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter111 in self.v:
-                iter111.write(oprot)
+            for iter118 in self.v:
+                iter118.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2508,19 +2727,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype115, _size112) = iprot.readListBegin()
-                    for _i116 in range(_size112):
-                        _elem117 = SpecValueSerial_BYTES()
-                        _elem117.read(iprot)
-                        self.v.append(_elem117)
+                    (_etype122, _size119) = iprot.readListBegin()
+                    for _i123 in range(_size119):
+                        _elem124 = SpecValueSerial_BYTES()
+                        _elem124.read(iprot)
+                        self.v.append(_elem124)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2533,16 +2752,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter118 in self.v:
-                iter118.write(oprot)
+            for iter125 in self.v:
+                iter125.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2745,19 +2964,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.fields = []
-                    (_etype122, _size119) = iprot.readListBegin()
-                    for _i123 in range(_size119):
-                        _elem124 = SpecValueSerialField()
-                        _elem124.read(iprot)
-                        self.fields.append(_elem124)
+                    (_etype129, _size126) = iprot.readListBegin()
+                    for _i130 in range(_size126):
+                        _elem131 = SpecValueSerialField()
+                        _elem131.read(iprot)
+                        self.fields.append(_elem131)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2770,16 +2989,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.fields is not None:
             oprot.writeFieldBegin('fields', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.fields))
-            for iter125 in self.fields:
-                iter125.write(oprot)
+            for iter132 in self.fields:
+                iter132.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2858,65 +3077,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype129, _size126) = iprot.readListBegin()
-                    for _i130 in range(_size126):
-                        _elem131 = iprot.readBinary()
-                        self.range_begin.append(_elem131)
+                    (_etype136, _size133) = iprot.readListBegin()
+                    for _i137 in range(_size133):
+                        _elem138 = iprot.readBinary()
+                        self.range_begin.append(_elem138)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype135, _size132) = iprot.readListBegin()
-                    for _i136 in range(_size132):
-                        _elem137 = iprot.readBinary()
-                        self.range_end.append(_elem137)
+                    (_etype142, _size139) = iprot.readListBegin()
+                    for _i143 in range(_size139):
+                        _elem144 = iprot.readBinary()
+                        self.range_end.append(_elem144)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype141, _size138) = iprot.readListBegin()
-                    for _i142 in range(_size138):
-                        _elem143 = iprot.readBinary()
-                        self.offset_key.append(_elem143)
+                    (_etype148, _size145) = iprot.readListBegin()
+                    for _i149 in range(_size145):
+                        _elem150 = iprot.readBinary()
+                        self.offset_key.append(_elem150)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype147, _size144) = iprot.readListBegin()
-                    for _i148 in range(_size144):
-                        _elem149 = SpecKeyInterval()
-                        _elem149.read(iprot)
-                        self.key_intervals.append(_elem149)
+                    (_etype154, _size151) = iprot.readListBegin()
+                    for _i155 in range(_size151):
+                        _elem156 = SpecKeyInterval()
+                        _elem156.read(iprot)
+                        self.key_intervals.append(_elem156)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype153, _size150) = iprot.readListBegin()
-                    for _i154 in range(_size150):
-                        _elem155 = SpecValueSerial()
-                        _elem155.read(iprot)
-                        self.values.append(_elem155)
+                    (_etype160, _size157) = iprot.readListBegin()
+                    for _i161 in range(_size157):
+                        _elem162 = SpecValueSerial()
+                        _elem162.read(iprot)
+                        self.values.append(_elem162)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -2954,48 +3173,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecIntervalSerial')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter156 in self.range_begin:
-                oprot.writeBinary(iter156)
+            for iter163 in self.range_begin:
+                oprot.writeBinary(iter163)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter157 in self.range_end:
-                oprot.writeBinary(iter157)
+            for iter164 in self.range_end:
+                oprot.writeBinary(iter164)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter158 in self.offset_key:
-                oprot.writeBinary(iter158)
+            for iter165 in self.offset_key:
+                oprot.writeBinary(iter165)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter159 in self.key_intervals:
-                iter159.write(oprot)
+            for iter166 in self.key_intervals:
+                iter166.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter160 in self.values:
-                iter160.write(oprot)
+            for iter167 in self.values:
+                iter167.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -3072,19 +3291,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype164, _size161) = iprot.readListBegin()
-                    for _i165 in range(_size161):
-                        _elem166 = SpecIntervalSerial()
-                        _elem166.read(iprot)
-                        self.intervals.append(_elem166)
+                    (_etype171, _size168) = iprot.readListBegin()
+                    for _i172 in range(_size168):
+                        _elem173 = SpecIntervalSerial()
+                        _elem173.read(iprot)
+                        self.intervals.append(_elem173)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3097,16 +3316,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter167 in self.intervals:
-                iter167.write(oprot)
+            for iter174 in self.intervals:
+                iter174.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3161,30 +3380,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.columns = []
-                    (_etype171, _size168) = iprot.readListBegin()
-                    for _i172 in range(_size168):
-                        _elem173 = SpecColumn()
-                        _elem173.read(iprot)
-                        self.columns.append(_elem173)
+                    (_etype178, _size175) = iprot.readListBegin()
+                    for _i179 in range(_size175):
+                        _elem180 = SpecColumn()
+                        _elem180.read(iprot)
+                        self.columns.append(_elem180)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.columns_serial = []
-                    (_etype177, _size174) = iprot.readListBegin()
-                    for _i178 in range(_size174):
-                        _elem179 = SpecColumnSerial()
-                        _elem179.read(iprot)
-                        self.columns_serial.append(_elem179)
+                    (_etype184, _size181) = iprot.readListBegin()
+                    for _i185 in range(_size181):
+                        _elem186 = SpecColumnSerial()
+                        _elem186.read(iprot)
+                        self.columns_serial.append(_elem186)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRUCT:
                     self.flags = SpecFlags()
                     self.flags.read(iprot)
@@ -3199,23 +3418,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecScan')
         if self.columns is not None:
             oprot.writeFieldBegin('columns', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.columns))
-            for iter180 in self.columns:
-                iter180.write(oprot)
+            for iter187 in self.columns:
+                iter187.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columns_serial is not None:
             oprot.writeFieldBegin('columns_serial', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.columns_serial))
-            for iter181 in self.columns_serial:
-                iter181.write(oprot)
+            for iter188 in self.columns_serial:
+                iter188.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.flags is not None:
             oprot.writeFieldBegin('flags', TType.STRUCT, 3)
             self.flags.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3288,18 +3507,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype185, _size182) = iprot.readListBegin()
-                    for _i186 in range(_size182):
-                        _elem187 = iprot.readBinary()
-                        self.k.append(_elem187)
+                    (_etype192, _size189) = iprot.readListBegin()
+                    for _i193 in range(_size189):
+                        _elem194 = iprot.readBinary()
+                        self.k.append(_elem194)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3332,16 +3551,16 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter188 in self.k:
-                oprot.writeBinary(iter188)
+            for iter195 in self.k:
+                oprot.writeBinary(iter195)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
@@ -3444,38 +3663,38 @@
                 if ftype == TType.STRING:
                     self.v_bytes = iprot.readBinary()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v_key = []
-                    (_etype192, _size189) = iprot.readListBegin()
-                    for _i193 in range(_size189):
-                        _elem194 = iprot.readBinary()
-                        self.v_key.append(_elem194)
+                    (_etype199, _size196) = iprot.readListBegin()
+                    for _i200 in range(_size196):
+                        _elem201 = iprot.readBinary()
+                        self.v_key.append(_elem201)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.v_li = []
-                    (_etype198, _size195) = iprot.readListBegin()
-                    for _i199 in range(_size195):
-                        _elem200 = iprot.readI64()
-                        self.v_li.append(_elem200)
+                    (_etype205, _size202) = iprot.readListBegin()
+                    for _i206 in range(_size202):
+                        _elem207 = iprot.readI64()
+                        self.v_li.append(_elem207)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.v_lb = []
-                    (_etype204, _size201) = iprot.readListBegin()
-                    for _i205 in range(_size201):
-                        _elem206 = iprot.readBinary()
-                        self.v_lb.append(_elem206)
+                    (_etype211, _size208) = iprot.readListBegin()
+                    for _i212 in range(_size208):
+                        _elem213 = iprot.readBinary()
+                        self.v_lb.append(_elem213)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3500,30 +3719,499 @@
         if self.v_bytes is not None:
             oprot.writeFieldBegin('v_bytes', TType.STRING, 4)
             oprot.writeBinary(self.v_bytes)
             oprot.writeFieldEnd()
         if self.v_key is not None:
             oprot.writeFieldBegin('v_key', TType.LIST, 5)
             oprot.writeListBegin(TType.STRING, len(self.v_key))
-            for iter207 in self.v_key:
-                oprot.writeBinary(iter207)
+            for iter214 in self.v_key:
+                oprot.writeBinary(iter214)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_li is not None:
             oprot.writeFieldBegin('v_li', TType.LIST, 6)
             oprot.writeListBegin(TType.I64, len(self.v_li))
-            for iter208 in self.v_li:
-                oprot.writeI64(iter208)
+            for iter215 in self.v_li:
+                oprot.writeI64(iter215)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_lb is not None:
             oprot.writeFieldBegin('v_lb', TType.LIST, 7)
             oprot.writeListBegin(TType.STRING, len(self.v_lb))
-            for iter209 in self.v_lb:
-                oprot.writeBinary(iter209)
+            for iter216 in self.v_lb:
+                oprot.writeBinary(iter216)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_INT64(object):
+    """
+    Serial INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.I64:
+                    self.v = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_INT64')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.I64, 5)
+            oprot.writeI64(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_DOUBLE(object):
+    """
+    Serial DOUBLE Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.DOUBLE:
+                    self.v = iprot.readDouble()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_DOUBLE')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.DOUBLE, 5)
+            oprot.writeDouble(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_BYTES(object):
+    """
+    Serial BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRING:
+                    self.v = iprot.readBinary()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_BYTES')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.STRING, 5)
+            oprot.writeBinary(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_LI(object):
+    """
+    Serial LIST_INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype220, _size217) = iprot.readListBegin()
+                    for _i221 in range(_size217):
+                        _elem222 = FU_INT64()
+                        _elem222.read(iprot)
+                        self.v.append(_elem222)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LI')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter223 in self.v:
+                iter223.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3543,14 +4231,284 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class FU_LB(object):
+    """
+    Serial LIST_BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype227, _size224) = iprot.readListBegin()
+                    for _i228 in range(_size224):
+                        _elem229 = FU_BYTES()
+                        _elem229.read(iprot)
+                        self.v.append(_elem229)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LB')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter230 in self.v:
+                iter230.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class CellValueSerialOp(object):
+    """
+    The Serial Values Cell field with Update Operation
+
+    Attributes:
+     - field_id: The Field ID, a single ID can have any/all the field types
+     - v_int64: The INT64 type update-field
+     - v_double: The DOUBLE type update-field
+     - v_bytes: The BYTES type update-field
+     - v_key: The Cell KEY type update-field
+     - v_li: The LIST INT64 type update-field
+     - v_lb: The LIST BYTES type update-field
+
+    """
+
+    __slots__ = (
+        'field_id',
+        'v_int64',
+        'v_double',
+        'v_bytes',
+        'v_key',
+        'v_li',
+        'v_lb',
+    )
+
+
+    def __init__(self, field_id=None, v_int64=None, v_double=None, v_bytes=None, v_key=None, v_li=None, v_lb=None,):
+        self.field_id = field_id
+        self.v_int64 = v_int64
+        self.v_double = v_double
+        self.v_bytes = v_bytes
+        self.v_key = v_key
+        self.v_li = v_li
+        self.v_lb = v_lb
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.field_id = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.v_int64 = FU_INT64()
+                    self.v_int64.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRUCT:
+                    self.v_double = FU_DOUBLE()
+                    self.v_double.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.v_bytes = FU_BYTES()
+                    self.v_bytes.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.LIST:
+                    self.v_key = []
+                    (_etype234, _size231) = iprot.readListBegin()
+                    for _i235 in range(_size231):
+                        _elem236 = iprot.readBinary()
+                        self.v_key.append(_elem236)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.STRUCT:
+                    self.v_li = FU_LI()
+                    self.v_li.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 7:
+                if ftype == TType.STRUCT:
+                    self.v_lb = FU_LB()
+                    self.v_lb.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('CellValueSerialOp')
+        if self.field_id is not None:
+            oprot.writeFieldBegin('field_id', TType.I32, 1)
+            oprot.writeI32(self.field_id)
+            oprot.writeFieldEnd()
+        if self.v_int64 is not None:
+            oprot.writeFieldBegin('v_int64', TType.STRUCT, 2)
+            self.v_int64.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_double is not None:
+            oprot.writeFieldBegin('v_double', TType.STRUCT, 3)
+            self.v_double.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_bytes is not None:
+            oprot.writeFieldBegin('v_bytes', TType.STRUCT, 4)
+            self.v_bytes.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_key is not None:
+            oprot.writeFieldBegin('v_key', TType.LIST, 5)
+            oprot.writeListBegin(TType.STRING, len(self.v_key))
+            for iter237 in self.v_key:
+                oprot.writeBinary(iter237)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_li is not None:
+            oprot.writeFieldBegin('v_li', TType.STRUCT, 6)
+            self.v_li.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_lb is not None:
+            oprot.writeFieldBegin('v_lb', TType.STRUCT, 7)
+            self.v_lb.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class UCellSerial(object):
     """
     The Cell data for using with Update of SERIAL Column Type
 
     Attributes:
      - f: The Cell Flag
      - k: The Cell Key
@@ -3592,18 +4550,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype213, _size210) = iprot.readListBegin()
-                    for _i214 in range(_size210):
-                        _elem215 = iprot.readBinary()
-                        self.k.append(_elem215)
+                    (_etype241, _size238) = iprot.readListBegin()
+                    for _i242 in range(_size238):
+                        _elem243 = iprot.readBinary()
+                        self.k.append(_elem243)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3612,19 +4570,19 @@
                 if ftype == TType.BOOL:
                     self.ts_desc = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype219, _size216) = iprot.readListBegin()
-                    for _i220 in range(_size216):
-                        _elem221 = CellValueSerial()
-                        _elem221.read(iprot)
-                        self.v.append(_elem221)
+                    (_etype247, _size244) = iprot.readListBegin()
+                    for _i248 in range(_size244):
+                        _elem249 = CellValueSerial()
+                        _elem249.read(iprot)
+                        self.v.append(_elem249)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
@@ -3642,31 +4600,31 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter222 in self.k:
-                oprot.writeBinary(iter222)
+            for iter250 in self.k:
+                oprot.writeBinary(iter250)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
             oprot.writeFieldBegin('ts_desc', TType.BOOL, 4)
             oprot.writeBool(self.ts_desc)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter223 in self.v:
-                iter223.write(oprot)
+            for iter251 in self.v:
+                iter251.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 6)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3733,18 +4691,18 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype227, _size224) = iprot.readListBegin()
-                    for _i228 in range(_size224):
-                        _elem229 = iprot.readBinary()
-                        self.k.append(_elem229)
+                    (_etype255, _size252) = iprot.readListBegin()
+                    for _i256 in range(_size252):
+                        _elem257 = iprot.readBinary()
+                        self.k.append(_elem257)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3767,16 +4725,16 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter230 in self.k:
-                oprot.writeBinary(iter230)
+            for iter258 in self.k:
+                oprot.writeBinary(iter258)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -3847,34 +4805,34 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype234, _size231) = iprot.readListBegin()
-                    for _i235 in range(_size231):
-                        _elem236 = iprot.readBinary()
-                        self.k.append(_elem236)
+                    (_etype262, _size259) = iprot.readListBegin()
+                    for _i263 in range(_size259):
+                        _elem264 = iprot.readBinary()
+                        self.k.append(_elem264)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype240, _size237) = iprot.readListBegin()
-                    for _i241 in range(_size237):
-                        _elem242 = CellValueSerial()
-                        _elem242.read(iprot)
-                        self.v.append(_elem242)
+                    (_etype268, _size265) = iprot.readListBegin()
+                    for _i269 in range(_size265):
+                        _elem270 = CellValueSerial()
+                        _elem270.read(iprot)
+                        self.v.append(_elem270)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3887,27 +4845,27 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter243 in self.k:
-                oprot.writeBinary(iter243)
+            for iter271 in self.k:
+                oprot.writeBinary(iter271)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter244 in self.v:
-                iter244.write(oprot)
+            for iter272 in self.v:
+                iter272.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3959,30 +4917,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype248, _size245) = iprot.readListBegin()
-                    for _i249 in range(_size245):
-                        _elem250 = Cell()
-                        _elem250.read(iprot)
-                        self.cells.append(_elem250)
+                    (_etype276, _size273) = iprot.readListBegin()
+                    for _i277 in range(_size273):
+                        _elem278 = Cell()
+                        _elem278.read(iprot)
+                        self.cells.append(_elem278)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype254, _size251) = iprot.readListBegin()
-                    for _i255 in range(_size251):
-                        _elem256 = CellSerial()
-                        _elem256.read(iprot)
-                        self.serial_cells.append(_elem256)
+                    (_etype282, _size279) = iprot.readListBegin()
+                    for _i283 in range(_size279):
+                        _elem284 = CellSerial()
+                        _elem284.read(iprot)
+                        self.serial_cells.append(_elem284)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3991,23 +4949,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Cells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter257 in self.cells:
-                iter257.write(oprot)
+            for iter285 in self.cells:
+                iter285.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter258 in self.serial_cells:
-                iter258.write(oprot)
+            for iter286 in self.serial_cells:
+                iter286.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4062,18 +5020,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype262, _size259) = iprot.readListBegin()
-                    for _i263 in range(_size259):
-                        _elem264 = iprot.readBinary()
-                        self.k.append(_elem264)
+                    (_etype290, _size287) = iprot.readListBegin()
+                    for _i291 in range(_size287):
+                        _elem292 = iprot.readBinary()
+                        self.k.append(_elem292)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -4092,16 +5050,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCell')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter265 in self.k:
-                oprot.writeBinary(iter265)
+            for iter293 in self.k:
+                oprot.writeBinary(iter293)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -4164,34 +5122,34 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype269, _size266) = iprot.readListBegin()
-                    for _i270 in range(_size266):
-                        _elem271 = iprot.readBinary()
-                        self.k.append(_elem271)
+                    (_etype297, _size294) = iprot.readListBegin()
+                    for _i298 in range(_size294):
+                        _elem299 = iprot.readBinary()
+                        self.k.append(_elem299)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype275, _size272) = iprot.readListBegin()
-                    for _i276 in range(_size272):
-                        _elem277 = CellValueSerial()
-                        _elem277.read(iprot)
-                        self.v.append(_elem277)
+                    (_etype303, _size300) = iprot.readListBegin()
+                    for _i304 in range(_size300):
+                        _elem305 = CellValueSerial()
+                        _elem305.read(iprot)
+                        self.v.append(_elem305)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4200,27 +5158,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCellSerial')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter278 in self.k:
-                oprot.writeBinary(iter278)
+            for iter306 in self.k:
+                oprot.writeBinary(iter306)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter279 in self.v:
-                iter279.write(oprot)
+            for iter307 in self.v:
+                iter307.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4272,30 +5230,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype283, _size280) = iprot.readListBegin()
-                    for _i284 in range(_size280):
-                        _elem285 = CCell()
-                        _elem285.read(iprot)
-                        self.cells.append(_elem285)
+                    (_etype311, _size308) = iprot.readListBegin()
+                    for _i312 in range(_size308):
+                        _elem313 = CCell()
+                        _elem313.read(iprot)
+                        self.cells.append(_elem313)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype289, _size286) = iprot.readListBegin()
-                    for _i290 in range(_size286):
-                        _elem291 = CCellSerial()
-                        _elem291.read(iprot)
-                        self.serial_cells.append(_elem291)
+                    (_etype317, _size314) = iprot.readListBegin()
+                    for _i318 in range(_size314):
+                        _elem319 = CCellSerial()
+                        _elem319.read(iprot)
+                        self.serial_cells.append(_elem319)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4304,23 +5262,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ColCells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter292 in self.cells:
-                iter292.write(oprot)
+            for iter320 in self.cells:
+                iter320.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter293 in self.serial_cells:
-                iter293.write(oprot)
+            for iter321 in self.serial_cells:
+                iter321.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4479,19 +5437,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype297, _size294) = iprot.readListBegin()
-                    for _i298 in range(_size294):
-                        _elem299 = CellValueSerial()
-                        _elem299.read(iprot)
-                        self.v.append(_elem299)
+                    (_etype325, _size322) = iprot.readListBegin()
+                    for _i326 in range(_size322):
+                        _elem327 = CellValueSerial()
+                        _elem327.read(iprot)
+                        self.v.append(_elem327)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4508,16 +5466,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter300 in self.v:
-                iter300.write(oprot)
+            for iter328 in self.v:
+                iter328.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4572,40 +5530,40 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype304, _size301) = iprot.readListBegin()
-                    for _i305 in range(_size301):
-                        _elem306 = iprot.readBinary()
-                        self.k.append(_elem306)
+                    (_etype332, _size329) = iprot.readListBegin()
+                    for _i333 in range(_size329):
+                        _elem334 = iprot.readBinary()
+                        self.k.append(_elem334)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype310, _size307) = iprot.readListBegin()
-                    for _i311 in range(_size307):
-                        _elem312 = KCell()
-                        _elem312.read(iprot)
-                        self.cells.append(_elem312)
+                    (_etype338, _size335) = iprot.readListBegin()
+                    for _i339 in range(_size335):
+                        _elem340 = KCell()
+                        _elem340.read(iprot)
+                        self.cells.append(_elem340)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype316, _size313) = iprot.readListBegin()
-                    for _i317 in range(_size313):
-                        _elem318 = KCellSerial()
-                        _elem318.read(iprot)
-                        self.serial_cells.append(_elem318)
+                    (_etype344, _size341) = iprot.readListBegin()
+                    for _i345 in range(_size341):
+                        _elem346 = KCellSerial()
+                        _elem346.read(iprot)
+                        self.serial_cells.append(_elem346)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4614,30 +5572,30 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('kCells')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter319 in self.k:
-                oprot.writeBinary(iter319)
+            for iter347 in self.k:
+                oprot.writeBinary(iter347)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter320 in self.cells:
-                iter320.write(oprot)
+            for iter348 in self.cells:
+                iter348.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter321 in self.serial_cells:
-                iter321.write(oprot)
+            for iter349 in self.serial_cells:
+                iter349.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4796,19 +5754,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype325, _size322) = iprot.readListBegin()
-                    for _i326 in range(_size322):
-                        _elem327 = CellValueSerial()
-                        _elem327.read(iprot)
-                        self.v.append(_elem327)
+                    (_etype353, _size350) = iprot.readListBegin()
+                    for _i354 in range(_size350):
+                        _elem355 = CellValueSerial()
+                        _elem355.read(iprot)
+                        self.v.append(_elem355)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4825,16 +5783,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter328 in self.v:
-                iter328.write(oprot)
+            for iter356 in self.v:
+                iter356.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4889,42 +5847,42 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.f = {}
-                    (_ktype330, _vtype331, _size329) = iprot.readMapBegin()
-                    for _i333 in range(_size329):
-                        _key334 = iprot.readBinary()
-                        _val335 = FCells()
-                        _val335.read(iprot)
-                        self.f[_key334] = _val335
+                    (_ktype358, _vtype359, _size357) = iprot.readMapBegin()
+                    for _i361 in range(_size357):
+                        _key362 = iprot.readBinary()
+                        _val363 = FCells()
+                        _val363.read(iprot)
+                        self.f[_key362] = _val363
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype339, _size336) = iprot.readListBegin()
-                    for _i340 in range(_size336):
-                        _elem341 = FCell()
-                        _elem341.read(iprot)
-                        self.cells.append(_elem341)
+                    (_etype367, _size364) = iprot.readListBegin()
+                    for _i368 in range(_size364):
+                        _elem369 = FCell()
+                        _elem369.read(iprot)
+                        self.cells.append(_elem369)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype345, _size342) = iprot.readListBegin()
-                    for _i346 in range(_size342):
-                        _elem347 = FCellSerial()
-                        _elem347.read(iprot)
-                        self.serial_cells.append(_elem347)
+                    (_etype373, _size370) = iprot.readListBegin()
+                    for _i374 in range(_size370):
+                        _elem375 = FCellSerial()
+                        _elem375.read(iprot)
+                        self.serial_cells.append(_elem375)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4933,31 +5891,31 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('FCells')
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.MAP, 1)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.f))
-            for kiter348, viter349 in self.f.items():
-                oprot.writeBinary(kiter348)
-                viter349.write(oprot)
+            for kiter376, viter377 in self.f.items():
+                oprot.writeBinary(kiter376)
+                viter377.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter350 in self.cells:
-                iter350.write(oprot)
+            for iter378 in self.cells:
+                iter378.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter351 in self.serial_cells:
-                iter351.write(oprot)
+            for iter379 in self.serial_cells:
+                iter379.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5021,31 +5979,31 @@
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.ccells = {}
-                    (_ktype353, _vtype354, _size352) = iprot.readMapBegin()
-                    for _i356 in range(_size352):
-                        _key357 = iprot.readString()
-                        _val358 = ColCells()
-                        _val358.read(iprot)
-                        self.ccells[_key357] = _val358
+                    (_ktype381, _vtype382, _size380) = iprot.readMapBegin()
+                    for _i384 in range(_size380):
+                        _key385 = iprot.readString()
+                        _val386 = ColCells()
+                        _val386.read(iprot)
+                        self.ccells[_key385] = _val386
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.kcells = []
-                    (_etype362, _size359) = iprot.readListBegin()
-                    for _i363 in range(_size359):
-                        _elem364 = kCells()
-                        _elem364.read(iprot)
-                        self.kcells.append(_elem364)
+                    (_etype390, _size387) = iprot.readListBegin()
+                    for _i391 in range(_size387):
+                        _elem392 = kCells()
+                        _elem392.read(iprot)
+                        self.kcells.append(_elem392)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.fcells = FCells()
                     self.fcells.read(iprot)
@@ -5064,24 +6022,24 @@
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 1)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.ccells is not None:
             oprot.writeFieldBegin('ccells', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.ccells))
-            for kiter365, viter366 in self.ccells.items():
-                oprot.writeString(kiter365)
-                viter366.write(oprot)
+            for kiter393, viter394 in self.ccells.items():
+                oprot.writeString(kiter393)
+                viter394.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.kcells is not None:
             oprot.writeFieldBegin('kcells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.kcells))
-            for iter367 in self.kcells:
-                iter367.write(oprot)
+            for iter395 in self.kcells:
+                iter395.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.fcells is not None:
             oprot.writeFieldBegin('fcells', TType.STRUCT, 4)
             self.fcells.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5222,36 +6180,36 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemas = []
-                    (_etype371, _size368) = iprot.readListBegin()
-                    for _i372 in range(_size368):
-                        _elem373 = Schema()
-                        _elem373.read(iprot)
-                        self.schemas.append(_elem373)
+                    (_etype399, _size396) = iprot.readListBegin()
+                    for _i400 in range(_size396):
+                        _elem401 = Schema()
+                        _elem401.read(iprot)
+                        self.schemas.append(_elem401)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRUCT:
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.compact = []
-                    (_etype377, _size374) = iprot.readListBegin()
-                    for _i378 in range(_size374):
-                        _elem379 = CompactResult()
-                        _elem379.read(iprot)
-                        self.compact.append(_elem379)
+                    (_etype405, _size402) = iprot.readListBegin()
+                    for _i406 in range(_size402):
+                        _elem407 = CompactResult()
+                        _elem407.read(iprot)
+                        self.compact.append(_elem407)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5260,27 +6218,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Result')
         if self.schemas is not None:
             oprot.writeFieldBegin('schemas', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemas))
-            for iter380 in self.schemas:
-                iter380.write(oprot)
+            for iter408 in self.schemas:
+                iter408.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 2)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.compact is not None:
             oprot.writeFieldBegin('compact', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.compact))
-            for iter381 in self.compact:
-                iter381.write(oprot)
+            for iter409 in self.compact:
+                iter409.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5384,27 +6342,36 @@
 )
 all_structs.append(SpecValue)
 SpecValue.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'comp', None, None, ),  # 1
     (2, TType.STRING, 'v', 'BINARY', None, ),  # 2
 )
+all_structs.append(SpecUpdateOP)
+SpecUpdateOP.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'op', None, None, ),  # 1
+    (2, TType.I32, 'pos', None, None, ),  # 2
+)
 all_structs.append(SpecIntervalUpdate)
 SpecIntervalUpdate.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'v', 'BINARY', None, ),  # 1
     (2, TType.I64, 'ts', None, None, ),  # 2
     (3, TType.I32, 'encoder', None, None, ),  # 3
+    (4, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 4
 )
 all_structs.append(SpecIntervalUpdateSerial)
 SpecIntervalUpdateSerial.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'ts', None, None, ),  # 1
     (2, TType.LIST, 'v', (TType.STRUCT, [CellValueSerial, None], False), None, ),  # 2
-    (3, TType.I32, 'encoder', None, None, ),  # 3
+    (3, TType.LIST, 'v_op', (TType.STRUCT, [CellValueSerialOp, None], False), None, ),  # 3
+    (4, TType.I32, 'encoder', None, None, ),  # 4
+    (5, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 5
 )
 all_structs.append(SpecInterval)
 SpecInterval.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'range_begin', (TType.STRING, 'BINARY', False), None, ),  # 1
     (2, TType.LIST, 'range_end', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.LIST, 'offset_key', (TType.STRING, 'BINARY', False), None, ),  # 3
@@ -5521,14 +6488,68 @@
     (2, TType.I64, 'v_int64', None, None, ),  # 2
     (3, TType.DOUBLE, 'v_double', None, None, ),  # 3
     (4, TType.STRING, 'v_bytes', 'BINARY', None, ),  # 4
     (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
     (6, TType.LIST, 'v_li', (TType.I64, None, False), None, ),  # 6
     (7, TType.LIST, 'v_lb', (TType.STRING, 'BINARY', False), None, ),  # 7
 )
+all_structs.append(FU_INT64)
+FU_INT64.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.I64, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_DOUBLE)
+FU_DOUBLE.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.DOUBLE, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_BYTES)
+FU_BYTES.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.STRING, 'v', 'BINARY', None, ),  # 5
+)
+all_structs.append(FU_LI)
+FU_LI.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_INT64, None], False), None, ),  # 4
+)
+all_structs.append(FU_LB)
+FU_LB.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_BYTES, None], False), None, ),  # 4
+)
+all_structs.append(CellValueSerialOp)
+CellValueSerialOp.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'field_id', None, None, ),  # 1
+    (2, TType.STRUCT, 'v_int64', [FU_INT64, None], None, ),  # 2
+    (3, TType.STRUCT, 'v_double', [FU_DOUBLE, None], None, ),  # 3
+    (4, TType.STRUCT, 'v_bytes', [FU_BYTES, None], None, ),  # 4
+    (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
+    (6, TType.STRUCT, 'v_li', [FU_LI, None], None, ),  # 6
+    (7, TType.STRUCT, 'v_lb', [FU_LB, None], None, ),  # 7
+)
 all_structs.append(UCellSerial)
 UCellSerial.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'f', None, None, ),  # 1
     (2, TType.LIST, 'k', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.I64, 'ts', None, None, ),  # 3
     (4, TType.BOOL, 'ts_desc', None, None, ),  # 4
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/pool.py` & `swcdb-0.5.9.0/swcdb/thrift/pool.py`

 * *Files identical despite different names*

### Comparing `swcdb-0.5.8.1/swcdb/thrift/service.py` & `swcdb-0.5.9.0/swcdb/thrift/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from thrift.transport import TTransport, TSocket
 TSSLSocket = None
 from thrift.protocol.TBinaryProtocol import TBinaryProtocol
 
 from swcdb.thrift.native import Service
 from swcdb.thrift.native.ttypes import *
+from swcdb.thrift.native.constants import *
 
 
 # Not Implemented thrift.transport.TSSLSocket
 # def init_ssl(handler=None, formatter=None):
 #    import logging
 #    from thrift.transport import TSSLSocket as _ssl_socket
 #    if not handler:
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/tornado/Service.py` & `swcdb-0.5.9.0/swcdb/thrift/tornado/Service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1976,19 +1976,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype385, _size382) = iprot.readListBegin()
-                    for _i386 in range(_size382):
-                        _elem387 = Schema()
-                        _elem387.read(iprot)
-                        self.success.append(_elem387)
+                    (_etype413, _size410) = iprot.readListBegin()
+                    for _i414 in range(_size410):
+                        _elem415 = Schema()
+                        _elem415.read(iprot)
+                        self.success.append(_elem415)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2002,16 +2002,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter388 in self.success:
-                iter388.write(oprot)
+            for iter416 in self.success:
+                iter416.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2143,19 +2143,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype392, _size389) = iprot.readListBegin()
-                    for _i393 in range(_size389):
-                        _elem394 = CompactResult()
-                        _elem394.read(iprot)
-                        self.success.append(_elem394)
+                    (_etype420, _size417) = iprot.readListBegin()
+                    for _i421 in range(_size417):
+                        _elem422 = CompactResult()
+                        _elem422.read(iprot)
+                        self.success.append(_elem422)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2169,16 +2169,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter395 in self.success:
-                iter395.write(oprot)
+            for iter423 in self.success:
+                iter423.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2469,20 +2469,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype397, _vtype398, _size396) = iprot.readMapBegin()
-                    for _i400 in range(_size396):
-                        _key401 = iprot.readString()
-                        _val402 = ColCells()
-                        _val402.read(iprot)
-                        self.success[_key401] = _val402
+                    (_ktype425, _vtype426, _size424) = iprot.readMapBegin()
+                    for _i428 in range(_size424):
+                        _key429 = iprot.readString()
+                        _val430 = ColCells()
+                        _val430.read(iprot)
+                        self.success[_key429] = _val430
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2496,17 +2496,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter403, viter404 in self.success.items():
-                oprot.writeString(kiter403)
-                viter404.write(oprot)
+            for kiter431, viter432 in self.success.items():
+                oprot.writeString(kiter431)
+                viter432.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -2638,19 +2638,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype408, _size405) = iprot.readListBegin()
-                    for _i409 in range(_size405):
-                        _elem410 = kCells()
-                        _elem410.read(iprot)
-                        self.success.append(_elem410)
+                    (_etype436, _size433) = iprot.readListBegin()
+                    for _i437 in range(_size433):
+                        _elem438 = kCells()
+                        _elem438.read(iprot)
+                        self.success.append(_elem438)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -2664,16 +2664,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('sql_select_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter411 in self.success:
-                iter411.write(oprot)
+            for iter439 in self.success:
+                iter439.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3685,25 +3685,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype413, _vtype414, _size412) = iprot.readMapBegin()
-                    for _i416 in range(_size412):
-                        _key417 = iprot.readI64()
-                        _val418 = []
-                        (_etype422, _size419) = iprot.readListBegin()
-                        for _i423 in range(_size419):
-                            _elem424 = UCell()
-                            _elem424.read(iprot)
-                            _val418.append(_elem424)
+                    (_ktype441, _vtype442, _size440) = iprot.readMapBegin()
+                    for _i444 in range(_size440):
+                        _key445 = iprot.readI64()
+                        _val446 = []
+                        (_etype450, _size447) = iprot.readListBegin()
+                        for _i451 in range(_size447):
+                            _elem452 = UCell()
+                            _elem452.read(iprot)
+                            _val446.append(_elem452)
                         iprot.readListEnd()
-                        self.cells[_key417] = _val418
+                        self.cells[_key445] = _val446
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -3717,19 +3717,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter425, viter426 in self.cells.items():
-                oprot.writeI64(kiter425)
-                oprot.writeListBegin(TType.STRUCT, len(viter426))
-                for iter427 in viter426:
-                    iter427.write(oprot)
+            for kiter453, viter454 in self.cells.items():
+                oprot.writeI64(kiter453)
+                oprot.writeListBegin(TType.STRUCT, len(viter454))
+                for iter455 in viter454:
+                    iter455.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -3863,25 +3863,25 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.cells = {}
-                    (_ktype429, _vtype430, _size428) = iprot.readMapBegin()
-                    for _i432 in range(_size428):
-                        _key433 = iprot.readI64()
-                        _val434 = []
-                        (_etype438, _size435) = iprot.readListBegin()
-                        for _i439 in range(_size435):
-                            _elem440 = UCellSerial()
-                            _elem440.read(iprot)
-                            _val434.append(_elem440)
+                    (_ktype457, _vtype458, _size456) = iprot.readMapBegin()
+                    for _i460 in range(_size456):
+                        _key461 = iprot.readI64()
+                        _val462 = []
+                        (_etype466, _size463) = iprot.readListBegin()
+                        for _i467 in range(_size463):
+                            _elem468 = UCellSerial()
+                            _elem468.read(iprot)
+                            _val462.append(_elem468)
                         iprot.readListEnd()
-                        self.cells[_key433] = _val434
+                        self.cells[_key461] = _val462
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.updater_id = iprot.readI64()
                 else:
@@ -3895,19 +3895,19 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('update_serial_args')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.MAP, 1)
             oprot.writeMapBegin(TType.I64, TType.LIST, len(self.cells))
-            for kiter441, viter442 in self.cells.items():
-                oprot.writeI64(kiter441)
-                oprot.writeListBegin(TType.STRUCT, len(viter442))
-                for iter443 in viter442:
-                    iter443.write(oprot)
+            for kiter469, viter470 in self.cells.items():
+                oprot.writeI64(kiter469)
+                oprot.writeListBegin(TType.STRUCT, len(viter470))
+                for iter471 in viter470:
+                    iter471.write(oprot)
                 oprot.writeListEnd()
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.updater_id is not None:
             oprot.writeFieldBegin('updater_id', TType.I64, 2)
             oprot.writeI64(self.updater_id)
             oprot.writeFieldEnd()
@@ -4275,19 +4275,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype447, _size444) = iprot.readListBegin()
-                    for _i448 in range(_size444):
-                        _elem449 = Schema()
-                        _elem449.read(iprot)
-                        self.success.append(_elem449)
+                    (_etype475, _size472) = iprot.readListBegin()
+                    for _i476 in range(_size472):
+                        _elem477 = Schema()
+                        _elem477.read(iprot)
+                        self.success.append(_elem477)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4301,16 +4301,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('list_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter450 in self.success:
-                iter450.write(oprot)
+            for iter478 in self.success:
+                iter478.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4443,19 +4443,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype454, _size451) = iprot.readListBegin()
-                    for _i455 in range(_size451):
-                        _elem456 = CompactResult()
-                        _elem456.read(iprot)
-                        self.success.append(_elem456)
+                    (_etype482, _size479) = iprot.readListBegin()
+                    for _i483 in range(_size479):
+                        _elem484 = CompactResult()
+                        _elem484.read(iprot)
+                        self.success.append(_elem484)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4469,16 +4469,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('compact_columns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter457 in self.success:
-                iter457.write(oprot)
+            for iter485 in self.success:
+                iter485.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4771,20 +4771,20 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.MAP:
                     self.success = {}
-                    (_ktype459, _vtype460, _size458) = iprot.readMapBegin()
-                    for _i462 in range(_size458):
-                        _key463 = iprot.readString()
-                        _val464 = ColCells()
-                        _val464.read(iprot)
-                        self.success[_key463] = _val464
+                    (_ktype487, _vtype488, _size486) = iprot.readMapBegin()
+                    for _i490 in range(_size486):
+                        _key491 = iprot.readString()
+                        _val492 = ColCells()
+                        _val492.read(iprot)
+                        self.success[_key491] = _val492
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4798,17 +4798,17 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_column_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.MAP, 0)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.success))
-            for kiter465, viter466 in self.success.items():
-                oprot.writeString(kiter465)
-                viter466.write(oprot)
+            for kiter493, viter494 in self.success.items():
+                oprot.writeString(kiter493)
+                viter494.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -4941,19 +4941,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype470, _size467) = iprot.readListBegin()
-                    for _i471 in range(_size467):
-                        _elem472 = kCells()
-                        _elem472.read(iprot)
-                        self.success.append(_elem472)
+                    (_etype498, _size495) = iprot.readListBegin()
+                    for _i499 in range(_size495):
+                        _elem500 = kCells()
+                        _elem500.read(iprot)
+                        self.success.append(_elem500)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.e = Exception.read(iprot)
                 else:
@@ -4967,16 +4967,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('scan_rslt_on_key_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter473 in self.success:
-                iter473.write(oprot)
+            for iter501 in self.success:
+                iter501.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.e is not None:
             oprot.writeFieldBegin('e', TType.STRUCT, 1)
             self.e.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
```

### Comparing `swcdb-0.5.8.1/swcdb/thrift/tornado/ttypes.py` & `swcdb-0.5.9.0/swcdb/thrift/tornado/ttypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,14 +246,41 @@
 
     _NAMES_TO_VALUES = {
         "UPDATING": 4,
         "DELETING": 8,
     }
 
 
+class UpdateOP(object):
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    SERIAL = 5
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "SERIAL",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "SERIAL": 5,
+    }
+
+
 class Flag(object):
     """
     The Cell Flag
 
     """
     NONE = 0
     INSERT = 1
@@ -271,14 +298,79 @@
         "NONE": 0,
         "INSERT": 1,
         "DELETE_LE": 2,
         "DELETE_EQ": 3,
     }
 
 
+class FU_MATH_OP(object):
+    """
+    MATH Operations for Serial Field Update of types INT64 and DOUBLE
+
+    """
+    EQUAL = 0
+    PLUS = 1
+    MULTIPLY = 2
+    DIVIDE = 3
+
+    _VALUES_TO_NAMES = {
+        0: "EQUAL",
+        1: "PLUS",
+        2: "MULTIPLY",
+        3: "DIVIDE",
+    }
+
+    _NAMES_TO_VALUES = {
+        "EQUAL": 0,
+        "PLUS": 1,
+        "MULTIPLY": 2,
+        "DIVIDE": 3,
+    }
+
+
+class FU_LIST_OP(object):
+    """
+    LIST Operations for Serial Field Update of array/list/bytes with LIST-op in the inner SERIAL fields
+
+    """
+    REPLACE = 0
+    APPEND = 1
+    PREPEND = 2
+    INSERT = 3
+    OVERWRITE = 4
+    ERASE = 5
+    BY_UNIQUE = 6
+    BY_COND = 7
+    BY_INDEX = 8
+
+    _VALUES_TO_NAMES = {
+        0: "REPLACE",
+        1: "APPEND",
+        2: "PREPEND",
+        3: "INSERT",
+        4: "OVERWRITE",
+        5: "ERASE",
+        6: "BY_UNIQUE",
+        7: "BY_COND",
+        8: "BY_INDEX",
+    }
+
+    _NAMES_TO_VALUES = {
+        "REPLACE": 0,
+        "APPEND": 1,
+        "PREPEND": 2,
+        "INSERT": 3,
+        "OVERWRITE": 4,
+        "ERASE": 5,
+        "BY_UNIQUE": 6,
+        "BY_COND": 7,
+        "BY_INDEX": 8,
+    }
+
+
 class CellsResult(object):
     """
     The Cells Results types for using with CellsGroup requests
 
     """
     IN_LIST = 0
     ON_COLUMN = 1
@@ -1519,36 +1611,119 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class SpecUpdateOP(object):
+    """
+    Attributes:
+     - op: The Operation of update
+     - pos: The position/index of INSERT and OVERWRITE update operations
+
+    """
+
+    __slots__ = (
+        'op',
+        'pos',
+    )
+
+
+    def __init__(self, op=None, pos=None,):
+        self.op = op
+        self.pos = pos
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('SpecUpdateOP')
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 1)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 2)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class SpecIntervalUpdate(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecInterval
 
     Attributes:
      - v: The value for the updated cell
      - ts: The timestamp for the updated cell NULL: MIN_INT64+1, AUTO:MIN_INT64+2 (or not-set)
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'v',
         'ts',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, v=None, ts=None, encoder=None,):
+    def __init__(self, v=None, ts=None, encoder=None, update_op=None,):
         self.v = v
         self.ts = ts
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1566,14 +1741,20 @@
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1588,14 +1769,18 @@
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 3)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 4)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1619,30 +1804,36 @@
 
 class SpecIntervalUpdateSerial(object):
     """
     The Value specs for an Updating Interval of 'updating' in SpecIntervalSerial
 
     Attributes:
      - ts: The timestamp for the updated cell NULL: MIN_INT64-1, AUTO:MIN_INT64-1
-     - v: The value for the updated cell
+     - v: The values of serial-fields for the updated cell
+     - v_op: The values of serial-fields for the the SERIAL operation update
      - encoder: Optionally the Cell Value Encoding Type: ZLIB/SNAPPY/ZSTD
+     - update_op: Optionally the operaton of value update
 
     """
 
     __slots__ = (
         'ts',
         'v',
+        'v_op',
         'encoder',
+        'update_op',
     )
 
 
-    def __init__(self, ts=None, v=None, encoder=None,):
+    def __init__(self, ts=None, v=None, v_op=None, encoder=None, update_op=None,):
         self.ts = ts
         self.v = v
+        self.v_op = v_op
         self.encoder = encoder
+        self.update_op = update_op
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
         iprot.readStructBegin()
         while True:
@@ -1662,18 +1853,35 @@
                         _elem54 = CellValueSerial()
                         _elem54.read(iprot)
                         self.v.append(_elem54)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
+                if ftype == TType.LIST:
+                    self.v_op = []
+                    (_etype58, _size55) = iprot.readListBegin()
+                    for _i59 in range(_size55):
+                        _elem60 = CellValueSerialOp()
+                        _elem60.read(iprot)
+                        self.v_op.append(_elem60)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
                     iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRUCT:
+                    self.update_op = SpecUpdateOP()
+                    self.update_op.read(iprot)
+                else:
+                    iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
 
     def write(self, oprot):
         if oprot._fast_encode is not None and self.thrift_spec is not None:
@@ -1683,22 +1891,33 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 1)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter55 in self.v:
-                iter55.write(oprot)
+            for iter61 in self.v:
+                iter61.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_op is not None:
+            oprot.writeFieldBegin('v_op', TType.LIST, 3)
+            oprot.writeListBegin(TType.STRUCT, len(self.v_op))
+            for iter62 in self.v_op:
+                iter62.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
-            oprot.writeFieldBegin('encoder', TType.I32, 3)
+            oprot.writeFieldBegin('encoder', TType.I32, 4)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
+        if self.update_op is not None:
+            oprot.writeFieldBegin('update_op', TType.STRUCT, 5)
+            self.update_op.write(oprot)
+            oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
 
     def __repr__(self):
@@ -1775,65 +1994,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype59, _size56) = iprot.readListBegin()
-                    for _i60 in range(_size56):
-                        _elem61 = iprot.readBinary()
-                        self.range_begin.append(_elem61)
+                    (_etype66, _size63) = iprot.readListBegin()
+                    for _i67 in range(_size63):
+                        _elem68 = iprot.readBinary()
+                        self.range_begin.append(_elem68)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype65, _size62) = iprot.readListBegin()
-                    for _i66 in range(_size62):
-                        _elem67 = iprot.readBinary()
-                        self.range_end.append(_elem67)
+                    (_etype72, _size69) = iprot.readListBegin()
+                    for _i73 in range(_size69):
+                        _elem74 = iprot.readBinary()
+                        self.range_end.append(_elem74)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype71, _size68) = iprot.readListBegin()
-                    for _i72 in range(_size68):
-                        _elem73 = iprot.readBinary()
-                        self.offset_key.append(_elem73)
+                    (_etype78, _size75) = iprot.readListBegin()
+                    for _i79 in range(_size75):
+                        _elem80 = iprot.readBinary()
+                        self.offset_key.append(_elem80)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype77, _size74) = iprot.readListBegin()
-                    for _i78 in range(_size74):
-                        _elem79 = SpecKeyInterval()
-                        _elem79.read(iprot)
-                        self.key_intervals.append(_elem79)
+                    (_etype84, _size81) = iprot.readListBegin()
+                    for _i85 in range(_size81):
+                        _elem86 = SpecKeyInterval()
+                        _elem86.read(iprot)
+                        self.key_intervals.append(_elem86)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype83, _size80) = iprot.readListBegin()
-                    for _i84 in range(_size80):
-                        _elem85 = SpecValue()
-                        _elem85.read(iprot)
-                        self.values.append(_elem85)
+                    (_etype90, _size87) = iprot.readListBegin()
+                    for _i91 in range(_size87):
+                        _elem92 = SpecValue()
+                        _elem92.read(iprot)
+                        self.values.append(_elem92)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -1871,48 +2090,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecInterval')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter86 in self.range_begin:
-                oprot.writeBinary(iter86)
+            for iter93 in self.range_begin:
+                oprot.writeBinary(iter93)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter87 in self.range_end:
-                oprot.writeBinary(iter87)
+            for iter94 in self.range_end:
+                oprot.writeBinary(iter94)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter88 in self.offset_key:
-                oprot.writeBinary(iter88)
+            for iter95 in self.offset_key:
+                oprot.writeBinary(iter95)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter89 in self.key_intervals:
-                iter89.write(oprot)
+            for iter96 in self.key_intervals:
+                iter96.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter90 in self.values:
-                iter90.write(oprot)
+            for iter97 in self.values:
+                iter97.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -1989,19 +2208,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype94, _size91) = iprot.readListBegin()
-                    for _i95 in range(_size91):
-                        _elem96 = SpecInterval()
-                        _elem96.read(iprot)
-                        self.intervals.append(_elem96)
+                    (_etype101, _size98) = iprot.readListBegin()
+                    for _i102 in range(_size98):
+                        _elem103 = SpecInterval()
+                        _elem103.read(iprot)
+                        self.intervals.append(_elem103)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2014,16 +2233,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter97 in self.intervals:
-                iter97.write(oprot)
+            for iter104 in self.intervals:
+                iter104.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2326,19 +2545,19 @@
                 if ftype == TType.I32:
                     self.seq = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype101, _size98) = iprot.readListBegin()
-                    for _i102 in range(_size98):
-                        _elem103 = SpecFraction()
-                        _elem103.read(iprot)
-                        self.v.append(_elem103)
+                    (_etype108, _size105) = iprot.readListBegin()
+                    for _i109 in range(_size105):
+                        _elem110 = SpecFraction()
+                        _elem110.read(iprot)
+                        self.v.append(_elem110)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2351,16 +2570,16 @@
         if self.seq is not None:
             oprot.writeFieldBegin('seq', TType.I32, 1)
             oprot.writeI32(self.seq)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter104 in self.v:
-                iter104.write(oprot)
+            for iter111 in self.v:
+                iter111.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2417,19 +2636,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype108, _size105) = iprot.readListBegin()
-                    for _i109 in range(_size105):
-                        _elem110 = SpecValueSerial_INT64()
-                        _elem110.read(iprot)
-                        self.v.append(_elem110)
+                    (_etype115, _size112) = iprot.readListBegin()
+                    for _i116 in range(_size112):
+                        _elem117 = SpecValueSerial_INT64()
+                        _elem117.read(iprot)
+                        self.v.append(_elem117)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2442,16 +2661,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter111 in self.v:
-                iter111.write(oprot)
+            for iter118 in self.v:
+                iter118.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2508,19 +2727,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype115, _size112) = iprot.readListBegin()
-                    for _i116 in range(_size112):
-                        _elem117 = SpecValueSerial_BYTES()
-                        _elem117.read(iprot)
-                        self.v.append(_elem117)
+                    (_etype122, _size119) = iprot.readListBegin()
+                    for _i123 in range(_size119):
+                        _elem124 = SpecValueSerial_BYTES()
+                        _elem124.read(iprot)
+                        self.v.append(_elem124)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2533,16 +2752,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter118 in self.v:
-                iter118.write(oprot)
+            for iter125 in self.v:
+                iter125.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2745,19 +2964,19 @@
                 if ftype == TType.I32:
                     self.comp = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.fields = []
-                    (_etype122, _size119) = iprot.readListBegin()
-                    for _i123 in range(_size119):
-                        _elem124 = SpecValueSerialField()
-                        _elem124.read(iprot)
-                        self.fields.append(_elem124)
+                    (_etype129, _size126) = iprot.readListBegin()
+                    for _i130 in range(_size126):
+                        _elem131 = SpecValueSerialField()
+                        _elem131.read(iprot)
+                        self.fields.append(_elem131)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -2770,16 +2989,16 @@
         if self.comp is not None:
             oprot.writeFieldBegin('comp', TType.I32, 1)
             oprot.writeI32(self.comp)
             oprot.writeFieldEnd()
         if self.fields is not None:
             oprot.writeFieldBegin('fields', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.fields))
-            for iter125 in self.fields:
-                iter125.write(oprot)
+            for iter132 in self.fields:
+                iter132.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -2858,65 +3077,65 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.range_begin = []
-                    (_etype129, _size126) = iprot.readListBegin()
-                    for _i130 in range(_size126):
-                        _elem131 = iprot.readBinary()
-                        self.range_begin.append(_elem131)
+                    (_etype136, _size133) = iprot.readListBegin()
+                    for _i137 in range(_size133):
+                        _elem138 = iprot.readBinary()
+                        self.range_begin.append(_elem138)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.range_end = []
-                    (_etype135, _size132) = iprot.readListBegin()
-                    for _i136 in range(_size132):
-                        _elem137 = iprot.readBinary()
-                        self.range_end.append(_elem137)
+                    (_etype142, _size139) = iprot.readListBegin()
+                    for _i143 in range(_size139):
+                        _elem144 = iprot.readBinary()
+                        self.range_end.append(_elem144)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.offset_key = []
-                    (_etype141, _size138) = iprot.readListBegin()
-                    for _i142 in range(_size138):
-                        _elem143 = iprot.readBinary()
-                        self.offset_key.append(_elem143)
+                    (_etype148, _size145) = iprot.readListBegin()
+                    for _i149 in range(_size145):
+                        _elem150 = iprot.readBinary()
+                        self.offset_key.append(_elem150)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.I64:
                     self.offset_rev = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.key_intervals = []
-                    (_etype147, _size144) = iprot.readListBegin()
-                    for _i148 in range(_size144):
-                        _elem149 = SpecKeyInterval()
-                        _elem149.read(iprot)
-                        self.key_intervals.append(_elem149)
+                    (_etype154, _size151) = iprot.readListBegin()
+                    for _i155 in range(_size151):
+                        _elem156 = SpecKeyInterval()
+                        _elem156.read(iprot)
+                        self.key_intervals.append(_elem156)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.values = []
-                    (_etype153, _size150) = iprot.readListBegin()
-                    for _i154 in range(_size150):
-                        _elem155 = SpecValueSerial()
-                        _elem155.read(iprot)
-                        self.values.append(_elem155)
+                    (_etype160, _size157) = iprot.readListBegin()
+                    for _i161 in range(_size157):
+                        _elem162 = SpecValueSerial()
+                        _elem162.read(iprot)
+                        self.values.append(_elem162)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.STRUCT:
                     self.ts_start = SpecTimestamp()
                     self.ts_start.read(iprot)
@@ -2954,48 +3173,48 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecIntervalSerial')
         if self.range_begin is not None:
             oprot.writeFieldBegin('range_begin', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.range_begin))
-            for iter156 in self.range_begin:
-                oprot.writeBinary(iter156)
+            for iter163 in self.range_begin:
+                oprot.writeBinary(iter163)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.range_end is not None:
             oprot.writeFieldBegin('range_end', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.range_end))
-            for iter157 in self.range_end:
-                oprot.writeBinary(iter157)
+            for iter164 in self.range_end:
+                oprot.writeBinary(iter164)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_key is not None:
             oprot.writeFieldBegin('offset_key', TType.LIST, 3)
             oprot.writeListBegin(TType.STRING, len(self.offset_key))
-            for iter158 in self.offset_key:
-                oprot.writeBinary(iter158)
+            for iter165 in self.offset_key:
+                oprot.writeBinary(iter165)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.offset_rev is not None:
             oprot.writeFieldBegin('offset_rev', TType.I64, 4)
             oprot.writeI64(self.offset_rev)
             oprot.writeFieldEnd()
         if self.key_intervals is not None:
             oprot.writeFieldBegin('key_intervals', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.key_intervals))
-            for iter159 in self.key_intervals:
-                iter159.write(oprot)
+            for iter166 in self.key_intervals:
+                iter166.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.values is not None:
             oprot.writeFieldBegin('values', TType.LIST, 6)
             oprot.writeListBegin(TType.STRUCT, len(self.values))
-            for iter160 in self.values:
-                iter160.write(oprot)
+            for iter167 in self.values:
+                iter167.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts_start is not None:
             oprot.writeFieldBegin('ts_start', TType.STRUCT, 7)
             self.ts_start.write(oprot)
             oprot.writeFieldEnd()
         if self.ts_finish is not None:
@@ -3072,19 +3291,19 @@
                 if ftype == TType.I64:
                     self.cid = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.intervals = []
-                    (_etype164, _size161) = iprot.readListBegin()
-                    for _i165 in range(_size161):
-                        _elem166 = SpecIntervalSerial()
-                        _elem166.read(iprot)
-                        self.intervals.append(_elem166)
+                    (_etype171, _size168) = iprot.readListBegin()
+                    for _i172 in range(_size168):
+                        _elem173 = SpecIntervalSerial()
+                        _elem173.read(iprot)
+                        self.intervals.append(_elem173)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3097,16 +3316,16 @@
         if self.cid is not None:
             oprot.writeFieldBegin('cid', TType.I64, 1)
             oprot.writeI64(self.cid)
             oprot.writeFieldEnd()
         if self.intervals is not None:
             oprot.writeFieldBegin('intervals', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.intervals))
-            for iter167 in self.intervals:
-                iter167.write(oprot)
+            for iter174 in self.intervals:
+                iter174.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3161,30 +3380,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.columns = []
-                    (_etype171, _size168) = iprot.readListBegin()
-                    for _i172 in range(_size168):
-                        _elem173 = SpecColumn()
-                        _elem173.read(iprot)
-                        self.columns.append(_elem173)
+                    (_etype178, _size175) = iprot.readListBegin()
+                    for _i179 in range(_size175):
+                        _elem180 = SpecColumn()
+                        _elem180.read(iprot)
+                        self.columns.append(_elem180)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.columns_serial = []
-                    (_etype177, _size174) = iprot.readListBegin()
-                    for _i178 in range(_size174):
-                        _elem179 = SpecColumnSerial()
-                        _elem179.read(iprot)
-                        self.columns_serial.append(_elem179)
+                    (_etype184, _size181) = iprot.readListBegin()
+                    for _i185 in range(_size181):
+                        _elem186 = SpecColumnSerial()
+                        _elem186.read(iprot)
+                        self.columns_serial.append(_elem186)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRUCT:
                     self.flags = SpecFlags()
                     self.flags.read(iprot)
@@ -3199,23 +3418,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('SpecScan')
         if self.columns is not None:
             oprot.writeFieldBegin('columns', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.columns))
-            for iter180 in self.columns:
-                iter180.write(oprot)
+            for iter187 in self.columns:
+                iter187.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.columns_serial is not None:
             oprot.writeFieldBegin('columns_serial', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.columns_serial))
-            for iter181 in self.columns_serial:
-                iter181.write(oprot)
+            for iter188 in self.columns_serial:
+                iter188.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.flags is not None:
             oprot.writeFieldBegin('flags', TType.STRUCT, 3)
             self.flags.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3288,18 +3507,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype185, _size182) = iprot.readListBegin()
-                    for _i186 in range(_size182):
-                        _elem187 = iprot.readBinary()
-                        self.k.append(_elem187)
+                    (_etype192, _size189) = iprot.readListBegin()
+                    for _i193 in range(_size189):
+                        _elem194 = iprot.readBinary()
+                        self.k.append(_elem194)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3332,16 +3551,16 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter188 in self.k:
-                oprot.writeBinary(iter188)
+            for iter195 in self.k:
+                oprot.writeBinary(iter195)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
@@ -3444,38 +3663,38 @@
                 if ftype == TType.STRING:
                     self.v_bytes = iprot.readBinary()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v_key = []
-                    (_etype192, _size189) = iprot.readListBegin()
-                    for _i193 in range(_size189):
-                        _elem194 = iprot.readBinary()
-                        self.v_key.append(_elem194)
+                    (_etype199, _size196) = iprot.readListBegin()
+                    for _i200 in range(_size196):
+                        _elem201 = iprot.readBinary()
+                        self.v_key.append(_elem201)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.LIST:
                     self.v_li = []
-                    (_etype198, _size195) = iprot.readListBegin()
-                    for _i199 in range(_size195):
-                        _elem200 = iprot.readI64()
-                        self.v_li.append(_elem200)
+                    (_etype205, _size202) = iprot.readListBegin()
+                    for _i206 in range(_size202):
+                        _elem207 = iprot.readI64()
+                        self.v_li.append(_elem207)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 7:
                 if ftype == TType.LIST:
                     self.v_lb = []
-                    (_etype204, _size201) = iprot.readListBegin()
-                    for _i205 in range(_size201):
-                        _elem206 = iprot.readBinary()
-                        self.v_lb.append(_elem206)
+                    (_etype211, _size208) = iprot.readListBegin()
+                    for _i212 in range(_size208):
+                        _elem213 = iprot.readBinary()
+                        self.v_lb.append(_elem213)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3500,30 +3719,499 @@
         if self.v_bytes is not None:
             oprot.writeFieldBegin('v_bytes', TType.STRING, 4)
             oprot.writeBinary(self.v_bytes)
             oprot.writeFieldEnd()
         if self.v_key is not None:
             oprot.writeFieldBegin('v_key', TType.LIST, 5)
             oprot.writeListBegin(TType.STRING, len(self.v_key))
-            for iter207 in self.v_key:
-                oprot.writeBinary(iter207)
+            for iter214 in self.v_key:
+                oprot.writeBinary(iter214)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_li is not None:
             oprot.writeFieldBegin('v_li', TType.LIST, 6)
             oprot.writeListBegin(TType.I64, len(self.v_li))
-            for iter208 in self.v_li:
-                oprot.writeI64(iter208)
+            for iter215 in self.v_li:
+                oprot.writeI64(iter215)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.v_lb is not None:
             oprot.writeFieldBegin('v_lb', TType.LIST, 7)
             oprot.writeListBegin(TType.STRING, len(self.v_lb))
-            for iter209 in self.v_lb:
-                oprot.writeBinary(iter209)
+            for iter216 in self.v_lb:
+                oprot.writeBinary(iter216)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_INT64(object):
+    """
+    Serial INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.I64:
+                    self.v = iprot.readI64()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_INT64')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.I64, 5)
+            oprot.writeI64(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_DOUBLE(object):
+    """
+    Serial DOUBLE Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.DOUBLE:
+                    self.v = iprot.readDouble()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_DOUBLE')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.DOUBLE, 5)
+            oprot.writeDouble(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_BYTES(object):
+    """
+    Serial BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - comp
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'comp',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, comp=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.comp = comp
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.I32:
+                    self.comp = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.STRING:
+                    self.v = iprot.readBinary()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_BYTES')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.comp is not None:
+            oprot.writeFieldBegin('comp', TType.I32, 4)
+            oprot.writeI32(self.comp)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.STRING, 5)
+            oprot.writeBinary(self.v)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class FU_LI(object):
+    """
+    Serial LIST_INT64 Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype220, _size217) = iprot.readListBegin()
+                    for _i221 in range(_size217):
+                        _elem222 = FU_INT64()
+                        _elem222.read(iprot)
+                        self.v.append(_elem222)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LI')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter223 in self.v:
+                iter223.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3543,14 +4231,284 @@
                 return False
         return True
 
     def __ne__(self, other):
         return not (self == other)
 
 
+class FU_LB(object):
+    """
+    Serial LIST_BYTES Field Update
+
+    Attributes:
+     - ctrl
+     - op
+     - pos
+     - v
+
+    """
+
+    __slots__ = (
+        'ctrl',
+        'op',
+        'pos',
+        'v',
+    )
+
+
+    def __init__(self, ctrl=0, op=0, pos=None, v=None,):
+        self.ctrl = ctrl
+        self.op = op
+        self.pos = pos
+        self.v = v
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.BYTE:
+                    self.ctrl = iprot.readByte()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.I32:
+                    self.op = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.I32:
+                    self.pos = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.LIST:
+                    self.v = []
+                    (_etype227, _size224) = iprot.readListBegin()
+                    for _i228 in range(_size224):
+                        _elem229 = FU_BYTES()
+                        _elem229.read(iprot)
+                        self.v.append(_elem229)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('FU_LB')
+        if self.ctrl is not None:
+            oprot.writeFieldBegin('ctrl', TType.BYTE, 1)
+            oprot.writeByte(self.ctrl)
+            oprot.writeFieldEnd()
+        if self.op is not None:
+            oprot.writeFieldBegin('op', TType.I32, 2)
+            oprot.writeI32(self.op)
+            oprot.writeFieldEnd()
+        if self.pos is not None:
+            oprot.writeFieldBegin('pos', TType.I32, 3)
+            oprot.writeI32(self.pos)
+            oprot.writeFieldEnd()
+        if self.v is not None:
+            oprot.writeFieldBegin('v', TType.LIST, 4)
+            oprot.writeListBegin(TType.STRUCT, len(self.v))
+            for iter230 in self.v:
+                iter230.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
+class CellValueSerialOp(object):
+    """
+    The Serial Values Cell field with Update Operation
+
+    Attributes:
+     - field_id: The Field ID, a single ID can have any/all the field types
+     - v_int64: The INT64 type update-field
+     - v_double: The DOUBLE type update-field
+     - v_bytes: The BYTES type update-field
+     - v_key: The Cell KEY type update-field
+     - v_li: The LIST INT64 type update-field
+     - v_lb: The LIST BYTES type update-field
+
+    """
+
+    __slots__ = (
+        'field_id',
+        'v_int64',
+        'v_double',
+        'v_bytes',
+        'v_key',
+        'v_li',
+        'v_lb',
+    )
+
+
+    def __init__(self, field_id=None, v_int64=None, v_double=None, v_bytes=None, v_key=None, v_li=None, v_lb=None,):
+        self.field_id = field_id
+        self.v_int64 = v_int64
+        self.v_double = v_double
+        self.v_bytes = v_bytes
+        self.v_key = v_key
+        self.v_li = v_li
+        self.v_lb = v_lb
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.I32:
+                    self.field_id = iprot.readI32()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.v_int64 = FU_INT64()
+                    self.v_int64.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRUCT:
+                    self.v_double = FU_DOUBLE()
+                    self.v_double.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRUCT:
+                    self.v_bytes = FU_BYTES()
+                    self.v_bytes.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 5:
+                if ftype == TType.LIST:
+                    self.v_key = []
+                    (_etype234, _size231) = iprot.readListBegin()
+                    for _i235 in range(_size231):
+                        _elem236 = iprot.readBinary()
+                        self.v_key.append(_elem236)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 6:
+                if ftype == TType.STRUCT:
+                    self.v_li = FU_LI()
+                    self.v_li.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 7:
+                if ftype == TType.STRUCT:
+                    self.v_lb = FU_LB()
+                    self.v_lb.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('CellValueSerialOp')
+        if self.field_id is not None:
+            oprot.writeFieldBegin('field_id', TType.I32, 1)
+            oprot.writeI32(self.field_id)
+            oprot.writeFieldEnd()
+        if self.v_int64 is not None:
+            oprot.writeFieldBegin('v_int64', TType.STRUCT, 2)
+            self.v_int64.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_double is not None:
+            oprot.writeFieldBegin('v_double', TType.STRUCT, 3)
+            self.v_double.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_bytes is not None:
+            oprot.writeFieldBegin('v_bytes', TType.STRUCT, 4)
+            self.v_bytes.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_key is not None:
+            oprot.writeFieldBegin('v_key', TType.LIST, 5)
+            oprot.writeListBegin(TType.STRING, len(self.v_key))
+            for iter237 in self.v_key:
+                oprot.writeBinary(iter237)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.v_li is not None:
+            oprot.writeFieldBegin('v_li', TType.STRUCT, 6)
+            self.v_li.write(oprot)
+            oprot.writeFieldEnd()
+        if self.v_lb is not None:
+            oprot.writeFieldBegin('v_lb', TType.STRUCT, 7)
+            self.v_lb.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, getattr(self, key))
+             for key in self.__slots__]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+        for attr in self.__slots__:
+            my_val = getattr(self, attr)
+            other_val = getattr(other, attr)
+            if my_val != other_val:
+                return False
+        return True
+
+    def __ne__(self, other):
+        return not (self == other)
+
+
 class UCellSerial(object):
     """
     The Cell data for using with Update of SERIAL Column Type
 
     Attributes:
      - f: The Cell Flag
      - k: The Cell Key
@@ -3592,18 +4550,18 @@
                 if ftype == TType.I32:
                     self.f = iprot.readI32()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype213, _size210) = iprot.readListBegin()
-                    for _i214 in range(_size210):
-                        _elem215 = iprot.readBinary()
-                        self.k.append(_elem215)
+                    (_etype241, _size238) = iprot.readListBegin()
+                    for _i242 in range(_size238):
+                        _elem243 = iprot.readBinary()
+                        self.k.append(_elem243)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3612,19 +4570,19 @@
                 if ftype == TType.BOOL:
                     self.ts_desc = iprot.readBool()
                 else:
                     iprot.skip(ftype)
             elif fid == 5:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype219, _size216) = iprot.readListBegin()
-                    for _i220 in range(_size216):
-                        _elem221 = CellValueSerial()
-                        _elem221.read(iprot)
-                        self.v.append(_elem221)
+                    (_etype247, _size244) = iprot.readListBegin()
+                    for _i248 in range(_size244):
+                        _elem249 = CellValueSerial()
+                        _elem249.read(iprot)
+                        self.v.append(_elem249)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 6:
                 if ftype == TType.I32:
                     self.encoder = iprot.readI32()
                 else:
@@ -3642,31 +4600,31 @@
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.I32, 1)
             oprot.writeI32(self.f)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter222 in self.k:
-                oprot.writeBinary(iter222)
+            for iter250 in self.k:
+                oprot.writeBinary(iter250)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.ts_desc is not None:
             oprot.writeFieldBegin('ts_desc', TType.BOOL, 4)
             oprot.writeBool(self.ts_desc)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 5)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter223 in self.v:
-                iter223.write(oprot)
+            for iter251 in self.v:
+                iter251.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.encoder is not None:
             oprot.writeFieldBegin('encoder', TType.I32, 6)
             oprot.writeI32(self.encoder)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -3733,18 +4691,18 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype227, _size224) = iprot.readListBegin()
-                    for _i228 in range(_size224):
-                        _elem229 = iprot.readBinary()
-                        self.k.append(_elem229)
+                    (_etype255, _size252) = iprot.readListBegin()
+                    for _i256 in range(_size252):
+                        _elem257 = iprot.readBinary()
+                        self.k.append(_elem257)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -3767,16 +4725,16 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter230 in self.k:
-                oprot.writeBinary(iter230)
+            for iter258 in self.k:
+                oprot.writeBinary(iter258)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -3847,34 +4805,34 @@
                 if ftype == TType.STRING:
                     self.c = iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype234, _size231) = iprot.readListBegin()
-                    for _i235 in range(_size231):
-                        _elem236 = iprot.readBinary()
-                        self.k.append(_elem236)
+                    (_etype262, _size259) = iprot.readListBegin()
+                    for _i263 in range(_size259):
+                        _elem264 = iprot.readBinary()
+                        self.k.append(_elem264)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype240, _size237) = iprot.readListBegin()
-                    for _i241 in range(_size237):
-                        _elem242 = CellValueSerial()
-                        _elem242.read(iprot)
-                        self.v.append(_elem242)
+                    (_etype268, _size265) = iprot.readListBegin()
+                    for _i269 in range(_size265):
+                        _elem270 = CellValueSerial()
+                        _elem270.read(iprot)
+                        self.v.append(_elem270)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3887,27 +4845,27 @@
         if self.c is not None:
             oprot.writeFieldBegin('c', TType.STRING, 1)
             oprot.writeString(self.c)
             oprot.writeFieldEnd()
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 2)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter243 in self.k:
-                oprot.writeBinary(iter243)
+            for iter271 in self.k:
+                oprot.writeBinary(iter271)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 3)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 4)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter244 in self.v:
-                iter244.write(oprot)
+            for iter272 in self.v:
+                iter272.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3959,30 +4917,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype248, _size245) = iprot.readListBegin()
-                    for _i249 in range(_size245):
-                        _elem250 = Cell()
-                        _elem250.read(iprot)
-                        self.cells.append(_elem250)
+                    (_etype276, _size273) = iprot.readListBegin()
+                    for _i277 in range(_size273):
+                        _elem278 = Cell()
+                        _elem278.read(iprot)
+                        self.cells.append(_elem278)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype254, _size251) = iprot.readListBegin()
-                    for _i255 in range(_size251):
-                        _elem256 = CellSerial()
-                        _elem256.read(iprot)
-                        self.serial_cells.append(_elem256)
+                    (_etype282, _size279) = iprot.readListBegin()
+                    for _i283 in range(_size279):
+                        _elem284 = CellSerial()
+                        _elem284.read(iprot)
+                        self.serial_cells.append(_elem284)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3991,23 +4949,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Cells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter257 in self.cells:
-                iter257.write(oprot)
+            for iter285 in self.cells:
+                iter285.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter258 in self.serial_cells:
-                iter258.write(oprot)
+            for iter286 in self.serial_cells:
+                iter286.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4062,18 +5020,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype262, _size259) = iprot.readListBegin()
-                    for _i263 in range(_size259):
-                        _elem264 = iprot.readBinary()
-                        self.k.append(_elem264)
+                    (_etype290, _size287) = iprot.readListBegin()
+                    for _i291 in range(_size287):
+                        _elem292 = iprot.readBinary()
+                        self.k.append(_elem292)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
@@ -4092,16 +5050,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCell')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter265 in self.k:
-                oprot.writeBinary(iter265)
+            for iter293 in self.k:
+                oprot.writeBinary(iter293)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
@@ -4164,34 +5122,34 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype269, _size266) = iprot.readListBegin()
-                    for _i270 in range(_size266):
-                        _elem271 = iprot.readBinary()
-                        self.k.append(_elem271)
+                    (_etype297, _size294) = iprot.readListBegin()
+                    for _i298 in range(_size294):
+                        _elem299 = iprot.readBinary()
+                        self.k.append(_elem299)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype275, _size272) = iprot.readListBegin()
-                    for _i276 in range(_size272):
-                        _elem277 = CellValueSerial()
-                        _elem277.read(iprot)
-                        self.v.append(_elem277)
+                    (_etype303, _size300) = iprot.readListBegin()
+                    for _i304 in range(_size300):
+                        _elem305 = CellValueSerial()
+                        _elem305.read(iprot)
+                        self.v.append(_elem305)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4200,27 +5158,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('CCellSerial')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter278 in self.k:
-                oprot.writeBinary(iter278)
+            for iter306 in self.k:
+                oprot.writeBinary(iter306)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter279 in self.v:
-                iter279.write(oprot)
+            for iter307 in self.v:
+                iter307.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4272,30 +5230,30 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype283, _size280) = iprot.readListBegin()
-                    for _i284 in range(_size280):
-                        _elem285 = CCell()
-                        _elem285.read(iprot)
-                        self.cells.append(_elem285)
+                    (_etype311, _size308) = iprot.readListBegin()
+                    for _i312 in range(_size308):
+                        _elem313 = CCell()
+                        _elem313.read(iprot)
+                        self.cells.append(_elem313)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype289, _size286) = iprot.readListBegin()
-                    for _i290 in range(_size286):
-                        _elem291 = CCellSerial()
-                        _elem291.read(iprot)
-                        self.serial_cells.append(_elem291)
+                    (_etype317, _size314) = iprot.readListBegin()
+                    for _i318 in range(_size314):
+                        _elem319 = CCellSerial()
+                        _elem319.read(iprot)
+                        self.serial_cells.append(_elem319)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4304,23 +5262,23 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('ColCells')
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter292 in self.cells:
-                iter292.write(oprot)
+            for iter320 in self.cells:
+                iter320.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter293 in self.serial_cells:
-                iter293.write(oprot)
+            for iter321 in self.serial_cells:
+                iter321.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4479,19 +5437,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype297, _size294) = iprot.readListBegin()
-                    for _i298 in range(_size294):
-                        _elem299 = CellValueSerial()
-                        _elem299.read(iprot)
-                        self.v.append(_elem299)
+                    (_etype325, _size322) = iprot.readListBegin()
+                    for _i326 in range(_size322):
+                        _elem327 = CellValueSerial()
+                        _elem327.read(iprot)
+                        self.v.append(_elem327)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4508,16 +5466,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter300 in self.v:
-                iter300.write(oprot)
+            for iter328 in self.v:
+                iter328.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4572,40 +5530,40 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.k = []
-                    (_etype304, _size301) = iprot.readListBegin()
-                    for _i305 in range(_size301):
-                        _elem306 = iprot.readBinary()
-                        self.k.append(_elem306)
+                    (_etype332, _size329) = iprot.readListBegin()
+                    for _i333 in range(_size329):
+                        _elem334 = iprot.readBinary()
+                        self.k.append(_elem334)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype310, _size307) = iprot.readListBegin()
-                    for _i311 in range(_size307):
-                        _elem312 = KCell()
-                        _elem312.read(iprot)
-                        self.cells.append(_elem312)
+                    (_etype338, _size335) = iprot.readListBegin()
+                    for _i339 in range(_size335):
+                        _elem340 = KCell()
+                        _elem340.read(iprot)
+                        self.cells.append(_elem340)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype316, _size313) = iprot.readListBegin()
-                    for _i317 in range(_size313):
-                        _elem318 = KCellSerial()
-                        _elem318.read(iprot)
-                        self.serial_cells.append(_elem318)
+                    (_etype344, _size341) = iprot.readListBegin()
+                    for _i345 in range(_size341):
+                        _elem346 = KCellSerial()
+                        _elem346.read(iprot)
+                        self.serial_cells.append(_elem346)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4614,30 +5572,30 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('kCells')
         if self.k is not None:
             oprot.writeFieldBegin('k', TType.LIST, 1)
             oprot.writeListBegin(TType.STRING, len(self.k))
-            for iter319 in self.k:
-                oprot.writeBinary(iter319)
+            for iter347 in self.k:
+                oprot.writeBinary(iter347)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter320 in self.cells:
-                iter320.write(oprot)
+            for iter348 in self.cells:
+                iter348.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter321 in self.serial_cells:
-                iter321.write(oprot)
+            for iter349 in self.serial_cells:
+                iter349.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4796,19 +5754,19 @@
                 if ftype == TType.I64:
                     self.ts = iprot.readI64()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.v = []
-                    (_etype325, _size322) = iprot.readListBegin()
-                    for _i326 in range(_size322):
-                        _elem327 = CellValueSerial()
-                        _elem327.read(iprot)
-                        self.v.append(_elem327)
+                    (_etype353, _size350) = iprot.readListBegin()
+                    for _i354 in range(_size350):
+                        _elem355 = CellValueSerial()
+                        _elem355.read(iprot)
+                        self.v.append(_elem355)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4825,16 +5783,16 @@
         if self.ts is not None:
             oprot.writeFieldBegin('ts', TType.I64, 2)
             oprot.writeI64(self.ts)
             oprot.writeFieldEnd()
         if self.v is not None:
             oprot.writeFieldBegin('v', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.v))
-            for iter328 in self.v:
-                iter328.write(oprot)
+            for iter356 in self.v:
+                iter356.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -4889,42 +5847,42 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.MAP:
                     self.f = {}
-                    (_ktype330, _vtype331, _size329) = iprot.readMapBegin()
-                    for _i333 in range(_size329):
-                        _key334 = iprot.readBinary()
-                        _val335 = FCells()
-                        _val335.read(iprot)
-                        self.f[_key334] = _val335
+                    (_ktype358, _vtype359, _size357) = iprot.readMapBegin()
+                    for _i361 in range(_size357):
+                        _key362 = iprot.readBinary()
+                        _val363 = FCells()
+                        _val363.read(iprot)
+                        self.f[_key362] = _val363
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.LIST:
                     self.cells = []
-                    (_etype339, _size336) = iprot.readListBegin()
-                    for _i340 in range(_size336):
-                        _elem341 = FCell()
-                        _elem341.read(iprot)
-                        self.cells.append(_elem341)
+                    (_etype367, _size364) = iprot.readListBegin()
+                    for _i368 in range(_size364):
+                        _elem369 = FCell()
+                        _elem369.read(iprot)
+                        self.cells.append(_elem369)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.serial_cells = []
-                    (_etype345, _size342) = iprot.readListBegin()
-                    for _i346 in range(_size342):
-                        _elem347 = FCellSerial()
-                        _elem347.read(iprot)
-                        self.serial_cells.append(_elem347)
+                    (_etype373, _size370) = iprot.readListBegin()
+                    for _i374 in range(_size370):
+                        _elem375 = FCellSerial()
+                        _elem375.read(iprot)
+                        self.serial_cells.append(_elem375)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -4933,31 +5891,31 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('FCells')
         if self.f is not None:
             oprot.writeFieldBegin('f', TType.MAP, 1)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.f))
-            for kiter348, viter349 in self.f.items():
-                oprot.writeBinary(kiter348)
-                viter349.write(oprot)
+            for kiter376, viter377 in self.f.items():
+                oprot.writeBinary(kiter376)
+                viter377.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.LIST, 2)
             oprot.writeListBegin(TType.STRUCT, len(self.cells))
-            for iter350 in self.cells:
-                iter350.write(oprot)
+            for iter378 in self.cells:
+                iter378.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.serial_cells is not None:
             oprot.writeFieldBegin('serial_cells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.serial_cells))
-            for iter351 in self.serial_cells:
-                iter351.write(oprot)
+            for iter379 in self.serial_cells:
+                iter379.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5021,31 +5979,31 @@
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.MAP:
                     self.ccells = {}
-                    (_ktype353, _vtype354, _size352) = iprot.readMapBegin()
-                    for _i356 in range(_size352):
-                        _key357 = iprot.readString()
-                        _val358 = ColCells()
-                        _val358.read(iprot)
-                        self.ccells[_key357] = _val358
+                    (_ktype381, _vtype382, _size380) = iprot.readMapBegin()
+                    for _i384 in range(_size380):
+                        _key385 = iprot.readString()
+                        _val386 = ColCells()
+                        _val386.read(iprot)
+                        self.ccells[_key385] = _val386
                     iprot.readMapEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.kcells = []
-                    (_etype362, _size359) = iprot.readListBegin()
-                    for _i363 in range(_size359):
-                        _elem364 = kCells()
-                        _elem364.read(iprot)
-                        self.kcells.append(_elem364)
+                    (_etype390, _size387) = iprot.readListBegin()
+                    for _i391 in range(_size387):
+                        _elem392 = kCells()
+                        _elem392.read(iprot)
+                        self.kcells.append(_elem392)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 4:
                 if ftype == TType.STRUCT:
                     self.fcells = FCells()
                     self.fcells.read(iprot)
@@ -5064,24 +6022,24 @@
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 1)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.ccells is not None:
             oprot.writeFieldBegin('ccells', TType.MAP, 2)
             oprot.writeMapBegin(TType.STRING, TType.STRUCT, len(self.ccells))
-            for kiter365, viter366 in self.ccells.items():
-                oprot.writeString(kiter365)
-                viter366.write(oprot)
+            for kiter393, viter394 in self.ccells.items():
+                oprot.writeString(kiter393)
+                viter394.write(oprot)
             oprot.writeMapEnd()
             oprot.writeFieldEnd()
         if self.kcells is not None:
             oprot.writeFieldBegin('kcells', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.kcells))
-            for iter367 in self.kcells:
-                iter367.write(oprot)
+            for iter395 in self.kcells:
+                iter395.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.fcells is not None:
             oprot.writeFieldBegin('fcells', TType.STRUCT, 4)
             self.fcells.write(oprot)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
@@ -5222,36 +6180,36 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 1:
                 if ftype == TType.LIST:
                     self.schemas = []
-                    (_etype371, _size368) = iprot.readListBegin()
-                    for _i372 in range(_size368):
-                        _elem373 = Schema()
-                        _elem373.read(iprot)
-                        self.schemas.append(_elem373)
+                    (_etype399, _size396) = iprot.readListBegin()
+                    for _i400 in range(_size396):
+                        _elem401 = Schema()
+                        _elem401.read(iprot)
+                        self.schemas.append(_elem401)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRUCT:
                     self.cells = Cells()
                     self.cells.read(iprot)
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.LIST:
                     self.compact = []
-                    (_etype377, _size374) = iprot.readListBegin()
-                    for _i378 in range(_size374):
-                        _elem379 = CompactResult()
-                        _elem379.read(iprot)
-                        self.compact.append(_elem379)
+                    (_etype405, _size402) = iprot.readListBegin()
+                    for _i406 in range(_size402):
+                        _elem407 = CompactResult()
+                        _elem407.read(iprot)
+                        self.compact.append(_elem407)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -5260,27 +6218,27 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('Result')
         if self.schemas is not None:
             oprot.writeFieldBegin('schemas', TType.LIST, 1)
             oprot.writeListBegin(TType.STRUCT, len(self.schemas))
-            for iter380 in self.schemas:
-                iter380.write(oprot)
+            for iter408 in self.schemas:
+                iter408.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.cells is not None:
             oprot.writeFieldBegin('cells', TType.STRUCT, 2)
             self.cells.write(oprot)
             oprot.writeFieldEnd()
         if self.compact is not None:
             oprot.writeFieldBegin('compact', TType.LIST, 3)
             oprot.writeListBegin(TType.STRUCT, len(self.compact))
-            for iter381 in self.compact:
-                iter381.write(oprot)
+            for iter409 in self.compact:
+                iter409.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -5384,27 +6342,36 @@
 )
 all_structs.append(SpecValue)
 SpecValue.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'comp', None, None, ),  # 1
     (2, TType.STRING, 'v', 'BINARY', None, ),  # 2
 )
+all_structs.append(SpecUpdateOP)
+SpecUpdateOP.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'op', None, None, ),  # 1
+    (2, TType.I32, 'pos', None, None, ),  # 2
+)
 all_structs.append(SpecIntervalUpdate)
 SpecIntervalUpdate.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'v', 'BINARY', None, ),  # 1
     (2, TType.I64, 'ts', None, None, ),  # 2
     (3, TType.I32, 'encoder', None, None, ),  # 3
+    (4, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 4
 )
 all_structs.append(SpecIntervalUpdateSerial)
 SpecIntervalUpdateSerial.thrift_spec = (
     None,  # 0
     (1, TType.I64, 'ts', None, None, ),  # 1
     (2, TType.LIST, 'v', (TType.STRUCT, [CellValueSerial, None], False), None, ),  # 2
-    (3, TType.I32, 'encoder', None, None, ),  # 3
+    (3, TType.LIST, 'v_op', (TType.STRUCT, [CellValueSerialOp, None], False), None, ),  # 3
+    (4, TType.I32, 'encoder', None, None, ),  # 4
+    (5, TType.STRUCT, 'update_op', [SpecUpdateOP, None], None, ),  # 5
 )
 all_structs.append(SpecInterval)
 SpecInterval.thrift_spec = (
     None,  # 0
     (1, TType.LIST, 'range_begin', (TType.STRING, 'BINARY', False), None, ),  # 1
     (2, TType.LIST, 'range_end', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.LIST, 'offset_key', (TType.STRING, 'BINARY', False), None, ),  # 3
@@ -5521,14 +6488,68 @@
     (2, TType.I64, 'v_int64', None, None, ),  # 2
     (3, TType.DOUBLE, 'v_double', None, None, ),  # 3
     (4, TType.STRING, 'v_bytes', 'BINARY', None, ),  # 4
     (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
     (6, TType.LIST, 'v_li', (TType.I64, None, False), None, ),  # 6
     (7, TType.LIST, 'v_lb', (TType.STRING, 'BINARY', False), None, ),  # 7
 )
+all_structs.append(FU_INT64)
+FU_INT64.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.I64, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_DOUBLE)
+FU_DOUBLE.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.DOUBLE, 'v', None, None, ),  # 5
+)
+all_structs.append(FU_BYTES)
+FU_BYTES.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.I32, 'comp', None, None, ),  # 4
+    (5, TType.STRING, 'v', 'BINARY', None, ),  # 5
+)
+all_structs.append(FU_LI)
+FU_LI.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_INT64, None], False), None, ),  # 4
+)
+all_structs.append(FU_LB)
+FU_LB.thrift_spec = (
+    None,  # 0
+    (1, TType.BYTE, 'ctrl', None, 0, ),  # 1
+    (2, TType.I32, 'op', None, 0, ),  # 2
+    (3, TType.I32, 'pos', None, None, ),  # 3
+    (4, TType.LIST, 'v', (TType.STRUCT, [FU_BYTES, None], False), None, ),  # 4
+)
+all_structs.append(CellValueSerialOp)
+CellValueSerialOp.thrift_spec = (
+    None,  # 0
+    (1, TType.I32, 'field_id', None, None, ),  # 1
+    (2, TType.STRUCT, 'v_int64', [FU_INT64, None], None, ),  # 2
+    (3, TType.STRUCT, 'v_double', [FU_DOUBLE, None], None, ),  # 3
+    (4, TType.STRUCT, 'v_bytes', [FU_BYTES, None], None, ),  # 4
+    (5, TType.LIST, 'v_key', (TType.STRING, 'BINARY', False), None, ),  # 5
+    (6, TType.STRUCT, 'v_li', [FU_LI, None], None, ),  # 6
+    (7, TType.STRUCT, 'v_lb', [FU_LB, None], None, ),  # 7
+)
 all_structs.append(UCellSerial)
 UCellSerial.thrift_spec = (
     None,  # 0
     (1, TType.I32, 'f', None, None, ),  # 1
     (2, TType.LIST, 'k', (TType.STRING, 'BINARY', False), None, ),  # 2
     (3, TType.I64, 'ts', None, None, ),  # 3
     (4, TType.BOOL, 'ts_desc', None, None, ),  # 4
```

### Comparing `swcdb-0.5.8.1/swcdb/serialization.py` & `swcdb-0.5.9.0/swcdb/serialization.py`

 * *Files identical despite different names*

### Comparing `swcdb-0.5.8.1/setup.py` & `swcdb-0.5.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,26 @@
                 '/usr/local/include', '/usr/include'] + \
                 ''.split(';') + \
                 ''.split(';') + \
                 '/usr/local/include'.split(';')
 include_dirs = list(set(include_dirs))
 
 extra_compile_args = [a for a in set([a.strip() 
-                      for a in " -D_LARGEFILE_SOURCE -m64 -D_FILE_OFFSET_BITS=64 -O3 -Wall -Werror -Wextra -Wpedantic -Wformat-security -Wformat-nonliteral -Wcast-align -Wnon-virtual-dtor -Wzero-as-null-pointer-constant -Wno-error=zero-as-null-pointer-constant -Wold-style-cast -Wno-error=old-style-cast -Wnull-dereference -Wno-error=null-dereference -Wformat-signedness -Wnoexcept -Wno-error=noexcept -Wsuggest-override -Wno-error=suggest-override -Wuseless-cast -Wno-error=useless-cast -Wstrict-null-sentinel -Wno-error=strict-null-sentinel -Wduplicated-cond -Wno-error=duplicated-cond -Wduplicated-branches -Wno-error=duplicated-branches -Wlogical-op -Wno-error=logical-op -Wshadow=compatible-local -Wshadow=local -Wshadow=global -Wshadow -Wno-error=shadow=compatible-local -Wno-error=shadow=local -Wno-error=shadow=global -Wno-error=shadow -Wstack-usage=16384 -Wno-error=stack-usage=16384 -Wtrampolines -Wsuggest-attribute=const -Wno-error=suggest-attribute=const -Wsuggest-attribute=pure -Wno-error=suggest-attribute=pure -Wsuggest-attribute=malloc -Wno-error=suggest-attribute=malloc -Wsuggest-attribute=cold -Wno-error=suggest-attribute=cold -Wtsan -DASIO_STANDALONE -DASIO_NO_DEPRECATED -DOPENSSL_NO_SSL2 -DOPENSSL_NO_SSL3  -D_LARGEFILE_SOURCE -m64 -D_FILE_OFFSET_BITS=64 -O3 -Wall -Werror -Wformat-security".split(' ')]) if a]
+                      for a in " -D_LARGEFILE_SOURCE -m64 -D_FILE_OFFSET_BITS=64 -O3 -flto -fuse-linker-plugin -ffat-lto-objects -fdevirtualize-at-ltrans -Wall -Werror -Wextra -Wpedantic -Wformat-security -Wformat-nonliteral -Wcast-align -Wnon-virtual-dtor -Wzero-as-null-pointer-constant -Wno-error=zero-as-null-pointer-constant -Wold-style-cast -Wno-error=old-style-cast -Wnull-dereference -Wno-error=null-dereference -Wformat-signedness -Wnoexcept -Wno-error=noexcept -Wsuggest-override -Wno-error=suggest-override -Wuseless-cast -Wno-error=useless-cast -Wstrict-null-sentinel -Wno-error=strict-null-sentinel -Wduplicated-cond -Wno-error=duplicated-cond -Wduplicated-branches -Wno-error=duplicated-branches -Wlogical-op -Wno-error=logical-op -Wshadow=compatible-local -Wshadow=local -Wshadow=global -Wshadow -Wno-error=shadow=compatible-local -Wno-error=shadow=local -Wno-error=shadow=global -Wno-error=shadow -Wstack-usage=16384 -Wno-error=stack-usage=16384 -Wtrampolines -Wsuggest-attribute=const -Wno-error=suggest-attribute=const -Wsuggest-attribute=pure -Wno-error=suggest-attribute=pure -Wsuggest-attribute=malloc -Wno-error=suggest-attribute=malloc -Wsuggest-attribute=cold -Wno-error=suggest-attribute=cold -Wtsan -DASIO_STANDALONE -DASIO_NO_DEPRECATED -DOPENSSL_NO_DEPRECATED -DOPENSSL_NO_SSL2 -DOPENSSL_NO_SSL3  -D_LARGEFILE_SOURCE -m64 -D_FILE_OFFSET_BITS=64 -O3 -flto -fuse-linker-plugin -ffat-lto-objects -Wall -Werror -Wformat-security".split(' ')]) if a]
 
 libraries=[l.split('/')[-1].split('.')[0][3:] 
            for l in '/usr/local/lib/libtcmalloc_minimal.so.4.5.9'.split(';') 
            if '/' in l]
 
 extensions = []
 
 
 setup(
     name='swcdb',
-    version='0.5.8.1',
+    version='0.5.9.0',
     description='The SWC-DB Python Package',
     long_description=long_description,
 
     # long_description_content_type='text/markdown',
     # install_requires=['thrift>=0.16.0'],
 
     url='https://github.com/kashirin-alex/swc-db',
```

