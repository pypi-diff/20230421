# Comparing `tmp/cumulus_kern-0.0.1.tar.gz` & `tmp/cumulus_kern-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_kern-0.0.1.tar", last modified: Fri Apr 21 00:17:11 2023, max compression
+gzip compressed data, was "cumulus_kern-0.0.2.tar", last modified: Fri Apr 21 00:42:32 2023, max compression
```

## Comparing `cumulus_kern-0.0.1.tar` & `cumulus_kern-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 00:17:11.237056 cumulus_kern-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 cumulus_kern-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      409 2023-04-21 00:17:11.236757 cumulus_kern-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-20 20:27:18.000000 cumulus_kern-0.0.1/README.md
--rw-rw-rw-   0        0        0      221 2023-04-21 00:16:05.000000 cumulus_kern-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 00:17:11.238058 cumulus_kern-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      697 2023-04-21 00:14:41.000000 cumulus_kern-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 00:17:11.195246 cumulus_kern-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-21 00:17:11.235056 cumulus_kern-0.0.1/src/cumulus_kern.egg-info/
--rw-rw-rw-   0        0        0      409 2023-04-21 00:17:11.000000 cumulus_kern-0.0.1/src/cumulus_kern.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-04-21 00:17:11.000000 cumulus_kern-0.0.1/src/cumulus_kern.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 00:17:11.000000 cumulus_kern-0.0.1/src/cumulus_kern.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 00:17:11.000000 cumulus_kern-0.0.1/src/cumulus_kern.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 00:42:32.542954 cumulus_kern-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 cumulus_kern-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1580 2023-04-21 00:42:32.544020 cumulus_kern-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-20 20:27:18.000000 cumulus_kern-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 00:42:32.410473 cumulus_kern-0.0.2/cumulus_kern.egg-info/
+-rw-rw-rw-   0        0        0     1580 2023-04-21 00:42:32.000000 cumulus_kern-0.0.2/cumulus_kern.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-04-21 00:42:32.000000 cumulus_kern-0.0.2/cumulus_kern.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 00:42:32.000000 cumulus_kern-0.0.2/cumulus_kern.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-21 00:42:32.000000 cumulus_kern-0.0.2/cumulus_kern.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      225 2023-04-21 00:23:51.000000 cumulus_kern-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      596 2023-04-21 00:42:32.558404 cumulus_kern-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      705 2023-04-21 00:41:24.000000 cumulus_kern-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 00:42:32.540953 cumulus_kern-0.0.2/src/
+-rw-rw-rw-   0        0        0      522 2023-02-13 21:12:26.000000 cumulus_kern-0.0.2/src/RequestHandler.py
+-rw-rw-rw-   0        0        0    14421 2023-02-13 13:17:25.000000 cumulus_kern-0.0.2/src/SharePointHandler.py
+-rw-rw-rw-   0        0        0     2250 2023-02-20 20:06:50.000000 cumulus_kern-0.0.2/src/TableLogHandler.py
+-rw-rw-rw-   0        0        0        0 2022-05-17 10:12:58.000000 cumulus_kern-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     8815 2023-02-21 02:51:22.000000 cumulus_kern-0.0.2/src/brzGlobal.py
+-rw-rw-rw-   0        0        0     4990 2023-04-18 16:46:19.000000 cumulus_kern-0.0.2/src/gbtGlobal.py
+-rw-rw-rw-   0        0        0    13474 2023-04-16 12:34:10.000000 cumulus_kern-0.0.2/src/mstAst.py
+-rw-rw-rw-   0        0        0      823 2023-04-20 21:56:20.000000 cumulus_kern-0.0.2/src/mstLog.py
```

### Comparing `cumulus_kern-0.0.1/LICENSE` & `cumulus_kern-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cumulus_kern-0.0.1/setup.py` & `cumulus_kern-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='cumulus_kern',  
-     version='0.0.1',
-     author="BayWa Data Services GmbH",
+     version='0.0.2',
+     author="BayWa r.e. Data Services GmbH",
      author_email="no-reply@baywa-re.com",
      description="Kernel functions for Cumulus",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/nino-baywa/cumulus_kern",
      classifiers=[
          "Programming Language :: Python :: 3",
          "Operating System :: OS Independent",
      ],
-    package_dir = {"": "src"},
+    package_dir = {"src": "src"},
     packages = setuptools.find_packages(where="src"),
     python_requires = ">=3.8"
  )
```

