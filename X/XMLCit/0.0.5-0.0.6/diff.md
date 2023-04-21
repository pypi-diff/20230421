# Comparing `tmp/xmlcit-0.0.5.tar.gz` & `tmp/XMLCit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "XMLCit-0.0.6.tar", last modified: Thu Apr 20 03:34:13 2023, max compression
```

## Comparing `xmlcit-0.0.5.tar` & `XMLCit-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,22 @@
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/__init__.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/addtagfunc.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/tagfunctions.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/VIAF_functions/VIAFreffun.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/VIAF_functions/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/opcit_functions/Ibidfunc.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 xmlcit-0.0.5/src/opcit_functions/__init__.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 xmlcit-0.0.5/LICENSE
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 xmlcit-0.0.5/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xmlcit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 xmlcit-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 03:34:13.976060 XMLCit-0.0.6/
+-rw-rw-rw-   0        0        0     1086 2023-04-20 02:25:43.000000 XMLCit-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1220 2023-04-20 03:34:13.977053 XMLCit-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-04-20 02:44:02.000000 XMLCit-0.0.6/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-20 03:33:56.000000 XMLCit-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-04-20 03:34:13.979046 XMLCit-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 03:34:13.950300 XMLCit-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 03:34:13.956267 XMLCit-0.0.6/src/VIAFfunctions/
+-rw-rw-rw-   0        0        0     4572 2023-04-20 00:39:27.000000 XMLCit-0.0.6/src/VIAFfunctions/VIAFreffun.py
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:24:16.000000 XMLCit-0.0.6/src/VIAFfunctions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:34:13.970608 XMLCit-0.0.6/src/XMLCit.egg-info/
+-rw-rw-rw-   0        0        0     1220 2023-04-20 03:34:13.000000 XMLCit-0.0.6/src/XMLCit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-04-20 03:34:13.000000 XMLCit-0.0.6/src/XMLCit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 03:34:13.000000 XMLCit-0.0.6/src/XMLCit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 03:34:13.000000 XMLCit-0.0.6/src/XMLCit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 03:34:13.972956 XMLCit-0.0.6/src/opcitfunctions/
+-rw-rw-rw-   0        0        0     3610 2023-04-20 00:39:07.000000 XMLCit-0.0.6/src/opcitfunctions/Ibidfunc.py
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:24:00.000000 XMLCit-0.0.6/src/opcitfunctions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 03:34:13.976060 XMLCit-0.0.6/src/tagfunctions/
+-rw-rw-rw-   0        0        0        0 2023-04-20 03:24:08.000000 XMLCit-0.0.6/src/tagfunctions/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-04-20 00:38:46.000000 XMLCit-0.0.6/src/tagfunctions/addtagfunc.py
+-rw-rw-rw-   0        0        0     5588 2023-04-20 00:39:24.000000 XMLCit-0.0.6/src/tagfunctions/tagfunctions.py
```

### Comparing `xmlcit-0.0.5/src/addtagfunc.py` & `XMLCit-0.0.6/src/tagfunctions/addtagfunc.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.5/src/tagfunctions.py` & `XMLCit-0.0.6/src/tagfunctions/tagfunctions.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.5/src/VIAF_functions/VIAFreffun.py` & `XMLCit-0.0.6/src/VIAFfunctions/VIAFreffun.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.5/src/opcit_functions/Ibidfunc.py` & `XMLCit-0.0.6/src/opcitfunctions/Ibidfunc.py`

 * *Files identical despite different names*

### Comparing `xmlcit-0.0.5/LICENSE` & `XMLCit-0.0.6/LICENSE`

 * *Files identical despite different names*

