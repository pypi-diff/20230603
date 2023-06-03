# Comparing `tmp/polyglot_piranha-0.3.7.tar.gz` & `tmp/polyglot_piranha-0.3.8-cp38-cp38-macosx_10_16_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

