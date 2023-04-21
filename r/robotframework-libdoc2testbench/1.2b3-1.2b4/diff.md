# Comparing `tmp/robotframework-libdoc2testbench-1.2b3.tar.gz` & `tmp/robotframework-libdoc2testbench-1.2b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-libdoc2testbench-1.2b3.tar", last modified: Fri Apr 21 08:29:54 2023, max compression
+gzip compressed data, was "robotframework-libdoc2testbench-1.2b4.tar", last modified: Fri Apr 21 08:33:05 2023, max compression
```

## Comparing `robotframework-libdoc2testbench-1.2b3.tar` & `robotframework-libdoc2testbench-1.2b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.499087 robotframework-libdoc2testbench-1.2b3/
--rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b3/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)      182 2022-02-01 11:40:46.000000 robotframework-libdoc2testbench-1.2b3/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:29:54.498786 robotframework-libdoc2testbench-1.2b3/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)     6163 2022-02-01 11:41:54.000000 robotframework-libdoc2testbench-1.2b3/README.md
--rw-r--r--   0 rener      (502) wheel        (0)     1671 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b3/Setup.py
--rwxr-xr-x   0 rener      (502) wheel        (0)      171 2023-04-21 08:20:32.000000 robotframework-libdoc2testbench-1.2b3/createPip_whl_tar.sh
--rw-r--r--   0 rener      (502) wheel        (0)     1431 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b3/pyproject.toml
--rw-r--r--   0 rener      (502) wheel        (0)       38 2023-04-21 08:29:54.499185 robotframework-libdoc2testbench-1.2b3/setup.cfg
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.491671 robotframework-libdoc2testbench-1.2b3/src/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.495339 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/
--rw-r--r--   0 rener      (502) wheel        (0)    10474 2023-04-21 08:28:55.000000 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)      852 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__main__.py
--rw-r--r--   0 rener      (502) wheel        (0)    22953 2023-04-21 08:24:38.000000 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/testbenchwriter.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.498369 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/
--rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)      545 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/dependency_links.txt
--rw-r--r--   0 rener      (502) wheel        (0)      118 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/entry_points.txt
--rw-r--r--   0 rener      (502) wheel        (0)       53 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/requires.txt
--rw-r--r--   0 rener      (502) wheel        (0)       17 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/top_level.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.082648 robotframework-libdoc2testbench-1.2b4/
+-rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b4/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)      182 2022-02-01 11:40:46.000000 robotframework-libdoc2testbench-1.2b4/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:33:05.082358 robotframework-libdoc2testbench-1.2b4/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     6163 2022-02-01 11:41:54.000000 robotframework-libdoc2testbench-1.2b4/README.md
+-rw-r--r--   0 rener      (502) wheel        (0)     1671 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b4/Setup.py
+-rwxr-xr-x   0 rener      (502) wheel        (0)      171 2023-04-21 08:20:32.000000 robotframework-libdoc2testbench-1.2b4/createPip_whl_tar.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     1431 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b4/pyproject.toml
+-rw-r--r--   0 rener      (502) wheel        (0)       38 2023-04-21 08:33:05.082740 robotframework-libdoc2testbench-1.2b4/setup.cfg
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.075831 robotframework-libdoc2testbench-1.2b4/src/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.079561 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/
+-rw-r--r--   0 rener      (502) wheel        (0)    10474 2023-04-21 08:32:19.000000 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)      852 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__main__.py
+-rw-r--r--   0 rener      (502) wheel        (0)    22962 2023-04-21 08:32:08.000000 robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/testbenchwriter.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:33:05.081945 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)      545 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      118 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       53 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       17 2023-04-21 08:33:05.000000 robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/top_level.txt
```

### Comparing `robotframework-libdoc2testbench-1.2b3/LICENSE` & `robotframework-libdoc2testbench-1.2b4/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b3/PKG-INFO` & `robotframework-libdoc2testbench-1.2b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-libdoc2testbench
-Version: 1.2b3
+Version: 1.2b4
 Summary: Robot Framework Libdoc Extension that generates imbus TestBench Library import formats.
 Home-page: https://github.com/imbus/robotframework-libdoc2testbench
 Author: imbus AG | Maximilian Birkenhagen
 Author-email: maximilian.birkenhagen@imbus.de
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-libdoc2testbench-1.2b3/README.md` & `robotframework-libdoc2testbench-1.2b4/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b3/Setup.py` & `robotframework-libdoc2testbench-1.2b4/Setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b3/pyproject.toml` & `robotframework-libdoc2testbench-1.2b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__init__.py` & `robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from robot.libdocpkg import LibraryDocumentation
 from robot.libdocpkg.robotbuilder import LibraryDoc
 from robot.version import get_full_version as robot_version_print
 
 from .testbenchwriter import Libdoc2TestBenchWriter
 
-__version__ = "1.2b3"
+__version__ = "1.2b4"
 
 
 def start_libdoc2testbench():
     """Command line entry point for the Libdoc2TestBench module."""
     parser = argparse.ArgumentParser(
         description="""Robot Framework Libdoc Extension that generates imbus
                     TestBench Library import formats. The easiest way to run
```

### Comparing `robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__main__.py` & `robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/testbenchwriter.py` & `robotframework-libdoc2testbench-1.2b4/src/Libdoc2TestBench/testbenchwriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,15 +477,15 @@
 
         for datatype_idx, data_type in enumerate(datatypes.values()):
             writer.start('element', {'type': ElementTypes.datatype.value})
             writer.element('pk', data_type.pk)
             writer.element('name', data_type.get_name())
             writer.element('uid', self._generate_UID('DT', data_type.name, libdoc.name))
             writer.element('locker', '')
-			writer.element('html-description', data_type.html_desc.replace('<br>', '<br/>').replace('<hr>', '<br>'))
+            writer.element('html-description', data_type.html_desc.replace('<br>', '<br/>').replace('<hr>', '<br>'))
             writer.element('historyPK', '-1')
             writer.element('identicalVersionPK', '-1')
             writer.start('equivalence-classes')
             for ec_name, ec_members in data_type.equivalence_classes.items():
                 writer.start('equivalence-class')
                 writer.element('pk', self.pk_generator.get_pk())
                 writer.element('name', ec_name)
```

### Comparing `robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/PKG-INFO` & `robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-libdoc2testbench
-Version: 1.2b3
+Version: 1.2b4
 Summary: Robot Framework Libdoc Extension that generates imbus TestBench Library import formats.
 Home-page: https://github.com/imbus/robotframework-libdoc2testbench
 Author: imbus AG | Maximilian Birkenhagen
 Author-email: maximilian.birkenhagen@imbus.de
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt` & `robotframework-libdoc2testbench-1.2b4/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

