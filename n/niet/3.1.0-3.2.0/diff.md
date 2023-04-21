# Comparing `tmp/niet-3.1.0.tar.gz` & `tmp/niet-3.2.0.tar.gz`

## Comparing `niet-3.1.0.tar` & `niet-3.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 niet-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 niet-3.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 niet-3.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 niet-3.1.0/ChangeLog.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 niet-3.1.0/Pipfile
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 niet-3.1.0/setup.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 niet-3.1.0/test-requirements.txt
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 niet-3.1.0/tox.ini
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 niet-3.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 niet-3.1.0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 niet-3.1.0/niet/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 niet-3.1.0/niet/__main__.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 niet-3.1.0/niet/output.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 niet-3.1.0/niet/url.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 niet-3.1.0/tests/test_output.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 niet-3.1.0/tests/test_url.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample.toml
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 niet-3.1.0/tests/samples/sample_not_indented.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 niet-3.1.0/.gitignore
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 niet-3.1.0/AUTHORS
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 niet-3.1.0/LICENSE
--rw-r--r--   0        0        0    24358 2020-02-02 00:00:00.000000 niet-3.1.0/README.md
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 niet-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    25519 2020-02-02 00:00:00.000000 niet-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 niet-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 niet-3.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 niet-3.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 niet-3.2.0/ChangeLog.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 niet-3.2.0/Pipfile
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 niet-3.2.0/setup.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 niet-3.2.0/test-requirements.txt
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 niet-3.2.0/tox.ini
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 niet-3.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 niet-3.2.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 niet-3.2.0/niet/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 niet-3.2.0/niet/__main__.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 niet-3.2.0/niet/output.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 niet-3.2.0/niet/url.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 niet-3.2.0/tests/test_output.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 niet-3.2.0/tests/test_url.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 niet-3.2.0/tests/samples/sample.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 niet-3.2.0/tests/samples/sample.toml
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 niet-3.2.0/tests/samples/sample.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 niet-3.2.0/tests/samples/sample_not_indented.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 niet-3.2.0/.gitignore
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 niet-3.2.0/AUTHORS
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 niet-3.2.0/LICENSE
+-rw-r--r--   0        0        0    26152 2020-02-02 00:00:00.000000 niet-3.2.0/README.md
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 niet-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    27313 2020-02-02 00:00:00.000000 niet-3.2.0/PKG-INFO
```

### Comparing `niet-3.1.0/.pre-commit-config.yaml` & `niet-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/CODE_OF_CONDUCT.md` & `niet-3.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/CONTRIBUTING.md` & `niet-3.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/ChangeLog.md` & `niet-3.2.0/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 CHANGES
 =======
 
+3.2.0
+-----
+
+* [feature] Introduce the `additional-objects` parameter to allow multi researches
+
 3.1.0
 -----
 
 * [feature] the toml format is now supported by niet (https://github.com/openuado/niet/pull/77)
-* [fix] replace deprecated pkg_resources by importlib.metadata
+* [fix] replace deprecated `pkg_resources` by `importlib.metadata`
 * [CI/CD] move away from travis CI and fix existing github actions
 * [CI/CD] publish to pypi with github actions
 * [CI/CD] introduce black and isort and a couple of new dev tools
 
 3.0.0
 -----
```

### Comparing `niet-3.1.0/.github/workflows/main.yml` & `niet-3.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/.github/workflows/python-app.yml` & `niet-3.2.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/niet/output.py` & `niet-3.2.0/niet/output.py`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/tests/test_output.py` & `niet-3.2.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/tests/test_url.py` & `niet-3.2.0/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/LICENSE` & `niet-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/README.md` & `niet-3.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,21 @@
 
 Niet is writen in Python so you can install it from a package manager (from
 PyPi) or directly by cloning this repository - no specific system rights are
 needed to install it.
 
 ## Main Features
 - Extract elements by using xpath syntax
-- Extract values from JSON format
-- Extract values from YAML format
-- Extract values from TOML format
+- Extract values from JSON, YAML, and TOML format
 - Automaticaly detect format (json/yaml)
 - Read data from a web resource
 - Read data from file or pass data from stdin
 - Format output values
 - Format output to be reused by shell `eval`
-- Convert YAML to JSON, or TOML
-- Convert JSON to YAML, or TOML
-- Convert TOML to YAML, or JSON
+- Convert YAML to JSON, or TOML and vice versa
 
 ## Install or Update niet
 
 ```sh
 $ pip install -U niet
 ```
 
@@ -71,37 +67,35 @@
 
 ## Usage
 
 ### Help and options
 
 ```shell
 $ niet --help
-usage: niet [-h] [-f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}] [-s] [-v]
-            object [file]
+usage: niet [-h] [-a ADDITIONAL_OBJECTS [ADDITIONAL_OBJECTS ...]] [-f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}] [-i] [-o OUTPUT_FILE] [-s] [-v] [--debug] object [file]
 
 Read data from YAML or JSON file
 
 positional arguments:
-  object                Path to object separated by dot (.). Use '.' to get
-                        whole file. eg: a.b.c
-  file                  Optional JSON or YAML filename. If not provided niet
-                        read from stdin
+  object                Path to object. Based on jsmespath identifiers (https://jmespath.org/specification.html#identifiers) Use '.' to get whole file. (eg: a.b.c)
+  file                  Optional JSON or YAML local filename or distant web resource at raw format. If not provided niet read from stdin
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -a ADDITIONAL_OBJECTS [ADDITIONAL_OBJECTS ...], --additional-objects ADDITIONAL_OBJECTS [ADDITIONAL_OBJECTS ...]
+                        Path to additional objects to search. Here you can pass a list of additional researchs. Allow you to combine researchs into the same command call. The researchs will be made on the original file as with the
+                        `object` parameter. Niet will output the results sequentially without delimiter between the results. If the `--output` argument is given by user, the results are appended at the end of the file sequentially. Based
+                        on jsmespath identifiers (https://jmespath.org/specification.html#identifiers) Use '.' to get whole file. (eg: a.b.c)
   -f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}, --format {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}
                         output format
   -i, --in-place        Perform modification in place. Will so alter read file
   -o OUTPUT_FILE, --output OUTPUT_FILE
-                        Print output in a file instead of stdout (surcharged
-                        by infile parameter if set)
-  -s, --silent          silent mode, doesn't display message when element was
-                        not found
-  -v, --version         print the Niet version number and exit (also
-                        --version)
+                        Print output in a file instead of stdout (surcharged by in-place parameter if set)
+  -s, --silent          silent mode, doesn't display message when element was not found
+  -v, --version         print the Niet version number and exit (also --version)
   --debug               Activate the debug mode (based on pdb)
 
 output formats:
   json          Return object in JSON
   yaml          Return object in YAML
   toml          Return object in TOML
   eval          Return result in a string evaluable by a shell eval command as an input
@@ -233,15 +227,15 @@
 $ echo $?
 1
 ```
 
 See the [related section](#deal-with-errors) for more info on how to manage
 errors with `niet`.
 
-Niet is based on `jmespath` to find results so for complex research you can
+Niet is based on `jmespath` to find results so for complexe research you can
 refer to the [jmespath specifications](http://jmespath.org/specification.html#identifiers)
 to use identifiers properly.
 
 If you try to search for an identifier who use some dash you need to surround
 your research expression with simple and double quotes, examples:
 
 ```sh
@@ -289,14 +283,57 @@
 Example:
 ```sh
 niet project.'"test-dash"' tests/sample/sample.json
 ```
 
 Further examples with [`jmespath` identifiers](http://jmespath.org/specification.html#examples).
 
+### Additional objects
+
+Additional objects allow you to combine more than one query.
+The `--additional-objects` parameter accept a list of objects strings.
+These objects are the same thing that the base object used to query
+your inputs.
+
+This parameter allow to generate advanced output from your input, let see an
+example:
+
+Consider the following yaml example:
+```
+configuration:
+  warehouse: warehouse-name
+  database: database-name
+  object_type:
+      schema:
+        schema1: "/path/to/schema1.sql"
+        schema2: "/path/to/schema2.sql"
+```
+
+The following command will allow us to generate an output constitued from the
+results of the two objects used as query:
+
+```
+$ niet ".configuration.object_type | keys(@)[0]" config.yaml
+-a ".configuration.object_type.schema.[keys(@)[0], values(@)[0]]"
+```
+
+The previous command will output:
+
+```
+schema
+schema1
+/path/to/schema1.sql
+```
+
+This output wouldn't be possible without combining the result of two queries,
+the additional objects are made for that.
+
+Outputs of these additional objects are printed sequentially in the order they
+are given in the command line.
+
 ### Output
 
 #### Stdout
 By default, niet print the output on stdout.
 
 #### Save output to a file
 It if possible to pass a filename using -o or --output argument to writes
```

### Comparing `niet-3.1.0/pyproject.toml` & `niet-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `niet-3.1.0/PKG-INFO` & `niet-3.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niet
-Version: 3.1.0
+Version: 3.2.0
 Summary: A command-line tool to work with YAML, JSON, and TOML files.
 Author-email: Hervé Beraud <herveberaud.pro@gmail.com>
 License: MIT
 License-File: AUTHORS
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -67,25 +67,21 @@
 
 Niet is writen in Python so you can install it from a package manager (from
 PyPi) or directly by cloning this repository - no specific system rights are
 needed to install it.
 
 ## Main Features
 - Extract elements by using xpath syntax
-- Extract values from JSON format
-- Extract values from YAML format
-- Extract values from TOML format
+- Extract values from JSON, YAML, and TOML format
 - Automaticaly detect format (json/yaml)
 - Read data from a web resource
 - Read data from file or pass data from stdin
 - Format output values
 - Format output to be reused by shell `eval`
-- Convert YAML to JSON, or TOML
-- Convert JSON to YAML, or TOML
-- Convert TOML to YAML, or JSON
+- Convert YAML to JSON, or TOML and vice versa
 
 ## Install or Update niet
 
 ```sh
 $ pip install -U niet
 ```
 
@@ -104,37 +100,35 @@
 
 ## Usage
 
 ### Help and options
 
 ```shell
 $ niet --help
-usage: niet [-h] [-f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}] [-s] [-v]
-            object [file]
+usage: niet [-h] [-a ADDITIONAL_OBJECTS [ADDITIONAL_OBJECTS ...]] [-f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}] [-i] [-o OUTPUT_FILE] [-s] [-v] [--debug] object [file]
 
 Read data from YAML or JSON file
 
 positional arguments:
-  object                Path to object separated by dot (.). Use '.' to get
-                        whole file. eg: a.b.c
-  file                  Optional JSON or YAML filename. If not provided niet
-                        read from stdin
+  object                Path to object. Based on jsmespath identifiers (https://jmespath.org/specification.html#identifiers) Use '.' to get whole file. (eg: a.b.c)
+  file                  Optional JSON or YAML local filename or distant web resource at raw format. If not provided niet read from stdin
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  -a ADDITIONAL_OBJECTS [ADDITIONAL_OBJECTS ...], --additional-objects ADDITIONAL_OBJECTS [ADDITIONAL_OBJECTS ...]
+                        Path to additional objects to search. Here you can pass a list of additional researchs. Allow you to combine researchs into the same command call. The researchs will be made on the original file as with the
+                        `object` parameter. Niet will output the results sequentially without delimiter between the results. If the `--output` argument is given by user, the results are appended at the end of the file sequentially. Based
+                        on jsmespath identifiers (https://jmespath.org/specification.html#identifiers) Use '.' to get whole file. (eg: a.b.c)
   -f {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}, --format {json,yaml,toml,eval,newline,ifs,squote,dquote,comma}
                         output format
   -i, --in-place        Perform modification in place. Will so alter read file
   -o OUTPUT_FILE, --output OUTPUT_FILE
-                        Print output in a file instead of stdout (surcharged
-                        by infile parameter if set)
-  -s, --silent          silent mode, doesn't display message when element was
-                        not found
-  -v, --version         print the Niet version number and exit (also
-                        --version)
+                        Print output in a file instead of stdout (surcharged by in-place parameter if set)
+  -s, --silent          silent mode, doesn't display message when element was not found
+  -v, --version         print the Niet version number and exit (also --version)
   --debug               Activate the debug mode (based on pdb)
 
 output formats:
   json          Return object in JSON
   yaml          Return object in YAML
   toml          Return object in TOML
   eval          Return result in a string evaluable by a shell eval command as an input
@@ -266,15 +260,15 @@
 $ echo $?
 1
 ```
 
 See the [related section](#deal-with-errors) for more info on how to manage
 errors with `niet`.
 
-Niet is based on `jmespath` to find results so for complex research you can
+Niet is based on `jmespath` to find results so for complexe research you can
 refer to the [jmespath specifications](http://jmespath.org/specification.html#identifiers)
 to use identifiers properly.
 
 If you try to search for an identifier who use some dash you need to surround
 your research expression with simple and double quotes, examples:
 
 ```sh
@@ -322,14 +316,57 @@
 Example:
 ```sh
 niet project.'"test-dash"' tests/sample/sample.json
 ```
 
 Further examples with [`jmespath` identifiers](http://jmespath.org/specification.html#examples).
 
+### Additional objects
+
+Additional objects allow you to combine more than one query.
+The `--additional-objects` parameter accept a list of objects strings.
+These objects are the same thing that the base object used to query
+your inputs.
+
+This parameter allow to generate advanced output from your input, let see an
+example:
+
+Consider the following yaml example:
+```
+configuration:
+  warehouse: warehouse-name
+  database: database-name
+  object_type:
+      schema:
+        schema1: "/path/to/schema1.sql"
+        schema2: "/path/to/schema2.sql"
+```
+
+The following command will allow us to generate an output constitued from the
+results of the two objects used as query:
+
+```
+$ niet ".configuration.object_type | keys(@)[0]" config.yaml
+-a ".configuration.object_type.schema.[keys(@)[0], values(@)[0]]"
+```
+
+The previous command will output:
+
+```
+schema
+schema1
+/path/to/schema1.sql
+```
+
+This output wouldn't be possible without combining the result of two queries,
+the additional objects are made for that.
+
+Outputs of these additional objects are printed sequentially in the order they
+are given in the command line.
+
 ### Output
 
 #### Stdout
 By default, niet print the output on stdout.
 
 #### Save output to a file
 It if possible to pass a filename using -o or --output argument to writes
```

