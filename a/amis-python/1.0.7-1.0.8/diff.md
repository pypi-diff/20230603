# Comparing `tmp/amis_python-1.0.7.tar.gz` & `tmp/amis_python-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amis_python-1.0.7.tar", max compression
+gzip compressed data, was "amis_python-1.0.8.tar", max compression
```

## Comparing `amis_python-1.0.7.tar` & `amis_python-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11356 2023-02-22 13:25:24.880801 amis_python-1.0.7/LICENSE
--rw-r--r--   0        0        0     1434 2023-02-22 13:25:24.880801 amis_python-1.0.7/README.md
--rw-r--r--   0        0        0      227 2023-02-22 13:25:24.880801 amis_python-1.0.7/amis/__init__.py
--rw-r--r--   0        0        0   134169 2023-02-22 13:25:24.880801 amis_python-1.0.7/amis/components.py
--rw-r--r--   0        0        0     1287 2023-02-22 13:25:24.880801 amis_python-1.0.7/amis/constants.py
--rw-r--r--   0        0        0     7392 2023-02-22 13:25:24.880801 amis_python-1.0.7/amis/templates/app.jinja2
--rw-r--r--   0        0        0     1634 2023-02-22 13:25:24.880801 amis_python-1.0.7/amis/templates/page.jinja2
--rw-r--r--   0        0        0     4550 2023-02-22 13:25:24.880801 amis_python-1.0.7/amis/types.py
--rw-r--r--   0        0        0      761 2023-02-22 13:25:24.880801 amis_python-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 amis_python-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-03 10:46:36.050519 amis_python-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1434 2023-06-03 10:46:36.050519 amis_python-1.0.8/README.md
+-rw-r--r--   0        0        0      227 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/__init__.py
+-rw-r--r--   0        0        0   179505 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/components.py
+-rw-r--r--   0        0        0     1287 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/constants.py
+-rw-r--r--   0        0        0     6859 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/templates/app.jinja2
+-rw-r--r--   0        0        0     1621 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/templates/page.jinja2
+-rw-r--r--   0        0        0     5918 2023-06-03 10:46:36.050519 amis_python-1.0.8/amis/types.py
+-rw-r--r--   0        0        0      761 2023-06-03 10:46:36.054519 amis_python-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 amis_python-1.0.8/PKG-INFO
```

### Comparing `amis_python-1.0.7/LICENSE` & `amis_python-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.7/README.md` & `amis_python-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 </p>
 
 基于 [百度amis](https://github.com/baidu/amis) 前端框架的python pydantic模型封装。
 
 由于[原版本](https://github.com/amisadmin/fastapi_amis_admin/tree/master/fastapi_amis_admin/amis)缺少大量amis新版本的组件或配置，因此本项目在其版本的基础上进行了扩充。
 
 相比fastapi-amis-admin的版本：
-- 涵盖amis截至2.3.1版本的所有组件
+- 涵盖amis截至3.1.0版本的所有组件
 - 使用jinja2模板
 - 支持修改主题
 ## 安装
 ```
 pip install amis-python
 ```
 ## 简单使用
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ## amis-python
                          [license] [python] [version]
 åºäº [ç¾åº¦amis](https://github.com/baidu/amis) åç«¯æ¡æ¶çpython
 pydanticæ¨¡åå°è£ã ç±äº[åçæ¬](https://github.com/amisadmin/
 fastapi_amis_admin/tree/master/fastapi_amis_admin/
 amis)ç¼ºå°å¤§éamisæ°çæ¬çç»ä»¶æéç½®ï¼å æ­¤æ¬é¡¹ç®å¨å¶çæ¬çåºç¡ä¸è¿è¡äºæ©åã
 ç¸æ¯fastapi-amis-adminççæ¬ï¼ -
-æ¶µçamisæªè³2.3.1çæ¬çææç»ä»¶ - ä½¿ç¨jinja2æ¨¡æ¿ -
+æ¶µçamisæªè³3.1.0çæ¬çææç»ä»¶ - ä½¿ç¨jinja2æ¨¡æ¿ -
 æ¯æä¿®æ¹ä¸»é¢ ## å®è£ ``` pip install amis-python ``` ## ç®åä½¿ç¨
 ```python from amis.components import Page page = Page(title='æ°é¡µé¢',
 body='Hello World') # è¾åºä¸ºpythonå­å¸ print(page.to_dict()) #
 è¾åºä¸ºjson print(page.to_json()) # è¾åºä¸ºstr print(page.render()) #
 ä¿å­ä¸ºhtmlæä»¶ with open('HelloWorld.html', 'w', encoding='utf-8') as f:
 f.write(page.render()) ``` ## è¯¦ç»ä½¿ç¨ è¯¦è§[amiså®æ¹ææ¡£](https://
 aisuda.bce.baidu.com/amis/zh-CN/docs/index) ## æè°¢ - [amis](https://
```

### Comparing `amis_python-1.0.7/amis/constants.py` & `amis_python-1.0.8/amis/constants.py`

 * *Files identical despite different names*

### Comparing `amis_python-1.0.7/amis/templates/app.jinja2` & `amis_python-1.0.8/amis/templates/app.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,170 +1,180 @@
 <!DOCTYPE html>
 <html lang="">
-    <head>
-        <meta charset="UTF-8"/>
-        <title>{{ site_title }}</title>
-        <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-        <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1"/>
-        <meta http-equiv="X-UA-Compatible" content="IE=Edge"/>
-        <link href="{{ site_icon }}" rel="shortcut icon" type="image/x-icon"/>
-        <link href="{{ cdn }}/amis@{{ version }}/sdk/{{ theme_css }}" rel="stylesheet" title="default"/>
-        <link href="{{ cdn }}/amis@{{ version }}/sdk/helper.css" rel="stylesheet"/>
-        <link href="{{ cdn }}/amis@{{ version }}/sdk/iconfont.css" rel="stylesheet"/>
-        <script src="{{ cdn }}/amis@{{ version }}/sdk/sdk.js"></script>
-        <script src="{{ cdn }}/vue@2.6.14/dist/vue.js"></script>
-        <script src="{{ cdn }}/history@4.10.1/umd/history.js"></script>
-        <style>
-            html, body,
-            .app-wrapper {
-                position: relative;
-                width: 100%;
-                height: 100%;
-                margin: 0;
-                padding: 0;
+<head>
+    <meta charset="UTF-8"/>
+    <title>{{ site_title }}</title>
+    <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
+    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1"/>
+    <meta http-equiv="X-UA-Compatible" content="IE=Edge"/>
+    <link href="{{ site_icon }}" rel="shortcut icon" type="image/x-icon"/>
+    <link href="{{ cdn }}/amis@{{ version }}/sdk/{{ theme_css }}" rel="stylesheet" title="default"/>
+    <link href="{{ cdn }}/amis@{{ version }}/sdk/helper.css" rel="stylesheet"/>
+    <link href="{{ cdn }}/amis@{{ version }}/sdk/iconfont.css" rel="stylesheet"/>
+    <script src="{{ cdn }}/amis@{{ version }}/sdk/sdk.js"></script>
+    <script src="{{ cdn }}/vue@2/dist/vue.js"></script>
+    <script src="{{ cdn }}/history@{{ version }}"></script>
+    <style>
+        html, body,
+        .app-wrapper {
+            position: relative;
+            width: 100%;
+            height: 100%;
+            margin: 0;
+            padding: 0;
+        }
+
+        /*DropDownButton组件下拉菜单样式修改*/
+        .amis-scope .cxd-DropDown-menu {
+            min-width: 100%;
+            text-align: center;
+        }
+    </style>
+</head>
+<body>
+<div class="app-wrapper" id="root"></div>
+<script>
+    (function () {
+        let amis = amisRequire('amis/embed');
+        const match = amisRequire('path-to-regexp').match;
+
+        // 如果想用 browserHistory 请切换下这处代码, 其他不用变
+        //const history = HistoryLibrary.createBrowserHistory();
+        //const history = HistoryLibrary.createHashHistory();
+        const history = HistoryLibrary.{{ routerModel }}();
+        const app = {{AmisSchemaJson }};
+
+        function normalizeLink(to, location = history.location) {
+            to = to || '';
+
+            if (to && to[0] === '#') {
+                to = location.pathname + location.search + to;
+            } else if (to && to[0] === '?') {
+                to = location.pathname + to;
             }
 
-            /*DropDownButton组件下拉菜单样式修改*/
-            .amis-scope .cxd-DropDown-menu {
-                min-width: 100%;
-                text-align: center;
-            }
-        </style>
-    </head>
-    <body>
-    <div class="app-wrapper" id="root"></div>
-        <script>
-            (function () {
-                let amis = amisRequire('amis/embed');
-                const match = amisRequire('path-to-regexp').match;
-
-                // 如果想用 browserHistory 请切换下这处代码, 其他不用变
-                // const history = History.createBrowserHistory();
-                const history = History.createHashHistory();
-                const app = {{ AmisSchemaJson }};
-
-                function normalizeLink(to, location = history.location) {
-                    to = to || '';
-
-                    if (to && to[0] === '#') {
-                        to = location.pathname + location.search + to;
-                    } else if (to && to[0] === '?') {
-                        to = location.pathname + to;
-                    }
-
-                    const idx = to.indexOf('?');
-                    const idx2 = to.indexOf('#');
-                    let pathname = ~idx ? to.substring(0, idx) : ~idx2 ? to.substring(0, idx2) : to;
-                    let search = ~idx ? to.substring(idx, ~idx2 ? idx2 : undefined) : '';
-                    let hash = ~idx2 ? to.substring(idx2) : location.hash;
-                    if (!pathname) {
-                        pathname = location.pathname;
-                    } else if (pathname[0] != '/' && !/^https?\:\/\//.test(pathname)) {
-                        let relativeBase = location.pathname;
-                        const paths = relativeBase.split('/');
+            const idx = to.indexOf('?');
+            const idx2 = to.indexOf('#');
+            let pathname = ~idx ? to.substring(0, idx) : ~idx2 ? to.substring(0, idx2) : to;
+            let search = ~idx ? to.substring(idx, ~idx2 ? idx2 : undefined) : '';
+            let hash = ~idx2 ? to.substring(idx2) : location.hash;
+            if (!pathname) {
+                pathname = location.pathname;
+            } else if (pathname[0] != '/' && !/^https?\:\/\//.test(pathname)) {
+                let relativeBase = location.pathname;
+                const paths = relativeBase.split('/');
+                paths.pop();
+                let m;
+                while ((m = /^\.\.?\//.exec(pathname))) {
+                    if (m[0] === '../') {
                         paths.pop();
-                        let m;
-                        while ((m = /^\.\.?\//.exec(pathname))) {
-                            if (m[0] === '../') {
-                                paths.pop();
-                            }
-                            pathname = pathname.substring(m[0].length);
-                        }
-                        pathname = paths.concat(pathname).join('/');
                     }
-                    return pathname + search + hash;
+                    pathname = pathname.substring(m[0].length);
                 }
+                pathname = paths.concat(pathname).join('/');
+            }
+            return pathname + search + hash;
+        }
+
+        function isCurrentUrl(to, ctx) {
+            if (!to) {
+                return false;
+            }
+            const pathname = history.location.pathname;
+            const link = normalizeLink(to, {
+                ...location,
+                pathname,
+                hash: ''
+            });
+
+            if (!~link.indexOf('http') && ~link.indexOf(':')) {
+                let strict = ctx && ctx.strict;
+                return match(link, {
+                    decode: decodeURIComponent,
+                    strict: typeof strict !== 'undefined' ? strict : true
+                })(pathname);
+            }
+
+            return decodeURI(pathname) === link;
+        }
 
-                function isCurrentUrl(to, ctx) {
-                    if (!to) {
-                        return false;
-                    }
-                    const pathname = history.location.pathname;
-                    const link = normalizeLink(to, {
-                        ...location,
-                        pathname,
-                        hash: ''
-                    });
-
-                    if (!~link.indexOf('http') && ~link.indexOf(':')) {
-                        let strict = ctx && ctx.strict;
-                        return match(link, {
-                            decode: decodeURIComponent,
-                            strict: typeof strict !== 'undefined' ? strict : true
-                        })(pathname);
+        let amisInstance = amis.embed(
+            '#root',
+            app,
+            {location: history.location, locale: "{{ locale}}"},
+            {
+
+                // watchRouteChange: fn => {
+                //   return history.listen(fn);
+                // },
+                {{ requestAdaptor }}
+                {{ responseAdaptor }}
+                updateLocation: (location, replace) => {
+                    location = normalizeLink(location);
+                    if (location === 'goBack') {
+                        return history.goBack();
+                    } else if (
+                        (!/^https?\:\/\//.test(location) &&
+                            location ===
+                            history.location.pathname + history.location.search) ||
+                        location === history.location.href
+                    ) {
+                        // 目标地址和当前地址一样，不处理，免得重复刷新
+                        return;
+                    } else if (/^https?\:\/\//.test(location) || !history) {
+                        return (window.location.href = location);
                     }
 
-                    return decodeURI(pathname) === link;
-                }
+                    history[replace ? 'replace' : 'push'](location);
+                },
+                jumpTo: (to, action) => {
+                    if (to === 'goBack') {
+                        return history.goBack();
+                    }
+
+                    to = normalizeLink(to);
+
+                    if (isCurrentUrl(to)) {
+                        return;
+                    }
+
+                    if (action && action.actionType === 'url') {
+                        action.blank === false
+                            ? (window.location.href = to)
+                            : window.open(to, '_blank');
+                        return;
+                    } else if (action && action.blank) {
+                        window.open(to, '_blank');
+                        return;
+                    }
+
+                    if (/^https?:\/\//.test(to)) {
+                        window.location.href = to;
+                    } else if (
+                        (!/^https?\:\/\//.test(to) &&
+                            to === history.pathname + history.location.search) ||
+                        to === history.location.href
+                    ) {
+                        // do nothing
+                    } else if (location.hash && to.indexOf("?") > -1) {
+                        //如果当前页面有hash，且跳转的页面有参数，将hash拼接到参数后面
+                        const [hash, search] = to.split("?");
+                        window.location.href = location.pathname + "?" + search + "#" + hash;
+                    } else {
+                        history.push(to);
+                    }
+                },
+                isCurrentUrl: isCurrentUrl,
+                theme: '{{ theme_name }}'
+            }
+        );
 
-                let amisInstance = amis.embed(
-                    '#root',
-                    app,
-                    {location: history.location, locale: "{{ locale }}"},
-                    {
-                        {{ requestAdaptor }}
-                        {{ responseAdaptor }}
-                        updateLocation: (location, replace) => {
-                            location = normalizeLink(location);
-                            if (location === 'goBack') {
-                                return history.goBack();
-                            } else if (
-                                (!/^https?\:\/\//.test(location) &&
-                                    location ===
-                                    history.location.pathname + history.location.search) ||
-                                location === history.location.href
-                            ) {
-                                // 目标地址和当前地址一样，不处理，免得重复刷新
-                                return;
-                            } else if (/^https?\:\/\//.test(location) || !history) {
-                                return (window.location.href = location);
-                            }
-
-                            history[replace ? 'replace' : 'push'](location);
-                        },
-                        jumpTo: (to, action) => {
-                            if (to === 'goBack') {
-                                return history.goBack();
-                            }
-
-                            to = normalizeLink(to);
-
-                            if (isCurrentUrl(to)) {
-                                return;
-                            }
-
-                            if (action && action.actionType === 'url') {
-                                action.blank === false
-                                    ? (window.location.href = to)
-                                    : window.open(to, '_blank');
-                                return;
-                            } else if (action && action.blank) {
-                                window.open(to, '_blank');
-                                return;
-                            }
-
-                            if (/^https?:\/\//.test(to)) {
-                                window.location.href = to;
-                            } else if (
-                                (!/^https?\:\/\//.test(to) &&
-                                    to === history.pathname + history.location.search) ||
-                                to === history.location.href
-                            ) {
-                                // do nothing
-                            } else {
-                                history.push(to);
-                            }
-                        },
-                        isCurrentUrl: isCurrentUrl,
-                        theme: '{{ theme_name }}'
-                    }
-                );
-
-                history.listen(state => {
-                    amisInstance.updateProps({
-                        location: state.location || state
-                    });
-                });
-            })();
-        </script>
-    </body>
+        history.listen(state => {
+            amisInstance.updateProps({
+                location: state.location || state,
+                locale: "{{locale}}"
+            });
+        });
+    })();
+</script>
+</body>
 </html>
```

### Comparing `amis_python-1.0.7/amis/templates/page.jinja2` & `amis_python-1.0.8/amis/templates/page.jinja2`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1" />
         <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
         <link href="{{ site_icon }}" rel="shortcut icon" type="image/x-icon"/>
         <link href="{{ cdn }}/amis@{{ version }}/sdk/{{ theme_css }}" rel="stylesheet" title="default"/>
         <link href="{{ cdn }}/amis@{{ version }}/sdk/helper.css" rel="stylesheet"/>
         <link href="{{ cdn }}/amis@{{ version }}/sdk/iconfont.css" rel="stylesheet"/>
         <script src="{{ cdn }}/amis@{{ version }}/sdk/sdk.js"></script>
-        <script src="{{ cdn }}/vue@2.6.14/dist/vue.js"></script>
-        <script src="{{ cdn }}/history@4.10.1/umd/history.js"></script>
+        <script src="{{ cdn }}/vue@2/dist/vue.js"></script>
+        <script src="{{ cdn }}/history@{{ version }}"></script>
         <style>
             html, body,
             .app-wrapper {
                 position: relative;
                 width: 100%;
                 height: 100%;
                 margin: 0;
```

### Comparing `amis_python-1.0.7/pyproject.toml` & `amis_python-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amis-python"
-version = "1.0.7"
+version = "1.0.8"
 description = "基于百度amis前端框架的python pydantic模型封装。"
 authors = ["惜月 <277073121@qq.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["amis"]
 homepage = "https://github.com/CMHopeSunshine/amis-py"
 repository = "https://github.com/CMHopeSunshine/amis-py"
```

### Comparing `amis_python-1.0.7/PKG-INFO` & `amis_python-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amis-python
-Version: 1.0.7
+Version: 1.0.8
 Summary: 基于百度amis前端框架的python pydantic模型封装。
 Home-page: https://github.com/CMHopeSunshine/amis-py
 License: Apache-2.0
 Keywords: amis
 Author: 惜月
 Author-email: 277073121@qq.com
 Requires-Python: >=3.7,<4.0
@@ -29,15 +29,15 @@
 </p>
 
 基于 [百度amis](https://github.com/baidu/amis) 前端框架的python pydantic模型封装。
 
 由于[原版本](https://github.com/amisadmin/fastapi_amis_admin/tree/master/fastapi_amis_admin/amis)缺少大量amis新版本的组件或配置，因此本项目在其版本的基础上进行了扩充。
 
 相比fastapi-amis-admin的版本：
-- 涵盖amis截至2.3.1版本的所有组件
+- 涵盖amis截至3.1.0版本的所有组件
 - 使用jinja2模板
 - 支持修改主题
 ## 安装
 ```
 pip install amis-python
 ```
 ## 简单使用
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amis-python Version: 1.0.7 Summary:
+Metadata-Version: 2.1 Name: amis-python Version: 1.0.8 Summary:
 åºäºç¾åº¦amisåç«¯æ¡æ¶çpython pydanticæ¨¡åå°è£ã Home-page: https:
 //github.com/CMHopeSunshine/amis-py License: Apache-2.0 Keywords: amis Author:
 ææ Author-email: 277073121@qq.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 text/markdown ## amis-python
                          [license] [python] [version]
 åºäº [ç¾åº¦amis](https://github.com/baidu/amis) åç«¯æ¡æ¶çpython
 pydanticæ¨¡åå°è£ã ç±äº[åçæ¬](https://github.com/amisadmin/
 fastapi_amis_admin/tree/master/fastapi_amis_admin/
 amis)ç¼ºå°å¤§éamisæ°çæ¬çç»ä»¶æéç½®ï¼å æ­¤æ¬é¡¹ç®å¨å¶çæ¬çåºç¡ä¸è¿è¡äºæ©åã
 ç¸æ¯fastapi-amis-adminççæ¬ï¼ -
-æ¶µçamisæªè³2.3.1çæ¬çææç»ä»¶ - ä½¿ç¨jinja2æ¨¡æ¿ -
+æ¶µçamisæªè³3.1.0çæ¬çææç»ä»¶ - ä½¿ç¨jinja2æ¨¡æ¿ -
 æ¯æä¿®æ¹ä¸»é¢ ## å®è£ ``` pip install amis-python ``` ## ç®åä½¿ç¨
 ```python from amis.components import Page page = Page(title='æ°é¡µé¢',
 body='Hello World') # è¾åºä¸ºpythonå­å¸ print(page.to_dict()) #
 è¾åºä¸ºjson print(page.to_json()) # è¾åºä¸ºstr print(page.render()) #
 ä¿å­ä¸ºhtmlæä»¶ with open('HelloWorld.html', 'w', encoding='utf-8') as f:
 f.write(page.render()) ``` ## è¯¦ç»ä½¿ç¨ è¯¦è§[amiså®æ¹ææ¡£](https://
 aisuda.bce.baidu.com/amis/zh-CN/docs/index) ## æè°¢ - [amis](https://
```

