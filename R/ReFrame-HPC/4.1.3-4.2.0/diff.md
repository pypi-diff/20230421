# Comparing `tmp/ReFrame-HPC-4.1.3.tar.gz` & `tmp/ReFrame-HPC-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReFrame-HPC-4.1.3.tar", last modified: Tue Apr 11 19:55:47 2023, max compression
+gzip compressed data, was "ReFrame-HPC-4.2.0.tar", last modified: Fri Apr 21 20:18:13 2023, max compression
```

## Comparing `ReFrame-HPC-4.1.3.tar` & `ReFrame-HPC-4.2.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.096786 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 19:55:47.000000 ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.096786 ReFrame-HPC-4.1.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/bin/reframe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.096786 ReFrame-HPC-4.1.3/reframe/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.100786 ReFrame-HPC-4.1.3/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    31089 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.100786 ReFrame-HPC-4.1.3/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/launchers/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32228 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    35258 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    93588 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    54049 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22001 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.104786 ReFrame-HPC-4.1.3/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    25779 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (123)    47416 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-11 19:55:37.000000 ReFrame-HPC-4.1.3/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-11 19:55:47.108786 ReFrame-HPC-4.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.554676 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 20:18:13.000000 ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.554676 ReFrame-HPC-4.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/bin/reframe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.554676 ReFrame-HPC-4.2.0/reframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.558676 ReFrame-HPC-4.2.0/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31411 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23075 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.558676 ReFrame-HPC-4.2.0/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/launchers/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32490 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35671 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94467 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14256 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22673 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28261 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55074 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.562676 ReFrame-HPC-4.2.0/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)    49317 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-21 20:18:00.000000 ReFrame-HPC-4.2.0/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-21 20:18:13.566676 ReFrame-HPC-4.2.0/setup.cfg
```

### Comparing `ReFrame-HPC-4.1.3/LICENSE` & `ReFrame-HPC-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/PKG-INFO` & `ReFrame-HPC-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.1.3
+Version: 4.2.0
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.1.3/README.md` & `ReFrame-HPC-4.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/reframe-hpc/reframe?include_prereleases)
 ![GitHub commits since latest release](https://img.shields.io/github/commits-since/reframe-hpc/reframe/latest)
 ![GitHub contributors](https://img.shields.io/github/contributors-anon/reframe-hpc/reframe)<br/>
 [![PyPI version](https://badge.fury.io/py/ReFrame-HPC.svg)](https://badge.fury.io/py/ReFrame-HPC)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc)](https://pepy.tech/project/reframe-hpc)
 [![Downloads](https://pepy.tech/badge/reframe-hpc/month)](https://pepy.tech/project/reframe-hpc)<br/>
-[![Slack](https://reframe-slack.herokuapp.com/badge.svg)](https://reframe-slack.herokuapp.com/)<br/>
+[![Slack](https://badgen.net/badge/icon/slack?icon=slack&label)](https://join.slack.com/t/reframetalk/shared_invite/zt-1tar8s71w-At0tolJ~~zxT2oG_2Ly9sw)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![DOI](https://zenodo.org/badge/89384186.svg)](https://zenodo.org/badge/latestdoi/89384186)<br/>
 [![Twitter Follow](https://img.shields.io/twitter/follow/ReFrameHPC?style=social)](https://twitter.com/ReFrameHPC)
 
 # ReFrame in a Nutshell
 
 ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems.
@@ -89,13 +89,13 @@
 
 ## Contact
 
 You can get in contact with the ReFrame community in the following ways:
 
 ### Slack
 
-Please join the community's [Slack channel](https://reframe-slack.herokuapp.com) for keeping up with the latest news about ReFrame, posting questions and, generally getting in touch with other users and the developers.
+Please join the community's [Slack channel](https://join.slack.com/t/reframetalk/shared_invite/zt-1tar8s71w-At0tolJ~~zxT2oG_2Ly9sw) for keeping up with the latest news about ReFrame, posting questions and, generally getting in touch with other users and the developers.
 
 ## Contributing back
 
 ReFrame is an open-source project and we welcome and encourage contributions!
 Check out our Contribution Guide [here](https://github.com/reframe-hpc/reframe/wiki/contributing-to-reframe).
```

### Comparing `ReFrame-HPC-4.1.3/README_minimal.md` & `ReFrame-HPC-4.2.0/README_minimal.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/PKG-INFO` & `ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.1.3
+Version: 4.2.0
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.1.3/ReFrame_HPC.egg-info/SOURCES.txt` & `ReFrame-HPC-4.2.0/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/bin/reframe` & `ReFrame-HPC-4.2.0/bin/reframe`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/__init__.py` & `ReFrame-HPC-4.2.0/reframe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.1.3'
+VERSION = '4.2.0'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/backends.py` & `ReFrame-HPC-4.2.0/reframe/core/backends.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/buildsystems.py` & `ReFrame-HPC-4.2.0/reframe/core/buildsystems.py`

 * *Files 1% similar despite different names*

```diff
@@ -865,25 +865,37 @@
 
     #: Options to pass to ``spack install``
     #:
     #: :type: :class:`List[str]`
     #: :default: ``[]``
     install_opts = variable(typ.List[str], value=[])
 
+    #: A list of Spack configurations in flattened YAML.
+    #:
+    #: :type: :class:`List[str]`
+    #: :default: ``[]``
+    #:
+    #: .. versionadded:: 4.2
+    config_opts = variable(typ.List[str], value=[])
+
     def __init__(self):
         # Set to True if the environment was auto-generated
         self._auto_env = False
 
     def emit_build_commands(self, environ):
         ret = self._create_env_cmds()
 
+        config_opts = []
         if self._auto_env:
             install_tree = self.install_tree or 'opt/spack'
-            ret.append(f'spack -e {self.environment} config add '
-                       f'"config:install_tree:root:{install_tree}"')
+            config_opts.append(f'config:install_tree:root:{install_tree}')
+
+        config_opts += self.config_opts
+        for opt in config_opts:
+            ret.append(f'spack -e {self.environment} config add "{opt}"')
 
         if self.specs:
             specs_str = ' '.join(self.specs)
             ret.append(f'spack -e {self.environment} add {specs_str}')
 
         install_cmd = f'spack -e {self.environment} install'
         if self.install_opts:
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/builtins.py` & `ReFrame-HPC-4.2.0/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/config.py` & `ReFrame-HPC-4.2.0/reframe/core/config.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/containers.py` & `ReFrame-HPC-4.2.0/reframe/core/containers.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/decorators.py` & `ReFrame-HPC-4.2.0/reframe/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/deferrable.py` & `ReFrame-HPC-4.2.0/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/environments.py` & `ReFrame-HPC-4.2.0/reframe/core/environments.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/exceptions.py` & `ReFrame-HPC-4.2.0/reframe/core/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,18 @@
     '''
 
 
 class FailureLimitError(ReframeError):
     '''Raised when the limit of test failures has been reached.'''
 
 
+class RunSessionTimeout(ReframeError):
+    '''Raised when the maximum duration for a test session expires.'''
+
+
 class AbortTaskError(ReframeError):
     '''Raised by the runtime inside a regression task to denote that it has
     been aborted due to an external reason (e.g., keyboard interrupt, fatal
     error in other places etc.)
     '''
 
 
@@ -351,14 +355,20 @@
     if isinstance(exc_value, soft_errors):
         return False
 
     # User errors are treated as soft
     return not is_user_error(exc_type, exc_value, tb)
 
 
+def is_warning(exc_type, exc_value, tb):
+    '''Check whether this exception can be treated as warning'''
+
+    return isinstance(exc_value, (RunSessionTimeout, KeyboardInterrupt))
+
+
 def what(exc_type, exc_value, tb):
     '''A short description of the error.'''
 
     if exc_type is None:
         return ''
 
     reason = utility.decamelize(exc_type.__name__, ' ')
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/fields.py` & `ReFrame-HPC-4.2.0/reframe/core/fields.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/fixtures.py` & `ReFrame-HPC-4.2.0/reframe/core/fixtures.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/hooks.py` & `ReFrame-HPC-4.2.0/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/launchers/__init__.py` & `ReFrame-HPC-4.2.0/reframe/core/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/launchers/local.py` & `ReFrame-HPC-4.2.0/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/launchers/mpi.py` & `ReFrame-HPC-4.2.0/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/launchers/ssh.py` & `ReFrame-HPC-4.2.0/reframe/core/launchers/ssh.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/logging.py` & `ReFrame-HPC-4.2.0/reframe/core/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -469,14 +469,15 @@
 
 
 def _create_httpjson_handler(site_config, config_prefix):
     url = site_config.get(f'{config_prefix}/url')
     extras = site_config.get(f'{config_prefix}/extras')
     ignore_keys = site_config.get(f'{config_prefix}/ignore_keys')
     json_formatter = site_config.get(f'{config_prefix}/json_formatter')
+    extra_headers = site_config.get(f'{config_prefix}/extra_headers')
     debug = site_config.get(f'{config_prefix}/debug')
 
     parsed_url = urllib.parse.urlparse(url)
     if parsed_url.scheme not in {'http', 'https'}:
         raise ConfigError(
             "httpjson handler: invalid url scheme: use 'http' or 'https'"
         )
@@ -510,15 +511,16 @@
         if not debug:
             return None
 
     if debug:
         getlogger().warning('httpjson: running in debug mode; '
                             'no data will be sent to the server')
 
-    return HTTPJSONHandler(url, extras, ignore_keys, json_formatter, debug)
+    return HTTPJSONHandler(url, extras, ignore_keys, json_formatter,
+                           extra_headers, debug)
 
 
 def _record_to_json(record, extras, ignore_keys):
     def _can_send(key):
         return not key.startswith('_') and not key in ignore_keys
 
     def _sanitize(s):
@@ -559,15 +561,16 @@
         'filename', 'funcName', 'levelname', 'levelno',
         'lineno', 'message', 'module', 'msecs', 'msg', 'name',
         'pathname', 'process', 'processName', 'relativeCreated',
         'stack_info', 'thread', 'threadName', 'exc_text'
     }
 
     def __init__(self, url, extras=None, ignore_keys=None,
-                 json_formatter=None, debug=False):
+                 json_formatter=None, extra_headers=None,
+                 debug=False):
         super().__init__()
         self._url = url
         self._extras = extras
         self._ignore_keys = self.LOG_ATTRS
         if ignore_keys:
             self._ignore_keys |= set(ignore_keys)
 
@@ -577,14 +580,19 @@
 
         if not is_trivially_callable(self._json_format, non_def_args=3):
             raise ConfigError(
                 "httpjson: 'json_formatter' has not the right signature: "
                 "it must be 'json_formatter(record, extras, ignore_keys)'"
             )
 
+        self._headers = {'Content-type': 'application/json',
+                         'Accept-Charset': 'UTF-8'}
+        if extra_headers:
+            self._headers.update(extra_headers)
+
         self._debug = debug
 
     def emit(self, record):
         # Convert tags to a list to make them JSON friendly
         record.check_tags = list(record.check_tags)
         json_record = self._json_format(record,
                                         self._extras,
@@ -600,16 +608,15 @@
                 fp.write(json_record)
 
             return
 
         try:
             requests.post(
                 self._url, data=json_record,
-                headers={'Content-type': 'application/json',
-                         'Accept-Charset': 'UTF-8'}
+                headers=self._headers
             )
         except requests.exceptions.RequestException as e:
             raise LoggingError('logging failed') from e
 
 
 def _extract_handlers(site_config, handlers_group):
     handler_prefix = f'logging/0/{handlers_group}'
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/meta.py` & `ReFrame-HPC-4.2.0/reframe/core/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 
 #
 # Meta-class for creating regression tests.
 #
 
 import functools
+import inspect
 import types
 import collections
 
 import reframe.core.builtins as builtins
 import reframe.core.namespaces as namespaces
 import reframe.core.parameters as parameters
 import reframe.core.variables as variables
@@ -817,15 +818,15 @@
         for c in cls.mro():
             if hasattr(c, '_rfm_loggable_props'):
                 loggable_props += c._rfm_loggable_props
 
         return sorted(loggable_props + loggable_vars + loggable_params)
 
 
-def make_test(name, bases, body, methods=None, **kwargs):
+def make_test(name, bases, body, methods=None, module=None, **kwargs):
     '''Define a new test class programmatically.
 
     Using this method is completely equivalent to using the :keyword:`class`
     to define the test class. More specifically, the following:
 
     .. code-block:: python
 
@@ -890,21 +891,26 @@
     :param bases: A tuple of the base classes of the class that is being
         created.
     :param body: A mapping of key/value pairs that will be inserted as class
         attributes in the newly created class.
     :param methods: A list of functions to be bound as methods to the class
         that is being created. The functions will be bound with their original
         name.
+    :param module: The module name of the new test class.
+        If :obj:`None`, the module of the caller will be used.
     :param kwargs: Any keyword arguments to be passed to the
         :class:`RegressionTestMeta` metaclass.
 
     .. versionadded:: 3.10.0
 
     .. versionchanged:: 3.11.0
-       Added the ``methods`` arguments.
+       Added the ``methods`` argument.
+
+    .. versionadded:: 4.2
+       Added the ``module`` argument.
 
     '''
     namespace = RegressionTestMeta.__prepare__(name, bases, **kwargs)
     methods = methods or []
 
     # Add methods to the body
     for m in methods:
@@ -915,8 +921,15 @@
     # `__setitem__()` as if the body elements were actually being typed in the
     # class definition
     namespace.update(body)
     for k in list(namespace.keys()):
         namespace.reset(k)
 
     cls = RegressionTestMeta(name, bases, namespace, **kwargs)
+
+    if not module:
+        # Set the test's module to be that of our callers
+        caller = inspect.currentframe().f_back
+        module = caller.f_globals['__name__']
+
+    cls.__module__ = module
     return cls
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/modules.py` & `ReFrame-HPC-4.2.0/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/namespaces.py` & `ReFrame-HPC-4.2.0/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/parameters.py` & `ReFrame-HPC-4.2.0/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/pipeline.py` & `ReFrame-HPC-4.2.0/reframe/core/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -958,14 +958,37 @@
     #: responsibility to check whether the build phase failed by adding an
     #: appropriate sanity check.
     #:
     #: :type: boolean
     #: :default: :class:`True`
     build_locally = variable(typ.Bool, value=True, loggable=True)
 
+    #: .. versionadded:: 4.2
+    #:
+    #: Extra options to be passed to the child CI pipeline generated for this
+    #: test using the :option:`--ci-generate` option.
+    #:
+    #: This variable is a dictionary whose keys refer the CI generate backend
+    #: and the values can be in any CI backend-specific format.
+    #:
+    #: Currently, the only key supported is ``'gitlab'`` and the values is a
+    #: Gitlab configuration in JSON format. For example, if we want a pipeline
+    #: to run only when files in ``backend`` or ``src/main.c`` have changed,
+    #: this variable should be set as follows:
+    #:
+    #: .. code-block:: python
+    #:
+    #:    ci_extras = {
+    #:        'only': {'changes': ['backend/*', 'src/main.c']}
+    #:    }
+    #:
+    #: :type: :class:`dict`
+    #: :default: ``{}``
+    ci_extras = variable(typ.Dict[typ.Str['gitlab'], object], value={})
+
     # Special variables
 
     #: Dry-run mode
     _rfm_dry_run = variable(typ.Bool, value=False)
 
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls)
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/runtime.py` & `ReFrame-HPC-4.2.0/reframe/core/runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,18 +166,31 @@
         '''Get a configuration option.
 
         :arg option: The option to be retrieved.
         :arg default: The value to return if ``option`` cannot be retrieved.
         :returns: The value of the option.
 
         .. versionchanged:: 3.11.0
-          Add ``default`` named argument.
+           Add ``default`` named argument.
         '''
         return self._site_config.get(option, default=default)
 
+    def get_default(self, option):
+        '''Get the default value for the option as defined in the configuration
+        schema.
+
+        :arg option: The option whose default value is requested
+        :returns: The default value of the requested option
+        :raises KeyError: if option does not have a default value
+
+        .. versionadded:: 4.2
+        '''
+
+        return self._site_config.schema['defaults'][option]
+
 
 # Global resources for the current host
 _runtime_context = None
 
 
 def init_runtime(site_config):
     global _runtime_context
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/__init__.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/flux.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/local.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,25 +94,32 @@
         '''Send SIGKILL to all the processes of the spawned job.'''
         try:
             os.killpg(job.jobid, signal.SIGKILL)
             job._signal = signal.SIGKILL
         except (ProcessLookupError, PermissionError):
             # The process group may already be dead or assigned to a different
             # group, so ignore this error
-            self.log(f'pid {job.jobid} already dead or assigned elsewhere')
+            self.log(f'pid {job.jobid} already dead')
         finally:
             # Close file handles
             job.f_stdout.close()
             job.f_stderr.close()
             job._state = 'FAILURE'
 
     def _term_all(self, job):
         '''Send SIGTERM to all the processes of the spawned job.'''
-        os.killpg(job.jobid, signal.SIGTERM)
-        job._signal = signal.SIGTERM
+        try:
+            os.killpg(job.jobid, signal.SIGTERM)
+            job._signal = signal.SIGTERM
+        except (ProcessLookupError, PermissionError):
+            # Job has finished already, close file handles
+            self.log(f'pid {job.jobid} already dead')
+            job.f_stdout.close()
+            job.f_stderr.close()
+            job._state = 'FAILURE'
 
     def cancel(self, job):
         '''Cancel job.
 
         The SIGTERM signal will be sent first to all the processes of this job
         and after a grace period (default 2s) the SIGKILL signal will be send.
```

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/lsf.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/oar.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/pbs.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/registry.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/sge.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/schedulers/slurm.py` & `ReFrame-HPC-4.2.0/reframe/core/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/settings.py` & `ReFrame-HPC-4.2.0/reframe/core/settings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/shell.py` & `ReFrame-HPC-4.2.0/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/systems.py` & `ReFrame-HPC-4.2.0/reframe/core/systems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/variables.py` & `ReFrame-HPC-4.2.0/reframe/core/variables.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/core/warnings.py` & `ReFrame-HPC-4.2.0/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/argparse.py` & `ReFrame-HPC-4.2.0/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/autodetect.py` & `ReFrame-HPC-4.2.0/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/cli.py` & `ReFrame-HPC-4.2.0/reframe/frontend/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 import reframe.frontend.filters as filters
 import reframe.frontend.runreport as runreport
 import reframe.utility as util
 import reframe.utility.jsonext as jsonext
 import reframe.utility.osext as osext
 import reframe.utility.typecheck as typ
 
-
 from reframe.frontend.testgenerators import (distribute_tests,
                                              getallnodes, repeat_tests)
 from reframe.frontend.executors.policies import (SerialExecutionPolicy,
                                                  AsynchronousExecutionPolicy)
 from reframe.frontend.executors import Runner, generate_testcases
 from reframe.frontend.loader import RegressionCheckLoader
 from reframe.frontend.printer import PrettyPrinter
@@ -399,14 +398,18 @@
     run_options.add_argument(
         '--distribute', action='store', metavar='{all|STATE}',
         nargs='?', const='idle',
         help=('Distribute the selected single-node jobs on every node that'
               'is in STATE (default: "idle"')
     )
     run_options.add_argument(
+        '--duration', action='store', metavar='TIMEOUT',
+        help='Run the test session repeatedly for the specified duration'
+    )
+    run_options.add_argument(
         '--exec-order', metavar='ORDER', action='store',
         choices=['name', 'random', 'rname', 'ruid', 'uid'],
         help='Impose an execution order for independent tests'
     )
     run_options.add_argument(
         '--exec-policy', metavar='POLICY', action='store',
         choices=['async', 'serial'], default='async',
@@ -435,14 +438,18 @@
         '--mode', action='store', help='Execution mode to use'
     )
     run_options.add_argument(
         '--repeat', action='store', metavar='N',
         help='Repeat selected tests N times'
     )
     run_options.add_argument(
+        '--reruns', action='store', metavar='N', default=0,
+        help='Rerun the whole test session N times', type=int
+    )
+    run_options.add_argument(
         '--restore-session', action='store', nargs='?', const='',
         metavar='REPORT',
         help='Restore a testing session from REPORT file'
     )
     run_options.add_argument(
         '-S', '--setvar', action='append', metavar='[TEST.]VAR=VAL',
         dest='vars', default=[],
@@ -1295,45 +1302,58 @@
             sched_flex_alloc_nodes = options.flex_alloc_nodes
 
         exec_policy.sched_flex_alloc_nodes = sched_flex_alloc_nodes
         exec_policy.sched_options = parsed_job_options
         if options.maxfail < 0:
             raise errors.CommandLineError(
                 f'--maxfail should be a non-negative integer: '
-                f'{options.maxfail!r}'
+                f'{options.maxfail}'
+            )
+
+        if options.reruns and options.duration:
+            raise errors.CommandLineError(
+                f"'--reruns' option cannot be combined with '--duration'"
+            )
+
+        if options.reruns < 0:
+            raise errors.CommandLineError(
+                f"'--reruns' should be a non-negative integer: {options.reruns}"
             )
 
         runner = Runner(exec_policy, printer, options.max_retries,
-                        options.maxfail)
+                        options.maxfail, options.reruns, options.duration)
         try:
             time_start = time.time()
             session_info['time_start'] = time.strftime(
                 '%FT%T%z', time.localtime(time_start),
             )
             runner.runall(testcases, restored_cases)
         finally:
             time_end = time.time()
             session_info['time_end'] = time.strftime(
                 '%FT%T%z', time.localtime(time_end)
             )
             session_info['time_elapsed'] = time_end - time_start
 
             # Print a retry report if we did any retries
-            if runner.stats.failed(run=0):
+            if options.max_retries and runner.stats.failed(run=0):
                 printer.info(runner.stats.retry_report())
 
             # Print a failure report if we had failures in the last run
             success = True
             if runner.stats.failed():
                 success = False
                 runner.stats.print_failure_report(
-                    printer, not options.distribute
+                    printer, not options.distribute,
+                    options.duration or options.reruns
                 )
                 if options.failure_stats:
-                    runner.stats.print_failure_stats(printer)
+                    runner.stats.print_failure_stats(
+                        printer, options.duration or options.reruns
+                    )
 
             if options.performance_report:
                 printer.info(runner.stats.performance_report())
 
             # Generate the report for this session
             report_file = os.path.normpath(
                 osext.expandvars(rt.get_option('general/0/report_file'))
@@ -1354,23 +1374,22 @@
                 'restored_cases': []
             }
             if options.restore_session is not None:
                 for c in restored_cases:
                     json_report['restored_cases'].append(report.case(*c))
 
             report_file = runreport.next_report_filename(report_file)
+            default_loc = os.path.dirname(
+                osext.expandvars(rt.get_default('general/report_file'))
+            )
             try:
-                with open(report_file, 'w') as fp:
-                    if rt.get_option('general/0/compress_report'):
-                        jsonext.dump(json_report, fp)
-                    else:
-                        jsonext.dump(json_report, fp, indent=2)
-                        fp.write('\n')
-
-                printer.info(f'Run report saved in {report_file!r}')
+                runreport.write_report(json_report, report_file,
+                                       rt.get_option(
+                                           'general/0/compress_report'),
+                                       os.path.dirname(report_file) == default_loc)
             except OSError as e:
                 printer.warning(
                     f'failed to generate report in {report_file!r}: {e}'
                 )
 
             # Generate the junit xml report for this session
             junit_report_file = rt.get_option('general/0/report_junit')
@@ -1390,15 +1409,20 @@
         if not success:
             sys.exit(1)
 
         sys.exit(0)
     except (Exception, KeyboardInterrupt, errors.ReframeFatalError):
         exc_info = sys.exc_info()
         tb = ''.join(traceback.format_exception(*exc_info))
-        printer.error(f'run session stopped: {errors.what(*exc_info)}')
+        message = f'run session stopped: {errors.what(*exc_info)}'
+        if errors.is_warning(*exc_info):
+            printer.warning(message)
+        else:
+            printer.error(message)
+
         if errors.is_exit_request(*exc_info):
             # Print stack traces for exit requests only when TOO verbose
             printer.debug2(tb)
         elif errors.is_severe(*exc_info):
             printer.error(tb)
         else:
             printer.verbose(tb)
```

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/dependencies.py` & `ReFrame-HPC-4.2.0/reframe/frontend/dependencies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/executors/__init__.py` & `ReFrame-HPC-4.2.0/reframe/frontend/executors/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 import copy
 import os
 import signal
 import sys
 import time
 import weakref
 
+import reframe.core.fields as fields
 import reframe.core.logging as logging
 import reframe.core.runtime as runtime
 import reframe.frontend.dependencies as dependencies
 import reframe.utility.jsonext as jsonext
+import reframe.utility.typecheck as typ
 from reframe.core.exceptions import (AbortTaskError,
                                      JobNotStartedError,
                                      FailureLimitError,
                                      ForceExitError,
+                                     RunSessionTimeout,
                                      SkipTestError,
                                      TaskExit)
 from reframe.core.schedulers.local import LocalJobScheduler
 from reframe.frontend.printer import PrettyPrinter
 from reframe.frontend.statistics import TestStats
 
 ABORT_REASONS = (AssertionError, FailureLimitError,
-                 KeyboardInterrupt, ForceExitError)
+                 KeyboardInterrupt, ForceExitError, RunSessionTimeout)
 
 
 class TestCase:
     '''A combination of a regression check, a system partition
     and a programming environment.
     '''
 
@@ -128,24 +131,29 @@
                     case.prepare()
 
                 cases.append(case)
 
     return cases
 
 
+def clone_testcases(cases):
+    new_cases = [tc.clone() for tc in cases]
+    return dependencies.toposort(dependencies.build_deps(new_cases)[0])
+
+
 class RegressionTask:
     '''A class representing a :class:`RegressionTest` through the regression
     pipeline.'''
 
-    def __init__(self, case, listeners=[]):
+    def __init__(self, case, listeners=None, timeout=None):
         self._case = case
         self._failed_stage = None
         self._current_stage = 'startup'
         self._exc_info = (None, None, None)
-        self._listeners = list(listeners)
+        self._listeners = listeners or []
         self._skipped = False
 
         # Reference count for dependent tests; safe to cleanup the test only
         # if it is zero
         self.ref_count = case.num_dependents
 
         # Test case has finished, but has not been waited for yet
@@ -387,46 +395,44 @@
         self._perflogger.log_performance(logging.INFO, self,
                                          multiline=self._perflog_compat)
 
     @logging.time_function
     def cleanup(self, *args, **kwargs):
         self._safe_call(self.check.cleanup, *args, **kwargs)
 
-    def fail(self, exc_info=None):
+    def fail(self, exc_info=None, callback='on_task_failure'):
         self._failed_stage = self._current_stage
         self._exc_info = exc_info or sys.exc_info()
-        self._notify_listeners('on_task_failure')
+        self._notify_listeners(callback)
         self._perflogger.log_performance(logging.INFO, self,
                                          multiline=self._perflog_compat)
 
     def skip(self, exc_info=None):
         self._skipped = True
         self._failed_stage = self._current_stage
         self._exc_info = exc_info or sys.exc_info()
         self._notify_listeners('on_task_skip')
 
     def abort(self, cause=None):
         if self.failed or self._aborted:
             return
 
-        logging.getlogger().debug2('Aborting test case: {self.testcase!r}')
+        logging.getlogger().debug2(f'Aborting test case: {self.testcase!r}')
         exc = AbortTaskError()
         exc.__cause__ = cause
         self._aborted = True
         try:
-            # FIXME: we should perhaps extend the RegressionTest interface
-            # for supporting job cancelling
             if not self.zombie and self.check.job:
                 self.check.job.cancel()
         except JobNotStartedError:
-            self.fail((type(exc), exc, None))
+            self.fail((type(exc), exc, None), 'on_task_abort')
         except BaseException:
             self.fail()
         else:
-            self.fail((type(exc), exc, None))
+            self.fail((type(exc), exc, None), 'on_task_abort')
 
     def info(self):
         '''Return an info string about this task.'''
         name = self.check.display_name
         hashcode = self.check.hashcode
         part = self.testcase.partition.fullname
         env  = self.testcase.environ.name
@@ -457,38 +463,52 @@
 
     @abc.abstractmethod
     def on_task_skip(self, task):
         '''Called whenever a RegressionTask is skipped.'''
 
     @abc.abstractmethod
     def on_task_failure(self, task):
-        '''Called when a regression test has failed.'''
+        '''Called when a RegressionTask has failed.'''
+
+    @abc.abstractmethod
+    def on_task_abort(self, task):
+        '''Called when a RegressionTask has aborted.'''
 
     @abc.abstractmethod
     def on_task_success(self, task):
         '''Called when a regression test has succeeded.'''
 
 
 def _handle_sigterm(signum, frame):
     raise ForceExitError('received TERM signal')
 
 
 class Runner:
     '''Responsible for executing a set of regression tests based on an
     execution policy.'''
 
+    _timeout = fields.TypedField(typ.Duration, type(None), allow_implicit=True)
+
     def __init__(self, policy, printer=None, max_retries=0,
-                 max_failures=sys.maxsize):
+                 max_failures=sys.maxsize, reruns=0, timeout=None):
         self._policy = policy
         self._printer = printer or PrettyPrinter()
         self._max_retries = max_retries
+        self._num_reruns = reruns
+        self._timeout = timeout
+        self._t_init = timeout
+        self._global_stats = False
+        if self._num_reruns or self._timeout:
+            self._global_stats = True
+
         self._stats = TestStats()
         self._policy.stats = self._stats
         self._policy.printer = self._printer
         self._policy.max_failures = max_failures
+
         signal.signal(signal.SIGTERM, _handle_sigterm)
 
     @property
     def max_failures(self):
         return self._max_failures
 
     @property
@@ -503,41 +523,68 @@
     def stats(self):
         return self._stats
 
     @logging.time_function
     def runall(self, testcases, restored_cases=None):
         num_checks = len({tc.check.unique_name for tc in testcases})
         self._printer.separator('short double line',
-                                'Running %d check(s)' % num_checks)
+                                f'Running {num_checks} check(s)')
         self._printer.timestamp('Started on', 'short double line')
         self._printer.info('')
         try:
+            self._t_init = time.time()
+            if self._timeout:
+                self._policy.set_expiry(self._t_init + self._timeout)
+
             self._runall(testcases)
             if self._max_retries:
                 restored_cases = restored_cases or []
                 self._retry_failed(testcases + restored_cases)
+
+            if self._timeout:
+                # Repeat the session until timeout expires
+                t_elapsed = time.time() - self._t_init
+                while self._timeout >= t_elapsed:
+                    rt = runtime.runtime()
+                    rt.next_run()
+                    self._runall(clone_testcases(testcases))
+                else:
+                    raise RunSessionTimeout('maximum session '
+                                            'duration exceeded')
+            else:
+                # Repeat the session if requested
+                for _ in range(self._num_reruns):
+                    rt = runtime.runtime()
+                    rt.next_run()
+                    self._runall(clone_testcases(testcases))
         finally:
             # Print the summary line
-            num_failures = len(self._stats.failed())
-            num_completed = len(self._stats.completed())
-            num_skipped = len(self._stats.skipped())
-            num_tasks = len(self._stats.tasks())
-            if num_failures > 0 or num_completed + num_skipped < num_tasks:
+            runid = None if self._global_stats else -1
+            num_aborted = len(self._stats.aborted(runid))
+            num_failures = len(self._stats.failed(runid))
+            num_completed = len(self._stats.completed(runid))
+            num_skipped = len(self._stats.skipped(runid))
+            num_tasks = self._stats.num_cases(runid)
+            if num_failures > 0:
                 status = 'FAILED'
+            elif num_aborted > 0:
+                status = 'ABORTED'
             else:
                 status = 'PASSED'
 
-            total_run = len(testcases)
-            total_completed = len(self._stats.completed(0))
-            total_skipped = len(self._stats.skipped(0))
+            runid = None if self._global_stats else 0
+            total_run = self._stats.num_cases(runid)
+            total_completed = len(self._stats.completed(runid))
+            total_skipped = len(self._stats.skipped(runid))
             self._printer.status(
                 status,
                 f'Ran {total_completed}/{total_run}'
                 f' test case(s) from {num_checks} check(s) '
-                f'({num_failures} failure(s), {total_skipped} skipped)',
+                f'({num_failures} failure(s), {total_skipped} skipped, '
+                f'{num_aborted} aborted)',
                 just='center'
             )
             self._printer.timestamp('Finished on', 'short double line')
 
     def _retry_failed(self, cases):
         rt = runtime.runtime()
         failures = self._stats.failed()
@@ -598,14 +645,26 @@
         self.sched_flex_alloc_nodes = None
         self.sched_options = []
 
         # Task event listeners
         self.task_listeners = []
         self.stats = None
 
+        # Expiration time
+        self._t_expire = None
+
+    def set_expiry(self, t_point):
+        self._t_expire = t_point
+
+    def timeout_expired(self):
+        if self._t_expire is None:
+            return False
+
+        return time.time() >= self._t_expire
+
     def enter(self):
         self._num_failed_tasks = 0
 
     def exit(self):
         pass
 
     @abc.abstractmethod
```

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/executors/policies.py` & `ReFrame-HPC-4.2.0/reframe/frontend/executors/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import math
 import sys
 import time
 
 import reframe.core.runtime as rt
 import reframe.utility as util
 from reframe.core.exceptions import (FailureLimitError,
+                                     RunSessionTimeout,
                                      SkipTestError,
                                      TaskDependencyError,
                                      TaskExit)
 from reframe.core.logging import getlogger, level_from_str
 from reframe.core.pipeline import (CompileOnlyRegressionTest,
                                    RunOnlyRegressionTest)
 from reframe.frontend.executors import (ExecutionPolicy, RegressionTask,
@@ -125,15 +126,14 @@
                     task.skip()
                     raise TaskExit from e
 
             task.setup(task.testcase.partition,
                        task.testcase.environ,
                        sched_flex_alloc_nodes=self.sched_flex_alloc_nodes,
                        sched_options=self.sched_options)
-
             task.compile()
             task.compile_wait()
             task.run()
 
             # Pick the right scheduler
             if task.check.local:
                 sched = self.local_scheduler
@@ -182,14 +182,18 @@
     def on_task_compile_exit(self, task):
         pass
 
     def on_task_skip(self, task):
         msg = str(task.exc_info[1])
         self.printer.status('SKIP', msg, just='right')
 
+    def on_task_abort(self, task):
+        msg = f'{task.info()}'
+        self.printer.status('ABORT', msg, just='right')
+
     def on_task_failure(self, task):
         self._num_failed_tasks += 1
         msg = f'{task.info()}'
         if task.failed_stage == 'cleanup':
             self.printer.status('ERROR', msg, just='right')
         else:
             self.printer.status('FAIL', msg, just='right')
@@ -205,14 +209,17 @@
                          f'test staged in {task.check.stagedir!r}')
         getlogger().verbose(f'==> {timings}')
         if self._num_failed_tasks >= self.max_failures:
             raise FailureLimitError(
                 f'maximum number of failures ({self.max_failures}) reached'
             )
 
+        if self.timeout_expired():
+            raise RunSessionTimeout('maximum session duration exceeded')
+
     def on_task_success(self, task):
         msg = f'{task.info()}'
         self.printer.status('OK', msg, just='right')
         _print_perf(task)
         timings = task.pipeline_timings(['setup',
                                          'compile_complete',
                                          'run_complete',
@@ -224,14 +231,16 @@
         # Update reference count of dependencies
         for c in task.testcase.deps:
             # NOTE: Restored dependencies are not in the task_index
             if c in self._task_index:
                 self._task_index[c].ref_count -= 1
 
         _cleanup_all(self._retired_tasks, not self.keep_stage_files)
+        if self.timeout_expired():
+            raise RunSessionTimeout('maximum session duration exceeded')
 
     def exit(self):
         # Clean up all remaining tasks
         _cleanup_all(self._retired_tasks, not self.keep_stage_files)
 
 
 class AsynchronousExecutionPolicy(ExecutionPolicy, TaskEventListener):
@@ -334,15 +343,14 @@
         while self._current_tasks:
             try:
                 self._poll_tasks()
                 num_running = sum(
                     1 if t.state in ('running', 'compiling') else 0
                     for t in self._current_tasks
                 )
-
                 timeout = rt.runtime().get_option(
                     'general/0/pipeline_timeout'
                 )
 
                 self._advance_all(self._current_tasks, timeout)
                 if self._pipeline_statistics:
                     num_retired = len(self._retired_tasks)
@@ -354,18 +362,23 @@
                     # Some tests might not be cleaned up because they are
                     # waiting for dependencies or because their dependencies
                     # have failed.
                     self._update_pipeline_progress(
                         'retired', 'completed', num_retired_actual
                     )
 
+                if self.timeout_expired():
+                    raise RunSessionTimeout(
+                        'maximum session duration exceeded'
+                    )
+
                 if num_running:
                     self._pollctl.snooze()
             except ABORT_REASONS as e:
-                self._failall(e)
+                self._abortall(e)
                 raise
 
         if self._pipeline_statistics:
             self._dump_pipeline_progress('pipeline-progress.json')
 
     def _poll_tasks(self):
         if self.dry_run_mode:
@@ -558,16 +571,17 @@
                    for c in task.testcase.deps if c in self._task_index)
 
     def deps_skipped(self, task):
         # NOTE: Restored dependencies are not in the task_index
         return any(self._task_index[c].skipped
                    for c in task.testcase.deps if c in self._task_index)
 
-    def _failall(self, cause):
+    def _abortall(self, cause):
         '''Mark all tests as failures'''
+
         getlogger().debug2(f'Aborting all tasks due to {type(cause).__name__}')
         for task in self._current_tasks:
             with contextlib.suppress(FailureLimitError):
                 task.abort(cause)
 
     # These function can be useful for tracking statistics of the framework,
     # such as number of tests that have finished setup etc.
@@ -586,14 +600,18 @@
     def on_task_compile_exit(self, task):
         self._pollctl.reset_snooze_time()
 
     def on_task_skip(self, task):
         msg = str(task.exc_info[1])
         self.printer.status('SKIP', msg, just='right')
 
+    def on_task_abort(self, task):
+        msg = f'{task.info()}'
+        self.printer.status('ABORT', msg, just='right')
+
     def on_task_failure(self, task):
         self._num_failed_tasks += 1
         msg = f'{task.info()}'
         if task.failed_stage == 'cleanup':
             self.printer.status('ERROR', msg, just='right')
         else:
             self.printer.status('FAIL', msg, just='right')
```

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/filters.py` & `ReFrame-HPC-4.2.0/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/loader.py` & `ReFrame-HPC-4.2.0/reframe/frontend/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,35 @@
 
 import reframe.utility as util
 import reframe.utility.osext as osext
 from reframe.core.exceptions import NameConflictError, is_severe, what
 from reframe.core.logging import getlogger, time_function
 
 
+class temp_sys_path:
+    def __init__(self, path):
+        self._path = path
+        self._pos = None
+
+    def __enter__(self):
+        self._pos = len(sys.path)
+        sys.path.append(self._path)
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        sys.path.pop(self._pos)
+
+
+class no_op:
+    def __enter__(self):
+        pass
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
+
 class RegressionCheckValidator(ast.NodeVisitor):
     def __init__(self):
         self._has_import = False
         self._has_regression_test = False
 
     @property
     def valid(self):
@@ -174,21 +195,25 @@
                         f'is already defined in {conflicted!r}'
                     )
 
         getlogger().debug(f'  > Loaded {len(final_tests)} test(s)')
         return final_tests
 
     def load_from_file(self, filename, force=False):
+        filename = os.path.abspath(filename)
         if not self._validate_source(filename):
             return []
 
         try:
-            return self.load_from_module(
-                util.import_module_from_file(filename, force)
-            )
+            dirname = os.path.dirname(filename)
+            with osext.change_dir(dirname):
+                with temp_sys_path(dirname):
+                    return self.load_from_module(
+                        util.import_module_from_file(filename, force)
+                    )
         except Exception:
             exc_info = sys.exc_info()
             if not is_severe(*exc_info):
                 # Simply skip the file in this case
                 getlogger().warning(
                     f"skipping test file {filename!r}: {what(*exc_info)} "
                     f"(rerun with '-v' for more information)"
```

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/printer.py` & `ReFrame-HPC-4.2.0/reframe/frontend/printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,24 +44,26 @@
         elif just == 'right':
             status = status.rjust(self.status_width - 2)
         else:
             status = status.ljust(self.status_width - 2)
 
         status_stripped = status.strip()
         if self.colorize:
-            if status_stripped in ('DRY', 'SKIP'):
+            if status_stripped in ('ABORT', 'ABORTED', 'DRY', 'SKIP'):
                 status = color.colorize(status, color.YELLOW)
             elif status_stripped in ('FAIL', 'FAILED', 'ERROR'):
                 status = color.colorize(status, color.RED)
             else:
                 status = color.colorize(status, color.GREEN)
 
         final_msg = f'[ {status} ] '
-        if status_stripped in ('OK', 'SKIP', 'FAIL'):
-            self._progress_count += 1
+        if status_stripped in ('ABORT', 'OK', 'SKIP', 'FAIL'):
+            if self._progress_count < self._progress_total:
+                self._progress_count += 1
+
             width = len(str(self._progress_total))
             padded_progress = str(self._progress_count).rjust(width)
             final_msg += f'({padded_progress}/{self._progress_total}) '
 
         final_msg += message
         logging.getlogger().log(level, final_msg)
```

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/runreport.py` & `ReFrame-HPC-4.2.0/reframe/frontend/runreport.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright 2016-2023 Swiss National Supercomputing Centre (CSCS/ETH Zurich)
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import decimal
+import functools
 import json
 import jsonschema
 import lxml.etree as etree
 import os
 import re
 
 import reframe as rfm
 import reframe.core.exceptions as errors
 import reframe.utility.jsonext as jsonext
+import reframe.utility.osext as osext
+from reframe.core.logging import getlogger
 from reframe.core.warnings import suppress_deprecations
 
 # The schema data version
 # Major version bumps are expected to break the validation of previous schemas
 
 DATA_VERSION = '3.1'
 _SCHEMA = os.path.join(rfm.INSTALL_PREFIX, 'reframe/schemas/runreport.json')
@@ -175,14 +178,44 @@
     # Add fallback reports
     for f in filenames[1:]:
         rpt.add_fallback(_load_report(f))
 
     return rpt
 
 
+def write_report(report, filename, compress=False, link_to_last=False):
+    with open(filename, 'w') as fp:
+        if compress:
+            jsonext.dump(report, fp)
+        else:
+            jsonext.dump(report, fp, indent=2)
+            fp.write('\n')
+
+        if not link_to_last:
+            return
+
+        # Add a symlink to the latest report
+        basedir = os.path.dirname(filename)
+        with osext.change_dir(basedir):
+            link_name = 'latest.json'
+            create_symlink = functools.partial(
+                os.symlink, os.path.basename(filename), link_name
+            )
+            if not os.path.exists(link_name):
+                create_symlink()
+            else:
+                if os.path.islink(link_name):
+                    os.remove(link_name)
+                    create_symlink()
+                else:
+                    getlogger().warning('could not create a symlink '
+                                        'to the latest report file: '
+                                        'path exists and is not a symlink')
+
+
 def junit_xml_report(json_report):
     '''Generate a JUnit report from a standard ReFrame JSON report.'''
 
     xml_testsuites = etree.Element('testsuites')
     for run_id, rfm_run in enumerate(json_report['runs']):
         xml_testsuite = etree.SubElement(
             xml_testsuites, 'testsuite',
```

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/statistics.py` & `ReFrame-HPC-4.2.0/reframe/frontend/statistics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2016-2023 Swiss National Supercomputing Centre (CSCS/ETH Zurich)
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import inspect
+import itertools
 import os
 import shutil
 import traceback
 
 import reframe.core.runtime as rt
 import reframe.core.exceptions as errors
 import reframe.utility as util
@@ -33,33 +34,40 @@
         current_run = rt.runtime().current_run
         if current_run == len(self._alltasks):
             self._alltasks.append([])
 
         self._alltasks[current_run].append(task)
 
     def tasks(self, run=-1):
-        try:
-            return self._alltasks[run]
-        except IndexError:
-            raise errors.StatisticsError(f'no such run: {run}') from None
+        if run is None:
+            yield from itertools.chain(*self._alltasks)
+        else:
+            try:
+                yield from self._alltasks[run]
+            except IndexError:
+                raise errors.StatisticsError(f'no such run: {run}') from None
 
     def failed(self, run=-1):
         return [t for t in self.tasks(run) if t.failed]
 
     def skipped(self, run=-1):
         return [t for t in self.tasks(run) if t.skipped]
 
     def aborted(self, run=-1):
         return [t for t in self.tasks(run) if t.aborted]
 
     def completed(self, run=-1):
         return [t for t in self.tasks(run) if t.completed]
 
     def num_cases(self, run=-1):
-        return len(self.tasks(run))
+        return sum(1 for _ in self.tasks(run))
+
+    @property
+    def num_runs(self):
+        return len(self._alltasks)
 
     def retry_report(self):
         # Return an empty report if no retries were done.
         if not rt.runtime().current_run:
             return ''
 
         line_width = shutil.get_terminal_size()[0]
@@ -225,15 +233,16 @@
                 'num_skipped': num_skipped,
                 'runid': runid,
                 'testcases': testcases
             })
 
         return self._run_data
 
-    def print_failure_report(self, printer, rerun_info=True):
+    def print_failure_report(self, printer, rerun_info=True,
+                             global_stats=False):
         def _head_n(filename, prefix, num_lines=10):
             # filename and prefix are `None` before setup
             if filename is None or prefix is None:
                 return []
 
             try:
                 with open(os.path.join(prefix, filename)) as fp:
@@ -247,91 +256,101 @@
 
                 lines += [f'--- {filename} ---']
             except OSError as e:
                 lines = [f'--- {filename} ({e}) ---']
 
             return lines
 
-        line_width = shutil.get_terminal_size()[0]
-        printer.info(line_width * '=')
-        printer.info('SUMMARY OF FAILURES')
-        run_report = self.json()[-1]
-        last_run = run_report['runid']
-        for r in run_report['testcases']:
-            if r['result'] in {'success', 'aborted', 'skipped'}:
-                continue
-
-            retry_info = (
-                f'(for the last of {last_run} retries)' if last_run > 0 else ''
-            )
+        def _print_failure_info(rec, runid, total_runs):
             printer.info(line_width * '-')
-            printer.info(f"FAILURE INFO for {r['unique_name']} {retry_info}")
-            printer.info(f"  * Expanded name: {r['display_name']}")
-            printer.info(f"  * Description: {r['description']}")
-            printer.info(f"  * System partition: {r['system']}")
-            printer.info(f"  * Environment: {r['environment']}")
-            printer.info(f"  * Stage directory: {r['stagedir']}")
+            printer.info(f"FAILURE INFO for {rec['display_name']} "
+                         f"(run: {runid}/{total_runs})")
+            printer.info(f"  * Description: {rec['description']}")
+            printer.info(f"  * System partition: {rec['system']}")
+            printer.info(f"  * Environment: {rec['environment']}")
+            printer.info(f"  * Stage directory: {rec['stagedir']}")
             printer.info(
-                f"  * Node list: {util.nodelist_abbrev(r['nodelist'])}"
+                f"  * Node list: {util.nodelist_abbrev(rec['nodelist'])}"
             )
-            job_type = 'local' if r['scheduler'] == 'local' else 'batch job'
-            printer.info(f"  * Job type: {job_type} (id={r['jobid']})")
+            job_type = 'local' if rec['scheduler'] == 'local' else 'batch job'
+            printer.info(f"  * Job type: {job_type} (id={rec['jobid']})")
             printer.info(f"  * Dependencies (conceptual): "
-                         f"{r['dependencies_conceptual']}")
+                         f"{rec['dependencies_conceptual']}")
             printer.info(f"  * Dependencies (actual): "
-                         f"{r['dependencies_actual']}")
-            printer.info(f"  * Maintainers: {r['maintainers']}")
-            printer.info(f"  * Failing phase: {r['fail_phase']}")
-            if rerun_info and not r['fixture']:
-                printer.info(f"  * Rerun with '-n /{r['hash']}"
-                             f" -p {r['environment']} --system "
-                             f"{r['system']} -r'")
+                         f"{rec['dependencies_actual']}")
+            printer.info(f"  * Maintainers: {rec['maintainers']}")
+            printer.info(f"  * Failing phase: {rec['fail_phase']}")
+            if rerun_info and not rec['fixture']:
+                printer.info(f"  * Rerun with '-n /{rec['hash']}"
+                             f" -p {rec['environment']} --system "
+                             f"{rec['system']} -r'")
 
-            msg = r['fail_reason']
-            if isinstance(r['fail_info']['exc_value'], errors.SanityError):
+            msg = rec['fail_reason']
+            if isinstance(rec['fail_info']['exc_value'], errors.SanityError):
                 lines = [msg]
-                lines += _head_n(r['job_stdout'], prefix = r['stagedir'])
-                lines += _head_n(r['job_stderr'], prefix = r['stagedir'])
+                lines += _head_n(rec['job_stdout'], prefix=rec['stagedir'])
+                lines += _head_n(rec['job_stderr'], prefix=rec['stagedir'])
                 msg = '\n'.join(lines)
 
             printer.info(f"  * Reason: {msg}")
 
-            tb = ''.join(traceback.format_exception(*r['fail_info'].values()))
-            if r['fail_severe']:
+            tb = ''.join(traceback.format_exception(
+                *rec['fail_info'].values()))
+            if rec['fail_severe']:
                 printer.info(tb)
             else:
                 printer.verbose(tb)
 
+        line_width = shutil.get_terminal_size()[0]
+        printer.info(line_width * '=')
+        printer.info('SUMMARY OF FAILURES')
+
+        run_report = self.json()
+        for run_no, run_info in enumerate(run_report, start=1):
+            if not global_stats and run_no != len(run_report):
+                continue
+
+            for r in run_info['testcases']:
+                if r['result'] in {'success', 'aborted', 'skipped'}:
+                    continue
+
+                _print_failure_info(r, run_no, len(run_report))
+
         printer.info(line_width * '-')
 
-    def print_failure_stats(self, printer):
+    def print_failure_stats(self, printer, global_stats=False):
+        if global_stats:
+            runid = None
+        else:
+            runid = rt.runtime().current_run
+
         failures = {}
-        current_run = rt.runtime().current_run
-        for tf in (t for t in self.tasks(current_run) if t.failed):
-            check = tf.check
-            partition = check.current_partition
-            partfullname = partition.fullname if partition else 'None'
-            environ_name = (check.current_environ.name
-                            if check.current_environ else 'None')
-            f = (f'[{check.display_name} (uid: {check.unique_name}), '
-                 f'{environ_name}, {partfullname}]')
+        for tf in (t for t in self.tasks(runid) if t.failed):
+            check, partition, environ = tf.testcase
+            info = f'[{check.display_name}]'
+            if partition:
+                info += f' @{partition.fullname}'
+
+            if environ:
+                info += f'+{environ.name}'
+
             if tf.failed_stage not in failures:
                 failures[tf.failed_stage] = []
 
-            failures[tf.failed_stage].append(f)
+            failures[tf.failed_stage].append(info)
 
         line_width = shutil.get_terminal_size()[0]
         stats_start = line_width * '='
         stats_title = 'FAILURE STATISTICS'
         stats_end = line_width * '-'
         stats_body = []
         row_format = "{:<13} {:<5} {}"
         stats_hline = row_format.format(13*'-', 5*'-', 60*'-')
         stats_header = row_format.format('Phase', '#', 'Failing test cases')
-        num_tests = len(self.tasks(current_run))
+        num_tests = self.num_cases(runid)
         num_failures = 0
         for fl in failures.values():
             num_failures += len(fl)
 
         stats_body = ['']
         stats_body.append(f'Total number of test cases: {num_tests}')
         stats_body.append(f'Total number of failures: {num_failures}')
```

### Comparing `ReFrame-HPC-4.1.3/reframe/frontend/testgenerators.py` & `ReFrame-HPC-4.2.0/reframe/frontend/testgenerators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/schemas/config.json` & `ReFrame-HPC-4.2.0/reframe/schemas/config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994283693415638%*

 * *Differences: {"'defaults'": "{'logging/handlers*/httpjson_extra_headers': OrderedDict()}",*

 * * "'defs'": "{'httpjson_handler': {'allOf': {1: {'properties': {'extra_headers': "*

 * *           "OrderedDict([('type', 'object')])}}}}}"}*

```diff
@@ -58,14 +58,15 @@
         "logging/handlers*/file_append": false,
         "logging/handlers*/file_name": "",
         "logging/handlers*/file_timestamp": false,
         "logging/handlers*/filelog_append": true,
         "logging/handlers*/filelog_basedir": "./perflogs",
         "logging/handlers*/graylog_extras": {},
         "logging/handlers*/httpjson_debug": false,
+        "logging/handlers*/httpjson_extra_headers": {},
         "logging/handlers*/httpjson_extras": {},
         "logging/handlers*/httpjson_ignore_keys": [],
         "logging/handlers*/httpjson_json_formatter": null,
         "logging/handlers*/stream_name": "stdout",
         "logging/handlers*/syslog_facility": "user",
         "logging/handlers*/syslog_socktype": "udp",
         "logging/handlers_perflog": [],
@@ -261,14 +262,17 @@
                     "$ref": "#/defs/handler_common"
                 },
                 {
                     "properties": {
                         "debug": {
                             "type": "boolean"
                         },
+                        "extra_headers": {
+                            "type": "object"
+                        },
                         "extras": {
                             "type": "object"
                         },
                         "ignore_keys": {
                             "items": {
                                 "type": "string"
                             },
```

### Comparing `ReFrame-HPC-4.1.3/reframe/schemas/junit.xsd` & `ReFrame-HPC-4.2.0/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/schemas/runreport.json` & `ReFrame-HPC-4.2.0/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/__init__.py` & `ReFrame-HPC-4.2.0/reframe/utility/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,24 @@
     spec.loader.exec_module(module)
     return module
 
 
 def import_module_from_file(filename, force=False):
     '''Import module from file.
 
+    If the file location refers to a directory, the contained ``__init__.py``
+    will be loaded. If the filename resolves to a location that is within the
+    current working directory, a module name will be derived from the supplied
+    file name and Python's :func:`importlib.import_module` will be invoked to
+    actually load the module. If the file location refers to a path outside
+    the current working directory, then the module will be loaded directly
+    from the file, but it will be assigned a mangled name in
+    :obj:`sys.modules`, to avoid clashes with other modules loaded using the
+    standard import mechanism.
+
     :arg filename: The path to the filename of a Python module.
     :arg force: Force reload of module in case it is already loaded.
     :returns: The loaded Python module.
     '''
 
     # Expand and sanitize filename
     filename = os.path.abspath(os.path.expandvars(filename))
@@ -105,14 +115,62 @@
 
     if force:
         sys.modules.pop(module_name, None)
 
     return importlib.import_module(module_name)
 
 
+def import_module(module_name, force=False):
+    '''Import a module.
+
+    This will not invoke directly the Python import mechanism. It will first
+    derive a path from the module name and will then call
+    :func:`import_module_from_file`.
+
+    :arg module_name: The name of the module to load.
+    :arg force: Force reload of module in case it is already loaded.
+    :returns: The loaded Python module.
+
+    .. versionadded:: 4.2
+    '''
+
+    # Calculate the number of levels that we need to go up
+    for num_dots, c in enumerate(module_name):
+        if c != '.':
+            break
+
+    if num_dots:
+        prefix = './'
+        for i in range(num_dots-1):
+            prefix += '../'
+    else:
+        prefix = ''
+
+    path = prefix + module_name.lstrip('.').replace('.', '/')
+    if os.path.isdir(path):
+        path += '/__init__.py'
+    else:
+        path += '.py'
+
+    return import_module_from_file(path, force)
+
+
+def import_from_module(module_name, symbol):
+    '''Import a symbol from module.
+
+    :arg module_name: The name of the module from which to import the symbol.
+    :arg symbol: The symbol to import.
+    :returns: The value of the requested symbol.
+
+    .. versionadded:: 4.2
+    '''
+
+    return getattr(import_module(module_name), symbol)
+
+
 def allx(iterable):
     '''Same as the built-in :py:func:`all`, except that it returns
     :class:`False` if ``iterable`` is empty.
     '''
 
     # Generators must be treated specially, because there is no way to get
     # their size without consuming their elements.
```

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/color.py` & `ReFrame-HPC-4.2.0/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/cpuinfo.py` & `ReFrame-HPC-4.2.0/reframe/utility/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/jsonext.py` & `ReFrame-HPC-4.2.0/reframe/utility/jsonext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/osext.py` & `ReFrame-HPC-4.2.0/reframe/utility/osext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/profile.py` & `ReFrame-HPC-4.2.0/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/sanity.py` & `ReFrame-HPC-4.2.0/reframe/utility/sanity.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/typecheck.py` & `ReFrame-HPC-4.2.0/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/udeps.py` & `ReFrame-HPC-4.2.0/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/reframe/utility/versioning.py` & `ReFrame-HPC-4.2.0/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.1.3/setup.cfg` & `ReFrame-HPC-4.2.0/setup.cfg`

 * *Files identical despite different names*

