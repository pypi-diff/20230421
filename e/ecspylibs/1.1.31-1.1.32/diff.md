# Comparing `tmp/ecspylibs-1.1.31.tar.gz` & `tmp/ecspylibs-1.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecspylibs-1.1.31.tar", max compression
+gzip compressed data, was "ecspylibs-1.1.32.tar", max compression
```

## Comparing `ecspylibs-1.1.31.tar` & `ecspylibs-1.1.32.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     9274 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/ChangeLog
--rw-r--r--   0        0        0     1075 2020-11-06 03:34:20.305134 ecspylibs-1.1.31/LICENSE.txt
--rw-r--r--   0        0        0     1537 2023-03-23 22:13:42.045610 ecspylibs-1.1.31/README.md
--rw-r--r--   0        0        0     1917 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/pyproject.toml
--rw-r--r--   0        0        0      465 2023-02-08 23:25:52.618443 ecspylibs-1.1.31/src/ecspylibs/__init__.py
--rw-r--r--   0        0        0     2623 2023-02-20 21:12:06.796621 ecspylibs-1.1.31/src/ecspylibs/buildfunctionlist.py
--rw-r--r--   0        0        0     8433 2023-02-20 21:12:06.796621 ecspylibs-1.1.31/src/ecspylibs/checkservice.py
--rw-r--r--   0        0        0     3107 2023-02-20 21:12:06.796621 ecspylibs-1.1.31/src/ecspylibs/cleanuptempdirs.py
--rw-r--r--   0        0        0     8051 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/src/ecspylibs/configfile.py
--rw-r--r--   0        0        0     3502 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/src/ecspylibs/initsetup.py
--rw-r--r--   0        0        0     1626 2023-04-13 20:37:00.519802 ecspylibs-1.1.31/src/ecspylibs/parallel.py
--rw-r--r--   0        0        0     5036 2023-02-20 21:12:06.797621 ecspylibs-1.1.31/src/ecspylibs/parseemail.py
--rw-r--r--   0        0        0     3739 2023-02-20 21:12:06.797621 ecspylibs-1.1.31/src/ecspylibs/parsexml.py
--rw-r--r--   0        0        0     3797 2023-02-21 17:11:02.916128 ecspylibs-1.1.31/src/ecspylibs/password.py
--rw-r--r--   0        0        0     1816 2023-02-20 21:58:09.629999 ecspylibs-1.1.31/src/ecspylibs/reapchildren.py
--rw-r--r--   0        0        0     3279 2023-02-20 21:12:06.797621 ecspylibs-1.1.31/src/ecspylibs/sendemail.py
--rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 ecspylibs-1.1.31/setup.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 ecspylibs-1.1.31/PKG-INFO
+-rw-r--r--   0        0        0     9554 2023-04-21 20:20:10.579476 ecspylibs-1.1.32/ChangeLog
+-rw-r--r--   0        0        0     1075 2020-11-06 03:34:20.305134 ecspylibs-1.1.32/LICENSE.txt
+-rw-r--r--   0        0        0     1537 2023-03-23 22:13:42.045610 ecspylibs-1.1.32/README.md
+-rw-r--r--   0        0        0     1917 2023-04-21 20:20:10.579476 ecspylibs-1.1.32/pyproject.toml
+-rw-r--r--   0        0        0      465 2023-02-08 23:25:52.618443 ecspylibs-1.1.32/src/ecspylibs/__init__.py
+-rw-r--r--   0        0        0     2658 2023-04-21 20:18:07.292356 ecspylibs-1.1.32/src/ecspylibs/buildfunctionlist.py
+-rw-r--r--   0        0        0     8433 2023-02-20 21:12:06.796621 ecspylibs-1.1.32/src/ecspylibs/checkservice.py
+-rw-r--r--   0        0        0     3107 2023-02-20 21:12:06.796621 ecspylibs-1.1.32/src/ecspylibs/cleanuptempdirs.py
+-rw-r--r--   0        0        0     8051 2023-04-13 20:37:00.519802 ecspylibs-1.1.32/src/ecspylibs/configfile.py
+-rw-r--r--   0        0        0     3502 2023-04-13 20:37:00.519802 ecspylibs-1.1.32/src/ecspylibs/initsetup.py
+-rw-r--r--   0        0        0     1654 2023-04-21 20:18:07.292356 ecspylibs-1.1.32/src/ecspylibs/parallel.py
+-rw-r--r--   0        0        0     5036 2023-02-20 21:12:06.797621 ecspylibs-1.1.32/src/ecspylibs/parseemail.py
+-rw-r--r--   0        0        0     3739 2023-02-20 21:12:06.797621 ecspylibs-1.1.32/src/ecspylibs/parsexml.py
+-rw-r--r--   0        0        0     3797 2023-02-21 17:11:02.916128 ecspylibs-1.1.32/src/ecspylibs/password.py
+-rw-r--r--   0        0        0     1816 2023-02-20 21:58:09.629999 ecspylibs-1.1.32/src/ecspylibs/reapchildren.py
+-rw-r--r--   0        0        0     3279 2023-02-20 21:12:06.797621 ecspylibs-1.1.32/src/ecspylibs/sendemail.py
+-rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 ecspylibs-1.1.32/setup.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 ecspylibs-1.1.32/PKG-INFO
```

### Comparing `ecspylibs-1.1.31/ChangeLog` & `ecspylibs-1.1.32/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+2023-04-21  Thomas R. Stevenson  <tom@tom.cc.wayne.edu>
+
+	* pyproject.toml: Update to version v1.1.32.
+
+	* src/ecspylibs/parallel.py (Parallel.__post_init__): Initialize
+	self.results.
+
+	* src/ecspylibs/buildfunctionlist.py (BuildFunctionList.__init__):
+	Fixed some minor typos.
+
 2023-04-13  Thomas R. Stevenson  <tom@tom.cc.wayne.edu>
 
 	* pyproject.toml: Update version to v1.1.31.
 
 	* src/ecspylibs/parallel.py (Parallel.run): Change self.arguments
 	into arguments.
```

### Comparing `ecspylibs-1.1.31/LICENSE.txt` & `ecspylibs-1.1.32/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/README.md` & `ecspylibs-1.1.32/README.md`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/pyproject.toml` & `ecspylibs-1.1.32/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 #
 # Do NOT edit this system file by hand -- use git.
 # See "URL to git source" below.
 #
 # Author:        $Id: Thomas R. Stevenson <aa0026@wayne.edu> $
 #
-# Last Changed:  $Date: Fri Mar 31 11:16:03 2023 -0400 $
+# Last Changed:  $Date: Fri Apr 21 16:19:50 2023 -0400 $
 #
 # URL to git source: $URL: git@git.wayne.edu:ECS_Projects/ECSpylibs.git $
 #
 [tool.poetry]
 name = "ecspylibs"
-version = "v1.1.31"
+version = "v1.1.32"
 packages = [{include = "ecspylibs", from = "src"}]
 description = "Local python libraries used across multiple programs."
 license = "GPL-3.0-or-later"
 authors = ["Thomas R. Stevenson <aa0026@wayne.edu>"]
 maintainers = ["Thomas R. Stevenson <aa0026@wayne.edu>"]
 readme = "README.md"
 homepage = "https://git.wayne.edu/ECS_Projects/ECSpylibs.git"
```

### Comparing `ecspylibs-1.1.31/src/ecspylibs/buildfunctionlist.py` & `ecspylibs-1.1.32/src/ecspylibs/buildfunctionlist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 # Do NOT edit this system file by hand -- use git.  See "URL to git source" below.
 #
 # Author:        $Id: Thomas R. Stevenson <aa0026@wayne.edu> $
 #
-# Last Changed:  $Date: Fri Feb 17 12:47:46 2023 -0500 $
+# Last Changed:  $Date: Fri Apr 21 16:17:46 2023 -0400 $
 #
 # URL to git source: $URL: git@git.wayne.edu:ECS_Projects/ECSpylibs.git $
 #
 
 # Futuristic implementation of commands.  Must be first from/import
 # command.
 
@@ -29,22 +29,23 @@
 @logged
 class BuildFunctionList:
     """Validate and call an internal function given the function name as a string."""
 
     def __init__(self, default_command_prefix: object = "function") -> None:
         """Set default function name prefix."""
 
+        self.function_name = None
         self.default_command_prefix = default_command_prefix
         self.program_errors = False
         self.xml_file_errors = False
 
     def call(self, function_name: object, function_args: object, command_prefix: object = None) -> object:
-        """Validate and call an internal funtion given the function name as a string."""
+        """Validate and call an internal function given the function name as a string."""
 
-        if command_prefix == None:
+        if command_prefix is None:
             self.function_name = "%s__%s" % (self.default_command_prefix, function_name,)
         else:
             self.function_name = "%s__%s" % (command_prefix, function_name,)
 
         self.__log.debug("Validating function : %s", self.function_name)
 
         if self.__class__.__dict__.get(self.function_name):
```

### Comparing `ecspylibs-1.1.31/src/ecspylibs/checkservice.py` & `ecspylibs-1.1.32/src/ecspylibs/checkservice.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/cleanuptempdirs.py` & `ecspylibs-1.1.32/src/ecspylibs/cleanuptempdirs.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/configfile.py` & `ecspylibs-1.1.32/src/ecspylibs/configfile.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/initsetup.py` & `ecspylibs-1.1.32/src/ecspylibs/initsetup.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/parallel.py` & `ecspylibs-1.1.32/src/ecspylibs/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 #
 # Do NOT edit this system file by hand -- use git.
 # See "URL to git source" below.
 #
 # Author:        $Id: Thomas R. Stevenson <aa0026@wayne.edu> $
 #
-# Last Changed:  $Date: Tue Feb 21 12:10:36 2023 -0500 $
+# Last Changed:  $Date: Fri Apr 21 16:17:46 2023 -0400 $
 #
 # URL to git source: $URL: git@git.wayne.edu:ECS_Projects/ECSpylibs.git $
 #
 
 """
 blah
 """
@@ -36,14 +36,15 @@
         """
         Blah
         """
 
         self.run_time = None
         self.results = None
         self.arguments = None
+        self.results = None
 
         if self.pool_size:
             if isinstance(self.pool_size, int) or self.pool_size.isnumeric():
                 self.pool_size = int(self.pool_size)
             else:
                 self.pool_size = None
         else:
```

### Comparing `ecspylibs-1.1.31/src/ecspylibs/parseemail.py` & `ecspylibs-1.1.32/src/ecspylibs/parseemail.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/parsexml.py` & `ecspylibs-1.1.32/src/ecspylibs/parsexml.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/password.py` & `ecspylibs-1.1.32/src/ecspylibs/password.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/reapchildren.py` & `ecspylibs-1.1.32/src/ecspylibs/reapchildren.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/src/ecspylibs/sendemail.py` & `ecspylibs-1.1.32/src/ecspylibs/sendemail.py`

 * *Files identical despite different names*

### Comparing `ecspylibs-1.1.31/setup.py` & `ecspylibs-1.1.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'requests>=2.28.2,<3.0.0',
  'toml>=0.10.2,<0.11.0',
  'urllib3>=1.26.15,<2.0.0',
  'xlrd==1.2.0']
 
 setup_kwargs = {
     'name': 'ecspylibs',
-    'version': '1.1.31',
+    'version': '1.1.32',
     'description': 'Local python libraries used across multiple programs.',
     'long_description': '# ECSpylibs\n\n# Package files\n    -rw-r--r--. 1 tom tom 2568 Feb  2 13:57 src/ecspylibs/buildfunctionlist.py\n    -rw-r--r--. 1 tom tom 8390 Feb  2 13:57 src/ecspylibs/checkservice.py\n    -rw-r--r--. 1 tom tom 3090 Feb  2 13:57 src/ecspylibs/cleanuptempdirs.py\n    -rw-r--r--. 1 tom tom 6123 Mar 16 17:03 src/ecspylibs/configfile.py\n    -rw-r--r--. 1 tom tom  465 Jan 26 11:05 src/ecspylibs/__init__.py\n    -rw-r--r--. 1 tom tom 3678 Feb  2 13:57 src/ecspylibs/initsetup.py\n    -rw-r--r--. 1 tom tom 1676 Feb  8 12:50 src/ecspylibs/parallel.py\n    -rw-r--r--. 1 tom tom 4965 Feb  2 13:57 src/ecspylibs/parseemail.py\n    -rw-r--r--. 1 tom tom 3644 Feb  2 13:57 src/ecspylibs/parsexml.py\n    -rw-r--r--. 1 tom tom 3650 Feb  2 13:57 src/ecspylibs/password.py\n    -rw-r--r--. 1 tom tom 1879 Feb  2 13:57 src/ecspylibs/reapchildren.py\n    -rw-r--r--. 1 tom tom 2993 Feb  2 13:57 src/ecspylibs/sendemail.py\n\n# Git information\n[GIT Home][ECSPYLIBS],\n[README File][README],\n[LICENSE File][LICENSE],\n[ChangeLog File][CHANGELOG],\n[pyproject.toml File][PYPROJECT].\n\n# About Me\n[My contact information][About Me].\n\n[ECSPYLIBS]: https://git.wayne.edu/ECS_Projects/ECSpylibs\n[README]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/README.md\n[LICENSE]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/LICENSE.txt\n[CHANGELOG]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/ChangeLog\n[PYPROJECT]: https://git.wayne.edu/ECS_Projects/ECSpylibs/-/blob/master/pyproject.toml\n[About Me]: https://About.Me/Thomas.R.Stevenson\n',
     'author': 'Thomas R. Stevenson',
     'author_email': 'aa0026@wayne.edu',
     'maintainer': 'Thomas R. Stevenson',
     'maintainer_email': 'aa0026@wayne.edu',
     'url': 'https://git.wayne.edu/ECS_Projects/ECSpylibs.git',
```

### Comparing `ecspylibs-1.1.31/PKG-INFO` & `ecspylibs-1.1.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecspylibs
-Version: 1.1.31
+Version: 1.1.32
 Summary: Local python libraries used across multiple programs.
 Home-page: https://git.wayne.edu/ECS_Projects/ECSpylibs.git
 License: GPL-3.0-or-later
 Keywords: buildfunctionlist,checkservice,cleanuptempdirs,initsetup,parallel,parseemail,parsexml,password,reapchildren,sendemail
 Author: Thomas R. Stevenson
 Author-email: aa0026@wayne.edu
 Maintainer: Thomas R. Stevenson
```

