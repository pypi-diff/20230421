# Comparing `tmp/avplib-1.4.1.tar.gz` & `tmp/avplib-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avplib-1.4.1.tar", last modified: Mon Mar 27 16:11:31 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "avplib-1.4.5.tar", last modified: Thu Apr 20 19:15:58 2023, max compression
```

## Comparing `avplib-1.4.1.tar` & `avplib-1.4.5.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 16:10:57.279984 avplib-1.4.1/
-drwxrwxrwx   0        0        0        0 2023-03-27 16:10:57.273776 avplib-1.4.1/avplib/
--rw-rw-rw-   0        0        0     2233 2023-03-27 16:02:25.000000 avplib-1.4.1/avplib/avf.py
--rw-rw-rw-   0        0        0     6175 2023-03-27 16:02:05.000000 avplib-1.4.1/avplib/avplib.py
--rwxrwxrwx   0        0        0     1352 2023-03-23 11:28:36.000000 avplib-1.4.1/avplib/avplib.pyi
--rw-rw-rw-   0        0        0      275 2022-11-10 17:45:04.000000 avplib-1.4.1/avplib/units.py
--rw-rw-rw-   0        0        0       38 2023-03-23 11:32:25.000000 avplib-1.4.1/avplib/__init__.py
--rw-rw-rw-   0        0        0     9325 2023-03-27 15:53:46.000000 avplib-1.4.1/avplib/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 16:10:57.278985 avplib-1.4.1/avplib.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-27 16:10:57.000000 avplib-1.4.1/avplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2295 2023-03-27 16:10:57.000000 avplib-1.4.1/avplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       79 2023-03-27 16:10:57.000000 avplib-1.4.1/avplib.egg-info/requires.txt
--rw-rw-rw-   0        0        0      252 2023-03-27 16:10:57.000000 avplib-1.4.1/avplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-03-27 16:10:57.000000 avplib-1.4.1/avplib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2295 2023-03-27 16:10:57.279984 avplib-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-03-27 16:06:22.000000 avplib-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-27 16:10:57.279984 avplib-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      813 2023-03-27 16:10:52.000000 avplib-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:15:58.588413 avplib-1.4.5/
+-rw-rw-rw-   0        0        0     2295 2023-04-20 19:15:58.588413 avplib-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1948 2023-03-27 16:06:22.000000 avplib-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 19:15:58.582410 avplib-1.4.5/avplib/
+-rw-rw-rw-   0        0        0       97 2023-04-20 19:03:28.000000 avplib-1.4.5/avplib/__init__.py
+-rw-rw-rw-   0        0        0    10154 2023-04-20 19:13:39.000000 avplib-1.4.5/avplib/__main__.py
+-rw-rw-rw-   0        0        0     2359 2023-04-20 18:38:12.000000 avplib-1.4.5/avplib/avf.py
+-rw-rw-rw-   0        0        0     8105 2023-04-20 12:53:03.000000 avplib-1.4.5/avplib/avplib.py
+-rw-rw-rw-   0        0        0      275 2023-04-20 18:51:04.000000 avplib-1.4.5/avplib/units.py
+drwxrwxrwx   0        0        0        0 2023-04-20 19:15:58.586425 avplib-1.4.5/avplib.egg-info/
+-rw-rw-rw-   0        0        0     2295 2023-04-20 19:15:58.000000 avplib-1.4.5/avplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-20 19:15:58.000000 avplib-1.4.5/avplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 19:15:58.000000 avplib-1.4.5/avplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-04-20 19:15:58.000000 avplib-1.4.5/avplib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 19:15:58.000000 avplib-1.4.5/avplib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 19:15:58.588413 avplib-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      813 2023-04-20 19:04:12.000000 avplib-1.4.5/setup.py
```

### Comparing `avplib-1.4.1/avplib/avf.py` & `avplib-1.4.5/avplib/avf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import pathlib
 from zipfile import ZipFile, ZIP_DEFLATED
 from tempfile import NamedTemporaryFile
 from typing import Tuple, List, Dict, Any, Literal, Union, TypeVar
+from .units import ASCII_CHARS
 
 T = TypeVar("T")
 D = TypeVar("D")
 
 def removes(l: List[Union[T, D]], rl: List[D]) -> List[T]:
     for i in rl:
         for i in range(l.count(i)):
@@ -24,25 +25,27 @@
     
     def set_info(
         self,
         title: str="",
         author: str="",
         fps: int=1,
         res: Tuple[int, int]=(1,1),
-        exists_audio: bool=False
+        exists_audio: bool=False,
+        ascii_chars: List[str]=ASCII_CHARS
     ) -> None:
         self.fp.writestr(
             "info",
             json.dumps(
                 {
                     "title": title,
                     "author": author,
                     "fps": fps,
                     "res": res,
-                    "exists_audio": exists_audio
+                    "exists_audio": exists_audio,
+                    "ascii_chars": ascii_chars
                 }
             )
         )
     
     def get_info(self) -> Dict[str, Any]:
         return json.loads(self.fp.read("info"))
```

### Comparing `avplib-1.4.1/avplib/avplib.py` & `avplib-1.4.5/avplib/avplib.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import time
 import moviepy.editor as mp
 import soundfile as sf
 from PIL import Image
 from io import BufferedReader, BytesIO
 from tempfile import NamedTemporaryFile
 from threading import Thread
+from multiprocessing import Process, Pipe
+from multiprocessing.connection import PipeConnection
 # > Typing
-from typing import Literal, Any, Optional, Tuple
+from typing import Literal, Any, Optional, Tuple, List
 # > Local Imports
-from .units import ASCII_CHARS_GRADIENTION
+from .units import ASCII_CHARS_GRADIENTION, ASCII_CHARS
 
 # > Temp Detected
 class TempDetected:
     def __init__(self) -> None:
         self.files = []
     def append(self, path: str) -> None: self.files.append(path)
     def clear(self) -> None:
@@ -24,14 +26,22 @@
 
 # > Initilation
 TEMP_DETECTOR = TempDetected()
 
 # > Functions
 def _callback(complited: int, total: int): ...
 
+def generate_ascii_chars_gradient(ascii_chars: List[str]=ASCII_CHARS) -> List[str]:
+    ascii_chars_gradient_k = int(256 / len(ascii_chars)) + 1
+    return [ascii_chars[i // ascii_chars_gradient_k] for i in range(0, 257)]
+
+def generate_ascii_frame(image_frame, frame_size: Tuple[int, int], ascii_chars_gradient: List[str]=ASCII_CHARS_GRADIENTION) -> str:
+    ac = "".join([ascii_chars_gradient[pixel] for pixel in Image.fromarray(image_frame).convert("L").resize(frame_size).getdata()])
+    return "\n".join([ac[index:(index+frame_size[0])] for index in range(0, len(ac), frame_size[0])])
+
 # > Classes
 class ProgressiveList:
     def __init__(
         self,
         max_size: int=256,
         pass_data: Optional[Any]=None
     ) -> None:
@@ -55,35 +65,70 @@
         c = 0
         for i in self.data: c += (1 if i != self.pass_data else 0)
         return c
     
     def clear(self) -> None: self.data = [self.pass_data for i in range(0, self.max_size)]
 
 class ThreadingFrameHandler:
-    def __init__(self, frames_count: int, frame_size: Tuple[int, int], callback=_callback) -> None:
+    def __init__(
+        self,
+        frames_count: int,
+        frame_size: Tuple[int, int],
+        callback=_callback,
+        ascii_chars_gradient: List[str]=ASCII_CHARS_GRADIENTION
+    ) -> None:
         self.frames_count = frames_count
         self.frame_size = frame_size
         self.pl = ProgressiveList(frames_count)
         self.done = 1
         self.callback = callback
+        self.ascii_chars_gradient = ascii_chars_gradient
     
     def _gaf(self, idx: int, data: Tuple[bool, Any]) -> None:
         ret, image_frame = data
         if ret:
+            self.pl[idx] = generate_ascii_frame(image_frame, self.frame_size, self.ascii_chars_gradient)
+        self.done += 1
+        self.callback(self.done, self.frames_count)
+    
+    def get_acsii_frame(self, idx: int, data: Tuple[bool, Any]) -> None:
+        Thread(target=self._gaf, args=(idx, data)).start()
+
+class MultiprocessingFrameHandler:
+    def __init__(self, frames_count: int, frame_size: Tuple[int, int], callback=_callback) -> None:
+        self.frames_count = frames_count
+        self.frame_size = frame_size
+        self.pl = ProgressiveList(frames_count)
+        self.done = 1
+        self.callback = callback
+        
+    @staticmethod
+    def _gaf(connection: PipeConnection) -> None:
+        self: MultiprocessingFrameHandler = connection.recv()
+        idx: int = connection.recv()
+        data: Tuple[bool, Any] = connection.recv()
+        
+        ret, image_frame = data
+        if ret:
             ac = "".join([ASCII_CHARS_GRADIENTION[pixel] for pixel in Image.fromarray(image_frame).convert("L").resize(self.frame_size).getdata()])
             self.pl[idx] = "\n".join([ac[index:(index+self.frame_size[0])] for index in range(0, len(ac), self.frame_size[0])])
         self.done += 1
         self.callback(self.done, self.frames_count)
     
     def get_acsii_frame(self, idx: int, data: Tuple[bool, Any]) -> None:
-        Thread(target=self._gaf, args=(idx, data)).start()
+        send_conn, recv_conn = Pipe()
+        Process(target=self._gaf, args=(recv_conn,)).start()
+        send_conn.send(self)
+        send_conn.send(idx)
+        send_conn.send(data)
 
 # > Main Class
 class AVP:
-    def __init__(self, fp) -> None:
+    def __init__(self, fp, ascii_chars: List[str]=ASCII_CHARS) -> None:
+        self.ascii_chars_gradient = generate_ascii_chars_gradient(ascii_chars)
         if isinstance(fp, str):
             self.path = os.path.abspath(fp)
         elif isinstance(fp, bytes):
             with NamedTemporaryFile("wb", delete=False) as tempfile:
                 tempfile.write(fp)
                 self.path = os.path.abspath(tempfile.name)
                 TEMP_DETECTOR.append(self.path)
@@ -132,27 +177,26 @@
         capture.set(1, 1)
         frames_count = self.get_frames_count()
         
         for i in range(1, frames_count):
             callback(i, frames_count)
             ret, image_frame = capture.read()
             if ret:
-                ac = "".join([ASCII_CHARS_GRADIENTION[pixel] for pixel in Image.fromarray(image_frame).convert("L").resize(frame_size).getdata()])
-                al.append("\n".join([ac[index:(index+frame_size[0])] for index in range(0, len(ac), frame_size[0])]))
+                al.append(generate_ascii_frame(image_frame, frame_size, self.ascii_chars_gradient))
             else:
                 break
         capture.release()
         return al
     
     def get_ascii_frames_threading(self, frame_size, callback=_callback):
         capture = cv2.VideoCapture(self.path)
         capture.set(1, 1)
         frames_count = self.get_frames_count()
         
-        thfn = ThreadingFrameHandler(frames_count, frame_size, callback)
+        thfn = ThreadingFrameHandler(frames_count, frame_size, callback, self.ascii_chars_gradient)
         
         for i in range(1, frames_count):
             ret, image_frame = capture.read()
             thfn.get_acsii_frame(i, (ret, image_frame))
         
         while thfn.frames_count > thfn.done: time.sleep(0.01)
```

### Comparing `avplib-1.4.1/avplib/__main__.py` & `avplib-1.4.5/avplib/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 import click
 import avplib
 import pygame
 import fpstimer
 import time
-import zipfile
-import json
-from tempfile import NamedTemporaryFile
 from rich.console import Console
 from rich.progress import Progress
 from rich.live import Live
-from typing import Tuple, List, Dict, Any
+from typing import Tuple, List
 # > Local Imports
 from .avf import AVFile
+from .units import ASCII_CHARS
 
 # ! Set Environ
 os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = "hide"
 
 # ! Reinitialize
 class Console(Console):
     def set_size(self, size: Tuple[int, int]) -> None:
@@ -72,27 +70,45 @@
     help="Disable audio playback."
 )
 @click.option(
     "--yes", "-y",
     is_flag=True,
     help="Disable playback confirmation."
 )
-def cav(video_path: str, res: Tuple[int, int], fps: int, threading: bool, no_audio: bool, yes: bool):
+@click.option(
+    "--ascii_chars",
+    type=list,
+    default=ASCII_CHARS,
+    show_default=True,
+    help="ASCII Chars for to create gradation (256 <= ascii_chars)."
+)
+def cav(
+    video_path: str,
+    res: Tuple[int, int],
+    fps: int,
+    threading: bool,
+    no_audio: bool,
+    yes: bool,
+    ascii_chars: List[str]
+):
     if sum(res) > 0:
         console.set_size((res[0]+1, res[1]))
     else:
         res = (console.size.width-1, console.size.height)
+    
+    if len(ascii_chars) > 256: ascii_chars = ascii_chars[:256]
 
     console.print(f"[#EA00FF]*[/] [#BBFF00]Video Path[/]: '{os.path.abspath(video_path)}'")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Resolution[/]: {res[0]}x{res[1]}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]FPS[/]: {fps}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Enable Threading[/]: {threading}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Disable Audio[/]: {no_audio}")
+    console.print(f"[#EA00FF]*[/] [#BBFF00]ASCII Chars[/]: {ascii_chars}")
 
-    video = avplib.AVP(video_path)
+    video = avplib.AVP(video_path, ascii_chars)
     if (fps != 30) and (fps != video.get_fps()):
         video.set_fps(fps)
     if not no_audio:
         audio_path = video.get_audio("file")
 
     st = time.time()
     with Progress(transient=True) as pr:
@@ -154,59 +170,71 @@
     default=""
 )
 @click.option(
     "--no_audio", "-na",
     is_flag=True,
     help="Disable audio playback."
 )
+@click.option(
+    "--ascii_chars",
+    type=list,
+    default=ASCII_CHARS,
+    show_default=True,
+    help="ASCII Chars for to create gradation (256 <= ascii_chars)."
+)
 def convert2avf(
     from_video_path: str,
     to_video_path: str,
     res: Tuple[int, int],
     fps: int,
     threading: bool,
     auto_res: bool,
     title: str,
     author: str,
-    no_audio: bool
+    no_audio: bool,
+    ascii_chars: List[str]
 ):
     if auto_res:
         res = (console.size.width-1, console.size.height)
-
+    
+    if len(ascii_chars) > 256: ascii_chars = ascii_chars[:256]
+    
     console.print(f"[#EA00FF]*[/] [#BBFF00]From Video Path[/]: {os.path.abspath(from_video_path).__repr__()}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]To Video Path[/]: {os.path.abspath(to_video_path).__repr__()}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Resolution[/]: {res[0]}x{res[1]}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]FPS[/]: {fps}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Enable Threading[/]: {threading}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Disable Audio[/]: {no_audio}")
+    console.print(f"[#EA00FF]*[/] [#BBFF00]ASCII Chars[/]: {ascii_chars}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Title[/]: {title.__repr__()}")
-    console.print(f"[#EA00FF]*[/] [#BBFF00]Title[/]: {author.__repr__()}")
+    console.print(f"[#EA00FF]*[/] [#BBFF00]Author[/]: {author.__repr__()}")
     
     st = time.time()
     with Progress(transient=True) as pr:
         preparation = pr.add_task("Creating an archive", total=5)
         gaf = pr.add_task("Generation ASCII")
         
         def update_bar(complited: int, total: int): pr.update(gaf, total=total, completed=complited)
         
         # * Подготовка
         avfile = AVFile(to_video_path, "w")
         
         pr.update(preparation, advance=1, description="Preparation Video File")
-        video = avplib.AVP(from_video_path)
+        video = avplib.AVP(from_video_path, ascii_chars)
         if fps != video.get_fps():
             video.set_fps(fps)
         
         pr.update(preparation, advance=1, description="Writing info")
         avfile.set_info(
             title,
             author,
             fps,
             res,
-            not(no_audio)
+            not(no_audio),
+            ascii_chars
         )
         
         pr.update(preparation, advance=1, description="Compressing audio")
         if not no_audio: avfile.set_audio_from_path(video.get_audio("file"))
         
         # * Convert
         pr.update(preparation, advance=1, description="Compressing Video")
@@ -260,14 +288,15 @@
     console.print(f"\n[#EA00FF]*[/] [#BBFF00]ASCII Video File[/]: {os.path.abspath(ascii_video_path).__repr__()}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Resolution[/]: {info['res'][0]}x{info['res'][1]}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]FPS[/]: {info['fps']}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Title[/]: {info['title'].__repr__()}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Author[/]: {info['author'].__repr__()}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Exists Audio[/]: {info['exists_audio']}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Disable Audio[/]: {no_audio}")
+    console.print(f"[#EA00FF]*[/] [#BBFF00]ASCII Chars[/]: {info['ascii_chars']}")
     console.print(f"[#EA00FF]*[/] [#BBFF00]Total Time[/]: {round(et-st,2)} [yellow]sec[/]\n[red](ENTER to continue)[/]")
     
     if not yes: input()
     if (not no_audio) and (info["exists_audio"]): play_audio(audio_path)
     
     play_video(frames, info['fps'])
```

### Comparing `avplib-1.4.1/avplib.egg-info/PKG-INFO` & `avplib-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avplib
-Version: 1.4.1
+Version: 1.4.5
 Summary: AVP - ASCII Video Player. Allows you to play any video as ASCII-art.
 Home-page: https://github.com/romanin-rf/avplib
 Author: ProgrammerFromParlament
 Author-email: semina054@gmail.com
 License: MIT
 Keywords: avplib
 Platform: UNKNOWN
```

### Comparing `avplib-1.4.1/PKG-INFO` & `avplib-1.4.5/avplib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avplib
-Version: 1.4.1
+Version: 1.4.5
 Summary: AVP - ASCII Video Player. Allows you to play any video as ASCII-art.
 Home-page: https://github.com/romanin-rf/avplib
 Author: ProgrammerFromParlament
 Author-email: semina054@gmail.com
 License: MIT
 Keywords: avplib
 Platform: UNKNOWN
```

### Comparing `avplib-1.4.1/README.md` & `avplib-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `avplib-1.4.1/setup.py` & `avplib-1.4.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import setuptools
 
 # * This setup
 setuptools.setup(
 	name="avplib",
-	version="1.4.1",
+	version="1.4.5",
 	description='AVP - ASCII Video Player. Allows you to play any video as ASCII-art.',
 	keywords=["avplib"],
 	packages=setuptools.find_packages(),
 	author_email='semina054@gmail.com',
 	url="https://github.com/romanin-rf/avplib",
 	long_description=open(os.path.join(os.path.dirname(__file__), 'README.md')).read(),
 	long_description_content_type="text/markdown",
```

