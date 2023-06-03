# Comparing `tmp/anticaptchaofficial-1.0.51-py3-none-any.whl.zip` & `tmp/anticaptchaofficial-1.0.52-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 17501 bytes, number of entries: 23
+Zip file size: 17490 bytes, number of entries: 23
 -rw-r--r--  2.0 unx      172 b- defN 20-Mar-11 07:55 anticaptchaofficial/__init__.py
 -rw-r--r--  2.0 unx     1013 b- defN 23-Jan-07 03:37 anticaptchaofficial/antibotcookietask.py
 -rw-r--r--  2.0 unx     2720 b- defN 22-Sep-27 14:01 anticaptchaofficial/antigatetask.py
 -rw-r--r--  2.0 unx     6743 b- defN 23-May-24 09:17 anticaptchaofficial/antinetworking.py
 -rw-r--r--  2.0 unx     1149 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyless.py
 -rw-r--r--  2.0 unx     1430 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyon.py
 -rw-r--r--  2.0 unx     1619 b- defN 22-Jun-01 07:46 anticaptchaofficial/geetestproxyless.py
@@ -14,12 +14,12 @@
 -rw-r--r--  2.0 unx     1278 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2enterpriseproxyon.py
 -rw-r--r--  2.0 unx     1045 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyless.py
 -rw-r--r--  2.0 unx     1339 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyon.py
 -rw-r--r--  2.0 unx     1318 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3enterpriseproxyless.py
 -rw-r--r--  2.0 unx     1270 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3proxyless.py
 -rw-r--r--  2.0 unx      943 b- defN 23-May-24 09:17 anticaptchaofficial/turnstileproxyless.py
 -rw-r--r--  2.0 unx     1252 b- defN 23-May-24 09:17 anticaptchaofficial/turnstileproxyon.py
--rw-r--r--  2.0 unx     9734 b- defN 23-May-24 09:18 anticaptchaofficial-1.0.51.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-24 09:18 anticaptchaofficial-1.0.51.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-24 09:18 anticaptchaofficial-1.0.51.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2208 b- defN 23-May-24 09:18 anticaptchaofficial-1.0.51.dist-info/RECORD
-23 files, 42657 bytes uncompressed, 13815 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx     9712 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2208 b- defN 23-Jun-03 08:32 anticaptchaofficial-1.0.52.dist-info/RECORD
+23 files, 42635 bytes uncompressed, 13804 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: anticaptchaofficial/turnstileproxyless.py
 Comment: 
 
 Filename: anticaptchaofficial/turnstileproxyon.py
 Comment: 
 
-Filename: anticaptchaofficial-1.0.51.dist-info/METADATA
+Filename: anticaptchaofficial-1.0.52.dist-info/METADATA
 Comment: 
 
-Filename: anticaptchaofficial-1.0.51.dist-info/WHEEL
+Filename: anticaptchaofficial-1.0.52.dist-info/WHEEL
 Comment: 
 
-Filename: anticaptchaofficial-1.0.51.dist-info/top_level.txt
+Filename: anticaptchaofficial-1.0.52.dist-info/top_level.txt
 Comment: 
 
-Filename: anticaptchaofficial-1.0.51.dist-info/RECORD
+Filename: anticaptchaofficial-1.0.52.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `anticaptchaofficial-1.0.51.dist-info/METADATA` & `anticaptchaofficial-1.0.52.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: anticaptchaofficial
-Version: 1.0.51
+Version: 1.0.52
 Summary: Official anti-captcha.com library
-Home-page: https://github.com/AdminAnticaptcha/anticaptcha-python
+Home-page: https://git.anti-captcha.com/sup/anticaptcha-python
 Author: Anti Admin
 Author-email: admin@anti-captcha.com
 License: MIT
 Keywords: anticaptcha anti captcha recognition solve bypass recaptcha enterprise funcaptcha arkoselabs geetest hcaptcha antigate turnstile
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: py (>=1.4.32)
 Requires-Dist: requests (>=2.22.0)
 
 anticaptchaofficial
 ===================
 
@@ -336,8 +335,7 @@
 
 ---
 Useful links:
 - [Как решить рекапчу автоматически](https://anti-captcha.com/ru/apidoc/task-types/RecaptchaV2TaskProxyless)
 - [Обход капчи](https://anti-captcha.com/ru/apidoc/task-types/ImageToTextTask)
 - [Cómo resolver un recaptcha automáticamente](https://anti-captcha.com/es/apidoc/task-types/RecaptchaV2TaskProxyless)
 - [Como resolver um recaptcha automaticamente](https://anti-captcha.com/pt/apidoc/task-types/RecaptchaV2TaskProxyless)
-
```

## Comparing `anticaptchaofficial-1.0.51.dist-info/RECORD` & `anticaptchaofficial-1.0.52.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 anticaptchaofficial/recaptchav2enterpriseproxyon.py,sha256=p7sdV0qHScbrIrhw00624pH_2hQeG95RTGjRQDutxs4,1278
 anticaptchaofficial/recaptchav2proxyless.py,sha256=12fviOgw1waeeRbyzwvSctIoc1w3qCBYJY7GYi0FSJc,1045
 anticaptchaofficial/recaptchav2proxyon.py,sha256=KKjm72dfxdCChyj3Qn5y5Twm8qT3sZsvSGSfjbdrIM8,1339
 anticaptchaofficial/recaptchav3enterpriseproxyless.py,sha256=exQ-sgvOdcSpsh0mWsUDKEGudM4k23SrROVZ9p0pU5M,1318
 anticaptchaofficial/recaptchav3proxyless.py,sha256=Fv0nfDG-Jp8Vzz8C4-vccz3BJ0hm89MTAs3y9Okzctw,1270
 anticaptchaofficial/turnstileproxyless.py,sha256=nK737Ccr8mZy0_CL6_gB1P5UiCWLaJ0gM9SoCVshMpg,943
 anticaptchaofficial/turnstileproxyon.py,sha256=0HpomUlH1PuLglzrtMBEu5R4287oE3cpp3QnsDhfF2k,1252
-anticaptchaofficial-1.0.51.dist-info/METADATA,sha256=IJQRV7AAtEvwbP0iUt5vmbiEmoIRTaEQqGlGnSI61IM,9734
-anticaptchaofficial-1.0.51.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-anticaptchaofficial-1.0.51.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
-anticaptchaofficial-1.0.51.dist-info/RECORD,,
+anticaptchaofficial-1.0.52.dist-info/METADATA,sha256=ps0gFvyNGFaNyDcK3g766bH4vBt_uhUGSrrtAw6IecU,9712
+anticaptchaofficial-1.0.52.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+anticaptchaofficial-1.0.52.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
+anticaptchaofficial-1.0.52.dist-info/RECORD,,
```

