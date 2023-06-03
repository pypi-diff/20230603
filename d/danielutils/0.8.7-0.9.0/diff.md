# Comparing `tmp/danielutils-0.8.7.tar.gz` & `tmp/danielutils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.8.7.tar", last modified: Fri Jun  2 10:05:08 2023, max compression
+gzip compressed data, was "danielutils-0.9.0.tar", last modified: Sat Jun  3 13:04:23 2023, max compression
```

## Comparing `danielutils-0.8.7.tar` & `danielutils-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.395799 danielutils-0.8.7/
--rw-rw-rw-   0        0        0     1967 2023-06-02 10:05:08.395799 danielutils-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2023-06-02 10:05:07.000000 danielutils-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.345655 danielutils-0.8.7/danielutils/
--rw-rw-rw-   0        0        0     4362 2023-06-02 08:57:30.000000 danielutils-0.8.7/danielutils/Aliases.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.354355 danielutils-0.8.7/danielutils/Classes/
--rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.8.7/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     1144 2023-06-01 23:36:28.000000 danielutils-0.8.7/danielutils/Classes/Counter.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.359391 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/
--rw-rw-rw-   0        0        0       96 2023-06-02 09:15:33.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/__init__.py
--rw-rw-rw-   0        0        0      477 2023-05-01 13:03:04.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tbase.py
--rw-rw-rw-   0        0        0     2042 2023-06-01 21:38:07.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tdict.py
--rw-rw-rw-   0        0        0     1824 2023-06-01 23:26:15.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tlist.py
--rw-rw-rw-   0        0        0      818 2023-05-01 13:01:21.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tset.py
--rw-rw-rw-   0        0        0      137 2023-06-02 09:13:53.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/ttuple.py
--rw-rw-rw-   0        0        0      126 2023-05-01 13:01:32.000000 danielutils-0.8.7/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0     1047 2023-06-01 21:36:49.000000 danielutils-0.8.7/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     4763 2023-06-01 23:17:25.000000 danielutils-0.8.7/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.360462 danielutils-0.8.7/danielutils/Conversions/
--rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.8.7/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.363055 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      491 2023-06-02 09:23:12.000000 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.7/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.8.7/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.370063 danielutils-0.8.7/danielutils/DataStructures/
--rw-rw-rw-   0        0        0     1056 2023-06-02 08:41:44.000000 danielutils-0.8.7/danielutils/DataStructures/Comparer.py
--rw-rw-rw-   0        0        0     2264 2023-06-02 09:00:59.000000 danielutils-0.8.7/danielutils/DataStructures/Graph.py
--rw-rw-rw-   0        0        0     3372 2023-06-02 08:43:49.000000 danielutils-0.8.7/danielutils/DataStructures/Heap.py
--rw-rw-rw-   0        0        0     2620 2023-06-02 08:58:56.000000 danielutils-0.8.7/danielutils/DataStructures/Node.py
--rw-rw-rw-   0        0        0     5065 2023-06-02 08:59:09.000000 danielutils-0.8.7/danielutils/DataStructures/Queue.py
--rw-rw-rw-   0        0        0     1507 2023-06-01 23:41:53.000000 danielutils-0.8.7/danielutils/DataStructures/Stack.py
--rw-rw-rw-   0        0        0      133 2023-05-10 19:33:24.000000 danielutils-0.8.7/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      607 2023-04-20 20:07:14.000000 danielutils-0.8.7/danielutils/DataStructures/functions.py
--rw-rw-rw-   0        0        0      135 2023-04-21 22:43:20.000000 danielutils-0.8.7/danielutils/DateTime.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.379999 danielutils-0.8.7/danielutils/Decorators/
--rw-rw-rw-   0        0        0      696 2023-04-29 17:38:05.000000 danielutils-0.8.7/danielutils/Decorators/PartiallyImplemented.py
--rw-rw-rw-   0        0        0      361 2023-06-01 10:32:05.000000 danielutils-0.8.7/danielutils/Decorators/__init__.py
--rw-rw-rw-   0        0        0      613 2023-06-01 23:35:30.000000 danielutils-0.8.7/danielutils/Decorators/atomic.py
--rw-rw-rw-   0        0        0     1213 2023-06-01 22:03:38.000000 danielutils-0.8.7/danielutils/Decorators/attach.py
--rw-rw-rw-   0        0        0      730 2023-04-29 17:58:20.000000 danielutils-0.8.7/danielutils/Decorators/chain_decorators.py
--rw-rw-rw-   0        0        0      853 2023-06-01 23:23:43.000000 danielutils-0.8.7/danielutils/Decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0      817 2023-04-29 18:02:16.000000 danielutils-0.8.7/danielutils/Decorators/delay_call.py
--rw-rw-rw-   0        0        0      587 2023-06-01 10:37:25.000000 danielutils-0.8.7/danielutils/Decorators/deprecate.py
--rw-rw-rw-   0        0        0     1479 2023-04-29 17:44:59.000000 danielutils-0.8.7/danielutils/Decorators/limit_recursion.py
--rw-rw-rw-   0        0        0      622 2023-04-29 17:38:26.000000 danielutils-0.8.7/danielutils/Decorators/memo.py
--rw-rw-rw-   0        0        0    10169 2023-06-02 09:22:26.000000 danielutils-0.8.7/danielutils/Decorators/overload.py
--rw-rw-rw-   0        0        0      661 2023-05-21 20:38:07.000000 danielutils-0.8.7/danielutils/Decorators/property.py
--rw-rw-rw-   0        0        0      595 2023-04-29 17:59:44.000000 danielutils-0.8.7/danielutils/Decorators/threadify.py
--rw-rw-rw-   0        0        0     1730 2023-06-01 23:20:48.000000 danielutils-0.8.7/danielutils/Decorators/timeout.py
--rw-rw-rw-   0        0        0     9642 2023-06-01 23:37:04.000000 danielutils-0.8.7/danielutils/Decorators/validate.py
--rw-rw-rw-   0        0        0     2130 2023-04-30 19:46:55.000000 danielutils-0.8.7/danielutils/Exceptions.py
--rw-rw-rw-   0        0        0     8761 2023-06-02 09:04:00.000000 danielutils-0.8.7/danielutils/Functions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.383389 danielutils-0.8.7/danielutils/Generators/
--rw-rw-rw-   0        0        0       70 2023-06-01 11:44:02.000000 danielutils-0.8.7/danielutils/Generators/__init__.py
--rw-rw-rw-   0        0        0      450 2023-06-01 12:22:56.000000 danielutils-0.8.7/danielutils/Generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2638 2023-06-01 23:35:56.000000 danielutils-0.8.7/danielutils/Generators/join_generators.py
--rw-rw-rw-   0        0        0     9424 2023-06-01 22:39:00.000000 danielutils-0.8.7/danielutils/IO.py
--rw-rw-rw-   0        0        0     1851 2023-06-01 22:39:25.000000 danielutils-0.8.7/danielutils/Internet.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.388073 danielutils-0.8.7/danielutils/Math/
--rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.8.7/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      341 2023-06-01 22:46:15.000000 danielutils-0.8.7/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0     1061 2023-06-01 23:34:42.000000 danielutils-0.8.7/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     3815 2023-06-01 22:45:35.000000 danielutils-0.8.7/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.7/danielutils/Math/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.391847 danielutils-0.8.7/danielutils/MetaClasses/
--rw-rw-rw-   0        0        0      724 2023-06-01 23:27:38.000000 danielutils-0.8.7/danielutils/MetaClasses/AtomicClassMeta.py
--rw-rw-rw-   0        0        0     1950 2023-06-01 23:27:26.000000 danielutils-0.8.7/danielutils/MetaClasses/ImplicitDataDeleterMeta.py
--rw-rw-rw-   0        0        0     1499 2023-05-01 12:50:48.000000 danielutils-0.8.7/danielutils/MetaClasses/InstanceCacheMeta.py
--rw-rw-rw-   0        0        0    10521 2023-06-02 08:37:49.000000 danielutils-0.8.7/danielutils/MetaClasses/Interface.py
--rw-rw-rw-   0        0        0       98 2023-04-30 22:02:36.000000 danielutils-0.8.7/danielutils/MetaClasses/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.7/danielutils/Path.py
--rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.7/danielutils/Print.py
--rw-rw-rw-   0        0        0     5412 2023-06-01 22:35:02.000000 danielutils-0.8.7/danielutils/Reflection.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.394288 danielutils-0.8.7/danielutils/Snippets/
--rw-rw-rw-   0        0        0       24 2023-06-01 14:01:33.000000 danielutils-0.8.7/danielutils/Snippets/__init__.py
--rw-rw-rw-   0        0        0      214 2023-06-01 14:01:26.000000 danielutils-0.8.7/danielutils/Snippets/try_get.py
--rw-rw-rw-   0        0        0     6444 2023-06-01 22:24:03.000000 danielutils-0.8.7/danielutils/System.py
--rw-rw-rw-   0        0        0     4213 2023-04-29 18:00:25.000000 danielutils-0.8.7/danielutils/Text.py
--rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.7/danielutils/Time.py
--rw-rw-rw-   0        0        0     2254 2023-04-21 15:17:41.000000 danielutils-0.8.7/danielutils/Windows.py
--rw-rw-rw-   0        0        0      688 2023-06-01 17:00:29.000000 danielutils-0.8.7/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.351697 danielutils-0.8.7/danielutils.egg-info/
--rw-rw-rw-   0        0        0     1967 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2616 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      728 2023-06-02 10:05:07.000000 danielutils-0.8.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 10:05:08.395799 danielutils-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0     1389 2023-06-02 10:05:07.000000 danielutils-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.673278 danielutils-0.9.0/
+-rw-rw-rw-   0        0        0     3313 2023-06-03 13:04:23.673278 danielutils-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2542 2023-06-03 13:04:22.000000 danielutils-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.607473 danielutils-0.9.0/danielutils/
+-rw-rw-rw-   0        0        0     4551 2023-06-03 11:02:15.000000 danielutils-0.9.0/danielutils/Aliases.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.620674 danielutils-0.9.0/danielutils/Classes/
+-rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.9.0/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     1144 2023-06-01 23:36:28.000000 danielutils-0.9.0/danielutils/Classes/Counter.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.626266 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/
+-rw-rw-rw-   0        0        0       94 2023-06-02 22:44:50.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/__init__.py
+-rw-rw-rw-   0        0        0      507 2023-06-03 11:23:40.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tbase.py
+-rw-rw-rw-   0        0        0     2086 2023-06-03 11:18:53.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tdict.py
+-rw-rw-rw-   0        0        0     4201 2023-06-03 11:21:46.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tlist.py
+-rw-rw-rw-   0        0        0      876 2023-06-03 11:23:36.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tset.py
+-rw-rw-rw-   0        0        0      151 2023-06-03 11:23:41.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/ttuple.py
+-rw-rw-rw-   0        0        0      126 2023-05-01 13:01:32.000000 danielutils-0.9.0/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-06-01 21:36:49.000000 danielutils-0.9.0/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     5440 2023-06-02 20:00:18.000000 danielutils-0.9.0/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.627529 danielutils-0.9.0/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.9.0/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.629539 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      505 2023-06-03 11:19:44.000000 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.9.0/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.9.0/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.636064 danielutils-0.9.0/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0     1056 2023-06-02 08:41:44.000000 danielutils-0.9.0/danielutils/DataStructures/Comparer.py
+-rw-rw-rw-   0        0        0     2282 2023-06-02 21:03:54.000000 danielutils-0.9.0/danielutils/DataStructures/Graph.py
+-rw-rw-rw-   0        0        0     3372 2023-06-02 08:43:49.000000 danielutils-0.9.0/danielutils/DataStructures/Heap.py
+-rw-rw-rw-   0        0        0     2620 2023-06-02 08:58:56.000000 danielutils-0.9.0/danielutils/DataStructures/Node.py
+-rw-rw-rw-   0        0        0     5065 2023-06-02 08:59:09.000000 danielutils-0.9.0/danielutils/DataStructures/Queue.py
+-rw-rw-rw-   0        0        0     1507 2023-06-01 23:41:53.000000 danielutils-0.9.0/danielutils/DataStructures/Stack.py
+-rw-rw-rw-   0        0        0      133 2023-05-10 19:33:24.000000 danielutils-0.9.0/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      616 2023-06-03 11:02:22.000000 danielutils-0.9.0/danielutils/DataStructures/functions.py
+-rw-rw-rw-   0        0        0      135 2023-04-21 22:43:20.000000 danielutils-0.9.0/danielutils/DateTime.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.648553 danielutils-0.9.0/danielutils/Decorators/
+-rw-rw-rw-   0        0        0      696 2023-04-29 17:38:05.000000 danielutils-0.9.0/danielutils/Decorators/PartiallyImplemented.py
+-rw-rw-rw-   0        0        0      361 2023-06-01 10:32:05.000000 danielutils-0.9.0/danielutils/Decorators/__init__.py
+-rw-rw-rw-   0        0        0      613 2023-06-01 23:35:30.000000 danielutils-0.9.0/danielutils/Decorators/atomic.py
+-rw-rw-rw-   0        0        0     1213 2023-06-01 22:03:38.000000 danielutils-0.9.0/danielutils/Decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2023-04-29 17:58:20.000000 danielutils-0.9.0/danielutils/Decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0      853 2023-06-01 23:23:43.000000 danielutils-0.9.0/danielutils/Decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0      817 2023-04-29 18:02:16.000000 danielutils-0.9.0/danielutils/Decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1082 2023-06-02 20:21:38.000000 danielutils-0.9.0/danielutils/Decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1552 2023-06-02 20:36:42.000000 danielutils-0.9.0/danielutils/Decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      622 2023-04-29 17:38:26.000000 danielutils-0.9.0/danielutils/Decorators/memo.py
+-rw-rw-rw-   0        0        0     7232 2023-06-03 11:24:52.000000 danielutils-0.9.0/danielutils/Decorators/overload.py
+-rw-rw-rw-   0        0        0      661 2023-05-21 20:38:07.000000 danielutils-0.9.0/danielutils/Decorators/property.py
+-rw-rw-rw-   0        0        0      595 2023-04-29 17:59:44.000000 danielutils-0.9.0/danielutils/Decorators/threadify.py
+-rw-rw-rw-   0        0        0     1730 2023-06-01 23:20:48.000000 danielutils-0.9.0/danielutils/Decorators/timeout.py
+-rw-rw-rw-   0        0        0     9685 2023-06-03 11:06:39.000000 danielutils-0.9.0/danielutils/Decorators/validate.py
+-rw-rw-rw-   0        0        0     2130 2023-04-30 19:46:55.000000 danielutils-0.9.0/danielutils/Exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.653613 danielutils-0.9.0/danielutils/Functions/
+-rw-rw-rw-   0        0        0      135 2023-06-03 10:48:20.000000 danielutils-0.9.0/danielutils/Functions/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-06-03 10:58:55.000000 danielutils-0.9.0/danielutils/Functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2023-06-03 10:45:50.000000 danielutils-0.9.0/danielutils/Functions/check_foreach.py
+-rw-rw-rw-   0        0        0     5498 2023-06-03 10:48:37.000000 danielutils-0.9.0/danielutils/Functions/isoftype.py
+-rw-rw-rw-   0        0        0     1372 2023-06-03 10:47:36.000000 danielutils-0.9.0/danielutils/Functions/isoneof.py
+-rw-rw-rw-   0        0        0      582 2023-06-03 10:45:17.000000 danielutils-0.9.0/danielutils/Functions/types_subseteq.py
+-rw-rw-rw-   0        0        0        0 2023-06-03 10:50:20.000000 danielutils-0.9.0/danielutils/Functions.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.656121 danielutils-0.9.0/danielutils/Generators/
+-rw-rw-rw-   0        0        0       70 2023-06-01 11:44:02.000000 danielutils-0.9.0/danielutils/Generators/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-06-01 12:22:56.000000 danielutils-0.9.0/danielutils/Generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2638 2023-06-01 23:35:56.000000 danielutils-0.9.0/danielutils/Generators/join_generators.py
+-rw-rw-rw-   0        0        0     9490 2023-06-02 20:25:10.000000 danielutils-0.9.0/danielutils/IO.py
+-rw-rw-rw-   0        0        0     1852 2023-06-02 19:50:25.000000 danielutils-0.9.0/danielutils/Internet.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.660501 danielutils-0.9.0/danielutils/Math/
+-rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.9.0/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      341 2023-06-01 22:46:15.000000 danielutils-0.9.0/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0     1061 2023-06-01 23:34:42.000000 danielutils-0.9.0/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     3815 2023-06-01 22:45:35.000000 danielutils-0.9.0/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.9.0/danielutils/Math/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.664675 danielutils-0.9.0/danielutils/MetaClasses/
+-rw-rw-rw-   0        0        0      724 2023-06-01 23:27:38.000000 danielutils-0.9.0/danielutils/MetaClasses/AtomicClassMeta.py
+-rw-rw-rw-   0        0        0     1950 2023-06-01 23:27:26.000000 danielutils-0.9.0/danielutils/MetaClasses/ImplicitDataDeleterMeta.py
+-rw-rw-rw-   0        0        0     1499 2023-05-01 12:50:48.000000 danielutils-0.9.0/danielutils/MetaClasses/InstanceCacheMeta.py
+-rw-rw-rw-   0        0        0    10521 2023-06-02 08:37:49.000000 danielutils-0.9.0/danielutils/MetaClasses/Interface.py
+-rw-rw-rw-   0        0        0     1422 2023-06-03 11:22:02.000000 danielutils-0.9.0/danielutils/MetaClasses/OverloadMeta.py
+-rw-rw-rw-   0        0        0       98 2023-04-30 22:02:36.000000 danielutils-0.9.0/danielutils/MetaClasses/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-06-02 20:14:53.000000 danielutils-0.9.0/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2799 2023-06-03 11:03:50.000000 danielutils-0.9.0/danielutils/Print.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.670229 danielutils-0.9.0/danielutils/Reflection/
+-rw-rw-rw-   0        0        0      945 2023-06-03 10:53:31.000000 danielutils-0.9.0/danielutils/Reflection/File.py
+-rw-rw-rw-   0        0        0     4042 2023-06-03 11:13:30.000000 danielutils-0.9.0/danielutils/Reflection/Function.py
+-rw-rw-rw-   0        0        0      507 2023-06-03 10:56:16.000000 danielutils-0.9.0/danielutils/Reflection/Module.py
+-rw-rw-rw-   0        0        0      876 2023-06-03 10:55:25.000000 danielutils-0.9.0/danielutils/Reflection/System.py
+-rw-rw-rw-   0        0        0     1476 2023-06-03 10:56:58.000000 danielutils-0.9.0/danielutils/Reflection/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-06-03 10:51:21.000000 danielutils-0.9.0/danielutils/Reflection/_get_prev_frame.py
+-rw-rw-rw-   0        0        0      275 2023-06-03 10:42:46.000000 danielutils-0.9.0/danielutils/Reflection/get_traceback.py
+-rw-rw-rw-   0        0        0      117 2023-06-02 22:45:41.000000 danielutils-0.9.0/danielutils/Relations.py
+-rw-rw-rw-   0        0        0      489 2023-06-02 19:49:07.000000 danielutils-0.9.0/danielutils/Signals.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.672235 danielutils-0.9.0/danielutils/Snippets/
+-rw-rw-rw-   0        0        0       24 2023-06-01 14:01:33.000000 danielutils-0.9.0/danielutils/Snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-06-02 19:32:42.000000 danielutils-0.9.0/danielutils/Snippets/try_get.py
+-rw-rw-rw-   0        0        0     6456 2023-06-02 20:14:24.000000 danielutils-0.9.0/danielutils/System.py
+-rw-rw-rw-   0        0        0     4224 2023-06-03 11:04:13.000000 danielutils-0.9.0/danielutils/Text.py
+-rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.9.0/danielutils/Time.py
+-rw-rw-rw-   0        0        0     2254 2023-04-21 15:17:41.000000 danielutils-0.9.0/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      712 2023-06-03 10:43:48.000000 danielutils-0.9.0/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.617256 danielutils-0.9.0/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     3313 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3107 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      767 2023-06-03 13:04:22.000000 danielutils-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 13:04:23.673278 danielutils-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-06-03 13:04:22.000000 danielutils-0.9.0/setup.py
```

### Comparing `danielutils-0.8.7/danielutils/Aliases.py` & `danielutils-0.9.0/danielutils/Aliases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 from abc import ABC, abstractmethod
-from typing import cast, TypeAlias, Union
-from .Functions import get_function_return_type, isoftype
-from .Reflection import get_caller_name
+from typing import cast
+from .Functions.isoftype import isoftype
+from .Reflection.Function import get_caller_name, get_function_return_type
 
 
 class SubscribableBase(ABC):
     """An abstract class that need __instanceCheck__ to be implemented
         will create default functions such that isinstance will work with the new type
         while it is used as all of the python's generic types
     """
@@ -105,30 +105,34 @@
 #         param_iter = iter(signature.parameters.values())
 #         param1_type = next(param_iter).annotation
 #         param2_type = next(param_iter).annotation
 #         try:
 #             return param1_type == param2_type == self.params[0] == self.params[1]
 #         except:
 #             return False
+# class Predicate(SubscribableBase):
+#     """create a type for functions to be a consumer function
+#     """
 
-# def predicate(func,self):
-#     if not callable(func):
+#     def __instancecheck__(self, func) -> bool:
+#         if not callable(func):
+#             return False
+#         signature = inspect.signature(func)
+#         if len(signature.parameters) != 0:
+#             return False
+
+#         return_type = get_function_return_type(func)
+#         try:
+#             return isoftype(return_type(), self.params)
+#         except:
 #             return False
-#     signature = inspect.signature(func)
-#     if len(signature.parameters) != 0:
-#         return False
-
-#     return_type = get_function_return_type(func)
-#     try:
-#         return isoftype(return_type(), self.params)
-#     except:
-#         return False
 
 
 # ListTupleType: TypeAlias = Union[list, tuple]
 __all__ = [
     "SubscribableBase",
     "Supplier",
     "Consumer",
     "BinaryConsumer",
+    # "Predicate"
     # "ListTupleType"
 ]
```

### Comparing `danielutils-0.8.7/danielutils/Classes/Counter.py` & `danielutils-0.9.0/danielutils/Classes/Counter.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tdict.py` & `danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tdict.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-from __future__ import annotations
-from typing import Iterable
-# from .tbase import tbase
-from ...Decorators import overload
-from ...Functions import isoftype
-
-
-class tdict(dict):
-    """like builtin dict but only a specif type is allowed
-    """
-    @overload(None, type, type)
-    def __init__(self, key_t: type, val_t: type):
-        self.key_t: type = key_t
-        self.val_t: type = val_t
-        super().__init__()
-
-    @overload(None, type, type, Iterable)
-    def __init__(self, key_t: type, val_t: type, iterable: Iterable[tuple]):
-        self.key_t: type = key_t
-        self.val_t: type = val_t
-        super().__init__(iterable)
-
-    @overload(None, type, type, dict)
-    def __init__(self, key_t: type, val_t: type, ** kwargs):
-        """dict(type,type) -> new empty dictionary dict(mapping) -> new dictionary initialized from a mapping object's
-                (key, value) pairs
-            dict(type,type,iterable) -> new dictionary initialized as if via:
-                d = {} for k, v in iterable:
-                    d[k] = v
-            dict(type,type,**kwargs) -> new dictionary initialized with the name=value pairs
-                in the keyword argument list. For example: dict(one=1, two=2)
-        """
-        super().__init__(**kwargs)
-        self.key_t: type = key_t
-        self.val_t: type = val_t
-
-    def __setitem__(self, key, value) -> None:
-        if not isoftype(key, self.key_t):
-            raise TypeError(
-                f"In class 'tdict' error creating new key-value pair as"
-                f" key = '{key}' is not of type '{self.key_t}'")
-        if not isoftype(value, self.val_t):
-            raise TypeError(
-                f"In class 'tdict' error creating new key-value pair"
-                f" as value = '{value}' is not of type '{ self.val_t}'")
-        super().__setitem__(key, value)
-
-    def __str__(self):
-        return f"dict[{self.key_t.__name__}, {self.val_t.__name__}]: {super().__str__()}"
-
-
-__all__ = [
-    "tdict"
-]
+# from __future__ import annotations
+# from typing import Iterable
+# # from .tbase import tbase
+
+# from ...Decorators import overload2
+# from ...Functions import isoftype
+
+
+# class tdict(dict):
+#     """like builtin dict but only a specif type is allowed
+#     """
+#     @overload2
+#     def __init__(self, key_t: type, val_t: type):
+#         self.key_t: type = key_t
+#         self.val_t: type = val_t
+#         super().__init__()
+
+#     @__init__.overload
+#     def __init__(self, key_t: type, val_t: type, iterable: Iterable[tuple]):
+#         self.key_t: type = key_t
+#         self.val_t: type = val_t
+#         super().__init__(iterable)
+
+#     @__init__.overload
+#     def __init__(self, key_t: type, val_t: type, ** kwargs):
+#         """dict(type,type) -> new empty dictionary dict(mapping) -> new dictionary initialized from a mapping object's
+#                 (key, value) pairs
+#             dict(type,type,iterable) -> new dictionary initialized as if via:
+#                 d = {} for k, v in iterable:
+#                     d[k] = v
+#             dict(type,type,**kwargs) -> new dictionary initialized with the name=value pairs
+#                 in the keyword argument list. For example: dict(one=1, two=2)
+#         """
+#         super().__init__(**kwargs)
+#         self.key_t: type = key_t
+#         self.val_t: type = val_t
+
+#     def __setitem__(self, key, value) -> None:
+#         if not isoftype(key, self.key_t):
+#             raise TypeError(
+#                 f"In class 'tdict' error creating new key-value pair as"
+#                 f" key = '{key}' is not of type '{self.key_t}'")
+#         if not isoftype(value, self.val_t):
+#             raise TypeError(
+#                 f"In class 'tdict' error creating new key-value pair"
+#                 f" as value = '{value}' is not of type '{ self.val_t}'")
+#         super().__setitem__(key, value)
+
+#     def __str__(self):
+#         return f"dict[{self.key_t.__name__}, {self.val_t.__name__}]: {super().__str__()}"
+
+
+# __all__ = [
+#     "tdict"
+# ]
```

### Comparing `danielutils-0.8.7/danielutils/Classes/frange.py` & `danielutils-0.9.0/danielutils/Classes/frange.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Colors.py` & `danielutils-0.9.0/danielutils/Colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from typing import Optional
+from typing import Optional, IO
 from .Decorators.validate import validate
 
 
+RESET = "\033[0m"
+
+
 class ColoredText:
     """static utility class with static functions:\n
         from_rgb,
         green,
         red,
         blue,
         red,
@@ -23,15 +26,15 @@
             g (int): The green component of the color.
             b (int): The blue component of the color.
             text (str): The text to apply the color to.
 
         Returns:
             str: The given text with an RGB color applied to it.
         """
-        return f"\033[38;2;{red};{green};{blue}m{text}\033[38;2;255;255;255m"
+        return f"\033[38;2;{red};{green};{blue}m{text}{RESET}"
 
     @staticmethod
     def green(text: str) -> str:
         """Applies green color to the given text.
 
         Args:
             text (str): The text to apply the green color to.
@@ -109,28 +112,52 @@
             text (str): The text to apply the black color to.
 
         Returns:
             str: The given text with black color applied to it.
         """
         return ColoredText.from_rgb(0, 0, 0, text)
 
+    @staticmethod
+    def supports_color(stream: IO) -> bool:
+        """return whether a stream will support colored text
+
+        Args:
+            stream (IO): stream to check
+
+        Returns:
+            bool: boolean result
+        """
+        return stream.isatty()
+
 
 def __special_print(*args, sep: str = " ", end: str = "\n", start_with: Optional[str] = None):
     """inner helper function"""
     if start_with:
         if "\n" not in sep:
             print(f"{start_with}: ", end="")
             print(sep.join([str(arg) for arg in args]), sep="", end=end)
         else:
             print(
                 sep.join([f"{start_with}: {str(arg)}" for arg in args]), sep="", end=end)
     else:
         print(*args, sep=sep, end=end)
 
 
+def success(*args, sep: str = " ", end: str = "\n"):
+    """print a success message
+
+    Args:
+        sep (str, optional): print separator. Defaults to " ".
+        end (str, optional): print endline. Defaults to "\\n".
+    """
+
+    __special_print(*args, sep=sep, end=end,
+                    start_with=ColoredText.green("SUCCESS"))
+
+
 def warning(*args, sep: str = " ", end: str = "\n"):
     """print a warning message
 
     Args:
         sep (str, optional): print separator. Defaults to " ".
         end (str, optional): print endline. Defaults to "\\n".
     """
@@ -159,10 +186,12 @@
     """
     __special_print(*args, sep=sep, end=end,
                     start_with=ColoredText.red("INFO"))
 
 
 __all__ = [
     "ColoredText",
+    "success",
     "warning",
-    "error"
+    "error",
+    "info"
 ]
```

### Comparing `danielutils-0.8.7/danielutils/Conversions/MainConversions.py` & `danielutils-0.9.0/danielutils/Conversions/MainConversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Data.py` & `danielutils-0.9.0/danielutils/Data.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/DataStructures/Comparer.py` & `danielutils-0.9.0/danielutils/DataStructures/Comparer.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/DataStructures/Graph.py` & `danielutils-0.9.0/danielutils/DataStructures/Graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,22 @@
         all_nodes = []
 
         def handle_node(node: MultiNode):
             nonlocal travel_index
             seen.add(node)
             all_nodes.append(node)
             yield node
-            for node in node._children:
-                if node not in seen:
+            for subnode in node._children:
+                if subnode not in seen:
                     travel_index += 1
-                    enter_times[node] = travel_index
-                    if node is not None:
-                        yield from handle_node(node)
+                    enter_times[subnode] = travel_index
+                    if subnode is not None:
+                        yield from handle_node(subnode)
                     travel_index += 1
-                    exit_times[node] = travel_index
+                    exit_times[subnode] = travel_index
 
         for node in self.nodes:
             if node not in seen:
                 enter_times[node] = travel_index
                 travel_index += 1
                 yield from handle_node(node)
                 travel_index += 1
```

### Comparing `danielutils-0.8.7/danielutils/DataStructures/Heap.py` & `danielutils-0.9.0/danielutils/DataStructures/Heap.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/DataStructures/Node.py` & `danielutils-0.9.0/danielutils/DataStructures/Node.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/DataStructures/Queue.py` & `danielutils-0.9.0/danielutils/DataStructures/Queue.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/DataStructures/Stack.py` & `danielutils-0.9.0/danielutils/DataStructures/Stack.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/DataStructures/functions.py` & `danielutils-0.9.0/danielutils/DataStructures/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any
-from ..Functions import isoftype
+from ..Functions.isoftype import isoftype
 
 
 def default_weight_function(v: Any) -> int | float:
     """will return the weight of an object
 
     Args:
         v (Any): object
```

### Comparing `danielutils-0.8.7/danielutils/Decorators/PartiallyImplemented.py` & `danielutils-0.9.0/danielutils/Decorators/PartiallyImplemented.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/atomic.py` & `danielutils-0.9.0/danielutils/Decorators/atomic.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/attach.py` & `danielutils-0.9.0/danielutils/Decorators/attach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/chain_decorators.py` & `danielutils-0.9.0/danielutils/Decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/decorate_conditionally.py` & `danielutils-0.9.0/danielutils/Decorators/decorate_conditionally.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/delay_call.py` & `danielutils-0.9.0/danielutils/Decorators/delay_call.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/limit_recursion.py` & `danielutils-0.9.0/danielutils/Decorators/limit_recursion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import functools
 import re
 import traceback
-from typing import Any
+from typing import Any, Callable
 from .validate import validate
 from ..Colors import warning
 
 
 @validate
-def limit_recursion(max_depth: int, return_value: Any = None, quiet: bool = True):
+def limit_recursion(max_depth: int, return_value: Any = None, quiet: bool = True) -> Callable:
     """decorator to limit recursion of functions
 
     Args:
         max_depth (int): max recursion depth which is allowed for this function
-        return_value (_type_, optional): The value to return when the limit is reached. Defaults to None.
-            if is None, will return the last (args, kwargs)
+        return_value (Any, optional): The value to return when the limit is reached. Defaults to None.
+            if is None, will return the last a tuple for the last args, kwargs given
         quiet (bool, optional): whether to print a warning message. Defaults to True.
     """
 
-    def deco(func):
+    def deco(func: Callable) -> Callable:
         @ functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args, **kwargs) -> Any:
             depth = functools.reduce(
                 lambda count, line:
                     count + 1 if re.search(rf"{func.__name__}\(.*\)$", line)
                     else count,
                 traceback.format_stack(), 0
             )
             if depth >= max_depth:
```

### Comparing `danielutils-0.8.7/danielutils/Decorators/memo.py` & `danielutils-0.9.0/danielutils/Decorators/memo.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/property.py` & `danielutils-0.9.0/danielutils/Decorators/property.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/threadify.py` & `danielutils-0.9.0/danielutils/Decorators/threadify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/timeout.py` & `danielutils-0.9.0/danielutils/Decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Decorators/validate.py` & `danielutils-0.9.0/danielutils/Decorators/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import inspect
 from typing import Callable, get_type_hints, cast
-from ..Functions import isoftype, get_function_return_type
+from ..Functions.isoftype import isoftype
+from ..Reflection.Function import get_function_return_type
 from ..Exceptions import EmptyAnnotationException,\
     InvalidDefaultValueException, ValidationException, InvalidReturnValueException
 
 
 def validate(strict: Callable | bool = True) -> Callable:
     """A decorator that validates the annotations and types of the arguments and return
     value of a function.
```

### Comparing `danielutils-0.8.7/danielutils/Exceptions.py` & `danielutils-0.9.0/danielutils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Generators/join_generators.py` & `danielutils-0.9.0/danielutils/Generators/join_generators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/IO.py` & `danielutils-0.9.0/danielutils/IO.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,69 +213,75 @@
         get_files(path)
     )
     for subdir in get_directories(path):
         for v in get_file_type_from_directory_recursively(f"{path}\\{subdir}", file_type):
             yield f"{subdir}\\{v}"
 
 
+@validate
 def rename_file(path: str, new_name: str) -> None:
     """renames a file
 
     Args:
         path (str): file to rename
         new_name (str): the desired new name
     """
     new_path = "./" + \
         "/".join(Path(path).parts[:-1])+"/"+new_name+Path(path).suffix
     move_file(path, new_path)
 
 
+@validate
 def move_file(old_path: str, new_path: str) -> None:
     """moves a file
 
     Args:
         old_path (str): old path
         new_path (str): new path
     """
     os.rename(old_path, new_path)
 
 
+@validate
 async def open_file(file_path: str, application_path: str) -> int:
     """open a file with the specified application
 
     Args:
         file_path (str): the file to open
         application_path (str): the application to open with
     Returns:
         int: return code
     """
     with subprocess.Popen([application_path, file_path]) as p:
         return p.wait()
 
 
+@validate
 def move_directory(old_path: str, new_path: str) -> None:
     """moves a directory
 
     Args:
         old_path (str): old path
         new_path (str): new path
     """
     shutil.move(old_path, new_path)
 
 
+@validate
 def copy_file(src: str, dest: str) -> None:
     """copies file from src to dest
 
     Args:
         src (str): src
         dest (str): dest
     """
     shutil.copy(src, dest)
 
 
+@validate
 def copy_directory(src: str, dest: str) -> None:
     """copies a directory from src to dest
 
     Args:
         src (str): stc
         dest (str): dest
     """
```

### Comparing `danielutils-0.8.7/danielutils/Internet.py` & `danielutils-0.9.0/danielutils/Internet.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # def prettify_html(html: str) -> str:
 #     return html
 
 
 @validate
 def get_html(url: str) -> str:
-    """retuns the html for a given url
+    """returns the html for a given url
 
     Args:
         url (str): url
 
     Returns:
         str: the html as a string
     """
```

### Comparing `danielutils-0.8.7/danielutils/Math/Constants.py` & `danielutils-0.9.0/danielutils/Math/Constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Math/MathPrint.py` & `danielutils-0.9.0/danielutils/Math/MathPrint.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Math/MathSymbols.py` & `danielutils-0.9.0/danielutils/Math/MathSymbols.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/MetaClasses/AtomicClassMeta.py` & `danielutils-0.9.0/danielutils/MetaClasses/AtomicClassMeta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/MetaClasses/ImplicitDataDeleterMeta.py` & `danielutils-0.9.0/danielutils/MetaClasses/ImplicitDataDeleterMeta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/MetaClasses/InstanceCacheMeta.py` & `danielutils-0.9.0/danielutils/MetaClasses/InstanceCacheMeta.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/MetaClasses/Interface.py` & `danielutils-0.9.0/danielutils/MetaClasses/Interface.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/Path.py` & `danielutils-0.9.0/danielutils/Path.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,9 +42,10 @@
     """
     return os.path.realpath(path)
 
 
 __all__ = [
     "get_current_working_directory",
     "set_current_working_directory",
-    "get_absolute_path"
+    "get_absolute_path",
+    "get_relative_path"
 ]
```

### Comparing `danielutils-0.8.7/danielutils/Print.py` & `danielutils-0.9.0/danielutils/Print.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
-from .Functions import areoneof
+from .Functions.areoneof import areoneof
 from .Math.MathPrint import mprint_parse_one
-from .Decorators import atomic
+from .Decorators import atomic, deprecate
 
 
 def mprint(*args, sep: str = " ", end: str = "\n", stream=sys.stdout) -> None:
     """Prints a formatted representation of mathematical expressions to the specified stream.
 
     Args:
         *args: The mathematical expressions to print.
@@ -20,14 +20,15 @@
         None
     """
     if not areoneof(args, [str]):
         raise TypeError("s must be a string")
     stream.write(sep.join([mprint_parse_one(s) for s in args])+end)
 
 
+@deprecate("The built-in 'print' function has an argument called 'file', use this instead")
 def sprint(*args, sep: str = " ", end: str = "\n", stream=sys.stdout) -> None:
     """Writes a string representation of the given arguments to the specified stream.
 
     Args:
         *args: The arguments to print.
         sep (str, optional): The separator to use between the arguments. Defaults to " ".
         end (str, optional): The string to append to the end of the printed arguments. Defaults to "\n".
```

### Comparing `danielutils-0.8.7/danielutils/System.py` & `danielutils-0.9.0/danielutils/System.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     b_end = str_to_bytes(end)
     p.stdin.write(b_args+b_end)
     p.stdin.flush()
 
 
 @validate
 def acm(command: str, inputs: Optional[list[str]] = None, i_timeout: float = 0.01,
-        shell: bool = False, use_write_helper: bool = True, cwd: Optional[str] = None) -> tuple[int, list[bytes] | None, list[bytes] | None]:
+        shell: bool = False, use_write_helper: bool = True, cwd: Optional[str] = None) -> tuple[int, Optional[list[bytes]], Optional[list[bytes]]]:
     """Advanced command
 
     Args:
         command (str): The command to execute\n
         inputs (list[str]): the inputs to give to the program from the command. Defaults to None.\n
         i_timeout (float, optional): An individual timeout for every step of the execution. Defaults to 0.01.\n
         cwd (?, optional): Current working directory. Defaults to None.\n
@@ -72,15 +72,15 @@
         would have been parse with builtin print() or to use raw text. Defaults to True.
 
     Raises:
         If @timeout will raise something other than TimeoutError.\n
         If the subprocess input and output handling will raise an exception.
 
     Returns:
-        tuple[int, list[bytes] | None, list[bytes] | None]: return code, stdout, stderr
+        tuple[int, Optional[list[bytes]], Optional[list[bytes]]]: return code, stdout, stderr
     """
 
     if inputs is None:
         inputs = []
 
     p = None
     try:
```

### Comparing `danielutils-0.8.7/danielutils/Text.py` & `danielutils-0.9.0/danielutils/Text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from typing import Union, TypeGuard
 from .Decorators.validate import validate
-from .Functions import check_foreach
+from .Functions.check_foreach import check_foreach
 HEBREW_LETTERS = ['\u05D0', '\u2135', '\uFB21', '\uFB2E', '\uFB2F',
                   '\uFB30', '\uFB4F', '\u05D1', '\u2136', '\uFB31',
                   '\uFB4C', '\u05D2', '\u2137', '\uFB32', '\u05D3',
                   '\u2138', '\uFB22', '\uFB33', '\u05D4', '\uFB23',
                   '\uFB34', '\u05D5', '\uFB4B', '\uFB35', '\u05F0',
                   '\u05F1', '\u05D6', '\uFB36', '\u05D7', '\u05D8',
                   '\uFB38', '\u05D9', '\uFB1D', '\uFB39', '\u05EF',
@@ -91,15 +91,15 @@
 def is_hebrew(s: str) -> TypeGuard[str]:
     """checks if a string is in hebrew
 
     Args:
         text (str): string to check
 
     Returns:
-        TypeGuard[str]: true iff all chars are in hebrew
+        TypeGuard[str]: true iff all chars are hebrew
     """
     return check_foreach(s, lambda c: c in HEBREW_LETTERS)
 
 
 @validate
 def is_binary(s: str) -> bool:
     """checks if s string has a binary value
```

### Comparing `danielutils-0.8.7/danielutils/Windows.py` & `danielutils-0.9.0/danielutils/Windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.7/danielutils/__init__.py` & `danielutils-0.9.0/danielutils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 from .Exceptions import PrintCatchOne
 from .Reflection import *
 from .DateTime import *
 from .MetaClasses import *
 from .Generators import *
 from .Snippets import *
 from .Aliases import *
+from .Signals import *
```

### Comparing `danielutils-0.8.7/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.0/danielutils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 danielutils/DateTime.py
 danielutils/Exceptions.py
 danielutils/Functions.py
 danielutils/IO.py
 danielutils/Internet.py
 danielutils/Path.py
 danielutils/Print.py
-danielutils/Reflection.py
+danielutils/Relations.py
+danielutils/Signals.py
 danielutils/System.py
 danielutils/Text.py
 danielutils/Time.py
 danielutils/Windows.py
 danielutils/__init__.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
-danielutils.egg-info/requires.txt
 danielutils.egg-info/top_level.txt
 danielutils/Classes/Convenience.py
 danielutils/Classes/Counter.py
 danielutils/Classes/__init__.py
 danielutils/Classes/frange.py
 danielutils/Classes/TypedBuiltins/__init__.py
 danielutils/Classes/TypedBuiltins/tbase.py
@@ -56,22 +56,36 @@
 danielutils/Decorators/limit_recursion.py
 danielutils/Decorators/memo.py
 danielutils/Decorators/overload.py
 danielutils/Decorators/property.py
 danielutils/Decorators/threadify.py
 danielutils/Decorators/timeout.py
 danielutils/Decorators/validate.py
+danielutils/Functions/__init__.py
+danielutils/Functions/areoneof.py
+danielutils/Functions/check_foreach.py
+danielutils/Functions/isoftype.py
+danielutils/Functions/isoneof.py
+danielutils/Functions/types_subseteq.py
 danielutils/Generators/__init__.py
 danielutils/Generators/generator_from_stream.py
 danielutils/Generators/join_generators.py
 danielutils/Math/Constants.py
 danielutils/Math/Functions.py
 danielutils/Math/MathPrint.py
 danielutils/Math/MathSymbols.py
 danielutils/Math/__init__.py
 danielutils/MetaClasses/AtomicClassMeta.py
 danielutils/MetaClasses/ImplicitDataDeleterMeta.py
 danielutils/MetaClasses/InstanceCacheMeta.py
 danielutils/MetaClasses/Interface.py
+danielutils/MetaClasses/OverloadMeta.py
 danielutils/MetaClasses/__init__.py
+danielutils/Reflection/File.py
+danielutils/Reflection/Function.py
+danielutils/Reflection/Module.py
+danielutils/Reflection/System.py
+danielutils/Reflection/__init__.py
+danielutils/Reflection/_get_prev_frame.py
+danielutils/Reflection/get_traceback.py
 danielutils/Snippets/__init__.py
 danielutils/Snippets/try_get.py
```

### Comparing `danielutils-0.8.7/pyproject.toml` & `danielutils-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.8.7"
+version = "0.9.0"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
 requires-python = ">=3.10.5"
 classifiers = [
+   "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     # "Operating System :: Unix",
     # "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
 ]
```

### Comparing `danielutils-0.8.7/setup.py` & `danielutils-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,40 +5,35 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.8.7"
+VERSION = "0.9.0"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
-    long_description=open('README.md').read(),
+    long_description=open('README.md', "r", encoding="utf8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/danielnachumdev/danielutils',
     license="MIT License",
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests", "archive/"]),
-    install_requires=[
-        # "bs4",
-        #   "pyautogui",
-        "screeninfo",
-        "Pillow"
-    ],
+    install_requires=[],
     platforms=["All"],
-    keywords=['functions', 'decorators', 'methods'],
+    keywords=['functions', 'decorators', 'methods', 'classes', 'metaclasses'],
     classifiers=[
-        # "Development Status :: In development",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
+        # "Operating System :: Unix",
+        # "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
 # python .\setup.py sdist
 # twine upload dist/...
```

