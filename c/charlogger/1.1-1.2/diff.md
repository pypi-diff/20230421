# Comparing `tmp/charlogger-1.1.tar.gz` & `tmp/charlogger-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charlogger-1.1.tar", last modified: Thu Feb 16 00:13:19 2023, max compression
+gzip compressed data, was "charlogger-1.2.tar", last modified: Fri Apr 21 19:45:45 2023, max compression
```

## Comparing `charlogger-1.1.tar` & `charlogger-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 00:13:19.463870 charlogger-1.1/
--rw-rw-rw-   0        0        0     3143 2023-02-16 00:13:19.462893 charlogger-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2928 2023-02-16 00:11:19.000000 charlogger-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-16 00:13:19.444263 charlogger-1.1/charlogger/
--rw-rw-rw-   0        0        0      199 2023-02-16 00:13:17.000000 charlogger-1.1/charlogger/__init__.py
--rw-rw-rw-   0        0        0     4763 2023-02-15 23:05:18.000000 charlogger-1.1/charlogger/logger.py
-drwxrwxrwx   0        0        0        0 2023-02-16 00:13:19.460940 charlogger-1.1/charlogger.egg-info/
--rw-rw-rw-   0        0        0     3143 2023-02-16 00:13:19.000000 charlogger-1.1/charlogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-02-16 00:13:19.000000 charlogger-1.1/charlogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 00:13:19.000000 charlogger-1.1/charlogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-16 00:13:19.000000 charlogger-1.1/charlogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-16 00:13:19.000000 charlogger-1.1/charlogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-16 00:13:19.463870 charlogger-1.1/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-02-16 00:13:11.000000 charlogger-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:45:45.987416 charlogger-1.2/
+-rw-rw-rw-   0        0        0     3157 2023-04-21 19:45:45.986416 charlogger-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2942 2023-04-21 19:43:40.000000 charlogger-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 19:45:45.972696 charlogger-1.2/charlogger/
+-rw-rw-rw-   0        0        0      199 2023-04-21 19:45:15.000000 charlogger-1.2/charlogger/__init__.py
+-rw-rw-rw-   0        0        0     4994 2023-04-21 19:45:06.000000 charlogger-1.2/charlogger/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-21 19:45:45.984249 charlogger-1.2/charlogger.egg-info/
+-rw-rw-rw-   0        0        0     3157 2023-04-21 19:45:45.000000 charlogger-1.2/charlogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-04-21 19:45:45.000000 charlogger-1.2/charlogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 19:45:45.000000 charlogger-1.2/charlogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 19:45:45.000000 charlogger-1.2/charlogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-21 19:45:45.000000 charlogger-1.2/charlogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 19:45:45.987416 charlogger-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-04-21 19:42:19.000000 charlogger-1.2/setup.py
```

### Comparing `charlogger-1.1/PKG-INFO` & `charlogger-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charlogger
-Version: 1.1
+Version: 1.2
 Summary: A logging library for Python.
 Home-page: https://github.com/chaarlottte/charlogger
 Author: chaarlottte
 Description-Content-Type: text/markdown
 
 # charlogger
 A logging library for Python.
@@ -31,40 +31,40 @@
 ### Advanced example
 ```python
 import charlogger
 
 # All parameters are optional.
 logger = charlogger.Logger(
     debug=True, # Whether to enable the output of debug logs
-    defaultPrefix="your prefix",
-    colorText=False, # Whether to have the info text be colored
-    logFile=open("log.txt", "a"), # The file to put logs in
-    indentLevel=8, # The indentation of the text when output.
+    default_prefix="your prefix",
+    color_text=False, # Whether to have the info text be colored
+    log_file_patj=open("log.txt", "a"), # The file to put logs in
+    indent_level=8, # The indentation of the text when output.
     centered=True # Whether to center text in the console.
 )
 
 logger.info("What a great logging library!")
 ```
 
 ### My personal configuration (best)
 ```python
 import charlogger
 
 logger = charlogger.Logger(
     debug=True,
-    defaultPrefix="<TIME> WORKER-001",
-    colorText=True
+    default_prefix="<TIME> | WORKER-001",
+    color_text=True
 )
 logger.info("What a great logging library!")
 ```
 
 ## More in-depth documentation
 
 ### `defaultPrefix`
-When initializing a Logger, you have the option of `defaultPrefix`.
+When initializing a Logger, you have the option of `default_prefix`.
 
 For now, if you add `"<TIME>"` anywhere in that string, it will replace it with the time of the logging.
 
 For instance, the following code will print `18:26:15 | hi! | i > What a great logging library! `
 ```python
 import charlogger
```

### Comparing `charlogger-1.1/README.md` & `charlogger-1.2/charlogger.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: charlogger
+Version: 1.2
+Summary: A logging library for Python.
+Home-page: https://github.com/chaarlottte/charlogger
+Author: chaarlottte
+Description-Content-Type: text/markdown
+
 # charlogger
 A logging library for Python.
 
 I've been using this myself for a while, and I thought that I may as well release it.
 
 It's filled with bad code, but now that it is public, I'll probably improve it over time.
 
@@ -23,40 +31,40 @@
 ### Advanced example
 ```python
 import charlogger
 
 # All parameters are optional.
 logger = charlogger.Logger(
     debug=True, # Whether to enable the output of debug logs
-    defaultPrefix="your prefix",
-    colorText=False, # Whether to have the info text be colored
-    logFile=open("log.txt", "a"), # The file to put logs in
-    indentLevel=8, # The indentation of the text when output.
+    default_prefix="your prefix",
+    color_text=False, # Whether to have the info text be colored
+    log_file_patj=open("log.txt", "a"), # The file to put logs in
+    indent_level=8, # The indentation of the text when output.
     centered=True # Whether to center text in the console.
 )
 
 logger.info("What a great logging library!")
 ```
 
 ### My personal configuration (best)
 ```python
 import charlogger
 
 logger = charlogger.Logger(
     debug=True,
-    defaultPrefix="<TIME> WORKER-001",
-    colorText=True
+    default_prefix="<TIME> | WORKER-001",
+    color_text=True
 )
 logger.info("What a great logging library!")
 ```
 
 ## More in-depth documentation
 
 ### `defaultPrefix`
-When initializing a Logger, you have the option of `defaultPrefix`.
+When initializing a Logger, you have the option of `default_prefix`.
 
 For now, if you add `"<TIME>"` anywhere in that string, it will replace it with the time of the logging.
 
 For instance, the following code will print `18:26:15 | hi! | i > What a great logging library! `
 ```python
 import charlogger
 
@@ -101,8 +109,8 @@
 
 # I can't imagine this one being all that useful. It's more there for my personal projects that use it,
 logger.choice(1, "Option 1") # 1 > Option 1 
 
 # Will wait for user input in the console.
 name = logger.ask("What is your name?") # ? > What is your name? > 
 print(name)
-```
+```
```

### Comparing `charlogger-1.1/charlogger/logger.py` & `charlogger-1.2/charlogger/logger.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from typing import TextIO
 import os, sys
 
 class Logger():
     def __init__(
                 self, 
                 debug: bool = False, 
-                defaultPrefix: str = None, 
-                colorText: bool = False,
-                indentLevel: int = 0,
+                default_prefix: str = None, 
+                color_text: bool = False,
+                indent_level: int = 0,
                 centered: bool = False,
                 stream: TextIO = sys.stdout,
-                logFile: TextIO = None
+                log_file_path: TextIO = None
             ) -> None:
-        self.debugMode = debug
-        self.defaultPrefix = defaultPrefix
-        self.colorText = colorText
-        self.indentLevel = indentLevel
+        self.debug_mode = debug
+        self.default_prefix = default_prefix
+        self.color_text = color_text
+        self.indent_level = indent_level
         self.centered = centered
         self.stream = stream
-        self.logFile = logFile
+        self.log_file_path = log_file_path
         pass
 
     def info(self, data: str, title: str = None) -> None:
         prefix = self.prefix("i", Fore.LIGHTBLUE_EX, title)
         self.output(f"{prefix} {data} {Fore.RESET}")
 
     def warn(self, data: str, title: str = None) -> None:
@@ -33,15 +33,15 @@
         self.output(f"{prefix} {data} {Fore.RESET}")
 
     def error(self, data: str, title: str = None) -> None:
         prefix = self.prefix("!", Fore.RED, title)
         self.output(f"{prefix} {data} {Fore.RESET}")
 
     def debug(self, data: str, title: str = None) -> None:
-        if self.debugMode:
+        if self.debug_mode:
             prefix = self.prefix("~", Fore.LIGHTMAGENTA_EX, title)
             self.output(f"{prefix} {data} {Fore.RESET}")
 
     def valid(self, data: str, title: str = None) -> None:
         prefix = self.prefix("✓", Fore.LIGHTGREEN_EX, title)
         self.output(f"{prefix} {data} {Fore.RESET}")
 
@@ -70,58 +70,61 @@
             self.stream.write(f"{s.center(os.get_terminal_size().columns)}\n")
             self.stream.flush()
         else:
             self.stream.write(f"{s}\n")
             self.stream.flush()
 
         # Please never look at this code
-        if self.logFile is not None:
+        if self.log_file_path is not None:
             toRemove = []
             for x in AnsiFore.__dict__:
                 toRemove.append(AnsiFore.__dict__[x])
 
             for x in toRemove:
                 s = s.replace(f"[{x}m", "")
 
             try:
-                self.logFile.write(f"{s}\n")
-                self.logFile.flush()
+                self.log_file_path.write(f"{s}\n")
+                self.log_file_path.flush()
             except UnicodeEncodeError as e:
-                self.logFile.write(f"{s[:e.start] + ' ' + s[e.end:]}\n")
-                self.logFile.flush()
+                self.log_file_path.write(f"{s[:e.start] + ' ' + s[e.end:]}\n")
+                self.log_file_path.flush()
 
     def prefix(self, data: str, color: Fore, title: str = None) -> str:
         s = Logger._prefix(
                 data=data,
                 color=color,
                 title=title,
-                defaultPrefix=self.defaultPrefix,
-                colorText=self.colorText,
+                default_prefix=self.default_prefix,
+                color_text=self.color_text,
                 centered=self.centered,
-                indentLevel=self.indentLevel
+                indent_level=self.indent_level
             )
         return s
 
-    def _prefix(data: str, color: Fore, title: str = None, defaultPrefix: str = None, colorText: bool = False, centered: bool = False, indentLevel: int = 0) -> str:
+    def _prefix(data: str, color: Fore, title: str = None, default_prefix: str = None, color_text: bool = False, centered: bool = False, indent_level: int = 0) -> str:
         pr1 = ""
         if not centered: 
-            for _ in range(indentLevel): 
+            for _ in range(indent_level): 
                 pr1 = pr1 + " "
 
-        if defaultPrefix is not None:
-            if "<TIME>" in defaultPrefix:
-                defaultPrefix = defaultPrefix.replace("<TIME>", f"{datetime.now().strftime(f'{color}%H{Fore.WHITE}:{color}%M{Fore.WHITE}:{color}%S')}{Fore.WHITE} |{color}")
-                
-            pr1 = pr1 + f"{color}{defaultPrefix}{Fore.RESET} | "
+        if default_prefix is not None:
+            if "<TIME>" in default_prefix:
+                default_prefix = default_prefix.replace("<TIME>", f"{datetime.now().strftime(f'{color}%H{Fore.LIGHTBLACK_EX}:{color}%M{Fore.LIGHTBLACK_EX}:{color}%S')}")
+            
+            if "|" in default_prefix:
+                default_prefix = default_prefix.replace("|", f"{Fore.LIGHTBLACK_EX}|{color}")
+
+            pr1 = pr1 + f"{color}{default_prefix}{Fore.LIGHTBLACK_EX} | "
 
            
-        pr2 = f"{color}{data} >"
+        pr2 = f"{Fore.LIGHTBLACK_EX}({color}{data}{Fore.LIGHTBLACK_EX})"
 
-        fullPrefix = f"{pr1}{pr2}"
+        full_prefix = f"{pr1}{pr2}"
 
         if title is not None:
-            fullPrefix = fullPrefix + f" {Fore.WHITE}[{color}{title}{Fore.WHITE}]{color}"
+            full_prefix = full_prefix + f" {color}{title}"
 
-        if not colorText: 
-            fullPrefix = fullPrefix + f"{Fore.RESET}"
+        if not color_text: 
+            full_prefix = full_prefix + f"{Fore.LIGHTBLACK_EX}"
         
-        return fullPrefix
+        return full_prefix
```

### Comparing `charlogger-1.1/charlogger.egg-info/PKG-INFO` & `charlogger-1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: charlogger
-Version: 1.1
-Summary: A logging library for Python.
-Home-page: https://github.com/chaarlottte/charlogger
-Author: chaarlottte
-Description-Content-Type: text/markdown
-
 # charlogger
 A logging library for Python.
 
 I've been using this myself for a while, and I thought that I may as well release it.
 
 It's filled with bad code, but now that it is public, I'll probably improve it over time.
 
@@ -31,40 +23,40 @@
 ### Advanced example
 ```python
 import charlogger
 
 # All parameters are optional.
 logger = charlogger.Logger(
     debug=True, # Whether to enable the output of debug logs
-    defaultPrefix="your prefix",
-    colorText=False, # Whether to have the info text be colored
-    logFile=open("log.txt", "a"), # The file to put logs in
-    indentLevel=8, # The indentation of the text when output.
+    default_prefix="your prefix",
+    color_text=False, # Whether to have the info text be colored
+    log_file_patj=open("log.txt", "a"), # The file to put logs in
+    indent_level=8, # The indentation of the text when output.
     centered=True # Whether to center text in the console.
 )
 
 logger.info("What a great logging library!")
 ```
 
 ### My personal configuration (best)
 ```python
 import charlogger
 
 logger = charlogger.Logger(
     debug=True,
-    defaultPrefix="<TIME> WORKER-001",
-    colorText=True
+    default_prefix="<TIME> | WORKER-001",
+    color_text=True
 )
 logger.info("What a great logging library!")
 ```
 
 ## More in-depth documentation
 
 ### `defaultPrefix`
-When initializing a Logger, you have the option of `defaultPrefix`.
+When initializing a Logger, you have the option of `default_prefix`.
 
 For now, if you add `"<TIME>"` anywhere in that string, it will replace it with the time of the logging.
 
 For instance, the following code will print `18:26:15 | hi! | i > What a great logging library! `
 ```python
 import charlogger
 
@@ -109,8 +101,8 @@
 
 # I can't imagine this one being all that useful. It's more there for my personal projects that use it,
 logger.choice(1, "Option 1") # 1 > Option 1 
 
 # Will wait for user input in the console.
 name = logger.ask("What is your name?") # ? > What is your name? > 
 print(name)
-```
+```
```

### Comparing `charlogger-1.1/setup.py` & `charlogger-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="charlogger",
-    version="1.1",
+    version="1.2",
     description="A logging library for Python.",
     url="https://github.com/chaarlottte/charlogger",
     author="chaarlottte",
     packages=[ "charlogger" ],
     install_requires=[ 
         "colorama"
     ],
```

