# Comparing `tmp/regex-2023.5.5.tar.gz` & `tmp/regex-2023.6.3-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2023.5.5.tar", last modified: Wed May  3 17:28:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

