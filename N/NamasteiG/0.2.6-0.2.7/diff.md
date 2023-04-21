# Comparing `tmp/NamasteiG-0.2.6.tar.gz` & `tmp/NamasteiG-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NamasteiG-0.2.6.tar", last modified: Fri Apr 21 14:15:13 2023, max compression
+gzip compressed data, was "NamasteiG-0.2.7.tar", last modified: Fri Apr 21 14:22:51 2023, max compression
```

## Comparing `NamasteiG-0.2.6.tar` & `NamasteiG-0.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.330563 NamasteiG-0.2.6/
--rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      838 2023-04-21 14:15:13.330563 NamasteiG-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.6/README.md
--rw-rw-rw-   0        0        0      593 2023-04-21 14:10:11.000000 NamasteiG-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 14:15:13.332038 NamasteiG-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.317646 NamasteiG-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.325092 NamasteiG-0.2.6/src/NamasteiG/
--rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.2.6/src/NamasteiG/VerifyData.py
--rw-rw-rw-   0        0        0    27820 2023-04-21 14:14:36.000000 NamasteiG-0.2.6/src/NamasteiG/__init__.py
--rw-rw-rw-   0        0        0      501 2023-04-21 14:14:22.000000 NamasteiG-0.2.6/src/NamasteiG/example.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:15:13.329144 NamasteiG-0.2.6/src/NamasteiG.egg-info/
--rw-rw-rw-   0        0        0      838 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-21 14:15:13.000000 NamasteiG-0.2.6/src/NamasteiG.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:22:51.177653 NamasteiG-0.2.7/
+-rw-rw-rw-   0        0        0     1077 2022-12-10 14:24:59.000000 NamasteiG-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      838 2023-04-21 14:22:51.177653 NamasteiG-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2022-12-14 19:04:09.000000 NamasteiG-0.2.7/README.md
+-rw-rw-rw-   0        0        0      593 2023-04-21 14:22:28.000000 NamasteiG-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:22:51.177653 NamasteiG-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 14:22:51.163125 NamasteiG-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:22:51.164635 NamasteiG-0.2.7/src/NamasteiG/
+-rw-rw-rw-   0        0        0     8405 2023-04-16 13:01:55.000000 NamasteiG-0.2.7/src/NamasteiG/VerifyData.py
+-rw-rw-rw-   0        0        0    27786 2023-04-21 14:22:28.000000 NamasteiG-0.2.7/src/NamasteiG/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-04-21 14:20:43.000000 NamasteiG-0.2.7/src/NamasteiG/example.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:22:51.164635 NamasteiG-0.2.7/src/NamasteiG.egg-info/
+-rw-rw-rw-   0        0        0      838 2023-04-21 14:22:51.000000 NamasteiG-0.2.7/src/NamasteiG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-21 14:22:51.000000 NamasteiG-0.2.7/src/NamasteiG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:22:51.000000 NamasteiG-0.2.7/src/NamasteiG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 14:22:51.000000 NamasteiG-0.2.7/src/NamasteiG.egg-info/top_level.txt
```

### Comparing `NamasteiG-0.2.6/LICENSE` & `NamasteiG-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.6/PKG-INFO` & `NamasteiG-0.2.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.6
+Version: 0.2.7
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NamasteiG-0.2.6/pyproject.toml` & `NamasteiG-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NamasteiG"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Abhinav Bhardwaj", email="abhinav.bhardwaj.56614@gmail.com" },
 ]
 description = "Most PowerFull Instagram Library"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `NamasteiG-0.2.6/src/NamasteiG/VerifyData.py` & `NamasteiG-0.2.7/src/NamasteiG/VerifyData.py`

 * *Files identical despite different names*

### Comparing `NamasteiG-0.2.6/src/NamasteiG/__init__.py` & `NamasteiG-0.2.7/src/NamasteiG/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,14 @@
                         'igrur': self.igrur,
                         'Xclaim': self.xclaim,
                         'BearerToken': self.bearer,
                         'igid': self.igid,
                         'UserId':self.userid
                     }
                     self.sessionid=self.bearer
-                    print(value)
 
 
                     return value
 
 
                 elif 'challenge_required' in response.text:
                     value = {
```

### Comparing `NamasteiG-0.2.6/src/NamasteiG.egg-info/PKG-INFO` & `NamasteiG-0.2.7/src/NamasteiG.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NamasteiG
-Version: 0.2.6
+Version: 0.2.7
 Summary: Most PowerFull Instagram Library
 Author-email: Abhinav Bhardwaj <abhinav.bhardwaj.56614@gmail.com>
 Project-URL: Homepage, https://t.me/namastelibrary
 Project-URL: Bug Tracker, https://t.me/namastehackers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

