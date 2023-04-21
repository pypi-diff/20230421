# Comparing `tmp/uw-it-build-fingerprinter-0.2.7.tar.gz` & `tmp/uw-it-build-fingerprinter-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uw-it-build-fingerprinter-0.2.7.tar", max compression
+gzip compressed data, was "uw-it-build-fingerprinter-0.2.8.tar", max compression
```

## Comparing `uw-it-build-fingerprinter-0.2.7.tar` & `uw-it-build-fingerprinter-0.2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2022-08-04 21:57:51.830089 uw-it-build-fingerprinter-0.2.7/LICENSE
--rw-r--r--   0        0        0       92 2022-08-04 21:57:51.830089 uw-it-build-fingerprinter-0.2.7/fingerprinter/__init__.py
--rwxr-xr-x   0        0        0     8552 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/build.sh
--rw-r--r--   0        0        0     1998 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/build_arg_resolver.py
--rw-r--r--   0        0        0     4261 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/cli.py
--rw-r--r--   0        0        0     1255 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/command_builder.py
--rw-r--r--   0        0        0      122 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/deployment.dockerfile
--rw-r--r--   0        0        0     4588 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/fingerprinter.py
--rw-r--r--   0        0        0     2076 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/models.py
--rw-r--r--   0        0        0     3215 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/fingerprinter/target_resolver.py
--rw-r--r--   0        0        0      487 2022-08-04 21:57:51.834089 uw-it-build-fingerprinter-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      742 2022-08-04 21:59:24.553860 uw-it-build-fingerprinter-0.2.7/setup.py
--rw-r--r--   0        0        0      434 2022-08-04 21:59:24.554141 uw-it-build-fingerprinter-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-21 17:43:17.680328 uw-it-build-fingerprinter-0.2.8/LICENSE
+-rw-r--r--   0        0        0       92 2023-04-21 17:43:17.680328 uw-it-build-fingerprinter-0.2.8/fingerprinter/__init__.py
+-rwxr-xr-x   0        0        0     8552 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/build.sh
+-rw-r--r--   0        0        0     1998 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/build_arg_resolver.py
+-rw-r--r--   0        0        0     4269 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/cli.py
+-rw-r--r--   0        0        0     1255 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/command_builder.py
+-rw-r--r--   0        0        0      122 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/deployment.dockerfile
+-rw-r--r--   0        0        0     4588 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/fingerprinter.py
+-rw-r--r--   0        0        0     2076 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/models.py
+-rw-r--r--   0        0        0     3215 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/fingerprinter/target_resolver.py
+-rw-r--r--   0        0        0      487 2023-04-21 17:43:17.684328 uw-it-build-fingerprinter-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      742 2023-04-21 17:44:40.250640 uw-it-build-fingerprinter-0.2.8/setup.py
+-rw-r--r--   0        0        0      434 2023-04-21 17:44:40.250897 uw-it-build-fingerprinter-0.2.8/PKG-INFO
```

### Comparing `uw-it-build-fingerprinter-0.2.7/LICENSE` & `uw-it-build-fingerprinter-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `uw-it-build-fingerprinter-0.2.7/fingerprinter/build.sh` & `uw-it-build-fingerprinter-0.2.8/fingerprinter/build.sh`

 * *Files identical despite different names*

### Comparing `uw-it-build-fingerprinter-0.2.7/fingerprinter/build_arg_resolver.py` & `uw-it-build-fingerprinter-0.2.8/fingerprinter/build_arg_resolver.py`

 * *Files identical despite different names*

### Comparing `uw-it-build-fingerprinter-0.2.7/fingerprinter/cli.py` & `uw-it-build-fingerprinter-0.2.8/fingerprinter/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import argparse
 import logging
 import os.path
+import textwrap
 
 import yaml
 
 from fingerprinter.target_resolver import TargetResolver
 from .models import BuildConfig
 
 
 def get_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
-        description="""
-        This tool can be used to build deterministic fingerprints, that 
+        description=textwrap.dedent("""
+        This tool can be used to build deterministic fingerprints, that
         are smartly flagged for updates based on configuration you provide.
         For full documentation, please refer to the README at
-            https://github.com/uwit-iam/fingerprinter/tree/main/README.md        
-       
-       
+            https://github.com/uwit-iam/fingerprinter/tree/main/README.md
+
+
         Behavior is mainly controlled by the output type (-o/--output):
-        
-        js/json        REQUIRES: -t/--target 
+
+        js/json        REQUIRES: -t/--target
                                  -c/--config (if not default)
                        OUTPUTS: the json build configuration for the target
                        This is the default output type
-                       
+
         pjs/pretty-json
                        Same as js/json, but the output is easier to read
-        
+
         build-script   OUTPUTS: The absolute path to the 'build-fp-targets.sh' script.
-        
+
         build-targets  REQUIRES: -c/c--config (if not default)
                        OUTPUTS: An acceptable order in which to build all configured targets
-         
-        """,
+
+        """),
         usage="fingerprinter [-o <OUTPUT_TYPE>] [-f <CONFIGURATION_FILE] [-t TARGET] [OPTIONS]",
+        formatter_class=argparse.RawTextHelpFormatter,
     )
     parser.add_argument('--config-file', '-f', default='fingerprints.yaml',
                         help='The config file you want to use to generate fingerprints.')
     parser.add_argument('--target', '-t', required=False, default=None,
                         help='The target from the config file whose configuration you want to get')
     parser.add_argument('--verbose', '-v', action='store_true', default=False,
                         help='Set log level to INFO')
```

### Comparing `uw-it-build-fingerprinter-0.2.7/fingerprinter/command_builder.py` & `uw-it-build-fingerprinter-0.2.8/fingerprinter/command_builder.py`

 * *Files identical despite different names*

### Comparing `uw-it-build-fingerprinter-0.2.7/fingerprinter/fingerprinter.py` & `uw-it-build-fingerprinter-0.2.8/fingerprinter/fingerprinter.py`

 * *Files identical despite different names*

### Comparing `uw-it-build-fingerprinter-0.2.7/fingerprinter/models.py` & `uw-it-build-fingerprinter-0.2.8/fingerprinter/models.py`

 * *Files identical despite different names*

### Comparing `uw-it-build-fingerprinter-0.2.7/fingerprinter/target_resolver.py` & `uw-it-build-fingerprinter-0.2.8/fingerprinter/target_resolver.py`

 * *Files identical despite different names*

### Comparing `uw-it-build-fingerprinter-0.2.7/setup.py` & `uw-it-build-fingerprinter-0.2.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['PyYAML>=6.0,<7.0', 'pydantic>=1.9.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['fingerprinter = fingerprinter.cli:main']}
 
 setup_kwargs = {
     'name': 'uw-it-build-fingerprinter',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': '',
     'long_description': None,
     'author': 'Tom Thorogood',
     'author_email': 'tom@tomthorogood.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

