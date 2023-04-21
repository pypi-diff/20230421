# Comparing `tmp/fold_core-0.1.2.tar.gz` & `tmp/fold_core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fold_core-0.1.2.tar", max compression
+gzip compressed data, was "fold_core-0.1.3.tar", max compression
```

## Comparing `fold_core-0.1.2.tar` & `fold_core-0.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3870 2023-04-20 10:47:50.852017 fold_core-0.1.2/LICENSE
--rw-r--r--   0        0        0    10111 2023-04-20 10:47:50.852017 fold_core-0.1.2/README.md
--rw-r--r--   0        0        0     3818 2023-04-20 10:47:50.892019 fold_core-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      474 2023-04-20 10:47:50.892019 fold_core-0.1.2/src/fold/__init__.py
--rw-r--r--   0        0        0     5273 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/base.py
--rw-r--r--   0        0        0      529 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/__init__.py
--rw-r--r--   0        0        0    10261 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/columns.py
--rw-r--r--   0        0        0     1577 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/common.py
--rw-r--r--   0        0        0     6272 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/concat.py
--rw-r--r--   0        0        0     2226 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/ensemble.py
--rw-r--r--   0        0        0     6359 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/metalabeling.py
--rw-r--r--   0        0        0     4760 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/residual.py
--rw-r--r--   0        0        0     3261 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/sample.py
--rw-r--r--   0        0        0     2064 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/select.py
--rw-r--r--   0        0        0     4545 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/composites/target.py
--rw-r--r--   0        0        0      345 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backend/__init__.py
--rw-r--r--   0        0        0     2408 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backend/ray.py
--rw-r--r--   0        0        0     1931 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backend/sequential.py
--rw-r--r--   0        0        0     3198 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/backtesting.py
--rw-r--r--   0        0        0      590 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/checks.py
--rw-r--r--   0        0        0     9922 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/common.py
--rw-r--r--   0        0        0     2109 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/convenience.py
--rw-r--r--   0        0        0     7138 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/encase.py
--rw-r--r--   0        0        0     2993 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/memory.py
--rw-r--r--   0        0        0     5735 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/training.py
--rw-r--r--   0        0        0     1845 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/loop/types.py
--rw-r--r--   0        0        0      381 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/__init__.py
--rw-r--r--   0        0        0     3212 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/base.py
--rw-r--r--   0        0        0     1926 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/baseline.py
--rw-r--r--   0        0        0     4349 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/dummy.py
--rw-r--r--   0        0        0     2187 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/random.py
--rw-r--r--   0        0        0     4310 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/models/sklearn.py
--rw-r--r--   0        0        0        0 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/py.typed
--rw-r--r--   0        0        0     6724 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/splitters.py
--rw-r--r--   0        0        0      928 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/__init__.py
--rw-r--r--   0        0        0     6034 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/columns.py
--rw-r--r--   0        0        0     8593 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/date.py
--rw-r--r--   0        0        0     4264 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/dev.py
--rw-r--r--   0        0        0     2906 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/difference.py
--rw-r--r--   0        0        0      798 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/function.py
--rw-r--r--   0        0        0     6569 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/holidays.py
--rw-r--r--   0        0        0     5675 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/lags.py
--rw-r--r--   0        0        0     7573 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/math.py
--rw-r--r--   0        0        0     3734 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/sklearn.py
--rw-r--r--   0        0        0      887 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/update.py
--rw-r--r--   0        0        0     4414 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/transformations/window.py
--rw-r--r--   0        0        0     2171 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/checks.py
--rw-r--r--   0        0        0     2240 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/dataset.py
--rw-r--r--   0        0        0     1591 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/list.py
--rw-r--r--   0        0        0     2955 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/tests.py
--rw-r--r--   0        0        0     1716 2023-04-20 10:47:50.896019 fold_core-0.1.2/src/fold/utils/trim.py
--rw-r--r--   0        0        0    12906 1970-01-01 00:00:00.000000 fold_core-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3870 2023-04-21 15:22:18.540089 fold_core-0.1.3/LICENSE
+-rw-r--r--   0        0        0    10364 2023-04-21 15:22:18.540089 fold_core-0.1.3/README.md
+-rw-r--r--   0        0        0     3820 2023-04-21 15:22:18.580089 fold_core-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      474 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/__init__.py
+-rw-r--r--   0        0        0     5273 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/base.py
+-rw-r--r--   0        0        0      529 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/__init__.py
+-rw-r--r--   0        0        0    10261 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/columns.py
+-rw-r--r--   0        0        0     1577 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/common.py
+-rw-r--r--   0        0        0     6272 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/concat.py
+-rw-r--r--   0        0        0     2226 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/ensemble.py
+-rw-r--r--   0        0        0     6359 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/metalabeling.py
+-rw-r--r--   0        0        0     4760 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/residual.py
+-rw-r--r--   0        0        0     3261 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/sample.py
+-rw-r--r--   0        0        0     2064 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/select.py
+-rw-r--r--   0        0        0     4545 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/composites/target.py
+-rw-r--r--   0        0        0      345 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/__init__.py
+-rw-r--r--   0        0        0     1355 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backend/__init__.py
+-rw-r--r--   0        0        0     2408 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backend/ray.py
+-rw-r--r--   0        0        0     1931 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backend/sequential.py
+-rw-r--r--   0        0        0     3198 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/backtesting.py
+-rw-r--r--   0        0        0      590 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/checks.py
+-rw-r--r--   0        0        0     9922 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/common.py
+-rw-r--r--   0        0        0     2109 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/convenience.py
+-rw-r--r--   0        0        0     7138 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/encase.py
+-rw-r--r--   0        0        0     2993 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/memory.py
+-rw-r--r--   0        0        0     5735 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/training.py
+-rw-r--r--   0        0        0     1845 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/loop/types.py
+-rw-r--r--   0        0        0      381 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/base.py
+-rw-r--r--   0        0        0     1926 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/baseline.py
+-rw-r--r--   0        0        0     4349 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/dummy.py
+-rw-r--r--   0        0        0     2187 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/random.py
+-rw-r--r--   0        0        0     4310 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/models/sklearn.py
+-rw-r--r--   0        0        0        0 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/py.typed
+-rw-r--r--   0        0        0     6724 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/splitters.py
+-rw-r--r--   0        0        0      928 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/__init__.py
+-rw-r--r--   0        0        0     6034 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/columns.py
+-rw-r--r--   0        0        0     8593 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/date.py
+-rw-r--r--   0        0        0     4264 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/dev.py
+-rw-r--r--   0        0        0     2906 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/difference.py
+-rw-r--r--   0        0        0      798 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/function.py
+-rw-r--r--   0        0        0     6569 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/holidays.py
+-rw-r--r--   0        0        0     5675 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/lags.py
+-rw-r--r--   0        0        0     7573 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/math.py
+-rw-r--r--   0        0        0     3734 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/sklearn.py
+-rw-r--r--   0        0        0      887 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/update.py
+-rw-r--r--   0        0        0     4414 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/transformations/window.py
+-rw-r--r--   0        0        0     2171 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/checks.py
+-rw-r--r--   0        0        0     2240 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/dataset.py
+-rw-r--r--   0        0        0     1591 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/list.py
+-rw-r--r--   0        0        0     2955 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/tests.py
+-rw-r--r--   0        0        0     1716 2023-04-21 15:22:18.580089 fold_core-0.1.3/src/fold/utils/trim.py
+-rw-r--r--   0        0        0    13161 1970-01-01 00:00:00.000000 fold_core-0.1.3/PKG-INFO
```

### Comparing `fold_core-0.1.2/LICENSE` & `fold_core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/README.md` & `fold_core-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,35 +10,46 @@
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/fold/">
     <img src="https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/logo.svg" alt="Logo" width="90" >
   </a>
-<h3 align="center"><b>FOLD</b><br> <i>(/fold/)</i></h3>
+<h3 align="center"><b>FOLD</b><br></h3>
   <p align="center">
-    <b>A <a href="https://dream-faster.github.io/fold/concepts/continuous-validation/">Time Series Continuous Validation</a> library that lets you build, deploy and update Composite Models easily. An order of magnitude speed-up, combined with flexibility and rigour.</b><br>
+    Fast <b>Adaptive ML </b> Engine
     <br/>
     <a href="https://dream-faster.github.io/fold/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 <!-- INTRO -->
 
-![Fold's main features](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/main_features.svg)
+![Adaptive Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/main_diagram.svg)
+
+The<b> <a href="https://dream-faster.github.io/fold/concepts/adaptive-ml/">Adaptive ML Engine</a></b> that lets you <b>build</b>, <b>deploy and update</b> Models easily. An order of magnitude speed-up, combined with flexibility and rigour.</b>
+<br/>
+
 
-- Composite Models with Continuous Validation - [What does that mean?](https://dream-faster.github.io/fold/concepts/continuous-validation/)
-- Distributed computing - [Why is this important?](#Fold-is-different)
-- Update deployed models (coming in May) - [Why is this important?](#Fold-is-different)
 
 ![Fold works with many third party libraries](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/third_party.svg)
 
 <!-- GETTING STARTED -->
 
+## Main Features
+
+![Fold's main features](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/main_features.svg)
+
+- 10x faster Adaptive Backtesting - [What does that mean?](https://dream-faster.github.io/fold/concepts/adaptive-ml/)
+- Composite Models made Adaptive - [What does that mean?](https://dream-faster.github.io/fold/concepts/adaptive-ml/)
+- Distributed computing - [Why is this important?](#Fold-is-different)
+- Update deployed models (coming in May) - [Why is this important?](#Fold-is-different)
+
+
 ## Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
 - Install from pypi:
   ```
   pip install fold-core
@@ -75,15 +86,15 @@
 
 Thinking of using `fold`? We'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/nowcasting/consultation)!
 
 (If you install `krisi` by running `pip install krisi` you get an extended report back, rather than a single metric.)
 
 ## Fold is different
 
-- Time Series Continuous Validation at lightning speed.<br/>
+- Adaptive Models and Backtesting at lightning speed.<br/>
   <span style="color:orange;">**→ fold allows to simulate and evaluate your models like they would have performed, in reality/when deployed, with clever use of paralellization and design.**</span>
 
 - Create composite models: ensembles, hybrids, stacking pipelines, easily.<br/>
   <span style="color:orange;">**→ Underutilized, but [the easiest, fastest way to increase performance of your Time Series models.](https://linkinghub.elsevier.com/retrieve/pii/S0169207022001480)**
   </span>
 
 - Built with Distributed Computing in mind.<br/>
@@ -176,20 +187,20 @@
 - Use any scikit-learn/tabular model natively!
 - Use any univariate or sequence models (wrappers provided in [fold-wrappers](https://github.com/dream-faster/fold-wrappers)).
 - Use any Deep Learning Time Series models (wrappers provided in [fold-wrappers](https://github.com/dream-faster/fold-wrappers)).
 - Super easy syntax!
 - Probabilistic foreacasts (currently, for Classification, full support coming in April).
 - Hyperparemeter optimization / Model selection. (coming in early April!)
 
-## What is Continuous Validation?
+## What is Adaptive Backtesting?
 
-![Continous Validation](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/technical_diagrams/continous_validation.svg)
+![Adaptive Backtesting](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/technical_diagrams/continous_validation.svg)
 
-It's Time Series Cross-Validation, plus: Inside a test window, and during deployment, fold provides a way for models to update their parameters or access the last value.
-[Learn more](https://dream-faster.github.io/fold/concepts/continuous-validation/)
+It's like classical Backtesting / Time Series Cross-Validation, plus: Inside a test window, and during deployment, fold provides a way for models to update their parameters or access the last value.
+[Learn more](https://dream-faster.github.io/fold/concepts/adaptive-ml/)
 
 ## Our Open-core Time Series Toolkit
 
 [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
 [![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
 [![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
 [![Fold/Wrappers](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
```

#### html2text {}

```diff
@@ -1,43 +1,47 @@
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
-                                 (/fold/) ****
-  A Time_Series_Continuous_Validation library that lets you build, deploy and
- update Composite Models easily. An order of magnitude speed-up, combined with
-                            flexibility and rigour.
-
+                                      ****
+                           Fast Adaptive ML Engine
                               Explore_the_docs_Â»
 
- ![Fold's main features](https://raw.githubusercontent.com/dream-faster/fold/
-main/docs/images/overview_diagrams/main_features.svg) - Composite Models with
-Continuous Validation - [What does that mean?](https://dream-faster.github.io/
-fold/concepts/continuous-validation/) - Distributed computing - [Why is this
-important?](#Fold-is-different) - Update deployed models (coming in May) - [Why
-is this important?](#Fold-is-different) ![Fold works with many third party
-libraries](https://raw.githubusercontent.com/dream-faster/fold/main/docs/
-images/overview_diagrams/third_party.svg)  ## Installation - Prerequisites:
-`python >= 3.7` and `pip` - Install from pypi: ``` pip install fold-core ``` ##
-Quickstart You can quickly train your chosen models and get predictions by
-running: ```py from sklearn.ensemble import RandomForestRegressor from
-statsforecast.models import ARIMA from fold import ExpandingWindowSplitter,
-train_evaluate from fold.composites import Ensemble from fold.transformations
-import OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset
-X, y = get_preprocessed_dataset( "weather/historical_hourly_la",
+ ![Adaptive Models](https://raw.githubusercontent.com/dream-faster/fold/main/
+docs/images/overview_diagrams/main_diagram.svg) TheAdaptive_ML_Engine that lets
+you build, deploy and update Models easily. An order of magnitude speed-up,
+combined with flexibility and rigour.
+
+![Fold works with many third party libraries](https://
+raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
+third_party.svg)  ## Main Features ![Fold's main features](https://
+raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
+main_features.svg) - 10x faster Adaptive Backtesting - [What does that mean?]
+(https://dream-faster.github.io/fold/concepts/adaptive-ml/) - Composite Models
+made Adaptive - [What does that mean?](https://dream-faster.github.io/fold/
+concepts/adaptive-ml/) - Distributed computing - [Why is this important?]
+(#Fold-is-different) - Update deployed models (coming in May) - [Why is this
+important?](#Fold-is-different) ## Installation - Prerequisites: `python >=
+3.7` and `pip` - Install from pypi: ``` pip install fold-core ``` ## Quickstart
+You can quickly train your chosen models and get predictions by running: ```py
+from sklearn.ensemble import RandomForestRegressor from statsforecast.models
+import ARIMA from fold import ExpandingWindowSplitter, train_evaluate from
+fold.composites import Ensemble from fold.transformations import
+OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset X, y =
+get_preprocessed_dataset( "weather/historical_hourly_la",
 target_col="temperature", shorten=1000 ) pipeline = [ Ensemble(
 [ RandomForestRegressor(), ARIMA(order=(1, 1, 0)), ] ), OnlyPredictions(), ]
 splitter = ExpandingWindowSplitter(initial_train_window=0.2, step=0.2)
 scorecard, prediction, trained_pipelines = train_evaluate(pipeline, X, y,
 splitter) ``` Thinking of using `fold`? We'd love to hear about your use case
 and help, [please book a free 30-min call with us](https://calendly.com/
 nowcasting/consultation)! (If you install `krisi` by running `pip install
 krisi` you get an extended report back, rather than a single metric.) ## Fold
-is different - Time Series Continuous Validation at lightning speed.
+is different - Adaptive Models and Backtesting at lightning speed.
 **â fold allows to simulate and evaluate your models like they would have
 performed, in reality/when deployed, with clever use of paralellization and
 design.** - Create composite models: ensembles, hybrids, stacking pipelines,
 easily.
 **â Underutilized, but [the easiest, fastest way to increase performance of
 your Time Series models.](https://linkinghub.elsevier.com/retrieve/pii/
 S0169207022001480)**  - Built with Distributed Computing in mind.
@@ -63,29 +67,30 @@
 and Mini-batch learning. - Feature selection and other transformations on an
 expanding/rolling window basis - Use any scikit-learn/tabular model natively! -
 Use any univariate or sequence models (wrappers provided in [fold-wrappers]
 (https://github.com/dream-faster/fold-wrappers)). - Use any Deep Learning Time
 Series models (wrappers provided in [fold-wrappers](https://github.com/dream-
 faster/fold-wrappers)). - Super easy syntax! - Probabilistic foreacasts
 (currently, for Classification, full support coming in April). - Hyperparemeter
-optimization / Model selection. (coming in early April!) ## What is Continuous
-Validation? ![Continous Validation](https://raw.githubusercontent.com/dream-
+optimization / Model selection. (coming in early April!) ## What is Adaptive
+Backtesting? ![Adaptive Backtesting](https://raw.githubusercontent.com/dream-
 faster/fold/main/docs/images/technical_diagrams/continous_validation.svg) It's
-Time Series Cross-Validation, plus: Inside a test window, and during
-deployment, fold provides a way for models to update their parameters or access
-the last value. [Learn more](https://dream-faster.github.io/fold/concepts/
-continuous-validation/) ## Our Open-core Time Series Toolkit [![Krisi](https://
-raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
-dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi) [![Fold]
-(https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
-overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-
-faster/fold) [![Fold/Models](https://raw.githubusercontent.com/dream-faster/
-fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)]
-(https://github.com/dream-faster/fold-models) [![Fold/Wrappers](https://
-raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
+like classical Backtesting / Time Series Cross-Validation, plus: Inside a test
+window, and during deployment, fold provides a way for models to update their
+parameters or access the last value. [Learn more](https://dream-
+faster.github.io/fold/concepts/adaptive-ml/) ## Our Open-core Time Series
+Toolkit [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/
+docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://
+github.com/dream-faster/krisi) [![Fold](https://raw.githubusercontent.com/
+dream-faster/fold/main/docs/images/overview_diagrams/
+dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold) [![Fold/
+Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
+overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/
+dream-faster/fold-models) [![Fold/Wrappers](https://raw.githubusercontent.com/
+dream-faster/fold/main/docs/images/overview_diagrams/
 dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-
 wrappers) If you want to try them out, we'd love to hear about your use case
 and help, [please book a free 30-min call with us](https://calendly.com/
 nowcasting/consultation)! [Explore our Commercial License options here](https:/
 /dream-faster.github.io/fold/product/pricing) ## Contribution Join our [Discord
 Community] for live discussion! Submit an issue or reach out to us on info at
 dream-faster.ai for any inquiries. ## Licence & Usage We want to **bring much-
```

### Comparing `fold_core-0.1.2/pyproject.toml` & `fold_core-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fold-core"
 packages = [
     { include="fold", from="./src" },
 ]
-version = "0.1.2"
+version = "0.1.3"
 authors = ["Mark Aron Szulyovszky", "Daniel Szemerey" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -48,15 +48,15 @@
 mkdocs-material = {version = ">=9.0.0", optional = true}
 mkdocstrings-python = {version = ">=0.9.0", optional = true}
 mkdocs-include-markdown-plugin = {version = ">=4.0", optional = true}
 mkdocs-autorefs = {version = ">=0.4", optional = true}
 mkdocs-jupyter = {version = ">=0.22", optional = true}
 image = {version = ">=1.5.33", optional = true}
 mkdocs-gallery = {version = ">=0.7", optional = true}
-mkdocs-glightbox = {version = ">=0.3", optional = true}
+mkdocs-glightbox = {version = "<=0.3.2", optional = true}
 ray = {version = ">=1.4", optional = true}
 
 [project.urls]
 Documentation = "https://dream-faster.github.io/fold"
 Issues = "https://github.com/dream-faster/fold/issues"
 Source = "https://github.com/dream-faster/fold"
 
@@ -124,15 +124,15 @@
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `fold_core-0.1.2/src/fold/base.py` & `fold_core-0.1.3/src/fold/base.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/__init__.py` & `fold_core-0.1.3/src/fold/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/columns.py` & `fold_core-0.1.3/src/fold/composites/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/common.py` & `fold_core-0.1.3/src/fold/composites/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/concat.py` & `fold_core-0.1.3/src/fold/composites/concat.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/ensemble.py` & `fold_core-0.1.3/src/fold/composites/ensemble.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/metalabeling.py` & `fold_core-0.1.3/src/fold/composites/metalabeling.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/residual.py` & `fold_core-0.1.3/src/fold/composites/residual.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/sample.py` & `fold_core-0.1.3/src/fold/composites/sample.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/select.py` & `fold_core-0.1.3/src/fold/composites/select.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/composites/target.py` & `fold_core-0.1.3/src/fold/composites/target.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/backend/__init__.py` & `fold_core-0.1.3/src/fold/loop/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/backend/ray.py` & `fold_core-0.1.3/src/fold/loop/backend/ray.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/backend/sequential.py` & `fold_core-0.1.3/src/fold/loop/backend/sequential.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/backtesting.py` & `fold_core-0.1.3/src/fold/loop/backtesting.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/checks.py` & `fold_core-0.1.3/src/fold/loop/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/common.py` & `fold_core-0.1.3/src/fold/loop/common.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/convenience.py` & `fold_core-0.1.3/src/fold/loop/convenience.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/encase.py` & `fold_core-0.1.3/src/fold/loop/encase.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/memory.py` & `fold_core-0.1.3/src/fold/loop/memory.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/training.py` & `fold_core-0.1.3/src/fold/loop/training.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/loop/types.py` & `fold_core-0.1.3/src/fold/loop/types.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/models/base.py` & `fold_core-0.1.3/src/fold/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if in_sample:
             return postpostprocess_prediction(
                 self.predict_in_sample(X, self._state.memory_y.shift(1)), self.name
             )
         else:
             return postpostprocess_prediction(
                 self.predict(
-                    X[-self.properties.memory_size + 1 : None],
+                    X[-(self.properties.memory_size + 1) : None],
                     pd.Series(
                         np.concatenate(
                             [
                                 np.ones((1,)) * np.nan,
                                 self._state.memory_y[
                                     -self.properties.memory_size : None
                                 ],
```

### Comparing `fold_core-0.1.2/src/fold/models/baseline.py` & `fold_core-0.1.3/src/fold/models/baseline.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/models/dummy.py` & `fold_core-0.1.3/src/fold/models/dummy.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/models/random.py` & `fold_core-0.1.3/src/fold/models/random.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/models/sklearn.py` & `fold_core-0.1.3/src/fold/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/splitters.py` & `fold_core-0.1.3/src/fold/splitters.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/__init__.py` & `fold_core-0.1.3/src/fold/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/columns.py` & `fold_core-0.1.3/src/fold/transformations/columns.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/date.py` & `fold_core-0.1.3/src/fold/transformations/date.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/dev.py` & `fold_core-0.1.3/src/fold/transformations/dev.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/difference.py` & `fold_core-0.1.3/src/fold/transformations/difference.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/function.py` & `fold_core-0.1.3/src/fold/transformations/function.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/holidays.py` & `fold_core-0.1.3/src/fold/transformations/holidays.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/lags.py` & `fold_core-0.1.3/src/fold/transformations/lags.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/math.py` & `fold_core-0.1.3/src/fold/transformations/math.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/sklearn.py` & `fold_core-0.1.3/src/fold/transformations/sklearn.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/update.py` & `fold_core-0.1.3/src/fold/transformations/update.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/transformations/window.py` & `fold_core-0.1.3/src/fold/transformations/window.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/utils/checks.py` & `fold_core-0.1.3/src/fold/utils/checks.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/utils/dataset.py` & `fold_core-0.1.3/src/fold/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/utils/list.py` & `fold_core-0.1.3/src/fold/utils/list.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/utils/tests.py` & `fold_core-0.1.3/src/fold/utils/tests.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/src/fold/utils/trim.py` & `fold_core-0.1.3/src/fold/utils/trim.py`

 * *Files identical despite different names*

### Comparing `fold_core-0.1.2/PKG-INFO` & `fold_core-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fold-core
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Time Series Cross-Validation library that lets you build, deploy and update composite models easily. An order of magnitude speed-up, combined with flexibility and rigour.
 License: Proprietary
 Keywords: time-series,machine-learning,forecasting,forecast,nowcast,models,time-series-regression,time-series-classification,financial-machine-learning
 Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
@@ -35,15 +35,15 @@
 Requires-Dist: imbalanced-learn (>=0.7.0) ; extra == "tests"
 Requires-Dist: isort (>=5.10.1,<5.11.0) ; extra == "quality"
 Requires-Dist: iteration_utilities (>=0.11)
 Requires-Dist: krisi (>=0.0.8,<0.1.0) ; extra == "extras"
 Requires-Dist: mkdocs (>=1.2)
 Requires-Dist: mkdocs-autorefs (>=0.4) ; extra == "docs"
 Requires-Dist: mkdocs-gallery (>=0.7) ; extra == "docs"
-Requires-Dist: mkdocs-glightbox (>=0.3) ; extra == "docs"
+Requires-Dist: mkdocs-glightbox (<=0.3.2) ; extra == "docs"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra == "docs"
 Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs"
 Requires-Dist: mkdocs-material (>=9.0.0) ; extra == "docs"
 Requires-Dist: mkdocstrings-python (>=0.9.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.16)
 Requires-Dist: pandas (>=1.2)
 Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra == "quality"
@@ -66,35 +66,46 @@
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://dream-faster.github.io/fold/">
     <img src="https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/logo.svg" alt="Logo" width="90" >
   </a>
-<h3 align="center"><b>FOLD</b><br> <i>(/fold/)</i></h3>
+<h3 align="center"><b>FOLD</b><br></h3>
   <p align="center">
-    <b>A <a href="https://dream-faster.github.io/fold/concepts/continuous-validation/">Time Series Continuous Validation</a> library that lets you build, deploy and update Composite Models easily. An order of magnitude speed-up, combined with flexibility and rigour.</b><br>
+    Fast <b>Adaptive ML </b> Engine
     <br/>
     <a href="https://dream-faster.github.io/fold/"><strong>Explore the docs »</strong></a>
   </p>
 </div>
 <br />
 
 <!-- INTRO -->
 
-![Fold's main features](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/main_features.svg)
+![Adaptive Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/main_diagram.svg)
+
+The<b> <a href="https://dream-faster.github.io/fold/concepts/adaptive-ml/">Adaptive ML Engine</a></b> that lets you <b>build</b>, <b>deploy and update</b> Models easily. An order of magnitude speed-up, combined with flexibility and rigour.</b>
+<br/>
+
 
-- Composite Models with Continuous Validation - [What does that mean?](https://dream-faster.github.io/fold/concepts/continuous-validation/)
-- Distributed computing - [Why is this important?](#Fold-is-different)
-- Update deployed models (coming in May) - [Why is this important?](#Fold-is-different)
 
 ![Fold works with many third party libraries](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/third_party.svg)
 
 <!-- GETTING STARTED -->
 
+## Main Features
+
+![Fold's main features](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/main_features.svg)
+
+- 10x faster Adaptive Backtesting - [What does that mean?](https://dream-faster.github.io/fold/concepts/adaptive-ml/)
+- Composite Models made Adaptive - [What does that mean?](https://dream-faster.github.io/fold/concepts/adaptive-ml/)
+- Distributed computing - [Why is this important?](#Fold-is-different)
+- Update deployed models (coming in May) - [Why is this important?](#Fold-is-different)
+
+
 ## Installation
 
 - Prerequisites: `python >= 3.7` and `pip`
 
 - Install from pypi:
   ```
   pip install fold-core
@@ -131,15 +142,15 @@
 
 Thinking of using `fold`? We'd love to hear about your use case and help, [please book a free 30-min call with us](https://calendly.com/nowcasting/consultation)!
 
 (If you install `krisi` by running `pip install krisi` you get an extended report back, rather than a single metric.)
 
 ## Fold is different
 
-- Time Series Continuous Validation at lightning speed.<br/>
+- Adaptive Models and Backtesting at lightning speed.<br/>
   <span style="color:orange;">**→ fold allows to simulate and evaluate your models like they would have performed, in reality/when deployed, with clever use of paralellization and design.**</span>
 
 - Create composite models: ensembles, hybrids, stacking pipelines, easily.<br/>
   <span style="color:orange;">**→ Underutilized, but [the easiest, fastest way to increase performance of your Time Series models.](https://linkinghub.elsevier.com/retrieve/pii/S0169207022001480)**
   </span>
 
 - Built with Distributed Computing in mind.<br/>
@@ -232,20 +243,20 @@
 - Use any scikit-learn/tabular model natively!
 - Use any univariate or sequence models (wrappers provided in [fold-wrappers](https://github.com/dream-faster/fold-wrappers)).
 - Use any Deep Learning Time Series models (wrappers provided in [fold-wrappers](https://github.com/dream-faster/fold-wrappers)).
 - Super easy syntax!
 - Probabilistic foreacasts (currently, for Classification, full support coming in April).
 - Hyperparemeter optimization / Model selection. (coming in early April!)
 
-## What is Continuous Validation?
+## What is Adaptive Backtesting?
 
-![Continous Validation](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/technical_diagrams/continous_validation.svg)
+![Adaptive Backtesting](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/technical_diagrams/continous_validation.svg)
 
-It's Time Series Cross-Validation, plus: Inside a test window, and during deployment, fold provides a way for models to update their parameters or access the last value.
-[Learn more](https://dream-faster.github.io/fold/concepts/continuous-validation/)
+It's like classical Backtesting / Time Series Cross-Validation, plus: Inside a test window, and during deployment, fold provides a way for models to update their parameters or access the last value.
+[Learn more](https://dream-faster.github.io/fold/concepts/adaptive-ml/)
 
 ## Our Open-core Time Series Toolkit
 
 [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi)
 [![Fold](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold)
 [![Fold/Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/dream-faster/fold-models)
 [![Fold/Wrappers](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-wrappers)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fold-core Version: 0.1.2 Summary: A Time Series
+Metadata-Version: 2.1 Name: fold-core Version: 0.1.3 Summary: A Time Series
 Cross-Validation library that lets you build, deploy and update composite
 models easily. An order of magnitude speed-up, combined with flexibility and
 rigour. License: Proprietary Keywords: time-series,machine-
 learning,forecasting,forecast,nowcast,models,time-series-regression,time-
 series-classification,financial-machine-learning Author: Mark Aron Szulyovszky
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: Other/Proprietary License Classifier: Operating
@@ -21,60 +21,64 @@
 extra == "quality" Requires-Dist: flake8 (>=4.0.1,<4.1.0) ; extra == "quality"
 Requires-Dist: holidays (>=0.10) ; extra == "tests" or extra == "extras"
 Requires-Dist: image (>=1.5.33) ; extra == "docs" Requires-Dist: imbalanced-
 learn (>=0.7.0) ; extra == "tests" Requires-Dist: isort (>=5.10.1,<5.11.0) ;
 extra == "quality" Requires-Dist: iteration_utilities (>=0.11) Requires-Dist:
 krisi (>=0.0.8,<0.1.0) ; extra == "extras" Requires-Dist: mkdocs (>=1.2)
 Requires-Dist: mkdocs-autorefs (>=0.4) ; extra == "docs" Requires-Dist: mkdocs-
-gallery (>=0.7) ; extra == "docs" Requires-Dist: mkdocs-glightbox (>=0.3) ;
+gallery (>=0.7) ; extra == "docs" Requires-Dist: mkdocs-glightbox (<=0.3.2) ;
 extra == "docs" Requires-Dist: mkdocs-include-markdown-plugin (>=4.0) ; extra
 == "docs" Requires-Dist: mkdocs-jupyter (>=0.22) ; extra == "docs" Requires-
 Dist: mkdocs-material (>=9.0.0) ; extra == "docs" Requires-Dist: mkdocstrings-
 python (>=0.9.0) ; extra == "docs" Requires-Dist: numpy (>=1.16) Requires-Dist:
 pandas (>=1.2) Requires-Dist: pre-commit (>=2.20.0,<2.21.0) ; extra ==
 "quality" Requires-Dist: pytest (>=7.1.2,<7.2.0) ; extra == "tests" Requires-
 Dist: pytest-cov (>=4.0) ; extra == "tests" Requires-Dist: ray (>=1.4) ; extra
 == "ray" or extra == "extras" Requires-Dist: scikit-learn (>=0.22) Requires-
 Dist: tqdm (>=4.0) Description-Content-Type: text/markdown
       [Docs] [https://codecov.io/gh/dream-faster/fold/branch/main/graph/
 badge.svg?token=Z7I2XSF188] [Tests] [Discord_Community] [Book_a_call_with_us!]
 
                                     [Logo]
                                    **** FOLD
-                                 (/fold/) ****
-  A Time_Series_Continuous_Validation library that lets you build, deploy and
- update Composite Models easily. An order of magnitude speed-up, combined with
-                            flexibility and rigour.
-
+                                      ****
+                           Fast Adaptive ML Engine
                               Explore_the_docs_Â»
 
- ![Fold's main features](https://raw.githubusercontent.com/dream-faster/fold/
-main/docs/images/overview_diagrams/main_features.svg) - Composite Models with
-Continuous Validation - [What does that mean?](https://dream-faster.github.io/
-fold/concepts/continuous-validation/) - Distributed computing - [Why is this
-important?](#Fold-is-different) - Update deployed models (coming in May) - [Why
-is this important?](#Fold-is-different) ![Fold works with many third party
-libraries](https://raw.githubusercontent.com/dream-faster/fold/main/docs/
-images/overview_diagrams/third_party.svg)  ## Installation - Prerequisites:
-`python >= 3.7` and `pip` - Install from pypi: ``` pip install fold-core ``` ##
-Quickstart You can quickly train your chosen models and get predictions by
-running: ```py from sklearn.ensemble import RandomForestRegressor from
-statsforecast.models import ARIMA from fold import ExpandingWindowSplitter,
-train_evaluate from fold.composites import Ensemble from fold.transformations
-import OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset
-X, y = get_preprocessed_dataset( "weather/historical_hourly_la",
+ ![Adaptive Models](https://raw.githubusercontent.com/dream-faster/fold/main/
+docs/images/overview_diagrams/main_diagram.svg) TheAdaptive_ML_Engine that lets
+you build, deploy and update Models easily. An order of magnitude speed-up,
+combined with flexibility and rigour.
+
+![Fold works with many third party libraries](https://
+raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
+third_party.svg)  ## Main Features ![Fold's main features](https://
+raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
+main_features.svg) - 10x faster Adaptive Backtesting - [What does that mean?]
+(https://dream-faster.github.io/fold/concepts/adaptive-ml/) - Composite Models
+made Adaptive - [What does that mean?](https://dream-faster.github.io/fold/
+concepts/adaptive-ml/) - Distributed computing - [Why is this important?]
+(#Fold-is-different) - Update deployed models (coming in May) - [Why is this
+important?](#Fold-is-different) ## Installation - Prerequisites: `python >=
+3.7` and `pip` - Install from pypi: ``` pip install fold-core ``` ## Quickstart
+You can quickly train your chosen models and get predictions by running: ```py
+from sklearn.ensemble import RandomForestRegressor from statsforecast.models
+import ARIMA from fold import ExpandingWindowSplitter, train_evaluate from
+fold.composites import Ensemble from fold.transformations import
+OnlyPredictions from fold.utils.dataset import get_preprocessed_dataset X, y =
+get_preprocessed_dataset( "weather/historical_hourly_la",
 target_col="temperature", shorten=1000 ) pipeline = [ Ensemble(
 [ RandomForestRegressor(), ARIMA(order=(1, 1, 0)), ] ), OnlyPredictions(), ]
 splitter = ExpandingWindowSplitter(initial_train_window=0.2, step=0.2)
 scorecard, prediction, trained_pipelines = train_evaluate(pipeline, X, y,
 splitter) ``` Thinking of using `fold`? We'd love to hear about your use case
 and help, [please book a free 30-min call with us](https://calendly.com/
 nowcasting/consultation)! (If you install `krisi` by running `pip install
 krisi` you get an extended report back, rather than a single metric.) ## Fold
-is different - Time Series Continuous Validation at lightning speed.
+is different - Adaptive Models and Backtesting at lightning speed.
 **â fold allows to simulate and evaluate your models like they would have
 performed, in reality/when deployed, with clever use of paralellization and
 design.** - Create composite models: ensembles, hybrids, stacking pipelines,
 easily.
 **â Underutilized, but [the easiest, fastest way to increase performance of
 your Time Series models.](https://linkinghub.elsevier.com/retrieve/pii/
 S0169207022001480)**  - Built with Distributed Computing in mind.
@@ -100,29 +104,30 @@
 and Mini-batch learning. - Feature selection and other transformations on an
 expanding/rolling window basis - Use any scikit-learn/tabular model natively! -
 Use any univariate or sequence models (wrappers provided in [fold-wrappers]
 (https://github.com/dream-faster/fold-wrappers)). - Use any Deep Learning Time
 Series models (wrappers provided in [fold-wrappers](https://github.com/dream-
 faster/fold-wrappers)). - Super easy syntax! - Probabilistic foreacasts
 (currently, for Classification, full support coming in April). - Hyperparemeter
-optimization / Model selection. (coming in early April!) ## What is Continuous
-Validation? ![Continous Validation](https://raw.githubusercontent.com/dream-
+optimization / Model selection. (coming in early April!) ## What is Adaptive
+Backtesting? ![Adaptive Backtesting](https://raw.githubusercontent.com/dream-
 faster/fold/main/docs/images/technical_diagrams/continous_validation.svg) It's
-Time Series Cross-Validation, plus: Inside a test window, and during
-deployment, fold provides a way for models to update their parameters or access
-the last value. [Learn more](https://dream-faster.github.io/fold/concepts/
-continuous-validation/) ## Our Open-core Time Series Toolkit [![Krisi](https://
-raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
-dream_faster_suite_krisi.svg)](https://github.com/dream-faster/krisi) [![Fold]
-(https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
-overview_diagrams/dream_faster_suite_fold.svg)](https://github.com/dream-
-faster/fold) [![Fold/Models](https://raw.githubusercontent.com/dream-faster/
-fold/main/docs/images/overview_diagrams/dream_faster_suite_fold_models.svg)]
-(https://github.com/dream-faster/fold-models) [![Fold/Wrappers](https://
-raw.githubusercontent.com/dream-faster/fold/main/docs/images/overview_diagrams/
+like classical Backtesting / Time Series Cross-Validation, plus: Inside a test
+window, and during deployment, fold provides a way for models to update their
+parameters or access the last value. [Learn more](https://dream-
+faster.github.io/fold/concepts/adaptive-ml/) ## Our Open-core Time Series
+Toolkit [![Krisi](https://raw.githubusercontent.com/dream-faster/fold/main/
+docs/images/overview_diagrams/dream_faster_suite_krisi.svg)](https://
+github.com/dream-faster/krisi) [![Fold](https://raw.githubusercontent.com/
+dream-faster/fold/main/docs/images/overview_diagrams/
+dream_faster_suite_fold.svg)](https://github.com/dream-faster/fold) [![Fold/
+Models](https://raw.githubusercontent.com/dream-faster/fold/main/docs/images/
+overview_diagrams/dream_faster_suite_fold_models.svg)](https://github.com/
+dream-faster/fold-models) [![Fold/Wrappers](https://raw.githubusercontent.com/
+dream-faster/fold/main/docs/images/overview_diagrams/
 dream_faster_suite_fold_wrappers.svg)](https://github.com/dream-faster/fold-
 wrappers) If you want to try them out, we'd love to hear about your use case
 and help, [please book a free 30-min call with us](https://calendly.com/
 nowcasting/consultation)! [Explore our Commercial License options here](https:/
 /dream-faster.github.io/fold/product/pricing) ## Contribution Join our [Discord
 Community] for live discussion! Submit an issue or reach out to us on info at
 dream-faster.ai for any inquiries. ## Licence & Usage We want to **bring much-
```

