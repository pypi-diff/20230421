# Comparing `tmp/dumbo_ae-0.1.3.tar.gz` & `tmp/dumbo_ae-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_ae-0.1.3.tar", max compression
+gzip compressed data, was "dumbo_ae-0.1.4.tar", max compression
```

## Comparing `dumbo_ae-0.1.3.tar` & `dumbo_ae-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-02-14 15:19:00.095165 dumbo_ae-0.1.3/LICENSE
--rw-r--r--   0        0        0      496 2023-02-14 15:28:05.842208 dumbo_ae-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-02-14 15:19:00.095165 dumbo_ae-0.1.3/dumbo_ae/__init__.py
--rw-r--r--   0        0        0       98 2023-02-14 15:27:05.567462 dumbo_ae-0.1.3/dumbo_ae/__main__.py
--rwxr-xr-x   0        0        0     2638 2023-02-14 15:19:00.095165 dumbo_ae-0.1.3/dumbo_ae/cli.py
--rw-r--r--   0        0        0      403 2023-02-14 15:36:30.720697 dumbo_ae-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 dumbo_ae-0.1.3/setup.py
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 dumbo_ae-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-14 15:19:00.095165 dumbo_ae-0.1.4/LICENSE
+-rw-r--r--   0        0        0      496 2023-02-14 15:28:05.842208 dumbo_ae-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-02-14 15:19:00.095165 dumbo_ae-0.1.4/dumbo_ae/__init__.py
+-rw-r--r--   0        0        0       98 2023-02-14 15:27:05.567462 dumbo_ae-0.1.4/dumbo_ae/__main__.py
+-rwxr-xr-x   0        0        0     2660 2023-04-21 18:23:50.848350 dumbo_ae-0.1.4/dumbo_ae/cli.py
+-rw-r--r--   0        0        0      403 2023-04-21 18:23:50.836350 dumbo_ae-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 dumbo_ae-0.1.4/setup.py
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 dumbo_ae-0.1.4/PKG-INFO
```

### Comparing `dumbo_ae-0.1.3/LICENSE` & `dumbo_ae-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_ae-0.1.3/dumbo_ae/cli.py` & `dumbo_ae-0.1.4/dumbo_ae/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         console.print("dumbo-ae", __version__)
         raise typer.Exit()
 
 
 @app.callback()
 def main(
         local_server: bool = typer.Option(False, "--local-server", help="Use a DEV local server"),
-        debug: bool = typer.Option(False, "--debug", help="Don't minimize browser"),
+        debug: bool = typer.Option(False, "--debug", help="Report more detailed errors (for developers)"),
         version: bool = typer.Option(False, "--version", callback=version_callback, is_eager=True,
                                      help="Print version and exit"),
 ):
     """
     CLI per il corso di Architettura degli Elaboratori.
     """
     global app_options
```

### Comparing `dumbo_ae-0.1.3/setup.py` & `dumbo_ae-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['dumbo-utils>=0.1.6,<0.2.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'dumbo-ae',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'CLI per il corso di Architettura degli Elaboratori',
     'long_description': "# Dumbo Architettura degli Elaboratori\n\nUna semplice interfaccia a linea di comando per il corso di Architettura degli Eleboratori.\n\n\n## Prerequisiti\n\nPython 3.10+\n\n## Installazione\n\nIl modo più semplice è usare pip:\n\n```bash\n$ pip3 install dumbo-ae\n```\n\n\n## Uso\n\nPer controllare la propria soluzione a un esercizio è necessario indicare l'UUID dell'esercizio (fornito in aula) e il file sorgente della propria soluzione: \n```bash\n$ python3 -m dumbo_ae checker --of <UUID> <file-sorgente>\n```\n",
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dumbo_ae-0.1.3/PKG-INFO` & `dumbo_ae-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbo-ae
-Version: 0.1.3
+Version: 0.1.4
 Summary: CLI per il corso di Architettura degli Elaboratori
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

