# Comparing `tmp/pylumber-0.1.0.tar.gz` & `tmp/pylumber-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylumber-0.1.0.tar", last modified: Mon Apr 17 01:41:18 2023, max compression
+gzip compressed data, was "pylumber-0.1.1.tar", last modified: Thu Apr 20 23:48:49 2023, max compression
```

## Comparing `pylumber-0.1.0.tar` & `pylumber-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 01:41:18.024585 pylumber-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-03-19 17:29:20.000000 pylumber-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      549 2023-04-17 01:41:18.023586 pylumber-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-03-19 17:29:20.000000 pylumber-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 01:41:18.015630 pylumber-0.1.0/pylumber/
--rw-rw-rw-   0        0        0     3051 2023-04-17 01:37:25.000000 pylumber-0.1.0/pylumber/__init__.py
--rw-rw-rw-   0        0        0       40 2023-04-10 23:14:37.000000 pylumber-0.1.0/pylumber/format.py
-drwxrwxrwx   0        0        0        0 2023-04-17 01:41:18.022280 pylumber-0.1.0/pylumber.egg-info/
--rw-rw-rw-   0        0        0      549 2023-04-17 01:41:17.000000 pylumber-0.1.0/pylumber.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-04-17 01:41:17.000000 pylumber-0.1.0/pylumber.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 01:41:17.000000 pylumber-0.1.0/pylumber.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-17 01:41:17.000000 pylumber-0.1.0/pylumber.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 01:41:18.024585 pylumber-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-17 01:24:56.000000 pylumber-0.1.0/setup.py
+drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-04-20 23:48:49.101161 pylumber-0.1.1/
+-rw-r--r--   0 thryang    (501) staff       (20)     1065 2023-03-14 19:30:15.000000 pylumber-0.1.1/LICENSE
+-rw-r--r--   0 thryang    (501) staff       (20)      535 2023-04-20 23:48:49.101055 pylumber-0.1.1/PKG-INFO
+-rw-r--r--   0 thryang    (501) staff       (20)      103 2023-03-14 19:30:15.000000 pylumber-0.1.1/README.md
+drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-04-20 23:48:49.100308 pylumber-0.1.1/pylumber/
+-rw-r--r--   0 thryang    (501) staff       (20)     2966 2023-04-20 23:17:25.000000 pylumber-0.1.1/pylumber/__init__.py
+-rw-r--r--   0 thryang    (501) staff       (20)       37 2023-04-10 22:49:31.000000 pylumber-0.1.1/pylumber/format.py
+drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-04-20 23:48:49.100891 pylumber-0.1.1/pylumber.egg-info/
+-rw-r--r--   0 thryang    (501) staff       (20)      535 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/PKG-INFO
+-rw-r--r--   0 thryang    (501) staff       (20)      194 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/SOURCES.txt
+-rw-r--r--   0 thryang    (501) staff       (20)        1 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/dependency_links.txt
+-rw-r--r--   0 thryang    (501) staff       (20)        9 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/top_level.txt
+-rw-r--r--   0 thryang    (501) staff       (20)       38 2023-04-20 23:48:49.101192 pylumber-0.1.1/setup.cfg
+-rw-r--r--   0 thryang    (501) staff       (20)      775 2023-04-20 23:48:35.000000 pylumber-0.1.1/setup.py
```

### Comparing `pylumber-0.1.0/pylumber/__init__.py` & `pylumber-0.1.1/pylumber/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# ~~~~~~ |
-# pyLumber.py - Lumberjack for your Code, Logs, Prints, 
-# Errors and more.
-# Author: Tim Yang (TimMUP)
-# Editor:
-# Status: In Development MIT License
-# Version: 0.0.1
-# Date: 2019-01-01
-# ~~~~~~ |
-
-import os
-import re
-import timeit
-
-class ANSI_MODI:
-    """ANSI Modification Codes"""
-    BOLD        = '\033[1m'             # BOLD
-    UNDERLINE   = '\033[4m'             # UNDERLINE
-    BLINK       = '\033[5m'             # BLINK
-    REVERSE     = '\033[7m'             # REVERSE
-    CONCEALED   = '\033[8m'             # CONCEALED
-    END         = '\033[0m'             # DEFAULT
-
-class ANSI_FORE:
-    """ANSI Foreground Color Codes"""
-    ACCENT1     = '\033[91m'            # RED
-    ACCENT2     = '\033[92m'            # GREEN
-    ACCENT3     = '\033[93m'            # YELLOW
-    ACCENT4     = '\033[94m'            # BLUE
-    ACCENT5     = '\033[95m'            # MAGENTA
-    ACCENT6     = '\033[96m'            # CYAN
-    
-class ANSI_BACK:
-    """ANSI Background Color Codes"""
-    ACCENT1     = '\033[101m'            # RED
-    ACCENT2     = '\033[102m'            # GREEN
-    ACCENT3     = '\033[103m'            # YELLOW
-    ACCENT4     = '\033[104m'            # BLUE
-    ACCENT5     = '\033[105m'            # MAGENTA
-    ACCENT6     = '\033[106m'            # CYAN
-
-class CONST:
-    PREFIX_SPACE = 8
-    PREFIX_CHAR = " "
-    PREFIX_MODI = [ANSI_MODI.BOLD]
-    DEFAULT_LOG_PARAM = [
-        # Default Parameters for Log Files:
-        ("ERROR", ANSI_FORE.ACCENT1),
-        ("OK", ANSI_FORE.ACCENT2),
-        ("WARN", ANSI_FORE.ACCENT3),
-        ("INFO", ANSI_FORE.ACCENT4),
-        ("DEBUG", ANSI_FORE.ACCENT5)
-    ]
-
-
-# q: What is the regex expression for matching all sets between '\' and 'm'?
-# a: \033\[[0-9;]*m
-
-
-# Helper Function (Library Use) | Removes all ANSI Codes from String
-def STRIP_ANSI(string):
-    return re.sub(r'\033\[[0-9;]*m', '', string)
-
-
-# Helper Function (User Use) | Formats string with 
-class lumberjack:
-    def __init__(self, logFile=None, logParameter: list = CONST.DEFAULT_LOG_PARAM, logPrint=False):
-        self.logFile = open(logFile, "w") if logFile else None
-        self.DICT = {}
-        for i in range(len(logParameter)):
-            logPrefix = f"{logParameter[i][1]}[{logParameter[i][0].center(CONST.PREFIX_SPACE, CONST.PREFIX_CHAR)}]{ANSI_MODI.END}"
-            self.DICT[i] = (logPrefix, logParameter[i][1])                          # (Prefix w/ Formatting, ANSI Formatting) 
-            self.DICT[logParameter[i][0]] = (logPrefix, logParameter[i][1])         # (Additional Key for Prefix Input)
-    
-    def logWriter(self, msg):
-        if self.logFile:
-            self.logFile.write(STRIP_ANSI(msg + "\n"))
-
-    def log(self, msg: str, logLevel = "OK"):
-        modiMsg = f"{self.DICT[logLevel][0]} {msg}{ANSI_MODI.END}"
-        self.logWriter(modiMsg)
-        print(modiMsg)
-    
-    def format(self, msg: str, logLevel = "OK"):
-        return f"{self.DICT[logLevel][1]}{msg}{ANSI_MODI.END}"
+# ~~~~~~ |
+# pyLumber.py - Lumberjack for your Code, Logs, Prints, 
+# Errors and more.
+# Author: Tim Yang (TimMUP)
+# Editor:
+# Status: In Development MIT License
+# Version: 0.0.1
+# Date: 2019-01-01
+# ~~~~~~ |
+
+import os
+import re
+import timeit
+
+class ANSI_MODI:
+    """ANSI Modification Codes"""
+    BOLD        = '\033[1m'             # BOLD
+    UNDERLINE   = '\033[4m'             # UNDERLINE
+    BLINK       = '\033[5m'             # BLINK
+    REVERSE     = '\033[7m'             # REVERSE
+    CONCEALED   = '\033[8m'             # CONCEALED
+    END         = '\033[0m'             # DEFAULT
+
+class ANSI_FORE:
+    """ANSI Foreground Color Codes"""
+    ACCENT1     = '\033[91m'            # RED
+    ACCENT2     = '\033[92m'            # GREEN
+    ACCENT3     = '\033[93m'            # YELLOW
+    ACCENT4     = '\033[94m'            # BLUE
+    ACCENT5     = '\033[95m'            # MAGENTA
+    ACCENT6     = '\033[96m'            # CYAN
+    
+class ANSI_BACK:
+    """ANSI Background Color Codes"""
+    ACCENT1     = '\033[101m'            # RED
+    ACCENT2     = '\033[102m'            # GREEN
+    ACCENT3     = '\033[103m'            # YELLOW
+    ACCENT4     = '\033[104m'            # BLUE
+    ACCENT5     = '\033[105m'            # MAGENTA
+    ACCENT6     = '\033[106m'            # CYAN
+
+class CONST:
+    PREFIX_SPACE = 8
+    PREFIX_CHAR = " "
+    PREFIX_MODI = [ANSI_MODI.BOLD]
+    DEFAULT_LOG_PARAM = [
+        # Default Parameters for Log Files:
+        ("ERROR", ANSI_FORE.ACCENT1),
+        ("OK", ANSI_FORE.ACCENT2),
+        ("WARN", ANSI_FORE.ACCENT3),
+        ("INFO", ANSI_FORE.ACCENT4),
+        ("DEBUG", ANSI_FORE.ACCENT5)
+    ]
+
+
+# q: What is the regex expression for matching all sets between '\' and 'm'?
+# a: \033\[[0-9;]*m
+
+
+# Helper Function (Library Use) | Removes all ANSI Codes from String
+def STRIP_ANSI(string):
+    return re.sub(r'\033\[[0-9;]*m', '', string)
+
+
+# Helper Function (User Use) | Formats string with 
+class lumberjack:
+    def __init__(self, logFile=None, logParameter: list = CONST.DEFAULT_LOG_PARAM, logPrint=False):
+        self.logFile = open(logFile, "w") if logFile else None
+        self.DICT = {}
+        for i in range(len(logParameter)):
+            logPrefix = f"{logParameter[i][1]}[{logParameter[i][0].center(CONST.PREFIX_SPACE, CONST.PREFIX_CHAR)}]{ANSI_MODI.END}"
+            self.DICT[i] = (logPrefix, logParameter[i][1])                          # (Prefix w/ Formatting, ANSI Formatting) 
+            self.DICT[logParameter[i][0]] = (logPrefix, logParameter[i][1])         # (Additional Key for Prefix Input)
+    
+    def logWriter(self, msg):
+        if self.logFile:
+            self.logFile.write(STRIP_ANSI(msg + "\n"))
+
+    def log(self, msg: str, logLevel = "OK"):
+        modiMsg = f"{self.DICT[logLevel][0]} {msg}{ANSI_MODI.END}"
+        self.logWriter(modiMsg)
+        print(modiMsg)
+    
+    def format(self, msg: str, logLevel = "OK"):
+        return f"{self.DICT[logLevel][1]}{msg}{ANSI_MODI.END}"
```

### Comparing `pylumber-0.1.0/setup.py` & `pylumber-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import setup, find_packages
-
-VERSION = '0.1.0'
-DESCRIPTION = 'Lumberjack for your Code, Logs, Prints, Errors and more.'
-LONG_DESCRIPTION = 'pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use.'
-
-setup(
-    name="pylumber",
-    version=VERSION,
-    author="Tim Yang (TimMUP)",
-    author_email="thryang@outlook.com",
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    packages=find_packages(),
-    install_requires=[],
-    keywords=['python', 'logging', 'debugging', 'lumberjack'],
-    classifiers= [
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License"
-    ]
-)
+from setuptools import setup, find_packages
+
+VERSION = '0.1.1'
+DESCRIPTION = 'Lumberjack for your Code, Logs, Prints, Errors and more.'
+LONG_DESCRIPTION = 'pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use.'
+
+setup(
+    name="pylumber",
+    version=VERSION,
+    author="Tim Yang (TimMUP)",
+    author_email="thryang@outlook.com",
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    install_requires=[],
+    keywords=['python', 'logging', 'debugging', 'lumberjack'],
+    classifiers= [
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License"
+    ]
+)
```

