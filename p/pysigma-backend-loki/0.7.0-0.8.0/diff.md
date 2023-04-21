# Comparing `tmp/pysigma_backend_loki-0.7.0.tar.gz` & `tmp/pysigma_backend_loki-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_loki-0.7.0.tar", max compression
+gzip compressed data, was "pysigma_backend_loki-0.8.0.tar", max compression
```

## Comparing `pysigma_backend_loki-0.7.0.tar` & `pysigma_backend_loki-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      598 2023-03-30 11:34:46.732138 pysigma_backend_loki-0.7.0/LICENSE
--rw-r--r--   0        0        0     4138 2023-03-30 11:34:46.732138 pysigma_backend_loki-0.7.0/README.md
--rw-r--r--   0        0        0      809 2023-03-30 11:34:46.732138 pysigma_backend_loki-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      102 2023-03-30 11:34:46.732138 pysigma_backend_loki-0.7.0/sigma/backends/loki/__init__.py
--rw-r--r--   0        0        0    43538 2023-03-30 11:34:46.732138 pysigma_backend_loki-0.7.0/sigma/backends/loki/loki.py
--rw-r--r--   0        0        0      414 2023-03-30 11:34:46.732138 pysigma_backend_loki-0.7.0/sigma/pipelines/loki/__init__.py
--rw-r--r--   0        0        0     4396 2023-03-30 11:34:46.732138 pysigma_backend_loki-0.7.0/sigma/pipelines/loki/loki.py
--rw-r--r--   0        0        0     4902 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.7.0/setup.py
--rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      598 2023-04-21 13:25:19.469689 pysigma_backend_loki-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4428 2023-04-21 13:25:19.469689 pysigma_backend_loki-0.8.0/README.md
+-rw-r--r--   0        0        0      809 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/backends/loki/__init__.py
+-rw-r--r--   0        0        0    43538 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/backends/loki/loki.py
+-rw-r--r--   0        0        0      533 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/pipelines/loki/__init__.py
+-rw-r--r--   0        0        0     8382 2023-04-21 13:25:19.473689 pysigma_backend_loki-0.8.0/sigma/pipelines/loki/loki.py
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.8.0/setup.py
+-rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 pysigma_backend_loki-0.8.0/PKG-INFO
```

### Comparing `pysigma_backend_loki-0.7.0/LICENSE` & `pysigma_backend_loki-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_loki-0.7.0/README.md` & `pysigma_backend_loki-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
   * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend
 
 Further, it contains the processing pipelines in `sigma.pipelines.loki`:
 
 * `loki_log_parser`: converts field names to logfmt labels used by Grafana
 * `loki_promtail_sysmon_message`: parse and adjust field names for Windows sysmon data produced by promtail
   * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)
+* `loki_okta_system_log_json`: parse the Okta System Log event json, adjusting field-names appropriately
 
 This backend is currently maintained by:
 
 * [Nick Moore](https://github.com/kelnage)
 * [Mostafa Moradian](https://github.com/mostafa)
 
 ## Installation
@@ -34,14 +35,18 @@
 1. [Install poetry](https://python-poetry.org/docs/#installation)
 2. Clone this repository and open a terminal/shell in the top-level directory
 3. Run `poetry install` to install the Python dependencies
 4. Run `poetry shell` to activate the poetry environment
 5. Check it all works by running `poetry run pytest`
 6. (Optional) If you wish to validate the generated rules using sigma\_backend\_tester.py, install
    [LogCLI](https://grafana.com/docs/loki/latest/tools/logcli/)
+7. (Optional, but recommended) To enable the Git hooks, run the following command from the root directory of the repository:
+```sh
+git config --local core.hooksPath .githooks/
+```
 
 ## Releasing
 
 To release new versions of pySigma-backend-loki, we use GitHub actions to update PyPI. When the main branch is in state that is ready to release, the process is as follows:
 
 1. Determine the correct version number using the [Semantic Versioning](https://semver.org/) methodology. All version numbers should be in the format `\d+\.\d+\.\d+(-[0-9A-Za-z-]+)?`
 2. Update [pyproject.toml](https://github.com/grafana/pySigma-backend-loki/blob/main/pyproject.toml) with the new version number
```

### Comparing `pysigma_backend_loki-0.7.0/pyproject.toml` & `pysigma_backend_loki-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "pySigma-backend-loki"
-version = "0.7.0"
+version = "0.8.0"
 description = "pySigma Loki backend"
 readme = "README.md"
 authors = ["Nick Moore <nicholas.moore@grafana.com>", "Mostafa Moradian <mostafa.moradian@grafana.com>"]
 license = "AGPL-3.0-only"
 repository = "https://github.com/grafana/pySigma-backend-loki"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pysigma = "^0.9.5"
+pysigma = "^0.9.6"
 pysigma-pipeline-sysmon = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.1.3"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-coverage = "^7.2.1"
-mypy = "^1.0.1"
+coverage = "^7.2.3"
+mypy = "^1.2.0"
 pytest-mypy = "^0.10.1"
-types-pyyaml = "6.0.12.8"
+types-pyyaml = "6.0.12.9"
 flake8 = "^5.0.4"
 black = "^23.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysigma_backend_loki-0.7.0/sigma/backends/loki/loki.py` & `pysigma_backend_loki-0.8.0/sigma/backends/loki/loki.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_loki-0.7.0/setup.py` & `pysigma_backend_loki-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['sigma', 'sigma.backends.loki', 'sigma.pipelines.loki']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pysigma-pipeline-sysmon>=1.0.1,<2.0.0', 'pysigma>=0.9.5,<0.10.0']
+['pysigma-pipeline-sysmon>=1.0.1,<2.0.0', 'pysigma>=0.9.6,<0.10.0']
 
 setup_kwargs = {
     'name': 'pysigma-backend-loki',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'pySigma Loki backend',
-    'long_description': '![PyPI](https://img.shields.io/pypi/v/pysigma-backend-loki)\n![Tests](https://github.com/grafana/pySigma-backend-loki/actions/workflows/test.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/grafana/pySigma-backend-loki/badge.svg?branch=main&t=lvM1Ns)](https://coveralls.io/github/grafana/pySigma-backend-loki?branch=main)\n\n# pySigma Loki Backend\n\nThis is the Loki backend for pySigma. It provides the package `sigma.backends.loki` with the `LogQLBackend` class.\n\nIt supports the following output formats:\n\n* `default`: plain Loki LogQL queries\n* `ruler`: creates Loki LogQL queries in the ruler (YAML) format for generating alerts\n\nIt includes the following pipeline transformations in `sigma.pipelines.loki`:\n\n* `SetCustomAttributeTransformation`: adds a specified custom attribute to a rule, which can be used to introduce a [stream selector](https://grafana.com/docs/loki/latest/logql/log_queries/#log-stream-selector) or [parser expression](https://grafana.com/docs/loki/latest/logql/log_queries/#parser-expression) into the generated query\n  * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend\n\nFurther, it contains the processing pipelines in `sigma.pipelines.loki`:\n\n* `loki_log_parser`: converts field names to logfmt labels used by Grafana\n* `loki_promtail_sysmon_message`: parse and adjust field names for Windows sysmon data produced by promtail\n  * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)\n\nThis backend is currently maintained by:\n\n* [Nick Moore](https://github.com/kelnage)\n* [Mostafa Moradian](https://github.com/mostafa)\n\n## Installation\n\nTo get started developing/testing pySigma-backend-loki, these steps may help you get started:\n\n1. [Install poetry](https://python-poetry.org/docs/#installation)\n2. Clone this repository and open a terminal/shell in the top-level directory\n3. Run `poetry install` to install the Python dependencies\n4. Run `poetry shell` to activate the poetry environment\n5. Check it all works by running `poetry run pytest`\n6. (Optional) If you wish to validate the generated rules using sigma\\_backend\\_tester.py, install\n   [LogCLI](https://grafana.com/docs/loki/latest/tools/logcli/)\n\n## Releasing\n\nTo release new versions of pySigma-backend-loki, we use GitHub actions to update PyPI. When the main branch is in state that is ready to release, the process is as follows:\n\n1. Determine the correct version number using the [Semantic Versioning](https://semver.org/) methodology. All version numbers should be in the format `\\d+\\.\\d+\\.\\d+(-[0-9A-Za-z-]+)?`\n2. Update [pyproject.toml](https://github.com/grafana/pySigma-backend-loki/blob/main/pyproject.toml) with the new version number\n3. Commit and push the change to GitHub, and validate that the GitHub actions tests pass\n4. Create a signed tag for the release, named the version number prefixed with a v, e.g., `git tag --sign --message="Release vX.X.X" vX.X.X`\n5. Push the tag to GitHub, e.g., `git push --tags`, and validate that the release to the test instance of PyPI is successful\n6. Run `poetry build` to produce distributable versions in `dist/`\n7. Create a release in GitHub against the appropriate tag. If the version number starts with `v0`, or ends with `-alpha/beta` etc., mark it as a pre-release, and attach the distributable files to the release\n8. Validate that the release to PyPI GitHub action is successful\n\n## Work in progress\n\nThese features are currently either WIP or are planned to be implemented in the near future.\n\n* Various processing pipelines for other applications and log sources\n* Generating more accurate log stream selectors based on logsource\n* Translate field names in Sigma signatures into relevant labels for Loki using pipelines\n\n## Won\'t implement (probably)\n\nThese features are not easily supported by the backend, and hence are unlikely to be implemented.\n\n* More complex keyword/line filter searches than ANDs of ORs\n',
+    'long_description': '![PyPI](https://img.shields.io/pypi/v/pysigma-backend-loki)\n![Tests](https://github.com/grafana/pySigma-backend-loki/actions/workflows/test.yml/badge.svg)\n[![Coverage Status](https://coveralls.io/repos/github/grafana/pySigma-backend-loki/badge.svg?branch=main&t=lvM1Ns)](https://coveralls.io/github/grafana/pySigma-backend-loki?branch=main)\n\n# pySigma Loki Backend\n\nThis is the Loki backend for pySigma. It provides the package `sigma.backends.loki` with the `LogQLBackend` class.\n\nIt supports the following output formats:\n\n* `default`: plain Loki LogQL queries\n* `ruler`: creates Loki LogQL queries in the ruler (YAML) format for generating alerts\n\nIt includes the following pipeline transformations in `sigma.pipelines.loki`:\n\n* `SetCustomAttributeTransformation`: adds a specified custom attribute to a rule, which can be used to introduce a [stream selector](https://grafana.com/docs/loki/latest/logql/log_queries/#log-stream-selector) or [parser expression](https://grafana.com/docs/loki/latest/logql/log_queries/#parser-expression) into the generated query\n  * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend\n\nFurther, it contains the processing pipelines in `sigma.pipelines.loki`:\n\n* `loki_log_parser`: converts field names to logfmt labels used by Grafana\n* `loki_promtail_sysmon_message`: parse and adjust field names for Windows sysmon data produced by promtail\n  * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)\n* `loki_okta_system_log_json`: parse the Okta System Log event json, adjusting field-names appropriately\n\nThis backend is currently maintained by:\n\n* [Nick Moore](https://github.com/kelnage)\n* [Mostafa Moradian](https://github.com/mostafa)\n\n## Installation\n\nTo get started developing/testing pySigma-backend-loki, these steps may help you get started:\n\n1. [Install poetry](https://python-poetry.org/docs/#installation)\n2. Clone this repository and open a terminal/shell in the top-level directory\n3. Run `poetry install` to install the Python dependencies\n4. Run `poetry shell` to activate the poetry environment\n5. Check it all works by running `poetry run pytest`\n6. (Optional) If you wish to validate the generated rules using sigma\\_backend\\_tester.py, install\n   [LogCLI](https://grafana.com/docs/loki/latest/tools/logcli/)\n7. (Optional, but recommended) To enable the Git hooks, run the following command from the root directory of the repository:\n```sh\ngit config --local core.hooksPath .githooks/\n```\n\n## Releasing\n\nTo release new versions of pySigma-backend-loki, we use GitHub actions to update PyPI. When the main branch is in state that is ready to release, the process is as follows:\n\n1. Determine the correct version number using the [Semantic Versioning](https://semver.org/) methodology. All version numbers should be in the format `\\d+\\.\\d+\\.\\d+(-[0-9A-Za-z-]+)?`\n2. Update [pyproject.toml](https://github.com/grafana/pySigma-backend-loki/blob/main/pyproject.toml) with the new version number\n3. Commit and push the change to GitHub, and validate that the GitHub actions tests pass\n4. Create a signed tag for the release, named the version number prefixed with a v, e.g., `git tag --sign --message="Release vX.X.X" vX.X.X`\n5. Push the tag to GitHub, e.g., `git push --tags`, and validate that the release to the test instance of PyPI is successful\n6. Run `poetry build` to produce distributable versions in `dist/`\n7. Create a release in GitHub against the appropriate tag. If the version number starts with `v0`, or ends with `-alpha/beta` etc., mark it as a pre-release, and attach the distributable files to the release\n8. Validate that the release to PyPI GitHub action is successful\n\n## Work in progress\n\nThese features are currently either WIP or are planned to be implemented in the near future.\n\n* Various processing pipelines for other applications and log sources\n* Generating more accurate log stream selectors based on logsource\n* Translate field names in Sigma signatures into relevant labels for Loki using pipelines\n\n## Won\'t implement (probably)\n\nThese features are not easily supported by the backend, and hence are unlikely to be implemented.\n\n* More complex keyword/line filter searches than ANDs of ORs\n',
     'author': 'Nick Moore',
     'author_email': 'nicholas.moore@grafana.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/grafana/pySigma-backend-loki',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pysigma_backend_loki-0.7.0/PKG-INFO` & `pysigma_backend_loki-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-loki
-Version: 0.7.0
+Version: 0.8.0
 Summary: pySigma Loki backend
 Home-page: https://github.com/grafana/pySigma-backend-loki
 License: AGPL-3.0-only
 Author: Nick Moore
 Author-email: nicholas.moore@grafana.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pysigma (>=0.9.5,<0.10.0)
+Requires-Dist: pysigma (>=0.9.6,<0.10.0)
 Requires-Dist: pysigma-pipeline-sysmon (>=1.0.1,<2.0.0)
 Project-URL: Repository, https://github.com/grafana/pySigma-backend-loki
 Description-Content-Type: text/markdown
 
 ![PyPI](https://img.shields.io/pypi/v/pysigma-backend-loki)
 ![Tests](https://github.com/grafana/pySigma-backend-loki/actions/workflows/test.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/grafana/pySigma-backend-loki/badge.svg?branch=main&t=lvM1Ns)](https://coveralls.io/github/grafana/pySigma-backend-loki?branch=main)
@@ -37,14 +37,15 @@
   * The `LokiCustomAttributes` enum contains the relevant custom attribute names used by the backend
 
 Further, it contains the processing pipelines in `sigma.pipelines.loki`:
 
 * `loki_log_parser`: converts field names to logfmt labels used by Grafana
 * `loki_promtail_sysmon_message`: parse and adjust field names for Windows sysmon data produced by promtail
   * Note: most rules lack the `sysmon` service tag, and hence this pipeline should be used in combination with the [generic sysmon pipeline](https://github.com/SigmaHQ/pySigma-pipeline-sysmon)
+* `loki_okta_system_log_json`: parse the Okta System Log event json, adjusting field-names appropriately
 
 This backend is currently maintained by:
 
 * [Nick Moore](https://github.com/kelnage)
 * [Mostafa Moradian](https://github.com/mostafa)
 
 ## Installation
@@ -54,14 +55,18 @@
 1. [Install poetry](https://python-poetry.org/docs/#installation)
 2. Clone this repository and open a terminal/shell in the top-level directory
 3. Run `poetry install` to install the Python dependencies
 4. Run `poetry shell` to activate the poetry environment
 5. Check it all works by running `poetry run pytest`
 6. (Optional) If you wish to validate the generated rules using sigma\_backend\_tester.py, install
    [LogCLI](https://grafana.com/docs/loki/latest/tools/logcli/)
+7. (Optional, but recommended) To enable the Git hooks, run the following command from the root directory of the repository:
+```sh
+git config --local core.hooksPath .githooks/
+```
 
 ## Releasing
 
 To release new versions of pySigma-backend-loki, we use GitHub actions to update PyPI. When the main branch is in state that is ready to release, the process is as follows:
 
 1. Determine the correct version number using the [Semantic Versioning](https://semver.org/) methodology. All version numbers should be in the format `\d+\.\d+\.\d+(-[0-9A-Za-z-]+)?`
 2. Update [pyproject.toml](https://github.com/grafana/pySigma-backend-loki/blob/main/pyproject.toml) with the new version number
```

