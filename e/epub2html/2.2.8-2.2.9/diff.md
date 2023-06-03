# Comparing `tmp/epub2html-2.2.8-py2.py3-none-any.whl.zip` & `tmp/epub2html-2.2.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 69639 bytes, number of entries: 11
+Zip file size: 69545 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      191 b- defN 20-Feb-16 09:41 epub2html/__init__.py
 -rw-r--r--  2.0 unx       81 b- defN 20-Feb-15 16:01 epub2html/__main__.py
--rw-r--r--  2.0 unx     7993 b- defN 20-Feb-16 17:17 epub2html/epub2html.py
+-rw-r--r--  2.0 unx     7566 b- defN 20-Feb-16 18:13 epub2html/epub2html.py
 -rw-r--r--  2.0 unx    95785 b- defN 20-Feb-16 10:14 epub2html/jquery.min.js
 -rw-r--r--  2.0 unx   100220 b- defN 20-Feb-16 16:04 epub2html/leader-line.min.js
 -rw-r--r--  2.0 unx     5657 b- defN 20-Feb-16 13:32 epub2html/template.html
--rw-r--r--  2.0 unx     1347 b- defN 20-Feb-16 17:28 epub2html-2.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Feb-16 17:28 epub2html-2.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 20-Feb-16 17:28 epub2html-2.2.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 20-Feb-16 17:28 epub2html-2.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      884 b- defN 20-Feb-16 17:28 epub2html-2.2.8.dist-info/RECORD
-11 files, 212331 bytes uncompressed, 68149 bytes compressed:  67.9%
+-rw-r--r--  2.0 unx     1347 b- defN 20-Feb-16 18:14 epub2html-2.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 20-Feb-16 18:14 epub2html-2.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 20-Feb-16 18:14 epub2html-2.2.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 20-Feb-16 18:14 epub2html-2.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      884 b- defN 20-Feb-16 18:14 epub2html-2.2.9.dist-info/RECORD
+11 files, 211904 bytes uncompressed, 68055 bytes compressed:  67.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: epub2html/leader-line.min.js
 Comment: 
 
 Filename: epub2html/template.html
 Comment: 
 
-Filename: epub2html-2.2.8.dist-info/METADATA
+Filename: epub2html-2.2.9.dist-info/METADATA
 Comment: 
 
-Filename: epub2html-2.2.8.dist-info/WHEEL
+Filename: epub2html-2.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: epub2html-2.2.8.dist-info/entry_points.txt
+Filename: epub2html-2.2.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: epub2html-2.2.8.dist-info/top_level.txt
+Filename: epub2html-2.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: epub2html-2.2.8.dist-info/RECORD
+Filename: epub2html-2.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## epub2html/epub2html.py

```diff
@@ -58,62 +58,74 @@
 
         return imagePath, textPath
 
     def getIndexLoc(self):
         return self.indexHtmlLoc
 
     
-    def _genMemuTree(self,node,need_hash_names,ulist,depth=0):
+    def _genMemuTree(self,node,need_hash_names,menu_names,ulist,depth=0):
         for cc in node.findall("."):
             name = cc.find("./navLabel/text").text.strip()
             link = cc.find("./content")
             attrib = link.attrib["src"]
+            
+            htmlpath  = re.findall(".+html",attrib)
+            if len(htmlpath)> 0:
+                n = htmlpath[0]
+                n = n.split("/")[-1]
+                if n not in menu_names:
+                    menu_names.append(n)
+
             # only page link, no hash jump
             if '#' not in attrib:
                 short_link = attrib.split('/')[-1]
-                attrib = "#"+self.hash(short_link)
                 need_hash_names.append(short_link)
+
+                attrib = "#"+self.hash(short_link)
+                attrib="index.html"+attrib
             else:
-                print("attrib",attrib)
+                attrib=re.sub(r".+html","index.html",attrib)
+            print("attrib",attrib)
 
-                attrib=re.sub(r"^.+html","index.html",attrib)
+            
 
             ulist.append(f"<li><a href=\"{attrib}\">{name}</a></li>")
 
             subs =cc.findall("./navPoint")
             if len(subs)>0:
                 for d in subs:
                     ulist.append("<ul>")
-                    self._genMemuTree(d,need_hash_names,ulist,depth+1)
+                    self._genMemuTree(d,need_hash_names,menu_names,ulist,depth+1)
                     ulist.append("</ul>")
 
     def genMemuTree(self,path):
         print("path",path)
         contents = Path(path).read_text()
         contents = re.sub(' xmlns="[^"]+"', '', contents, count=1)
         contents = contents.encode('utf-8')
         root = etree.fromstring(contents)
         ulist =[]
         need_hash_names = []
+        menu_names = []
         ulist.append("<ul class=\"nav nav-sidebar \">")
         for c in root.findall("./navMap/navPoint"):
-            self._genMemuTree(c,need_hash_names,ulist,0)
+            self._genMemuTree(c,need_hash_names,menu_names,ulist,0)
         ulist.append("</ul>")
-        return "\n".join(ulist),need_hash_names
+        return "\n".join(ulist),need_hash_names,menu_names
 
     def unzip(self):
         with zipfile.ZipFile(self.epubpath,'r') as zip_ref:
             zip_ref.extractall(self.outputdirSplashOnlyname)
 
 
 
-    def genContent(self,hash_files):
+    def genContent(self,hash_files,menu_names):
         content_list = []
         # print("self.textdir",self.textdir)
-        for only_name in  self.traverse(self.textdir):
+        for only_name in  menu_names:
             if only_name in  ["part0000.html","part0001.html"]:
                 continue
 
             full_path = os.path.join(self.textdir,only_name)
             raw_content = Path(full_path).read_text()
 
 
@@ -153,39 +165,20 @@
                 return filenames 
     def hash(self, s):
         import base64
         tag = base64.b64encode(s.encode('ascii'))
         tag = tag.decode("ascii")
         return tag
 
-    def genMenu(self,menuhtmlname):
-        raw_menu =Path(join(self.textdir,menuhtmlname)).read_text()
-        raw_menu = raw_menu.encode('utf-8')
-        raw_menu_dom = etree.HTML(raw_menu)
-        parts = raw_menu_dom.xpath("//body/*")
-        raw_menus = []
-        need_hash_names = []
-        for p in parts:
-            raw_menu = etree.tostring(p,method='html').decode('utf-8')
-            # only page link, no hash jump
-            a = re.search("\"part\d+.html\"",raw_menu)
-            if a:
-                need_hash_names.append(a.group())
-                raw_menu = re.sub("(part\d+.html)","#"+self.hash(a.group()),raw_menu)
-            else:
-                raw_menu=re.sub(r"part\w+\.html","",raw_menu)
-            
-            raw_menus.append(raw_menu) 
-        return "".join(raw_menus),need_hash_names
 
     
     def gen(self):
-        menu, hash_files= self.genMemuTree(os.path.join(self.outputdirSplashOnlyname,"toc.ncx"))
+        menu, hash_files, menu_names= self.genMemuTree(os.path.join(self.outputdirSplashOnlyname,"toc.ncx"))
 
-        full_content = self.genContent(hash_files)
+        full_content = self.genContent(hash_files,menu_names)
 
         self.template = self.template.replace("${menu}$",menu)
         self.template = self.template.replace("${content}$",full_content)
         Path(join(self.outputdir, self.only_name,"./index.html")).write_text(self.template)
         self.copyJs()
 
     def copyJs(self):
@@ -203,18 +196,18 @@
     outputdir =tempfile.gettempdir()
     if args.outputdir:
         outputdir = os.path.abspath(args.outputdir)
 
     e = Epub2Html(filepath,outputdir)
     e.gen()
     print("converted! "+ e.getIndexLoc())
-    if sys.platform == 'darwin':
-        bashCommand = "open '" + e.getIndexLoc() +"'"
-        subprocess.check_call(bashCommand,
-                              shell=True)
+    # if sys.platform == 'darwin':
+    #     bashCommand = "open '" + e.getIndexLoc() +"'"
+    #     subprocess.check_call(bashCommand,
+    #                           shell=True)
 
 
 
 def entry_point():
     parser = createParse()
     mainArgs=parser.parse_args()
     main(mainArgs)
```

## Comparing `epub2html-2.2.8.dist-info/METADATA` & `epub2html-2.2.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epub2html
-Version: 2.2.8
+Version: 2.2.9
 Summary: this is a description
 Home-page: https://github.com/zk4/epub2html
 Author: zk
 Author-email: liuzq7@gmail.com
 License: BSD
 Download-URL: https://github.com/zk4/epub2html/archive/master.zip
 Keywords: best practice for python project
```

## Comparing `epub2html-2.2.8.dist-info/RECORD` & `epub2html-2.2.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 epub2html/__init__.py,sha256=qS-e5kcaUCljmUzYLvwfcpLC1sns-068d_-IA0R7EBY,191
 epub2html/__main__.py,sha256=NdX6IzCDYNwkqIaCdVYJjWoiCOSrimbsRWfMcIidCAE,81
-epub2html/epub2html.py,sha256=PcaPqW7lniebDqiu_YBeCdpq_ykuj3DBC4qqPg9RtlQ,7993
+epub2html/epub2html.py,sha256=qjGrhJzdN9Ijq5HCiElCtfh81wi2UgBBFwe-IH9HWX4,7566
 epub2html/jquery.min.js,sha256=JCYrqv7xcJKSfD2v52SqpSoqNxuD7SJJzKfkFN-Z-sE,95785
 epub2html/leader-line.min.js,sha256=NyE3tVrpLCon8XyRk8WWlPyOmx3VMUmda7Z7J7RN4B8,100220
 epub2html/template.html,sha256=H7BMTUTCDoqOWMy-jaiREAcd6qlEcUn7fr1-G-aMrSw,5657
-epub2html-2.2.8.dist-info/METADATA,sha256=nGV4TQ2aSrWqVU6AYJyd40QXVCj0Av_mAqPsdNTL7Qg,1347
-epub2html-2.2.8.dist-info/WHEEL,sha256=_wJFdOYk7i3xxT8ElOkUJvOdOvfNGbR9g-bf6UQT6sU,110
-epub2html-2.2.8.dist-info/entry_points.txt,sha256=Egr7eeM9yU3ijbnnfXlirWZwDa8RF1jeH-LuSU-QDf0,53
-epub2html-2.2.8.dist-info/top_level.txt,sha256=_vcDrnLuHoXleRpS_eFSKnuCuzx5jVOYWNF1wt4QB3Q,10
-epub2html-2.2.8.dist-info/RECORD,,
+epub2html-2.2.9.dist-info/METADATA,sha256=6vCxz2LnjT30uI2642edpUewKdy5hKp4vze5RM-Z6W0,1347
+epub2html-2.2.9.dist-info/WHEEL,sha256=_wJFdOYk7i3xxT8ElOkUJvOdOvfNGbR9g-bf6UQT6sU,110
+epub2html-2.2.9.dist-info/entry_points.txt,sha256=Egr7eeM9yU3ijbnnfXlirWZwDa8RF1jeH-LuSU-QDf0,53
+epub2html-2.2.9.dist-info/top_level.txt,sha256=_vcDrnLuHoXleRpS_eFSKnuCuzx5jVOYWNF1wt4QB3Q,10
+epub2html-2.2.9.dist-info/RECORD,,
```

