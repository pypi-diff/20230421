# Comparing `tmp/ambrosia-0.3.0.tar.gz` & `tmp/ambrosia-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambrosia-0.3.0.tar", max compression
+gzip compressed data, was "ambrosia-0.4.0.tar", max compression
```

## Comparing `ambrosia-0.3.0.tar` & `ambrosia-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
--rw-r--r--   0        0        0    11419 2023-02-15 11:59:14.040142 ambrosia-0.3.0/LICENSE
--rw-r--r--   0        0        0     4549 2023-02-15 11:59:14.040142 ambrosia-0.3.0/README.rst
--rw-r--r--   0        0        0        6 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/VERSION
--rw-r--r--   0        0        0     1815 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/__init__.py
--rw-r--r--   0        0        0      991 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/designer/__init__.py
--rw-r--r--   0        0        0    33945 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/designer/designer.py
--rw-r--r--   0        0        0     3723 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/designer/handlers.py
--rw-r--r--   0        0        0     1189 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/preprocessing/__init__.py
--rw-r--r--   0        0        0     9977 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/preprocessing/aggregate.py
--rw-r--r--   0        0        0    18786 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/preprocessing/cuped.py
--rw-r--r--   0        0        0    12442 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/preprocessing/ml_var_reducer.py
--rw-r--r--   0        0        0    16192 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/preprocessing/preprocessor.py
--rw-r--r--   0        0        0    16535 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/preprocessing/robust.py
--rw-r--r--   0        0        0    12166 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/preprocessing/transformers.py
--rw-r--r--   0        0        0      749 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/spark_tools/__init__.py
--rw-r--r--   0        0        0    15653 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/spark_tools/empiric.py
--rw-r--r--   0        0        0     6853 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/spark_tools/split_tools.py
--rw-r--r--   0        0        0     4642 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/spark_tools/stat_criteria.py
--rw-r--r--   0        0        0     2141 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/spark_tools/stratification.py
--rw-r--r--   0        0        0     5923 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/spark_tools/theory.py
--rw-r--r--   0        0        0      766 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/splitter/__init__.py
--rw-r--r--   0        0        0     5268 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/splitter/handlers.py
--rw-r--r--   0        0        0    16444 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/splitter/splitter.py
--rw-r--r--   0        0        0      728 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tester/__init__.py
--rw-r--r--   0        0        0     4932 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tester/binary_result_evaluation.py
--rw-r--r--   0        0        0    27121 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tester/tester.py
--rw-r--r--   0        0        0      598 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/__init__.py
--rw-r--r--   0        0        0      598 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/_lib/__init__.py
--rw-r--r--   0        0        0     5609 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/_lib/_bin_ci_aide.py
--rw-r--r--   0        0        0     2420 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/_lib/_bootstrap_tools.py
--rw-r--r--   0        0        0     3071 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/_lib/_selection_aide.py
--rw-r--r--   0        0        0     6849 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/_lib/_tools_aide.py
--rw-r--r--   0        0        0    12761 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/ab_abstract_component.py
--rw-r--r--   0        0        0     1072 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/back_tools.py
--rw-r--r--   0        0        0    27067 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/bin_intervals.py
--rw-r--r--   0        0        0    16344 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/empirical_tools.py
--rw-r--r--   0        0        0     2387 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/knn.py
--rw-r--r--   0        0        0     2648 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/log.py
--rw-r--r--   0        0        0     9271 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/pvalue_tools.py
--rw-r--r--   0        0        0    17951 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/split_tools.py
--rw-r--r--   0        0        0    10365 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/stat_criteria.py
--rw-r--r--   0        0        0     5793 2023-02-15 11:59:14.040142 ambrosia-0.3.0/ambrosia/tools/stratification.py
--rw-r--r--   0        0        0    29988 2023-02-15 11:59:14.044142 ambrosia-0.3.0/ambrosia/tools/theoretical_tools.py
--rw-r--r--   0        0        0    44777 2023-02-15 11:59:14.044142 ambrosia-0.3.0/ambrosia/tools/tools.py
--rw-r--r--   0        0        0     5562 2023-02-15 11:59:14.044142 ambrosia-0.3.0/ambrosia/tools/type_checks.py
--rw-r--r--   0        0        0     3618 2023-02-15 11:59:14.044142 ambrosia-0.3.0/ambrosia/types.py
--rw-r--r--   0        0        0      797 2023-02-15 11:59:14.044142 ambrosia-0.3.0/ambrosia/version.py
--rw-r--r--   0        0        0     2456 2023-02-15 11:59:14.048142 ambrosia-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 ambrosia-0.3.0/setup.py
--rw-r--r--   0        0        0     6491 1970-01-01 00:00:00.000000 ambrosia-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11419 2023-04-21 15:59:30.505907 ambrosia-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4372 2023-04-21 15:59:30.505907 ambrosia-0.4.0/README.rst
+-rw-r--r--   0        0        0        6 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/VERSION
+-rw-r--r--   0        0        0     1815 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/__init__.py
+-rw-r--r--   0        0        0      991 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/designer/__init__.py
+-rw-r--r--   0        0        0    34918 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/designer/designer.py
+-rw-r--r--   0        0        0     3806 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/designer/handlers.py
+-rw-r--r--   0        0        0     1189 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/preprocessing/__init__.py
+-rw-r--r--   0        0        0     9977 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/preprocessing/aggregate.py
+-rw-r--r--   0        0        0    18786 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/preprocessing/cuped.py
+-rw-r--r--   0        0        0    12442 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/preprocessing/ml_var_reducer.py
+-rw-r--r--   0        0        0    16348 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/preprocessing/preprocessor.py
+-rw-r--r--   0        0        0    16535 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/preprocessing/robust.py
+-rw-r--r--   0        0        0    12166 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/preprocessing/transformers.py
+-rw-r--r--   0        0        0      749 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/spark_tools/__init__.py
+-rw-r--r--   0        0        0    15736 2023-04-21 15:59:30.505907 ambrosia-0.4.0/ambrosia/spark_tools/empiric.py
+-rw-r--r--   0        0        0     6939 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/spark_tools/split_tools.py
+-rw-r--r--   0        0        0    10956 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/spark_tools/stat_criteria.py
+-rw-r--r--   0        0        0     2228 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/spark_tools/stratification.py
+-rw-r--r--   0        0        0     6006 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/spark_tools/theory.py
+-rw-r--r--   0        0        0      766 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/splitter/__init__.py
+-rw-r--r--   0        0        0     5393 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/splitter/handlers.py
+-rw-r--r--   0        0        0    16966 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/splitter/splitter.py
+-rw-r--r--   0        0        0      728 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tester/__init__.py
+-rw-r--r--   0        0        0     4932 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tester/binary_result_evaluation.py
+-rw-r--r--   0        0        0     3755 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tester/handlers.py
+-rw-r--r--   0        0        0    27930 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tester/tester.py
+-rw-r--r--   0        0        0      860 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/_lib/__init__.py
+-rw-r--r--   0        0        0     5609 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/_lib/_bin_ci_aide.py
+-rw-r--r--   0        0        0     2420 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/_lib/_bootstrap_tools.py
+-rw-r--r--   0        0        0     3071 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/_lib/_selection_aide.py
+-rw-r--r--   0        0        0     7000 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/_lib/_tools_aide.py
+-rw-r--r--   0        0        0    13164 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/ab_abstract_component.py
+-rw-r--r--   0        0        0     2654 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/back_tools.py
+-rw-r--r--   0        0        0    28241 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/bin_intervals.py
+-rw-r--r--   0        0        0     1561 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/configs.py
+-rw-r--r--   0        0        0      575 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/decorators.py
+-rw-r--r--   0        0        0    20102 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/empirical_tools.py
+-rw-r--r--   0        0        0     1703 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/import_tools.py
+-rw-r--r--   0        0        0     2387 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/knn.py
+-rw-r--r--   0        0        0     2648 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/log.py
+-rw-r--r--   0        0        0     9271 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/pvalue_tools.py
+-rw-r--r--   0        0        0    18073 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/split_tools.py
+-rw-r--r--   0        0        0    10392 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/stat_criteria.py
+-rw-r--r--   0        0        0     5793 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/stratification.py
+-rw-r--r--   0        0        0    31724 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/theoretical_tools.py
+-rw-r--r--   0        0        0    40529 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/tools.py
+-rw-r--r--   0        0        0     5562 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/tools/type_checks.py
+-rw-r--r--   0        0        0     3904 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/types.py
+-rw-r--r--   0        0        0      797 2023-04-21 15:59:30.509907 ambrosia-0.4.0/ambrosia/version.py
+-rw-r--r--   0        0        0     2530 2023-04-21 15:59:30.517907 ambrosia-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5818 1970-01-01 00:00:00.000000 ambrosia-0.4.0/setup.py
+-rw-r--r--   0        0        0     6355 1970-01-01 00:00:00.000000 ambrosia-0.4.0/PKG-INFO
```

### Comparing `ambrosia-0.3.0/LICENSE` & `ambrosia-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/README.rst` & `ambrosia-0.4.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -27,43 +27,30 @@
 .. image:: https://raw.githubusercontent.com/MobileTeleSystems/Ambrosia/main/docs/source/_static/ambrosia.png
    :height: 320 px
    :width: 320 px
    :align: center
 
 .. title
 
-**Ambrosia** is a Python library for A/B tests design, split and effect 
-measurement. It provides rich set of methods for conducting full 
-A/B test pipeline. 
-
-An experiment design stage is performed using metrics historical data 
-which could be processed in both forms of pandas and spark dataframes 
-with either theoretical or empirical approach. 
-
-Group split methods support different strategies and multi-group split, 
-which allows to quickly create control and test groups of interest. 
-
-Final effect measurement stage is conducted via testing tools that 
-are able to return relative and absolute effects and construct corresponding 
-confidence intervalsfor continious and binary variables. 
-Testing tools as well as design ones support significant number of 
-statistical criteria, like t-test, non-parametric, and bootstrap. 
+*Ambrosia* is a Python library for A/B tests design, split and effect measurement. 
+It provides rich set of methods for conducting full A/B testing pipeline. 
 
-For additional A/B tests support library provides features and tools 
-for data preproccesing and experiment acceleration.
+The project is intended for use in research and production environments 
+based on data in pandas and Spark format.
 
 .. functional
 
 Key functionality
 -----------------
 
-* Pilots design ✈
+* Pilots design 🛫
 * Multi-group split 🎳
 * Matching of new control group to the existing pilot 🎏
-* Getting the experiments result evaluation as p-value, point estimate of effect and confidence interval 🎞
+* Experiments result evaluation as p-value, point estimate of effect and confidence interval 🎞
+* Data preprocessing ✂️
 * Experiments acceleration 🎢
 
 .. documentation
 
 Documentation
 -------------
 
@@ -71,49 +58,59 @@
 and `Tutorials <https://github.com/MobileTeleSystems/Ambrosia/tree/main/examples>`_.
 
 .. install
 
 Installation
 ------------
 
+You can always get the newest *Ambrosia* release using ``pip``.
 Stable version is released on every tag to ``main`` branch. 
 
 .. code:: bash
     
     pip install ambrosia 
 
-**Ambrosia requires Python 3.7+**
+Starting from version ``0.4.0``, the ability to process PySpark data is optional and can be enabled 
+using ``pip`` extras during the installation.
+
+.. code:: bash
+    
+    pip install ambrosia[pyspark]
 
 .. usage
 
 Usage
 -----
 
-Designer 
-~~~~~~~~
+The main functionality of *Ambrosia* is contained in several core classes and methods, 
+which are autonomic for each stage of an experiment and have very intuitive interface. 
+
+|
+
+Below is a brief overview example of using a set of three classes to conduct some simple experiment.
+
+**Designer**
 
 .. code:: python
 
     from ambrosia.designer import Designer
     designer = Designer(dataframe=df, effects=1.2, metrics='portfel_clc') # 20% effect, and loaded data frame df
     designer.run('size') 
 
 
-Splitter
-~~~~~~~~
+**Splitter**
 
 .. code:: python
 
     from ambrosia.splitter import Splitter
     splitter = Splitter(dataframe=df, id_column='id') # loaded data frame df with column with id - 'id'
     splitter.run(groups_size=500, method='simple') 
 
 
-Tester 
-~~~~~~
+**Tester**
 
 .. code:: python
 
     from ambrosia.tester import Tester
     tester = Tester(dataframe=df, column_groups='group') # loaded data frame df with groups info 'group'
     tester.run(metrics='retention', method='theory', criterion='ttest')
 
@@ -158,15 +155,15 @@
 
 .. code:: bash
 
     make clean
 
 .. contributors
 
-Communication
--------------
+Authors
+-------
 
 **Developers and evangelists**:
 
 * `Bayramkulov Aslan <https://github.com/aslanbm>`_
 * `Khakimov Artem <https://github.com/xandaau>`_
 * `Vasin Artem <https://github.com/VictorFromChoback>`_
```

### Comparing `ambrosia-0.3.0/ambrosia/__init__.py` & `ambrosia-0.4.0/ambrosia/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/designer/__init__.py` & `ambrosia-0.4.0/ambrosia/designer/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/designer/designer.py` & `ambrosia-0.4.0/ambrosia/designer/designer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+
 """
 Experiment design methods.
 
 Module contains `Designer` core class and `design` method which are
 intended to conduct the experiment design for A/B/.. tests via different
 methods.
 
@@ -44,18 +45,19 @@
 EFFECT: str = "effect"
 POWER: str = "power"
 BINARY_DESIGN_METHODS: List[str] = ["theory", "binary"]
 
 
 class Designer(yaml.YAMLObject, ABToolAbstract, metaclass=ABMetaClass):
     """
-    Unit for experiments and pilots design.
+    Unit for experiments and pilots parameters design.
 
     Enables to design missing experiment parameters using historical data.
     The main related to each other designable parameters for a single metric are:
+
         - Effect (Minimal Detectible Effect):
             old_mean_metric_value * effect_value = new_mean_metric_value
         - Sample size:
             Number of research objects in sample
             (for example number of users and their retention).
         - Errors (I type error, II type error):
             I error (alpha):
@@ -119,69 +121,73 @@
 
     We add onboarding to our app and want to estimate an effect, by A/B testing
     and wish to increase retention value to 31% percents, so our effect
     parameter gets value of ``1.0(3)``. Now we want to find how much users we
     need in both groups to detect such effect.
 
     We can use ``Designer`` class in the following way:
-        >>> designer = Designer(dataframe=df, metric='retention', effect=1.033)
-        >>> designer.run("size")
+
+    >>> designer = Designer(dataframe=df, metric='retention', effect=1.033)
+    >>> designer.run("size")
 
     Note, that default values for errors are:
         ``first_type_error`` = ``0.05``
 
         ``second_type_error`` = ``0.2``
 
     Then we get dataframe that contains value of  sufficient number of users
     for our experiment.
 
     Notes
     -----
 
     Constructors:
-        >>> designer = Designer()
-        >>> # You can pass an Iterable or single object for some parameters
-        >>> designer = Designer(
-        >>>     dataframe=df,
-        >>>     sizes=[100, 200],
-        >>>     metrics='LTV',
-        >>>     effects=1.05
-        >>> )
-        >>> designer = Desginer(sizes=1000, metrics=['retention', 'LTV'])
-        >>> # You can use path to .csv table for pandas
-        >>> designer = Designer('./data/table.csv')
+
+    >>> designer = Designer()
+    >>> # You can pass an Iterable or single object for some parameters
+    >>> designer = Designer(
+    >>>     dataframe=df,
+    >>>     sizes=[100, 200],
+    >>>     metrics='LTV',
+    >>>     effects=1.05
+    >>> )
+    >>> designer = Desginer(sizes=1000, metrics=['retention', 'LTV'])
+    >>> # You can use path to .csv table for pandas
+    >>> designer = Designer('./data/table.csv')
 
     Setters:
-        >>> designer.set_first_errors([0.05, 0.01])
-        >>> desginer.set_dataframe(df)
+
+    >>> designer.set_first_errors([0.05, 0.01])
+    >>> desginer.set_dataframe(df)
 
     Run:
-        >>> # One can pass arguments and they will have higher priority
-        >>> designer.run('size', effects=1.1)
-        >>> designer.run('effect', sizes=[500, 1000], metrics='retention')
-        >>> # You can set method (watch below)
-        >>> designer.run('effect', sizes=[500, 1000], metrics='retention', method='binary')
+
+    >>> # One can pass arguments and they will have higher priority
+    >>> designer.run('size', effects=1.1)
+    >>> designer.run('effect', sizes=[500, 1000], metrics='retention')
+    >>> # You can set method (watch below)
+    >>> designer.run('effect', sizes=[500, 1000], metrics='retention', method='binary')
 
     Load from yaml config:
-        >>> config = '''
-                !splitter # <--- this is yaml tag (!important)
-                    effects:
-                        - 0.9
-                        - 1.05
-                    sizes:
-                        - 1000
-                    dataframe:
-                        ./data/table.csv
-            '''
-        >>> designer = yaml.load(config)
-        >>> # Or use the implmented function
-        >>> designer = load_from_config(config)
+
+    >>> config = '''
+            !splitter # <--- this is yaml tag (!important)
+                effects:
+                    - 0.9
+                    - 1.05
+                sizes:
+                    - 1000
+        '''
+    >>> designer = yaml.load(config)
+    >>> # Or use the implmented function
+    >>> designer = load_from_config(config)
 
     Use standalone function instead of a class:
-        >>> design('size', dataframe=df, effects=1.05, metrics='retention')
+
+    >>> design('size', dataframe=df, effects=1.05, metrics='retention')
     """
 
     # YAML tag for loading from configs
     yaml_tag = "!designer"
 
     def set_first_errors(self, first_type_errors: types.StatErrorType) -> None:
         if isinstance(first_type_errors, float):
@@ -198,15 +204,15 @@
     def set_sizes(self, sizes: types.SampleSizeType) -> None:
         if isinstance(sizes, int):
             self.__size = [sizes]
         else:
             self.__size = sizes
 
     def set_effects(self, effects: types.EffectType) -> None:
-        if isinstance(effects, float):
+        if isinstance(effects, (float, int)):
             self.__effect = [effects]
         else:
             self.__effect = effects
 
     def set_dataframe(self, dataframe: types.PassedDataType) -> None:
         if isinstance(dataframe, str):
             if dataframe.endswith(".csv"):
@@ -242,14 +248,27 @@
         self.set_second_errors(second_type_errors)
         self.set_sizes(sizes)
         self.set_effects(effects)
         self.set_metrics(metrics)
         self.set_dataframe(dataframe)
         self.set_method(method)
 
+    def __getstate__(self):
+        """
+        Get the state of the object to serialize.
+        """
+        return dict(
+            effects=self.__effect,
+            sizes=self.__size,
+            first_type_errors=self.__alpha,
+            second_type_errors=self.__beta,
+            metrics=self.__metrics,
+            method=self.__method,
+        )
+
     @classmethod
     def from_yaml(cls, loader: yaml.Loader, node: yaml.Node):
         kwargs = loader.construct_mapping(node)
         return cls(**kwargs)
 
     @staticmethod
     def __dataframe_handler(handler: SimpleDesigner, parameter: str, **kwargs) -> pd.DataFrame:
@@ -302,16 +321,17 @@
         if label == SIZE:
             kwargs["effects"] = args[EFFECT]
             kwargs["betas"] = np.array(args["beta"])
         elif label == EFFECT:
             kwargs["group_sizes"] = args[SIZE]
             kwargs["betas"] = np.array(args["beta"])
         elif label == POWER:
+            groups_ratio: float = kwargs.pop("groups_ratio") if "groups_ratio" in kwargs else 1.0
             kwargs["sample_sizes_a"] = args[SIZE]
-            kwargs["sample_sizes_b"] = args[SIZE]
+            kwargs["sample_sizes_b"] = [int(groups_ratio * size) for size in args[SIZE]]
             kwargs["effects"] = args[EFFECT]
         return Designer.__dataframe_handler(EmpiricHandler(), label, **kwargs)
 
     @staticmethod
     def __binary_design(label: str, args: types._UsageArgumentsType, **kwargs) -> types.DesignerResult:
         """
         Designing an experiment, using the approach for binary metrics.
@@ -401,35 +421,33 @@
         Other Parameters
         ----------------
         as_numeric : bool, default: ``False``
             The result of calculations can be obtained as a percentage string
             either as a number, this parameter could used to toggle.
         groups_ratio : float, default: ``1.0``
             Ratio between two groups.
-            Acceptable only for ``"theory"`` method!
         alternative : str, default: ``"two-sided"``
             Alternative hypothesis, can be ``"two-sided"``, ``"greater"``
             or ``"less"``.
             ``"greater"`` - if effect is positive.
             ``"less"`` - if effect is negative.
-            Acceptable only for ``"theory"`` method!
         stabilizing_method : str, default: ``"asin"``
             Effect trasformation. Can be ``"asin"`` and ``"norm"``.
             For non-binary metrics: only ``"norm"`` is accceptable.
             For binary metrics: ``"norm"`` and ``"asin"``, but ``"asin"``
             is more robust and accurate.
             Acceptable only for ``"theory"`` method and actual for binary metrics!
 
         Returns
         -------
         result : DesignerResult
             Table or dictionary with the results of parameter design for each
             metric.
         """
-        if isinstance(effects, float):
+        if isinstance(effects, (float, int)):
             effects = [effects]
         if isinstance(sizes, int):
             sizes = [sizes]
         if isinstance(first_type_errors, float):
             first_type_errors = [first_type_errors]
         if isinstance(second_type_errors, float):
             second_type_errors = [second_type_errors]
@@ -440,15 +458,14 @@
             "df": (self.__df, dataframe),
             "alpha": (self.__alpha, first_type_errors),
             "metric": (self.__metrics, metrics),
             "method": (self.__method, method),
         }
 
         designable_parameters: List[str] = [SIZE, EFFECT, POWER]
-
         if to_design == SIZE:
             arguments_choice[EFFECT] = (self.__effect, effects)
             arguments_choice["beta"] = (self.__beta, second_type_errors)
             chosen_args: types._UsageArgumentsType = Designer._prepare_arguments(arguments_choice)
             return Designer.__pre_design(SIZE, chosen_args, **kwargs)
         elif to_design == EFFECT:
             arguments_choice[SIZE] = (self.__size, sizes)
@@ -462,15 +479,15 @@
             return Designer.__pre_design(POWER, chosen_args, **kwargs)
         else:
             raise ValueError(f'Incorrect parameter name to design, choose from {", ".join(designable_parameters)}')
 
 
 def load_from_config(yaml_config: str, loader: type = yaml.Loader) -> Designer:
     """
-    Create Designer class instance from yaml config.
+    Restore a ``Designer`` class instance from a yaml config.
 
     For yaml_config you can pass file name with config,
     it must ends with .yaml, for example: "config.yaml".
 
     For loader you can choose SafeLoader.
     """
     if isinstance(yaml_config, str) and yaml_config.endswith(".yaml"):
@@ -487,16 +504,21 @@
     effects: types.EffectType = None,
     first_type_errors: types.StatErrorType = (0.05,),
     second_type_errors: types.StatErrorType = (0.2,),
     method: str = "theory",
     **kwargs,
 ) -> types.DesignerResult:
     """
+    Function wrapper around the ``Designer`` class.
+
     Make experiment design based on historical data using passed arguments.
 
+    Creates an instance of the ``Designer`` class internally and execute
+    run method with corresponding arguments.
+
     Parameters
     ----------
     to_design : str
         Parameter that will be designed using historical data.
         Can take the values of ``"size"``, ``"effect"`` or ``"power"``.
     dataframe : PassedDataType
         DataFrame with metrics historical values.
@@ -524,21 +546,19 @@
     Other Parameters
     ----------------
     as_numeric : bool, default: ``False``
         The result of calculations can be obtained as a percentage string
         either as a number, this parameter could used to toggle.
     groups_ratio : float, default: ``1.0``
         Ratio between two groups.
-        Acceptable only for ``"theory"`` method!
     alternative : str, default: ``"two-sided"``
         Alternative hypothesis, can be ``"two-sided"``, ``"greater"``
         or ``"less"``.
         ``"greater"`` - if effect is positive.
         ``"less"`` - if effect is negative.
-        Acceptable only for ``"theory"`` method!
     stabilizing_method : str, default: ``"asin"``
         Effect trasformation. Can be ``"asin"`` and ``"norm"``.
         For non-binary metrics: only ``"norm"`` is accceptable.
         For binary metrics: ``"norm"`` and ``"asin"``, but ``"asin"``
         is more robust and accurate.
         Acceptable only for ``"theory"`` method and actual for binary metrics!
 
@@ -606,15 +626,15 @@
         Other keyword arguments.
 
     Returns
     -------
     result_table : pd.DataFrame
         Table with results of design.
     """
-    if isinstance(effects, float):
+    if isinstance(effects, (float, int)):
         effects = [effects]
     if isinstance(first_type_errors, float):
         first_type_errors = [first_type_errors]
     if isinstance(second_type_errors, float):
         second_type_errors = [second_type_errors]
     if method == "theory":
         return theory_pkg.get_table_sample_size(
@@ -645,14 +665,15 @@
     sizes: types.SampleSizeType,
     first_type_errors: types.StatErrorType = (0.05,),
     second_type_errors: types.StatErrorType = (0.2,),
     method: str = "theory",
     groups_ratio: float = 1.0,
     alternative: str = "two-sided",
     stabilizing_method: str = "asin",
+    as_numeric: bool = False,
     **kwargs,
 ) -> pd.DataFrame:
     """
     Design effect for binary metrics.
 
     Parameters
     ----------
@@ -679,14 +700,17 @@
         ``"greater"`` - if effect is positive.
         ``"less"`` - if effect is negative.
     stabilizing_method : str, default: ``"asin"``
         Effect trasformation. Can be ``"asin"`` and ``"norm"``.
         For non-binary metrics: only ``"norm"`` is accceptable.
         For binary metrics: ``"norm"`` and ``"asin"``, but ``"asin"``
         is more robust and accurate.
+    as_numeric : bool, default: ``False``
+        The result of calculations can be obtained as a percentage string
+        either as a number, this parameter could used to toggle.
     **kwargs : Dict
         Other keyword arguments.
 
     Returns
     -------
     result_table : pd.DataFrame
         Table with results of design.
@@ -700,36 +724,43 @@
     if method == "theory":
         return theory_pkg.get_minimal_effects_table(
             mean=prob_a,
             std=None,
             sample_sizes=sizes,
             first_errors=first_type_errors,
             second_errors=second_type_errors,
+            as_numeric=as_numeric,
             target_type="binary",
             groups_ratio=groups_ratio,
             alternative=alternative,
             stabilizing_method=stabilizing_method,
         )
     elif method == "binary":
         return bin_pkg.get_table_effect_on_sample_size(
-            p_a=prob_a, sample_sizes=sizes, first_errors=first_type_errors, second_errors=second_type_errors, **kwargs
+            p_a=prob_a,
+            sample_sizes=sizes,
+            first_errors=first_type_errors,
+            second_errors=second_type_errors,
+            as_numeric=as_numeric,
+            **kwargs,
         )
     else:
         raise ValueError(f"Choose valid method from {BINARY_DESIGN_METHODS}, got {method}")
 
 
 def design_binary_power(
     prob_a: float,
     sizes: types.SampleSizeType,
     effects: types.EffectType,
     first_type_errors: types.StatErrorType = (0.05,),
     method: str = "theory",
     groups_ratio: float = 1.0,
     alternative: str = "two-sided",
     stabilizing_method: str = "asin",
+    as_numeric: bool = False,
     **kwargs,
 ) -> pd.DataFrame:
     """
     Design power for binary metrics.
 
     Parameters
     ----------
@@ -756,46 +787,51 @@
         ``"greater"`` - if effect is positive.
         ``"less"`` - if effect is negative.
     stabilizing_method : str, default: ``"asin"``
         Effect trasformation. Can be ``"asin"`` and ``"norm"``.
         For non-binary metrics: only ``"norm"`` is accceptable.
         For binary metrics: ``"norm"`` and ``"asin"``, but ``"asin"``
         is more robust and accurate.
+    as_numeric : bool, default: ``False``
+        The result of calculations can be obtained as a percentage string
+        either as a number, this parameter could used to toggle.
     **kwargs : Dict
         Other keyword arguments.
 
     Returns
     -------
     result_table : pd.DataFrame
         Table with results of design.
     """
-    if isinstance(effects, float):
+    if isinstance(effects, (int, float)):
         effects = [effects]
     if isinstance(sizes, int):
         sizes = [sizes]
     if isinstance(first_type_errors, float):
         first_type_errors = [first_type_errors]
     if method == "theory":
         return theory_pkg.get_power_table(
             mean=prob_a,
             std=None,
             sample_sizes=sizes,
             effects=effects,
             first_errors=first_type_errors,
+            as_numeric=as_numeric,
             target_type="binary",
             groups_ratio=groups_ratio,
             alternative=alternative,
             stabilizing_method=stabilizing_method,
         )
     elif method == "binary":
         return bin_pkg.get_table_power_on_size_and_delta(
             p_a=prob_a,
             sample_sizes=sizes,
             first_errors=first_type_errors,
             delta_relative_values=effects,
+            as_numeric=as_numeric,
             **kwargs,
         )
     else:
         raise ValueError(f"Choose valid method from {BINARY_DESIGN_METHODS}, got {method}")
 
 
 def design_binary(
@@ -808,15 +844,16 @@
     method: str = "theory",
     groups_ratio: float = 1.0,
     alternative: str = "two-sided",
     stabilizing_method: str = "asin",
     **kwargs,
 ) -> pd.DataFrame:
     """
-    Design desired parameter for binary metrics.
+    Design of experiment parameters for binary metrics based
+    on a known conversion value.
 
     Parameters
     ----------
     to_design : str
         Parameter to design.
     prob_a : float
         Probability of success for the control group.
@@ -844,15 +881,14 @@
         ``"greater"`` - if effect is positive.
         ``"less"`` - if effect is negative.
     stabilizing_method : str, default: ``"asin"``
         Effect trasformation. Can be ``"asin"`` and ``"norm"``.
         For non-binary metrics: only ``"norm"`` is accceptable.
         For binary metrics: ``"norm"`` and ``"asin"``, but ``"asin"``
         is more robust and accurate.
-
     **kwargs : Dict
         Other keyword arguments.
 
     Returns
     -------
     result_table : pd.DataFrame
         Table with results of design.
```

### Comparing `ambrosia-0.3.0/ambrosia/designer/handlers.py` & `ambrosia-0.4.0/ambrosia/designer/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,22 +20,26 @@
 
 These objects are used in `Designer` core class.
 """
 import warnings
 from typing import List
 
 import pandas as pd
-import pyspark.sql.functions as spark_functions
 
 import ambrosia.spark_tools.empiric as empiric_spark
 import ambrosia.spark_tools.theory as theory_spark
 import ambrosia.tools.theoretical_tools as theory_pkg
 import ambrosia.tools.tools as empiric_pkg
 from ambrosia import types
 from ambrosia.tools.ab_abstract_component import SimpleDesigner
+from ambrosia.tools.import_tools import spark_installed
+
+if spark_installed():
+    import pyspark.sql.functions as spark_functions
+
 
 DATA: str = "dataframe"
 AVAILABLE: List[str] = ["pandas", "spark"]
 AVAILABLE_TABLES_ERROR = TypeError(f'Type of table must be one of {", ".join(AVAILABLE)}')
 
 
 class TheoryHandler(SimpleDesigner):
@@ -65,15 +69,15 @@
         return self._handle_cases(empiric_pkg.get_empirical_mde_table, empiric_spark.get_table_effect, **kwargs)
 
     def power_design(self, **kwargs) -> pd.DataFrame:
         if isinstance(kwargs[DATA], types.SparkDataFrame):
             kwargs["group_sizes"] = kwargs["sample_sizes_a"]
             del kwargs["sample_sizes_a"]
             del kwargs["sample_sizes_b"]
-        return self._handle_cases(empiric_pkg.get_empirical_errors_table, empiric_spark.get_table_power, **kwargs)
+        return self._handle_cases(empiric_pkg.get_empirical_table_power, empiric_spark.get_table_power, **kwargs)
 
 
 def calc_prob_control_class(table: types.PassedDataType, metric: types.MetricNameType) -> float:
     """
     Calculate conversion on binary metric for pandas or Spark dataframe.
 
     Parameters
```

### Comparing `ambrosia-0.3.0/ambrosia/preprocessing/__init__.py` & `ambrosia-0.4.0/ambrosia/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/preprocessing/aggregate.py` & `ambrosia-0.4.0/ambrosia/preprocessing/aggregate.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/preprocessing/cuped.py` & `ambrosia-0.4.0/ambrosia/preprocessing/cuped.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/preprocessing/ml_var_reducer.py` & `ambrosia-0.4.0/ambrosia/preprocessing/ml_var_reducer.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/preprocessing/preprocessor.py` & `ambrosia-0.4.0/ambrosia/preprocessing/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,15 +441,18 @@
 
         Returns
         -------
         dataframe : pd.DataFrame
             Transformed inner data frame
         """
         for transformer in self.transformers:
-            transformer.transform(self.dataframe, inplace=True)
+            if isinstance(transformer, AggregatePreprocessor):
+                self.dataframe = transformer.transform(self.dataframe)
+            else:
+                transformer.transform(self.dataframe, inplace=True)
         return self.data()
 
     def transform_from_config(self, load_path: Path) -> pd.DataFrame:
         """
         Run transformations from the config file on the internal data frame.
 
         Parameters
```

### Comparing `ambrosia-0.3.0/ambrosia/preprocessing/robust.py` & `ambrosia-0.4.0/ambrosia/preprocessing/robust.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         """
         self.fit(dataframe, column_names, alpha, tail)
         return self.transform(dataframe, inplace)
 
 
 class IQRPreprocessor(AbstractFittableTransformer):
     """
-    Unit for iqr transformation of the data to exclude outliers.
+    Unit for IQR transformation of the data to exclude outliers.
 
     It cuts the points from the distribution which are behind the range of
     0.25 quantile - 1,5 * iqr and 0.75 quantile + 1,5 * iqr
     for each given metric.
 
 
     Parameters
```

### Comparing `ambrosia-0.3.0/ambrosia/preprocessing/transformers.py` & `ambrosia-0.4.0/ambrosia/preprocessing/transformers.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/spark_tools/__init__.py` & `ambrosia-0.4.0/ambrosia/spark_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/spark_tools/empiric.py` & `ambrosia-0.4.0/ambrosia/spark_tools/empiric.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Any, Dict, Iterable, List
 
 import numpy as np
 import pandas as pd
-import pyspark.sql.functions as spark_functions
 from joblib import Parallel, delayed, parallel_backend
 from tqdm.auto import tqdm
 
 import ambrosia.spark_tools.theory as th_pkg
 import ambrosia.tools._lib._bootstrap_tools as solver_pkg
 import ambrosia.tools._lib._selection_aide as select_pkg
 from ambrosia import types
+from ambrosia.tools.import_tools import spark_installed
+
+if spark_installed():
+    import pyspark.sql.functions as spark_functions
 
 BOOSTRAP_BASE_CONST: int = 10
 RANDOM_SAMPLE_SEED: int = 42
 FIRST_TYPE_ERROR: float = 0.05
 THREADS_BOOTSTRAP: int = 2  # Creates a significant reduction in runtime
 N_JOBS_MULTIPROCESS: int = 1
 ACCEPTED_CRITERIA: List[str] = ["ttest"]
```

### Comparing `ambrosia-0.3.0/ambrosia/spark_tools/split_tools.py` & `ambrosia-0.4.0/ambrosia/spark_tools/split_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Iterable, List, Optional
 
-import pyspark.sql.functions as spark_funcs
-from pyspark.sql import Window
-
 import ambrosia.spark_tools.stratification as strat_pkg
 from ambrosia import types
 from ambrosia.tools import split_tools
+from ambrosia.tools.import_tools import spark_installed
+
+if spark_installed():
+    import pyspark.sql.functions as spark_funcs
+    from pyspark.sql import Window
 
 HASH_COLUMN_NAME: str = "__hashed_ambrosia_column"
 GROUPS_COLUMN: str = "group"
 ROW_NUMBER: str = "__row_number"
 EMPTY_VALUE: int = 0
```

### Comparing `ambrosia-0.3.0/ambrosia/spark_tools/stratification.py` & `ambrosia-0.4.0/ambrosia/spark_tools/stratification.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Any, Dict, Iterable, Optional
 
-import pyspark.sql.functions as spark_funcs
-from pyspark.sql import Window
-
 import ambrosia.tools.ab_abstract_component as ab_abstract
 from ambrosia import types
+from ambrosia.tools.import_tools import spark_installed
+
+if spark_installed():
+    import pyspark.sql.functions as spark_funcs
+    from pyspark.sql import Window
+
 
 EMPTY_VALUE: int = 0
 STRAT_GROUPS: str = "__ambrosia_strat"
 
 
 class Stratification(ab_abstract.StratificationUtil):
     """
```

### Comparing `ambrosia-0.3.0/ambrosia/spark_tools/theory.py` & `ambrosia-0.4.0/ambrosia/spark_tools/theory.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Iterable, Tuple
 
 import pandas as pd
-import pyspark.sql.functions as funcs
 import scipy.stats as sps
 
 import ambrosia.tools.theoretical_tools as theory_pkg
 from ambrosia import types
+from ambrosia.tools.import_tools import spark_installed
+
+if spark_installed():
+    import pyspark.sql.functions as funcs
 
 
 def get_stats_from_table(dataframe: types.SparkDataFrame, column: types.ColumnNameType) -> Tuple[float, float]:
     """
     Get table for designing samples size for experiment.
     """
     stats = dataframe.select(
```

### Comparing `ambrosia-0.3.0/ambrosia/splitter/__init__.py` & `ambrosia-0.4.0/ambrosia/splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/splitter/handlers.py` & `ambrosia-0.4.0/ambrosia/splitter/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,25 @@
 with data of different type during the groups split task.
 
 Mainly these functions are used in `Splitter` core class.
 """
 from typing import List, Optional
 
 import pandas as pd
-import pyspark.sql.functions as spark_funcs
 
 import ambrosia.spark_tools.split_tools as split_spark
 import ambrosia.tools.split_tools as split_pandas
 from ambrosia import types
+from ambrosia.tools.import_tools import spark_installed
+
+# Avoid errors with not installed spark
+
+if spark_installed():
+    import pyspark.sql.functions as spark_funcs
+
 
 AVAILABLE: List[str] = ["pandas", "spark"]
 GROUPS_COLUMN: str = "group"
 DATA: str = "dataframe"
 THREADS: str = "threads"
```

### Comparing `ambrosia-0.3.0/ambrosia/splitter/splitter.py` & `ambrosia-0.4.0/ambrosia/splitter/splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from .handlers import data_shape, handle_full_split, split_data_handler
 
 SPLITTING_BOUND_CONST: float = 0.5
 
 
 class Splitter(yaml.YAMLObject, ABToolAbstract, metaclass=ABMetaClass):
     """
-    Unit for splitting data into groups.
+    Unit for creating experimental groups from batch data.
 
     Split your data into groups of selected size with respect to:
         - Stratification columns
         - Metric distance of objects in feature space
         - Set of passed ids
 
     Parameters
@@ -107,14 +107,15 @@
     >>> splitter.run(method='hash',
     >>>              salt='onboarding',
     >>>              test_group_ids=B_group_id
     >>> )
 
     Notes
     -----
+
     Main methods for split:
 
     Simple:
         - Randomly chosen groups (via ``np.random.choice``).
 
     Hash:
         - Using hashing of identifiers and distribution
@@ -123,58 +124,59 @@
     Metric:
         - For a fixed reference group or a randomly selected one,
           other groups are selected using the nearest neighbor method
           (for desired list of columns passed in ``fit_columns`` parameter).
 
     Constructors:
 
-    >>> # Empty constructor
-    >>> splitter = Splitter()
-    >>> # Some data
-    >>> splitter = Splitter(dataframe=df,
-    >>>                     id_column='my_id_column',
-    >>>                     strat_columns=['gender', 'age'],
-    >>>                     test_group_ids=ids_for_B_group
-    >>> )
+        >>> # Empty constructor
+        >>> splitter = Splitter()
+        >>> # Some data
+        >>> splitter = Splitter(dataframe=df,
+        >>>                     id_column='my_id_column',
+        >>>                     strat_columns=['gender', 'age'],
+        >>>                     test_group_ids=ids_for_B_group
+        >>> )
 
     Setters:
 
-    >>> splitter.set_dataframe(dataframe)
-    >>> # You can pass string for pd.read_csv
-    >>> splitter.set_dataframe('name_of_table.csv')
-    >>> # Other setters
-    >>> splitter.set_group_size(1000)
-    >>> splitter.set_strat_columns(['age', 'region'])
+        >>> splitter.set_dataframe(dataframe)
+        >>> # You can pass string for pd.read_csv
+        >>> splitter.set_dataframe('name_of_table.csv')
+        >>> # Other setters
+        >>> splitter.set_group_size(1000)
+        >>> splitter.set_strat_columns(['age', 'region'])
 
     Run:
 
-    >>> splitter.run(method='hash', groups_size=10000)
-    >>> splitter.run(method='metric'
-    >>>              test_group_ids=b_group,
-    >>>              id_column='id',
-    >>>              strat_columns=['age', 'city']
-    >>>              fit_columns=['metric_history_column', 'other_metric']
-    >>>              method_meric='fast', # It is used as kwarg
-    >>>              norm='l2' # It is used as kwarg
-    >>> )
+        >>> splitter.run(method='hash', groups_size=10000)
+        >>> splitter.run(method='metric'
+        >>>              test_group_ids=b_group,
+        >>>              id_column='id',
+        >>>              strat_columns=['age', 'city']
+        >>>              fit_columns=['metric_history_column', 'other_metric']
+        >>>              method_meric='fast', # It is used as kwarg
+        >>>              norm='l2' # It is used as kwarg
+        >>> )
 
-    YAML config:
+    Load from yaml config:
 
     >>> config = '''
                 !splitter # <--- this is yaml tag (important!)
                     groups_size:
                         1000
-                    dataframe:
-                        ./data/table.csv
                     id_column:
                         id
                     strat_columns:
                         - age
                         - country
             '''
+    >>> splitter = yaml.load(config)
+    >>> # Or use the implmented function
+    >>> splitter = load_from_config(config)
     """
 
     yaml_tag = "!splitter"
 
     @type_checks.check_type_decorator(type_checks.check_type_dataframe)
     def set_dataframe(self, dataframe: Optional[types.PassedDataType]) -> None:
         self.__df = dataframe
@@ -214,14 +216,25 @@
         self.set_dataframe(dataframe)
         self.set_id_column(id_column)
         self.set_group_size(groups_size)
         self.set_test_group_ids(test_group_ids)
         self.set_fit_columns(fit_columns)
         self.set_strat_columns(strat_columns)
 
+    def __getstate__(self):
+        """
+        Get the state of the object to serialize.
+        """
+        return dict(
+            id_column=self.__id_column,
+            groups_size=self.__groups_size,
+            fit_columns=self.__fit_columns,
+            strat_columns=self.__strat_columns,
+        )
+
     @classmethod
     def from_yaml(cls, loader: yaml.Loader, node: yaml.Node):
         kwargs = loader.construct_mapping(node)
         return cls(**kwargs)
 
     def run(
         self,
@@ -332,15 +345,15 @@
             return handle_full_split(chosen_args["dataframe"], groups, part_of_table, id_column)
 
         return groups
 
 
 def load_from_config(yaml_config: str, loader: type = yaml.Loader) -> Splitter:
     """
-    Creates Splitter class instance from yaml config.
+    Restore a ``Splitter`` class instance from a yaml config.
 
     For yaml_config parameter you can pass file name with
     config, which must ends with .yaml, for example: "config.yaml".
     For loader you can choose SafeLoader.
     """
     if isinstance(yaml_config, str) and yaml_config.endswith(".yaml"):
         with open(yaml_config, "r", encoding="utf-8") as file:
@@ -359,15 +372,17 @@
     strat_columns: Optional[types.ColumnNamesType] = None,
     salt: Optional[str] = None,
     fit_columns: Optional[types.ColumnNamesType] = None,
     threads: int = 1,
     **kwargs,
 ) -> types.SplitterResult:
     """
-    Standalone function used to create splitted groups from the dataframe.
+    Function wrapper around the ``Splitter`` class.
+
+    Used to create splitted groups from the dataframe.
 
     Creates an instance of the ``Splitter`` class internally and execute
     run method with corresponding arguments.
 
     Parameters
     ----------
     method : str
```

### Comparing `ambrosia-0.3.0/ambrosia/tester/__init__.py` & `ambrosia-0.4.0/ambrosia/tester/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tester/binary_result_evaluation.py` & `ambrosia-0.4.0/ambrosia/tester/binary_result_evaluation.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tester/tester.py` & `ambrosia-0.4.0/ambrosia/tester/tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,29 +38,30 @@
 import ambrosia.tools.empirical_tools as empirical_pkg
 import ambrosia.tools.pvalue_tools as pvalue_pkg
 import ambrosia.tools.stat_criteria as criteria_pkg
 from ambrosia import types
 from ambrosia.tools.ab_abstract_component import ABStatCriterion, ABToolAbstract, DataframeHandler, StatCriterion
 
 from .binary_result_evaluation import binary_absolute_result, binary_relative_result
+from .handlers import TheoreticalTesterHandler, filter_spark_and_make_groups
 
-BOOTSTRAP_SIZE: int = 1000
+BOOTSTRAP_SIZE: int = 10000
 AVAILABLE: List[str] = ["pandas", "spark"]
 AVAILABLE_AB_CRITERIA: Dict[str, ABStatCriterion] = {
     "ttest": criteria_pkg.TtestIndCriterion,
     "ttest_rel": criteria_pkg.TtestRelCriterion,
     "mw": criteria_pkg.MannWhitneyCriterion,
     "wilcoxon": criteria_pkg.WilcoxonCriterion,
 }
 AVAILABLE_MULTITEST_CORRECTIONS: List[str] = ["bonferroni"]
 
 
 class Tester(ABToolAbstract):
     """
-    Unit for experimental data test and evaluation.
+    Unit for evaluating the results of experiments.
 
     The experiment evaluation result contains:
         - Pvalue for the selected criterion
         - Point effect estimation
         - Corresponding confidence interval for the effect
         - Boolean result - presence / absence of the effect
 
@@ -77,15 +78,15 @@
     column_groups : ColumnNameType, optional
         Column which contains groups label of objects.
     group_labels : GroupLabelsType, optional
         Labels for experimental groups. If ``column_groups`` contains
         at least two values, they will choose for labels.
     id_column : ColumnNameType, optional
         Name of column with objects ids in ``df_mapping`` dataframe.
-    first_errors : StatErrorType, default: ``0.05``
+    first_type_errors : StatErrorType, default: ``0.05``
         I type errors values. Fix P (detect difference for equal) to be less
         than threshold. Used to construct confidence intervals.
     metrics : MetricNameType, optional
         Metrics (columns of dataframe) which is used to calculate
         experiment result.
 
     Attributes
@@ -98,15 +99,15 @@
         Dict with separate experiment results for each group.
     column_groups : ColumnNameType
         Column which contains groups label of objects.
     group_labels : GroupLabelsType
         Labels for experimental groups.
     id_column : ColumnNameType
         Name of column with objects ids in ``df_mapping`` dataframe.
-    first_errors : StatErrorType, default: ``0.05``
+    first_type_errors : StatErrorType, default: ``0.05``
         I type errors values.
     metrics : MetricNameType
         Columns of dataframe with experiment results.
 
     Examples
     --------
     We've experimented with adding onboarding to our mobile app and
@@ -154,15 +155,15 @@
     >>> tester = Tester()
     >>> # You can pass Iterable or single object for some parameters
     >>> tester = Tester(
     >>>     dataframe=df,
     >>>     columns_groups='groups',
     >>>     metrics=['ltv', 'retention']
     >>> )
-    >>> tester = Tester(metrics='retention', first_errors=[0.01, 0.05])
+    >>> tester = Tester(metrics='retention', first_type_errors=[0.01, 0.05])
     >>> # You can set a separate table containing information about
     >>> # the partitioning in the experiment
     >>> tester = tester = Tester(
     >>>     dataframe=df, # main dataframe with metrics
     >>>     df_mapping=groups, # table with information about groups
     >>>     metrics='metric', # Metric to be tested
     >>>     column_groups='group', # Column in df_mapping with labels
@@ -193,19 +194,19 @@
 
     # This is for avoiding warnings from pytest
     __test__ = False
 
     def set_experiment_results(self, experiment_results: types.ExperimentResults) -> None:
         self.__experiment_results = experiment_results
 
-    def set_errors(self, first_errors: types.StatErrorType) -> None:
-        if isinstance(first_errors, float):
-            self.__alpha = np.array([first_errors])
+    def set_errors(self, first_type_errors: types.StatErrorType) -> None:
+        if isinstance(first_type_errors, float):
+            self.__alpha = np.array([first_type_errors])
         else:
-            self.__alpha = np.array(first_errors)
+            self.__alpha = np.array(first_type_errors)
 
     def set_metrics(self, metrics: types.MetricNamesType) -> None:
         if isinstance(metrics, types.MetricNameType):
             self.__metrics = [metrics]
         else:
             self.__metrics = metrics
 
@@ -221,26 +222,28 @@
             "dataframe": dataframe,
             "df_mapping": df_mapping,
             "column_groups": column_groups,
             "group_labels": group_labels,
             "id_column": id_column,
         }
         self.__experiment_results = DataframeHandler()._handle_cases(
-            Tester.__filter_data, Tester.__filter_spark_data, **__filtering_kwargs
+            Tester.__filter_data,
+            filter_spark_and_make_groups,
+            **__filtering_kwargs,
         )
 
     def __init__(
         self,
         dataframe: Optional[types.PassedDataType] = None,
         df_mapping: Optional[types.GroupsInfoType] = None,
         experiment_results: Optional[types.ExperimentResults] = None,
         column_groups: Optional[types.ColumnNameType] = None,
         group_labels: Optional[types.GroupLabelsType] = None,
         id_column: Optional[types.ColumnNameType] = None,
-        first_errors: types.StatErrorType = 0.05,
+        first_type_errors: types.StatErrorType = 0.05,
         metrics: Optional[types.MetricNamesType] = None,
     ):
         """
         Tester class constructor to initialize the object.
         """
         if dataframe is not None:
             self.set_dataframe(
@@ -248,15 +251,15 @@
                 column_groups,
                 group_labels,
                 df_mapping,
                 id_column,
             )
         else:
             self.set_experiment_results(experiment_results=experiment_results)
-        self.set_errors(first_errors)
+        self.set_errors(first_type_errors)
         self.set_metrics(metrics)
 
     @staticmethod
     def __filter_data(
         dataframe: types.PassedDataType,
         df_mapping: types.GroupsInfoType,
         column_groups: types.ColumnNameType,
@@ -284,19 +287,14 @@
         else:
             group_labels = dataframe[column_groups].unique()
         experiment_results: types.ExperimentResults = {
             group_label: dataframe[dataframe[column_groups] == group_label] for group_label in group_labels
         }
         return experiment_results
 
-    def __filter_spark_data(self):
-        """
-        Function to handle setting of Spark data.
-        """
-
     @staticmethod
     def __bootstrap_result(
         group_a: types.GroupType,
         group_b: types.GroupType,
         alpha: np.ndarray,
         bootstrap_size: int = BOOTSTRAP_SIZE,
         effect_type: str = "absolute",
@@ -309,16 +307,17 @@
             metric = "mean"
             point_effect = np.mean(group_b) - np.mean(group_a)
         elif effect_type == "relative":
             metric = "fraction"
             point_effect = np.mean(group_b) / np.mean(group_a) - 1
         else:
             raise ValueError("Set effect_type as 'absolute' or 'relative'")
-        bootstrap_handler = empirical_pkg.BootstrapStats(bootstrap_size=bootstrap_size, metric=metric)
-        bootstrap_handler.fit(group_a, group_b)
+        paired: bool = kwargs.pop("paired") if "paired" in kwargs else False
+        bootstrap_handler = empirical_pkg.BootstrapStats(bootstrap_size=bootstrap_size, metric=metric, paired=paired)
+        bootstrap_handler.fit(group_a, group_b, **kwargs)
         left_bounds, right_bounds = bootstrap_handler.confidence_interval(confidence_level=1 - alpha, **kwargs)
         pvalue = bootstrap_handler.pvalue_criterion(**kwargs)
         confidence_interval = list(zip(left_bounds, right_bounds))
         return {
             "first_type_error": alpha,
             "pvalue": pvalue,
             "effect": point_effect,
@@ -351,80 +350,81 @@
         criterion: Optional[ABStatCriterion] = None,
         **kwargs,
     ) -> types._SubResultType:
         """
         Function to handle the theoretical approach to testing.
         """
         criterion: Union[str, StatCriterion] = criterion if criterion is not None else "ttest"
-        if isinstance(criterion, str) & (criterion in AVAILABLE_AB_CRITERIA):
+        if isinstance(criterion, str) and (criterion in AVAILABLE_AB_CRITERIA):
             criterion = AVAILABLE_AB_CRITERIA[criterion]
         elif not (hasattr(criterion, "get_results") and callable(criterion.get_results)):
             raise ValueError(
                 f"Choose correct criterion name from {list(AVAILABLE_AB_CRITERIA)} or pass correct custom class"
             )
         return criterion().get_results(group_a=group_a, group_b=group_b, alpha=alpha, effect_type=effect_type, **kwargs)
 
     @staticmethod
     def __pre_run(method: str, args: types._UsageArgumentsType, **kwargs) -> types.TesterResult:
         """
         Function to handle run method on pandas dataframes.
         """
+        # TODO: add methods to enum
         accepted_methods: List[str] = ["theory", "empiric", "binary"]
         if method not in accepted_methods:
             raise ValueError(f'Choose method from {", ".join(accepted_methods)}')
         result: types.TesterResult = {}
         for metric in args["metrics"]:
             a_values: np.ndarray = args["data_a_group"][metric].values
             b_values: np.ndarray = args["data_b_group"][metric].values
             if method == "theory":
-                sub_result = Tester.__theory_handler(
-                    a_values,
-                    b_values,
-                    np.array(args["alpha"]),
+                # TODO: Make it SolverClass ~ method
+                # solver = SolverClass(...)
+                # sub_result = solver.solve()
+                solver = TheoreticalTesterHandler(
+                    args["data_a_group"],
+                    args["data_b_group"],
+                    column=metric,
+                    alpha=np.array(args["alpha"]),
                     effect_type=args["effect_type"],
                     criterion=args["criterion"],
                     **kwargs,
                 )
+                sub_result = solver.solve()
             elif method == "empiric":
                 sub_result = Tester.__bootstrap_result(
                     a_values, b_values, np.array(args["alpha"]), effect_type=args["effect_type"], **kwargs
                 )
             elif method == "binary":
                 sub_result = Tester.__binary_result(
                     a_values, b_values, np.array(args["alpha"]), effect_type=args["effect_type"], **kwargs
                 )
             result[metric] = sub_result
         return result
 
     @staticmethod
-    def __pre_run_spark():
-        """
-        Function to handle run method on Spark dataframes.
-        """
-
-    @staticmethod
     def __apply_first_stage_multitest_correction(
         alphas: types.StatErrorType, hypothesis_num: int, method: str = "bonferroni"
     ) -> types.StatErrorType:
         """
         Apply first stage of multitest correction for first type errors.
         """
+        alphas = alphas.copy()
         if method == "bonferroni":
             alphas /= hypothesis_num
         return alphas
 
     @staticmethod
     def __apply_second_stage_multitest_correction(
         result: types.TesterResult, hypothesis_num: int, method: str = "bonferroni"
     ):
         """
         Apply second stage of multitest correction.
         """
         if method == "bonferroni":
-            result["pvalue"] *= hypothesis_num
+            result["pvalue"] = (result["pvalue"].values * hypothesis_num).clip(max=1)
             result["first_type_error"] *= hypothesis_num
         return result
 
     @staticmethod
     def as_table(dict_result: types.TesterResult) -> pd.DataFrame:
         """
         Transform dict type output result to pandas DataFrame format.
@@ -465,15 +465,15 @@
         dataframe: Optional[types.PassedDataType] = None,
         df_mapping: Optional[types.GroupsInfoType] = None,
         experiment_results: Optional[types.ExperimentResults] = None,
         id_column: Optional[str] = None,
         column_groups: Optional[str] = None,
         group_labels: Optional[types.GroupLabelsType] = None,
         metrics: Optional[types.MetricNamesType] = None,
-        first_errors: Optional[types.StatErrorType] = None,
+        first_type_errors: Optional[types.StatErrorType] = None,
         criterion: Optional[ABStatCriterion] = None,
         correction_method: Union[str, None] = "bonferroni",
         as_table: bool = True,
         **kwargs,
     ) -> types.TesterResult:
         """
         The main method for testing and evaluating experimental results.
@@ -496,93 +496,96 @@
             pandas or Spark dataframes.
         column_groups : ColumnNameType
             Column which contains groups label of objects.
         group_labels : GroupLabelsType
             Labels for experimental groups.
         id_column : ColumnNameType
             Name of column with objects ids in ``df_mapping`` dataframe.
-        first_errors : StatErrorType, default: ``0.05``
+        first_type_errors : StatErrorType, default: ``0.05``
             I type errors values.
         metrics : MetricNameType
             Columns of dataframe with experiment results.
         criterion : ABStatCriterion, optional
             Statistical criterion for hypotheses testing.
             If ``method`` is ``"theory"`` and no criterion provided,
             ttest for independent samples will be used.
         correction_method : Union[str, None], default: ``bonferroni``
             Method for pvalues and confidence intervals multitest correction.
+            Total number of hypothesis is equal to the number of
+            variants combinations * number of metrics passed.
         as_table : bool, default: ``True``
             Return the test results as a pandas dataframe.
             If ``False``, a list of dicts with results will be returned.
         **kwargs : Dict
             Other keyword arguments.
 
         Returns
         -------
         result : types.TesterResult
             Experiment results as pandas table or list of dicts for each metric
             and first type error.
         """
         if isinstance(metrics, types.MetricNameType):
             metrics = [metrics]
-        if isinstance(first_errors, float):
-            first_errors = [first_errors]
+        if first_type_errors is not None:
+            if isinstance(first_type_errors, float):
+                first_type_errors = np.array([first_type_errors])
+            else:
+                first_type_errors = np.array(first_type_errors)
         if "alternative" in kwargs:
             pvalue_pkg.check_alternative(kwargs["alternative"])
+        else:
+            kwargs["alternative"] = "two-sided"
 
         __filtering_kwargs = {
             "dataframe": dataframe,
             "df_mapping": df_mapping,
             "column_groups": column_groups,
             "group_labels": group_labels,
             "id_column": id_column,
         }
         if dataframe is not None:
             experiment_results = DataframeHandler()._handle_cases(
-                Tester.__filter_data, Tester.__filter_spark_data, **__filtering_kwargs
+                Tester.__filter_data, filter_spark_and_make_groups, **__filtering_kwargs
             )
 
         arguments_choice: types._PrepareArgumentsType = {
             "experiment_results": (self.__experiment_results, experiment_results),
             "metrics": (self.__metrics, metrics),
-            "alpha": (self.__alpha, first_errors),
+            "alpha": (self.__alpha, first_type_errors),
         }
         chosen_args: types._UsageArgumentsType = Tester._prepare_arguments(arguments_choice)
         chosen_args["effect_type"] = effect_type
         chosen_args["criterion"] = criterion
 
-        hypothesis_num: int = len(list(itertools.combinations(chosen_args["experiment_results"], 2)))
-        correction_available: Optional[bool] = None
-        if hypothesis_num > 1:
+        hypothesis_num: int = len(list(itertools.combinations(chosen_args["experiment_results"], 2))) * len(
+            chosen_args["metrics"]
+        )
+        if correction_method is not None and hypothesis_num > 1:
             if correction_method in AVAILABLE_MULTITEST_CORRECTIONS:
-                correction_available = True
+                chosen_args["alpha"] = Tester.__apply_first_stage_multitest_correction(
+                    chosen_args["alpha"], hypothesis_num, correction_method
+                )
             else:
                 raise ValueError(f"Choose correction method from {AVAILABLE_MULTITEST_CORRECTIONS}")
 
-        if correction_available:
-            chosen_args["alpha"] = Tester.__apply_first_stage_multitest_correction(
-                chosen_args["alpha"], hypothesis_num, correction_method
-            )
-
         result: types.TesterResult = {}
         # Variating over all pairs of groups - comb(n, 2)
         for group_a_label, group_b_label in itertools.combinations(chosen_args["experiment_results"], 2):
             test_name = f"group_{group_a_label}_vs_group_{group_b_label}"
             chosen_args["data_a_group"] = chosen_args["experiment_results"][group_a_label]
             chosen_args["data_b_group"] = chosen_args["experiment_results"][group_b_label]
             pre_run_args = (method, chosen_args)
-            subresult: types.TesterResult = DataframeHandler()._handle_on_table(
-                Tester.__pre_run, Tester.__pre_run_spark, chosen_args["data_a_group"], *pre_run_args, **kwargs
-            )
+            subresult: types.TesterResult = Tester.__pre_run(*pre_run_args, **kwargs)
             subresult["group_a_label"] = group_a_label
             subresult["group_b_label"] = group_b_label
             result[test_name] = subresult
 
         result = Tester.as_table(result)
-        if correction_available:
+        if correction_method is not None and hypothesis_num > 1:
             result = Tester.__apply_second_stage_multitest_correction(result, hypothesis_num, correction_method)
         if not as_table:
             result = result.to_dict(orient="records")
         return result
 
 
 def test(
@@ -591,22 +594,24 @@
     dataframe: Optional[types.PassedDataType] = None,
     df_mapping: Optional[types.GroupsInfoType] = None,
     experiment_results: Optional[types.ExperimentResults] = None,
     id_column: Optional[str] = None,
     column_groups: Optional[str] = None,
     group_labels: Optional[types.GroupLabelsType] = None,
     metrics: Optional[types.MetricNamesType] = None,
-    first_errors: Optional[types.StatErrorType] = None,
+    first_type_errors: Optional[types.StatErrorType] = None,
     criterion: Optional[ABStatCriterion] = None,
     correction_method: Union[str, None] = "bonferroni",
     as_table: bool = True,
     **kwargs,
 ) -> types.TesterResult:
     """
-    Standalone function used to get the results of an experiment.
+    Function wrapper around the ``Tester`` class.
+
+    Apply on the experimental data to get the results of an experiment.
 
     Creates an instance of the ``Tester`` class internally and execute
     run method with corresponding arguments.
 
     Parameters
     ----------
     effect_type : str, default: ``"absolute"``
@@ -625,24 +630,26 @@
         pandas or Spark dataframes.
     column_groups : ColumnNameType
         Column which contains groups label of objects.
     group_labels : GroupLabelsType
         Labels for experimental groups.
     id_column : ColumnNameType
         Name of column with objects ids in ``df_mapping`` dataframe.
-    first_errors : StatErrorType, default: ``0.05``
+    first_type_errors : StatErrorType, default: ``0.05``
         I type errors values.
     metrics : MetricNameType
         Columns of dataframe with experiment results.
     criterion : ABStatCriterion, optional
         Statistical criterion for hypotheses testing.
         If ``method`` is ``"theory"`` and no criterion provided,
         ttest for independent samples will be used.
     correction_method : Union[str, None], default: ``bonferroni``
         Method for pvalues and confidence intervals multitest correction.
+        Total number of hypothesis is equal to the number of
+        variants combinations * number of metrics passed.
     as_table : bool, default: ``True``
         Return the test results as a pandas dataframe.
         If ``False``, a list of dicts with results will be returned.
     **kwargs : Dict
         Other keyword arguments.
 
     Returns
@@ -654,15 +661,15 @@
     return Tester(
         dataframe=dataframe,
         df_mapping=df_mapping,
         id_column=id_column,
         column_groups=column_groups,
         group_labels=group_labels,
         metrics=metrics,
-        first_errors=first_errors,
+        first_type_errors=first_type_errors,
     ).run(
         effect_type=effect_type,
         method=method,
         experiment_results=experiment_results,
         criterion=criterion,
         correction_method=correction_method,
         as_table=as_table,
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/__init__.py` & `ambrosia-0.4.0/ambrosia/tools/_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tools/_lib/_bin_ci_aide.py` & `ambrosia-0.4.0/ambrosia/tools/_lib/_bin_ci_aide.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tools/_lib/_bootstrap_tools.py` & `ambrosia-0.4.0/ambrosia/tools/_lib/_bootstrap_tools.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tools/_lib/_selection_aide.py` & `ambrosia-0.4.0/ambrosia/tools/_lib/_selection_aide.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tools/_lib/_tools_aide.py` & `ambrosia-0.4.0/ambrosia/tools/_lib/_tools_aide.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from typing import Callable, List, Optional, Sequence
 
 import numpy as np
 import pandas as pd
 
-import ambrosia.tools as tools_pkg
+import ambrosia.tools.empirical_tools as emp_pkg
 from ambrosia import types
 
 EPSILON: float = 0.001
 
 
 def __helper_generate_bootstrap_samples(
     dataframe: pd.DataFrame, metrics: List[str], total_size: int, bootstrap_size: int, random_seed: Optional[int] = None
@@ -48,15 +48,15 @@
     random_seed: Optional[int] = None,
 ) -> types.BootstrapedSamplesType:
     """
     Help to inject effect after sampling groups A/B.
     """
     modified_samples_values: types.BootstrapedSamplesType = {}
     for metric, sampled_metric in sampled_metrics.items():
-        modified_samples_values[metric] = tools_pkg.empirical_tools.inject_effect(
+        modified_samples_values[metric] = emp_pkg.inject_effect(
             sampled_metric,
             sample_size_a=sample_size_a,
             effect=effect,
             modeling_method=injection_method,
             variation_factor=variation_factor,
             random_seed=random_seed,
         )
@@ -64,64 +64,69 @@
 
 
 def __helper_get_power_for_bootstraped(
     modified_samples: types.BootstrapedSamplesType,
     sample_size: int,
     bound_size: int,
     alpha: float,
+    groups_ratio: float = 1.0,
     criterion: str = "ttest",
     random_seed: Optional[int] = None,
-    use_tqdm: bool = False,
-    parallel: bool = False,
+    n_jobs: int = 1,
     verbose: bool = False,
+    **kwargs,
 ) -> List[float]:
     """
     Calculate power for bootstraped samples.
     """
-    result_power = [None]
+    result_power = []
     for _, values in modified_samples.items():
-        power = 1 - tools_pkg.tools.eval_error(
-            np.vstack([values[:sample_size], values[bound_size : bound_size + sample_size]]),
+        sampled_metric_vals = np.vstack(
+            [values[:sample_size], values[bound_size : bound_size + int(groups_ratio * sample_size)]]
+        )
+        power = emp_pkg.eval_error(
+            sampled_metric_vals,
             sample_size_a=sample_size,
             alpha=alpha,
             mode=criterion,
             random_seed=random_seed,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
+            n_jobs=n_jobs,
             verbose=verbose,
+            **kwargs,
         )
         result_power.append(power)
     return result_power
 
 
 def estimate_power(power_function: Callable, **kwargs_power) -> float:
     """
     Helps calc power with cases with cases with multioutput.
     """
     power_estimation = power_function(**kwargs_power)
-    # Power function can return [correctness, power]
     if isinstance(power_estimation, Sequence):
-        power_estimation = power_estimation[1]
+        power_estimation = power_estimation[0]
     return power_estimation
 
 
 def helper_bin_search_upper_bound_size(
     power_function: Callable,
     power_level: float,
     groups_sizes_names: List[str],
+    groups_ratio: float = 1.0,
     **kwargs_power,
 ) -> int:
     """
     Binary search for upper bound group size.
     """
     upper_bound_degree: int = 4
     power_estimation: float = 0
     while power_estimation < power_level:
         for gr_name in groups_sizes_names:
             kwargs_power[gr_name] = 2**upper_bound_degree
+        kwargs_power[groups_sizes_names[-1]] = int(groups_ratio * kwargs_power[groups_sizes_names[-1]])
         power_estimation: float = estimate_power(power_function, **kwargs_power)
         upper_bound_degree += 1
     return upper_bound_degree
 
 
 def helper_bin_searh_upper_bound_effect(power_function: Callable, power_level: float, **kwargs_power) -> int:
     """
@@ -155,15 +160,15 @@
         modified_samples = __helper_inject_effect(
             bootstraped_samples,
             sample_size_a=kwargs_power["sample_size"],
             effect=middle,
             injection_method=injection_method,
             random_seed=kwargs_power["random_seed"],
         )
-        power_estimation: float = power_function(**kwargs_power, modified_samples=modified_samples)[1]
+        power_estimation: float = power_function(**kwargs_power, modified_samples=modified_samples)[0]
         if power_estimation >= power_level:
             right = middle
         else:
             left = middle
     return right
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/ab_abstract_component.py` & `ambrosia-0.4.0/ambrosia/tools/ab_abstract_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from yaml import YAMLObjectMetaclass
 
+import ambrosia.tools.pvalue_tools as pvalue_pkg
 from ambrosia import types
 from ambrosia.tools import log
 
 AVAILABLE: List[str] = ["pandas", "spark"]
 DATA: str = "dataframe"
 
 
@@ -221,42 +222,45 @@
         Verbose method for transform operation Log.
         """
         part_of_variance: float = new_variance / (old_variance + AbstractVarianceReducer.EPSILON)
         log.info_log(f"After transformation {self}, the variance is {(part_of_variance * 100):.4f} % of the original")
         log.info_log(f"Variance transformation {old_variance:.4f} ===> {new_variance:.4f}")
 
 
+def choose_on_table(alternatives: List[Any], dataframe) -> Any:
+    """
+    alternatives: [alternative_pandas, alternative_spark, ...]
+    """
+    if isinstance(dataframe, pd.DataFrame):
+        return alternatives[0]
+    elif isinstance(dataframe, types.SparkDataFrame):
+        return alternatives[1]
+    raise TypeError(f'Type of table must be one of {", ".join(AVAILABLE)}')
+
+
 class DataframeHandler:
     @staticmethod
     def _handle_cases(__func_pandas: Callable, __func_spark: Callable, *args, **kwargs):
         """
         Helps handle cases with different types of dataframe in kwargs,
         available types - pandas, spark.
         """
-        if isinstance(kwargs[DATA], pd.DataFrame):
-            return __func_pandas(*args, **kwargs)
-        elif isinstance(kwargs[DATA], types.SparkDataFrame):
-            return __func_spark(*args, **kwargs)
-        else:
-            raise TypeError(f'Type of table must be one of {", ".join(AVAILABLE)}')
+        __func = choose_on_table([__func_pandas, __func_spark], kwargs[DATA])
+        return __func(*args, **kwargs)
 
     @staticmethod
     def _handle_on_table(
         __func_pandas: Callable, __func_spark: Callable, variable: types.SparkOrPandas, *args, **kwargs
     ):
         """
         Helps handle cases with different types of dataframe as additional variable,
         available types - pandas, spark.
         """
-        if isinstance(variable, pd.DataFrame):
-            return __func_pandas(*args, **kwargs)
-        elif isinstance(variable, types.SparkDataFrame):
-            return __func_spark(*args, **kwargs)
-        else:
-            raise TypeError(f'Type of table must be one of {", ".join(AVAILABLE)}')
+        __func = choose_on_table([__func_pandas, __func_spark], variable)
+        return __func(*args, **kwargs)
 
 
 class SimpleDesigner(ABC, DataframeHandler):
     """
     Simple designer is the interface for designers for each dataframe and method.
 
     kwargs must contain parameter dataframe.
@@ -391,21 +395,28 @@
 
     @abstractmethod
     def calculate_conf_interval(
         self, group_a: Iterable[float], group_b: Iterable[float], alpha: types.StatErrorType, effect_type: str, **kwargs
     ) -> List[Tuple]:
         pass
 
+    def _make_ci(self, left_ci: np.ndarray, right_ci: np.ndarray, alternative: str) -> List:
+        left_ci, right_ci = pvalue_pkg.choose_from_bounds(left_ci, right_ci, alternative)
+        conf_intervals = list(zip(left_ci, right_ci))
+        return conf_intervals
+
     def get_results(
         self,
         group_a: np.ndarray,
         group_b: np.ndarray,
         alpha: types.StatErrorType = 0.05,
         effect_type: str = "absolute",
         **kwargs,
     ) -> types.StatCriterionResult:
         return {
             "first_type_error": alpha,
-            "pvalue": self.calculate_pvalue(group_a, group_b, **kwargs),
-            "effect": self.calculate_effect(group_a, group_b, effect_type),
-            "confidence_interval": self.calculate_conf_interval(group_a, group_b, alpha, effect_type, **kwargs),
+            "pvalue": self.calculate_pvalue(group_a, group_b, effect_type=effect_type, **kwargs),
+            "effect": self.calculate_effect(group_a, group_b, effect_type=effect_type),
+            "confidence_interval": self.calculate_conf_interval(
+                group_a, group_b, alpha=alpha, effect_type=effect_type, **kwargs
+            ),
         }
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/bin_intervals.py` & `ambrosia-0.4.0/ambrosia/tools/bin_intervals.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 import pandas as pd
 import scipy.stats as sps
 
 import ambrosia.tools._lib._bin_ci_aide as helper_dir
 import ambrosia.tools.pvalue_tools as pvalue_pkg
 from ambrosia import types
 
+from . import EFFECT_COL_NAME, FIRST_TYPE_ERROR_COL_NAME, GROUP_SIZE_COL_NAME, STAT_ERRORS_COL_NAME
+
 RELATIVE_ABSOLUTE_DELTA_ERROR = ValueError("Choose relative or absolute delta, not both")
 ROUND_DIGITS: int = 3
+ROUND_DIGITS_TABLE: int = 3
+ROUND_DIGITS_PERCENT: int = 1
 
 
 class BinomTwoSampleCI(ABC):
     """
     Implementation of two-sample confidence interval.
     Supported the following types  interval_type:
 
@@ -450,63 +454,66 @@
     sample_sizes: Iterable[int],
     first_errors: Iterable[float] = (0.05,),
     delta_values: Iterable[float] = None,
     delta_relative_values: Iterable[float] = None,
     interval_type: str = "wald",
     # alternative: str = "two-sided",
     amount: int = 10000,
+    as_numeric: bool = False,
 ) -> pd.DataFrame:
     """
     Table with power / empirical 1 type error = 1 - coverage for fixed size and effect.
 
     Parameters
     ----------
     p_a : Iterable[float]
         Conversion in A group
     sample_sizes : Iterable[float]
         Sizes for samples
     first_errors : Iterable[float], default : ``(0.05,)``
         First type error values
     delta_values : Iterable[float]
-        Absolute delta values: p_a - p_b = delta
+        Absolute delta values: p_b - p_a = delta
     delta_relative_values : Iterable[float]
-        Relative delta values: delta_relative * p_a = p_b
+        Relative delta values: p_b = delta_relative * p_a
     interval_type : str
         interval_type for confidence interval
     alternative : str, default : ``"two-sided"``
         Alternative for static criteria - two-sided, less, greater
         Less means, that mean in first group less, than mean in second group
     amount : int, default : ``10000``
         Amount of generated samples for one n(trials amount), to estimate power
+    as_numeric : bool, default: ``False``
+        The result of calculations can be obtained as a percentage string
+        either as a number, this parameter could used to toggle.
+        Works only for relative values of power.
 
     Returns
     -------
     table : pd.DataFrame
         Required table with power
     """
     trials = np.array(sample_sizes)
     if not (delta_values is None) ^ (delta_relative_values is None):
         raise RELATIVE_ABSOLUTE_DELTA_ERROR
     if delta_values is not None:
-        p_b_values: np.ndarray = p_a - np.array(delta_values)
+        p_b_values: np.ndarray = p_a + np.array(delta_values)
         grid_delta: np.ndarray = delta_values
-        delta_name: str = r"$\Delta$-absolute"
     else:
         p_b_values: np.ndarray = p_a * np.array(delta_relative_values)
-        grid_delta: np.ndarray = delta_relative_values
-        delta_name: str = r"$\delta$-relative"
+        grid_delta: np.ndarray = [f"{np.round((x - 1) * 100, ROUND_DIGITS_PERCENT)}%" for x in delta_relative_values]
     if not np.all((p_b_values >= 0) & (p_b_values <= 1)):
         raise ValueError(f"Probability of success in group B must be positive, not {p_b_values}")
 
     values = [(round(a, ROUND_DIGITS), b) for a in first_errors for b in grid_delta]
     table: pd.DataFrame = pd.DataFrame(
-        index=pd.MultiIndex.from_tuples(values, names=[r"$\alpha$", delta_name]),
+        index=pd.MultiIndex.from_tuples(values, names=[FIRST_TYPE_ERROR_COL_NAME, EFFECT_COL_NAME]),
         columns=trials,
     )
-    table.columns.name = "sample sizes"
+    table.columns.name = GROUP_SIZE_COL_NAME
     sample_a = sps.binom.rvs(n=trials, p=p_a, size=(amount, trials.shape[0]))
     for alpha in first_errors:
         for p_b, delta in zip(p_b_values, grid_delta):
             sample_b = sps.binom.rvs(n=trials, p=p_b, size=(amount, trials.shape[0]))
             binom_kwargs = {
                 "interval_type": interval_type,
                 "a_success": sample_a,
@@ -514,19 +521,19 @@
                 "a_trials": trials,
                 "b_trials": trials,
                 "confidence_level": 1 - alpha,
                 #    "alternative": alternative,
             }
             conf_interval: types.ManyIntervalType = BinomTwoSampleCI.confidence_interval(**binom_kwargs)
             power: np.ndarray = helper_dir.__helper_calc_empirical_power(conf_interval)
-            table.loc[(alpha, delta), trials] = [str(round(power_val * 100, 1)) + "%" for power_val in power]
-    table_title: str = r"$1 - \beta$: power of criterion, " + (
-        r"$p_a-p_b=\Delta$" if delta_values else r"$p_a\delta=p_b$"
-    )
-    table = table.style.set_caption(table_title)
+            if as_numeric:
+                power = [round(power_val, ROUND_DIGITS_TABLE) for power_val in power]
+            else:
+                power = [str(round(power_val * 100, ROUND_DIGITS_PERCENT)) + "%" for power_val in power]
+            table.loc[(alpha, delta), trials] = power
     return table
 
 
 def iterate_for_sample_size(
     interval_type: str,
     first_errors: Iterable[float],
     second_errors: Iterable[float],
@@ -534,32 +541,38 @@
     p_b_values: Iterable[float],
     grid_delta: Iterable[float],
     amount: int,
 ) -> pd.DataFrame:
     """
     Iterate over params for different sample size
     """
-    values = [(round(a, ROUND_DIGITS), round(b, ROUND_DIGITS)) for a in first_errors for b in second_errors]
-    table: pd.DataFrame = pd.DataFrame(
-        index=pd.MultiIndex.from_tuples(values, names=[r"$\alpha$", r"$\beta$"]),
-        columns=grid_delta,
+    # values = [(round(a, ROUND_DIGITS), round(b, ROUND_DIGITS)) for a in first_errors for b in second_errors]
+    # table: pd.DataFrame = pd.DataFrame(
+    #     index=pd.MultiIndex.from_tuples(values, names=[r"$\alpha$", r"$\beta$"]),
+    #     columns=grid_delta,
+    # )
+    multiindex = pd.MultiIndex.from_tuples([(eff,) for eff in grid_delta], names=[EFFECT_COL_NAME])
+    multicols = pd.MultiIndex.from_tuples(
+        [(f"({alpha}; {beta})",) for alpha in first_errors for beta in second_errors],
+        names=[STAT_ERRORS_COL_NAME],
     )
+    table: pd.DataFrame = pd.DataFrame(index=multiindex, columns=multicols)
     for alpha in first_errors:
-        for second_error in second_errors:
-            power = 1 - second_error
+        for beta in second_errors:
+            power = 1 - beta
             for p_b, delta in zip(p_b_values, grid_delta):
                 trials = helper_dir.__helper_bin_search_for_size(
                     interval_type=interval_type,
                     confidence_level=1 - alpha,
                     p_a=p_a,
                     p_b=p_b,
                     amount=amount,
                     power=power,
                 )
-                table.loc[(alpha, second_error), delta] = trials
+                table.loc[delta, f"({alpha}; {beta})"] = trials
     return table
 
 
 def get_table_sample_size_on_effect(
     interval_type: str = "wald",
     first_errors: Iterable[float] = (0.05,),
     second_errors: Iterable[float] = (0.2,),
@@ -578,17 +591,17 @@
     first_errors : Iterable[float], default : ``(0.05,)``
         First type error values
     second_errors : Iterable[float], default : ``(0.2,)``
         Second type error values
     p_a : Iterable[float]
         Conversion in A group, default : ``0.5``
     delta_values : Iterable[float]
-        Absolute delta values: p_a - p_b = delta
+        Absolute delta values: p_b - p_a = delta
     delta_relative_values : Iterable[float]
-        Relative delta values: delta_relative * p_a = p_b
+        Relative delta values: p_b = delta_relative * p_a
     amount : int, default : ``1000``
         Amount of generated samples for one n(trials amount), to estimate power
 
     Returns
     -------
     table : pd.DataFrame
         Required table with sample sizes
@@ -604,71 +617,74 @@
         raise RELATIVE_ABSOLUTE_DELTA_ERROR
 
     # If delta type not set => set to absolute
     if delta_values is None and delta_relative_values is None:
         delta_values = [p_a / 2]
 
     if delta_values is not None:
-        p_b_values: np.ndarray = p_a - np.array(delta_values)
+        p_b_values: np.ndarray = p_a + np.array(delta_values)
+        grid_delta: np.ndarray = delta_values
     else:
         p_b_values: np.ndarray = p_a * np.array(delta_relative_values)
+        grid_delta: np.ndarray = [f"{np.round((x - 1) * 100, ROUND_DIGITS_PERCENT)}%" for x in delta_relative_values]
     if not np.all((p_b_values >= 0) & (p_b_values <= 1)):
         raise ValueError(f"Probability of success in group B must be positive, not {p_b_values}")
-
-    grid_delta: np.ndarray = delta_values if delta_values is not None else delta_relative_values
     table = iterate_for_sample_size(interval_type, first_errors, second_errors, p_a, p_b_values, grid_delta, amount)
-
-    table.columns.name = r"$\Delta$-absolute" if delta_values is not None else r"$\delta$-relative"
     return table
 
 
 def iterate_for_delta(
     interval_type: str,
     first_errors: Iterable[float],
     second_errors: Iterable[float],
     sample_sizes: Iterable[int],
     p_a: float,
     amount: int,
     delta_type: str,
+    as_numeric: bool = False,
 ) -> pd.DataFrame:
     """
-    Helps find effect for different params
+    Helps to find effect for different params.
     """
-    values = [(round(a, ROUND_DIGITS), round(b, ROUND_DIGITS)) for a in first_errors for b in second_errors]
-    table: pd.DataFrame = pd.DataFrame(
-        index=pd.MultiIndex.from_tuples(values, names=[r"$\alpha$", r"$\beta$"]),
-        columns=sample_sizes,
+    multiindex = pd.MultiIndex.from_tuples([(trials,) for trials in sample_sizes], names=[GROUP_SIZE_COL_NAME])
+    multicols = pd.MultiIndex.from_tuples(
+        [(f"({alpha}; {beta})",) for alpha in first_errors for beta in second_errors],
+        names=[STAT_ERRORS_COL_NAME],
     )
+    table: pd.DataFrame = pd.DataFrame(index=multiindex, columns=multicols)
     for alpha in first_errors:
-        for second_error in second_errors:
-            power = 1 - second_error
+        for beta in second_errors:
+            power = 1 - beta
             for trials in sample_sizes:
                 delta = helper_dir.__helper_bin_search_for_delta(
                     interval_type=interval_type,
                     confidence_level=1 - alpha,
                     p_a=p_a,
                     trials=trials,
                     amount=amount,
                     power=power,
                 )
                 if delta is not None and delta_type == "relative":
-                    delta = str(round(abs(delta) / p_a * 100, 2)) + "%"
-
-                table.loc[(alpha, second_error), trials] = delta
+                    if as_numeric:
+                        delta = round(abs(delta) / p_a, ROUND_DIGITS_TABLE) + 1
+                    else:
+                        delta = str(round(abs(delta) / p_a * 100, ROUND_DIGITS_PERCENT)) + "%"
+                table.loc[trials, f"({alpha}; {beta})"] = delta
     return table
 
 
 def get_table_effect_on_sample_size(
     interval_type: str = "wald",
     first_errors: Iterable[float] = (0.05,),
     second_errors: Iterable[float] = (0.2,),
     sample_sizes: Iterable[int] = (100,),
     p_a: float = 0.5,
     amount: int = 10000,
-    delta_type: str = "absolute",
+    delta_type: str = "relative",
+    as_numeric: bool = False,
 ) -> pd.DataFrame:
     """
     Table for effects with given sample sizes and erros.
     If there are no effects satisfy first and second errors value will be set to None
 
     Parameters
     ----------
@@ -681,15 +697,19 @@
     p_a : Iterable[float], default : ``0.5``
         Conversion in A group
     amount : int, default : ``10000``
         Amount of generated samples for one n(trials amount), to estimate power
     sample_sizes : Iterable[int], default : ``(100,)``
         Sample sizes for A/B group
     delta_type : str, default : ``"absolute``
-        absolute or relative, if relative give effect if percent: |delta| / p_a
+        absolute or relative, if relative gives effect in percents: |delta| / p_a
+    as_numeric : bool, default: ``False``
+        The result of calculations can be obtained as a percentage string
+        either as a number, this parameter could used to toggle.
+        Works only for relative values of effect.
 
     Returns
     -------
     table : pd.DataFrame
         Required table with effects
     """
     errors_condition = np.all((np.array(first_errors) >= 0) & (np.array(first_errors) <= 1)) and np.all(
@@ -698,19 +718,11 @@
     if not errors_condition:
         error_mesage_errors: str = "Errors must be from 0 to 1"
         raise ValueError(error_mesage_errors)
 
     delta_types: List[str] = ["absolute", "relative"]
     if delta_type not in delta_types:
         raise ValueError(f"Delta type must be absolute relative, not {delta_type}")
-
     table: pd.DataFrame = iterate_for_delta(
-        interval_type,
-        first_errors,
-        second_errors,
-        sample_sizes,
-        p_a,
-        amount,
-        delta_type,
+        interval_type, first_errors, second_errors, sample_sizes, p_a, amount, delta_type, as_numeric
     )
-    table.columns.name = "Sample size"
     return table
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/empirical_tools.py` & `ambrosia-0.4.0/ambrosia/tools/empirical_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,55 +8,34 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import Callable, Dict, Iterable, List, Optional, Union
+
+from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
-from joblib import Parallel, delayed
-from tqdm.auto import tqdm
+from joblib import Parallel, delayed, parallel_backend
 
 import ambrosia.tools.pvalue_tools as pvalue_pkg
 import ambrosia.tools.stat_criteria as criteria_pkg
 from ambrosia import types
 from ambrosia.tools.ab_abstract_component import ABStatCriterion
+from ambrosia.tools.decorators import filter_kwargs
 
 AVAILABLE_AB_CRITERIA: Dict[str, ABStatCriterion] = {
     "ttest": criteria_pkg.TtestIndCriterion,
     "ttest_rel": criteria_pkg.TtestRelCriterion,
     "mw": criteria_pkg.MannWhitneyCriterion,
     "wilcoxon": criteria_pkg.WilcoxonCriterion,
 }
 
 
-def create_seed_sequence(length: int, entropy: Optional[Union[int, Iterable[int]]] = None) -> np.ndarray:
-    """
-    Create a seed sequence using ``numpy.random.SeedSequence`` class.
-
-    Parameters
-    ----------
-    length : int
-        Total length of a sequence.
-    entropy : Union[int,Iterable[int]], optional
-        The entropy for creating a ``SeedSequence``.
-        Used to get a deterministic result.
-
-    Returns
-    -------
-    seed_sequence : List
-        The seed sequence of requested length.
-    """
-    rng = np.random.SeedSequence(entropy)
-    seed_sequence: np.ndarray = rng.generate_state(length)
-    return seed_sequence
-
-
 def inject_effect(
     sampled_metric_vals: np.ndarray,
     sample_size_a: int,
     effect: float,
     modeling_method: str = "constant",
     variation_factor: float = 10,
     random_seed: Optional[int] = None,
@@ -94,49 +73,52 @@
     mean: np.ndarray = modified_metric_vals[sample_size_a:, :].mean()
     bs_size: int = modified_metric_vals.shape[1]
     sample_size_b: int = len(modified_metric_vals) - sample_size_a
 
     if modeling_method == "constant":
         modified_metric_vals[sample_size_a:, :] = effect * modified_metric_vals[sample_size_a:, :]
     elif modeling_method == "shift":
-        modified_metric_vals[sample_size_a:, :] += (effect - 1) * mean
+        modified_metric_vals[sample_size_a:, :] = modified_metric_vals[sample_size_a:, :] + (effect - 1) * mean
     elif modeling_method == "normal":
         effect_delta = (effect - 1) * mean
         effect_std = modified_metric_vals[sample_size_a:, :].std(ddof=1) / variation_factor
         modified_metric_vals[sample_size_a:, :] = modified_metric_vals[sample_size_a:, :] + rng.normal(
             loc=effect_delta, scale=effect_std, size=(sample_size_b, bs_size)
         )
     else:
         raise ValueError(
             f"Effect modeling method {modeling_method} is not found, chose from {available_modeling_mehods}"
         )
     return modified_metric_vals
 
 
-def stat_criterion_power(
+def estim_stat_criterion_power(
     sampled_metric_vals: np.ndarray,
     sample_size_a: int,
     criterion: types.CompoundCriterionType = "ttest",
     alpha: float = 0.05,
+    **kwargs,
 ) -> float:
     """
-    Power of statistic criterion.
+    Estimate power of statistical criterion.
 
     Parameters
     ----------
     sampled_metric_vals : np.ndarray
         Sampled metrics for groups A/B
         |group A values|group B values|
     sample_size_a : int
         Size of group A
     criterion : Union[Callable[[np.ndarray, np.ndarray], CriterionResultType], str], default: ``"ttest"``
         Statistical criterion - function f: f(group A, group B) = (statistic, p_value)
         or name of criterion as string, for example 'ttest'
-    apha : float, default: ``0.05``
+    alpha : float, default: ``0.05``
         First type error bound, 1 - alpha: correctness
+    **kwargs : Dict
+        Keyword arguments for statistical criterion.
 
     Returns
     -------
     power : float
         Empirical bootstraped estimation for power
     """
     a_group_metrics: np.ndarray = sampled_metric_vals[:sample_size_a]
@@ -144,15 +126,15 @@
 
     if isinstance(criterion, str) & (criterion in AVAILABLE_AB_CRITERIA):
         criterion = AVAILABLE_AB_CRITERIA[criterion]
     elif not (hasattr(criterion, "calculate_pvalue") and callable(criterion.calculate_pvalue)):
         raise ValueError(
             f"Choose correct criterion name from {list(AVAILABLE_AB_CRITERIA)} or pass correct custom class"
         )
-    power: float = np.mean(criterion().calculate_pvalue(a_group_metrics, b_group_metrics) <= alpha)
+    power: float = np.mean(criterion().calculate_pvalue(a_group_metrics, b_group_metrics, **kwargs) <= alpha)
     return power
 
 
 def get_bs_stat(sample: np.ndarray, stat: str = "mean", N: int = 1000, random_seed: Optional[int] = None) -> np.ndarray:
     """
     Evaluate statistic (mean / median) using bootstrap method.
 
@@ -160,23 +142,25 @@
     ----------
     sample : np.ndarray
         Given sample array
     stat : str, default: ``"mean"``
         Name of statistic to be calculated
     N : int, default: ``1000``
        Bootstrap size
+    random_seed : int, optional
+        A seed for the deterministic outcome of random processes.
 
     Returns
     -------
     bs_stat : np.ndarray
-        Statistic calculated via booststrap
+        Statistic calculated via bootstrap
     """
     rng = np.random.default_rng(random_seed)
     permissible_string_statistics: List[str] = ["mean", "median"]
-    bs_samples: np.ndaray = rng.choice(sample, replace=True, size=(len(sample), N))
+    bs_samples: np.ndarray = rng.choice(sample, replace=True, size=(len(sample), N))
     if stat == "mean":
         bs_stat: np.ndarray = np.mean(bs_samples, axis=0)
     elif stat == "median":
         bs_stat: np.ndarray = np.median(bs_samples, axis=0)
     else:
         raise ValueError(f'Statistic is not found, choose from {", ".join(permissible_string_statistics)}')
     return bs_stat
@@ -185,59 +169,76 @@
 def get_bs_sample_stat(
     sample: np.ndarray,
     sample_size_a: int,
     alpha: float,
     N: int = 1000,
     stat: str = "mean",
     random_seed: Optional[int] = None,
+    alternative: str = "two-sided",
 ) -> bool:
     """
     Evaluate if difference in groups is significant.
-    If confidence interval contains 0 then effect is not significant else significant.
-    Return True if we have effect else False.
+
+    If confidence interval contains 0 then effect is not statistically significant.
+    Returns ``True`` if we have effect else ``False``.
 
     Parameters
     ----------
     sample : np.ndarray
         Sample with groups A and B
     sample_size_a : int
         Size of group A => sample = |group A| group B|
     alpha : float
         Bound for first type error
     N : int, default: ``1000``
        Bootstrap size
     stat : str, default: ``"mean"``
           Name of calculated statistic, for example 'mean'
+    random_seed : int, optional
+        A seed for the deterministic outcome of random processes.
+    alternative : str, default: ``"two-sided"``
+        Alternative hypothesis, can be ``"two-sided"``, ``"greater"``
+        or ``"less"``.
 
     Returns
     -------
     overlap : bool
         True => H_0 is rejected <-> there is effect in groups
         False => H_0 is not rejected <-> there is no effect in groups
     """
     rng = np.random.SeedSequence(random_seed)
     seed_sequence: np.ndarray = rng.generate_state(2)
     bs_stat_a = get_bs_stat(sample[:sample_size_a], stat=stat, N=N, random_seed=seed_sequence[0])
     bs_stat_b = get_bs_stat(sample[sample_size_a:], stat=stat, N=N, random_seed=seed_sequence[1])
-    bs_stat_diff = bs_stat_b - bs_stat_a
-    left_side, right_side = np.percentile(bs_stat_diff, [100 * alpha / 2.0, 100 * (1 - alpha / 2.0)])
-    overlap = not left_side <= 0 <= right_side
+    bs_stat_diff: np.ndarray = bs_stat_b - bs_stat_a
+    if alternative == "less":
+        right_side = np.quantile(bs_stat_diff, 1 - alpha)
+        overlap = right_side <= 0
+    elif alternative == "greater":
+        left_side = np.quantile(bs_stat_diff, alpha)
+        overlap = left_side >= 0
+    elif alternative == "two-sided":
+        left_side, right_side = np.quantile(bs_stat_diff, [alpha / 2.0, 1 - alpha / 2.0])
+        overlap = not left_side <= 0 <= right_side
+    else:
+        raise ValueError(f"Incorrect alternative value - {alternative}, choose from two-sided, less, greater")
     return overlap
 
 
 def make_bootstrap(
     sampled_metric_vals: np.ndarray,
     sample_size_a: int,
     alpha: float = 0.05,
     N: int = 1000,
     stat: str = "mean",
     random_seed: Optional[int] = None,
-    use_tqdm: bool = False,
-    parallel: bool = False,
+    n_jobs: int = 1,
+    backend: str = "loky",
     verbose: bool = False,
+    **kwargs,
 ) -> float:
     """
     Evaluate share of cases when we find difference in groups using bootstrap.
     We can use parallel mode for faster evaluations in case of large data.
 
     Parameters
     ----------
@@ -247,60 +248,116 @@
         Size of group A => |group A| group B|.
     alpha : float, default: ``0.05``
         Bound for the first type error.
     N : int, default: ``1000``
        Number of bootstraps.
     stat : str, default: ``"mean"``
         Statistics to be calculated.
-    use_tqdm : bool, default: ``False``
-        Whether to use tqdm bar progress.
-    parallel : bool, default: ``False``
-        Whether to use parallel calculations.
+    random_seed : int, optional
+        A seed for the deterministic outcome of random processes.
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
+    backend : str, default: ``"loky"``
+        Type of backend for joblib parallel computation.
     verbose : bool, default: ``False``
         Whether to make logging.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
     test_result : float
         Empirical estimation for power.
     """
     num_samples = sampled_metric_vals.shape[1]
     rng = np.random.SeedSequence(random_seed)
     seed_sequence: np.ndarray = rng.generate_state(num_samples)
     iterator = zip(range(num_samples), seed_sequence)
-    if parallel:
-        results_parallel = Parallel(n_jobs=64, verbose=verbose, backend="multiprocessing")(
+    with parallel_backend(backend=backend, n_jobs=n_jobs):
+        results_parallel = Parallel(verbose=verbose)(
             delayed(get_bs_sample_stat)(
                 sample=sampled_metric_vals[:, sample_num],
                 sample_size_a=sample_size_a,
                 alpha=alpha,
                 N=N,
                 stat=stat,
                 random_seed=seed,
+                **kwargs,
             )
             for sample_num, seed in iterator
         )
-        test_result = np.mean(results_parallel)
+    return np.mean(results_parallel)
+
+
+def eval_error(
+    sampled_metric_vals: np.ndarray,
+    sample_size_a: int,
+    alpha: float,
+    mode: str = "ttest",
+    stat: str = "mean",
+    bootstrap_size: int = 1000,
+    random_seed: Optional[int] = None,
+    n_jobs: int = 1,
+    verbose: bool = False,
+    **kwargs,
+) -> float:
+    """
+    Evaluate I type error/power of the experiment.
+
+    Parameters
+    ----------
+    sampled_metric_vals : np.ndarray
+        Samples of A/B groups: |group A values|group B values|.
+    sample_size_a : int
+        Size of  the group A in ``sampled_metric_vals``, i.e.
+        first ``sample_size_a`` elements correspond to the group A.
+    alpha : float
+        First type error bound, 1 - alpha: correctness.
+    mode : str, default: ``"ttest"``
+        Statistical criterion, for example ``'ttest'``.
+    stat : str, default: ``mean``
+        Statistic to be calculated for sample groups during a bootstrap.
+    bootstrap_size : int, default: ``1000``
+        Number of bootstrap of A/B pairs.
+    random_seed : int, optional
+        A seed for the deterministic outcome of random processes.
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
+    verbose : bool, default: ``False``
+        Whether use logging.
+    **kwargs : Dict
+        Keyword arguments for statistical criterion.
+
+    Returns
+    -------
+    error : float
+        Second type error estimation or correctness, i.e.
+        1 - P_{A=B} (criterion is completed) - correctness
+        P_{A!=B} (criterion is completed) - second type error.
+    """
+    not_bootstrap_criteria: List[str] = ["ttest", "ttest_rel", "mw", "wilcoxon"]
+    if mode in not_bootstrap_criteria:
+        power: float = estim_stat_criterion_power(
+            sampled_metric_vals, sample_size_a, criterion=mode, alpha=alpha, **kwargs
+        )
+    elif mode == "bootstrap":
+        power: float = make_bootstrap(
+            sampled_metric_vals,
+            sample_size_a,
+            alpha,
+            N=bootstrap_size,
+            stat=stat,
+            random_seed=random_seed,
+            n_jobs=n_jobs,
+            verbose=verbose,
+            **kwargs,
+        )
     else:
-        over_group_statistic = []
-        rng = range(num_samples)
-        if use_tqdm:
-            iterator = tqdm(iterator)
-        for sample_num, seed in iterator:
-            overlap = get_bs_sample_stat(
-                sample=sampled_metric_vals[:, sample_num],
-                sample_size_a=sample_size_a,
-                alpha=alpha,
-                N=N,
-                stat=stat,
-                random_seed=seed,
-            )
-            over_group_statistic.append(overlap)
-        test_result = np.mean(over_group_statistic)
-    return test_result
+        raise ValueError(f"Criterion {mode} is not found, choose from {not_bootstrap_criteria} or 'bootstrap'")
+    return power
 
 
 class BootstrapStats:
     """
     Generation empirical distribution for statistic(group A values, group B values).
 
     Attributes
@@ -317,71 +374,103 @@
         given confidence level
 
     pvalue_criterion()
         Calculate pvalue using confidence interval as criterion
 
     """
 
-    def __init__(self, bootstrap_size: int = 100, metric: Union[str, Callable] = "mean"):
+    def __init__(self, bootstrap_size: int = 10000, metric: Union[str, Callable] = "mean", paired: bool = False):
+        """
+        Parameters
+        ----------
+        bootstrap_size: int
+            Amount of bootstrap groups
+        metric: str or callable
+            Metric to be calculated - mean or fraction
+        paired: bool, default False
+            If True use paired sampling, could be usefull for paired groups
+        """
         self.__bs_size = bootstrap_size
         self.__metric_distribution = np.nan
         if isinstance(metric, str):
-            accepted_str_metrics: List[str] = ["mean", "fraction"]
+            accepted_str_metrics: List[str] = ["mean", "fraction", "median"]
             if metric not in accepted_str_metrics:
                 raise ValueError(f'Choose metric name from - {", ".join(accepted_str_metrics)}')
         self.__metric = metric
         self.__min_of_distribution = None
         self.__max_of_distribution = None
+        if isinstance(paired, bool):
+            self.__paired = paired
+        else:
+            raise ValueError("Parameter paired can only take boolean values")
 
     def __handle_str_metric(self, bootstrap_a: np.ndarray, bootstrap_b: np.ndarray) -> None:
         """
         Handle case if metric is string.
         """
         if self.__metric == "mean":
             self.__metric_distribution = np.mean(bootstrap_b, axis=1) - np.mean(bootstrap_a, axis=1)
         elif self.__metric == "fraction":
             self.__metric_distribution = np.mean(bootstrap_b, axis=1) / np.mean(bootstrap_a, axis=1) - 1
+        elif self.__metric == "median":
+            self.__metric_distribution = np.median(bootstrap_b, axis=1) - np.median(bootstrap_a, axis=1)
 
     def __handle_std_value(self) -> float:
         """
         Calculate value for criterion.
         """
         if isinstance(self.__metric, str):
-            if self.__metric in ["mean", "fraction"]:
+            if self.__metric in ["mean", "fraction", "median"]:
                 val = 0
         else:
             val = self.__metric(np.array([1]), np.array([1]))
         return val
 
-    def fit(self, group_a: Iterable[float], group_b: Iterable[float]) -> None:
+    def __handle_sampling(
+        self, group_a: Iterable[float], group_b: Iterable[float], random_seed: Optional[int] = None
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        rng = np.random.default_rng(random_seed)
+        if self.__paired:
+            a_size, b_size = len(group_a), len(group_b)
+            if a_size != b_size:
+                err: str = f"Paired groups must have equal sizes, have - {len(group_a)} and {len(group_b)}"
+                raise ValueError(err)
+            idxs: np.ndarray = rng.choice(np.arange(a_size), size=(self.__bs_size, a_size))
+            return group_a[idxs], group_b[idxs]
+        return (
+            rng.choice(group_a, size=(self.__bs_size, len(group_a))),
+            rng.choice(group_b, size=(self.__bs_size, len(group_b))),
+        )
+
+    @filter_kwargs
+    def fit(self, group_a: Iterable[float], group_b: Iterable[float], random_seed: Optional[int] = None) -> None:
         """
         Make bootstrap samples from given groups.
         Calculates and store empiric distribution for saved metric in __init__
 
         Parameters
         ----------
         group_a : Iterable[float]
             Values of A group
         group_b : Iterable[float]
             Values of B group
+        random_seed : int, optional
+            A seed for the deterministic outcome of random bootstrap processes.
 
         Returns
         -------
             Nothing
         """
         group_a = np.array(group_a)
         group_b = np.array(group_b)
-        bootstraped_a_group: np.ndarray = np.random.choice(group_a, size=(self.__bs_size, len(group_a)))
-        bootstraped_b_group: np.ndarray = np.random.choice(group_b, size=(self.__bs_size, len(group_b)))
+        bootstraped_a_group, bootstraped_b_group = self.__handle_sampling(group_a, group_b, random_seed)
         if isinstance(self.__metric, str):
             self.__handle_str_metric(bootstraped_a_group, bootstraped_b_group)
         else:
-            self.__metric_distribution = self.__metric(
-                np.mean(bootstraped_a_group, axis=1), np.mean(bootstraped_b_group, axis=1)
-            )
+            self.__metric_distribution = self.__metric(bootstraped_a_group, bootstraped_b_group)
 
     def min_of_distrbution(self) -> float:
         """
         Minimum empirical distribution
         """
         if self.__min_of_distribution is None:
             self.__min_of_distribution = np.min(self.__metric_distribution)
@@ -391,60 +480,62 @@
         """
         Maximum empirical distribution
         """
         if self.__max_of_distribution is None:
             self.__max_of_distribution = np.max(self.__metric_distribution)
         return self.__max_of_distribution
 
+    @filter_kwargs
     def confidence_interval(
         self, confidence_level: Union[float, Iterable[float]] = 0.95, alternative: str = "two-sided"
     ) -> types.IntervalType:
         """
         Returns bootstraped confidence interval, based on fit method.
 
         Parameters
         ----------
         confidence_level: Union[float, Iterable[float]], default: ``0.95``
             Bounds for error, that is
             Pr (mean(metric) not in interval) <= alpha
-        alternative : str, defaulte: ``"two-sided"``
+        alternative : str, default: ``"two-sided"``
                 Alternative for static criteria - two-sided, less, greater
                 Less means, that mean in first group less, than mean in second group
         Returns
         -------
         interval : IntervalType
             Confidence interval for each error in alpha
         """
         if not hasattr(self, "_BootstrapStats__metric_distribution"):
             raise AttributeError("Use method fit to build empirical distribution on metric")
 
         alpha: Union[float, Iterable[float]] = 1 - confidence_level
         alpha = pvalue_pkg.corrected_alpha(alpha, alternative)
         if not isinstance(alpha, float):
             alpha = np.array(alpha)
-
         left_bounds: np.ndarray = np.quantile(self.__metric_distribution, q=alpha / 2)
         right_bounds: np.ndarray = np.quantile(self.__metric_distribution, q=1 - alpha / 2)
+
         return pvalue_pkg.choose_from_bounds(
             left_bounds,
             right_bounds,
             alternative,
             left_bound=self.min_of_distrbution(),
             right_bound=self.max_of_distribution(),
         )
 
+    @filter_kwargs
     def pvalue_criterion(self, alternative: str = "two-sided") -> float:
         """
         Calculate pvalue for bootstrap criterion.
 
         Returns
         --------
         pvalue : float
             Corresponding pvalue
         alternative : str, defaulte: ``"two-sided"``
                 Alternative for static criteria - two-sided, less, greater
                 Less means, that mean in first group less, than mean in second group
         """
         criterion_value: float = self.__handle_std_value()
         return pvalue_pkg.calculate_pvalue_by_interval(
-            BootstrapStats.confidence_interval, criterion_value, self=self, alternative=alternative
+            BootstrapStats.confidence_interval, criterion_value, self=self, alternative=alternative, precision=10e-15
         )
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/knn.py` & `ambrosia-0.4.0/ambrosia/tools/knn.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tools/log.py` & `ambrosia-0.4.0/ambrosia/tools/log.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tools/pvalue_tools.py` & `ambrosia-0.4.0/ambrosia/tools/pvalue_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,17 +110,17 @@
             mean_a, mean_b, var_group_a, var_group_b, covariance_ab, mean_size
         )
         statistic: float = point_estimate / fraction_se
     else:
         raise ValueError(f"Got unknown random variable transformation: {ADMISSIBLE_TRANSFORMATIONS}")
 
     if alternative == "less":
-        pvalue: float = sps.norm.sf(statistic)
-    elif alternative == "greater":
         pvalue: float = sps.norm.cdf(statistic)
+    elif alternative == "greater":
+        pvalue: float = sps.norm.sf(statistic)
     elif alternative == "two-sided":
         pvalue: float = 2 * min(sps.norm.cdf(statistic), sps.norm.sf(statistic))
     else:
         raise ValueError(f"Incorrect alternative value - {alternative}, choose from two-sided, less, greater")
     return pvalue
 
 
@@ -153,17 +153,17 @@
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Choose left and right bounds according to alternative
     """
     cond_many: bool = isinstance(left_ci, Iterable)
     amount: int = len(left_ci) if cond_many else 1
     if alternative == "greater":
-        left_ci = np.ones(amount) * left_bound if cond_many else left_bound
-    if alternative == "less":
         right_ci = np.ones(amount) * right_bound if cond_many else right_bound
+    if alternative == "less":
+        left_ci = np.ones(amount) * left_bound if cond_many else left_bound
     return left_ci, right_ci
 
 
 def calculate_intervals_by_delta_method(
     mean_a: float,
     mean_b: float,
     var_group_a: float,
@@ -220,30 +220,30 @@
     else:
         raise ValueError(f"Got unknown random variable transformation: {ADMISSIBLE_TRANSFORMATIONS}")
     conf_intervals: List[Tuple] = list(zip(left_bounds, right_bounds))
     return conf_intervals
 
 
 def calculate_pvalue_by_interval(
-    interval_function: Callable, criterion_value_label: float = 0, precision: float = 0.00001, **kwargs
+    interval_function: Callable, criterion_value_label: float = 0, precision: float = 10e-7, **kwargs
 ) -> float:
     """
     Calculate pvalue for confidence interval.
     pvalue(x) = inf_a {a | x \\in S_a }
     S_a = {x | 0 not in interval(x) }.
 
     Parameters
     ----------
     interval_function : Callable
         Function returns confidence interval using kwargs
         Function must have argument confidence_level !!!
     criterion_value_label : float, default: ``0``
         This number indicates whether the null hypothesis should
         be rejected if it falls within the interval.
-    precision : float, default: ``0.00001``
+    precision : float, default: ``0.0000001``
         Precision for binary search solution.
 
     Returns
     -------
     pvalue : float
         P-value of the interval-induced criterion.
     """
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/split_tools.py` & `ambrosia-0.4.0/ambrosia/tools/split_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,19 @@
     id_column: Optional[types.ColumnNameType] = None,
 ) -> None:
     """
     Check if column with objects ids contains duplicates.
     """
     indices: np.ndarray = dataframe[id_column].values if id_column is not None else dataframe.index
     if len(indices) > len(set(indices)):
-        raise ValueError(f"Id column {id_column} contains duplicates, ids must be unique for split")
+        if id_column is None:
+            msg_part: str = "Index"
+        else:
+            msg_part: str = f"Id column {id_column}"
+        raise ValueError(f"{msg_part} contains duplicates, ids must be unique for split")
 
 
 def get_integer_salt(salt: Optional[str]) -> int:
     """
     Returns integer for random state numpy.
 
     Parameters
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/stat_criteria.py` & `ambrosia-0.4.0/ambrosia/tools/stat_criteria.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 import ambrosia.tools.theoretical_tools as theory_pkg
 from ambrosia import types
 from ambrosia.tools.ab_abstract_component import ABStatCriterion, StatCriterion
 
 
 def get_results_dict(alpha: float, pvalue: float, effect: float, conf_int: Tuple[float, float]):
     """
-    Returns dictionary with given values
+    Returns dictionary with given values.
     """
     return {"first_type_error": alpha, "pvalue": pvalue, "effect": effect, "confidence_interval": conf_int}
 
 
 def get_calc_effect_ttest(group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute"):
     """
-    Calculation effect for ttest
+    Calculation effect for ttest.
     """
     if effect_type == "absolute":
         return np.mean(group_b, axis=0) - np.mean(group_a, axis=0)
     elif effect_type == "relative":
         return np.mean(group_b, axis=0) / np.mean(group_a, axis=0) - 1
     else:
         raise ValueError(ABStatCriterion._send_type_error_msg())  # pylint: disable=W0212
@@ -48,15 +48,15 @@
     Unit for independent T-test.
     """
 
     implemented_effect_types: List = ["absolute", "relative"]
 
     def calculate_pvalue(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute", **kwargs):
         if effect_type == "absolute":
-            return sps.ttest_ind(a=group_a, b=group_b, equal_var=False, **kwargs).pvalue
+            return sps.ttest_ind(a=group_b, b=group_a, equal_var=False, **kwargs).pvalue
         elif effect_type == "relative":
             _, pvalue = theory_pkg.apply_delta_method(group_a, group_b, "fraction", **kwargs)
             return pvalue
         else:
             raise ValueError(self._send_type_error_msg())
 
     def calculate_effect(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute"):
@@ -67,15 +67,15 @@
         center: float,
         group_a: np.ndarray,
         group_b: np.ndarray,
         alpha: types.StatErrorType = np.array([0.05]),
         alternative: str = "two-sided",
     ):
         """
-        Helps handle different alternatives and dimension for student distribution
+        Helps handle different alternatives and dimension for student distribution.
         """
         alpha_corrected: float = pvalue_pkg.corrected_alpha(alpha, alternative)
         quantiles, std_error = theory_pkg.get_ttest_info(group_a, group_b, alpha_corrected)
         left_ci: np.ndarray = center - quantiles * std_error
         right_ci: np.ndarray = center + quantiles * std_error
         left_ci, right_ci = pvalue_pkg.choose_from_bounds(left_ci, right_ci, alternative)
         conf_intervals = list(zip(left_ci, right_ci))
@@ -123,15 +123,15 @@
     Unit for relative paired T-test.
     """
 
     implemented_effect_types: List = ["absolute", "relative"]
 
     def calculate_pvalue(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute", **kwargs):
         if effect_type == "absolute":
-            return sps.ttest_rel(a=group_a, b=group_b, **kwargs).pvalue
+            return sps.ttest_rel(a=group_b, b=group_a, **kwargs).pvalue
         elif effect_type == "relative":
             _, pvalue = theory_pkg.apply_delta_method(group_a, group_b, "fraction", dependent=True, **kwargs)
             return pvalue
         else:
             raise ValueError(self._send_type_error_msg())
 
     def calculate_effect(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute"):
@@ -204,21 +204,21 @@
     Unit for Mann-Whitney U test.
     """
 
     implemented_effect_types: List = ["absolute"]
 
     def calculate_pvalue(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute", **kwargs):
         if effect_type == "absolute":
-            return sps.mannwhitneyu(x=group_a, y=group_b, **kwargs).pvalue
+            return sps.mannwhitneyu(x=group_b, y=group_a, **kwargs).pvalue
         else:
             raise ValueError(self._send_type_error_msg())
 
     def calculate_effect(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute"):
         if effect_type == "absolute":
-            return np.median(group_b, axis=0) - np.median(group_a, axis=0)
+            return np.median(group_b, axis=0) - np.median(group_a, axis=0)  # to discuss
         else:
             raise ValueError(self._send_type_error_msg())
 
     def calculate_conf_interval(
         self,
         group_a: np.ndarray,
         group_b: np.ndarray,
@@ -239,15 +239,15 @@
     Unit for Wilcoxon paired test.
     """
 
     implemented_effect_types: List = ["absolute"]
 
     def calculate_pvalue(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute", **kwargs):
         if effect_type == "absolute":
-            return sps.wilcoxon(x=group_a, y=group_b, **kwargs).pvalue
+            return sps.wilcoxon(x=group_b, y=group_a, **kwargs).pvalue
         else:
             raise ValueError(self._send_type_error_msg())
 
     def calculate_effect(self, group_a: np.ndarray, group_b: np.ndarray, effect_type: str = "absolute"):
         if effect_type == "absolute":
             return np.median(group_b, axis=0) - np.median(group_a, axis=0)
         else:
@@ -267,7 +267,9 @@
             raise ValueError(self._send_type_error_msg())
 
 
 class ShapiroCriterion(StatCriterion):
     """
     Unit for Shapiro-Wilk test.
     """
+
+    pass
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/stratification.py` & `ambrosia-0.4.0/ambrosia/tools/stratification.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/tools/theoretical_tools.py` & `ambrosia-0.4.0/ambrosia/tools/theoretical_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 from typing import Dict, Iterable, List, Set, Tuple
 
 import numpy as np
 import pandas as pd
 import scipy.stats as sps
 import statsmodels.stats as stats
 import statsmodels.stats.api as sms
-from scipy.stats import norm
 
 import ambrosia.tools.pvalue_tools as pvalue_pkg
 from ambrosia import types
+from ambrosia.tools.configs import Alternatives
+
+from . import EFFECT_COL_NAME, FIRST_TYPE_ERROR_COL_NAME, GROUP_SIZE_COL_NAME, STAT_ERRORS_COL_NAME
 
 FIRST_TYPE_ERROR: float = 0.05
 SECOND_TYPE_ERROR: float = 0.2
 EFFECT_DEFAULT: float = 1.01
 ROUND_DIGITS_TABLE: int = 3
 ROUND_DIGITS_PERCENT: int = 1
 
@@ -54,14 +56,22 @@
     statsmodels_alternatives_encoding: Dict = {"two-sided": "two-sided", "greater": "larger", "less": "smaller"}
     if alternative not in alternatives:
         raise ValueError(f"Alternative must be one of '{alternatives}'.")
     else:
         return statsmodels_alternatives_encoding[alternative]
 
 
+def unbiased_to_sufficient(std: float, size: int) -> float:
+    """
+    Transforms unbiased estimation of standard deviation to sufficient
+    (ddof = 1) => (ddof = 0)
+    """
+    return std * np.sqrt((size - 1) / size)
+
+
 def check_target_type(
     dataframe: pd.DataFrame,
     column: types.ColumnNameType,
 ):
     """
     Check type of target: binary / non-binary.
     """
@@ -343,17 +353,18 @@
         is more robust and accurate.
 
     Returns
     -------
     df_results : pd.DataFrame
         Table with minimal sample sizes for each effect and error from input data.
     """
-    multiindex = pd.MultiIndex.from_tuples([(eff,) for eff in effects], names=["effect"])
+    multiindex = pd.MultiIndex.from_tuples([(eff,) for eff in effects], names=[EFFECT_COL_NAME])
     multicols = pd.MultiIndex.from_tuples(
-        [(f"({err_one}; {err_two})",) for err_one in first_errors for err_two in second_errors], names=["errors"]
+        [(f"({err_one}; {err_two})",) for err_one in first_errors for err_two in second_errors],
+        names=[STAT_ERRORS_COL_NAME],
     )
     df_results = pd.DataFrame(index=multiindex, columns=multicols)
 
     for eff in effects:
         for first_err in first_errors:
             for second_err in second_errors:
                 err = f"({first_err}; {second_err})"
@@ -367,15 +378,15 @@
                     groups_ratio=groups_ratio,
                     alternative=alternative,
                     stabilizing_method=stabilizing_method,
                 )
     df_results.index = pd.MultiIndex(
         levels=[[f"{np.round((x - 1) * 100, ROUND_DIGITS_PERCENT)}%" for x in effects]],
         codes=[np.arange(len(effects))],
-        names=["effects"],
+        names=[EFFECT_COL_NAME],
     )
     return df_results
 
 
 def design_groups_size(
     dataframe: pd.DataFrame,
     column: types.ColumnNameType,
@@ -477,17 +488,18 @@
         is more robust and accurate.
 
     Returns
     -------
     df_results : pd.DataFrame
         Table with minimal effects for each sample size and error from input data.
     """
-    multiindex = pd.MultiIndex.from_tuples([(size,) for size in sample_sizes], names=["sample_size"])
+    multiindex = pd.MultiIndex.from_tuples([(size,) for size in sample_sizes], names=[GROUP_SIZE_COL_NAME])
     multicols = pd.MultiIndex.from_tuples(
-        [(f"({err_one}; {err_two})",) for err_one in first_errors for err_two in second_errors], names=["errors"]
+        [(f"({err_one}; {err_two})",) for err_one in first_errors for err_two in second_errors],
+        names=[STAT_ERRORS_COL_NAME],
     )
     df_results = pd.DataFrame(index=multiindex, columns=multicols)
     for sample_size in sample_sizes:
         for first_err in first_errors:
             for second_err in second_errors:
                 err = f"({first_err}; {second_err})"
                 effect = get_minimal_determinable_effect(
@@ -497,23 +509,22 @@
                     alpha=first_err,
                     beta=second_err,
                     target_type=target_type,
                     groups_ratio=groups_ratio,
                     alternative=alternative,
                     stabilizing_method=stabilizing_method,
                 )
-                str_effect = str(np.round(effect * 100, ROUND_DIGITS_PERCENT)) + "%"
                 if as_numeric:
                     df_results.loc[(sample_size,), (err,)] = round(effect, ROUND_DIGITS_TABLE) + 1
                 else:
-                    df_results.loc[(sample_size,), (err,)] = str_effect
+                    df_results.loc[(sample_size,), (err,)] = str(np.round(effect * 100, ROUND_DIGITS_PERCENT)) + "%"
     df_results.index = pd.MultiIndex(
         levels=[sample_sizes],
         codes=[np.arange(len(sample_sizes))],
-        names=["sample_sizes"],
+        names=[GROUP_SIZE_COL_NAME],
     )
     return df_results
 
 
 def design_effect(
     dataframe: pd.DataFrame,
     column: types.ColumnNameType,
@@ -630,19 +641,19 @@
     -------
     df_results : pd.DataFrame
         Table with  sample sizes for each effect and error from input data.
     """
     effects_str = [str(round((effect - 1) * 100, ROUND_DIGITS_PERCENT)) + "%" for effect in effects]
     multiindex = pd.MultiIndex.from_tuples(
         [(first_error, effect_str) for first_error in first_errors for effect_str in effects_str],
-        names=["First type error", "Effect"],
+        names=[FIRST_TYPE_ERROR_COL_NAME, EFFECT_COL_NAME],
     )
     powers: List[np.ndarray] = []
-    for effect in effects:
-        for first_err in first_errors:
+    for first_err in first_errors:
+        for effect in effects:
             power: np.ndarray = get_power(
                 mean=mean,
                 std=std,
                 sample_size=np.array(sample_sizes),
                 effect=effect,
                 alpha=first_err,
                 target_type=target_type,
@@ -657,15 +668,15 @@
             powers.append(power)
     df_results = pd.DataFrame(
         np.vstack(powers),
         columns=sample_sizes,
         index=multiindex,
     )
     df_results.index.name = "Errors and Effects"
-    df_results.columns.name = "sample sizes"
+    df_results.columns.name = "Group sizes"
     return df_results
 
 
 def design_power(
     dataframe: pd.DataFrame,
     column: types.ColumnNameType,
     sample_sizes: Iterable[int],
@@ -726,14 +737,27 @@
         target_type,
         groups_ratio,
         alternative,
         stabilizing_method,
     )
 
 
+def get_ttest_info_from_stats(
+    var_a: float, var_b: float, n_obs_a: int, n_obs_b: int, alpha: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Returns quantiles and standard deviation of Ttest criterion statistic
+    """
+    compound_se: float = np.sqrt(var_a / n_obs_a + var_b / n_obs_b)
+    denominator: float = (var_a / n_obs_a) ** 2 / (n_obs_a - 1) + (var_b / n_obs_b) ** 2 / (n_obs_b - 1)
+    dim: float = compound_se**2 / denominator
+    quantiles: np.ndarray = sps.t.ppf(1 - alpha / 2, df=dim)
+    return quantiles, compound_se
+
+
 def get_ttest_info(group_a: np.ndarray, group_b: np.ndarray, alpha: np.ndarray) -> Tuple[np.ndarray, float]:
     """
     Compute standart error and quatiles for ttest (Welch)
     https://en.wikipedia.org/wiki/Student%27s_t-test
 
     Arguments
     ---------
@@ -748,33 +772,27 @@
     -------
     quantiles, compound_se : np.ndarray, float
         Quantiles of T_dim corresponding each alpha
         compound_se - Standart error used in t-test
     """
     variance_group_a: float = group_a.var(ddof=1)
     variance_group_b: float = group_b.var(ddof=1)
-    compound_se: float = np.sqrt(variance_group_a / len(group_a) + variance_group_b / len(group_b))
-    denominator: float = (variance_group_a / len(group_a)) ** 2 / (len(group_a) - 1) + (
-        variance_group_b / len(group_b)
-    ) ** 2 / (len(group_b) - 1)
-    dim: float = compound_se**2 / denominator
-    quantiles: np.ndarray = sps.t.ppf(1 - alpha / 2, df=dim)
-    return quantiles, compound_se
+    return get_ttest_info_from_stats(variance_group_a, variance_group_b, len(group_a), len(group_b), alpha)
 
 
 def apply_delta_method_by_stats(
     size: int,
     mean_group_a: float,
     var_group_a: float,
     mean_group_b: float,
     var_group_b: float,
     cov_groups: float = 0,
     transformation: str = "fraction",
     alpha: np.ndarray = np.array([FIRST_TYPE_ERROR]),
-    alternative: str = "two_sided",
+    alternative: str = "two-sided",
 ) -> Tuple[types.ManyIntervalType, float]:
     """
     Computation of pvalue and confidence intervals for each I type error bound (alpha)
     using Delta-method by statistics.
 
     Arguments
     ---------
@@ -867,7 +885,42 @@
         mean_b,
         std_group_b**2,
         covariance_ab,
         transformation,
         alpha,
         alternative=alternative,
     )
+
+
+def ttest_1samp_from_stats(
+    mean: float, std: float, n_obs: int, alternative: str = Alternatives.ts.value
+) -> Tuple[float, float]:
+    """
+    Implementation of ttest_1samp for stats, not from observations
+
+    Parameters
+    ----------
+    mean: float
+        Mean of samples
+    std: float
+        Standart deviation (consistent estimation)
+    n_obs: int
+        Amount of observations
+    alternative: str
+        One of two-sided, less, greater
+
+    Returns
+    -------
+    (statistic, pvalue): Tuple[float, float]
+    Statistic of criterion and pvalue
+    """
+    statistic: float = mean / std * np.sqrt(n_obs)
+
+    if alternative == Alternatives.gr.value:
+        pvalue: float = sps.t.sf(statistic, df=n_obs - 1)
+    elif alternative == Alternatives.less.value:
+        pvalue: float = sps.t.cdf(statistic, df=n_obs - 1)
+    elif alternative == Alternatives.ts.value:
+        pvalue: float = sps.t.cdf(-np.abs(statistic), df=n_obs - 1) + sps.t.sf(np.abs(statistic), df=n_obs - 1)
+    else:
+        Alternatives.raise_if_value_incorrect_enum(alternative)
+    return statistic, pvalue
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/tools.py` & `ambrosia-0.4.0/ambrosia/tools/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,107 +14,41 @@
 
 from itertools import product
 from typing import Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from hyperopt import fmin, hp, tpe
-from joblib import Parallel, delayed
-from tqdm.auto import tqdm
+from joblib import Parallel, delayed, parallel_backend
 
 import ambrosia.tools._lib._tools_aide as aid_pkg
 import ambrosia.tools.empirical_tools as emp_pkg
 from ambrosia import types
 from ambrosia.tools import back_tools
 
+from . import EFFECT_COL_NAME, FIRST_TYPE_ERROR_COL_NAME, GROUP_SIZE_COL_NAME, STAT_ERRORS_COL_NAME
+
 ROUND_DIGITS_TABLE: int = 3
 ROUND_DIGITS_PERCENT: int = 1
 
 
-def eval_error(
-    sampled_metric_vals: np.ndarray,
-    sample_size_a: int,
-    alpha: float,
-    mode: str = "ttest",
-    stat: str = "mean",
-    bootstrap_size: int = 1000,
-    random_seed: Optional[int] = None,
-    parallel: bool = False,
-    use_tqdm: bool = False,
-    verbose: bool = False,
-) -> float:
-    """
-    Evaluate correctness/II type error of the experiment.
-
-    Parameters
-    ----------
-    sampled_metric_vals : np.ndarray
-        Samples of A/B groups: |group A values|group B values|.
-    sample_size_a : int
-        Size of  the group A in ``sampled_metric_vals``, i.e.
-        first ``sample_size_a`` elements correspond to the group A.
-    alpha : float
-        First type error bound, 1 - alpha: correctness.
-    mode : str, default: ``"ttest"``
-        Statistical criterion, for example ``'ttest'``.
-    stat : str, default: ``mean``
-        Statistic to be calculated for sample groups during a bootstrap.
-    bootstrap_size : int, default: ``1000``
-        Number of bootstrap of A/B pairs.
-    random_seed: int, optional
-        A seed for the deterministic outcome of random processes.
-    parallel : bool, default: ``False``
-        Use parallel computations.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    verbose : bool, default: ``False``
-        Whether use logging.
-
-    Returns
-    -------
-    error : float
-        Second type error estimation or correctness, i.e.
-        1 - P_{A=B} (criterion is completed) - correctness
-        P_{A!=B} (criterion is completed) - second type error.
-    """
-    not_bootstrap_criteria: List[str] = ["ttest", "ttest_rel", "mw", "shapiro"]
-    if mode in not_bootstrap_criteria:
-        power: float = emp_pkg.stat_criterion_power(sampled_metric_vals, sample_size_a, criterion=mode, alpha=alpha)
-    elif mode == "bootstrap":
-        power: float = emp_pkg.make_bootstrap(
-            sampled_metric_vals,
-            sample_size_a,
-            alpha,
-            N=bootstrap_size,
-            stat=stat,
-            random_seed=random_seed,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
-            verbose=verbose,
-        )
-    else:
-        raise ValueError(f"Criterion {mode} is not found, choose from {not_bootstrap_criteria} or 'bootstrap'")
-    return 1 - power
-
-
 def bootstrap_over_statistical_population(
     dataframe: pd.DataFrame,
     metrics: List,
     sample_size_a: int,
     sample_size_b: int,
     effect: float,
     alpha: float,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
-    calculate_alpha: bool = False,
-    use_tqdm: bool = False,
-    parallel: bool = False,
+    n_jobs: bool = 1,
     verbose: bool = False,
+    **kwargs,
 ) -> List[Optional[float]]:
     """
     Evaluate errors of the experiment setup for each metric and set of parameters.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
@@ -133,88 +67,269 @@
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion to apply.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
-    calculate_alpha : bool, default: ``False``
-        Whether calculate correctness of criterion or not.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
     result_list : List[Optional[float]]
         List of calculated correctness/power for bootstraped groups
-        [corretness_0, power_0, correctness_1, power_1 ... corretness_k, power_k]
-        If not calculate_alpha -> corretness_i = None.
+        [corretness_0/power_0, correctness_1/power_1 ... corretness_k/power_k]
     """
-    seed_sequence: np.ndarray = emp_pkg.create_seed_sequence(len(metrics), random_seed)
+    seed_sequence: np.ndarray = back_tools.create_seed_sequence(len(metrics), random_seed)
     iterator = zip(metrics, seed_sequence)
     result_list = []
     for metric, seed in iterator:
-        metric_vals = dataframe[metric].values
+        metric_vals = dataframe[metric].values.astype("float32")  ## to discuss
         sampled_metric_vals = np.random.default_rng(seed).choice(
             metric_vals, size=(sample_size_a + sample_size_b, bs_samples), replace=True
         )
         modified_metric_vals = emp_pkg.inject_effect(
             sampled_metric_vals, sample_size_a, effect, modeling_method=injection_method, random_seed=seed
         )
-        if calculate_alpha:
-            correctness = eval_error(
-                sampled_metric_vals,
-                sample_size_a,
-                alpha,
-                mode=criterion,
-                random_seed=seed,
-                use_tqdm=use_tqdm,
-                parallel=parallel,
-                verbose=verbose,
-            )
-        else:
-            correctness = None
-        power = 1 - eval_error(
+        power = emp_pkg.eval_error(
             modified_metric_vals,
             sample_size_a,
             alpha,
             mode=criterion,
             random_seed=seed,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
+            n_jobs=n_jobs,
             verbose=verbose,
+            **kwargs,
         )
-        result_list.append(correctness)
         result_list.append(power)
     return result_list
 
 
+def get_errors(
+    dataframe: pd.DataFrame,
+    metrics: List,
+    sample_sizes_a: Iterable[int],
+    sample_sizes_b: Iterable[int],
+    effects: Iterable[float],
+    alphas: Iterable[float],
+    bs_samples: int = 1000,
+    criterion: str = "ttest",
+    injection_method: str = "constant",
+    random_seed: Optional[int] = None,
+    n_jobs: int = 1,
+    verbose: bool = False,
+    **kwargs,
+) -> Tuple[np.ndarray, List[np.ndarray]]:
+    """
+    Get I/II type errors estimation for the parameters of experiment.
+
+    Parameters
+    ----------
+    dataframe : pd.DataFrame
+        Given datframe with data for experiment.
+    metrics : List
+        Columns of ``dataframe`` for calculating errors.
+    sample_sizes_a : Iterable[int]
+        List of A group sizes.
+    sample_sizes_b : Iterable[int]
+        List of B group sizes.
+    effect : float
+        Expected effect in group B for the modeling.
+    alpha : float
+        First type error bound, 1 - alpha: correctness.
+    beta : float
+        Second type error, 1 - beta - power of criterion.
+    bs_samples : int, default: ``1000``
+        Amount of bootstrap pairs A/B.
+    criterion : str, default: ``"ttest"``
+        Statistical criterion.
+    injection_method : str, default: ``"constant"``
+        Method to modify group B, for example
+        constant: value = value * effect
+        for more information inspect ``inject_effect`` function.
+    random_seed : int, optional
+        A seed for the deterministic outcome of random processes.
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
+    verbose : bool, default: ``False``
+        Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
+
+    Returns
+    -------
+    parameters, empirical_errors : Tuple[Tuple, np.ndarray]
+        Parameters - Cartesian product of all sample sizes, effects, alphas
+        empirical_errors - Array of lists [corretness_0, power_0,
+        correctness_1, power_1 ... corretness_k, power_k].
+    """
+    parameters = tuple(product(zip(sample_sizes_a, sample_sizes_b), effects, alphas))
+    seed_sequence: np.ndarray = back_tools.create_seed_sequence(len(parameters), random_seed)
+    iterator = zip(parameters, seed_sequence)
+    handled_params: Dict = back_tools.handle_nested_multiprocessing(
+        n_jobs,
+        criterion,
+        bootstrap_over_statistical_population,
+        desc="Empirical errors calculation",
+        total=len(parameters),
+        **kwargs,
+    )
+    with handled_params["progress_bar"]:
+        with parallel_backend(n_jobs=handled_params["n_jobs"], backend="loky"):
+            empirical_errors = Parallel(verbose=verbose)(
+                delayed(handled_params["parallel_func"])(
+                    dataframe=dataframe,
+                    metrics=metrics,
+                    sample_size_a=params[0][0],
+                    sample_size_b=params[0][1],
+                    effect=params[1],
+                    alpha=params[2],
+                    bs_samples=bs_samples,
+                    criterion=criterion,
+                    injection_method=injection_method,
+                    random_seed=seed,
+                    n_jobs=handled_params["nested_n_jobs"],
+                    verbose=verbose,
+                    **handled_params["kwargs"],
+                )
+                for params, seed in iterator
+            )
+    return parameters, empirical_errors
+
+
+def get_empirical_table_power(
+    dataframe: pd.DataFrame,
+    metrics: List,
+    sample_sizes_a: Iterable[int],
+    sample_sizes_b: Optional[Iterable[int]],
+    effects: Iterable[int],
+    alphas: Iterable[int],
+    bs_samples: int = 1000,
+    criterion: str = "ttest",
+    injection_method: str = "constant",
+    random_seed: Optional[int] = None,
+    n_jobs: int = 1,
+    as_numeric: bool = False,
+    verbose: bool = False,
+    **kwargs,
+) -> pd.DataFrame:
+    """
+    Create table with calculated power for given data and set of parameters.
+
+    Parameters
+    ----------
+    dataframe : pd.DataFrame
+        Given datframe with data for experiment.
+    metrics : str
+        Columns of ``dataframe`` for calculating errors.
+    sample_sizes_a : Iterable[int]
+        List of A group sizes.
+    sample_sizes_b : Optional[Iterable[int]]
+        List of B group sizes, if None it will copy group A sizes.
+    effects : Iterable[float]
+        Expected effects in group B.
+    alphas : Iterable[float]
+        First type error bounds, 1 - alpha: correctness
+    bs_samples : int, default: ``1000``
+        Amount of bootstrap pairs A/B.
+    criterion : str, default: ``"ttest"``
+        Statistical criterion.
+    injection_method : str, default: ``"constant"``
+        Method to modify group B, for example
+        constant: value = value * effect
+        for more information inspect ``inject_effect`` function.
+    random_seed : int, optional
+        A seed for the deterministic outcome of random processes.
+    parallel : bool, default: ``False``
+        Whether to use parallel computing.
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
+    as_numeric : bool, default False
+        Whether to return a number or a string with percentages.
+    verbose : bool, default: ``False``
+        Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
+
+    Returns
+    -------
+    report : pd.DataFrame
+        Table with sizes for group A, group B, effects, erros and metrics names
+        |A size | B size | effect | alpha | name_correctness| name_power| ...
+    """
+    if isinstance(sample_sizes_a, List):
+        sample_sizes_a = np.array(sample_sizes_a)
+    if sample_sizes_b is None:
+        sample_sizes_b = np.copy(sample_sizes_a)
+    elif isinstance(sample_sizes_b, List):
+        sample_sizes_b = np.array(sample_sizes_b)
+    parameters, emprical_errors = get_errors(
+        dataframe=dataframe,
+        metrics=metrics,
+        sample_sizes_a=sample_sizes_a,
+        sample_sizes_b=sample_sizes_b,
+        effects=effects,
+        alphas=alphas,
+        bs_samples=bs_samples,
+        criterion=criterion,
+        injection_method=injection_method,
+        random_seed=random_seed,
+        n_jobs=n_jobs,
+        verbose=verbose,
+        **kwargs,
+    )
+    reports = {}
+    for num, metric in enumerate(metrics):
+        metric_errors: List = [errors_subset[num] for errors_subset in emprical_errors]
+        report = pd.DataFrame(
+            list(parameters), columns=[GROUP_SIZE_COL_NAME, EFFECT_COL_NAME, FIRST_TYPE_ERROR_COL_NAME]
+        ).join(pd.DataFrame(metric_errors, columns=[STAT_ERRORS_COL_NAME]))
+        report[EFFECT_COL_NAME] = (round((report[EFFECT_COL_NAME] - 1) * 100, ROUND_DIGITS_PERCENT)).astype(str) + "%"
+        report = report.pivot_table(
+            index=[FIRST_TYPE_ERROR_COL_NAME, EFFECT_COL_NAME],
+            columns=GROUP_SIZE_COL_NAME,
+            values=STAT_ERRORS_COL_NAME,
+            sort=False,
+        )
+        report = report[list(zip(sample_sizes_a, sample_sizes_b))]
+        if as_numeric:
+            report = report.applymap(lambda x: round(x, ROUND_DIGITS_TABLE))
+        else:
+            report = report.applymap(lambda x: str(round(x * 100, ROUND_DIGITS_PERCENT)) + "%")
+        if len(metrics) == 1:
+            reports = report
+        else:
+            reports[metric] = report
+    return reports
+
+
 def optimize_group_size(
     dataframe: pd.DataFrame,
     metric: str,
     effect: float,
     alpha: float,
     power: float,
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
-    calculate_alpha: bool = False,
     evals: int = 50,
     epsilon: float = 0.001,
     solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = True,
+    n_jobs: int = 1,
     verbose: bool = False,
+    **kwargs,
 ) -> int:
     """
     Find optimal group size for each metric on given parameters set.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
@@ -222,102 +337,103 @@
     metric : str
         Column of ``dataframe`` to calculate criterion.
     effect : float
         Expected effect in group B for the modeling.
     alpha : float
         First type error bound, 1 - alpha: correctness.
     power : float
-        Desired power of criterion
+        Desired power of criterion.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
-    calculate_alpha : bool, default: ``False``
-        Whether calculate correctness of criterion.
     evals : int, default: ``50``
         Evals number for optimization.
     epsilon : float, default: ``0.001``
         Precision for power estimation solution.
     soltuion : str, default: ``"binary"``
         Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
     optimal_group_size : int
         Optimal size for groups A/B to reach sufficient power and confidence
         levels.
     """
     solutions_names: List[str] = ["hyperopt", "binary"]
     power_calculation: Callable = bootstrap_over_statistical_population
 
     def objective(params: Dict) -> float:
-        group_size = int(params["group_size"])
+        group_size_a = int(params["group_size"])
+        group_size_b = int(groups_ratio * params["group_size"])
         power_emp = power_calculation(
             dataframe=dataframe,
             metrics=[metric],
-            sample_size_a=group_size,
-            sample_size_b=group_size,
+            sample_size_a=group_size_a,
+            sample_size_b=group_size_b,
             effect=effect,
             alpha=alpha,
             bs_samples=bs_samples,
             criterion=criterion,
             injection_method=injection_method,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
+            n_jobs=n_jobs,
             verbose=verbose,
-            calculate_alpha=calculate_alpha,
-        )[1]
+            **kwargs,
+        )
         delta = abs(power_emp - (power + epsilon))
         return delta
 
     upper_bound_degree: int = aid_pkg.helper_bin_search_upper_bound_size(
         power_calculation,
         power,
         ["sample_size_a", "sample_size_b"],
+        groups_ratio,
         dataframe=dataframe,
         metrics=[metric],
         effect=effect,
         alpha=alpha,
         bs_samples=bs_samples,
         criterion=criterion,
         injection_method=injection_method,
         random_seed=random_seed,
-        use_tqdm=use_tqdm,
-        parallel=parallel,
+        n_jobs=n_jobs,
         verbose=verbose,
-        calculate_alpha=calculate_alpha,
+        **kwargs,
     )
     if solution == "hyperopt":
         lower_bound_degree: int = max(0, upper_bound_degree // 2)
         # log(2) for reduction to binary logarithm
         space = {
             "group_size": hp.qloguniform(
                 "group_size", lower_bound_degree * np.log(2), upper_bound_degree * np.log(2), 1
             )
         }
         best = fmin(objective, space, algo=tpe.suggest, max_evals=evals, verbose=False)
         optimal_group_size = int(best["group_size"])
     elif solution == "binary":
         upper_bound: int = 2**upper_bound_degree
+        total_size: int = int((1 + groups_ratio) * upper_bound)
         bootstraped_samples: types.BootstrapedSamplesType = aid_pkg.__helper_generate_bootstrap_samples(
             dataframe=dataframe,
             metrics=[metric],
-            total_size=upper_bound * 2,
+            total_size=total_size,
             bootstrap_size=bs_samples,
             random_seed=random_seed,
         )
 
         modified_samples: types.BootstrapedSamplesType = aid_pkg.__helper_inject_effect(
             sampled_metrics=bootstraped_samples,
             sample_size_a=upper_bound,
@@ -329,178 +445,42 @@
             aid_pkg.__helper_get_power_for_bootstraped,
             power,
             upper_bound,
             ["sample_size"],
             modified_samples=modified_samples,
             bound_size=upper_bound,
             alpha=alpha,
+            groups_ratio=groups_ratio,
             criterion=criterion,
             random_seed=random_seed,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
+            n_jobs=n_jobs,
             verbose=verbose,
+            **kwargs,
         )
     else:
         raise ValueError(f'Choose soltuion from {", ".join(solutions_names)}')
     return optimal_group_size
 
 
-def optimize_mde(
-    dataframe: pd.DataFrame,
-    metric: str,
-    group_size: int,
-    alpha: float = 0.05,
-    power: float = 0.8,
-    bs_samples: int = 1000,
-    criterion: str = "ttest",
-    injection_method: str = "constant",
-    random_seed: Optional[int] = None,
-    calculate_alpha: bool = False,
-    evals: int = 50,
-    solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = True,
-    verbose: bool = False,
-) -> float:
-    """
-    Find minimum detectable effect for each metric on given parameters set.
-
-    Parameters
-    ----------
-    dataframe : pd.DataFrame
-        Given datframe with data for experiment.
-    metric : str
-        Column of ``dataframe`` to calculate criterion.
-    group_size : int
-        Size for group A/B.
-    alpha : float
-        First type error bound, 1 - alpha: correctness.
-    power : float
-        Desired power of criterion
-    bs_samples : int, default: ``1000``
-        Amount of bootstrap pairs A/B.
-    criterion : str, default: ``"ttest"``
-        Statistical criterion.
-    injection_method : str, default: ``"constant"``
-        Method to modify group B, for example
-        constant: value = value * effect
-        for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
-        A seed for the deterministic outcome of random processes.
-    calculate_alpha : bool, default: ``False``
-        Whether calculate correctness of criterion or not.
-    evals : int, default: ``50``
-        Evals amount for optimization.
-    solution : str, default: ``"binary"``
-        Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
-    verbose : bool, default: ``False``
-        Whether use logging or not.
-
-    Returns
-    -------
-    mde : float
-        Minimal detectable effect for given power and group size.
-    """
-    solutions_names: List[str] = ["hyperopt", "binary"]
-    power_calculation: Callable = bootstrap_over_statistical_population
-
-    def objective(params):
-        effect = params["effect"]
-        power_emp = bootstrap_over_statistical_population(
-            dataframe=dataframe,
-            metrics=[metric],
-            sample_size_a=group_size,
-            sample_size_b=group_size,
-            effect=effect,
-            alpha=alpha,
-            bs_samples=bs_samples,
-            criterion=criterion,
-            injection_method=injection_method,
-            calculate_alpha=calculate_alpha,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
-            verbose=verbose,
-        )[1]
-        if power_emp > power:
-            val = effect
-        else:
-            # Some value more than right bound
-            val = np.inf
-        return val
-
-    upper_bound_effect: float = 2 ** aid_pkg.helper_bin_searh_upper_bound_effect(
-        power_calculation,
-        power,
-        dataframe=dataframe,
-        metrics=[metric],
-        alpha=alpha,
-        sample_size_a=group_size,
-        sample_size_b=group_size,
-        bs_samples=bs_samples,
-        criterion=criterion,
-        injection_method=injection_method,
-        random_seed=random_seed,
-        calculate_alpha=calculate_alpha,
-        use_tqdm=use_tqdm,
-        parallel=parallel,
-        verbose=verbose,
-    )
-    if solution == "hyperopt":
-        space = {"effect": hp.uniform("effect", 1, upper_bound_effect)}
-        best = fmin(objective, space, algo=tpe.suggest, max_evals=evals, verbose=False)
-        optimal_effect: float = best["effect"]
-
-    elif solution == "binary":
-        bootstraped_samples: types.BootstrapedSamplesType = aid_pkg.__helper_generate_bootstrap_samples(
-            dataframe=dataframe,
-            metrics=[metric],
-            total_size=group_size * 2,
-            bootstrap_size=bs_samples,
-            random_seed=random_seed,
-        )
-        optimal_effect: int = aid_pkg.helper_binary_search_optimal_effect(
-            aid_pkg.__helper_get_power_for_bootstraped,
-            power,
-            upper_bound_effect,
-            bootstraped_samples,
-            injection_method,
-            bound_size=group_size,
-            sample_size=group_size,
-            alpha=alpha,
-            criterion=criterion,
-            random_seed=random_seed,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
-            verbose=verbose,
-        )
-    else:
-        raise ValueError(f'Choose soltuion from {", ".join(solutions_names)}')
-    return optimal_effect
-
-
 def calculate_group_size(
     dataframe: pd.DataFrame,
     metrics: List,
     effect: float,
     alpha: float,
     beta: float,
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
-    calculate_alpha: bool = False,
     evals: int = 50,
     optim_solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = True,
+    n_jobs: int = 1,
     verbose: bool = False,
+    **kwargs,
 ) -> np.ndarray:
     """
     Calculate optimal group_size for each metric on given set of parameters.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
@@ -509,691 +489,589 @@
         Columns of ``dataframe`` for calculating sufficient group sizes.
     effect : float
         Expected effect in group B for the modeling.
     alpha : float
         First type error bound, 1 - alpha: correctness.
     beta : float
         Second type error, 1 - beta - power of criterion.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
-    calculate_alpha : bool, default: ``False``
-        Whether calculate correctness of criterion.
     evals : int, default: ``50``
         Evals number for optimization.
     optim_soltuion : str, default: ``"binary"``
         Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
     group_sizes : np.ndarray
         Optimal group size for each metric from metrics list
     """
     power: float = 1 - beta
-    seed_sequence: np.ndarray = emp_pkg.create_seed_sequence(len(metrics), random_seed)
+    seed_sequence: np.ndarray = back_tools.create_seed_sequence(len(metrics), random_seed)
     iterator = zip(metrics, seed_sequence)
     group_sizes: List = []
     for metric, seed in iterator:
         optimal_group_size = optimize_group_size(
             dataframe=dataframe,
             metric=metric,
             effect=effect,
             alpha=alpha,
             power=power,
+            groups_ratio=groups_ratio,
             bs_samples=bs_samples,
             criterion=criterion,
             injection_method=injection_method,
             random_seed=seed,
-            calculate_alpha=calculate_alpha,
             evals=evals,
             solution=optim_solution,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
+            n_jobs=n_jobs,
             verbose=verbose,
+            **kwargs,
         )
         group_sizes.append(optimal_group_size)
     return np.array(group_sizes)
 
 
-def calculate_empirical_mde(
+def get_group_sizes(
     dataframe: pd.DataFrame,
     metrics: List,
-    group_size: int,
-    alpha: float,
-    beta: float,
+    effects: Iterable[float],
+    alphas: Iterable[float],
+    betas: Iterable[float],
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
-    calculate_alpha: bool = False,
     evals: int = 50,
     optim_solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = False,
+    n_jobs: int = 1,
     verbose: bool = False,
-) -> np.ndarray:
+    **kwargs,
+) -> Tuple[Tuple, List[np.ndarray]]:
     """
-    Calculate empirical MDE for each metric on given set of parameters.
+    Get optimal group sizes for the possible parameters sets of the experiment.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
         Given datframe with data for experiment.
-    metric : str
-        Column of ``dataframe`` to calculate criterion.
-    group_size : int
-        Size for group A/B.
-    alpha : float
-        First type error bound, 1 - alpha: correctness.
-    beta : float
-        Second type error, 1 - beta - power of criterion.
+    metrics : List
+        Columns of ``dataframe`` for calculating sufficient group sizes.
+    effects : Iterable[float]
+        Expected effects in group B for the modeling.
+    alphas : Iterable[float]
+        First type error bounds, 1 - alpha: correctness.
+    betas : Iterable[float]
+        Second type errors, 1 - beta = power.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
-    calculate_alpha : bool, default: ``False``
-        Whether calculate correctness of criterion or not.
     evals : int, default: ``50``
-        Evals amount for optimization.
-    optim_solution : str, default: ``"binary"``
+        Evals number for optimization.
+    optim_soltuion : str, default: ``"binary"``
         Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
-    verbose : bool, default: ``False``
-        Whether use logging or not.
-
-    Returns
-    -------
-    mdes : np.ndarray
-        List of minimal detectable effect for each metric from metrics list.
-    """
-    power: float = 1 - beta
-    seed_sequence: np.ndarray = emp_pkg.create_seed_sequence(len(metrics), random_seed)
-    iterator = zip(metrics, seed_sequence)
-    mdes: List = []
-    for metric, seed in iterator:
-        mde: float = optimize_mde(
-            dataframe=dataframe,
-            metric=metric,
-            group_size=group_size,
-            alpha=alpha,
-            power=power,
-            bs_samples=bs_samples,
-            criterion=criterion,
-            injection_method=injection_method,
-            random_seed=seed,
-            calculate_alpha=calculate_alpha,
-            evals=evals,
-            solution=optim_solution,
-            use_tqdm=use_tqdm,
-            parallel=parallel,
-            verbose=verbose,
-        )
-        mdes.append(mde)
-    return mdes
-
-
-def get_errors(
-    dataframe: pd.DataFrame,
-    metrics: List,
-    sample_sizes_a: Iterable[int],
-    sample_sizes_b: Iterable[int],
-    effects: Iterable[float],
-    alphas: Iterable[float],
-    bs_samples: int = 1000,
-    criterion: str = "ttest",
-    injection_method: str = "constant",
-    random_seed: Optional[int] = None,
-    use_tqdm: bool = False,
-    parallel: bool = False,
-    n_jobs: int = 8,
-    verbose: bool = False,
-) -> Tuple[np.ndarray, List[np.ndarray]]:
-    """
-    Get I/II type errors estimation for the parameters of experiment.
-
-    Parameters
-    ----------
-    dataframe : pd.DataFrame
-        Given datframe with data for experiment.
-    metrics : List
-        Columns of ``dataframe`` for calculating errors.
-    sample_sizes_a : Iterable[int]
-        List of A group sizes.
-    sample_sizes_b : Iterable[int]
-        List of B group sizes.
-    effect : float
-        Expected effect in group B for the modeling.
-    alpha : float
-        First type error bound, 1 - alpha: correctness.
-    beta : float
-        Second type error, 1 - beta - power of criterion.
-    bs_samples : int, default: ``1000``
-        Amount of bootstrap pairs A/B.
-    criterion : str, default: ``"ttest"``
-        Statistical criterion.
-    injection_method : str, default: ``"constant"``
-        Method to modify group B, for example
-        constant: value = value * effect
-        for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
-        A seed for the deterministic outcome of random processes.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
-    n_jobs : int, default: ``8``
+    n_jobs : int, default: ``1``
         Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
-    parameters, empirical_errors : Tuple[Tuple, np.ndarray]
+    parameters, group_sizes_list : Tuple[Tuple, Tuple[np.ndarray]]
         Parameters - Cartesian product of all sample sizes, effects, alphas
-        empirical_errors - Array of lists [corretness_0, power_0,
-        correctness_1, power_1 ... corretness_k, power_k].
+        group_sizes_list - Array of lists of sizes for each metric from metrics list.
     """
-    parameters: Tuple = tuple(product(sample_sizes_a, sample_sizes_b, effects, alphas))
-    seed_sequence: np.ndarray = emp_pkg.create_seed_sequence(len(parameters), random_seed)
+    parameters: Tuple = tuple(product(effects, alphas, betas))
+    seed_sequence: np.ndarray = back_tools.create_seed_sequence(len(parameters), random_seed)
     iterator = zip(parameters, seed_sequence)
-    if parallel:
-        with back_tools.tqdm_joblib(tqdm(desc="Empirical errors calculation", total=len(parameters))):
-            empirical_errors = Parallel(n_jobs=n_jobs, verbose=verbose, backend="multiprocessing")(
-                delayed(bootstrap_over_statistical_population)(
+    handled_params: Dict = back_tools.handle_nested_multiprocessing(
+        n_jobs, criterion, calculate_group_size, desc="Group sizes calculation", total=len(parameters), **kwargs
+    )
+    with handled_params["progress_bar"]:
+        with parallel_backend(n_jobs=handled_params["n_jobs"], backend="loky"):
+            group_sizes_list = Parallel(verbose=verbose)(
+                delayed(handled_params["parallel_func"])(
                     dataframe=dataframe,
                     metrics=metrics,
-                    sample_size_a=params[0],
-                    sample_size_b=params[1],
-                    effect=params[2],
-                    alpha=params[3],
-                    bs_samples=bs_samples,
+                    effect=params[0],
+                    alpha=params[1],
+                    beta=params[2],
+                    groups_ratio=groups_ratio,
                     criterion=criterion,
+                    bs_samples=bs_samples,
                     injection_method=injection_method,
-                    random_seed=seed,
-                    calculate_alpha=True,
-                    use_tqdm=use_tqdm,
-                    parallel=parallel,
+                    n_jobs=handled_params["nested_n_jobs"],
                     verbose=verbose,
+                    evals=evals,
+                    optim_solution=optim_solution,
+                    random_seed=seed,
+                    **handled_params["kwargs"],
                 )
                 for params, seed in iterator
             )
-    else:
-        empirical_errors: List[np.ndarray] = []
-        if use_tqdm:
-            iterator = tqdm(iterator)
-        for params, seed in iterator:
-            errors = bootstrap_over_statistical_population(
-                dataframe=dataframe,
-                metrics=metrics,
-                sample_size_a=params[0],
-                sample_size_b=params[1],
-                effect=params[2],
-                alpha=params[3],
-                bs_samples=bs_samples,
-                criterion=criterion,
-                injection_method=injection_method,
-                random_seed=seed,
-                calculate_alpha=True,
-                use_tqdm=use_tqdm,
-                parallel=parallel,
-                verbose=verbose,
-            )
-            empirical_errors.append(errors)
-    return parameters, empirical_errors
+    return parameters, group_sizes_list
 
 
-def get_group_sizes(
+def get_empirical_table_sample_size(
     dataframe: pd.DataFrame,
     metrics: List,
     effects: Iterable[float],
     alphas: Iterable[float],
     betas: Iterable[float],
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
     evals: int = 50,
     optim_solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = False,
-    n_jobs: int = 8,
+    n_jobs: int = 1,
     verbose: bool = False,
-) -> Tuple[Tuple, List[np.ndarray]]:
+    **kwargs,
+) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
     """
-    Get optimal group sizes for the possible parameters sets of the experiment.
+    Create pandas table with optimal group sizes for given data and set of parameters.
 
     Parameters
     ----------
-    dataframe : pd.DataFrame
+    dataframe: pd.DataFrame
         Given datframe with data for experiment.
     metrics : List
         Columns of ``dataframe`` for calculating sufficient group sizes.
     effects : Iterable[float]
-        Expected effects in group B for the modeling.
+        Expected effects in group B.
     alphas : Iterable[float]
         First type error bounds, 1 - alpha: correctness.
     betas : Iterable[float]
         Second type errors, 1 - beta = power.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
-    calculate_alpha : bool, default: ``False``
-        Whether calculate correctness of criterion.
     evals : int, default: ``50``
-        Evals number for optimization.
-    optim_soltuion : str, default: ``"binary"``
+        Evals amount for optimization.
+    optim_solution : str, default: ``"binary"``
         Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
-    n_jobs : int, default: ``8``
-        Amount of threads/workers for parallel
+    n_jobs : int, default: ``1``
+        Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
-    parameters, group_sizes_list : Tuple[Tuple, Tuple[np.ndarray]]
-        Parameters - Cartesian product of all sample sizes, effects, alphas
-        group_sizes_list - Array of lists of sizes for each metric from metrics list.
+    report : Union[pd.DataFrame, Dict[str, pd.DataFrame]
+        Tables with sizes for group A, group B, effects, errors and metrics names
+        Effects as indices
+        (alpha(1 type error), beta(2 type error)) for columns
+        table for each metric: dict[metric name] = table with sizes.
     """
-    parameters: Tuple = tuple(product(effects, alphas, betas))
-    seed_sequence: np.ndarray = emp_pkg.create_seed_sequence(len(parameters), random_seed)
-    iterator = zip(parameters, seed_sequence)
-    if parallel:
-        with back_tools.tqdm_joblib(tqdm(desc="Group sizes calculation", total=len(parameters))):
-            group_sizes_list = Parallel(n_jobs=n_jobs, verbose=verbose, backend="multiprocessing")(
-                delayed(calculate_group_size)(
-                    dataframe=dataframe,
-                    metrics=metrics,
-                    effect=params[0],
-                    alpha=params[1],
-                    beta=params[2],
-                    criterion=criterion,
-                    bs_samples=bs_samples,
-                    injection_method=injection_method,
-                    use_tqdm=use_tqdm,
-                    parallel=parallel,
-                    verbose=verbose,
-                    evals=evals,
-                    optim_solution=optim_solution,
-                    random_seed=seed,
-                )
-                for params, seed in iterator
-            )
-    else:
-        if use_tqdm:
-            iterator = tqdm(iterator)
-        group_sizes_list: List[np.ndarray] = []
-        for params, seed in iterator:
-            group_sizes = calculate_group_size(
-                dataframe=dataframe,
-                metrics=metrics,
-                effect=params[0],
-                alpha=params[1],
-                beta=params[2],
-                criterion=criterion,
-                bs_samples=bs_samples,
-                injection_method=injection_method,
-                random_seed=seed,
-                evals=evals,
-                optim_solution=optim_solution,
-                use_tqdm=use_tqdm,
-                parallel=parallel,
-                verbose=verbose,
-            )
-            group_sizes_list.append(group_sizes)
-    return parameters, group_sizes_list
+    parameters, group_sizes_list = get_group_sizes(
+        dataframe=dataframe,
+        metrics=metrics,
+        effects=effects,
+        alphas=alphas,
+        betas=betas,
+        groups_ratio=groups_ratio,
+        bs_samples=bs_samples,
+        criterion=criterion,
+        injection_method=injection_method,
+        random_seed=random_seed,
+        evals=evals,
+        optim_solution=optim_solution,
+        n_jobs=n_jobs,
+        verbose=verbose,
+        **kwargs,
+    )
+    reports = {}
+    for num, metric in enumerate(metrics):
+        report = pd.DataFrame(list(parameters), columns=[EFFECT_COL_NAME, "alpha", "beta"]).join(
+            pd.DataFrame(list(np.array(group_sizes_list)[:, num]), columns=[GROUP_SIZE_COL_NAME])
+        )
+        report[STAT_ERRORS_COL_NAME] = tuple(zip(report["alpha"], report["beta"]))
+        report = report.pivot_table(
+            index=EFFECT_COL_NAME, columns=STAT_ERRORS_COL_NAME, values=GROUP_SIZE_COL_NAME, sort=False
+        )
+        report.index = (np.round((report.index - 1) * 100, ROUND_DIGITS_PERCENT)).astype(str) + "%"
+        if len(metrics) == 1:
+            reports = report
+        else:
+            reports[metric] = report
+    return reports
 
 
-def get_empirical_mde(
+def optimize_mde(
     dataframe: pd.DataFrame,
-    metrics: List,
-    group_sizes: Iterable[int],
-    alphas: Iterable[float],
-    betas: Iterable[float],
+    metric: str,
+    group_size: int,
+    alpha: float = 0.05,
+    power: float = 0.8,
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
     evals: int = 50,
-    optim_solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = False,
-    n_jobs: int = 8,
+    solution: str = "binary",
+    n_jobs: int = 1,
     verbose: bool = False,
-) -> Tuple[Tuple, List[np.ndarray]]:
+    **kwargs,
+) -> float:
     """
-    Get empirical MDEs for the possible parameters sets of experiment.
+    Find minimum detectable effect for each metric on given parameters set.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
         Given datframe with data for experiment.
-    metrics : str
-        Column of ``dataframe`` to calculate minimal detectable effect.
-    group_sizes : Iterable[int]
-        Sizes for groups A/B.
-    alphas : Iterable[float]
-        First type error bounds, 1 - alpha: correctness
-    betas : Iterable[float]
-        Second type erros, 1 - beta = power
+    metric : str
+        Column of ``dataframe`` to calculate criterion.
+    group_size : int
+        Size for group A/B.
+    alpha : float
+        First type error bound, 1 - alpha: correctness.
+    power : float
+        Desired power of criterion.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
-    calculate_alpha : bool, default: ``False``
-        Whether calculate correctness of criterion or not.
     evals : int, default: ``50``
         Evals amount for optimization.
-    optim_solution : str, default: ``"binary"``
+    solution : str, default: ``"binary"``
         Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
-    n_jobs : int, default: ``8``
+    n_jobs : int, default: ``1``
         Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
-    parameters, empirical_errors : Tuple[Tuple, np.ndarray]
-        Parameters - Cartesian product of all sample sizes, effects, alphas
-        mde_list - Array of lists of mde lists for each metric from metrics list.
+    mde : float
+        Minimal detectable effect for given power and group size.
     """
-    parameters: Tuple = tuple(product(group_sizes, alphas, betas))
-    seed_sequence: np.ndarray = emp_pkg.create_seed_sequence(len(parameters), random_seed)
-    iterator = zip(parameters, seed_sequence)
-    if parallel:
-        with back_tools.tqdm_joblib(tqdm(desc="MDE calculation", total=len(parameters))):
-            mde_list = Parallel(n_jobs=n_jobs, verbose=verbose, backend="multiprocessing")(
-                delayed(calculate_empirical_mde)(
-                    dataframe=dataframe,
-                    metrics=metrics,
-                    group_size=params[0],
-                    alpha=params[1],
-                    beta=params[2],
-                    criterion=criterion,
-                    bs_samples=bs_samples,
-                    injection_method=injection_method,
-                    random_seed=seed,
-                    evals=evals,
-                    optim_solution=optim_solution,
-                    use_tqdm=use_tqdm,
-                    parallel=parallel,
-                    verbose=verbose,
-                )
-                for params, seed in iterator
-            )
+    solutions_names: List[str] = ["hyperopt", "binary"]
+    power_calculation: Callable = bootstrap_over_statistical_population
+    sample_size_a, sample_size_b = group_size, int(groups_ratio * group_size)
+
+    def objective(params):
+        effect = params["effect"]
+        power_emp = power_calculation(
+            dataframe=dataframe,
+            metrics=[metric],
+            sample_size_a=sample_size_a,
+            sample_size_b=sample_size_b,
+            effect=effect,
+            alpha=alpha,
+            bs_samples=bs_samples,
+            criterion=criterion,
+            injection_method=injection_method,
+            n_jobs=n_jobs,
+            verbose=verbose,
+            **kwargs,
+        )
+        if power_emp > power:
+            val = effect
+        else:
+            # Some value more than right bound
+            val = np.inf
+        return val
+
+    upper_bound_effect: float = 2 ** aid_pkg.helper_bin_searh_upper_bound_effect(
+        power_calculation,
+        power,
+        dataframe=dataframe,
+        metrics=[metric],
+        alpha=alpha,
+        sample_size_a=sample_size_a,
+        sample_size_b=sample_size_b,
+        bs_samples=bs_samples,
+        criterion=criterion,
+        injection_method=injection_method,
+        random_seed=random_seed,
+        n_jobs=n_jobs,
+        verbose=verbose,
+        **kwargs,
+    )
+    if solution == "hyperopt":
+        space = {"effect": hp.uniform("effect", 1, upper_bound_effect)}
+        best = fmin(objective, space, algo=tpe.suggest, max_evals=evals, verbose=False)
+        optimal_effect: float = best["effect"]
+
+    elif solution == "binary":
+        bootstraped_samples: types.BootstrapedSamplesType = aid_pkg.__helper_generate_bootstrap_samples(
+            dataframe=dataframe,
+            metrics=[metric],
+            total_size=sample_size_a + sample_size_b,
+            bootstrap_size=bs_samples,
+            random_seed=random_seed,
+        )
+        optimal_effect: int = aid_pkg.helper_binary_search_optimal_effect(
+            aid_pkg.__helper_get_power_for_bootstraped,
+            power,
+            upper_bound_effect,
+            bootstraped_samples,
+            injection_method,
+            bound_size=group_size,
+            sample_size=group_size,
+            alpha=alpha,
+            groups_ratio=groups_ratio,
+            criterion=criterion,
+            random_seed=random_seed,
+            n_jobs=n_jobs,
+            verbose=verbose,
+            **kwargs,
+        )
     else:
-        mde_list: List[np.ndarray] = []
-        if use_tqdm:
-            iterator = tqdm(iterator)
-        for params, seed in iterator:
-            mdes = calculate_empirical_mde(
-                dataframe=dataframe,
-                metrics=metrics,
-                group_size=params[0],
-                alpha=params[1],
-                beta=params[2],
-                criterion=criterion,
-                bs_samples=bs_samples,
-                injection_method=injection_method,
-                random_seed=seed,
-                evals=evals,
-                optim_solution=optim_solution,
-                use_tqdm=use_tqdm,
-                parallel=parallel,
-                verbose=verbose,
-            )
-            mde_list.append(mdes)
-    return parameters, mde_list
+        raise ValueError(f'Choose soltuion from {", ".join(solutions_names)}')
+    return optimal_effect
 
 
-def get_empirical_errors_table(
+def calculate_empirical_mde(
     dataframe: pd.DataFrame,
     metrics: List,
-    sample_sizes_a: Iterable[int],
-    sample_sizes_b: Optional[Iterable[int]],
-    effects: Iterable[int],
-    alphas: Iterable[int],
+    group_size: int,
+    alpha: float,
+    beta: float,
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
-    use_tqdm: bool = False,
-    parallel: bool = False,
-    n_jobs: int = 8,
+    evals: int = 50,
+    optim_solution: str = "binary",
+    n_jobs: int = 1,
     verbose: bool = False,
-) -> pd.DataFrame:
+    **kwargs,
+) -> np.ndarray:
     """
-    Create pandas table with type I and type II errors (power) for given data and set of parameters.
+    Calculate empirical MDE for each metric on given set of parameters.
 
     Parameters
     ----------
     dataframe : pd.DataFrame
         Given datframe with data for experiment.
-    metrics : str
-        Columns of ``dataframe`` for calculating errors.
-    sample_sizes_a : Iterable[int]
-        List of A group sizes.
-    sample_sizes_b : Optional[Iterable[int]]
-        List of B group sizes, if None it will copy group A sizes.
-    effects : Iterable[float]
-        Expected effects in group B.
-    alphas : Iterable[float]
-        First type error bounds, 1 - alpha: correctness
+    metric : str
+        Column of ``dataframe`` to calculate criterion.
+    group_size : int
+        Size for group A/B.
+    alpha : float
+        First type error bound, 1 - alpha: correctness.
+    beta : float
+        Second type error, 1 - beta - power of criterion.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
-    n_jobs : int, default: ``8``
+    evals : int, default: ``50``
+        Evals amount for optimization.
+    optim_solution : str, default: ``"binary"``
+        Optimizer method.
+    n_jobs : int, default: ``1``
         Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
-    report : pd.DataFrame
-        Table with sizes for group A, group B, effects, erros and metrics names
-        |A size | B size | effect | alpha | name_correctness| name_power| ...
+    mdes : np.ndarray
+        List of minimal detectable effect for each metric from metrics list.
     """
-    if isinstance(sample_sizes_a, List):
-        sample_sizes_a = np.array(sample_sizes_a)
-    if sample_sizes_b is None:
-        sample_sizes_b = np.copy(sample_sizes_a)
-    elif isinstance(sample_sizes_b, List):
-        sample_sizes_b = np.array(sample_sizes_b)
-    parameters, emprical_errors = get_errors(
-        dataframe=dataframe,
-        metrics=metrics,
-        sample_sizes_a=sample_sizes_a,
-        sample_sizes_b=sample_sizes_b,
-        effects=effects,
-        alphas=alphas,
-        bs_samples=bs_samples,
-        criterion=criterion,
-        injection_method=injection_method,
-        random_seed=random_seed,
-        use_tqdm=use_tqdm,
-        parallel=parallel,
-        n_jobs=n_jobs,
-        verbose=verbose,
-    )
-    columns_params = ["size_A", "size_B", "effect", "alpha"]
-    columns_errors = []
-    for metric in metrics:
-        columns_errors += [metric + "_correctness", metric + "_power"]
-    report = pd.DataFrame(list(parameters), columns=columns_params).join(
-        pd.DataFrame(list(emprical_errors), columns=columns_errors)
-    )
-    return report
+    power: float = 1 - beta
+    seed_sequence: np.ndarray = back_tools.create_seed_sequence(len(metrics), random_seed)
+    iterator = zip(metrics, seed_sequence)
+    mdes: List = []
+    for metric, seed in iterator:
+        mde: float = optimize_mde(
+            dataframe=dataframe,
+            metric=metric,
+            group_size=group_size,
+            alpha=alpha,
+            power=power,
+            groups_ratio=groups_ratio,
+            bs_samples=bs_samples,
+            criterion=criterion,
+            injection_method=injection_method,
+            random_seed=seed,
+            evals=evals,
+            solution=optim_solution,
+            n_jobs=n_jobs,
+            verbose=verbose,
+            **kwargs,
+        )
+        mdes.append(mde)
+    return mdes
 
 
-def get_empirical_table_sample_size(
+def get_empirical_mde(
     dataframe: pd.DataFrame,
     metrics: List,
-    effects: Iterable[float],
+    group_sizes: Iterable[int],
     alphas: Iterable[float],
     betas: Iterable[float],
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
     evals: int = 50,
     optim_solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = True,
-    n_jobs: int = 8,
+    n_jobs: int = 1,
     verbose: bool = False,
-) -> Union[pd.DataFrame, Dict[str, pd.DataFrame]]:
+    **kwargs,
+) -> Tuple[Tuple, List[np.ndarray]]:
     """
-    Create pandas table with optimal group sizes for given data and set of parameters.
+    Get empirical MDEs for the possible parameters sets of experiment.
 
     Parameters
     ----------
-    dataframe: pd.DataFrame
+    dataframe : pd.DataFrame
         Given datframe with data for experiment.
-    metrics : List
-        Columns of ``dataframe`` for calculating sufficient group sizes.
-    effects : Iterable[float]
-        Expected effects in group B.
+    metrics : str
+        Column of ``dataframe`` to calculate minimal detectable effect.
+    group_sizes : Iterable[int]
+        Sizes for groups A/B.
     alphas : Iterable[float]
-        First type error bounds, 1 - alpha: correctness.
+        First type error bounds, 1 - alpha: correctness
     betas : Iterable[float]
-        Second type errors, 1 - beta = power.
+        Second type erros, 1 - beta = power.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
     evals : int, default: ``50``
         Evals amount for optimization.
     optim_solution : str, default: ``"binary"``
         Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing.
-    n_jobs : int, default: ``8``
+    n_jobs : int, default: ``1``
         Amount of threads/workers for parallel.
     verbose : bool, default: ``False``
         Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
-    report : Union[pd.DataFrame, Dict[str, pd.DataFrame]
-        Tables with sizes for group A, group B, effects, erros and metrics names
-        Effects as indices
-        (alpha(1 type error), beta(2 type error)) for columns
-        table for each metric: dict[metric name] = table with sizes.
+    parameters, empirical_errors : Tuple[Tuple, np.ndarray]
+        Parameters - Cartesian product of all sample sizes, effects, alphas
+        mde_list - Array of lists of mde lists for each metric from metrics list.
     """
-    parameters, group_sizes_list = get_group_sizes(
-        dataframe=dataframe,
-        metrics=metrics,
-        effects=effects,
-        alphas=alphas,
-        betas=betas,
-        bs_samples=bs_samples,
-        criterion=criterion,
-        injection_method=injection_method,
-        random_seed=random_seed,
-        evals=evals,
-        optim_solution=optim_solution,
-        use_tqdm=use_tqdm,
-        parallel=parallel,
-        n_jobs=n_jobs,
-        verbose=verbose,
+    parameters: Tuple = tuple(product(group_sizes, alphas, betas))
+    seed_sequence: np.ndarray = back_tools.create_seed_sequence(len(parameters), random_seed)
+    iterator = zip(parameters, seed_sequence)
+    handled_params: Dict = back_tools.handle_nested_multiprocessing(
+        n_jobs, criterion, calculate_empirical_mde, desc="MDE calculation", total=len(parameters), **kwargs
     )
-    reports = {}
-    for num, metric in enumerate(metrics):
-        report = pd.DataFrame(list(parameters), columns=["effect", "alpha", "beta"]).join(
-            pd.DataFrame(list(np.array(group_sizes_list)[:, num]), columns=["sample_sizes"])
-        )
-        report["effect"] = (round((report["effect"] - 1) * 100, ROUND_DIGITS_PERCENT)).astype(str) + "%"
-        report["errors"] = tuple(zip(report["alpha"], report["beta"]))
-        report = report.pivot(index="effect", columns="errors", values="sample_sizes")
-        report = report.sort_values(report.columns[0])
-        if len(metrics) == 1:
-            reports = report
-        else:
-            reports[metric] = report
-    return reports
+    with handled_params["progress_bar"]:
+        with parallel_backend(n_jobs=handled_params["n_jobs"], backend="loky"):
+            mde_list = Parallel(verbose=verbose)(
+                delayed(handled_params["parallel_func"])(
+                    dataframe=dataframe,
+                    metrics=metrics,
+                    group_size=params[0],
+                    alpha=params[1],
+                    beta=params[2],
+                    groups_ratio=groups_ratio,
+                    criterion=criterion,
+                    bs_samples=bs_samples,
+                    injection_method=injection_method,
+                    random_seed=seed,
+                    evals=evals,
+                    optim_solution=optim_solution,
+                    n_jobs=handled_params["nested_n_jobs"],
+                    verbose=verbose,
+                    **handled_params["kwargs"],
+                )
+                for params, seed in iterator
+            )
+    return parameters, mde_list
 
 
 def get_empirical_mde_table(
     dataframe: pd.DataFrame,
     metrics: List,
     group_sizes: Iterable[int],
     alphas: Iterable[float],
     betas: Iterable[float],
+    groups_ratio: float = 1.0,
     bs_samples: int = 1000,
     criterion: str = "ttest",
     injection_method: str = "constant",
     random_seed: Optional[int] = None,
     evals: int = 50,
     optim_solution: str = "binary",
-    use_tqdm: bool = False,
-    parallel: bool = True,
-    n_jobs: int = 8,
-    verbose: bool = False,
+    n_jobs: int = 1,
     as_numeric: bool = False,
+    verbose: bool = False,
+    **kwargs,
 ) -> Union[pd.DataFrame, Dict]:
     """
     Create pandas table with MDEs for given data and set of parameters.
 
     Parameters
     ----------
     dataframe: pd.DataFrame
@@ -1202,38 +1080,38 @@
         Columns of ``dataframe`` for calculating sufficient group sizes.
     group_sizes : Iterable[int]
         Sizes for groups A/B.
     alphas : Iterable[float]
         First type error bounds, 1 - alpha: correctness.
     betas : Iterable[float]
         Second type errors, 1 - beta = power.
+    groups_ratio : float, default: ``1.0``
+        Ratio between groups A and B.
     bs_samples : int, default: ``1000``
         Amount of bootstrap pairs A/B.
     criterion : str, default: ``"ttest"``
         Statistical criterion.
     injection_method : str, default: ``"constant"``
         Method to modify group B, for example
         constant: value = value * effect
         for more information inspect ``inject_effect`` function.
-    random_seed: int, optional
+    random_seed : int, optional
         A seed for the deterministic outcome of random processes.
     evals : int, default: ``50``
         Evals amount for optimization.
     optim_solution : str, default: ``"binary"``
         Optimizer method.
-    use_tqdm : bool, default: ``False``
-        Use tqdm progress bar.
-    parallel : bool, default: ``False``
-        Whether to use parallel computing,
-    n_jobs : int, default: ``8``
+    n_jobs : int, default: ``1``
         Amount of threads/workers for parallel.
-    verbose : bool, default: ``False``
-        Whether use logging or not.
     as_numeric : bool, default False
         Whether to return a number or a string with percentages.
+    verbose : bool, default: ``False``
+        Whether use logging or not.
+    **kwargs : Dict
+        Other keyword arguments.
 
     Returns
     -------
     report: Union[pd.DataFrame, Dict[str, pd.DataFrame]
         Tables with sizes for group A, group B, effects, erros and metrics names
         Group sizes for indices
         (alpha(1 type error), beta(2 type error)) for columns
@@ -1241,35 +1119,37 @@
     """
     parameters, effects = get_empirical_mde(
         dataframe=dataframe,
         metrics=metrics,
         group_sizes=group_sizes,
         alphas=alphas,
         betas=betas,
+        groups_ratio=groups_ratio,
         bs_samples=bs_samples,
         criterion=criterion,
         injection_method=injection_method,
         random_seed=random_seed,
         evals=evals,
         optim_solution=optim_solution,
-        use_tqdm=use_tqdm,
-        parallel=parallel,
         n_jobs=n_jobs,
         verbose=verbose,
+        **kwargs,
     )
     reports = {}
     for num, metric in enumerate(metrics):
-        report = pd.DataFrame(list(parameters), columns=["group_sizes", "alpha", "beta"]).join(
-            pd.DataFrame(list(np.array(effects)[:, num]), columns=["effect"])
+        report = pd.DataFrame(list(parameters), columns=[GROUP_SIZE_COL_NAME, "alpha", "beta"]).join(
+            pd.DataFrame(list(np.array(effects)[:, num]), columns=[EFFECT_COL_NAME])
+        )
+        report[STAT_ERRORS_COL_NAME] = tuple(zip(report["alpha"], report["beta"]))
+        report = report.pivot_table(
+            index=GROUP_SIZE_COL_NAME, columns=STAT_ERRORS_COL_NAME, values=EFFECT_COL_NAME, sort=False
         )
         if as_numeric:
-            report["effect"] = round(report["effect"], ROUND_DIGITS_TABLE)
+            report = report.applymap(lambda x: round(x, ROUND_DIGITS_TABLE))
         else:
-            report["effect"] = (round((report["effect"] - 1) * 100, ROUND_DIGITS_PERCENT)).astype(str) + "%"
-        report["errors"] = tuple(zip(report["alpha"], report["beta"]))
-        report = report.pivot(index="group_sizes", columns="errors", values="effect")
-        report = report.sort_index()
+            report = report.applymap(lambda x: str(round((x - 1) * 100, ROUND_DIGITS_PERCENT)) + "%")
+        report = report[[(alpha, beta) for alpha in alphas for beta in betas]]
         if len(metrics) == 1:
             reports = report
         else:
             reports[metric] = report
     return reports
```

### Comparing `ambrosia-0.3.0/ambrosia/tools/type_checks.py` & `ambrosia-0.4.0/ambrosia/tools/type_checks.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/ambrosia/types.py` & `ambrosia-0.4.0/ambrosia/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,22 +12,38 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import Any, Callable, Dict, Iterable, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
-import pyspark
+
+from ambrosia.tools.import_tools import spark_installed
+
+if spark_installed():
+    import pyspark
 
 # PySpark types
 
-SparkSession = pyspark.sql.session.SparkSession
-SparkDataFrame = pyspark.sql.dataframe.DataFrame
-SparkColumn = pyspark.sql.column.Column
-SparkOrPandas = Union[SparkDataFrame, pd.DataFrame]
+
+class PySparkStub:
+    pass
+
+
+if spark_installed():
+    SparkSession = pyspark.sql.session.SparkSession
+    SparkDataFrame = pyspark.sql.dataframe.DataFrame
+    SparkColumn = pyspark.sql.column.Column
+    SparkOrPandas = Union[SparkDataFrame, pd.DataFrame]
+else:
+    SparkSession = PySparkStub
+    SparkDataFrame = PySparkStub
+    SparkColumn = PySparkStub
+    SparkOrPandas = PySparkStub
+
 
 # Global types
 
 # Type for passed data
 PassedDataType = Union[pd.DataFrame, SparkDataFrame, str]
 
 # Type for selected set of arguments names and values
```

### Comparing `ambrosia-0.3.0/ambrosia/version.py` & `ambrosia-0.4.0/ambrosia/version.py`

 * *Files identical despite different names*

### Comparing `ambrosia-0.3.0/pyproject.toml` & `ambrosia-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Ambrosia"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Python library for working with A/B tests."
 license = "Apache-2.0"
 authors = [
     "Aslan Bayramkulov <aslan.bayramkulov96@gmail.com>",
     "Artem Khakimov <artem.khakimov@gmail.com>",
     "Artem Vasin <p1not1equals1np@gmail.com>",
 ]
@@ -41,15 +41,15 @@
 [tool.poetry.dependencies]
 python = ">=3.7.2, <3.11.0"
 jinja2 = "^3.0.0"
 joblib = "^1.1.0"
 nmslib = "^2.0.4"
 numpy = ">=1.19.5, <2.0.0"
 pandas = ">=0.25.3, <2.0.0"
-pyspark = "^3.2"
+pyspark = { version = "^3.2", optional = true }
 PyYAML = "6.0"
 scikit-learn = "^1.0.2"
 scipy = "^1.6.3"
 tqdm = "^4.27.0"
 hyperopt = "^0.2.7"
 catboost = "^1.0.4"
 statsmodels = ">=0.13.0"
@@ -61,14 +61,17 @@
 pylint = "2.14.5"
 flake8 = "4.0.1"
 flake8-docstrings = "1.6.0"
 pytest = "7.1.2"
 pytest-cov = "3.0.0"
 pytest-lazy-fixture = "0.6.3"
 
+[tool.poetry.extras]
+spark = ["pyspark"]
+
 [tool.black]
 line-length = 120
 target-version = ['py37', 'py38', 'py39', 'py310']
 include = '\.pyi?$'
 exclude = '''
 
 (
@@ -95,8 +98,8 @@
 markers = [
     "unit: mark a test as a unit test",
     "smoke: mark a test as smoke test"
 ]
 
 [build-system]
 requires = ["poetry>=1.0.5"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.masonry.api"
```

### Comparing `ambrosia-0.3.0/setup.py` & `ambrosia-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,32 +22,35 @@
  'catboost>=1.0.4,<2.0.0',
  'hyperopt>=0.2.7,<0.3.0',
  'jinja2>=3.0.0,<4.0.0',
  'joblib>=1.1.0,<2.0.0',
  'nmslib>=2.0.4,<3.0.0',
  'numpy>=1.19.5,<2.0.0',
  'pandas>=0.25.3,<2.0.0',
- 'pyspark>=3.2,<4.0',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.6.3,<2.0.0',
  'statsmodels>=0.13.0',
  'tqdm>=4.27.0,<5.0.0']
 
+extras_require = \
+{'spark': ['pyspark>=3.2,<4.0']}
+
 setup_kwargs = {
     'name': 'ambrosia',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'A Python library for working with A/B tests.',
-    'long_description': ".. shields start\n\nAmbrosia\n========\n\n|PyPI| |PyPI License| |ReadTheDocs| |Tests| |Coverage| |Black| |Python Versions| |Telegram Channel|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/ambrosia\n    :target: https://pypi.org/project/ambrosia\n.. |PyPI License| image:: https://img.shields.io/pypi/l/ambrosia.svg\n    :target: https://github.com/MobileTeleSystems/Ambrosia/blob/main/LICENSE\n.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/ambrosia.svg\n    :target: https://ambrosia.readthedocs.io\n.. |Tests| image:: https://img.shields.io/github/actions/workflow/status/MobileTeleSystems/Ambrosia/test.yaml?branch=main\n    :target: https://github.com/MobileTeleSystems/Ambrosia/actions/workflows/test.yaml?query=branch%3Amain+\n.. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/Ambrosia/branch/main/graph/badge.svg\n    :target: https://codecov.io/gh/MobileTeleSystems/Ambrosia\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/ambrosia.svg\n    :target: https://pypi.org/project/ambrosia  \n.. |Telegram Channel| image:: https://img.shields.io/badge/telegram-Ambrosia-blueviolet.svg?logo=telegram\n    :target: https://t.me/+Tkt43TNUUSAxNWNi\n\n.. shields end\n\n.. image:: https://raw.githubusercontent.com/MobileTeleSystems/Ambrosia/main/docs/source/_static/ambrosia.png\n   :height: 320 px\n   :width: 320 px\n   :align: center\n\n.. title\n\n**Ambrosia** is a Python library for A/B tests design, split and effect \nmeasurement. It provides rich set of methods for conducting full \nA/B test pipeline. \n\nAn experiment design stage is performed using metrics historical data \nwhich could be processed in both forms of pandas and spark dataframes \nwith either theoretical or empirical approach. \n\nGroup split methods support different strategies and multi-group split, \nwhich allows to quickly create control and test groups of interest. \n\nFinal effect measurement stage is conducted via testing tools that \nare able to return relative and absolute effects and construct corresponding \nconfidence intervalsfor continious and binary variables. \nTesting tools as well as design ones support significant number of \nstatistical criteria, like t-test, non-parametric, and bootstrap. \n\nFor additional A/B tests support library provides features and tools \nfor data preproccesing and experiment acceleration.\n\n.. functional\n\nKey functionality\n-----------------\n\n* Pilots design ✈\n* Multi-group split 🎳\n* Matching of new control group to the existing pilot 🎏\n* Getting the experiments result evaluation as p-value, point estimate of effect and confidence interval 🎞\n* Experiments acceleration 🎢\n\n.. documentation\n\nDocumentation\n-------------\n\nFor more details, see the `Documentation <https://ambrosia.readthedocs.io/>`_ \nand `Tutorials <https://github.com/MobileTeleSystems/Ambrosia/tree/main/examples>`_.\n\n.. install\n\nInstallation\n------------\n\nStable version is released on every tag to ``main`` branch. \n\n.. code:: bash\n    \n    pip install ambrosia \n\n**Ambrosia requires Python 3.7+**\n\n.. usage\n\nUsage\n-----\n\nDesigner \n~~~~~~~~\n\n.. code:: python\n\n    from ambrosia.designer import Designer\n    designer = Designer(dataframe=df, effects=1.2, metrics='portfel_clc') # 20% effect, and loaded data frame df\n    designer.run('size') \n\n\nSplitter\n~~~~~~~~\n\n.. code:: python\n\n    from ambrosia.splitter import Splitter\n    splitter = Splitter(dataframe=df, id_column='id') # loaded data frame df with column with id - 'id'\n    splitter.run(groups_size=500, method='simple') \n\n\nTester \n~~~~~~\n\n.. code:: python\n\n    from ambrosia.tester import Tester\n    tester = Tester(dataframe=df, column_groups='group') # loaded data frame df with groups info 'group'\n    tester.run(metrics='retention', method='theory', criterion='ttest')\n\n.. develop\n\nDevelopment\n-----------\n\nTo install all requirements run\n\n.. code:: bash\n\n    make install\n\nYou must have ``python3`` and ``poetry`` installed.\n\nFor autoformatting run\n\n.. code:: bash\n\n    make autoformat\n\nFor linters check run\n\n.. code:: bash\n\n    make lint\n\nFor tests run\n\n.. code:: bash\n\n    make test\n\nFor coverage run\n\n.. code:: bash\n\n    make coverage\n\nTo remove virtual environment run\n\n.. code:: bash\n\n    make clean\n\n.. contributors\n\nCommunication\n-------------\n\n**Developers and evangelists**:\n\n* `Bayramkulov Aslan <https://github.com/aslanbm>`_\n* `Khakimov Artem <https://github.com/xandaau>`_\n* `Vasin Artem <https://github.com/VictorFromChoback>`_\n",
+    'long_description': ".. shields start\n\nAmbrosia\n========\n\n|PyPI| |PyPI License| |ReadTheDocs| |Tests| |Coverage| |Black| |Python Versions| |Telegram Channel|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/ambrosia\n    :target: https://pypi.org/project/ambrosia\n.. |PyPI License| image:: https://img.shields.io/pypi/l/ambrosia.svg\n    :target: https://github.com/MobileTeleSystems/Ambrosia/blob/main/LICENSE\n.. |ReadTheDocs| image:: https://img.shields.io/readthedocs/ambrosia.svg\n    :target: https://ambrosia.readthedocs.io\n.. |Tests| image:: https://img.shields.io/github/actions/workflow/status/MobileTeleSystems/Ambrosia/test.yaml?branch=main\n    :target: https://github.com/MobileTeleSystems/Ambrosia/actions/workflows/test.yaml?query=branch%3Amain+\n.. |Coverage| image:: https://codecov.io/gh/MobileTeleSystems/Ambrosia/branch/main/graph/badge.svg\n    :target: https://codecov.io/gh/MobileTeleSystems/Ambrosia\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/ambrosia.svg\n    :target: https://pypi.org/project/ambrosia  \n.. |Telegram Channel| image:: https://img.shields.io/badge/telegram-Ambrosia-blueviolet.svg?logo=telegram\n    :target: https://t.me/+Tkt43TNUUSAxNWNi\n\n.. shields end\n\n.. image:: https://raw.githubusercontent.com/MobileTeleSystems/Ambrosia/main/docs/source/_static/ambrosia.png\n   :height: 320 px\n   :width: 320 px\n   :align: center\n\n.. title\n\n*Ambrosia* is a Python library for A/B tests design, split and effect measurement. \nIt provides rich set of methods for conducting full A/B testing pipeline. \n\nThe project is intended for use in research and production environments \nbased on data in pandas and Spark format.\n\n.. functional\n\nKey functionality\n-----------------\n\n* Pilots design 🛫\n* Multi-group split 🎳\n* Matching of new control group to the existing pilot 🎏\n* Experiments result evaluation as p-value, point estimate of effect and confidence interval 🎞\n* Data preprocessing ✂️\n* Experiments acceleration 🎢\n\n.. documentation\n\nDocumentation\n-------------\n\nFor more details, see the `Documentation <https://ambrosia.readthedocs.io/>`_ \nand `Tutorials <https://github.com/MobileTeleSystems/Ambrosia/tree/main/examples>`_.\n\n.. install\n\nInstallation\n------------\n\nYou can always get the newest *Ambrosia* release using ``pip``.\nStable version is released on every tag to ``main`` branch. \n\n.. code:: bash\n    \n    pip install ambrosia \n\nStarting from version ``0.4.0``, the ability to process PySpark data is optional and can be enabled \nusing ``pip`` extras during the installation.\n\n.. code:: bash\n    \n    pip install ambrosia[pyspark]\n\n.. usage\n\nUsage\n-----\n\nThe main functionality of *Ambrosia* is contained in several core classes and methods, \nwhich are autonomic for each stage of an experiment and have very intuitive interface. \n\n|\n\nBelow is a brief overview example of using a set of three classes to conduct some simple experiment.\n\n**Designer**\n\n.. code:: python\n\n    from ambrosia.designer import Designer\n    designer = Designer(dataframe=df, effects=1.2, metrics='portfel_clc') # 20% effect, and loaded data frame df\n    designer.run('size') \n\n\n**Splitter**\n\n.. code:: python\n\n    from ambrosia.splitter import Splitter\n    splitter = Splitter(dataframe=df, id_column='id') # loaded data frame df with column with id - 'id'\n    splitter.run(groups_size=500, method='simple') \n\n\n**Tester**\n\n.. code:: python\n\n    from ambrosia.tester import Tester\n    tester = Tester(dataframe=df, column_groups='group') # loaded data frame df with groups info 'group'\n    tester.run(metrics='retention', method='theory', criterion='ttest')\n\n.. develop\n\nDevelopment\n-----------\n\nTo install all requirements run\n\n.. code:: bash\n\n    make install\n\nYou must have ``python3`` and ``poetry`` installed.\n\nFor autoformatting run\n\n.. code:: bash\n\n    make autoformat\n\nFor linters check run\n\n.. code:: bash\n\n    make lint\n\nFor tests run\n\n.. code:: bash\n\n    make test\n\nFor coverage run\n\n.. code:: bash\n\n    make coverage\n\nTo remove virtual environment run\n\n.. code:: bash\n\n    make clean\n\n.. contributors\n\nAuthors\n-------\n\n**Developers and evangelists**:\n\n* `Bayramkulov Aslan <https://github.com/aslanbm>`_\n* `Khakimov Artem <https://github.com/xandaau>`_\n* `Vasin Artem <https://github.com/VictorFromChoback>`_\n",
     'author': 'Aslan Bayramkulov',
     'author_email': 'aslan.bayramkulov96@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MobileTeleSystems/Ambrosia',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.7.2,<3.11.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ambrosia-0.3.0/PKG-INFO` & `ambrosia-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambrosia
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for working with A/B tests.
 Home-page: https://github.com/MobileTeleSystems/Ambrosia
 License: Apache-2.0
 Keywords: ambrosia,ab testing,split testing,experiment design,groups split
 Author: Aslan Bayramkulov
 Author-email: aslan.bayramkulov96@gmail.com
 Requires-Python: >=3.7.2,<3.11.0
@@ -22,23 +22,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: spark
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: catboost (>=1.0.4,<2.0.0)
 Requires-Dist: hyperopt (>=0.2.7,<0.3.0)
 Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0)
 Requires-Dist: nmslib (>=2.0.4,<3.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: pandas (>=0.25.3,<2.0.0)
-Requires-Dist: pyspark (>=3.2,<4.0)
+Requires-Dist: pyspark (>=3.2,<4.0) ; extra == "spark"
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (>=1.6.3,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.0)
 Requires-Dist: tqdm (>=4.27.0,<5.0.0)
 Project-URL: Documentation, https://ambrosia.readthedocs.io
 Project-URL: Repository, https://github.com/MobileTeleSystems/Ambrosia
 Description-Content-Type: text/x-rst
@@ -72,43 +73,30 @@
 .. image:: https://raw.githubusercontent.com/MobileTeleSystems/Ambrosia/main/docs/source/_static/ambrosia.png
    :height: 320 px
    :width: 320 px
    :align: center
 
 .. title
 
-**Ambrosia** is a Python library for A/B tests design, split and effect 
-measurement. It provides rich set of methods for conducting full 
-A/B test pipeline. 
-
-An experiment design stage is performed using metrics historical data 
-which could be processed in both forms of pandas and spark dataframes 
-with either theoretical or empirical approach. 
-
-Group split methods support different strategies and multi-group split, 
-which allows to quickly create control and test groups of interest. 
-
-Final effect measurement stage is conducted via testing tools that 
-are able to return relative and absolute effects and construct corresponding 
-confidence intervalsfor continious and binary variables. 
-Testing tools as well as design ones support significant number of 
-statistical criteria, like t-test, non-parametric, and bootstrap. 
+*Ambrosia* is a Python library for A/B tests design, split and effect measurement. 
+It provides rich set of methods for conducting full A/B testing pipeline. 
 
-For additional A/B tests support library provides features and tools 
-for data preproccesing and experiment acceleration.
+The project is intended for use in research and production environments 
+based on data in pandas and Spark format.
 
 .. functional
 
 Key functionality
 -----------------
 
-* Pilots design ✈
+* Pilots design 🛫
 * Multi-group split 🎳
 * Matching of new control group to the existing pilot 🎏
-* Getting the experiments result evaluation as p-value, point estimate of effect and confidence interval 🎞
+* Experiments result evaluation as p-value, point estimate of effect and confidence interval 🎞
+* Data preprocessing ✂️
 * Experiments acceleration 🎢
 
 .. documentation
 
 Documentation
 -------------
 
@@ -116,49 +104,59 @@
 and `Tutorials <https://github.com/MobileTeleSystems/Ambrosia/tree/main/examples>`_.
 
 .. install
 
 Installation
 ------------
 
+You can always get the newest *Ambrosia* release using ``pip``.
 Stable version is released on every tag to ``main`` branch. 
 
 .. code:: bash
     
     pip install ambrosia 
 
-**Ambrosia requires Python 3.7+**
+Starting from version ``0.4.0``, the ability to process PySpark data is optional and can be enabled 
+using ``pip`` extras during the installation.
+
+.. code:: bash
+    
+    pip install ambrosia[pyspark]
 
 .. usage
 
 Usage
 -----
 
-Designer 
-~~~~~~~~
+The main functionality of *Ambrosia* is contained in several core classes and methods, 
+which are autonomic for each stage of an experiment and have very intuitive interface. 
+
+|
+
+Below is a brief overview example of using a set of three classes to conduct some simple experiment.
+
+**Designer**
 
 .. code:: python
 
     from ambrosia.designer import Designer
     designer = Designer(dataframe=df, effects=1.2, metrics='portfel_clc') # 20% effect, and loaded data frame df
     designer.run('size') 
 
 
-Splitter
-~~~~~~~~
+**Splitter**
 
 .. code:: python
 
     from ambrosia.splitter import Splitter
     splitter = Splitter(dataframe=df, id_column='id') # loaded data frame df with column with id - 'id'
     splitter.run(groups_size=500, method='simple') 
 
 
-Tester 
-~~~~~~
+**Tester**
 
 .. code:: python
 
     from ambrosia.tester import Tester
     tester = Tester(dataframe=df, column_groups='group') # loaded data frame df with groups info 'group'
     tester.run(metrics='retention', method='theory', criterion='ttest')
 
@@ -203,16 +201,16 @@
 
 .. code:: bash
 
     make clean
 
 .. contributors
 
-Communication
--------------
+Authors
+-------
 
 **Developers and evangelists**:
 
 * `Bayramkulov Aslan <https://github.com/aslanbm>`_
 * `Khakimov Artem <https://github.com/xandaau>`_
 * `Vasin Artem <https://github.com/VictorFromChoback>`_
```

