# Comparing `tmp/fal-0.8.4.tar.gz` & `tmp/fal-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-0.8.4.tar", max compression
+gzip compressed data, was "fal-0.8.5.tar", max compression
```

## Comparing `fal-0.8.4.tar` & `fal-0.8.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11804 2023-04-04 10:44:08.419638 fal-0.8.4/README.md
--rw-r--r--   0        0        0     2627 2023-04-04 10:44:16.687642 fal-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      221 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/__init__.py
--rw-r--r--   0        0        0       21 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/__init__.py
--rw-r--r--   0        0        0     8470 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/args.py
--rw-r--r--   0        0        0     2120 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/cli.py
--rw-r--r--   0        0        0     5243 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/dbt_runner.py
--rw-r--r--   0        0        0     6045 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/fal_runner.py
--rw-r--r--   0        0        0     4473 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/flow_runner.py
--rw-r--r--   0        0        0       56 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/model_generator/__init__.py
--rw-r--r--   0        0        0     5505 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/model_generator/model_generator.py
--rw-r--r--   0        0        0     3180 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/model_generator/module_check.py
--rw-r--r--   0        0        0     9707 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/cli/selectors.py
--rw-r--r--   0        0        0    12367 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/fal_script.py
--rw-r--r--   0        0        0        0 2023-04-04 10:44:08.427638 fal-0.8.4/src/fal/feature_store/__init__.py
--rw-r--r--   0        0        0      401 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/feature_store/feature.py
--rw-r--r--   0        0        0     8394 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/node_graph.py
--rw-r--r--   0        0        0        0 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/__init__.py
--rw-r--r--   0        0        0     1603 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/bridge.py
--rw-r--r--   0        0        0     5332 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/dependency_analysis.py
--rw-r--r--   0        0        0      793 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/environments/__init__.py
--rw-r--r--   0        0        0     9482 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/environments/base.py
--rw-r--r--   0        0        0     4395 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/environments/conda.py
--rw-r--r--   0        0        0     3369 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/environments/virtual_env.py
--rw-r--r--   0        0        0     4776 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/packages/isolated_runner.py
--rw-r--r--   0        0        0        0 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/planner/__init__.py
--rw-r--r--   0        0        0     5635 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/planner/executor.py
--rw-r--r--   0        0        0     6475 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/planner/plan.py
--rw-r--r--   0        0        0     6761 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/planner/schedule.py
--rw-r--r--   0        0        0     9041 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/planner/tasks.py
--rw-r--r--   0        0        0        0 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/telemetry/__init__.py
--rw-r--r--   0        0        0    11416 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/telemetry/telemetry.py
--rw-r--r--   0        0        0     3043 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/typing.py
--rw-r--r--   0        0        0     1654 2023-04-04 10:44:08.431638 fal-0.8.4/src/fal/utils.py
--rw-r--r--   0        0        0        0 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/__init__.py
--rw-r--r--   0        0        0    24315 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/lib.py
--rw-r--r--   0        0        0     3273 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/logger.py
--rw-r--r--   0        0        0     1850 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/magics.py
--rw-r--r--   0        0        0     8935 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/parse.py
--rw-r--r--   0        0        0    25721 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/project.py
--rw-r--r--   0        0        0        0 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/utils/__init__.py
--rw-r--r--   0        0        0     1970 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/utils/yaml_helper.py
--rw-r--r--   0        0        0      317 2023-04-04 10:44:08.431638 fal-0.8.4/src/faldbt/version.py
--rw-r--r--   0        0        0       33 2023-04-04 10:44:08.431638 fal-0.8.4/tests/_fal_testing/__init__.py
--rw-r--r--   0        0        0     1782 2023-04-04 10:44:08.431638 fal-0.8.4/tests/_fal_testing/utils.py
--rw-r--r--   0        0        0    14134 2023-04-04 10:44:18.071168 fal-0.8.4/setup.py
--rw-r--r--   0        0        0    13983 2023-04-04 10:44:18.072226 fal-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0    11804 2023-04-21 13:31:16.737053 fal-0.8.5/README.md
+-rw-r--r--   0        0        0     2627 2023-04-21 13:31:27.553114 fal-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/__init__.py
+-rw-r--r--   0        0        0     8470 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/args.py
+-rw-r--r--   0        0        0     2120 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/cli.py
+-rw-r--r--   0        0        0     5243 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/dbt_runner.py
+-rw-r--r--   0        0        0     6045 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/fal_runner.py
+-rw-r--r--   0        0        0     4473 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/flow_runner.py
+-rw-r--r--   0        0        0       56 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/model_generator/__init__.py
+-rw-r--r--   0        0        0     5505 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/model_generator/model_generator.py
+-rw-r--r--   0        0        0     3180 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/model_generator/module_check.py
+-rw-r--r--   0        0        0     9707 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/cli/selectors.py
+-rw-r--r--   0        0        0    12367 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/fal_script.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/feature_store/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/feature_store/feature.py
+-rw-r--r--   0        0        0     8394 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/node_graph.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/__init__.py
+-rw-r--r--   0        0        0     1603 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/bridge.py
+-rw-r--r--   0        0        0     5332 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/dependency_analysis.py
+-rw-r--r--   0        0        0      793 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/environments/__init__.py
+-rw-r--r--   0        0        0     9482 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/environments/base.py
+-rw-r--r--   0        0        0     4395 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/environments/conda.py
+-rw-r--r--   0        0        0     3369 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/environments/virtual_env.py
+-rw-r--r--   0        0        0     4776 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/packages/isolated_runner.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/planner/__init__.py
+-rw-r--r--   0        0        0     5635 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/planner/executor.py
+-rw-r--r--   0        0        0     6475 2023-04-21 13:31:16.753053 fal-0.8.5/src/fal/planner/plan.py
+-rw-r--r--   0        0        0     6761 2023-04-21 13:31:16.757053 fal-0.8.5/src/fal/planner/schedule.py
+-rw-r--r--   0        0        0     9041 2023-04-21 13:31:16.757053 fal-0.8.5/src/fal/planner/tasks.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:31:16.757053 fal-0.8.5/src/fal/telemetry/__init__.py
+-rw-r--r--   0        0        0    11416 2023-04-21 13:31:16.757053 fal-0.8.5/src/fal/telemetry/telemetry.py
+-rw-r--r--   0        0        0     3043 2023-04-21 13:31:16.757053 fal-0.8.5/src/fal/typing.py
+-rw-r--r--   0        0        0     1654 2023-04-21 13:31:16.757053 fal-0.8.5/src/fal/utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/__init__.py
+-rw-r--r--   0        0        0    24315 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/lib.py
+-rw-r--r--   0        0        0     3273 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/logger.py
+-rw-r--r--   0        0        0     1850 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/magics.py
+-rw-r--r--   0        0        0     8935 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/parse.py
+-rw-r--r--   0        0        0    25764 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/project.py
+-rw-r--r--   0        0        0        0 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/utils/__init__.py
+-rw-r--r--   0        0        0     1970 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/utils/yaml_helper.py
+-rw-r--r--   0        0        0      317 2023-04-21 13:31:16.757053 fal-0.8.5/src/faldbt/version.py
+-rw-r--r--   0        0        0       33 2023-04-21 13:31:16.757053 fal-0.8.5/tests/_fal_testing/__init__.py
+-rw-r--r--   0        0        0     1782 2023-04-21 13:31:16.757053 fal-0.8.5/tests/_fal_testing/utils.py
+-rw-r--r--   0        0        0    14134 2023-04-21 13:31:29.493404 fal-0.8.5/setup.py
+-rw-r--r--   0        0        0    13983 2023-04-21 13:31:29.494459 fal-0.8.5/PKG-INFO
```

### Comparing `fal-0.8.4/README.md` & `fal-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/pyproject.toml` & `fal-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fal"
-version = "0.8.4"
+version = "0.8.5"
 description = "fal allows you to run python scripts directly from your dbt project."
 homepage = "https://github.com/fal-ai/fal/blob/-/projects/fal"
 documentation = "https://docs.fal.ai"
 repository = "https://github.com/fal-ai/fal"
 readme = "README.md"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
```

### Comparing `fal-0.8.4/src/fal/cli/args.py` & `fal-0.8.5/src/fal/cli/args.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/cli/cli.py` & `fal-0.8.5/src/fal/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/cli/dbt_runner.py` & `fal-0.8.5/src/fal/cli/dbt_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/cli/fal_runner.py` & `fal-0.8.5/src/fal/cli/fal_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/cli/flow_runner.py` & `fal-0.8.5/src/fal/cli/flow_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/cli/model_generator/model_generator.py` & `fal-0.8.5/src/fal/cli/model_generator/model_generator.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/cli/model_generator/module_check.py` & `fal-0.8.5/src/fal/cli/model_generator/module_check.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/cli/selectors.py` & `fal-0.8.5/src/fal/cli/selectors.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/fal_script.py` & `fal-0.8.5/src/fal/fal_script.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/node_graph.py` & `fal-0.8.5/src/fal/node_graph.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/packages/bridge.py` & `fal-0.8.5/src/fal/packages/bridge.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/packages/dependency_analysis.py` & `fal-0.8.5/src/fal/packages/dependency_analysis.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/packages/environments/__init__.py` & `fal-0.8.5/src/fal/packages/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/packages/environments/base.py` & `fal-0.8.5/src/fal/packages/environments/base.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/packages/environments/conda.py` & `fal-0.8.5/src/fal/packages/environments/conda.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/packages/environments/virtual_env.py` & `fal-0.8.5/src/fal/packages/environments/virtual_env.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/packages/isolated_runner.py` & `fal-0.8.5/src/fal/packages/isolated_runner.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/planner/executor.py` & `fal-0.8.5/src/fal/planner/executor.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/planner/plan.py` & `fal-0.8.5/src/fal/planner/plan.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/planner/schedule.py` & `fal-0.8.5/src/fal/planner/schedule.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/planner/tasks.py` & `fal-0.8.5/src/fal/planner/tasks.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/telemetry/telemetry.py` & `fal-0.8.5/src/fal/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/typing.py` & `fal-0.8.5/src/fal/typing.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/fal/utils.py` & `fal-0.8.5/src/fal/utils.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/faldbt/lib.py` & `fal-0.8.5/src/faldbt/lib.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/faldbt/logger.py` & `fal-0.8.5/src/faldbt/logger.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/faldbt/magics.py` & `fal-0.8.5/src/faldbt/magics.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/faldbt/parse.py` & `fal-0.8.5/src/faldbt/parse.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/src/faldbt/project.py` & `fal-0.8.5/src/faldbt/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,15 @@
 
         lib.initialize_dbt_flags(profiles_dir=self.profiles_dir)
 
         # Can be overwritten if profile_target is not None
         self._config = parse.get_dbt_config(
             project_dir=self.project_dir,
             profiles_dir=self.profiles_dir,
+            profile_target=profile_target,
             threads=threads,
         )
 
         self._run_results = DbtRunResult(
             parse.get_dbt_results(self.project_dir, self._config)
         )
```

### Comparing `fal-0.8.4/src/faldbt/utils/yaml_helper.py` & `fal-0.8.5/src/faldbt/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/tests/_fal_testing/utils.py` & `fal-0.8.5/tests/_fal_testing/utils.py`

 * *Files identical despite different names*

### Comparing `fal-0.8.4/setup.py` & `fal-0.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
           'pytest-mock>=3.7.0,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['fal = fal.cli:cli']}
 
 setup_kwargs = {
     'name': 'fal',
-    'version': '0.8.4',
+    'version': '0.8.5',
     'description': 'fal allows you to run python scripts directly from your dbt project.',
     'long_description': '<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/fal/" target="_blank" /> -->\n\n# fal: do more with dbt\n\nfal is the easiest way to run Python with your [dbt](https://www.getdbt.com/) project.\n\n# Introduction\n\nWith the `fal` CLI, you can:\n\n- [Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example) upon dbt model success or failure.\n- [Load data from external data sources](https://blog.fal.ai/populate-dbt-models-with-csv-data/) before a model starts running.\n- [Download dbt models](https://docs.fal.ai/fal/python-package) into a Python context with a familiar syntax: `ref(\'my_dbt_model\')` using `FalDbt`\n- [Programatically access rich metadata](https://docs.fal.ai/fal/reference/variables-and-functions) about your dbt project.\n\nHead to our [documentation site](https://docs.fal.ai/) for a deeper dive or play with [in-depth examples](https://github.com/fal-ai/fal/blob/-/examples/README.md) to see how fal can help you get more done with dbt.\n\n> ❗️ If you would like to write data back to your data-warehouse, we recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter.\n\n# Getting Started\n\n## 1. Install `fal`\n\n```bash\n$ pip install fal\n```\n\n## 2. Go to your dbt project directory\n\n```bash\n$ cd ~/src/my_dbt_project\n```\n\n## 3. Create a Python script: `send_slack_message.py`\n\n```python\nimport os\nfrom slack_sdk import WebClient\nfrom slack_sdk.errors import SlackApiError\n\nCHANNEL_ID = os.getenv("SLACK_BOT_CHANNEL")\nSLACK_TOKEN = os.getenv("SLACK_BOT_TOKEN")\n\nclient = WebClient(token=SLACK_TOKEN)\nmessage_text = f"Model: {context.current_model.name}. Status: {context.current_model.status}."\n\ntry:\n    response = client.chat_postMessage(\n        channel=CHANNEL_ID,\n        text=message_text\n    )\nexcept SlackApiError as e:\n    assert e.response["error"]\n```\n\n## 4. Add a `meta` section in your `schema.yml`\n\n```yaml\nmodels:\n  - name: historical_ozone_levels\n    description: Ozone levels\n    config:\n      materialized: table\n    columns:\n      - name: ozone_level\n        description: Ozone level\n      - name: ds\n        description: Date\n    meta:\n      fal:\n        scripts:\n          - send_slack_message.py\n```\n\n## 5. Run `fal flow run`\n\n```bash\n$ fal flow run\n# both your dbt models and fal scripts are run\n```\n\n## 6. Alternatively run `dbt` and `fal` consecutively\n\n```bash\n$ dbt run\n# Your dbt models are run\n\n$ fal run\n# Your python scripts are run\n```\n\n# Examples\n\nTo explore what is possible with fal, take a look at the in-depth examples below. We will be adding more examples here over time:\n\n- [Example 1: Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example/README.md)\n- [Example 2: Use dbt from a Jupyter Notebook](https://github.com/fal-ai/fal/blob/-/examples/write_jupyter_notebook/README.md)\n- [Example 3: Read and parse dbt metadata](https://github.com/fal-ai/fal/blob/-/examples/read_dbt_metadata/README.md)\n- [Example 4: Metric forecasting](https://github.com/fal-ai/fal/blob/-/examples/metric-forecast/README.md)\n- [Example 5: Sentiment analysis on support tickets](https://github.com/fal-ai/fal/blob/-/examples/sentiment-analysis/README.md)\n- [Example 6: Anomaly Detection](https://github.com/fal-ai/fal/blob/-/examples/anomaly-detection/README.md)\n- [Example 7: Incorporate fal in CI/CD workflow](https://github.com/fal-ai/fal/blob/-/examples/ci_example/README.md)\n- [Example 8: Send events to Datadog](https://github.com/fal-ai/fal/blob/-/examples/datadog_event/README.md)\n- [Example 9: Write dbt artifacts to GCS](https://github.com/fal-ai/fal/blob/-/examples/write_to_gcs/README.md)\n- [Example 10: Write dbt artifacts to AWS S3](https://github.com/fal-ai/fal/blob/-/examples/write_to_aws/README.md)\n\n[Check out the examples directory for more](https://github.com/fal-ai/fal/blob/-/examples/README.md)\n\n# How it works?\n\n`fal` is a command line tool that can read the state of your `dbt` project and help you run Python scripts after your `dbt run`s by leveraging the [`meta` config](https://docs.getdbt.com/reference/resource-configs/meta).\n\n```yaml\nmodels:\n  - name: historical_ozone_levels\n    ...\n    meta:\n      fal:\n        post-hook:\n          # scripts will run concurrently\n          - send_slack_message.py\n          - another_python_script.py\n```\n\n`fal` also provides useful helpers within the Python context to seamlessly interact with dbt models: `ref("my_dbt_model_name")` will pull a dbt model into your Python script as a [`pandas.DataFrame`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).\n\n## Running scripts before dbt runs\n\nRun scripts before the model runs by using the `pre-hook:` configuration option.\n\nGiven the following schema.yml:\n\n```\nmodels:\n  - name: boston\n    description: Ozone levels\n    config:\n      materialized: table\n    meta:\n      owner: "@meder"\n      fal:\n        pre-hook:\n          - fal_scripts/trigger_fivetran.py\n        post-hook:\n          - fal_scripts/slack.py\n```\n\n`fal flow run` will run `fal_scripts/trigger_fivetran.py`, then the `boston` dbt model, and finally `fal_scripts/slack.py`.\nIf a model is selected with a selection flag (e.g. `--select boston`), the hooks associated to the model will always run with it.\n\n```bash\n$ fal flow run --select boston\n```\n\n# Concepts\n\n## profile.yml and Credentials\n\n`fal` integrates with `dbt`\'s `profile.yml` file to access and read data from the data warehouse. Once you setup credentials in your `profile.yml` file for your existing `dbt` workflows anytime you use `ref` or `source` to create a dataframe `fal` authenticates using the credentials specified in the `profile.yml` file.\n\n## `meta` Syntax\n\n```yaml\nmodels:\n  - name: historical_ozone_levels\n    ...\n    meta:\n      owner: "@me"\n      fal:\n        post-hook:\n          - send_slack_message.py\n          - another_python_script.py\n```\n\nUse the `fal` and `post-hook` keys underneath the `meta` config to let `fal` CLI know where to look for the Python scripts. You can pass a list of scripts as shown above to run one or more scripts as a post-hook operation after a `dbt run`.\n\n## Variables and functions\n\nInside a Python script, you get access to some useful variables and functions\n\n### Variables\n\nA `context` object with information relevant to the model through which the script was run. For the [`meta` Syntax](#meta-syntax) example, we would get the following:\n\n```python\ncontext.current_model.name\n#= historical_ozone_levels\n\ncontext.current_model.meta\n#= {\'owner\': \'@me\'}\n\ncontext.current_model.meta.get("owner")\n#= \'@me\'\n\ncontext.current_model.status\n# Could be one of\n#= \'success\'\n#= \'error\'\n#= \'skipped\'\n```\n\n`context` object also has access to test information related to the current model. If the previous dbt command was either `test` or `build`, the `context.current_model.test` property is populated with a list of tests:\n\n```python\ncontext.current_model.tests\n#= [CurrentTest(name=\'not_null\', modelname=\'historical_ozone_levels, column=\'ds\', status=\'Pass\')]\n```\n\n### `ref` and `source` functions\n\nThere are also available some familiar functions from `dbt`\n\n```python\n# Refer to dbt models or sources by name and returns it as `pandas.DataFrame`\nref(\'model_name\')\nsource(\'source_name\', \'table_name\')\n\n# You can use it to get the running model data\nref(context.current_model.name)\n```\n\n### `write_to_model` function\n\n> ❗️ We recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter for writing data back to your data-warehouse.\n\nIt is also possible to send data back to your data-warehouse. This makes it easy to get the data, process it and upload it back into dbt territory.\n\nThis function is available in fal Python models only, that is a Python script inside a `fal_models` directory and add a `fal-models-paths` to your `dbt_project.yml`\n\n```yaml\nname: "jaffle_shop"\n# ...\nmodel-paths: ["models"]\n# ...\n\nvars:\n  # Add this to your dbt_project.yml\n  fal-models-paths: ["fal_models"]\n```\n\nOnce added, it will automatically be run by fal without having to add any extra configurations in the `schema.yml`.\n\n```python\nsource_df = source(\'source_name\', \'table_name\')\nref_df = ref(\'a_model\')\n\n# Your code here\ndf = ...\n\n# Upload a `pandas.DataFrame` back to the datawarehouse\nwrite_to_model(df)\n```\n\n`write_to_model` also accepts an optional `dtype` argument, which lets you specify datatypes of columns. It works the same way as `dtype` argument for [`DataFrame.to_sql` function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_sql.html).\n\n```python\nfrom sqlalchemy.types import Integer\n# Upload but specifically create the `value` column with type `integer`\n# Can be useful if data has `None` values\nwrite_to_model(df, dtype={\'value\': Integer()})\n```\n\n## Importing `fal` as a Python package\n\nYou may be interested in accessing dbt models and sources easily from a Jupyter Notebook or another Python script.\nFor that, just import the `fal` package and intantiate a FalDbt project:\n\n```py\nfrom fal import FalDbt\nfaldbt = FalDbt(profiles_dir="~/.dbt", project_dir="../my_project")\n\nfaldbt.list_sources()\n# [\n#    DbtSource(name=\'results\' ...),\n#    DbtSource(name=\'ticket_data_sentiment_analysis\' ...)\n#    ...\n# ]\n\nfaldbt.list_models()\n# [\n#    DbtModel(name=\'zendesk_ticket_data\' ...),\n#    DbtModel(name=\'agent_wait_time\' ...)\n#    ...\n# ]\n\n\nsentiments = faldbt.source(\'results\', \'ticket_data_sentiment_analysis\')\n# pandas.DataFrame\ntickets = faldbt.ref(\'stg_zendesk_ticket_data\')\n# pandas.DataFrame\n```\n\n# Supported `dbt` versions\n\nThe latest `fal` version currently supports dbt `1.4.*`.\n\nIf you need another version, [open an issue](https://github.com/fal-ai/fal/issues/new) and we will take a look!\n\n# Contributing / Development\n\nWe use Poetry for dependency management and easy development testing.\n\nUse Poetry shell to trying your changes right away:\n\n```sh\n~ $ cd fal\n\n~/fal $ poetry install\n\n~/fal $ poetry shell\nSpawning shell within [...]/fal-eFX98vrn-py3.8\n\n~/fal fal-eFX98vrn-py3.8 $ cd ../dbt_project\n\n~/dbt_project fal-eFX98vrn-py3.8 $ fal flow run\n19:27:30  Found 5 models, 0 tests, 0 snapshots, 0 analyses, 165 macros, 0 operations, 0 seed files, 1 source, 0 exposures, 0 metrics\n19:27:30 | Starting fal run for following models and scripts:\n[...]\n```\n\n## Running tests\n\nTests rely on a Postgres database to be present, this can be achieved with docker-compose:\n\n```sh\n~/fal $ docker-compose -f tests/docker-compose.yml up -d\nCreating network "tests_default" with the default driver\nCreating fal_db ... done\n\n# Necessary for the import test\n~/fal $ dbt run --profiles-dir tests/mock/mockProfile --project-dir tests/mock\nRunning with dbt=1.0.1\n[...]\nCompleted successfully\nDone. PASS=5 WARN=0 ERROR=0 SKIP=0 TOTAL=5\n\n~/fal $ pytest -s\n```\n\n# Why are we building this?\n\nWe think `dbt` is great because it empowers data people to get more done with the tools that they are already familiar with.\n\n`dbt`\'s SQL only design is powerful, but if you ever want to get out of SQL-land and connect to external services or get into Python-land for any reason, you will have a hard time. We built `fal` to enable Python workloads (sending alerts to Slack, building predictive models, pushing data to non-data-warehouse destinations and more) **right within `dbt`**.\n\nThis library will form the basis of our attempt to more comprehensively enable **data science workloads** downstream of `dbt`. And because having reliable data pipelines is the most important ingredient in building predictive analytics, we are building a library that integrates well with dbt.\n\n# Have feedback or need help?\n\n- Join us in [fal on Discord](https://discord.com/invite/Fyc9PwrccF)\n- Join the [dbt Community](http://community.getdbt.com/) and go into our [#tools-fal channel](https://getdbt.slack.com/archives/C02V8QW3Q4Q)\n',
     'author': 'Features & Labels',
     'author_email': 'hello@fal.ai',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fal-ai/fal/blob/-/projects/fal',
```

### Comparing `fal-0.8.4/PKG-INFO` & `fal-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 0.8.4
+Version: 0.8.5
 Summary: fal allows you to run python scripts directly from your dbt project.
 Home-page: https://github.com/fal-ai/fal/blob/-/projects/fal
 Keywords: dbt,pandas
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7.2,<3.11
 Classifier: Development Status :: 4 - Beta
```

