# Comparing `tmp/django-imgwidget-0.0.2.1.tar.gz` & `tmp/django-imgwidget-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-imgwidget-0.0.2.1.tar", last modified: Sat Jun  3 05:18:39 2023, max compression
+gzip compressed data, was "django-imgwidget-0.0.2.2.tar", last modified: Sat Jun  3 07:14:21 2023, max compression
```

## Comparing `django-imgwidget-0.0.2.1.tar` & `django-imgwidget-0.0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.565789 django-imgwidget-0.0.2.1/
--rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2.1/MANIFEST.in
--rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 05:18:39.565623 django-imgwidget-0.0.2.1/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)     1747 2023-06-03 04:43:52.000000 django-imgwidget-0.0.2.1/README.md
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.562956 django-imgwidget-0.0.2.1/django_imguploder/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/admin.py
--rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2.1/django_imguploder/apps.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563177 django-imgwidget-0.0.2.1/django_imguploder/forms/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2.1/django_imguploder/forms/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)      871 2023-06-03 05:18:17.000000 django-imgwidget-0.0.2.1/django_imguploder/forms/widget.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563406 django-imgwidget-0.0.2.1/django_imguploder/migrations/
--rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/migrations/__init__.py
--rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/models.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561152 django-imgwidget-0.0.2.1/django_imguploder/static/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561298 django-imgwidget-0.0.2.1/django_imguploder/static/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563490 django-imgwidget-0.0.2.1/django_imguploder/static/admin/css/
--rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.2.1/django_imguploder/static/admin/css/imgwidget.css
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563729 django-imgwidget-0.0.2.1/django_imguploder/static/admin/imgs/
--rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2.1/django_imguploder/static/admin/imgs/add.png
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.563976 django-imgwidget-0.0.2.1/django_imguploder/static/admin/js/
--rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2.1/django_imguploder/static/admin/js/jquery.min.js
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561396 django-imgwidget-0.0.2.1/django_imguploder/templates/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.561434 django-imgwidget-0.0.2.1/django_imguploder/templates/admin/
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.564645 django-imgwidget-0.0.2.1/django_imguploder/templates/admin/widgets/
--rw-r--r--   0 donghao    (501) staff       (20)     5790 2023-06-03 05:18:17.000000 django-imgwidget-0.0.2.1/django_imguploder/templates/admin/widgets/img_multi_upload.html
--rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/tests.py
--rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.1/django_imguploder/views.py
-drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 05:18:39.565464 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/
--rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/PKG-INFO
--rw-r--r--   0 donghao    (501) staff       (20)      749 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/SOURCES.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/dependency_links.txt
--rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/not-zip-safe
--rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/requires.txt
--rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 05:18:39.000000 django-imgwidget-0.0.2.1/django_imgwidget.egg-info/top_level.txt
--rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 05:18:39.565838 django-imgwidget-0.0.2.1/setup.cfg
--rw-r--r--   0 donghao    (501) staff       (20)      878 2023-06-03 05:18:38.000000 django-imgwidget-0.0.2.1/setup.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.930136 django-imgwidget-0.0.2.2/
+-rw-r--r--   0 donghao    (501) staff       (20)      148 2023-06-03 04:16:28.000000 django-imgwidget-0.0.2.2/MANIFEST.in
+-rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 07:14:21.930006 django-imgwidget-0.0.2.2/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)     1747 2023-06-03 04:43:52.000000 django-imgwidget-0.0.2.2/README.md
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927404 django-imgwidget-0.0.2.2/django_imguploder/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/admin.py
+-rw-r--r--   0 donghao    (501) staff       (20)      164 2023-06-03 03:56:23.000000 django-imgwidget-0.0.2.2/django_imguploder/apps.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927599 django-imgwidget-0.0.2.2/django_imguploder/forms/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:12:44.000000 django-imgwidget-0.0.2.2/django_imguploder/forms/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)      871 2023-06-03 05:18:17.000000 django-imgwidget-0.0.2.2/django_imguploder/forms/widget.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927809 django-imgwidget-0.0.2.2/django_imguploder/migrations/
+-rw-r--r--   0 donghao    (501) staff       (20)        0 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/migrations/__init__.py
+-rw-r--r--   0 donghao    (501) staff       (20)       57 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/models.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925678 django-imgwidget-0.0.2.2/django_imguploder/static/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925820 django-imgwidget-0.0.2.2/django_imguploder/static/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.927894 django-imgwidget-0.0.2.2/django_imguploder/static/admin/css/
+-rw-r--r--   0 donghao    (501) staff       (20)     2121 2023-06-03 03:37:46.000000 django-imgwidget-0.0.2.2/django_imguploder/static/admin/css/imgwidget.css
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.928113 django-imgwidget-0.0.2.2/django_imguploder/static/admin/imgs/
+-rw-r--r--   0 donghao    (501) staff       (20)     6064 2022-03-02 10:11:37.000000 django-imgwidget-0.0.2.2/django_imguploder/static/admin/imgs/add.png
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.928338 django-imgwidget-0.0.2.2/django_imguploder/static/admin/js/
+-rwxr-xr-x   0 donghao    (501) staff       (20)    84349 2018-07-26 06:41:58.000000 django-imgwidget-0.0.2.2/django_imguploder/static/admin/js/jquery.min.js
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925915 django-imgwidget-0.0.2.2/django_imguploder/templates/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.925954 django-imgwidget-0.0.2.2/django_imguploder/templates/admin/
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.929001 django-imgwidget-0.0.2.2/django_imguploder/templates/admin/widgets/
+-rw-r--r--   0 donghao    (501) staff       (20)     6300 2023-06-03 07:14:17.000000 django-imgwidget-0.0.2.2/django_imguploder/templates/admin/widgets/img_multi_upload.html
+-rw-r--r--   0 donghao    (501) staff       (20)       60 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/tests.py
+-rw-r--r--   0 donghao    (501) staff       (20)       63 2023-06-02 10:11:54.000000 django-imgwidget-0.0.2.2/django_imguploder/views.py
+drwxr-xr-x   0 donghao    (501) staff       (20)        0 2023-06-03 07:14:21.929832 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/
+-rw-r--r--   0 donghao    (501) staff       (20)     2174 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/PKG-INFO
+-rw-r--r--   0 donghao    (501) staff       (20)      749 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/SOURCES.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/dependency_links.txt
+-rw-r--r--   0 donghao    (501) staff       (20)        1 2023-06-03 03:51:52.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/not-zip-safe
+-rw-r--r--   0 donghao    (501) staff       (20)        7 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/requires.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       18 2023-06-03 07:14:21.000000 django-imgwidget-0.0.2.2/django_imgwidget.egg-info/top_level.txt
+-rw-r--r--   0 donghao    (501) staff       (20)       38 2023-06-03 07:14:21.930174 django-imgwidget-0.0.2.2/setup.cfg
+-rw-r--r--   0 donghao    (501) staff       (20)      878 2023-06-03 07:14:17.000000 django-imgwidget-0.0.2.2/setup.py
```

### Comparing `django-imgwidget-0.0.2.1/PKG-INFO` & `django-imgwidget-0.0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
```

### Comparing `django-imgwidget-0.0.2.1/README.md` & `django-imgwidget-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.1/django_imguploder/forms/widget.py` & `django-imgwidget-0.0.2.2/django_imguploder/forms/widget.py`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.1/django_imguploder/static/admin/css/imgwidget.css` & `django-imgwidget-0.0.2.2/django_imguploder/static/admin/css/imgwidget.css`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.1/django_imguploder/static/admin/imgs/add.png` & `django-imgwidget-0.0.2.2/django_imguploder/static/admin/imgs/add.png`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.1/django_imguploder/static/admin/js/jquery.min.js` & `django-imgwidget-0.0.2.2/django_imguploder/static/admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.1/django_imguploder/templates/admin/widgets/img_multi_upload.html` & `django-imgwidget-0.0.2.2/django_imguploder/templates/admin/widgets/img_multi_upload.html`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,42 @@
     </div>
 </div>
 <script type="text/javascript">
     //因为图片是动态添加的，所以不能使用选择器选择。
     function show_big_img(obj) {
         imgShow("#outerdiv", "#innerdiv", "#bigimg", obj);
     }
+
+    function getRotate(_this, index) {
+        var degree = (_this.data('rotate') || 0) - 90;
+        _this.css('transform', 'rotate(' + degree + 'deg)');
+        _this.css('-ms-transform', 'rotate(' + degree + 'deg)');
+        _this.css('-webkit-transform', 'rotate(' + degree + 'deg)');
+        _this.css('-moz-transform', 'rotate(' + degree + 'deg)');
+        _this.data('rotate', degree);
+    }
+
+    $("#bigimg").click(function () {//再次点击淡出消失弹出层
+        getRotate($("#bigimg"), 1);
+        return false;
+    });
+    $("#outerdiv").click(function () {//再次点击淡出消失弹出层
+        $(this).fadeOut("fast");
+        return false;
+    });
+
     function imgShow(outerdiv, innerdiv, bigimg, obj) {
         var src = obj.src;//获取当前点击的pimg元素中的src属性
         $(bigimg).attr("src", src);//设置#bigimg元素的src属性
         var windowW = $(window).width();//获取当前窗口宽度
         var windowH = $(window).height();//获取当前窗口高度
         var realWidth = obj.naturalWidth;//获取图片真实宽度
         var realHeight = obj.naturalHeight;//获取图片真实高度
         var imgWidth, imgHeight;
-        var scale = 1;//缩放尺寸，当图片真实宽度和高度大于窗口宽度和高度时进行缩放
+        var scale = 0.9;//缩放尺寸，当图片真实宽度和高度大于窗口宽度和高度时进行缩放
         if (realHeight > windowH * scale) {//判断图片高度
             imgHeight = windowH * scale;//如大于窗口高度，图片高度进行缩放
             imgWidth = imgHeight / realHeight * realWidth;//等比例缩放宽度
             if (imgWidth > windowW * scale) {//如宽度扔大于窗口宽度
                 imgWidth = windowW * scale;//再对宽度进行缩放
             }
         } else if (realWidth > windowW * scale) {//如图片高度合适，判断图片宽度
@@ -45,28 +64,23 @@
             imgHeight = realHeight;
         }
         $(bigimg).css("width", imgWidth);//以最终的宽度对图片缩放
         var w = (windowW - imgWidth) / 2;//计算图片与窗口左边距
         var h = (windowH - imgHeight) / 2;//计算图片与窗口上边距
         $(innerdiv).css({"top": h, "left": w});//设置#innerdiv的top和left属性
         $(outerdiv).fadeIn("fast");//淡入显示#outerdiv及.pimg
-
-        $(outerdiv).click(function () {//再次点击淡出消失弹出层
-            $(this).fadeOut("fast");
-        });
     }
 
     function updateTextareaValue(widget_name) {
         var imageUrls = [];
         $('.' + widget_name + '_values').each(function () {
             var imgUrl = $(this).attr('src');
             imageUrls.push(imgUrl);
         });
         $('#' + widget_name).val(imageUrls);
-        console.log(widget_name, imageUrls)
     }
 
     function add_selected_img(src, widget_name) {
         $("#upload_image_" + widget_name).before("<div class=\"selected-img\">\n" +
             "    <i class=\"iconfont icon-delete delete_icon_image\" data-widgetname=\"" + widget_name + "\" title=\"删除图片\" onclick='delete_img(this)'></i>\n" +
             "    <img class=\"" + widget_name + "_values cover_image\" src=\"" + src.replace("'", '').replace("'", '') + "\" alt=\"待选图片\" onclick='show_big_img(this)'>\n" +
             "</div>");
```

### Comparing `django-imgwidget-0.0.2.1/django_imgwidget.egg-info/PKG-INFO` & `django-imgwidget-0.0.2.2/django_imgwidget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-imgwidget
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: 上传图片组件
 Home-page: https://github.com/RelaxedDong/django_imguploder
 Author: donghao
 Author-email: 1417766861@qq.com
 License: Apache License 2.0
 Keywords: django,admin,widget,image,uploader
 Platform: UNKNOWN
```

### Comparing `django-imgwidget-0.0.2.1/django_imgwidget.egg-info/SOURCES.txt` & `django-imgwidget-0.0.2.2/django_imgwidget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-imgwidget-0.0.2.1/setup.py` & `django-imgwidget-0.0.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 long_description = "\n".join([
     open('README.md', 'r', encoding='utf-8').read(),
 ])
 
 NAME = 'django-imgwidget'
-VERSION = '0.0.2.1'
+VERSION = '0.0.2.2'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(
         exclude=()
     ),
```

