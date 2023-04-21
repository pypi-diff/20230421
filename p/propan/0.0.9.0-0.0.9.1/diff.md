# Comparing `tmp/propan-0.0.9.0.tar.gz` & `tmp/propan-0.0.9.1.tar.gz`

## Comparing `propan-0.0.9.0.tar` & `propan-0.0.9.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.0/SECURITY.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/1_basic_usage.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/5_publishing.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.0/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/__about__.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/__main__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/annotations.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/__init__.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/app.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/main.py
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/imports.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/log/__init__.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/log/logging.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/classes.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/functions.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/context/__init__.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/context/main.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 propan-0.0.9.0/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.0/scripts/test.sh
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 propan-0.0.9.0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.0/LICENSE
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 propan-0.0.9.0/README.md
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 propan-0.0.9.0/pyproject.toml
--rw-r--r--   0        0        0    13373 2020-02-02 00:00:00.000000 propan-0.0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.1/SECURITY.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/5_publishing.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 propan-0.0.9.1/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/__about__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/__main__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/annotations.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0     8829 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/__init__.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/app.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/main.py
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/log/__init__.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/log/logging.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/classes.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/functions.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/context/main.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 propan-0.0.9.1/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.1/scripts/test.sh
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 propan-0.0.9.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.1/LICENSE
+-rw-r--r--   0        0        0     9956 2020-02-02 00:00:00.000000 propan-0.0.9.1/README.md
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 propan-0.0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 propan-0.0.9.1/PKG-INFO
```

### Comparing `propan-0.0.9.0/CONTRIBUTING.md` & `propan-0.0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/SECURITY.md` & `propan-0.0.9.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/.github/workflows/documentation.yml` & `propan-0.0.9.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/.github/workflows/publish_coverage.yml` & `propan-0.0.9.1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/.github/workflows/publish_pypi.yml` & `propan-0.0.9.1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/.github/workflows/tests.yml` & `propan-0.0.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/3_lifespan_events.py` & `propan-0.0.9.1/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/4_cli_attributes_promotion.py` & `propan-0.0.9.1/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/5_publishing.py` & `propan-0.0.9.1/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/6_arguments_casting.py` & `propan-0.0.9.1/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/7_handler_errors_processing.py` & `propan-0.0.9.1/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/dependencies/1_dependency_injection.py` & `propan-0.0.9.1/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/dependencies/2_dependency_declaration.py` & `propan-0.0.9.1/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.0.9.1/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/dependencies/5_dependency_nesting.py` & `propan-0.0.9.1/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/dependencies/6_dependecy_calling.py` & `propan-0.0.9.1/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/dependencies/7_annotated.py` & `propan-0.0.9.1/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.0.9.1/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.0.9.1/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/http_frameworks_integrations/falcon.py` & `propan-0.0.9.1/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/http_frameworks_integrations/fastapi.py` & `propan-0.0.9.1/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/http_frameworks_integrations/quart.py` & `propan-0.0.9.1/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/http_frameworks_integrations/sanic.py` & `propan-0.0.9.1/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/examples/http_frameworks_integrations/tornado.py` & `propan-0.0.9.1/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/annotations.py` & `propan-0.0.9.1/propan/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 RabbitBroker = NatsBroker = RabbitMessage = NatsMessage = None
 
 try:
     import aio_pika
     from propan.brokers.rabbit import RabbitBroker as RB
 
     RabbitBroker = Annotated[RB, ContextField("broker")]
-    RabbitMessage = Annotated[aio_pika.IncomingMessage, ContextField("message")]
+    RabbitMessage = Annotated[aio_pika.message.IncomingMessage, ContextField("message")]
 except Exception:
     pass
 
 try:
     from nats.aio.msg import Msg
     from propan.brokers.nats import NatsBroker as NB
```

### Comparing `propan-0.0.9.0/propan/brokers/push_back_watcher.py` & `propan-0.0.9.1/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/brokers/model/broker_usecase.py` & `propan-0.0.9.1/propan/brokers/model/broker_usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,18 @@
     ):
         self.logger = logger
         self.log_level = log_level
         self._fmt = log_fmt
 
         self._connection = None
         self._is_apply_types = apply_types
+        self.handlers = []
+
         self._connection_args = args
         self._connection_kwargs = kwargs
-        self.handlers = []
 
         context.set_context("logger", logger)
         context.set_context("broker", self)
 
     async def connect(self, *args: Any, **kwargs: Any) -> Any:
         if self._connection is None:
             _args = args or self._connection_args
```

### Comparing `propan-0.0.9.0/propan/brokers/model/schemas.py` & `propan-0.0.9.1/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/brokers/nats/nats_broker.py` & `propan-0.0.9.1/propan/brokers/nats/nats_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 if handler.subject == subject and handler.queue == queue:
                     raise ValueError(
                         f"`{func.__name__}` uses already "
                         f"using `{subject}` subject with "
                         f"`{queue}` queue"
                     )
 
-            func = parent.handle(func, retry, queue=queue, subject=subject)
+            func = parent._wrap_handler(func, retry, queue=queue, subject=subject)
             handler = Handler(callback=func, subject=subject, queue=queue)
             self.handlers.append(handler)
 
         return wrapper
 
     async def start(self) -> None:
         await super().start()
```

### Comparing `propan-0.0.9.0/propan/brokers/nats/nats_broker.pyi` & `propan-0.0.9.1/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/brokers/nats/nats_js_broker.py` & `propan-0.0.9.1/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/brokers/nats/schemas.py` & `propan-0.0.9.1/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         **publish_args,
     ) -> Optional[aiormq.abc.ConfirmationFrameType]:
         if self._channel is None:
             raise ValueError("RabbitBroker channel not started yet")
 
         queue, exchange = _validate_exchange_and_queue(queue, exchange)
 
-        if not isinstance(message, aio_pika.Message):
+        if not isinstance(message, aio_pika.message.Message):
             if isinstance(message, dict):
                 message = aio_pika.Message(
                     json.dumps(message).encode(), content_type=ContentTypes.json.value
                 )
             else:
                 message = aio_pika.Message(
                     message.encode(), content_type=ContentTypes.text.value
```

### Comparing `propan-0.0.9.0/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.0.9.1/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/brokers/rabbit/schemas.py` & `propan-0.0.9.1/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/app.py` & `propan-0.0.9.1/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/main.py` & `propan-0.0.9.1/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/startproject.py` & `propan-0.0.9.1/propan/cli/startproject.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/supervisors/basereload.py` & `propan-0.0.9.1/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/supervisors/multiprocess.py` & `propan-0.0.9.1/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/supervisors/utils.py` & `propan-0.0.9.1/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/supervisors/watchfiles.py` & `propan-0.0.9.1/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/utils/imports.py` & `propan-0.0.9.1/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/utils/logs.py` & `propan-0.0.9.1/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/cli/utils/parser.py` & `propan-0.0.9.1/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/log/formatter.py` & `propan-0.0.9.1/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/log/logging.py` & `propan-0.0.9.1/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/utils/context/main.py` & `propan-0.0.9.1/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/propan/utils/context/types.py` & `propan-0.0.9.1/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/LICENSE` & `propan-0.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.0/README.md` & `propan-0.0.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 <p align="center">
-    <img src="https://lancetnik.github.io/Propan/assets/img/logo-no-background.png" alt="Propan logo" style="height: 250px; width: 600px;"/>
+    <a href="https://lancetnik.github.io/Propan/" target="_blank">
+        <img src="https://lancetnik.github.io/Propan/assets/img/logo-no-background.png" alt="Propan logo" style="height: 250px; width: 600px;"/>
+    </a>
 </p>
 
 <p align="center">
     <a href="https://github.com/Lancetnik/Propan/actions/workflows/tests.yml" target="_blank">
         <img src="https://github.com/Lancetnik/Propan/actions/workflows/tests.yml/badge.svg" alt="Tests coverage"/>
     </a>
     <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/lancetnik/propan" target="_blank">
@@ -107,16 +109,15 @@
 ```
 
 **aio-pika** is a really great tool with a really easy learning curve. But it's still imperative. You need to connect, declare channel, queues, exchanges by yourself. Also, you need to manage connection, message, queue context to avoid any troubles.
 
 It is not a bad way, but it can be easy.
 
 ```python
-from propan import PropanApp
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 @broker.handle("test_queue")
 async def base_handler(body):
@@ -139,16 +140,16 @@
 
 ### Basic usage
 
 Create an application with the following code at `serve.py`:
 
 ```python
 from propan import PropanApp
-from propan.brokers.rabbit import RabbitBroker
-# from propan.brokers.nats import NatsBroker
+from propan import RabbitBroker
+# from propan import NatsBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 # broker = NatsBroker("nats://localhost:4222")
 
 app = PropanApp(broker)
 
 @broker.handle("test")
@@ -167,16 +168,15 @@
 
 ## Type casting
 
 Propan uses `pydantic` to cast incoming function arguments to types according their annotation.
 
 ```python
 from pydantic import BaseModel
-from propan import PropanApp, Context
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, Context, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 app = PropanApp(broker)
 
 class SimpleMessage(BaseModel):
     key: int
 
@@ -200,16 +200,15 @@
 But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 from logging import Logger
 
 import aio_pika
-from propan import PropanApp, Context
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, Context, RabbitBroker
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(rabbit_broker)
 
 @rabbit_broker.handle("test")
 async def base_handler(body: dict,
@@ -231,17 +230,16 @@
 
 For example: pass your current *.env* project setting to context
 ```bash
 $ propan run serve:app --env=.env.dev
 ```
 
 ```python
-from propan import PropanApp
+from propan import PropanApp, RabbitBroker
 from propan.annotations import ContextRepo
-from propan.brokers.rabbit import RabbitBroker
 from pydantic import BaseSettings
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 class Settings(BaseSettings):
@@ -282,15 +280,15 @@
 You can use Propan MQBrokers without PropanApp.
 Just *start* and *stop* them according your application lifespan.
 
 ```python
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = FastAPI()
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
```

### Comparing `propan-0.0.9.0/pyproject.toml` & `propan-0.0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,18 @@
     "pytest-asyncio>=0.21",
     "pytest-xdist[psutil]",
 
     "asyncmock; python_version < '3.8'",
 ]
 
 doc = [
-    "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=8.1.4,<9.0.0",
     "mkdocs-static-i18n",
     "mdx-include >=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin >=0.1.7,<0.3.0",
-    "pyyaml >=5.3.1,<7.0.0",
 
     "typer[all]",
 ]
 
 dev = [
     "propan[test]",
     "propan[doc]",
```

### Comparing `propan-0.0.9.0/PKG-INFO` & `propan-0.0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.0.9.0
+Version: 0.0.9.1
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -53,29 +53,29 @@
 Requires-Dist: ruff==0.0.261; extra == 'dev'
 Requires-Dist: typer[all]; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'doc'
-Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc'
-Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
 Requires-Dist: typer[all]; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
 Requires-Dist: pytest-xdist[psutil]; extra == 'test'
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="https://lancetnik.github.io/Propan/assets/img/logo-no-background.png" alt="Propan logo" style="height: 250px; width: 600px;"/>
+    <a href="https://lancetnik.github.io/Propan/" target="_blank">
+        <img src="https://lancetnik.github.io/Propan/assets/img/logo-no-background.png" alt="Propan logo" style="height: 250px; width: 600px;"/>
+    </a>
 </p>
 
 <p align="center">
     <a href="https://github.com/Lancetnik/Propan/actions/workflows/tests.yml" target="_blank">
         <img src="https://github.com/Lancetnik/Propan/actions/workflows/tests.yml/badge.svg" alt="Tests coverage"/>
     </a>
     <a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/lancetnik/propan" target="_blank">
@@ -179,16 +179,15 @@
 ```
 
 **aio-pika** is a really great tool with a really easy learning curve. But it's still imperative. You need to connect, declare channel, queues, exchanges by yourself. Also, you need to manage connection, message, queue context to avoid any troubles.
 
 It is not a bad way, but it can be easy.
 
 ```python
-from propan import PropanApp
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 @broker.handle("test_queue")
 async def base_handler(body):
@@ -211,16 +210,16 @@
 
 ### Basic usage
 
 Create an application with the following code at `serve.py`:
 
 ```python
 from propan import PropanApp
-from propan.brokers.rabbit import RabbitBroker
-# from propan.brokers.nats import NatsBroker
+from propan import RabbitBroker
+# from propan import NatsBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 # broker = NatsBroker("nats://localhost:4222")
 
 app = PropanApp(broker)
 
 @broker.handle("test")
@@ -239,16 +238,15 @@
 
 ## Type casting
 
 Propan uses `pydantic` to cast incoming function arguments to types according their annotation.
 
 ```python
 from pydantic import BaseModel
-from propan import PropanApp, Context
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, Context, RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 app = PropanApp(broker)
 
 class SimpleMessage(BaseModel):
     key: int
 
@@ -272,16 +270,15 @@
 But you can specify your own dependencies, call dependencies functions (like `Fastapi Depends`)
 and [more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 
 ```python
 from logging import Logger
 
 import aio_pika
-from propan import PropanApp, Context
-from propan.brokers.rabbit import RabbitBroker
+from propan import PropanApp, Context, RabbitBroker
 
 rabbit_broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(rabbit_broker)
 
 @rabbit_broker.handle("test")
 async def base_handler(body: dict,
@@ -303,17 +300,16 @@
 
 For example: pass your current *.env* project setting to context
 ```bash
 $ propan run serve:app --env=.env.dev
 ```
 
 ```python
-from propan import PropanApp
+from propan import PropanApp, RabbitBroker
 from propan.annotations import ContextRepo
-from propan.brokers.rabbit import RabbitBroker
 from pydantic import BaseSettings
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 class Settings(BaseSettings):
@@ -354,15 +350,15 @@
 You can use Propan MQBrokers without PropanApp.
 Just *start* and *stop* them according your application lifespan.
 
 ```python
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
-from propan.brokers.rabbit import RabbitBroker
+from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = FastAPI()
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.0.9.0 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.0.9.1 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 4 - Beta
@@ -31,23 +31,22 @@
 Requires-Dist: isort>=5; extra == 'dev' Requires-Dist: mypy==1.1.1; extra ==
 'dev' Requires-Dist: propan[doc]; extra == 'dev' Requires-Dist: propan[test];
 extra == 'dev' Requires-Dist: ruff==0.0.261; extra == 'dev' Requires-Dist:
 typer[all]; extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-
 include<2.0.0,>=1.4.1; extra == 'doc' Requires-Dist: mkdocs-markdownextradata-
 plugin<0.3.0,>=0.1.7; extra == 'doc' Requires-Dist: mkdocs-
 material<9.0.0,>=8.1.4; extra == 'doc' Requires-Dist: mkdocs-static-i18n; extra
-== 'doc' Requires-Dist: mkdocs<2.0.0,>=1.1.2; extra == 'doc' Requires-Dist:
-pyyaml<7.0.0,>=5.3.1; extra == 'doc' Requires-Dist: typer[all]; extra == 'doc'
-Provides-Extra: test Requires-Dist: asyncmock; python_version < '3.8' and extra
-== 'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist:
-propan[async-nats]; extra == 'test' Requires-Dist: propan[async-rabbit]; extra
-== 'test' Requires-Dist: pytest-asyncio>=0.21; extra == 'test' Requires-Dist:
-pytest-xdist[psutil]; extra == 'test' Requires-Dist: pytest>=7; extra == 'test'
+== 'doc' Requires-Dist: typer[all]; extra == 'doc' Provides-Extra: test
+Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test' Requires-
+Dist: coverage[toml]>=7.2; extra == 'test' Requires-Dist: propan[async-nats];
+extra == 'test' Requires-Dist: propan[async-rabbit]; extra == 'test' Requires-
+Dist: pytest-asyncio>=0.21; extra == 'test' Requires-Dist: pytest-xdist
+[psutil]; extra == 'test' Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
-                                 [Propan logo]
+                                 [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *an another one HTTP* a **declarative Python MQ
 framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides helpful development
 toolkit, existed only at HTTP-frameworks world until now. It's designed to
 create reactive microservices around Messaging_Architecture. It is a modern,
@@ -89,64 +88,62 @@
 "test_queue" async with connection: channel = await connection.channel() queue
 = await channel.declare_queue(queue_name) async with queue.iterator() as
 queue_iter: async for message in queue_iter: async with message.process():
 print(message.body) asyncio.run(main()) ``` **aio-pika** is a really great tool
 with a really easy learning curve. But it's still imperative. You need to
 connect, declare channel, queues, exchanges by yourself. Also, you need to
 manage connection, message, queue context to avoid any troubles. It is not a
-bad way, but it can be easy. ```python from propan import PropanApp from
-propan.brokers.rabbit import RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
-async def base_handler(body): print(body) ``` This is the **Propan**
-declarative way to write the same code. That is so much easier, isn't it? --
-- ## Quickstart Install using `pip`: ```shell $ pip install "propan[async-
-rabbit]" # or $ pip install "propan[async-nats]" ``` ### Basic usage Create an
-application with the following code at `serve.py`: ```python from propan import
-PropanApp from propan.brokers.rabbit import RabbitBroker # from
-propan.brokers.nats import NatsBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") app =
-PropanApp(broker) @broker.handle("test") async def base_handler(body):
+bad way, but it can be easy. ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
+print(body) ``` This is the **Propan** declarative way to write the same code.
+That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
+```shell $ pip install "propan[async-rabbit]" # or $ pip install "propan[async-
+nats]" ``` ### Basic usage Create an application with the following code at
+`serve.py`: ```python from propan import PropanApp from propan import
+RabbitBroker # from propan import NatsBroker broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222")
+app = PropanApp(broker) @broker.handle("test") async def base_handler(body):
 '''Handle all default exchange messages with `test` routing key''' print(body)
 ``` And just run it: ```shell $ propan run serve:app ``` --- ## Type casting
 Propan uses `pydantic` to cast incoming function arguments to types according
 their annotation. ```python from pydantic import BaseModel from propan import
-PropanApp, Context from propan.brokers.rabbit import RabbitBroker broker =
-RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp(broker)
-class SimpleMessage(BaseModel): key: int @broker.handle("test2") async def
-second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` --
-- ## Dependencies Propan has dependencies management policy close to `pytest
-fixtures`. You can specify in functions arguments which dependencies you would
-to use. Framework passes them from the global Context object. Already existed
-context fields are: *app*, *broker*, *context* (itself), *logger* and
-*message*. If you call not existed field, raises
-*pydantic.error_wrappers.ValidationError* value. But you can specify your own
-dependencies, call dependencies functions (like `Fastapi Depends`) and [more]
-(https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
-```python from logging import Logger import aio_pika from propan import
-PropanApp, Context from propan.brokers.rabbit import RabbitBroker rabbit_broker
-= RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
-(rabbit_broker) @rabbit_broker.handle("test") async def base_handler(body:
-dict, broker: RabbitBroker = Context()): assert broker is rabbit_broker ``` --
-- ## CLI power Propan has own cli tool provided the following features: *
-project generation * multiprocessing workers * project hot reloading * custom
-command line arguments passing ### Context passing For example: pass your
-current *.env* project setting to context ```bash $ propan run serve:app --
-env=.env.dev ``` ```python from propan import PropanApp from propan.annotations
-import ContextRepo from propan.brokers.rabbit import RabbitBroker from pydantic
-import BaseSettings broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-app = PropanApp(broker) class Settings(BaseSettings): ... @app.on_startup async
-def setup(env: str, context: ContextRepo): settings = Settings(_env_file=env)
-context.set_context("settings", settings) ``` ### Project template Also
-**propan cli** is able to generate production-ready application template:
-```shell $ propan create [projectname] ``` *Notice: project template require*
-`pydantic[dotenv]` *installation.* Run created project: ```shell # Run rabbimq
-first $ docker compose --file [projectname]/docker-compose.yaml up -d # Run
-project $ propan run [projectname].app.serve:app --env=.env --reload ``` Now
-you can enjoy a new development experience! --- ## HTTP Frameworks integrations
-You can use Propan MQBrokers without PropanApp. Just *start* and *stop* them
-according your application lifespan. ```python from contextlib import
-asynccontextmanager from fastapi import FastAPI from propan.brokers.rabbit
-import RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-app = FastAPI() @asynccontextmanager async def lifespan(app: FastAPI): await
-broker.start() yield await broker.close() @broker.handle("test") async def
-base_handler(body): print(body) ``` ## Examples To see more framework usages go
-to [**examples/**](https://github.com/Lancetnik/Propan/tree/main/examples)
+PropanApp, Context, RabbitBroker broker = RabbitBroker("amqp://guest:
+guest@localhost:5672/") app = PropanApp(broker) class SimpleMessage(BaseModel):
+key: int @broker.handle("test2") async def second_handler(body: SimpleMessage):
+assert isinstance(body.key, int) ``` --- ## Dependencies Propan has
+dependencies management policy close to `pytest fixtures`. You can specify in
+functions arguments which dependencies you would to use. Framework passes them
+from the global Context object. Already existed context fields are: *app*,
+*broker*, *context* (itself), *logger* and *message*. If you call not existed
+field, raises *pydantic.error_wrappers.ValidationError* value. But you can
+specify your own dependencies, call dependencies functions (like `Fastapi
+Depends`) and [more](https://github.com/Lancetnik/Propan/tree/main/examples/
+dependencies). ```python from logging import Logger import aio_pika from propan
+import PropanApp, Context, RabbitBroker rabbit_broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(rabbit_broker)
+@rabbit_broker.handle("test") async def base_handler(body: dict, broker:
+RabbitBroker = Context()): assert broker is rabbit_broker ``` --- ## CLI power
+Propan has own cli tool provided the following features: * project generation *
+multiprocessing workers * project hot reloading * custom command line arguments
+passing ### Context passing For example: pass your current *.env* project
+setting to context ```bash $ propan run serve:app --env=.env.dev ``` ```python
+from propan import PropanApp, RabbitBroker from propan.annotations import
+ContextRepo from pydantic import BaseSettings broker = RabbitBroker("amqp://
+guest:guest@localhost:5672/") app = PropanApp(broker) class Settings
+(BaseSettings): ... @app.on_startup async def setup(env: str, context:
+ContextRepo): settings = Settings(_env_file=env) context.set_context
+("settings", settings) ``` ### Project template Also **propan cli** is able to
+generate production-ready application template: ```shell $ propan create
+[projectname] ``` *Notice: project template require* `pydantic[dotenv]`
+*installation.* Run created project: ```shell # Run rabbimq first $ docker
+compose --file [projectname]/docker-compose.yaml up -d # Run project $ propan
+run [projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
+development experience! --- ## HTTP Frameworks integrations You can use Propan
+MQBrokers without PropanApp. Just *start* and *stop* them according your
+application lifespan. ```python from contextlib import asynccontextmanager from
+fastapi import FastAPI from propan import RabbitBroker broker = RabbitBroker
+("amqp://guest:guest@localhost:5672/") app = FastAPI() @asynccontextmanager
+async def lifespan(app: FastAPI): await broker.start() yield await broker.close
+() @broker.handle("test") async def base_handler(body): print(body) ``` ##
+Examples To see more framework usages go to [**examples/**](https://github.com/
+Lancetnik/Propan/tree/main/examples)
```

