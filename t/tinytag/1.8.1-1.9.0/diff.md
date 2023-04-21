# Comparing `tmp/tinytag-1.8.1.tar.gz` & `tmp/tinytag-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinytag-1.8.1.tar", last modified: Sat Mar 12 17:50:45 2022, max compression
+gzip compressed data, was "tinytag-1.9.0.tar", last modified: Fri Apr 21 11:04:10 2023, max compression
```

## Comparing `tinytag-1.8.1.tar` & `tinytag-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-03-12 17:50:45.154016 tinytag-1.8.1/
--rw-r--r--   0 tom       (1000) users      (100)     1075 2018-02-10 18:18:45.000000 tinytag-1.8.1/LICENSE
--rw-r--r--   0 tom       (1000) users      (100)      130 2019-04-13 13:12:24.000000 tinytag-1.8.1/MANIFEST.in
--rw-r--r--   0 tom       (1000) users      (100)     9116 2022-03-12 17:50:45.154016 tinytag-1.8.1/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (100)     7940 2022-03-12 17:47:32.000000 tinytag-1.8.1/README.md
--rw-r--r--   0 tom       (1000) users      (100)     1748 2022-03-12 17:50:45.154016 tinytag-1.8.1/setup.cfg
--rwxr-xr-x   0 tom       (1000) users      (100)      396 2022-03-12 15:44:41.000000 tinytag-1.8.1/setup.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-03-12 17:50:45.154016 tinytag-1.8.1/tinytag/
--rw-r--r--   0 tom       (1000) users      (100)      171 2022-03-12 17:48:01.000000 tinytag-1.8.1/tinytag/__init__.py
--rwxr-xr-x   0 tom       (1000) users      (100)     2833 2022-03-12 15:44:41.000000 tinytag-1.8.1/tinytag/__main__.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-03-12 17:50:45.154016 tinytag-1.8.1/tinytag/tests/
--rw-r--r--   0 tom       (1000) users      (100)        0 2018-02-10 18:18:45.000000 tinytag-1.8.1/tinytag/tests/__init__.py
--rw-r--r--   0 tom       (1000) users      (100)      846 2022-03-04 16:28:54.000000 tinytag-1.8.1/tinytag/tests/__test_getid3.py
--rw-r--r--   0 tom       (1000) users      (100)    34912 2022-03-12 17:10:16.000000 tinytag-1.8.1/tinytag/tests/test_all.py
--rw-r--r--   0 tom       (1000) users      (100)     4190 2022-03-12 15:44:41.000000 tinytag-1.8.1/tinytag/tests/test_cli.py
--rw-r--r--   0 tom       (1000) users      (100)    65853 2022-03-12 17:49:16.000000 tinytag-1.8.1/tinytag/tinytag.py
-drwxr-xr-x   0 tom       (1000) users      (100)        0 2022-03-12 17:50:45.154016 tinytag-1.8.1/tinytag.egg-info/
--rw-r--r--   0 tom       (1000) users      (100)     9116 2022-03-12 17:50:45.000000 tinytag-1.8.1/tinytag.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (100)      404 2022-03-12 17:50:45.000000 tinytag-1.8.1/tinytag.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) users      (100)        1 2022-03-12 17:50:45.000000 tinytag-1.8.1/tinytag.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) users      (100)       20 2022-03-12 17:50:45.000000 tinytag-1.8.1/tinytag.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1000) users      (100)       34 2022-03-12 17:50:45.000000 tinytag-1.8.1/tinytag.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) users      (100)        8 2022-03-12 17:50:45.000000 tinytag-1.8.1/tinytag.egg-info/top_level.txt
+drwxr-xr-x   0 tom       (1000) users      (100)        0 2023-04-21 11:04:10.857250 tinytag-1.9.0/
+-rw-r--r--   0 tom       (1000) users      (100)     1075 2018-02-10 18:18:45.000000 tinytag-1.9.0/LICENSE
+-rw-r--r--   0 tom       (1000) users      (100)      130 2019-04-13 13:12:24.000000 tinytag-1.9.0/MANIFEST.in
+-rw-r--r--   0 tom       (1000) users      (100)     9986 2023-04-21 11:04:10.857250 tinytag-1.9.0/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (100)     8810 2023-04-21 11:00:35.000000 tinytag-1.9.0/README.md
+-rw-r--r--   0 tom       (1000) users      (100)     1721 2023-04-21 11:04:10.857250 tinytag-1.9.0/setup.cfg
+-rwxr-xr-x   0 tom       (1000) users      (100)      396 2022-03-12 15:44:41.000000 tinytag-1.9.0/setup.py
+drwxr-xr-x   0 tom       (1000) users      (100)        0 2023-04-21 11:04:10.857250 tinytag-1.9.0/tinytag/
+-rw-r--r--   0 tom       (1000) users      (100)      225 2023-04-21 11:02:56.000000 tinytag-1.9.0/tinytag/__init__.py
+-rwxr-xr-x   0 tom       (1000) users      (100)     2833 2022-03-12 15:44:41.000000 tinytag-1.9.0/tinytag/__main__.py
+drwxr-xr-x   0 tom       (1000) users      (100)        0 2023-04-21 11:04:10.857250 tinytag-1.9.0/tinytag/tests/
+-rw-r--r--   0 tom       (1000) users      (100)        0 2018-02-10 18:18:45.000000 tinytag-1.9.0/tinytag/tests/__init__.py
+-rw-r--r--   0 tom       (1000) users      (100)      846 2022-03-04 16:28:54.000000 tinytag-1.9.0/tinytag/tests/__test_getid3.py
+-rw-r--r--   0 tom       (1000) users      (100)    37411 2023-04-21 10:54:52.000000 tinytag-1.9.0/tinytag/tests/test_all.py
+-rw-r--r--   0 tom       (1000) users      (100)     4227 2023-04-21 10:54:52.000000 tinytag-1.9.0/tinytag/tests/test_cli.py
+-rw-r--r--   0 tom       (1000) users      (100)    67069 2023-04-21 10:54:52.000000 tinytag-1.9.0/tinytag/tinytag.py
+drwxr-xr-x   0 tom       (1000) users      (100)        0 2023-04-21 11:04:10.857250 tinytag-1.9.0/tinytag.egg-info/
+-rw-r--r--   0 tom       (1000) users      (100)     9986 2023-04-21 11:04:10.000000 tinytag-1.9.0/tinytag.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (100)      404 2023-04-21 11:04:10.000000 tinytag-1.9.0/tinytag.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) users      (100)        1 2023-04-21 11:04:10.000000 tinytag-1.9.0/tinytag.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) users      (100)       20 2023-04-21 11:04:10.000000 tinytag-1.9.0/tinytag.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1000) users      (100)       34 2023-04-21 11:04:10.000000 tinytag-1.9.0/tinytag.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) users      (100)        8 2023-04-21 11:04:10.000000 tinytag-1.9.0/tinytag.egg-info/top_level.txt
```

### Comparing `tinytag-1.8.1/LICENSE` & `tinytag-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinytag-1.8.1/PKG-INFO` & `tinytag-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinytag
-Version: 1.8.1
+Version: 1.9.0
 Summary: Read music meta data and length of MP3, OGG, OPUS, MP4, M4A, FLAC, WMA and Wave files
 Home-page: https://github.com/devsnd/tinytag
 Author: Tom Wallroth
 Author-email: tomwallroth@gmail.com
 License: MIT
 Keywords: metadata,music
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 License-File: LICENSE
 
 tinytag 
 =======
 
 tinytag is a library for reading music meta data of most common audio files in pure python
 
-[![Build Status](https://travis-ci.org/devsnd/tinytag.png?branch=master)](https://travis-ci.org/devsnd/tinytag)
+[![Build Status](https://github.com/devsnd/tinytag/actions/workflows/tests.yml/badge.svg)](https://github.com/devsnd/tinytag/actions?query=workflow:%22Tests%22)
 [![Build status](https://ci.appveyor.com/api/projects/status/w9y2kg97869g1edj?svg=true)](https://ci.appveyor.com/project/devsnd/tinytag)
 [![Coverage Status](https://coveralls.io/repos/devsnd/tinytag/badge.svg)](https://coveralls.io/r/devsnd/tinytag)
 [![PyPI version](https://badge.fury.io/py/tinytag.svg)](https://pypi.org/project/tinytag/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/tinytag.svg)](https://pypistats.org/packages/tinytag)
 
 Install
 -------
@@ -53,15 +53,15 @@
   * supported formats
     * MP3/MP2/MP1 (ID3 v1, v1.1, v2.2, v2.3+)
     * Wave/RIFF
     * OGG
     * OPUS
     * FLAC
     * WMA
-    * MP4/M4A/M4B/M4R/ALAC
+    * MP4/M4A/M4B/M4R/M4V/ALAC/AAX/AAXC
     * AIFF/AIFF-C
   * pure python, no dependencies
   * supports python 2.7 and 3.4 or higher
   * high test coverage
   * Just a few hundred lines of code (just include it in your project!) 
 
 tinytag only provides the minimum needed for _reading_ meta-data.
@@ -81,47 +81,61 @@
 
 List of possible attributes you can get with TinyTag:
 
     tag.album         # album as string
     tag.albumartist   # album artist as string
     tag.artist        # artist name as string
     tag.audio_offset  # number of bytes before audio data begins
+    tag.bitdepth      # bit depth for lossless audio
     tag.bitrate       # bitrate in kBits/s
     tag.comment       # file comment as string
     tag.composer      # composer as string 
     tag.disc          # disc number
     tag.disc_total    # the total number of discs
     tag.duration      # duration of the song in seconds
     tag.filesize      # file size in bytes
     tag.genre         # genre as string
     tag.samplerate    # samples per second
     tag.title         # title of the song
     tag.track         # track number as string
     tag.track_total   # total number of tracks as string
-    tag.year          # year or data as string
+    tag.year          # year or date as string
 
 For non-common fields and fields specific to single file formats use extra
 
     tag.extra         # a dict of additional data
 
 The `extra` dict currently *may* contain the following data:
    `url`, `isrc`, `text`, `initial_key`, `lyrics`, `copyright`
 
-Aditionally you can also get cover images from ID3 tags:
+Additionally you can also get cover images from ID3 tags:
 
     tag = TinyTag.get('/some/music.mp3', image=True)
     image_data = tag.get_image()
 
 To open files using a specific encoding, you can use the `encoding` parameter.
 This parameter is however only used for formats where the encoding isn't explicitly
 specified.
 
     TinyTag.get('a_file_with_gbk_encoding.mp3', encoding='gbk')
 
 Changelog:
+ * 1.9.0  (2023-04-23)
+   - Add bitdepth attribute for lossless audio #157
+   - Add recognition of Audible formats #163 (thanks to snowskeleton)
+   - Add .m4v to list of supported file extensions #142
+   - Aiff: Implement replacement for Python's aifc module #164
+   - ID3: Only check for language in COMM and USLT frames #147
+   - ID3: Read the correct number of bytes from Xing header #154
+   - ID3: Add support for ID3v2.4 TDRC frame #156 (thanks to Uninen)
+   - M4A: Add description fields #168 (thanks to snowskeleton)
+   - RIFF: Handle tags containing extra zero-byte #141
+   - Vorbis: Parse OGG cover art #144 (thanks to Pseurae)
+   - Vorbis: Support standard disctotal/tracktotal comments #171
+   - Wave: Add proper support for padded IFF chunks
  * 1.8.1  (2022-03-12) [still mathiascode-edition]
    - MP3 ID3: Set correct file position if tag reading is disabled #119 (thanks to mathiascode)
    - MP3: Fix incorrect calculation of duration for VBR encoded MP3s #128 (thanks to mathiascode)
  * 1.8.0  (2022-03-05) [mathiascode-edition]
    - Add support for ALAC audio files #130 (thanks to mathiascode)
    - AIFF: Fixed bitrate calculation for certain files #129 (thanks to mathiascode)
    - MP3: Do not round MP3 bitrates #131 (thanks to mathiascode)
```

### Comparing `tinytag-1.8.1/README.md` & `tinytag-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 tinytag 
 =======
 
 tinytag is a library for reading music meta data of most common audio files in pure python
 
-[![Build Status](https://travis-ci.org/devsnd/tinytag.png?branch=master)](https://travis-ci.org/devsnd/tinytag)
+[![Build Status](https://github.com/devsnd/tinytag/actions/workflows/tests.yml/badge.svg)](https://github.com/devsnd/tinytag/actions?query=workflow:%22Tests%22)
 [![Build status](https://ci.appveyor.com/api/projects/status/w9y2kg97869g1edj?svg=true)](https://ci.appveyor.com/project/devsnd/tinytag)
 [![Coverage Status](https://coveralls.io/repos/devsnd/tinytag/badge.svg)](https://coveralls.io/r/devsnd/tinytag)
 [![PyPI version](https://badge.fury.io/py/tinytag.svg)](https://pypi.org/project/tinytag/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/tinytag.svg)](https://pypistats.org/packages/tinytag)
 
 Install
 -------
@@ -22,15 +22,15 @@
   * supported formats
     * MP3/MP2/MP1 (ID3 v1, v1.1, v2.2, v2.3+)
     * Wave/RIFF
     * OGG
     * OPUS
     * FLAC
     * WMA
-    * MP4/M4A/M4B/M4R/ALAC
+    * MP4/M4A/M4B/M4R/M4V/ALAC/AAX/AAXC
     * AIFF/AIFF-C
   * pure python, no dependencies
   * supports python 2.7 and 3.4 or higher
   * high test coverage
   * Just a few hundred lines of code (just include it in your project!) 
 
 tinytag only provides the minimum needed for _reading_ meta-data.
@@ -50,47 +50,61 @@
 
 List of possible attributes you can get with TinyTag:
 
     tag.album         # album as string
     tag.albumartist   # album artist as string
     tag.artist        # artist name as string
     tag.audio_offset  # number of bytes before audio data begins
+    tag.bitdepth      # bit depth for lossless audio
     tag.bitrate       # bitrate in kBits/s
     tag.comment       # file comment as string
     tag.composer      # composer as string 
     tag.disc          # disc number
     tag.disc_total    # the total number of discs
     tag.duration      # duration of the song in seconds
     tag.filesize      # file size in bytes
     tag.genre         # genre as string
     tag.samplerate    # samples per second
     tag.title         # title of the song
     tag.track         # track number as string
     tag.track_total   # total number of tracks as string
-    tag.year          # year or data as string
+    tag.year          # year or date as string
 
 For non-common fields and fields specific to single file formats use extra
 
     tag.extra         # a dict of additional data
 
 The `extra` dict currently *may* contain the following data:
    `url`, `isrc`, `text`, `initial_key`, `lyrics`, `copyright`
 
-Aditionally you can also get cover images from ID3 tags:
+Additionally you can also get cover images from ID3 tags:
 
     tag = TinyTag.get('/some/music.mp3', image=True)
     image_data = tag.get_image()
 
 To open files using a specific encoding, you can use the `encoding` parameter.
 This parameter is however only used for formats where the encoding isn't explicitly
 specified.
 
     TinyTag.get('a_file_with_gbk_encoding.mp3', encoding='gbk')
 
 Changelog:
+ * 1.9.0  (2023-04-23)
+   - Add bitdepth attribute for lossless audio #157
+   - Add recognition of Audible formats #163 (thanks to snowskeleton)
+   - Add .m4v to list of supported file extensions #142
+   - Aiff: Implement replacement for Python's aifc module #164
+   - ID3: Only check for language in COMM and USLT frames #147
+   - ID3: Read the correct number of bytes from Xing header #154
+   - ID3: Add support for ID3v2.4 TDRC frame #156 (thanks to Uninen)
+   - M4A: Add description fields #168 (thanks to snowskeleton)
+   - RIFF: Handle tags containing extra zero-byte #141
+   - Vorbis: Parse OGG cover art #144 (thanks to Pseurae)
+   - Vorbis: Support standard disctotal/tracktotal comments #171
+   - Wave: Add proper support for padded IFF chunks
  * 1.8.1  (2022-03-12) [still mathiascode-edition]
    - MP3 ID3: Set correct file position if tag reading is disabled #119 (thanks to mathiascode)
    - MP3: Fix incorrect calculation of duration for VBR encoded MP3s #128 (thanks to mathiascode)
  * 1.8.0  (2022-03-05) [mathiascode-edition]
    - Add support for ALAC audio files #130 (thanks to mathiascode)
    - AIFF: Fixed bitrate calculation for certain files #129 (thanks to mathiascode)
    - MP3: Do not round MP3 bitrates #131 (thanks to mathiascode)
```

### Comparing `tinytag-1.8.1/setup.cfg` & `tinytag-1.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 [flake8]
 max-line-length = 100
 exclude = .git,__pycache__,.eggs/,doc/,docs/,build/,dist/,archive/,src/
 
 [coverage:run]
 cover_pylib = false
 omit = 
-	/home/travis/virtualenv/*
 	*/site-packages/*
 	*/bin/*
 	*/src/*
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
```

### Comparing `tinytag-1.8.1/tinytag/__main__.py` & `tinytag-1.9.0/tinytag/__main__.py`

 * *Files identical despite different names*

### Comparing `tinytag-1.8.1/tinytag/tests/__test_getid3.py` & `tinytag-1.9.0/tinytag/tests/__test_getid3.py`

 * *Files identical despite different names*

### Comparing `tinytag-1.8.1/tinytag/tests/test_all.py` & `tinytag-1.9.0/tinytag/tests/test_all.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # see custom_samples/instructions.txt
 #
 
 
 from __future__ import unicode_literals
 
 import io
+import operator
 import os
 import re
 import shutil
 import sys
 
 import pytest
 from pytest import raises
@@ -26,83 +27,81 @@
 except ImportError:
     OrderedDict = dict  # python 2.6 and 3.2 compat
 
 
 testfiles = OrderedDict([
     # MP3
     ('samples/vbri.mp3',
-        {'extra': {'url': ''}, 'channels': 2, 'samplerate': 44100, 'track_total': None,
+        {'extra': {'url': ''}, 'channels': 2, 'samplerate': 44100,
          'duration': 0.47020408163265304, 'album': 'I Can Walk On Water I Can Fly', 'year': '2007',
          'title': 'I Can Walk On Water I Can Fly', 'artist': 'Basshunter', 'track': '01',
          'filesize': 8192, 'audio_offset': 1007, 'genre': '(3)Dance',
          'comment': 'Ripped by THSLIVE', 'composer': '', 'bitrate': 125.33333333333333}),
     ('samples/cbr.mp3',
-        {'extra': {}, 'channels': 2, 'samplerate': 44100, 'track_total': None, 'duration': 0.49,
+        {'extra': {}, 'channels': 2, 'samplerate': 44100, 'duration': 0.49,
          'album': 'I Can Walk On Water I Can Fly', 'year': '2007',
          'title': 'I Can Walk On Water I Can Fly', 'artist': 'Basshunter', 'track': '01',
          'filesize': 8186, 'audio_offset': 246, 'bitrate': 128.0, 'genre': 'Dance',
          'comment': 'Ripped by THSLIVE'}),
     # the output of the lame encoder was 185.4 bitrate, but this is good enough for now
     ('samples/vbr_xing_header.mp3',
         {'extra': {}, 'bitrate': 186.04383278145696, 'channels': 1, 'samplerate': 44100,
-         'duration': 3.944489795918367, 'filesize': 91731, 'audio_offset': 441}),
+         'duration': 3.944489795918367, 'filesize': 91731, 'audio_offset': 141}),
     ('samples/vbr_xing_header_2channel.mp3',
         {'extra': {}, 'filesize': 2000, 'album': "The Harpers' Masque",
-         'artist': 'Knodel and Valencia', 'audio_offset': 694, 'bitrate': 46.276128290848305,
+         'artist': 'Knodel and Valencia', 'audio_offset': 394, 'bitrate': 46.276128290848305,
          'channels': 2, 'duration': 250.04408163265308, 'samplerate': 22050,
          'title': 'Lochaber No More', 'year': '1992'}),
     ('samples/id3v22-test.mp3',
         {'extra': {}, 'channels': 2, 'samplerate': 44100, 'track_total': '11', 'duration': 0.138,
          'album': 'Hymns for the Exiled', 'year': '2004', 'title': 'cosmic american',
          'artist': 'Anais Mitchell', 'track': '3', 'filesize': 5120, 'audio_offset': 2225,
          'bitrate': 160.0, 'comment': 'Waterbug Records, www.anaismitchell.com'}),
     ('samples/silence-44-s-v1.mp3',
-        {'extra': {}, 'channels': 2, 'samplerate': 44100, 'genre': 'Darkwave', 'track_total': None,
+        {'extra': {}, 'channels': 2, 'samplerate': 44100, 'genre': 'Darkwave',
          'duration': 3.7355102040816326, 'album': 'Quod Libet Test Data', 'year': '2004',
          'title': 'Silence', 'artist': 'piman', 'track': '2', 'filesize': 15070, 'audio_offset': 0,
          'bitrate': 32.0, 'comment': ''}),
     ('samples/id3v1-latin1.mp3',
-        {'extra': {}, 'channels': None, 'samplerate': None, 'genre': 'Rock',
+        {'extra': {}, 'genre': 'Rock',
          'album': 'The Young Americans', 'title': 'Play Dead', 'filesize': 256, 'track': '12',
-         'artist': 'Björk', 'track_total': None, 'year': '1993',
-         'comment': '                            '}),
+         'artist': 'Björk', 'year': '1993', 'comment': '                            '}),
     ('samples/UTF16.mp3',
         {'extra': {'text': 'MusicBrainz Artist Id664c3e0e-42d8-48c1-b209-1efca19c0325',
-         'url': 'WIKIPEDIA_RELEASEhttp://en.wikipedia.org/wiki/High_Violet'}, 'channels': None,
-         'samplerate': None, 'track_total': '11', 'track': '07', 'artist': 'The National',
+         'url': 'WIKIPEDIA_RELEASEhttp://en.wikipedia.org/wiki/High_Violet'}, 'track_total': '11',
+         'track': '07', 'artist': 'The National',
          'year': '2010', 'album': 'High Violet', 'title': 'Lemonworld', 'filesize': 20480,
          'genre': 'Indie', 'comment': 'Track 7'}),
     ('samples/utf-8-id3v2.mp3',
-        {'extra': {}, 'channels': None, 'samplerate': None, 'genre': 'Acustico',
+        {'extra': {}, 'genre': 'Acustico',
          'track_total': '21', 'track': '01', 'filesize': 2119, 'title': 'Gran día',
-         'artist': 'Paso a paso', 'album': 'S/T', 'year': None, 'disc': '', 'disc_total': '0'}),
+         'artist': 'Paso a paso', 'album': 'S/T', 'disc': '', 'disc_total': '0', 'year': '2003'}),
     ('samples/empty_file.mp3',
-        {'extra': {}, 'channels': None, 'samplerate': None, 'track_total': None, 'album': None,
-         'year': None, 'title': None, 'track': None, 'artist': None, 'filesize': 0}),
+        {'extra': {}, 'filesize': 0}),
     ('samples/silence-44khz-56k-mono-1s.mp3',
         {'extra': {}, 'channels': 1, 'samplerate': 44100, 'duration': 1.018, 'filesize': 7280,
          'audio_offset': 0, 'bitrate': 56.0}),
     ('samples/silence-22khz-mono-1s.mp3',
         {'extra': {}, 'channels': 1, 'samplerate': 22050, 'filesize': 4284, 'audio_offset': 0,
          'bitrate': 32.0, 'duration': 1.0438932496075353}),
     ('samples/id3v24-long-title.mp3',
         {'extra': {}, 'track': '1', 'disc_total': '1',
          'album': 'The Double EP: A Sea of Split Peas', 'filesize': 10000,
-         'channels': None, 'track_total': '12', 'genre': 'AlternRock',
+         'track_total': '12', 'genre': 'AlternRock',
          'title': 'Out of the Woodwork', 'artist': 'Courtney Barnett',
-         'albumartist': 'Courtney Barnett', 'samplerate': None, 'year': None, 'disc': '1',
-         'comment': 'Amazon.com Song ID: 240853806', 'composer': 'Courtney Barnett'}),
+         'albumartist': 'Courtney Barnett', 'disc': '1',
+         'comment': 'Amazon.com Song ID: 240853806', 'composer': 'Courtney Barnett',
+         'year': '2013'}),
     ('samples/utf16be.mp3',
         {'extra': {}, 'title': '52-girls', 'filesize': 2048, 'track': '6', 'album': 'party mix',
-         'artist': 'The B52s', 'genre': 'Rock', 'albumartist': None, 'disc': None,
-         'channels': None}),
+         'artist': 'The B52s', 'genre': 'Rock', 'year': '1981'}),
     ('samples/id3v22_image.mp3',
         {'extra': {}, 'title': 'Kids (MGMT Cover) ', 'filesize': 35924,
          'album': 'winniecooper.net ', 'artist': 'The Kooks', 'year': '2008',
-         'channels': None, 'genre': '.'}),
+         'genre': '.'}),
     ('samples/id3v22.TCO.genre.mp3',
         {'extra': {}, 'filesize': 500, 'album': 'ARTPOP', 'artist': 'Lady GaGa',
          'comment': 'engiTunPGAP0', 'genre': 'Pop', 'title': 'Applause'}),
     ('samples/id3_comment_utf_16_with_bom.mp3',
         {'extra': {'isrc': 'USTC40852229'}, 'filesize': 19980, 'album': 'Ghosts I-IV',
          'albumartist': 'Nine Inch Nails', 'artist': 'Nine Inch Nails', 'disc': '1',
          'disc_total': '2', 'title': '1 Ghosts I', 'track': '1', 'track_total': '36',
@@ -144,75 +143,80 @@
          'artist': 'A Perfect Circle', 'audio_offset': 3647, 'bitrate': 192.0, 'channels': 2,
          'duration': 0.13198711063372717, 'genre': 'Rock',
          'samplerate': 44100, 'title': 'Counting Bodies Like Sheep to the Rhythm of the War Drums',
          'track': '10', 'comment': '                            ',
          'composer': 'Billy Howerdel/Maynard James Keenan', 'disc': '1', 'disc_total': '1',
          'track_total': '12', 'year': '2004'}),
     ('samples/mp3/vbr/vbr8.mp3',
-     {'filesize': 9504, 'audio_offset': 433, 'bitrate': 8.25, 'channels': 1, 'duration': 9.2,
-      'extra': {}, 'samplerate': 8000}),
+        {'filesize': 9504, 'audio_offset': 133, 'bitrate': 8.25, 'channels': 1, 'duration': 9.2,
+         'extra': {}, 'samplerate': 8000}),
     ('samples/mp3/vbr/vbr8stereo.mp3',
-     {'filesize': 9504, 'audio_offset': 441, 'bitrate': 8.25, 'channels': 2, 'duration': 9.216,
-      'extra': {}, 'samplerate': 8000}),
+        {'filesize': 9504, 'audio_offset': 141, 'bitrate': 8.25, 'channels': 2, 'duration': 9.216,
+         'extra': {}, 'samplerate': 8000}),
     ('samples/mp3/vbr/vbr11.mp3',
-     {'filesize': 9360, 'audio_offset': 433, 'bitrate': 8.143465909090908, 'channels': 1,
-      'duration': 9.2, 'extra': {}, 'samplerate': 11025}),
+        {'filesize': 9360, 'audio_offset': 133, 'bitrate': 8.143465909090908, 'channels': 1,
+         'duration': 9.2, 'extra': {}, 'samplerate': 11025}),
     ('samples/mp3/vbr/vbr11stereo.mp3',
-     {'filesize': 9360, 'audio_offset': 441, 'bitrate': 8.143465909090908, 'channels': 2,
-      'duration': 9.195102040816327, 'extra': {}, 'samplerate': 11025}),
+        {'filesize': 9360, 'audio_offset': 141, 'bitrate': 8.143465909090908, 'channels': 2,
+         'duration': 9.195102040816327, 'extra': {}, 'samplerate': 11025}),
     ('samples/mp3/vbr/vbr16.mp3',
-     {'filesize': 9432, 'audio_offset': 433, 'bitrate': 8.251968503937007, 'channels': 1,
-      'duration': 9.2, 'extra': {}, 'samplerate': 16000}),
+        {'filesize': 9432, 'audio_offset': 133, 'bitrate': 8.251968503937007, 'channels': 1,
+         'duration': 9.2, 'extra': {}, 'samplerate': 16000}),
     ('samples/mp3/vbr/vbr16stereo.mp3',
-     {'filesize': 9432, 'audio_offset': 441, 'bitrate': 8.251968503937007, 'channels': 2,
-      'duration': 9.144, 'extra': {}, 'samplerate': 16000}),
+        {'filesize': 9432, 'audio_offset': 141, 'bitrate': 8.251968503937007, 'channels': 2,
+         'duration': 9.144, 'extra': {}, 'samplerate': 16000}),
     ('samples/mp3/vbr/vbr22.mp3',
-     {'filesize': 9282, 'audio_offset': 433, 'bitrate': 8.145021489971347, 'channels': 1,
-      'duration': 9.2, 'extra': {}, 'samplerate': 22050}),
+        {'filesize': 9282, 'audio_offset': 133, 'bitrate': 8.145021489971347, 'channels': 1,
+         'duration': 9.2, 'extra': {}, 'samplerate': 22050}),
     ('samples/mp3/vbr/vbr22stereo.mp3',
-     {'filesize': 9282, 'audio_offset': 441, 'bitrate': 8.145021489971347, 'channels': 2,
-      'duration': 9.11673469387755, 'extra': {}, 'samplerate': 22050}),
+        {'filesize': 9282, 'audio_offset': 141, 'bitrate': 8.145021489971347, 'channels': 2,
+         'duration': 9.11673469387755, 'extra': {}, 'samplerate': 22050}),
     ('samples/mp3/vbr/vbr32.mp3',
-     {'filesize': 37008, 'audio_offset': 441, 'bitrate': 32.50592885375494, 'channels': 1,
-      'duration': 9.108, 'extra': {}, 'samplerate': 32000}),
+        {'filesize': 37008, 'audio_offset': 141, 'bitrate': 32.50592885375494, 'channels': 1,
+         'duration': 9.108, 'extra': {}, 'samplerate': 32000}),
     ('samples/mp3/vbr/vbr32stereo.mp3',
-     {'filesize': 37008, 'audio_offset': 456, 'bitrate': 32.50592885375494, 'channels': 2,
-      'duration': 9.108, 'extra': {}, 'samplerate': 32000}),
+        {'filesize': 37008, 'audio_offset': 156, 'bitrate': 32.50592885375494, 'channels': 2,
+         'duration': 9.108, 'extra': {}, 'samplerate': 32000}),
     ('samples/mp3/vbr/vbr44.mp3',
-     {'filesize': 36609, 'audio_offset': 441, 'bitrate': 32.21697198275862, 'channels': 1,
-      'duration': 9.09061224489796, 'extra': {}, 'samplerate': 44100}),
+        {'filesize': 36609, 'audio_offset': 141, 'bitrate': 32.21697198275862, 'channels': 1,
+         'duration': 9.09061224489796, 'extra': {}, 'samplerate': 44100}),
     ('samples/mp3/vbr/vbr44stereo.mp3',
-     {'filesize': 36609, 'audio_offset': 456, 'bitrate': 32.21697198275862, 'channels': 2,
-      'duration': 9.0, 'extra': {}, 'samplerate': 44100}),
+        {'filesize': 36609, 'audio_offset': 156, 'bitrate': 32.21697198275862, 'channels': 2,
+         'duration': 9.0, 'extra': {}, 'samplerate': 44100}),
     ('samples/mp3/vbr/vbr48.mp3',
-     {'filesize': 36672, 'audio_offset': 441, 'bitrate': 32.33862433862434, 'channels': 1,
-      'duration': 9.072, 'extra': {}, 'samplerate': 48000}),
+        {'filesize': 36672, 'audio_offset': 141, 'bitrate': 32.33862433862434, 'channels': 1,
+         'duration': 9.072, 'extra': {}, 'samplerate': 48000}),
     ('samples/mp3/vbr/vbr48stereo.mp3',
-     {'filesize': 36672, 'audio_offset': 456, 'bitrate': 32.33862433862434, 'channels': 2,
-      'duration': 9.072, 'extra': {}, 'samplerate': 48000}),
+        {'filesize': 36672, 'audio_offset': 156, 'bitrate': 32.33862433862434, 'channels': 2,
+         'duration': 9.072, 'extra': {}, 'samplerate': 48000}),
+    ('samples/id3v24_genre_null_byte.mp3',
+        {'extra': {}, 'filesize': 256, 'album': '\u79d8\u5bc6', 'albumartist': 'aiko',
+         'artist': 'aiko', 'disc': '1', 'genre': 'Pop',
+         'title': '\u661f\u306e\u306a\u3044\u4e16\u754c', 'track': '10', 'year': '2008'}),
+    ('samples/vbr_xing_header_short.mp3',
+        {'filesize': 432, 'audio_offset': 133, 'bitrate': 24.0, 'channels': 1, 'duration': 0.144,
+         'extra': {}, 'samplerate': 8000}),
 
     # OGG
     ('samples/empty.ogg',
-        {'extra': {}, 'track_total': None, 'duration': 3.684716553287982, 'album': None,
-         '_max_samplenum': 162496, 'year': None, 'title': None, 'artist': None, 'track': None,
-         '_tags_parsed': False, 'filesize': 4328, 'audio_offset': 0, 'bitrate': 112.0,
+        {'extra': {}, 'duration': 3.684716553287982,
+         'filesize': 4328, 'audio_offset': 0, 'bitrate': 112.0,
          'samplerate': 44100}),
     ('samples/multipagecomment.ogg',
-        {'extra': {}, 'track_total': None, 'duration': 3.684716553287982, 'album': None,
-         '_max_samplenum': 162496, 'year': None, 'title': None, 'artist': None, 'track': None,
-         '_tags_parsed': False, 'filesize': 135694, 'audio_offset': 0, 'bitrate': 112,
+        {'extra': {}, 'duration': 3.684716553287982,
+         'filesize': 135694, 'audio_offset': 0, 'bitrate': 112,
          'samplerate': 44100}),
     ('samples/multipage-setup.ogg',
-        {'extra': {}, 'genre': 'JRock', 'track_total': None, 'duration': 4.128798185941043,
+        {'extra': {}, 'genre': 'JRock', 'duration': 4.128798185941043,
          'album': 'Timeless', 'year': '2006', 'title': 'Burst', 'artist': 'UVERworld', 'track': '7',
-         '_tags_parsed': False, 'filesize': 76983, 'audio_offset': 0, 'bitrate': 160.0,
+         'filesize': 76983, 'audio_offset': 0, 'bitrate': 160.0,
          'samplerate': 44100}),
     ('samples/test.ogg',
-        {'extra': {}, 'track_total': None, 'duration': 1.0, 'album': 'the boss', 'year': '2006',
-         'title': 'the boss', 'artist': 'james brown', 'track': '1', '_tags_parsed': False,
+        {'extra': {}, 'duration': 1.0, 'album': 'the boss', 'year': '2006',
+         'title': 'the boss', 'artist': 'james brown', 'track': '1',
          'filesize': 7467, 'audio_offset': 0, 'bitrate': 160.0, 'samplerate': 44100,
          'comment': 'hello!'}),
     ('samples/corrupt_metadata.ogg',
         {'extra': {}, 'filesize': 18648, 'audio_offset': 0, 'bitrate': 80.0,
          'duration': 2.132358276643991, 'samplerate': 44100}),
     ('samples/composer.ogg',
         {'extra': {}, 'filesize': 4480, 'album': 'An Album', 'artist': 'An Artist',
@@ -222,117 +226,129 @@
 
     # OPUS
     ('samples/test.opus',
         {'extra': {}, 'albumartist': 'Alstroemeria Records', 'samplerate': 48000, 'channels': 2,
          'track': '1', 'disc': '1', 'title': 'Bad Apple!!', 'duration': 2.0, 'year': '2008.05.25',
          'filesize': 10000, 'artist': 'nomico',
          'album': 'Exserens - A selection of Alstroemeria Records',
-         'comment': 'ARCD0018 - Lovelight'}),
+         'comment': 'ARCD0018 - Lovelight', 'disc_total': '1', 'track_total': '13'}),
     ('samples/8khz_5s.opus',
         {'extra': {}, 'filesize': 7251, 'channels': 1, 'samplerate': 48000, 'duration': 5.0}),
 
     # WAV
     ('samples/test.wav',
         {'extra': {}, 'channels': 2, 'duration': 1.0, 'filesize': 176444, 'bitrate': 1411.2,
-         'samplerate': 44100, 'audio_offset': 36}),
+         'samplerate': 44100, 'bitdepth': 16, 'audio_offset': 36}),
     ('samples/test3sMono.wav',
         {'extra': {}, 'channels': 1, 'duration': 3.0, 'filesize': 264644, 'bitrate': 705.6,
-         'samplerate': 44100, 'audio_offset': 36}),
+         'samplerate': 44100, 'bitdepth': 16, 'audio_offset': 36}),
     ('samples/test-tagged.wav',
         {'extra': {}, 'channels': 2, 'duration': 1.0, 'filesize': 176688, 'album': 'thealbum',
          'artist': 'theartisst', 'bitrate': 1411.2, 'genre': 'Acid', 'samplerate': 44100,
-         'title': 'thetitle', 'track': '66', 'audio_offset': 36, 'comment': 'hello',
+         'bitdepth': 16, 'title': 'thetitle', 'track': '66', 'audio_offset': 36, 'comment': 'hello',
          'year': '2014'}),
     ('samples/test-riff-tags.wav',
-        {'extra': {}, 'channels': 2, 'duration': 1.0, 'filesize': 176540, 'album': None,
+        {'extra': {}, 'channels': 2, 'duration': 1.0, 'filesize': 176540,
          'artist': 'theartisst', 'bitrate': 1411.2, 'genre': 'Acid', 'samplerate': 44100,
-         'title': 'thetitle', 'track': None, 'audio_offset': 36, 'comment': 'hello',
+         'bitdepth': 16, 'title': 'thetitle', 'audio_offset': 36, 'comment': 'hello',
          'year': '2014'}),
     ('samples/silence-22khz-mono-1s.wav',
         {'extra': {}, 'channels': 1, 'duration': 1.0, 'filesize': 48160, 'bitrate': 352.8,
-         'samplerate': 22050, 'audio_offset': 4088}),
+         'samplerate': 22050, 'bitdepth': 16, 'audio_offset': 4088}),
     ('samples/id3_header_with_a_zero_byte.wav',
         {'extra': {}, 'channels': 1, 'duration': 1.0, 'filesize': 44280, 'bitrate': 352.8,
-         'samplerate': 22050, 'audio_offset': 122, 'artist': 'Purpley', 'title': 'Test000',
-         'track': '17'}),
+         'samplerate': 22050, 'bitdepth': 16, 'audio_offset': 122, 'artist': 'Purpley',
+         'title': 'Test000', 'track': '17', 'album': 'prototypes'}),
     ('samples/adpcm.wav',
         {'extra': {}, 'channels': 1, 'duration': 12.167256235827665, 'filesize': 268686,
-         'bitrate': 176.4, 'samplerate': 44100, 'audio_offset': 82, 'artist': 'test artist',
-         'title': 'test title', 'track': '1', 'album': 'test album', 'comment': 'test comment',
-         'genre': 'test genre', 'year': '1990'}),
+         'bitrate': 176.4, 'samplerate': 44100, 'bitdepth': 4, 'audio_offset': 82,
+         'artist': 'test artist', 'title': 'test title', 'track': '1', 'album': 'test album',
+         'comment': 'test comment', 'genre': 'test genre', 'year': '1990'}),
+    ('samples/riff_extra_zero.wav',
+        {'extra': {}, 'channels': 2, 'duration': 0.11609977324263039, 'filesize': 20670,
+         'bitrate': 1411.2, 'samplerate': 44100, 'bitdepth': 16, 'audio_offset': 182,
+         'artist': 'B.O.S.E.', 'title': 'Mission Bass', 'album': '808 Bass Express',
+         'genre': 'Hip-Hop/Rap', 'year': '1996'}),
+    ('samples/riff_extra_zero_2.wav',
+        {'extra': {}, 'channels': 2, 'duration': 0.11609977324263039, 'filesize': 20682,
+         'bitrate': 1411.2, 'samplerate': 44100, 'bitdepth': 16, 'audio_offset': 194,
+         'artist': 'The Jimmy Castor Bunch', 'title': 'It\'s Just Begun',
+         'album': 'The Perfect Beats, Vol. 4', 'genre': 'Pop Electronica'}),
 
     # FLAC
     ('samples/flac1sMono.flac',
-        {'extra': {}, 'genre': 'Avantgarde', 'track_total': None, 'album': 'alb', 'year': '2014',
+        {'extra': {}, 'genre': 'Avantgarde', 'album': 'alb', 'year': '2014',
          'duration': 1.0, 'title': 'track', 'track': '23', 'artist': 'art', 'channels': 1,
-         'filesize': 26632, 'bitrate': 213.056, 'samplerate': 44100}),
+         'filesize': 26632, 'bitrate': 213.056, 'samplerate': 44100, 'bitdepth': 16}),
     ('samples/flac453sStereo.flac',
-        {'extra': {}, 'channels': 2, 'track_total': None, 'album': None, 'year': None,
-         'duration': 453.51473922902494, 'title': None, 'track': None, 'artist': None,
-         'filesize': 84236, 'bitrate': 1.4859230399999999, 'samplerate': 44100}),
+        {'extra': {}, 'channels': 2, 'duration': 453.51473922902494, 'filesize': 84236,
+         'bitrate': 1.4859230399999999, 'samplerate': 44100, 'bitdepth': 16}),
     ('samples/flac1.5sStereo.flac',
-        {'extra': {}, 'channels': 2, 'track_total': None, 'album': 'alb', 'year': '2014',
+        {'extra': {}, 'channels': 2, 'album': 'alb', 'year': '2014',
          'duration': 1.4995238095238095, 'title': 'track', 'track': '23', 'artist': 'art',
          'filesize': 59868, 'bitrate': 319.39739599872973, 'genre': 'Avantgarde',
-         'samplerate': 44100}),
+         'samplerate': 44100, 'bitdepth': 16}),
     ('samples/flac_application.flac',
         {'extra': {}, 'channels': 2, 'track_total': '11',
          'album': 'Belle and Sebastian Write About Love', 'year': '2010-10-11', 'duration': 273.64,
          'title': 'I Want the World to Stop', 'track': '4', 'artist': 'Belle and Sebastian',
-         'filesize': 13000, 'bitrate': 0.38006139453296306, 'samplerate': 44100}),
+         'filesize': 13000, 'bitrate': 0.38006139453296306, 'samplerate': 44100, 'bitdepth': 16}),
     ('samples/no-tags.flac',
-        {'extra': {}, 'channels': 2, 'track_total': None, 'album': None, 'year': None,
-         'duration': 3.684716553287982, 'title': None, 'track': None, 'artist': None,
-         'filesize': 4692, 'bitrate': 10.186943678613627, 'samplerate': 44100}),
+        {'extra': {}, 'channels': 2, 'duration': 3.684716553287982, 'filesize': 4692,
+         'bitrate': 10.186943678613627, 'samplerate': 44100, 'bitdepth': 16}),
     ('samples/variable-block.flac',
         {'extra': {}, 'channels': 2, 'album': 'Appleseed Original Soundtrack', 'year': '2004',
          'duration': 261.68, 'title': 'DIVE FOR YOU', 'track': '01', 'track_total': '11',
          'artist': 'Boom Boom Satellites', 'filesize': 10240, 'bitrate': 0.31305411189238763,
-         'disc': '1', 'genre': 'Anime Soundtrack', 'samplerate': 44100,
+         'disc': '1', 'genre': 'Anime Soundtrack', 'samplerate': 44100, 'bitdepth': 16,
          'composer': 'Boom Boom Satellites (Lyrics)', 'disc_total': '2'}),
     ('samples/106-invalid-streaminfo.flac',
         {'extra': {}, 'filesize': 4692}),
     ('samples/106-short-picture-block-size.flac',
         {'extra': {}, 'filesize': 4692, 'bitrate': 10.186943678613627, 'channels': 2,
-         'duration': 3.68, 'samplerate': 44100}),
+         'duration': 3.68, 'samplerate': 44100, 'bitdepth': 16}),
     ('samples/with_id3_header.flac',
         {'extra': {}, 'filesize': 64837, 'album': '   ', 'artist': '群星', 'disc': '0',
          'title': 'A 梦 哆啦 机器猫 短信铃声', 'track': '0', 'bitrate': 1143.72468, 'channels': 1,
-         'duration': 0.45351473922902497, 'genre': 'genre', 'samplerate': 44100, 'year': '2018'}),
+         'duration': 0.45351473922902497, 'genre': 'genre', 'samplerate': 44100, 'bitdepth': 16,
+         'year': '2018'}),
     ('samples/with_padded_id3_header.flac',
-        {'extra': {}, 'filesize': 16070, 'album': 'album', 'albumartist': None, 'artist': 'artist',
-         'audio_offset': None, 'bitrate': 283.4748, 'channels': 1, 'comment': None, 'disc': None,
-         'disc_total': None, 'duration': 0.45351473922902497, 'genre': 'genre', 'samplerate': 44100,
-         'title': 'title', 'track': '1', 'track_total': None, 'year': '2018'}),
+        {'extra': {}, 'filesize': 16070, 'album': 'album', 'artist': 'artist',
+         'bitrate': 283.4748, 'channels': 1,
+         'duration': 0.45351473922902497, 'genre': 'genre', 'samplerate': 44100, 'bitdepth': 16,
+         'title': 'title', 'track': '1', 'year': '2018'}),
     ('samples/with_padded_id3_header2.flac',
-        {'extra': {}, 'filesize': 19522, 'album': 'Unbekannter Titel', 'albumartist': None,
-         'artist': 'Unbekannter Künstler', 'audio_offset': None, 'bitrate': 344.36807999999996,
-         'channels': 1, 'comment': None, 'disc': '1', 'disc_total': '1',
-         'duration': 0.45351473922902497, 'genre': 'genre', 'samplerate': 44100, 'title': 'Track01',
-         'track': '01', 'track_total': '05', 'year': '2018'}),
+        {'extra': {}, 'filesize': 19522, 'album': 'Unbekannter Titel',
+         'artist': 'Unbekannter Künstler', 'bitrate': 344.36807999999996,
+         'channels': 1, 'disc': '1', 'disc_total': '1',
+         'duration': 0.45351473922902497, 'genre': 'genre', 'samplerate': 44100, 'bitdepth': 16,
+         'title': 'Track01', 'track': '01', 'track_total': '05', 'year': '2018'}),
     ('samples/flac_with_image.flac',
         {'extra': {}, 'filesize': 80000, 'album': 'smilin´ in circles', 'artist': 'Andreas Kümmert',
          'bitrate': 7.6591670655816175, 'channels': 2, 'disc': '1', 'disc_total': '1',
-         'duration': 83.56, 'genre': 'Blues', 'samplerate': 44100, 'title': 'intro', 'track': '01',
-         'track_total': '8'}),
+         'duration': 83.56, 'genre': 'Blues', 'samplerate': 44100, 'bitdepth': 16, 'title': 'intro',
+         'track': '01', 'track_total': '8'}),
 
     # WMA
     ('samples/test2.wma',
         {'extra': {}, 'samplerate': 44100, 'album': 'The Colour and the Shape', 'title': 'Doll',
          'bitrate': 64.04, 'filesize': 5800, 'track': '1', 'albumartist': 'Foo Fighters',
-         'artist': 'Foo Fighters', 'duration': 83.406, 'track_total': None, 'year': '1997',
+         'artist': 'Foo Fighters', 'duration': 83.406, 'year': '1997',
          'genre': 'Alternative', 'comment': '', 'composer': 'Foo Fighters'}),
+    ('samples/lossless.wma',
+        {'extra': {}, 'samplerate': 44100, 'bitrate': 667.296, 'filesize': 2500, 'bitdepth': 16,
+         'duration': 43.133, 'artist': '', 'comment': '', 'title': ''}),
 
     # ALAC/M4A/MP4
     ('samples/test.m4a',
         {'extra': {}, 'samplerate': 44100, 'duration': 314.97, 'bitrate': 256.0, 'channels': 2,
          'genre': 'Pop', 'year': '2011', 'title': 'Nothing', 'album': 'Only Our Hearts To Lose',
          'track_total': '11', 'track': '11', 'artist': 'Marian', 'filesize': 61432}),
     ('samples/test2.m4a',
-        {'extra': {}, 'bitrate': 256.0, 'track': '1',
+        {'extra': {'copyright': '℗ 1992 Ace Records'}, 'bitrate': 256.0, 'track': '1',
          'albumartist': "Millie Jackson - Get It Out 'cha System - 1978",
          'duration': 167.78739229024944, 'filesize': 223365, 'channels': 2, 'year': '1978',
          'artist': 'Millie Jackson', 'track_total': '9', 'disc_total': '1', 'genre': 'R&B/Soul',
          'album': "Get It Out 'cha System", 'samplerate': 44100, 'disc': '1',
          'title': 'Go Out and Get Some',
          'comment': "Millie Jackson - Get It Out 'cha System - 1978",
          'composer': "Millie Jackson - Get It Out 'cha System - 1978"}),
@@ -340,108 +356,152 @@
         {'extra': {}, 'artist': 'Major Lazer', 'filesize': 57017,
          'title': 'Cold Water (feat. Justin Bieber & M�)',
          'album': 'Cold Water (feat. Justin Bieber & M�) - Single', 'year': '2016',
          'samplerate': 44100, 'duration': 188.545, 'genre': 'Electronic;Music',
          'albumartist': 'Major Lazer', 'channels': 2, 'bitrate': 125.584,
          'comment': '? 2016 Mad Decent'}),
     ('samples/alac_file.m4a',
-        {'extra': {}, 'artist': 'Howard Shelley', 'composer': 'Clementi, Muzio (1752-1832)',
+        {'extra': {'copyright': '© Hyperion Records Ltd, London', 'lyrics': 'Album notes:'},
+         'artist': 'Howard Shelley', 'composer': 'Clementi, Muzio (1752-1832)',
          'filesize': 20000,
          'title': 'Clementi: Piano Sonata in D major, Op 25 No 6 - Movement 2: Un poco andante',
          'album': 'Clementi: The Complete Piano Sonatas, Vol. 4', 'year': '2009', 'track': '14',
          'track_total': '27', 'disc': '1', 'disc_total': '1', 'samplerate': 44100,
          'duration': 166.62639455782312, 'genre': 'Classical', 'albumartist': 'Howard Shelley',
-         'channels': 2, 'bitrate': 436.743}),
-
+         'channels': 2, 'bitrate': 436.743, 'bitdepth': 16}),
+    ('samples/mpeg4_desc_cmt.m4a', {
+        'filesize': 32006,
+        'bitrate': 101.038,
+        'channels': 2,
+        'comment': 'test comment',
+        'duration': 2.36,
+        'extra': {'description': 'test description'},
+        'samplerate': 44100}),
+    ('samples/mpeg4_xa9des.m4a', {
+        'filesize': 2639,
+        'comment': 'test comment',
+        'duration': 727.1066666666667,
+        'extra': {'description': 'test description'}}),
     # AIFF
     ('samples/test-tagged.aiff',
         {'extra': {}, 'channels': 2, 'duration': 1.0, 'filesize': 177620, 'artist': 'theartist',
-         'bitrate': 1411.2, 'genre': 'Acid', 'samplerate': 44100, 'track': '1', 'title': 'thetitle',
-         'album': 'thealbum', 'audio_offset': 76, 'comment': 'hello', 'year': '2014'}),
+         'bitrate': 1411.2, 'genre': 'Acid', 'samplerate': 44100, 'bitdepth': 16, 'track': '1',
+         'title': 'thetitle', 'album': 'thealbum', 'audio_offset': 76, 'comment': 'hello',
+         'year': '2014'}),
     ('samples/test.aiff',
         {'extra': {'copyright': '℗ 1992 Ace Records'}, 'channels': 2, 'duration': 0.0,
-         'filesize': 164, 'artist': None, 'bitrate': 1411.2, 'genre': None, 'samplerate': 44100,
-         'track': None, 'title': 'Go Out and Get Some', 'album': None, 'audio_offset': 156,
+         'filesize': 164, 'bitrate': 1411.2, 'samplerate': 44100, 'bitdepth': 16,
+         'title': 'Go Out and Get Some', 'audio_offset': 156,
          'comment': 'Millie Jackson - Get It Out \'cha System - 1978'}),
     ('samples/pluck-pcm8.aiff',
         {'extra': {}, 'channels': 2, 'duration': 0.2999546485260771, 'filesize': 6892,
          'artist': 'Serhiy Storchaka', 'title': 'Pluck', 'album': 'Python Test Suite',
-         'bitrate': 176.4, 'samplerate': 11025, 'audio_offset': 116,
-         'comment': 'Audacity Pluck + Wahwah'}),
+         'bitrate': 176.4, 'samplerate': 11025, 'bitdepth': 8, 'audio_offset': 116,
+         'comment': 'Audacity Pluck + Wahwah', 'year': '2013'}),
     ('samples/M1F1-mulawC-AFsp.afc',
-        {'extra': {}, 'channels': 2, 'duration': 2.936625, 'filesize': 47148, 'artist': None,
-         'title': None, 'album': None, 'bitrate': 256.0, 'samplerate': 8000, 'audio_offset': 154,
+        {'extra': {}, 'channels': 2, 'duration': 2.936625, 'filesize': 47148,
+         'bitrate': 256.0, 'samplerate': 8000, 'bitdepth': 16, 'audio_offset': 154,
          'comment': 'AFspdate: 2003-01-30 03:28:34 UTCuser: kabal@CAPELLAprogram: CopyAudio'}),
+    ('samples/invalid_sample_rate.aiff',
+        {'extra': {}, 'channels': 1, 'filesize': 4096, 'bitdepth': 16}),
 
 ])
 
 testfolder = os.path.join(os.path.dirname(__file__))
 
-# load custom samples
-custom_samples_folder = os.path.join(testfolder, 'custom_samples')
-pattern_field_name_type = [
-    (r'sr=(\d+)', 'samplerate', int),
-    (r'dn=(\d+)', 'disc', str),
-    (r'dt=(\d+)', 'disc_total', str),
-    (r'd=(\d+.?\d*)', 'duration', float),
-    (r'b=(\d+)', 'bitrate', int),
-    (r'c=(\d)', 'channels', int),
-    (r'genre="([^"]+)"', 'genre', str),
-]
-for filename in os.listdir(custom_samples_folder):
-    if filename == 'instructions.txt':
-        continue
-    if os.path.isdir(os.path.join(custom_samples_folder, filename)):
-        continue
-    expected_values = {}
-    for pattern, fieldname, _type in pattern_field_name_type:
-        match = re.findall(pattern, filename)
-        if match:
-            expected_values[fieldname] = _type(match[0])
-    if expected_values:
-        expected_values['__do_not_require_all_values'] = True
-        testfiles[os.path.join('custom_samples', filename)] = expected_values
-    else:
-        # if there are no expected values, just try parsing the file
-        testfiles[os.path.join('custom_samples', filename)] = {}
+
+def load_custom_samples():
+    retval = {}
+    custom_samples_folder = os.path.join(testfolder, 'custom_samples')
+    pattern_field_name_type = [
+        (r'sr=(\d+)', 'samplerate', int),
+        (r'dn=(\d+)', 'disc', str),
+        (r'dt=(\d+)', 'disc_total', str),
+        (r'd=(\d+.?\d*)', 'duration', float),
+        (r'b=(\d+)', 'bitrate', int),
+        (r'c=(\d)', 'channels', int),
+        (r'genre="([^"]+)"', 'genre', str),
+    ]
+    for filename in os.listdir(custom_samples_folder):
+        if filename == 'instructions.txt':
+            continue
+        if os.path.isdir(os.path.join(custom_samples_folder, filename)):
+            continue
+        expected_values = {}
+        for pattern, fieldname, _type in pattern_field_name_type:
+            match = re.findall(pattern, filename)
+            if match:
+                expected_values[fieldname] = _type(match[0])
+        if expected_values:
+            expected_values['_do_not_require_all_values'] = True
+            retval[os.path.join('custom_samples', filename)] = expected_values
+        else:
+            # if there are no expected values, just try parsing the file
+            retval[os.path.join('custom_samples', filename)] = {}
+    return retval
+
+
+testfiles.update(load_custom_samples())
+
+
+def almost_equal_float(val1, val2):
+    # allow duration to be off by 100 ms and a maximum of 1%
+    if val1 == val2:
+        return True
+    if abs(val1 - val2) < 0.100:
+        if val2 and min(val1, val2) / max(val1, val2) > 0.99:
+            return True
+    return False
+
+
+def startswith(val1, val2):
+    return val1.startswith(val2)
+
+
+def error_fmt(value):
+    return '%s (%s)' % (repr(value), type(value))
+
+
+def compare(results, expected, file, prev_path=None):
+    assert isinstance(results, dict)
+    missing_keys = set(expected.keys()) - set(results)
+    assert not missing_keys, 'Missing data in fixture \n%s' % str(missing_keys)
+
+    for key, result_val in results.items():
+        path = prev_path + '.' + key if prev_path else key
+        try:
+            expected_val = expected[key]
+        except KeyError:
+            assert False, 'Missing field "%s": "%s" in fixture "%s"!' % (
+                key, error_fmt(result_val), file)
+        # recurse if the result and expected values are a dict:
+        if isinstance(result_val, dict) and isinstance(expected_val, dict):
+            compare(result_val, expected_val, file, prev_path=key)
+        else:
+            fmt_string = 'field "%s": got %s expected %s in %s!'
+            fmt_values = (key, error_fmt(result_val), error_fmt(expected_val), file)
+            op = operator.eq
+            if path == 'duration':  # allow duration to be off by 100 ms and a maximum of 1%
+                op = almost_equal_float
+            if path == 'extra.lyrics':  # lets not copy *all* the lyrics inside the fixture
+                op = startswith
+            assert op(result_val, expected_val), fmt_string % fmt_values
 
 
 @pytest.mark.parametrize("testfile,expected", [
     pytest.param(testfile, expected) for testfile, expected in testfiles.items()
 ])
 def test_file_reading(testfile, expected):
     filename = os.path.join(testfolder, testfile)
     tag = TinyTag.get(filename)
-
-    for key, expected_val in expected.items():
-        if key.startswith('__'):
-            continue
-        result = getattr(tag, key)
-        fmt_string = 'field "%s": got %s (%s) expected %s (%s)!'
-        fmt_values = (key, repr(result), type(result), repr(expected_val), type(expected_val))
-        if key == 'duration' and result is not None and expected_val is not None:
-            # allow duration to be off by 100 ms and a maximum of 1%
-            if abs(result - expected_val) < 0.100:
-                if expected_val and min(result, expected_val) / max(result, expected_val) > 0.99:
-                    continue
-        assert result == expected_val, fmt_string % fmt_values
-    # for custom samples, allow not specifying all values
-    if expected.get('_do_not_require_all_values'):
-        return
-    undefined_in_fixture = {}
-    for key, val in tag.__dict__.items():
-        if key.startswith('_') or val is None:
-            continue
-        if key not in expected:
-            undefined_in_fixture[key] = val
-    assert not undefined_in_fixture, 'Missing data in fixture \n%s' % str(undefined_in_fixture)
-#
-# def test_generator():
-#     for testfile, expected in testfiles.items():
-#         yield get_info, testfile, expected
+    results = {
+        key: val for key, val in tag.__dict__.items()
+        if not key.startswith('_') and val is not None
+    }
+    compare(results, expected, filename)
 
 
 def test_pathlib_compatibility():
     try:
         import pathlib
     except ImportError:
         return
@@ -608,14 +668,24 @@
     assert image_data is not None
     assert 70000 < len(image_data) < 80000, ('Image is %d bytes but should be around 75kb' %
                                              len(image_data))
     assert image_data.startswith(b'\xff\xd8\xff\xe0'), ('The image data must start with a jpeg '
                                                         'header')
 
 
+def test_ogg_image_loading():
+    tag = TinyTag.get(os.path.join(testfolder, 'samples/ogg_with_image.ogg'), image=True)
+    image_data = tag.get_image()
+    assert image_data is not None
+    assert 1000 < len(image_data) < 2000, ('Image is %d bytes but should be around 1.2kb' %
+                                           len(image_data))
+    assert image_data.startswith(b'\xff\xd8\xff\xe0'), ('The image data must start with a jpeg '
+                                                        'header')
+
+
 def test_aiff_image_loading():
     tag = TinyTag.get(os.path.join(testfolder, 'samples/test_with_image.aiff'), image=True)
     image_data = tag.get_image()
     assert image_data is not None
     assert 15000 < len(image_data) < 25000, ('Image is %d bytes but should be around 20kb' %
                                              len(image_data))
     assert image_data.startswith(b'\xff\xd8\xff\xe0'), ('The image data must start with a jpeg '
@@ -650,12 +720,12 @@
 
 def test_to_str():
     tag = TinyTag.get(os.path.join(testfolder, 'samples/id3v22-test.mp3'))
     assert str(tag)  # since the dict is not ordered we cannot == 'somestring'
     assert repr(tag)  # since the dict is not ordered we cannot == 'somestring'
     assert str(tag) == (
         '{"album": "Hymns for the Exiled", "albumartist": null, "artist": "Anais Mitchell", '
-        '"audio_offset": 2225, "bitrate": 160.0, "channels": 2, "comment": "Waterbug Records, '
-        'www.anaismitchell.com", "composer": null, "disc": null, "disc_total": null, '
-        '"duration": 0.13836297152858082, "extra": {}, "filesize": 5120, "genre": null, '
-        '"samplerate": 44100, "title": "cosmic american", "track": "3", "track_total": "11", '
-        '"year": "2004"}')
+        '"audio_offset": 2225, "bitdepth": null, "bitrate": 160.0, "channels": 2, '
+        '"comment": "Waterbug Records, www.anaismitchell.com", "composer": null, "disc": null, '
+        '"disc_total": null, "duration": 0.13836297152858082, "extra": {}, "filesize": 5120, '
+        '"genre": null, "samplerate": 44100, "title": "cosmic american", "track": "3", '
+        '"track_total": "11", "year": "2004"}')
```

### Comparing `tinytag-1.8.1/tinytag/tests/test_cli.py` & `tinytag-1.9.0/tinytag/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 project_folder = os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
 sample_folder = os.path.join(project_folder, 'tinytag', 'tests', 'samples')
 mp3_with_image = os.path.join(sample_folder, 'id3image_without_description.mp3')
 bogus_file = os.path.join(sample_folder, 'there_is_no_such_ext.bogus')
 assert os.path.exists(mp3_with_image)
 
-tinytag_attributes = {'album', 'albumartist', 'artist', 'audio_offset', 'bitrate', 'channels',
-                      'comment', 'composer', 'disc', 'disc_total', 'duration', 'extra', 'filesize',
-                      'filename', 'genre', 'samplerate', 'title', 'track', 'track_total', 'year'}
+tinytag_attributes = {'album', 'albumartist', 'artist', 'audio_offset', 'bitdepth', 'bitrate',
+                      'channels', 'comment', 'composer', 'disc', 'disc_total', 'duration', 'extra',
+                      'filesize', 'filename', 'genre', 'samplerate', 'title', 'track',
+                      'track_total', 'year'}
 
 
 def run_cli(args):
     output = check_output('python -m tinytag ' + args, cwd=project_folder, shell=True)
     return output.decode('utf-8')
 
 
@@ -33,37 +34,37 @@
 
 def test_print_help():
     assert 'tinytag [options] <filename' in run_cli('-h')
     assert 'tinytag [options] <filename' in run_cli('--help')
 
 
 @pytest.mark.skipif(sys.platform == "win32",
-                    reason="NamedTemporaryFile cant be reopened on windows")
+                    reason="NamedTemporaryFile can't be reopened on windows")
 def test_save_image_long_opt():
     temp_file = NamedTemporaryFile()
     assert file_size(temp_file.name) == 0
     run_cli('--save-image %s %s' % (temp_file.name, mp3_with_image))
     assert file_size(temp_file.name) > 0
     with open(temp_file.name, 'rb') as fh:
         image_data = fh.read(20)
         assert image_data.startswith(b'\xff')
         assert b'JFIF' in image_data
 
 
 @pytest.mark.skipif(sys.platform == "win32",
-                    reason="NamedTemporaryFile cant be reopened on windows")
+                    reason="NamedTemporaryFile can't be reopened on windows")
 def test_save_image_short_opt():
     temp_file = NamedTemporaryFile()
     assert file_size(temp_file.name) == 0
     run_cli('-i %s %s' % (temp_file.name, mp3_with_image))
     assert file_size(temp_file.name) > 0
 
 
 @pytest.mark.skipif(sys.platform == "win32",
-                    reason="NamedTemporaryFile cant be reopened on windows")
+                    reason="NamedTemporaryFile can't be reopened on windows")
 def test_save_image_bulk():
     temp_file = NamedTemporaryFile(suffix='.jpg')
     temp_file_no_ext = temp_file.name[:-4]
     assert file_size(temp_file.name) == 0
     run_cli('-i %s %s %s %s' % (temp_file.name, mp3_with_image, mp3_with_image, mp3_with_image))
     assert file_size(temp_file.name) == 0
     assert file_size(temp_file_no_ext + '00000.jpg') > 0
```

### Comparing `tinytag-1.8.1/tinytag/tinytag.py` & `tinytag-1.9.0/tinytag/tinytag.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,22 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
 from __future__ import division, print_function
-from chunk import Chunk
 from collections import OrderedDict, defaultdict
 try:
     from collections.abc import MutableMapping
 except ImportError:
     from collections import MutableMapping
 from functools import reduce
 from io import BytesIO
-import aifc
+import base64
 import codecs
 import io
 import json
 import operator
 import os
 import re
 import struct
@@ -99,14 +98,15 @@
         self.composer = None
         self.disc = None
         self.disc_total = None
         self.duration = None
         self.extra = defaultdict(lambda: None)
         self.genre = None
         self.samplerate = None
+        self.bitdepth = None
         self.title = None
         self.track = None
         self.track_total = None
         self.year = None
         self._parse_tags = True
         self._load_image = False
         self._image_data = None
@@ -126,15 +126,15 @@
     def _get_parser_for_filename(cls, filename):
         mapping = {
             (b'.mp1', b'.mp2', b'.mp3'): ID3,
             (b'.oga', b'.ogg', b'.opus'): Ogg,
             (b'.wav',): Wave,
             (b'.flac',): Flac,
             (b'.wma',): Wma,
-            (b'.m4b', b'.m4a', b'.m4r', b'.mp4'): MP4,
+            (b'.m4b', b'.m4a', b'.m4r', b'.m4v', b'.mp4', b'.aax', b'.aaxc'): MP4,
             (b'.aiff', b'.aifc', b'.aif', b'.afc'): Aiff,
         }
         if not isinstance(filename, bytes):  # convert filename to binary
             filename = filename.encode('ASCII', errors='ignore').lower()
         for ext, tagclass in mapping.items():
             if filename.endswith(ext):
                 return tagclass
@@ -146,14 +146,16 @@
             b'^ID3': ID3,
             b'^\xff\xfb': ID3,
             b'^OggS': Ogg,
             b'^RIFF....WAVE': Wave,
             b'^fLaC': Flac,
             b'^\x30\x26\xB2\x75\x8E\x66\xCF\x11\xA6\xD9\x00\xAA\x00\x62\xCE\x6C': Wma,
             b'....ftypM4A': MP4,  # https://www.file-recovery.com/m4a-signature-format.htm
+            b'....ftypaax': MP4,  # Audible proprietary M4A container
+            b'....ftypaaxc': MP4,  # Audible proprietary M4A container
             b'\xff\xf1': MP4,  # https://www.garykessler.net/library/file_sigs.html
             b'^FORM....AIFF': Aiff,
             b'^FORM....AIFC': Aiff,
         }
         header = fh.peek(max(len(sig) for sig in magic_bytes_mapping))
         for magic, parser in magic_bytes_mapping.items():
             if re.match(magic, header):
@@ -207,29 +209,27 @@
         if tags:
             self._parse_tag(self._filehandler)
         if duration:
             if tags:  # rewind file if the tags were already parsed
                 self._filehandler.seek(0)
             self._determine_duration(self._filehandler)
 
-    def _set_field(self, fieldname, bytestring, transfunc=None, overwrite=True):
-        """convienience function to set fields of the tinytag by name.
-        the payload (bytestring) can be changed using the transfunc"""
+    def _set_field(self, fieldname, value, overwrite=True):
+        """convenience function to set fields of the tinytag by name"""
         write_dest = self  # write into the TinyTag by default
         get_func = getattr
         set_func = setattr
         is_extra = fieldname.startswith('extra.')  # but if it's marked as extra field
         if is_extra:
             fieldname = fieldname[6:]
             write_dest = self.extra  # write into the extra field instead
             get_func = operator.getitem
             set_func = operator.setitem
         if get_func(write_dest, fieldname):  # do not overwrite existing data
             return
-        value = bytestring if transfunc is None else transfunc(bytestring)
         if DEBUG:
             stderr('Setting field "%s" to "%s"' % (fieldname, value))
         if fieldname == 'genre':
             genre_id = 255
             if value.isdigit():  # funky: id3v1 genre hidden in a id3v2 field
                 genre_id = int(value)
             else:  # funkier: the TCO may contain genres in parens, e.g. '(13)'
@@ -266,17 +266,16 @@
     @staticmethod
     def _unpad(s):
         # strings in mp3 and asf *may* be terminated with a zero byte at the end
         return s.replace('\x00', '')
 
 
 class MP4(TinyTag):
-    # see: https://developer.apple.com/library/mac/documentation/QuickTime/QTFF/Metadata/
-    # Metadata.html
-    # and: https://developer.apple.com/library/mac/documentation/QuickTime/QTFF/QTFFChap2/qtff2.html
+    # https://developer.apple.com/library/mac/documentation/QuickTime/QTFF/Metadata/Metadata.html
+    # https://developer.apple.com/library/mac/documentation/QuickTime/QTFF/QTFFChap2/qtff2.html
 
     class Parser:
         # https://developer.apple.com/library/mac/documentation/QuickTime/QTFF/Metadata/Metadata.html#//apple_ref/doc/uid/TP40000939-CH1-SW34
         ATOM_DECODER_BY_TYPE = {
             0: lambda x: x,  # 'reserved',
             1: lambda x: codecs.decode(x, 'utf-8', 'replace'),   # UTF-8
             2: lambda x: codecs.decode(x, 'utf-16', 'replace'),  # UTF-16
@@ -364,20 +363,22 @@
             return {'channels': channels, 'samplerate': sr, 'bitrate': avg_br}
 
         @classmethod
         def parse_audio_sample_entry_alac(cls, data):
             # https://github.com/macosforge/alac/blob/master/ALACMagicCookieDescription.txt
             alac_atom_size = struct.unpack('>I', data[28:32])[0]
             alac_atom = BytesIO(data[36:36 + alac_atom_size])
-            alac_atom.seek(13, os.SEEK_CUR)
+            alac_atom.seek(9, os.SEEK_CUR)
+            bitdepth = struct.unpack('b', alac_atom.read(1))[0]
+            alac_atom.seek(3, os.SEEK_CUR)
             channels = struct.unpack('b', alac_atom.read(1))[0]
             alac_atom.seek(6, os.SEEK_CUR)
             avg_br = struct.unpack('>I', alac_atom.read(4))[0] / 1000  # kbit/s
             sr = struct.unpack('>I', alac_atom.read(4))[0]
-            return {'channels': channels, 'samplerate': sr, 'bitrate': avg_br}
+            return {'channels': channels, 'samplerate': sr, 'bitrate': avg_br, 'bitdepth': bitdepth}
 
         @classmethod
         def parse_mvhd(cls, data):
             # http://stackoverflow.com/a/3639993/1191373
             walker = BytesIO(data)
             version = struct.unpack('b', walker.read(1))[0]
             walker.seek(3, os.SEEK_CUR)  # jump over flags
@@ -397,26 +398,35 @@
             return {}
 
     # The parser tree: Each key is an atom name which is traversed if existing.
     # Leaves of the parser tree are callables which receive the atom data.
     # callables return {fieldname: value} which is updates the TinyTag.
     META_DATA_TREE = {b'moov': {b'udta': {b'meta': {b'ilst': {
         # see: http://atomicparsley.sourceforge.net/mpeg-4files.html
-        b'\xa9alb': {b'data': Parser.make_data_atom_parser('album')},
+        # and: https://metacpan.org/dist/Image-ExifTool/source/lib/Image/ExifTool/QuickTime.pm#L3093
         b'\xa9ART': {b'data': Parser.make_data_atom_parser('artist')},
-        b'aART': {b'data': Parser.make_data_atom_parser('albumartist')},
-        # b'cpil':    {b'data': Parser.make_data_atom_parser('compilation')},
+        b'\xa9alb': {b'data': Parser.make_data_atom_parser('album')},
         b'\xa9cmt': {b'data': Parser.make_data_atom_parser('comment')},
-        b'disk': {b'data': Parser.make_number_parser('disc', 'disc_total')},
-        b'\xa9wrt': {b'data': Parser.make_data_atom_parser('composer')},
+        # need test-data for this
+        # b'cpil':   {b'data': Parser.make_data_atom_parser('extra.compilation')},
         b'\xa9day': {b'data': Parser.make_data_atom_parser('year')},
+        b'\xa9des': {b'data': Parser.make_data_atom_parser('extra.description')},
         b'\xa9gen': {b'data': Parser.make_data_atom_parser('genre')},
-        b'gnre': {b'data': Parser.parse_id3v1_genre},
+        b'\xa9lyr': {b'data': Parser.make_data_atom_parser('extra.lyrics')},
+        b'\xa9mvn': {b'data': Parser.make_data_atom_parser('movement')},
         b'\xa9nam': {b'data': Parser.make_data_atom_parser('title')},
+        b'\xa9wrt': {b'data': Parser.make_data_atom_parser('composer')},
+        b'aART': {b'data': Parser.make_data_atom_parser('albumartist')},
+        b'cprt': {b'data': Parser.make_data_atom_parser('extra.copyright')},
+        b'desc': {b'data': Parser.make_data_atom_parser('extra.description')},
+        b'disk': {b'data': Parser.make_number_parser('disc', 'disc_total')},
+        b'gnre': {b'data': Parser.parse_id3v1_genre},
         b'trkn': {b'data': Parser.make_number_parser('track', 'track_total')},
+        # need test-data for this
+        # b'tmpo': {b'data': Parser.make_data_atom_parser('extra.bmp')},
     }}}}}
 
     # see: https://developer.apple.com/library/mac/documentation/QuickTime/QTFF/QTFFChap3/qtff3.html
     AUDIO_DATA_TREE = {
         b'moov': {
             b'mvhd': Parser.parse_mvhd,
             b'trak': {b'mdia': {b"minf": {b"stbl": {b"stsd": {
@@ -483,15 +493,15 @@
             atom_header = fh.read(header_size)  # read next atom
 
 
 class ID3(TinyTag):
     FRAME_ID_TO_FIELD = {  # Mapping from Frame ID to a field of the TinyTag
         'COMM': 'comment', 'COM': 'comment',
         'TRCK': 'track', 'TRK': 'track',
-        'TYER': 'year', 'TYE': 'year',
+        'TYER': 'year', 'TYE': 'year', 'TDRC': 'year',
         'TALB': 'album', 'TAL': 'album',
         'TPE1': 'artist', 'TP1': 'artist',
         'TIT2': 'title', 'TT2': 'title',
         'TCON': 'genre', 'TCO': 'genre',
         'TPOS': 'disc',
         'TPE2': 'albumartist', 'TCOM': 'composer',
         'WXXX': 'extra.url',
@@ -549,15 +559,15 @@
         'Psytrance', 'Shoegaze', 'Space Rock', 'Trop Rock', 'World Music',
         'Neoclassical', 'Audiobook', 'Audio Theatre', 'Neue Deutsche Welle',
         'Podcast', 'Indie Rock', 'G-Funk', 'Dubstep', 'Garage Rock', 'Psybient',
     ]
 
     def __init__(self, filehandler, filesize, *args, **kwargs):
         TinyTag.__init__(self, filehandler, filesize, *args, **kwargs)
-        # save position after the ID3 tag for duration mesurement speedup
+        # save position after the ID3 tag for duration measurement speedup
         self._bytepos_after_id3v2 = None
 
     @classmethod
     def set_estimation_precision(cls, estimation_in_seconds):
         cls._MAX_ESTIMATION_SEC = estimation_in_seconds
 
     # see this page for the magic values used in mp3:
@@ -595,15 +605,15 @@
         header_flags = struct.unpack('>i', fh.read(4))[0]
         frames = byte_count = toc = vbr_scale = None
         if header_flags & 1:  # FRAMES FLAG
             frames = struct.unpack('>i', fh.read(4))[0]
         if header_flags & 2:  # BYTES FLAG
             byte_count = struct.unpack('>i', fh.read(4))[0]
         if header_flags & 4:  # TOC FLAG
-            toc = [struct.unpack('>i', fh.read(4))[0] for _ in range(100)]
+            toc = [struct.unpack('>i', fh.read(4))[0] for _ in range(25)]  # 100 bytes
         if header_flags & 8:  # VBR SCALE FLAG
             vbr_scale = struct.unpack('>i', fh.read(4))[0]
         return frames, byte_count, toc, vbr_scale
 
     def _determine_duration(self, fh):
         # if tag reading was disabled, find start position of audio data
         if self._bytepos_after_id3v2 is None:
@@ -734,23 +744,23 @@
             fh.seek(end_pos, os.SEEK_SET)
 
     def _parse_id3v1(self, fh):
         if fh.read(3) == b'TAG':  # check if this is an ID3 v1 tag
             def asciidecode(x):
                 return self._unpad(codecs.decode(x, self._default_encoding or 'latin1'))
             fields = fh.read(30 + 30 + 30 + 4 + 30 + 1)
-            self._set_field('title', fields[:30], transfunc=asciidecode, overwrite=False)
-            self._set_field('artist', fields[30:60], transfunc=asciidecode, overwrite=False)
-            self._set_field('album', fields[60:90], transfunc=asciidecode, overwrite=False)
-            self._set_field('year', fields[90:94], transfunc=asciidecode, overwrite=False)
+            self._set_field('title', asciidecode(fields[:30]), overwrite=False)
+            self._set_field('artist', asciidecode(fields[30:60]), overwrite=False)
+            self._set_field('album', asciidecode(fields[60:90]), overwrite=False)
+            self._set_field('year', asciidecode(fields[90:94]), overwrite=False)
             comment = fields[94:124]
             if b'\x00\x00' < comment[-2:] < b'\x01\x00':
                 self._set_field('track', str(ord(comment[-1:])), overwrite=False)
                 comment = comment[:-2]
-            self._set_field('comment', comment, transfunc=asciidecode, overwrite=False)
+            self._set_field('comment', asciidecode(comment), overwrite=False)
             genre_id = ord(fields[124:125])
             if genre_id < len(ID3.ID3V1_GENRES):
                 self._set_field('genre', ID3.ID3V1_GENRES[genre_id], overwrite=False)
 
     @staticmethod
     def index_utf16(s, search):
         for i in range(0, len(s), len(search)):
@@ -777,15 +787,16 @@
             # flags = frame[1+frame_size_bytes:] # dont care about flags.
             if frame_id not in ID3.PARSABLE_FRAME_IDS:  # jump over unparsable frames
                 fh.seek(frame_size, os.SEEK_CUR)
                 return frame_size
             content = fh.read(frame_size)
             fieldname = ID3.FRAME_ID_TO_FIELD.get(frame_id)
             if fieldname:
-                self._set_field(fieldname, content, self._decode_string)
+                language = fieldname in ("comment", "extra.lyrics")
+                self._set_field(fieldname, self._decode_string(content, language))
             elif frame_id in self.IMAGE_FRAME_IDS and self._load_image:
                 # See section 4.14: http://id3.org/id3v2.4.0-frames
                 encoding = content[0:1]
                 if frame_id == 'PIC':  # ID3 v2.2:
                     desc_start_pos = 1 + 3 + 1  # skip encoding (1), imgformat (3), pictype(1)
                 else:  # ID3 v2.3+
                     desc_start_pos = content.index(b'\x00', 1) + 1 + 1  # skip mimetype, pictype(1)
@@ -793,33 +804,34 @@
                 termination = b'\x00' if encoding in (b'\x00', b'\x03') else b'\x00\x00'
                 desc_length = ID3.index_utf16(content[desc_start_pos:], termination)
                 desc_end_pos = desc_start_pos + desc_length + len(termination)
                 self._image_data = content[desc_end_pos:]
             return frame_size
         return 0
 
-    def _decode_string(self, bytestr):
+    def _decode_string(self, bytestr, language=False):
         default_encoding = 'ISO-8859-1'
         if self._default_encoding:
             default_encoding = self._default_encoding
         try:  # it's not my fault, this is the spec.
             first_byte = bytestr[:1]
             if first_byte == b'\x00':  # ISO-8859-1
                 bytestr = bytestr[1:]
                 encoding = default_encoding
             elif first_byte == b'\x01':  # UTF-16 with BOM
                 bytestr = bytestr[1:]
                 # remove language (but leave BOM)
-                if bytestr[3:5] in (b'\xfe\xff', b'\xff\xfe'):
-                    bytestr = bytestr[3:]
-                if bytestr[:3].isalpha() and bytestr[3:4] == b'\x00':
-                    bytestr = bytestr[4:]  # remove language
-                if bytestr[:1] == b'\x00':
-                    bytestr = bytestr[1:]  # strip optional additional null byte
-                # read byte order mark to determine endianess
+                if language:
+                    if bytestr[3:5] in (b'\xfe\xff', b'\xff\xfe'):
+                        bytestr = bytestr[3:]
+                    if bytestr[:3].isalpha() and bytestr[3:4] == b'\x00':
+                        bytestr = bytestr[4:]  # remove language
+                    if bytestr[:1] == b'\x00':
+                        bytestr = bytestr[1:]  # strip optional additional null byte
+                # read byte order mark to determine endianness
                 encoding = 'UTF-16be' if bytestr[0:2] == b'\xfe\xff' else 'UTF-16le'
                 # strip the bom if it exists
                 if bytestr[:2] in (b'\xfe\xff', b'\xff\xfe'):
                     bytestr = bytestr[2:] if len(bytestr) % 2 == 0 else bytestr[2:-1]
                 # remove ADDITIONAL EXTRA BOM :facepalm:
                 if bytestr[:4] == b'\x00\x00\xff\xfe':
                     bytestr = bytestr[4:]
@@ -829,15 +841,15 @@
                 encoding = 'UTF-16le'
             elif first_byte == b'\x03':  # UTF-8
                 bytestr = bytestr[1:]
                 encoding = 'UTF-8'
             else:
                 bytestr = bytestr
                 encoding = default_encoding  # wild guess
-            if bytestr[:3].isalpha() and bytestr[3:4] == b'\x00':
+            if language and bytestr[:3].isalpha() and bytestr[3:4] == b'\x00':
                 bytestr = bytestr[4:]  # remove language
             errors = 'ignore' if self._ignore_errors else 'strict'
             return self._unpad(codecs.decode(bytestr, encoding, errors))
         except UnicodeDecodeError:
             raise TinyTagException('Error decoding ID3 Tag!')
 
     def _calc_size(self, bytestr, bits_per_byte):
@@ -868,15 +880,15 @@
                 self.duration = self._max_samplenum / self.samplerate
             else:
                 idx = b.find(b'OggS')  # try to find header in peeked data
                 seekpos = idx if idx != -1 else len(b) - 3
                 fh.seek(max(seekpos, 1), os.SEEK_CUR)
 
     def _parse_tag(self, fh):
-        page_start_pos = fh.tell()  # set audio_offest later if its audio data
+        page_start_pos = fh.tell()  # set audio_offset later if its audio data
         for packet in self._parse_pages(fh):
             walker = BytesIO(packet)
             if packet[0:7] == b"\x01vorbis":
                 (channels, self.samplerate, max_bitrate, bitrate,
                  min_bitrate) = struct.unpack("<B4i", packet[11:28])
                 if not self.audio_offset:
                     self.bitrate = bitrate / 1000
@@ -908,16 +920,18 @@
         comment_type_to_attr_mapping = {
             'album': 'album',
             'albumartist': 'albumartist',
             'title': 'title',
             'artist': 'artist',
             'date': 'year',
             'tracknumber': 'track',
+            'tracktotal': 'track_total',
             'totaltracks': 'track_total',
             'discnumber': 'disc',
+            'disctotal': 'disc_total',
             'totaldiscs': 'disc_total',
             'genre': 'genre',
             'description': 'comment',
             'composer': 'composer',
         }
         vendor_length = struct.unpack('I', fh.read(4))[0]
         fh.seek(vendor_length, os.SEEK_CUR)  # jump over vendor
@@ -926,19 +940,26 @@
             length = struct.unpack('I', fh.read(4))[0]
             try:
                 keyvalpair = codecs.decode(fh.read(length), 'UTF-8')
             except UnicodeDecodeError:
                 continue
             if '=' in keyvalpair:
                 key, value = keyvalpair.split('=', 1)
-                if DEBUG:
-                    stderr('Found Vorbis Comment', key, value[:64])
-                fieldname = comment_type_to_attr_mapping.get(key.lower())
-                if fieldname:
-                    self._set_field(fieldname, value)
+                key_lowercase = key.lower()
+
+                if key_lowercase == "metadata_block_picture" and self._load_image:
+                    if DEBUG:
+                        stderr('Found Vorbis Image', key, value[:64])
+                    self._image_data = Flac._parse_image(BytesIO(base64.b64decode(value)))
+                else:
+                    if DEBUG:
+                        stderr('Found Vorbis Comment', key, value[:64])
+                    fieldname = comment_type_to_attr_mapping.get(key_lowercase)
+                    if fieldname:
+                        self._set_field(fieldname, value)
 
     def _parse_pages(self, fh):
         # for the spec, see: https://wiki.xiph.org/Ogg
         previous_page = b''  # contains data from previous (continuing) pages
         header_data = fh.read(27)  # read ogg page header
         while len(header_data) != 0:
             header = struct.unpack('<4sBBqIIiB', header_data)
@@ -965,19 +986,21 @@
 
 
 class Wave(TinyTag):
     # https://sno.phy.queensu.ca/~phil/exiftool/TagNames/RIFF.html
     riff_mapping = {
         b'INAM': 'title',
         b'TITL': 'title',
+        b'IPRD': 'album',
         b'IART': 'artist',
         b'ICMT': 'comment',
         b'ICRD': 'year',
         b'IGNR': 'genre',
         b'ISRC': 'extra.isrc',
+        b'ITRK': 'track',
         b'TRCK': 'track',
         b'PRT1': 'track',
         b'PRT2': 'track_number',
         b'YEAR': 'year',
         # riff format is lacking the composer field.
     }
 
@@ -987,47 +1010,48 @@
 
     def _determine_duration(self, fh):
         # see: http://www-mmsp.ece.mcgill.ca/Documents/AudioFormats/WAVE/WAVE.html
         # and: https://en.wikipedia.org/wiki/WAV
         riff, size, fformat = struct.unpack('4sI4s', fh.read(12))
         if riff != b'RIFF' or fformat != b'WAVE':
             raise TinyTagException('not a wave file!')
-        bitdepth = 16  # assume 16bit depth (CD quality)
+        self.bitdepth = 16  # assume 16bit depth (CD quality)
         chunk_header = fh.read(8)
         while len(chunk_header) == 8:
             subchunkid, subchunksize = struct.unpack('4sI', chunk_header)
+            subchunksize += subchunksize % 2  # IFF chunks are padded to an even number of bytes
             if subchunkid == b'fmt ':
                 _, self.channels, self.samplerate = struct.unpack('HHI', fh.read(8))
-                _, _, bitdepth = struct.unpack('<IHH', fh.read(8))
-                if bitdepth == 0:
+                _, _, self.bitdepth = struct.unpack('<IHH', fh.read(8))
+                if self.bitdepth == 0:
                     # Certain codecs (e.g. GSM 6.10) give us a bit depth of zero.
                     # Avoid division by zero when calculating duration.
-                    bitdepth = 1
-                self.bitrate = self.samplerate * self.channels * bitdepth / 1000
+                    self.bitdepth = 1
+                self.bitrate = self.samplerate * self.channels * self.bitdepth / 1000
                 remaining_size = subchunksize - 16
                 if remaining_size > 0:
                     fh.seek(remaining_size, 1)  # skip remaining data in chunk
             elif subchunkid == b'data':
-                self.duration = subchunksize / self.channels / self.samplerate / (bitdepth / 8)
+                self.duration = subchunksize / self.channels / self.samplerate / (self.bitdepth / 8)
                 self.audio_offset = fh.tell() - 8  # rewind to data header
                 fh.seek(subchunksize, 1)
             elif subchunkid == b'LIST' and self._parse_tags:
                 is_info = fh.read(4)  # check INFO header
                 if is_info != b'INFO':  # jump over non-INFO sections
                     fh.seek(subchunksize - 4, os.SEEK_CUR)
                 else:
                     sub_fh = BytesIO(fh.read(subchunksize - 4))
                     field = sub_fh.read(4)
                     while len(field) == 4:
                         data_length = struct.unpack('I', sub_fh.read(4))[0]
+                        data_length += data_length % 2  # IFF chunks are padded to an even size
                         data = sub_fh.read(data_length).split(b'\x00', 1)[0]  # strip zero-byte
-                        data = codecs.decode(data, 'utf-8')
                         fieldname = self.riff_mapping.get(field)
                         if fieldname:
-                            self._set_field(fieldname, data)
+                            self._set_field(fieldname, codecs.decode(data, 'utf-8'))
                         field = sub_fh.read(4)
             elif subchunkid in (b'id3 ', b'ID3 ') and self._parse_tags:
                 id3 = ID3(fh, 0)
                 id3._parse_id3v2(fh)
                 self.update(id3)
             else:  # some other chunk, just skip the data
                 fh.seek(subchunksize, 1)
@@ -1072,15 +1096,15 @@
             size = _bytes_to_int(meta_header[1:4])
             # http://xiph.org/flac/format.html#metadata_block_streaminfo
             if block_type == Flac.METADATA_STREAMINFO:
                 stream_info_header = fh.read(size)
                 if len(stream_info_header) < 34:  # invalid streaminfo
                     return
                 header = struct.unpack('HH3s3s8B16s', stream_info_header)
-                # From the ciph documentation:
+                # From the xiph documentation:
                 # py | <bits>
                 # ----------------------------------------------
                 # H  | <16>  The minimum block size (in samples)
                 # H  | <16>  The maximum block size (in samples)
                 # 3s | <24>  The minimum frame size (in bytes)
                 # 3s | <24>  The maximum frame size (in bytes)
                 # 8B | <20>  Sample rate in Hz.
@@ -1093,44 +1117,47 @@
                 # max_frm = _bytes_to_int(struct.unpack('3B', max_frm))
                 #                 channels--.  bits      total samples
                 # |----- samplerate -----| |-||----| |---------~   ~----|
                 # 0000 0000 0000 0000 0000 0000 0000 0000 0000      0000
                 # #---4---# #---5---# #---6---# #---7---# #--8-~   ~-12-#
                 self.samplerate = _bytes_to_int(header[4:7]) >> 4
                 self.channels = ((header[6] >> 1) & 0x07) + 1
-                # bit_depth = ((header[6] & 1) << 4) + ((header[7] & 0xF0) >> 4)
-                # bit_depth = (bit_depth + 1)
+                self.bitdepth = (((header[6] & 1) << 4) + ((header[7] & 0xF0) >> 4) + 1)
                 total_sample_bytes = [(header[7] & 0x0F)] + list(header[8:12])
                 total_samples = _bytes_to_int(total_sample_bytes)
                 self.duration = total_samples / self.samplerate
                 if self.duration > 0:
                     self.bitrate = self.filesize / self.duration * 8 / 1000
             elif block_type == Flac.METADATA_VORBIS_COMMENT and self._parse_tags:
                 oggtag = Ogg(fh, 0)
                 oggtag._parse_vorbis_comment(fh)
                 self.update(oggtag)
             elif block_type == Flac.METADATA_PICTURE and self._load_image:
-                # https://xiph.org/flac/format.html#metadata_block_picture
-                pic_type, mime_len = struct.unpack('>2I', fh.read(8))
-                fh.read(mime_len)
-                description_len = struct.unpack('>I', fh.read(4))[0]
-                fh.read(description_len)
-                width, height, depth, colors, pic_len = struct.unpack('>5I', fh.read(20))
-                self._image_data = fh.read(pic_len)
+                self._image_data = self._parse_image(fh)
             elif block_type >= 127:
                 return  # invalid block type
             else:
                 if DEBUG:
                     stderr('Unknown FLAC block type', block_type)
                 fh.seek(size, 1)  # seek over this block
 
             if is_last_block:
                 return
             header_data = fh.read(4)
 
+    @staticmethod
+    def _parse_image(fh):
+        # https://xiph.org/flac/format.html#metadata_block_picture
+        pic_type, mime_len = struct.unpack('>2I', fh.read(8))
+        fh.read(mime_len)
+        description_len = struct.unpack('>I', fh.read(4))[0]
+        fh.read(description_len)
+        width, height, depth, colors, pic_len = struct.unpack('>5I', fh.read(20))
+        return fh.read(pic_len)
+
 
 class Wma(TinyTag):
     ASF_CONTENT_DESCRIPTION_OBJECT = b'3&\xb2u\x8ef\xcf\x11\xa6\xd9\x00\xaa\x00b\xcel'
     ASF_EXTENDED_CONTENT_DESCRIPTION_OBJECT = (b'@\xa4\xd0\xd2\x07\xe3\xd2\x11\x97\xf0\x00'
                                                b'\xa0\xc9^\xa8P')
     STREAM_BITRATE_PROPERTIES_OBJECT = b'\xceu\xf8{\x8dF\xd1\x11\x8d\x82\x00`\x97\xc9\xa2\xb2'
     ASF_FILE_PROPERTY_OBJECT = b'\xa1\xdc\xab\x8cG\xa9\xcf\x11\x8e\xe4\x00\xc0\x0c Se'
@@ -1209,27 +1236,26 @@
                     ('artist', len_blocks['author_length'], False),
                     ('', len_blocks['copyright_length'], True),
                     ('comment', len_blocks['description_length'], False),
                     ('', len_blocks['rating_length'], True),
                 ])
                 for field_name, bytestring in data_blocks.items():
                     if field_name:
-                        self._set_field(field_name, bytestring, self.__decode_string)
+                        self._set_field(field_name, self.__decode_string(bytestring))
             elif object_id == Wma.ASF_EXTENDED_CONTENT_DESCRIPTION_OBJECT and self._parse_tags:
                 mapping = {
                     'WM/TrackNumber': 'track',
                     'WM/PartOfSet': 'disc',
                     'WM/Year': 'year',
                     'WM/AlbumArtist': 'albumartist',
                     'WM/Genre': 'genre',
                     'WM/AlbumTitle': 'album',
                     'WM/Composer': 'composer',
                 }
-                # see: http://web.archive.org/web/20131203084402/http://msdn.microsoft.com/en-us/
-                # library/bb643323.aspx#_Toc509555195
+                # http://web.archive.org/web/20131203084402/http://msdn.microsoft.com/en-us/library/bb643323.aspx#_Toc509555195
                 descriptor_count = _bytes_to_int_le(fh.read(2))
                 for _ in range(descriptor_count):
                     name_len = _bytes_to_int_le(fh.read(2))
                     name = self.__decode_string(fh.read(name_len))
                     value_type = _bytes_to_int_le(fh.read(2))
                     value_len = _bytes_to_int_le(fh.read(2))
                     value = fh.read(value_len)
@@ -1273,106 +1299,96 @@
                         ('samples_per_second', 4, True),
                         ('avg_bytes_per_second', 4, True),
                         ('block_alignment', 2, True),
                         ('bits_per_sample', 2, True),
                     ])
                     self.samplerate = stream_info['samples_per_second']
                     self.bitrate = stream_info['avg_bytes_per_second'] * 8 / 1000
+                    if stream_info['codec_id_format_tag'] == 355:  # lossless
+                        self.bitdepth = stream_info['bits_per_sample']
                     already_read = 16
                 fh.seek(blocks['type_specific_data_length'] - already_read, os.SEEK_CUR)
                 fh.seek(blocks['error_correction_data_length'], os.SEEK_CUR)
             else:
                 fh.seek(object_size - 24, os.SEEK_CUR)  # read over onknown object ids
 
 
 class Aiff(ID3):
     #
-    # AIFF is part of the IFF family of file formats.  That means it has a _wide_
-    # variety of things that can appear in it.  However... Python natively
-    # supports reading/writing the most common AIFF formats! But it does not
-    # support pulling tags out of them.  Therefore, Python is going to do the
-    # heavy lifting and this code just handles the metadata chunks.
+    # AIFF is part of the IFF family of file formats.
     #
     # https://en.wikipedia.org/wiki/Audio_Interchange_File_Format#Data_format
     # https://web.archive.org/web/20171118222232/http://www-mmsp.ece.mcgill.ca/documents/audioformats/aiff/aiff.html
     # https://web.archive.org/web/20071219035740/http://www.cnpbagwell.com/aiff-c.txt
     #
     # A few things about the spec:
     #
     # * IFF strings are not supposed to be null terminated.  They sometimes are.
-    # * The spec is a bit contradictory in terms of strings being ASCII or not. The assumption
-    #   here is that they are.
     # * Some tools might throw more metadata into the ANNO chunk but it is
     #   wildly unreliable to count on it. In fact, the official spec recommends against
     #   using it. That said... this code throws the ANNO field into comment and hopes
     #   for the best.
     #
-    # Additionally:
-    #
-    # * Python allegedly supports ALAW/alaw, G722, and ULAW/ulaw AIFF-C compression.
-    #   However it does seem to have implementation bugs.
-    #   Anything it doesn't understand (e.g., 'sowt') will throw an exception.
-    #
     # The key thing here is that AIFF metadata is usually in a handful of fields
     # and the rest is an ID3 or XMP field.  XMP is too complicated and only Adobe-related
     # products support it. The vast majority use ID3. As such, this code inherits from
     # ID3 rather than TinyTag since it does everything that needs to be done here.
     #
-    #
-    def __init__(self, filehandler, filesize, *args, **kwargs):
-        super(Aiff, self).__init__(filehandler, filesize, *args, **kwargs)
-        self.__tag_parsed = False
 
-    def _determine_duration(self, fh):
-        fh.seek(0, 0)
-        # NOTE: aifc will throw an exception if a compression
-        # type is not supported, such as 'sowt'
-        aiffobj = aifc.open(fh, 'rb')
-        self.channels = aiffobj.getnchannels()
-        self.samplerate = aiffobj.getframerate()
-        self.duration = aiffobj.getnframes() / self.samplerate
-        self.bitrate = self.samplerate * self.channels * aiffobj.getsampwidth() * 8 / 1000
+    aiff_mapping = {
+        #
+        # "Name Chunk text contains the name of the sampled sound."
+        #
+        # "Author Chunk text contains one or more author names.  An author in
+        # this case is the creator of a sampled sound."
+        #
+        # "Annotation Chunk text contains a comment.  Use of this chunk is
+        # discouraged within FORM AIFC." Some tools: "hold my beer"
+        #
+        # "The Copyright Chunk contains a copyright notice for the sound.  text
+        #  contains a date followed by the copyright owner.  The chunk ID '[c] '
+        # serves as the copyright character. " Some tools: "hold my beer"
+        #
+        b'NAME': 'title',
+        b'AUTH': 'artist',
+        b'ANNO': 'comment',
+        b'(c) ': 'extra.copyright',
+    }
 
-    def _parse_tag(self, fh):
-        fh.seek(0, 0)
-        self.__tag_parsed = True
-        chunk = Chunk(fh)
-        if chunk.getname() != b'FORM':
-            raise TinyTagException('not an aiff file!')
+    def __init__(self, filehandler, filesize, *args, **kwargs):
+        ID3.__init__(self, filehandler, filesize, *args, **kwargs)
+        self._tags_parsed = False
 
-        formdata = chunk.read(4)
-        if formdata not in (b'AIFC', b'AIFF'):
+    def _parse_tag(self, fh):
+        chunk_id, size, form = struct.unpack('>4sI4s', fh.read(12))
+        if chunk_id != b'FORM' or form not in (b'AIFC', b'AIFF'):
             raise TinyTagException('not an aiff file!')
-
-        while True:
-            try:
-                chunk = Chunk(fh)
-            except EOFError:
-                break
-
-            chunkname = chunk.getname()
-            if chunkname == b'NAME':
-                # "Name Chunk text contains the name of the sampled sound."
-                self.title = self._unpad(chunk.read().decode('utf-8'))
-            elif chunkname == b'AUTH':
-                # "Author Chunk text contains one or more author names.  An author in
-                # this case is the creator of a sampled sound."
-                self.artist = self._unpad(chunk.read().decode('utf-8'))
-            elif chunkname == b'ANNO':
-                # "Annotation Chunk text contains a comment.  Use of this chunk is
-                # discouraged within FORM AIFC." Some tools: "hold my beer"
-                self._set_field('comment', self._unpad(chunk.read().decode('utf-8')))
-            elif chunkname == b'(c) ':
-                # "The Copyright Chunk contains a copyright notice for the sound.  text
-                #  contains a date followed by the copyright owner.  The chunk ID '[c] '
-                # serves as the copyright character. " Some tools: "hold my beer"
-                field = chunk.read().decode('utf-8')
-                self._set_field('extra.copyright', field)
-            elif chunkname == b'ID3 ':
-                super(Aiff, self)._parse_tag(fh)
-            elif chunkname == b'SSND':
-                # probably the closest equivalent, but this isn't particular viable
-                # for AIFF
+        chunk_header = fh.read(8)
+        while len(chunk_header) == 8:
+            sub_chunk_id, sub_chunk_size = struct.unpack('>4sI', chunk_header)
+            sub_chunk_size += sub_chunk_size % 2  # IFF chunks are padded to an even number of bytes
+            if sub_chunk_id in self.aiff_mapping and self._parse_tags:
+                value = self._unpad(fh.read(sub_chunk_size).decode('utf-8'))
+                self._set_field(self.aiff_mapping[sub_chunk_id], value)
+            elif sub_chunk_id == b'COMM':
+                self.channels, num_frames, self.bitdepth = struct.unpack('>hLh', fh.read(8))
+                try:
+                    exponent, mantissa = struct.unpack('>HQ', fh.read(10))   # Extended precision
+                    self.samplerate = int(mantissa * (2 ** (exponent - 0x3FFF - 63)))
+                    self.duration = num_frames / self.samplerate
+                    self.bitrate = self.samplerate * self.channels * self.bitdepth / 1000
+                except OverflowError:
+                    self.samplerate = self.duration = self.bitrate = None  # invalid sample rate
+                fh.seek(sub_chunk_size - 18, 1)  # skip remaining data in chunk
+            elif sub_chunk_id in (b'id3 ', b'ID3 ') and self._parse_tags:
+                ID3._parse_tag(self, fh)
+            elif sub_chunk_id == b'SSND':
                 self.audio_offset = fh.tell()
-                chunk.skip()
-            else:
-                chunk.skip()
+                fh.seek(sub_chunk_size, 1)
+            else:  # some other chunk, just skip the data
+                fh.seek(sub_chunk_size, 1)
+            chunk_header = fh.read(8)
+        self._tags_parsed = True
+
+    def _determine_duration(self, fh):
+        if not self._tags_parsed:
+            self._parse_tag(fh)
```

### Comparing `tinytag-1.8.1/tinytag.egg-info/PKG-INFO` & `tinytag-1.9.0/tinytag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinytag
-Version: 1.8.1
+Version: 1.9.0
 Summary: Read music meta data and length of MP3, OGG, OPUS, MP4, M4A, FLAC, WMA and Wave files
 Home-page: https://github.com/devsnd/tinytag
 Author: Tom Wallroth
 Author-email: tomwallroth@gmail.com
 License: MIT
 Keywords: metadata,music
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 License-File: LICENSE
 
 tinytag 
 =======
 
 tinytag is a library for reading music meta data of most common audio files in pure python
 
-[![Build Status](https://travis-ci.org/devsnd/tinytag.png?branch=master)](https://travis-ci.org/devsnd/tinytag)
+[![Build Status](https://github.com/devsnd/tinytag/actions/workflows/tests.yml/badge.svg)](https://github.com/devsnd/tinytag/actions?query=workflow:%22Tests%22)
 [![Build status](https://ci.appveyor.com/api/projects/status/w9y2kg97869g1edj?svg=true)](https://ci.appveyor.com/project/devsnd/tinytag)
 [![Coverage Status](https://coveralls.io/repos/devsnd/tinytag/badge.svg)](https://coveralls.io/r/devsnd/tinytag)
 [![PyPI version](https://badge.fury.io/py/tinytag.svg)](https://pypi.org/project/tinytag/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/tinytag.svg)](https://pypistats.org/packages/tinytag)
 
 Install
 -------
@@ -53,15 +53,15 @@
   * supported formats
     * MP3/MP2/MP1 (ID3 v1, v1.1, v2.2, v2.3+)
     * Wave/RIFF
     * OGG
     * OPUS
     * FLAC
     * WMA
-    * MP4/M4A/M4B/M4R/ALAC
+    * MP4/M4A/M4B/M4R/M4V/ALAC/AAX/AAXC
     * AIFF/AIFF-C
   * pure python, no dependencies
   * supports python 2.7 and 3.4 or higher
   * high test coverage
   * Just a few hundred lines of code (just include it in your project!) 
 
 tinytag only provides the minimum needed for _reading_ meta-data.
@@ -81,47 +81,61 @@
 
 List of possible attributes you can get with TinyTag:
 
     tag.album         # album as string
     tag.albumartist   # album artist as string
     tag.artist        # artist name as string
     tag.audio_offset  # number of bytes before audio data begins
+    tag.bitdepth      # bit depth for lossless audio
     tag.bitrate       # bitrate in kBits/s
     tag.comment       # file comment as string
     tag.composer      # composer as string 
     tag.disc          # disc number
     tag.disc_total    # the total number of discs
     tag.duration      # duration of the song in seconds
     tag.filesize      # file size in bytes
     tag.genre         # genre as string
     tag.samplerate    # samples per second
     tag.title         # title of the song
     tag.track         # track number as string
     tag.track_total   # total number of tracks as string
-    tag.year          # year or data as string
+    tag.year          # year or date as string
 
 For non-common fields and fields specific to single file formats use extra
 
     tag.extra         # a dict of additional data
 
 The `extra` dict currently *may* contain the following data:
    `url`, `isrc`, `text`, `initial_key`, `lyrics`, `copyright`
 
-Aditionally you can also get cover images from ID3 tags:
+Additionally you can also get cover images from ID3 tags:
 
     tag = TinyTag.get('/some/music.mp3', image=True)
     image_data = tag.get_image()
 
 To open files using a specific encoding, you can use the `encoding` parameter.
 This parameter is however only used for formats where the encoding isn't explicitly
 specified.
 
     TinyTag.get('a_file_with_gbk_encoding.mp3', encoding='gbk')
 
 Changelog:
+ * 1.9.0  (2023-04-23)
+   - Add bitdepth attribute for lossless audio #157
+   - Add recognition of Audible formats #163 (thanks to snowskeleton)
+   - Add .m4v to list of supported file extensions #142
+   - Aiff: Implement replacement for Python's aifc module #164
+   - ID3: Only check for language in COMM and USLT frames #147
+   - ID3: Read the correct number of bytes from Xing header #154
+   - ID3: Add support for ID3v2.4 TDRC frame #156 (thanks to Uninen)
+   - M4A: Add description fields #168 (thanks to snowskeleton)
+   - RIFF: Handle tags containing extra zero-byte #141
+   - Vorbis: Parse OGG cover art #144 (thanks to Pseurae)
+   - Vorbis: Support standard disctotal/tracktotal comments #171
+   - Wave: Add proper support for padded IFF chunks
  * 1.8.1  (2022-03-12) [still mathiascode-edition]
    - MP3 ID3: Set correct file position if tag reading is disabled #119 (thanks to mathiascode)
    - MP3: Fix incorrect calculation of duration for VBR encoded MP3s #128 (thanks to mathiascode)
  * 1.8.0  (2022-03-05) [mathiascode-edition]
    - Add support for ALAC audio files #130 (thanks to mathiascode)
    - AIFF: Fixed bitrate calculation for certain files #129 (thanks to mathiascode)
    - MP3: Do not round MP3 bitrates #131 (thanks to mathiascode)
```

