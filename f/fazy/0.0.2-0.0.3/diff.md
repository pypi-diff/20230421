# Comparing `tmp/fazy-0.0.2.tar.gz` & `tmp/fazy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fazy-0.0.2.tar", last modified: Thu Apr 20 13:54:26 2023, max compression
+gzip compressed data, was "fazy-0.0.3.tar", last modified: Fri Apr 21 05:31:30 2023, max compression
```

## Comparing `fazy-0.0.2.tar` & `fazy-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-20 13:54:26.777886 fazy-0.0.2/
--rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-12 12:31:37.000000 fazy-0.0.2/LICENSE
--rw-r--r--   0 pomponchik   (501) staff       (20)    12305 2023-04-20 13:54:26.777646 fazy-0.0.2/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)    11753 2023-04-20 12:01:02.000000 fazy-0.0.2/README.md
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-20 13:54:26.776253 fazy-0.0.2/f/
--rw-r--r--   0 pomponchik   (501) staff       (20)       98 2023-04-20 12:08:45.000000 fazy-0.0.2/f/__init__.py
--rw-r--r--   0 pomponchik   (501) staff       (20)      286 2023-04-20 12:02:43.000000 fazy-0.0.2/f/chain_unit.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     6839 2023-04-20 12:04:13.000000 fazy-0.0.2/f/lazy_string.py
--rw-r--r--   0 pomponchik   (501) staff       (20)     2380 2023-04-20 12:36:07.000000 fazy-0.0.2/f/proxy_module.py
-drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-20 13:54:26.777283 fazy-0.0.2/fazy.egg-info/
--rw-r--r--   0 pomponchik   (501) staff       (20)    12305 2023-04-20 13:54:26.000000 fazy-0.0.2/fazy.egg-info/PKG-INFO
--rw-r--r--   0 pomponchik   (501) staff       (20)      203 2023-04-20 13:54:26.000000 fazy-0.0.2/fazy.egg-info/SOURCES.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-20 13:54:26.000000 fazy-0.0.2/fazy.egg-info/dependency_links.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)        2 2023-04-20 13:54:26.000000 fazy-0.0.2/fazy.egg-info/top_level.txt
--rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-20 13:54:26.777943 fazy-0.0.2/setup.cfg
--rw-r--r--   0 pomponchik   (501) staff       (20)      833 2023-04-20 12:02:56.000000 fazy-0.0.2/setup.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-21 05:31:30.929652 fazy-0.0.3/
+-rw-r--r--   0 pomponchik   (501) staff       (20)     1067 2023-04-12 12:31:37.000000 fazy-0.0.3/LICENSE
+-rw-r--r--   0 pomponchik   (501) staff       (20)    12315 2023-04-21 05:31:30.929413 fazy-0.0.3/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)    11763 2023-04-21 04:18:58.000000 fazy-0.0.3/README.md
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-21 05:31:30.928039 fazy-0.0.3/f/
+-rw-r--r--   0 pomponchik   (501) staff       (20)       98 2023-04-20 12:08:45.000000 fazy-0.0.3/f/__init__.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)      286 2023-04-20 12:02:43.000000 fazy-0.0.3/f/chain_unit.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     6839 2023-04-20 12:04:13.000000 fazy-0.0.3/f/lazy_string.py
+-rw-r--r--   0 pomponchik   (501) staff       (20)     2405 2023-04-21 05:21:58.000000 fazy-0.0.3/f/proxy_module.py
+drwxr-xr-x   0 pomponchik   (501) staff       (20)        0 2023-04-21 05:31:30.929109 fazy-0.0.3/fazy.egg-info/
+-rw-r--r--   0 pomponchik   (501) staff       (20)    12315 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/PKG-INFO
+-rw-r--r--   0 pomponchik   (501) staff       (20)      203 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/SOURCES.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        1 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/dependency_links.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)        2 2023-04-21 05:31:30.000000 fazy-0.0.3/fazy.egg-info/top_level.txt
+-rw-r--r--   0 pomponchik   (501) staff       (20)       38 2023-04-21 05:31:30.929713 fazy-0.0.3/setup.cfg
+-rw-r--r--   0 pomponchik   (501) staff       (20)      833 2023-04-21 05:31:02.000000 fazy-0.0.3/setup.py
```

### Comparing `fazy-0.0.2/LICENSE` & `fazy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fazy-0.0.2/PKG-INFO` & `fazy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fazy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lazy f-strings for everyone
 Home-page: https://github.com/pomponchik/fazy
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,15 +20,15 @@
 [![Downloads](https://pepy.tech/badge/fazy)](https://pepy.tech/project/fazy)
 [![codecov](https://codecov.io/gh/pomponchik/fazy/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/fazy)
 [![Test-Package](https://github.com/pomponchik/fazy/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/fazy/actions/workflows/coverage.yml)
 [![PyPI version](https://badge.fury.io/py/fazy.svg)](https://badge.fury.io/py/fazy)
 [![Python versions](https://img.shields.io/pypi/pyversions/fazy.svg)](https://pypi.python.org/pypi/fazy)
 
 
-Lazy f-strings are the holy grail of Python development. Now they are found.
+Lazy f-strings are the holy grail of Python development. Now it is found.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**The problem**](#the-problem)
 - [**How does it work?**](#how-does-it-work)
@@ -43,19 +43,19 @@
 ```bash
 pip install fazy
 ```
 
 And use:
 
 ```python
-import f
-
-number = 33
-print(f('{number} kittens drink milk'))
-# 33 kittens drink milk
+>>> import f
+>>>
+>>> number = 33
+>>> print(f('{number} kittens drink milk'))
+33 kittens drink milk
 ```
 
 ## The problem
 
 The main problem that this library solves is the transfer of the cost of calculating the extrapolation of a string from the moment when it is determined to the moment when it is used. And all this while preserving the classic look of the f-string, which we are so used to on modern versions of Python.
 
 The main use case that the author had in mind is related to logging. The fact is that many messages that are created for logging may eventually not be printed, because the logging level is too low for them. The classic solution to the problem is to calculate the string in a [lazy](https://en.wikipedia.org/wiki/Lazy_evaluation) way. However, until now, this solution has been incompatible with the convenient syntax of f-strings. You needed to use % expressions for this, it looks much worse.
```

### Comparing `fazy-0.0.2/README.md` & `fazy-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Downloads](https://pepy.tech/badge/fazy)](https://pepy.tech/project/fazy)
 [![codecov](https://codecov.io/gh/pomponchik/fazy/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/fazy)
 [![Test-Package](https://github.com/pomponchik/fazy/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/fazy/actions/workflows/coverage.yml)
 [![PyPI version](https://badge.fury.io/py/fazy.svg)](https://badge.fury.io/py/fazy)
 [![Python versions](https://img.shields.io/pypi/pyversions/fazy.svg)](https://pypi.python.org/pypi/fazy)
 
 
-Lazy f-strings are the holy grail of Python development. Now they are found.
+Lazy f-strings are the holy grail of Python development. Now it is found.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**The problem**](#the-problem)
 - [**How does it work?**](#how-does-it-work)
@@ -27,19 +27,19 @@
 ```bash
 pip install fazy
 ```
 
 And use:
 
 ```python
-import f
-
-number = 33
-print(f('{number} kittens drink milk'))
-# 33 kittens drink milk
+>>> import f
+>>>
+>>> number = 33
+>>> print(f('{number} kittens drink milk'))
+33 kittens drink milk
 ```
 
 ## The problem
 
 The main problem that this library solves is the transfer of the cost of calculating the extrapolation of a string from the moment when it is determined to the moment when it is used. And all this while preserving the classic look of the f-string, which we are so used to on modern versions of Python.
 
 The main use case that the author had in mind is related to logging. The fact is that many messages that are created for logging may eventually not be printed, because the logging level is too low for them. The classic solution to the problem is to calculate the string in a [lazy](https://en.wikipedia.org/wiki/Lazy_evaluation) way. However, until now, this solution has been incompatible with the convenient syntax of f-strings. You needed to use % expressions for this, it looks much worse.
```

### Comparing `fazy-0.0.2/f/lazy_string.py` & `fazy-0.0.3/f/lazy_string.py`

 * *Files identical despite different names*

### Comparing `fazy-0.0.2/f/proxy_module.py` & `fazy-0.0.3/f/proxy_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             {**inspect.stack(0)[1].frame.f_locals},
             {**inspect.stack(0)[1].frame.f_globals},
             self.sum_of_nonlocals(inspect.stack(0)[1].frame.f_back, self.get_qualname(inspect.stack(0)[1].frame.f_code)),
             lazy,
         )
 
     def sum_of_nonlocals(self, first_frame, base_qualname):
-        if first_frame is None:
+        if first_frame is None or base_qualname is None:
             return {}
 
         all_locals = []
         while first_frame is not None:
             code = first_frame.f_code
 
             qualname = self.get_qualname(code)
```

### Comparing `fazy-0.0.2/fazy.egg-info/PKG-INFO` & `fazy-0.0.3/fazy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fazy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lazy f-strings for everyone
 Home-page: https://github.com/pomponchik/fazy
 Author: Evgeniy Blinov
 Author-email: zheni-b@yandex.ru
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,15 +20,15 @@
 [![Downloads](https://pepy.tech/badge/fazy)](https://pepy.tech/project/fazy)
 [![codecov](https://codecov.io/gh/pomponchik/fazy/branch/main/graph/badge.svg)](https://codecov.io/gh/pomponchik/fazy)
 [![Test-Package](https://github.com/pomponchik/fazy/actions/workflows/coverage.yml/badge.svg)](https://github.com/pomponchik/fazy/actions/workflows/coverage.yml)
 [![PyPI version](https://badge.fury.io/py/fazy.svg)](https://badge.fury.io/py/fazy)
 [![Python versions](https://img.shields.io/pypi/pyversions/fazy.svg)](https://pypi.python.org/pypi/fazy)
 
 
-Lazy f-strings are the holy grail of Python development. Now they are found.
+Lazy f-strings are the holy grail of Python development. Now it is found.
 
 
 ## Table of contents
 
 - [**Quick start**](#quick-start)
 - [**The problem**](#the-problem)
 - [**How does it work?**](#how-does-it-work)
@@ -43,19 +43,19 @@
 ```bash
 pip install fazy
 ```
 
 And use:
 
 ```python
-import f
-
-number = 33
-print(f('{number} kittens drink milk'))
-# 33 kittens drink milk
+>>> import f
+>>>
+>>> number = 33
+>>> print(f('{number} kittens drink milk'))
+33 kittens drink milk
 ```
 
 ## The problem
 
 The main problem that this library solves is the transfer of the cost of calculating the extrapolation of a string from the moment when it is determined to the moment when it is used. And all this while preserving the classic look of the f-string, which we are so used to on modern versions of Python.
 
 The main use case that the author had in mind is related to logging. The fact is that many messages that are created for logging may eventually not be printed, because the logging level is too low for them. The classic solution to the problem is to calculate the string in a [lazy](https://en.wikipedia.org/wiki/Lazy_evaluation) way. However, until now, this solution has been incompatible with the convenient syntax of f-strings. You needed to use % expressions for this, it looks much worse.
```

