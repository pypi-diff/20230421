# Comparing `tmp/apdaily-1.0.2.tar.gz` & `tmp/apdaily-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apdaily-1.0.2.tar", last modified: Fri Apr 21 00:22:14 2023, max compression
+gzip compressed data, was "apdaily-1.0.3.tar", last modified: Fri Apr 21 00:24:03 2023, max compression
```

## Comparing `apdaily-1.0.2.tar` & `apdaily-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:22:14.063712 apdaily-1.0.2/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      834 2023-04-21 00:22:14.065717 apdaily-1.0.2/PKG-INFO
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      505 2023-04-20 17:56:45.000000 apdaily-1.0.2/README.md
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      103 2023-04-20 17:56:45.000000 apdaily-1.0.2/pyproject.toml
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      712 2023-04-21 00:22:14.078742 apdaily-1.0.2/setup.cfg
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:22:13.186158 apdaily-1.0.2/src/
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:22:13.434498 apdaily-1.0.2/src/apdaily/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.2/src/apdaily/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      143 2023-04-20 17:56:45.000000 apdaily-1.0.2/src/apdaily/main.py
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:22:13.766198 apdaily-1.0.2/src/apdaily.egg-info/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      834 2023-04-21 00:22:12.000000 apdaily-1.0.2/src/apdaily.egg-info/PKG-INFO
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      428 2023-04-21 00:22:13.000000 apdaily-1.0.2/src/apdaily.egg-info/SOURCES.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        1 2023-04-21 00:22:12.000000 apdaily-1.0.2/src/apdaily.egg-info/dependency_links.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)       12 2023-04-21 00:22:12.000000 apdaily-1.0.2/src/apdaily.egg-info/requires.txt
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)       40 2023-04-21 00:22:12.000000 apdaily-1.0.2/src/apdaily.egg-info/top_level.txt
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:22:13.911075 apdaily-1.0.2/src/apdaily_methods/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.2/src/apdaily_methods/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     3487 2023-04-21 00:14:47.000000 apdaily-1.0.2/src/apdaily_methods/apdaily_m1.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)      335 2023-04-20 17:56:45.000000 apdaily-1.0.2/src/apdaily_methods/mouse_util.py
-drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:22:13.997508 apdaily-1.0.2/src/apdaily_startup/
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.2/src/apdaily_startup/__init__.py
--rwxrwxrwx   0 redshift  (1000) redshift  (1000)     4603 2023-04-21 00:21:18.000000 apdaily-1.0.2/src/apdaily_startup/apdaily_startup_main.py
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:24:03.719644 apdaily-1.0.3/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      834 2023-04-21 00:24:03.723718 apdaily-1.0.3/PKG-INFO
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      505 2023-04-20 17:56:45.000000 apdaily-1.0.3/README.md
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      103 2023-04-20 17:56:45.000000 apdaily-1.0.3/pyproject.toml
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      712 2023-04-21 00:24:03.746703 apdaily-1.0.3/setup.cfg
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:24:02.334127 apdaily-1.0.3/src/
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:24:02.568821 apdaily-1.0.3/src/apdaily/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.3/src/apdaily/__init__.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      143 2023-04-20 17:56:45.000000 apdaily-1.0.3/src/apdaily/main.py
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:24:03.045109 apdaily-1.0.3/src/apdaily.egg-info/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      834 2023-04-21 00:24:01.000000 apdaily-1.0.3/src/apdaily.egg-info/PKG-INFO
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      428 2023-04-21 00:24:02.000000 apdaily-1.0.3/src/apdaily.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        1 2023-04-21 00:24:01.000000 apdaily-1.0.3/src/apdaily.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)       12 2023-04-21 00:24:01.000000 apdaily-1.0.3/src/apdaily.egg-info/requires.txt
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)       40 2023-04-21 00:24:01.000000 apdaily-1.0.3/src/apdaily.egg-info/top_level.txt
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:24:03.404179 apdaily-1.0.3/src/apdaily_methods/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.3/src/apdaily_methods/__init__.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)     3487 2023-04-21 00:14:47.000000 apdaily-1.0.3/src/apdaily_methods/apdaily_m1.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)      335 2023-04-20 17:56:45.000000 apdaily-1.0.3/src/apdaily_methods/mouse_util.py
+drwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-21 00:24:03.611779 apdaily-1.0.3/src/apdaily_startup/
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)        0 2023-04-20 17:56:45.000000 apdaily-1.0.3/src/apdaily_startup/__init__.py
+-rwxrwxrwx   0 redshift  (1000) redshift  (1000)     4567 2023-04-21 00:23:47.000000 apdaily-1.0.3/src/apdaily_startup/apdaily_startup_main.py
```

### Comparing `apdaily-1.0.2/PKG-INFO` & `apdaily-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apdaily
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that allows you to watch AP Classroom Daily videos automatically.
 Home-page: https://github.com/SarangaR/APDaily-Dev
 Author: Saranga Rajagopalan
 Author-email: sarnga.raj@gmail.com
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `apdaily-1.0.2/setup.cfg` & `apdaily-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apdaily
-version = 1.0.2
+version = 1.0.3
 author = Saranga Rajagopalan
 author_email = sarnga.raj@gmail.com
 description = A package that allows you to watch AP Classroom Daily videos automatically.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SarangaR/APDaily-Dev
 project_urls =
```

### Comparing `apdaily-1.0.2/src/apdaily.egg-info/PKG-INFO` & `apdaily-1.0.3/src/apdaily.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apdaily
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package that allows you to watch AP Classroom Daily videos automatically.
 Home-page: https://github.com/SarangaR/APDaily-Dev
 Author: Saranga Rajagopalan
 Author-email: sarnga.raj@gmail.com
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `apdaily-1.0.2/src/apdaily_methods/apdaily_m1.py` & `apdaily-1.0.3/src/apdaily_methods/apdaily_m1.py`

 * *Files identical despite different names*

### Comparing `apdaily-1.0.2/src/apdaily_startup/apdaily_startup_main.py` & `apdaily-1.0.3/src/apdaily_startup/apdaily_startup_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,20 @@
             logger.error("Browser not found")
             sys.exit(0)
         os.chdir(browser_prefix_path)
         os.system(f'gtk-launch {browser_executable} > /dev/null 2>&1 &')
     elif platform.system() == "Windows":
         windows_config = toml.load("C:\\Program Files\\apdaily\\apdaily-config.toml")
         config = windows_config
-        browser_prefix_path = str(config["startup-config"]["browser-prefix-path"])
-        browser_executable = str(config["startup-config"]["browser-executable"])
-        if not os.path.exists(os.path.join(browser_prefix_path, browser_executable)):
-            logger.error("Browser not found")
-            sys.exit(0)
-        subprocess.Popen(os.path.join(browser_prefix_path, browser_executable))
+        # browser_prefix_path = str(config["startup-config"]["browser-prefix-path"])
+        # browser_executable = str(config["startup-config"]["browser-executable"])
+        # if not os.path.exists(os.path.join(browser_prefix_path, browser_executable)):
+        #     logger.error("Browser not found")
+        #     sys.exit(0)
+        os.system("start msedge")
     else:
         logger.error("OS not supported")
         sys.exit(0)
 
     keyboard = kb.Controller()
     mouse = ms.Controller()
```

