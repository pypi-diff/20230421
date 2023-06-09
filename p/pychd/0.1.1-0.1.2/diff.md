# Comparing `tmp/pychd-0.1.1.tar.gz` & `tmp/pychd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychd-0.1.1.tar", max compression
+gzip compressed data, was "pychd-0.1.2.tar", max compression
```

## Comparing `pychd-0.1.1.tar` & `pychd-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.1/LICENSE
--rw-r--r--   0        0        0    19111 2023-04-21 03:33:26.493614 pychd-0.1.1/README.md
--rw-r--r--   0        0        0      785 2023-04-21 03:40:04.606726 pychd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.1/src/pychd/__init__.py
--rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.1/src/pychd/compile.py
--rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.1/src/pychd/decompile.py
--rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.1/src/pychd/logging.conf.template
--rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.1/src/pychd/main.py
--rw-r--r--   0        0        0    19920 1970-01-01 00:00:00.000000 pychd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-19 22:05:09.083953 pychd-0.1.2/LICENSE
+-rw-r--r--   0        0        0    19431 2023-04-21 03:53:19.623020 pychd-0.1.2/README.md
+-rw-r--r--   0        0        0      791 2023-04-21 03:54:41.397613 pychd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 21:37:37.817710 pychd-0.1.2/src/pychd/__init__.py
+-rw-r--r--   0        0        0      685 2023-04-21 02:25:57.414400 pychd-0.1.2/src/pychd/compile.py
+-rw-r--r--   0        0        0     3091 2023-04-21 03:12:30.874370 pychd-0.1.2/src/pychd/decompile.py
+-rw-r--r--   0        0        0      439 2023-04-21 02:25:57.435574 pychd-0.1.2/src/pychd/logging.conf.template
+-rw-r--r--   0        0        0     1709 2023-04-21 03:39:52.243145 pychd-0.1.2/src/pychd/main.py
+-rw-r--r--   0        0        0    20246 1970-01-01 00:00:00.000000 pychd-0.1.2/PKG-INFO
```

### Comparing `pychd-0.1.1/LICENSE` & `pychd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pychd-0.1.1/README.md` & `pychd-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # pychd
 
-Python decompiler using ChatGPT
+[![CI](https://github.com/diohabara/pychd/actions/workflows/ci.yml/badge.svg)](https://github.com/diohabara/pychd/actions/workflows/ci.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/pychd.svg)](https://pypi.python.org/pypi/pychd)
 
-## Setup
+The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 
-```bash
-poetry install
-poetry run pre-commit install
-```
+## Usage
 
-Set `OPENAI_API_KEY` environment variable. If you're using `direnv`, you can use `.envrc.template` as a template.
-Put `src/pychd/logging.conf`. You can copy `src/pychd/logging.conf.template` like this:
+### Install
+
+From pip
 
 ```bash
-cp src/pychd/logging.conf.template src/pychd/logging.conf
+pip install pychd
 ```
 
-## Compile
+### Compile
 
 ```bash
-poetry run pychd compile <directory | file> # you need to specify a directory or a .py file
+pychd compile <directory | file> # you need to specify a directory or a .py file
 ```
 
 E.g.,
 
 ```bash
-poetry run pychd compile examples/01_example_variables.py # `example/__pycache__/01_example_variables.cpython-310.pyc` will be created
+pychd compile examples/01_example_variables.py # `example/__pycache__/01_example_variables.cpython-310.pyc` will be created
 ```
 
-## Decompile
+### Decompile
 
 ```bash
-poetry run pychd decompile <pyc-file> # you need to specify a .pyc file
+pychd decompile <pyc-file> # you need to specify a .pyc file
 ```
 
 E.g.,
 
 ```bash
-poetry run pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc # decompiled code will be printed
+pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc # decompiled code will be printed
 ```
 
 ```bash
-poetry run pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc -o example/__pycache__/01_example_variables.cpython-310.py # decompiled code will be written to `example/__pycache__/01_example_variables.cpython-310.py`
+pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc -o example/__pycache__/01_example_variables.cpython-310.py # decompiled code will be written to `example/__pycache__/01_example_variables.cpython-310.py`
 ```
 
 ## Examples
 
 You can find examples in `example` directory or below (decompiled code is generated by `pychd`).
 
 ### Variables
@@ -878,7 +877,23 @@
 with open(temp_path, 'r') as temp_file:
     content = temp_file.read()
     print('Content of the temporary file: {0}'.format(content))
 
 os.remove(temp_path)
 print('Removed temporary file: {0}'.format(temp_path))
 ```
+
+## Development
+
+## Setup
+
+```bash
+poetry install
+poetry run pre-commit install
+```
+
+Set `OPENAI_API_KEY` environment variable. If you're using `direnv`, you can use `.envrc.template` as a template.
+Put `src/pychd/logging.conf`. You can copy `src/pychd/logging.conf.template` like this:
+
+```bash
+cp src/pychd/logging.conf.template src/pychd/logging.conf
+```
```

### Comparing `pychd-0.1.1/pyproject.toml` & `pychd-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 authors = ["卍diohabara卍 <diohabara@gmail.com>"]
-description = "The ChatGPT-powered Python decompiler provided superior code analysis capabilities"
+description = "The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities"
 keywords = ["decompiler", "python", "poetry", "bytecode"]
 license = "MIT"
 name = "pychd"
 packages = [{include = "src/pychd"}]
 readme = "README.md"
 repository = "https://github.com/diohabara/pychd"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 openai = "^0.27.4"
 pytest = "^7.3.1"
 python = ">=3.8, <3.11"
 pytype = "^2023.4.18"
```

### Comparing `pychd-0.1.1/src/pychd/compile.py` & `pychd-0.1.2/src/pychd/compile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.1/src/pychd/decompile.py` & `pychd-0.1.2/src/pychd/decompile.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.1/src/pychd/main.py` & `pychd-0.1.2/src/pychd/main.py`

 * *Files identical despite different names*

### Comparing `pychd-0.1.1/PKG-INFO` & `pychd-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pychd
-Version: 0.1.1
-Summary: The ChatGPT-powered Python decompiler provided superior code analysis capabilities
+Version: 0.1.2
+Summary: The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 Home-page: https://github.com/diohabara/pychd
 License: MIT
 Keywords: decompiler,python,poetry,bytecode
 Author: 卍diohabara卍
 Author-email: diohabara@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -17,56 +17,55 @@
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: pytype (>=2023.4.18,<2024.0.0)
 Project-URL: Repository, https://github.com/diohabara/pychd
 Description-Content-Type: text/markdown
 
 # pychd
 
-Python decompiler using ChatGPT
+[![CI](https://github.com/diohabara/pychd/actions/workflows/ci.yml/badge.svg)](https://github.com/diohabara/pychd/actions/workflows/ci.yml)
+[![PyPI Version](https://img.shields.io/pypi/v/pychd.svg)](https://pypi.python.org/pypi/pychd)
 
-## Setup
+The ChatGPT-powered decompiler for Python, providing superior code analysis capabilities
 
-```bash
-poetry install
-poetry run pre-commit install
-```
+## Usage
 
-Set `OPENAI_API_KEY` environment variable. If you're using `direnv`, you can use `.envrc.template` as a template.
-Put `src/pychd/logging.conf`. You can copy `src/pychd/logging.conf.template` like this:
+### Install
+
+From pip
 
 ```bash
-cp src/pychd/logging.conf.template src/pychd/logging.conf
+pip install pychd
 ```
 
-## Compile
+### Compile
 
 ```bash
-poetry run pychd compile <directory | file> # you need to specify a directory or a .py file
+pychd compile <directory | file> # you need to specify a directory or a .py file
 ```
 
 E.g.,
 
 ```bash
-poetry run pychd compile examples/01_example_variables.py # `example/__pycache__/01_example_variables.cpython-310.pyc` will be created
+pychd compile examples/01_example_variables.py # `example/__pycache__/01_example_variables.cpython-310.pyc` will be created
 ```
 
-## Decompile
+### Decompile
 
 ```bash
-poetry run pychd decompile <pyc-file> # you need to specify a .pyc file
+pychd decompile <pyc-file> # you need to specify a .pyc file
 ```
 
 E.g.,
 
 ```bash
-poetry run pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc # decompiled code will be printed
+pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc # decompiled code will be printed
 ```
 
 ```bash
-poetry run pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc -o example/__pycache__/01_example_variables.cpython-310.py # decompiled code will be written to `example/__pycache__/01_example_variables.cpython-310.py`
+pychd decompile example/__pycache__/01_example_variables.cpython-310.pyc -o example/__pycache__/01_example_variables.cpython-310.py # decompiled code will be written to `example/__pycache__/01_example_variables.cpython-310.py`
 ```
 
 ## Examples
 
 You can find examples in `example` directory or below (decompiled code is generated by `pychd`).
 
 ### Variables
@@ -900,7 +899,23 @@
     content = temp_file.read()
     print('Content of the temporary file: {0}'.format(content))
 
 os.remove(temp_path)
 print('Removed temporary file: {0}'.format(temp_path))
 ```
 
+## Development
+
+## Setup
+
+```bash
+poetry install
+poetry run pre-commit install
+```
+
+Set `OPENAI_API_KEY` environment variable. If you're using `direnv`, you can use `.envrc.template` as a template.
+Put `src/pychd/logging.conf`. You can copy `src/pychd/logging.conf.template` like this:
+
+```bash
+cp src/pychd/logging.conf.template src/pychd/logging.conf
+```
+
```

