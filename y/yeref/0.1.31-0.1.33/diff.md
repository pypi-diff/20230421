# Comparing `tmp/yeref-0.1.31.tar.gz` & `tmp/yeref-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.31.tar", last modified: Fri Apr 21 16:33:32 2023, max compression
+gzip compressed data, was "yeref-0.1.33.tar", last modified: Fri Apr 21 17:01:36 2023, max compression
```

## Comparing `yeref-0.1.31.tar` & `yeref-0.1.33.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 16:33:32.155248 yeref-0.1.31/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 16:33:32.155480 yeref-0.1.31/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 16:33:32.156654 yeref-0.1.31/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1106 2023-04-21 16:33:19.000000 yeref-0.1.31/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 16:33:32.145733 yeref-0.1.31/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       21 2022-09-17 12:40:01.000000 yeref-0.1.31/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   241961 2023-04-20 14:54:58.000000 yeref-0.1.31/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 16:33:32.154456 yeref-0.1.31/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 16:33:31.000000 yeref-0.1.31/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      167 2023-04-21 16:33:32.000000 yeref-0.1.31/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 16:33:31.000000 yeref-0.1.31/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 16:33:31.000000 yeref-0.1.31/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:01:36.162832 yeref-0.1.33/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:01:36.162977 yeref-0.1.33/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-21 17:01:36.163552 yeref-0.1.33/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1106 2023-04-21 16:53:09.000000 yeref-0.1.33/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:01:36.156404 yeref-0.1.33/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       21 2022-09-17 12:40:01.000000 yeref-0.1.33/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   241923 2023-04-21 16:49:48.000000 yeref-0.1.33/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-21 17:01:36.162447 yeref-0.1.33/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      167 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-21 17:01:36.000000 yeref-0.1.33/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.31/setup.py` & `yeref-0.1.33/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.31',
+      version='0.1.33',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -35,8 +35,8 @@
 # python setup.py sdist
 # python setup.py install
 # python setup.py develop
 # twine upload dist/*
 # python3 -m pip install --upgrade yeref
 
 # python setup.py bdist_wheel
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.31-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.33-py3-none-any.whl
```

### Comparing `yeref-0.1.31/yeref/yeref.py` & `yeref-0.1.33/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from oauth2client.service_account import ServiceAccountCredentials
 from pyrogram import enums, Client
 from pyrogram.errors import FloodWait, UserAlreadyParticipant, UsernameInvalid, BadRequest, SlowmodeWait, \
     UserDeactivatedBan, SessionRevoked, SessionExpired, AuthKeyUnregistered, AuthKeyInvalid, AuthKeyDuplicated, \
     InviteHashExpired, InviteHashInvalid, ChatAdminRequired, UserDeactivated, UsernameNotOccupied, ChannelBanned
 from pyrogram.raw import functions
 from stegano import lsb, exifHeader
-from telegram.error import RetryAfter
 from telegraph import Telegraph
 
 one_minute = 60
 one_hour = 3600
 seconds_in_day = 86400
 my_tid = 5491025132
 my_tids = [
```

