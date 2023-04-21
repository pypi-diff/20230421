# Comparing `tmp/PM3-0.3.8.tar.gz` & `tmp/PM3-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PM3-0.3.8.tar", last modified: Sun Jun 26 21:56:25 2022, max compression
+gzip compressed data, was "PM3-0.3.9.tar", last modified: Sun Jun 26 22:04:50 2022, max compression
```

## Comparing `PM3-0.3.8.tar` & `PM3-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 21:56:25.055769 PM3-0.3.8/
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     1813 2021-12-30 15:09:54.000000 PM3-0.3.8/.gitignore
--rw-rw-r--   0 ilario    (1000) ilario    (1000)    35149 2021-12-27 18:27:28.000000 PM3-0.3.8/LICENSE
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     4527 2022-06-26 21:56:25.055769 PM3-0.3.8/PKG-INFO
-drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 21:56:25.051769 PM3-0.3.8/PM3/
--rw-rw-r--   0 ilario    (1000) ilario    (1000)       40 2022-01-02 17:31:46.000000 PM3-0.3.8/PM3/__init__.py
--rwxr-xr-x   0 ilario    (1000) ilario    (1000)    11581 2022-06-24 13:59:20.000000 PM3-0.3.8/PM3/app.py
--rwxr-xr-x   0 ilario    (1000) ilario    (1000)    21961 2022-06-26 21:50:08.000000 PM3-0.3.8/PM3/cli.py
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     1664 2022-06-24 22:16:47.000000 PM3-0.3.8/PM3/cron_checker.py
-drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 21:56:25.051769 PM3-0.3.8/PM3/libs/
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     3340 2022-06-24 14:04:40.000000 PM3-0.3.8/PM3/libs/pm3table.py
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     1514 2022-06-25 14:07:22.000000 PM3-0.3.8/PM3/libs/system_scripts.py
-drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 21:56:25.051769 PM3-0.3.8/PM3/model/
--rw-rw-r--   0 ilario    (1000) ilario    (1000)      507 2022-06-24 13:13:13.000000 PM3-0.3.8/PM3/model/pm3_protocol.py
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     7947 2022-06-26 21:49:16.000000 PM3-0.3.8/PM3/model/process.py
-drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 21:56:25.051769 PM3-0.3.8/PM3.egg-info/
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     4527 2022-06-26 21:56:24.000000 PM3-0.3.8/PM3.egg-info/PKG-INFO
--rw-rw-r--   0 ilario    (1000) ilario    (1000)      526 2022-06-26 21:56:24.000000 PM3-0.3.8/PM3.egg-info/SOURCES.txt
--rw-rw-r--   0 ilario    (1000) ilario    (1000)        1 2022-06-26 21:56:24.000000 PM3-0.3.8/PM3.egg-info/dependency_links.txt
--rw-rw-r--   0 ilario    (1000) ilario    (1000)      105 2022-06-26 21:56:24.000000 PM3-0.3.8/PM3.egg-info/entry_points.txt
--rw-rw-r--   0 ilario    (1000) ilario    (1000)      156 2022-06-26 21:56:24.000000 PM3-0.3.8/PM3.egg-info/requires.txt
--rw-rw-r--   0 ilario    (1000) ilario    (1000)        4 2022-06-26 21:56:24.000000 PM3-0.3.8/PM3.egg-info/top_level.txt
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     4074 2022-06-26 21:55:26.000000 PM3-0.3.8/README.md
--rwxr-xr-x   0 ilario    (1000) ilario    (1000)       73 2021-12-29 16:44:27.000000 PM3-0.3.8/build.sh
--rw-rw-r--   0 ilario    (1000) ilario    (1000)      155 2022-06-22 14:51:38.000000 PM3-0.3.8/requirements.txt
-drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 21:56:25.055769 PM3-0.3.8/screenshots/
--r--------   0 ilario    (1000) ilario    (1000)    54624 2022-06-25 23:07:04.000000 PM3-0.3.8/screenshots/dump.png
--r--------   0 ilario    (1000) ilario    (1000)    89828 2022-06-25 23:03:23.000000 PM3-0.3.8/screenshots/help.png
--rw-rw-r--   0 ilario    (1000) ilario    (1000)    74594 2022-06-25 23:01:05.000000 PM3-0.3.8/screenshots/ls.png
--r--------   0 ilario    (1000) ilario    (1000)    73063 2022-06-25 23:04:08.000000 PM3-0.3.8/screenshots/new_help.png
--r--------   0 ilario    (1000) ilario    (1000)    55668 2022-06-25 23:02:36.000000 PM3-0.3.8/screenshots/ps.png
--r--------   0 ilario    (1000) ilario    (1000)   101774 2022-06-25 23:06:21.000000 PM3-0.3.8/screenshots/systemd_script.png
--rw-rw-r--   0 ilario    (1000) ilario    (1000)       38 2022-06-26 21:56:25.055769 PM3-0.3.8/setup.cfg
--rw-rw-r--   0 ilario    (1000) ilario    (1000)     1019 2022-06-26 21:55:26.000000 PM3-0.3.8/setup.py
--rwxr-xr-x   0 ilario    (1000) ilario    (1000)       40 2021-12-29 16:50:20.000000 PM3-0.3.8/upload.sh
+drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 22:04:50.052103 PM3-0.3.9/
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     1813 2021-12-30 15:09:54.000000 PM3-0.3.9/.gitignore
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)    35149 2021-12-27 18:27:28.000000 PM3-0.3.9/LICENSE
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     4685 2022-06-26 22:04:50.052103 PM3-0.3.9/PKG-INFO
+drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 22:04:50.052103 PM3-0.3.9/PM3/
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)       40 2022-01-02 17:31:46.000000 PM3-0.3.9/PM3/__init__.py
+-rwxr-xr-x   0 ilario    (1000) ilario    (1000)    11581 2022-06-24 13:59:20.000000 PM3-0.3.9/PM3/app.py
+-rwxr-xr-x   0 ilario    (1000) ilario    (1000)    21961 2022-06-26 21:50:08.000000 PM3-0.3.9/PM3/cli.py
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     1664 2022-06-24 22:16:47.000000 PM3-0.3.9/PM3/cron_checker.py
+drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 22:04:50.052103 PM3-0.3.9/PM3/libs/
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     3340 2022-06-24 14:04:40.000000 PM3-0.3.9/PM3/libs/pm3table.py
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     1514 2022-06-25 14:07:22.000000 PM3-0.3.9/PM3/libs/system_scripts.py
+drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 22:04:50.052103 PM3-0.3.9/PM3/model/
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)      507 2022-06-24 13:13:13.000000 PM3-0.3.9/PM3/model/pm3_protocol.py
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     7947 2022-06-26 21:49:16.000000 PM3-0.3.9/PM3/model/process.py
+drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 22:04:50.052103 PM3-0.3.9/PM3.egg-info/
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     4685 2022-06-26 22:04:49.000000 PM3-0.3.9/PM3.egg-info/PKG-INFO
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)      526 2022-06-26 22:04:49.000000 PM3-0.3.9/PM3.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)        1 2022-06-26 22:04:49.000000 PM3-0.3.9/PM3.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)      105 2022-06-26 22:04:49.000000 PM3-0.3.9/PM3.egg-info/entry_points.txt
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)      156 2022-06-26 22:04:49.000000 PM3-0.3.9/PM3.egg-info/requires.txt
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)        4 2022-06-26 22:04:49.000000 PM3-0.3.9/PM3.egg-info/top_level.txt
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     4232 2022-06-26 22:03:42.000000 PM3-0.3.9/README.md
+-rwxr-xr-x   0 ilario    (1000) ilario    (1000)       73 2021-12-29 16:44:27.000000 PM3-0.3.9/build.sh
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)      155 2022-06-22 14:51:38.000000 PM3-0.3.9/requirements.txt
+drwxrwxr-x   0 ilario    (1000) ilario    (1000)        0 2022-06-26 22:04:50.052103 PM3-0.3.9/screenshots/
+-r--------   0 ilario    (1000) ilario    (1000)    54624 2022-06-25 23:07:04.000000 PM3-0.3.9/screenshots/dump.png
+-r--------   0 ilario    (1000) ilario    (1000)    89828 2022-06-25 23:03:23.000000 PM3-0.3.9/screenshots/help.png
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)    74594 2022-06-25 23:01:05.000000 PM3-0.3.9/screenshots/ls.png
+-r--------   0 ilario    (1000) ilario    (1000)    73063 2022-06-25 23:04:08.000000 PM3-0.3.9/screenshots/new_help.png
+-r--------   0 ilario    (1000) ilario    (1000)    55668 2022-06-25 23:02:36.000000 PM3-0.3.9/screenshots/ps.png
+-r--------   0 ilario    (1000) ilario    (1000)   101774 2022-06-25 23:06:21.000000 PM3-0.3.9/screenshots/systemd_script.png
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)       38 2022-06-26 22:04:50.052103 PM3-0.3.9/setup.cfg
+-rw-rw-r--   0 ilario    (1000) ilario    (1000)     1019 2022-06-26 22:04:36.000000 PM3-0.3.9/setup.py
+-rwxr-xr-x   0 ilario    (1000) ilario    (1000)       40 2021-12-29 16:50:20.000000 PM3-0.3.9/upload.sh
```

### Comparing `PM3-0.3.8/.gitignore` & `PM3-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/LICENSE` & `PM3-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/PKG-INFO` & `PM3-0.3.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-Metadata-Version: 2.1
-Name: PM3
-Version: 0.3.8
-Summary: Like pm2 without node.js ;-)
-Home-page: https://github.com/ilariofebi/PM3.git 
-Author: Ilario Febi
-Author-email: ilario@febi.biz
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PM3
 Like pm2 without node.js ;-)
 ![](https://github.com/ilariofebi/PM3/blob/main/screenshots/ls.png?raw=true)
 # PM3 CheatSheet:
 ### Install and update
+Build a [virtualenv](https://docs.python.org/3.9/tutorial/venv.html) environment (recommended)
+```
+python3.9 -m venv PM3venv
+. PM3venv/bin/activate
+```
+Then:
 ```
 pip install pm3             # Install pm3
 pip install -U pm3          # Upgrade pm3
 ```
 
 ### Start
 ```
```

### Comparing `PM3-0.3.8/PM3/app.py` & `PM3-0.3.9/PM3/app.py`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/PM3/cli.py` & `PM3-0.3.9/PM3/cli.py`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/PM3/cron_checker.py` & `PM3-0.3.9/PM3/cron_checker.py`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/PM3/libs/pm3table.py` & `PM3-0.3.9/PM3/libs/pm3table.py`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/PM3/libs/system_scripts.py` & `PM3-0.3.9/PM3/libs/system_scripts.py`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/PM3/model/process.py` & `PM3-0.3.9/PM3/model/process.py`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/PM3.egg-info/PKG-INFO` & `PM3-0.3.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PM3
-Version: 0.3.8
+Version: 0.3.9
 Summary: Like pm2 without node.js ;-)
 Home-page: https://github.com/ilariofebi/PM3.git 
 Author: Ilario Febi
 Author-email: ilario@febi.biz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
@@ -13,14 +13,20 @@
 License-File: LICENSE
 
 # PM3
 Like pm2 without node.js ;-)
 ![](https://github.com/ilariofebi/PM3/blob/main/screenshots/ls.png?raw=true)
 # PM3 CheatSheet:
 ### Install and update
+Build a [virtualenv](https://docs.python.org/3.9/tutorial/venv.html) environment (recommended)
+```
+python3.9 -m venv PM3venv
+. PM3venv/bin/activate
+```
+Then:
 ```
 pip install pm3             # Install pm3
 pip install -U pm3          # Upgrade pm3
 ```
 
 ### Start
 ```
```

### Comparing `PM3-0.3.8/PM3.egg-info/SOURCES.txt` & `PM3-0.3.9/PM3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/README.md` & `PM3-0.3.9/PM3.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,32 @@
+Metadata-Version: 2.1
+Name: PM3
+Version: 0.3.9
+Summary: Like pm2 without node.js ;-)
+Home-page: https://github.com/ilariofebi/PM3.git 
+Author: Ilario Febi
+Author-email: ilario@febi.biz
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PM3
 Like pm2 without node.js ;-)
 ![](https://github.com/ilariofebi/PM3/blob/main/screenshots/ls.png?raw=true)
 # PM3 CheatSheet:
 ### Install and update
+Build a [virtualenv](https://docs.python.org/3.9/tutorial/venv.html) environment (recommended)
+```
+python3.9 -m venv PM3venv
+. PM3venv/bin/activate
+```
+Then:
 ```
 pip install pm3             # Install pm3
 pip install -U pm3          # Upgrade pm3
 ```
 
 ### Start
 ```
```

### Comparing `PM3-0.3.8/screenshots/dump.png` & `PM3-0.3.9/screenshots/dump.png`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/screenshots/help.png` & `PM3-0.3.9/screenshots/help.png`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/screenshots/ls.png` & `PM3-0.3.9/screenshots/ls.png`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/screenshots/new_help.png` & `PM3-0.3.9/screenshots/new_help.png`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/screenshots/ps.png` & `PM3-0.3.9/screenshots/ps.png`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/screenshots/systemd_script.png` & `PM3-0.3.9/screenshots/systemd_script.png`

 * *Files identical despite different names*

### Comparing `PM3-0.3.8/setup.py` & `PM3-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     install_req_list = fh.read().split('\n')
 
 setuptools.setup(
     name="PM3",
-    version="0.3.8",
+    version="0.3.9",
     author="Ilario Febi",
     author_email="ilario@febi.biz",
     description="Like pm2 without node.js ;-)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ilariofebi/PM3.git ",
     # packages=setuptools.find_packages(),
```

