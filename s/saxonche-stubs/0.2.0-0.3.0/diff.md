# Comparing `tmp/saxonche_stubs-0.2.0.tar.gz` & `tmp/saxonche_stubs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saxonche_stubs-0.2.0.tar", max compression
+gzip compressed data, was "saxonche_stubs-0.3.0.tar", max compression
```

## Comparing `saxonche_stubs-0.2.0.tar` & `saxonche_stubs-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      686 2023-04-20 17:10:55.421979 saxonche_stubs-0.2.0/README.md
--rw-r--r--   0        0        0      684 2023-04-21 15:02:32.477664 saxonche_stubs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5201 2023-04-21 14:43:15.182623 saxonche_stubs-0.2.0/saxonche-stubs/__init__.pyi
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 saxonche_stubs-0.2.0/setup.py
--rw-r--r--   0        0        0     1313 1970-01-01 00:00:00.000000 saxonche_stubs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      490 2023-04-21 15:06:15.152853 saxonche_stubs-0.3.0/README.md
+-rw-r--r--   0        0        0     1572 2023-04-21 15:30:13.967154 saxonche_stubs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7464 2023-04-21 15:27:32.263455 saxonche_stubs-0.3.0/saxonche-stubs/__init__.pyi
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 saxonche_stubs-0.3.0/setup.py
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 saxonche_stubs-0.3.0/PKG-INFO
```

### Comparing `saxonche_stubs-0.2.0/setup.py` & `saxonche_stubs-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['saxonche>=12.1.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'saxonche-stubs',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Type stubs for saxonche',
-    'long_description': '# saxonche-stubs\n\nType stubs for the [saxonche](https://pypi.org/project/saxonche/) python package. This package has no functionality itself, but is merely an addition to the completion within IDEs. The basis for type annotations and comments is the documentation of [the Saxon Python API](https://www.saxonica.com/saxon-c/doc11/html/saxonc.html).\n\nAt the moment not all APIs are fully typed. To install the stubs just install the git repo via poetry or any other package manager.\n\nYou can use `stubtest` to get an impression of untyped components:\n\n```sh\npoetry run stubtest saxonche\n```\n\n## Author / Contact\n\n- [Bastian Politycki](https://github.com/Bpolitycki) – Swiss Law Sources\n',
+    'long_description': '# saxonche-stubs\n\nType stubs for the [saxonche](https://pypi.org/project/saxonche/) python package. This package has no functionality itself, but is merely an addition to the completion within IDEs. The basis for type annotations and comments is the documentation of [the Saxon Python API](https://www.saxonica.com/saxon-c/doc11/html/saxonc.html).\n\nAt the moment not all APIs are fully typed.\n\n## Author / Contact\n\n- [Bastian Politycki](https://github.com/Bpolitycki) – Swiss Law Sources\n',
     'author': 'Bpolitycki',
     'author_email': 'bastian.politycki@unisg.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

