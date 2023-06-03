# Comparing `tmp/Kekik-1.3.0.tar.gz` & `tmp/Kekik-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kekik-1.3.0.tar", last modified: Sun May 14 07:05:16 2023, max compression
+gzip compressed data, was "Kekik-1.3.1.tar", last modified: Sat Jun  3 15:49:42 2023, max compression
```

## Comparing `Kekik-1.3.0.tar` & `Kekik-1.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:16.126480 Kekik-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:16.122480 Kekik-1.3.0/Kekik/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/BIST.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/Nesne.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/csv2dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/dict2csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/dict2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/dosya2set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/dosya_indir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/hwid_kontrol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:16.126480 Kekik-1.3.0/Kekik/kisi_ver/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/kisi_ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189486 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/kisi_ver/biyografiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    88066 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/kisi_ver/isimler.py
--rw-r--r--   0 runner    (1001) docker     (123)    78485 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/kisi_ver/soyisimler.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/link_islemleri.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/list2html.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/liste_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/mail_gonder.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/okunabilir_byte.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/proxy_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/qr_ver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/ses_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/slugify.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/terminal_baslik.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/txt_fetis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/unicode_tr.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-14 07:04:53.000000 Kekik-1.3.0/Kekik/zaman_donustur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 07:05:16.122480 Kekik-1.3.0/Kekik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-14 07:05:15.000000 Kekik-1.3.0/Kekik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-14 07:05:15.000000 Kekik-1.3.0/Kekik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 07:05:15.000000 Kekik-1.3.0/Kekik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-14 07:05:15.000000 Kekik-1.3.0/Kekik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 07:05:15.000000 Kekik-1.3.0/Kekik.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 07:04:53.000000 Kekik-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 07:04:53.000000 Kekik-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-14 07:05:16.126480 Kekik-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-14 07:04:53.000000 Kekik-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 07:05:16.126480 Kekik-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-14 07:04:53.000000 Kekik-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:49:42.815023 Kekik-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:49:42.815023 Kekik-1.3.1/Kekik/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/BIST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/Nesne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/csv2dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/dict2csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/dict2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/dosya2set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/dosya_indir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/hwid_kontrol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:49:42.815023 Kekik-1.3.1/Kekik/kisi_ver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/kisi_ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189486 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/kisi_ver/biyografiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88066 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/kisi_ver/isimler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78485 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/kisi_ver/soyisimler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/link_islemleri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/list2html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/liste_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/mail_gonder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/okunabilir_byte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/proxy_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/qr_ver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/ses_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/slugify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/terminal_baslik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/txt_fetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/unicode_tr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-03 15:49:21.000000 Kekik-1.3.1/Kekik/zaman_donustur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:49:42.815023 Kekik-1.3.1/Kekik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-03 15:49:42.000000 Kekik-1.3.1/Kekik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-03 15:49:42.000000 Kekik-1.3.1/Kekik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:49:42.000000 Kekik-1.3.1/Kekik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-03 15:49:42.000000 Kekik-1.3.1/Kekik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 15:49:42.000000 Kekik-1.3.1/Kekik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 15:49:21.000000 Kekik-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 15:49:21.000000 Kekik-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-06-03 15:49:42.815023 Kekik-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-06-03 15:49:21.000000 Kekik-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:49:42.819023 Kekik-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-03 15:49:21.000000 Kekik-1.3.1/setup.py
```

### Comparing `Kekik-1.3.0/Kekik/BIST.py` & `Kekik-1.3.1/Kekik/BIST.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/Nesne.py` & `Kekik-1.3.1/Kekik/Nesne.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/__init__.py` & `Kekik-1.3.1/Kekik/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 ####
 from Kekik.slugify         import slugify
 from Kekik.unicode_tr      import unicode_tr
 from Kekik.link_islemleri  import link_ayikla, youtube_link_mi
 from Kekik.okunabilir_byte import okunabilir_byte
 from Kekik.zaman_donustur  import sure2saniye, zaman_donustur
 from Kekik.dict2json       import dict2json
-from Kekik.qr_ver          import qr_ver
-from Kekik.dosya_indir     import dosya_indir
+# from Kekik.qr_ver          import qr_ver
+# from Kekik.dosya_indir     import dosya_indir
 from Kekik.hwid_kontrol    import benim_hwid, hwid_kontrol
 from Kekik.txt_fetis       import satir_ekle, satirlar_ekle, satir_sil
 from Kekik.list2html       import list2html
 from Kekik.csv2dict        import csv2dict
 from Kekik.dict2csv        import dict2csv
 from Kekik.mail_gonder     import mail_gonder
 from Kekik.dosya2set       import dosya2set
 from Kekik.proxy_ver       import proxy_ver
-from Kekik.kisi_ver        import kisi_ver
+# from Kekik.kisi_ver        import kisi_ver
 from Kekik.Nesne           import Nesne
 from Kekik.terminal_baslik import terminal_baslik
 ####
```

### Comparing `Kekik-1.3.0/Kekik/cli.py` & `Kekik-1.3.1/Kekik/cli.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/dict2csv.py` & `Kekik-1.3.1/Kekik/dict2csv.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/dict2json.py` & `Kekik-1.3.1/Kekik/dict2json.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/dosya_indir.py` & `Kekik-1.3.1/Kekik/dosya_indir.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/hwid_kontrol.py` & `Kekik-1.3.1/Kekik/hwid_kontrol.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/kisi_ver/__init__.py` & `Kekik-1.3.1/Kekik/kisi_ver/__init__.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/kisi_ver/biyografiler.py` & `Kekik-1.3.1/Kekik/kisi_ver/biyografiler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/kisi_ver/isimler.py` & `Kekik-1.3.1/Kekik/kisi_ver/isimler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/kisi_ver/soyisimler.py` & `Kekik-1.3.1/Kekik/kisi_ver/soyisimler.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/link_islemleri.py` & `Kekik-1.3.1/Kekik/link_islemleri.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/list2html.py` & `Kekik-1.3.1/Kekik/list2html.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/mail_gonder.py` & `Kekik-1.3.1/Kekik/mail_gonder.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/okunabilir_byte.py` & `Kekik-1.3.1/Kekik/okunabilir_byte.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/proxy_ver.py` & `Kekik-1.3.1/Kekik/proxy_ver.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/qr_ver.py` & `Kekik-1.3.1/Kekik/qr_ver.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/ses_fetis.py` & `Kekik-1.3.1/Kekik/ses_fetis.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/slugify.py` & `Kekik-1.3.1/Kekik/slugify.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/terminal_baslik.py` & `Kekik-1.3.1/Kekik/terminal_baslik.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/txt_fetis.py` & `Kekik-1.3.1/Kekik/txt_fetis.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/unicode_tr.py` & `Kekik-1.3.1/Kekik/unicode_tr.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik/zaman_donustur.py` & `Kekik-1.3.1/Kekik/zaman_donustur.py`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/Kekik.egg-info/PKG-INFO` & `Kekik-1.3.1/Kekik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kekik
-Version: 1.3.0
+Version: 1.3.1
 Summary: İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..
 Home-page: https://github.com/keyiflerolsun/Kekik
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Kekik,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Kekik Version: 1.3.0 Summary: Ä°Ålerimizi
+Metadata-Version: 2.1 Name: Kekik Version: 1.3.1 Summary: Ä°Ålerimizi
 kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane.. Home-page:
 https://github.com/keyiflerolsun/Kekik Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 Kekik,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `Kekik-1.3.0/Kekik.egg-info/SOURCES.txt` & `Kekik-1.3.1/Kekik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/LICENSE` & `Kekik-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/PKG-INFO` & `Kekik-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kekik
-Version: 1.3.0
+Version: 1.3.1
 Summary: İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..
 Home-page: https://github.com/keyiflerolsun/Kekik
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: Kekik,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Kekik Version: 1.3.0 Summary: Ä°Ålerimizi
+Metadata-Version: 2.1 Name: Kekik Version: 1.3.1 Summary: Ä°Ålerimizi
 kolaylaÅtÄ±racak fonksiyonlarÄ±n el altÄ±nda durduÄu kÃ¼tÃ¼phane.. Home-page:
 https://github.com/keyiflerolsun/Kekik Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 Kekik,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `Kekik-1.3.0/README.md` & `Kekik-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Kekik-1.3.0/setup.py` & `Kekik-1.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "Kekik",
-    version      = "1.3.0",
+    version      = "1.3.1",
     url          = "https://github.com/keyiflerolsun/Kekik",
     description  = "İşlerimizi kolaylaştıracak fonksiyonların el altında durduğu kütüphane..",
     keywords     = ["Kekik", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -34,19 +34,19 @@
         "httpx",
         "parsel",
         "cssselect",
         # "thispersondoesnotexist",
         "simplejson",
         "rich",
         "tabulate",
-        "tqdm",
-        "qrcode",
-        "pyfiglet",
-        "Pillow",
-        "notify-py",
+        # "tqdm",
+        # "qrcode",
+        # "pyfiglet",
+        # "Pillow",
+        # "notify-py",
         # "py3-validate-email"
     ],
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
```

