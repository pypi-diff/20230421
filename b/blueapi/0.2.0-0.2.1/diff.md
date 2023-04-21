# Comparing `tmp/blueapi-0.2.0.tar.gz` & `tmp/blueapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.2.0.tar", last modified: Thu Apr 20 10:06:04 2023, max compression
+gzip compressed data, was "blueapi-0.2.1.tar", last modified: Fri Apr 21 14:15:23 2023, max compression
```

## Comparing `blueapi-0.2.0.tar` & `blueapi-0.2.1.tar`

### file list

```diff
@@ -1,171 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.510317 blueapi-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-20 10:05:49.000000 blueapi-0.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-20 10:05:49.000000 blueapi-0.2.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.474317 blueapi-0.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 10:05:49.000000 blueapi-0.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-20 10:05:49.000000 blueapi-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-20 10:05:49.000000 blueapi-0.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-20 10:05:49.000000 blueapi-0.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 10:05:49.000000 blueapi-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-20 10:06:04.510317 blueapi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-20 10:05:49.000000 blueapi-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-20 10:05:49.000000 blueapi-0.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/config/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 10:05:49.000000 blueapi-0.2.0/config/adsim.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-20 10:05:49.000000 blueapi-0.2.0/config/bl45p.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.482318 blueapi-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.486317 blueapi-0.2.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.486317 blueapi-0.2.0/docs/developer/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.486317 blueapi-0.2.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/explanations/type_validators.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   236122 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/images/blueapi-architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-20 10:05:49.000000 blueapi-0.2.0/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.478318 blueapi-0.2.0/helm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.494317 blueapi-0.2.0/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-20 10:05:49.000000 blueapi-0.2.0/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-20 10:05:49.000000 blueapi-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:06:04.510317 blueapi-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.478318 blueapi-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/amq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/plans/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/plans/plans.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/plans/stubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/service/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/service/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.502318 blueapi-0.2.0/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/adsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/bl45p.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/thread_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/utils/type_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-20 10:05:49.000000 blueapi-0.2.0/src/blueapi/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.498318 blueapi-0.2.0/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 10:06:04.000000 blueapi-0.2.0/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/core/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/messaging/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.506317 blueapi-0.2.0/tests/plans/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/plans/test_scanspec_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:06:04.510317 blueapi-0.2.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_thread_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-20 10:05:49.000000 blueapi-0.2.0/tests/utils/test_type_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.076542 blueapi-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 14:15:11.000000 blueapi-0.2.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-21 14:15:11.000000 blueapi-0.2.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.060541 blueapi-0.2.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-21 14:15:11.000000 blueapi-0.2.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-21 14:15:11.000000 blueapi-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-21 14:15:11.000000 blueapi-0.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 14:15:11.000000 blueapi-0.2.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-21 14:15:11.000000 blueapi-0.2.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-21 14:15:11.000000 blueapi-0.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-21 14:15:11.000000 blueapi-0.2.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 14:15:11.000000 blueapi-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-21 14:15:23.076542 blueapi-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-21 14:15:11.000000 blueapi-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-21 14:15:11.000000 blueapi-0.2.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 14:15:11.000000 blueapi-0.2.1/config/adsim.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 14:15:11.000000 blueapi-0.2.1/config/bl45p.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/docs/developer/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/explanations/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/explanations/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/explanations/type_validators.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.064541 blueapi-0.2.1/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   236122 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-21 14:15:11.000000 blueapi-0.2.1/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.060541 blueapi-0.2.1/helm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 14:15:11.000000 blueapi-0.2.1/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-21 14:15:11.000000 blueapi-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:15:23.076542 blueapi-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.060541 blueapi-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 14:15:22.000000 blueapi-0.2.1/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/cli/amq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/src/blueapi/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/plans/plans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/plans/stubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/service/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/service/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/startup/adsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/startup/bl45p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/startup/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/utils/thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/utils/type_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-21 14:15:11.000000 blueapi-0.2.1/src/blueapi/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.068541 blueapi-0.2.1/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-04-21 14:15:23.000000 blueapi-0.2.1/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-21 14:15:23.000000 blueapi-0.2.1/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:15:23.000000 blueapi-0.2.1/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 14:15:23.000000 blueapi-0.2.1/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-21 14:15:23.000000 blueapi-0.2.1/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 14:15:23.000000 blueapi-0.2.1/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.072542 blueapi-0.2.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.076542 blueapi-0.2.1/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.076542 blueapi-0.2.1/tests/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/plans/test_scanspec_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:23.076542 blueapi-0.2.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/test_thread_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15499 2023-04-21 14:15:11.000000 blueapi-0.2.1/tests/utils/test_type_validator.py
```

### Comparing `blueapi-0.2.0/.devcontainer/Dockerfile` & `blueapi-0.2.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.devcontainer/devcontainer.json` & `blueapi-0.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/CONTRIBUTING.rst` & `blueapi-0.2.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/actions/install_requirements/action.yml` & `blueapi-0.2.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/dependabot.yml` & `blueapi-0.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/pages/make_switcher.py` & `blueapi-0.2.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/workflows/code.yml` & `blueapi-0.2.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/workflows/docs.yml` & `blueapi-0.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/workflows/docs_clean.yml` & `blueapi-0.2.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/workflows/helm.yml` & `blueapi-0.2.1/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.github/workflows/linkcheck.yml` & `blueapi-0.2.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.gitignore` & `blueapi-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.pre-commit-config.yaml` & `blueapi-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.vscode/launch.json` & `blueapi-0.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/.vscode/settings.json` & `blueapi-0.2.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/LICENSE` & `blueapi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/PKG-INFO` & `blueapi-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.2.0/README.rst` & `blueapi-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/conf.py` & `blueapi-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/explanations/architecture.rst` & `blueapi-0.2.1/docs/developer/explanations/architecture.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/explanations/decisions.rst` & `blueapi-0.2.1/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/explanations/lifecycle.rst` & `blueapi-0.2.1/docs/developer/explanations/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/explanations/type_validators.rst` & `blueapi-0.2.1/docs/developer/explanations/type_validators.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/how-to/build-docs.rst` & `blueapi-0.2.1/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/how-to/lint.rst` & `blueapi-0.2.1/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/how-to/make-release.rst` & `blueapi-0.2.1/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/how-to/run-tests.rst` & `blueapi-0.2.1/docs/developer/how-to/run-tests.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/how-to/update-tools.rst` & `blueapi-0.2.1/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/index.rst` & `blueapi-0.2.1/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/reference/standards.rst` & `blueapi-0.2.1/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/developer/tutorials/dev-install.rst` & `blueapi-0.2.1/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/images/blueapi-architecture.png` & `blueapi-0.2.1/docs/images/blueapi-architecture.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/images/dls-favicon.ico` & `blueapi-0.2.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/images/dls-logo.svg` & `blueapi-0.2.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/index.rst` & `blueapi-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/user/explanations/docs-structure.rst` & `blueapi-0.2.1/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/user/index.rst` & `blueapi-0.2.1/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/docs/user/tutorials/installation.rst` & `blueapi-0.2.1/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/helm/blueapi/Chart.yaml` & `blueapi-0.2.1/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.2.1/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/helm/blueapi/templates/deployment.yaml` & `blueapi-0.2.1/helm/blueapi/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.2.1/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/helm/blueapi/values.yaml` & `blueapi-0.2.1/helm/blueapi/values.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/pyproject.toml` & `blueapi-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/cli/amq.py` & `blueapi-0.2.1/src/blueapi/cli/amq.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/cli/cli.py` & `blueapi-0.2.1/src/blueapi/cli/cli.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/cli/updates.py` & `blueapi-0.2.1/src/blueapi/cli/updates.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/config.py` & `blueapi-0.2.1/src/blueapi/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from pathlib import Path
 from typing import Union
 
-from pydantic import BaseModel, Field
+from pydantic import Field
 
+from blueapi.utils import BlueapiBaseModel
 
-class StompConfig(BaseModel):
+
+class StompConfig(BlueapiBaseModel):
     """
     Config for connecting to stomp broker
     """
 
     host: str = "localhost"
     port: int = 61613
 
 
-class EnvironmentConfig(BaseModel):
+class EnvironmentConfig(BlueapiBaseModel):
     """
     Config for the RunEngine environment
     """
 
     startup_script: Union[Path, str] = "blueapi.startup.example"
 
 
-class LoggingConfig(BaseModel):
+class LoggingConfig(BlueapiBaseModel):
     level: str = "INFO"
 
 
-class ApplicationConfig(BaseModel):
+class ApplicationConfig(BlueapiBaseModel):
     """
     Config for the worker application as a whole. Root of
     config tree.
     """
 
     stomp: StompConfig = Field(default_factory=StompConfig)
     env: EnvironmentConfig = Field(default_factory=EnvironmentConfig)
```

### Comparing `blueapi-0.2.0/src/blueapi/core/__init__.py` & `blueapi-0.2.1/src/blueapi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/core/bluesky_types.py` & `blueapi-0.2.1/src/blueapi/core/bluesky_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     Subscribable,
     Triggerable,
     WritesExternalAssets,
 )
 from bluesky.utils import Msg
 from pydantic import BaseModel, Field
 
+from blueapi.utils import BlueapiBaseModel
+
 try:
     from typing import Protocol, runtime_checkable
 except ImportError:
     from typing_extensions import Protocol, runtime_checkable  # type: ignore
 
 #: A true "plan", usually the output of a generator function
 MsgGenerator = Generator[Msg, Any, None]
@@ -75,26 +77,26 @@
 def is_bluesky_plan_generator(func: PlanGenerator) -> bool:
     return (
         hasattr(func, "__annotations__")
         and func.__annotations__.get("return") is MsgGenerator
     )
 
 
-class Plan(BaseModel):
+class Plan(BlueapiBaseModel):
     """
     A plan that can be run
     """
 
     name: str = Field(description="Referenceable name of the plan")
     model: Type[BaseModel] = Field(
         description="Validation model of the parameters for the plan"
     )
 
 
-class DataEvent(BaseModel):
+class DataEvent(BlueapiBaseModel):
     """
     Event representing collection of some data. Conforms to the Bluesky event model:
     https://github.com/bluesky/event-model
     """
 
     name: str
     doc: Mapping[str, Any]
```

### Comparing `blueapi-0.2.0/src/blueapi/core/context.py` & `blueapi-0.2.1/src/blueapi/core/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from importlib import import_module
 from pathlib import Path
 from types import ModuleType
 from typing import Dict, Iterable, List, Optional, Union
 
 from bluesky import RunEngine
 from bluesky.protocols import Flyable, Readable
-from pydantic import BaseConfig
 
 from blueapi.utils import (
+    BlueapiPlanModelConfig,
     TypeValidatorDefinition,
     create_model_with_type_validators,
     load_module_all,
 )
 
 from .bluesky_types import (
     BLUESKY_PROTOCOLS,
@@ -24,18 +24,14 @@
     is_bluesky_plan_generator,
 )
 from .device_lookup import find_component
 
 LOGGER = logging.getLogger(__name__)
 
 
-class PlanModelConfig(BaseConfig):
-    arbitrary_types_allowed = True
-
-
 @dataclass
 class BlueskyContext:
     """
     Context for building a Bluesky application
     """
 
     run_engine: RunEngine = field(
@@ -118,15 +114,15 @@
             raise TypeError(f"{plan} is not a valid plan generator function")
 
         validators = list(device_validators(self))
         model = create_model_with_type_validators(
             plan.__name__,
             validators,
             func=plan,
-            config=PlanModelConfig,
+            config=BlueapiPlanModelConfig,
         )
         self.plans[plan.__name__] = Plan(name=plan.__name__, model=model)
         self.plan_functions[plan.__name__] = plan
         return plan
 
     def device(self, device: Device, name: Optional[str] = None) -> None:
         """
```

### Comparing `blueapi-0.2.0/src/blueapi/core/device_lookup.py` & `blueapi-0.2.1/src/blueapi/core/device_lookup.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/core/event.py` & `blueapi-0.2.1/src/blueapi/core/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/messaging/base.py` & `blueapi-0.2.1/src/blueapi/messaging/base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.2.1/src/blueapi/messaging/stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/messaging/utils.py` & `blueapi-0.2.1/src/blueapi/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/plans/plans.py` & `blueapi-0.2.1/src/blueapi/plans/plans.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/plans/stubs.py` & `blueapi-0.2.1/src/blueapi/plans/stubs.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/service/app.py` & `blueapi-0.2.1/src/blueapi/service/app.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/service/model.py` & `blueapi-0.2.1/src/blueapi/service/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Iterable, List
 
 from bluesky.protocols import HasName
-from pydantic import BaseModel, Field
+from pydantic import Field
 
 from blueapi.core import BLUESKY_PROTOCOLS, Device, Plan
+from blueapi.utils import BlueapiBaseModel
 
 _UNKNOWN_NAME = "UNKNOWN"
 
 
-class DeviceModel(BaseModel):
+class DeviceModel(BlueapiBaseModel):
     """
     Representation of a device
     """
 
     name: str = Field(description="Name of the device")
     protocols: List[str] = Field(
         description="Protocols that a device conforms to, indicating its capabilities"
@@ -26,57 +27,57 @@
 
 def _protocol_names(device: Device) -> Iterable[str]:
     for protocol in BLUESKY_PROTOCOLS:
         if isinstance(device, protocol):
             yield protocol.__name__
 
 
-class DeviceRequest(BaseModel):
+class DeviceRequest(BlueapiBaseModel):
     """
     A query for devices
     """
 
     ...
 
 
-class DeviceResponse(BaseModel):
+class DeviceResponse(BlueapiBaseModel):
     """
     Response to a query for devices
     """
 
     devices: List[DeviceModel] = Field(description="Devices available to use in plans")
 
 
-class PlanModel(BaseModel):
+class PlanModel(BlueapiBaseModel):
     """
     Representation of a plan
     """
 
     name: str = Field(description="Name of the plan")
 
     @classmethod
     def from_plan(cls, plan: Plan) -> "PlanModel":
         return cls(name=plan.name)
 
 
-class PlanRequest(BaseModel):
+class PlanRequest(BlueapiBaseModel):
     """
     A query for plans
     """
 
     ...
 
 
-class PlanResponse(BaseModel):
+class PlanResponse(BlueapiBaseModel):
     """
     Response to a query for plans
     """
 
     plans: List[PlanModel] = Field(description="Plans available to use by a worker")
 
 
-class TaskResponse(BaseModel):
+class TaskResponse(BlueapiBaseModel):
     """
     Acknowledgement that a task has started, includes its ID
     """
 
     task_name: str = Field(description="Unique identifier for the task")
```

### Comparing `blueapi-0.2.0/src/blueapi/startup/adsim.py` & `blueapi-0.2.1/src/blueapi/startup/adsim.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/startup/bl45p.py` & `blueapi-0.2.1/src/blueapi/startup/bl45p.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/startup/example.py` & `blueapi-0.2.1/src/blueapi/startup/example.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/startup/simmotor.py` & `blueapi-0.2.1/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/utils/config.py` & `blueapi-0.2.1/src/blueapi/utils/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/utils/modules.py` & `blueapi-0.2.1/src/blueapi/utils/modules.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/utils/serialization.py` & `blueapi-0.2.1/src/blueapi/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/utils/thread_exception.py` & `blueapi-0.2.1/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/utils/type_validator.py` & `blueapi-0.2.1/src/blueapi/utils/type_validator.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/worker/event.py` & `blueapi-0.2.1/src/blueapi/worker/event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from enum import Enum
 from typing import List, Mapping, Optional, Union
 
 from bluesky.run_engine import RunEngineStateMachine
-from pydantic import BaseModel, Field
+from pydantic import Field
 from super_state_machine.extras import PropertyMachine, ProxyString
 
+from blueapi.utils import BlueapiBaseModel
+
 # The RunEngine can return any of these three types as its state
 RawRunEngineState = Union[PropertyMachine, ProxyString, str]
 
 
 class WorkerState(str, Enum):
     """
     The state of the Worker.
@@ -37,15 +39,15 @@
         """
 
         if isinstance(bluesky_state, RunEngineStateMachine.States):
             return cls.from_bluesky_state(bluesky_state.value)
         return WorkerState(str(bluesky_state).upper())
 
 
-class StatusView(BaseModel):
+class StatusView(BlueapiBaseModel):
     """
     A snapshot of a Status of an operation, optionally representing progress
     """
 
     display_name: str = Field(
         description="Human-readable name indicating what this status describes",
         default="Unknown",
@@ -76,35 +78,35 @@
     )
     time_remaining: Optional[float] = Field(
         description="Estimated time remaining until operation completion, if known",
         default=None,
     )
 
 
-class ProgressEvent(BaseModel):
+class ProgressEvent(BlueapiBaseModel):
     """
     Event describing the progress of processes within a running task,
     such as moving motors and exposing detectors.
     """
 
     task_name: str
     statuses: Mapping[str, StatusView] = Field(default_factory=dict)
 
 
-class TaskStatus(BaseModel):
+class TaskStatus(BlueapiBaseModel):
     """
     Status of a task the worker is running.
     """
 
     task_name: str
     task_complete: bool
     task_failed: bool
 
 
-class WorkerEvent(BaseModel):
+class WorkerEvent(BlueapiBaseModel):
     """
     Event describing the state of the worker and any tasks it's running.
     Includes error and warning information.
     """
 
     state: WorkerState
     task_status: Optional[TaskStatus] = None
```

### Comparing `blueapi-0.2.0/src/blueapi/worker/multithread.py` & `blueapi-0.2.1/src/blueapi/worker/multithread.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/worker/reworker.py` & `blueapi-0.2.1/src/blueapi/worker/reworker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi/worker/task.py` & `blueapi-0.2.1/src/blueapi/worker/task.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Mapping
 
 from pydantic import BaseModel, Field, parse_obj_as
 
 from blueapi.core import BlueskyContext, Plan
+from blueapi.utils import BlueapiBaseModel
 
 
 # TODO: Make a TaggedUnion
-class Task(ABC, BaseModel):
+class Task(ABC, BlueapiBaseModel):
     """
     Object that can run with a TaskContext
     """
 
     @abstractmethod
     def do_task(self, __ctx: BlueskyContext) -> None:
         """
```

### Comparing `blueapi-0.2.0/src/blueapi/worker/worker.py` & `blueapi-0.2.1/src/blueapi/worker/worker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.2.1/src/blueapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: One line description of your module
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.2.0/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.2.1/src/blueapi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 src/blueapi/service/model.py
 src/blueapi/startup/__init__.py
 src/blueapi/startup/adsim.py
 src/blueapi/startup/bl45p.py
 src/blueapi/startup/example.py
 src/blueapi/startup/simmotor.py
 src/blueapi/utils/__init__.py
+src/blueapi/utils/base_model.py
 src/blueapi/utils/config.py
 src/blueapi/utils/modules.py
 src/blueapi/utils/serialization.py
 src/blueapi/utils/thread_exception.py
 src/blueapi/utils/type_validator.py
 src/blueapi/worker/__init__.py
 src/blueapi/worker/event.py
```

### Comparing `blueapi-0.2.0/tests/conftest.py` & `blueapi-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/core/test_context.py` & `blueapi-0.2.1/tests/core/test_context.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/core/test_event.py` & `blueapi-0.2.1/tests/core/test_event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/messaging/test_stomptemplate.py` & `blueapi-0.2.1/tests/messaging/test_stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/messaging/test_utils.py` & `blueapi-0.2.1/tests/messaging/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/plans/test_scanspec_metadata.py` & `blueapi-0.2.1/tests/plans/test_scanspec_metadata.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/utils/test_config.py` & `blueapi-0.2.1/tests/utils/test_config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/utils/test_thread_exception.py` & `blueapi-0.2.1/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.2.0/tests/utils/test_type_validator.py` & `blueapi-0.2.1/tests/utils/test_type_validator.py`

 * *Files identical despite different names*

