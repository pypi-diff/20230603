# Comparing `tmp/rapidfuzz-3.0.0.tar.gz` & `tmp/rapidfuzz-3.1.0-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-3.0.0.tar", last modified: Mon Apr 17 00:36:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

