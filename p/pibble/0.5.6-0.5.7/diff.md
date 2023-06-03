# Comparing `tmp/pibble-0.5.6.tar.gz` & `tmp/pibble-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.5.6.tar", last modified: Tue May 16 17:44:22 2023, max compression
+gzip compressed data, was "pibble-0.5.7.tar", last modified: Sat Jun  3 21:55:54 2023, max compression
```

## Comparing `pibble-0.5.6.tar` & `pibble-0.5.7.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-16 17:44:22.846976 pibble-0.5.6/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-05-16 17:44:22.000000 pibble-0.5.6/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9049 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/configuration.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6101 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/database/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2841 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.838976 pibble-0.5.6/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/awslambda.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    38922 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/drivers/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1489 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/driver_cherrypy.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2229 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/driver_gunicorn.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1078 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/drivers/driver_werkzeug.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/jsonapi.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4149 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16963 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/dedupe.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10593 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    28607 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/database/view.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/middleware.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/cms/server/extension.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15664 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/server/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7245 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:21.000000 pibble-0.5.6/pibble/ext/session/server/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5087 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.842976 pibble-0.5.6/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24936 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/resources/retriever.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/scripts/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/scripts/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/scripts/importcheck.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/scripts/templatefiles.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32914 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/imaging.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6330 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    27424 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.846976 pibble-0.5.6/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-05-16 17:44:20.000000 pibble-0.5.6/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-05-16 17:44:22.834976 pibble-0.5.6/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-05-16 17:44:22.000000 pibble-0.5.6/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-05-16 17:44:22.846976 pibble-0.5.6/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-05-16 17:44:22.000000 pibble-0.5.6/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-06-03 21:55:54.424484 pibble-0.5.7/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-06-03 21:55:54.000000 pibble-0.5.7/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.412485 pibble-0.5.7/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9049 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.412485 pibble-0.5.7/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.412485 pibble-0.5.7/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.412485 pibble-0.5.7/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.412485 pibble-0.5.7/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/configuration.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6402 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/database/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2841 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/limit.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.416484 pibble-0.5.7/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/awslambda.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    39048 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/api/server/webservice/drivers/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/drivers/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1600 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/drivers/driver_cherrypy.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2318 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/drivers/driver_gunicorn.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1120 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/drivers/driver_werkzeug.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/jsonapi.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4149 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16963 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/database/dedupe.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10591 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    28607 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/database/view.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/middleware.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/cms/server/extension.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/rest/server/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16200 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/rest/server/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7474 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/session/server/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5087 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.420484 pibble-0.5.7/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/client/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/database/notification.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/database/permission.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24936 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/resources/retriever.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/scripts/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/scripts/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/scripts/importcheck.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/scripts/templatefiles.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32914 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/imaging.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6634 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    27424 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.424484 pibble-0.5.7/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3227 2023-06-03 21:55:53.000000 pibble-0.5.7/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-03 21:55:54.412485 pibble-0.5.7/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5627 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-06-03 21:55:54.000000 pibble-0.5.7/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-06-03 21:55:54.424484 pibble-0.5.7/setup.cfg
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-06-03 21:55:54.000000 pibble-0.5.7/setup.py
```

### Comparing `pibble-0.5.6/PKG-INFO` & `pibble-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.6
+Version: 0.5.7
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.6/README.md` & `pibble-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/__main__.py` & `pibble-0.5.7/pibble/__main__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/base.py` & `pibble-0.5.7/pibble/api/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/apachethrift/__init__.py` & `pibble-0.5.7/pibble/api/client/apachethrift/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.5.7/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/base.py` & `pibble-0.5.7/pibble/api/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/file/base.py` & `pibble-0.5.7/pibble/api/client/file/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/file/ftp.py` & `pibble-0.5.7/pibble/api/client/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/file/hdfs.py` & `pibble-0.5.7/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/file/local.py` & `pibble-0.5.7/pibble/api/client/file/local.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/file/sftp.py` & `pibble-0.5.7/pibble/api/client/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/googlerpc.py` & `pibble-0.5.7/pibble/api/client/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/apachethrift.py` & `pibble-0.5.7/pibble/api/client/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/base.py` & `pibble-0.5.7/pibble/api/client/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/jsonapi.py` & `pibble-0.5.7/pibble/api/client/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/rpc/base.py` & `pibble-0.5.7/pibble/api/client/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.5.7/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.5.7/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/soap.py` & `pibble-0.5.7/pibble/api/client/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/webservice/wrapper.py` & `pibble-0.5.7/pibble/api/client/webservice/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/client/wrapper.py` & `pibble-0.5.7/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/configuration.py` & `pibble-0.5.7/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/exceptions.py` & `pibble-0.5.7/pibble/api/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,14 +124,24 @@
     An exception indicating the client is making too many requests.
     """
 
     def __init__(self, msg: str = "Too many requests."):
         super(TooManyRequestsError, self).__init__(msg)
 
 
+class StateConflictError(Exception):
+    """
+    An exception indicating something about the users request cannot
+    be fulfilled because it violates domain logic.
+    """
+
+    def __init__(self, msg: str = "The request cannot be fulfilled."):
+        super(StateConflictError, self).__init__(msg)
+
+
 class UnknownError(Exception):
     """
     An exception indicating somethign went wrong that was unexpected.
 
     :param msg str: The message to send. Defaults to "An unknown error occurred."
     """
```

### Comparing `pibble-0.5.6/pibble/api/helpers/apachethrift.py` & `pibble-0.5.7/pibble/api/helpers/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/helpers/authentication.py` & `pibble-0.5.7/pibble/api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/helpers/googlerpc.py` & `pibble-0.5.7/pibble/api/helpers/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/helpers/store.py` & `pibble-0.5.7/pibble/api/helpers/store.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/helpers/wrappers.py` & `pibble-0.5.7/pibble/api/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/meta/base.py` & `pibble-0.5.7/pibble/api/meta/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/meta/helpers.py` & `pibble-0.5.7/pibble/api/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/apachethrift/base.py` & `pibble-0.5.7/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.5.7/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/database/orm.py` & `pibble-0.5.7/pibble/api/middleware/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.5.7/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/googlerpc/base.py` & `pibble-0.5.7/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.5.7/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/screening.py` & `pibble-0.5.7/pibble/api/middleware/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.5.7/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.5.7/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.5.7/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.5.7/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.5.7/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/base.py` & `pibble-0.5.7/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/limit.py` & `pibble-0.5.7/pibble/api/middleware/webservice/limit.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/middleware/webservice/screening.py` & `pibble-0.5.7/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/protocol/apachethrift.py` & `pibble-0.5.7/pibble/api/protocol/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/apachethrift.py` & `pibble-0.5.7/pibble/api/server/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/base.py` & `pibble-0.5.7/pibble/api/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/file/ftp.py` & `pibble-0.5.7/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/file/sftp.py` & `pibble-0.5.7/pibble/api/server/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/googlerpc.py` & `pibble-0.5.7/pibble/api/server/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/apachethrift.py` & `pibble-0.5.7/pibble/api/server/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/awslambda.py` & `pibble-0.5.7/pibble/api/server/webservice/awslambda.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/base.py` & `pibble-0.5.7/pibble/api/server/webservice/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     BadRequestError,
     BadResponseError,
     NotFoundError,
     UnsupportedMethodError,
     AuthenticationError,
     PermissionError,
     ConfigurationError,
+    StateConflictError,
     TooManyRequestsError,
 )
 
 from pibble.api.helpers.wrappers import (
     RequestWrapper,
     ResponseWrapper,
 )
@@ -78,14 +79,15 @@
 
     EXCEPTION_CODES = {
         BadRequestError: 400,
         AuthenticationError: 401,
         PermissionError: 403,
         NotFoundError: 404,
         UnsupportedMethodError: 405,
+        StateConflictError: 409,
         TooManyRequestsError: 429,
         NotImplementedError: 501,
     }
 
     class_handlers: List[WebServiceAPIHandlerRegistry]
 
     def __init__(self) -> None:
@@ -371,14 +373,15 @@
                 PermissionError,
                 AuthenticationError,
                 NotFoundError,
                 UnsupportedMethodError,
                 NotImplementedError,
                 BadRequestError,
                 TooManyRequestsError,
+                StateConflictError,
             ) as ex:
                 logger.warning(
                     "Received exception in handler: {0}({1})".format(
                         type(ex).__name__, str(ex)
                     )
                 )
                 logger.debug(format_exc())
@@ -459,14 +462,15 @@
             run_driver: Optional[Callable] = None
 
             if driver == "cherrypy":
                 from pibble.api.server.webservice.drivers.driver_cherrypy import (
                     run_cherrypy,
                 )
 
+                destroy_on_stop = False
                 run_driver = run_cherrypy
             elif driver == "werkzeug":
                 from pibble.api.server.webservice.drivers.driver_werkzeug import (
                     run_werkzeug,
                 )
 
                 run_driver = run_werkzeug
@@ -477,15 +481,15 @@
 
                 run_driver = run_gunicorn
 
             if run_driver is None:
                 raise ConfigurationError(
                     "Server driver {0} not supported.".format(driver)
                 )
-            run_driver(self.wsgi(), host, port, secure, cert, key, workers)
+            run_driver(self, host, port, secure, cert, key, workers)
         except KeyError as ex:
             raise ConfigurationError(str(ex))
         finally:
             if destroy_on_stop:
                 self.destroy()
```

### Comparing `pibble-0.5.6/pibble/api/server/webservice/drivers/driver_cherrypy.py` & `pibble-0.5.7/pibble/api/server/webservice/drivers/driver_cherrypy.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import cherrypy
 from typing import Optional, TYPE_CHECKING
 from multiprocessing import cpu_count
 from pibble.util.log import logger
 
 if TYPE_CHECKING:
-    from _typeshed.wsgi import WSGIApplication
+    from pibble.api.server.webservice.base import WebServiceAPIServerBase
 
 
 def run_cherrypy(
-    application: WSGIApplication,
+    application: WebServiceAPIServerBase,
     host: str,
     port: int,
     secure: bool = False,
     cert: Optional[str] = None,
     key: Optional[str] = None,
     workers: Optional[int] = None,
 ) -> None:
     """
     Runs the cherrypy engine synchronously.
     """
-    cherrypy.tree.graft(application, "/")
+    cherrypy.tree.graft(application.wsgi(), "/")
     cherrypy.server.unsubscribe()
     cherrypy.config.update(
         {"global": {"environment": "production"}}
     )  # Disable reloading
 
     server = cherrypy._cpserver.Server()
     server.socket_host = host
@@ -41,9 +41,10 @@
         )
     elif secure:
         logger.warning(
             "No SSL keyfile/certfile specific, but SSL enabled. If this server is being proxied through another service that provides SSL context this is okay, otherwise connections will fail."
         )
 
     server.subscribe()
+    cherrypy.engine.subscribe("exit", lambda: application.destroy())
     cherrypy.engine.start()
     cherrypy.engine.block()
```

### Comparing `pibble-0.5.6/pibble/api/server/webservice/drivers/driver_gunicorn.py` & `pibble-0.5.7/pibble/api/server/webservice/drivers/driver_gunicorn.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from typing import Optional, TYPE_CHECKING
 from multiprocessing import cpu_count
 from gunicorn.app.base import Application
 from pibble.util.log import logger
 
 if TYPE_CHECKING:
-    from _typeshed.wsgi import WSGIApplication
+    from pibble.api.server.webservice.base import WebServiceAPIServerBase
+    from typeshed._wsgi import WSGIApplication
 
 
 class PibbleGunicornApplication(Application):  # type: ignore
     """
     A simple extension of the gunicorn application base to work with the webservice.
     """
 
@@ -36,15 +37,15 @@
             self.cfg.set(key.lower(), config[key])
 
     def load(self) -> WSGIApplication:
         return self.application
 
 
 def run_gunicorn(
-    application: WSGIApplication,
+    application: WebServiceAPIServerBase,
     host: str,
     port: int,
     secure: bool = False,
     cert: Optional[str] = None,
     key: Optional[str] = None,
     workers: Optional[int] = None,
 ) -> None:
@@ -64,9 +65,9 @@
             f"Loading SSL certificate chain from keyfile {key:s}, certfile {cert:s}"
         )
     elif secure:
         logger.warning(
             "No SSL keyfile/certfile specific, but SSL enabled. If this server is being proxied through another service that provides SSL context this is okay, otherwise connections will fail."
         )
 
-    application = PibbleGunicornApplication(application, options)
+    application = PibbleGunicornApplication(application.wsgi(), options)
     application.run()
```

### Comparing `pibble-0.5.6/pibble/api/server/webservice/drivers/driver_werkzeug.py` & `pibble-0.5.7/pibble/api/server/webservice/drivers/driver_werkzeug.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import ssl
 from typing import Optional, TYPE_CHECKING
 from werkzeug.serving import run_simple
 from pibble.util.log import logger
 
 if TYPE_CHECKING:
-    from _typeshed.wsgi import WSGIApplication
+    from pibble.api.server.webservice.base import WebServiceAPIServerBase
 
 
 def run_werkzeug(
-    application: WSGIApplication,
+    application: WebServiceAPIServerBase,
     host: str,
     port: int,
     secure: bool = False,
     cert: Optional[str] = None,
     key: Optional[str] = None,
     workers: Optional[int] = None,
 ) -> None:
@@ -27,8 +27,8 @@
             f"Loading SSL certificate chain from keyfile {key:s}, certfile {cert:s}"
         )
         ssl_context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
     elif secure:
         logger.warning(
             "No SSL keyfile/certfile specific, but SSL enabled. If this server is being proxied through another service that provides SSL context this is okay, otherwise connections will fail."
         )
-    run_simple(host, port, application, ssl_context=ssl_context)
+    run_simple(host, port, application.wsgi(), ssl_context=ssl_context)
```

### Comparing `pibble-0.5.6/pibble/api/server/webservice/handler.py` & `pibble-0.5.7/pibble/api/server/webservice/handler.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/jsonapi.py` & `pibble-0.5.7/pibble/api/server/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/orm.py` & `pibble-0.5.7/pibble/api/server/webservice/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/rpc/base.py` & `pibble-0.5.7/pibble/api/server/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.5.7/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.5.7/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/soap.py` & `pibble-0.5.7/pibble/api/server/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/template/__init__.py` & `pibble-0.5.7/pibble/api/server/webservice/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/template/extensions.py` & `pibble-0.5.7/pibble/api/server/webservice/template/extensions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/api/server/webservice/template/loader.py` & `pibble-0.5.7/pibble/api/server/webservice/template/loader.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/database/dedupe.py` & `pibble-0.5.7/pibble/database/dedupe.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/database/engine.py` & `pibble-0.5.7/pibble/database/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         Builds the actual SQLAlchemy engine.
         """
         conn_string = URL(**{**self.connection_params, **{"database": database_name}})
         logger.info(
             "Creating SQLAlchemy engine using connection string {0}".format(conn_string)
         )
         self.engines[database_name] = sqlalchemy.create_engine(
-            conn_string, 
-            pool_reset_on_return=None, 
+            conn_string,
+            pool_reset_on_return=None,
         )
         if "pyodbc" in self.connection_params["drivername"]:
             if pyodbc is None:
                 raise OSError(
                     "Failed to import PyODBC. This server/container likely needs ODBC configuration."
                 )
```

### Comparing `pibble-0.5.6/pibble/database/orm.py` & `pibble-0.5.7/pibble/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/database/util.py` & `pibble-0.5.7/pibble/database/util.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/cms/database/__init__.py` & `pibble-0.5.7/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/cms/database/interface.py` & `pibble-0.5.7/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/cms/database/menu.py` & `pibble-0.5.7/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/cms/database/view.py` & `pibble-0.5.7/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/cms/middleware.py` & `pibble-0.5.7/pibble/ext/cms/middleware.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/cms/server/base.py` & `pibble-0.5.7/pibble/ext/cms/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/cms/server/extension.py` & `pibble-0.5.7/pibble/ext/cms/server/extension.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/dam/database/files.py` & `pibble-0.5.7/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/rest/server/base.py` & `pibble-0.5.7/pibble/ext/rest/server/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import re
+import logging
 
 from sqlalchemy import and_, or_, not_
 from sqlalchemy.orm.query import Query
 from sqlalchemy.orm.attributes import QueryableAttribute
 from sqlalchemy.sql.elements import ColumnElement
 
 from pibble.api.exceptions import (
@@ -226,16 +227,16 @@
 
             hidden_relationships = getattr(orm_object, "__hidden_relationships__", [])
             if hidden_relationships is None:
                 hidden_relationships = []
 
             filter_kwargs = {}
             for key in kwargs:
-                if kwargs[key]:
-                    filter_kwargs[key] = kwargs[key]
+                if kwargs[key] is not None and kwargs[key] != "":
+                    filter_kwargs[key] = str(kwargs[key])
 
             input_dict = {}
             if method in ["POST", "PUT", "PATCH"]:
                 input_dict = request.parsed
 
             for key in input_dict:
                 if key in hidden_columns:
@@ -360,15 +361,15 @@
         else:
             root = self.configuration.get("rest.root", "/rest")
             scopes = self.configuration.get("rest.scopes", [])
             if not scopes:
                 logger.error(
                     "REST server scope configuration missing. No handlers will be registered."
                 )
-
+            logger.debug("REST server adding {0} scoped handlers".format(len(scopes)))
             for scope in scopes:
                 handler_classname = scope["class"]
                 handler_scope = scope["scope"]
                 if isinstance(handler_classname, type):
                     handler_classname = handler_classname.__name__
                 handler_root = scope.get("root", handler_classname)
                 handler_parent = scope.get("parent", [])
@@ -381,14 +382,20 @@
 
                 handler_regex = f"^{root:s}/{handler_root:s}"
 
                 for handler_parent_part in handler_parent:
                     handler_regex += f"/(?P<{handler_parent_part:s}>[a-zA-Z0-9_\-]+)"
                 handler_regex += f"(/(?P<{handler_scope:s}>[a-zA-Z0-9_\-]+))?$"
 
+                if logger.isEnabledFor(logging.DEBUG):
+                    handler_parent_string = ",".join(handler_parent)
+                    logger.debug(
+                        f"REST server registering scoped handler for class {handler_classname}, handler root '{handler_root}', parent(s) '{handler_parent_string}', scope(s) '{handler_scope}', regex {handler_regex}"
+                    )
+
                 self.bind_rest_handler(
                     handler_classname,
                     handler_methods,
                     handler_root,
                     handler_parent,
                     handler_scope,
                     handler_regex,
```

### Comparing `pibble-0.5.6/pibble/ext/rest/server/user.py` & `pibble-0.5.7/pibble/ext/rest/server/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,14 +177,20 @@
                 if not permission:
                     raise PermissionError(
                         "User {0} is not authorized to {1} on {2}.".format(
                             request.token.user.email, action, handler_classname
                         )
                     )
 
+            scope_user_fields = scope.get("user", {})
+            for field in scope_user_fields:
+                kwargs[scope_user_fields[field]] = getattr(
+                    request.token.user, field, None
+                )
+
             handler_result = handler(self, request, response, **kwargs)
 
             if action:
                 after = scope.get("actions", {}).get(action, {})
                 if isinstance(handler_result, list):
                     results = handler_result
                 else:
```

### Comparing `pibble-0.5.6/pibble/ext/session/database/session.py` & `pibble-0.5.7/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/session/server/base.py` & `pibble-0.5.7/pibble/ext/session/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/user/client/base.py` & `pibble-0.5.7/pibble/ext/user/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/user/database/__init__.py` & `pibble-0.5.7/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/user/database/authentication.py` & `pibble-0.5.7/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/user/database/notification.py` & `pibble-0.5.7/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/user/database/permission.py` & `pibble-0.5.7/pibble/ext/user/database/permission.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/user/database/user.py` & `pibble-0.5.7/pibble/ext/user/database/user.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/ext/user/server/base.py` & `pibble-0.5.7/pibble/ext/user/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/hooks/aws.py` & `pibble-0.5.7/pibble/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/media/thumbnail.py` & `pibble-0.5.7/pibble/media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/resources/retriever.py` & `pibble-0.5.7/pibble/resources/retriever.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/scripts/importcheck.py` & `pibble-0.5.7/pibble/scripts/importcheck.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/scripts/templatefiles.py` & `pibble-0.5.7/pibble/scripts/templatefiles.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/setup.py` & `pibble-0.5.7/pibble/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "6"
+version_patch = "7"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

### Comparing `pibble-0.5.6/pibble/util/encryption.py` & `pibble-0.5.7/pibble/util/encryption.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/util/files.py` & `pibble-0.5.7/pibble/util/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/util/helpers.py` & `pibble-0.5.7/pibble/util/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/util/imaging.py` & `pibble-0.5.7/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/util/log.py` & `pibble-0.5.7/pibble/util/log.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     FileHandler,
     Formatter,
     LogRecord,
     Logger,
     getLogger,
     DEBUG,
 )
-from typing import Any
+from typing import Any, List
 from logging.handlers import SysLogHandler
 from termcolor import colored
 
 from pibble.api.configuration import APIConfiguration
 
 __all__ = [
     "logger",
@@ -67,25 +67,25 @@
     A context manager that will remove logger handlers, then set the handler and level for the root
     logger to specified parameters.
 
     Will set logger variables back to their predefined values on exit.
 
     :param handler: The handler to set the root logger to.
     :param level: The log level.
-    :param others: Any other loggers to create contexts for.
+    :param silenced: A list of any loggers to silence.
     """
 
     DEFAULT_FORMAT = (
         "%(asctime)s [%(name)s] %(levelname)s (%(filename)s:%(lineno)s) %(message)s"
     )
 
-    def __init__(self, handler: Handler, level: int, *others: str):
+    def __init__(self, handler: Handler, level: int, silenced: List[str] = []):
         self.level = level
         self.handler = handler
-        self.others = others
+        self.silenced = silenced
 
     def __enter__(self) -> None:
         self.start()
 
     def __exit__(self, *args: Any) -> None:
         self.stop()
 
@@ -103,15 +103,18 @@
         getLogger().setLevel(self.level)
 
         for loggerName in Logger.manager.loggerDict:
             self.handlers[loggerName] = getLogger(loggerName).handlers
             self.levels[loggerName] = getLogger(loggerName).level
 
             getLogger(loggerName).handlers = []
-            getLogger(loggerName).setLevel(self.level)
+            if loggerName in self.silenced:
+                getLogger(loggerName).setLevel(99)
+            else:
+                getLogger(loggerName).setLevel(self.level)
 
         getLogger().addHandler(self.handler)
 
         def print_http_client(*args: Any, **kwargs: Any) -> None:
             for line in (" ".join(args)).splitlines():
                 getLogger("http.client").log(DEBUG, line)
 
@@ -133,47 +136,49 @@
 class LevelUnifiedLoggingContext(UnifiedLoggingContext):
     """
     An extension of the UnifiedLoggingContext for use in debugging.
 
     :param level int: The log level.
     """
 
-    def __init__(self, level: int) -> None:
+    def __init__(self, level: int, silenced: List[str] = []) -> None:
         self.level = level
         self.handler = StreamHandler(sys.stdout)
         self.handler.setFormatter(ColoredLoggingFormatter(self.DEFAULT_FORMAT))
+        self.silenced = silenced
 
 
 class DebugUnifiedLoggingContext(LevelUnifiedLoggingContext):
     """
     A shortand for LevelUnifiedLoggingContext(DEBUG)
     """
 
-    def __init__(self) -> None:
-        super(DebugUnifiedLoggingContext, self).__init__(DEBUG)
+    def __init__(self, silenced: List[str] = []) -> None:
+        super(DebugUnifiedLoggingContext, self).__init__(DEBUG, silenced)
 
 
 class ConfigurationLoggingContext(UnifiedLoggingContext):
     """
     An extension of the UnifiedLoggingContext that reads an :class:`pibble.api.configuration.APIConfiguration` object.
     """
 
     def __init__(self, configuration: APIConfiguration, prefix: str = "logging."):
         self.level = configuration.get(f"{prefix}level", "CRITICAL").upper()
+        self.silenced = configuration.get(f"{prefix}silenced", [])
         handler_class = configuration.get(f"{prefix}handler", "stream")
         if handler_class == "stream":
             stream = configuration.get(f"{prefix}stream", "stderr")
             if isinstance(stream, str):
                 self.handler = StreamHandler(
                     sys.stdout if stream == "stdout" else sys.stderr
                 )
             else:
                 self.handler = StreamHandler(stream)
         elif handler_class == "file":
-            self.handler = FileHandler(configuration["file"])
+            self.handler = FileHandler(configuration[f"{prefix}file"])
         elif handler_class == "syslog":
             self.handler = SysLogHandler(
                 address=(
                     configuration["host"],
                     int(configuration["port"]),
                 ),
                 facility=configuration["facility"],
```

### Comparing `pibble-0.5.6/pibble/util/numeric.py` & `pibble-0.5.7/pibble/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/util/strings.py` & `pibble-0.5.7/pibble/util/strings.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble/web/scraper.py` & `pibble-0.5.7/pibble/web/scraper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble.egg-info/PKG-INFO` & `pibble-0.5.7/pibble.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.6
+Version: 0.5.7
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.6/pibble.egg-info/SOURCES.txt` & `pibble-0.5.7/pibble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/pibble.egg-info/requires.txt` & `pibble-0.5.7/pibble.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.6/setup.py` & `pibble-0.5.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
 version_minor = "5"
-version_patch = "6"
+version_patch = "7"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

