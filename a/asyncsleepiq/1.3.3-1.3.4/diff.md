# Comparing `tmp/asyncsleepiq-1.3.3.tar.gz` & `tmp/asyncsleepiq-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncsleepiq-1.3.3.tar", last modified: Thu Apr 20 18:36:15 2023, max compression
+gzip compressed data, was "asyncsleepiq-1.3.4.tar", last modified: Fri Apr 21 20:29:29 2023, max compression
```

## Comparing `asyncsleepiq-1.3.3.tar` & `asyncsleepiq-1.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/asyncsleepiq/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 18:36:08.000000 asyncsleepiq-1.3.3/asyncsleepiq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/asyncsleepiq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/bed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/bed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/foundation.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/fuzion/sleeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-20 18:35:59.000000 asyncsleepiq-1.3.3/asyncsleepiq/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 18:36:15.000000 asyncsleepiq-1.3.3/asyncsleepiq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:36:15.463537 asyncsleepiq-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-20 18:36:08.000000 asyncsleepiq-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:29:29.073212 asyncsleepiq-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 20:29:29.073212 asyncsleepiq-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:29:29.073212 asyncsleepiq-1.3.4/asyncsleepiq/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-21 20:29:22.000000 asyncsleepiq-1.3.4/asyncsleepiq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/asyncsleepiq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:29:29.073212 asyncsleepiq-1.3.4/asyncsleepiq/fuzion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/fuzion/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/fuzion/bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/fuzion/foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/fuzion/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/fuzion/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/fuzion/sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-21 20:29:14.000000 asyncsleepiq-1.3.4/asyncsleepiq/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:29:29.073212 asyncsleepiq-1.3.4/asyncsleepiq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 20:29:29.000000 asyncsleepiq-1.3.4/asyncsleepiq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-21 20:29:29.000000 asyncsleepiq-1.3.4/asyncsleepiq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:29:29.000000 asyncsleepiq-1.3.4/asyncsleepiq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 20:29:29.000000 asyncsleepiq-1.3.4/asyncsleepiq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 20:29:29.000000 asyncsleepiq-1.3.4/asyncsleepiq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 20:29:29.073212 asyncsleepiq-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-21 20:29:22.000000 asyncsleepiq-1.3.4/setup.py
```

### Comparing `asyncsleepiq-1.3.3/LICENSE` & `asyncsleepiq-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/PKG-INFO` & `asyncsleepiq-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncsleepiq
-Version: 1.3.3
+Version: 1.3.4
 Summary: ASync SleepIQ API
 Home-page: http://github.com/kbickar/asyncsleepiq
 Author: Keilin Bickar
 Author-email: trumpetgod@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `asyncsleepiq-1.3.3/README.md` & `asyncsleepiq-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/actuator.py` & `asyncsleepiq-1.3.4/asyncsleepiq/actuator.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/api.py` & `asyncsleepiq-1.3.4/asyncsleepiq/api.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/asyncsleepiq.py` & `asyncsleepiq-1.3.4/asyncsleepiq/asyncsleepiq.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/bed.py` & `asyncsleepiq-1.3.4/asyncsleepiq/bed.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/consts.py` & `asyncsleepiq-1.3.4/asyncsleepiq/consts.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/foundation.py` & `asyncsleepiq-1.3.4/asyncsleepiq/foundation.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/fuzion/actuator.py` & `asyncsleepiq-1.3.4/asyncsleepiq/fuzion/actuator.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/fuzion/bed.py` & `asyncsleepiq-1.3.4/asyncsleepiq/fuzion/bed.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/fuzion/foundation.py` & `asyncsleepiq-1.3.4/asyncsleepiq/fuzion/foundation.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/fuzion/light.py` & `asyncsleepiq-1.3.4/asyncsleepiq/fuzion/light.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/fuzion/preset.py` & `asyncsleepiq-1.3.4/asyncsleepiq/fuzion/preset.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/fuzion/sleeper.py` & `asyncsleepiq-1.3.4/asyncsleepiq/fuzion/sleeper.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,24 +18,26 @@
             raise ValueError("Invalid SleepNumber, must be between 0 and 100")
         setting = int(round(setting / 5)) * 5
         args = [SIDES_FULL[self.side].lower(), setting]
         await self.api.bamkey(self.bed_id, "StartSleepNumberAdjustment", args=args)
 
     async def fetch_sleepnumber(self) -> None:
         """Update fav_sleep_number from API."""
-        result = await self.api.bamkey(self.bed_id, "GetSleepNumberControls")
-        updating, current, last = result.split()
-        self.sleep_number = int(current)
+        args = [SIDES_FULL[self.side].lower()]
+        result = await self.api.bamkey(self.bed_id, "GetSleepNumberControls", args=args)
+        is_updating, ambient_number, user_number = result.split()
+        self.sleep_number = int(user_number)
 
     async def set_favsleepnumber(self, setting: int) -> None:
         """Set favorite sleep number 5-100 (multiple of 5)."""
         if 0 > setting or setting > 100:
             raise ValueError("Invalid SleepNumber, must be between 0 and 100")
         setting = int(round(setting / 5)) * 5
         args = [SIDES_FULL[self.side].lower(), setting]
         await self.api.bamkey(self.bed_id, "SetFavoriteSleepNumber", args=args)
         await self.fetch_favsleepnumber()
 
     async def fetch_favsleepnumber(self) -> None:
         """Update fav_sleep_number from API."""
-        result = await self.api.bamkey(self.bed_id, "GetFavoriteSleepNumber")
+        args = [SIDES_FULL[self.side].lower()]
+        result = await self.api.bamkey(self.bed_id, "GetFavoriteSleepNumber", args=args)
         self.fav_sleep_number = int(result)
```

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/light.py` & `asyncsleepiq-1.3.4/asyncsleepiq/light.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/preset.py` & `asyncsleepiq-1.3.4/asyncsleepiq/preset.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq/sleeper.py` & `asyncsleepiq-1.3.4/asyncsleepiq/sleeper.py`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq.egg-info/PKG-INFO` & `asyncsleepiq-1.3.4/asyncsleepiq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncsleepiq
-Version: 1.3.3
+Version: 1.3.4
 Summary: ASync SleepIQ API
 Home-page: http://github.com/kbickar/asyncsleepiq
 Author: Keilin Bickar
 Author-email: trumpetgod@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `asyncsleepiq-1.3.3/asyncsleepiq.egg-info/SOURCES.txt` & `asyncsleepiq-1.3.4/asyncsleepiq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncsleepiq-1.3.3/setup.py` & `asyncsleepiq-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         return f.read()
 
 
 setup(
     name="asyncsleepiq",
     packages=["asyncsleepiq", "asyncsleepiq.fuzion"],
     package_data={"asyncsleepiq": ["py.typed"]},
-    version="1.3.3",
+    version="1.3.4",
     description="ASync SleepIQ API",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="http://github.com/kbickar/asyncsleepiq",
     author="Keilin Bickar",
     author_email="trumpetgod@gmail.com",
     license="MIT",
```

