# Comparing `tmp/cortex_cli-1.12.5.tar.gz` & `tmp/cortex_cli-1.12.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.12.5.tar", last modified: Fri Apr 14 18:12:12 2023, max compression
+gzip compressed data, was "cortex_cli-1.12.6.tar", last modified: Fri Apr 21 19:48:48 2023, max compression
```

## Comparing `cortex_cli-1.12.5.tar` & `cortex_cli-1.12.6.tar`

### file list

```diff
@@ -1,65 +1,86 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.5/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-14 18:12:01.000000 cortex_cli-1.12.5/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.5/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.5/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.5/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    22365 2023-04-14 16:22:47.000000 cortex_cli-1.12.5/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.5/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-14 17:16:40.000000 cortex_cli-1.12.5/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-13 17:02:54.000000 cortex_cli-1.12.5/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     7183 2023-04-14 17:17:17.000000 cortex_cli-1.12.5/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1681 2023-04-14 17:21:25.000000 cortex_cli-1.12.5/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-11 16:29:39.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-11 16:28:41.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      533 2023-04-06 19:56:03.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-06 19:56:06.000000 cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.5/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1928 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-14 18:12:12.000000 cortex_cli-1.12.5/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.5/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-14 18:12:12.019189 cortex_cli-1.12.5/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1053 2023-04-07 18:01:54.000000 cortex_cli-1.12.5/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5185 2023-04-06 19:56:17.000000 cortex_cli-1.12.6/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-04-20 17:50:53.000000 cortex_cli-1.12.6/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.12.6/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3990 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      880 2023-04-07 17:56:26.000000 cortex_cli-1.12.6/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      971 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.12.6/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24183 2023-04-21 19:48:42.000000 cortex_cli-1.12.6/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3248 2023-04-07 17:56:26.000000 cortex_cli-1.12.6/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.12.6/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-21 19:32:17.000000 cortex_cli-1.12.6/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-20 19:24:15.000000 cortex_cli-1.12.6/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-04-20 19:25:56.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.537815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-20 19:27:56.000000 cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-03-21 14:31:47.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1602 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-04-20 17:50:53.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-17 18:14:34.000000 cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.12.6/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3123 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-04-21 19:48:48.000000 cortex_cli-1.12.6/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.12.6/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-04-21 19:48:48.547815 cortex_cli-1.12.6/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-20 19:25:09.000000 cortex_cli-1.12.6/setup.py
```

### Comparing `cortex_cli-1.12.5/README.md` & `cortex_cli-1.12.6/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.12.6/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.12.6/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.12.6/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.12.6/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/configure.py` & `cortex_cli-1.12.6/cortex_cli/cli/configure.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.12.6/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/generic_get.py` & `cortex_cli-1.12.6/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/inferences.py` & `cortex_cli-1.12.6/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/models.py` & `cortex_cli-1.12.6/cortex_cli/cli/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 
 class ModelsCli(plumbum.cli.Application):
     NAME = 'models'
 
 
 @ModelsCli.subcommand('init')
 class InitModel(CliApiBase):
-    ML_MODEL_TEMPLATE_PATH = 'ml_model_template'
+    MODEL_TEMPLATES_PATH = 'model_templates'
+    MODEL_TEMPLATES = [
+        'digits_model',
+        'chatgpt_model'
+    ]
 
 
     _name = plumbum.cli.SwitchAttr(
         names=['-n', '--name'],
         argtype=str,
         help='The name of the model. Should use a readable format, ie. Digits Model',
         default=None
@@ -52,14 +56,21 @@
     _description = plumbum.cli.SwitchAttr(
         names=['-d', '--description'],
         argtype=str,
         default='A model that is initialized through the Cortex CLI.',
         help='A description of the model'
     )
 
+    _template = plumbum.cli.SwitchAttr(
+        names=['-t', '--template'],
+        argtype=str,
+        default='digits_model',
+        help='The template to use for the model. The default is "digits_model".\nAvailable choices are: ' + ', '.join(MODEL_TEMPLATES),
+    )
+
     _token = plumbum.cli.SwitchAttr(
         names=['--github-token'],
         argtype=str,
         envname='GH_TOKEN'
     )
 
     _org = plumbum.cli.SwitchAttr(
@@ -82,15 +93,16 @@
     )
 
     # Properties
 
     @property
     def _template_location(self):
         current = os.path.dirname(os.path.realpath(__file__))
-        return os.path.join(os.path.dirname(current), self.ML_MODEL_TEMPLATE_PATH)
+        template_path = os.path.join(current, self.MODEL_TEMPLATES_PATH)
+        return os.path.join(template_path, self._template)
 
     @property
     def _model_path(self):
         return os.path.join(self._path, self._repo)
 
 
     def main(self, *args):
@@ -299,49 +311,39 @@
 
 # -------------------------------------------------------------------------------
 
     def main(self, *args):
         # Change to working directory
         os.chdir(self._path)
 
-        model = None
+        self.model = None
         self._error_message = None
         self._success = False
         self._model_json = None
         self._pipeline_json = None
+        self._requested_secrets = []
         try:
             self._model_json = self._get_model()
             # Step 1 - Get live model data
             if self._tracking:
                 self._mlflow_client = self._setup_mlflow()
                 self._setup_pipeline()
 
             # Step 2 - Load the Model Class
-            model = self._instantiate_model(self._config)
+            self.model = self._instantiate_model(self._config)
 
             # Step 3 - Initialize the pipeline steps
             self._initialize_steps()
 
             # Step 4 - Run the pipeline
             if self._tracking:
                 self._pipeline_json = self._run_pipeline()
 
             # Step 5 - Run the pipeline steps
-            self._run_pipeline_steps(model)
-
-            # Step 6 - Save the pipeline artifacts
-            self._save_pipeline(model)
-
-            # Step 7 - Save the conda environment
-            # if self._tracking:
-            self._save_environment()
-
-            # Step 8 - Upload the pipeline artifacts
-            if self._tracking:
-                self._upload_pipeline()
+            self._run_pipeline_steps()
         except Exception as e:
             if not self._error_message:
                 self._error_message = traceback.format_exc()
         finally:
 
             try:
                 # Step 9 - Contact callback route to update currentStage of model pipeline
@@ -360,21 +362,64 @@
                 self._pass('Completed Cortex Pipeline Run')
 
 # -------------------------------------------------------------------------------
 
     def _initialize_steps(self):
         # Convert yaml steps to ml-api format
         _steps = []
+
+        # Add default download data step
+        _steps.append({
+            'name':   'Download data',
+            'type':   'download_data',
+            'config': {}
+        })
+
         for step in self._pipeline_steps:
             _steps.append({
                 'name':   step.name,
                 'type':   step.type,
                 'config': {}
             })
         
+        # Add default download data step
+        _steps.append({
+            'name':   'Cleanup model params',
+            'type':   'cleanup_self',
+            'config': {}
+        })
+
+        # Add default save pipeline artifacts step
+        _steps.append({
+            'name':   'Save pipeline artifacts',
+            'type':   '_save_pipeline',
+            'config': {
+                'cortex_cli_func': True
+            }
+        })
+
+        # Add default save pipeline environment step
+        _steps.append({
+            'name':   'Save pipeline environment',
+            'type':   '_save_environment',
+            'config': {
+                'cortex_cli_func': True
+            }
+        })
+
+        # Add default upload to cortex step
+        _steps.append({
+            'name':   'Upload pipeline artifacts',
+            'type':   '_upload_pipeline',
+            'config': {
+                'cortex_cli_func': True,
+                'requires_tracking': True
+            }
+        })
+        
         if self._tracking:
             # Set cortex steps
             self._steps = self._create_steps(_steps)
         else:
             # Set normal steps
             self._steps = _steps
 
@@ -487,27 +532,33 @@
             headers=self._headers,
             json={
                 'modelId': self._model_id
             }
         ).json()
 
 
-    def _run_pipeline_steps(self, model):
+    def _run_pipeline_steps(self):
         current_step = None
         try:
             for step in self._steps:
                 current_step = step['type']
-                step_func = getattr(model, current_step)
+                step_config = step['config']
+                step_func = getattr(self if step_config.get('cortex_cli_func') else self.model, current_step)
                 step_result = None
 
+                # Extract secrets from model if we are in cleanup step
+                if current_step == 'cleanup_self':
+                    self._requested_secrets = self.model.secrets_manager.secrets
+
                 # Handle special case for passing testing inferences to test_predict function
                 if current_step == 'detect_drift':
                     step_result = step_func(self._get_drift_inferences())
                 else:
-                    step_result = step_func()
+                    if (step_config.get('requires_tracking') and self._tracking) or (not step_config.get('requires_tracking')):
+                        step_result = step_func()
 
                 if self._tracking:
                     step_risk = ''
 
                     # Get ethics check results (if it exists)
                     if type(step_result) is EthicsResult:
                         # Parse out risk level
@@ -582,62 +633,63 @@
         return model[0]
 
 
     def _complete_callback(self, status, error_message=None):
         body = {
             'modelId':      self._model_id,
             'currentStage': status,
+            'secrets': self._requested_secrets
         }
 
         if error_message:
             body['message']: error_message
 
         requests.put(
             url=f'{self._api_url}/pipelines/{self._pipeline_id}/run/complete',
             headers=self._headers,
             json=body
         )
 
 
-    def _save_pipeline(self, model):
+    def _save_pipeline(self):
         self._info('Saving pipeline artifacts...')
-        signature = infer_signature(model.input_example, model.output_example)
+        signature = infer_signature(self.model.input_example, self.model.output_example)
 
         # Save model
         modules = list(self._modules.keys())
         modules.append(self._model_module)
-        if model.model_type == 'cortex':
+        if self.model.model_type == 'cortex':
             mlflow_cortex.save_model(
-                python_model=model, 
+                python_model=self.model, 
                 path=self._artifacts_dir,                   # Where artifacts are stored locally
                 code_path=list(modules),                    # Local code paths not on
                 conda_env='conda.yml',
                 artifacts={},
-                custom_objects=model.custom_objects,
+                custom_objects=self.model.custom_objects,
                 signature=signature
             )
         else:
             self._error_message = f"An error occurred while detecting the Cortex model type. \
-            Found '{model.model_type}', but only ['cortex'] are acceptable values"
+            Found '{self.model.model_type}', but only ['cortex'] are acceptable values"
             raise Exception
 
-        self._pass(f'Saved the pipeline artifacts to disk: ({self._artifacts_dir})')
+        return f'Saved the pipeline artifacts to disk: ({self._artifacts_dir})'
 
 
     def _save_environment(self):
         self._info('Packing conda environment...')
 
         conda_pack.pack(
             output=f'{self._artifacts_dir}/environment.tar.gz',
             force=True,
             verbose=True,
             ignore_editable_packages=False,
             ignore_missing_files=True)
 
-        self._pass(f'Packed conda environment to disk: ({self._artifacts_dir})')
+        return f'Packed conda environment to disk: ({self._artifacts_dir})'
 
 
     def _upload_pipeline(self):
         self._info('Uploading pipeline artifacts to Cortex...')
 
         file_names = []
         file_paths = []
@@ -663,15 +715,15 @@
         for i in range(len(file_names)):
             with open(file_paths[i], 'rb') as f:
                 requests.put(
                     upload_urls[i],
                     data=f
                 )
         
-        self._pass(f'Uploaded the pipeline artifacts to Cortex')
+        return f'Uploaded the pipeline artifacts to Cortex'
 
 
     def _instantiate_model(self, config):
         # LOAD DEPENDENCY MODULES (except model)
         for path, module in self._modules.items():
             self._load_module(path, module)
```

### Comparing `cortex_cli-1.12.5/cortex_cli/cli/pipelines.py` & `cortex_cli-1.12.6/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/core/cortex_data.py` & `cortex_cli-1.12.6/cortex_cli/core/cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/core/drift_checks.py` & `cortex_cli-1.12.6/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.12.6/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.12.6/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.12.6/cortex_cli/core/models/cortex_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import mlflow.pyfunc
+from typing import List, Union
 
 from cortex_cli.core.cortex_data import CortexData
 from cortex_cli.core.ethics_checks import EthicsManager, EthicsTypeEnum
 from cortex_cli.core.drift_checks import DriftManager, DriftTypeEnum
 from cortex_cli.core.secrets_manager import SecretsManager
 
 
@@ -20,14 +21,15 @@
         self.cortex_data = CortexData(model_id, api_url, headers)
         self.ethics_manager = None
         self.drift_manager = DriftManager()
         self.secrets_manager = SecretsManager(api_url, headers)
 
         self.metrics = {}
         self.custom_objects = {}
+        self.cleanup_vars = []
 
 
     def download_data(self):
         """Downloads data during initial training
 
             Parameters:
             N/A
@@ -97,20 +99,22 @@
             Returns:
             N/A
 
         """
         self.secrets_manager.reset_secrets()
 
         try:
-            for s in ['cortex_data', 'ethics_manager']:
+            for s in ['cortex_data', 'ethics_manager'] + self.cleanup_vars:
                 if s in self.__dict__:
                     del self.__dict__[s]
         except AttributeError:
             pass
 
+        return 'Successfully cleaned up self variables'
+
 
     def predict(self, model_input):
         """Predicts using a TBD model
 
             Parameters:
             model_input: (pandas.DataFrame, numpy.ndarray, scipy.sparse.(csc.csc_matrix | csr.csr_matrix), List[Any], Dict[str, Any]): Input for prediction
 
@@ -198,33 +202,57 @@
         """Adds a metric to be automatically saved after training
 
             Parameters:
             metric_name (str): Name of metric to save
             metric_value (str): Value of metric to save
 
             Returns:
-            N/A
+            str: Success message
 
         """
         self.metrics[metric_name] = metric_value
+
+        return 'Successfully added metric'
     
 
     def _add_custom_object(self, object_name, object_value):
         """Adds a custom keras object to the model to be automatically saved and loaded
 
             Parameters:
             object_name (str): Name of custom object to save
             object_value (str): Value of custom object to save
 
             Returns:
-            N/A
+            str: Success message
 
         """
         self.custom_objects[object_name] = object_value
 
+        return 'Successfully added custom object'
+
+
+    def _add_cleanup_var(self, var_name: Union[str, List[str]]):
+        """Adds a variable to be cleaned up after training
+
+            Parameters:
+            var_name (str / list(str)): Name of variable to clean up
+
+            Returns:
+            str: Success message
+
+        """
+        if isinstance(var_name, list):
+            self.cleanup_vars = self.cleanup_vars + var_name
+            return 'Successfully added cleanup variables'
+        elif isinstance(var_name, str):
+            self.cleanup_vars.append(var_name)
+            return 'Successfully added cleanup variable'
+
+        return 'Failed to add cleanup variable(s)'
+
 
     def _set_input_output_examples(self, input_example, output_example):
         """Sets input and output examples for the model
 
             Parameters:
             input_example (pandas.DataFrame, numpy.ndarray, scipy.sparse.(csc.csc_matrix | csr.csr_matrix), List[Any], Dict[str, Any]): An input example for the model
             output_example (pandas.DataFrame, numpy.ndarray, scipy.sparse.(csc.csc_matrix | csr.csr_matrix), List[Any], Dict[str, Any]): An output example for the model
```

### Comparing `cortex_cli-1.12.5/cortex_cli/ml_model_template/.gitignore` & `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/ml_model_template/README.md` & `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.12.6/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.12.6/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.12.6/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.12.6/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.12.5/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.12.6/cortex_cli.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -27,23 +27,37 @@
 cortex_cli/core/drift_checks.py
 cortex_cli/core/ethics_checks.py
 cortex_cli/core/secrets_manager.py
 cortex_cli/core/mlflow/__init__.py
 cortex_cli/core/mlflow/mlflow_cortex.py
 cortex_cli/core/models/__init__.py
 cortex_cli/core/models/cortex_model.py
-cortex_cli/ml_model_template/.gitignore
-cortex_cli/ml_model_template/README.md
-cortex_cli/ml_model_template/__init__.py
-cortex_cli/ml_model_template/cookiecutter.json
-cortex_cli/ml_model_template/requirements.txt
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/.gitignore
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/README.md
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/conda.yml
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/cortex.yml
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/data/.gitkeep
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
-cortex_cli/ml_model_template/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+cortex_cli/model_templates/__init__.py
+cortex_cli/model_templates/chatgpt_model/.gitignore
+cortex_cli/model_templates/chatgpt_model/README.md
+cortex_cli/model_templates/chatgpt_model/__init__.py
+cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+cortex_cli/model_templates/chatgpt_model/requirements.txt
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+cortex_cli/model_templates/digits_model/.gitignore
+cortex_cli/model_templates/digits_model/README.md
+cortex_cli/model_templates/digits_model/__init__.py
+cortex_cli/model_templates/digits_model/cookiecutter.json
+cortex_cli/model_templates/digits_model/requirements.txt
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
 cortex_cli/tests/__init__.py
 cortex_cli/tests/test_cortex_data.py
 cortex_cli/tests/test_ethics_checks.py
```

### Comparing `cortex_cli-1.12.5/setup.py` & `cortex_cli-1.12.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         'mlflow',
         'mlserver',
         'mlserver-mlflow',
         'fairlearn',
         'prophet'
     ],
     package_data={
-        'cortex_cli.ml_model_template': ['*', '*/*', '*/*/*', '*/*/*/*', '.*', '*/.*', '*/*/.*']
+        'cortex_cli.model_templates': ['*', '*/*', '*/*/*', '*/*/*/*', '*/*/*/*/*', '.*', '*/.*', '*/*/.*', '*/*/*/.*']
     }
 )
```

