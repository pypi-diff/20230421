# Comparing `tmp/robotframework-libdoc2testbench-1.2b2.tar.gz` & `tmp/robotframework-libdoc2testbench-1.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-libdoc2testbench-1.2b2.tar", last modified: Fri Nov  4 10:46:25 2022, max compression
+gzip compressed data, was "robotframework-libdoc2testbench-1.2b3.tar", last modified: Fri Apr 21 08:29:54 2023, max compression
```

## Comparing `robotframework-libdoc2testbench-1.2b2.tar` & `robotframework-libdoc2testbench-1.2b3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-04 10:46:25.489715 robotframework-libdoc2testbench-1.2b2/
--rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b2/LICENSE
--rw-r--r--   0 rener      (502) wheel        (0)      182 2022-02-01 11:40:46.000000 robotframework-libdoc2testbench-1.2b2/MANIFEST.in
--rw-r--r--   0 rener      (502) wheel        (0)     7062 2022-11-04 10:46:25.489390 robotframework-libdoc2testbench-1.2b2/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)     6163 2022-02-01 11:41:54.000000 robotframework-libdoc2testbench-1.2b2/README.md
--rw-r--r--   0 rener      (502) wheel        (0)     1626 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b2/Setup.py
--rwxrwxrwx   0 rener      (502) wheel        (0)      171 2021-06-02 08:26:07.000000 robotframework-libdoc2testbench-1.2b2/createPip_whl_tar.sh
--rw-r--r--   0 rener      (502) wheel        (0)       38 2022-11-04 10:46:25.489784 robotframework-libdoc2testbench-1.2b2/setup.cfg
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-04 10:46:25.483419 robotframework-libdoc2testbench-1.2b2/src/
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-04 10:46:25.486426 robotframework-libdoc2testbench-1.2b2/src/Libdoc2TestBench/
--rw-r--r--   0 rener      (502) wheel        (0)    10474 2022-11-04 10:46:06.000000 robotframework-libdoc2testbench-1.2b2/src/Libdoc2TestBench/__init__.py
--rw-r--r--   0 rener      (502) wheel        (0)      852 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b2/src/Libdoc2TestBench/__main__.py
--rw-r--r--   0 rener      (502) wheel        (0)    18305 2022-11-04 10:46:06.000000 robotframework-libdoc2testbench-1.2b2/src/Libdoc2TestBench/testbenchwriter.py
-drwxr-xr-x   0 rener      (502) wheel        (0)        0 2022-11-04 10:46:25.489013 robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/
--rw-r--r--   0 rener      (502) wheel        (0)     7062 2022-11-04 10:46:25.000000 robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/PKG-INFO
--rw-r--r--   0 rener      (502) wheel        (0)      530 2022-11-04 10:46:25.000000 robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt
--rw-r--r--   0 rener      (502) wheel        (0)        1 2022-11-04 10:46:25.000000 robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/dependency_links.txt
--rw-r--r--   0 rener      (502) wheel        (0)      119 2022-11-04 10:46:25.000000 robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/entry_points.txt
--rw-r--r--   0 rener      (502) wheel        (0)       22 2022-11-04 10:46:25.000000 robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/requires.txt
--rw-r--r--   0 rener      (502) wheel        (0)       17 2022-11-04 10:46:25.000000 robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/top_level.txt
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.499087 robotframework-libdoc2testbench-1.2b3/
+-rw-r--r--   0 rener      (502) wheel        (0)    11339 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b3/LICENSE
+-rw-r--r--   0 rener      (502) wheel        (0)      182 2022-02-01 11:40:46.000000 robotframework-libdoc2testbench-1.2b3/MANIFEST.in
+-rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:29:54.498786 robotframework-libdoc2testbench-1.2b3/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)     6163 2022-02-01 11:41:54.000000 robotframework-libdoc2testbench-1.2b3/README.md
+-rw-r--r--   0 rener      (502) wheel        (0)     1671 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b3/Setup.py
+-rwxr-xr-x   0 rener      (502) wheel        (0)      171 2023-04-21 08:20:32.000000 robotframework-libdoc2testbench-1.2b3/createPip_whl_tar.sh
+-rw-r--r--   0 rener      (502) wheel        (0)     1431 2023-04-21 08:18:41.000000 robotframework-libdoc2testbench-1.2b3/pyproject.toml
+-rw-r--r--   0 rener      (502) wheel        (0)       38 2023-04-21 08:29:54.499185 robotframework-libdoc2testbench-1.2b3/setup.cfg
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.491671 robotframework-libdoc2testbench-1.2b3/src/
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.495339 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/
+-rw-r--r--   0 rener      (502) wheel        (0)    10474 2023-04-21 08:28:55.000000 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__init__.py
+-rw-r--r--   0 rener      (502) wheel        (0)      852 2021-05-25 11:38:22.000000 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__main__.py
+-rw-r--r--   0 rener      (502) wheel        (0)    22953 2023-04-21 08:24:38.000000 robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/testbenchwriter.py
+drwxr-xr-x   0 rener      (502) wheel        (0)        0 2023-04-21 08:29:54.498369 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/
+-rw-r--r--   0 rener      (502) wheel        (0)     7046 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/PKG-INFO
+-rw-r--r--   0 rener      (502) wheel        (0)      545 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt
+-rw-r--r--   0 rener      (502) wheel        (0)        1 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/dependency_links.txt
+-rw-r--r--   0 rener      (502) wheel        (0)      118 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/entry_points.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       53 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/requires.txt
+-rw-r--r--   0 rener      (502) wheel        (0)       17 2023-04-21 08:29:54.000000 robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/top_level.txt
```

### Comparing `robotframework-libdoc2testbench-1.2b2/LICENSE` & `robotframework-libdoc2testbench-1.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b2/PKG-INFO` & `robotframework-libdoc2testbench-1.2b3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: robotframework-libdoc2testbench
-Version: 1.2b2
+Version: 1.2b3
 Summary: Robot Framework Libdoc Extension that generates imbus TestBench Library import formats.
 Home-page: https://github.com/imbus/robotframework-libdoc2testbench
 Author: imbus AG | Maximilian Birkenhagen
 Author-email: maximilian.birkenhagen@imbus.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Libdoc2TestBench
 Robot Framework Libdoc Extension that generates imbus [TestBench Enterprise](https://www.imbus.de/en/testbench-enterprise) Library import formats.
 It can be used to generate Testbench interactions from Robotframework keywords.
 ___
 
@@ -171,8 +170,7 @@
 ___
 ### Contributing
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 For consistent code formatting, please use [Black - The Uncompromising Code Formatter](https://github.com/psf/black) with the following arguments in the root directory:
 ```bash
 black -l 100 -S .
 ```
-
```

### Comparing `robotframework-libdoc2testbench-1.2b2/README.md` & `robotframework-libdoc2testbench-1.2b3/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b2/Setup.py` & `robotframework-libdoc2testbench-1.2b3/Setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from setuptools import setup
-from setuptools import find_packages
 import re
 from os.path import abspath, dirname, join
 
+from setuptools import find_packages, setup
+
 CURDIR = dirname(abspath(__file__))
 
 with open(join(CURDIR, "src", "Libdoc2TestBench", "__init__.py"), encoding="utf-8") as f:
     VERSION = re.search('\n__version__ = "(.*)"', f.read()).group(1)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
@@ -35,9 +35,10 @@
         "Operating System :: OS Independent",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Software Development :: Testing",
         "Topic :: Software Development :: Testing :: Acceptance",
         "Framework :: Robot Framework",
     ],
     install_requires=["robotframework >= 4.0.0"],
+    extras_require={'dev': ['isort', 'mypy', 'pylint', 'black']},
     python_requires=">=3.7",
 )
```

### Comparing `robotframework-libdoc2testbench-1.2b2/src/Libdoc2TestBench/__init__.py` & `robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import argparse
 import os
 import re
-import sys
-import argparse
 import shutil
+import sys
 from pathlib import Path
 from zipfile import ZipFile
 
-from .testbenchwriter import Libdoc2TestBenchWriter
 from robot.libdocpkg import LibraryDocumentation
-from robot.version import get_full_version as robot_version_print
 from robot.libdocpkg.robotbuilder import LibraryDoc
+from robot.version import get_full_version as robot_version_print
 
-__version__ = "1.2b2"
+from .testbenchwriter import Libdoc2TestBenchWriter
+
+__version__ = "1.2b3"
 
 
 def start_libdoc2testbench():
     """Command line entry point for the Libdoc2TestBench module."""
     parser = argparse.ArgumentParser(
         description="""Robot Framework Libdoc Extension that generates imbus
                     TestBench Library import formats. The easiest way to run
@@ -195,15 +196,14 @@
         outfile_path = (
             outfile_path
             if os.path.splitext(outfile_path)[1].lower() == '.zip'
             else f"{outfile_path}.zip"
         )
 
     with open(project_dump_path, "w", encoding='UTF-8') as outfile:
-
         # The write method returns the last issued primary key.
         Libdoc2TestBenchWriter().write(
             libraries,
             resources,
             outfile,
             repo_id,
             library_root,
```

### Comparing `robotframework-libdoc2testbench-1.2b2/src/Libdoc2TestBench/__main__.py` & `robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-libdoc2testbench-1.2b2/src/Libdoc2TestBench/testbenchwriter.py` & `robotframework-libdoc2testbench-1.2b3/src/Libdoc2TestBench/testbenchwriter.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This code contains derived code from Robot Framework Core Project
 #  under Apache 2.0 License.
 #  https://github.com/robotframework/robotframework
 
-import enum, os
+import enum
+import os
 from datetime import datetime
 from hashlib import sha1
 from pathlib import Path
-from typing import List
+from typing import Dict, List, Optional, Set
 
-from robot.utils import XmlWriter
 from robot.libdocpkg.robotbuilder import LibraryDoc
+from robot.running.arguments.argumentspec import ArgInfo
+from robot.utils import XmlWriter
 
 
 class ElementTypes(enum.Enum):
     """Enum for different test elements found in the imbus TestBench."""
 
     subdivision = 'subdivision'
     datatype = 'datatype'
@@ -59,64 +61,59 @@
 
 class Element:
     """A class to represent imbus TestBench related test elements."""
 
     # Remember all created element objects and their associated pk.
     all_elements = {}
 
-    def __init__(self, pk_generator: PKGenerator, element, parent_element=None):
-        self.element = element
-        self.pk = pk_generator.get_pk()
-        self.parent = parent_element
-
-        if element["doc"]:
-            self.html_desc = f"<html>{element['doc']}</html>"
-
-        self._set_name_and_register_in_all_elements()
-
-    def _set_name_and_register_in_all_elements(self):
-        # Each element's name is build via its hierarchy.
-        # If it has a parent, the parent's name will be the prefix.
-        if self.parent:
-            self.name = self.parent.name + '.' + self.element.name
+    def __init__(self, pk_generator: PKGenerator, name, documentation="", parent_element=None):
+        self.html_desc = f"<html>{documentation}</html>"
+        if parent_element:
+            self.name = parent_element.name + '.' + name
         else:
-            self.name = self.element['name']
-
+            self.name = name
         # Register element for later access to element's unique pk
+        self.pk = pk_generator.get_pk()
         Element.all_elements[self.name] = self.pk
 
     def get_name(self) -> str:
         # Returns the element's name without the parent-prefix.
         return self.name.split('.', 1)[-1]
 
 
 class DataType(Element):
     """A class used to gather information for imbus TestBench
     data types from the associated Robot Framework data type.
     Each Robot Framework data type is converted into one
     "members" equivalence class and each valid value is one
     representative in the imbus TestBench."""
 
-    def __init__(self, pk_generator: PKGenerator, data_type, parent_element=None):
-        super().__init__(pk_generator, data_type)
-        self.type = data_type['type']
+    def __init__(
+        self, pk_generator: PKGenerator, name: str, documentation: str = "", parent_element=None
+    ):
+        super().__init__(pk_generator, name, documentation, parent_element)
 
         # Holds all enum values, typed_dics are considered to be
         # generic for imbus TestBench purposes.
+        self.pk_generator = pk_generator
+        self.equivalence_classes: Dict[str, Set[str]] = {}
         self.representatives = {}
+        self.name = name
 
-        if self.type == 'Enum':
-            self.members = data_type['members']
-            for member in self.members:
-                key = f"{self.name}.{member['name']}"
-                value = f"{self.name}.{member['value']}"
-                self.representatives[key] = value
-
-                # Register in all_elements dic for later access of pks.
-                Element.all_elements[key] = pk_generator.get_pk()
+    def add_equivalence_class(
+        self, equivalence_class_name: str, members: Optional[Set[str]] = None
+    ):
+        existing_eqivalence_class = self.equivalence_classes.get(equivalence_class_name)
+        if not existing_eqivalence_class:
+            self.equivalence_classes[equivalence_class_name] = set()
+        if members:
+            for member in members:
+                if (Element.all_elements.get(f"{self.name}.{member}")) is None:
+                    self.equivalence_classes[equivalence_class_name].add(member)
+                    Element.all_elements[f"{self.name}.{member}"] = self.pk_generator.get_pk()
 
 
 class Libdoc2TestBenchWriter:
     """A class to generate imbus TestBench readable xml-files from Robot Framework
     libraries.
 
     Methods
@@ -131,15 +128,15 @@
     testobject_state = ProjectStates.active.value
     testobject_desc = "Robot Framework Import"
     created_time = f"{datetime.utcnow().strftime('%Y-%m-%d %H:%M:%S')} +0000"
     libdoc_name = None  # set-up in write() method.
     attachment_reference_pk = {}  # Needed for resource files - holds exactly one pk
 
     # Attributes used in the header of the xml-file
-    xml_attributes = {'version': "2.6.1", 'build-number': "201215/dcee", 'repository': "iTB_RF"}
+    xml_attributes = {'version': "3.0", 'build-number': "230202/6a0c", 'repository': "iTB_RF"}
 
     # Values used to fill imbus TestBench project settings.
     project_settings = {
         'overwrite-exec-responsible': 'false',
         'optional-checkin': 'false',
         'filter-sync-interval': '30',
         'ignore-not-edited': 'false',
@@ -210,22 +207,24 @@
         self._write_start(writer)
         if attachment:
             self._write_attachments(resources, writer)
         self._start_testobjectversion(writer)
         if libraries:
             self._start_root_subdivision(writer, library_root, 'Robot Framework Libraries')
             for libdoc in libraries:
+                Element.all_elements = {}
                 self._start_library_subdivision(libdoc, writer)
                 self._write_data_types(libdoc, writer)
                 self._write_interactions(libdoc, writer)
                 self._end_library_subdivision(writer)
             self._end_root_subdivision(writer)
         if resources:
             self._start_root_subdivision(writer, resource_root, 'Robot Framework Resource Files')
             for libdoc in resources:
+                Element.all_elements = {}
                 self._start_library_subdivision(libdoc, writer)
                 self._write_data_types(libdoc, writer)
                 self._write_interactions(libdoc, writer, attachment)
                 self._end_library_subdivision(writer)
             self._end_root_subdivision(writer)
         self._end_testobjectversion(writer)
         self._write_end(writer)
@@ -318,108 +317,201 @@
             'html-description',
             f"<html><p> Import of {libdoc.name} {libdoc.version}</p>{libdoc.doc}</html>",
         )
         writer.element('historyPK', '-1')
         writer.element('identicalVersionPK', '-1')
         writer.element('references', '')
 
+    def _get_argument_name_prefix(self, argument_kind: str) -> str:
+        if argument_kind == ArgInfo.VAR_POSITIONAL:
+            return "* "
+        elif argument_kind == ArgInfo.VAR_NAMED:
+            return "** "
+        elif argument_kind == ArgInfo.NAMED_ONLY:
+            return "- "
+        return ""
+
     def _write_interactions(self, libdoc, writer, attachment=False):
-        for keyword in libdoc.keywords:
+        libdoc_dic = libdoc.to_dictionary()
+        for keyword in libdoc_dic["keywords"]:
             writer.start('element', {'type': ElementTypes.interaction.value})
             writer.element('pk', self.pk_generator.get_pk())
-            writer.element('name', keyword.name)
-            writer.element('uid', self._generate_UID('IA', keyword.name, libdoc.name))
+            writer.element('name', keyword['name'])
+            writer.element('uid', self._generate_UID('IA', keyword['name'], libdoc.name))
             writer.element('locker', '')
             writer.element('status', '3')
-            writer.element('html-description', f"<html>{keyword.doc.replace('<br>', '<br/>').replace('<hr>', '<br>')}</html>")
+            writer.element('html-description', f"<html>{keyword['doc'].replace('<br>', '<br/>').replace('<hr>', '<br>')}</html>")
             writer.element('historyPK', '-1')
             writer.element('identicalVersionPK', '-1')
             writer.start('references')
 
             if attachment:
                 writer.element(
                     'reference-ref', attrs={'pk': self.attachment_reference_pk[libdoc.name]}
                 )
-
             writer.end('references')
             writer.start('parameters')
-            for arg in keyword.args:
+            for arg in keyword['args']:
+                argument_kind = arg.get('kind')
+                if (
+                    not argument_kind
+                    or argument_kind == ArgInfo.POSITIONAL_ONLY_MARKER
+                    or argument_kind == ArgInfo.NOTSET
+                ):
+                    continue
                 writer.start('parameter')
                 writer.element('pk', self.pk_generator.get_pk())
-                writer.element('name', arg.name)
-                # For each parameter of the keyword, check whether
-                # it is already in the all_elements dic
-                # and thus already has a key.
-                # If not, its a generic data type => -1
-                typ_pk = '-1'
-                for typ in arg.types_reprs:
-                    typ_pk = Element.all_elements.get(typ, '-1')
-                    if typ_pk != '-1':
-                        break
-                # datatype-ref provides the mapping in the testbench
+                argument_name_prefix = self._get_argument_name_prefix(argument_kind)
+                writer.element('name', f"{argument_name_prefix}{arg['name']}")
+                type_name = self._get_datatype_name(arg)
+                typ_pk = Element.all_elements.get(type_name, '-1')
+
                 writer.element('datatype-ref', '', {'pk': typ_pk})
                 writer.element('definition-type', '0')
                 writer.element('use-type', '1')
+                writer.element('datatype-name', type_name)
+                default_value = arg.get('defaultValue')
+                if default_value is None:
+                    default_value = self._get_arg_kind_default_value(argument_kind)
+                if default_value is not None:
+                    writer.start('default-value', {'type': 'representative'})
+                    writer.element('type', '1')
+                    representative_pk = Element.all_elements.get(
+                        f"{type_name}.{default_value}", '-1'
+                    )
+                    writer.element('representative-ref', '', {'pk': representative_pk})
+                    writer.element('representative-name', default_value)
+                    writer.end('default-value')
                 writer.end('parameter')
             writer.end('parameters')
             writer.end('element')  # close interaction tag
 
+    def _get_arg_kind_default_value(self, argument_kind: str) -> Optional[str]:
+        if argument_kind == ArgInfo.VAR_POSITIONAL:
+            return "@{EMPTY}"
+        elif argument_kind == ArgInfo.VAR_NAMED:
+            return "&{EMPTY}"
+        return None
+
+    def _get_datatype_name(self, argument: Dict[str, str]) -> str:
+        for argument_type in argument.get('typedocs', {}).values():
+            if argument_type in self.enum_types or argument_type in self.typed_dicts:
+                return argument_type
+        return argument.get('name', "")
+
+    def _get_datatype_documentation(self, datatype_name, libdoc_dic: Dict[str, any]) -> str:
+        if datatype_name in self.enum_types:
+            return next(
+                filter(lambda enum: enum['name'] == datatype_name, libdoc_dic['dataTypes']['enums'])
+            ).get('doc', '')
+        if datatype_name in self.typed_dicts:
+            return next(
+                filter(
+                    lambda typedDict: typedDict['name'] == datatype_name,
+                    libdoc_dic['dataTypes']['typedDicts'],
+                )
+            ).get('doc', '')
+        return ""
+
+    def _get_enum_types(self, libdoc_dic: Dict[str, any]) -> Set[str]:
+        return {enum.get('name') for enum in libdoc_dic.get('dataTypes').get('enums')}
+
+    def _get_typed_dicts(self, libdoc_dic: Dict[str, any]) -> Set[str]:
+        return {enum.get('name') for enum in libdoc_dic.get('dataTypes').get('typedDicts')}
+
     def _write_data_types(self, libdoc: LibraryDoc, writer):
-        datatypes = []
         libdoc_dic = libdoc.to_dictionary()
-        if libdoc_dic["dataTypes"]["enums"]:
-            for data_type in libdoc_dic["dataTypes"]["enums"]:
-                datatypes.append(DataType(self.pk_generator, data_type))
+        self.enum_types = set(self._get_enum_types(libdoc_dic))
+        self.typed_dicts = self._get_typed_dicts(libdoc_dic)
 
-            writer.start('element', {'type': ElementTypes.subdivision.value})
-            writer.element('pk', self.pk_generator.get_pk())
-            writer.element('name', '_Datatypes')
-            writer.element('uid', self._generate_UID('SD', '_Datatypes', libdoc.name))
+        datatypes = {}
+        keyword_arguments = [
+            argument for keyword in libdoc_dic['keywords'] for argument in keyword['args']
+        ]
+        for argument in keyword_arguments:
+            argument_kind = argument.get('kind')
+            if (
+                not argument_kind
+                or argument_kind == ArgInfo.POSITIONAL_ONLY_MARKER
+                or argument_kind == ArgInfo.NOTSET
+            ):
+                continue
+            datatype_name = self._get_datatype_name(argument)
+            datatype_documentation = self._get_datatype_documentation(datatype_name, libdoc_dic)
+            datatype = datatypes.get(datatype_name) or DataType(
+                self.pk_generator, datatype_name, datatype_documentation
+            )
+            default_value = argument.get('defaultValue')
+            if default_value is None:
+                default_value = self._get_arg_kind_default_value(argument_kind)
+            for idx, type_name in enumerate(argument.get('typedocs', {}).keys()):
+                members = set()
+                if type_name == "bool":
+                    members = {'True', 'False', '${True}', '${False}'}
+                    datatype.add_equivalence_class(type_name, members)
+                elif type_name in self.enum_types:
+                    members_list = next(
+                        filter(
+                            lambda enum: enum['name'] == datatype_name,
+                            libdoc_dic['dataTypes']['enums'],
+                        )
+                    ).get('members', [])
+                    members = {member.get('name') for member in members_list}
+                    datatype.add_equivalence_class(type_name, members)
+            if default_value == "None":
+                datatype.add_equivalence_class("None", {default_value})
+            else:
+                datatype.add_equivalence_class(datatype_name, {default_value})
+            datatype.add_equivalence_class(datatype_name)
+            datatypes[datatype_name] = datatype
+
+        writer.start('element', {'type': ElementTypes.subdivision.value})
+        writer.element('pk', self.pk_generator.get_pk())
+        writer.element('name', '_Datatypes')
+        writer.element('uid', self._generate_UID('SD', '_Datatypes', libdoc.name))
+        writer.element('locker', '')
+        writer.element('status', '3')
+        writer.element('html-description', '')
+        writer.element('historyPK', '-1')
+        writer.element('identicalVersionPK', '-1')
+        writer.element('references', '')
+
+        for datatype_idx, data_type in enumerate(datatypes.values()):
+            writer.start('element', {'type': ElementTypes.datatype.value})
+            writer.element('pk', data_type.pk)
+            writer.element('name', data_type.get_name())
+            writer.element('uid', self._generate_UID('DT', data_type.name, libdoc.name))
             writer.element('locker', '')
-            writer.element('status', '3')
-            writer.element('html-description', '')
+			writer.element('html-description', data_type.html_desc.replace('<br>', '<br/>').replace('<hr>', '<br>'))
             writer.element('historyPK', '-1')
             writer.element('identicalVersionPK', '-1')
-            writer.element('references', '')
-
-            for idx, data_type in enumerate(datatypes):
-                writer.start('element', {'type': ElementTypes.datatype.value})
-                writer.element('pk', data_type.pk)
-                writer.element('name', data_type.get_name())
-                writer.element('uid', self._generate_UID('DT', data_type.name, libdoc.name))
-                writer.element('locker', '')
-                writer.element('html-description', data_type.html_desc.replace('<br>', '<br/>').replace('<hr>', '<br>'))
-                writer.element('historyPK', '-1')
-                writer.element('identicalVersionPK', '-1')
-                writer.start('equivalence-classes')
+            writer.start('equivalence-classes')
+            for ec_name, ec_members in data_type.equivalence_classes.items():
                 writer.start('equivalence-class')
                 writer.element('pk', self.pk_generator.get_pk())
-                writer.element('name', 'members')
-                writer.element('description', 'Valid members')
-                writer.element('ordering', str(1024 * idx))
-
+                writer.element('name', ec_name)
+                writer.element('description', ec_name)
+                writer.element('ordering', str(1024 * datatype_idx))
                 writer.start('representatives')
                 default_pk = '-1'
-                for idx, representative in enumerate(data_type.representatives.keys()):
+                for idx, representative in enumerate(ec_members):
                     writer.start('representative')
-                    pk = Element.all_elements[representative]
+                    pk = Element.all_elements[f"{data_type.get_name()}.{representative}"]
                     if idx == 0:
-                        # if non-generic => set default-representative
                         default_pk = pk
                     writer.element('pk', pk)
-                    writer.element('name', representative.split(f"{data_type.get_name()}.", 1)[-1])
+                    writer.element('name', representative)
                     writer.element('ordering', str(1024 * (idx + 1)))
                     writer.end('representative')
-
                 writer.end('representatives')
                 writer.element('default-representative-ref', '', {'pk': default_pk})
                 writer.end('equivalence-class')
-                writer.end('equivalence-classes')
-                writer.end('element')  # close dataType tag
-            writer.end('element')  # close datatype subdivision tag
+            writer.end('equivalence-classes')
+            writer.end('element')  # close dataType tag
+        writer.end('element')  # close datatype subdivision tag
 
     def _end_library_subdivision(self, writer):
         writer.end('element')  # close Library Subdivision tag
 
     def _end_root_subdivision(self, writer):
         writer.end('element')  # close RF or Resource subdivision tag
```

### Comparing `robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/PKG-INFO` & `robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: robotframework-libdoc2testbench
-Version: 1.2b2
+Version: 1.2b3
 Summary: Robot Framework Libdoc Extension that generates imbus TestBench Library import formats.
 Home-page: https://github.com/imbus/robotframework-libdoc2testbench
 Author: imbus AG | Maximilian Birkenhagen
 Author-email: maximilian.birkenhagen@imbus.de
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Acceptance
 Classifier: Framework :: Robot Framework
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Libdoc2TestBench
 Robot Framework Libdoc Extension that generates imbus [TestBench Enterprise](https://www.imbus.de/en/testbench-enterprise) Library import formats.
 It can be used to generate Testbench interactions from Robotframework keywords.
 ___
 
@@ -171,8 +170,7 @@
 ___
 ### Contributing
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 For consistent code formatting, please use [Black - The Uncompromising Code Formatter](https://github.com/psf/black) with the following arguments in the root directory:
 ```bash
 black -l 100 -S .
 ```
-
```

### Comparing `robotframework-libdoc2testbench-1.2b2/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt` & `robotframework-libdoc2testbench-1.2b3/src/robotframework_libdoc2testbench.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 Setup.py
 createPip_whl_tar.sh
+pyproject.toml
 setup.py
 src/Libdoc2TestBench/__init__.py
 src/Libdoc2TestBench/__main__.py
 src/Libdoc2TestBench/testbenchwriter.py
 src/robotframework_libdoc2testbench.egg-info/PKG-INFO
 src/robotframework_libdoc2testbench.egg-info/SOURCES.txt
 src/robotframework_libdoc2testbench.egg-info/dependency_links.txt
```

