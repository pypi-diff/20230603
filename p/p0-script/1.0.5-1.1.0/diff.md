# Comparing `tmp/p0-script-1.0.5.tar.gz` & `tmp/p0_script-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\thiba\dev\code\projects\p0_script\dist\.tmp-huzrwqqt\p0-script-1.0.5.tar", last modified: Sat Jun  3 04:59:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

