# Comparing `tmp/testgear-adapter-pytest-2.1.1.tar.gz` & `tmp/testgear-adapter-pytest-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgear-adapter-pytest-2.1.1.tar", last modified: Fri Mar 31 06:31:25 2023, max compression
+gzip compressed data, was "testgear-adapter-pytest-2.1.2.tar", last modified: Fri Apr 21 14:56:06 2023, max compression
```

## Comparing `testgear-adapter-pytest-2.1.1.tar` & `testgear-adapter-pytest-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 06:31:25.363318 testgear-adapter-pytest-2.1.1/
--rw-rw-rw-   0        0        0    14810 2023-03-31 06:31:25.363318 testgear-adapter-pytest-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11760 2023-03-31 06:28:55.000000 testgear-adapter-pytest-2.1.1/README.md
--rw-rw-rw-   0        0        0      113 2023-01-19 07:55:39.000000 testgear-adapter-pytest-2.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 06:31:25.363318 testgear-adapter-pytest-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1007 2023-03-31 06:28:55.000000 testgear-adapter-pytest-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:31:25.357214 testgear-adapter-pytest-2.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 06:31:25.362213 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest/
--rw-rw-rw-   0        0        0        0 2023-03-22 12:27:08.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest/__init__.py
--rw-rw-rw-   0        0        0     7533 2023-03-27 12:00:18.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest/listener.py
--rw-rw-rw-   0        0        0     3621 2023-03-27 12:00:18.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest/plugin.py
-drwxrwxrwx   0        0        0        0 2023-03-31 06:31:25.363318 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest.egg-info/
--rw-rw-rw-   0        0        0    14810 2023-03-31 06:31:25.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-03-31 06:31:25.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 06:31:25.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-03-31 06:31:25.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-03-31 06:31:25.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-03-31 06:31:25.000000 testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/
+-rw-rw-rw-   0        0        0    12314 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11760 2023-03-31 06:28:55.000000 testgear-adapter-pytest-2.1.2/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-21 13:48:08.000000 testgear-adapter-pytest-2.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-04-21 14:03:30.000000 testgear-adapter-pytest-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.315995 testgear-adapter-pytest-2.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.315995 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/
+-rw-rw-rw-   0        0        0        0 2023-04-21 13:47:37.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/__init__.py
+-rw-rw-rw-   0        0        0     7533 2023-04-21 13:57:30.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/listener.py
+-rw-rw-rw-   0        0        0     3621 2023-04-21 13:58:22.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:56:06.331037 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/
+-rw-rw-rw-   0        0        0    12314 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-21 14:56:06.000000 testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testgear-adapter-pytest-2.1.1/README.md` & `testgear-adapter-pytest-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `testgear-adapter-pytest-2.1.1/setup.py` & `testgear-adapter-pytest-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testgear-adapter-pytest',
-    version='2.1.1',
+    version='2.1.2',
     description='Pytest adapter for Test Gear',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testgear-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@test-gear.io',
     license='Apache-2.0',
@@ -16,10 +16,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testgear_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'testgear-python-commons==2.1.1'],
+    install_requires=['pytest', 'pytest-xdist', 'testgear-python-commons==2.1.2'],
     entry_points={'pytest11': ['testgear_adapter_pytest = testgear_adapter_pytest.plugin']}
 )
```

### Comparing `testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest/listener.py` & `testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/listener.py`

 * *Files identical despite different names*

### Comparing `testgear-adapter-pytest-2.1.1/src/testgear_adapter_pytest/plugin.py` & `testgear-adapter-pytest-2.1.2/src/testgear_adapter_pytest/plugin.py`

 * *Files identical despite different names*

