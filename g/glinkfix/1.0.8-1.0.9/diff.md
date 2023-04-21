# Comparing `tmp/glinkfix-1.0.8.tar.gz` & `tmp/glinkfix-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glinkfix-1.0.8.tar", last modified: Sat Jul 23 11:29:40 2022, max compression
+gzip compressed data, was "glinkfix-1.0.9.tar", last modified: Thu Oct 13 21:42:46 2022, max compression
```

## Comparing `glinkfix-1.0.8.tar` & `glinkfix-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-07-23 11:29:40.434143 glinkfix-1.0.8/
--rw-rw-r--   0 nardi     (1000) nardi     (1000)     1075 2022-06-25 18:02:06.000000 glinkfix-1.0.8/LICENSE
--rw-rw-r--   0 nardi     (1000) nardi     (1000)       16 2022-06-25 18:02:06.000000 glinkfix-1.0.8/MANIFEST.in
--rw-rw-r--   0 nardi     (1000) nardi     (1000)     5088 2022-07-23 11:29:40.434143 glinkfix-1.0.8/PKG-INFO
--rw-rw-r--   0 nardi     (1000) nardi     (1000)     3922 2022-07-23 11:24:58.000000 glinkfix-1.0.8/README.md
--rw-rw-r--   0 nardi     (1000) nardi     (1000)      168 2022-07-17 23:43:00.000000 glinkfix-1.0.8/pyproject.toml
--rw-rw-r--   0 nardi     (1000) nardi     (1000)     1739 2022-07-23 11:29:40.434143 glinkfix-1.0.8/setup.cfg
--rw-rw-r--   0 nardi     (1000) nardi     (1000)       83 2022-06-25 18:02:06.000000 glinkfix-1.0.8/setup.py
-drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-07-23 11:29:40.430142 glinkfix-1.0.8/src/
-drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-07-23 11:29:40.434143 glinkfix-1.0.8/src/glinkfix/
--rw-rw-r--   0 nardi     (1000) nardi     (1000)       50 2022-07-21 20:29:08.000000 glinkfix-1.0.8/src/glinkfix/__init__.py
--rwxrwxr-x   0 nardi     (1000) nardi     (1000)     1291 2022-07-21 20:29:08.000000 glinkfix-1.0.8/src/glinkfix/__main__.py
--rw-rw-r--   0 nardi     (1000) nardi     (1000)     2347 2022-07-22 20:27:17.000000 glinkfix-1.0.8/src/glinkfix/tools.py
-drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-07-23 11:29:40.434143 glinkfix-1.0.8/src/glinkfix.egg-info/
--rw-rw-r--   0 nardi     (1000) nardi     (1000)     5088 2022-07-23 11:29:40.000000 glinkfix-1.0.8/src/glinkfix.egg-info/PKG-INFO
--rw-rw-r--   0 nardi     (1000) nardi     (1000)      318 2022-07-23 11:29:40.000000 glinkfix-1.0.8/src/glinkfix.egg-info/SOURCES.txt
--rw-rw-r--   0 nardi     (1000) nardi     (1000)        1 2022-07-23 11:29:40.000000 glinkfix-1.0.8/src/glinkfix.egg-info/dependency_links.txt
--rw-rw-r--   0 nardi     (1000) nardi     (1000)       52 2022-07-23 11:29:40.000000 glinkfix-1.0.8/src/glinkfix.egg-info/entry_points.txt
--rw-rw-r--   0 nardi     (1000) nardi     (1000)        9 2022-07-23 11:29:40.000000 glinkfix-1.0.8/src/glinkfix.egg-info/top_level.txt
+drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-10-13 21:42:46.189338 glinkfix-1.0.9/
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)     1075 2022-10-13 21:00:43.000000 glinkfix-1.0.9/LICENSE
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)       16 2022-10-13 21:00:43.000000 glinkfix-1.0.9/MANIFEST.in
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)     5354 2022-10-13 21:42:46.189338 glinkfix-1.0.9/PKG-INFO
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)     4188 2022-10-13 21:27:50.000000 glinkfix-1.0.9/README.md
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)      168 2022-10-13 21:00:43.000000 glinkfix-1.0.9/pyproject.toml
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)     1739 2022-10-13 21:42:46.193338 glinkfix-1.0.9/setup.cfg
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)       83 2022-10-13 21:00:43.000000 glinkfix-1.0.9/setup.py
+drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-10-13 21:42:46.189338 glinkfix-1.0.9/src/
+drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-10-13 21:42:46.189338 glinkfix-1.0.9/src/glinkfix/
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)       22 2022-10-13 21:40:58.000000 glinkfix-1.0.9/src/glinkfix/__init__.py
+-rwxrwxr-x   0 nardi     (1000) nardi     (1000)     1308 2022-10-13 21:40:58.000000 glinkfix-1.0.9/src/glinkfix/__main__.py
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)     2421 2022-10-13 21:26:07.000000 glinkfix-1.0.9/src/glinkfix/tools.py
+drwxrwxr-x   0 nardi     (1000) nardi     (1000)        0 2022-10-13 21:42:46.189338 glinkfix-1.0.9/src/glinkfix.egg-info/
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)     5354 2022-10-13 21:42:46.000000 glinkfix-1.0.9/src/glinkfix.egg-info/PKG-INFO
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)      318 2022-10-13 21:42:46.000000 glinkfix-1.0.9/src/glinkfix.egg-info/SOURCES.txt
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)        1 2022-10-13 21:42:46.000000 glinkfix-1.0.9/src/glinkfix.egg-info/dependency_links.txt
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)       52 2022-10-13 21:42:46.000000 glinkfix-1.0.9/src/glinkfix.egg-info/entry_points.txt
+-rw-rw-r--   0 nardi     (1000) nardi     (1000)        9 2022-10-13 21:42:46.000000 glinkfix-1.0.9/src/glinkfix.egg-info/top_level.txt
```

### Comparing `glinkfix-1.0.8/LICENSE` & `glinkfix-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glinkfix-1.0.8/PKG-INFO` & `glinkfix-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glinkfix
-Version: 1.0.8
+Version: 1.0.9
 Summary: Google Drive Link Fixer
 Home-page: https://github.com/geozeke/glinkfix
 Author: Peter Nardi
 Author-email: pete@nardi.com
 Maintainer: Peter Nardi
 Maintainer-email: pete@nardi.com
 License: MIT
@@ -95,14 +95,21 @@
 
 * There is a 40MB size limit for a single file when using Google Drive sharing links directly for viewing or downloading. Individual files larger than 40MB will not render/download properly. This limit is a function of how Google Drive works and is not related to `glinkfix`.
 * When creating a download link for use with `curl`, make sure to use `curl`'s `-L` option to allow for redirects.
 * `glinkfix` supports links that use Google's [resource key](https://support.google.com/a/answer/10685032) security feature.
 
 ## Version History
 
+* 1.0.9 (2022-10-13)
+  * Fixed a bug when IDs or resource keys contain underscore characters (`_`)
+  * Additional test case for bug fix.
+  * Moved task runner to make.
+  * Build local virtual environment for development.
+  * Code refactoring and linting.
+  <br><br>
 * 1.0.8 (2022-07-23)
   * Implemented code coverage for testing infrastructure.
   * Code refactoring and linting.
   <br><br>
 * 1.0.7 (2022-07-15)
   * Fixed handling of URLs with resource keys.
   * Code cleanup and refactoring.
```

### Comparing `glinkfix-1.0.8/README.md` & `glinkfix-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,14 +65,21 @@
 
 * There is a 40MB size limit for a single file when using Google Drive sharing links directly for viewing or downloading. Individual files larger than 40MB will not render/download properly. This limit is a function of how Google Drive works and is not related to `glinkfix`.
 * When creating a download link for use with `curl`, make sure to use `curl`'s `-L` option to allow for redirects.
 * `glinkfix` supports links that use Google's [resource key](https://support.google.com/a/answer/10685032) security feature.
 
 ## Version History
 
+* 1.0.9 (2022-10-13)
+  * Fixed a bug when IDs or resource keys contain underscore characters (`_`)
+  * Additional test case for bug fix.
+  * Moved task runner to make.
+  * Build local virtual environment for development.
+  * Code refactoring and linting.
+  <br><br>
 * 1.0.8 (2022-07-23)
   * Implemented code coverage for testing infrastructure.
   * Code refactoring and linting.
   <br><br>
 * 1.0.7 (2022-07-15)
   * Fixed handling of URLs with resource keys.
   * Code cleanup and refactoring.
```

### Comparing `glinkfix-1.0.8/setup.cfg` & `glinkfix-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.8
+current_version = 1.0.9
 
 [bumpversion:file:setup.cfg]
 search = {current_version}
 replace = {new_version}
 
 [bumpversion:file:version.txt]
 search = {current_version}
```

### Comparing `glinkfix-1.0.8/src/glinkfix/__main__.py` & `glinkfix-1.0.9/src/glinkfix/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python3
 
 """Main module."""
 
 import argparse
 
-from glinkfix import fixlink
+from glinkfix.tools import fix_link
 
 
-def main():
+def main() -> None:
     """Initiate link fixing.
 
     1. Generate an argument parser to collect command line input.
-    2. Call `fixlink` to perform link correction.
+    2. Call `fix_link` to perform link correction.
     """
     msg = """This program takes a Google Drive sharing link for a
     file and repackages it into a link that can be downloaded directly
     (e.g. using curl) or embedded in a document to be viewed (e.g. an
     image in a markdown document). Note: there is a size limit of 40MB
     for a single file when using Google Drive links in this manner."""
 
-    epi = "Version: 1.0.8"
+    epi = "Version: 1.0.9"
     parser = argparse.ArgumentParser(description=msg, epilog=epi)
     group = parser.add_mutually_exclusive_group(required=True)
 
     msg = """repackage the link for viewing (e.g. as an embedded
     link in a markdown document)."""
     group.add_argument('-v', '--view',
                        action='store_true',
@@ -32,13 +32,13 @@
     msg = """repackage the link for downloading (e.g. downloading
     using curl)."""
     group.add_argument('-d', '--download',
                        action='store_true',
                        help=msg)
 
     args = parser.parse_args()
-    fixlink(args)
+    fix_link(args)
     return
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `glinkfix-1.0.8/src/glinkfix/tools.py` & `glinkfix-1.0.9/src/glinkfix/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tools to perform link fixing."""
 
+import argparse
 import os
 import re
 
 
 class InvalidLinkError(Exception):
     """Custom exception for handling invalid sharing links.
 
@@ -26,65 +27,65 @@
         -------
         str
             The message string.
         """
         return self.message
 
 
-def clear():
+def clear() -> None:
     """Clear the screen.
 
     OS-agnostic version, which will work with both Windows and Linux.
     """
     os.system('clear' if os.name == 'posix' else 'cls')
 
 
-def fixlink(args):
+def fix_link(args: argparse.Namespace) -> None:
     """Fix malformed Google link.
 
     Prompt for a Google link to fix (usually entered by pasting into the
     terminal) and generate a corrected version.
 
     Parameters
     ----------
-    args : argparse
+    args : argparse.Namespace
         Command line arguments to determine how to prep the fixed link.
         If `-v` was selected (`args.view`) then prep the link for
         embedding into a file. If `-d` was selected (`args.download`)
         then prep the link for use with a download tool like `curl`.
     """
     clear()
 
     print('Enter a Google Drive sharing URL to be repackaged:\n')
-    oldlink = input()
+    old_link = input()
     resourcekey = None
     template = "https://drive.google.com/uc?export=ACTION&id=IDNUM"
     prefix = "https://drive.google.com/file/d/"
     suffix = "/view\\?usp=sharing"
 
-    parts = re.findall(rf'{prefix}([0-9A-Za-z-]*){suffix}', oldlink)
+    parts = re.findall(rf'{prefix}([0-9A-Za-z_-]*){suffix}', old_link)
     if len(parts) != 1:
-        raise(InvalidLinkError)
+        raise InvalidLinkError
     else:
         idstring = parts[0]
 
-    parts = re.findall(r'resourcekey=([0-9A-Za-z-]*)', oldlink)
+    parts = re.findall(r'resourcekey=([0-9A-Za-z_-]*)', old_link)
     if len(parts) == 1:
         resourcekey = parts[0]
 
     if args.view:
         action = template.replace('ACTION', 'view')
-        linkType = 'viewing'
+        link_type = 'viewing'
     else:
         action = template.replace('ACTION', 'download')
-        linkType = 'downloading'
+        link_type = 'downloading'
 
-    print(f'\nClean {linkType} URL is:\n')
-    newlink = action.replace("IDNUM", idstring)
+    print(f'\nClean {link_type} URL is:\n')
+    new_link = action.replace("IDNUM", idstring)
     if resourcekey:
-        newlink = f'{newlink}&resourcekey={resourcekey}'
-    print(f'{newlink}\n')
+        new_link = f'{new_link}&resourcekey={resourcekey}'
+    print(f'{new_link}\n')
     return
 
 
 if __name__ == '__main__':  # pragma no cover
     pass
```

### Comparing `glinkfix-1.0.8/src/glinkfix.egg-info/PKG-INFO` & `glinkfix-1.0.9/src/glinkfix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glinkfix
-Version: 1.0.8
+Version: 1.0.9
 Summary: Google Drive Link Fixer
 Home-page: https://github.com/geozeke/glinkfix
 Author: Peter Nardi
 Author-email: pete@nardi.com
 Maintainer: Peter Nardi
 Maintainer-email: pete@nardi.com
 License: MIT
@@ -95,14 +95,21 @@
 
 * There is a 40MB size limit for a single file when using Google Drive sharing links directly for viewing or downloading. Individual files larger than 40MB will not render/download properly. This limit is a function of how Google Drive works and is not related to `glinkfix`.
 * When creating a download link for use with `curl`, make sure to use `curl`'s `-L` option to allow for redirects.
 * `glinkfix` supports links that use Google's [resource key](https://support.google.com/a/answer/10685032) security feature.
 
 ## Version History
 
+* 1.0.9 (2022-10-13)
+  * Fixed a bug when IDs or resource keys contain underscore characters (`_`)
+  * Additional test case for bug fix.
+  * Moved task runner to make.
+  * Build local virtual environment for development.
+  * Code refactoring and linting.
+  <br><br>
 * 1.0.8 (2022-07-23)
   * Implemented code coverage for testing infrastructure.
   * Code refactoring and linting.
   <br><br>
 * 1.0.7 (2022-07-15)
   * Fixed handling of URLs with resource keys.
   * Code cleanup and refactoring.
```

