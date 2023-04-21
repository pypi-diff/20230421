# Comparing `tmp/prelude-cli-1.0.0.tar.gz` & `tmp/prelude-cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.0.0.tar", last modified: Tue Apr 18 19:09:56 2023, max compression
+gzip compressed data, was "prelude-cli-1.0.1.tar", last modified: Fri Apr 21 19:57:04 2023, max compression
```

## Comparing `prelude-cli-1.0.0.tar` & `prelude-cli-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.637009 prelude-cli-1.0.0/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-18 19:09:56.637062 prelude-cli-1.0.0/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.0.0/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.633476 prelude-cli-1.0.0/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1243 2023-04-18 14:03:55.000000 prelude-cli-1.0.0/prelude_cli/cli.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.634751 prelude-cli-1.0.0/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-1.0.0/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.636792 prelude-cli-1.0.0/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-1.0.0/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.0.0/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     6089 2023-04-18 17:04:09.000000 prelude-cli-1.0.0/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3763 2023-04-18 14:03:55.000000 prelude-cli-1.0.0/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)    29181 2023-04-18 17:04:09.000000 prelude-cli-1.0.0/prelude_cli/views/interactive.py
--rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-1.0.0/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-1.0.0/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.634528 prelude-cli-1.0.0/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       59 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      690 2023-04-18 19:09:56.637282 prelude-cli-1.0.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.978189 prelude-cli-1.0.1/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-21 19:57:04.978257 prelude-cli-1.0.1/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.0.1/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.974379 prelude-cli-1.0.1/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1243 2023-04-18 14:03:55.000000 prelude-cli-1.0.1/prelude_cli/cli.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.975671 prelude-cli-1.0.1/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-1.0.1/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.977982 prelude-cli-1.0.1/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-1.0.1/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.0.1/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     6089 2023-04-18 17:04:09.000000 prelude-cli-1.0.1/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3757 2023-04-21 19:52:17.000000 prelude-cli-1.0.1/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    29181 2023-04-18 17:04:09.000000 prelude-cli-1.0.1/prelude_cli/views/interactive.py
+-rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-1.0.1/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-1.0.1/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-21 19:57:04.975461 prelude-cli-1.0.1/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       59 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-21 19:57:04.000000 prelude-cli-1.0.1/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.0.1/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      690 2023-04-21 19:57:04.978511 prelude-cli-1.0.1/setup.cfg
```

### Comparing `prelude-cli-1.0.0/LICENSE` & `prelude-cli-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/PKG-INFO` & `prelude-cli-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.0.0/prelude_cli/cli.py` & `prelude-cli-1.0.1/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/prelude_cli/views/build.py` & `prelude-cli-1.0.1/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/prelude_cli/views/configure.py` & `prelude-cli-1.0.1/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/prelude_cli/views/detect.py` & `prelude-cli-1.0.1/prelude_cli/views/detect.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/prelude_cli/views/iam.py` & `prelude-cli-1.0.1/prelude_cli/views/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
 def delete_user(controller, handle):
     """ Remove a user from your account """
     controller.delete_user(handle=handle)
 
 
 @iam.command('attach-partner')
 @click.argument('name')
-@click.option('--api', required=True, help='API endpoint of the partner')
-@click.option('--user', required=True, help='user identifier')
+@click.option('--api', default='', help='API endpoint of the partner')
+@click.option('--user', default='', help='user identifier')
 @click.option('--secret', default='', help='secret for OAUTH use cases')
 @click.pass_obj
 @handle_api_error
 def attach_partner(controller, name, api, user, secret):
     """ Attach an EDR to Detect """
     controller.attach_partner(name=name, api=api, user=user, secret=secret)
```

### Comparing `prelude-cli-1.0.0/prelude_cli/views/interactive.py` & `prelude-cli-1.0.1/prelude_cli/views/interactive.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/prelude_cli/views/partner.py` & `prelude-cli-1.0.1/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.0.1/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.0.0/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.0.1/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.0/setup.cfg` & `prelude-cli-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.0.0
+version = 1.0.1
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.0.0
+	prelude-sdk == 1.0.1
 	click
 	rich
 	simple-term-menu
 	gnureadline
 
 [options.entry_points]
 console_scripts =
```

