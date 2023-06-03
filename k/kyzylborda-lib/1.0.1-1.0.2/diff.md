# Comparing `tmp/kyzylborda_lib-1.0.1.tar.gz` & `tmp/kyzylborda_lib-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyzylborda_lib-1.0.1.tar", last modified: Fri Jan 13 18:38:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

