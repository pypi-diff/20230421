# Comparing `tmp/FastDub-3.6.0b1.tar.gz` & `tmp/FastDub-3.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastDub-3.6.0b1.tar", last modified: Fri Apr 21 08:36:23 2023, max compression
+gzip compressed data, was "FastDub-3.6.0b2.tar", last modified: Fri Apr 21 08:37:35 2023, max compression
```

## Comparing `FastDub-3.6.0b1.tar` & `FastDub-3.6.0b2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.564911 FastDub-3.6.0b1/
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.518911 FastDub-3.6.0b1/FastDub.egg-info/
--rw-rw-rw-   0        0        0    17643 2023-04-21 08:36:23.000000 FastDub-3.6.0b1/FastDub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-04-21 08:36:23.000000 FastDub-3.6.0b1/FastDub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 08:36:23.000000 FastDub-3.6.0b1/FastDub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      338 2023-04-21 08:36:23.000000 FastDub-3.6.0b1/FastDub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 08:36:23.000000 FastDub-3.6.0b1/FastDub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17643 2023-04-21 08:36:23.564911 FastDub-3.6.0b1/PKG-INFO
--rw-rw-rw-   0        0        0    10519 2023-04-21 08:36:11.000000 FastDub-3.6.0b1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.525911 FastDub-3.6.0b1/fastdub/
--rw-rw-rw-   0        0        0      913 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/__init__.py
--rw-rw-rw-   0        0        0    12593 2023-04-20 09:52:10.000000 FastDub-3.6.0b1/fastdub/__main__.py
--rw-rw-rw-   0        0        0     2779 2023-04-21 08:15:56.000000 FastDub-3.6.0b1/fastdub/audio.py
--rw-rw-rw-   0        0        0     7022 2023-04-21 07:55:57.000000 FastDub-3.6.0b1/fastdub/dubber.py
--rw-rw-rw-   0        0        0     4363 2023-04-21 08:02:10.000000 FastDub-3.6.0b1/fastdub/ffmpeg_wrapper.py
--rw-rw-rw-   0        0        0     3038 2023-04-20 08:07:29.000000 FastDub-3.6.0b1/fastdub/subtitles.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.527911 FastDub-3.6.0b1/fastdub/translator/
--rw-rw-rw-   0        0        0      605 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/translator/__init__.py
--rw-rw-rw-   0        0        0     2005 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/translator/subs_translate.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.529911 FastDub-3.6.0b1/fastdub/utils/
--rw-rw-rw-   0        0        0       84 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/utils/__init__.py
--rw-rw-rw-   0        0        0      968 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/utils/json2srt.py
--rw-rw-rw-   0        0        0     2644 2023-04-20 08:34:17.000000 FastDub-3.6.0b1/fastdub/voicer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.531911 FastDub-3.6.0b1/fastdub/youtube/
--rw-rw-rw-   0        0        0      402 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/__init__.py
--rw-rw-rw-   0        0        0     5885 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/downloader.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.541911 FastDub-3.6.0b1/fastdub/youtube/pafy/
--rw-rw-rw-   0        0        0      371 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/__init__.py
--rw-rw-rw-   0        0        0    16042 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/backend_internal.py
--rw-rw-rw-   0        0        0    23099 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/backend_shared.py
--rw-rw-rw-   0        0        0     7231 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/backend_youtube_dl.py
--rw-rw-rw-   0        0        0     7957 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/channel.py
--rw-rw-rw-   0        0        0     3880 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/g.py
--rw-rw-rw-   0        0        0    10071 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/jsinterp.py
--rw-rw-rw-   0        0        0     6229 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/pafy.py
--rw-rw-rw-   0        0        0    10668 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/playlist.py
--rw-rw-rw-   0        0        0     1404 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/pafy/util.py
--rw-rw-rw-   0        0        0     1953 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/subtitles.py
-drwxrwxrwx   0        0        0        0 2023-04-21 08:36:23.562910 FastDub-3.6.0b1/fastdub/youtube/yt_upload/
--rw-rw-rw-   0        0        0      210 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/yt_upload/__init__.py
--rw-rw-rw-   0        0        0     6664 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/yt_upload/upload_video.py
--rw-rw-rw-   0        0        0     1809 2023-04-20 07:12:06.000000 FastDub-3.6.0b1/fastdub/youtube/yt_upload/uploader.py
--rw-rw-rw-   0        0        0       42 2023-04-21 08:36:23.564911 FastDub-3.6.0b1/setup.cfg
--rw-rw-rw-   0        0        0     3168 2023-04-21 08:34:59.000000 FastDub-3.6.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.920640 FastDub-3.6.0b2/
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.894640 FastDub-3.6.0b2/FastDub.egg-info/
+-rw-rw-rw-   0        0        0    17643 2023-04-21 08:37:35.000000 FastDub-3.6.0b2/FastDub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2023-04-21 08:37:35.000000 FastDub-3.6.0b2/FastDub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 08:37:35.000000 FastDub-3.6.0b2/FastDub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2023-04-21 08:37:35.000000 FastDub-3.6.0b2/FastDub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-21 08:37:35.000000 FastDub-3.6.0b2/FastDub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17643 2023-04-21 08:37:35.920640 FastDub-3.6.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0    10519 2023-04-21 08:36:11.000000 FastDub-3.6.0b2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.901640 FastDub-3.6.0b2/fastdub/
+-rw-rw-rw-   0        0        0      913 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/__init__.py
+-rw-rw-rw-   0        0        0    12593 2023-04-20 09:52:10.000000 FastDub-3.6.0b2/fastdub/__main__.py
+-rw-rw-rw-   0        0        0     2779 2023-04-21 08:15:56.000000 FastDub-3.6.0b2/fastdub/audio.py
+-rw-rw-rw-   0        0        0     7022 2023-04-21 07:55:57.000000 FastDub-3.6.0b2/fastdub/dubber.py
+-rw-rw-rw-   0        0        0     4363 2023-04-21 08:02:10.000000 FastDub-3.6.0b2/fastdub/ffmpeg_wrapper.py
+-rw-rw-rw-   0        0        0     3038 2023-04-20 08:07:29.000000 FastDub-3.6.0b2/fastdub/subtitles.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.903639 FastDub-3.6.0b2/fastdub/translator/
+-rw-rw-rw-   0        0        0      605 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/translator/__init__.py
+-rw-rw-rw-   0        0        0     2005 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/translator/subs_translate.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.904639 FastDub-3.6.0b2/fastdub/utils/
+-rw-rw-rw-   0        0        0       84 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/utils/__init__.py
+-rw-rw-rw-   0        0        0      968 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/utils/json2srt.py
+-rw-rw-rw-   0        0        0     2644 2023-04-20 08:34:17.000000 FastDub-3.6.0b2/fastdub/voicer.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.907640 FastDub-3.6.0b2/fastdub/youtube/
+-rw-rw-rw-   0        0        0      402 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/__init__.py
+-rw-rw-rw-   0        0        0     5885 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/downloader.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.916639 FastDub-3.6.0b2/fastdub/youtube/pafy/
+-rw-rw-rw-   0        0        0      371 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/__init__.py
+-rw-rw-rw-   0        0        0    16042 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/backend_internal.py
+-rw-rw-rw-   0        0        0    23099 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/backend_shared.py
+-rw-rw-rw-   0        0        0     7231 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/backend_youtube_dl.py
+-rw-rw-rw-   0        0        0     7957 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/channel.py
+-rw-rw-rw-   0        0        0     3880 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/g.py
+-rw-rw-rw-   0        0        0    10071 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/jsinterp.py
+-rw-rw-rw-   0        0        0     6229 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/pafy.py
+-rw-rw-rw-   0        0        0    10668 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/playlist.py
+-rw-rw-rw-   0        0        0     1404 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/pafy/util.py
+-rw-rw-rw-   0        0        0     1953 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/subtitles.py
+drwxrwxrwx   0        0        0        0 2023-04-21 08:37:35.919639 FastDub-3.6.0b2/fastdub/youtube/yt_upload/
+-rw-rw-rw-   0        0        0      210 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/yt_upload/__init__.py
+-rw-rw-rw-   0        0        0     6664 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/yt_upload/upload_video.py
+-rw-rw-rw-   0        0        0     1809 2023-04-20 07:12:06.000000 FastDub-3.6.0b2/fastdub/youtube/yt_upload/uploader.py
+-rw-rw-rw-   0        0        0       42 2023-04-21 08:37:35.920640 FastDub-3.6.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     3168 2023-04-21 08:37:14.000000 FastDub-3.6.0b2/setup.py
```

### Comparing `FastDub-3.6.0b1/FastDub.egg-info/PKG-INFO` & `FastDub-3.6.0b2/FastDub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastDub
-Version: 3.6.0b1
+Version: 3.6.0b2
 Summary: A Python CLI package for voice over subtitles, with the ability to embed in video, audio ducking, and dynamic voice changer for a single track; auto translating; download and upload to YouTube supports
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: Download Voices, https://rhvoice.su/voices
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/FastDub
 Project-URL: YouTube, https://www.youtube.com/channel/UC8JV3zPSVm9EKSWD1XdkQvw
```

### Comparing `FastDub-3.6.0b1/FastDub.egg-info/SOURCES.txt` & `FastDub-3.6.0b2/FastDub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/PKG-INFO` & `FastDub-3.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastDub
-Version: 3.6.0b1
+Version: 3.6.0b2
 Summary: A Python CLI package for voice over subtitles, with the ability to embed in video, audio ducking, and dynamic voice changer for a single track; auto translating; download and upload to YouTube supports
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 License: MIT
 Project-URL: Download Voices, https://rhvoice.su/voices
 Project-URL: GitHub, https://github.com/NIKDISSV-Forever/FastDub
 Project-URL: YouTube, https://www.youtube.com/channel/UC8JV3zPSVm9EKSWD1XdkQvw
```

### Comparing `FastDub-3.6.0b1/README.md` & `FastDub-3.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/__init__.py` & `FastDub-3.6.0b2/fastdub/__init__.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/__main__.py` & `FastDub-3.6.0b2/fastdub/__main__.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/audio.py` & `FastDub-3.6.0b2/fastdub/audio.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/dubber.py` & `FastDub-3.6.0b2/fastdub/dubber.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/ffmpeg_wrapper.py` & `FastDub-3.6.0b2/fastdub/ffmpeg_wrapper.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/subtitles.py` & `FastDub-3.6.0b2/fastdub/subtitles.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/translator/__init__.py` & `FastDub-3.6.0b2/fastdub/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/translator/subs_translate.py` & `FastDub-3.6.0b2/fastdub/translator/subs_translate.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/utils/json2srt.py` & `FastDub-3.6.0b2/fastdub/utils/json2srt.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/voicer.py` & `FastDub-3.6.0b2/fastdub/voicer.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/downloader.py` & `FastDub-3.6.0b2/fastdub/youtube/downloader.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/backend_internal.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/backend_internal.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/backend_shared.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/backend_shared.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/backend_youtube_dl.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/backend_youtube_dl.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/channel.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/channel.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/g.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/g.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/jsinterp.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/jsinterp.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/pafy.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/pafy.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/playlist.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/playlist.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/pafy/util.py` & `FastDub-3.6.0b2/fastdub/youtube/pafy/util.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/subtitles.py` & `FastDub-3.6.0b2/fastdub/youtube/subtitles.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/yt_upload/upload_video.py` & `FastDub-3.6.0b2/fastdub/youtube/yt_upload/upload_video.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/fastdub/youtube/yt_upload/uploader.py` & `FastDub-3.6.0b2/fastdub/youtube/yt_upload/uploader.py`

 * *Files identical despite different names*

### Comparing `FastDub-3.6.0b1/setup.py` & `FastDub-3.6.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 for require in Path('extra_requires').glob('*_*.txt'):
     with open(require, encoding='UTF-8') as f:
         extras_require[require.name.split('.', 1)[0].rsplit('_', 1)[-1].casefold()] = f.read().strip().splitlines()
 extras_require['all'] = sum(extras_require.values(), requires)
 
 setuptools.setup(
     name="FastDub",
-    version="3.6.0b1",
+    version="3.6.0b2",
 
     description="A Python CLI package "
                 "for voice over subtitles, with the ability to embed in video, audio ducking, "
                 "and dynamic voice changer for a single track; "
                 "auto translating; "
                 "download and upload to YouTube supports",
```

