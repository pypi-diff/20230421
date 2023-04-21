# Comparing `tmp/FastDub-3.5.2.tar.gz` & `tmp/FastDub-3.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastDub-3.5.2.tar", last modified: Sat Feb 18 08:38:09 2023, max compression
+gzip compressed data, was "FastDub-3.6.0b0.tar", last modified: Fri Apr 21 08:34:01 2023, max compression
```

## Comparing `FastDub-3.5.2.tar` & `FastDub-3.6.0b0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.426762 FastDub-3.5.2/
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.369765 FastDub-3.5.2/FastDub.egg-info/
--rw-rw-rw-   0        0        0    15969 2023-02-18 08:38:09.000000 FastDub-3.5.2/FastDub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-02-18 08:38:09.000000 FastDub-3.5.2/FastDub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 08:38:09.000000 FastDub-3.5.2/FastDub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      338 2023-02-18 08:38:09.000000 FastDub-3.5.2/FastDub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-18 08:38:09.000000 FastDub-3.5.2/FastDub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    15969 2023-02-18 08:38:09.426762 FastDub-3.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     9185 2023-02-18 05:43:34.000000 FastDub-3.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.374761 FastDub-3.5.2/fastdub/
--rw-rw-rw-   0        0        0      913 2023-02-18 08:16:05.000000 FastDub-3.5.2/fastdub/__init__.py
--rw-rw-rw-   0        0        0    12595 2023-02-18 08:36:25.000000 FastDub-3.5.2/fastdub/__main__.py
--rw-rw-rw-   0        0        0     3362 2023-02-15 09:05:44.000000 FastDub-3.5.2/fastdub/audio.py
--rw-rw-rw-   0        0        0     7026 2023-02-18 05:33:19.000000 FastDub-3.5.2/fastdub/dubber.py
--rw-rw-rw-   0        0        0     3482 2023-02-18 08:27:40.000000 FastDub-3.5.2/fastdub/ffmpeg_wrapper.py
--rw-rw-rw-   0        0        0     2950 2023-02-18 08:15:35.000000 FastDub-3.5.2/fastdub/subtitles.py
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.390763 FastDub-3.5.2/fastdub/translator/
--rw-rw-rw-   0        0        0      605 2023-02-18 08:33:17.000000 FastDub-3.5.2/fastdub/translator/__init__.py
--rw-rw-rw-   0        0        0     2005 2022-12-21 15:12:58.000000 FastDub-3.5.2/fastdub/translator/subs_translate.py
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.391763 FastDub-3.5.2/fastdub/utils/
--rw-rw-rw-   0        0        0       84 2022-09-01 08:47:25.000000 FastDub-3.5.2/fastdub/utils/__init__.py
--rw-rw-rw-   0        0        0      968 2023-01-29 05:38:56.000000 FastDub-3.5.2/fastdub/utils/json2srt.py
--rw-rw-rw-   0        0        0     2368 2022-12-04 07:09:03.000000 FastDub-3.5.2/fastdub/voicer.py
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.403764 FastDub-3.5.2/fastdub/youtube/
--rw-rw-rw-   0        0        0      402 2022-09-20 03:37:23.000000 FastDub-3.5.2/fastdub/youtube/__init__.py
--rw-rw-rw-   0        0        0     5885 2022-12-03 06:39:17.000000 FastDub-3.5.2/fastdub/youtube/downloader.py
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.409762 FastDub-3.5.2/fastdub/youtube/pafy/
--rw-rw-rw-   0        0        0      371 2022-09-01 07:44:54.000000 FastDub-3.5.2/fastdub/youtube/pafy/__init__.py
--rw-rw-rw-   0        0        0    16042 2022-09-01 09:43:55.000000 FastDub-3.5.2/fastdub/youtube/pafy/backend_internal.py
--rw-rw-rw-   0        0        0    23099 2022-09-01 09:43:55.000000 FastDub-3.5.2/fastdub/youtube/pafy/backend_shared.py
--rw-rw-rw-   0        0        0     7231 2022-09-17 14:51:28.000000 FastDub-3.5.2/fastdub/youtube/pafy/backend_youtube_dl.py
--rw-rw-rw-   0        0        0     7957 2022-09-01 09:31:44.000000 FastDub-3.5.2/fastdub/youtube/pafy/channel.py
--rw-rw-rw-   0        0        0     3880 2022-09-01 08:31:43.000000 FastDub-3.5.2/fastdub/youtube/pafy/g.py
--rw-rw-rw-   0        0        0    10071 2022-11-20 14:11:33.000000 FastDub-3.5.2/fastdub/youtube/pafy/jsinterp.py
--rw-rw-rw-   0        0        0     6229 2022-09-01 09:38:50.000000 FastDub-3.5.2/fastdub/youtube/pafy/pafy.py
--rw-rw-rw-   0        0        0    10668 2022-09-01 08:31:43.000000 FastDub-3.5.2/fastdub/youtube/pafy/playlist.py
--rw-rw-rw-   0        0        0     1404 2022-11-20 14:11:33.000000 FastDub-3.5.2/fastdub/youtube/pafy/util.py
--rw-rw-rw-   0        0        0     1953 2022-12-02 10:39:37.000000 FastDub-3.5.2/fastdub/youtube/subtitles.py
-drwxrwxrwx   0        0        0        0 2023-02-18 08:38:09.425765 FastDub-3.5.2/fastdub/youtube/yt_upload/
--rw-rw-rw-   0        0        0      210 2022-09-01 08:47:25.000000 FastDub-3.5.2/fastdub/youtube/yt_upload/__init__.py
--rw-rw-rw-   0        0        0     6664 2022-11-20 14:11:33.000000 FastDub-3.5.2/fastdub/youtube/yt_upload/upload_video.py
--rw-rw-rw-   0        0        0     1809 2022-09-17 15:00:26.000000 FastDub-3.5.2/fastdub/youtube/yt_upload/uploader.py
--rw-rw-rw-   0        0        0       42 2023-02-18 08:38:09.426762 FastDub-3.5.2/setup.cfg
--rw-rw-rw-   0        0        0     3151 2023-02-18 08:15:45.000000 FastDub-3.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.271207 FastDub-3.6.0b0/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.240239 FastDub-3.6.0b0/FastDub.egg-info/
+-rw-rw-rw-   0        0        0    16309 2023-04-21 08:34:00.000000 FastDub-3.6.0b0/FastDub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2023-04-21 08:34:01.000000 FastDub-3.6.0b0/FastDub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:34:00.000000 FastDub-3.6.0b0/FastDub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2023-04-21 08:34:01.000000 FastDub-3.6.0b0/FastDub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 08:34:01.000000 FastDub-3.6.0b0/FastDub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16309 2023-04-21 08:34:01.271207 FastDub-3.6.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     9185 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.248206 FastDub-3.6.0b0/fastdub/
+-rw-rw-rw-   0        0        0      913 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/__init__.py
+-rw-rw-rw-   0        0        0    12593 2023-04-20 09:52:10.000000 FastDub-3.6.0b0/fastdub/__main__.py
+-rw-rw-rw-   0        0        0     2779 2023-04-21 08:15:56.000000 FastDub-3.6.0b0/fastdub/audio.py
+-rw-rw-rw-   0        0        0     7022 2023-04-21 07:55:57.000000 FastDub-3.6.0b0/fastdub/dubber.py
+-rw-rw-rw-   0        0        0     4363 2023-04-21 08:02:10.000000 FastDub-3.6.0b0/fastdub/ffmpeg_wrapper.py
+-rw-rw-rw-   0        0        0     3038 2023-04-20 08:07:29.000000 FastDub-3.6.0b0/fastdub/subtitles.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.250208 FastDub-3.6.0b0/fastdub/translator/
+-rw-rw-rw-   0        0        0      605 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/translator/__init__.py
+-rw-rw-rw-   0        0        0     2005 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/translator/subs_translate.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.252207 FastDub-3.6.0b0/fastdub/utils/
+-rw-rw-rw-   0        0        0       84 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/utils/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/utils/json2srt.py
+-rw-rw-rw-   0        0        0     2644 2023-04-20 08:34:17.000000 FastDub-3.6.0b0/fastdub/voicer.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.255207 FastDub-3.6.0b0/fastdub/youtube/
+-rw-rw-rw-   0        0        0      402 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/__init__.py
+-rw-rw-rw-   0        0        0     5885 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/downloader.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.266207 FastDub-3.6.0b0/fastdub/youtube/pafy/
+-rw-rw-rw-   0        0        0      371 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/__init__.py
+-rw-rw-rw-   0        0        0    16042 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/backend_internal.py
+-rw-rw-rw-   0        0        0    23099 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/backend_shared.py
+-rw-rw-rw-   0        0        0     7231 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/backend_youtube_dl.py
+-rw-rw-rw-   0        0        0     7957 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/channel.py
+-rw-rw-rw-   0        0        0     3880 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/g.py
+-rw-rw-rw-   0        0        0    10071 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/jsinterp.py
+-rw-rw-rw-   0        0        0     6229 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/pafy.py
+-rw-rw-rw-   0        0        0    10668 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/playlist.py
+-rw-rw-rw-   0        0        0     1404 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/pafy/util.py
+-rw-rw-rw-   0        0        0     1953 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/subtitles.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:34:01.270208 FastDub-3.6.0b0/fastdub/youtube/yt_upload/
+-rw-rw-rw-   0        0        0      210 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/yt_upload/__init__.py
+-rw-rw-rw-   0        0        0     6664 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/yt_upload/upload_video.py
+-rw-rw-rw-   0        0        0     1809 2023-04-20 07:12:06.000000 FastDub-3.6.0b0/fastdub/youtube/yt_upload/uploader.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:34:01.271207 FastDub-3.6.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     3168 2023-04-21 08:24:35.000000 FastDub-3.6.0b0/setup.py
```

### Comparing `FastDub-3.5.2/FastDub.egg-info/PKG-INFO` & `FastDub-3.6.0b0/FastDub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: FastDub
-Version: 3.5.2
+Version: 3.6.0b0
 Summary: A Python CLI package for voice over subtitles, with the ability to embed in video, audio ducking, and dynamic voice changer for a single track; auto translating; download and upload to YouTube supports
-Home-page: UNKNOWN
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: Download Voices, https://rhvoice.su/voices
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/FastDub
 Project-URL: YouTube, https://www.youtube.com/channel/UC8JV3zPSVm9EKSWD1XdkQvw
 Keywords: dubbing,voicing,fastdub,JustDub,SpeedDub,offline,free,easiest,subtitles,videos,veed,fast
@@ -259,18 +258,32 @@
 
 ### The `fastdub.utils` module stores helper functions.
 
 ### python -m pydoc -w fastdub
 
 ### You can write your issues on [GitHub](https://github.com/NIKDISSV-Forever/fastdub/issues) in English or in Russian.
 
+---
 
 # CHANGELOG
 
----
+# 3.6.0
+
+## General
+
+- Bugfix
+
+## Audio Processing
+
+- sidechain теперь намного быстрее, используя FFMpeg
+
+## CLI
+
+- Аргумент `--sidechain-ffmpeg-params` см. [FFMpeg Documentation](https://ffmpeg.org/ffmpeg-all.html#sidechaincompress)
+- Отдельный `--sidechain-level-sc` см. `level_sc` выше.
 
 # 3.5.2
 
 ## Translator
 
 - Теперь не вызовет ошибки при отсутствии интернета.
```

### Comparing `FastDub-3.5.2/FastDub.egg-info/SOURCES.txt` & `FastDub-3.6.0b0/FastDub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/PKG-INFO` & `FastDub-3.6.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: FastDub
-Version: 3.5.2
+Version: 3.6.0b0
 Summary: A Python CLI package for voice over subtitles, with the ability to embed in video, audio ducking, and dynamic voice changer for a single track; auto translating; download and upload to YouTube supports
-Home-page: UNKNOWN
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: Download Voices, https://rhvoice.su/voices
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/FastDub
 Project-URL: YouTube, https://www.youtube.com/channel/UC8JV3zPSVm9EKSWD1XdkQvw
 Keywords: dubbing,voicing,fastdub,JustDub,SpeedDub,offline,free,easiest,subtitles,videos,veed,fast
@@ -259,18 +258,32 @@
 
 ### The `fastdub.utils` module stores helper functions.
 
 ### python -m pydoc -w fastdub
 
 ### You can write your issues on [GitHub](https://github.com/NIKDISSV-Forever/fastdub/issues) in English or in Russian.
 
+---
 
 # CHANGELOG
 
----
+# 3.6.0
+
+## General
+
+- Bugfix
+
+## Audio Processing
+
+- sidechain теперь намного быстрее, используя FFMpeg
+
+## CLI
+
+- Аргумент `--sidechain-ffmpeg-params` см. [FFMpeg Documentation](https://ffmpeg.org/ffmpeg-all.html#sidechaincompress)
+- Отдельный `--sidechain-level-sc` см. `level_sc` выше.
 
 # 3.5.2
 
 ## Translator
 
 - Теперь не вызовет ошибки при отсутствии интернета.
```

### Comparing `FastDub-3.5.2/README.md` & `FastDub-3.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/__init__.py` & `FastDub-3.6.0b0/fastdub/__init__.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/__main__.py` & `FastDub-3.6.0b0/fastdub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 import argparse
 from glob import iglob
-from math import inf
 from multiprocessing import cpu_count
 from os import getcwd
 from time import perf_counter
 
 import rich.traceback
 
 import fastdub.youtube
 from fastdub import GlobalSettings, PrettyViewPrefix, dubber, translator, voicer, youtube
 from fastdub.ffmpeg_wrapper import DefaultFFMpegParams
 from fastdub.translator.subs_translate import SrtTranslate
 
 __all__ = ('parse_args', 'main')
 
+ANY_EXTRAS_SUPPORTED = youtube.SUPPORTED or translator.SUPPORTED
+
 
 class BooleanOptionalAction(argparse.Action):
     __slots__ = ()
 
     def __init__(self, option_strings, dest, default=None, type=None,
                  choices=None, required=False, help=None, metavar=None):
         _option_strings = (*option_strings,
@@ -57,15 +58,15 @@
                                  '\t2 - Delete cache after voice acting (default)')
     arg_parser.add_argument('-ra', '--cleanup-audio', action=BooleanOptionalAction, default=True,
                             help='Remove result audio if video exists (default True)')
     arg_parser.add_argument('-ev', '--export-video', action=BooleanOptionalAction, default=True)
     arg_parser.add_argument('-l', '--language', default='ru',
                             help='Subtitles language (ru)')
 
-    if youtube.SUPPORTED or translator.SUPPORTED:
+    if ANY_EXTRAS_SUPPORTED:
         arg_parser.add_argument('-tc', '--threads-count', default=cpu_count(),
                                 type=_thread_count_type,
                                 help='Process count to download (pass to cpu count, < 2 to disable)\n'
                                      '\t*N = N * cpu count')
 
     input_group = arg_parser.add_argument_group('Input')
     input_group.add_argument('-i', '--input', default=getcwd(), required=True,
@@ -78,22 +79,20 @@
     exclude_input_group = arg_parser.add_argument_group('Input Exclude')
     exclude_input_group.add_argument('-En', '--exclude', type=iglob, nargs='+', default=(),
                                      help='Exclude <name> (glob)')
     exclude_input_group.add_argument('-Eu', '--exclude-underscore', default=True,
                                      help='Exclude files starts with underscore')
 
     ducking_group = arg_parser.add_argument_group('Audio Ducking')
-    ducking_group.add_argument('-sc', '--side-chain', action=BooleanOptionalAction, default=True,
+    ducking_group.add_argument('-sc', '--sidechain', action=BooleanOptionalAction, default=True,
                                help='Enable audio side chain compress (ducking)')
-    ducking_group.add_argument('-sc-msl', '--min-silence-len', '--attack', default=100, type=int,
-                               help='Minimum silence length in ms (default: 100)')
-    ducking_group.add_argument('-sc-st', '--silence-thresh', default=-inf, type=float,
-                               help='Silence threshold in dB')
-    ducking_group.add_argument('-sc-gdo', '--gain-during-overlay', default=-11, type=int,
-                               help='Gain during overlay in dB (default: -11)')
+    ducking_group.add_argument('-sc-args', '--sidechain-ffmpeg-params', default=DefaultFFMpegParams.sidechain_args,
+                               help=f'sidechain FFMpeg parameters (default {DefaultFFMpegParams.sidechain_args!r})')
+    ducking_group.add_argument('-sc-lvl', '--sidechain-level-sc', type=float, default=.8,
+                               help='Set sidechain gain. Range is between 0.015625 and 64. (default 0.8)')
 
     voicer_group = arg_parser.add_argument_group('Voicer')
     voicer_group.add_argument('-v', '--voice', type=str.lower, choices=voicer.VOICES_NAMES.keys(),
                               help='SAPI voice for voice acting.')
     voicer_group.add_argument('-a', '--align', default=2., type=float,
                               help='Audio fit align (divisor)'
                                    '\n\t1 = right'
@@ -178,15 +177,17 @@
     DefaultFFMpegParams.ffmpeg_log_level = args.loglevel
 
     total_time = 0
     if args.confirm:
         DefaultFFMpegParams.args += '-y',
         total_time = perf_counter()
 
-    GlobalSettings.threads_count = args.threads_count
+    if ANY_EXTRAS_SUPPORTED:
+        GlobalSettings.threads_count = args.threads_count
+
     if youtube.SUPPORTED and args.youtube:
         query: str = args.input
         if args.youtube_search and not query.startswith('?'):
             query = f'?{query.strip()}'
         youtube.downloader.DownloadYTVideo.API_KEYS |= {*args.api_keys}
         downloader = youtube.downloader.DownloadYTVideo(query,
                                                         args.language,
@@ -201,16 +202,17 @@
 
     videos = dubber.Dubber.collect_videos(args.input, args.exclude_underscore, (*sum(args.exclude, []),))
 
     translate_serv = args.translate_service if translator.SUPPORTED else None
     if translator.SUPPORTED and args.translate:
         SrtTranslate(args.language, translate_serv, args.rewrite_srt).translate_dir(videos, subtitles_format)
 
-    dubs = dubber.Dubber(args.voice, args.language, audio_format, args.side_chain, args.min_silence_len,
-                         args.silence_thresh, args.gain_during_overlay, args.align,
+    dubs = dubber.Dubber(args.voice, args.language, audio_format,
+                         args.sidechain, args.sidechain_level_sc, args.sidechain_ffmpeg_params,
+                         args.align,
                          args.cleanup_audio, args.export_video)
 
     dubs.dub_dir(videos, video_format, subtitles_format)
 
     if remove_cache == 2:
         voicer.Voicer().cleanup()
```

### Comparing `FastDub-3.5.2/fastdub/audio.py` & `FastDub-3.6.0b0/fastdub/audio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 
 import math
 import os.path
 from copy import copy
-from math import inf
 from tempfile import TemporaryDirectory
 
 import pydub.silence
-from tqdm import tqdm
 
 from fastdub.ffmpeg_wrapper import FFMpegWrapper
 
 __all__ = ('AudioSegment',
            'speed_change', 'calc_speed_change_ffmpeg_arg',
-           'fit', 'side_chain')
+           'fit')
 
 
 class AudioSegment(pydub.AudioSegment):
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -69,18 +67,7 @@
     if (audio_duration := audio.duration_ms) > (free := (left_border + need_duration + right_border)):
         audio = speed_change(audio, audio_duration / free)
         audio_duration = audio.duration_ms
     return AudioSegment.silent(
         (free - audio_duration) / align
         if audio_duration > need_duration + right_border
         else left_border) + audio
-
-
-def side_chain(sound1: AudioSegment, sound2: AudioSegment,
-               min_silence_len: int = 100, silence_thresh: float = -inf,
-               gain_during_overlay: int = -10
-               ) -> AudioSegment:
-    for start, end in tqdm(
-            pydub.silence.detect_nonsilent(sound2, min_silence_len=min_silence_len, silence_thresh=silence_thresh),
-            desc="Ducking"):
-        sound1 = sound1.overlay(sound2[start:end], start, times=1, gain_during_overlay=gain_during_overlay)
-    return sound1
```

### Comparing `FastDub-3.5.2/fastdub/dubber.py` & `FastDub-3.6.0b0/fastdub/dubber.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,44 @@
 from pathlib import Path
 from typing import Sequence
 
 import rich.align
 from tqdm import tqdm
 
 from fastdub import audio, subtitles, voicer
-from fastdub.audio import calc_speed_change_ffmpeg_arg
+from fastdub.audio import AudioSegment, calc_speed_change_ffmpeg_arg
 from fastdub.ffmpeg_wrapper import FFMpegWrapper
 
 __all__ = ('Dubber', 'VOICER')
 
+from fastdub.subtitles import Line, TimeLabel
+
 VOICER = voicer.Voicer()
 
 
 class Dubber:
     __slots__ = (
         'fit_align', 'language', 'audio_format',
         'cleanup_audio', 'export_video',
         'ducking',
-        'min_silence_len', 'silence_thresh', 'gain_during_overlay'
+        'sidechain_level_sc', 'sidechain_ffmpeg_params'
     )
 
     def __init__(self, voice: str, language: str, audio_format: str,
-                 ducking: bool, min_silence_len: int, silence_thresh: float, gain_during_overlay: int,
+                 ducking: bool, sidechain_level_sc: float, sidechain_ffmpeg_params: str,
                  fit_align: float = 2., cleanup_audio: bool = True, export_video: bool = True):
         self.language = language
         self.audio_format = audio_format
         self.fit_align = fit_align
         if voice:
             VOICER.set_voice(voice)
 
         self.ducking = ducking
-        self.min_silence_len = min_silence_len
-        self.silence_thresh = silence_thresh
-        self.gain_during_overlay = gain_during_overlay
+        self.sidechain_level_sc = sidechain_level_sc
+        self.sidechain_ffmpeg_params = sidechain_ffmpeg_params
 
         self.cleanup_audio = cleanup_audio
         self.export_video = export_video
 
     @staticmethod
     def collect_videos(path_to_files: str, skip_starts_underscore: bool = True,
                        exclude_files: Sequence[str] = frozenset()):
@@ -74,93 +75,90 @@
 
         rich.print(rich.align.Align(fn, 'center'))
         result_dir = Path(target_sub).parent / '_result'
         result_dir.mkdir(exist_ok=True)
         out_audio_base = result_dir / f'{fn}_{self.language}.{self.audio_format}'
 
         subs = subtitles.parse(target_sub)
-
         default_right_border = 0
         if target_vid and subs:
-            default_right_border = FFMpegWrapper.get_video_duration_ms(target_vid) - subs[-1].ms.end
-        default_right_border = max(default_right_border, 0)
+            default_right_border = FFMpegWrapper.get_video_duration_ms(target_vid)
+        default_right_border = max(default_right_border, end := subs[-1].ms.end)
+        subs += Line(TimeLabel(default_right_border, end, end - default_right_border)),
 
-        progress_total = len(subs)
+        progress_total = len(subs) - 1
 
-        total_duration_ms = 0
         fit_align = self.fit_align
         audio_format = self.audio_format
 
         working_dir = result_dir / '_working_dir'
         working_dir.mkdir(exist_ok=True)
 
-        _audio_filename_format = str(working_dir / ('{0:0>%i}.%s' % (len(str(progress_total)), audio_format))
-                                     ).format
-        filenames: tuple[str] = *(_audio_filename_format(pos) for pos in range(len(subs))),
-        for pos, line in tqdm(enumerate(subs[:-1]),
-                              desc='Creating audio',
-                              total=progress_total - 1, unit='line',
-                              dynamic_ncols=True):
-            ms = subs[pos].ms
-            tts = VOICER.voice(line.text)
+        filenames: tuple[str] = *map(
+            str(working_dir / ('{0:0>%i}.%s' % (len(str(progress_total)), audio_format))).format, range(len(subs))),
+
+        filename_sub = *zip(filenames_striped := filenames[:-1], subs[:-1]),
+        cached_tts = [VOICER.voice(line.text) for fn, line in tqdm(filename_sub,
+                                                                   desc='TTS',
+                                                                   total=progress_total, unit='line',
+                                                                   dynamic_ncols=True)]
+
+        total_duration_ms = 0
+        for pos, ((tts_fn, line), cached) in tqdm(
+                enumerate(zip(filename_sub, cached_tts), 1),
+                desc='Fitting',
+                total=progress_total, unit='line',
+                dynamic_ncols=True):
+            ms = line.ms
             new_audio = audio.fit(
-                tts,
+                AudioSegment.from_file(cached, 'wav'),
                 ms.start - total_duration_ms,
                 ms.duration,
-                subs[pos + 1].ms.start - ms.end,
+                subs[pos].ms.start - ms.end,
                 fit_align
             )
             total_duration_ms += new_audio.duration_ms
-            new_audio.export(filenames[pos], audio_format)
-        ms = subs[-1].ms
-        tts = VOICER.voice(subs[-1].text)
-        new_audio = audio.fit(tts,
-                              ms.start - total_duration_ms,
-                              ms.duration,
-                              default_right_border,
-                              fit_align)
-        total_duration_ms += new_audio.duration_ms
-        new_audio.export(filenames[-1], audio_format)
-
-        with open(list_file := os.path.join(working_dir, 'list.txt'), 'w') as f:
-            f.write('\n'.join(f"file '{fn}'" for fn in filenames))
-        max_duration = ms.end
+            new_audio.export(tts_fn, audio_format)
+        with open(list_file := working_dir / 'list.txt', 'w') as f:
+            f.writelines(f"file '{fn}'\n" for fn in filenames_striped)
+        max_duration = subs[-1].ms.end
 
         ffmpeg_concat_args = ()
         if total_duration_ms > max_duration:
             change_speed = total_duration_ms / max_duration
             rich.print(f'Changing audio speed to {change_speed:g}')
             ffmpeg_concat_args += '-af', calc_speed_change_ffmpeg_arg(change_speed)
         else:
             ffmpeg_concat_args += '-c', 'copy'
 
-        fitted_audio_file = str(out_audio_base.with_stem(f'_{out_audio_base.stem}'))
+        temp_audio_file = str(out_audio_base.with_stem(f'_{out_audio_base.stem}'))
         rich.print('Concatenating parts...', flush=True)
         FFMpegWrapper.convert('-f', 'concat', '-safe', '0', '-i', list_file, *ffmpeg_concat_args,
-                              fitted_audio_file)
-        cur_audio = audio.AudioSegment.from_file(fitted_audio_file)
+                              temp_audio_file)
+        cur_audio = audio.AudioSegment.from_file(temp_audio_file)
         shutil.rmtree(working_dir, ignore_errors=True)
 
         if total_duration_ms != max_duration:
             cur_audio = audio.AudioSegment.silent(
                 min(max_duration - total_duration_ms, subs[0].ms.start)
             ) + cur_audio
 
         result_out_audio = str(out_audio_base)
         if target_vid:
+            cur_audio.export(temp_audio_file, format='wav')
             if self.ducking:
-                audio.side_chain(audio.AudioSegment.from_file(target_vid),
-                                 cur_audio,
-                                 self.min_silence_len, self.silence_thresh, self.gain_during_overlay
-                                 ).export(result_out_audio)
+                FFMpegWrapper.sidechain(target_vid,
+                                        temp_audio_file,
+                                        result_out_audio,
+                                        self.sidechain_level_sc,
+                                        self.sidechain_ffmpeg_params)
             else:
-                audio.AudioSegment.from_file(target_vid).overlay(cur_audio,
-                                                                 gain_during_overlay=self.gain_during_overlay
-                                                                 ).export(result_out_audio)
+                FFMpegWrapper.amix(target_vid, temp_audio_file, out=result_out_audio)
+                # audio.AudioSegment.from_file(target_vid).overlay(cur_audio).export(result_out_audio)
             if export_video:
                 FFMpegWrapper.save_result_data(target_vid, result_out_audio, target_sub,
-                                               result_dir / f'{fn}_{self.language}.mp4')
+                                               result_dir / f'{fn}_{self.language}.mkv')
                 if cleanup_audio:
                     os.remove(result_out_audio)
         else:
             cur_audio.export(result_out_audio)
-        os.remove(fitted_audio_file)
+        os.remove(temp_audio_file)
```

### Comparing `FastDub-3.5.2/fastdub/ffmpeg_wrapper.py` & `FastDub-3.6.0b0/fastdub/ffmpeg_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 __all__ = ('FFMpegWrapper', 'DefaultFFMpegParams')
 
 
 class DefaultFFMpegParams:
     __slots__ = ()
     ffmpeg_log_level = 'panic'
     args = ()
+    sidechain_args = ''
     executable = get_ffmpeg_exe()
 
 
 def _ignore():
     pass
 
 
@@ -49,18 +50,19 @@
 
 
 class FFMpegWrapper:
     __slots__ = ()
     DURATION_RE = re.compile(r'Duration: (\d\d):(\d\d):(\d\d\.\d\d)')
 
     @classmethod
-    def convert(cls, *args, loglevel=None):
+    def convert(cls, *args, loglevel=None) -> int:
         if not loglevel:
             loglevel = DefaultFFMpegParams.ffmpeg_log_level
-        check_call([str(i) for i in (DefaultFFMpegParams.executable, '-v', loglevel, *DefaultFFMpegParams.args, *args)])
+        return check_call(
+            [str(i) for i in (DefaultFFMpegParams.executable, '-v', loglevel, *DefaultFFMpegParams.args, *args)])
 
     @classmethod
     def get_video_duration_ms(cls, video_path: str | Path) -> float:
         return cls.get_video_duration_s(video_path) * 1000.
 
     @classmethod
     def get_video_duration_s(cls, video_path: str | Path) -> float:
@@ -81,19 +83,37 @@
         if (subtitles_path := subtitles_path.with_stem(f'_{subtitles_path.stem}')).is_file():
             inputs += '-i', subtitles_path
             maps += '-map', '3:0'
         if GlobalSettings.watermark:
             watermark_args = cls.get_watermark_vf(GlobalSettings.watermark)
             copy_codec = '-c:a'
 
-        FFMpegWrapper.convert(
+        return cls.convert(
             *inputs, *maps,
             '-disposition:a:0', 'default', '-disposition:a:1', '0',
-            *watermark_args, copy_codec, 'copy', '-c:s', 'mov_text',
+            *watermark_args, copy_codec, 'copy',
             output_path)
 
     @classmethod
     def get_watermark_vf(cls, text: str) -> tuple[str, str]:
         return ('-vf',
                 f"drawtext=text='{text}'{_get_default_font_args()}"
                 ":fontcolor=white@0.5:box=1:boxcolor=black@0.5"
                 ":x='mod(n,w-text_w)':y='mod(n,h-text_h)'")
+
+    @classmethod
+    def sidechain(cls, background: str, foreground: str, out: str,
+                  level_sc: float = 0.8, params: str = None):
+        if params is None:
+            params = DefaultFFMpegParams.sidechain_args
+        return cls.convert('-i', background, '-i', foreground,
+                           '-filter_complex',
+                           '[1:a]asplit=2[sc][mix];'
+                           f'[0:a][sc]sidechaincompress=level_sc={level_sc}:{params}[compr];'
+                           '[compr][mix]amix',
+                           out)
+
+    @classmethod
+    def amix(cls, *inputs: str, out: str):
+        inputs_count = len(inputs)
+        return cls.convert(*sum(zip(('-i',) * inputs_count, inputs), ()), '-filter_complex',
+                           f'amix=inputs={len(inputs)}:duration=longest', out)
```

### Comparing `FastDub-3.5.2/fastdub/subtitles.py` & `FastDub-3.6.0b0/fastdub/subtitles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import datetime
 import os.path
 import re
+from typing import NamedTuple
 
 from chardet import detect as detect_encoding
 
 from fastdub.ffmpeg_wrapper import FFMpegWrapper
 
 __all__ = ('LINE_REGEX',
-           'Line',
+           'Line', 'TimeLabel',
            'parse', 'unparse',
            'ms_to_srt_time')
 
 LINE_REGEX = re.compile(r'\n\n^\d+$\n', re.M)
 
 
 def _read_file(filename) -> str:
@@ -25,35 +26,40 @@
 def ms_to_srt_time(ms: int) -> str:
     s, ms = divmod(ms, 1000)
     m, s = divmod(s, 60)
     h, m = divmod(m, 60)
     return f'{h:0>2}:{m:0>2}:{s:0>2},{ms:0>3}'
 
 
-class TimeLabel:
-    __slots__ = ('start', 'duration', 'end', 'time_str')
-
-    def __init__(self, start: int, end: int):
-        self.duration = end - start
-        self.start = start
-        self.end = end
-        self.time_str = f'{start} --> {end}'
+class TimeLabel(NamedTuple):
+    start: int
+    end: int
+    duration: int
 
     def __str__(self):
-        return (f"{ms_to_srt_time(self.start)}"
-                " --> "
-                f"{ms_to_srt_time(self.end)}")
+        return (f'{ms_to_srt_time(self.start)}'
+                ' --> '
+                f'{ms_to_srt_time(self.end)}')
 
 
 class Line:
     __slots__ = ('ms', 'text')
+    ms: TimeLabel
+    text: str
 
-    def __init__(self, time_labels: tuple[datetime.time], text: str):
-        self.ms: TimeLabel = TimeLabel(self._calc_ms_label(time_labels[0]), self._calc_ms_label(time_labels[-1]))
+    def __init__(self, time_labels: tuple[datetime.time] | TimeLabel, text: str = ''):
         self.text = text
+        if isinstance(time_labels, TimeLabel):
+            self.ms = time_labels
+            return
+
+        self.ms: TimeLabel = TimeLabel(
+            start := self._calc_ms_label(time_labels[0]),
+            end := self._calc_ms_label(time_labels[-1]),
+            end - start)
 
     @staticmethod
     def _calc_ms_label(label: datetime.time) -> int:
         return int(label.hour * 3600000
                    + label.minute * 60000
                    + label.second * 1000
                    + label.microsecond / 1000)
```

### Comparing `FastDub-3.5.2/fastdub/translator/__init__.py` & `FastDub-3.6.0b0/fastdub/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/translator/subs_translate.py` & `FastDub-3.6.0b0/fastdub/translator/subs_translate.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/utils/json2srt.py` & `FastDub-3.6.0b0/fastdub/utils/json2srt.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/voicer.py` & `FastDub-3.6.0b0/fastdub/voicer.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,51 +18,61 @@
 
 _voices = pyttsx3.init().proxy.getProperty('voices')
 VOICES_NAMES = {i.name.casefold(): i for i in _voices}
 VOICES_ID = {i.id: i for i in _voices}
 del _voices
 
 
+def _no_update_voice_anchor(_):
+    return False
+
+
 class Voicer:
-    __slots__ = ('engine', 'cache_dir', '_update_voice_anchor')
+    __slots__ = ('engine', 'cache_dir', '_update_voice_anchor', '_nul_file')
 
-    def __init__(self, cache_dir: str = None, anchor: str = '!:'):
+    def __init__(self, cache_dir: str = None, anchor: str = '!:', tts_driver_name: str = None, tts_debug: bool = False):
         if anchor:
             def _update_voice_anchor(line: str) -> bool:
                 if line.startswith(anchor):
                     self.set_voice(line.removeprefix(anchor))
                     return True
                 return False
         else:
-            def _update_voice_anchor(_: str) -> bool:
-                return False
+            _update_voice_anchor = _no_update_voice_anchor
         self._update_voice_anchor = _update_voice_anchor
-        self.cache_dir = Path(__file__).parent / '_cached_texts' if cache_dir is None else Path(cache_dir)
-        self.engine = pyttsx3.init()
-        self.cache_dir.mkdir(parents=True, exist_ok=True)
+
+        cache_dir = Path(__file__).parent / '_cached_texts' if cache_dir is None else Path(cache_dir)
+        cache_dir.mkdir(parents=True, exist_ok=True)
+        nul_file = cache_dir / 'nul.wav'
+        if not nul_file.is_file():
+            AudioSegment.silent(0).export(nul_file, 'wav')
+        self.cache_dir = cache_dir
+        self._nul_file = str(nul_file)
+
+        self.engine = pyttsx3.init(tts_driver_name, tts_debug)
 
     def cleanup(self):
         rmtree(self.cache_dir)
 
     def set_voice(self, voice: str):
         voice_name = voice.casefold()
         voice_property = self.engine.proxy.getProperty('voice')
         voice = VOICES_NAMES.get(voice_name)
         if not voice:
             raise UnknownVoice(f'{voice_name} not in {str(tuple(VOICES_NAMES.keys()))}')
         if VOICES_ID.get(voice_property).name.casefold() != voice_name:
             self.engine.proxy.setProperty('voice', voice.id)
 
-    def voice(self, text: str) -> AudioSegment:
+    def voice(self, text: str) -> str:
         text = text.strip()
         if not text:
-            return AudioSegment.silent(0)
+            return self._nul_file
 
         if self._update_voice_anchor((lines := text.splitlines())[0]):
             text = '\n'.join(lines[1:])
 
         cached_file = f'''{self.cache_dir / md5(f"{text}{self.engine.proxy.getProperty('voice')}".encode())
         .hexdigest()}.wav'''
         if not isfile(cached_file):
             self.engine.save_to_file(text, cached_file, 'fastdub')
             self.engine.runAndWait()
-        return AudioSegment.from_file(cached_file, format='wav')
+        return cached_file
```

### Comparing `FastDub-3.5.2/fastdub/youtube/downloader.py` & `FastDub-3.6.0b0/fastdub/youtube/downloader.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/backend_internal.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/backend_internal.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/backend_shared.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/backend_shared.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/backend_youtube_dl.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/backend_youtube_dl.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/channel.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/channel.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/g.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/g.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/jsinterp.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/jsinterp.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/pafy.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/pafy.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/playlist.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/playlist.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/pafy/util.py` & `FastDub-3.6.0b0/fastdub/youtube/pafy/util.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/subtitles.py` & `FastDub-3.6.0b0/fastdub/youtube/subtitles.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/yt_upload/upload_video.py` & `FastDub-3.6.0b0/fastdub/youtube/yt_upload/upload_video.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/fastdub/youtube/yt_upload/uploader.py` & `FastDub-3.6.0b0/fastdub/youtube/yt_upload/uploader.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.5.2/setup.py` & `FastDub-3.6.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import setuptools
 
 with open('requires.txt', encoding='utf-8') as f:
     requires = f.read().strip().splitlines()
 with open('CHANGELOG.md', encoding='utf-8') as f:
     changelog = f.read()
 with open('README.md', encoding='utf-8') as f:
-    readme = f.read()
-readme += f'\n\n# CHANGELOG\n\n{changelog}'
+    readme = f.read().strip()
+readme += f'\n\n---\n\n# CHANGELOG\n\n{changelog}'
 
 extras_require = {}
 for require in Path('extra_requires').glob('*_*.txt'):
     with open(require, encoding='UTF-8') as f:
         extras_require[require.name.split('.', 1)[0].rsplit('_', 1)[-1].casefold()] = f.read().strip().splitlines()
 extras_require['all'] = sum(extras_require.values(), requires)
 
 setuptools.setup(
     name="FastDub",
-    version="3.5.2",
+    version="3.6.0b0",
 
     description="A Python CLI package "
                 "for voice over subtitles, with the ability to embed in video, audio ducking, "
                 "and dynamic voice changer for a single track; "
                 "auto translating; "
                 "download and upload to YouTube supports",
```

