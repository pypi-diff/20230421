# Comparing `tmp/mite-1.1.6.tar.gz` & `tmp/mite-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mite-1.1.6.tar", last modified: Thu Mar 23 10:45:01 2023, max compression
+gzip compressed data, was "mite-1.1.7.tar", last modified: Fri Apr 21 11:15:36 2023, max compression
```

## Comparing `mite-1.1.6.tar` & `mite-1.1.7.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.419394 mite-1.1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/.circleci/
--rw-r--r--   0 root         (0) root         (0)     5548 2023-03-23 10:44:49.000000 mite-1.1.6/.circleci/config.yml
--rw-r--r--   0 root         (0) root         (0)      233 2023-03-23 10:44:49.000000 mite-1.1.6/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      479 2023-03-23 10:44:49.000000 mite-1.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      604 2023-03-23 10:44:49.000000 mite-1.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 root         (0) root         (0)      115 2023-03-23 10:44:49.000000 mite-1.1.6/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1212 2023-03-23 10:44:49.000000 mite-1.1.6/.gitignore
--rw-r--r--   0 root         (0) root         (0)      138 2023-03-23 10:44:49.000000 mite-1.1.6/.isort.cfg
--rw-r--r--   0 root         (0) root         (0)      332 2023-03-23 10:44:49.000000 mite-1.1.6/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      696 2023-03-23 10:44:49.000000 mite-1.1.6/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     3230 2023-03-23 10:44:49.000000 mite-1.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     3929 2023-03-23 10:44:49.000000 mite-1.1.6/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     3082 2023-03-23 10:44:49.000000 mite-1.1.6/DEV.md
--rw-r--r--   0 root         (0) root         (0)     1444 2023-03-23 10:44:49.000000 mite-1.1.6/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      307 2023-03-23 10:44:49.000000 mite-1.1.6/Dockerfile.perftest
--rw-r--r--   0 root         (0) root         (0)     1100 2023-03-23 10:44:49.000000 mite-1.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-23 10:44:49.000000 mite-1.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9319 2023-03-23 10:45:01.419394 mite-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8676 2023-03-23 10:44:49.000000 mite-1.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/cd-scripts/
--rwxr-xr-x   0 root         (0) root         (0)      526 2023-03-23 10:44:49.000000 mite-1.1.6/cd-scripts/cdBuild-1.sh
--rw-r--r--   0 root         (0) root         (0)     4138 2023-03-23 10:44:49.000000 mite-1.1.6/cd-scripts/cdRelease.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-03-23 10:44:49.000000 mite-1.1.6/cd.yml
--rw-r--r--   0 root         (0) root         (0)      103 2023-03-23 10:44:49.000000 mite-1.1.6/dev-requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1624 2023-03-23 10:44:49.000000 mite-1.1.6/docker_compose.yml
--rw-r--r--   0 root         (0) root         (0)      698 2023-03-23 10:44:49.000000 mite-1.1.6/docker_compose_monitoring.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-03-23 10:44:49.000000 mite-1.1.6/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     6220 2023-03-23 10:44:49.000000 mite-1.1.6/docs/components.rst
--rw-r--r--   0 root         (0) root         (0)     2165 2023-03-23 10:44:49.000000 mite-1.1.6/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-03-23 10:44:49.000000 mite-1.1.6/docs/config.rst
--rw-r--r--   0 root         (0) root         (0)     7835 2023-03-23 10:44:49.000000 mite-1.1.6/docs/design-deployment.rst
--rw-r--r--   0 root         (0) root         (0)      945 2023-03-23 10:44:49.000000 mite-1.1.6/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     3908 2023-03-23 10:44:49.000000 mite-1.1.6/docs/journeys.rst
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-23 10:44:49.000000 mite-1.1.6/docs/notes.txt
--rw-r--r--   0 root         (0) root         (0)     2324 2023-03-23 10:44:49.000000 mite-1.1.6/docs/prometheus.rst
--rw-r--r--   0 root         (0) root         (0)     6507 2023-03-23 10:44:49.000000 mite-1.1.6/docs/stats.rst
--rw-r--r--   0 root         (0) root         (0)     1717 2023-03-23 10:44:49.000000 mite-1.1.6/docs/volume-model.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/grafana/
--rw-r--r--   0 root         (0) root         (0)      129 2023-03-23 10:44:49.000000 mite-1.1.6/grafana/Dockerfile
--rw-r--r--   0 root         (0) root         (0)       77 2023-03-23 10:44:49.000000 mite-1.1.6/grafana/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.387395 mite-1.1.6/grafana/provisioning/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/grafana/provisioning/dashboards/
--rw-r--r--   0 root         (0) root         (0)      145 2023-03-23 10:44:49.000000 mite-1.1.6/grafana/provisioning/dashboards/dashboards.yml
--rw-r--r--   0 root         (0) root         (0)    27978 2023-03-23 10:44:49.000000 mite-1.1.6/grafana/provisioning/dashboards/grafana_dashboard_template.json
--rw-r--r--   0 root         (0) root         (0)    28427 2023-03-23 10:44:49.000000 mite-1.1.6/grafana/provisioning/dashboards/mite_docker.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/grafana/provisioning/datasources/
--rw-r--r--   0 root         (0) root         (0)      180 2023-03-23 10:44:49.000000 mite-1.1.6/grafana/provisioning/datasources/datasources.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.399394 mite-1.1.6/local/
--rw-r--r--   0 root         (0) root         (0)      628 2023-03-23 10:44:49.000000 mite-1.1.6/local/Makefile
--rw-r--r--   0 root         (0) root         (0)     1349 2023-03-23 10:44:49.000000 mite-1.1.6/local/README.md
--rw-r--r--   0 root         (0) root         (0)      678 2023-03-23 10:44:49.000000 mite-1.1.6/local/demo.py
--rwxr-xr-x   0 root         (0) root         (0)     1024 2023-03-23 10:44:49.000000 mite-1.1.6/local/run_mite.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite/
--rwxr-xr-x   0 root         (0) root         (0)     2353 2023-03-23 10:44:49.000000 mite-1.1.6/mite/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    15198 2023-03-23 10:44:49.000000 mite-1.1.6/mite/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/cat.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/collector.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/common.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/duplicator.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/receiver.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/stats.py
--rw-r--r--   0 root         (0) root         (0)     6560 2023-03-23 10:44:49.000000 mite-1.1.6/mite/cli/test.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-03-23 10:44:49.000000 mite-1.1.6/mite/collector.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-03-23 10:44:49.000000 mite-1.1.6/mite/config.py
--rwxr-xr-x   0 root         (0) root         (0)     4815 2023-03-23 10:44:49.000000 mite-1.1.6/mite/context.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-03-23 10:44:49.000000 mite-1.1.6/mite/controller.py
--rw-r--r--   0 root         (0) root         (0)     2477 2023-03-23 10:44:49.000000 mite-1.1.6/mite/datapools.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-03-23 10:44:49.000000 mite-1.1.6/mite/example.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-03-23 10:44:49.000000 mite-1.1.6/mite/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-03-23 10:44:49.000000 mite-1.1.6/mite/har_to_mite.py
--rw-r--r--   0 root         (0) root         (0)     4804 2023-03-23 10:44:49.000000 mite-1.1.6/mite/logoutput.py
--rwxr-xr-x   0 root         (0) root         (0)     4591 2023-03-23 10:44:49.000000 mite-1.1.6/mite/nanomsg.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-03-23 10:44:49.000000 mite-1.1.6/mite/recorder.py
--rwxr-xr-x   0 root         (0) root         (0)     6986 2023-03-23 10:44:49.000000 mite-1.1.6/mite/runner.py
--rw-r--r--   0 root         (0) root         (0)     6226 2023-03-23 10:44:49.000000 mite-1.1.6/mite/scenario.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-03-23 10:44:49.000000 mite-1.1.6/mite/stats.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-03-23 10:44:49.000000 mite-1.1.6/mite/test.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-03-23 10:44:49.000000 mite-1.1.6/mite/utils.py
--rw-r--r--   0 root         (0) root         (0)     4584 2023-03-23 10:44:49.000000 mite-1.1.6/mite/volume_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite/web/
--rw-r--r--   0 root         (0) root         (0)      469 2023-03-23 10:44:49.000000 mite-1.1.6/mite/web/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3559 2023-03-23 10:44:49.000000 mite-1.1.6/mite/web/prometheus.py
--rwxr-xr-x   0 root         (0) root         (0)     6247 2023-03-23 10:44:49.000000 mite-1.1.6/mite/zmq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9319 2023-03-23 10:45:01.000000 mite-1.1.6/mite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3460 2023-03-23 10:45:01.000000 mite-1.1.6/mite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 10:45:01.000000 mite-1.1.6/mite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-03-23 10:45:01.000000 mite-1.1.6/mite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-23 10:45:01.000000 mite-1.1.6/mite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-03-23 10:45:01.000000 mite-1.1.6/mite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite_amqp/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-03-23 10:44:49.000000 mite-1.1.6/mite_amqp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite_browser/
--rwxr-xr-x   0 root         (0) root         (0)    17442 2023-03-23 10:44:49.000000 mite-1.1.6/mite_browser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite_finagle/
--rw-r--r--   0 root         (0) root         (0)     8329 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/README.md
--rw-r--r--   0 root         (0) root         (0)     6504 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11258 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/mux.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite_finagle/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.403394 mite-1.1.6/mite_finagle/tests/foo_service/
--rwxr-xr-x   0 root         (0) root         (0)     2698 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/foo_service/Foo-remote
--rw-r--r--   0 root         (0) root         (0)     7560 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/foo_service/Foo.py
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/foo_service/__init__.py
--rw-r--r--   0 root         (0) root         (0)      366 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/foo_service/constants.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/foo_service/ttypes.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/foo_service.thrift
--rw-r--r--   0 root         (0) root         (0)     3503 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/test_integration.py
--rw-r--r--   0 root         (0) root         (0)     4738 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/test_mux.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/tests/test_thrift.py
--rw-r--r--   0 root         (0) root         (0)     9650 2023-03-23 10:44:49.000000 mite-1.1.6/mite_finagle/thrift.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.407394 mite-1.1.6/mite_http/
--rw-r--r--   0 root         (0) root         (0)     2964 2023-03-23 10:44:49.000000 mite-1.1.6/mite_http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-03-23 10:44:49.000000 mite-1.1.6/mite_http/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.407394 mite-1.1.6/mite_selenium/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-03-23 10:44:49.000000 mite-1.1.6/mite_selenium/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-03-23 10:44:49.000000 mite-1.1.6/mite_selenium/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.407394 mite-1.1.6/mite_websocket/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-03-23 10:44:49.000000 mite-1.1.6/mite_websocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.407394 mite-1.1.6/prometheus/
--rw-r--r--   0 root         (0) root         (0)      188 2023-03-23 10:44:49.000000 mite-1.1.6/prometheus/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      206 2023-03-23 10:44:49.000000 mite-1.1.6/prometheus/prometheus_config_docker.yml
--rw-r--r--   0 root         (0) root         (0)      136 2023-03-23 10:44:49.000000 mite-1.1.6/prometheus/prometheus_config_template.yml
--rw-r--r--   0 root         (0) root         (0)      165 2023-03-23 10:44:49.000000 mite-1.1.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       70 2023-03-23 10:44:49.000000 mite-1.1.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-03-23 10:45:01.419394 mite-1.1.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      114 2023-03-23 10:44:49.000000 mite-1.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.415394 mite-1.1.6/test/
--rw-r--r--   0 root         (0) root         (0)      124 2023-03-23 10:44:49.000000 mite-1.1.6/test/legacy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.415394 mite-1.1.6/test/mocks/
--rw-r--r--   0 root         (0) root         (0)      272 2023-03-23 10:44:49.000000 mite-1.1.6/test/mocks/mock_collector.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-03-23 10:44:49.000000 mite-1.1.6/test/mocks/mock_context.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-03-23 10:44:49.000000 mite-1.1.6/test/mocks/mock_direct_receiver.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-03-23 10:44:49.000000 mite-1.1.6/test/mocks/mock_direct_runner_transport.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-23 10:44:49.000000 mite-1.1.6/test/mocks/mock_recorder_msg_http.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-03-23 10:44:49.000000 mite-1.1.6/test/mocks/mock_selenium.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-03-23 10:44:49.000000 mite-1.1.6/test/mocks/mock_sender.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 10:45:01.419394 mite-1.1.6/test/perf/
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-23 10:44:49.000000 mite-1.1.6/test/perf/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1677 2023-03-23 10:44:49.000000 mite-1.1.6/test/perf/http_server.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-03-23 10:44:49.000000 mite-1.1.6/test/perf/http_server_aiohttp.py
--rw-r--r--   0 root         (0) root         (0)      817 2023-03-23 10:44:49.000000 mite-1.1.6/test/perf/mite_perftest.py
--rwxr-xr-x   0 root         (0) root         (0)     4625 2023-03-23 10:44:49.000000 mite-1.1.6/test/perf/perftest.py
--rwxr-xr-x   0 root         (0) root         (0)     1330 2023-03-23 10:44:49.000000 mite-1.1.6/test/perf/run-perftest.sh
--rw-r--r--   0 root         (0) root         (0)       35 2023-03-23 10:44:49.000000 mite-1.1.6/test/perf/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0) 10236043 2023-03-23 10:44:49.000000 mite-1.1.6/test/test.har
--rw-r--r--   0 root         (0) root         (0)     5240 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_collector.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_config.py
--rw-r--r--   0 root         (0) root         (0)     4547 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_context.py
--rw-r--r--   0 root         (0) root         (0)     3700 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_controller.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_datapools.py
--rw-r--r--   0 root         (0) root         (0)     7712 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_har_to_mite.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_mite_amqp.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_mite_browser.py
--rw-r--r--   0 root         (0) root         (0)     2302 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_mite_http.py
--rw-r--r--   0 root         (0) root         (0)      818 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_mite_utils.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_mite_websockets.py
--rw-r--r--   0 root         (0) root         (0)     4015 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_prometheus_mite.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_recorder.py
--rw-r--r--   0 root         (0) root         (0)     2394 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_runner_tracker.py
--rw-r--r--   0 root         (0) root         (0)     2699 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_scenario.py
--rw-r--r--   0 root         (0) root         (0)     5867 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_stats.py
--rw-r--r--   0 root         (0) root         (0)     3375 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_volume_model.py
--rw-r--r--   0 root         (0) root         (0)     8670 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_webdriver.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-03-23 10:44:49.000000 mite-1.1.6/test/test_work_tracker.py
--rw-r--r--   0 root         (0) root         (0)      151 2023-03-23 10:44:49.000000 mite-1.1.6/test-requirements.txt
--rw-r--r--   0 root         (0) root         (0) 10236043 2023-03-23 10:44:49.000000 mite-1.1.6/test.har
--rw-r--r--   0 root         (0) root         (0)     1860 2023-03-23 10:44:49.000000 mite-1.1.6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/.circleci/
+-rw-r--r--   0 root         (0) root         (0)     5548 2023-04-21 11:15:24.000000 mite-1.1.7/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)      233 2023-04-21 11:15:24.000000 mite-1.1.7/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-21 11:15:24.000000 mite-1.1.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      604 2023-04-21 11:15:24.000000 mite-1.1.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 root         (0) root         (0)      115 2023-04-21 11:15:24.000000 mite-1.1.7/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-04-21 11:15:24.000000 mite-1.1.7/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      138 2023-04-21 11:15:24.000000 mite-1.1.7/.isort.cfg
+-rw-r--r--   0 root         (0) root         (0)      332 2023-04-21 11:15:24.000000 mite-1.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-21 11:15:24.000000 mite-1.1.7/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)     3230 2023-04-21 11:15:24.000000 mite-1.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     3929 2023-04-21 11:15:24.000000 mite-1.1.7/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-04-21 11:15:24.000000 mite-1.1.7/DEV.md
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-04-21 11:15:24.000000 mite-1.1.7/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-21 11:15:24.000000 mite-1.1.7/Dockerfile.perftest
+-rw-r--r--   0 root         (0) root         (0)     1100 2023-04-21 11:15:24.000000 mite-1.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-21 11:15:24.000000 mite-1.1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9319 2023-04-21 11:15:36.870287 mite-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8676 2023-04-21 11:15:24.000000 mite-1.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/cd-scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      526 2023-04-21 11:15:24.000000 mite-1.1.7/cd-scripts/cdBuild-1.sh
+-rw-r--r--   0 root         (0) root         (0)     4138 2023-04-21 11:15:24.000000 mite-1.1.7/cd-scripts/cdRelease.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-04-21 11:15:24.000000 mite-1.1.7/cd.yml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-21 11:15:24.000000 mite-1.1.7/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1624 2023-04-21 11:15:24.000000 mite-1.1.7/docker_compose.yml
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-21 11:15:24.000000 mite-1.1.7/docker_compose_monitoring.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-21 11:15:24.000000 mite-1.1.7/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6220 2023-04-21 11:15:24.000000 mite-1.1.7/docs/components.rst
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-04-21 11:15:24.000000 mite-1.1.7/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-04-21 11:15:24.000000 mite-1.1.7/docs/config.rst
+-rw-r--r--   0 root         (0) root         (0)     7835 2023-04-21 11:15:24.000000 mite-1.1.7/docs/design-deployment.rst
+-rw-r--r--   0 root         (0) root         (0)      945 2023-04-21 11:15:24.000000 mite-1.1.7/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3908 2023-04-21 11:15:24.000000 mite-1.1.7/docs/journeys.rst
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-21 11:15:24.000000 mite-1.1.7/docs/notes.txt
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-04-21 11:15:24.000000 mite-1.1.7/docs/prometheus.rst
+-rw-r--r--   0 root         (0) root         (0)     6507 2023-04-21 11:15:24.000000 mite-1.1.7/docs/stats.rst
+-rw-r--r--   0 root         (0) root         (0)     1717 2023-04-21 11:15:24.000000 mite-1.1.7/docs/volume-model.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/grafana/
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.842288 mite-1.1.7/grafana/provisioning/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/grafana/provisioning/dashboards/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/dashboards/dashboards.yml
+-rw-r--r--   0 root         (0) root         (0)    27978 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/dashboards/grafana_dashboard_template.json
+-rw-r--r--   0 root         (0) root         (0)    28427 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/dashboards/mite_docker.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/grafana/provisioning/datasources/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-21 11:15:24.000000 mite-1.1.7/grafana/provisioning/datasources/datasources.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.854288 mite-1.1.7/local/
+-rw-r--r--   0 root         (0) root         (0)      628 2023-04-21 11:15:24.000000 mite-1.1.7/local/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-04-21 11:15:24.000000 mite-1.1.7/local/README.md
+-rw-r--r--   0 root         (0) root         (0)      678 2023-04-21 11:15:24.000000 mite-1.1.7/local/demo.py
+-rwxr-xr-x   0 root         (0) root         (0)     1024 2023-04-21 11:15:24.000000 mite-1.1.7/local/run_mite.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite/
+-rwxr-xr-x   0 root         (0) root         (0)     2353 2023-04-21 11:15:24.000000 mite-1.1.7/mite/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15198 2023-04-21 11:15:24.000000 mite-1.1.7/mite/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/cat.py
+-rw-r--r--   0 root         (0) root         (0)      791 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/collector.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/duplicator.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/receiver.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/stats.py
+-rw-r--r--   0 root         (0) root         (0)     6560 2023-04-21 11:15:24.000000 mite-1.1.7/mite/cli/test.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-04-21 11:15:24.000000 mite-1.1.7/mite/collector.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-04-21 11:15:24.000000 mite-1.1.7/mite/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     4815 2023-04-21 11:15:24.000000 mite-1.1.7/mite/context.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-04-21 11:15:24.000000 mite-1.1.7/mite/controller.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-04-21 11:15:24.000000 mite-1.1.7/mite/datapools.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-04-21 11:15:24.000000 mite-1.1.7/mite/example.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-04-21 11:15:24.000000 mite-1.1.7/mite/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-04-21 11:15:24.000000 mite-1.1.7/mite/har_to_mite.py
+-rw-r--r--   0 root         (0) root         (0)     4804 2023-04-21 11:15:24.000000 mite-1.1.7/mite/logoutput.py
+-rwxr-xr-x   0 root         (0) root         (0)     4591 2023-04-21 11:15:24.000000 mite-1.1.7/mite/nanomsg.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-21 11:15:24.000000 mite-1.1.7/mite/recorder.py
+-rwxr-xr-x   0 root         (0) root         (0)     6986 2023-04-21 11:15:24.000000 mite-1.1.7/mite/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-04-21 11:15:24.000000 mite-1.1.7/mite/scenario.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-21 11:15:24.000000 mite-1.1.7/mite/stats.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-04-21 11:15:24.000000 mite-1.1.7/mite/test.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-04-21 11:15:24.000000 mite-1.1.7/mite/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-04-21 11:15:24.000000 mite-1.1.7/mite/volume_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite/web/
+-rw-r--r--   0 root         (0) root         (0)      469 2023-04-21 11:15:24.000000 mite-1.1.7/mite/web/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3559 2023-04-21 11:15:24.000000 mite-1.1.7/mite/web/prometheus.py
+-rwxr-xr-x   0 root         (0) root         (0)     6247 2023-04-21 11:15:24.000000 mite-1.1.7/mite/zmq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9319 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-21 11:15:36.000000 mite-1.1.7/mite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_amqp/
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-04-21 11:15:24.000000 mite-1.1.7/mite_amqp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_browser/
+-rwxr-xr-x   0 root         (0) root         (0)    17442 2023-04-21 11:15:24.000000 mite-1.1.7/mite_browser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_finagle/
+-rw-r--r--   0 root         (0) root         (0)     8329 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/README.md
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11258 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/mux.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.858288 mite-1.1.7/mite_finagle/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_finagle/tests/foo_service/
+-rwxr-xr-x   0 root         (0) root         (0)     2698 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/Foo-remote
+-rw-r--r--   0 root         (0) root         (0)     7560 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/Foo.py
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/constants.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service/ttypes.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/foo_service.thrift
+-rw-r--r--   0 root         (0) root         (0)     3503 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/test_integration.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/test_mux.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/tests/test_thrift.py
+-rw-r--r--   0 root         (0) root         (0)     9650 2023-04-21 11:15:24.000000 mite-1.1.7/mite_finagle/thrift.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_http/
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-04-21 11:15:24.000000 mite-1.1.7/mite_http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-21 11:15:24.000000 mite-1.1.7/mite_http/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_selenium/
+-rw-r--r--   0 root         (0) root         (0)    11427 2023-04-21 11:15:24.000000 mite-1.1.7/mite_selenium/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-04-21 11:15:24.000000 mite-1.1.7/mite_selenium/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/mite_websocket/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-04-21 11:15:24.000000 mite-1.1.7/mite_websocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.862288 mite-1.1.7/prometheus/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-04-21 11:15:24.000000 mite-1.1.7/prometheus/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      206 2023-04-21 11:15:24.000000 mite-1.1.7/prometheus/prometheus_config_docker.yml
+-rw-r--r--   0 root         (0) root         (0)      136 2023-04-21 11:15:24.000000 mite-1.1.7/prometheus/prometheus_config_template.yml
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-21 11:15:24.000000 mite-1.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-21 11:15:24.000000 mite-1.1.7/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-04-21 11:15:36.870287 mite-1.1.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      114 2023-04-21 11:15:24.000000 mite-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/test/
+-rw-r--r--   0 root         (0) root         (0)      124 2023-04-21 11:15:24.000000 mite-1.1.7/test/legacy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/test/mocks/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_collector.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_context.py
+-rw-r--r--   0 root         (0) root         (0)      584 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_direct_receiver.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_direct_runner_transport.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_recorder_msg_http.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_selenium.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-04-21 11:15:24.000000 mite-1.1.7/test/mocks/mock_sender.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 11:15:36.870287 mite-1.1.7/test/perf/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/http_server.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/http_server_aiohttp.py
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/mite_perftest.py
+-rwxr-xr-x   0 root         (0) root         (0)     4625 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/perftest.py
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/run-perftest.sh
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-21 11:15:24.000000 mite-1.1.7/test/perf/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0) 10236043 2023-04-21 11:15:24.000000 mite-1.1.7/test/test.har
+-rw-r--r--   0 root         (0) root         (0)     5240 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_collector.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     4547 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_context.py
+-rw-r--r--   0 root         (0) root         (0)     3700 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_datapools.py
+-rw-r--r--   0 root         (0) root         (0)     7712 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_har_to_mite.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_amqp.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_browser.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_http.py
+-rw-r--r--   0 root         (0) root         (0)      818 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_mite_websockets.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_prometheus_mite.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_recorder.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_runner_tracker.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_scenario.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_stats.py
+-rw-r--r--   0 root         (0) root         (0)     3375 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_volume_model.py
+-rw-r--r--   0 root         (0) root         (0)     8670 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_webdriver.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-21 11:15:24.000000 mite-1.1.7/test/test_work_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-04-21 11:15:24.000000 mite-1.1.7/test-requirements.txt
+-rw-r--r--   0 root         (0) root         (0) 10236043 2023-04-21 11:15:24.000000 mite-1.1.7/test.har
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-04-21 11:15:24.000000 mite-1.1.7/tox.ini
```

### Comparing `mite-1.1.6/.circleci/config.yml` & `mite-1.1.7/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `mite-1.1.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/.gitignore` & `mite-1.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/.travis.yml` & `mite-1.1.7/.travis.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/CODE_OF_CONDUCT.md` & `mite-1.1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/CONTRIBUTING.md` & `mite-1.1.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/DEV.md` & `mite-1.1.7/DEV.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/Dockerfile` & `mite-1.1.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/LICENSE` & `mite-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/PKG-INFO` & `mite-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mite
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Python Performance Testing Framework
 Home-page: https://github.com/sky-uk/mite/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mite-1.1.6/README.md` & `mite-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/cd-scripts/cdBuild-1.sh` & `mite-1.1.7/cd-scripts/cdBuild-1.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/cd-scripts/cdRelease.py` & `mite-1.1.7/cd-scripts/cdRelease.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/cd.yml` & `mite-1.1.7/cd.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docker_compose.yml` & `mite-1.1.7/docker_compose.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docker_compose_monitoring.yml` & `mite-1.1.7/docker_compose_monitoring.yml`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/Makefile` & `mite-1.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/components.rst` & `mite-1.1.7/docs/components.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/conf.py` & `mite-1.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/config.rst` & `mite-1.1.7/docs/config.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/design-deployment.rst` & `mite-1.1.7/docs/design-deployment.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/index.rst` & `mite-1.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/journeys.rst` & `mite-1.1.7/docs/journeys.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/prometheus.rst` & `mite-1.1.7/docs/prometheus.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/stats.rst` & `mite-1.1.7/docs/stats.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/docs/volume-model.rst` & `mite-1.1.7/docs/volume-model.rst`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/grafana/provisioning/dashboards/grafana_dashboard_template.json` & `mite-1.1.7/grafana/provisioning/dashboards/grafana_dashboard_template.json`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/grafana/provisioning/dashboards/mite_docker.json` & `mite-1.1.7/grafana/provisioning/dashboards/mite_docker.json`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/local/Makefile` & `mite-1.1.7/local/Makefile`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/local/README.md` & `mite-1.1.7/local/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/local/demo.py` & `mite-1.1.7/local/demo.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/local/run_mite.sh` & `mite-1.1.7/local/run_mite.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/__init__.py` & `mite-1.1.7/mite/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/__main__.py` & `mite-1.1.7/mite/__main__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/cli/cat.py` & `mite-1.1.7/mite/cli/cat.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/cli/collector.py` & `mite-1.1.7/mite/cli/collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/cli/common.py` & `mite-1.1.7/mite/cli/common.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/cli/duplicator.py` & `mite-1.1.7/mite/cli/duplicator.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/cli/receiver.py` & `mite-1.1.7/mite/cli/receiver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/cli/stats.py` & `mite-1.1.7/mite/cli/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/cli/test.py` & `mite-1.1.7/mite/cli/test.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/collector.py` & `mite-1.1.7/mite/collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/config.py` & `mite-1.1.7/mite/config.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/context.py` & `mite-1.1.7/mite/context.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/controller.py` & `mite-1.1.7/mite/controller.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/datapools.py` & `mite-1.1.7/mite/datapools.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/example.py` & `mite-1.1.7/mite/example.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/har_to_mite.py` & `mite-1.1.7/mite/har_to_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/logoutput.py` & `mite-1.1.7/mite/logoutput.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/nanomsg.py` & `mite-1.1.7/mite/nanomsg.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/recorder.py` & `mite-1.1.7/mite/recorder.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/runner.py` & `mite-1.1.7/mite/runner.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/scenario.py` & `mite-1.1.7/mite/scenario.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/stats.py` & `mite-1.1.7/mite/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/test.py` & `mite-1.1.7/mite/test.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/utils.py` & `mite-1.1.7/mite/utils.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/volume_model.py` & `mite-1.1.7/mite/volume_model.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/web/prometheus.py` & `mite-1.1.7/mite/web/prometheus.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite/zmq.py` & `mite-1.1.7/mite/zmq.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite.egg-info/PKG-INFO` & `mite-1.1.7/mite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mite
-Version: 1.1.6
+Version: 1.1.7
 Summary: A Python Performance Testing Framework
 Home-page: https://github.com/sky-uk/mite/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mite-1.1.6/mite.egg-info/SOURCES.txt` & `mite-1.1.7/mite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_amqp/__init__.py` & `mite-1.1.7/mite_amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_browser/__init__.py` & `mite-1.1.7/mite_browser/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/README.md` & `mite-1.1.7/mite_finagle/README.md`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/__init__.py` & `mite-1.1.7/mite_finagle/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/mux.py` & `mite-1.1.7/mite_finagle/mux.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/stats.py` & `mite-1.1.7/mite_finagle/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/tests/conftest.py` & `mite-1.1.7/mite_finagle/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/tests/foo_service/Foo-remote` & `mite-1.1.7/mite_finagle/tests/foo_service/Foo-remote`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/tests/foo_service/Foo.py` & `mite-1.1.7/mite_finagle/tests/foo_service/Foo.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/tests/foo_service/ttypes.py` & `mite-1.1.7/mite_finagle/tests/foo_service/ttypes.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/tests/test_integration.py` & `mite-1.1.7/mite_finagle/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/tests/test_mux.py` & `mite-1.1.7/mite_finagle/tests/test_mux.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/tests/test_thrift.py` & `mite-1.1.7/mite_finagle/tests/test_thrift.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_finagle/thrift.py` & `mite-1.1.7/mite_finagle/thrift.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_http/__init__.py` & `mite-1.1.7/mite_http/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_http/stats.py` & `mite-1.1.7/mite_http/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_selenium/__init__.py` & `mite-1.1.7/mite_selenium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib.util
 import logging
 import socket
 import time
 from contextlib import asynccontextmanager
+from copy import deepcopy
 from functools import wraps
 
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver import Remote as SeleniumRemote
 from selenium.webdriver.remote.remote_connection import RemoteConnection
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
@@ -31,15 +32,15 @@
             ),
             resolve_ip=False,
         )
         self._keep_alive = self._context.config.get("webdriver_keep_alive", False)
         self._file_detector = self._spec_import_if_not_none("webdriver_file_detector")
         self._proxy = self._spec_import_if_not_none("webdriver_proxy")
         self._browser_profile = self._spec_import_if_not_none("webdriver_browser_profile")
-        self._options = self._spec_import_if_not_none("webdriver_options")
+        self._options = deepcopy(self._spec_import_if_not_none("webdriver_options"))
 
         # Required param
         self._capabilities = self._context.config.get("webdriver_capabilities")
         self._capabilities = spec_import(self._capabilities)
 
     def _spec_import_if_not_none(self, config_option):
         value = self._context.config.get(config_option, None)
```

### Comparing `mite-1.1.6/mite_selenium/stats.py` & `mite-1.1.7/mite_selenium/stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/mite_websocket/__init__.py` & `mite-1.1.7/mite_websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/setup.cfg` & `mite-1.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/mocks/mock_direct_receiver.py` & `mite-1.1.7/test/mocks/mock_direct_receiver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/mocks/mock_direct_runner_transport.py` & `mite-1.1.7/test/mocks/mock_direct_runner_transport.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/mocks/mock_recorder_msg_http.py` & `mite-1.1.7/test/mocks/mock_recorder_msg_http.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/mocks/mock_selenium.py` & `mite-1.1.7/test/mocks/mock_selenium.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/perf/http_server.py` & `mite-1.1.7/test/perf/http_server.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/perf/http_server_aiohttp.py` & `mite-1.1.7/test/perf/http_server_aiohttp.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/perf/mite_perftest.py` & `mite-1.1.7/test/perf/mite_perftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/perf/perftest.py` & `mite-1.1.7/test/perf/perftest.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/perf/run-perftest.sh` & `mite-1.1.7/test/perf/run-perftest.sh`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test.har` & `mite-1.1.7/test/test.har`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_collector.py` & `mite-1.1.7/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_config.py` & `mite-1.1.7/test/test_config.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_context.py` & `mite-1.1.7/test/test_context.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_controller.py` & `mite-1.1.7/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_datapools.py` & `mite-1.1.7/test/test_datapools.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_har_to_mite.py` & `mite-1.1.7/test/test_har_to_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_mite_amqp.py` & `mite-1.1.7/test/test_mite_amqp.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_mite_browser.py` & `mite-1.1.7/test/test_mite_browser.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_mite_http.py` & `mite-1.1.7/test/test_mite_http.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_mite_utils.py` & `mite-1.1.7/test/test_mite_utils.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_mite_websockets.py` & `mite-1.1.7/test/test_mite_websockets.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_prometheus_mite.py` & `mite-1.1.7/test/test_prometheus_mite.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_recorder.py` & `mite-1.1.7/test/test_recorder.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_runner.py` & `mite-1.1.7/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_runner_tracker.py` & `mite-1.1.7/test/test_runner_tracker.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_scenario.py` & `mite-1.1.7/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_stats.py` & `mite-1.1.7/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_volume_model.py` & `mite-1.1.7/test/test_volume_model.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_webdriver.py` & `mite-1.1.7/test/test_webdriver.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test/test_work_tracker.py` & `mite-1.1.7/test/test_work_tracker.py`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/test.har` & `mite-1.1.7/test.har`

 * *Files identical despite different names*

### Comparing `mite-1.1.6/tox.ini` & `mite-1.1.7/tox.ini`

 * *Files identical despite different names*

