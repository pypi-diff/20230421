# Comparing `tmp/xinlan-tools-0.0.1.tar.gz` & `tmp/xinlan-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinlan-tools-0.0.1.tar", last modified: Thu Apr 20 11:07:32 2023, max compression
+gzip compressed data, was "xinlan-tools-0.0.2.tar", last modified: Fri Apr 21 11:44:11 2023, max compression
```

## Comparing `xinlan-tools-0.0.1.tar` & `xinlan-tools-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-20 11:07:32.263458 xinlan-tools-0.0.1/
--rw-r--r--   0 superfan   (501) staff       (20)     1065 2023-04-20 06:47:45.000000 xinlan-tools-0.0.1/LICENSE
--rw-r--r--   0 superfan   (501) staff       (20)     1919 2023-04-20 11:07:32.263172 xinlan-tools-0.0.1/PKG-INFO
--rw-r--r--   0 superfan   (501) staff       (20)        0 2023-04-20 06:39:20.000000 xinlan-tools-0.0.1/README.md
--rw-r--r--   0 superfan   (501) staff       (20)      885 2023-04-20 09:51:45.000000 xinlan-tools-0.0.1/pyproject.toml
--rw-r--r--   0 superfan   (501) staff       (20)       38 2023-04-20 11:07:32.263553 xinlan-tools-0.0.1/setup.cfg
-drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-20 11:07:32.257232 xinlan-tools-0.0.1/src/
-drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-20 11:07:32.259850 xinlan-tools-0.0.1/src/tools/
--rw-r--r--   0 superfan   (501) staff       (20)      220 2023-04-20 09:49:08.000000 xinlan-tools-0.0.1/src/tools/__init__.py
--rw-r--r--   0 superfan   (501) staff       (20)     1879 2023-04-20 09:18:50.000000 xinlan-tools-0.0.1/src/tools/base.py
-drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-20 11:07:32.261317 xinlan-tools-0.0.1/src/tools/commands/
--rw-r--r--   0 superfan   (501) staff       (20)      148 2023-04-20 09:20:43.000000 xinlan-tools-0.0.1/src/tools/commands/__init__.py
--rw-r--r--   0 superfan   (501) staff       (20)     1701 2023-04-20 11:07:17.000000 xinlan-tools-0.0.1/src/tools/commands/encrypt.py
--rw-r--r--   0 superfan   (501) staff       (20)     1319 2023-04-20 09:53:33.000000 xinlan-tools-0.0.1/src/tools/core.py
-drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-20 11:07:32.262800 xinlan-tools-0.0.1/src/xinlan_tools.egg-info/
--rw-r--r--   0 superfan   (501) staff       (20)     1919 2023-04-20 11:07:32.000000 xinlan-tools-0.0.1/src/xinlan_tools.egg-info/PKG-INFO
--rw-r--r--   0 superfan   (501) staff       (20)      354 2023-04-20 11:07:32.000000 xinlan-tools-0.0.1/src/xinlan_tools.egg-info/SOURCES.txt
--rw-r--r--   0 superfan   (501) staff       (20)        1 2023-04-20 11:07:32.000000 xinlan-tools-0.0.1/src/xinlan_tools.egg-info/dependency_links.txt
--rw-r--r--   0 superfan   (501) staff       (20)       38 2023-04-20 11:07:32.000000 xinlan-tools-0.0.1/src/xinlan_tools.egg-info/entry_points.txt
--rw-r--r--   0 superfan   (501) staff       (20)        6 2023-04-20 11:07:32.000000 xinlan-tools-0.0.1/src/xinlan_tools.egg-info/top_level.txt
+drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-21 11:44:11.771033 xinlan-tools-0.0.2/
+-rw-r--r--   0 superfan   (501) staff       (20)     1065 2023-04-20 06:47:45.000000 xinlan-tools-0.0.2/LICENSE
+-rw-r--r--   0 superfan   (501) staff       (20)     2529 2023-04-21 11:44:11.770573 xinlan-tools-0.0.2/PKG-INFO
+-rw-r--r--   0 superfan   (501) staff       (20)      608 2023-04-21 11:39:59.000000 xinlan-tools-0.0.2/README.md
+-rw-r--r--   0 superfan   (501) staff       (20)      896 2023-04-21 11:44:01.000000 xinlan-tools-0.0.2/pyproject.toml
+-rw-r--r--   0 superfan   (501) staff       (20)       38 2023-04-21 11:44:11.771221 xinlan-tools-0.0.2/setup.cfg
+drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-21 11:44:11.761927 xinlan-tools-0.0.2/src/
+drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-21 11:44:11.764623 xinlan-tools-0.0.2/src/tools/
+-rw-r--r--   0 superfan   (501) staff       (20)      220 2023-04-20 09:49:08.000000 xinlan-tools-0.0.2/src/tools/__init__.py
+-rw-r--r--   0 superfan   (501) staff       (20)     1879 2023-04-20 09:18:50.000000 xinlan-tools-0.0.2/src/tools/base.py
+drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-21 11:44:11.767103 xinlan-tools-0.0.2/src/tools/commands/
+-rw-r--r--   0 superfan   (501) staff       (20)      148 2023-04-20 09:20:43.000000 xinlan-tools-0.0.2/src/tools/commands/__init__.py
+-rw-r--r--   0 superfan   (501) staff       (20)     1096 2023-04-21 11:19:43.000000 xinlan-tools-0.0.2/src/tools/commands/convert.py
+-rw-r--r--   0 superfan   (501) staff       (20)     1701 2023-04-20 11:07:17.000000 xinlan-tools-0.0.2/src/tools/commands/encrypt.py
+-rw-r--r--   0 superfan   (501) staff       (20)     1436 2023-04-21 09:14:27.000000 xinlan-tools-0.0.2/src/tools/core.py
+drwxr-xr-x   0 superfan   (501) staff       (20)        0 2023-04-21 11:44:11.769727 xinlan-tools-0.0.2/src/xinlan_tools.egg-info/
+-rw-r--r--   0 superfan   (501) staff       (20)     2529 2023-04-21 11:44:11.000000 xinlan-tools-0.0.2/src/xinlan_tools.egg-info/PKG-INFO
+-rw-r--r--   0 superfan   (501) staff       (20)      423 2023-04-21 11:44:11.000000 xinlan-tools-0.0.2/src/xinlan_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 superfan   (501) staff       (20)        1 2023-04-21 11:44:11.000000 xinlan-tools-0.0.2/src/xinlan_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 superfan   (501) staff       (20)       38 2023-04-21 11:44:11.000000 xinlan-tools-0.0.2/src/xinlan_tools.egg-info/entry_points.txt
+-rw-r--r--   0 superfan   (501) staff       (20)        7 2023-04-21 11:44:11.000000 xinlan-tools-0.0.2/src/xinlan_tools.egg-info/requires.txt
+-rw-r--r--   0 superfan   (501) staff       (20)        6 2023-04-21 11:44:11.000000 xinlan-tools-0.0.2/src/xinlan_tools.egg-info/top_level.txt
```

### Comparing `xinlan-tools-0.0.1/LICENSE` & `xinlan-tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xinlan-tools-0.0.1/pyproject.toml` & `xinlan-tools-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xinlan-tools"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="xinlan", email="117220100@qq.com" },
 ]
 description = "python开发的实用小工具"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
@@ -28,10 +28,11 @@
 ]
 
 # [project.urls]
 # "Homepage" = "http"
 # "Bug Tracker" = ""
 
 dependencies = [
+  "pillow"
 ]
 [project.scripts]
 tools="tools:tools"
```

### Comparing `xinlan-tools-0.0.1/src/tools/base.py` & `xinlan-tools-0.0.2/src/tools/base.py`

 * *Files identical despite different names*

### Comparing `xinlan-tools-0.0.1/src/tools/commands/encrypt.py` & `xinlan-tools-0.0.2/src/tools/commands/encrypt.py`

 * *Files identical despite different names*

### Comparing `xinlan-tools-0.0.1/src/tools/core.py` & `xinlan-tools-0.0.2/src/tools/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,17 @@
         else:
             self.args = vars(parser.parse_args())
 
     def fetch_command(self, subcommand):
         if subcommand == 'encrypt':
             from .commands.encrypt import Command
             return Command()
+        elif subcommand == 'convert':
+            from .commands.convert import Command
+            return Command()
 
     def execute(self):
         try:
             subcommand = self.args[0]
         except IndexError:
             subcommand = 'help'
```

