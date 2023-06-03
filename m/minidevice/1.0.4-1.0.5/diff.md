# Comparing `tmp/minidevice-1.0.4.tar.gz` & `tmp/minidevice-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.4.tar", last modified: Thu Jun  1 04:33:27 2023, max compression
+gzip compressed data, was "minidevice-1.0.5.tar", last modified: Sat Jun  3 06:33:32 2023, max compression
```

## Comparing `minidevice-1.0.4.tar` & `minidevice-1.0.5.tar`

### file list

```diff
@@ -1,192 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.845041 minidevice-1.0.4/
--rw-rw-rw-   0        0        0     1394 2023-06-01 04:33:27.844064 minidevice-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2023-06-01 04:04:50.000000 minidevice-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.723023 minidevice-1.0.4/minidevice/
--rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.4/minidevice/__init__.py
--rw-rw-rw-   0        0        0     2040 2023-06-01 01:14:31.000000 minidevice-1.0.4/minidevice/adb.py
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.739750 minidevice-1.0.4/minidevice/bin/
--rw-rw-rw-   0        0        0    97792 2023-03-12 01:13:21.000000 minidevice-1.0.4/minidevice/bin/AdbWinApi.dll
--rw-rw-rw-   0        0        0    62976 2023-03-12 01:13:21.000000 minidevice-1.0.4/minidevice/bin/AdbWinUsbApi.dll
--rwxrwxrwx   0        0        0  6021632 2023-03-12 01:13:21.000000 minidevice-1.0.4/minidevice/bin/adb.exe
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.705831 minidevice-1.0.4/minidevice/bin/minicap/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.704856 minidevice-1.0.4/minidevice/bin/minicap/jni/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.659726 minidevice-1.0.4/minidevice/bin/minicap/jni/android-10/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.747592 minidevice-1.0.4/minidevice/bin/minicap/jni/android-10/armeabi-v7a/
--rw-rw-rw-   0        0        0     9688 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-10/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.660703 minidevice-1.0.4/minidevice/bin/minicap/jni/android-14/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.749987 minidevice-1.0.4/minidevice/bin/minicap/jni/android-14/armeabi-v7a/
--rw-rw-rw-   0        0        0     5700 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-14/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.750965 minidevice-1.0.4/minidevice/bin/minicap/jni/android-14/x86/
--rw-rw-rw-   0        0        0    11385 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-14/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.662654 minidevice-1.0.4/minidevice/bin/minicap/jni/android-15/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.751940 minidevice-1.0.4/minidevice/bin/minicap/jni/android-15/armeabi-v7a/
--rw-rw-rw-   0        0        0     5700 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-15/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.753894 minidevice-1.0.4/minidevice/bin/minicap/jni/android-15/x86/
--rw-rw-rw-   0        0        0    11385 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-15/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.663631 minidevice-1.0.4/minidevice/bin/minicap/jni/android-16/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.754869 minidevice-1.0.4/minidevice/bin/minicap/jni/android-16/armeabi-v7a/
--rw-rw-rw-   0        0        0     9420 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-16/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.755845 minidevice-1.0.4/minidevice/bin/minicap/jni/android-16/x86/
--rw-rw-rw-   0        0        0    11929 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-16/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.665583 minidevice-1.0.4/minidevice/bin/minicap/jni/android-17/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.757827 minidevice-1.0.4/minidevice/bin/minicap/jni/android-17/armeabi-v7a/
--rw-rw-rw-   0        0        0    13472 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-17/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.758823 minidevice-1.0.4/minidevice/bin/minicap/jni/android-17/x86/
--rw-rw-rw-   0        0        0    23907 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-17/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.666560 minidevice-1.0.4/minidevice/bin/minicap/jni/android-18/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.759802 minidevice-1.0.4/minidevice/bin/minicap/jni/android-18/armeabi-v7a/
--rw-rw-rw-   0        0        0    13492 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-18/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.761755 minidevice-1.0.4/minidevice/bin/minicap/jni/android-18/x86/
--rw-rw-rw-   0        0        0    23491 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-18/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.668563 minidevice-1.0.4/minidevice/bin/minicap/jni/android-19/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.762730 minidevice-1.0.4/minidevice/bin/minicap/jni/android-19/armeabi-v7a/
--rw-rw-rw-   0        0        0    13488 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-19/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.763709 minidevice-1.0.4/minidevice/bin/minicap/jni/android-19/x86/
--rw-rw-rw-   0        0        0    23725 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-19/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.671666 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.764683 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/arm64-v8a/
--rw-rw-rw-   0        0        0    22000 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.766634 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/armeabi-v7a/
--rw-rw-rw-   0        0        0    13492 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.767641 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/x86/
--rw-rw-rw-   0        0        0    21676 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.768649 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/x86_64/
--rw-rw-rw-   0        0        0    26328 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-21/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.674592 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.769629 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/arm64-v8a/
--rw-rw-rw-   0        0        0    22000 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.771582 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/armeabi-v7a/
--rw-rw-rw-   0        0        0    13492 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.772557 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/x86/
--rw-rw-rw-   0        0        0    21676 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.773534 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/x86_64/
--rw-rw-rw-   0        0        0    26328 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-22/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.677553 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.774509 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/arm64-v8a/
--rw-rw-rw-   0        0        0    22328 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.775486 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/armeabi-v7a/
--rw-rw-rw-   0        0        0    22128 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.776462 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/x86/
--rw-rw-rw-   0        0        0    21932 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.778463 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/x86_64/
--rw-rw-rw-   0        0        0    26688 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-23/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.679793 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.779615 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/arm64-v8a/
--rw-rw-rw-   0        0        0    22576 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.780590 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/armeabi-v7a/
--rw-rw-rw-   0        0        0    22100 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.781567 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/x86/
--rw-rw-rw-   0        0        0    21944 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.783519 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/x86_64/
--rw-rw-rw-   0        0        0    26672 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-24/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.683697 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.784495 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/arm64-v8a/
--rw-rw-rw-   0        0        0    22576 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.785472 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/armeabi-v7a/
--rw-rw-rw-   0        0        0    22100 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.787452 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/x86/
--rw-rw-rw-   0        0        0    21944 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.788449 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/x86_64/
--rw-rw-rw-   0        0        0    26672 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-25/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.686624 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.789492 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/arm64-v8a/
--rw-rw-rw-   0        0        0    23592 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.790473 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/armeabi-v7a/
--rw-rw-rw-   0        0        0    24760 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.791448 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/x86/
--rw-rw-rw-   0        0        0    22588 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.793400 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/x86_64/
--rw-rw-rw-   0        0        0    27280 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-26/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.689599 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.794376 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/arm64-v8a/
--rw-rw-rw-   0        0        0    23592 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.795353 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/armeabi-v7a/
--rw-rw-rw-   0        0        0    24784 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.796329 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/x86/
--rw-rw-rw-   0        0        0    22564 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.797837 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/x86_64/
--rw-rw-rw-   0        0        0    27280 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-27/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.692526 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.799302 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/arm64-v8a/
--rw-rw-rw-   0        0        0    68736 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.800282 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/armeabi-v7a/
--rw-rw-rw-   0        0        0    28900 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.801258 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/x86/
--rw-rw-rw-   0        0        0    23032 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.802767 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/x86_64/
--rw-rw-rw-   0        0        0    27776 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-28/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.695456 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.803762 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/arm64-v8a/
--rw-rw-rw-   0        0        0    29088 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.805714 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/armeabi-v7a/
--rw-rw-rw-   0        0        0    28888 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.806689 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/x86/
--rw-rw-rw-   0        0        0    31868 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.807696 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/x86_64/
--rw-rw-rw-   0        0        0    37272 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-29/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.698437 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.808690 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/arm64-v8a/
--rw-rw-rw-   0        0        0    25136 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.810061 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/armeabi-v7a/
--rw-rw-rw-   0        0        0    21360 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.811041 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/x86/
--rw-rw-rw-   0        0        0    21272 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.812995 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/x86_64/
--rw-rw-rw-   0        0        0    23448 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-30/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.701366 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.813969 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/arm64-v8a/
--rw-rw-rw-   0        0        0    24488 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.815922 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/armeabi-v7a/
--rw-rw-rw-   0        0        0    20956 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.815922 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/x86/
--rw-rw-rw-   0        0        0    20532 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.817431 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/x86_64/
--rw-rw-rw-   0        0        0    20136 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-31/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.704856 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.818432 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/arm64-v8a/
--rw-rw-rw-   0        0        0    24488 2023-04-15 05:48:30.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/arm64-v8a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.819745 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/armeabi-v7a/
--rw-rw-rw-   0        0        0    20956 2023-04-15 05:48:30.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.821695 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/x86/
--rw-rw-rw-   0        0        0    20532 2023-04-15 05:48:30.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/x86/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.822672 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/x86_64/
--rw-rw-rw-   0        0        0   176193 2023-05-31 05:40:13.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-32/x86_64/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.705831 minidevice-1.0.4/minidevice/bin/minicap/jni/android-9/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.824625 minidevice-1.0.4/minidevice/bin/minicap/jni/android-9/armeabi-v7a/
--rw-rw-rw-   0        0        0     9688 2023-04-15 03:42:07.000000 minidevice-1.0.4/minidevice/bin/minicap/jni/android-9/armeabi-v7a/minicap.so
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.707812 minidevice-1.0.4/minidevice/bin/minicap/libs/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.825599 minidevice-1.0.4/minidevice/bin/minicap/libs/arm64-v8a/
--rw-rw-rw-   0        0        0   537552 2023-04-15 05:39:49.000000 minidevice-1.0.4/minidevice/bin/minicap/libs/arm64-v8a/minicap
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.827583 minidevice-1.0.4/minidevice/bin/minicap/libs/armeabi-v7a/
--rw-rw-rw-   0        0        0   298356 2023-04-15 05:39:37.000000 minidevice-1.0.4/minidevice/bin/minicap/libs/armeabi-v7a/minicap
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.828581 minidevice-1.0.4/minidevice/bin/minicap/libs/x86/
--rw-rw-rw-   0        0        0   651488 2023-04-15 05:40:06.000000 minidevice-1.0.4/minidevice/bin/minicap/libs/x86/minicap
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.830863 minidevice-1.0.4/minidevice/bin/minicap/libs/x86_64/
--rw-rw-rw-   0        0        0   665096 2023-04-15 05:40:18.000000 minidevice-1.0.4/minidevice/bin/minicap/libs/x86_64/minicap
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.709279 minidevice-1.0.4/minidevice/bin/minitouch/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.711236 minidevice-1.0.4/minidevice/bin/minitouch/libs/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.833841 minidevice-1.0.4/minidevice/bin/minitouch/libs/arm64-v8a/
--rw-rw-rw-   0        0        0    25528 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/arm64-v8a/minitouch
--rw-rw-rw-   0        0        0    25528 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/arm64-v8a/minitouch-nopie
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.836718 minidevice-1.0.4/minidevice/bin/minitouch/libs/armeabi-v7a/
--rw-rw-rw-   0        0        0    17272 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/armeabi-v7a/minitouch
--rw-rw-rw-   0        0        0    17272 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/armeabi-v7a/minitouch-nopie
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.838719 minidevice-1.0.4/minidevice/bin/minitouch/libs/x86/
--rw-rw-rw-   0        0        0    25684 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/x86/minitouch
--rw-rw-rw-   0        0        0    25684 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/x86/minitouch-nopie
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.842113 minidevice-1.0.4/minidevice/bin/minitouch/libs/x86_64/
--rw-rw-rw-   0        0        0    27464 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/x86_64/minitouch
--rw-rw-rw-   0        0        0    27464 2023-04-27 11:32:08.000000 minidevice-1.0.4/minidevice/bin/minitouch/libs/x86_64/minitouch-nopie
--rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.4/minidevice/config.py
--rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.4/minidevice/device.py
--rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.4/minidevice/minicap.py
--rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.4/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.4/minidevice/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 04:33:27.735491 minidevice-1.0.4/minidevice.egg-info/
--rw-rw-rw-   0        0        0     1394 2023-06-01 04:33:27.000000 minidevice-1.0.4/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4560 2023-06-01 04:33:27.000000 minidevice-1.0.4/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 04:33:27.000000 minidevice-1.0.4/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-01 04:33:27.000000 minidevice-1.0.4/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 04:33:27.000000 minidevice-1.0.4/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 04:33:27.845041 minidevice-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      899 2023-06-01 04:33:03.000000 minidevice-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.636500 minidevice-1.0.5/
+-rw-rw-rw-   0        0        0     1373 2023-06-03 06:33:32.633518 minidevice-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2023-06-01 04:04:50.000000 minidevice-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.579619 minidevice-1.0.5/minidevice/
+-rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.5/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-06-02 05:28:24.000000 minidevice-1.0.5/minidevice/adb.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.614520 minidevice-1.0.5/minidevice/bin/
+-rw-rw-rw-   0        0        0    97792 2023-03-12 01:13:21.000000 minidevice-1.0.5/minidevice/bin/AdbWinApi.dll
+-rw-rw-rw-   0        0        0    62976 2023-03-12 01:13:21.000000 minidevice-1.0.5/minidevice/bin/AdbWinUsbApi.dll
+-rwxrwxrwx   0        0        0  6021632 2023-03-12 01:13:21.000000 minidevice-1.0.5/minidevice/bin/adb.exe
+-rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.5/minidevice/config.py
+-rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.5/minidevice/device.py
+-rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.5/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.5/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.5/minidevice/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-03 06:33:32.603057 minidevice-1.0.5/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1373 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 06:33:32.000000 minidevice-1.0.5/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 06:33:32.636995 minidevice-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-06-03 06:32:42.000000 minidevice-1.0.5/setup.py
```

### Comparing `minidevice-1.0.4/PKG-INFO` & `minidevice-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.4
+Version: 1.0.5
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # minidevice 
 
 ## CaptureScreen类
 初始化时会判断minicap在该设备是否可用 不可用时则抛出异常
@@ -48,8 +47,7 @@
     - `adb.exe`
     - `__init__.py`
     - `adb.py`
     - `AdbWinApi.dll`
     - `AdbWinUsbApi.dll`
     - `utils.py`
 项目结构
-
```

### Comparing `minidevice-1.0.4/README.md` & `minidevice-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.4/minidevice/bin/AdbWinApi.dll` & `minidevice-1.0.5/minidevice/bin/AdbWinApi.dll`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.4/minidevice/bin/AdbWinUsbApi.dll` & `minidevice-1.0.5/minidevice/bin/AdbWinUsbApi.dll`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.4/minidevice/bin/adb.exe` & `minidevice-1.0.5/minidevice/bin/adb.exe`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.4/minidevice/device.py` & `minidevice-1.0.5/minidevice/device.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.4/minidevice/minicap.py` & `minidevice-1.0.5/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.4/minidevice.egg-info/PKG-INFO` & `minidevice-1.0.5/minidevice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.4
+Version: 1.0.5
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # minidevice 
 
 ## CaptureScreen类
 初始化时会判断minicap在该设备是否可用 不可用时则抛出异常
@@ -48,8 +47,7 @@
     - `adb.exe`
     - `__init__.py`
     - `adb.py`
     - `AdbWinApi.dll`
     - `AdbWinUsbApi.dll`
     - `utils.py`
 项目结构
-
```

### Comparing `minidevice-1.0.4/setup.py` & `minidevice-1.0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.0.4',
+      version='1.0.5',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku',
       license='MIT',
@@ -17,13 +17,14 @@
       packages=find_packages(),
       package_data={
           "minidevice": [
               "bin/*",
           ]
       },
       include_package_data=True,
-      install_requires=['opencv-python>=4.7.0.72',
+      install_requires=['requests>=2.31.0',
+                        'opencv-python>=4.7.0.72',
                         'uiautomator2>=2.16.23',
                         'pyminitouch>=0.3.3',
                         'urllib3'],
       python_requires='>=3'
       )
```

