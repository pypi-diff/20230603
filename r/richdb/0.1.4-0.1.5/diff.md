# Comparing `tmp/richdb-0.1.4.tar.gz` & `tmp/richdb-0.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richdb-0.1.4.tar", last modified: Sat Oct 29 19:59:58 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

