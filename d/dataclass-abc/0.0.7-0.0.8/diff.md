# Comparing `tmp/dataclass_abc-0.0.7.tar.gz` & `tmp/dataclass-abc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_abc-0.0.7.tar", last modified: Tue Jan 31 09:04:07 2023, max compression
+gzip compressed data, was "dataclass-abc-0.0.8.tar", last modified: Fri Apr 21 06:53:52 2023, max compression
```

## Comparing `dataclass_abc-0.0.7.tar` & `dataclass-abc-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:04:07.168627 dataclass_abc-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-01-31 09:03:51.000000 dataclass_abc-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-01-31 09:04:07.168627 dataclass_abc-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-31 09:03:51.000000 dataclass_abc-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:04:07.168627 dataclass_abc-0.0.7/dataclass_abc/
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-01-31 09:03:51.000000 dataclass_abc-0.0.7/dataclass_abc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 09:04:07.168627 dataclass_abc-0.0.7/dataclass_abc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-01-31 09:04:07.000000 dataclass_abc-0.0.7/dataclass_abc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-31 09:04:07.000000 dataclass_abc-0.0.7/dataclass_abc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 09:04:07.000000 dataclass_abc-0.0.7/dataclass_abc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-31 09:04:07.000000 dataclass_abc-0.0.7/dataclass_abc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 09:04:07.168627 dataclass_abc-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-01-31 09:03:51.000000 dataclass_abc-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:53:52.394163 dataclass-abc-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-21 06:53:37.000000 dataclass-abc-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-21 06:53:52.394163 dataclass-abc-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-21 06:53:37.000000 dataclass-abc-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:53:52.394163 dataclass-abc-0.0.8/dataclass_abc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-21 06:53:52.000000 dataclass-abc-0.0.8/dataclass_abc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-21 06:53:52.000000 dataclass-abc-0.0.8/dataclass_abc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:53:52.000000 dataclass-abc-0.0.8/dataclass_abc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 06:53:52.000000 dataclass-abc-0.0.8/dataclass_abc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:53:52.394163 dataclass-abc-0.0.8/dataclassabc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-21 06:53:37.000000 dataclass-abc-0.0.8/dataclassabc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:53:52.394163 dataclass-abc-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-21 06:53:37.000000 dataclass-abc-0.0.8/setup.py
```

### Comparing `dataclass_abc-0.0.7/LICENSE` & `dataclass-abc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_abc-0.0.7/PKG-INFO` & `dataclass-abc-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
-Name: dataclass_abc
-Version: 0.0.7
+Name: dataclass-abc
+Version: 0.0.8
 Summary: Library that lets you define abstract properties for dataclasses.
 Home-page: https://github.com/MichaelSchneeberger/dataclass-abc
 Author: Michael Schneeberger
 Author-email: michael.schneeb@outlook.com
-Keywords: dataclass_abc abstract abc property
+Keywords: dataclass-abc abstract abc property
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dataclass ABC
@@ -18,42 +18,42 @@
 
 ## Installation
 
 ```pip install dataclass-abc```
 
 ## Usage
 
-The `dataclass_abc` class decorator resolves the abstract properties 
+The `dataclassabc` class decorator resolves the abstract properties 
 overwritten by a field.
 
 ``` python
 from abc import ABC, abstractmethod
 
-from dataclass_abc import dataclass_abc
+from dataclassabc import dataclassabc
 
 class A(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
-@dataclass_abc(frozen=True)
+@dataclassabc(frozen=True)
 class B(A):
     name: str        # overwrites the abstract property 'name' in 'A'
 ```
 
 ## Define mutable variables
 
 Define a mutable variable `name` in the abstract class `A` by using the
 `name.setter` decorator. 
 
 ``` python
 from abc import ABC, abstractmethod
 
-from dataclass_abc import dataclass_abc
+from dataclassabc import dataclassabc
 
 class A(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
@@ -61,15 +61,15 @@
     @abstractmethod
     def name(self, val: str):
         ...
 
     def set_name(self, val: str):
         self.name = val
 
-@dataclass_abc
+@dataclassabc
 class B(A):
     name: str
 
 b = B(name='A')
 b.set_name('B')
 ```
 
@@ -86,11 +86,11 @@
 - **mixins** - a *mixin* is an abstract class that implements data as abstract
 properties and methods based on the abstract properties.
 - **classes** - an abstract class inherits from one or more mixins
 (see `City` or `CapitalCity` in the example). This class is used for pattern matching,
 e.g. using `isinstance` method.
 - **impl** - an *implementation class* implements the abstract properties. 
 (see `CityImpl` or `CapitalCityImpl` in the example). This class is decorated with
-`dataclass_abc` and `resolve_abc_prop` and should always be called through an 
+`dataclassabc` and `resolve_abc_prop` and should always be called through an 
 *initialize function*.
 - **init** - an *initialize function* (or *constructor function*) initializes an 
 *implementation class*.
```

### Comparing `dataclass_abc-0.0.7/README.md` & `dataclass-abc-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,42 +4,42 @@
 
 ## Installation
 
 ```pip install dataclass-abc```
 
 ## Usage
 
-The `dataclass_abc` class decorator resolves the abstract properties 
+The `dataclassabc` class decorator resolves the abstract properties 
 overwritten by a field.
 
 ``` python
 from abc import ABC, abstractmethod
 
-from dataclass_abc import dataclass_abc
+from dataclassabc import dataclassabc
 
 class A(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
-@dataclass_abc(frozen=True)
+@dataclassabc(frozen=True)
 class B(A):
     name: str        # overwrites the abstract property 'name' in 'A'
 ```
 
 ## Define mutable variables
 
 Define a mutable variable `name` in the abstract class `A` by using the
 `name.setter` decorator. 
 
 ``` python
 from abc import ABC, abstractmethod
 
-from dataclass_abc import dataclass_abc
+from dataclassabc import dataclassabc
 
 class A(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
@@ -47,15 +47,15 @@
     @abstractmethod
     def name(self, val: str):
         ...
 
     def set_name(self, val: str):
         self.name = val
 
-@dataclass_abc
+@dataclassabc
 class B(A):
     name: str
 
 b = B(name='A')
 b.set_name('B')
 ```
 
@@ -72,11 +72,11 @@
 - **mixins** - a *mixin* is an abstract class that implements data as abstract
 properties and methods based on the abstract properties.
 - **classes** - an abstract class inherits from one or more mixins
 (see `City` or `CapitalCity` in the example). This class is used for pattern matching,
 e.g. using `isinstance` method.
 - **impl** - an *implementation class* implements the abstract properties. 
 (see `CityImpl` or `CapitalCityImpl` in the example). This class is decorated with
-`dataclass_abc` and `resolve_abc_prop` and should always be called through an 
+`dataclassabc` and `resolve_abc_prop` and should always be called through an 
 *initialize function*.
 - **init** - an *initialize function* (or *constructor function*) initializes an 
 *implementation class*.
```

### Comparing `dataclass_abc-0.0.7/dataclass_abc.egg-info/PKG-INFO` & `dataclass-abc-0.0.8/dataclass_abc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: dataclass-abc
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library that lets you define abstract properties for dataclasses.
 Home-page: https://github.com/MichaelSchneeberger/dataclass-abc
 Author: Michael Schneeberger
 Author-email: michael.schneeb@outlook.com
-Keywords: dataclass_abc abstract abc property
+Keywords: dataclass-abc abstract abc property
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dataclass ABC
@@ -18,42 +18,42 @@
 
 ## Installation
 
 ```pip install dataclass-abc```
 
 ## Usage
 
-The `dataclass_abc` class decorator resolves the abstract properties 
+The `dataclassabc` class decorator resolves the abstract properties 
 overwritten by a field.
 
 ``` python
 from abc import ABC, abstractmethod
 
-from dataclass_abc import dataclass_abc
+from dataclassabc import dataclassabc
 
 class A(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
-@dataclass_abc(frozen=True)
+@dataclassabc(frozen=True)
 class B(A):
     name: str        # overwrites the abstract property 'name' in 'A'
 ```
 
 ## Define mutable variables
 
 Define a mutable variable `name` in the abstract class `A` by using the
 `name.setter` decorator. 
 
 ``` python
 from abc import ABC, abstractmethod
 
-from dataclass_abc import dataclass_abc
+from dataclassabc import dataclassabc
 
 class A(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
@@ -61,15 +61,15 @@
     @abstractmethod
     def name(self, val: str):
         ...
 
     def set_name(self, val: str):
         self.name = val
 
-@dataclass_abc
+@dataclassabc
 class B(A):
     name: str
 
 b = B(name='A')
 b.set_name('B')
 ```
 
@@ -86,11 +86,11 @@
 - **mixins** - a *mixin* is an abstract class that implements data as abstract
 properties and methods based on the abstract properties.
 - **classes** - an abstract class inherits from one or more mixins
 (see `City` or `CapitalCity` in the example). This class is used for pattern matching,
 e.g. using `isinstance` method.
 - **impl** - an *implementation class* implements the abstract properties. 
 (see `CityImpl` or `CapitalCityImpl` in the example). This class is decorated with
-`dataclass_abc` and `resolve_abc_prop` and should always be called through an 
+`dataclassabc` and `resolve_abc_prop` and should always be called through an 
 *initialize function*.
 - **init** - an *initialize function* (or *constructor function*) initializes an 
 *implementation class*.
```

### Comparing `dataclass_abc-0.0.7/setup.py` & `dataclass-abc-0.0.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    name='dataclass_abc',
-    version='0.0.7',
+    name='dataclass-abc',
+    version='0.0.8',
     description='Library that lets you define abstract properties for dataclasses.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MichaelSchneeberger/dataclass-abc',
     author='Michael Schneeberger',
     author_email='michael.schneeb@outlook.com',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.11',
     ],
-    keywords='dataclass_abc abstract abc property',
-    packages=['dataclass_abc'],
+    keywords='dataclass-abc abstract abc property',
+    packages=['dataclassabc'],
     python_requires='>=3.10',
 )
```

