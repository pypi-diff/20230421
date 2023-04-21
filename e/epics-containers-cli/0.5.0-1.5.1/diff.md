# Comparing `tmp/epics-containers-cli-0.5.0.tar.gz` & `tmp/epics-containers-cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epics-containers-cli-0.5.0.tar", last modified: Thu Apr  6 10:24:07 2023, max compression
+gzip compressed data, was "epics-containers-cli-1.5.1.tar", last modified: Fri Apr 21 13:39:45 2023, max compression
```

## Comparing `epics-containers-cli-0.5.0.tar` & `epics-containers-cli-1.5.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.897408 epics-containers-cli-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.889407 epics-containers-cli-0.5.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.889407 epics-containers-cli-0.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.885407 epics-containers-cli-0.5.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.889407 epics-containers-cli-0.5.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.889407 epics-containers-cli-0.5.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.889407 epics-containers-cli-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.889407 epics-containers-cli-0.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-06 10:24:07.897408 epics-containers-cli-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.893407 epics-containers-cli-0.5.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/docs/user/tutorials/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)    11156 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/get_helm.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 10:24:07.897408 epics-containers-cli-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.889407 epics-containers-cli-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.897408 epics-containers-cli-0.5.0/src/epics_containers_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 10:24:07.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/cmd_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/cmd_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/src/epics_containers_cli/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.897408 epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-06 10:24:07.000000 epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-06 10:24:07.000000 epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:24:07.000000 epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 10:24:07.000000 epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-06 10:24:07.000000 epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-06 10:24:07.000000 epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:24:07.897408 epics-containers-cli-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-06 10:23:59.000000 epics-containers-cli-0.5.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.856371 epics-containers-cli-1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.844371 epics-containers-cli-1.5.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-21 13:39:45.856371 epics-containers-cli-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/docs/user/tutorials/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11156 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/get_helm.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:39:45.856371 epics-containers-cli-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.848371 epics-containers-cli-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/src/epics_containers_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/src/epics_containers_cli/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 13:39:45.000000 epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:39:45.852371 epics-containers-cli-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-21 13:39:36.000000 epics-containers-cli-1.5.1/tests/test_cli.py
```

### Comparing `epics-containers-cli-0.5.0/.devcontainer/devcontainer.json` & `epics-containers-cli-1.5.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/CONTRIBUTING.rst` & `epics-containers-cli-1.5.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/actions/install_requirements/action.yml` & `epics-containers-cli-1.5.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/dependabot.yml` & `epics-containers-cli-1.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/pages/make_switcher.py` & `epics-containers-cli-1.5.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/workflows/code.yml` & `epics-containers-cli-1.5.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/workflows/docs.yml` & `epics-containers-cli-1.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/workflows/docs_clean.yml` & `epics-containers-cli-1.5.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.github/workflows/linkcheck.yml` & `epics-containers-cli-1.5.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.gitignore` & `epics-containers-cli-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/.vscode/launch.json` & `epics-containers-cli-1.5.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/Dockerfile` & `epics-containers-cli-1.5.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/LICENSE` & `epics-containers-cli-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/PKG-INFO` & `epics-containers-cli-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epics-containers-cli
-Version: 0.5.0
+Version: 1.5.1
 Summary: One line description of your module
 Author-email: Giles Knap <giles.knap@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `epics-containers-cli-0.5.0/README.rst` & `epics-containers-cli-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/conf.py` & `epics-containers-cli-1.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `epics-containers-cli-1.5.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/explanations/decisions.rst` & `epics-containers-cli-1.5.1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/how-to/build-docs.rst` & `epics-containers-cli-1.5.1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/how-to/lint.rst` & `epics-containers-cli-1.5.1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/how-to/make-release.rst` & `epics-containers-cli-1.5.1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/how-to/pin-requirements.rst` & `epics-containers-cli-1.5.1/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/how-to/test-container.rst` & `epics-containers-cli-1.5.1/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/how-to/update-tools.rst` & `epics-containers-cli-1.5.1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/index.rst` & `epics-containers-cli-1.5.1/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/reference/standards.rst` & `epics-containers-cli-1.5.1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/developer/tutorials/dev-install.rst` & `epics-containers-cli-1.5.1/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/images/dls-favicon.ico` & `epics-containers-cli-1.5.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/images/dls-logo.svg` & `epics-containers-cli-1.5.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/index.rst` & `epics-containers-cli-1.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/user/explanations/docs-structure.rst` & `epics-containers-cli-1.5.1/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/user/index.rst` & `epics-containers-cli-1.5.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/docs/user/tutorials/installation.rst` & `epics-containers-cli-1.5.1/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/get_helm.sh` & `epics-containers-cli-1.5.1/get_helm.sh`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/pyproject.toml` & `epics-containers-cli-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli/__main__.py` & `epics-containers-cli-1.5.1/src/epics_containers_cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,25 @@
 ):
     """List the IOCs running in the current domain"""
 
     bl = ctx.obj.domain
 
     if all:
         run_command(
-            f"kubectl -n {bl} get deploy -l is_ioc==True -o {fmt_deploys}", show=True
+            f"kubectl -n {bl} get deploy -l is_ioc==True -o {fmt_deploys}",
+            show=True,
+            interactive=True,
         )
     else:
         format = fmt_pods_wide if wide else fmt_pods
-        run_command(f"kubectl -n {bl} get pod -l is_ioc==True -o {format}", show=True)
+        run_command(
+            f"kubectl -n {bl} get pod -l is_ioc==True -o {format}",
+            show=True,
+            interactive=True,
+        )
 
 
 @cli.command()
 def resources(ctx: typer.Context):
     """Output information about a domain's cluster resources"""
 
     bl = ctx.obj.domain
```

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli/cmd_dev.py` & `epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         # the rsync command refreshes repos but does not overwrite local changes
         f"--entrypoint rsync {image} " f"-au /repos/ /copy",
         interactive=True,
         show_cmd=True,
     )
 
     # overwrite repos/epics/ioc folder with any local changes
+    # TODO would this not be better as a mount point?
     run_command(f"rsync -au {folder}/ioc {repos}/epics/", show_cmd=True)
 
     return image
 
 
 @dev.command()
 def launch(
```

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli/cmd_ioc.py` & `epics-containers-cli-1.5.1/src/epics_containers_cli/cmd_ioc.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,14 +239,15 @@
     check_domain(bl)
     check_ioc(ioc_name, bl)
 
     pod_name = run_command(f"kubectl get -n {bl} pod -l app={ioc_name} -o name")
     run_command(
         f"kubectl delete -n {bl} {pod_name}",
         show=True,
+        interactive=True,
         show_cmd=c.show_cmd,
     )
 
 
 @ioc.command()
 def start(
     ctx: typer.Context,
@@ -258,14 +259,15 @@
     bl = c.domain
     check_domain(bl)
     check_ioc(ioc_name, bl)
 
     run_command(
         f"kubectl scale -n {bl} deploy --replicas=1 {ioc_name}",
         show=True,
+        interactive=True,
         show_cmd=c.show_cmd,
     )
 
 
 @ioc.command()
 def stop(
     ctx: typer.Context,
@@ -277,14 +279,15 @@
     bl = c.domain
     check_domain(bl)
     check_ioc(ioc_name, bl)
 
     run_command(
         f"kubectl scale -n {bl} deploy --replicas=0 {ioc_name}",
         show=True,
+        interactive=True,
         show_cmd=c.show_cmd,
     )
 
 
 @ioc.command()
 def versions(
     ctx: typer.Context,
@@ -293,9 +296,10 @@
     """List all versions of the IOC available in the helm registry"""
     c: Context = ctx.obj
 
     run_command(
         f"podman run --rm quay.io/skopeo/stable "
         f"list-tags docker://{c.helm_registry}/{ioc_name}",
         show=True,
+        interactive=True,
         show_cmd=c.show_cmd,
     )
```

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli/kubectl.py` & `epics-containers-cli-1.5.1/src/epics_containers_cli/kubectl.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli/logging.py` & `epics-containers-cli-1.5.1/src/epics_containers_cli/logging.py`

 * *Files identical despite different names*

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli/shell.py` & `epics-containers-cli-1.5.1/src/epics_containers_cli/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,32 +40,24 @@
 
 ERROR = """
 [bold red]Command failed: [/bold red][gray37]{0}[/gray37]
 {1}"""
 
 
 def run_command(
-    command: str,
-    error_OK=False,
-    show=False,
-    show_cmd=False,
-    interactive=False,
-    shell=True,
+    command: str, error_OK=False, show=False, show_cmd=False, interactive=False
 ) -> Optional[str]:
     """Run a command and return the output"""
 
     if show_cmd:
         print(f"[gray37]{command}[/gray37]")
 
-    if not shell:
-        commands = command.split()
-    else:
-        commands = [command]
+    commands = [command]
 
-    result = subprocess.run(commands, capture_output=not interactive, shell=shell)
+    result = subprocess.run(commands, capture_output=not interactive, shell=True)
 
     if interactive:
         if result.returncode != 0 and not error_OK:
             raise typer.Exit(1)
         return None
     else:
         if result.returncode == 0:
@@ -129,15 +121,15 @@
 
     return registry
 
 
 def get_image_name(
     repo: str, arch: Architecture = Architecture.linux, target: str = "developer"
 ) -> str:
-    registry = repo2registry(repo)
+    registry = repo2registry(repo).lower()
     image = f"{registry}-{arch}-{target}"
     log.info("repo = %s image  = %s", repo, image)
     return image
 
 
 def get_git_name(folder: Path = Path("."), full: bool = False) -> str:
     if not folder.joinpath(".git").exists():
```

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/PKG-INFO` & `epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epics-containers-cli
-Version: 0.5.0
+Version: 1.5.1
 Summary: One line description of your module
 Author-email: Giles Knap <giles.knap@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `epics-containers-cli-0.5.0/src/epics_containers_cli.egg-info/SOURCES.txt` & `epics-containers-cli-1.5.1/src/epics_containers_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

