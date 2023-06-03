# Comparing `tmp/nonebot_plugin_watermarker-0.1.5.1.tar.gz` & `tmp/nonebot_plugin_watermarker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_watermarker-0.1.5.1.tar", last modified: Sat May 13 13:43:23 2023, max compression
+gzip compressed data, was "nonebot_plugin_watermarker-0.2.0.tar", last modified: Sat Jun  3 12:05:36 2023, max compression
```

## Comparing `nonebot_plugin_watermarker-0.1.5.1.tar` & `nonebot_plugin_watermarker-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 13:43:23.408734 nonebot_plugin_watermarker-0.1.5.1/
--rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot_plugin_watermarker-0.1.5.1/LICENSE
--rw-rw-rw-   0        0        0     4002 2023-05-13 13:43:23.403748 nonebot_plugin_watermarker-0.1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3644 2023-05-02 00:05:20.000000 nonebot_plugin_watermarker-0.1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 13:43:23.375825 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker/
--rw-rw-rw-   0        0        0     2125 2023-05-13 13:15:02.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker/__init__.py
--rw-rw-rw-   0        0        0      842 2023-05-01 09:25:17.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker/config.py
--rw-rw-rw-   0        0        0     2366 2023-05-13 13:40:22.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker/fuctions.py
-drwxrwxrwx   0        0        0        0 2023-05-13 13:43:23.400756 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker.egg-info/
--rw-rw-rw-   0        0        0     4002 2023-05-13 13:43:23.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-13 13:43:23.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 13:43:23.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-13 13:43:23.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-13 13:43:23.000000 nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 13:43:23.408734 nonebot_plugin_watermarker-0.1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     4210 2023-05-13 13:43:18.000000 nonebot_plugin_watermarker-0.1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:05:36.983851 nonebot_plugin_watermarker-0.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-05-01 12:04:12.000000 nonebot_plugin_watermarker-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4467 2023-06-03 12:05:36.982856 nonebot_plugin_watermarker-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4109 2023-06-03 11:55:26.000000 nonebot_plugin_watermarker-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 12:05:36.968893 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker/
+-rw-rw-rw-   0        0        0     1454 2023-06-03 11:43:49.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-06-03 11:26:27.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker/config.py
+-rw-rw-rw-   0        0        0     4917 2023-06-03 11:55:20.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker/fuctions.py
+drwxrwxrwx   0        0        0        0 2023-06-03 12:05:36.980866 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker.egg-info/
+-rw-rw-rw-   0        0        0     4467 2023-06-03 12:05:36.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-06-03 12:05:36.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 12:05:36.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-03 12:05:36.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-03 12:05:36.000000 nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 12:05:36.983851 nonebot_plugin_watermarker-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     4675 2023-06-03 12:05:32.000000 nonebot_plugin_watermarker-0.2.0/setup.py
```

### Comparing `nonebot_plugin_watermarker-0.1.5.1/LICENSE` & `nonebot_plugin_watermarker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_watermarker-0.1.5.1/PKG-INFO` & `nonebot_plugin_watermarker-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_watermarker
-Version: 0.1.5.1
+Version: 0.2.0
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -50,27 +50,27 @@
 ## 💿安装方法
 ### ```nb脚手架```
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```cmd
-nb plugin install nonebot_piugin_watermarker
+nb plugin install nonebot-piugin-watermarker
 ```
 
 </details>
 
 ### ```pip```
 <details>
 <summary>pip安装</summary>
 
 命令行输入以下命令
 
 ```cmd
-pip install nonebot_plugin_watermarker
+pip install nonebot-plugin-watermarker
 ```
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_rename"]
 
 ```
@@ -78,19 +78,19 @@
 plugins = []
 plugin_dirs = ["src/plugins"]
 ```
 </details>
 
 ##  ⚙插件配置项
 
-| 变量名      |       变量类型    |   变量概述       |
-|------------|----------------------------------|----------------|
-| ```watermark_image_path```   |```str```|水印图片存放目录,目录下的所有水印图片会被随机选取|
-| ```watermark_image_size```   |```float```|水印相对图片的大小(保持水印原来的形状)|
-| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件(未完工)|
+|  变量名                                 | 变量类型      |          变量概述                             |    使用示例   |
+|----------------------------------------|---------------|----------------------------------------------|-----------------|
+| ```watermark_image_path```             |```str```      |水印图片存放目录,目录下的所有水印图片会被随机选取 | ```F:\image``` |
+| ```watermark_image_size```             |```float```    |水印相对图片的大小(保持水印原来的形状)|```0.15```|
+| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件                      |```[插件位置.plugins.插件名称]```(如```src.plugins.nonebot_plugin_petpet```)
 
 ## 🎉目前已实现的功能
 
 ### 加水印捏
 <details>
 <summary>效果图</summary>
 
@@ -100,25 +100,29 @@
 
 ![G37PR_ KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)
 
 </details>
 
 ## 💡待实现的功能
 
-1. -[ ] 对特定的插件的图片不进行贴水印操作
-2. -[ ] 待补充.....
+1. -[x] 对特定的插件的图片不进行贴水印操作
+2. -[x] 对GIF图片进行适配
+3. -[ ] 更多不同的贴水印方式
+4. -[ ] 贴图片怎么够,我要贴文字!
+5. -[ ] 待补充.....
 
 # 💣已知bug
 
-水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(
+水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(已解决,base64解码问题,为末位不足位没有补上=)
 
 # 🔥鸣谢
 
 [Nonebot2](https://github.com/nonebot/nonebot2),不用说,没有Nonebot就没有这个插件
 
 ~~[我自己](https://github.com/X-Skirt-X),因为我做的PoweredByNonebot的Logo~~
 
 # 💦其他
 
 没有其他,想到再补
 
 
+
```

#### html2text {}

```diff
@@ -1,41 +1,47 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_watermarker Version: 0.1.5.1
-Summary: ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://
-github.com/X-Skirt-X/nonebot-plugin-watermarker Author: XU Author-email:
-Woyerpa@outlook.com License: MIT License Platform: UNKNOWN Description-Content-
-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: nonebot_plugin_watermarker Version: 0.2.0 Summary:
+ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
+Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
+License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
+License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-watermarker _â¨ ä¸ºä½ çbotååºçå¾çæ·»å æ°´å°! â¨_
                            [license] [pypi] [python]
  * [ðç®ä»](#ç®ä») * [ð¿ å®è£æ¹æ³](#å®è£æ¹æ³) *
 [âï¸æä»¶éç½®é¡¹](#æä»¶éç½®é¡¹) * [ðç®åå·²å®ç°çåè½]
 (#ç®åå·²å®ç°çåè½) * [ð¡å¾å®ç°çåè½](#å¾å®ç°çåè½) *
 [ð£å·²ç¥bug](#å·²ç¥bug) * [ð¥é¸£è°¢](#é¸£è°¢) * [ð¦å¶ä»](#å¶ä»)  ##
 ðç®ä» ä¸ºbotååºçææå¾çé½å ä¸æ°´å°
 (æçæ¶åæ°´å°å¾ç¦,ä½æ¯å¸æ°çæ°´å°è½å¢å å¾ççç¾æ,ä¸æ¯å?)
 ## ð¿å®è£æ¹æ³ ### ```nbèææ¶```  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```cmd nb
-plugin install nonebot_piugin_watermarker ```  ### ```pip```  pipå®è£
-å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot_plugin_watermarker ```
+plugin install nonebot-piugin-watermarker ```  ### ```pip```  pipå®è£
+å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot-plugin-watermarker ```
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_rename"] ```
 [tool.nonebot] plugins = [] plugin_dirs = ["src/plugins"] ```  ##
-âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | |------------|--
---------------------------------|----------------| | ```watermark_image_path```
-|```str```|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå|
-| ```watermark_image_size``` |```float```|æ°´å°ç¸å¯¹å¾ççå¤§å°
-(ä¿ææ°´å°åæ¥çå½¢ç¶)| | ```watermark_image_exculed_plugin``` |```List
-[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶(æªå®å·¥)| ##
-ðç®åå·²å®ç°çåè½ ### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{
-{XBE](https://user-images.githubusercontent.com/91937041/235442049-67ac0b4c-
-1629-4d78-9858-8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_
-KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-
-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[ ]
-å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[ ] å¾è¡¥å..... #
-ð£å·²ç¥bug
+âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | ä½¿ç¨ç¤ºä¾ |
+|----------------------------------------|---------------|---------------------
+-------------------------|-----------------| | ```watermark_image_path```
+|```str```
+|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå |
+```F:\image``` | | ```watermark_image_size``` |```float```
+|æ°´å°ç¸å¯¹å¾ççå¤§å°(ä¿ææ°´å°åæ¥çå½¢ç¶)|```0.15```| |
+```watermark_image_exculed_plugin``` |```List
+[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶ |```[æä»¶ä½ç½®.plugins.æä»¶åç§°]```
+(å¦```src.plugins.nonebot_plugin_petpet```) ## ðç®åå·²å®ç°çåè½
+### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{{XBE](https://user-
+images.githubusercontent.com/91937041/235442049-67ac0b4c-1629-4d78-9858-
+8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_ KAWEUINI_ _B)H2E]
+(https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-
+4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[x]
+å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[x]
+å¯¹GIFå¾çè¿è¡éé 3. -[ ] æ´å¤ä¸åçè´´æ°´å°æ¹å¼ 4. -[ ]
+è´´å¾çæä¹å¤,æè¦è´´æå­! 5. -[ ] å¾è¡¥å..... # ð£å·²ç¥bug
 æ°´å°å°æ¦çè´´ä¸ä¸,åºè¯¥æ¯base64çåå ,ä½æ¯æä¸ç´æ¾ä¸å°çæ­£çé®é¢æº,å ä¸ºææ¶åè´´çä¸ææ¶åè´´ä¸ä¸
-( # ð¥é¸£è°¢ [Nonebot2](https://github.com/nonebot/
+(å·²è§£å³,base64è§£ç é®é¢,ä¸ºæ«ä½ä¸è¶³ä½æ²¡æè¡¥ä¸=) # ð¥é¸£è°¢
+[Nonebot2](https://github.com/nonebot/
 nonebot2),ä¸ç¨è¯´,æ²¡æNonebotå°±æ²¡æè¿ä¸ªæä»¶ ~~[æèªå·±](https://
 github.com/X-Skirt-X),å ä¸ºæåçPoweredByNonebotçLogo~~ # ð¦å¶ä»
 æ²¡æå¶ä»,æ³å°åè¡¥
```

### Comparing `nonebot_plugin_watermarker-0.1.5.1/README.md` & `nonebot_plugin_watermarker-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,19 +66,19 @@
 plugins = []
 plugin_dirs = ["src/plugins"]
 ```
 </details>
 
 ##  ⚙插件配置项
 
-| 变量名      |       变量类型    |   变量概述       |
-|------------|----------------------------------|----------------|
-| ```watermark_image_path```   |```str```|水印图片存放目录,目录下的所有水印图片会被随机选取|
-| ```watermark_image_size```   |```float```|水印相对图片的大小(保持水印原来的形状)|
-| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件(未完工)|
+|  变量名                                 | 变量类型      |          变量概述                             |    使用示例   |
+|----------------------------------------|---------------|----------------------------------------------|-----------------|
+| ```watermark_image_path```             |```str```      |水印图片存放目录,目录下的所有水印图片会被随机选取 | ```F:\image``` |
+| ```watermark_image_size```             |```float```    |水印相对图片的大小(保持水印原来的形状)|```0.15```|
+| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件                      |```[插件位置.plugins.插件名称]```(如```src.plugins.nonebot_plugin_petpet```)
 
 ## 🎉目前已实现的功能
 
 ### 加水印捏
 <details>
 <summary>效果图</summary>
 
@@ -88,20 +88,23 @@
 
 ![G37PR_ KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)
 
 </details>
 
 ## 💡待实现的功能
 
-1. -[ ] 对特定的插件的图片不进行贴水印操作
-2. -[ ] 待补充.....
+1. -[x] 对特定的插件的图片不进行贴水印操作
+2. -[x] 对GIF图片进行适配
+3. -[ ] 更多不同的贴水印方式
+4. -[ ] 贴图片怎么够,我要贴文字!
+5. -[ ] 待补充.....
 
 # 💣已知bug
 
-水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(
+水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(已解决,base64解码问题,为末位不足位没有补上=)
 
 # 🔥鸣谢
 
 [Nonebot2](https://github.com/nonebot/nonebot2),不用说,没有Nonebot就没有这个插件
 
 ~~[我自己](https://github.com/X-Skirt-X),因为我做的PoweredByNonebot的Logo~~
```

#### html2text {}

```diff
@@ -12,25 +12,31 @@
 ## ð¿å®è£æ¹æ³ ### ```nbèææ¶```  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```cmd nb
 plugin install nonebot-piugin-watermarker ```  ### ```pip```  pipå®è£
 å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot-plugin-watermarker ```
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_rename"] ```
 [tool.nonebot] plugins = [] plugin_dirs = ["src/plugins"] ```  ##
-âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | |------------|--
---------------------------------|----------------| | ```watermark_image_path```
-|```str```|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå|
-| ```watermark_image_size``` |```float```|æ°´å°ç¸å¯¹å¾ççå¤§å°
-(ä¿ææ°´å°åæ¥çå½¢ç¶)| | ```watermark_image_exculed_plugin``` |```List
-[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶(æªå®å·¥)| ##
-ðç®åå·²å®ç°çåè½ ### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{
-{XBE](https://user-images.githubusercontent.com/91937041/235442049-67ac0b4c-
-1629-4d78-9858-8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_
-KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-
-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[ ]
-å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[ ] å¾è¡¥å..... #
-ð£å·²ç¥bug
+âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | ä½¿ç¨ç¤ºä¾ |
+|----------------------------------------|---------------|---------------------
+-------------------------|-----------------| | ```watermark_image_path```
+|```str```
+|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå |
+```F:\image``` | | ```watermark_image_size``` |```float```
+|æ°´å°ç¸å¯¹å¾ççå¤§å°(ä¿ææ°´å°åæ¥çå½¢ç¶)|```0.15```| |
+```watermark_image_exculed_plugin``` |```List
+[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶ |```[æä»¶ä½ç½®.plugins.æä»¶åç§°]```
+(å¦```src.plugins.nonebot_plugin_petpet```) ## ðç®åå·²å®ç°çåè½
+### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{{XBE](https://user-
+images.githubusercontent.com/91937041/235442049-67ac0b4c-1629-4d78-9858-
+8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_ KAWEUINI_ _B)H2E]
+(https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-
+4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[x]
+å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[x]
+å¯¹GIFå¾çè¿è¡éé 3. -[ ] æ´å¤ä¸åçè´´æ°´å°æ¹å¼ 4. -[ ]
+è´´å¾çæä¹å¤,æè¦è´´æå­! 5. -[ ] å¾è¡¥å..... # ð£å·²ç¥bug
 æ°´å°å°æ¦çè´´ä¸ä¸,åºè¯¥æ¯base64çåå ,ä½æ¯æä¸ç´æ¾ä¸å°çæ­£çé®é¢æº,å ä¸ºææ¶åè´´çä¸ææ¶åè´´ä¸ä¸
-( # ð¥é¸£è°¢ [Nonebot2](https://github.com/nonebot/
+(å·²è§£å³,base64è§£ç é®é¢,ä¸ºæ«ä½ä¸è¶³ä½æ²¡æè¡¥ä¸=) # ð¥é¸£è°¢
+[Nonebot2](https://github.com/nonebot/
 nonebot2),ä¸ç¨è¯´,æ²¡æNonebotå°±æ²¡æè¿ä¸ªæä»¶ ~~[æèªå·±](https://
 github.com/X-Skirt-X),å ä¸ºæåçPoweredByNonebotçLogo~~ # ð¦å¶ä»
 æ²¡æå¶ä»,æ³å°åè¡¥
```

### Comparing `nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker/__init__.py` & `nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-import base64
-import random
-
-from PIL import Image
-from io import BytesIO
 from typing import Dict, Any
 from dataclasses import asdict
-from contextvars import copy_context
 
 from nonebot.log import logger
 from nonebot.plugin import PluginMetadata
 from nonebot.adapters import Bot
-
+from nonebot.internal.matcher import current_matcher
 from .config import *
 from .fuctions import *
 
 image_dirs = get_image_dirs(config.watermark_image_path)
 
 __plugin_meta__ = PluginMetadata(
     name="图片水印",
@@ -24,38 +18,25 @@
 )
 
 
 @Bot.on_calling_api
 async def _handle(bot: Bot, api: str, data: Dict[str, Any]):
     if api not in ["send_msg", "send_message"]:
         return
+    if i := current_matcher.get().module_name:
+        if i in config.watermark_image_exculed_plugin:
+            return
+
     logger.debug("handle start")
     for i in range(len(data["message"])):
         image_data = asdict(data["message"][i])
-        if image_data["type"] != "image":
-            continue
-        file = image_data["data"]["file"]
-        if image := await str2img(file):
-            image_size = image.size
-            watermark_path = random.choice(image_dirs)
-            watermark = Image.open(watermark_path)
-            mix = tuple([int((k + j) / 2) for k, j in zip(watermark.size, image_size)])
-            watermark_size = tuple([int(k * config.watermark_image_size) for k in mix])
-            watermark_position = tuple(
-                [k - j for k, j in zip(image_size, watermark_size)]
-            )
-            watermark.thumbnail(watermark_size)
-            logger.debug(f"watermark_size:{watermark_size}\nimage_size:{image_size}")
-            image = image.convert("RGBA")
-            watermark = watermark.convert("RGBA")
-            mask = watermark.split()[3]
-
-            image.paste(watermark, watermark_position, mask)
-
-            buffered = BytesIO()
-            image.save(buffered, format="PNG")
-            byte_data = buffered.getvalue()
-            base64_str = base64.b64encode(byte_data).decode("utf-8")
+        if image_data["type"] != "image":continue
+        #有减少嵌套的方法记得踹我
+        if image := await str2img(image_data["data"]["file"]):
+            if image.format == 'GIF':
+                base64_str = watermark_on_gif(image)
+            else:
+                base64_str = watermark_on_jpg(image)
             data["message"][i].data["file"] = "base64://" + base64_str
 
         else:
-            logger.debug(file)
+            logger.debug("这是一个代表图片的东西吗???:\n"+image_data["data"]["file"][:50])
```

### Comparing `nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker/config.py` & `nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_watermarker-0.1.5.1/nonebot_plugin_watermarker.egg-info/PKG-INFO` & `nonebot_plugin_watermarker-0.2.0/nonebot_plugin_watermarker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-watermarker
-Version: 0.1.5.1
+Version: 0.2.0
 Summary: 为nonebot机器人发送的图片加上水印
 Home-page: https://github.com/X-Skirt-X/nonebot-plugin-watermarker
 Author: XU
 Author-email: Woyerpa@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -50,27 +50,27 @@
 ## 💿安装方法
 ### ```nb脚手架```
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```cmd
-nb plugin install nonebot_piugin_watermarker
+nb plugin install nonebot-piugin-watermarker
 ```
 
 </details>
 
 ### ```pip```
 <details>
 <summary>pip安装</summary>
 
 命令行输入以下命令
 
 ```cmd
-pip install nonebot_plugin_watermarker
+pip install nonebot-plugin-watermarker
 ```
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_rename"]
 
 ```
@@ -78,19 +78,19 @@
 plugins = []
 plugin_dirs = ["src/plugins"]
 ```
 </details>
 
 ##  ⚙插件配置项
 
-| 变量名      |       变量类型    |   变量概述       |
-|------------|----------------------------------|----------------|
-| ```watermark_image_path```   |```str```|水印图片存放目录,目录下的所有水印图片会被随机选取|
-| ```watermark_image_size```   |```float```|水印相对图片的大小(保持水印原来的形状)|
-| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件(未完工)|
+|  变量名                                 | 变量类型      |          变量概述                             |    使用示例   |
+|----------------------------------------|---------------|----------------------------------------------|-----------------|
+| ```watermark_image_path```             |```str```      |水印图片存放目录,目录下的所有水印图片会被随机选取 | ```F:\image``` |
+| ```watermark_image_size```             |```float```    |水印相对图片的大小(保持水印原来的形状)|```0.15```|
+| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件                      |```[插件位置.plugins.插件名称]```(如```src.plugins.nonebot_plugin_petpet```)
 
 ## 🎉目前已实现的功能
 
 ### 加水印捏
 <details>
 <summary>效果图</summary>
 
@@ -100,25 +100,29 @@
 
 ![G37PR_ KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)
 
 </details>
 
 ## 💡待实现的功能
 
-1. -[ ] 对特定的插件的图片不进行贴水印操作
-2. -[ ] 待补充.....
+1. -[x] 对特定的插件的图片不进行贴水印操作
+2. -[x] 对GIF图片进行适配
+3. -[ ] 更多不同的贴水印方式
+4. -[ ] 贴图片怎么够,我要贴文字!
+5. -[ ] 待补充.....
 
 # 💣已知bug
 
-水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(
+水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(已解决,base64解码问题,为末位不足位没有补上=)
 
 # 🔥鸣谢
 
 [Nonebot2](https://github.com/nonebot/nonebot2),不用说,没有Nonebot就没有这个插件
 
 ~~[我自己](https://github.com/X-Skirt-X),因为我做的PoweredByNonebot的Logo~~
 
 # 💦其他
 
 没有其他,想到再补
 
 
+
```

#### html2text {}

```diff
@@ -1,41 +1,47 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.1.5.1
-Summary: ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://
-github.com/X-Skirt-X/nonebot-plugin-watermarker Author: XU Author-email:
-Woyerpa@outlook.com License: MIT License Platform: UNKNOWN Description-Content-
-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: nonebot-plugin-watermarker Version: 0.2.0 Summary:
+ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å° Home-page: https://github.com/X-
+Skirt-X/nonebot-plugin-watermarker Author: XU Author-email: Woyerpa@outlook.com
+License: MIT License Platform: UNKNOWN Description-Content-Type: text/markdown
+License-File: LICENSE
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-watermarker _â¨ ä¸ºä½ çbotååºçå¾çæ·»å æ°´å°! â¨_
                            [license] [pypi] [python]
  * [ðç®ä»](#ç®ä») * [ð¿ å®è£æ¹æ³](#å®è£æ¹æ³) *
 [âï¸æä»¶éç½®é¡¹](#æä»¶éç½®é¡¹) * [ðç®åå·²å®ç°çåè½]
 (#ç®åå·²å®ç°çåè½) * [ð¡å¾å®ç°çåè½](#å¾å®ç°çåè½) *
 [ð£å·²ç¥bug](#å·²ç¥bug) * [ð¥é¸£è°¢](#é¸£è°¢) * [ð¦å¶ä»](#å¶ä»)  ##
 ðç®ä» ä¸ºbotååºçææå¾çé½å ä¸æ°´å°
 (æçæ¶åæ°´å°å¾ç¦,ä½æ¯å¸æ°çæ°´å°è½å¢å å¾ççç¾æ,ä¸æ¯å?)
 ## ð¿å®è£æ¹æ³ ### ```nbèææ¶```  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```cmd nb
-plugin install nonebot_piugin_watermarker ```  ### ```pip```  pipå®è£
-å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot_plugin_watermarker ```
+plugin install nonebot-piugin-watermarker ```  ### ```pip```  pipå®è£
+å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot-plugin-watermarker ```
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_rename"] ```
 [tool.nonebot] plugins = [] plugin_dirs = ["src/plugins"] ```  ##
-âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | |------------|--
---------------------------------|----------------| | ```watermark_image_path```
-|```str```|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå|
-| ```watermark_image_size``` |```float```|æ°´å°ç¸å¯¹å¾ççå¤§å°
-(ä¿ææ°´å°åæ¥çå½¢ç¶)| | ```watermark_image_exculed_plugin``` |```List
-[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶(æªå®å·¥)| ##
-ðç®åå·²å®ç°çåè½ ### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{
-{XBE](https://user-images.githubusercontent.com/91937041/235442049-67ac0b4c-
-1629-4d78-9858-8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_
-KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-
-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[ ]
-å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[ ] å¾è¡¥å..... #
-ð£å·²ç¥bug
+âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | ä½¿ç¨ç¤ºä¾ |
+|----------------------------------------|---------------|---------------------
+-------------------------|-----------------| | ```watermark_image_path```
+|```str```
+|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå |
+```F:\image``` | | ```watermark_image_size``` |```float```
+|æ°´å°ç¸å¯¹å¾ççå¤§å°(ä¿ææ°´å°åæ¥çå½¢ç¶)|```0.15```| |
+```watermark_image_exculed_plugin``` |```List
+[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶ |```[æä»¶ä½ç½®.plugins.æä»¶åç§°]```
+(å¦```src.plugins.nonebot_plugin_petpet```) ## ðç®åå·²å®ç°çåè½
+### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{{XBE](https://user-
+images.githubusercontent.com/91937041/235442049-67ac0b4c-1629-4d78-9858-
+8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_ KAWEUINI_ _B)H2E]
+(https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-
+4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[x]
+å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[x]
+å¯¹GIFå¾çè¿è¡éé 3. -[ ] æ´å¤ä¸åçè´´æ°´å°æ¹å¼ 4. -[ ]
+è´´å¾çæä¹å¤,æè¦è´´æå­! 5. -[ ] å¾è¡¥å..... # ð£å·²ç¥bug
 æ°´å°å°æ¦çè´´ä¸ä¸,åºè¯¥æ¯base64çåå ,ä½æ¯æä¸ç´æ¾ä¸å°çæ­£çé®é¢æº,å ä¸ºææ¶åè´´çä¸ææ¶åè´´ä¸ä¸
-( # ð¥é¸£è°¢ [Nonebot2](https://github.com/nonebot/
+(å·²è§£å³,base64è§£ç é®é¢,ä¸ºæ«ä½ä¸è¶³ä½æ²¡æè¡¥ä¸=) # ð¥é¸£è°¢
+[Nonebot2](https://github.com/nonebot/
 nonebot2),ä¸ç¨è¯´,æ²¡æNonebotå°±æ²¡æè¿ä¸ªæä»¶ ~~[æèªå·±](https://
 github.com/X-Skirt-X),å ä¸ºæåçPoweredByNonebotçLogo~~ # ð¦å¶ä»
 æ²¡æå¶ä»,æ³å°åè¡¥
```

### Comparing `nonebot_plugin_watermarker-0.1.5.1/setup.py` & `nonebot_plugin_watermarker-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
     
 setup(
     name='nonebot_plugin_watermarker',
 
-    version="0.1.5.1",
+    version="0.2.0",
     description=(
         '为nonebot机器人发送的图片加上水印'
 
     ),
     long_description="""<div align="center">
   <p><img src="https://user-images.githubusercontent.com/91937041/235443858-85949be1-08d6-4d7a-b132-b1aed71ab943.png" width="560" alt="PoweredByNonebotLogo"></p>
   <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
@@ -49,27 +49,27 @@
 ## 💿安装方法
 ### ```nb脚手架```
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
 ```cmd
-nb plugin install nonebot_piugin_watermarker
+nb plugin install nonebot-piugin-watermarker
 ```
 
 </details>
 
 ### ```pip```
 <details>
 <summary>pip安装</summary>
 
 命令行输入以下命令
 
 ```cmd
-pip install nonebot_plugin_watermarker
+pip install nonebot-plugin-watermarker
 ```
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
     plugins = ["nonebot_plugin_rename"]
 
 ```
@@ -77,19 +77,19 @@
 plugins = []
 plugin_dirs = ["src/plugins"]
 ```
 </details>
 
 ##  ⚙插件配置项
 
-| 变量名      |       变量类型    |   变量概述       |
-|------------|----------------------------------|----------------|
-| ```watermark_image_path```   |```str```|水印图片存放目录,目录下的所有水印图片会被随机选取|
-| ```watermark_image_size```   |```float```|水印相对图片的大小(保持水印原来的形状)|
-| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件(未完工)|
+|  变量名                                 | 变量类型      |          变量概述                             |    使用示例   |
+|----------------------------------------|---------------|----------------------------------------------|-----------------|
+| ```watermark_image_path```             |```str```      |水印图片存放目录,目录下的所有水印图片会被随机选取 | ```F:\image``` |
+| ```watermark_image_size```             |```float```    |水印相对图片的大小(保持水印原来的形状)|```0.15```|
+| ```watermark_image_exculed_plugin```   |```List[str]```|不想被贴水印的插件                      |```[插件位置.plugins.插件名称]```(如```src.plugins.nonebot_plugin_petpet```)
 
 ## 🎉目前已实现的功能
 
 ### 加水印捏
 <details>
 <summary>效果图</summary>
 
@@ -99,30 +99,34 @@
 
 ![G37PR_ KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)
 
 </details>
 
 ## 💡待实现的功能
 
-1. -[ ] 对特定的插件的图片不进行贴水印操作
-2. -[ ] 待补充.....
+1. -[x] 对特定的插件的图片不进行贴水印操作
+2. -[x] 对GIF图片进行适配
+3. -[ ] 更多不同的贴水印方式
+4. -[ ] 贴图片怎么够,我要贴文字!
+5. -[ ] 待补充.....
 
 # 💣已知bug
 
-水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(
+水印小概率贴不上,应该是base64的原因,但是我一直找不到真正的问题源,因为有时候贴的上有时候贴不上(已解决,base64解码问题,为末位不足位没有补上=)
 
 # 🔥鸣谢
 
 [Nonebot2](https://github.com/nonebot/nonebot2),不用说,没有Nonebot就没有这个插件
 
 ~~[我自己](https://github.com/X-Skirt-X),因为我做的PoweredByNonebot的Logo~~
 
 # 💦其他
 
 没有其他,想到再补
+
 """,
     long_description_content_type="text/markdown",
     author='XU',
     author_email='Woyerpa@outlook.com',
     license='MIT License',
     packages=find_packages(),
     url='https://github.com/X-Skirt-X/nonebot-plugin-watermarker',
```

#### html2text {}

```diff
@@ -1,42 +1,48 @@
 from setuptools import setup, find_packages setup
-( name='nonebot_plugin_watermarker', version="0.1.5.1", description=
+( name='nonebot_plugin_watermarker', version="0.2.0", description=
 ( 'ä¸ºnonebotæºå¨äººåéçå¾çå ä¸æ°´å°' ), long_description="""
                             [PoweredByNonebotLogo]
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-watermarker _â¨ ä¸ºä½ çbotååºçå¾çæ·»å æ°´å°! â¨_
                            [license] [pypi] [python]
  * [ðç®ä»](#ç®ä») * [ð¿ å®è£æ¹æ³](#å®è£æ¹æ³) *
 [âï¸æä»¶éç½®é¡¹](#æä»¶éç½®é¡¹) * [ðç®åå·²å®ç°çåè½]
 (#ç®åå·²å®ç°çåè½) * [ð¡å¾å®ç°çåè½](#å¾å®ç°çåè½) *
 [ð£å·²ç¥bug](#å·²ç¥bug) * [ð¥é¸£è°¢](#é¸£è°¢) * [ð¦å¶ä»](#å¶ä»)  ##
 ðç®ä» ä¸ºbotååºçææå¾çé½å ä¸æ°´å°
 (æçæ¶åæ°´å°å¾ç¦,ä½æ¯å¸æ°çæ°´å°è½å¢å å¾ççç¾æ,ä¸æ¯å?)
 ## ð¿å®è£æ¹æ³ ### ```nbèææ¶```  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```cmd nb
-plugin install nonebot_piugin_watermarker ```  ### ```pip```  pipå®è£
-å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot_plugin_watermarker ```
+plugin install nonebot-piugin-watermarker ```  ### ```pip```  pipå®è£
+å½ä»¤è¡è¾å¥ä»¥ä¸å½ä»¤ ```cmd pip install nonebot-plugin-watermarker ```
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_rename"] ```
 [tool.nonebot] plugins = [] plugin_dirs = ["src/plugins"] ```  ##
-âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | |------------|--
---------------------------------|----------------| | ```watermark_image_path```
-|```str```|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå|
-| ```watermark_image_size``` |```float```|æ°´å°ç¸å¯¹å¾ççå¤§å°
-(ä¿ææ°´å°åæ¥çå½¢ç¶)| | ```watermark_image_exculed_plugin``` |```List
-[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶(æªå®å·¥)| ##
-ðç®åå·²å®ç°çåè½ ### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{
-{XBE](https://user-images.githubusercontent.com/91937041/235442049-67ac0b4c-
-1629-4d78-9858-8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_
-KAWEUINI_ _B)H2E](https://user-images.githubusercontent.com/91937041/235442112-
-c35e08ed-64c4-4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[ ]
-å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[ ] å¾è¡¥å..... #
-ð£å·²ç¥bug
+âæä»¶éç½®é¡¹ | åéå | åéç±»å | åéæ¦è¿° | ä½¿ç¨ç¤ºä¾ |
+|----------------------------------------|---------------|---------------------
+-------------------------|-----------------| | ```watermark_image_path```
+|```str```
+|æ°´å°å¾çå­æ¾ç®å½,ç®å½ä¸çæææ°´å°å¾çä¼è¢«éæºéå |
+```F:\image``` | | ```watermark_image_size``` |```float```
+|æ°´å°ç¸å¯¹å¾ççå¤§å°(ä¿ææ°´å°åæ¥çå½¢ç¶)|```0.15```| |
+```watermark_image_exculed_plugin``` |```List
+[str]```|ä¸æ³è¢«è´´æ°´å°çæä»¶ |```[æä»¶ä½ç½®.plugins.æä»¶åç§°]```
+(å¦```src.plugins.nonebot_plugin_petpet```) ## ðç®åå·²å®ç°çåè½
+### å æ°´å°æ  ææå¾ ![6PHLH{(JH $R~J2H@8{{XBE](https://user-
+images.githubusercontent.com/91937041/235442049-67ac0b4c-1629-4d78-9858-
+8b411b7ebe7b.jpg) å¤ªå°äºçä¸è§æ¾å¤§ç( ![G37PR_ KAWEUINI_ _B)H2E]
+(https://user-images.githubusercontent.com/91937041/235442112-c35e08ed-64c4-
+4b09-93f6-5976bb70de60.jpg)  ## ð¡å¾å®ç°çåè½ 1. -[x]
+å¯¹ç¹å®çæä»¶çå¾çä¸è¿è¡è´´æ°´å°æä½ 2. -[x]
+å¯¹GIFå¾çè¿è¡éé 3. -[ ] æ´å¤ä¸åçè´´æ°´å°æ¹å¼ 4. -[ ]
+è´´å¾çæä¹å¤,æè¦è´´æå­! 5. -[ ] å¾è¡¥å..... # ð£å·²ç¥bug
 æ°´å°å°æ¦çè´´ä¸ä¸,åºè¯¥æ¯base64çåå ,ä½æ¯æä¸ç´æ¾ä¸å°çæ­£çé®é¢æº,å ä¸ºææ¶åè´´çä¸ææ¶åè´´ä¸ä¸
-( # ð¥é¸£è°¢ [Nonebot2](https://github.com/nonebot/
+(å·²è§£å³,base64è§£ç é®é¢,ä¸ºæ«ä½ä¸è¶³ä½æ²¡æè¡¥ä¸=) # ð¥é¸£è°¢
+[Nonebot2](https://github.com/nonebot/
 nonebot2),ä¸ç¨è¯´,æ²¡æNonebotå°±æ²¡æè¿ä¸ªæä»¶ ~~[æèªå·±](https://
 github.com/X-Skirt-X),å ä¸ºæåçPoweredByNonebotçLogo~~ # ð¦å¶ä»
 æ²¡æå¶ä»,æ³å°åè¡¥ """, long_description_content_type="text/markdown",
 author='XU', author_email='Woyerpa@outlook.com', license='MIT License',
 packages=find_packages(), url='https://github.com/X-Skirt-X/nonebot-plugin-
 watermarker', install_requires=[ "nonebot2", "pillow", "" ] )
```

