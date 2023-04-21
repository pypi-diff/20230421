# Comparing `tmp/py_experimenter-1.2.0.tar.gz` & `tmp/py_experimenter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_experimenter-1.2.0.tar", max compression
+gzip compressed data, was "py_experimenter-1.2.1.tar", max compression
```

## Comparing `py_experimenter-1.2.0.tar` & `py_experimenter-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1183 2023-02-16 12:30:15.046670 py_experimenter-1.2.0/LICENSE
--rw-r--r--   0        0        0     2234 2023-02-16 12:30:15.046824 py_experimenter-1.2.0/README.md
--rw-r--r--   0        0        0        1 2023-02-16 12:30:15.050204 py_experimenter-1.2.0/py_experimenter/__init__.py
--rw-r--r--   0        0        0    13837 2023-04-04 09:33:58.356828 py_experimenter-1.2.0/py_experimenter/database_connector.py
--rw-r--r--   0        0        0     3205 2023-04-04 09:33:58.357136 py_experimenter-1.2.0/py_experimenter/database_connector_lite.py
--rw-r--r--   0        0        0     5211 2023-04-04 09:33:58.357465 py_experimenter-1.2.0/py_experimenter/database_connector_mysql.py
--rw-r--r--   0        0        0      907 2023-04-04 09:33:58.357634 py_experimenter-1.2.0/py_experimenter/exceptions.py
--rw-r--r--   0        0        0      156 2023-02-16 12:30:15.050509 py_experimenter-1.2.0/py_experimenter/experiment_status.py
--rw-r--r--   0        0        0    22555 2023-04-04 09:33:58.358029 py_experimenter-1.2.0/py_experimenter/experimenter.py
--rw-r--r--   0        0        0     4476 2023-04-04 09:33:58.358327 py_experimenter-1.2.0/py_experimenter/result_processor.py
--rw-r--r--   0        0        0     8454 2023-04-04 09:33:58.358636 py_experimenter-1.2.0/py_experimenter/utils.py
--rw-r--r--   0        0        0     1671 2023-04-04 09:33:58.358911 py_experimenter-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3175 1970-01-01 00:00:00.000000 py_experimenter-1.2.0/setup.py
--rw-r--r--   0        0        0     3622 1970-01-01 00:00:00.000000 py_experimenter-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1183 2023-02-16 12:30:15.046670 py_experimenter-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3461 2023-04-21 15:31:15.552785 py_experimenter-1.2.1/README.md
+-rw-r--r--   0        0        0        1 2023-02-16 12:30:15.050204 py_experimenter-1.2.1/py_experimenter/__init__.py
+-rw-r--r--   0        0        0    14295 2023-04-21 15:54:05.717303 py_experimenter-1.2.1/py_experimenter/database_connector.py
+-rw-r--r--   0        0        0     3216 2023-04-21 15:54:05.717692 py_experimenter-1.2.1/py_experimenter/database_connector_lite.py
+-rw-r--r--   0        0        0     5222 2023-04-21 15:54:05.718090 py_experimenter-1.2.1/py_experimenter/database_connector_mysql.py
+-rw-r--r--   0        0        0      907 2023-04-04 09:33:58.357634 py_experimenter-1.2.1/py_experimenter/exceptions.py
+-rw-r--r--   0        0        0      156 2023-02-16 12:30:15.050509 py_experimenter-1.2.1/py_experimenter/experiment_status.py
+-rw-r--r--   0        0        0    22555 2023-04-04 09:33:58.358029 py_experimenter-1.2.1/py_experimenter/experimenter.py
+-rw-r--r--   0        0        0     4476 2023-04-04 09:33:58.358327 py_experimenter-1.2.1/py_experimenter/result_processor.py
+-rw-r--r--   0        0        0     8454 2023-04-04 09:33:58.358636 py_experimenter-1.2.1/py_experimenter/utils.py
+-rw-r--r--   0        0        0     1671 2023-04-21 15:54:05.718291 py_experimenter-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 py_experimenter-1.2.1/setup.py
+-rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 py_experimenter-1.2.1/PKG-INFO
```

### Comparing `py_experimenter-1.2.0/LICENSE` & `py_experimenter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.0/README.md` & `py_experimenter-1.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,14 @@
-[![doc](https://img.shields.io/badge/doc-success-success)](https://tornede.github.io/py_experimenter)
-[![pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)
-[![GitHub](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)
+[![Project Homepage](https://img.shields.io/badge/Project%20Homepage-tornede.github.io/py_experimenter-0092CD)](https://tornede.github.io/py_experimenter)
+[![Pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)
+[![License](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05149/status.svg)](https://doi.org/10.21105/joss.05149)
+
+![Tests](https://github.com/tornede/py_experimenter/actions/workflows/tests.yml/badge.svg)
+![GitHub Pages](https://github.com/tornede/py_experimenter/actions/workflows/github-pages.yml/badge.svg)
 
 <img src="docs/source/_static/py-experimenter-logo.png" alt="PyExperimenter Logo: Python biting a database" width="200px"/>
 
 # PyExperimenter
 
 `PyExperimenter` is a tool to facilitate the setup, documentation, execution, and subsequent evaluation of results from an empirical study of algorithms and in particular is designed to reduce the involved manual effort significantly.
 It is intended to be used by researchers in the field of artificial intelligence, but is not limited to those.
@@ -20,7 +24,31 @@
 
 ![General schema of `PyExperimenter`.](docs/source/_static/workflow.png)
 
 For more details check out the [`PyExperimenter` documentation](https://tornede.github.io/py_experimenter/):
 
 - [Installation](https://tornede.github.io/py_experimenter/installation.html)
 - [Examples](https://tornede.github.io/py_experimenter/examples/example_general_usage.html)
+
+## Cite PyExperimenter
+
+If you use `PyExperimenter` in a scientific publication, we would appreciate a citation in one of the following ways.
+
+### Citation String
+
+Tornede et al., (2023). PyExperimenter: Easily distribute experiments and track results. Journal of Open Source Software, 8(84), 5149, https://doi.org/10.21105/joss.05149
+
+### BibTex
+```
+@article{Tornede2023, 
+    title = {{PyExperimenter}: Easily distribute experiments and track results}, 
+    author = {Tanja Tornede and Alexander Tornede and Lukas Fehring and Lukas Gehring and Helena Graf and Jonas Hanselle and Felix Mohr and Marcel Wever}, 
+    journal = {Journal of Open Source Software},
+    publisher = {The Open Journal},  
+    year = {2023}, 
+    volume = {8}, 
+    number = {84}, 
+    pages = {5149}, 
+    doi = {10.21105/joss.05149}, 
+    url = {https://doi.org/10.21105/joss.05149}
+}
+```
```

### Comparing `py_experimenter-1.2.0/py_experimenter/database_connector.py` & `py_experimenter-1.2.1/py_experimenter/database_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,43 +136,47 @@
         pass
 
     @abc.abstractmethod
     def _table_has_correct_structure(self, cursor, typed_fields):
         pass
 
     def fill_table(self, parameters=None, fixed_parameter_combinations=None) -> None:
-        logging.debug("Fill table with parameters")
+        logging.debug("Fill table with parameters.")
         parameters = parameters if parameters is not None else {}
         fixed_parameter_combinations = fixed_parameter_combinations if fixed_parameter_combinations is not None else []
 
         keyfield_names = utils.get_keyfield_names(self.config)
         combinations = utils.combine_fill_table_parameters(keyfield_names, parameters, fixed_parameter_combinations)
 
         if len(combinations) == 0:
             raise EmptyFillDatabaseCallError("No combinations to execute found.")
 
-        column_names = ','.join(combinations[0].keys())
-
-        existing_rows = self._get_existing_rows(column_names)
-
-        column_names += ",status"
-        column_names += ",creation_date"
-
+        column_names = list(combinations[0].keys())
+        logging.debug("Getting existing rows.")
+        existing_rows = set(self._get_existing_rows(column_names))
         time = utils.get_timestamp_representation()
-        values_added = 0
+
+        rows_skipped = 0
+        rows = []
+        logging.debug("Checking which of the experiments to be inserted already exist.")
         for combination in combinations:
             if self._check_combination_in_existing_rows(combination, existing_rows, keyfield_names):
+                rows_skipped += 1
                 continue
             values = list(combination.values())
             values.append(ExperimentStatus.CREATED.value)
             values.append(time)
+            rows.append(values)
 
-            self._write_to_database(column_names.split(', '), values)
-            values_added += 1
-        logging.info(f"{values_added} values successfully added to database")
+        if rows:
+            logging.debug(f"Now adding {len(rows)} rows to database. {rows_skipped} rows were skipped.")
+            self._write_to_database(pd.DataFrame(rows, columns=column_names + ["status", "creation_date"]))
+            logging.info(f"{len(rows)} rows successfully added to database. {rows_skipped} rows were skipped.")
+        else:
+            logging.info(f"No rows to add. All the {len(combinations)} experiments already exist.")
 
     def _check_combination_in_existing_rows(self, combination, existing_rows, keyfield_names) -> bool:
         def _get_column_values():
             return [combination[keyfield_name] for keyfield_name in keyfield_names]
         return ("[" + " ".join([str(value) for value in _get_column_values()]) + "]") in existing_rows
 
     @abc.abstractmethod
@@ -204,19 +208,19 @@
         description = cursor.description
         return experiment_id, description, values
 
     @abc.abstractmethod
     def _pull_open_experiment(self) -> Tuple[int, List, List]:
         pass
 
-    def _write_to_database(self, keys, values) -> None:
-        keys = ", ".join(keys)
-        values = "'" + self.__class__._write_to_database_separator.join([str(value) for value in values]) + "'"
+    def _write_to_database(self, df) -> None:
+        keys = ", ".join(df.columns)
+        values = df.apply(lambda row: "('" + self.__class__._write_to_database_separator.join([str(value) for value in row]) + "')", axis=1)
 
-        stmt = f"INSERT INTO {self.table_name} ({keys}) VALUES ({values})"
+        stmt = f"INSERT INTO {self.table_name} ({keys}) VALUES {', '.join(values)}"
 
         connection = self.connect()
         cursor = self.cursor(connection)
         self.execute(cursor, stmt)
         self.commit(connection)
         self.close_connection(connection)
```

### Comparing `py_experimenter-1.2.0/py_experimenter/database_connector_lite.py` & `py_experimenter-1.2.1/py_experimenter/database_connector_lite.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         return set(columns) == set(config_columns)
 
     def _get_existing_rows(self, column_names):
         def _remove_string_markers(row):
             return row.replace("'", "")
         connection = self.connect()
         cursor = self.cursor(connection)
-        self.execute(cursor, f"SELECT {column_names} FROM {self.table_name}")
+        self.execute(cursor, f"SELECT {', '.join(column_names)} FROM {self.table_name}")
         existing_rows = list(map(np.array2string, np.array(self.fetchall(cursor))))
         existing_rows = [' '.join(_remove_string_markers(row).split()) for row in existing_rows]
         self.close_connection(connection)
         return existing_rows
 
     def get_structure_from_table(self, cursor):
         def _get_column_names_from_entries(entries):
```

### Comparing `py_experimenter-1.2.0/py_experimenter/database_connector_mysql.py` & `py_experimenter-1.2.1/py_experimenter/database_connector_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             return [' '.join(row.split()) for row in existing_rows]
 
         def _remove_string_markers(existing_rows):
             return [row.replace("'", "") for row in existing_rows]
 
         connection = self.connect()
         cursor = self.cursor(connection)
-        self.execute(cursor, f"SELECT {column_names} FROM {self.table_name}")
+        self.execute(cursor, f"SELECT {', '.join(column_names)} FROM {self.table_name}")
         existing_rows = list(map(np.array2string, np.array(self.fetchall(cursor))))
         existing_rows = _remove_string_markers(existing_rows)
         existing_rows = _remove_double_whitespaces(existing_rows)
         self.close_connection(connection)
         return existing_rows
 
     def get_structure_from_table(self, cursor):
```

### Comparing `py_experimenter-1.2.0/py_experimenter/exceptions.py` & `py_experimenter-1.2.1/py_experimenter/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.0/py_experimenter/experimenter.py` & `py_experimenter-1.2.1/py_experimenter/experimenter.py`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.0/py_experimenter/result_processor.py` & `py_experimenter-1.2.1/py_experimenter/result_processor.py`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.0/py_experimenter/utils.py` & `py_experimenter-1.2.1/py_experimenter/utils.py`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.0/pyproject.toml` & `py_experimenter-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-experimenter"
-version = "1.2.0"
+version = "1.2.1"
 description = "The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database."
 authors = [
     "Tanja Tornede <t.tornede@ai.uni-hannover.de>",
     "Alexander Tornede <a.tornede@ai.uni-hannover.de>",
     "Lukas Fehring <lukas.fehring@stud.uni-hannover.de>",
     "Lukas Gehring",
     "Helena Graf <h.graf@ai.uni-hannover.de>",
```

### Comparing `py_experimenter-1.2.0/setup.py` & `py_experimenter-1.2.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'jupyterlab>=3.5.0,<4.0.0',
  'mysql-connector-python>=8.0',
  'numpy>=1.15',
  'pandas>=1.0']
 
 setup_kwargs = {
     'name': 'py-experimenter',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database.',
-    'long_description': '[![doc](https://img.shields.io/badge/doc-success-success)](https://tornede.github.io/py_experimenter)\n[![pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)\n[![GitHub](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)\n\n<img src="docs/source/_static/py-experimenter-logo.png" alt="PyExperimenter Logo: Python biting a database" width="200px"/>\n\n# PyExperimenter\n\n`PyExperimenter` is a tool to facilitate the setup, documentation, execution, and subsequent evaluation of results from an empirical study of algorithms and in particular is designed to reduce the involved manual effort significantly.\nIt is intended to be used by researchers in the field of artificial intelligence, but is not limited to those.\n\nThe empirical analysis of algorithms is often accompanied by the execution of algorithms for different inputs and variants of the algorithms (specified via parameters) and the measurement of non-functional properties.\nSince the individual evaluations are usually independent, the evaluation can be performed in a distributed manner on an HPC system.\nHowever, setting up, documenting, and evaluating the results of such a study is often file-based.\nUsually, this requires extensive manual work to create configuration files for the inputs or to read and aggregate measured results from a report file.\nIn addition, monitoring and restarting individual executions is tedious and time-consuming.\n\nThese challenges are addressed by `PyExperimenter` by means of a single well defined configuration file and a central database for managing massively parallel evaluations, as well as collecting and aggregating their results.\nThereby, `PyExperimenter` alleviates the aforementioned overhead and allows experiment executions to be defined and monitored with ease.\n\n![General schema of `PyExperimenter`.](docs/source/_static/workflow.png)\n\nFor more details check out the [`PyExperimenter` documentation](https://tornede.github.io/py_experimenter/):\n\n- [Installation](https://tornede.github.io/py_experimenter/installation.html)\n- [Examples](https://tornede.github.io/py_experimenter/examples/example_general_usage.html)\n',
+    'long_description': '[![Project Homepage](https://img.shields.io/badge/Project%20Homepage-tornede.github.io/py_experimenter-0092CD)](https://tornede.github.io/py_experimenter)\n[![Pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)\n[![License](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.05149/status.svg)](https://doi.org/10.21105/joss.05149)\n\n![Tests](https://github.com/tornede/py_experimenter/actions/workflows/tests.yml/badge.svg)\n![GitHub Pages](https://github.com/tornede/py_experimenter/actions/workflows/github-pages.yml/badge.svg)\n\n<img src="docs/source/_static/py-experimenter-logo.png" alt="PyExperimenter Logo: Python biting a database" width="200px"/>\n\n# PyExperimenter\n\n`PyExperimenter` is a tool to facilitate the setup, documentation, execution, and subsequent evaluation of results from an empirical study of algorithms and in particular is designed to reduce the involved manual effort significantly.\nIt is intended to be used by researchers in the field of artificial intelligence, but is not limited to those.\n\nThe empirical analysis of algorithms is often accompanied by the execution of algorithms for different inputs and variants of the algorithms (specified via parameters) and the measurement of non-functional properties.\nSince the individual evaluations are usually independent, the evaluation can be performed in a distributed manner on an HPC system.\nHowever, setting up, documenting, and evaluating the results of such a study is often file-based.\nUsually, this requires extensive manual work to create configuration files for the inputs or to read and aggregate measured results from a report file.\nIn addition, monitoring and restarting individual executions is tedious and time-consuming.\n\nThese challenges are addressed by `PyExperimenter` by means of a single well defined configuration file and a central database for managing massively parallel evaluations, as well as collecting and aggregating their results.\nThereby, `PyExperimenter` alleviates the aforementioned overhead and allows experiment executions to be defined and monitored with ease.\n\n![General schema of `PyExperimenter`.](docs/source/_static/workflow.png)\n\nFor more details check out the [`PyExperimenter` documentation](https://tornede.github.io/py_experimenter/):\n\n- [Installation](https://tornede.github.io/py_experimenter/installation.html)\n- [Examples](https://tornede.github.io/py_experimenter/examples/example_general_usage.html)\n\n## Cite PyExperimenter\n\nIf you use `PyExperimenter` in a scientific publication, we would appreciate a citation in one of the following ways.\n\n### Citation String\n\nTornede et al., (2023). PyExperimenter: Easily distribute experiments and track results. Journal of Open Source Software, 8(84), 5149, https://doi.org/10.21105/joss.05149\n\n### BibTex\n```\n@article{Tornede2023, \n    title = {{PyExperimenter}: Easily distribute experiments and track results}, \n    author = {Tanja Tornede and Alexander Tornede and Lukas Fehring and Lukas Gehring and Helena Graf and Jonas Hanselle and Felix Mohr and Marcel Wever}, \n    journal = {Journal of Open Source Software},\n    publisher = {The Open Journal},  \n    year = {2023}, \n    volume = {8}, \n    number = {84}, \n    pages = {5149}, \n    doi = {10.21105/joss.05149}, \n    url = {https://doi.org/10.21105/joss.05149}\n}\n```\n',
     'author': 'Tanja Tornede',
     'author_email': 't.tornede@ai.uni-hannover.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tornede/py_experimenter',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `py_experimenter-1.2.0/PKG-INFO` & `py_experimenter-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-experimenter
-Version: 1.2.0
+Version: 1.2.1
 Summary: The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database.
 Home-page: https://github.com/tornede/py_experimenter
 License: MIT
 Keywords: python,experiments,database,executor
 Author: Tanja Tornede
 Author-email: t.tornede@ai.uni-hannover.de
 Requires-Python: >=3.9,<4.0
@@ -24,17 +24,21 @@
 Requires-Dist: mysql-connector-python (>=8.0)
 Requires-Dist: numpy (>=1.15)
 Requires-Dist: pandas (>=1.0)
 Project-URL: Documentation, https://tornede.github.io/py_experimenter/
 Project-URL: Repository, https://github.com/tornede/py_experimenter
 Description-Content-Type: text/markdown
 
-[![doc](https://img.shields.io/badge/doc-success-success)](https://tornede.github.io/py_experimenter)
-[![pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)
-[![GitHub](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)
+[![Project Homepage](https://img.shields.io/badge/Project%20Homepage-tornede.github.io/py_experimenter-0092CD)](https://tornede.github.io/py_experimenter)
+[![Pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)
+[![License](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05149/status.svg)](https://doi.org/10.21105/joss.05149)
+
+![Tests](https://github.com/tornede/py_experimenter/actions/workflows/tests.yml/badge.svg)
+![GitHub Pages](https://github.com/tornede/py_experimenter/actions/workflows/github-pages.yml/badge.svg)
 
 <img src="docs/source/_static/py-experimenter-logo.png" alt="PyExperimenter Logo: Python biting a database" width="200px"/>
 
 # PyExperimenter
 
 `PyExperimenter` is a tool to facilitate the setup, documentation, execution, and subsequent evaluation of results from an empirical study of algorithms and in particular is designed to reduce the involved manual effort significantly.
 It is intended to be used by researchers in the field of artificial intelligence, but is not limited to those.
@@ -51,7 +55,31 @@
 ![General schema of `PyExperimenter`.](docs/source/_static/workflow.png)
 
 For more details check out the [`PyExperimenter` documentation](https://tornede.github.io/py_experimenter/):
 
 - [Installation](https://tornede.github.io/py_experimenter/installation.html)
 - [Examples](https://tornede.github.io/py_experimenter/examples/example_general_usage.html)
 
+## Cite PyExperimenter
+
+If you use `PyExperimenter` in a scientific publication, we would appreciate a citation in one of the following ways.
+
+### Citation String
+
+Tornede et al., (2023). PyExperimenter: Easily distribute experiments and track results. Journal of Open Source Software, 8(84), 5149, https://doi.org/10.21105/joss.05149
+
+### BibTex
+```
+@article{Tornede2023, 
+    title = {{PyExperimenter}: Easily distribute experiments and track results}, 
+    author = {Tanja Tornede and Alexander Tornede and Lukas Fehring and Lukas Gehring and Helena Graf and Jonas Hanselle and Felix Mohr and Marcel Wever}, 
+    journal = {Journal of Open Source Software},
+    publisher = {The Open Journal},  
+    year = {2023}, 
+    volume = {8}, 
+    number = {84}, 
+    pages = {5149}, 
+    doi = {10.21105/joss.05149}, 
+    url = {https://doi.org/10.21105/joss.05149}
+}
+```
+
```

