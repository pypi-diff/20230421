# Comparing `tmp/duckietown-shell-5.5.2.tar.gz` & `tmp/duckietown-shell-5.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckietown-shell-5.5.2.tar", last modified: Thu Apr 20 14:43:16 2023, max compression
+gzip compressed data, was "duckietown-shell-5.5.3.tar", last modified: Thu Apr 20 15:13:57 2023, max compression
```

## Comparing `duckietown-shell-5.5.2.tar` & `duckietown-shell-5.5.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:43:16.647573 duckietown-shell-5.5.2/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/LICENSE.pdf
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-20 14:43:16.647573 duckietown-shell-5.5.2/PKG-INFO
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:43:16.643573 duckietown-shell-5.5.2/lib/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:43:16.647573 duckietown-shell-5.5.2/lib/dt_shell/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1128 2023-04-20 14:43:14.000000 duckietown-shell-5.5.2/lib/dt_shell/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13053 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1306 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/cli_options.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1680 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/col_logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2307 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/commands_.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4291 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/config.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      895 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2984 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/dt_command_abs.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      201 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/dt_command_placeholder.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3835 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/duckietown_tokens.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4741 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/env_checks.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      683 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      664 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5530 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/main.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2467 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/package_version_check.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1994 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/tokens_cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4610 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/update_utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3239 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/utils.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4528 2023-04-19 20:12:13.000000 duckietown-shell-5.5.2/lib/dt_shell/version_check.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 14:43:16.647573 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-20 14:43:16.000000 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      854 2023-04-20 14:43:16.000000 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 14:43:16.000000 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       43 2023-04-20 14:43:16.000000 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 04:24:53.000000 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/not-zip-safe
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      259 2023-04-20 14:43:16.000000 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        9 2023-04-20 14:43:16.000000 duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/top_level.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 14:43:16.647573 duckietown-shell-5.5.2/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2008 2023-04-20 14:42:56.000000 duckietown-shell-5.5.2/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:57.135884 duckietown-shell-5.5.3/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    75933 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/LICENSE.pdf
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-20 15:13:57.135884 duckietown-shell-5.5.3/PKG-INFO
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:57.135884 duckietown-shell-5.5.3/lib/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:57.135884 duckietown-shell-5.5.3/lib/dt_shell/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1128 2023-04-20 15:13:55.000000 duckietown-shell-5.5.3/lib/dt_shell/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13053 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1306 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/cli_options.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1680 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/col_logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2307 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/commands_.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4291 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/config.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      895 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2984 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/dt_command_abs.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      201 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/dt_command_placeholder.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3835 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/duckietown_tokens.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4741 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/env_checks.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      683 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      664 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     5530 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/main.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2467 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/package_version_check.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1994 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/tokens_cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4610 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/update_utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3239 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/utils.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4528 2023-04-19 20:12:13.000000 duckietown-shell-5.5.3/lib/dt_shell/version_check.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 15:13:57.135884 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      241 2023-04-20 15:13:57.000000 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      854 2023-04-20 15:13:57.000000 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 15:13:57.000000 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       43 2023-04-20 15:13:57.000000 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 04:24:53.000000 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/not-zip-safe
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      259 2023-04-20 15:13:57.000000 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        9 2023-04-20 15:13:57.000000 duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/top_level.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 15:13:57.135884 duckietown-shell-5.5.3/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2008 2023-04-20 15:13:44.000000 duckietown-shell-5.5.3/setup.py
```

### Comparing `duckietown-shell-5.5.2/LICENSE.pdf` & `duckietown-shell-5.5.3/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/__init__.py` & `duckietown-shell-5.5.3/lib/dt_shell/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Optional
 
 logging.basicConfig()
 
 dtslogger = logging.getLogger("dts")
 dtslogger.setLevel(logging.INFO)
 
-__version__ = "5.5.2"
+__version__ = "5.5.3"
 
 
 dtslogger.debug(f"duckietown-shell {__version__}")
 
 import sys
 
 if sys.version_info < (3, 6):
```

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/cli.py` & `duckietown-shell-5.5.3/lib/dt_shell/cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/cli_options.py` & `duckietown-shell-5.5.3/lib/dt_shell/cli_options.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/col_logging.py` & `duckietown-shell-5.5.3/lib/dt_shell/col_logging.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/commands_.py` & `duckietown-shell-5.5.3/lib/dt_shell/commands_.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/config.py` & `duckietown-shell-5.5.3/lib/dt_shell/config.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/constants.py` & `duckietown-shell-5.5.3/lib/dt_shell/constants.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/dt_command_abs.py` & `duckietown-shell-5.5.3/lib/dt_shell/dt_command_abs.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/duckietown_tokens.py` & `duckietown-shell-5.5.3/lib/dt_shell/duckietown_tokens.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/env_checks.py` & `duckietown-shell-5.5.3/lib/dt_shell/env_checks.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/exceptions.py` & `duckietown-shell-5.5.3/lib/dt_shell/exceptions.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/logging.py` & `duckietown-shell-5.5.3/lib/dt_shell/logging.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/main.py` & `duckietown-shell-5.5.3/lib/dt_shell/main.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/package_version_check.py` & `duckietown-shell-5.5.3/lib/dt_shell/package_version_check.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/tokens_cli.py` & `duckietown-shell-5.5.3/lib/dt_shell/tokens_cli.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/update_utils.py` & `duckietown-shell-5.5.3/lib/dt_shell/update_utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/utils.py` & `duckietown-shell-5.5.3/lib/dt_shell/utils.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/dt_shell/version_check.py` & `duckietown-shell-5.5.3/lib/dt_shell/version_check.py`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/lib/duckietown_shell.egg-info/SOURCES.txt` & `duckietown-shell-5.5.3/lib/duckietown_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckietown-shell-5.5.2/setup.py` & `duckietown-shell-5.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     'duckietown-docker-utils-{}>=6.0.90'.format(distro),
     'zeroconf',
     'requests',
     'pytz',
     'dt-authentication-{}'.format(distro),
     'dt-data-api-{}>=1.2.0'.format(distro),
     "pip",
-    "dockertown>=0.2.0",
+    "dockertown>=0.2.1",
     "dtproject",
 ]
 
 system_version = tuple(sys.version_info)[:3]
 if system_version < (3, 7):
     install_requires.append('dataclasses')
```

