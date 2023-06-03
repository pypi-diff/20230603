# Comparing `tmp/tamp-1.0.3.tar.gz` & `tmp/tamp-1.1.0-cp39-cp39-macosx_12_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.0.3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

