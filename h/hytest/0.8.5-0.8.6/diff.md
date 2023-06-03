# Comparing `tmp/hytest-0.8.5-py3-none-any.whl.zip` & `tmp/hytest-0.8.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27165 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat       69 b- defN 21-Jun-03 08:24 hytest/__init__.py
--rw-rw-rw-  2.0 fat      705 b- defN 23-Jan-08 10:00 hytest/cfg.py
--rw-rw-rw-  2.0 fat     2795 b- defN 23-May-29 09:38 hytest/common.py
--rw-rw-rw-  2.0 fat       16 b- defN 23-May-31 01:06 hytest/product.py
--rw-rw-rw-  2.0 fat     6536 b- defN 23-Jan-09 02:09 hytest/run.py
+Zip file size: 27528 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat      131 b- defN 23-Jun-01 12:48 hytest/__init__.py
+-rw-rw-rw-  2.0 fat      958 b- defN 23-Jun-01 03:57 hytest/cfg.py
+-rw-rw-rw-  2.0 fat     3294 b- defN 23-Jun-01 13:15 hytest/common.py
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-01 03:35 hytest/product.py
+-rw-rw-rw-  2.0 fat     6718 b- defN 23-Jun-01 12:42 hytest/run.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-24 03:36 hytest/utils/__init__.py
--rw-rw-rw-  2.0 fat    30996 b- defN 23-Apr-06 02:10 hytest/utils/log.py
+-rw-rw-rw-  2.0 fat    31024 b- defN 23-Jun-02 10:17 hytest/utils/log.py
 -rw-rw-rw-  2.0 fat     3471 b- defN 23-Feb-22 02:05 hytest/utils/report.css
 -rw-rw-rw-  2.0 fat     1891 b- defN 22-Sep-12 03:09 hytest/utils/report.js
--rw-rw-rw-  2.0 fat    24796 b- defN 23-Jan-08 04:19 hytest/utils/runner.py
+-rw-rw-rw-  2.0 fat    24790 b- defN 23-Jun-02 03:27 hytest/utils/runner.py
 -rw-rw-rw-  2.0 fat      571 b- defN 21-Jun-03 08:24 hytest/utils/signal.py
--rw-rw-rw-  2.0 fat    11535 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1244 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       42 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1308 b- defN 23-May-31 03:20 hytest-0.8.5.dist-info/RECORD
-17 files, 86074 bytes uncompressed, 25039 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat    11535 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1244 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1309 b- defN 23-Jun-03 13:52 hytest-0.8.6.dist-info/RECORD
+17 files, 87093 bytes uncompressed, 25402 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: hytest/utils/runner.py
 Comment: 
 
 Filename: hytest/utils/signal.py
 Comment: 
 
-Filename: hytest-0.8.5.dist-info/LICENSE.txt
+Filename: hytest-0.8.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hytest-0.8.5.dist-info/METADATA
+Filename: hytest-0.8.6.dist-info/METADATA
 Comment: 
 
-Filename: hytest-0.8.5.dist-info/WHEEL
+Filename: hytest-0.8.6.dist-info/WHEEL
 Comment: 
 
-Filename: hytest-0.8.5.dist-info/entry_points.txt
+Filename: hytest-0.8.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: hytest-0.8.5.dist-info/top_level.txt
+Filename: hytest-0.8.6.dist-info/top_level.txt
 Comment: 
 
-Filename: hytest-0.8.5.dist-info/RECORD
+Filename: hytest-0.8.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hytest/__init__.py

```diff
@@ -1,4 +1,4 @@
-from .common import *
+from .common import signal,GSTORE,INFO,STEP,CHECK_POINT,LOG_IMG,SELENIUM_LOG_SCREEN
 
 import os, sys
 sys.path.append(os.getcwd())
```

## hytest/cfg.py

```diff
@@ -1,20 +1,30 @@
-# 执行语言编号
+supportedLang = ['zh','en']
 class l:
     LANGS = {
         'zh' : 0,
         'en' : 1,
     }
-    n = 1  # 当前使用的语言编号
+    n = None  # 当前使用的语言编号
 
-import locale
-if 'zh_CN' in locale.getdefaultlocale():
-    l.n = l.LANGS['zh']
-else :
-    l.n = l.LANGS['en']
+import sys
+if '--lang' in sys.argv:
+    try:
+        idx = sys.argv.index('--lang')
+        lang = sys.argv[idx+1]
+        if lang in supportedLang:
+            l.n = l.LANGS[lang]
+    except:...
+
+if l.n is None:
+    import locale
+    if 'zh_CN' in locale.getdefaultlocale():
+        l.n = l.LANGS['zh']
+    else :
+        l.n = l.LANGS['en']
 
 
 LANG_TABLE = {
     '测试报告' : ['测试报告','Test Report'],
     '指定测试报告标题' : ['指定测试报告标题','set test report title'],
 }
```

## hytest/common.py

```diff
@@ -9,48 +9,57 @@
             return getattr(self, key)
         else:
             return default
     def __setitem__(self,key,value):
         setattr(self, key, value )
 
     get = __getitem__
-# 存储 全局共享 数据
+
+# used for storing global shared data
 GSTORE = _GlobalStore()
 
 def INFO(info):
     """
-    在日志和测试报告中打印 重要信息，
-    使得 运行报告更加清晰
+    print information in log and report.
+    This will not show in terminal window.
 
-    参数：
-    @param info :   信息描述
+    Parameters
+    ----------
+    info : object to print
     """
     signal.info(f'{info}')
 
 def STEP(stepNo:int,desc:str):
     """
-    在日志和测试报告中打印出 测试步骤说明，
-    使得 运行报告更加清晰
+    print information about test steps in log and report .
+    This will not show in terminal window.
+
 
-    参数：
-    @param stepNo : 指定 是第几步
-    @param desc :   步骤描述
+    Parameters
+    ----------
+    stepNo : step number
+    desc :   description about this step
     """
     signal.step(stepNo,desc)
 
 
 def CHECK_POINT(desc:str, condition, failStop=True, failLogScreenWebDriver = None):
     """
-    检查点
-
-    参数：
-    @param desc :   检查点 文字描述
-    @param condition : 检查点 表达式
-    @param failStop : 检查点即使不通过也继续
-    @param failLogScreenWebDriver ： 如果检查错误，需要截屏，提供的webdirver对象
+    check point of testing.
+    pass or fail of this check point depends on argument condition is true or false.
+    it will print information about check point in log and report.
+
+    Parameters
+    ----------
+    desc :    check point description, like check what.
+    condition : usually it's a bool expression, like  `a==b`, 
+        so actually, after evaluating the expression, it's a result bool object passed in .
+    failStop : switch for whether continue this test cases when the condition is false 
+    failLogScreenWebDriver : Selenium web driver object,
+        when you want a screenshot image of browser in test report if current check point fail.
     """
 
     if condition:
         signal.checkpoint_pass(desc)
     else:
         signal.checkpoint_fail(desc)
 
@@ -64,28 +73,33 @@
         Runner.curRunningCase.stacktrace="\n"*3+('具体错误看测试步骤检查点','see checkpoint of case for details')[l.n]
         # 如果失败停止，中止此测试用例
         if failStop:
             raise AssertionError()
 
 def LOG_IMG(imgPath: str, width: str = None):
     """
-    在日志中加入图片
+    add image in test report
 
-    @param imgPath: 插入日志的图片路径
-    @param width:  图片html 显示宽度， 可以是 50% / 800px / 30em 这些格式
+    Parameters
+    ----------
+    imgPath: the path of image
+    width:  display width of image in html, like 50% / 800px / 30em 
     """
 
     signal.log_img(imgPath, width)
 
 
 def SELENIUM_LOG_SCREEN(driver, width: str = None):
     """
+    add screenshot image of browser into test report when using Selenium
     在日志中加入selenium控制的 浏览器截屏图片
 
-    @param driver: selenium webdriver对象
-    @param width:  图片html 显示宽度， 可以是 50% / 800px / 30em 这些格式
+    Parameters
+    ----------
+    driver: selenium webdriver
+    width:  display width of image in html, like 50% / 800px / 30em 
     """
     filename = datetime.now().strftime('%Y%m%d%H%M%S%f')
     filepath = f'log/imgs/{filename}.png'
     filepath_relative_to_log = f'imgs/{filename}.png'
     driver.get_screenshot_as_file(filepath)
     signal.log_img(filepath_relative_to_log, width)
```

## hytest/product.py

```diff
@@ -1 +1 @@
-version= '0.8.5'
+version= '0.8.6'
```

## hytest/run.py

```diff
@@ -18,21 +18,21 @@
     return ' or '.join(tagRules)
 
 def run() :
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', action='version', version=f'hytest v{version}',
                         help=("显示版本号", 'display hytest version')[l.n])
     parser.add_argument('--lang', choices=['zh', 'en'],
-                        help=("设置工具语言", 'set language to use')[l.n])
+                        help=("设置工具语言", 'set language')[l.n])
     parser.add_argument('--new', metavar='project_dir',
                         help=("创建新项目目录", "create a project folder")[l.n])
     parser.add_argument("case_dir", nargs='?', default='cases',
                         help=("用例根目录", "")[l.n])
     parser.add_argument("--loglevel", metavar='Level_Number', type=int, default=3,
-                        help=("日志级别  0,1,2,3,4,5(数字越大，日志越详细)", "log level 0,1,2,3,4,5(bigger for more info")[l.n])
+                        help=("日志级别 0,1,2,3,4,5(数字越大，日志越详细)", "log level 0,1,2,3,4,5(bigger for more info)")[l.n])
 
     parser.add_argument('--auto_open_report', choices=['yes', 'no'], default='yes',
                         help=("测试结束不自动打开报告", "don't open report automatically after testing")[l.n])
     parser.add_argument("--report_title", metavar='Report_Title',
                         default=['测试报告','Test Report'][l.n],
                         help=['指定测试报告标题','set test report title'][l.n])
     parser.add_argument("--report_url_prefix", metavar='Url_Prefix',
@@ -79,42 +79,52 @@
     if args.new:
         projDir =  args.new
         if os.path.exists(projDir):
             print(f'{projDir} already exists！')
             exit(2)
         os.makedirs(f'{projDir}/cases')
         with open(f'{projDir}/cases/case1.py','w',encoding='utf8') as f:
-            f.write('''class c1:
+            caseContent = [
+'''class c1:
     name = '用例名称 - 0001'
 
     # 测试用例步骤
-    def teststeps(self):...''')
+    def teststeps(self):
+        ret = 1
+        ''' ,
+
+'''class c1:
+    name = 'test case name - 0001'
+
+    # test case steps
+    def teststeps(self):...''',
+    ][l.n]
+            f.write(caseContent)
 
         exit()
 
 
     if not os.path.exists(args.case_dir) :
         print(f' {args.case_dir} {("目录不存在，工作目录为：","folder not exists, workding dir is:")[l.n]} {os.getcwd()}')
-        exit(2)  #  2 表示没有可以执行的用例
+        exit(2)  #  '2' stands for no test cases to run
 
     if not os.path.isdir(args.case_dir) :
         print(f' {args.case_dir}  {("不是目录，工作目录为：","is not a folder, workding dir is:")[l.n]} {os.getcwd()}')
-        exit(2) #  2 表示没有可以执行的用例
+        exit(2)  #  '2' stands for no test cases to run
 
     # 同时执行log里面的初始化日志模块，注册signal的代码
     from .utils.log import LogLevel
     from .utils.runner import Collector, Runner
 
     LogLevel.level = args.loglevel
     # print('loglevel',LogLevel.level)
 
 
     # --tag "'冒烟测试' and 'UITest' or (not '快速' and 'fast')" --tag 白月 --tag 黑羽
 
-
     tag_include_expr = tagExpressionGen(args.tag)
     tag_exclude_expr = tagExpressionGen(args.tagnot)
 
     # print(tag_include_expr)
     # print(tag_exclude_expr)
```

## hytest/utils/log.py

```diff
@@ -76,15 +76,15 @@
 
 
 class Stats:
 
     def test_start(self,_title='Test Report'):
         self.result = {
             # 这是准备执行的用例数量
-            'case_count_toberun': Collector.case_number,
+            'case_count_to_run': Collector.case_number,
             # 这个是实际执行的用例数量，可能有其他的用例因为初始化失败没有执行
             'case_count' : 0,
             'case_pass'  : 0,
             'case_fail'  : 0,
             'case_abort' : 0,
             'suite_setup_fail' : 0,
             'case_setup_fail' : 0,
@@ -146,15 +146,15 @@
     
     def test_end(self, runner):
         ret = stats.result
         print((f'\n\n  ========= 测试耗时 : {stats.test_duration:.3f} 秒 =========\n',
                f'\n\n  ========= Duration Of Testing : {stats.test_duration:.3f} seconds =========\n')[l.n])
 
 
-        print(f"\n  {('预备执行用例数量','number of cases to run')[l.n]} : {ret['case_count_toberun']}")
+        print(f"\n  {('预备执行用例数量','number of cases plan to run')[l.n]} : {ret['case_count_to_run']}")
 
         print(f"\n  {('实际执行用例数量','number of cases actually run')[l.n]} : {ret['case_count']}")
 
         print(f"\n  {('通过','passed')[l.n]} : {ret['case_pass']}", style='green')
         
         num = ret['case_fail']
         style = 'white' if num == 0 else 'bright_red'
@@ -266,15 +266,15 @@
         endTime = time.strftime('%Y%m%d_%H%M%S',
                                   time.localtime(stats.end_time))
         logger.info(f'\n\n  ========= {("测试结束","Test End")[l.n]} : {endTime} =========\n')
 
         logger.info(f"\n  {('耗时','Duration Of Testing ')[l.n]}    : {(stats.end_time-stats.start_time):.3f} 秒\n")
         ret = stats.result
 
-        logger.info(f"\n  {('预备执行用例数量','number of cases to run')[l.n]} : {ret['case_count_toberun']}")
+        logger.info(f"\n  {('预备执行用例数量','number of cases plan to run')[l.n]} : {ret['case_count_to_run']}")
         logger.info(f"\n  {('实际执行用例数量','number of cases actually run')[l.n]} : {ret['case_count']}")
         logger.info(f"\n  {('通过','passed')[l.n]} : {ret['case_pass']}")
         logger.info(f"\n  {('失败','failed')[l.n]} : {ret['case_fail']}")
         logger.info(f"\n  {('异常','exception aborted')[l.n]} : {ret['case_abort']}")
         logger.info(f"\n  {('套件初始化失败','suite setup failed')[l.n]} : {ret['suite_setup_fail']}")
         logger.info(f"\n  {('套件清除  失败','suite teardown failed')[l.n]} : {ret['suite_teardown_fail']}")
         logger.info(f"\n  {('用例初始化失败','cases setup failed')[l.n]} : {ret['case_setup_fail']}")
@@ -463,34 +463,34 @@
 
         trs = []
         trs.append(tr(td(('开始时间','Test Start Time')[l.n]), td(f'{execStartTime}')))
         trs.append(tr(td(('结束时间','Test End Time')[l.n]), td(f'{execEndTime}')))
 
         trs.append(tr(td(('耗时','Duration Of Testing')[l.n]), td(f'{stats.test_duration:.3f}' + (' 秒',' Seconds')[l.n])))
 
-        trs.append(tr(td(('预备执行用例数量','number of cases to run')[l.n]), td(f"{ret['case_count_toberun']}")))
+        trs.append(tr(td(('预备执行用例数量','number of cases plan to run')[l.n]), td(f"{ret['case_count_to_run']}")))
         trs.append(tr(td(('实际执用例行数量','number of cases actually run')[l.n]), td(f"{ret['case_count']}")))
 
         trs.append(tr(td(('通过','passed')[l.n]), td(f"{ret['case_pass']}")))
 
 
-        case_count_toberun = ret['case_count_toberun']
+        case_count_to_run = ret['case_count_to_run']
 
         num = ret['case_fail']
         style = '' if num == 0 else 'color:red'
         trs.append(tr(td(('失败','failed')[l.n]), td(f"{num}", style=style)))
         errorNum += num
         
         num = ret['case_abort']
         style = '' if num == 0 else 'color:red'
         trs.append(tr(td(('异常','exception aborted')[l.n]), td(f"{num}", style=style)))
         errorNum += num
 
         # 计算阻塞用例个数
-        blocked_num = case_count_toberun - ret['case_pass'] - ret['case_fail'] - ret['case_abort']
+        blocked_num = case_count_to_run - ret['case_pass'] - ret['case_fail'] - ret['case_abort']
         style = '' if blocked_num == 0 else 'color:red'
         trs.append(tr(td(('阻塞','blocked')[l.n]), td(f"{blocked_num}", style=style)))
         
         num = ret['suite_setup_fail']
         style = '' if num == 0 else 'color:red'
         trs.append(tr(td(('套件初始化失败','suite setup failed')[l.n]), td(f"{num}", style=style)))
         errorNum += num
@@ -551,34 +551,34 @@
 
 
         def percentCalc(upper,lower):
             percent = str(round(upper * 100 / lower, 1))
             percent = percent[:-2] if percent.endswith('.0') else percent
             return percent
 
-        percent = percentCalc(ret['case_pass'], case_count_toberun)
+        percent = percentCalc(ret['case_pass'], case_count_to_run)
         add_barchar_item(
             f"{('用例通过','cases passed')[l.n]} {percent}% ： {ret['case_pass']} {('个','')[l.n]}",
             float(percent),
             '#04AA6D')
 
-        percent = percentCalc(ret['case_fail'], case_count_toberun)
+        percent = percentCalc(ret['case_fail'], case_count_to_run)
         add_barchar_item(
             f"{('用例失败','cases failed')[l.n]} {percent}% ： {ret['case_fail']} {('个','')[l.n]}",
             float(percent),
             '#bb4069')
 
-        percent = percentCalc(ret['case_abort'], case_count_toberun)
+        percent = percentCalc(ret['case_abort'], case_count_to_run)
         add_barchar_item(
             f"{('用例异常','cases exception aborted')[l.n]} {percent}% ： {ret['case_abort']} {('个','')[l.n]}",
             float(percent),
             '#9c27b0')
 
 
-        percent = percentCalc(blocked_num, case_count_toberun)
+        percent = percentCalc(blocked_num, case_count_to_run)
         add_barchar_item(
             f"{('用例阻塞','cases blocked')[l.n]} {percent}% ： {blocked_num} {('个','')[l.n]}",
             float(percent),
             '#dcbdbd')
 
         # st_fail = ret['suite_setup_fail'] + ret['case_setup_fail'] + ret['suite_teardown_fail'] + ret['case_teardown_fail']
         # percent = '100%' if st_fail > 0 else '0%'
@@ -815,14 +815,15 @@
     def teardown_fail(self,name, utype, e, stacktrace):           
         self.curTeardownEle['class'] += ' fail'
 
         stacktrace = "Traceback:\n" +stacktrace.split("\n",3)[3]
         self.curEle += div(f'{utype} teardown fail | {e} \n{stacktrace}', _class='info error-info')
 
     def info(self, msg):
+        msg = f'{msg}'
         if self.curEle is None:
             return
 
         self.curEle += div(msg, _class='info')
 
 
     def step(self,stepNo,desc):
```

## hytest/utils/runner.py

```diff
@@ -74,15 +74,15 @@
             tag_include_expr=None,    
             tag_exclude_expr=None,   
             ):
 
 
         signal.info(
             ('\n\n===   [ 收集测试用例 ]  === \n',
-            '\n\n===   [ collect test cases ]  ****  === \n')[l.n]
+            '\n\n===   [ collect test cases ]  === \n')[l.n]
         )
 
         for (dirpath, dirnames, filenames) in os.walk(casedir):
             # 确保 __st__.py 在最前面
             if '__st__.py' in filenames:
                 filenames.remove('__st__.py')
                 filenames.insert(0,'__st__.py')
@@ -424,15 +424,15 @@
     def run(cls,):
         
         signal.info(
             ('\n\n===   [ 执行测试用例 ]  === \n',
             '\n\n===   [ execute test cases ]  === \n')[l.n]
         )
 
-        # 如果本次没有可以执行的用例（可能时过滤项原因），直接返回
+        # 如果本次没有可以执行的用例（可能是过滤项原因），直接返回
         if not Collector.exec_list:
             signal.error(('!! 没有可以执行的测试用例','!! No cases to run')[l.n])
             return 2 # 2 表示没有可以执行的用例
 
         signal.info(f"{('预备执行用例数量','Number of cases to run')[l.n]} : {Collector.case_number}\n")
 
         # 执行用例时，为每个用例分配一个id，方便测试报告里面根据id跳转到用例
```

## Comparing `hytest-0.8.5.dist-info/LICENSE.txt` & `hytest-0.8.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hytest-0.8.5.dist-info/METADATA` & `hytest-0.8.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hytest
-Version: 0.8.5
+Version: 0.8.6
 Summary: 一款系统测试自动化框架 Generic automation framework for QA testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hytest
 Author: 白月黑羽 - Jiangchunyang
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hytest automation testautomation
```

