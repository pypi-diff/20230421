# Comparing `tmp/grizzly-loadtester-2.6.2.tar.gz` & `tmp/grizzly-loadtester-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grizzly-loadtester-2.6.2.tar", last modified: Mon Apr  3 09:20:57 2023, max compression
+gzip compressed data, was "grizzly-loadtester-2.6.3.tar", last modified: Fri Apr 21 06:49:19 2023, max compression
```

## Comparing `grizzly-loadtester-2.6.2.tar` & `grizzly-loadtester-2.6.3.tar`

### file list

```diff
@@ -1,325 +1,325 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.396459 grizzly-loadtester-2.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.340459 grizzly-loadtester-2.6.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.328459 grizzly-loadtester-2.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.340459 grizzly-loadtester-2.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.github/workflows/code-quality.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.340459 grizzly-loadtester-2.6.2/.pytest_tmp/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.pytest_tmp/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.340459 grizzly-loadtester-2.6.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-03 09:20:57.396459 grizzly-loadtester-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.340459 grizzly-loadtester-2.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/build.novella
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.344459 grizzly-loadtester-2.6.2/docs/content/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.344459 grizzly-loadtester-2.6.2/docs/content/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.348459 grizzly-loadtester-2.6.2/docs/content/assets/logo/
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png
--rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   116365 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_1024.png
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_128.png
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_16.png
--rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_256.png
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_48.png
--rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_512.png
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_64.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.348459 grizzly-loadtester-2.6.2/docs/content/command-line-interface/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/command-line-interface/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/command-line-interface/licenses.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.348459 grizzly-loadtester-2.6.2/docs/content/command-line-interface/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/command-line-interface/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/command-line-interface/usage/metadata.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.348459 grizzly-loadtester-2.6.2/docs/content/editor-support/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/editor-support/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.348459 grizzly-loadtester-2.6.2/docs/content/editor-support/editors/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/editor-support/editors/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/editor-support/editors/vscode.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/editor-support/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/editor-support/language-server.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/editor-support/licenses.md
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/example.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.352459 grizzly-loadtester-2.6.2/docs/content/framework/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/framework/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/framework/licenses.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.332459 grizzly-loadtester-2.6.2/docs/content/framework/usage/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.352459 grizzly-loadtester-2.6.2/docs/content/framework/usage/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/framework/usage/variables/environment-configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/framework/usage/variables/templating.md
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/content/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/docs/mkdocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.352459 grizzly-loadtester-2.6.2/example/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.352459 grizzly-loadtester-2.6.2/example/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/environments/example.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.352459 grizzly-loadtester-2.6.2/example/features/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/features/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/features/example.feature
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.332459 grizzly-loadtester-2.6.2/example/features/requests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.352459 grizzly-loadtester-2.6.2/example/features/requests/books/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/features/requests/books/books.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.352459 grizzly-loadtester-2.6.2/example/features/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/features/steps/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/features/steps/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/example/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.356459 grizzly-loadtester-2.6.2/grizzly/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-03 09:20:57.000000 grizzly-loadtester-2.6.2/grizzly/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/behave.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.356459 grizzly-loadtester-2.6.2/grizzly/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/listeners/appinsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/listeners/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    27043 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/locust.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.356459 grizzly-loadtester-2.6.2/grizzly/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/scenarios/iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.356459 grizzly-loadtester-2.6.2/grizzly/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.356459 grizzly-loadtester-2.6.2/grizzly/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/background/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/background/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.360459 grizzly-loadtester-2.6.2/grizzly/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/scenario/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/scenario/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/scenario/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    33390 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/scenario/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/scenario/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/steps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.360459 grizzly-loadtester-2.6.2/grizzly/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/async_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.360459 grizzly-loadtester-2.6.2/grizzly/tasks/clients/
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/clients/blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/clients/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/clients/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/clients/servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/set_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/task_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/until.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/tasks/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.364459 grizzly-loadtester-2.6.2/grizzly/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.364459 grizzly-loadtester-2.6.2/grizzly/testdata/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/integer_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/random_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/testdata/variables/random_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.364459 grizzly-loadtester-2.6.2/grizzly/types/
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/types/behave.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/types/locust.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.368459 grizzly-loadtester-2.6.2/grizzly/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.368459 grizzly-loadtester-2.6.2/grizzly/users/base/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/base/grizzly_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/base/request_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/base/response_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/base/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/iothub.py
--rw-r--r--   0 runner    (1001) docker     (123)    16642 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/users/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.368459 grizzly-loadtester-2.6.2/grizzly_extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.368459 grizzly-loadtester-2.6.2/grizzly_extras/async_message/
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/async_message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/async_message/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.368459 grizzly-loadtester-2.6.2/grizzly_extras/async_message/mq/
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/async_message/mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/async_message/mq/rfh2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/async_message/sb.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/dummy_pymqi.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/grizzly_extras/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.372459 grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-03 09:20:57.000000 grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-03 09:20:57.000000 grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 09:20:57.000000 grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 09:20:57.000000 grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-03 09:20:57.000000 grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-03 09:20:57.000000 grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.372459 grizzly-loadtester-2.6.2/script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/script/docs-generate-changelog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4893 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/script/docs-generate-licenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/script/docs-generate.bash
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 09:20:57.396459 grizzly-loadtester-2.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.372459 grizzly-loadtester-2.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.376459 grizzly-loadtester-2.6.2/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.376459 grizzly-loadtester-2.6.2/tests/e2e/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.376459 grizzly-loadtester-2.6.2/tests/e2e/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/background/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/background/test_shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.376459 grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    41158 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/steps/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/test_failure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/test_iteration_pace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/test_until.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/e2e/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    38022 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.376459 grizzly-loadtester-2.6.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.380459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.380459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/test_appinsights.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/test_influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.380459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/scenarios/test_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.380459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.380459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/background/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/background/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/background/test_shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.384459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    31205 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    21230 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/test__helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/test_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.388459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.388459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    21166 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_async_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_log_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_set_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_task_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_until.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_behave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    31766 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_locust.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    25758 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.388459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test_communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    20125 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.392459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_random_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_random_string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.392459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.396459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_grizzly_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_request_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_response_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    35818 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_blobstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_iothub.py
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)    44377 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23649 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_servicebus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_sftp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.396459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.396459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 09:20:57.396459 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/mq/
--rw-r--r--   0 runner    (1001) docker     (123)    35169 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/test___init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    37104 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/test_sb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-03 09:19:51.000000 grizzly-loadtester-2.6.2/tests/webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.010635 grizzly-loadtester-2.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.github/workflows/code-quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.pytest_tmp/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.pytest_tmp/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/build.novella
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/docs/content/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.022635 grizzly-loadtester-2.6.3/docs/content/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.026635 grizzly-loadtester-2.6.3/docs/content/assets/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   116365 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_1024.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_48.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_64.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.026635 grizzly-loadtester-2.6.3/docs/content/command-line-interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/licenses.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.026635 grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/metadata.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/editor-support/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/editor-support/editors/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/editors/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/editors/vscode.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/language-server.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/editor-support/licenses.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/example.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/licenses.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.014634 grizzly-loadtester-2.6.3/docs/content/framework/usage/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/environment-configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/templating.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/content/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/docs/mkdocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/environments/example.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/example.feature
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.014634 grizzly-loadtester-2.6.3/example/features/requests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/features/requests/books/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/requests/books/books.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.030634 grizzly-loadtester-2.6.3/example/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/steps/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/features/steps/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/example/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/listeners/appinsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/listeners/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26780 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/locust.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/scenarios/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.034634 grizzly-loadtester-2.6.3/grizzly/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/background/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/background/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.038634 grizzly-loadtester-2.6.3/grizzly/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35217 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/scenario/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/steps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.042634 grizzly-loadtester-2.6.3/grizzly/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/async_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.042634 grizzly-loadtester-2.6.3/grizzly/tasks/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/clients/servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/set_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/task_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/tasks/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.042634 grizzly-loadtester-2.6.3/grizzly/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/testdata/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/integer_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/types/behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/types/locust.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.046634 grizzly-loadtester-2.6.3/grizzly/users/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/grizzly_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/request_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/response_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/base/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31082 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/users/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.050634 grizzly-loadtester-2.6.3/grizzly_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.050634 grizzly-loadtester-2.6.3/grizzly_extras/async_message/
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.050634 grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/rfh2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25809 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/async_message/sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/dummy_pymqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/grizzly_extras/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-21 06:49:19.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 06:49:18.000000 grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1858 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/script/docs-generate-changelog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4893 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/script/docs-generate-licenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2855 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/script/docs-generate.bash
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.054634 grizzly-loadtester-2.6.3/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/e2e/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/e2e/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41596 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/steps/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_iteration_pace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/e2e/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38477 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.058634 grizzly-loadtester-2.6.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18649 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_appinsights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36224 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/test_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.062634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34083 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21230 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test__helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12509 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30575 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24915 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_async_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_log_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10944 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_set_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_task_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17583 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_until.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9970 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_behave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21307 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32204 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_locust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.066634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20125 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.074634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12430 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.074634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.074634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_grizzly_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_request_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35818 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_blobstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_iothub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44377 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_servicebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12862 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_sftp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:49:19.078634 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/
+-rw-r--r--   0 runner    (1001) docker     (123)    35067 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test___init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-21 06:47:45.000000 grizzly-loadtester-2.6.3/tests/webserver.py
```

### Comparing `grizzly-loadtester-2.6.2/.devcontainer/Dockerfile` & `grizzly-loadtester-2.6.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/.devcontainer/devcontainer.json` & `grizzly-loadtester-2.6.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/.github/workflows/code-quality.yaml` & `grizzly-loadtester-2.6.3/.github/workflows/code-quality.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/.github/workflows/release.yaml` & `grizzly-loadtester-2.6.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/.vscode/launch.json` & `grizzly-loadtester-2.6.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/LICENSE.md` & `grizzly-loadtester-2.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/PKG-INFO` & `grizzly-loadtester-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester
-Version: 2.6.2
+Version: 2.6.3
 Summary: Traffic generator based on locust and behave
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,load,loadtest,performance,traffic generator
```

### Comparing `grizzly-loadtester-2.6.2/README.md` & `grizzly-loadtester-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/build.novella` & `grizzly-loadtester-2.6.3/docs/build.novella`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/favicon.ico` & `grizzly-loadtester-2.6.3/docs/content/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown.svg` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_128px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_256px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_32px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_512px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_brown_64px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange.svg` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_128px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_256px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_32px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_512px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_grasshopper_orange_64px.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo.svg` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo.svg`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_1024.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_1024.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_128.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_128.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_16.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_16.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_256.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_256.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_32.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_32.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_48.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_48.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_512.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_512.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/assets/logo/grizzly_logo_64.png` & `grizzly-loadtester-2.6.3/docs/content/assets/logo/grizzly_logo_64.png`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/command-line-interface/usage/metadata.md` & `grizzly-loadtester-2.6.3/docs/content/command-line-interface/usage/metadata.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/editor-support/index.md` & `grizzly-loadtester-2.6.3/docs/content/editor-support/index.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/example.md` & `grizzly-loadtester-2.6.3/docs/content/example.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/framework/usage/variables/environment-configuration.md` & `grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/environment-configuration.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/content/framework/usage/variables/templating.md` & `grizzly-loadtester-2.6.3/docs/content/framework/usage/variables/templating.md`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/docs/mkdocs.yaml` & `grizzly-loadtester-2.6.3/docs/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/example/features/environment.py` & `grizzly-loadtester-2.6.3/example/features/environment.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/example/features/example.feature` & `grizzly-loadtester-2.6.3/example/features/example.feature`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/example/features/steps/custom.py` & `grizzly-loadtester-2.6.3/example/features/steps/custom.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/example/features/steps/steps.py` & `grizzly-loadtester-2.6.3/example/features/steps/steps.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/behave.py` & `grizzly-loadtester-2.6.3/grizzly/behave.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/clients.py` & `grizzly-loadtester-2.6.3/grizzly/clients.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/context.py` & `grizzly-loadtester-2.6.3/grizzly/context.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/exceptions.py` & `grizzly-loadtester-2.6.3/grizzly/exceptions.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/listeners/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/listeners/appinsights.py` & `grizzly-loadtester-2.6.3/grizzly/listeners/appinsights.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/listeners/influxdb.py` & `grizzly-loadtester-2.6.3/grizzly/listeners/influxdb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/locust.py` & `grizzly-loadtester-2.6.3/grizzly/locust.py`

 * *Files 2% similar despite different names*

```diff
@@ -401,21 +401,15 @@
 
                 def watch_running_external_processes() -> None:
                     while runner.user_count > 0:
                         _processes = processes.copy()
                         for dependency, process in _processes.items():
                             if process.poll() is not None:
                                 logger.error(f'{dependency} is not running, restarting')
-                                processes.update({dependency: subprocess.Popen(
-                                    [dependency],
-                                    env=env,
-                                    shell=False,
-                                    stdout=subprocess.DEVNULL,
-                                    stderr=subprocess.DEVNULL,
-                                )})
+                                raise SystemExit(1)
 
                         gevent.sleep(10.0)
 
                     logger.info('stop watching external processes')
 
                 return watch_running_external_processes
 
@@ -597,15 +591,19 @@
 def _grizzly_sort_stats(stats: lstats.RequestStats) -> List[Tuple[str, str, int]]:
     locust_keys: List[Tuple[str, str]] = sorted(stats.entries.keys())
 
     previous_ident: Optional[str] = None
     scenario_keys: List[Tuple[str, str]] = []
     scenario_sorted_keys: List[Tuple[str, str, int]] = []
     for index, key in enumerate(locust_keys):
-        ident, _ = key[0].split(' ', 1)
+        try:
+            ident, _ = key[0].split(' ', 1)
+        except ValueError:
+            ident = '999'
+
         is_last = index == len(locust_keys) - 1
         if (previous_ident is not None and previous_ident != ident) or is_last:
             if is_last:
                 scenario_keys.append(key[:2])
 
             scenario_sorted_keys += sorted([
                 (name, method, RequestType.get_method_weight(method), ) for name, method in scenario_keys
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/scenarios/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/scenarios/iterator.py` & `grizzly-loadtester-2.6.3/grizzly/scenarios/iterator.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/_helpers.py` & `grizzly-loadtester-2.6.3/grizzly/steps/_helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/background/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/steps/background/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/background/setup.py` & `grizzly-loadtester-2.6.3/grizzly/steps/background/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/background/shapes.py` & `grizzly-loadtester-2.6.3/grizzly/steps/background/shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/scenario/response.py` & `grizzly-loadtester-2.6.3/grizzly/steps/scenario/response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/scenario/results.py` & `grizzly-loadtester-2.6.3/grizzly/steps/scenario/results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/scenario/setup.py` & `grizzly-loadtester-2.6.3/grizzly/steps/scenario/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/scenario/tasks.py` & `grizzly-loadtester-2.6.3/grizzly/steps/scenario/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -338,42 +338,77 @@
         content=content,
         content_type=content_type,
         expression=expression,
         variable=variable,
     ))
 
 
-@then(u'get "{endpoint}" with name "{name}" and save response in "{variable}"')
-def step_task_client_get_endpoint(context: Context, endpoint: str, name: str, variable: str) -> None:
+@then(u'get "{endpoint}" with name "{name}" and save response payload in "{payload_variable}" and metadata in "{metadata_variable}"')
+def step_task_client_get_endpoint_payload_metadata(context: Context, endpoint: str, name: str, payload_variable: str, metadata_variable: str) -> None:
     """
     Creates an instance of a {@pylink grizzly.tasks.clients} task, actual implementation of the task is determined
     based on the URL scheme specified in `endpoint`. Gets information from another host or endpoint than the scenario
     is load testing and saves the response in a variable.
 
     See {@pylink grizzly.tasks.clients} task documentation for more information about client tasks.
 
     Example:
 
     ``` gherkin
-    Then get "https://www.example.org/example.json" with name "example-1" and save response in "example_openapi"
-    Then get "http://{{ endpoint }}" with name "example-2" and save response in "endpoint_result"
+    Then get "https://www.example.org/example.json" with name "example-1" and save response payload in "example_openapi" and metadata in "example_metadata"
+    Then get "http://{{ endpoint }}" with name "example-2" and save response payload in "endpoint_result" and metadata in "result_metadata"
     ```
 
     Args:
         endpoint (str): information about where to get information, see the specific getter task implementations for more information
         name (str): name of the request, used in request statistics
-        variable (str): name of, initialized, variable where response will be saved in
+        payload_variable (str): name of, initialized, variable where response payload will be saved in
+        metadata_variable (str): name of, initialized, variable where response metadata will be saved in
     """
     grizzly = cast(GrizzlyContext, context.grizzly)
 
     grizzly.scenario.tasks.add(get_task_client(endpoint)(
         RequestDirection.FROM,
         endpoint,
         name,
-        variable=variable,
+        payload_variable=payload_variable,
+        metadata_variable=metadata_variable,
+        text=context.text,
+    ))
+
+
+@then(u'get "{endpoint}" with name "{name}" and save response payload in "{variable}"')
+def step_task_client_get_endpoint_payload(context: Context, endpoint: str, name: str, variable: str) -> None:
+    """
+    Creates an instance of a {@pylink grizzly.tasks.clients} task, actual implementation of the task is determined
+    based on the URL scheme specified in `endpoint`. Gets information from another host or endpoint than the scenario
+    is load testing and saves the response in a variable.
+
+    See {@pylink grizzly.tasks.clients} task documentation for more information about client tasks.
+
+    Example:
+
+    ``` gherkin
+    Then get "https://www.example.org/example.json" with name "example-1" and save response payload in "example_openapi"
+    Then get "http://{{ endpoint }}" with name "example-2" and save response payload in "endpoint_result"
+    ```
+
+    Args:
+        endpoint (str): information about where to get information, see the specific getter task implementations for more information
+        name (str): name of the request, used in request statistics
+        variable (str): name of, initialized, variable where response payload will be saved in
+    """
+    grizzly = cast(GrizzlyContext, context.grizzly)
+
+    grizzly.scenario.tasks.add(get_task_client(endpoint)(
+        RequestDirection.FROM,
+        endpoint,
+        name,
+        payload_variable=variable,
+        metadata_variable=None,
         text=context.text,
     ))
 
 
 @then(u'get "{endpoint}" with name "{name}" until "{condition}"')
 def step_task_client_get_endpoint_until(context: Context, endpoint: str, name: str, condition: str) -> None:
     """
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/scenario/user.py` & `grizzly-loadtester-2.6.3/grizzly/steps/scenario/user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/steps/setup.py` & `grizzly-loadtester-2.6.3/grizzly/steps/setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/async_group.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/async_group.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/clients/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/clients/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,28 +50,30 @@
         RequestDirection.TO: '->',
     }
 
     grizzly: GrizzlyContext
     direction: RequestDirection
     endpoint: str
     name: Optional[str]
-    variable: Optional[str]
+    payload_variable: Optional[str]
+    metadata_variable: Optional[str]
     source: Optional[str]
     destination: Optional[str]
     _text: Optional[str]
 
     log_dir: Path
 
     def __init__(
         self,
         direction: RequestDirection,
         endpoint: str,
         name: Optional[str] = None,
         /,
-        variable: Optional[str] = None,
+        payload_variable: Optional[str] = None,
+        metadata_variable: Optional[str] = None,
         source: Optional[str] = None,
         destination: Optional[str] = None,
         text: Optional[str] = None,
         scenario: Optional[GrizzlyContextScenario] = None,
     ) -> None:
         super().__init__(scenario)
 
@@ -110,26 +112,33 @@
 
             endpoint = value
 
         self.content_type = content_type
         self.direction = direction
         self.endpoint = endpoint
         self.name = name
-        self.variable = variable
+        self.payload_variable = payload_variable
+        self.metadata_variable = metadata_variable
         self.source = source
         self.destination = destination
 
-        if self.variable is not None and self.direction != RequestDirection.FROM:
+        if self.payload_variable is not None and self.direction != RequestDirection.FROM:
             raise AttributeError(f'{self.__class__.__name__}: variable argument is not applicable for direction {self.direction.name}')
 
         if self.source is not None and self.direction != RequestDirection.TO:
             raise AttributeError(f'{self.__class__.__name__}: source argument is not applicable for direction {self.direction.name}')
 
-        if self.variable is not None and self.variable not in self.grizzly.state.variables:
-            raise ValueError(f'{self.__class__.__name__}: variable {self.variable} has not been initialized')
+        if self.payload_variable is not None and self.payload_variable not in self.grizzly.state.variables:
+            raise ValueError(f'{self.__class__.__name__}: variable {self.payload_variable} has not been initialized')
+
+        if self.metadata_variable is not None and self.metadata_variable not in self.grizzly.state.variables:
+            raise ValueError(f'{self.__class__.__name__}: variable {self.metadata_variable} has not been initialized')
+
+        if self.payload_variable is None and self.metadata_variable is not None:
+            raise ValueError(f'{self.__class__.__name__}: payload variable is not set, but metadata variable is set')
 
         if self.source is None and self.direction == RequestDirection.TO:
             raise ValueError(f'{self.__class__.__name__}: source must be set for direction {self.direction.name}')
 
         self._short_name = self.__class__.__name__.replace('ClientTask', '')
 
         context_root = environ.get('GRIZZLY_CONTEXT_ROOT', None)
@@ -151,18 +160,23 @@
         raise NotImplementedError(f'{self.__class__.__name__} has not implemented support for step text')
 
     text = property(text_fget, text_fset)
     # EOW
 
     @property
     def variable_template(self) -> Optional[str]:
-        if self.variable is None or ('{{' in self.variable and '}}' in self.variable):
-            return self.variable
+        if self.payload_variable is None or ('{{' in self.payload_variable and '}}' in self.payload_variable):
+            return self.payload_variable
+
+        template = f'{{{{ {self.payload_variable} }}}}'
+
+        if self.metadata_variable is not None:
+            template = f'{template} {{{{ {self.metadata_variable} }}}}'
 
-        return f'{{{{ {self.variable} }}}}'
+        return template
 
     @final
     def __call__(self) -> grizzlytask:
         @grizzlytask
         def task(parent: 'GrizzlyScenario') -> GrizzlyResponse:
             if self.direction == RequestDirection.FROM:
                 return self.get(parent)
@@ -200,15 +214,15 @@
         try:
             # get metadata back from actual implementation
             yield meta
         except Exception as e:
             exception = e
         finally:
             if self.name is None:
-                action = action or meta.get('action', self.variable)
+                action = action or meta.get('action', self.payload_variable)
                 name = f'{parent.user._scenario.identifier} {self._short_name}{meta.get("direction", self._direction_arrow[self.direction])}{action}'
             else:
                 rendered_name = parent.render(self.name)
                 name = f'{parent.user._scenario.identifier} {rendered_name}'
 
             response_time = int((time() - start_time) * 1000)
             response_length = meta.get('response_length', None) or 0
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/clients/blobstorage.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/clients/blobstorage.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,25 +72,27 @@
 
     def __init__(
         self,
         direction: RequestDirection,
         endpoint: str,
         name: Optional[str] = None,
         /,
-        variable: Optional[str] = None,
+        payload_variable: Optional[str] = None,
+        metadata_variable: Optional[str] = None,
         source: Optional[str] = None,
         destination: Optional[str] = None,
         text: Optional[str] = None,
         scenario: Optional[GrizzlyContextScenario] = None,
     ) -> None:
         super().__init__(
             direction,
             endpoint,
             name,
-            variable=variable,
+            payload_variable=payload_variable,
+            metadata_variable=metadata_variable,
             destination=destination,
             source=source,
             scenario=scenario,
             text=text,
         )
 
         parsed = urlparse(self.endpoint)
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/clients/http.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/clients/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 This is useful if the scenario is using a non-HTTP user or a request to a URL other than the one under testing is needed, e.g. for testdata.
 
 Only supports `RequestDirection.FROM`.
 
 ## Step implementations
 
-* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint}
+* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint_payload}
+
+* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint_payload_metadata}
 
 ## Arguments
 
 * `direction` _RequestDirection_ - only `RequestDirection.FROM` is implemented
 
 * `endpoint` _str_ - URL to perform GET request from
 
 * `name` _str_ - name used in `locust` statistics
 '''
 from typing import Optional, Dict, Any
+from json import dumps as jsondumps
 
 import requests
 
 from locust.exception import CatchResponseError
 from grizzly_extras.arguments import split_value, parse_arguments
 
 from grizzly.types import GrizzlyResponse, RequestDirection, bool_type
@@ -37,15 +40,16 @@
 
     def __init__(
         self,
         direction: RequestDirection,
         endpoint: str,
         name: Optional[str] = None,
         /,
-        variable: Optional[str] = None,
+        payload_variable: Optional[str] = None,
+        metadata_variable: Optional[str] = None,
         source: Optional[str] = None,
         destination: Optional[str] = None,
         text: Optional[str] = None,
         scenario: Optional[GrizzlyContextScenario] = None,
     ) -> None:
         verify = True
 
@@ -60,15 +64,16 @@
             if len(arguments) > 0:
                 endpoint = f'{endpoint} | {", ".join([f"{key}={value}" for key, value in arguments.items()])}'
 
         super().__init__(
             direction,
             endpoint,
             name,
-            variable=variable,
+            payload_variable=payload_variable,
+            metadata_variable=metadata_variable,
             source=source,
             destination=destination,
             scenario=scenario,
             text=text,
         )
 
         self.arguments = {}
@@ -86,31 +91,37 @@
             meta.update({'request': {
                 'url': url,
                 'metadata': self.headers,
                 'payload': None,
             }})
 
             response = requests.get(url, headers=self.headers, **self.arguments)
-            value = response.text
-            if self.variable is not None:
-                parent.user._context['variables'][self.variable] = value
-            meta['response_length'] = len(value.encode('utf-8'))
+            payload = response.text
+            metadata = dict(response.headers)
+
+            if self.payload_variable is not None:
+                parent.user._context['variables'][self.payload_variable] = payload
+
+            if self.metadata_variable is not None:
+                parent.user._context['variables'][self.metadata_variable] = jsondumps(metadata)
+
+            meta['response_length'] = len(payload.encode('utf-8'))
 
             exception: Optional[Exception] = None
 
             if response.status_code != 200:
-                exception = CatchResponseError(f'{response.status_code} not in [200]: {value}')
+                exception = CatchResponseError(f'{response.status_code} not in [200]: {payload}')
 
             meta.update({
                 'response': {
                     'url': response.url,
-                    'metadata': dict(response.headers),
-                    'payload': value,
+                    'metadata': metadata,
+                    'payload': payload,
                     'status': response.status_code,
                 },
                 'exception': exception,
             })
 
-            return dict(response.headers), value
+            return metadata, payload
 
     def put(self, parent: GrizzlyScenario) -> GrizzlyResponse:
         raise NotImplementedError(f'{self.__class__.__name__} has not implemented PUT')
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/clients/messagequeue.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/clients/messagequeue.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 ``` plain
 pip3 install grizzly-loadtester[mq]
 ```
 
 ## Step implementations
 
-* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint}
+* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint_payload}
+
+* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint_payload_metadata}
 
 * {@pylink grizzly.steps.scenario.tasks.step_task_client_put_endpoint_file}
 
 ## Arguments
 
 * `direction` _RequestDirection_ - if the request is upstream or downstream
 
@@ -69,22 +71,22 @@
 * `MaxMessageSize` _int_ (optional) - maximum number of bytes a message can be for the client to accept it, default is `None` which implies that the client will throw `MQRC_TRUNCATED_MSG_FAILED`, adjust buffer and try again.
 '''  # noqa: E501
 from contextlib import contextmanager
 from typing import Optional, Dict, Any, Generator, List, cast
 from urllib.parse import urlparse, parse_qs, unquote
 from pathlib import Path
 from platform import node as hostname
+from json import dumps as jsondumps
 
 import zmq.green as zmq
 
-from zmq.error import Again as ZMQAgain, ZMQError
-from zmq.sugar.constants import NOBLOCK as ZMQ_NOBLOCK, REQ as ZMQ_REQ, LINGER as ZMQ_LINGER
+from zmq.error import ZMQError
+from zmq.sugar.constants import REQ as ZMQ_REQ, LINGER as ZMQ_LINGER
 
-from gevent import sleep as gsleep
-from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageResponse, AsyncMessageRequest
+from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageResponse, AsyncMessageRequest, async_message_request
 
 from grizzly.types import GrizzlyResponse, RequestDirection, RequestType
 from grizzly.context import GrizzlyContextScenario
 from grizzly.scenarios import GrizzlyScenario
 from grizzly.testdata.utils import resolve_variable
 
 from . import client, ClientTask, logger
@@ -110,15 +112,16 @@
 
     def __init__(
         self,
         direction: RequestDirection,
         endpoint: str,
         name: Optional[str] = None,
         /,
-        variable: Optional[str] = None,
+        payload_variable: Optional[str] = None,
+        metadata_variable: Optional[str] = None,
         source: Optional[str] = None,
         destination: Optional[str] = None,
         text: Optional[str] = None,
         scenario: Optional[GrizzlyContextScenario] = None,
     ) -> None:
         if pymqi.__name__ == 'grizzly_extras.dummy_pymqi':
             pymqi.raise_for_error(self.__class__)
@@ -126,15 +129,16 @@
         if destination is not None:
             raise ValueError(f'{self.__class__.__name__}: destination is not allowed')
 
         super().__init__(
             direction,
             endpoint,
             name,
-            variable=variable,
+            payload_variable=payload_variable,
+            metadata_variable=metadata_variable,
             destination=destination,
             source=source,
             scenario=scenario,
             text=text,
         )
 
         self.create_context()
@@ -245,88 +249,67 @@
             raise
         finally:
             if client is not None:
                 client.setsockopt(ZMQ_LINGER, 0)
                 client.close()
 
     def connect(self, client_id: int, client: zmq.Socket, meta: Dict[str, Any]) -> None:
-        request = {
+        request: AsyncMessageRequest = {
             'action': RequestType.CONNECT(),
+            'client': client_id,
             'context': self.context,
         }
 
         meta.update({'action': self.endpoint_path, 'direction': '<->'})
+        response: Optional[AsyncMessageResponse] = None
 
-        client.send_json(request)
-
-        response = None
-
-        while True:
-            try:
-                response = client.recv_json(flags=ZMQ_NOBLOCK)
-                break
-            except ZMQAgain:
-                gsleep(0.1)
-
-        meta.update({'response_length': len((response or {}).get('payload', None) or '')})
-
-        if response is None:
-            raise RuntimeError('no response when trying to connect')
-
-        message = response.get('message', None)
-        if not response['success']:
-            raise RuntimeError(message)
+        try:
+            response = async_message_request(client, request)
+        except:
+            raise
+        finally:
+            meta.update({'response_length': len((response or {}).get('payload', None) or '')})
 
         self._worker.update({client_id: response['worker']})
 
     def request(self, parent: GrizzlyScenario, request: AsyncMessageRequest) -> AsyncMessageResponse:
         with self.create_client() as client:
-            client_id = id(parent)
+            client_id = id(parent.user)
             worker = self._worker.get(client_id, None)
             if worker is None:
                 with self.action(parent, suppress=True) as meta:
                     self.connect(client_id, client, meta)
                     worker = self._worker.get(client_id, None)
                     parent.logger.debug(f'connected to worker {worker} at {hostname()}')
 
             if worker is None:
                 raise RuntimeError(f'{parent.__class__.__name__}/{client_id} was unable to get an worker assigned')
 
             with self.action(parent) as meta:
-                request['worker'] = worker
-
-                client.send_json(request)
-
-                response = None
-
-                parent.logger.debug(f'waiting for response from {worker} at {hostname()}')
-                while True:
-                    try:
-                        response = cast(AsyncMessageResponse, client.recv_json(flags=ZMQ_NOBLOCK))
-                        break
-                    except ZMQAgain:
-                        gsleep(0.1)
-
-                parent.logger.debug(f'got response from {worker} at {hostname()}')
-
-                response_length_source = ((response or {}).get('payload', None) or '').encode('utf-8')
-
-                meta.update({
-                    'action': self.endpoint_path,
-                    'request': request.copy(),
-                    'response_length': len(response_length_source),
-                    'response': response,
+                request.update({
+                    'worker': worker,
+                    'client': client_id,
                 })
+                response: Optional[AsyncMessageResponse] = None
 
-                if response is None:
-                    raise RuntimeError('no response')
+                try:
+                    response = async_message_request(client, request)
 
-                message = response.get('message', None)
-                if not response['success']:
-                    raise RuntimeError(message)
+                    parent.logger.debug(f'got response from {worker} at {hostname()}')
+                except:
+                    raise
+                finally:
+                    response_length_source = ((response or {}).get('payload', None) or '').encode('utf-8')
+
+                    meta.update({
+                        'action': self.endpoint_path,
+                        'request': request.copy(),
+                        'response_length': len(response_length_source),
+                        'response': response,
+                    })
 
                 payload = response.get('payload', None)
                 if payload is None or len(payload) < 1:
                     raise RuntimeError('response did not contain any payload')
 
                 return response
 
@@ -341,16 +324,20 @@
             'context': {
                 'endpoint': ', '.join(endpoint),
             },
             'payload': None,
         }
         response = self.request(parent, request)
 
-        if response is not None and self.variable is not None:
-            parent.user._context['variables'][self.variable] = response['payload']
+        if response is not None:
+            if self.payload_variable is not None and response.get('payload', None) is not None:
+                parent.user._context['variables'][self.payload_variable] = response['payload']
+
+            if self.metadata_variable is not None and response.get('metadata', None) is not None:
+                parent.user._context['variables'][self.metadata_variable] = jsondumps(response['metadata'])
 
         response = response or {}
 
         return response.get('metadata', None), response.get('payload', None)
 
     def put(self, parent: GrizzlyScenario) -> GrizzlyResponse:
         source = parent.render(cast(str, self.source))
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/clients/servicebus.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/clients/servicebus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=line-too-long
 """This task performs Azure SerciceBus operations to a specified endpoint.
 
-
 ## Step implementations
 
-* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint}
+* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint_payload}
+
+* {@pylink grizzly.steps.scenario.tasks.step_task_client_get_endpoint_payload_metadata}
 
 * {@pylink grizzly.steps.scenario.tasks.step_task_client_put_endpoint_file}
 
 ## Arguments
 
 * `direction` _RequestDirection_ - if the request is upstream or downstream
 
@@ -38,15 +39,15 @@
 
 Path:
 
 * `<queue name>` _str_ - name of queue, prefixed with `queue:` of an existing queue (mutual exclusive<sup>1</sup>)
 
 * `<topic name>` _str_ - name of topic, prefixed with `topic:` of an existing topic (mutual exclusive<sup>1</sup>)
 
-* `<subscription name>` _str_ - name of an subscription on `topic name`, either an existing, or one to be created (if step text containing SQL Filter rule is specified)
+* `<subscription name>` _str_ - name of an subscription on `topic name`, either an existing, or one to be created (if step text containing SQL Filter rule is specified), the actual subscription name will be suffixed with unique id related to the user instance
 
 * `<expression>` _str_ - JSON or XPath expression to filter out message on payload, only applicable when receiving messages
 
 <sup>1</sup> Either specify `queue:` or `topic`, not both
 
 Query:
 
@@ -63,21 +64,23 @@
 * `<content type>` _str_ - content type of response payload, should be used in combination with `<expression>`
 """  # noqa: E501
 from typing import Optional, cast
 from urllib.parse import urlparse, parse_qs
 from platform import node as hostname
 from pathlib import Path
 from textwrap import dedent
+from json import dumps as jsondumps
 
 import zmq.green as zmq
 
 from zmq.sugar.constants import REQ as ZMQ_REQ, LINGER as ZMQ_LINGER
 
 from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageRequest, AsyncMessageResponse
 from grizzly_extras.transformer import TransformerContentType
+from grizzly_extras.arguments import parse_arguments
 
 from grizzly.types import GrizzlyResponse, RequestDirection, RequestType
 from grizzly.context import GrizzlyContextScenario
 from grizzly.scenarios import GrizzlyScenario
 from grizzly.tasks import template
 from grizzly.utils import async_message_request_wrapper
 
@@ -92,28 +95,40 @@
     _zmq_url = 'tcp://127.0.0.1:5554'
     _zmq_context: zmq.Context
 
     _client: Optional[zmq.Socket] = None
     worker_id: Optional[str]
     context: AsyncMessageContext
     _parent: Optional[GrizzlyScenario]
+    _first_response: Optional[AsyncMessageResponse]
 
     def __init__(
         self,
         direction: RequestDirection,
         endpoint: str,
         name: Optional[str] = None,
         /,
-        variable: Optional[str] = None,
+        payload_variable: Optional[str] = None,
+        metadata_variable: Optional[str] = None,
         source: Optional[str] = None,
         destination: Optional[str] = None,
         text: Optional[str] = None,
         scenario: Optional[GrizzlyContextScenario] = None,
     ) -> None:
-        super().__init__(direction, endpoint, name, variable=variable, destination=destination, source=source, text=text, scenario=scenario)
+        super().__init__(
+            direction,
+            endpoint,
+            name,
+            payload_variable=payload_variable,
+            metadata_variable=metadata_variable,
+            destination=destination,
+            source=source,
+            text=text,
+            scenario=scenario,
+        )
 
         url = self.endpoint.replace(';', '?', 1).replace(';', '&')
 
         parsed = urlparse(url)
 
         self.endpoint = f'{parsed.scheme}://{parsed.netloc}/;{parsed.query.replace("&", ";")}'
         self._parent = None
@@ -152,14 +167,16 @@
             'message_wait': message_wait,
             'consume': consume,
         }
 
         if content_type is not None:
             self.context.update({'content_type': content_type})
 
+        self._first_response = None
+
         # zmq connection to async-messaged must be done when creating the instance
         self._client = cast(zmq.Socket, self._zmq_context.socket(ZMQ_REQ))
         self.client.connect(self._zmq_url)
 
     @property
     def parent(self) -> GrizzlyScenario:
         if self._parent is None:
@@ -183,29 +200,40 @@
 
     @ClientTask.text.setter  # type: ignore
     def text(self, value: str) -> None:
         self._text = dedent(value).strip()
 
     def connect(self) -> None:
         if self.worker_id is not None:
+            logger.debug(f'{id(self.parent.user)}::sb already connected')
             return
 
+        if self._first_response is not None:
+            self.worker_id = self._first_response.get('worker', None)
+
+        logger.debug(f'{id(self.parent.user)}::sb connecting, {self.worker_id=}')
+
         request: AsyncMessageRequest = {
             'worker': self.worker_id,
             'action': RequestType.HELLO.name,
             'context': self.context,
         }
 
         response = async_message_request_wrapper(self.parent, self.client, request)
 
-        self.worker_id = response['worker']
+        if self._first_response is None:
+            self.worker_id = response['worker']
+            self._first_response = response
 
-        logger.debug(f'connected to worker {self.worker_id} at {hostname()}')
+        logger.debug(f'{id(self.parent.user)}::sb connected to worker {self.worker_id} at {hostname()}')
 
     def disconnect(self) -> None:
+        if self._client is None:
+            return
+
         request: AsyncMessageRequest = {
             'worker': self.worker_id,
             'action': RequestType.DISCONNECT.name,
             'context': self.context,
         }
 
         async_message_request_wrapper(self.parent, self.client, request)
@@ -222,14 +250,16 @@
             'context': self.context,
             'payload': self.text,
         }
 
         response = async_message_request_wrapper(self.parent, self.client, request)
         logger.info(response['message'])
 
+        self._first_response = response
+
     def unsubscribe(self) -> None:
         request: AsyncMessageRequest = {
             'worker': self.worker_id,
             'action': RequestType.UNSUBSCRIBE.name,
             'context': self.context,
         }
 
@@ -237,14 +267,21 @@
         logger.info(response['message'])
 
     def on_start(self, parent: GrizzlyScenario) -> None:
         self.parent = parent
 
         # create subscription before connecting to it
         if self.text is not None:
+            # add id of user as suffix to subscription name, to make it unique
+            endpoint_arguments = parse_arguments(self.context['endpoint'], separator=':')
+
+            if 'subscription' in endpoint_arguments:
+                endpoint_arguments['subscription'] = f'{endpoint_arguments["subscription"]}_{id(self.parent)}'
+                self.context['endpoint'] = ', '.join([f'{key}:{value}' for key, value in endpoint_arguments.items()])
+
             self.subscribe()
 
         self.connect()
 
     def on_stop(self, parent: GrizzlyScenario) -> None:
         self.parent = parent
 
@@ -282,16 +319,19 @@
         }
 
         response = self.request(parent, request)
 
         metadata = response.get('metadata', None)
         payload = response.get('payload', None)
 
-        if payload is not None and self.variable is not None:
-            parent.user._context['variables'][self.variable] = payload
+        if payload is not None and self.payload_variable is not None:
+            parent.user._context['variables'][self.payload_variable] = payload
+
+        if metadata is not None and self.metadata_variable is not None:
+            parent.user._context['variables'][self.metadata_variable] = jsondumps(metadata)
 
         return metadata, payload
 
     def put(self, parent: GrizzlyScenario) -> GrizzlyResponse:
         source = parent.render(cast(str, self.source))
         source_file = Path(self._context_root) / 'requests' / source
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/conditional.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/conditional.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ## Arguments
 
 * `name` _str_: name of the conditional, used in `locust` statistics
 
 * `condition` _str_: {@link framework.usage.variables.templating} string that must render `True` or `False`
 """
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Dict
+from typing import TYPE_CHECKING, Any, List, Optional, Dict
 from time import perf_counter
 
 from gevent import sleep as gsleep
 
 from grizzly.exceptions import StopUser, RestartScenario
 
 from . import GrizzlyTask, GrizzlyTaskWrapper, template, grizzlytask
@@ -83,15 +83,15 @@
     def peek(self) -> List[GrizzlyTask]:
         if self._pointer is not None:
             return self.tasks[self._pointer]
 
         return []
 
     def __call__(self) -> grizzlytask:
-        tasks: Dict[bool, List[Callable[['GrizzlyScenario'], Any]]] = {}
+        tasks: Dict[bool, List[grizzlytask]] = {}
 
         for pointer, pointer_tasks in self.tasks.items():
             tasks.update({pointer: list(map(lambda t: t(), pointer_tasks))})
 
         @grizzlytask
         def task(parent: 'GrizzlyScenario') -> Any:
             condition_rendered = parent.render(self.condition)
@@ -137,8 +137,18 @@
                 else:
                     stats = parent.user.environment.stats.get(name, 'COND')
                     stats.log_error(None)
 
                 if exception is not None and self.scenario.failure_exception is not None:
                     raise self.scenario.failure_exception()
 
+        @task.on_start
+        def on_start(parent: 'GrizzlyScenario') -> None:
+            for task in tasks.get(True, []) + tasks.get(False, []):
+                task.on_start(parent)
+
+        @task.on_stop
+        def on_stop(parent: 'GrizzlyScenario') -> None:
+            for task in tasks.get(True, []) + tasks.get(False, []):
+                task.on_stop(parent)
+
         return task
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/date.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/log_message.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/log_message.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/loop.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/loop.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,28 +92,32 @@
                         task(parent)
                         gsleep(parent.user.wait_time())
 
                     parent.user._context['variables'].update({self.variable: orig_value})
             except Exception as e:
                 exception = e
             finally:
-                if orig_value is None:
-                    try:
-                        del parent.user._context['variables'][self.variable]
-                    except:
-                        pass
-
                 response_time = int((perf_counter() - start) * 1000)
 
                 parent.user.environment.events.request.fire(
                     request_type='LOOP',
                     name=f'{self.scenario.identifier} {self.name} ({task_count})',
                     response_time=response_time,
                     response_length=response_length,
                     context=parent.user._context,
                     exception=exception,
                 )
 
                 if exception is not None and self.scenario.failure_exception is not None:
                     raise self.scenario.failure_exception()
 
+        @task.on_start
+        def on_start(parent: 'GrizzlyScenario') -> None:
+            for task in tasks:
+                task.on_start(parent)
+
+        @task.on_stop
+        def on_stop(parent: 'GrizzlyScenario') -> None:
+            for task in tasks:
+                task.on_stop(parent)
+
         return task
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/request.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/request.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/set_variable.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/set_variable.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/task_wait.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/task_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/timer.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/timer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/transformer.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/transformer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/until.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/until.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,59 +39,34 @@
 
 * `expected_matches` _int_ (optional): number of matches that the expression should match (default `1`)
 
 """
 import json
 import logging
 
-from typing import TYPE_CHECKING, Callable, Any, Type, List, Optional, Generator, Dict, cast
+from typing import TYPE_CHECKING, Callable, Any, Type, List, Optional, cast
 from time import perf_counter
-from contextlib import contextmanager
 
 from jinja2 import Template
 from gevent import sleep as gsleep
 from grizzly_extras.transformer import Transformer, TransformerContentType, TransformerError, transformer
 from grizzly_extras.arguments import get_unsupported_arguments, parse_arguments, split_value
 
-from grizzly.types.locust import Environment
 from grizzly.types import RequestType
 
 from . import GrizzlyTask, GrizzlyMetaRequestTask, template, grizzlytask
 
 if TYPE_CHECKING:  # pragma: no cover
     from grizzly.context import GrizzlyContextScenario, GrizzlyContext
     from grizzly.scenarios import GrizzlyScenario
 
 
 logger = logging.getLogger(__name__)
 
 
-def no_error_handler(environment: Environment) -> Callable[..., None]:
-    def no_error_handler_wrapper(request_type: str, name: str, response_time: int, response_length: int, exception: Optional[Exception] = None, **_kwargs: Dict[str, Any]) -> None:
-        environment.stats.log_request(request_type, name, response_time, response_length)
-
-        if exception is not None:
-            logger.error(f'{request_type} {name}: {response_time=}, {response_length=}, {exception=}')
-            environment.stats.total.log_error(None)
-            environment.stats.get(name, request_type).log_error(None)
-
-    return no_error_handler_wrapper
-
-
-@contextmanager
-def suppress(environment: Environment) -> Generator[None, None, None]:
-    original_handlers = environment.events.request._handlers.copy()
-    environment.events.request._handlers = [no_error_handler(environment)]
-
-    try:
-        yield
-    finally:
-        environment.events.request._handlers = original_handlers
-
-
 @template('condition', 'request')
 class UntilRequestTask(GrizzlyTask):
     request: GrizzlyMetaRequestTask
     condition: str
 
     transform: Optional[Type[Transformer]]
     matcher: Callable[[Any], List[str]]
@@ -163,16 +138,15 @@
             try:
                 while retry < self.retries:
                     number_of_matches = 0
 
                     try:
                         gsleep(self.wait)
 
-                        with suppress(parent.user.environment):
-                            _, payload = self.request.execute(parent)
+                        _, payload = self.request.execute(parent)
 
                         if payload is not None:
                             transformed = transform.transform(payload)
                             response_length += len(payload)
                         else:
                             raise TransformerError('response payload was not set')
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/tasks/wait.py` & `grizzly-loadtester-2.6.3/grizzly/tasks/wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/ast.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/ast.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,17 @@
         # can raise TemplateError which should be handled else where
         for template in template_sources:
             j2env = Jinja2Environment(
                 autoescape=False,
                 loader=Jinja2FileSystemLoader('.'),
             )
 
+            # json.dumps escapes quote (") causing it to be \\", which inturn causes problems for jinja
+            template = template.replace('\\"', "'")
+
             parsed = j2env.parse(template)
 
             for body in getattr(parsed, 'body', []):
                 for node in getattr(body, 'nodes', []):
                     for attributes in _getattr(node):
                         variables[scenario_name].add('.'.join(attributes))
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/communication.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/communication.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/utils.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/csv_reader.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_reader.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/csv_writer.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/csv_writer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/date.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/directory_contents.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/directory_contents.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/integer_incrementer.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/integer_incrementer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/random_integer.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_integer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/testdata/variables/random_string.py` & `grizzly-loadtester-2.6.3/grizzly/testdata/variables/random_string.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/types/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/types/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/types/locust.py` & `grizzly-loadtester-2.6.3/grizzly/types/locust.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/users/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/base/__init__.py` & `grizzly-loadtester-2.6.3/grizzly/users/base/__init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/base/grizzly_user.py` & `grizzly-loadtester-2.6.3/grizzly/users/base/grizzly_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/base/request_logger.py` & `grizzly-loadtester-2.6.3/grizzly/users/base/request_logger.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/base/response_event.py` & `grizzly-loadtester-2.6.3/grizzly/users/base/response_event.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/base/response_handler.py` & `grizzly-loadtester-2.6.3/grizzly/users/base/response_handler.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/blobstorage.py` & `grizzly-loadtester-2.6.3/grizzly/users/blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/dummy.py` & `grizzly-loadtester-2.6.3/grizzly/users/dummy.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/iothub.py` & `grizzly-loadtester-2.6.3/grizzly/users/iothub.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/messagequeue.py` & `grizzly-loadtester-2.6.3/grizzly/users/messagequeue.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,25 +119,23 @@
 ``` gherkin
 Then put request "test/queue-message.j2.json" with name "gzipped-message" to endpoint "queue:GZIPPED.MESSAGES"
 And metadata "filename" is "my_filename"
 ```
 '''
 import logging
 
-from typing import Dict, Any, Generator, Tuple, Optional, cast
+from typing import Dict, Any, Generator, Tuple, Optional
 from urllib.parse import urlparse, parse_qs, unquote
 from contextlib import contextmanager
 from time import perf_counter as time
 
-from zmq.sugar.constants import NOBLOCK as ZMQ_NOBLOCK, REQ as ZMQ_REQ
-from zmq.error import Again as ZMQAgain
+from zmq.sugar.constants import REQ as ZMQ_REQ
 import zmq.green as zmq
 
-from gevent import sleep as gsleep
-from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageRequest, AsyncMessageResponse, AsyncMessageError
+from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageRequest, AsyncMessageResponse, async_message_request
 from grizzly_extras.arguments import get_unsupported_arguments, parse_arguments
 
 from grizzly.types import GrizzlyResponse, RequestDirection, RequestType
 from grizzly.types.locust import Environment, StopUser
 from grizzly.tasks import RequestTask
 from grizzly.utils import merge_dicts
 
@@ -302,23 +300,15 @@
 
         response: Optional[AsyncMessageResponse] = None
 
         start_time = time()
         try:
             yield action
 
-            self.zmq_client.send_json(am_request)
-
-            # do not block all other "threads", just it self
-            while True:
-                try:
-                    response = cast(AsyncMessageResponse, self.zmq_client.recv_json(flags=ZMQ_NOBLOCK))
-                    break
-                except ZMQAgain:
-                    gsleep(0.1)
+            response = async_message_request(self.zmq_client, am_request)
 
         except Exception as e:
             exception = e
             self.logger.error(str(e), exc_info=True)
         finally:
             total_time = int((time() - start_time) * 1000)  # do not include event handling in request time
 
@@ -329,17 +319,14 @@
                     assert self.worker_id == response['worker'], f'worker changed from {self.worker_id} to {response["worker"]}'
 
                 mq_response_time = response.get('response_time', 0)
 
                 delta = total_time - mq_response_time
                 if delta > 100:  # @TODO: what is a suitable value?
                     logger.warning(f'{self.__class__.__name__}: communicating with async-messaged took {delta} ms')
-
-                if not response['success'] and exception is None:
-                    exception = AsyncMessageError(response['message'])
             else:
                 response = {}
 
             action['metadata'] = response.get('metadata', None)
             action['payload'] = response.get('payload', None)
 
             try:
@@ -381,14 +368,15 @@
         request_name, endpoint, payload, _, metadata = self.render(request)
 
         name = f'{request.scenario.identifier} {request_name}'
 
         am_request: AsyncMessageRequest = {
             'action': request.method.name,
             'worker': self.worker_id,
+            'client': id(self),
             'context': {
                 'endpoint': endpoint,
                 'metadata': metadata,
             },
             'payload': payload,
         }
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/restapi.py` & `grizzly-loadtester-2.6.3/grizzly/users/restapi.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/servicebus.py` & `grizzly-loadtester-2.6.3/grizzly/users/servicebus.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,18 @@
 import logging
 
 from typing import Generator, Dict, Any, Tuple, Optional, Set, cast
 from urllib.parse import urlparse, parse_qs
 from time import perf_counter as time
 from contextlib import contextmanager
 
-from zmq.error import Again as ZMQAgain
-from zmq.sugar.constants import NOBLOCK as ZMQ_NOBLOCK, REQ as ZMQ_REQ
+from zmq.sugar.constants import REQ as ZMQ_REQ
 import zmq.green as zmq
 
-from gevent import sleep as gsleep
-from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageResponse, AsyncMessageRequest, AsyncMessageError
+from grizzly_extras.async_message import AsyncMessageContext, AsyncMessageResponse, AsyncMessageRequest, async_message_request
 from grizzly_extras.arguments import parse_arguments, get_unsupported_arguments
 
 from grizzly.types import RequestMethod, RequestDirection, GrizzlyResponse, RequestType
 from grizzly.types.locust import StopUser, Environment
 from grizzly.tasks import RequestTask
 from grizzly.utils import merge_dicts
 
@@ -209,15 +207,14 @@
 
         context = cast(AsyncMessageContext, dict(self.am_context))
         context.update({
             'endpoint': cache_endpoint,
         })
 
         request: AsyncMessageRequest = {
-            'worker': self.worker_id,
             'action': RequestType.DISCONNECT.name,
             'context': context,
         }
 
         with self.async_action(task, request, description) as metadata:
             metadata.update({
                 'meta': True,
@@ -238,15 +235,14 @@
 
         context = cast(AsyncMessageContext, dict(self.am_context))
         context.update({
             'endpoint': cache_endpoint,
         })
 
         request: AsyncMessageRequest = {
-            'worker': self.worker_id,
             'action': RequestType.HELLO.name,
             'context': context,
         }
 
         with self.async_action(task, request, description) as metadata:
             metadata.update({
                 'meta': True,
@@ -283,15 +279,20 @@
     @contextmanager
     def async_action(self, task: RequestTask, request: AsyncMessageRequest, name: str) -> Generator[Dict[str, Any], None, None]:
         if not name.startswith(f'{self._scenario.identifier} '):
             name = f'{self._scenario.identifier} {name}'
 
         if len(name) > 65:
             name = f'{name[:65]}...'
-        request.update({'worker': self.worker_id})
+
+        request.update({
+            'worker': self.worker_id,
+            'client': id(self),
+        })
+
         connection = 'sender' if task.method.direction == RequestDirection.TO else 'receiver'
         request['context'].update({'connection': connection})
         action: Dict[str, Any] = {
             'failure_exception': None,
             'meta': False,
             'metadata': None,
             'payload': None,
@@ -303,36 +304,26 @@
         exception: Optional[Exception] = None
 
         start_time = time()
 
         try:
             yield action
 
-            self.zmq_client.send_json(request)
-
-            while True:
-                try:
-                    response = cast(AsyncMessageResponse, self.zmq_client.recv_json(flags=ZMQ_NOBLOCK))
-                    break
-                except ZMQAgain:
-                    gsleep(0.1)
+            response = async_message_request(self.zmq_client, request)
         except Exception as e:
             exception = e
         finally:
             response_time = int((time() - start_time) * 1000)
 
             if response is not None:
                 response_worker = response.get('worker', None)
                 if self.worker_id is None:
                     self.worker_id = response_worker
 
                 assert self.worker_id == response_worker
-
-                if not response.get('success', False) and exception is None:
-                    exception = AsyncMessageError(response['message'])
             else:
                 response = {}
 
             action['metadata'] = response.get('metadata', None)
             action['payload'] = response.get('payload', None)
 
             try:
```

### Comparing `grizzly-loadtester-2.6.2/grizzly/users/sftp.py` & `grizzly-loadtester-2.6.3/grizzly/users/sftp.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly/utils.py` & `grizzly-loadtester-2.6.3/grizzly/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,19 @@
     print_table('AMQ FDC files', 'File', amqerr_fdc_files)
 
 
 def async_message_request_wrapper(parent: GrizzlyScenario, client: zmq.Socket, request: AsyncMessageRequest) -> AsyncMessageResponse:
     request_json = jsondumps(request)
     request = jsonloads(parent.render(request_json))
 
+    if request.get('client', None) is None:
+        request.update({'client': id(parent.user)})
+
+    parent.logger.debug(f'{request=}')
+
     return async_message_request(client, request)
 
 
 def safe_del(struct: Dict[str, Any], key: str) -> None:
     try:
         del struct[key]
     except KeyError:
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/arguments.py` & `grizzly-loadtester-2.6.3/grizzly_extras/arguments.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,29 +44,36 @@
         value = value.strip()
 
         if len(value) < 1:
             raise ValueError(f'invalid value for argument "{key}"')
 
         start_quote: Optional[str] = None
 
-        if value[0] in ['"', "'"]:
-            if value[-1] != value[0]:
+        inline_quotes = '==' in value and value.index('==') == value.rindex('==') and '?' not in value and '@' not in value
+
+        if not inline_quotes:
+            start_index = 0
+        else:
+            start_index = value.index('==') + 2  # == = 2 characters
+
+        if value[start_index] in ['"', "'"]:
+            if value[-1] != value[start_index]:
                 if previous_part is None and part_index < len(argument_parts) - 1:
                     previous_part = argument
                     continue
 
                 raise ValueError(f'value is incorrectly quoted: "{value}"')
-            start_quote = value[0]
-            if unquote:
+            start_quote = value[start_index]
+            if unquote and start_index == 0:
                 value = value[1:]
 
         if value[-1] in ['"', "'"]:
             if start_quote is None:
                 raise ValueError(f'value is incorrectly quoted: "{value}"')
-            if unquote:
+            if unquote and start_index == 0:
                 value = value[:-1]
 
         if start_quote is None and ' ' in value:
             raise ValueError(f'value needs to be quoted: "{value}"')
 
         parsed[key] = value
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/async_message/__init__.py` & `grizzly-loadtester-2.6.3/grizzly_extras/async_message/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 from os import environ, path
 from platform import node as hostname
 from json import dumps as jsondumps
 from time import monotonic as time
 from io import StringIO
 from threading import Lock
 from datetime import datetime
-from time import sleep
+from time import sleep, perf_counter
 
 import zmq.green as zmq
 
 from zmq.error import Again as ZMQAgain
 from zmq.sugar.constants import NOBLOCK as ZMQ_NOBLOCK
 from grizzly_extras.transformer import JsonBytesEncoder
 
 __all__: List[str] = []
 
 
+logger = logging.getLogger(__name__)
+
+
 AsyncMessageMetadata = Optional[Dict[str, Any]]
 AsyncMessagePayload = Optional[Any]
 
 
 class ThreadLogger:
     _logger: logging.Logger
     _lock: Lock = Lock()
@@ -94,14 +97,15 @@
     metadata: Optional[Dict[str, str]]
     consume: bool
 
 
 class AsyncMessageRequest(TypedDict, total=False):
     action: str
     worker: Optional[str]
+    client: int
     context: AsyncMessageContext
     payload: AsyncMessagePayload
 
 
 class AsyncMessageResponse(TypedDict, total=False):
     success: bool
     worker: str
@@ -136,34 +140,37 @@
 
     @abstractmethod
     def close(self) -> None:
         raise NotImplementedError(f'{self.__class__.__name__}: close is not implemented')
 
     @final
     def handle(self, request: AsyncMessageRequest) -> AsyncMessageResponse:
-        action = request['action']
-        request_handler = self.get_handler(action)
-        self.logger.debug(f'handling {action}, request=\n{jsondumps(request, indent=2, cls=JsonBytesEncoder)}')
-
-        response: AsyncMessageResponse
-
         start_time = time()
 
         try:
+            action = request.get('action', None)
+            if action is None:
+                raise RuntimeError('no action in request')
+
+            request_handler = self.get_handler(action)
+            self.logger.debug(f'handling {action}, request=\n{jsondumps(request, indent=2, cls=JsonBytesEncoder)}')
+
+            response: AsyncMessageResponse
+
             if request_handler is None:
                 raise AsyncMessageError(f'no implementation for {action}')
 
             response = request_handler(self, request)
             response['success'] = True
         except Exception as e:
             response = {
                 'success': False,
-                'message': f'{action}: {e.__class__.__name__}="{str(e)}"',
+                'message': f'{action or "UNKNOWN"}: {e.__class__.__name__}="{str(e)}"',
             }
-            self.logger.error(f'{action}: {e.__class__.__name__}="{str(e)}"', exc_info=True)
+            self.logger.error(f'{action or "UNKNOWN"}: {e.__class__.__name__}="{str(e)}"', exc_info=True)
         finally:
             total_time = int((time() - start_time) * 1000)
             response.update({
                 'worker': self.worker,
                 'response_time': total_time,
             })
 
@@ -194,25 +201,34 @@
 
         return func
 
     return decorator
 
 
 def async_message_request(client: zmq.Socket, request: AsyncMessageRequest) -> AsyncMessageResponse:
-    client.send_json(request)
-
-    while True:
-        try:
-            response = cast(AsyncMessageResponse, client.recv_json(flags=ZMQ_NOBLOCK))
-            break
-        except ZMQAgain:
-            sleep(0.1)
-
-    if response is None:
-        raise RuntimeError('no response')
-
-    message = response.get('message', None)
-
-    if not response['success']:
-        raise RuntimeError(message)
+    try:
+        client.send_json(request)
 
-    return response
+        while True:
+            start = perf_counter()
+            try:
+                response = cast(AsyncMessageResponse, client.recv_json(flags=ZMQ_NOBLOCK))
+                break
+            except ZMQAgain:
+                sleep(0.1)
+            delta = perf_counter() - start
+            if delta > 1.0:
+                logger.debug(f'async_message_request::recv_json took {delta} seconds')
+
+        if response is None:
+            raise AsyncMessageError('no response')
+
+        message = response.get('message', None)
+
+        if not response['success']:
+            raise AsyncMessageError(message)
+
+        return response
+    except Exception as e:
+        if not isinstance(e, AsyncMessageError):
+            logger.error(f'failed to send {request=}', exc_info=True)
+        raise
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/async_message/daemon.py` & `grizzly-loadtester-2.6.3/grizzly_extras/async_message/daemon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union, cast
+from typing import List, Optional, Union, Dict, cast
 from types import FrameType
 from uuid import uuid4
 from json import loads as jsonloads, dumps as jsondumps
 from threading import Thread
 from urllib.parse import urlparse
 from signal import signal, SIGTERM, SIGINT, Signals
 from time import sleep
@@ -60,16 +60,20 @@
         thread.daemon = True
         worker_threads.append(thread)
         thread.start()
         logger.info(f'spawned worker {identity} ({thread.ident})')
 
     workers_available: List[str] = []
 
+    client_worker_map: Dict[str, str] = {}
+
     spawn_worker()
 
+    worker_id: str
+
     while run:
         socks = dict(poller.poll(timeout=1000))
 
         if not socks:
             continue
 
         logger.debug("i'm alive!")
@@ -82,48 +86,76 @@
                 sleep(0.1)
                 continue
 
             if not backend_response:
                 continue
 
             reply = backend_response[2:]
+            worker_id = backend_response[0].decode()
+
             if reply[0] != LRU_READY.encode():
                 frontend.send_multipart(reply)
+                logger.debug(f'forwarding backend response from {worker_id}')
             else:
-                worker_id = backend_response[0]
-                logger.info(f'worker {worker_id.decode()} ready')
+                logger.info(f'worker {worker_id} ready')
                 workers_available.append(worker_id)
 
         if socks.get(frontend) == zmq.POLLIN:
             logger.debug('polling frontend')
             try:
                 msg = frontend.recv_multipart(flags=zmq.NOBLOCK)
             except zmq.Again:
                 sleep(0.1)
                 continue
 
             request_id = msg[0]
-            payload = jsonloads(msg[-1].decode())
+            payload = cast(AsyncMessageRequest, jsonloads(msg[-1].decode()))
+
+            request_worker_id = payload.get('worker', None)
+            request_client_id = payload.get('client', None)
+            client_key: Optional[str] = None
+
+            logger.debug(f'{request_worker_id=} ({type(request_worker_id)}), {request_client_id=} ({type(request_client_id)})')
 
-            worker_id = payload.get('worker', None)
+            if request_client_id is not None:
+                integration_url = payload.get('context', {}).get('url', None)
+                parsed = urlparse(integration_url)
+                scheme = parsed.scheme
+                if isinstance(scheme, bytes):
+                    scheme = scheme.decode()
+
+                client_key = f'{request_client_id}::{scheme}'
+
+            if request_worker_id is None and client_key is not None:
+                request_worker_id = client_worker_map.get(client_key, None)
 
-            if worker_id is None:
+            if request_worker_id is None:
                 worker_id = workers_available.pop()
-                payload['worker'] = worker_id.decode()
-                logger.info(f'assigning worker {payload["worker"]}')
-                request = jsondumps(payload).encode()
+
+                if client_key is not None:
+                    client_worker_map.update({client_key: worker_id})
+
+                payload['worker'] = worker_id
+                logger.info(f'assigned worker {payload["worker"]} to {client_key}')
+
                 if len(workers_available) == 0:
                     logger.debug('spawning an additional worker, for next client')
                     spawn_worker()
             else:
-                worker_id = worker_id.encode()
-                request = msg[-1]
+                logger.debug(f'{request_client_id} is assigned {request_worker_id}')
+                worker_id = request_worker_id
+
+                if payload.get('worker', None) is None:
+                    payload['worker'] = worker_id
 
-            backend_request = [worker_id, SPLITTER_FRAME, request_id, SPLITTER_FRAME, request]
+            request = jsondumps(payload).encode()
+            backend_request = [worker_id.encode(), SPLITTER_FRAME, request_id, SPLITTER_FRAME, request]
+            logger.debug(f'{backend_request=}')
             backend.send_multipart(backend_request)
+            logger.debug(f'forwarding frontend request to worker {request_worker_id}')
 
     logger.info('stopping')
     for worker_thread in worker_threads:
         logger.debug(f'waiting for {worker_thread.ident}')
         worker_thread.join()
 
     try:
@@ -158,51 +190,59 @@
             continue
 
         request = cast(
             AsyncMessageRequest,
             jsonloads(request_proto[-1].decode()),
         )
 
-        if request['worker'] != identity:
-            logger.error(f'got {request["worker"]}, expected {identity}')
-            continue
-
         response: Optional[AsyncMessageResponse] = None
-        if integration is None:
-            try:
-                integration_url = request.get('context', {}).get('url', None)
-                if integration_url is None:
-                    raise RuntimeError('no url found in request context')
 
-                parsed = urlparse(integration_url)
+        try:
+            if request['worker'] != identity:
+                raise RuntimeError(f'got {request["worker"]}, expected {identity}')
 
-                if parsed.scheme in ['mq', 'mqs']:
-                    from .mq import AsyncMessageQueueHandler
-                    integration = AsyncMessageQueueHandler(identity)
-                elif parsed.scheme == 'sb':
-                    from .sb import AsyncServiceBusHandler
-                    integration = AsyncServiceBusHandler(identity)
-                else:
-                    raise RuntimeError(f'integration for {str(parsed.scheme)}:// is not implemented')
+            action = request.get('action', None)
 
-            except Exception as e:
-                response = {
-                    'worker': identity,
-                    'response_time': 0,
-                    'success': False,
-                    'message': str(e),
-                }
+            if integration is None:
+                if action not in ['DISCONNECT', 'DISC']:
+                    integration_url = request.get('context', {}).get('url', None)
+                    if integration_url is None:
+                        raise RuntimeError('no url found in request context')
+
+                    parsed = urlparse(integration_url)
+
+                    if parsed.scheme in ['mq', 'mqs']:
+                        from .mq import AsyncMessageQueueHandler
+                        integration = AsyncMessageQueueHandler(identity)
+                    elif parsed.scheme == 'sb':
+                        from .sb import AsyncServiceBusHandler
+                        integration = AsyncServiceBusHandler(identity)
+                    else:
+                        raise RuntimeError(f'integration for {str(parsed.scheme)}:// is not implemented')
+                else:
+                    response = {
+                        'worker': identity,
+                        'response_time': 0,
+                        'success': True,
+                        'message': f'already handled {action}',
+                    }
+        except Exception as e:
+            response = {
+                'worker': identity,
+                'response_time': 0,
+                'success': False,
+                'message': str(e),
+            }
 
         if response is None and integration is not None:
             logger.debug('send request to handler')
             response = integration.handle(request)
             logger.debug('got response from handler')
 
-            if request.get('action', None) in ['DISCONNECT', 'DISC']:
-                integration.close()
+            if action in ['DISCONNECT', 'DISC']:
                 integration = None
 
         response_proto = [
             request_proto[0],
             SPLITTER_FRAME,
             jsondumps(response, cls=JsonBytesEncoder).encode(),
         ]
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/async_message/mq/__init__.py` & `grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,21 +71,23 @@
 
         return {
             'message': 'disconnected',
         }
 
     @register(handlers, 'CONN')
     def connect(self, request: AsyncMessageRequest) -> AsyncMessageResponse:
-        if self.qmgr is not None:
-            raise AsyncMessageError('already connected')
-
         context = request.get('context', None)
         if context is None:
             raise AsyncMessageError('no context in request')
 
+        if self.qmgr is not None:
+            return {
+                'message': 're-used connection',
+            }
+
         connection = context['connection']
         queue_manager = context['queue_manager']
         channel = context['channel']
         username = context.get('username', None)
         password = context.get('password', None)
         key_file = context.get('key_file', None)
         cert_label = context.get('cert_label', None) or username
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/async_message/mq/rfh2.py` & `grizzly-loadtester-2.6.3/grizzly_extras/async_message/mq/rfh2.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/async_message/sb.py` & `grizzly-loadtester-2.6.3/grizzly_extras/async_message/sb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from typing import Any, Callable, Dict, Optional, Union, Tuple, Iterable, cast
 from time import perf_counter, sleep
+
 from mypy_extensions import VarArg, KwArg
 
 from azure.servicebus import ServiceBusClient, ServiceBusMessage, TransportType, ServiceBusSender, ServiceBusReceiver, ServiceBusReceivedMessage
 from azure.servicebus.management import ServiceBusAdministrationClient, TopicProperties, SqlRuleFilter
 from azure.servicebus.amqp import AmqpMessageBodyType
 from azure.servicebus.amqp._amqp_message import DictMixin
 from azure.core.exceptions import ResourceNotFoundError, ResourceExistsError
@@ -35,83 +36,99 @@
 
 
 class AsyncServiceBusHandler(AsyncMessageHandler):
     _sender_cache: Dict[str, ServiceBusSender]
     _receiver_cache: Dict[str, ServiceBusReceiver]
     _arguments: Dict[str, Dict[str, str]]
 
-    client: Optional[ServiceBusClient] = None
+    _client: Optional[ServiceBusClient] = None
     mgmt_client: Optional[ServiceBusAdministrationClient] = None
 
     def __init__(self, worker: str) -> None:
         super().__init__(worker)
 
         self._sender_cache = {}
         self._receiver_cache = {}
         self._arguments = {}
 
+    @property
+    def client(self) -> ServiceBusClient:
+        if self._client is None:
+            raise AttributeError('no client')
+
+        return self._client
+
+    @client.setter
+    def client(self, value: ServiceBusClient) -> None:
+        self._client = value
+
     def close(self) -> None:
         for key, sender in self._sender_cache.items():
             self.logger.debug(f'closing sender {key}')
             sender.close()
 
+        self._sender_cache.clear()
+
         for key, receiver in self._receiver_cache.items():
             self.logger.debug(f'closing receiver {key}')
             receiver.close()
 
-        if self.client is not None:
-            self.logger.debug('closing client')
-            self.client.close()
-
-        if self.mgmt_client is not None:
-            self.logger.debug('closing management client')
-            self.mgmt_client.close()
+        self._receiver_cache.clear()
 
-    @classmethod
-    def get_sender_instance(cls, client: ServiceBusClient, arguments: Dict[str, str]) -> ServiceBusSender:
+        if len(self._sender_cache) + len(self._receiver_cache) == 0:
+            if self.client is not None:
+                self.logger.debug('closing client')
+                self.client.close()
+
+            if self.mgmt_client is not None:
+                self.logger.debug('closing management client')
+                self.mgmt_client.close()
+
+    def get_sender_instance(self, arguments: Dict[str, str]) -> ServiceBusSender:
         endpoint_type = arguments['endpoint_type']
         endpoint_name = arguments['endpoint']
 
-        sender_arguments: Dict[str, str] = {}
+        sender_arguments: Dict[str, str] = {'client_identifier': self.worker}
 
         sender_type: Callable[[KwArg(Any)], ServiceBusSender]
 
         if endpoint_type == 'queue':
             sender_arguments.update({'queue_name': endpoint_name})
             sender_type = cast(
                 Callable[[KwArg(Any)], ServiceBusSender],
-                client.get_queue_sender,
+                self.client.get_queue_sender,
             )
         else:
             sender_arguments.update({'topic_name': endpoint_name})
             sender_type = cast(
                 Callable[[KwArg(Any)], ServiceBusSender],
-                client.get_topic_sender,
+                self.client.get_topic_sender,
             )
 
         return sender_type(**sender_arguments)
 
-    @classmethod
-    def get_receiver_instance(cls, client: ServiceBusClient, arguments: Dict[str, str]) -> ServiceBusReceiver:
+    def get_receiver_instance(self, arguments: Dict[str, str]) -> ServiceBusReceiver:
         endpoint_type = arguments['endpoint_type']
         endpoint_name = arguments['endpoint']
         subscription_name = arguments.get('subscription', None)
         message_wait = arguments.get('wait', None)
 
-        receiver_arguments: Dict[str, Any] = {}
+        receiver_arguments: Dict[str, Any] = {
+            'client_identifier': self.worker,
+        }
         receiver_type: Callable[[KwArg(Any)], ServiceBusReceiver]
 
         if message_wait is not None:
             receiver_arguments.update({'max_wait_time': int(message_wait)})
 
         if endpoint_type == 'queue':
-            receiver_type = cast(Callable[[KwArg(Any)], ServiceBusReceiver], client.get_queue_receiver)
+            receiver_type = cast(Callable[[KwArg(Any)], ServiceBusReceiver], self.client.get_queue_receiver)
             receiver_arguments.update({'queue_name': endpoint_name})
         else:
-            receiver_type = cast(Callable[[KwArg(Any)], ServiceBusReceiver], client.get_subscription_receiver)
+            receiver_type = cast(Callable[[KwArg(Any)], ServiceBusReceiver], self.client.get_subscription_receiver)
             receiver_arguments.update({
                 'topic_name': endpoint_name,
                 'subscription_name': subscription_name,
             })
 
         return receiver_type(**receiver_arguments)
 
@@ -229,14 +246,16 @@
                     pass
 
             try:
                 del cache[cache_endpoint]
             except:  # pragma: no cover
                 pass
 
+        self.close()
+
         return {
             'message': 'thanks for all the fish',
         }
 
     @register(handlers, 'SUBSCRIBE')
     def subscribe(self, request: AsyncMessageRequest) -> AsyncMessageResponse:
         context = request.get('context', None)
@@ -367,49 +386,37 @@
         if context is None:
             raise AsyncMessageError('no context in request')
 
         url = context['url']
         if not url.startswith('Endpoint='):
             url = f'Endpoint={url}'
 
-        if self.client is None or force:
-            if self.client is not None:
-                try:
-                    self.client.close()
-                except:
-                    pass
-
+        if self._client is None:
             self.client = ServiceBusClient.from_connection_string(
                 conn_str=url,
                 transport_type=TransportType.AmqpOverWebsocket,
             )
 
-        if self.mgmt_client is None or force:
-            if self.mgmt_client is not None:
-                try:
-                    self.mgmt_client.close()
-                except:
-                    pass
-
-            if self.logger._logger.level == logging.DEBUG:
-                self.mgmt_client = ServiceBusAdministrationClient.from_connection_string(conn_str=url)
+        if self.mgmt_client is None and self.logger._logger.level == logging.DEBUG:
+            self.mgmt_client = ServiceBusAdministrationClient.from_connection_string(conn_str=url)
 
         endpoint = context['endpoint']
         instance_type = context['connection']
         message_wait = context.get('message_wait', None)
         arguments = self.get_endpoint_arguments(instance_type, endpoint)
         endpoint_arguments = parse_arguments(endpoint, ':')
+
         try:
             del endpoint_arguments['expression']
         except:
             pass
 
         cache_endpoint = ', '.join([f'{key}:{value}' for key, value in endpoint_arguments.items()])
 
-        if message_wait is not None and instance_type == 'receiver':
+        if instance_type == 'receiver' and message_wait is not None:
             arguments['wait'] = str(message_wait)
 
         cache: GenericCache
 
         get_instance: GenericInstance
 
         if instance_type == 'sender':
@@ -428,15 +435,15 @@
             if instance is not None:
                 try:
                     self.logger.info(f'cleaning up stale {instance_type} instance for {cache_endpoint}')
                     instance.__exit__()
                 except:
                     pass
 
-            cache.update({cache_endpoint: get_instance(self.client, arguments).__enter__()})
+            cache.update({cache_endpoint: get_instance(arguments).__enter__()})
 
             self.logger.debug(f'cached {instance_type} instance for {cache_endpoint}')
 
         return {
             'message': 'there general kenobi',
         }
 
@@ -491,14 +498,20 @@
 
             receiver = self._receiver_cache[cache_endpoint]
             message_wait = int(request_arguments.get('message_wait', str(context.get('message_wait', 0))))
             consume = context.get('consume', False)
 
             wait_start = perf_counter()
 
+            # reset last activity timestamp, might be set from previous usage that was more
+            # than message_wait ago, which will cause a "timeout" when trying to read it now
+            # which means we'll not get any messages, even though the endpoint isn't empty
+            if message_wait > 0:
+                receiver._handler._last_activity_timestamp = None
+
             for retry in range(1, 4):
                 try:
                     if expression is not None:
                         try:
                             content_type = TransformerContentType.from_string(cast(str, request.get('context', {})['content_type']))
                             transform = transformer.available[content_type]
                             get_values = transform.parser(request_arguments['expression'])
@@ -556,55 +569,57 @@
 
                                 sleep(0.2)
 
                     if message is None:
                         raise StopIteration()
 
                     break
-
                 except StopIteration:
+                    if message_wait > 0:
+                        receiver._handler._last_activity_timestamp = None
                     delta = perf_counter() - wait_start
 
-                    if message_wait > 0 and delta >= message_wait:
-                        error_message = f'no messages on {endpoint}'
-                        message = None
-                        if message_wait > 0:
-                            error_message = f'{error_message} within {message_wait} seconds'
-                    else:
-                        # ugly brute-force way of handling no messages on service bus
-                        if retry < 3:
-                            self.logger.warning(f'receiver for {cache_endpoint} returned no message without trying, brute-force retry #{retry}')
-                            # <!-- useful debugging information, actual message count on message entity
-                            if self.logger._logger.level == logging.DEBUG and self.mgmt_client is not None:
-                                if 'topic' in endpoint_arguments:
-                                    topic_properties = self.mgmt_client.get_subscription_runtime_properties(
-                                        topic_name=endpoint_arguments['topic'],
-                                        subscription_name=endpoint_arguments['subscription']
-                                    )
-                                    self.logger.debug((
-                                        f'{cache_endpoint}: {topic_properties.active_message_count=}, '
-                                        f'{topic_properties.total_message_count=}, {topic_properties.transfer_dead_letter_message_count=}, '
-                                        f'{topic_properties.transfer_message_count=}'
-                                    ))
-                                elif 'queue' in endpoint_arguments:
-                                    queue_properties = self.mgmt_client.get_queue_runtime_properties(
-                                        queue_name=endpoint_arguments['queue'],
-                                    )
-                                    self.logger.debug((
-                                        f'{cache_endpoint}: {queue_properties.active_message_count=}, '
-                                        f'{queue_properties.total_message_count=}, {queue_properties.transfer_dead_letter_message_count=}, '
-                                        f'{queue_properties.transfer_message_count=}'
-                                    ))
-                            # // useful debugging information -->
-
-                            self._hello(request, force=True)
-                            receiver = self._receiver_cache[cache_endpoint]
+                    if message_wait > 0:
+                        if delta >= message_wait:
+                            error_message = f'no messages on {endpoint}'
                             message = None
-                            continue
-
+                            if message_wait > 0:
+                                error_message = f'{error_message} within {message_wait} seconds'
+                        else:
+                            # ugly brute-force way of handling no messages on service bus
+                            if retry < 3:
+                                self.logger.warning(f'receiver for {cache_endpoint} returned no message without trying, brute-force retry #{retry}')
+                                # <!-- useful debugging information, actual message count on message entity
+                                if self.logger._logger.level == logging.DEBUG and self.mgmt_client is not None:
+                                    if 'topic' in endpoint_arguments:
+                                        topic_properties = self.mgmt_client.get_subscription_runtime_properties(
+                                            topic_name=endpoint_arguments['topic'],
+                                            subscription_name=endpoint_arguments['subscription']
+                                        )
+                                        self.logger.debug((
+                                            f'{cache_endpoint}: {topic_properties.active_message_count=}, '
+                                            f'{topic_properties.total_message_count=}, {topic_properties.transfer_dead_letter_message_count=}, '
+                                            f'{topic_properties.transfer_message_count=}'
+                                        ))
+                                    elif 'queue' in endpoint_arguments:
+                                        queue_properties = self.mgmt_client.get_queue_runtime_properties(
+                                            queue_name=endpoint_arguments['queue'],
+                                        )
+                                        self.logger.debug((
+                                            f'{cache_endpoint}: {queue_properties.active_message_count=}, '
+                                            f'{queue_properties.total_message_count=}, {queue_properties.transfer_dead_letter_message_count=}, '
+                                            f'{queue_properties.transfer_message_count=}'
+                                        ))
+                                # // useful debugging information -->
+
+                                self._hello(request, force=True)
+                                receiver = self._receiver_cache[cache_endpoint]
+                                message = None
+                                continue
+                    else:
                         error_message = f'{endpoint} receiver returned no messages, without trying'
 
                     raise AsyncMessageError(error_message)
 
         if expression is None:
             metadata, payload = self.from_message(message)
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/text.py` & `grizzly-loadtester-2.6.3/grizzly_extras/text.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly_extras/transformer.py` & `grizzly-loadtester-2.6.3/grizzly_extras/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,21 @@
             valid = False
 
         return valid
 
     @classmethod
     def parser(cls, expression: str) -> Callable[[Any], List[str]]:
         try:
+            expected: Optional[str] = None
+
+            # we only have one instance of equals
+            if '==' in expression and expression.index('==') == expression.rindex('==') and not ('?' in expression and '@' in expression):
+                expression, expected = expression.split('==', 1)
+                expected = expected.strip('"\'')
+
             if not cls.validate(expression):
                 raise RuntimeError(f'{cls.__name__}: not a valid expression')
 
             jsonpath = jsonpath_parse(expression)
 
             def _parser(input_payload: Any) -> List[str]:
                 values: List[str] = []
@@ -125,15 +132,16 @@
                         continue
 
                     if isinstance(m.value, (dict, list, )):
                         value = jsondumps(m.value)
                     else:
                         value = str(m.value)
 
-                    values.append(value)
+                    if expected is None or expected == value:
+                        values.append(value)
 
                 return values
 
             return _parser
         except Exception as e:
             raise ValueError(f'{cls.__name__}: unable to parse "{expression}": {str(e)}') from e
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/PKG-INFO` & `grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grizzly-loadtester
-Version: 2.6.2
+Version: 2.6.3
 Summary: Traffic generator based on locust and behave
 Author-email: biometria <opensource@biometria.se>
 License: MIT
 Project-URL: Documentation, https://biometria-se.github.io/grizzly/
 Project-URL: Code, https://github.com/biometria-se/grizzly/
 Project-URL: Tracker, https://github.com/Biometria-se/grizzly/issues
 Keywords: locust,behave,load,loadtest,performance,traffic generator
```

### Comparing `grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/SOURCES.txt` & `grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/grizzly_loadtester.egg-info/requires.txt` & `grizzly-loadtester-2.6.3/grizzly_loadtester.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 [:python_version < "3.9"]
 backports.zoneinfo>=0.2.1
 
 [ci]
 build>=0.7.0
 twine<4.0.0,>=3.8.0
-pip-tools>=6.5.0
 
 [dev]
 wheel>=0.37.0
 astunparse>=1.6.3
 mypy>=0.931
 flake8-pyproject>=1.1.0
 pylint>=2.12.2
@@ -40,10 +39,11 @@
 atomicwrites>=1.4.0
 types-paramiko>=2.8.13
 types-python-dateutil>=2.8.9
 types-PyYAML<6.0.0,>=5.3.0
 types-requests>=2.27.0
 types-Jinja2>=2.0.0
 types-backports>=0.1.3
+snakeviz
 
 [mq]
 pymqi==1.12.0
```

### Comparing `grizzly-loadtester-2.6.2/pyproject.toml` & `grizzly-loadtester-2.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -79,20 +79,20 @@
     "pytest-timeout >=2.1.0",
     "atomicwrites >= 1.4.0",
     "types-paramiko >=2.8.13",
     "types-python-dateutil >=2.8.9",
     "types-PyYAML <6.0.0,>=5.3.0",
     "types-requests >=2.27.0",
     "types-Jinja2 >=2.0.0",
-    "types-backports >=0.1.3"
+    "types-backports >=0.1.3",
+    "snakeviz"
 ]
 ci = [
     "build >=0.7.0",
-    "twine >=3.8.0,<4.0.0",
-    "pip-tools >=6.5.0"
+    "twine >=3.8.0,<4.0.0"
 ]
 
 [tool.setuptools_scm]
 write_to = "grizzly/__version__.py"
 local_scheme = "no-local-version"
 
 [tool.setuptools.packages.find]
@@ -261,9 +261,10 @@
 addopts = [
     "--cov=.",
     "--cov-report=",
     "--no-cov-on-fail"
 ]
 timeout = 10
 filterwarnings = [
-    "ignore:setDaemon\\(\\) is deprecated.*:DeprecationWarning"
+    "ignore:setDaemon\\(\\) is deprecated.*:DeprecationWarning",
+    "ignore:.*pkg_resources.*:DeprecationWarning"
 ]
```

### Comparing `grizzly-loadtester-2.6.2/script/docs-generate-changelog.py` & `grizzly-loadtester-2.6.3/script/docs-generate-changelog.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/script/docs-generate-licenses.py` & `grizzly-loadtester-2.6.3/script/docs-generate-licenses.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/script/docs-generate.bash` & `grizzly-loadtester-2.6.3/script/docs-generate.bash`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             local tag
             if [[ "${target}" == "cli" ]]; then
                 local version
                 version="$(grizzly-${target} --version | awk '{print $NF}')"
                 rc=$(( rc + $? ))
                 tag="v${version}"
             else
-                tag="$(git tag | grep -E '^v' | sort | tail -1)"
+                tag="$(git tag | grep -E '^v' | sort --version-sort | tail -1)"
             fi
 
             >&2 echo "checking out tag ${tag}"
             git checkout "tags/${tag}" -b "${tag}"
             rc=$(( rc + $? ))
 
             case "${what}" in
```

### Comparing `grizzly-loadtester-2.6.2/tests/conftest.py` & `grizzly-loadtester-2.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/background/test_setup.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from tempfile import NamedTemporaryFile
+import inspect
+
 from typing import cast, Dict, Any, List
 
 import pytest
-import yaml
 
 from grizzly.types.behave import Context
 from grizzly.context import GrizzlyContext
 
 from tests.fixtures import End2EndFixture
+from tests.helpers import message_callback
 
 
 @pytest.mark.parametrize('url', [
-    'influxdb://grizzly:password@localhost/grizzly-statistics',
+    'influxdb://grizzly:password@localhost/grizzly-statistics?Testplan=grizzly-statistics',
     'insights://localhost/?Testplan=grizzly-statistics&InstrumentationKey=asdfasdf=',
-    'influxdb://$conf::statistics.username$:$conf::statistics.password$@localhost/$conf::statistics.database$',
+    'influxdb://$conf::statistics.username$:$conf::statistics.password$@localhost/$conf::statistics.database$?Testplan=grizzly-statistics',
 ])
 def test_e2e_step_setup_save_statistics(e2e_fixture: End2EndFixture, url: str) -> None:
     env_conf: Dict[str, Any] = {
         'configuration': {
             'statistics': {
                 'username': 'grizzly',
                 'password': 'password',
@@ -53,21 +54,17 @@
     feature_file = e2e_fixture.test_steps(
         background=[
             f'And save statistics to "{url}"',
         ],
         identifier=url,
     )
 
-    with NamedTemporaryFile(delete=True, suffix='.yaml', dir=e2e_fixture.test_tmp_dir) as env_conf_file:
-        env_conf_file.write(yaml.dump(env_conf, Dumper=yaml.Dumper).encode())
-        env_conf_file.flush()
-
-        rc, _ = e2e_fixture.execute(feature_file, env_conf_file=env_conf_file.name)
+    rc, _ = e2e_fixture.execute(feature_file, env_conf=env_conf)
 
-        assert rc == 0
+    assert rc == 0
 
 
 @pytest.mark.parametrize('level', [
     'INFO',
     'DEBUG',
     'WARNING',
     'ERROR',
@@ -188,34 +185,41 @@
         from grizzly.types import MessageDirection
         grizzly = cast(GrizzlyContext, context.grizzly)
         data = list(context.table)[0].as_dict()
 
         direction = MessageDirection.from_string(data['direction'])
         message_type = data['message_type']
 
-        from tests.helpers import message_callback
+        from steps.helpers import message_callback  # type: ignore  # pylint: disable=import-error
 
         assert grizzly.setup.locust.messages == {
             direction: {
                 message_type: message_callback,
             }
         }
 
         grizzly.setup.locust.messages.clear()
 
+    with open(e2e_fixture.root / 'features' / 'steps' / 'helpers.py', 'w+') as fd:
+        source = inspect.getsource(message_callback)
+        fd.write(f'''from grizzly.types.locust import Message, Environment
+
+{source}
+''')
+
     table: List[Dict[str, str]] = [{
         'direction': f'{from_node}_{to_node}',
         'message_type': message_type,
     }]
 
     e2e_fixture.add_validator(validator, table=table)
 
     feature_file = e2e_fixture.test_steps(
         background=[
-            f'And add callback "tests.helpers.message_callback" for message type "{message_type}" from {from_node} to {to_node}',
+            f'And add callback "steps.helpers.message_callback" for message type "{message_type}" from {from_node} to {to_node}',
         ],
         identifier=message_type,
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
```

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/background/test_shapes.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/background/test_shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_response.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_results.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_setup.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_tasks.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from json import dumps as jsondumps
-from tempfile import NamedTemporaryFile
 from typing import cast, List, Dict
 from textwrap import dedent
 
 import pytest
-import yaml
 
 from grizzly.context import GrizzlyContext
 from grizzly.types.behave import Context, Feature
 
 from tests.fixtures import End2EndFixture
 
 
@@ -440,47 +438,52 @@
         assert len(tasks) == 3
 
         task = tasks[0]
         assert isinstance(task, HttpClientTask)
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == f'https://{e2e_fixture_host}/example.json'
         assert task.name == 'https-get'
-        assert task.variable == 'example_openapi', f'{task.variable} != example_openapi'
+        assert task.payload_variable == 'example_openapi', f'{task.payload_variable} != example_openapi'
+        assert task.metadata_variable is None
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         actual_templates = task.get_templates()
         assert actual_templates == ['{{ example_openapi }}'], f"{actual_templates} != ['{{{{ example_openapi }}}}']"
 
         task = tasks[1]
         assert isinstance(task, HttpClientTask)
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == '{{ endpoint }}'
         assert task.name == 'http-get'
-        assert task.variable == 'endpoint_result'
+        assert task.payload_variable == 'endpoint_payload'
+        assert task.metadata_variable == 'endpoint_metadata'
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         actual_templates = task.get_templates()
-        assert sorted(actual_templates) == sorted(['{{ endpoint }}', '{{ endpoint_result }}']), f"{actual_templates} != ['{{{{ endpoint }}}}', '{{{{ endpoint_result }}}}']"
+        assert (
+            sorted(actual_templates) == sorted(['{{ endpoint }}', '{{ endpoint_payload }} {{ endpoint_metadata }}'])
+        ), f"{actual_templates} != ['{{{{ endpoint }}}}', '{{{{ endpoint_payload }}}} {{{{ endpoint_metadata}}}}']"
 
     table: List[Dict[str, str]] = [{
         'e2e_fixture.host': e2e_fixture.host,
     }]
 
     e2e_fixture.add_validator(validate_client_task, table=table)
 
     feature_file = e2e_fixture.test_steps(
         scenario=[
             'And value for variable "example_openapi" is "None"',
-            'And value for variable "endpoint_result" is "None"',
+            'And value for variable "endpoint_payload" is "None"',
+            'And value for variable "endpoint_metadata" is "None"',
             f'And value for variable "endpoint" is "{e2e_fixture.host}"',
-            f'Then get "https://{e2e_fixture.host}/example.json" with name "https-get" and save response in "example_openapi"',
-            'Then get "http://{{ endpoint }}" with name "http-get" and save response in "endpoint_result"',
-            'Then log message "example_openapi={{ example_openapi }}, endpoint_result={{ endpoint_result }}"',
+            f'Then get "https://{e2e_fixture.host}/example.json" with name "https-get" and save response payload in "example_openapi"',
+            'Then get "http://{{ endpoint }}" with name "http-get" and save response payload in "endpoint_payload" and metadata in "endpoint_metadata"',
+            'Then log message "example_openapi={{ example_openapi }}, endpoint_payload={{ endpoint_payload }}, endpoint_metadata={{ endpoint_metadata }}"',
         ]
     )
 
     rc, _ = e2e_fixture.execute(feature_file)
 
     assert rc == 0
 
@@ -510,15 +513,16 @@
         task = parent_task.request
         assert isinstance(task, HttpClientTask)
         assert task.arguments == {}
         assert task.content_type == TransformerContentType.JSON
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == f'http://{e2e_fixture_host}/api/until/id?nth=2&wrong=bar&right=foo&as_array=True', f'{task.name=}, {task.endpoint=}'
         assert task.name == 'https-get'
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         assert task.get_templates() == []
 
         parent_task = tasks[1]
         assert isinstance(parent_task, UntilRequestTask)
@@ -528,15 +532,16 @@
         task = parent_task.request
         assert isinstance(task, HttpClientTask)
         assert task.arguments == {}
         assert task.content_type == TransformerContentType.JSON
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == '{{ endpoint }}/api/until/success?nth=2&wrong=false&right=true&as_array=True', f'{task.name=}, {task.endpoint=}'
         assert task.name == 'http-get'
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         assert task.get_templates() == ['{{ endpoint }}/api/until/success?nth=2&wrong=false&right=true&as_array=True'], f'{task.name=}, {task.get_templates()=}'
 
         parent_task = tasks[2]
         assert isinstance(parent_task, UntilRequestTask)
@@ -546,15 +551,16 @@
         task = parent_task.request
         assert isinstance(task, HttpClientTask)
         assert task.arguments == {'verify': False}
         assert task.content_type == TransformerContentType.JSON
         assert task.direction == RequestDirection.FROM
         assert task.endpoint == f'http://{e2e_fixture_host}/api/until/hello?nth=2&wrong=foobar&right=world&as_array=True', f'{task.name=}, {task.endpoint=}'
         assert task.name == 'https-env-get'
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.source is None
         assert task.destination is None
         assert task._short_name == 'Http'
         assert task.get_templates() == []
 
     table: List[Dict[str, str]] = [{
         'e2e_fixture.host': e2e_fixture.host,
@@ -576,28 +582,25 @@
             (
                 'Then get "https://$conf::test.host$/api/until/hello?nth=2&wrong=foobar&right=world&as_array=True | content_type=json, verify=False" with name "https-env-get" '
                 'until "$.`this`[?hello=\"world\"] | retries=4, expected_matches=1"'
             ),
         ]
     )
 
-    with NamedTemporaryFile(delete=True, suffix='.yaml', dir=e2e_fixture.test_tmp_dir) as env_conf_file:
-        env_conf: Dict[str, Dict[str, Dict[str, str]]] = {
-            'configuration': {
-                'test': {
-                    'host': f'http://{e2e_fixture.host}',
-                }
+    env_conf: Dict[str, Dict[str, Dict[str, str]]] = {
+        'configuration': {
+            'test': {
+                'host': f'http://{e2e_fixture.host}',
             }
         }
-        env_conf_file.write(yaml.dump(env_conf, Dumper=yaml.Dumper).encode())
-        env_conf_file.flush()
+    }
 
-        rc, _ = e2e_fixture.execute(feature_file, env_conf_file=env_conf_file.name)
+    rc, _ = e2e_fixture.execute(feature_file, env_conf=env_conf)
 
-        assert rc == 0
+    assert rc == 0
 
 
 def test_e2e_step_task_client_put_endpoint_file_destination(e2e_fixture: End2EndFixture) -> None:
     def validate_client_task(context: Context) -> None:
         from grizzly.types import RequestDirection
         from grizzly.tasks.clients import BlobStorageClientTask
 
@@ -609,15 +612,16 @@
         assert len(tasks) == 2
 
         task = tasks[0]
         assert isinstance(task, BlobStorageClientTask)
         assert task.direction == RequestDirection.TO
         assert task.endpoint == 'bs://my-unsecure-storage?AccountKey=aaaabbb=&Container=my-container'
         assert task.name == 'bs-put'
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.source == 'test-file.json'
         assert task.destination == 'uploaded-test-file.json'
         assert task._short_name == 'BlobStorage'
         assert task.get_templates() == []
         assert task._endpoints_protocol == 'http'
         assert task.account_name == 'my-unsecure-storage'
         assert task.account_key == 'aaaabbb='
@@ -625,15 +629,16 @@
         assert task.connection_string == 'DefaultEndpointsProtocol=http;AccountName=my-unsecure-storage;AccountKey=aaaabbb=;EndpointSuffix=core.windows.net'
 
         task = tasks[1]
         assert isinstance(task, BlobStorageClientTask)
         assert task.direction == RequestDirection.TO
         assert task.endpoint == 'bss://my-storage?AccountKey=aaaabbb=&Container=my-container'
         assert task.name == 'bss-put'
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.source == 'test-files.json'
         assert task.destination == 'uploaded-test-files.json'
         assert task._short_name == 'BlobStorage'
         assert task.get_templates() == []
         assert task._endpoints_protocol == 'https'
         assert task.account_name == 'my-storage'
         assert task.account_key == 'aaaabbb='
@@ -667,15 +672,16 @@
         assert len(tasks) == 2
 
         task = tasks[0]
         assert isinstance(task, BlobStorageClientTask)
         assert task.direction == RequestDirection.TO
         assert task.endpoint == 'bs://my-unsecure-storage?AccountKey=aaaabbb=&Container=my-container'
         assert task.name == 'bs-put'
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.source == 'test-file.json'
         assert task.destination is None
         assert task._short_name == 'BlobStorage'
         assert task.get_templates() == []
         assert task._endpoints_protocol == 'http'
         assert task.account_name == 'my-unsecure-storage'
         assert task.account_key == 'aaaabbb='
@@ -683,15 +689,16 @@
         assert task.connection_string == 'DefaultEndpointsProtocol=http;AccountName=my-unsecure-storage;AccountKey=aaaabbb=;EndpointSuffix=core.windows.net'
 
         task = tasks[1]
         assert isinstance(task, BlobStorageClientTask)
         assert task.direction == RequestDirection.TO
         assert task.endpoint == 'bss://my-storage?AccountKey=aaaabbb=&Container=my-container'
         assert task.name == 'bss-put'
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.source == 'test-files.json'
         assert task.destination is None
         assert task._short_name == 'BlobStorage'
         assert task.get_templates() == []
         assert task._endpoints_protocol == 'https'
         assert task.account_name == 'my-storage'
         assert task.account_key == 'aaaabbb='
```

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/scenario/test_user.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/scenario/test_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/test_setup.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/steps/test_utils.py` & `grizzly-loadtester-2.6.3/tests/e2e/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/test_failure.py` & `grizzly-loadtester-2.6.3/tests/e2e/test_failure.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/test_iteration_pace.py` & `grizzly-loadtester-2.6.3/tests/e2e/test_iteration_pace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from typing import Dict, cast
 from textwrap import dedent
-from tempfile import NamedTemporaryFile
-
-import yaml
 
 from grizzly.context import GrizzlyContext
 from grizzly.types.behave import Context, Feature
 
 from tests.fixtures import End2EndFixture
 
 
@@ -66,14 +63,10 @@
         When condition "{{{{ AtomicIntegerIncrementer.run_id < 3 }}}}" with name "run" is true, execute these tasks
         Then get request with name "sleep-1" from endpoint "/api/sleep/{{{{ AtomicRandomInteger.sleep1 / 1000 / 2 }}}}"
         But if condition is false, execute these tasks
         Then get request with name "sleep-2" from endpoint "/api/sleep/0.6"
         Then end condition
     '''))  # noqa: E501
 
-    with NamedTemporaryFile(delete=True, suffix='.yaml', dir=e2e_fixture.test_tmp_dir) as env_conf_file:
-        env_conf_file.write(yaml.dump(env_conf, Dumper=yaml.Dumper).encode())
-        env_conf_file.flush()
-
-        rc, _ = e2e_fixture.execute(feature_file, env_conf_file=env_conf_file.name)
+    rc, _ = e2e_fixture.execute(feature_file, env_conf=env_conf)
 
-        assert rc == 0
+    assert rc == 0
```

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/test_persistence.py` & `grizzly-loadtester-2.6.3/tests/e2e/test_persistence.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/test_until.py` & `grizzly-loadtester-2.6.3/tests/e2e/test_until.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from typing import Dict, cast
 from textwrap import dedent
-from tempfile import NamedTemporaryFile
-
-import yaml
 
 from grizzly.types.behave import Context, Feature
 from grizzly.context import GrizzlyContext
 
 from tests.fixtures import End2EndFixture
 
 
@@ -27,15 +24,15 @@
             ('001 request-task, w=1.0s, r=2, em=1', 'UNTL', 0, 1,),
             ('002 HttpClientTask', 'SCEN', 0, 1,),
             ('002 HttpClientTask', 'TSTD', 0, 1,),
             ('002 http-client-task, w=1.0s, r=3, em=1', 'UNTL', 0, 1,),
             ('002 http-client-task', 'CLTSK', 1, 2,),
         ]
 
-        assert stats.errors == {}, f'expected 0 logged errors, got {len(stats.errors)}'
+        assert len(stats.errors) == 2, f'expected 0 logged errors, got {len(stats.errors)}'
 
         for name, method, expected_num_failures, expected_num_requests in expectations:
             stat = stats.get(name, method)
             assert stat.num_failures == expected_num_failures, f'{stat.method}:{stat.name}.num_failures: {stat.num_failures} != {expected_num_failures}'
             assert stat.num_requests == expected_num_requests, f'{stat.method}:{stat.name}.num_requests: {stat.num_requests} != {expected_num_requests}'
 
     e2e_fixture.add_after_feature(after_feature)
@@ -68,14 +65,10 @@
     Scenario: HttpClientTask
         Given a user of type "RestApi" load testing "http://{e2e_fixture.host}"
         And repeat for "1" iteration
         And stop user on failure
         Then get "http://$conf::test.host$/api/until/foofoo?nth=2&wrong=foobar&right=world&as_array=true | content_type=json" with name "http-client-task" until "$.`this`[?foofoo="world"] | retries=3, expected_matches=1"
     '''))  # noqa: E501
 
-    with NamedTemporaryFile(delete=True, suffix='.yaml', dir=e2e_fixture.test_tmp_dir) as env_conf_file:
-        env_conf_file.write(yaml.dump(env_conf, Dumper=yaml.Dumper).encode())
-        env_conf_file.flush()
-
-        rc, _ = e2e_fixture.execute(feature_file, env_conf_file=env_conf_file.name)
+    rc, _ = e2e_fixture.execute(feature_file, env_conf=env_conf)
 
-        assert rc == 0
+    assert rc == 0
```

### Comparing `grizzly-loadtester-2.6.2/tests/e2e/test_variables.py` & `grizzly-loadtester-2.6.3/tests/e2e/test_variables.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/fixtures.py` & `grizzly-loadtester-2.6.3/tests/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 import re
 
 from typing import TYPE_CHECKING, Optional, Union, Callable, Any, Literal, List, Tuple, Type, Dict, cast
 from types import TracebackType
 from unittest.mock import MagicMock
 from urllib.parse import urlparse
 from mypy_extensions import VarArg, KwArg
-from os import environ, getcwd, path
-from shutil import rmtree, copytree
+from os import environ, path
+from shutil import rmtree
 from json import dumps as jsondumps
 from pathlib import Path
 from textwrap import dedent, indent
 from hashlib import sha1
 from getpass import getuser
+from cProfile import Profile
+from contextlib import nullcontext
+from tempfile import NamedTemporaryFile
+
+import yaml
 
 from locust.clients import ResponseContextManager
 from locust.contrib.fasthttp import FastResponse, FastRequest
 from geventhttpclient.header import Headers
 from geventhttpclient.response import HTTPSocketPoolResponse
 from _pytest.tmpdir import TempPathFactory
 from pytest_mock.plugin import MockerFixture
@@ -619,14 +624,33 @@
     {dedent(source)}
     if on_local(context) or on_worker(context):
         {self.name}_{self.implementation.__name__}(context)
 '''
 
 
 class End2EndFixture:
+    step_start_webserver = '''
+
+@then(u'start webserver on master port "{{port:d}}"')
+def step_start_webserver(context: Context, port: int) -> None:
+    from grizzly.locust import on_master
+    if not on_master(context):
+        return
+
+    from importlib.machinery import SourceFileLoader
+
+    w = SourceFileLoader(
+        'steps.webserver',
+        '{}/features/steps/webserver.py',
+    ).load_module('steps.webserver')
+
+    webserver = w.Webserver(port)
+    webserver.start()
+'''
+
     _tmp_path_factory: TempPathFactory
     _env: Dict[str, str]
     _validators: Dict[Optional[str], List[End2EndValidator]]
     _distributed: bool
 
     _after_features: Dict[str, Callable[[BehaveContext, Feature], None]]
     _before_features: Dict[str, Callable[[BehaveContext, Feature], None]]
@@ -635,40 +659,32 @@
 
     _has_pymqi: Optional[bool]
 
     cwd: Path
     test_tmp_dir: Path
     _tmp_path_factory_basetemp: Optional[Path]
     webserver: Webserver
+    profile: Optional[Profile]
 
     def __init__(self, tmp_path_factory: TempPathFactory, webserver: Webserver, distributed: bool) -> None:
         self.test_tmp_dir = (Path(__file__) / '..' / '..' / '.pytest_tmp').resolve()
         self._tmp_path_factory_basetemp = tmp_path_factory._basetemp
         self.webserver = webserver
         tmp_path_factory._basetemp = self.test_tmp_dir
 
         self._tmp_path_factory = tmp_path_factory
-        self.cwd = Path(getcwd())
+        self.cwd = Path.cwd()
         self._env = {}
         self._validators = {}
         self._root = None
         self._after_features = {}
         self._before_features = {}
         self._distributed = distributed
         self._has_pymqi = None
-
-    @property
-    def mode_root(self) -> Path:
-        if self._root is None:
-            raise AttributeError('root is not set')
-
-        if self._distributed:
-            return self.cwd
-        else:
-            return self._root
+        self.profile = None
 
     @property
     def root(self) -> Path:
         if self._root is None:
             raise AttributeError('root is not set')
 
         return self._root
@@ -691,14 +707,18 @@
             requirements_file = self.root / 'requirements.txt'
 
             self._has_pymqi = '[mq]' in requirements_file.read_text()
 
         return self._has_pymqi
 
     def __enter__(self) -> 'End2EndFixture':
+        if environ.get('PROFILE', None) is not None:
+            self.profile = Profile()
+            self.profile.enable()
+
         project_name = 'test-project'
         test_context = self._tmp_path_factory.mktemp('test_context')
 
         virtual_env_path = test_context / 'grizzly-venv'
 
         # create virtualenv
         rc, output = run_command(
@@ -754,74 +774,48 @@
 
         self._root = test_context / project_name
 
         assert self._root.is_dir()
 
         (self._root / 'features' / f'{project_name}.feature').unlink()
 
-        step_start_webserver = '''
-
-@then(u'start webserver on master port "{{port:d}}"')
-def step_start_webserver(context: Context, port: int) -> None:
-    from grizzly.locust import on_master
-    if not on_master(context):
-        return
-
-    from importlib.machinery import SourceFileLoader
-
-    w = SourceFileLoader(
-        'steps.webserver',
-        '{}/features/steps/webserver.py',
-    ).load_module('steps.webserver')
-
-    webserver = w.Webserver(port)
-    webserver.start()
-'''
-
         # create base test-project ... steps.py
-        with open(self._root / 'features' / 'steps' / 'steps.py', 'w') as fd:
+        with open(self.root / 'features' / 'steps' / 'steps.py', 'w') as fd:
             fd.write('from importlib import import_module\n')
             fd.write('from typing import cast, Callable, Any\n\n')
             fd.write('from grizzly.types.behave import Context, then\n')
             fd.write('from grizzly.locust import on_master, on_worker, on_local\n')
             fd.write('from grizzly.context import GrizzlyContext, GrizzlyContextScenario\n')
             fd.write('from grizzly.tasks import GrizzlyTask\n')
             fd.write('from grizzly.scenarios import GrizzlyScenario\n')
             fd.write('from grizzly.steps import *\n')
 
         if self._distributed:
-            # copy examples
-            source = (Path(__file__) / '..' / '..' / 'example').resolve()
-            destination = test_context / 'test-example'
-            copytree(source, destination)
-
             # rewrite test requirements.txt to point to local code
-            for root in [self._root, destination]:
-                with open(f'{root}/requirements.txt', 'r+') as fd:
-                    fd.truncate(0)
-                    fd.flush()
-                    fd.write('grizzly-loadtester\n')
-
-                with open(root / 'features' / 'steps' / 'steps.py', 'a') as fd:
-                    fd.write(
-                        step_start_webserver.format(
-                            str(root).replace(f'{Path.cwd()}', '/srv/grizzly'),
-                        )
+            with open(f'{self.root}/requirements.txt', 'r+') as fd:
+                fd.truncate(0)
+                fd.flush()
+                fd.write('grizzly-loadtester\n')
+
+            with open(self.root / 'features' / 'steps' / 'steps.py', 'a') as fd:
+                fd.write(
+                    self.step_start_webserver.format(
+                        str(self.root).replace(str(self.root), '/srv/grizzly'),
                     )
+                )
 
-                # create steps/webserver.py
-                webserver_source = self.test_tmp_dir.parent / 'tests' / 'webserver.py'
-                webserver_destination = root / 'features' / 'steps' / 'webserver.py'
-
-                webserver_destination.write_text(webserver_source.read_text())
+            # create steps/webserver.py
+            webserver_source = self.test_tmp_dir.parent / 'tests' / 'webserver.py'
+            webserver_destination = self.root / 'features' / 'steps' / 'webserver.py'
+            webserver_destination.write_text(webserver_source.read_text())
 
-            command = ['grizzly-cli', 'dist', '--project-name', self._root.name, 'build', '--no-cache', '--local-install']
+            command = ['grizzly-cli', 'dist', '--project-name', self.root.name, 'build', '--no-cache', '--local-install']
             rc, output = run_command(
                 command,
-                cwd=str(self.mode_root),
+                cwd=str(self.cwd),
                 env=self._env,
             )
             try:
                 assert rc == 0
             except AssertionError:
                 print(''.join(output))
                 raise
@@ -841,35 +835,43 @@
                 assert rc == 0
             except AssertionError:
                 print(''.join(output))
                 raise
 
         return self
 
+    @property
+    def keep_files(self) -> bool:
+        return environ.get('KEEP_FILES', None) is not None
+
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Literal[True]:
         # reset fixture basetemp
         self._tmp_path_factory._basetemp = self._tmp_path_factory_basetemp
 
+        if self.profile is not None:
+            self.profile.disable()
+            self.profile.dump_stats('grizzly-e2e-tests.hprof')
+
         if exc is None:
-            if self._distributed:
+            if self._distributed and not self.keep_files:
                 rc, output = run_command(
                     ['grizzly-cli', 'dist', '--project-name', self.root.name, 'clean'],
-                    cwd=str(self.mode_root),
+                    cwd=str(self.root),
                     env=self._env,
                 )
 
                 if rc != 0:
                     print(''.join(output))
 
-            if environ.get('KEEP_FILES', None) is None:
+            if not self.keep_files:
                 try:
                     rmtree(self.root.parent, onerror=onerror)
                 except AttributeError:
                     pass
             else:
                 print(self._root)
 
@@ -1061,52 +1063,58 @@
                 fd.write(source + '\n\n')
 
         # step validators are are now "burned"...
         self._validators.clear()
 
         return feature_file_name
 
-    def execute(self, feature_file: str, env_conf_file: Optional[str] = None, testdata: Optional[Dict[str, str]] = None) -> Tuple[int, List[str]]:
-        if self._distributed:
-            root = (Path(__file__) / '..' / '..').resolve()
-            feature_file_root = str(self.root).replace(f'{root}/', '')
-            feature_file = f'{feature_file_root}/{feature_file}'
-
-        command = [
-            'grizzly-cli',
-            self.mode,
-            'run',
-            '--yes',
-            '--verbose',
-            feature_file,
-        ]
+    def execute(self, feature_file: str, env_conf: Optional[Dict[str, Any]] = None, testdata: Optional[Dict[str, str]] = None) -> Tuple[int, List[str]]:
+        env_conf_fd: Any
+        if env_conf is not None:
+            prefix = path.basename(feature_file).replace('.feature', '')
+            env_conf_fd = NamedTemporaryFile(delete=not self.keep_files, prefix=prefix, suffix='.yaml', dir=(self.root / 'environments'))
+        else:
+            env_conf_fd = nullcontext()
 
-        if self._distributed:
-            command = command[:2] + ['--project-name', self.root.name] + command[2:]
+        with env_conf_fd as env_conf_file:
+            command = [
+                'grizzly-cli',
+                self.mode,
+                'run',
+                '--yes',
+                '--verbose',
+                feature_file,
+            ]
 
-        if env_conf_file is not None:
-            command += ['-e', env_conf_file]
+            if self._distributed:
+                command = command[:2] + ['--project-name', self.root.name] + command[2:]
 
-        if testdata is not None:
-            for key, value in testdata.items():
-                command += ['-T', f'{key}={value}']
+            if env_conf is not None:
+                env_conf_file.write(yaml.dump(env_conf, Dumper=yaml.Dumper).encode())
+                env_conf_file.flush()
+                env_conf_path = str(env_conf_file.name).replace(f'{self.root}/', '')
+                command += ['-e', env_conf_path]
+
+            if testdata is not None:
+                for key, value in testdata.items():
+                    command += ['-T', f'{key}={value}']
 
-        rc, output = run_command(
-            command,
-            cwd=str(self.mode_root),
-            env=self._env,
-        )
+            rc, output = run_command(
+                command,
+                cwd=str(self.root),
+                env=self._env,
+            )
 
-        if rc != 0:
-            print(''.join(output))
+            if rc != 0:
+                print(''.join(output))
 
-            for container in ['master', 'worker'] if self._distributed else []:
-                command = ['docker', 'container', 'logs', f'{self.root.name}-{getuser()}_{container}_1']
-                _, output = run_command(
-                    command,
-                    cwd=str(self.mode_root),
-                    env=self._env,
-                )
+                for container in ['master', 'worker'] if self._distributed else []:
+                    command = ['docker', 'container', 'logs', f'{self.root.name}-{getuser()}_{container}_1']
+                    _, output = run_command(
+                        command,
+                        cwd=str(self.root),
+                        env=self._env,
+                    )
 
-                print(''.join(output))
+                    print(''.join(output))
 
-        return rc, output
+            return rc, output
```

### Comparing `grizzly-loadtester-2.6.2/tests/helpers.py` & `grizzly-loadtester-2.6.3/tests/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,20 @@
 
     def __init__(self, name: Optional[str] = None, scenario: Optional[GrizzlyContextScenario] = None) -> None:
         super().__init__(scenario)
         self.name = name
         self.call_count = 0
         self.task_call_count = 0
 
+    def on_start(self, parent: 'GrizzlyScenario') -> None:
+        return
+
+    def on_stop(self, parent: 'GrizzlyScenario') -> None:
+        return
+
     def __call__(self) -> grizzlytask:
         self.call_count += 1
 
         @grizzlytask
         def task(parent: 'GrizzlyScenario') -> Any:
             parent.user.environment.events.request.fire(
                 request_type='TSTSK',
@@ -100,14 +106,22 @@
                 response_length=37,
                 context=fastdeepcopy(parent.user._context),
                 exception=None,
             )
             self.task_call_count += 1
             parent.user.logger.debug(f'{self.name} executed')
 
+        @task.on_start
+        def on_start(parent: 'GrizzlyScenario') -> None:
+            self.on_start(parent)
+
+        @task.on_stop
+        def on_stop(parent: 'GrizzlyScenario') -> None:
+            self.on_stop(parent)
+
         return task
 
 
 class ResultSuccess(Exception):
     pass
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/test___init__.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/test_appinsights.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_appinsights.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/listeners/test_influxdb.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/listeners/test_influxdb.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/scenarios/test_iterator.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/scenarios/test_iterator.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/background/test_setup.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/background/test_shapes.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/background/test_shapes.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_response.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_response.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_results.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_results.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_setup.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_tasks.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -375,52 +375,104 @@
 <document>
     <id>DOCUMENT_8483-1</id>
     <title>TPM Report {{ year }}</title>
 </document>
         '''
 
 
-def test_step_task_client_get_endpoint(behave_fixture: BehaveFixture) -> None:
+def test_step_task_client_get_endpoint_payload_metadata(behave_fixture: BehaveFixture) -> None:
     behave = behave_fixture.context
     grizzly = cast(GrizzlyContext, behave.grizzly)
 
     with pytest.raises(AssertionError) as ae:
-        step_task_client_get_endpoint(behave, 'obscure.example.com', 'step-name', 'test')
+        step_task_client_get_endpoint_payload_metadata(behave, 'obscure.example.com', 'step-name', 'test', 'metadata')
     assert 'could not find scheme in "obscure.example.com"' in str(ae)
 
     with pytest.raises(AssertionError) as ae:
-        step_task_client_get_endpoint(behave, 'obscure://obscure.example.com', 'step-name', 'test')
+        step_task_client_get_endpoint_payload_metadata(behave, 'obscure://obscure.example.com', 'step-name', 'test', 'metadata')
     assert 'no client task registered for obscure' in str(ae)
 
     with pytest.raises(ValueError) as ve:
-        step_task_client_get_endpoint(behave, 'http://www.example.org', 'step-name', 'test')
+        step_task_client_get_endpoint_payload_metadata(behave, 'http://www.example.org', 'step-name', 'test', 'metadata')
     assert 'HttpClientTask: variable test has not been initialized' in str(ve)
 
     if pymqi.__name__ != 'grizzly_extras.dummy_pymqi':
         with pytest.raises(ValueError) as ve:
-            step_task_client_get_endpoint(behave, 'mq://mq.example.org', 'step-name', 'test')
+            step_task_client_get_endpoint_payload_metadata(behave, 'mq://mq.example.org', 'step-name', 'test', 'metadata')
+        assert 'MessageQueueClientTask: variable test has not been initialized' in str(ve)
+
+    grizzly.state.variables['test'] = 'none'
+
+    with pytest.raises(ValueError) as ve:
+        step_task_client_get_endpoint_payload_metadata(behave, 'http://www.example.org', 'step-name', 'test', 'metadata')
+    assert 'HttpClientTask: variable metadata has not been initialized' in str(ve)
+
+    if pymqi.__name__ != 'grizzly_extras.dummy_pymqi':
+        with pytest.raises(ValueError) as ve:
+            step_task_client_get_endpoint_payload_metadata(behave, 'mq://mq.example.org', 'step-name', 'test', 'metadata')
+        assert 'MessageQueueClientTask: variable metadata has not been initialized' in str(ve)
+
+    grizzly.state.variables['metadata'] = 'none'
+
+    assert len(grizzly.scenario.tasks()) == 0
+    step_task_client_get_endpoint_payload_metadata(behave, 'http://www.example.org', 'step-name', 'test', 'metadata')
+    assert len(grizzly.scenario.tasks()) == 1
+
+    grizzly.state.variables['endpoint_url'] = 'https://example.org'
+    step_task_client_get_endpoint_payload_metadata(behave, 'https://{{ endpoint_url }}', 'step-name', 'test', 'metadata')
+
+    task = grizzly.scenario.tasks()[-1]
+    assert isinstance(task, HttpClientTask)
+    assert task.endpoint == '{{ endpoint_url }}'
+    assert sorted(task.get_templates()) == sorted(['{{ endpoint_url }}', '{{ test }} {{ metadata }}'])
+
+    behave.text = '1=1'
+    with pytest.raises(NotImplementedError) as nie:
+        step_task_client_get_endpoint_payload_metadata(behave, 'https://{{ endpoint_url }}', 'step-name', 'test', 'metadata')
+    assert str(nie.value) == 'HttpClientTask has not implemented support for step text'
+
+
+def test_step_task_client_get_endpoint_payload(behave_fixture: BehaveFixture) -> None:
+    behave = behave_fixture.context
+    grizzly = cast(GrizzlyContext, behave.grizzly)
+
+    with pytest.raises(AssertionError) as ae:
+        step_task_client_get_endpoint_payload(behave, 'obscure.example.com', 'step-name', 'test')
+    assert 'could not find scheme in "obscure.example.com"' in str(ae)
+
+    with pytest.raises(AssertionError) as ae:
+        step_task_client_get_endpoint_payload(behave, 'obscure://obscure.example.com', 'step-name', 'test')
+    assert 'no client task registered for obscure' in str(ae)
+
+    with pytest.raises(ValueError) as ve:
+        step_task_client_get_endpoint_payload(behave, 'http://www.example.org', 'step-name', 'test')
+    assert 'HttpClientTask: variable test has not been initialized' in str(ve)
+
+    if pymqi.__name__ != 'grizzly_extras.dummy_pymqi':
+        with pytest.raises(ValueError) as ve:
+            step_task_client_get_endpoint_payload(behave, 'mq://mq.example.org', 'step-name', 'test')
         assert 'MessageQueueClientTask: variable test has not been initialized' in str(ve)
 
     grizzly.state.variables['test'] = 'none'
 
     assert len(grizzly.scenario.tasks()) == 0
-    step_task_client_get_endpoint(behave, 'http://www.example.org', 'step-name', 'test')
+    step_task_client_get_endpoint_payload(behave, 'http://www.example.org', 'step-name', 'test')
     assert len(grizzly.scenario.tasks()) == 1
 
     grizzly.state.variables['endpoint_url'] = 'https://example.org'
-    step_task_client_get_endpoint(behave, 'https://{{ endpoint_url }}', 'step-name', 'test')
+    step_task_client_get_endpoint_payload(behave, 'https://{{ endpoint_url }}', 'step-name', 'test')
 
     task = grizzly.scenario.tasks()[-1]
     assert isinstance(task, HttpClientTask)
     assert task.endpoint == '{{ endpoint_url }}'
     assert sorted(task.get_templates()) == sorted(['{{ endpoint_url }}', '{{ test }}'])
 
     behave.text = '1=1'
     with pytest.raises(NotImplementedError) as nie:
-        step_task_client_get_endpoint(behave, 'https://{{ endpoint_url }}', 'step-name', 'test')
+        step_task_client_get_endpoint_payload(behave, 'https://{{ endpoint_url }}', 'step-name', 'test')
     assert str(nie.value) == 'HttpClientTask has not implemented support for step text'
 
 
 def test_step_task_client_get_endpoint_until(behave_fixture: BehaveFixture) -> None:
     behave = behave_fixture.context
     grizzly = cast(GrizzlyContext, behave.grizzly)
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/scenario/test_user.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/scenario/test_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/test__helpers.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test__helpers.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/steps/test_setup.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/steps/test_setup.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_blobstorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,16 @@
             source='',
         )
 
         assert isinstance(task.service_client, BlobServiceClient)
         assert task.endpoint == 'bs://my-storage?AccountKey=aaaabbb=&Container=my-container'
         assert task.name is None
         assert task.source == ''
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.destination is None
         assert task._endpoints_protocol == 'http'
         assert task.account_name == 'my-storage'
         assert task.account_key == 'aaaabbb='
         assert task.container == 'my-container'
         assert task.connection_string == 'DefaultEndpointsProtocol=http;AccountName=my-storage;AccountKey=aaaabbb=;EndpointSuffix=core.windows.net'
         assert not task.overwrite
@@ -83,15 +84,16 @@
             source='',
         )
 
         assert isinstance(task.service_client, BlobServiceClient)
         assert task.endpoint == 'bss://my-storage?AccountKey=aaaabbb=&Container=my-container&Overwrite=True'
         assert task.name == 'upload-empty-file'
         assert task.source == ''
-        assert task.variable is None
+        assert task.payload_variable is None
+        assert task.metadata_variable is None
         assert task.destination is None
         assert task._endpoints_protocol == 'https'
         assert task.account_name == 'my-storage'
         assert task.account_key == 'aaaabbb='
         assert task.container == 'my-container'
         assert task.connection_string == 'DefaultEndpointsProtocol=https;AccountName=my-storage;AccountKey=aaaabbb=;EndpointSuffix=core.windows.net'
         assert task.overwrite
@@ -119,15 +121,15 @@
         behave = behave_fixture.context
         grizzly = cast(GrizzlyContext, behave.grizzly)
         grizzly.state.variables['test'] = 'none'
 
         task_factory = BlobStorageClientTask(
             RequestDirection.FROM,
             'bs://my-storage?AccountKey=aaaabbb=&Container=my-container',
-            variable='test',
+            payload_variable='test',
         )
         task = task_factory()
 
         _, _, scenario = grizzly_fixture()
         assert scenario is not None
 
         with pytest.raises(NotImplementedError) as nie:
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_http.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import cast
 from json import dumps as jsondumps, loads as jsonloads
 
 import pytest
 
 from pytest_mock import MockerFixture
 from requests import Response
+from requests.structures import CaseInsensitiveDict
 
 from grizzly_extras.transformer import TransformerContentType
 from grizzly.context import GrizzlyContext
 from grizzly.tasks.clients import HttpClientTask
 from grizzly.exceptions import RestartScenario
 from grizzly.types import RequestDirection
 from grizzly.types.locust import StopUser, CatchResponseError
@@ -18,59 +19,72 @@
 
 class TestHttpClientTask:
     def test_get(self, mocker: MockerFixture, grizzly_fixture: GrizzlyFixture) -> None:
         behave = grizzly_fixture.behave
         grizzly = cast(GrizzlyContext, behave.grizzly)
 
         with pytest.raises(AttributeError) as ae:
-            HttpClientTask(RequestDirection.TO, 'http://example.org', variable='test')
+            HttpClientTask(RequestDirection.TO, 'http://example.org', payload_variable='test')
         assert 'HttpClientTask: variable argument is not applicable for direction TO' in str(ae.value)
 
         with pytest.raises(AttributeError) as ae:
             HttpClientTask(RequestDirection.FROM, 'http://example.org', source='test')
         assert 'HttpClientTask: source argument is not applicable for direction FROM' in str(ae.value)
 
         with pytest.raises(ValueError) as ve:
-            HttpClientTask(RequestDirection.FROM, 'http://example.org', variable='test')
+            HttpClientTask(RequestDirection.FROM, 'http://example.org', payload_variable='test')
+        assert 'HttpClientTask: variable test has not been initialized' in str(ve)
+
+        with pytest.raises(ValueError) as ve:
+            HttpClientTask(RequestDirection.FROM, 'http://example.org', payload_variable=None, metadata_variable='test')
         assert 'HttpClientTask: variable test has not been initialized' in str(ve)
 
         response = Response()
         response.url = 'http://example.org'
         response._content = jsondumps({'hello': 'world'}).encode()
         response.status_code = 200
 
         requests_get_spy = mocker.patch(
             'grizzly.tasks.clients.http.requests.get',
             side_effect=[response, RuntimeError, RuntimeError, RuntimeError, RuntimeError, response, response, response, response]
         )
 
         grizzly.state.variables.update({'test': 'none'})
 
+        with pytest.raises(ValueError) as ve:
+            HttpClientTask(RequestDirection.FROM, 'http://example.org', payload_variable=None, metadata_variable='test')
+        assert 'HttpClientTask: payload variable is not set, but metadata variable is set' in str(ve)
+
         _, _, scenario = grizzly_fixture()
 
         assert scenario is not None
 
         request_fire_spy = mocker.spy(scenario.user.environment.events.request, 'fire')
 
-        task_factory = HttpClientTask(RequestDirection.FROM, 'http://example.org', variable='test')
+        grizzly.state.variables.update({'test_payload': 'none', 'test_metadata': 'none'})
+
+        task_factory = HttpClientTask(RequestDirection.FROM, 'http://example.org', payload_variable='test_payload', metadata_variable='test_metadata')
         assert task_factory.arguments == {}
         assert task_factory.__template_attributes__ == {'endpoint', 'destination', 'source', 'name', 'variable_template'}
 
         task = task_factory()
 
         assert callable(task)
 
-        assert scenario.user._context['variables'].get('test', None) is None
+        assert scenario.user._context['variables'].get('test_payload', None) is None
+        assert scenario.user._context['variables'].get('test_metadata', None) is None
 
         task_factory.name = 'test-1'
         response.status_code = 400
+        response.headers = CaseInsensitiveDict({'x-foo-bar': 'test'})
 
         task(scenario)
 
-        assert scenario.user._context['variables'].get('test', '') == jsondumps({'hello': 'world'})
+        assert scenario.user._context['variables'].get('test_payload', '') == jsondumps({'hello': 'world'})
+        assert scenario.user._context['variables'].get('test_metadata', '') == jsondumps({'x-foo-bar': 'test'})
         assert requests_get_spy.call_count == 1
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'http://example.org'
         assert len(kwargs) == 1
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
 
         assert request_fire_spy.call_count == 1
@@ -89,15 +103,15 @@
         request_log = request_logs[-1]
         log_entry = jsonloads(request_log.read_text())
         assert log_entry.get('request', {}).get('time', None) >= 0.0
         assert log_entry.get('request', {}).get('url', None) == 'http://example.org'
         assert log_entry.get('request', {}).get('metadata', None) is not None
         assert log_entry.get('request', {}).get('payload', '') is None
         assert log_entry.get('response', {}).get('url', None) == 'http://example.org'
-        assert log_entry.get('response', {}).get('metadata', None) == {}
+        assert log_entry.get('response', {}).get('metadata', None) == {'x-foo-bar': 'test'}
         assert log_entry.get('response', {}).get('payload', None) is not None
         assert log_entry.get('response', {}).get('status', None) == 400
 
         scenario.user._context['variables']['test'] = None
         response.status_code = 200
         task_factory.name = 'test-2'
 
@@ -147,15 +161,15 @@
         assert kwargs.get('response_length') == 0
         assert kwargs.get('context', None) is scenario.user._context
         assert isinstance(kwargs.get('exception', None), RuntimeError)
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 4
 
         scenario.user._scenario.failure_exception = None
 
-        task_factory = HttpClientTask(RequestDirection.FROM, 'http://example.org', 'http-get', variable='test')
+        task_factory = HttpClientTask(RequestDirection.FROM, 'http://example.org', 'http-get', payload_variable='test')
         task = task_factory()
         assert task_factory.arguments == {}
         assert task_factory.content_type == TransformerContentType.UNDEFINED
 
         task(scenario)
 
         assert scenario.user._context['variables'].get('test', '') is None  # not set
@@ -173,30 +187,30 @@
         assert kwargs.get('response_length') == 0
         assert kwargs.get('context', None) is scenario.user._context
         assert isinstance(kwargs.get('exception', None), RuntimeError)
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 5
 
         grizzly.state.configuration['test.host'] = 'https://example.org'
 
-        task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test', 'http-env-get', variable='test')
+        task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test', 'http-env-get', payload_variable='test')
         assert task_factory.arguments == {'verify': True}
         assert task_factory.content_type == TransformerContentType.UNDEFINED
         task = task_factory()
 
         task(scenario)
 
         assert requests_get_spy.call_count == 6
         args, kwargs = requests_get_spy.call_args_list[-1]
         assert args[0] == 'https://example.org/api/test'
         assert len(kwargs) == 2
         assert kwargs.get('verify', None)
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 5
 
-        task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=False, content_type=json', 'http-env-get-1', variable='test')
+        task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=False, content_type=json', 'http-env-get-1', payload_variable='test')
         task = task_factory()
         assert task_factory.arguments == {'verify': False}
         assert task_factory.content_type == TransformerContentType.JSON
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 5
 
         task(scenario)
 
@@ -205,15 +219,15 @@
         assert args[0] == 'https://example.org/api/test'
         assert len(kwargs) == 2
         assert not kwargs.get('verify', None)
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
         assert request_fire_spy.call_count == 7
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 5
 
-        task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=True, content_type=json', 'http-env-get-2', variable='test')
+        task_factory = HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=True, content_type=json', 'http-env-get-2', payload_variable='test')
         task = task_factory()
         assert task_factory.arguments == {'verify': True}
         assert task_factory.content_type == TransformerContentType.JSON
 
         scenario.user._scenario.context['log_all_requests'] = True
 
         task(scenario)
@@ -225,15 +239,15 @@
         assert kwargs.get('verify', None)
         assert kwargs.get('headers', {}).get('x-grizzly-user', None).startswith('HttpClientTask::')
         assert request_fire_spy.call_count == 8
         args, kwargs = request_fire_spy.call_args_list[-1]
         assert len(list(task_factory.log_dir.rglob('**/*'))) == 6
 
         with pytest.raises(NotImplementedError) as nie:
-            HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=True, content_type=json', 'http-env-get-2', variable='test', text='foobar')
+            HttpClientTask(RequestDirection.FROM, 'https://$conf::test.host$/api/test | verify=True, content_type=json', 'http-env-get-2', payload_variable='test', text='foobar')
         assert str(nie.value) == 'HttpClientTask has not implemented support for step text'
 
     def test_put(self, grizzly_fixture: GrizzlyFixture) -> None:
         task_factory = HttpClientTask(RequestDirection.TO, 'http://put.example.org', source='')
         task = task_factory()
 
         _, _, scenario = grizzly_fixture()
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_messagequeue.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pytest_mock import MockerFixture
 
 import zmq.green as zmq
 from zmq.error import Again as ZMQAgain
 
 from grizzly.tasks.clients import MessageQueueClientTask
 from grizzly.types import RequestDirection
+from grizzly_extras.async_message import AsyncMessageError
 
 try:
     import pymqi
 except:
     from grizzly_extras import dummy_pymqi as pymqi
 
 from tests.fixtures import GrizzlyFixture, NoopZmqFixture
@@ -73,15 +74,16 @@
             assert create_client_mocked.call_count == 0
 
             assert isinstance(task_factory._zmq_context, zmq.Context)
             assert task_factory._zmq_url == 'tcp://127.0.0.1:5554'
             assert task_factory._worker == {}
             assert task_factory.endpoint == 'mqs://localhost:1'
             assert task_factory.name is None
-            assert task_factory.variable is None
+            assert task_factory.payload_variable is None
+            assert task_factory.metadata_variable is None
             assert task_factory.destination is None
             assert task_factory.source is None
             assert not hasattr(task_factory, 'scenario')
             assert task_factory.__template_attributes__ == {'endpoint', 'destination', 'source', 'name', 'variable_template'}
         finally:
             if zmq_context is not None:
                 zmq_context.destroy()
@@ -95,15 +97,16 @@
             assert create_client_mocked.call_count == 0
 
             assert isinstance(task_factory._zmq_context, zmq.Context)
             assert task_factory._zmq_url == 'tcp://127.0.0.1:5554'
             assert task_factory._worker == {}
             assert task_factory.endpoint == 'mqs://localhost:1'
             assert task_factory.name == 'messagequeue-request'
-            assert task_factory.variable is None
+            assert task_factory.payload_variable is None
+            assert task_factory.metadata_variable is None
             assert task_factory.destination is None
             assert task_factory.source is None
             assert not hasattr(task_factory, 'scenario')
 
             with pytest.raises(NotImplementedError) as nie:
                 MessageQueueClientTask(RequestDirection.FROM, 'mqs://localhost:1', 'messagequeue-request', text='foobar')
             assert str(nie.value) == 'MessageQueueClientTask has not implemented support for step text'
@@ -297,43 +300,43 @@
             assert args[1] == 0
 
             assert close_mock.call_count == 1
         finally:
             if zmq_context is not None:
                 zmq_context.destroy()
 
-    def test_connect(self, grizzly_fixture: GrizzlyFixture, noop_zmq: NoopZmqFixture) -> None:
+    def test_connect(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture, noop_zmq: NoopZmqFixture) -> None:
         noop_zmq('grizzly.tasks.clients.messagequeue')
 
-        recv_json_mock = noop_zmq.get_mock('recv_json')
-        send_json_mock = noop_zmq.get_mock('send_json')
-
-        recv_json_mock.side_effect = [ZMQAgain, None]
-
         zmq_context: Optional[zmq.Context] = None
         try:
             task_factory = MessageQueueClientTask(
                 RequestDirection.FROM,
                 'mqs://mq_username:mq_password@mq.example.io/topic:INCOMING.MSG?QueueManager=QM01&Channel=TCP.IN',
             )
             zmq_context = task_factory._zmq_context
 
             with task_factory.create_client() as client:
+                recv_json_mock = mocker.patch.object(client, 'recv_json')
+                send_json_mock = mocker.patch.object(client, 'send_json')
+                recv_json_mock.side_effect = [ZMQAgain, None]
+
                 meta: Dict[str, Any] = {}
-                with pytest.raises(RuntimeError) as re:
+                with pytest.raises(AsyncMessageError) as ame:
                     task_factory.connect(111111, client, meta)
-                assert str(re.value) == 'no response when trying to connect'
+                assert str(ame.value) == 'no response'
                 assert meta.get('response_length', None) == 0
                 assert meta.get('action', None) == 'topic:INCOMING.MSG'
                 assert meta.get('direction', None) == '<->'
 
                 assert send_json_mock.call_count == 1
                 args, kwargs = send_json_mock.call_args_list[-1]
                 assert args == ({
                     'action': 'CONN',
+                    'client': 111111,
                     'context': {
                         'url': task_factory.endpoint,
                         'connection': 'mq.example.io(1414)',
                         'queue_manager': 'QM01',
                         'channel': 'TCP.IN',
                         'username': 'mq_username',
                         'password': 'mq_password',
@@ -350,17 +353,17 @@
                 _, kwargs = recv_json_mock.call_args_list[-1]
                 assert kwargs.get('flags', None) == zmq.NOBLOCK
 
                 meta = {}
                 message = {'success': False, 'message': 'unknown error yo'}
                 recv_json_mock.side_effect = [message]
 
-                with pytest.raises(RuntimeError) as re:
+                with pytest.raises(AsyncMessageError) as ame:
                     task_factory.connect(222222, client, meta)
-                assert str(re.value) == 'unknown error yo'
+                assert str(ame.value) == 'unknown error yo'
 
                 assert send_json_mock.call_count == 2
                 assert recv_json_mock.call_count == 3
                 assert meta.get('response_length', None) == 0
                 assert meta.get('action', None) == 'topic:INCOMING.MSG'
 
                 meta = {}
@@ -383,20 +386,25 @@
             task_factory = MessageQueueClientTask(
                 RequestDirection.FROM,
                 'mqs://mq_username:mq_password@mq.example.io/topic:INCOMING.MSG?QueueManager=QM01&Channel=TCP.IN&HeaderType=RFH2',
             )
             zmq_context = task_factory._zmq_context
 
             with task_factory.create_client() as client:
+                recv_json_mock = mocker.patch.object(client, 'recv_json')
+                send_json_mock = mocker.patch.object(client, 'send_json')
+
                 task_factory.connect(444444, client, meta)
-                assert send_json_mock.call_count == 4
-                assert recv_json_mock.call_count == 5
+
+                assert send_json_mock.call_count == 1
+                assert recv_json_mock.call_count == 1
                 args, kwargs = send_json_mock.call_args_list[-1]
                 assert args == ({
                     'action': 'CONN',
+                    'client': 444444,
                     'context': {
                         'url': task_factory.endpoint,
                         'connection': 'mq.example.io(1414)',
                         'queue_manager': 'QM01',
                         'channel': 'TCP.IN',
                         'username': 'mq_username',
                         'password': 'mq_password',
@@ -405,58 +413,59 @@
                         'ssl_cipher': 'ECDHE_RSA_AES_256_GCM_SHA384',
                         'message_wait': None,
                         'heartbeat_interval': None,
                         'header_type': 'rfh2',
                     },
                 },)
                 assert kwargs == {}
-
         finally:
             if zmq_context is not None:
                 zmq_context.destroy()
 
     def test_get(self, mocker: MockerFixture, noop_zmq: NoopZmqFixture, grizzly_fixture: GrizzlyFixture) -> None:
         noop_zmq('grizzly.tasks.clients.messagequeue')
 
         _, _, scenario = grizzly_fixture()
 
         assert scenario is not None
 
-        scenario.grizzly.state.variables['mq-client-var'] = 'none'
+        scenario.grizzly.state.variables.update({'mq-client-var': 'none', 'mq-client-metadata': 'none'})
 
         fire_spy = mocker.spy(scenario.user.environment.events.request, 'fire')
 
         recv_json_mock = noop_zmq.get_mock('recv_json')
         send_json_mock = noop_zmq.get_mock('send_json')
 
         recv_json_mock.side_effect = [ZMQAgain, None]
 
         zmq_context: Optional[zmq.Context] = None
         try:
             task_factory = MessageQueueClientTask(
                 RequestDirection.FROM,
                 'mqs://mq_username:mq_password@mq.example.io/topic:INCOMING.MSG?QueueManager=QM01&Channel=TCP.IN',
-                variable='mq-client-var',
+                payload_variable='mq-client-var',
             )
             zmq_context = task_factory._zmq_context
 
             task = task_factory()
 
             messages: List[Any] = [{'success': True, 'message': 'hello there', 'worker': 'dddd-eeee-ffff-9999'}, ZMQAgain, None]
             recv_json_mock.side_effect = messages
 
             task(scenario)
 
             assert scenario.user._context['variables'].get('mq-client-var', None) is None
-            assert task_factory._worker.get(id(scenario), None) == 'dddd-eeee-ffff-9999'
+            assert scenario.user._context['variables'].get('mq-client-metadata', None) is None
+            assert task_factory._worker.get(id(scenario.user), None) == 'dddd-eeee-ffff-9999'
             assert send_json_mock.call_count == 2
             args, kwargs = send_json_mock.call_args_list[-1]
             assert args == ({
                 'action': 'GET',
                 'worker': 'dddd-eeee-ffff-9999',
+                'client': id(scenario.user),
                 'context': {
                     'endpoint': 'topic:INCOMING.MSG',
                 },
                 'payload': None,
             },)
             assert kwargs == {}
             assert recv_json_mock.call_count == 3
@@ -465,33 +474,35 @@
             _, kwargs = fire_spy.call_args_list[-1]  # get
             assert kwargs.get('request_type', None) == 'CLTSK'
             assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} MessageQueue<-topic:INCOMING.MSG'
             assert kwargs.get('response_time', None) >= 0.0
             assert kwargs.get('response_length', None) == 0
             assert kwargs.get('context', None) == scenario.user._context
             exception = kwargs.get('exception', None)
-            assert isinstance(exception, RuntimeError)
+            assert isinstance(exception, AsyncMessageError)
             assert str(exception) == 'no response'
 
             messages = [{'success': False, 'message': 'memory corruption'}]
             recv_json_mock.side_effect = messages
 
             task_factory.endpoint = 'mqs://mq_username:mq_password@mq.example.io/topic:INCOMING.MSG?QueueManager=QM01&Channel=TCP.IN&MaxMessageSize=13337'
             task_factory.create_context()
 
             task = task_factory()
 
             task(scenario)
 
             assert scenario.user._context['variables'].get('mq-client-var', None) is None
+            assert scenario.user._context['variables'].get('mq-client-metadata', None) is None
             assert send_json_mock.call_count == 3
             args, kwargs = send_json_mock.call_args_list[-1]
             assert args == ({
                 'action': 'GET',
                 'worker': 'dddd-eeee-ffff-9999',
+                'client': id(scenario.user),
                 'context': {
                     'endpoint': 'topic:INCOMING.MSG, max_message_size:13337',
                 },
                 'payload': None,
             },)
             assert kwargs == {}
             assert recv_json_mock.call_count == 4
@@ -500,44 +511,47 @@
             _, kwargs = fire_spy.call_args_list[-1]
             assert kwargs.get('request_type', None) == 'CLTSK'
             assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} MessageQueue<-topic:INCOMING.MSG'
             assert kwargs.get('response_time', None) >= 0.0
             assert kwargs.get('response_length', None) == 0
             assert kwargs.get('context', None) == scenario.user._context
             exception = kwargs.get('exception', None)
-            assert isinstance(exception, RuntimeError)
+            assert isinstance(exception, AsyncMessageError)
             assert str(exception) == 'memory corruption'
 
             messages = [{'success': True, 'payload': None}]
             recv_json_mock.side_effect = messages
 
             task(scenario)
 
             assert scenario.user._context['variables'].get('mq-client-var', None) is None
+            assert scenario.user._context['variables'].get('mq-client-metadata', None) is None
             assert send_json_mock.call_count == 4
             assert recv_json_mock.call_count == 5
 
             assert fire_spy.call_count == 3
             _, kwargs = fire_spy.call_args_list[-1]
             assert kwargs.get('request_type', None) == 'CLTSK'
             assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} MessageQueue<-topic:INCOMING.MSG'
             assert kwargs.get('response_time', None) >= 0.0
             assert kwargs.get('response_length', None) == 0
             assert kwargs.get('context', None) == scenario.user._context
             exception = kwargs.get('exception', None)
             assert isinstance(exception, RuntimeError)
             assert str(exception) == 'response did not contain any payload'
 
-            messages = [{'success': True, 'payload': '{"hello": "world", "foo": "bar"}'}]
+            messages = [{'success': True, 'payload': '{"hello": "world", "foo": "bar"}', 'metadata': {'x-foo-bar': 'test'}}]
             recv_json_mock.side_effect = messages
             task_factory.name = 'mq-get-example'
+            task_factory.metadata_variable = 'mq-client-metadata'
 
             task(scenario)
 
             assert scenario.user._context['variables'].get('mq-client-var', None) == '{"hello": "world", "foo": "bar"}'
+            assert scenario.user._context['variables'].get('mq-client-metadata', None) == '{"x-foo-bar": "test"}'
             assert send_json_mock.call_count == 5
             assert recv_json_mock.call_count == 6
 
             assert fire_spy.call_count == 4
             _, kwargs = fire_spy.call_args_list[-1]
             assert kwargs.get('request_type', None) == 'CLTSK'
             assert kwargs.get('name', None) == f'{scenario.user._scenario.identifier} mq-get-example'
@@ -592,22 +606,23 @@
             messages: List[Any] = [{'success': True, 'message': 'hello there', 'worker': 'dddd-eeee-ffff-9999'}, {'success': True, 'payload': source}]
             recv_json_mock.side_effect = messages
 
             task = task_factory()
 
             task(scenario)
 
-            assert task_factory._worker.get(id(scenario), None) == 'dddd-eeee-ffff-9999'
+            assert task_factory._worker.get(id(scenario.user), None) == 'dddd-eeee-ffff-9999'
 
             assert recv_json_mock.call_count == 2
             assert send_json_mock.call_count == 2
             args, kwargs = send_json_mock.call_args_list[-1]
             assert args == ({
                 'action': 'PUT',
                 'worker': 'dddd-eeee-ffff-9999',
+                'client': id(scenario.user),
                 'context': {
                     'endpoint': 'queue:INCOMING.MSG',
                 },
                 'payload': source,
             },)
             assert kwargs == {}
 
@@ -633,14 +648,15 @@
 
             assert recv_json_mock.call_count == 3
             assert send_json_mock.call_count == 3
             args, kwargs = send_json_mock.call_args_list[-1]
             assert args == ({
                 'action': 'PUT',
                 'worker': 'dddd-eeee-ffff-9999',
+                'client': id(scenario.user),
                 'context': {
                     'endpoint': 'queue:INCOMING.MSG',
                 },
                 'payload': source_file.read_text(),
             },)
             assert kwargs == {}
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/clients/test_servicebus.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/clients/test_servicebus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 
 from typing import Dict, Any
+from json import dumps as jsondumps
+
 import pytest
 
 from _pytest.logging import LogCaptureFixture
 from zmq.sugar.constants import LINGER as ZMQ_LINGER, REQ as ZMQ_REQ
 from grizzly.tasks.clients import ServiceBusClientTask
 from grizzly.types import RequestDirection
 from grizzly_extras.async_message import AsyncMessageRequest
@@ -67,36 +69,71 @@
             RequestDirection.FROM,
             (
                 'sb://$conf::sbns.host$/topic:my-topic/subscription:my-subscription-{{ id }}/expression:$.hello.world'
                 ';SharedAccessKeyName=$conf::sbns.key.name$;SharedAccessKey=$conf::sbns.key.secret$#Consume=True&MessageWait=300&ContentType=json'
             ),
             'test',
             text='foobar',
-            variable='foobar',
+            payload_variable='foobar',
         )
 
         assert task.endpoint == 'sb://sb.windows.net/;SharedAccessKeyName=KeyName;SharedAccessKey=SeCrEtKeY=='
         assert task.context == {
             'url': task.endpoint,
             'connection': 'receiver',
             'endpoint': 'topic:my-topic, subscription:my-subscription-{{ id }}, expression:$.hello.world',
             'consume': True,
             'message_wait': 300,
             'content_type': 'JSON'
         }
         assert task.text == 'foobar'
-        assert task.variable == 'foobar'
+        assert task.payload_variable == 'foobar'
+        assert task.metadata_variable is None
         assert task.source is None
         assert task.worker_id is None
         assert sorted(task.get_templates()) == sorted(['topic:my-topic, subscription:my-subscription-{{ id }}, expression:$.hello.world', '{{ foobar }}'])
         context_mock.assert_called_once_with()
         context_mock.return_value.socket.assert_called_once_with(ZMQ_REQ)
         context_mock.return_value.socket.return_value.connect.assert_called_once_with('tcp://127.0.0.1:5554')
         context_mock.reset_mock()
 
+        grizzly.state.variables.update({'barfoo': 'none'})
+
+        task = ServiceBusClientTask(
+            RequestDirection.FROM,
+            (
+                'sb://$conf::sbns.host$/topic:my-topic/subscription:my-subscription-{{ id }}/expression:$.hello.world'
+                ';SharedAccessKeyName=$conf::sbns.key.name$;SharedAccessKey=$conf::sbns.key.secret$#Consume=True&MessageWait=300&ContentType=json'
+            ),
+            'test',
+            text='foobar',
+            payload_variable='foobar',
+            metadata_variable='barfoo',
+        )
+
+        assert task.endpoint == 'sb://sb.windows.net/;SharedAccessKeyName=KeyName;SharedAccessKey=SeCrEtKeY=='
+        assert task.context == {
+            'url': task.endpoint,
+            'connection': 'receiver',
+            'endpoint': 'topic:my-topic, subscription:my-subscription-{{ id }}, expression:$.hello.world',
+            'consume': True,
+            'message_wait': 300,
+            'content_type': 'JSON'
+        }
+        assert task.text == 'foobar'
+        assert task.payload_variable == 'foobar'
+        assert task.metadata_variable == 'barfoo'
+        assert task.source is None
+        assert task.worker_id is None
+        assert sorted(task.get_templates()) == sorted(['topic:my-topic, subscription:my-subscription-{{ id }}, expression:$.hello.world', '{{ foobar }} {{ barfoo }}'])
+        context_mock.assert_called_once_with()
+        context_mock.return_value.socket.assert_called_once_with(ZMQ_REQ)
+        context_mock.return_value.socket.return_value.connect.assert_called_once_with('tcp://127.0.0.1:5554')
+        context_mock.reset_mock()
+
         task = ServiceBusClientTask(
             RequestDirection.FROM, (
                 'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription'
                 ';SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=#MessageWait=120&ContentType=json'
             ),
             'test',
         )
@@ -192,43 +229,45 @@
         task.connect()
 
         assert task.worker_id == 'foo-bar-baz-foo'
         assert task.endpoint == 'sb://my-sbns.servicebus.windows.net/;SharedAccessKeyName=AccessKey;SharedAccessKey=fooBARfoo'
 
         async_message_request_mock.assert_called_once_with(task.client, {
             'worker': None,
+            'client': id(scenario.user),
             'action': 'HELLO',
             'context': task.context,
         })
 
     def test_disconnect(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
+        _, _, scenario = grizzly_fixture()
+        assert scenario is not None
+
         client_mock = mocker.MagicMock()
 
-        async_message_request_mock = mocker.patch('grizzly.tasks.clients.servicebus.async_message_request_wrapper')
+        async_message_request_mock = mocker.patch('grizzly.utils.async_message_request')
 
         task = ServiceBusClientTask(RequestDirection.FROM, 'sb://my-sbns.servicebus.windows.net/;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=', 'test')
+        task._parent = scenario
 
-        task._parent = mocker.MagicMock()
-
-        # not connected
+        # not connected, don't do anything
         task._client = None
-        with pytest.raises(ConnectionError) as ce:
-            task.disconnect()
-        assert str(ce.value) == 'not connected to async-messaged'
+        task.disconnect()
 
         client_mock.close.assert_not_called()
 
         # connected
         task._client = client_mock
         task.worker_id = 'foo-bar-baz-foo'
 
         task.disconnect()
 
-        async_message_request_mock.assert_called_once_with(task.parent, client_mock, {
+        async_message_request_mock.assert_called_once_with(client_mock, {
             'worker': 'foo-bar-baz-foo',
+            'client': id(task.parent.user),
             'action': 'DISCONNECT',
             'context': task.context,
         })
         client_mock.setsockopt.assert_called_once_with(ZMQ_LINGER, 0)
         client_mock.close.assert_called_once_with()
 
         assert getattr(task, 'worker_id', True) is None
@@ -260,42 +299,47 @@
 
         with caplog.at_level(logging.INFO):
             task.subscribe()
 
         assert caplog.messages == ['foobar!']
         async_message_request_mock.assert_called_once_with(client_mock, {
             'worker': 'foo-bar-baz',
+            'client': id(scenario.user),
             'action': 'SUBSCRIBE',
             'context': expected_context,
             'payload': '1=2'
         })
 
     def test_unsubscribe(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture, caplog: LogCaptureFixture) -> None:
+        _, _, scenario = grizzly_fixture()
+        assert scenario is not None
+
         client_mock = mocker.MagicMock()
 
-        async_message_request_mock = mocker.patch('grizzly.tasks.clients.servicebus.async_message_request_wrapper', return_value={'message': 'hello world!'})
+        async_message_request_mock = mocker.patch('grizzly.utils.async_message_request', return_value={'message': 'hello world!'})
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
 
-        task._parent = mocker.MagicMock()
+        task._parent = scenario
 
         task._client = client_mock
         task.worker_id = 'foo-bar-baz'
 
         with caplog.at_level(logging.INFO):
             task.unsubscribe()
 
         assert caplog.messages == ['hello world!']
 
-        async_message_request_mock.assert_called_once_with(task.parent, client_mock, {
+        async_message_request_mock.assert_called_once_with(client_mock, {
             'worker': 'foo-bar-baz',
+            'client': id(task.parent.user),
             'action': 'UNSUBSCRIBE',
             'context': task.context,
         })
 
     def test_on_start(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
 
@@ -313,25 +357,27 @@
         # no text
         assert task._text is None
 
         task.on_start(scenario)
 
         connect_mock.assert_called_once_with()
         subscribe_mock.assert_not_called()
+        assert task.context.get('endpoint', None) == 'topic:my-topic, subscription:my-subscription'
 
         connect_mock.reset_mock()
         subscribe_mock.reset_mock()
 
         # text
         task._text = '1=1'
 
         task.on_start(scenario)
 
         connect_mock.assert_called_once_with()
         subscribe_mock.assert_called_once_with()
+        assert task.context.get('endpoint', None) == f'topic:my-topic, subscription:my-subscription_{id(scenario)}'
 
     def test_on_stop(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
 
         assert scenario is not None
 
         task = ServiceBusClientTask(
@@ -359,41 +405,47 @@
 
         task.on_stop(scenario)
 
         disconnect_mock.assert_called_once_with()
         unsubscribe_mock.assert_called_once_with()
 
     def test_request(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
+        _, _, scenario = grizzly_fixture()
+
+        assert scenario is not None
+
         client_mock = mocker.MagicMock()
 
-        async_message_request_mock = mocker.patch('grizzly.tasks.clients.servicebus.async_message_request_wrapper', return_value={'message': 'foobar!'})
+        async_message_request_mock = mocker.patch('grizzly.utils.async_message_request', return_value={'message': 'foobar!'})
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
-        task._parent = mocker.MagicMock()
         task._client = client_mock
+        task._parent = scenario
 
-        parent_mock = mocker.MagicMock()
         action_mock = mocker.MagicMock()
         meta_mock: Dict[str, Any] = {}
         action_mock.__enter__.return_value = meta_mock
         context_mock = mocker.patch.object(task, 'action', return_value=action_mock)
 
         # got response, empty payload
         request: AsyncMessageRequest = {
             'context': task.context,
         }
 
-        assert task.request(parent_mock, request) == {'message': 'foobar!'}
+        assert task.request(task.parent, request) == {'message': 'foobar!'}
+
+        context_mock.assert_called_once_with(task.parent)
+        request.update({'client': id(task.parent.user)})
+        async_message_request_mock.assert_called_once_with(client_mock, request)
+        del request['client']
 
-        context_mock.assert_called_once_with(parent_mock)
-        async_message_request_mock.assert_called_once_with(parent_mock, client_mock, request)
         assert meta_mock == {
             'action': 'topic:my-topic, subscription:my-subscription',
             'request': request,
             'response_length': 0,
             'response': {'message': 'foobar!'}
         }
 
@@ -401,141 +453,187 @@
         async_message_request_mock.reset_mock()
         meta_mock.clear()
 
         # got response, some payload
         del request['context']['url']
         async_message_request_mock = mocker.patch('grizzly.tasks.clients.servicebus.async_message_request_wrapper', return_value={'message': 'foobar!', 'payload': '1234567890'})
 
-        assert task.request(parent_mock, request) == {'message': 'foobar!', 'payload': '1234567890'}
+        assert task.request(task.parent, request) == {'message': 'foobar!', 'payload': '1234567890'}
 
-        context_mock.assert_called_once_with(parent_mock)
-        async_message_request_mock.assert_called_once_with(parent_mock, client_mock, request)
+        context_mock.assert_called_once_with(task.parent)
+        async_message_request_mock.assert_called_once_with(task.parent, client_mock, request)
         assert meta_mock == {
             'action': 'topic:my-topic, subscription:my-subscription',
             'request': request,
             'response_length': 10,
             'response': {'message': 'foobar!', 'payload': '1234567890'}
         }
 
     def test_get(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
+        _, _, scenario = grizzly_fixture()
+
+        assert scenario is not None
+
         client_mock = mocker.MagicMock()
-        parent_mock = mocker.MagicMock()
-        parent_mock.user._context = {'variables': {}}
+        scenario.user._context = {'variables': {}}
 
         task = ServiceBusClientTask(
             RequestDirection.FROM,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic/subscription:my-subscription;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
         )
         task._client = client_mock
+        task._parent = scenario
         task.worker_id = 'foo-bar'
 
         request_mock = mocker.patch.object(task, 'request', return_value={'metadata': None, 'payload': 'foobar'})
 
-        # no variable
-        task.variable = None
+        # no variables
+        task.payload_variable = None
 
-        assert task.get(parent_mock) == (None, 'foobar',)
+        assert task.get(task.parent) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(parent_mock, {
+        request_mock.assert_called_once_with(task.parent, {
             'action': 'RECEIVE',
             'worker': 'foo-bar',
             'context': task.context,
             'payload': None,
         })
 
-        assert parent_mock.user._context['variables'] == {}
+        assert task.parent.user._context['variables'] == {}
 
         request_mock.reset_mock()
 
-        # with variable
-        task.variable = 'foobaz'
+        # with payload variable
+        task.payload_variable = 'foobaz'
 
-        assert task.get(parent_mock) == (None, 'foobar',)
+        assert task.get(task.parent) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(parent_mock, {
+        request_mock.assert_called_once_with(task.parent, {
             'action': 'RECEIVE',
             'worker': 'foo-bar',
             'context': task.context,
             'payload': None,
         })
 
-        assert parent_mock.user._context['variables'] == {'foobaz': 'foobar'}
+        assert task.parent.user._context['variables'] == {'foobaz': 'foobar'}
+
+        # with payload and metadata variable
+        task.payload_variable = 'foobaz'
+        task.metadata_variable = 'bazfoo'
+        request_mock = mocker.patch.object(task, 'request', return_value={'metadata': {'x-foo-bar': 'hello'}, 'payload': 'foobar'})
+
+        assert task.get(task.parent) == ({'x-foo-bar': 'hello'}, 'foobar',)
+
+        request_mock.assert_called_once_with(task.parent, {
+            'action': 'RECEIVE',
+            'worker': 'foo-bar',
+            'context': task.context,
+            'payload': None,
+        })
+
+        assert task.parent.user._context['variables'] == {'foobaz': 'foobar', 'bazfoo': jsondumps({'x-foo-bar': 'hello'})}
 
     def test_put(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         _, _, scenario = grizzly_fixture()
         assert scenario is not None
 
         client_mock = mocker.MagicMock()
-        parent_mock = mocker.MagicMock()
         scenario.user._context = {'variables': {}}
-        parent_mock.render = scenario.render
 
         task = ServiceBusClientTask(
             RequestDirection.TO,
             'sb://my-sbns.servicebus.windows.net/topic:my-topic;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
             'test',
             source='hello world',
         )
         task._client = client_mock
+        task._parent = scenario
         task.worker_id = 'foo-baz'
 
         request_mock = mocker.patch.object(task, 'request', return_value={'metadata': None, 'payload': 'foobar'})
 
         # inline source, no file
-        assert task.put(parent_mock) == (None, 'foobar',)
+        assert task.put(task.parent) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(parent_mock, {
+        request_mock.assert_called_once_with(task.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
             'context': task.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
 
         # inline source, template
         task.source = '{{ foobar }}'
         scenario.user._context['variables'].update({'foobar': 'hello world'})
 
-        assert task.put(parent_mock) == (None, 'foobar',)
+        assert task.put(task.parent) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(parent_mock, {
+        request_mock.assert_called_once_with(task.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
             'context': task.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
         del scenario.user._context['variables']['foobar']
 
         # source file
         (grizzly_fixture.test_context / 'source.json').write_text('hello world')
         task.source = 'source.json'
 
-        assert task.put(parent_mock) == (None, 'foobar',)
+        assert task.put(task.parent) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(parent_mock, {
+        request_mock.assert_called_once_with(task.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
             'context': task.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
 
         # source file, with template
         scenario.user._context['variables'].update({'foobar': 'hello world', 'filename': 'source.j2.json'})
         (grizzly_fixture.test_context / 'source.j2.json').write_text('{{ foobar }}')
         task.source = '{{ filename }}'
 
-        assert task.put(parent_mock) == (None, 'foobar',)
+        assert task.put(task.parent) == (None, 'foobar',)
 
-        request_mock.assert_called_once_with(parent_mock, {
+        request_mock.assert_called_once_with(task.parent, {
             'action': 'SEND',
             'worker': 'foo-baz',
             'context': task.context,
             'payload': 'hello world',
         })
 
         request_mock.reset_mock()
+
+    def test_parent(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
+        _, _, scenario = grizzly_fixture()
+        assert scenario is not None
+
+        client_mock = mocker.MagicMock()
+
+        task = ServiceBusClientTask(
+            RequestDirection.TO,
+            'sb://my-sbns.servicebus.windows.net/topic:my-topic;SharedAccessKeyName=AccessKey;SharedAccessKey=37aabb777f454324=',
+            'test',
+            source='hello world',
+        )
+
+        task._client = client_mock
+
+        with pytest.raises(AttributeError) as ae:
+            _ = task.parent
+        assert str(ae.value) == 'no parent set'
+
+        task.parent = mocker.MagicMock()
+
+        _ = task.parent
+
+        with pytest.raises(AttributeError) as ae:
+            task.parent = scenario
+        assert str(ae.value) == 'parent already set, why are a different parent being set?'
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test___init__.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_async_group.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_async_group.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_conditional.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_conditional.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any, cast
 
 import pytest
 
 from pytest_mock import MockerFixture
-from _pytest.logging import LogCaptureFixture
 from grizzly.tasks import ConditionalTask, grizzlytask
 from grizzly.scenarios import GrizzlyScenario
 from grizzly.context import GrizzlyContextScenario
 from grizzly.exceptions import RestartScenario, StopUser
 
 from tests.fixtures import GrizzlyFixture
 from tests.helpers import TestTask
@@ -18,14 +17,18 @@
         task_factory = ConditionalTask(name='test', condition='{{ value | int > 0 }}')
 
         assert task_factory.tasks == {}
         assert task_factory.name == 'test'
         assert task_factory.condition == '{{ value | int > 0 }}'
         assert task_factory._pointer is None
         assert task_factory.__template_attributes__ == {'condition', 'tasks', 'name'}
+        assert task_factory.get_templates() == ['{{ value | int > 0 }}']
+
+        task_factory = ConditionalTask(name='test', condition='{{ value == "True" }}')
+        assert task_factory.get_templates() == ['{{ value == "True" }}']
 
     def test_switch(self) -> None:
         task_factory = ConditionalTask(name='test', condition='{{ value | int > 0 }}')
 
         assert task_factory._pointer is None
 
         task_factory.switch(True)
@@ -33,15 +36,15 @@
 
         task_factory.switch(False)
         assert not getattr(task_factory, '_pointer', True)
 
         task_factory.switch(None)
         assert task_factory._pointer is None
 
-    def test_add(self) -> None:
+    def test_add_and_peek(self) -> None:
         task_factory = ConditionalTask(name='test', condition='{{ value | int > 0 }}')
 
         # do not add task
         assert task_factory._pointer is None
         assert task_factory.tasks == {}
 
         test_task = TestTask()
@@ -56,22 +59,33 @@
 
         # add as False task
         task_factory.switch(False)
         for _ in range(0, 4):
             task_factory.add(test_task)
         assert task_factory.tasks == {True: [test_task] * 3, False: [test_task] * 4}
 
+        # peek at tasks
+        task_factory.switch(True)
+        assert len(task_factory.peek()) == 3
+
+        task_factory.switch(False)
+        assert len(task_factory.peek()) == 4
+
+        task_factory._pointer = None
+        assert len(task_factory.peek()) == 0
+
         # task has name attribute, prefix it
+        task_factory.switch(False)
         task_factory.add(TestTask(name='dummy task'))
         test_task = cast(TestTask, task_factory.tasks.get(False, [])[-1])
         assert test_task.name == 'test:dummy task'
         test_task = cast(TestTask, task_factory.tasks.get(False, [])[-2])
         assert test_task.name is None
 
-    def test___call__(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture, caplog: LogCaptureFixture) -> None:
+    def test___call__(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
         # pre: get context
         _, _, scenario = grizzly_fixture()
 
         class TestRestartScenarioTask(TestTask):
             def __call__(self) -> grizzlytask:
                 @grizzlytask
                 def task(parent: 'GrizzlyScenario') -> Any:
@@ -229,7 +243,64 @@
         # true condition
         task_factory.condition = '{{ value | int > 0 }}'
         scenario.user._context.update({'variables': {'value': 1}})
 
         task(scenario)
 
         assert len(scenario._user.environment.stats.serialize_errors().keys()) == 1
+
+    def test_on_event(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
+        _, _, scenario = grizzly_fixture()
+
+        assert scenario is not None
+
+        scenario_context = GrizzlyContextScenario(1)
+        scenario_context.name = scenario_context.description = 'test scenario'
+        task_factory = ConditionalTask(name='test', condition='{{ value }}', scenario=scenario_context)
+
+        task_factory.switch(True)
+        for i in range(0, 3):
+            task_factory.add(TestTask(name=f'dummy-true-{i}', scenario=scenario_context))
+
+        task_factory.switch(False)
+        for i in range(0, 4):
+            task_factory.add(TestTask(name=f'dummy-false-{i}', scenario=scenario_context))
+
+        mocker.patch('grizzly.tasks.conditional.gsleep', autospec=True)
+
+        task = task_factory()
+
+        on_start_mock = mocker.patch.object(TestTask, 'on_start', return_value=None)
+        on_stop_mock = mocker.patch.object(TestTask, 'on_stop', return_value=None)
+
+        task.on_start(scenario)
+
+        on_start_mock.call_count == 7
+        on_stop_mock.call_count == 0
+
+        task.on_stop(scenario)
+
+        on_start_mock.call_count == 7
+        on_stop_mock.call_count == 7
+
+        on_start_mock.reset_mock()
+        on_stop_mock.reset_mock()
+
+        task_factory = ConditionalTask(name='test', condition='{{ value }}', scenario=scenario_context)
+
+        task_factory.switch(True)
+        for i in range(0, 3):
+            task_factory.add(TestTask(name=f'dummy-true-{i}', scenario=scenario_context))
+
+        assert task_factory.tasks.get(False, None) is None
+
+        task = task_factory()
+
+        task.on_start(scenario)
+
+        on_start_mock.call_count == 3
+        on_stop_mock.call_count == 0
+
+        task.on_stop(scenario)
+
+        on_start_mock.call_count == 3
+        on_stop_mock.call_count == 3
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_date.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_log_message.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_log_message.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_loop.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_loop.py`

 * *Files 13% similar despite different names*

```diff
@@ -241,7 +241,39 @@
         assert kwargs.get('name', None) == '003 test (2)'
         assert kwargs.get('response_time', None) >= 0
         assert kwargs.get('response_length', None) == 2
         assert kwargs.get('context', None) == {'variables': {'foobar': 'world'}}
         exception = kwargs.get('exception', '')
         assert isinstance(exception, ValueError)
         assert str(exception) == 'error'
+
+    def test_on_event(self, grizzly_fixture: GrizzlyFixture, mocker: MockerFixture) -> None:
+        mocker.patch('grizzly.tasks.loop.gsleep', autospec=True)
+        _, _, scenario = grizzly_fixture()
+
+        assert scenario is not None
+
+        grizzly = grizzly_fixture.grizzly
+
+        scenario_context = GrizzlyContextScenario(3)
+        scenario_context.name = scenario_context.description = 'test scenario'
+
+        grizzly.state.variables['foobar'] = scenario.user._context['variables']['foobar'] = 'none'
+
+        task_factory = LoopTask(grizzly, 'test', '[1, 2, 3, 4]', 'foobar', scenario_context)
+        task_factory.add(TestTask(name='test-1'))
+        task_factory.add(TestTask(name='test-2'))
+
+        on_start_mock = mocker.patch.object(TestTask, 'on_start', return_value=None)
+        on_stop_mock = mocker.patch.object(TestTask, 'on_stop', return_value=None)
+
+        task = task_factory()
+
+        task.on_start(scenario)
+
+        assert on_start_mock.call_count == 2
+        assert on_stop_mock.call_count == 0
+
+        task.on_stop(scenario)
+
+        assert on_start_mock.call_count == 2
+        assert on_stop_mock.call_count == 2
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_request.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_request.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_set_variable.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_set_variable.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_task_wait.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_task_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_timer.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_timer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_transformer.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,29 @@
         assert scenario.user._context['variables']['test_variable'] == '''{"value": "hello world!"}
 {"value": "hello world!"}
 {"value": "hello world!"}'''
 
         task_factory = TransformerTask(
             grizzly,
             variable='test_variable',
+            expression='$.success',
+            content_type=TransformerContentType.JSON,
+            content=jsondumps({
+                'success': True,
+            }),
+            scenario=scenario_context,
+        )
+        task = task_factory()
+        task(scenario)
+
+        assert scenario.user._context['variables']['test_variable'] == 'True'
+
+        task_factory = TransformerTask(
+            grizzly,
+            variable='test_variable',
             expression='//actor[@id="9"]',
             content_type=TransformerContentType.XML,
             content='''<root xmlns:foo="http://www.foo.org/" xmlns:bar="http://www.bar.org">
   <actors>
     <actor id="7">Christian Bale</actor>
     <actor id="8">Liam Neeson</actor>
     <actor id="9">Michael Caine</actor>
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_until.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_until.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,112 +8,19 @@
 from _pytest.logging import LogCaptureFixture
 
 from grizzly.exceptions import RestartScenario
 from grizzly.types import RequestDirection, RequestMethod
 from grizzly.types.locust import StopUser
 from grizzly.tasks import GrizzlyMetaRequestTask, UntilRequestTask, RequestTask
 from grizzly.tasks.clients import HttpClientTask
-from grizzly.tasks.until import suppress, no_error_handler
 from grizzly_extras.transformer import TransformerContentType, TransformerError, transformer
 
 from tests.fixtures import GrizzlyFixture
 
 
-def test_no_error_handler(mocker: MockerFixture, grizzly_fixture: GrizzlyFixture, caplog: LogCaptureFixture) -> None:
-    grizzly_fixture()
-
-    env = grizzly_fixture.locust_env
-
-    assert len(env.events.request._handlers) == 1
-
-    handler = no_error_handler(env)
-
-    log_request_spy = mocker.spy(env.stats, 'log_request')
-    total_log_error_spy = mocker.spy(env.stats.total, 'log_error')
-    request_stats_spy = mocker.patch.object(env.stats, 'get', return_value=mocker.MagicMock())
-
-    with caplog.at_level(ERROR):
-        handler('TEST', 'test-event-1', 1337, 337, None)
-
-    assert len(caplog.messages) == 0
-    assert total_log_error_spy.call_count == 0
-    assert request_stats_spy.call_count == 1
-    assert request_stats_spy.return_value.log_error.call_count == 0
-    assert log_request_spy.call_count == 1
-
-    args, kwargs = log_request_spy.call_args_list[-1]
-    assert kwargs == {}
-    assert len(args) == 4
-    assert args[0] == 'TEST'
-    assert args[1] == 'test-event-1'
-    assert args[2] == 1337
-    assert args[3] == 337
-
-    args, kwargs = request_stats_spy.call_args_list[-1]
-    assert kwargs == {}
-    assert len(args) == 2
-    assert args[0] == 'test-event-1'
-    assert args[1] == 'TEST'
-
-    with caplog.at_level(ERROR):
-        handler('TEST', 'test-event-2', 1337, 337, RuntimeError('foo'))
-
-    assert len(caplog.messages) == 1
-    assert total_log_error_spy.call_count == 1
-    assert request_stats_spy.call_count == 3
-    assert request_stats_spy.return_value.log_error.call_count == 1
-    assert log_request_spy.call_count == 2
-
-    assert caplog.messages[0] == "TEST test-event-2: response_time=1337, response_length=337, exception=RuntimeError('foo')"
-
-    args, kwargs = total_log_error_spy.call_args_list[-1]
-    assert kwargs == {}
-    assert len(args) == 1
-    assert args[0] is None
-
-    args, kwargs = request_stats_spy.return_value.log_error.call_args_list[-1]
-    assert kwargs == {}
-    assert len(args) == 1
-    assert args[0] is None
-
-    args, kwargs = log_request_spy.call_args_list[-1]
-    assert kwargs == {}
-    assert len(args) == 4
-    assert args[0] == 'TEST'
-    assert args[1] == 'test-event-2'
-    assert args[2] == 1337
-    assert args[3] == 337
-
-
-def test_supress(grizzly_fixture: GrizzlyFixture) -> None:
-    grizzly_fixture()
-
-    env = grizzly_fixture.locust_env
-
-    original_handlers = env.events.request._handlers.copy()
-
-    assert len(env.events.request._handlers) == 1
-
-    with suppress(env):
-        assert env.events.request._handlers != original_handlers
-        assert len(env.events.request._handlers) == 1
-        assert env.events.request._handlers[0].__name__ == 'no_error_handler_wrapper'
-
-    assert env.events.request._handlers == original_handlers
-
-    with pytest.raises(RuntimeError):
-        with suppress(env):
-            assert env.events.request._handlers != original_handlers
-            assert len(env.events.request._handlers) == 1
-            assert env.events.request._handlers[0].__name__ == 'no_error_handler_wrapper'
-            raise RuntimeError()
-
-    assert env.events.request._handlers == original_handlers
-
-
 class TestUntilRequestTask:
     def test___init__(self, grizzly_fixture: GrizzlyFixture) -> None:
         grizzly_fixture()
         grizzly = grizzly_fixture.grizzly
 
         request = RequestTask(RequestMethod.GET, name='test', endpoint='/api/test')
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/tasks/test_wait.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/tasks/test_wait.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_behave.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_behave.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_clients.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_clients.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_context.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_context.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_locust.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_locust.py`

 * *Files 1% similar despite different names*

```diff
@@ -781,25 +781,28 @@
     # create stats
     stats = RequestStats()
 
     request_types_sequence = ['GET', 'GET', 'POST', 'PUT', 'UNTL', 'ASYNC']
     request_types_sequence_count = 5
     scenario_count = 10
 
-    for ident in range(1, scenario_count):
+    for ident in range(1, scenario_count + 1):
         for index, method in enumerate(request_types_sequence * request_types_sequence_count, 1):
             name = f'{ident:03} {index:02}-{method.lower()}-test'
 
             stats.log_request(
                 method,
                 name,
                 response_time=randint(200, 300),
                 content_length=(index * randint(10, 20)),
             )
 
+        stats.log_request('DOC', 'TPM report OUT', response_time=randint(200, 300), content_length=999)
+        stats.log_request('DOC', 'TPM report IN', response_time=randint(200, 300), content_length=999)
+
         for method in ['SCEN', 'TSTD', 'VAR', 'CLTSK']:
             stats.log_request(
                 method,
                 f'{ident:03} {method.lower()}-test',
                 response_time=randint(200, 300),
                 content_length=(2 * randint(10, 20)),
             )
@@ -827,14 +830,19 @@
     for ident in range(1, scenario_count):
         index = (ident - 1) * ((len(request_types_sequence) * request_types_sequence_count) + 4) + 2
         assert re.match(fr'^SCEN\s+{ident:03}', grizzly_stats[index].strip())
         assert re.match(fr'^TSTD\s+{ident:03}', grizzly_stats[index + 1].strip())
         assert re.match(fr'^GET\s+{ident:03} 01-get-test', grizzly_stats[index + 2].strip())
         assert re.match(fr'^VAR\s+{ident:03} var-test', grizzly_stats[index + (len(request_types_sequence) * request_types_sequence_count) + 3].strip())
 
+    last_stat_row = len(grizzly_stats) - 4
+
+    assert re.match(r'^DOC\s+TPM report OUT\s+10', grizzly_stats[last_stat_row].strip())
+    assert re.match(r'^DOC\s+TPM report IN\s+10', grizzly_stats[last_stat_row - 1].strip())
+
     for stat in grizzly_stats:
         assert stat in locust_stats
 
     # total = grizzly_time + locust_time
     # grizzly_ratio = (grizzly_time / total) * 100
     # locust_ratio = (locust_time / total) * 100
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_types.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_types.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/test_utils.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,33 +676,39 @@
         'context': {
             'endpoint': 'hello world'
         }
     }
 
     async_message_request_wrapper(scenario, client_mock, request)
 
+    request.update({'client': id(scenario.user)})
+
     async_message_request_mock.assert_called_once_with(client_mock, request)
     async_message_request_mock.reset_mock()
 
+    del request['client']
+
     # template to render, variable not set
     request = {
         'context': {
             'endpoint': 'hello {{ world }}!'
         }
     }
 
     async_message_request_wrapper(scenario, client_mock, request)
-    async_message_request_mock.assert_called_once_with(client_mock, {'context': {'endpoint': 'hello !'}})
+
+    async_message_request_mock.assert_called_once_with(client_mock, {'context': {'endpoint': 'hello !'}, 'client': id(scenario.user)})
     async_message_request_mock.reset_mock()
 
     # template to render, variable set
     scenario.user._context['variables'].update({'world': 'foobar'})
 
     async_message_request_wrapper(scenario, client_mock, request)
-    async_message_request_mock.assert_called_once_with(client_mock, {'context': {'endpoint': 'hello foobar!'}})
+
+    async_message_request_mock.assert_called_once_with(client_mock, {'context': {'endpoint': 'hello foobar!'}, 'client': id(scenario.user)})
 
 
 def test_safe_del() -> None:
     struct = {'hello': 'world', 'foo': 'bar'}
 
     safe_del(struct, 'bar')
     assert struct == {'hello': 'world', 'foo': 'bar'}
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test___init__.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test_ast.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,35 +17,36 @@
     source = jsonloads(request.source)
     source['result']['CsvRowValue1'] = '{{ AtomicCsvReader.test.header1 }}'
     source['result']['CsvRowValue2'] = '{{ AtomicCsvReader.test.header2 }}'
     source['result']['File'] = '{{ AtomicDirectoryContents.test }}'
     source['result']['TestSubString'] = '{{ a_sub_string[:3] }}'
     source['result']['TestString'] = '{{ a_string }}'
     source['result']['FooBar'] = '{{ (AtomicIntegerIncrementer.file_number | int) }}'
+    source['result']['Expression'] = '{{ expression == "True" }}'
 
     request.source = jsondumps(source)
     scenario = GrizzlyContextScenario(1)
     scenario.name = 'TestScenario'
     scenario.tasks.add(request)
 
     templates = {scenario: set(request.get_templates())}
-
     variables = _parse_templates(templates)
 
     assert variables == {
         'TestScenario_001': {
             'messageID',
             'AtomicIntegerIncrementer.messageID',
             'AtomicDate.now',
             'AtomicCsvReader.test.header1',
             'AtomicCsvReader.test.header2',
             'AtomicDirectoryContents.test',
             'a_sub_string',
             'a_string',
             'AtomicIntegerIncrementer.file_number',
+            'expression',
         },
     }
 
 
 def test__parse_template_nested_pipe(request_task: RequestTaskFixture) -> None:
     request = request_task.request
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test_communication.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_communication.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/test_utils.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/test_utils.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test___init__.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test___init__.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_date.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_date.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_directory_contents.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_integer_incrementer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_random_integer.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_integer.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/testdata/variables/test_random_string.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/testdata/variables/test_random_string.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_grizzly_user.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_grizzly_user.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_request_logger.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_request_logger.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_response_event.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_event.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/base/test_response_handler.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/base/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_blobstorage.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_blobstorage.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_dummy.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_dummy.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_iothub.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_iothub.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_messagequeue.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_messagequeue.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_restapi.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_restapi.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_servicebus.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_servicebus.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,14 @@
 
             assert async_action_spy.call_count == 1
             args, kwargs = async_action_spy.call_args_list[0]
 
             assert len(args) == 3
             assert len(kwargs) == 0
             assert args[1] == {
-                'worker': None,
                 'action': 'DISCONNECT',
                 'context': {
                     'endpoint': 'queue:test-queue',
                     'url': user.am_context['url'],
                     'message_wait': None,
                 }
             }
@@ -239,15 +238,14 @@
         assert async_action_spy.call_count == 1
         args, kwargs = async_action_spy.call_args_list[0]
 
         assert len(args) == 4
         assert len(kwargs) == 0
         assert args[1] is task
         assert args[2] == {
-            'worker': None,
             'action': 'HELLO',
             'context': {
                 'endpoint': 'topic:test-topic',
                 'url': user.am_context['url'],
                 'message_wait': None,
             }
         }
@@ -270,15 +268,14 @@
         assert async_action_spy.call_count == 2
         args, kwargs = async_action_spy.call_args_list[1]
 
         assert len(args) == 4
         assert len(kwargs) == 0
         assert args[1] is task
         assert args[2] == {
-            'worker': None,
             'action': 'HELLO',
             'context': {
                 'endpoint': 'topic:test-topic, subscription:test-subscription',
                 'url': user.am_context['url'],
                 'message_wait': None,
             }
         }
@@ -416,14 +413,15 @@
         exception = kwargs.get('exception', None)
         assert 'unknown error' in str(exception)
 
         args, kwargs = send_json_spy.call_args_list[0]
         assert kwargs == {}
         assert args == ({
             'worker': 'asdf-asdf-asdf',
+            'client': id(user),
             'action': 'SEND',
             'payload': 'hello',
             'context': {
                 'endpoint': 'queue:test-queue',
                 'connection': 'sender',
                 'content_type': 'undefined',
                 'url': 'sb://sb.example.org/;SharedAccessKeyName=RootManageSharedAccessKey;SharedAccessKey=abc123def456ghi789=',
@@ -470,14 +468,15 @@
         assert kwargs.get('context', None) == user._context
         assert kwargs.get('exception', '') is None
 
         args, kwargs = send_json_spy.call_args_list[1]
         assert kwargs == {}
         assert args == ({
             'worker': 'asdf-asdf-asdf',
+            'client': id(user),
             'action': 'RECEIVE',
             'payload': None,
             'context': {
                 'endpoint': 'queue:test-queue',
                 'connection': 'receiver',
                 'content_type': 'undefined',
                 'url': 'sb://sb.example.org/;SharedAccessKeyName=RootManageSharedAccessKey;SharedAccessKey=abc123def456ghi789=',
@@ -525,14 +524,15 @@
         assert kwargs.get('context', None) == user._context
         assert kwargs.get('exception', '') is None
 
         args, kwargs = send_json_spy.call_args_list[2]
         assert kwargs == {}
         assert args == ({
             'worker': 'asdf-asdf-asdf',
+            'client': id(user),
             'action': 'RECEIVE',
             'payload': None,
             'context': {
                 'endpoint': 'queue:test-queue, expression:"$.document[?(@.name=="TPM Report")]',
                 'connection': 'receiver',
                 'url': 'sb://sb.example.org/;SharedAccessKeyName=RootManageSharedAccessKey;SharedAccessKey=abc123def456ghi789=',
                 'message_wait': None,
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly/users/test_sftp.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly/users/test_sftp.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test___init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 import sys
 
-from typing import Any, List, Tuple, Dict, cast
+from typing import Any, List, Tuple, cast
 from os import environ
 
 import pytest
 
 from pytest_mock.plugin import MockerFixture
 
 from grizzly_extras.async_message import AsyncMessageRequest, AsyncMessageError
@@ -140,47 +140,43 @@
 
         request: AsyncMessageRequest = {
             'action': 'CONN',
         }
 
         with pytest.raises(AsyncMessageError) as mqe:
             handlers[request['action']](handler, request)
-        assert 'already connected' in str(mqe)
-
-        handler.qmgr = None
-
-        with pytest.raises(AsyncMessageError) as mqe:
-            handlers[request['action']](handler, request)
         assert 'no context' in str(mqe)
 
-        def mocked_connect(*args: Tuple[Any, ...], **kwargs: Dict[str, Any]) -> Any:
-            pass
-
-        mocker.patch.object(
-            pymqi.QueueManager,
-            'connect_with_options',
-            mocked_connect,
-        )
-
-        pymqi_sco_spy = mocker.spy(pymqi.SCO, '__init__')
-        pymqi_cd_spy = mocker.spy(pymqi.CD, '__init__')
-        pymqi_connect_with_options_spy = mocker.spy(pymqi.QueueManager, 'connect_with_options')
-
         request.update({
             'context': {
                 'url': 'mq://mq.example.com?QueueManager=QM1&Channel=SYS.CONN',
                 'username': 'bob',
                 'password': 'secret',
                 'channel': 'SYS.CONN',
                 'connection': 'mq.example.com(1414)',
                 'queue_manager': 'QM1',
             }
         })
 
         response = handlers[request['action']](handler, request)
+        assert response.get('message', None) == 're-used connection'
+
+        handler.qmgr = None
+
+        mocker.patch.object(
+            pymqi.QueueManager,
+            'connect_with_options',
+            autospec=True,
+        )
+
+        pymqi_sco_spy = mocker.spy(pymqi.SCO, '__init__')
+        pymqi_cd_spy = mocker.spy(pymqi.CD, '__init__')
+        pymqi_connect_with_options_spy = mocker.spy(pymqi.QueueManager, 'connect_with_options')
+
+        response = handlers[request['action']](handler, request)
 
         assert response['message'] == 'connected'
         assert handler.message_wait == 0
         assert handler.qmgr is not None
 
         assert pymqi_sco_spy.call_count == 1
         _, kwargs = pymqi_sco_spy.call_args_list[0]
@@ -200,15 +196,15 @@
 
         assert args[0] is handler.qmgr
         assert kwargs.get('user', b'').decode().strip() == 'bob'
         assert kwargs.get('password', b'').decode().strip() == 'secret'
 
         pymqi_sco_spy.reset_mock()
         pymqi_cd_spy.reset_mock()
-        pymqi_connect_with_options_spy.reset_mock()
+        pymqi_connect_with_options_spy.reset_mock()  # does not reset call count?!
         pymqi_cd_setitem_spy = mocker.spy(pymqi.CD, '__setitem__')
 
         request['context'].update({
             'key_file': '/test/key',
             'message_wait': 10,
         })
 
@@ -233,16 +229,16 @@
         assert kwargs.get('TransportType', None) == pymqi.CMQC.MQXPT_TCP
 
         assert pymqi_cd_setitem_spy.call_count == 1
         args, _ = pymqi_cd_setitem_spy.call_args_list[0]
         assert args[1] == 'SSLCipherSpec'
         assert args[2].decode().strip() == 'ECDHE_RSA_AES_256_GCM_SHA384'
 
-        assert pymqi_connect_with_options_spy.call_count == 1
-        args, kwargs = pymqi_connect_with_options_spy.call_args_list[0]
+        assert pymqi_connect_with_options_spy.call_count == 2
+        args, kwargs = pymqi_connect_with_options_spy.call_args_list[-1]
 
         assert args[0] is handler.qmgr
         assert kwargs.get('user', b'').decode().strip() == 'bob'
         assert kwargs.get('password', b'').decode().strip() == 'secret'
 
         pymqi_sco_spy.reset_mock()
         pymqi_cd_spy.reset_mock()
@@ -268,16 +264,16 @@
 
         assert pymqi_cd_spy.call_count == 1
         assert pymqi_cd_setitem_spy.call_count == 1
         args, _ = pymqi_cd_setitem_spy.call_args_list[0]
         assert args[1] == 'SSLCipherSpec'
         assert args[2].decode().strip() == 'rot13'
 
-        assert pymqi_connect_with_options_spy.call_count == 1
-        args, kwargs = pymqi_connect_with_options_spy.call_args_list[0]
+        assert pymqi_connect_with_options_spy.call_count == 3
+        args, kwargs = pymqi_connect_with_options_spy.call_args_list[-1]
 
         assert args[0] is handler.qmgr
         assert kwargs.get('user', b'').decode().strip() == 'bob'
         assert kwargs.get('password', b'').decode().strip() == 'secret'
 
     def test__create_gmo(self, mocker: MockerFixture) -> None:
         handler = AsyncMessageQueueHandler(worker='asdf-asdf-asdf')
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/mq/test_rfh2.py`

 * *Files identical despite different names*

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/test___init__.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test___init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from _pytest.capture import CaptureFixture
 
 from grizzly_extras.async_message import (
     AsyncMessageRequestHandler,
     AsyncMessageResponse,
     AsyncMessageRequest,
     AsyncMessageHandler,
+    AsyncMessageError,
     ThreadLogger,
     register,
     async_message_request,
 )
 
 from tests.helpers import onerror
 
@@ -191,15 +192,15 @@
     client_mock.recv_json.side_effect = [ZMQAgain, None]
 
     request: AsyncMessageRequest = {
         'worker': None,
         'action': 'HELLO',
     }
 
-    with pytest.raises(RuntimeError) as re:
+    with pytest.raises(AsyncMessageError) as re:
         async_message_request(client_mock, request)
     assert str(re.value) == 'no response'
 
     sleep_mock.assert_called_once_with(0.1)
     client_mock.send_json.assert_called_once_with(request)
 
     assert client_mock.recv_json.call_count == 2
@@ -211,15 +212,15 @@
     sleep_mock.reset_mock()
     client_mock.reset_mock()
 
     # unsuccessful response
     client_mock.recv_json.side_effect = None
     client_mock.recv_json.return_value = {'success': False, 'message': 'error! error! error!'}
 
-    with pytest.raises(RuntimeError) as re:
+    with pytest.raises(AsyncMessageError) as re:
         async_message_request(client_mock, request)
     assert str(re.value) == 'error! error! error!'
 
     sleep_mock.assert_not_called()
     client_mock.send_json.assert_called_once_with(request)
     client_mock.recv_json.assert_called_once_with(flags=ZMQ_NOBLOCK)
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/test_daemon.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @pytest.mark.parametrize('scheme,implementation', [
     ('mq', 'AsyncMessageQueueHandler',),
     ('sb', 'AsyncServiceBusHandler',),
 ])
 def test_worker(mocker: MockerFixture, capsys: CaptureFixture, scheme: str, implementation: str) -> None:
     context_mock = mocker.MagicMock()
     worker_mock = mocker.MagicMock()
-    worker_mock.send_multipart.return_value = StopAsyncIteration
+    worker_mock.send_multipart.side_effect = cycle([StopAsyncIteration])
 
     context_mock.socket.return_value = worker_mock
 
     def mock_recv_multipart(message: AsyncMessageRequest) -> None:
         def build_zmq_message(_message: AsyncMessageRequest) -> List[bytes]:
             worker = cast(str, _message.get('worker', ''))
             return [
@@ -45,43 +45,42 @@
                 b'',
                 jsondumps(_message).encode(),
             ]
 
         worker_mock.recv_multipart.side_effect = [
             zmq.Again,
             None,
-            build_zmq_message({'worker': 'ID-54321'}),
             build_zmq_message(message),
         ]
 
     def mock_handle_response(response: AsyncMessageResponse) -> None:
         mocker.patch(
             'grizzly_extras.async_message.AsyncMessageHandler.handle',
             side_effect=[response],
         )
 
-    mock_recv_multipart({'worker': 'ID-12345'})
+    mock_recv_multipart({'worker': 'ID-54321', 'context': {'url': f'{scheme}://dummy'}})
 
-    with pytest.raises(StopIteration):
+    with pytest.raises(StopAsyncIteration):
         worker(context_mock, 'ID-12345')
 
     assert worker_mock.send_multipart.call_count == 1
     args, _ = worker_mock.send_multipart.call_args_list[0]
     actual_response_proto = args[0]
-    assert actual_response_proto[0] == b'ID-12345'
+    assert actual_response_proto[0] == b'ID-54321'
     assert actual_response_proto[-1] == jsondumps({
         'worker': 'ID-12345',
         'response_time': 0,
         'success': False,
-        'message': 'no url found in request context',
+        'message': 'got ID-54321, expected ID-12345',
     }).encode()
 
     mock_recv_multipart({'worker': 'ID-12345', 'context': {'url': 'http://www.example.com'}})
 
-    with pytest.raises(StopIteration):
+    with pytest.raises(StopAsyncIteration):
         worker(context_mock, 'ID-12345')
 
     assert worker_mock.send_multipart.call_count == 2
     args, _ = worker_mock.send_multipart.call_args_list[1]
     actual_response_proto = args[0]
     assert actual_response_proto[0] == b'ID-12345'
     assert actual_response_proto[-1] == jsondumps({
@@ -103,15 +102,15 @@
         'payload': 'hello world',
         'metadata': {
             'some': 'metadata',
         },
         'response_time': 439,
     })
 
-    with pytest.raises(StopIteration):
+    with pytest.raises(StopAsyncIteration):
         worker(context_mock, 'ID-12345')
 
     assert integration_spy.call_count == 1
     args, _ = integration_spy.call_args_list[0]
     assert args[0] == 'ID-12345'
 
     assert worker_mock.send_multipart.call_count == 3
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/async_message/test_sb.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/async_message/test_sb.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         assert sender.close.call_count == 1
         assert receiver.close.call_count == 1
 
     def test_disconnect(self, mocker: MockerFixture) -> None:
         from grizzly_extras.async_message.sb import handlers
 
         handler = AsyncServiceBusHandler(worker='asdf-asdf-asdf')
+        handler._client = mocker.MagicMock()
         request: AsyncMessageRequest = {
             'action': 'DISCONNECT',
         }
 
         with pytest.raises(AsyncMessageError) as ame:
             handlers[request['action']](handler, request)
         assert 'no context in request' in str(ame)
@@ -370,90 +371,89 @@
         )
 
         queue_spy = mocker.spy(client, 'get_queue_sender')
         topic_spy = mocker.spy(client, 'get_topic_sender')
 
         handler = AsyncServiceBusHandler('asdf-asdf-asdf')
 
-        sender = handler.get_sender_instance(client, handler.get_endpoint_arguments('sender', 'queue:test-queue'))
+        handler._client = client
+
+        sender = handler.get_sender_instance(handler.get_endpoint_arguments('sender', 'queue:test-queue'))
         assert isinstance(sender, ServiceBusSender)
         assert topic_spy.call_count == 0
         assert queue_spy.call_count == 1
-        _, kwargs = queue_spy.call_args_list[0]
-        assert len(kwargs) == 1
-        assert kwargs.get('queue_name', None) == 'test-queue'
+        args, kwargs = queue_spy.call_args_list[0]
+        assert args == ()
+        assert kwargs == {'client_identifier': 'asdf-asdf-asdf', 'queue_name': 'test-queue'}
 
-        sender = handler.get_sender_instance(client, handler.get_endpoint_arguments('sender', 'topic:test-topic'))
+        sender = handler.get_sender_instance(handler.get_endpoint_arguments('sender', 'topic:test-topic'))
         assert isinstance(sender, ServiceBusSender)
         assert queue_spy.call_count == 1
         assert topic_spy.call_count == 1
-        _, kwargs = topic_spy.call_args_list[0]
-        assert len(kwargs) == 1
-        assert kwargs.get('topic_name', None) == 'test-topic'
+        args, kwargs = topic_spy.call_args_list[0]
+        assert args == ()
+        assert kwargs == {'client_identifier': 'asdf-asdf-asdf', 'topic_name': 'test-topic'}
 
     def test_get_receiver_instance(self, mocker: MockerFixture) -> None:
         url = 'Endpoint=sb://sb.example.org/;SharedAccessKeyName=RootManageSharedAccessKey;SharedAccessKey=abc123def456ghi789='
         client = ServiceBusClient.from_connection_string(
             conn_str=url,
             transport_type=TransportType.AmqpOverWebsocket,
         )
 
         queue_spy = mocker.spy(client, 'get_queue_receiver')
         topic_spy = mocker.spy(client, 'get_subscription_receiver')
 
         handler = AsyncServiceBusHandler('asdf-asdf-asdf')
+        handler._client = client
 
-        receiver = handler.get_receiver_instance(client, handler.get_endpoint_arguments('receiver', 'queue:test-queue'))
+        receiver = handler.get_receiver_instance(handler.get_endpoint_arguments('receiver', 'queue:test-queue'))
         assert isinstance(receiver, ServiceBusReceiver)
         assert topic_spy.call_count == 0
         assert queue_spy.call_count == 1
-        _, kwargs = queue_spy.call_args_list[-1]
-        assert len(kwargs) == 1
-        assert kwargs.get('queue_name', None) == 'test-queue'
+        args, kwargs = queue_spy.call_args_list[-1]
+        assert args == ()
+        assert kwargs == {'client_identifier': 'asdf-asdf-asdf', 'queue_name': 'test-queue'}
 
-        handler.get_receiver_instance(client, dict({'wait': '100'}, **handler.get_endpoint_arguments('receiver', 'queue:test-queue')))
+        handler.get_receiver_instance(dict({'wait': '100'}, **handler.get_endpoint_arguments('receiver', 'queue:test-queue')))
         assert topic_spy.call_count == 0
         assert queue_spy.call_count == 2
-        _, kwargs = queue_spy.call_args_list[-1]
-        assert len(kwargs) == 2
-        assert kwargs.get('queue_name', None) == 'test-queue'
-        assert kwargs.get('max_wait_time', None) == 100
+        args, kwargs = queue_spy.call_args_list[-1]
+        assert args == ()
+        assert kwargs == {'client_identifier': 'asdf-asdf-asdf', 'queue_name': 'test-queue', 'max_wait_time': 100}
 
-        receiver = handler.get_receiver_instance(client, handler.get_endpoint_arguments('receiver', 'topic:test-topic, subscription: test-subscription'))
+        receiver = handler.get_receiver_instance(handler.get_endpoint_arguments('receiver', 'topic:test-topic, subscription: test-subscription'))
         assert topic_spy.call_count == 1
         assert queue_spy.call_count == 2
-        _, kwargs = topic_spy.call_args_list[-1]
-        assert len(kwargs) == 2
-        assert kwargs.get('topic_name', None) == 'test-topic'
-        assert kwargs.get('subscription_name', None) == 'test-subscription'
+        args, kwargs = topic_spy.call_args_list[-1]
+        assert args == ()
+        assert kwargs == {'client_identifier': 'asdf-asdf-asdf', 'topic_name': 'test-topic', 'subscription_name': 'test-subscription'}
 
-        receiver = handler.get_receiver_instance(client, dict({'wait': '100'}, **handler.get_endpoint_arguments(
+        receiver = handler.get_receiver_instance(dict({'wait': '100'}, **handler.get_endpoint_arguments(
             'receiver', 'topic:test-topic, subscription:test-subscription, expression:$.foo.bar',
         )))
         assert topic_spy.call_count == 2
         assert queue_spy.call_count == 2
-        _, kwargs = topic_spy.call_args_list[-1]
-        assert len(kwargs) == 3
-        assert kwargs.get('topic_name', None) == 'test-topic'
-        assert kwargs.get('subscription_name', None) == 'test-subscription'
-        assert kwargs.get('max_wait_time', None) == 100
+        args, kwargs = topic_spy.call_args_list[-1]
+        assert args == ()
+        assert kwargs == {'client_identifier': 'asdf-asdf-asdf', 'topic_name': 'test-topic', 'subscription_name': 'test-subscription', 'max_wait_time': 100}
 
     def test_hello(self, mocker: MockerFixture) -> None:
         from grizzly_extras.async_message.sb import handlers
 
         handler = AsyncServiceBusHandler(worker='asdf-asdf-asdf')
         request: AsyncMessageRequest = {
             'action': 'HELLO',
         }
 
         with pytest.raises(AsyncMessageError) as ame:
             handlers[request['action']](handler, request)
         assert 'no context in request' in str(ame)
 
-        assert handler.client is None
+        assert handler._client is None
 
         servicebusclient_connect_spy = mocker.spy(ServiceBusClient, 'from_connection_string')
 
         request = {
             'action': 'HELLO',
             'context': {
                 'message_wait': 10,
@@ -485,18 +485,17 @@
             'message': 'there general kenobi',
         }
 
         assert sender_instance_spy.call_count == 1
         assert sender_instance_spy.return_value.__enter__.call_count == 1
         assert receiver_instance_spy.call_count == 0
 
-        args, _ = sender_instance_spy.call_args_list[0]
-        assert len(args) == 2
-        assert args[0] is handler.client
-        assert args[1] == {'endpoint_type': 'queue', 'endpoint': 'test-queue'}
+        args, kwargs = sender_instance_spy.call_args_list[0]
+        assert args == ({'endpoint_type': 'queue', 'endpoint': 'test-queue'},)
+        assert kwargs == {}
 
         assert handler._sender_cache.get('queue:test-queue', None) is not None
         assert handler._receiver_cache == {}
 
         # read from cache
         assert handlers[request['action']](handler, request) == {
             'message': 'there general kenobi',
@@ -516,18 +515,17 @@
         }
 
         assert sender_instance_spy.call_count == 1
         assert sender_instance_spy.return_value.__enter__.call_count == 1
         assert receiver_instance_spy.call_count == 1
         assert receiver_instance_spy.return_value.__enter__.call_count == 1
 
-        args, _ = receiver_instance_spy.call_args_list[0]
-        assert len(args) == 2
-        assert args[0] is handler.client
-        assert args[1] == {'endpoint_type': 'topic', 'endpoint': 'test-topic', 'subscription': 'test-subscription', 'wait': '10'}
+        args, kwargs = receiver_instance_spy.call_args_list[0]
+        assert kwargs == {}
+        assert args == ({'endpoint_type': 'topic', 'endpoint': 'test-topic', 'subscription': 'test-subscription', 'wait': '10'},)
 
         assert handler._sender_cache.get('queue:test-queue', None) is not None
         assert handler._receiver_cache.get('topic:test-topic, subscription:test-subscription', None) is not None
 
         # read from cache, not new instance needed
         assert handlers[request['action']](handler, request) == {
             'message': 'there general kenobi',
@@ -568,15 +566,15 @@
             else:
                 handler._receiver_cache[endpoint] = receiver_instance_mock.return_value
 
         with pytest.raises(AsyncMessageError) as ame:
             handlers[request['action']](handler, request)
         assert 'no context in request' in str(ame)
 
-        assert handler.client is None
+        assert handler._client is None
 
         # sender request
         request = {
             'action': 'SEND',
             'context': {
                 'message_wait': 10,
                 'url': 'sb://sb.example.org/;SharedAccessKeyName=RootManageSharedAccessKey;SharedAccessKey=abc123def456ghi789=',
@@ -822,14 +820,43 @@
 
         assert receiver_instance_mock.return_value.__iter__.call_count == 1
         assert receiver_instance_mock.return_value.complete_message.call_count == 2
         assert receiver_instance_mock.return_value.abandon_message.call_count == 0
 
         assert response.get('payload', None) == jsondumps({'document': {'name': 'test', 'id': 13}})
 
+        message1 = ServiceBusMessage(jsondumps({
+            'name': 'bob',
+        }))
+
+        message2 = ServiceBusMessage(jsondumps({
+            'name': 'alice',
+        }))
+
+        message3 = ServiceBusMessage(jsondumps({
+            'name': 'mallory',
+        }))
+
+        receiver_instance_mock.return_value.__iter__.side_effect = [
+            iter([message1, message2, message3]),
+        ]
+        receiver_instance_mock.reset_mock()
+
+        request['context'].update({'endpoint': 'queue:test-queue, expression:$.name=="mallory"'})
+
+        setup_handler(handler, request)
+
+        response = handlers[request['action']](handler, request)
+
+        assert response.get('payload', None) == jsondumps({'name': 'mallory'})
+
+        assert receiver_instance_mock.return_value.__iter__.call_count == 1
+        assert receiver_instance_mock.return_value.complete_message.call_count == 3
+        assert receiver_instance_mock.return_value.abandon_message.call_count == 0
+
     def test_get_handler(self) -> None:
         handler = AsyncServiceBusHandler(worker='asdf-asdf-asdf')
 
         assert handler.get_handler('NONE') is None
         assert handler.get_handler('HELLO') is AsyncServiceBusHandler.hello
         assert handler.get_handler('RECEIVE') is AsyncServiceBusHandler.request
         assert handler.get_handler('SEND') is AsyncServiceBusHandler.request
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/test_arguments.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,20 @@
     arguments = parse_arguments(f'arg1{separator}testvalue1, arg2{separator}"test value 2"', separator)
 
     assert arguments == {
         'arg1': 'testvalue1',
         'arg2': 'test value 2',
     }
 
+    arguments = parse_arguments(f'arg1{separator}$.expression=="{{{{ value }}}}"', separator)
+
+    assert arguments == {
+        'arg1': '$.expression=="{{ value }}"',
+    }
+
     with pytest.raises(ValueError) as ve:
         parse_arguments(f'url{separator}http://www.example.com?query_string{separator}value', separator)
     assert 'incorrect format in arguments: ' in str(ve)
 
     with pytest.raises(ValueError) as ve:
         parse_arguments(f'url{separator}"http://www.example.com?query_string{separator}value', separator)
     assert 'incorrect format in arguments: ' in str(ve)
```

### Comparing `grizzly-loadtester-2.6.2/tests/unit/test_grizzly_extras/test_transformer.py` & `grizzly-loadtester-2.6.3/tests/unit/test_grizzly_extras/test_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,22 @@
         }
 
         get_values = JsonTransformer.parser('$.glossary.GlossDiv.GlossList.GlossEntry.Abbrev')
         actual = get_values(example)
         assert len(actual) == 1
         assert ['ISO 8879:1986'] == actual
 
+        get_values = JsonTransformer.parser('$.glossary.title=="example glossary"')
+        actual = get_values(example)
+        assert ['example glossary'] == actual
+
+        get_values = JsonTransformer.parser("$.glossary.title=='template glossary'")
+        actual = get_values(example)
+        assert [] == actual
+
         get_values = JsonTransformer.parser('$.*..title')
         actual = get_values(example)
         assert len(actual) == 2
         assert ['example glossary', 'S'] == actual
 
         get_values = JsonTransformer.parser('$.*..GlossSeeAlso')
         actual = get_values(example)
```

### Comparing `grizzly-loadtester-2.6.2/tests/webserver.py` & `grizzly-loadtester-2.6.3/tests/webserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 logger = logging.getLogger('webserver')
 
 
 app = Flask('webserver')
 
 # ugly hack to get correct path when webserver.py is injected for running distributed
 root_dir = (Path(__file__).parent / '..').resolve()
-project_name = 'example'
 
-if '.pytest_tmp' in __file__:
-    root_dir = (root_dir / '..' / '..').resolve()
-    project_name = 'test-example'
+if '/srv/grizzly' not in str(root_dir):
+    root_dir = root_dir / 'example' / 'features'
 
 
 @app.route('/api/v1/resources/dogs')
 def app_get_dog_fact() -> FlaskResponse:
     logger.debug('route /api/v1/resources/dogs called')
     _ = int(request.args.get('number', ''))
 
@@ -42,17 +40,16 @@
     _ = int(request.args.get('limit', ''))
 
     return jsonify(['meow meow meow'])
 
 
 @app.route('/books/<book>.json')
 def app_get_book(book: str) -> FlaskResponse:
-    logger.debug(f'/books/{book}.json called')
-    logger.debug(f'{root_dir=}, {project_name=}')
-    with open(f'{root_dir}/{project_name}/features/requests/books/books.csv', 'r') as fd:
+    logger.debug(f'/books/{book}.json called, {root_dir=}')
+    with open(f'{root_dir}/requests/books/books.csv', 'r') as fd:
         reader = csv.DictReader(fd)
         for row in reader:
             if row['book'] == book:
                 return jsonify({
                     'number_of_pages': row['pages'],
                     'isbn_10': [row['isbn_10']] * 2,
                     'authors': [
```

