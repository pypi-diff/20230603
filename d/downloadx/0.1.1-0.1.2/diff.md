# Comparing `tmp/downloadx-0.1.1.tar.gz` & `tmp/downloadx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "downloadx-0.1.1.tar", last modified: Sat Jun  3 10:04:58 2023, max compression
+gzip compressed data, was "downloadx-0.1.2.tar", last modified: Sat Jun  3 10:39:59 2023, max compression
```

## Comparing `downloadx-0.1.1.tar` & `downloadx-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:04:58.378137 downloadx-0.1.1/
--rw-r--r--   0 ruriazz    (501) staff       (20)      369 2023-06-03 10:04:58.377948 downloadx-0.1.1/PKG-INFO
--rw-r--r--   0 ruriazz    (501) staff       (20)       11 2023-06-03 09:59:52.000000 downloadx-0.1.1/README.md
-drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:04:58.374234 downloadx-0.1.1/downloadx/
--rw-r--r--   0 ruriazz    (501) staff       (20)       17 2023-06-03 10:04:42.000000 downloadx-0.1.1/downloadx/__init__.py
--rw-r--r--   0 ruriazz    (501) staff       (20)       78 2023-06-03 09:06:43.000000 downloadx-0.1.1/downloadx/__main__.py
--rw-r--r--   0 ruriazz    (501) staff       (20)      630 2023-06-03 07:24:37.000000 downloadx-0.1.1/downloadx/_typed.py
-drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:04:58.376412 downloadx-0.1.1/downloadx/cmd/
--rw-r--r--   0 ruriazz    (501) staff       (20)      814 2023-06-03 08:05:33.000000 downloadx-0.1.1/downloadx/cmd/__init__.py
--rw-r--r--   0 ruriazz    (501) staff       (20)     1010 2023-06-03 07:12:36.000000 downloadx-0.1.1/downloadx/cmd/__main__.py
--rw-r--r--   0 ruriazz    (501) staff       (20)      704 2023-06-03 07:12:34.000000 downloadx-0.1.1/downloadx/cmd/instagram_cli.py
--rw-r--r--   0 ruriazz    (501) staff       (20)     3528 2023-06-03 09:45:12.000000 downloadx-0.1.1/downloadx/cmd/youtube_cli.py
-drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:04:58.376931 downloadx-0.1.1/downloadx/helpers/
--rw-r--r--   0 ruriazz    (501) staff       (20)      285 2023-06-02 18:54:43.000000 downloadx-0.1.1/downloadx/helpers/enums.py
--rw-r--r--   0 ruriazz    (501) staff       (20)      206 2023-06-02 18:34:11.000000 downloadx-0.1.1/downloadx/helpers/strings.py
--rw-r--r--   0 ruriazz    (501) staff       (20)       53 2023-06-03 09:33:47.000000 downloadx-0.1.1/downloadx/requirements.txt
-drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:04:58.377645 downloadx-0.1.1/downloadx/utils/
--rw-r--r--   0 ruriazz    (501) staff       (20)      249 2023-06-02 18:24:34.000000 downloadx-0.1.1/downloadx/utils/__init__.py
--rw-r--r--   0 ruriazz    (501) staff       (20)     3225 2023-06-03 09:33:08.000000 downloadx-0.1.1/downloadx/utils/youtube.py
-drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:04:58.375175 downloadx-0.1.1/downloadx.egg-info/
--rw-r--r--   0 ruriazz    (501) staff       (20)      369 2023-06-03 10:04:58.000000 downloadx-0.1.1/downloadx.egg-info/PKG-INFO
--rw-r--r--   0 ruriazz    (501) staff       (20)      538 2023-06-03 10:04:58.000000 downloadx-0.1.1/downloadx.egg-info/SOURCES.txt
--rw-r--r--   0 ruriazz    (501) staff       (20)        1 2023-06-03 10:04:58.000000 downloadx-0.1.1/downloadx.egg-info/dependency_links.txt
--rw-r--r--   0 ruriazz    (501) staff       (20)       54 2023-06-03 10:04:58.000000 downloadx-0.1.1/downloadx.egg-info/entry_points.txt
--rw-r--r--   0 ruriazz    (501) staff       (20)       54 2023-06-03 10:04:58.000000 downloadx-0.1.1/downloadx.egg-info/requires.txt
--rw-r--r--   0 ruriazz    (501) staff       (20)       23 2023-06-03 10:04:58.000000 downloadx-0.1.1/downloadx.egg-info/top_level.txt
--rw-r--r--   0 ruriazz    (501) staff       (20)      735 2023-06-03 10:02:45.000000 downloadx-0.1.1/pyproject.toml
--rw-r--r--   0 ruriazz    (501) staff       (20)       38 2023-06-03 10:04:58.378184 downloadx-0.1.1/setup.cfg
+drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:39:59.043696 downloadx-0.1.2/
+-rw-r--r--   0 ruriazz    (501) staff       (20)      339 2023-06-02 20:37:03.000000 downloadx-0.1.2/.gitignore
+-rw-r--r--   0 ruriazz    (501) staff       (20)      588 2023-06-03 09:50:13.000000 downloadx-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 ruriazz    (501) staff       (20)     1801 2023-06-03 10:39:59.043528 downloadx-0.1.2/PKG-INFO
+-rw-r--r--   0 ruriazz    (501) staff       (20)     1285 2023-06-03 10:31:01.000000 downloadx-0.1.2/README.md
+drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:39:59.040557 downloadx-0.1.2/downloadx/
+-rw-r--r--   0 ruriazz    (501) staff       (20)       18 2023-06-03 10:33:10.000000 downloadx-0.1.2/downloadx/__init__.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)       79 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/__main__.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)      591 2023-06-03 10:32:09.000000 downloadx-0.1.2/downloadx/_typed.py
+drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:39:59.042354 downloadx-0.1.2/downloadx/cmd/
+-rw-r--r--   0 ruriazz    (501) staff       (20)      806 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/cmd/__init__.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)     1056 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/cmd/__main__.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)      767 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/cmd/instagram_cli.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)     3960 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/cmd/youtube_cli.py
+drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:39:59.042854 downloadx-0.1.2/downloadx/helpers/
+-rw-r--r--   0 ruriazz    (501) staff       (20)      285 2023-06-02 18:54:43.000000 downloadx-0.1.2/downloadx/helpers/enums.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)      207 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/helpers/strings.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)       53 2023-06-03 09:33:47.000000 downloadx-0.1.2/downloadx/requirements.txt
+drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:39:59.043307 downloadx-0.1.2/downloadx/utils/
+-rw-r--r--   0 ruriazz    (501) staff       (20)      250 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/utils/__init__.py
+-rw-r--r--   0 ruriazz    (501) staff       (20)     3228 2023-06-03 10:31:47.000000 downloadx-0.1.2/downloadx/utils/youtube.py
+drwxr-xr-x   0 ruriazz    (501) staff       (20)        0 2023-06-03 10:39:59.041451 downloadx-0.1.2/downloadx.egg-info/
+-rw-r--r--   0 ruriazz    (501) staff       (20)     1801 2023-06-03 10:39:59.000000 downloadx-0.1.2/downloadx.egg-info/PKG-INFO
+-rw-r--r--   0 ruriazz    (501) staff       (20)      573 2023-06-03 10:39:59.000000 downloadx-0.1.2/downloadx.egg-info/SOURCES.txt
+-rw-r--r--   0 ruriazz    (501) staff       (20)        1 2023-06-03 10:39:59.000000 downloadx-0.1.2/downloadx.egg-info/dependency_links.txt
+-rw-r--r--   0 ruriazz    (501) staff       (20)       54 2023-06-03 10:39:59.000000 downloadx-0.1.2/downloadx.egg-info/entry_points.txt
+-rw-r--r--   0 ruriazz    (501) staff       (20)       54 2023-06-03 10:39:59.000000 downloadx-0.1.2/downloadx.egg-info/requires.txt
+-rw-r--r--   0 ruriazz    (501) staff       (20)       23 2023-06-03 10:39:59.000000 downloadx-0.1.2/downloadx.egg-info/top_level.txt
+-rw-r--r--   0 ruriazz    (501) staff       (20)      894 2023-06-03 10:39:46.000000 downloadx-0.1.2/pyproject.toml
+-rw-r--r--   0 ruriazz    (501) staff       (20)       38 2023-06-03 10:39:59.043734 downloadx-0.1.2/setup.cfg
```

### Comparing `downloadx-0.1.1/downloadx/_typed.py` & `downloadx-0.1.2/downloadx/_typed.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from enum import Enum
-from pydantic import BaseModel, Field, validator
-from pytube.streams import Stream
+
+from pydantic import BaseModel, Field
 
 
 class CLIMode(Enum):
-    YOUTUBE = 'youtube'
-    INSTAGRAM = 'instagram'
+    YOUTUBE = "youtube"
+    INSTAGRAM = "instagram"
+
 
 class MainCLI(BaseModel):
     mode: str
 
+
 class YoutubeCLI(MainCLI):
     url: str | None
     url_file: str | None
     audio_only: bool
     output: str
     urls: list[str] = Field(default=[])
 
+
 class InstagramCLI(MainCLI):
     url: str | None
     url_file: str | None
 
+
 class YouTubeStream(BaseModel):
     itag: int
     str_size: str
     resolution: str
 
+
 class YouTubeInfo(BaseModel):
     title: str
     streams: list[YouTubeStream] = Field(default=[])
```

### Comparing `downloadx-0.1.1/downloadx/cmd/__init__.py` & `downloadx-0.1.2/downloadx/cmd/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import os
 import sys
 from abc import ABC
 
 
 class Command(ABC):
     def clear(self) -> None:
-        os.system('cls' if os.name == 'nt' else 'clear')
+        os.system("cls" if os.name == "nt" else "clear")
 
     def confirm(self, message: str) -> bool:
         if message:
             message += "\n\n"
         confirmation = input(f"{message}Are you sure you want to proceed? (y/n): ")
-        return confirmation.lower() == 'y'
+        return confirmation.lower() == "y"
 
     def abort(self, message: str = "") -> None:
         if message:
             message = f"\n{message.strip()}"
 
-        message = message or ''
+        message = message or ""
         print(f"\033[F\033[K\n🚫 abort {message}")
-        
-        sys.exit(0)
 
+        sys.exit(0)
 
     def ok(self, message: str = "") -> None:
         if message:
             message = f"\n{message.strip()}"
 
-        message = message or ''
+        message = message or ""
         print(f"\033[F\033[K\n✅ OK {message}")
-        sys.exit(0)
+        sys.exit(0)
```

### Comparing `downloadx-0.1.1/downloadx/cmd/__main__.py` & `downloadx-0.1.2/downloadx/cmd/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import argparse
+
+from downloadx._typed import CLIMode, MainCLI
 from downloadx.cmd import Command as _Command
-from downloadx.cmd.youtube_cli import YoutubeCLI
 from downloadx.cmd.instagram_cli import InstagramCLI
-from downloadx._typed import CLIMode, MainCLI
+from downloadx.cmd.youtube_cli import YoutubeCLI
 from downloadx.helpers import enums
 
 
 class Command(_Command):
     def __init__(self) -> None:
         super().__init__()
 
         parser = argparse.ArgumentParser(description="DownloadX CLI")
-        subparser = parser.add_subparsers(title='DownloadX CLI Mode', dest='mode')
+        subparser = parser.add_subparsers(title="DownloadX CLI Mode", dest="mode")
 
-        youtube_cli = YoutubeCLI(parser, subparser.add_parser("youtube", help="YouTube CLI"))
-        instagram_cli = InstagramCLI(parser, subparser.add_parser("instagram", help="Instagram CLI"))
+        youtube_cli = YoutubeCLI(
+            parser, subparser.add_parser("youtube", help="YouTube CLI")
+        )
+        instagram_cli = InstagramCLI(
+            parser, subparser.add_parser("instagram", help="Instagram CLI")
+        )
 
         switcher = {
             CLIMode.YOUTUBE.value: youtube_cli,
-            CLIMode.INSTAGRAM.value: instagram_cli
+            CLIMode.INSTAGRAM.value: instagram_cli,
         }
 
         args = MainCLI(**parser.parse_args().__dict__)
 
         if mode := enums.from_str(CLIMode, args.mode):
             if func := switcher.get(mode.value):
                 return func.exec()
```

### Comparing `downloadx-0.1.1/downloadx/cmd/youtube_cli.py` & `downloadx-0.1.2/downloadx/cmd/youtube_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,46 @@
-
 import argparse
-from downloadx.cmd import Command as _Coomand
+
 from downloadx._typed import YoutubeCLI as _YoutubeCLI
+from downloadx.cmd import Command as _Coomand
 from downloadx.helpers.strings import is_url
 from downloadx.utils.youtube import Youtube
 
 
 class YoutubeCLI(_Coomand):
     _parser: argparse.ArgumentParser
 
-    def __init__(self, parser: argparse.ArgumentParser, sp: argparse.ArgumentParser) -> None:
+    def __init__(
+        self, parser: argparse.ArgumentParser, sp: argparse.ArgumentParser
+    ) -> None:
         super().__init__()
 
         self._parser = parser
-        sp.add_argument("-u", "--url", type=str, help="single url download", dest="url", metavar='')
-        sp.add_argument("-f", "--url-file", type=str, help="multiple url download by defining url inside a file", metavar='')
-        sp.add_argument("-o", "--output", help="folder to save downloaded files. default is './outputs' directory", default='outputs', metavar='')
-        sp.add_argument("--audio-only", help="download audio only (.mp3)", action="store_true")
+        sp.add_argument(
+            "-u", "--url", type=str, help="single url download", dest="url", metavar=""
+        )
+        sp.add_argument(
+            "-f",
+            "--url-file",
+            type=str,
+            help="multiple url download by defining url inside a file",
+            metavar="",
+        )
+        sp.add_argument(
+            "-o",
+            "--output",
+            help="folder to save downloaded files. default is './outputs' directory",
+            default="outputs",
+            metavar="",
+        )
+        sp.add_argument(
+            "--audio-only", help="download audio only (.mp3)", action="store_true"
+        )
 
-        parser.parse_args(['youtube'])
+        parser.parse_args(["youtube"])
 
     def exec(self) -> None:
         args = self._optimize_args()
 
         urls = [f"\n> {i}" for i in args.urls]
         if self.confirm(f'\nURL of the content to be downloaded:{"".join(urls)}'):
             queues: list[dict] = []
@@ -32,62 +50,71 @@
                 if args.audio_only:
                     yt.download_audio(args.output)
                     continue
 
                 yt.init_video()
                 choices: list[str] = []
                 for i, stream in enumerate(yt._instance_info.streams):
-                    choices.append(f"\n   {i + 1}. \u0009{stream.resolution} - {stream.str_size}")
+                    choices.append(
+                        f"\n   {i + 1}. \u0009{stream.resolution} - {stream.str_size}"
+                    )
 
                 _range = len(choices)
                 if _range > 1:
                     _range = f"1 - {_range}"
 
                 idx = 0
                 while True:
                     try:
                         self.clear()
-                        idx = int(input(f"\nplease select the resolution to download for '{yt._instance_info.title}': {''.join(choices)} \n\n[{_range}]: "))
+                        idx = int(
+                            input(
+                                f"\nplease select the resolution to download for '{yt._instance_info.title}': {''.join(choices)} \n\n[{_range}]: "
+                            )
+                        )
                         if idx >= 1 and idx <= len(choices):
                             idx -= 1
                             break
                     except Exception:
                         pass
 
-                queues.append({
-                    'func': yt.download_video,
-                    'arg': yt._instance_info.streams[idx]
-                })
+                queues.append(
+                    {"func": yt.download_video, "arg": yt._instance_info.streams[idx]}
+                )
 
             if queues:
                 self.clear()
                 for queue in queues:
-                    queue['func'](queue['arg'])
+                    queue["func"](queue["arg"], args.output)
 
             self.ok()
 
     def _optimize_args(self) -> _YoutubeCLI:
         args = _YoutubeCLI(**self._parser.parse_args().__dict__)
 
         if not args.url and not args.url_file:
-            self.abort("there is no content to download. you need to provide a value in the --url or --url-file argument")
+            self.abort(
+                "there is no content to download. you need to provide a value in the --url or --url-file argument"
+            )
 
         args.urls = []
-        if url := is_url(args.url or ''):
+        if url := is_url(args.url or ""):
             args.urls.append(url)
-        elif args.url is not None and args.url != '':
+        elif args.url is not None and args.url != "":
             self.abort(f"'{args.url}' is not valid YouTube url")
 
         if file := args.url_file:
             try:
-                with open(file, 'r') as f:
-                    contents = [i.strip() for i in f.read().split('\n') if i.strip() != '']
+                with open(file, "r") as f:
+                    contents = [
+                        i.strip() for i in f.read().split("\n") if i.strip() != ""
+                    ]
                     for url in contents:
                         if u := is_url(url):
                             args.urls.append(u)
                             continue
 
                         self.abort(f"'{url}' is not valid YouTube url")
             except Exception as err:
                 self.abort(str(err))
 
-        return args
+        return args
```

### Comparing `downloadx-0.1.1/downloadx/utils/youtube.py` & `downloadx-0.1.2/downloadx/utils/youtube.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 from pathlib import Path
-from downloadx.utils import Utils
-from downloadx.helpers.strings import is_url
-from downloadx._typed import YouTubeInfo, YouTubeStream
-from pytube import YouTube as _Youtube
+
 from alive_progress import alive_bar
+from pytube import YouTube as _Youtube
+
+from downloadx._typed import YouTubeInfo, YouTubeStream
+from downloadx.helpers.strings import is_url
+from downloadx.utils import Utils
 
 
 class Youtube(Utils):
     _is_title: bool = True
 
     _instance: _Youtube
     _instance_info: YouTubeInfo
@@ -25,66 +27,69 @@
 
     def verify(self) -> None:
         try:
             self._instance.check_availability()
         except Exception as err:
             self.is_error(err)
 
-    def download_audio(self, output: str = 'outputs') -> None:
-        aud = self._instance \
-            .streams \
-            .filter(only_audio=True) \
-            .first()
+    def download_audio(self, output: str = "outputs") -> None:
+        aud = self._instance.streams.filter(only_audio=True).first()
 
         if not aud:
-            return self.is_error(Exception('content not found'))
+            return self.is_error(Exception("content not found"))
 
         if not os.path.exists(Path(output)):
             os.makedirs(output, exist_ok=True)
 
-        filename = f"{aud.title}.mp3" if not self._is_title else f"{aud.title.title()}.mp3"
+        filename = (
+            f"{aud.title}.mp3" if not self._is_title else f"{aud.title.title()}.mp3"
+        )
         file_save = Path(output).joinpath(filename).as_posix()
 
         print(f"\033[F\033[K > {self._instance.watch_url}: {filename}")
         with alive_bar(round(aud.filesize_mb)) as bar:
+
             def on_prog(s, c, b) -> None:
                 bar(len(c) / (1024 * 1024))
 
             self._instance.register_on_progress_callback(on_prog)
             aud.download(filename=file_save, skip_existing=True, max_retries=3)
             bar(aud.filesize_mb)
 
     def init_video(self) -> None:
-        streams = self._instance \
-            .streams \
-            .filter(type='video', progressive=True)
+        streams = self._instance.streams.filter(type="video", progressive=True)
 
         self._instance_info = YouTubeInfo(title=self._instance.title)
         for stream in streams:
             _stream = YouTubeStream(
                 itag=stream.itag,
                 resolution=f"{stream.resolution} {stream.mime_type.split('/')[1]}",
-                str_size=f"{round(stream.filesize_mb, 1)} MB"
+                str_size=f"{round(stream.filesize_mb, 1)} MB",
             )
 
             self._instance_info.streams.append(_stream)
 
-    def download_video(self, stream: YouTubeStream, output: str = 'outputs') -> None:
+    def download_video(self, stream: YouTubeStream, output: str = "outputs") -> None:
         _stream = self._instance.streams.get_by_itag(stream.itag)
         if not _stream:
             raise Exception(f"No stream found with itag '{stream.itag}'")
 
         if not os.path.exists(Path(output)):
             os.makedirs(output, exist_ok=True)
 
-        ext = _stream.mime_type.split('/')[1]
-        filename = f"{_stream.title}.{ext}" if not self._is_title else f"{_stream.title.title()}.{ext}"
+        ext = _stream.mime_type.split("/")[1]
+        filename = (
+            f"{_stream.title}.{ext}"
+            if not self._is_title
+            else f"{_stream.title.title()}.{ext}"
+        )
         file_save = Path(output).joinpath(filename).as_posix()
 
         print(f"\033[F\033[K > {self._instance.watch_url}: {filename}")
         with alive_bar(round(_stream.filesize_mb)) as bar:
+
             def on_prog(s, c, b) -> None:
                 bar(len(c) / (1024 * 1024))
 
             self._instance.register_on_progress_callback(on_prog)
             _stream.download(filename=file_save, skip_existing=True, max_retries=3)
-            bar(_stream.filesize_mb)
+            bar(_stream.filesize_mb)
```

### Comparing `downloadx-0.1.1/downloadx.egg-info/SOURCES.txt` & `downloadx-0.1.2/downloadx.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.gitignore
+.pre-commit-config.yaml
 README.md
 pyproject.toml
 downloadx/__init__.py
 downloadx/__main__.py
 downloadx/_typed.py
 downloadx/requirements.txt
 downloadx.egg-info/PKG-INFO
```

### Comparing `downloadx-0.1.1/pyproject.toml` & `downloadx-0.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 name = "downloadx"
 authors = [{ name = "ruriazz", email = "azizruri.s@gmail.com" }]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
 ]
-description = "DownloadX CLI"
+description = "DownloadX CLI - Content download CLI tools"
 dynamic = ["version", "dependencies"]
 keywords = ["downloadx", "DownloadX"]
 readme = "README.md"
 requires-python = ">=3.10"
 
 [project.scripts]
 downloadx = "downloadx.__main__:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "downloadx.VERSION"}
 dependencies = {file = ["downloadx/requirements.txt"]}
 
 [tool.setuptools.packages.find]
-exclude = ["tests*", "example*"]
+exclude = ["tests*", "example*"]
+
+[project.urls]
+"Homepage" = "https://github.com/ruriazz/downloadx"
+"Bug Tracker" = "https://github.com/ruriazz/downloadx/issues"
```

