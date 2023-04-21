# Comparing `tmp/trops-0.2.8.tar.gz` & `tmp/trops-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trops-0.2.8.tar", last modified: Thu Apr 21 12:44:16 2022, max compression
+gzip compressed data, was "trops-0.2.9.tar", last modified: Mon Apr 25 15:08:14 2022, max compression
```

## Comparing `trops-0.2.8.tar` & `trops-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-21 12:44:16.097496 trops-0.2.8/
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     1068 2021-12-17 00:39:25.000000 trops-0.2.8/LICENSE
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     3568 2022-04-21 12:44:16.097496 trops-0.2.8/PKG-INFO
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     2382 2022-04-07 13:11:07.000000 trops-0.2.8/README.rst
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)       38 2022-04-21 12:44:16.097496 trops-0.2.8/setup.cfg
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)      875 2022-04-21 12:41:33.000000 trops-0.2.8/setup.py
-drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-21 12:44:16.093496 trops-0.2.8/src/
-drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-21 12:44:16.093496 trops-0.2.8/src/trops/
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)      577 2022-04-17 14:14:23.000000 trops-0.2.8/src/trops/__init__.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)    10311 2022-04-17 14:14:23.000000 trops-0.2.8/src/trops/capcmd.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)    13315 2022-04-17 14:14:23.000000 trops-0.2.8/src/trops/env.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     4559 2022-04-21 12:41:21.000000 trops-0.2.8/src/trops/exec.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     2465 2022-04-21 02:38:17.000000 trops-0.2.8/src/trops/file.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     3352 2022-04-17 14:14:23.000000 trops-0.2.8/src/trops/init.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     7127 2022-04-21 01:53:23.000000 trops-0.2.8/src/trops/koumyo.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)       22 2022-04-21 12:41:33.000000 trops-0.2.8/src/trops/release.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     3695 2022-04-17 14:14:23.000000 trops-0.2.8/src/trops/repo.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)    10600 2022-04-21 12:41:21.000000 trops-0.2.8/src/trops/trops.py
--rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)      510 2022-04-17 14:14:23.000000 trops-0.2.8/src/trops/utils.py
-drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-21 12:44:16.097496 trops-0.2.8/src/trops.egg-info/
--rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)     3568 2022-04-21 12:44:16.000000 trops-0.2.8/src/trops.egg-info/PKG-INFO
--rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)      437 2022-04-21 12:44:16.000000 trops-0.2.8/src/trops.egg-info/SOURCES.txt
--rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)        1 2022-04-21 12:44:16.000000 trops-0.2.8/src/trops.egg-info/dependency_links.txt
--rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)       43 2022-04-21 12:44:16.000000 trops-0.2.8/src/trops.egg-info/entry_points.txt
--rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)       16 2022-04-21 12:44:16.000000 trops-0.2.8/src/trops.egg-info/requires.txt
--rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)        6 2022-04-21 12:44:16.000000 trops-0.2.8/src/trops.egg-info/top_level.txt
+drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-25 15:08:14.075832 trops-0.2.9/
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     1068 2021-12-17 00:39:25.000000 trops-0.2.9/LICENSE
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     3568 2022-04-25 15:08:14.075832 trops-0.2.9/PKG-INFO
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     2382 2022-04-07 13:11:07.000000 trops-0.2.9/README.rst
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)       38 2022-04-25 15:08:14.075832 trops-0.2.9/setup.cfg
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)      875 2022-04-25 15:07:41.000000 trops-0.2.9/setup.py
+drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-25 15:08:14.071831 trops-0.2.9/src/
+drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-25 15:08:14.075832 trops-0.2.9/src/trops/
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)      577 2022-04-17 14:14:23.000000 trops-0.2.9/src/trops/__init__.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)    10359 2022-04-25 15:07:41.000000 trops-0.2.9/src/trops/capcmd.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)    13315 2022-04-17 14:14:23.000000 trops-0.2.9/src/trops/env.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     4559 2022-04-21 12:41:21.000000 trops-0.2.9/src/trops/exec.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     2465 2022-04-21 02:38:17.000000 trops-0.2.9/src/trops/file.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     3352 2022-04-17 14:14:23.000000 trops-0.2.9/src/trops/init.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     7699 2022-04-25 15:07:41.000000 trops-0.2.9/src/trops/koumyo.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)       22 2022-04-25 15:07:41.000000 trops-0.2.9/src/trops/release.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     3695 2022-04-17 14:14:23.000000 trops-0.2.9/src/trops/repo.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)    10600 2022-04-21 12:41:21.000000 trops-0.2.9/src/trops/trops.py
+-rw-rw-r--   0 ktanaka   (1000) ktanaka   (1000)     1559 2022-04-25 15:07:41.000000 trops-0.2.9/src/trops/utils.py
+drwxrwxr-x   0 ktanaka   (1000) ktanaka   (1000)        0 2022-04-25 15:08:14.075832 trops-0.2.9/src/trops.egg-info/
+-rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)     3568 2022-04-25 15:08:14.000000 trops-0.2.9/src/trops.egg-info/PKG-INFO
+-rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)      437 2022-04-25 15:08:14.000000 trops-0.2.9/src/trops.egg-info/SOURCES.txt
+-rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)        1 2022-04-25 15:08:14.000000 trops-0.2.9/src/trops.egg-info/dependency_links.txt
+-rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)       43 2022-04-25 15:08:14.000000 trops-0.2.9/src/trops.egg-info/entry_points.txt
+-rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)       16 2022-04-25 15:08:14.000000 trops-0.2.9/src/trops.egg-info/requires.txt
+-rw-r--r--   0 ktanaka   (1000) ktanaka   (1000)        6 2022-04-25 15:08:14.000000 trops-0.2.9/src/trops.egg-info/top_level.txt
```

### Comparing `trops-0.2.8/LICENSE` & `trops-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/PKG-INFO` & `trops-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trops
-Version: 0.2.8
+Version: 0.2.9
 Summary: Track operations
 Home-page: http://github.com/kojiwell/trops
 Author: Koji Tanaka
 Author-email: kojiwelly@gmail.com
 License: MIT
 Description: ******************************
         Trops tracks system operations
```

### Comparing `trops-0.2.8/README.rst` & `trops-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/setup.py` & `trops-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setuptools.setup(
     name="trops",
-    version="0.2.8",
+    version="0.2.9",
     author="Koji Tanaka",
     author_email="kojiwelly@gmail.com",
     description=("Track operations"),
     long_description_content_type="text/x-rst",
     license="MIT",
     keywords="linux system administration",
     url="http://github.com/kojiwell/trops",
```

### Comparing `trops-0.2.8/src/trops/__init__.py` & `trops-0.2.9/src/trops/__init__.py`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/src/trops/capcmd.py` & `trops-0.2.9/src/trops/capcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,16 @@
         if executed_cmd[0] in editors:
             # Add the edited file in trops git
             for ii in executed_cmd[1:]:
                 ii_path = absolute_path(ii)
                 if os.path.isfile(ii_path):
                     # Ignore the file if it is under a git repository
                     ii_parent_dir = os.path.dirname(ii_path)
-                    os.chdir(ii_parent_dir)
+                    if ii_parent_dir != '':
+                        os.chdir(ii_parent_dir)
                     cmd = ['git', 'rev-parse', '--is-inside-work-tree']
                     result = subprocess.run(cmd, capture_output=True)
                     if result.returncode == 0:
                         self.logger.info(
                             f"FL { ii_path } is under a git repository #> PWD=*, EXIT=*, TROPS_SID={ self.trops_sid }, TROPS_ENV={ self.trops_env }")
                         exit(0)
                     # Check if the path is in the git repo
```

### Comparing `trops-0.2.8/src/trops/env.py` & `trops-0.2.9/src/trops/env.py`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/src/trops/exec.py` & `trops-0.2.9/src/trops/exec.py`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/src/trops/file.py` & `trops-0.2.9/src/trops/file.py`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/src/trops/init.py` & `trops-0.2.9/src/trops/init.py`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/src/trops/koumyo.py` & `trops-0.2.9/src/trops/koumyo.py`

 * *Files 8% similar despite different names*

```diff
@@ -134,26 +134,39 @@
                         formatted_log[i] = n.replace(
                             'TROPS_ENV=', '').rstrip(',')
                     elif 'TROPS_TAGS=' in n:
                         formatted_log[i] = n.replace(
                             'TROPS_TAGS=', '').rstrip(',')
                 while len(formatted_log) < 10:
                     formatted_log.append('-')
-            headers = ['date', 'time', 'user',
-                       'level', 'type', 'command', 'directory', 'exit', 'id', 'env', 'tags']
+            dict_headers = {
+                '%D': 'Date',
+                '%T': 'Time',
+                '%u': 'User@host',
+                '%ll': 'Log level',
+                '%lt': 'Log type',
+                '%c': 'Command',
+                '%d': 'Directory/O,G,M',
+                '%x': 'Excode',
+                '%i': 'ID',
+                '%e': 'Env',
+                '%t': 'Tags'}
+            headers = []
+            for k, v in dict_headers.items():
+                headers.append(f'{v}[{k}]')
             # if --only is added, pick the only chosen elements
-            if hasattr(self, 'only_list'):
+            if hasattr(self, 'only_list') and self.args.all != True:
                 i = []
                 selected_log = []
                 selected_headers = []
                 for item in self.only_list:
-                    i.append(headers.index(item))
+                    i.append(list(dict_headers.keys()).index(item))
                 for index in i:
                     selected_log.append(formatted_log[index])
-                    selected_headers.append(headers[index])
+                    selected_headers.append(list(dict_headers.values())[index])
                 headers = selected_headers
                 formatted_logs.append(selected_log)
             else:
                 formatted_logs.append(formatted_log)
         if self.args.markdown:
             print(tabulate(formatted_logs, headers, tablefmt="github"))
         elif self.args.html:
@@ -172,21 +185,24 @@
     tk.run()
 
 
 def add_koumyo_subparsers(subparsers):
 
     # trops koumyo
     parser_koumyo = subparsers.add_parser(
-        'km', help='(KM)Kou-Myo sheds light on trops log')
+        'km', help=dedent('kou-myo(km) sheds light on trops log'))
     parser_koumyo.add_argument(
-        '-o', '--only',
-        help='list of items (e.g. --only=command,directory')
+        '-o', '--only', default='%D,%T,%u,%c,%d',
+        help='list of items (default: %(default)s)')
     parser_koumyo.add_argument(
-        '--no-declutter', action='store_true',
+        '-n', '--no-declutter', action='store_true',
         help='disable log-decluttering')
+    parser_koumyo.add_argument(
+        '-a', '--all', action='store_true',
+        help='all items in the log')
     group = parser_koumyo.add_mutually_exclusive_group()
     group.add_argument(
         '-m', '--markdown', action='store_true',
         help='markdown table format')
     group.add_argument(
         '--html', action='store_true',
         help='HTML table format')
```

### Comparing `trops-0.2.8/src/trops/repo.py` & `trops-0.2.9/src/trops/repo.py`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/src/trops/trops.py` & `trops-0.2.9/src/trops/trops.py`

 * *Files identical despite different names*

### Comparing `trops-0.2.8/src/trops.egg-info/PKG-INFO` & `trops-0.2.9/src/trops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trops
-Version: 0.2.8
+Version: 0.2.9
 Summary: Track operations
 Home-page: http://github.com/kojiwell/trops
 Author: Koji Tanaka
 Author-email: kojiwelly@gmail.com
 License: MIT
 Description: ******************************
         Trops tracks system operations
```

