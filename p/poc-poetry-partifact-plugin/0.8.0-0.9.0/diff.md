# Comparing `tmp/poc_poetry_partifact_plugin-0.8.0.tar.gz` & `tmp/poc_poetry_partifact_plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poc_poetry_partifact_plugin-0.8.0.tar", max compression
+gzip compressed data, was "poc_poetry_partifact_plugin-0.9.0.tar", max compression
```

## Comparing `poc_poetry_partifact_plugin-0.8.0.tar` & `poc_poetry_partifact_plugin-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        3 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/__init__.py
--rw-r--r--   0        0        0     1478 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/auth_token.py
--rw-r--r--   0        0        0     4479 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/config.py
--rw-r--r--   0        0        0     1156 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/main.py
--rw-r--r--   0        0        0     2089 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/shell_commands.py
--rw-r--r--   0        0        0     4701 2023-04-20 19:28:04.753344 poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/plugin.py
--rw-r--r--   0        0        0     1088 2023-04-20 19:28:05.709350 poc_poetry_partifact_plugin-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0        3 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/__init__.py
+-rw-r--r--   0        0        0     1478 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/auth_token.py
+-rw-r--r--   0        0        0     4479 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/config.py
+-rw-r--r--   0        0        0     1156 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/main.py
+-rw-r--r--   0        0        0     2089 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/shell_commands.py
+-rw-r--r--   0        0        0     4935 2023-04-20 19:49:58.122591 poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/plugin.py
+-rw-r--r--   0        0        0     1088 2023-04-20 19:49:58.958588 poc_poetry_partifact_plugin-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      784 1970-01-01 00:00:00.000000 poc_poetry_partifact_plugin-0.9.0/PKG-INFO
```

### Comparing `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/auth_token.py` & `poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/auth_token.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/config.py` & `poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/config.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/main.py` & `poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/main.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/partifact/shell_commands.py` & `poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/partifact/shell_commands.py`

 * *Files identical despite different names*

### Comparing `poc_poetry_partifact_plugin-0.8.0/poc_poetry_partifact_plugin/plugin.py` & `poc_poetry_partifact_plugin-0.9.0/poc_poetry_partifact_plugin/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,19 @@
             return
 
         if not any(isinstance(command, t) for t in [InstallCommand, AddCommand]):
             # Only run the plugin for install and add commands
             return
 
         # run a codeartifact login command
-        login(repository="aws", profile="amino-shared")
+        try:
+            login(repository="aws", profile="amino-shared", role=None)
+            io.write_line("<fg=green>aws codeartifact successfully configured</info>")
+        except Exception as e:
+            io.write_error_line(f"<error>Failed to configure aws codeartifact: {e}</>")
 
     def _handle_post_command(
         self, event: ConsoleTerminateEvent, event_name: str, dispatcher: EventDispatcher
     ) -> None:
         if event.exit_code != 0:
             # The command failed, so the plugin shouldn't do anything
             # if the event was a "HTTPSConnectionPool" error, then try to login
```

### Comparing `poc_poetry_partifact_plugin-0.8.0/pyproject.toml` & `poc_poetry_partifact_plugin-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poc-poetry-partifact-plugin"
-version = "0.8.0"
+version = "0.9.0"
 description = "A POC poetry plugin that configure partifact"
 authors = ["timothestes <timothestes@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "poc_poetry_partifact_plugin" },
 ]
 homepage = "https://github.com/timothestes/poc-poetry-partifact-plugin"
```

### Comparing `poc_poetry_partifact_plugin-0.8.0/PKG-INFO` & `poc_poetry_partifact_plugin-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poc-poetry-partifact-plugin
-Version: 0.8.0
+Version: 0.9.0
 Summary: A POC poetry plugin that configure partifact
 Home-page: https://github.com/timothestes/poc-poetry-partifact-plugin
 Author: timothestes
 Author-email: timothestes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

