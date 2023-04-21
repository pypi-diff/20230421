# Comparing `tmp/jaxsim-0.1.dev135.tar.gz` & `tmp/jaxsim-0.1.dev137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev135.tar", last modified: Fri Apr 21 08:24:38 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev137.tar", last modified: Fri Apr 21 08:29:59 2023, max compression
```

## Comparing `jaxsim-0.1.dev135.tar` & `jaxsim-0.1.dev137.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.307442 jaxsim-0.1.dev135/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    33921 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18797 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.315442 jaxsim-0.1.dev135/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-21 08:24:21.000000 jaxsim-0.1.dev135/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:24:38.311442 jaxsim-0.1.dev135/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 08:24:38.000000 jaxsim-0.1.dev135/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33908 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/top_level.txt
```

### Comparing `jaxsim-0.1.dev135/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev137/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev135/.github/workflows/style.yml` & `jaxsim-0.1.dev137/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev135/.gitignore` & `jaxsim-0.1.dev137/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev135/LICENSE` & `jaxsim-0.1.dev137/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev135/PKG-INFO` & `jaxsim-0.1.dev137/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev135
+Version: 0.1.dev137
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev135/README.md` & `jaxsim-0.1.dev137/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev135/setup.cfg` & `jaxsim-0.1.dev137/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev135/src/jaxsim/__init__.py` & `jaxsim-0.1.dev137/src/jaxsim/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from . import logging
 
 
 # Follow upstream development in https://github.com/google/jax/pull/13304
 def _jnp_options() -> None:
-
     import os
 
     from jax.config import config
 
     # Enable by default
     if not ("JAX_ENABLE_X64" in os.environ and os.environ["JAX_ENABLE_X64"] == "0"):
         logging.info("Enabling JAX to use 64bit precision")
@@ -17,22 +16,20 @@
         import numpy as np
 
         if jnp.empty(0, dtype=float).dtype != jnp.empty(0, dtype=np.float64).dtype:
             logging.warning("Failed to enable 64bit precision in JAX")
 
 
 def _np_options() -> None:
-
     import numpy as np
 
     np.set_printoptions(precision=5, suppress=True, linewidth=150, threshold=10_000)
 
 
 def _is_editable() -> bool:
-
     import importlib.util
     import pathlib
     import site
 
     # Get the ModuleSpec of jaxsim
     jaxsim_spec = importlib.util.find_spec(name="jaxsim")
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev137/src/jaxsim/high_level/joint.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,74 +6,60 @@
 import jaxsim.parsers.descriptions as descriptions
 import jaxsim.typing as jtp
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class Joint(JaxsimDataclass):
-
     joint_description: descriptions.JointDescription = jax_dataclasses.static_field()
     parent_model: "jaxsim.high_level.model.Model" = jax_dataclasses.field(
         default=None, repr=False, compare=False
     )
 
     def valid(self) -> bool:
-
         return self.parent_model is not None
 
     def index(self) -> int:
-
         return self.joint_description.index
 
     def dofs(self) -> int:
-
         return 1
 
     def name(self) -> str:
-
         return self.joint_description.name
 
     def position(self, dof: int = 0) -> float:
-
         return self.parent_model.joint_positions(joint_names=[self.name()])[dof]
 
     def velocity(self, dof: int = 0) -> float:
-
         return self.parent_model.joint_velocities(joint_names=[self.name()])[dof]
 
     def acceleration(self, dof: int = 0) -> float:
-
         return self.parent_model.joint_accelerations(joint_names=[self.name()])[dof]
 
     def force(self, dof: int = 0) -> float:
-
         return self.parent_model.joint_generalized_forces(joint_names=[self.name()])[
             dof
         ]
 
     def position_limit(self, dof: int = 0) -> Tuple[float, float]:
-
         if dof != 0:
             msg = "Only joints with 1 DoF are currently supported"
             raise ValueError(msg)
 
         return self.joint_description.position_limit
 
     # =================
     # Multi-DoF methods
     # =================
 
     def joint_position(self) -> jtp.Vector:
-
         return self.parent_model.joint_positions(joint_names=[self.name()])
 
     def joint_velocity(self) -> jtp.Vector:
-
         return self.parent_model.joint_velocities(joint_names=[self.name()])
 
     def joint_acceleration(self) -> jtp.Vector:
-
         return self.parent_model.joint_accelerations(joint_names=[self.name()])
 
     def joint_force(self) -> jtp.Vector:
-
         return self.parent_model.joint_generalized_forces(joint_names=[self.name()])
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev137/src/jaxsim/high_level/link.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,50 +10,43 @@
 from jaxsim.utils import JaxsimDataclass
 
 from .common import VelRepr
 
 
 @jax_dataclasses.pytree_dataclass
 class Link(JaxsimDataclass):
-
     link_description: descriptions.LinkDescription = jax_dataclasses.static_field()
     parent_model: "jaxsim.high_level.model.Model" = jax_dataclasses.field(
         default=None, repr=False, compare=False
     )
 
     def valid(self) -> bool:
-
         return self.parent_model is not None
 
     # ==========
     # Properties
     # ==========
 
     def name(self) -> str:
-
         return self.link_description.name
 
     def index(self) -> int:
-
         return self.link_description.index
 
     # ========
     # Dynamics
     # ========
 
     def mass(self) -> jtp.Float:
-
         return self.link_description.mass
 
     def spatial_inertia(self) -> jtp.Matrix:
-
         return self.link_description.inertia
 
     def com_position(self, in_link_frame: bool = True) -> jtp.VectorJax:
-
         from jaxsim.math.inertia import Inertia
 
         _, L_p_CoM, _ = Inertia.to_params(M=self.spatial_inertia())
 
         if in_link_frame:
             return L_p_CoM.squeeze()
 
@@ -63,72 +56,62 @@
         return W_ph_CoM[0:3].squeeze()
 
     # ==========
     # Kinematics
     # ==========
 
     def position(self) -> jtp.Vector:
-
         return self.transform()[0:3, 3]
 
     def orientation(self, dcm: bool = False) -> jtp.Vector:
-
         R = self.transform()[0:3, 0:3]
 
         to_wxyz = np.array([3, 0, 1, 2])
         return R if dcm else sixd.so3.SO3.from_matrix(R).as_quaternion_xyzw()[to_wxyz]
 
     def transform(self) -> jtp.Matrix:
-
         return self.parent_model.forward_kinematics()[self.index()]
 
     def velocity(self, vel_repr: VelRepr = None) -> jtp.Vector:
-
         v_WL = (
             self.jacobian(output_vel_repr=vel_repr)
             @ self.parent_model.generalized_velocity()
         )
         return v_WL
 
     def linear_velocity(self, vel_repr: VelRepr = None) -> jtp.Vector:
-
         return self.velocity(vel_repr=vel_repr)[0:3]
 
     def angular_velocity(self, vel_repr: VelRepr = None) -> jtp.Vector:
-
         return self.velocity(vel_repr=vel_repr)[3:6]
 
     def jacobian(self, output_vel_repr: VelRepr = None) -> jtp.Matrix:
-
         if output_vel_repr is None:
             output_vel_repr = self.parent_model.velocity_representation
 
         # Return the doubly left-trivialized free-floating jacobian
         L_J_WL_B = jacobian(
             model=self.parent_model.physics_model,
             body_index=self.index(),
             q=self.parent_model.data.model_state.joint_positions,
         )
 
         if self.parent_model.velocity_representation is VelRepr.Body:
-
             L_J_WL_target = L_J_WL_B
 
         elif self.parent_model.velocity_representation is VelRepr.Inertial:
-
             dofs = self.parent_model.dofs()
             W_H_B = self.parent_model.base_transform()
 
             B_X_W = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint()
             zero_6n = jnp.zeros(shape=(6, dofs))
             B_T_W = jnp.block([[B_X_W, zero_6n], [zero_6n.T, jnp.eye(dofs)]])
             L_J_WL_target = L_J_WL_B @ B_T_W
 
         elif self.parent_model.velocity_representation is VelRepr.Mixed:
-
             dofs = self.parent_model.dofs()
             W_H_B = self.parent_model.base_transform()
             BW_H_B = jnp.array(W_H_B).at[0:3, 3].set(jnp.zeros(3))
 
             B_X_BW = sixd.se3.SE3.from_matrix(BW_H_B).inverse().adjoint()
             zero_6n = jnp.zeros(shape=(6, dofs))
             B_T_BW = jnp.block([[B_X_BW, zero_6n], [zero_6n.T, jnp.eye(dofs)]])
@@ -138,71 +121,64 @@
         else:
             raise ValueError(self.parent_model.velocity_representation)
 
         if output_vel_repr is VelRepr.Body:
             return L_J_WL_target
 
         elif output_vel_repr is VelRepr.Inertial:
-
             W_H_L = self.transform()
             W_X_L = sixd.se3.SE3.from_matrix(W_H_L).adjoint()
             return W_X_L @ L_J_WL_target
 
         elif output_vel_repr is VelRepr.Mixed:
-
             W_H_L = self.transform()
             LW_H_L = jnp.array(W_H_L).at[0:3, 3].set(jnp.zeros(3))
             LW_X_L = sixd.se3.SE3.from_matrix(LW_H_L).adjoint()
             return LW_X_L @ L_J_WL_target
 
         else:
             raise ValueError(output_vel_repr)
 
     def external_force(self) -> jtp.Vector:
-
         W_f_ext = self.parent_model.data.model_input.f_ext[self.index()]
 
         if self.parent_model.velocity_representation is VelRepr.Inertial:
             return W_f_ext
 
         elif self.parent_model.velocity_representation is VelRepr.Body:
-
             W_H_B = self.parent_model.base_transform()
             W_X_B = sixd.se3.SE3.from_matrix(W_H_B).adjoint()
 
             return W_X_B.transpose() @ W_f_ext
 
         elif self.parent_model.velocity_representation is VelRepr.Mixed:
             raise NotImplementedError
 
         else:
             raise ValueError(self.parent_model.velocity_representation)
 
     def add_external_force(
         self, force: jtp.Array = None, torque: jtp.Array = None
     ) -> None:
-
         force = force if force is not None else jnp.zeros(3)
         torque = torque if torque is not None else jnp.zeros(3)
 
         f_ext = jnp.hstack([force, torque])
 
         if self.parent_model.velocity_representation is VelRepr.Inertial:
             W_f_ext = f_ext
 
         elif self.parent_model.velocity_representation is VelRepr.Body:
-
             L_f_ext = f_ext
             W_H_L = self.transform()
             L_X_W = sixd.se3.SE3.from_matrix(W_H_L).inverse().adjoint()
 
             W_f_ext = L_X_W.transpose() @ L_f_ext
 
         elif self.parent_model.velocity_representation is VelRepr.Mixed:
-
             LW_f_ext = f_ext
 
             W_p_L = self.transform()[0:3, 3]
             W_H_LW = jnp.eye(4).at[0:3, 3].set(W_p_L)
             LW_X_W = sixd.se3.SE3.from_matrix(W_H_LW).inverse().adjoint()
 
             W_f_ext = LW_X_W @ LW_f_ext
@@ -217,38 +193,34 @@
                 W_f_ext_current + W_f_ext
             )
         )
 
     def add_com_external_force(
         self, force: jtp.Array = None, torque: jtp.Array = None
     ) -> None:
-
         force = force if force is not None else jnp.zeros(3)
         torque = torque if torque is not None else jnp.zeros(3)
 
         f_ext = jnp.hstack([force, torque])
 
         if self.parent_model.velocity_representation is VelRepr.Inertial:
-
             W_f_ext = f_ext
 
         elif self.parent_model.velocity_representation is VelRepr.Body:
-
             GL_f_ext = f_ext
 
             W_H_L = self.transform()
             L_p_CoM = self.com_position(in_link_frame=True)
             L_H_GL = jnp.eye(4).at[0:3, 3].set(L_p_CoM)
             W_H_GL = W_H_L @ L_H_GL
             GL_X_W = sixd.se3.SE3.from_matrix(W_H_GL).inverse().adjoint()
 
             W_f_ext = GL_X_W.transpose() @ GL_f_ext
 
         elif self.parent_model.velocity_representation is VelRepr.Mixed:
-
             GW_f_ext = f_ext
 
             W_p_CoM = self.com_position(in_link_frame=False)
             W_H_GW = jnp.eye(4).at[0:3, 3].set(W_p_CoM)
             GW_X_W = sixd.se3.SE3.from_matrix(W_H_GW).inverse().adjoint()
 
             W_f_ext = GW_X_W.transpose() @ GW_f_ext
@@ -261,9 +233,8 @@
         self.parent_model.data.model_input.f_ext = (
             self.parent_model.data.model_input.f_ext.at[self.index(), :].set(
                 W_f_ext_current + W_f_ext
             )
         )
 
     def in_contact(self) -> jtp.Bool:
-
         return not jnp.allclose(self.external_force(), 0)
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev137/src/jaxsim/high_level/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 import pathlib
-from typing import Dict, List, Tuple, Union, Any
+from typing import Any, Dict, List, Tuple, Union
 
 import jax.experimental.ode
 import jax.numpy as jnp
 import jax_dataclasses
 import numpy as np
 
 import jaxsim
@@ -23,22 +23,20 @@
 from jaxsim.utils import JaxsimDataclass, Mutability
 
 from .common import VelRepr
 
 
 @jax_dataclasses.pytree_dataclass
 class ModelData(JaxsimDataclass):
-
     model_state: jaxsim.physics.model.physics_model_state.PhysicsModelState
     model_input: jaxsim.physics.model.physics_model_state.PhysicsModelInput
     contact_state: jaxsim.physics.algos.soft_contacts.SoftContactsState
 
     @staticmethod
     def zero(physics_model: physics.model.physics_model.PhysicsModel) -> "ModelData":
-
         return ModelData(
             model_state=jaxsim.physics.model.physics_model_state.PhysicsModelState.zero(
                 physics_model=physics_model
             ),
             model_input=jaxsim.physics.model.physics_model_state.PhysicsModelInput.zero(
                 physics_model=physics_model
             ),
@@ -46,15 +44,14 @@
                 physics_model=physics_model
             ),
         )
 
 
 @jax_dataclasses.pytree_dataclass
 class StepData(JaxsimDataclass):
-
     t0: float
     tf: float
     dt: float
 
     # Starting model data and real input (tau, f_ext) computed at t0
     t0_model_data: ModelData = dataclasses.field(repr=False)
     t0_model_input_real: jaxsim.physics.model.physics_model_state.PhysicsModelInput = (
@@ -73,17 +70,17 @@
     )
     tf_contact_state: jaxsim.physics.algos.soft_contacts.SoftContactsState = (
         dataclasses.field(repr=False)
     )
 
     aux: Dict[str, Any] = dataclasses.field(default_factory=dict)
 
+
 @jax_dataclasses.pytree_dataclass
 class Model(JaxsimDataclass):
-
     model_name: str = jax_dataclasses.static_field()
     physics_model: physics.model.physics_model.PhysicsModel = dataclasses.field(
         repr=False
     )
 
     velocity_representation: VelRepr = jax_dataclasses.static_field(
         default=VelRepr.Mixed
@@ -107,15 +104,14 @@
         sdf: Union[str, pathlib.Path],
         model_name: str = None,
         vel_repr: VelRepr = VelRepr.Mixed,
         gravity: jtp.Array = jaxsim.physics.default_gravity(),
         is_urdf: bool = False,
         considered_joints: List[str] = None,
     ) -> "Model":
-
         import jaxsim.parsers.sdf
 
         if is_urdf:
             raise ValueError("Converting URDF to SDF is not yet supported")
 
         model_description = jaxsim.parsers.sdf.build_model_from_sdf(sdf=sdf)
 
@@ -136,15 +132,14 @@
 
     @staticmethod
     def build(
         physics_model: jaxsim.physics.model.physics_model.PhysicsModel,
         model_name: str = None,
         vel_repr: VelRepr = VelRepr.Mixed,
     ) -> "Model":
-
         model_name = (
             model_name if model_name is not None else physics_model.description.name
         )
 
         sorted_links = {
             l.name: high_level.link.Link(link_description=l)
             for l in sorted(
@@ -173,15 +168,14 @@
 
         if not model.valid():
             raise RuntimeError
 
         return model
 
     def __post_init__(self):
-
         original_mutability = self._mutability()
         self._set_mutability(Mutability.MUTABLE_NO_VALIDATION)
 
         for l in self._links.values():
             l.mutable(validate=False).parent_model = self
 
         for j in self._joints.values():
@@ -194,15 +188,14 @@
         self._joints: Dict[str, high_level.joint.Joint] = {
             k: v for k, v in sorted(self._joints.items(), key=lambda kv: kv[1].index())
         }
 
         self._set_mutability(original_mutability)
 
     def reduce(self, considered_joints: List[str]) -> None:
-
         reduced_model_description = self.physics_model.description.reduce(
             considered_joints=considered_joints
         )
 
         physics_model = jaxsim.physics.model.physics_model.PhysicsModel.build_from(
             model_description=reduced_model_description,
             gravity=self.physics_model.gravity[0:3],
@@ -219,133 +212,114 @@
         self.physics_model = reduced_model.physics_model
         self.data = reduced_model.data
         self._links = reduced_model._links
         self._joints = reduced_model._joints
         self._set_mutability(original_mutability)
 
     def zero(self) -> None:
-
         self.data = ModelData.zero(physics_model=self.physics_model)
         self.data._set_mutability(self._mutability())
 
     def zero_input(self) -> None:
-
         self.data.model_input = ModelData.zero(
             physics_model=self.physics_model
         ).model_input
 
         self.data._set_mutability(self._mutability())
 
     def zero_state(self) -> None:
-
         model_data_zero = ModelData.zero(physics_model=self.physics_model)
         self.data.model_state = model_data_zero.model_state
         self.data.contact_state = model_data_zero.contact_state
 
         self.data._set_mutability(self._mutability())
 
     def set_velocity_representation(self, vel_repr: VelRepr) -> None:
-
         if self.velocity_representation is vel_repr:
             return
 
         self.velocity_representation = vel_repr
 
     # ==========
     # Properties
     # ==========
 
     def valid(self) -> bool:
-
         valid = True
         valid = valid and all([l.valid() for l in self.links()])
         valid = valid and all([j.valid() for j in self.joints()])
         return valid
 
     def floating_base(self) -> bool:
-
         return self.physics_model.is_floating_base
 
     def dofs(self) -> int:
-
         return self.physics_model.dofs()
 
     def name(self) -> str:
-
         return self.model_name
 
     def nr_of_links(self) -> int:
-
         return len(self._links)
 
     def nr_of_joints(self) -> int:
-
         return len(self._joints)
 
     def total_mass(self) -> jtp.Float:
-
         return jnp.sum(jnp.array([l.mass() for l in self.links()]))
 
     def get_link(self, link_name: str) -> high_level.link.Link:
-
         if link_name not in self.link_names():
             msg = f"Link '{link_name}' is not part of model '{self.name()}'"
             raise ValueError(msg)
 
         return self.links(link_names=[link_name])[0]
 
     def get_joint(self, joint_name: str) -> high_level.joint.Joint:
-
         if joint_name not in self.joint_names():
             msg = f"Joint '{joint_name}' is not part of model '{self.name()}'"
             raise ValueError(msg)
 
         return self.joints(joint_names=[joint_name])[0]
 
     def link_names(self) -> List[str]:
-
         return list(self._links.keys())
 
     def joint_names(self) -> List[str]:
-
         return list(self._joints.keys())
 
     def links(self, link_names: List[str] = None) -> List[high_level.link.Link]:
-
         if link_names is None:
             return list(self._links.values())
 
         return [self._links[name] for name in link_names]
 
     def joints(self, joint_names: List[str] = None) -> List[high_level.joint.Joint]:
-
         if joint_names is None:
             return list(self._joints.values())
 
         return [self._joints[name] for name in joint_names]
 
     # ==================
     # Vectorized methods
     # ==================
 
     def joint_positions(self, joint_names: List[str] = None) -> jtp.Vector:
-
         if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
             return jnp.array([])
 
         return self.data.model_state.joint_positions[
             self._joint_indices(joint_names=joint_names)
         ]
 
     def joint_random_positions(
         self,
         joint_names: List[str] = None,
         key: jax.random.PRNGKeyArray = jax.random.PRNGKey(seed=0),
     ) -> jtp.Vector:
-
         if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
             return jnp.array([])
 
         s_min, s_max = self.joint_limits(joint_names=joint_names)
 
         s_random = jax.random.uniform(
             minval=s_min,
@@ -353,26 +327,24 @@
             key=key,
             shape=s_min.shape,
         )
 
         return s_random
 
     def joint_velocities(self, joint_names: List[str] = None) -> jtp.Vector:
-
         if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
             return jnp.array([])
 
         return self.data.model_state.joint_velocities[
             self._joint_indices(joint_names=joint_names)
         ]
 
     def joint_limits(
         self, joint_names: List[str] = None
     ) -> Tuple[jtp.Vector, jtp.Vector]:
-
         if self.dofs() == 0 and (joint_names is None or len(joint_names) == 0):
             return jnp.array([])
 
         joint_names = joint_names if joint_names is not None else self.joint_names()
 
         s_min = jnp.array(
             [min(self.get_joint(name).position_limit()) for name in joint_names]
@@ -385,147 +357,132 @@
         return s_min, s_max
 
     # =========
     # Base link
     # =========
 
     def base_frame(self) -> str:
-
         return self.physics_model.description.root.name
 
     def base_position(self) -> jtp.Vector:
-
         return self.data.model_state.base_position.squeeze()
 
     def base_orientation(self, dcm: bool = False) -> jtp.Vector:
-
         to_xyzw = np.array([1, 2, 3, 0])
 
         return (
             self.data.model_state.base_quaternion
             if not dcm
             else sixd.so3.SO3.from_quaternion_xyzw(
                 self.data.model_state.base_quaternion[to_xyzw]
             ).as_matrix()
         )
 
     def base_transform(self) -> jtp.MatrixJax:
-
         return jnp.block(
             [
                 [self.base_orientation(dcm=True), jnp.vstack(self.base_position())],
                 [0, 0, 0, 1],
             ]
         )
 
     def base_velocity(self) -> jtp.Vector:
-
         W_v_WB = jnp.hstack(
             [
                 self.data.model_state.base_linear_velocity,
                 self.data.model_state.base_angular_velocity,
             ]
         )
 
         return self.inertial_to_active_representation(array=W_v_WB)
 
     def external_forces(self) -> jtp.Matrix:
-
         W_f_ext = self.data.model_input.f_ext
 
         inertial_to_active = lambda f: self.inertial_to_active_representation(
             f, is_force=True
         )
 
         return jax.vmap(inertial_to_active, in_axes=0)(W_f_ext)
 
     # ==================
     # Dynamic properties
     # ==================
 
     def generalized_position(self) -> Tuple[jtp.Matrix, jtp.Vector]:
-
         return self.base_transform(), self.joint_positions()
 
     def generalized_velocity(self) -> jtp.Vector:
-
         return jnp.hstack([self.base_velocity(), self.joint_velocities()])
 
     def generalized_jacobian(self, output_vel_repr: VelRepr = None) -> jtp.Matrix:
-
         return jnp.vstack(
             [
                 self.get_link(link_name=link_name).jacobian(
                     output_vel_repr=output_vel_repr
                 )
                 for link_name in self.link_names()
             ]
         )
 
     def free_floating_mass_matrix(self) -> jtp.Matrix:
-
         M_body = jaxsim.physics.algos.crba.crba(
             model=self.physics_model,
             q=self.data.model_state.joint_positions,
         )
 
         if self.velocity_representation is VelRepr.Body:
             return M_body
 
         elif self.velocity_representation is VelRepr.Inertial:
-
             zero_6n = jnp.zeros(shape=(6, self.dofs()))
             B_X_W = sixd.se3.SE3.from_matrix(self.base_transform()).inverse().adjoint()
 
             invT = jnp.block([[B_X_W, zero_6n], [zero_6n.T, jnp.eye(self.dofs())]])
 
             return invT.T @ M_body @ invT
 
         elif self.velocity_representation is VelRepr.Mixed:
-
             zero_6n = jnp.zeros(shape=(6, self.dofs()))
             W_H_BW = self.base_transform().at[0:3, 3].set(jnp.zeros(3))
             BW_X_W = sixd.se3.SE3.from_matrix(W_H_BW).inverse().adjoint()
 
             invT = jnp.block([[BW_X_W, zero_6n], [zero_6n.T, jnp.eye(self.dofs())]])
 
             return invT.T @ M_body @ invT
 
         else:
             raise ValueError(self.velocity_representation)
 
     def free_floating_generalized_forces(self) -> jtp.Vector:
-
         model_state = self.data.model_state
         model = self.copy().mutable(validate=True)
 
         model.zero()
         model.data.model_state.base_position = model_state.base_position
         model.data.model_state.base_quaternion = model_state.base_quaternion
         model.data.model_state.joint_positions = model_state.joint_positions
         model.data.model_state.base_linear_velocity = model_state.base_linear_velocity
         model.data.model_state.base_angular_velocity = model_state.base_angular_velocity
         model.data.model_state.joint_velocities = model_state.joint_velocities
 
         return jnp.hstack(model.inverse_dynamics())
 
     def free_floating_gravity_forces(self) -> jtp.Vector:
-
         model_state = self.data.model_state
         model = self.copy().mutable(validate=True)
 
         model.zero()
         model.data.model_state.base_position = model_state.base_position
         model.data.model_state.base_quaternion = model_state.base_quaternion
         model.data.model_state.joint_positions = model_state.joint_positions
 
         return jnp.hstack(model.inverse_dynamics())
 
     def momentum(self) -> jtp.Vector:
-
         with self.editable(validate=True) as m:
             m.set_velocity_representation(vel_repr=VelRepr.Body)
 
         # Compute the momentum in body-fixed velocity representation.
         # Note: the first 6 rows of the mass matrix define the jacobian of the
         #       floating-base momentum.
         B_h = m.free_floating_mass_matrix()[0:6, :] @ m.generalized_velocity()
@@ -537,15 +494,14 @@
         return self.inertial_to_active_representation(array=W_h, is_force=True)
 
     # ==============================
     # Quantities related to the CoM
     # ==============================
 
     def com_position(self) -> jtp.Vector:
-
         m = self.total_mass()
 
         W_H_L = self.forward_kinematics()
         W_H_B = self.base_transform()
         B_H_W = jnp.linalg.inv(W_H_B)
 
         com_links = [
@@ -558,29 +514,27 @@
         return (W_H_B @ B_ph_CoM)[0:3]
 
     # ==========
     # Algorithms
     # ==========
 
     def forward_kinematics(self) -> jtp.Array:
-
         W_H_i = jaxsim.physics.algos.forward_kinematics.forward_kinematics_model(
             model=self.physics_model,
             q=self.data.model_state.joint_positions,
             xfb=self.data.model_state.xfb(),
         )
 
         return W_H_i
 
     def inverse_dynamics(
         self,
         joint_accelerations: jtp.Vector = None,
         base_acceleration: jtp.Vector = jnp.zeros(6),
     ) -> Tuple[jtp.Vector, jtp.Vector]:
-
         if (
             self.velocity_representation is VelRepr.Mixed
             and self.floating_base()
             and not jnp.allclose(self.data.model_state.base_angular_velocity, 0)
         ):
             msg = "This method has to be fixed in Mixed representation"
             raise ValueError(msg)
@@ -619,25 +573,23 @@
         f_B = self.inertial_to_active_representation(array=W_f_B, is_force=True)
 
         return f_B, tau
 
     def forward_dynamics(
         self, tau: jtp.Vector = None, prefer_aba: float = True
     ) -> Tuple[jtp.Vector, jtp.Vector]:
-
         return (
             self.forward_dynamics_aba(tau=tau)
             if prefer_aba
             else self.forward_dynamics_crb(tau=tau)
         )
 
     def forward_dynamics_aba(
         self, tau: jtp.Vector = None
     ) -> Tuple[jtp.Vector, jtp.Vector]:
-
         if (
             self.velocity_representation is not VelRepr.Inertial
             and (self.data.model_input.f_ext != 0).any()
         ):
             msg1 = "This method has to be fixed for Body and Mixed representation, "
             msg2 = "use forward_dynamics_crb instead."
             raise ValueError(msg1 + msg2)
@@ -662,35 +614,32 @@
         a_WB = self.inertial_to_active_representation(array=W_a_WB)
 
         return a_WB, sdd
 
     def forward_dynamics_crb(
         self, tau: jtp.Vector = None
     ) -> Tuple[jtp.Vector, jtp.Vector]:
-
         # Build joint torques if not provided
         tau = tau if tau is not None else jnp.zeros_like(self.joint_positions())
         tau = jnp.atleast_1d(tau.squeeze())
         tau = jnp.vstack(tau) if tau.size > 0 else jnp.empty(shape=(0, 1))
 
         # Compute terms of the floating-base EoM
         M = self.free_floating_mass_matrix()
         h = jnp.vstack(self.free_floating_generalized_forces())
         J = self.generalized_jacobian()
         f_ext = jnp.vstack(self.external_forces().flatten())
         S = jnp.block([jnp.zeros(shape=(self.dofs(), 6)), jnp.eye(self.dofs())]).T
 
         if self.floating_base():
-
             nu_dot = jnp.linalg.inv(M) @ (S @ tau - h + J.T @ f_ext)
             sdd = nu_dot[6:]
             a_WB = nu_dot[0:6]
 
         else:
-
             hss = h[6:]
             Jss = J[:, 6:]
             Mss = M[6:, 6:]
 
             a_WB = jnp.zeros(6)
             sdd = jnp.linalg.inv(Mss) @ (tau - hss + Jss.T @ f_ext)
 
@@ -701,46 +650,42 @@
         return a_WB, sdd
 
     # ======
     # Energy
     # ======
 
     def mechanical_energy(self) -> jtp.Float:
-
         K = self.kinetic_energy()
         U = self.potential_energy()
 
         return K + U
 
     def kinetic_energy(self) -> jtp.Float:
-
         with self.editable(validate=True) as m:
             m.set_velocity_representation(vel_repr=VelRepr.Body)
 
         nu = m.generalized_velocity()
         M = m.free_floating_mass_matrix()
 
         return 0.5 * nu.T @ M @ nu
 
     def potential_energy(self) -> jtp.Float:
-
         m = self.total_mass()
         W_p_CoM = jnp.hstack([self.com_position(), 1])
         gravity = self.physics_model.gravity[3:6].squeeze()
 
         return -(m * jnp.hstack([gravity, 0]) @ W_p_CoM)
 
     # ===========
     # Set targets
     # ===========
 
     def set_joint_generalized_force_targets(
         self, forces: jtp.Vector, joint_names: List[str] = None
     ) -> None:
-
         if joint_names is None:
             joint_names = self.joint_names()
 
         if forces.size != len(joint_names):
             raise ValueError("Wrong arguments size", forces.size, len(joint_names))
 
         self.data.model_input.tau = self.data.model_input.tau.at[
@@ -750,15 +695,14 @@
     # ==========
     # Reset data
     # ==========
 
     def reset_joint_positions(
         self, positions: jtp.Vector, joint_names: List[str] = None
     ) -> None:
-
         if joint_names is None:
             joint_names = self.joint_names()
 
         if positions.size != len(joint_names):
             raise ValueError("Wrong arguments size", positions.size, len(joint_names))
 
         if positions.size == 0:
@@ -771,15 +715,14 @@
                 self._joint_indices(joint_names=joint_names)
             ].set(positions)
         )
 
     def reset_joint_velocities(
         self, velocities: jtp.Vector, joint_names: List[str] = None
     ) -> None:
-
         if joint_names is None:
             joint_names = self.joint_names()
 
         if velocities.size != len(joint_names):
             raise ValueError("Wrong arguments size", velocities.size, len(joint_names))
 
         if velocities.size == 0:
@@ -790,65 +733,58 @@
         self.data.model_state.joint_velocities = (
             self.data.model_state.joint_velocities.at[
                 self._joint_indices(joint_names=joint_names)
             ].set(velocities)
         )
 
     def reset_base_position(self, position: jtp.Vector) -> None:
-
         self.data.model_state.base_position = position
 
     def reset_base_orientation(self, orientation: jtp.Array, dcm: bool = False) -> None:
-
         if dcm:
             to_wxyz = np.array([3, 0, 1, 2])
             orientation_xyzw = sixd.so3.SO3.from_matrix(
                 orientation
             ).as_quaternion_xyzw()
             orientation = orientation_xyzw[to_wxyz]
 
         self.data.model_state.base_quaternion = orientation
 
     def reset_base_transform(self, transform: jtp.Matrix) -> None:
-
         if transform.shape != (4, 4):
             raise ValueError(transform.shape)
 
         self.reset_base_position(position=transform[0:3, 3])
         self.reset_base_orientation(orientation=transform[0:3, 0:3], dcm=True)
 
     def reset_base_velocity(self, base_velocity: jtp.VectorJax) -> None:
-
         if not self.physics_model.is_floating_base:
             msg = "Changing the base velocity of a fixed-based model is not allowed"
             raise RuntimeError(msg)
 
         # Remove extra dimensions
         base_velocity = base_velocity.squeeze()
 
         # Check for a valid shape
         if base_velocity.shape != (6,):
             raise ValueError(base_velocity.shape)
 
         # Convert, if needed, to the representation used internally (VelRepr.Inertial)
         if self.velocity_representation is VelRepr.Inertial:
-
             base_velocity_inertial = base_velocity
 
         elif self.velocity_representation is VelRepr.Body:
-
             w_X_b = sixd.se3.SE3.from_rotation_and_translation(
                 rotation=sixd.so3.SO3.from_matrix(self.base_orientation(dcm=True)),
                 translation=self.base_position(),
             ).adjoint()
 
             base_velocity_inertial = w_X_b @ base_velocity
 
         elif self.velocity_representation is VelRepr.Mixed:
-
             w_X_bw = sixd.se3.SE3.from_rotation_and_translation(
                 rotation=sixd.so3.SO3.identity(),
                 translation=self.base_position(),
             ).adjoint()
 
             base_velocity_inertial = w_X_bw @ base_velocity
 
@@ -868,15 +804,14 @@
         tf: jtp.Float,
         sub_steps: int = 1,
         integrator_type: IntegratorType = IntegratorType.EulerForward,
         terrain: soft_contacts.Terrain = soft_contacts.FlatTerrain(),
         contact_parameters: soft_contacts.SoftContactsParams = soft_contacts.SoftContactsParams(),
         clear_inputs: bool = False,
     ) -> StepData:
-
         x0 = ode_integration.ode.ode_data.ODEState(
             physics_model=self.data.model_state,
             soft_contacts=self.data.contact_state,
         )
 
         ode_input = ode_integration.ode.ode_data.ODEInput(
             physics_model=self.data.model_input
@@ -904,20 +839,25 @@
             num_sub_steps=sub_steps,
             terrain=terrain,
             return_aux=True,
         )
 
         # Get quantities at t0
         t0_model_data = self.data
-        t0_model_input = jax.tree_util.tree_map(lambda l: l[0], aux["ode_input"])
+        t0_model_input = jax.tree_util.tree_map(
+            lambda l: l[0],
+            aux["ode_input"],
+        )
         t0_model_input_real = jax.tree_util.tree_map(
-            lambda l: l[0], aux["ode_input_real"]
+            lambda l: l[0],
+            aux["ode_input_real"],
         )
         t0_model_acceleration = jax.tree_util.tree_map(
-            lambda l: l[0], aux["model_acceleration"]
+            lambda l: l[0],
+            aux["model_acceleration"],
         )
 
         # Get quantities at tf
         ode_states: ode_data.ODEState
         tf_model_state = jax.tree_util.tree_map(
             lambda l: l[-1], ode_states.physics_model
         )
@@ -967,40 +907,36 @@
     # ===============
     # Private methods
     # ===============
 
     def inertial_to_active_representation(
         self, array: jtp.Array, is_force: bool = False
     ) -> jtp.Array:
-
         W_array = array.squeeze()
 
         if W_array.size != 6:
             raise ValueError(W_array.size)
 
         if self.velocity_representation is VelRepr.Inertial:
-
             return W_array
 
         elif self.velocity_representation is VelRepr.Body:
-
             W_H_B = self.base_transform()
 
             if not is_force:
                 B_X_W: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint()
                 B_array = B_X_W @ W_array
 
             else:
                 W_X_B: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).adjoint()
                 B_array = W_X_B.T @ W_array
 
             return B_array
 
         elif self.velocity_representation is VelRepr.Mixed:
-
             W_H_BW = jnp.eye(4).at[0:3, 3].set(self.base_position())
 
             if not is_force:
                 BW_X_W = sixd.se3.SE3.from_matrix(W_H_BW).inverse().adjoint()
                 BW_array = BW_X_W @ W_array
 
             else:
@@ -1011,42 +947,38 @@
 
         else:
             raise ValueError(self.velocity_representation)
 
     def active_to_inertial_representation(
         self, array: jtp.Array, is_force: bool = False
     ) -> jtp.Array:
-
         array = array.squeeze()
 
         if array.size != 6:
             raise ValueError(array.size)
 
         if self.velocity_representation is VelRepr.Inertial:
-
             W_array = array
             return W_array
 
         elif self.velocity_representation is VelRepr.Body:
-
             B_array = array
             W_H_B = self.base_transform()
 
             if not is_force:
                 W_X_B: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).adjoint()
                 W_array = W_X_B @ B_array
 
             else:
                 B_X_W: jtp.Array = sixd.se3.SE3.from_matrix(W_H_B).inverse().adjoint()
                 W_array = B_X_W.T @ B_array
 
             return W_array
 
         elif self.velocity_representation is VelRepr.Mixed:
-
             BW_array = array
             W_H_BW = jnp.eye(4).at[0:3, 3].set(self.base_position())
 
             if not is_force:
                 W_X_BW: jtp.Array = sixd.se3.SE3.from_matrix(W_H_BW).adjoint()
                 W_array = W_X_BW @ BW_array
 
@@ -1056,15 +988,14 @@
 
             return W_array
 
         else:
             raise ValueError(self.velocity_representation)
 
     def _joint_indices(self, joint_names: List[str] = None) -> jtp.Vector:
-
         if joint_names is None:
             joint_names = self.joint_names()
 
         if set(joint_names) - set(self._joints.keys()) != set():
             raise ValueError("One or more joint names are not part of the model")
 
         # Note: joints share the same index as their child link, therefore the first
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/logging.py` & `jaxsim-0.1.dev137/src/jaxsim/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,44 +4,39 @@
 
 import coloredlogs
 
 LOGGER_NAME = "jaxsim"
 
 
 class LoggingLevel(enum.IntEnum):
-
     NOTSET = logging.NOTSET
     DEBUG = logging.DEBUG
     INFO = logging.INFO
     WARNING = logging.WARNING
     ERROR = logging.ERROR
     CRITICAL = logging.CRITICAL
 
 
 def _logger() -> logging.Logger:
-
     return logging.getLogger(name=LOGGER_NAME)
 
 
 def set_logging_level(level: Union[int, LoggingLevel] = LoggingLevel.WARNING):
-
     if isinstance(level, int):
         level = LoggingLevel(level)
 
     _logger().setLevel(level=level.value)
 
 
 def get_logging_level() -> LoggingLevel:
-
     level = _logger().getEffectiveLevel()
     return LoggingLevel(level)
 
 
 def configure(level: LoggingLevel = LoggingLevel.WARNING) -> None:
-
     info("Configuring the 'jaxsim' logger")
 
     handler = logging.StreamHandler()
     fmt = "%(name)s[%(process)d] %(levelname)s %(message)s"
     handler.setFormatter(fmt=coloredlogs.ColoredFormatter(fmt=fmt))
     _logger().addHandler(hdlr=handler)
 
@@ -49,34 +44,28 @@
     # (preventing duplicate logging)
     _logger().propagate = False
 
     set_logging_level(level=level)
 
 
 def debug(msg: str = "") -> None:
-
     _logger().debug(msg=msg)
 
 
 def info(msg: str = "") -> None:
-
     _logger().info(msg=msg)
 
 
 def warning(msg: str = "") -> None:
-
     _logger().warning(msg=msg)
 
 
 def error(msg: str = "") -> None:
-
     _logger().error(msg=msg)
 
 
 def critical(msg: str = "") -> None:
-
     _logger().critical(msg=msg)
 
 
 def exception(msg: str = "") -> None:
-
     _logger().exception(msg=msg)
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev137/src/jaxsim/math/adjoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     @staticmethod
     def from_quaternion_and_translation(
         quaternion: jtp.Vector = jnp.array([1.0, 0, 0, 0]),
         translation: jtp.Vector = jnp.zeros(3),
         inverse: bool = False,
         normalize_quaternion: bool = False,
     ) -> jtp.Matrix:
-
         assert quaternion.size == 4
         assert translation.size == 3
 
         Q_sixd = so3.SO3.from_quaternion_xyzw(xyzw=Quaternion.to_xyzw(quaternion))
         Q_sixd = Q_sixd if not normalize_quaternion else Q_sixd.normalize()
 
         return Adjoint.from_rotation_and_translation(
@@ -28,15 +27,14 @@
 
     @staticmethod
     def from_rotation_and_translation(
         rotation: jtp.Matrix = jnp.eye(3),
         translation: jtp.Vector = jnp.zeros(3),
         inverse: bool = False,
     ) -> jtp.Matrix:
-
         assert rotation.shape == (3, 3)
         assert translation.size == 3
 
         A_R_B = rotation.squeeze()
         A_o_B = translation.squeeze()
 
         if not inverse:
@@ -54,15 +52,14 @@
                 ]
             )
 
         return X
 
     @staticmethod
     def to_transform(adjoint: jtp.Matrix) -> jtp.Matrix:
-
         X = adjoint.squeeze()
         assert X.shape == (6, 6)
 
         R = X[0:3, 0:3]
         o_x_R = X[0:3, 3:6]
 
         H = jnp.block(
@@ -72,15 +69,14 @@
             ]
         )
 
         return H
 
     @staticmethod
     def inverse(adjoint: jtp.Matrix) -> jtp.Matrix:
-
         A_X_B = adjoint
         A_H_B = Adjoint.to_transform(adjoint=A_X_B)
 
         A_R_B = A_H_B[0:3, 0:3]
         A_o_B = A_H_B[0:3, 3]
 
         return Adjoint.from_rotation_and_translation(
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev137/src/jaxsim/math/conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from .skew import Skew
 
 
 class Convert:
     @staticmethod
     def coordinates_tf(X: jtp.Matrix, p: jtp.Matrix) -> jtp.Matrix:
-
         X = X.squeeze()
         p = p.squeeze()
 
         # If p has shape (X,), transform it to column vector
         p = jnp.vstack(p) if len(p.shape) == 1 else p
         rows_p, cols_p = p.shape
 
@@ -28,15 +27,14 @@
         assert r.shape == p.shape, (r.shape, p.shape)
 
         xp = R @ (p - r)
         return jnp.vstack(xp)
 
     @staticmethod
     def velocities_threed(v_6d: jtp.Matrix, p: jtp.Matrix) -> jtp.Matrix:
-
         v = v_6d.squeeze()
         p = p.squeeze()
 
         # If the arrays have shape (X,), transform them to column vectors
         v = jnp.vstack(v) if len(v.shape) == 1 else v
         p = jnp.vstack(p) if len(p.shape) == 1 else p
 
@@ -51,15 +49,14 @@
         else:
             raise ValueError(v.shape)
 
         return jnp.vstack(vp)
 
     @staticmethod
     def forces_sixd(f_3d: jtp.Matrix, p: jtp.Matrix) -> jtp.Matrix:
-
         f = f_3d.squeeze()
         p = p.squeeze()
 
         # If the arrays have shape (X,), transform them to column vectors
         fp = jnp.vstack(f) if len(f.shape) == 1 else f
         p = jnp.vstack(p) if len(p.shape) == 1 else p
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev137/src/jaxsim/math/cross.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 
 from .skew import Skew
 
 
 class Cross:
     @staticmethod
     def vx(velocity_sixd: jtp.Vector) -> jtp.Matrix:
-
         v, ω = jnp.split(velocity_sixd.squeeze(), 2)
 
         v_cross = jnp.block(
             [
                 [Skew.wedge(vector=ω), Skew.wedge(vector=v)],
                 [jnp.zeros(shape=(3, 3)), Skew.wedge(vector=ω)],
             ]
         )
 
         return v_cross
 
     @staticmethod
     def vx_star(velocity_sixd: jtp.Vector) -> jtp.Matrix:
-
         v_cross_star = -Cross.vx(velocity_sixd).T
         return v_cross_star
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev137/src/jaxsim/math/inertia.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from .skew import Skew
 
 
 class Inertia:
     @staticmethod
     def to_sixd(mass: jtp.Float, com: jtp.Vector, I: jtp.Matrix) -> jtp.Matrix:
-
         if I.shape != (3, 3):
             raise ValueError(I, I.shape)
 
         c = Skew.wedge(vector=com)
 
         M = jnp.block(
             [
@@ -23,15 +22,14 @@
             ]
         )
 
         return M
 
     @staticmethod
     def to_params(M: jtp.Matrix) -> Tuple[jtp.Float, jtp.Vector, jtp.Matrix]:
-
         m = jnp.diag(M[0:3, 0:3]).sum() / 3
 
         mC = M[3:6, 0:3]
         c = Skew.vee(mC) / m
         I = M[3:6, 3:6] - (mC @ mC.T / m)
 
         return m, c, I
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev137/src/jaxsim/math/joint.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,87 +8,78 @@
 from .adjoint import Adjoint
 from .rotation import Rotation
 
 
 def jcalc(
     jtyp: Union[JointType, JointDescriptor], q: jtp.Float
 ) -> Tuple[jtp.Matrix, jtp.Vector]:
-
     if isinstance(jtyp, JointType):
         code = jtyp
     elif isinstance(jtyp, JointDescriptor):
         code = jtyp.code
     else:
         raise ValueError(jtyp)
 
     if code is JointType.F:
         raise ValueError("Fixed joints shouldn't be here")
 
     elif code is JointType.R:
-
         jtyp: JointGenericAxis
 
         Xj = Adjoint.from_rotation_and_translation(
             rotation=Rotation.from_axis_angle(vector=(q * jtyp.axis)), inverse=True
         )
 
         S = jnp.vstack(jnp.hstack([jnp.zeros(3), jtyp.axis.squeeze()]))
 
     elif code is JointType.P:
-
         jtyp: JointGenericAxis
 
         Xj = Adjoint.from_rotation_and_translation(
             translation=jnp.array(q * jtyp.axis), inverse=True
         )
 
         S = jnp.vstack(jnp.hstack([jtyp.axis.squeeze(), jnp.zeros(3)]))
 
     elif code is JointType.Rx:
-
         Xj = Adjoint.from_rotation_and_translation(
             rotation=Rotation.x(theta=q), inverse=True
         )
 
         S = jnp.vstack([0, 0, 0, 1.0, 0, 0])
 
     elif code is JointType.Ry:
-
         Xj = Adjoint.from_rotation_and_translation(
             rotation=Rotation.y(theta=q), inverse=True
         )
 
         S = jnp.vstack([0, 0, 0, 0, 1.0, 0])
 
     elif code is JointType.Rz:
-
         Xj = Adjoint.from_rotation_and_translation(
             rotation=Rotation.z(theta=q), inverse=True
         )
 
         S = jnp.vstack([0, 0, 0, 0, 0, 1.0])
 
     elif code is JointType.Px:
-
         Xj = Adjoint.from_rotation_and_translation(
             translation=jnp.array([q, 0.0, 0.0]), inverse=True
         )
 
         S = jnp.vstack([1.0, 0, 0, 0, 0, 0])
 
     elif code is JointType.Py:
-
         Xj = Adjoint.from_rotation_and_translation(
             translation=jnp.array([0.0, q, 0.0]), inverse=True
         )
 
         S = jnp.vstack([0, 1.0, 0, 0, 0, 0])
 
     elif code is JointType.Pz:
-
         Xj = Adjoint.from_rotation_and_translation(
             translation=jnp.array([0.0, 0.0, q]), inverse=True
         )
 
         S = jnp.vstack([0, 0, 1.0, 0, 0, 0])
 
     else:
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev137/src/jaxsim/math/plucker.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,39 +6,36 @@
 
 from .skew import Skew
 
 
 class Plucker:
     @staticmethod
     def from_rot_and_trans(dcm: jtp.Matrix, translation: jtp.Vector) -> jtp.Matrix:
-
         R = dcm
 
         X = jnp.block(
             [
                 [R, -R @ Skew.wedge(vector=translation)],
                 [jnp.zeros(shape=(3, 3)), R],
             ]
         )
 
         return X
 
     @staticmethod
     def to_rot_and_trans(adjoint: jtp.Matrix) -> Tuple[jtp.Matrix, jtp.Vector]:
-
         X = adjoint
 
         R = X[0:3, 0:3]
         p = -Skew.vee(R.T @ X[0:3, 3:6])
 
         return R, p
 
     @staticmethod
     def from_transform(transform: jtp.Matrix) -> jtp.Matrix:
-
         H = transform
 
         R = H[0:3, 0:3]
         p = H[0:3, 3]
 
         X = jnp.block(
             [
@@ -47,15 +44,14 @@
             ]
         )
 
         return X
 
     @staticmethod
     def to_transform(adjoint: jtp.Matrix) -> jtp.Matrix:
-
         X = adjoint
 
         R = X[0:3, 0:3]
         o_x_R = X[0:3, 3:6]
 
         H = jnp.vstack(
             [
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev137/src/jaxsim/math/quaternion.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,62 +4,55 @@
 import jaxsim.typing as jtp
 from jaxsim.sixd import so3
 
 
 class Quaternion:
     @staticmethod
     def to_xyzw(wxyz: jtp.Vector) -> jtp.Vector:
-
         return wxyz.squeeze()[jnp.array([1, 2, 3, 0])]
 
     @staticmethod
     def to_wxyz(xyzw: jtp.Vector) -> jtp.Vector:
-
         return xyzw.squeeze()[jnp.array([3, 0, 1, 2])]
 
     @staticmethod
     def to_dcm(quaternion: jtp.Vector) -> jtp.Matrix:
-
         return so3.SO3.from_quaternion_xyzw(
             xyzw=Quaternion.to_xyzw(quaternion)
         ).as_matrix()
 
     @staticmethod
     def from_dcm(dcm: jtp.Matrix) -> jtp.Vector:
-
         return Quaternion.to_wxyz(
             xyzw=so3.SO3.from_matrix(matrix=dcm).as_quaternion_xyzw()
         )
 
     @staticmethod
     def derivative(
         quaternion: jtp.Vector,
         omega: jtp.Vector,
         omega_in_body_fixed: bool = False,
         K: float = 0.1,
     ) -> jtp.Vector:
-
         w = omega.squeeze()
         quaternion = quaternion.squeeze()
 
         def Q_body(q: jtp.Vector) -> jtp.Matrix:
-
             qw, qx, qy, qz = q
 
             return jnp.array(
                 [
                     [qw, -qx, -qy, -qz],
                     [qx, qw, -qz, qy],
                     [qy, qz, qw, -qx],
                     [qz, -qy, qx, qw],
                 ]
             )
 
         def Q_inertial(q: jtp.Vector) -> jtp.Matrix:
-
             qw, qx, qy, qz = q
 
             return jnp.array(
                 [
                     [qw, -qx, -qy, -qz],
                     [qx, qw, qz, -qy],
                     [qy, -qz, qw, qx],
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev137/src/jaxsim/math/rotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,30 @@
 
 from .skew import Skew
 
 
 class Rotation:
     @staticmethod
     def x(theta: jtp.Float) -> jtp.Matrix:
-
         return so3.SO3.from_x_radians(theta=theta).as_matrix()
 
     @staticmethod
     def y(theta: jtp.Float) -> jtp.Matrix:
-
         return so3.SO3.from_y_radians(theta=theta).as_matrix()
 
     @staticmethod
     def z(theta: jtp.Float) -> jtp.Matrix:
-
         return so3.SO3.from_z_radians(theta=theta).as_matrix()
 
     @staticmethod
     def from_axis_angle(vector: jtp.Vector) -> jtp.Matrix:
-
         vector = vector.squeeze()
         theta = jnp.linalg.norm(vector)
 
         def theta_is_not_zero(theta_and_v: Tuple[jtp.Float, jtp.Vector]) -> jtp.Matrix:
-
             theta, v = theta_and_v
 
             s = jnp.sin(theta)
             c = jnp.cos(theta)
 
             c1 = 2 * jnp.sin(theta / 2.0) ** 2
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev137/src/jaxsim/math/skew.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 import jaxsim.typing as jtp
 
 
 class Skew:
     @staticmethod
     def wedge(vector: jtp.Vector) -> jtp.Matrix:
-
         vector = vector.squeeze()
 
         x, y, z = vector
         skew = jnp.array([[0, -z, y], [z, 0, -x], [-y, x, 0]])
 
         return skew
 
     @staticmethod
     def vee(matrix: jtp.Matrix) -> jtp.Vector:
-
         # Note: if the input is not already skew-symmetric, this method returns
         #       the values of the skew-symmetric component
         vector = 0.5 * jnp.vstack(
             [
                 matrix[2, 1] - matrix[1, 2],
                 matrix[0, 2] - matrix[2, 0],
                 matrix[1, 0] - matrix[0, 1],
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/collision.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 import jaxsim.logging as logging
 
 from .link import LinkDescription
 
 
 @dataclasses.dataclass
 class CollidablePoint:
-
     parent_link: LinkDescription
     position: npt.NDArray = dataclasses.field(default_factory=lambda: np.zeros(3))
     enabled: bool = True
 
     def change_link(
         self, new_link: LinkDescription, new_H_old: npt.NDArray
     ) -> "CollidablePoint":
-
         msg = f"Moving collidable point: {self.parent_link.name} -> {new_link.name}"
         logging.debug(msg=msg)
 
         return CollidablePoint(
             parent_link=new_link,
             position=(new_H_old @ jnp.hstack([self.position, 1.0])).squeeze()[0:3],
             enabled=self.enabled,
@@ -39,29 +37,26 @@
             + f", enabled={self.enabled}"
             + ")"
         )
 
 
 @dataclasses.dataclass
 class CollisionShape(abc.ABC):
-
     collidable_points: List[CollidablePoint]
 
     def __str__(self):
         return (
             f"{self.__class__.__name__}("
             + "collidable_points=[\n    "
             + ",\n    ".join(str(cp) for cp in self.collidable_points)
             + "\n])"
         )
 
 
 @dataclasses.dataclass
 class BoxCollision(CollisionShape):
-
     center: npt.NDArray
 
 
 @dataclasses.dataclass
 class SphereCollision(CollisionShape):
-
     center: npt.NDArray
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/joint.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 import numpy.typing as npt
 
 from .link import LinkDescription
 
 
 class JointType(enum.IntEnum):
-
     F = enum.auto()  # Fixed
     R = enum.auto()  # Revolute
     P = enum.auto()  # Prismatic
 
     # Revolute joints, single axis
     Rx = enum.auto()
     Ry = enum.auto()
@@ -23,44 +22,37 @@
     Px = enum.auto()
     Py = enum.auto()
     Pz = enum.auto()
 
 
 @dataclasses.dataclass
 class JointDescriptor:
-
     code: JointType
 
     def __hash__(self) -> int:
-
         return hash(self.__repr__())
 
 
 @dataclasses.dataclass
 class JointGenericAxis(JointDescriptor):
-
     axis: npt.NDArray
 
     def __post_init__(self):
-
         if np.allclose(self.axis, 0.0):
             raise ValueError(self.axis)
 
     def __eq__(self, other):
-
         return super().__eq__(other) and np.allclose(self.axis, other.axis)
 
     def __hash__(self) -> int:
-
         return hash(self.__repr__())
 
 
 @dataclasses.dataclass
 class JointDescription:
-
     name: str
     axis: npt.NDArray
     pose: npt.NDArray
     jtype: Union[JointType, JointDescriptor]
     child: LinkDescription = dataclasses.dataclass(repr=False)
     parent: LinkDescription = dataclasses.dataclass(repr=False)
 
@@ -72,16 +64,13 @@
     position_limit_damper: float = 0.0
     position_limit_spring: float = 0.0
 
     position_limit: Tuple[float, float] = (0.0, 0.0)
     initial_position: Union[float, npt.NDArray] = 0.0
 
     def __post_init__(self):
-
         if self.axis is not None:
-
             norm_of_axis = np.linalg.norm(self.axis)
             self.axis = self.axis / norm_of_axis
 
     def __hash__(self) -> int:
-
         return hash(self.__repr__())
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/link.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,38 +8,34 @@
 import jaxsim.typing as jtp
 from jaxsim.sixd import se3
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class LinkDescription(JaxsimDataclass):
-
     name: str = jax_dataclasses.static_field()
     mass: float
     inertia: jtp.Matrix
     index: Optional[int] = None
     parent: "LinkDescription" = jax_dataclasses.static_field(default=None, repr=False)
     pose: jtp.Matrix = dataclasses.field(default_factory=lambda: jnp.eye(4), repr=False)
     children: List["LinkDescription"] = jax_dataclasses.static_field(
         default_factory=list, repr=False
     )
 
     def __hash__(self) -> int:
-
         return hash(self.__repr__())
 
     @property
     def name_and_index(self) -> str:
-
         return f"#{self.index}_<{self.name}>"
 
     def lump_with(
         self, link: "LinkDescription", lumped_H_removed: jtp.Matrix
     ) -> "LinkDescription":
-
         # Get the 6D inertia of the link to remove
         I_removed = link.inertia
 
         # Create the SE3 object. Note the inverse.
         r_H_l = se3.SE3.from_matrix(lumped_H_removed).inverse()
         r_X_l = r_H_l.adjoint()
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .collision import CollidablePoint, CollisionShape
 from .joint import JointDescription
 from .link import LinkDescription
 
 
 @dataclasses.dataclass(frozen=True)
 class ModelDescription(KinematicGraph):
-
     name: str = None
     fixed_base: bool = True
     collision_shapes: List[CollisionShape] = dataclasses.field(default_factory=list)
 
     @staticmethod
     def build_model_from(
         name: str,
@@ -26,36 +25,33 @@
         joints: List[JointDescription],
         collisions: List[CollisionShape] = (),
         fixed_base: bool = False,
         base_link_name: str = None,
         considered_joints: List[str] = None,
         model_pose: RootPose = RootPose(),
     ) -> "ModelDescription":
-
         # Create the full kinematic graph
         kinematic_graph = KinematicGraph.build_from(
             links=links,
             joints=joints,
             root_link_name=base_link_name,
             root_pose=model_pose,
         )
 
         # Reduce the graph if needed
         if considered_joints is not None:
-
             kinematic_graph = kinematic_graph.reduce(
                 considered_joints=considered_joints
             )
 
         # Store here the final model collisions
         final_collisions: List[CollisionShape] = []
 
         # Move and express the collision shapes of the removed link to the lumped link
         for collision_shape in collisions:
-
             # Get all the collidable points of the shape
             coll_points = [cp for cp in collision_shape.collidable_points]
 
             # Assume they have an unique parent link
             if not len(set({cp.parent_link.name for cp in coll_points})) == 1:
                 msg = "Collision shape not currently supported (multiple parent links)"
                 raise RuntimeError(msg)
@@ -79,15 +75,14 @@
             # Create a new collision shape
             new_collision_shape = CollisionShape(collidable_points=[])
             final_collisions.append(new_collision_shape)
 
             # If the frame was found, update the collidable points' pose and add them
             #  to the new collision shape
             for cp in collision_shape.collidable_points:
-
                 # Find the link that is part of the (reduced) model in which the
                 # collision shape's parent was lumped into
                 real_parent_link_of_shape = kinematic_graph.frames_dict[
                     parent_link_of_shape.name
                 ].parent
 
                 # Change the link associated to the collidable point, updating their
@@ -114,15 +109,14 @@
             frames=kinematic_graph.frames,
         )
         assert kinematic_graph.root.name == base_link_name, kinematic_graph.root.name
 
         return model
 
     def reduce(self, considered_joints: List[str]) -> "ModelDescription":
-
         msg = "The model reduction logic assumes that removed joints have zero angles"
         logging.info(msg=msg)
 
         if len(set(considered_joints) - set(self.joint_names())) != 0:
             extra_joints = set(considered_joints) - set(self.joint_names())
             msg = f"Found joints not part of the model: {extra_joints}"
             raise ValueError(msg)
@@ -135,39 +129,36 @@
             fixed_base=self.fixed_base,
             base_link_name=list(iter(self))[0].name,
             model_pose=self.root_pose,
             considered_joints=considered_joints,
         )
 
     def update_collision_shape_of_link(self, link_name: str, enabled: bool) -> None:
-
         if link_name not in self.link_names():
             raise ValueError(link_name)
 
         for point in self.collision_shape_of_link(
             link_name=link_name
         ).collidable_points:
             point.enabled = enabled
 
     def collision_shape_of_link(self, link_name: str) -> CollisionShape:
-
         if link_name not in self.link_names():
             raise ValueError(link_name)
 
         return CollisionShape(
             collidable_points=[
                 point
                 for shape in self.collision_shapes
                 for point in shape.collidable_points
                 if point.parent_link.name == link_name
             ]
         )
 
     def all_enabled_collidable_points(self) -> List[CollidablePoint]:
-
         # Get iterator of all collidable points
         all_collidable_points = itertools.chain.from_iterable(
             [shape.collidable_points for shape in self.collision_shapes]
         )
 
         # Return enabled collidable points
         return [cp for cp in all_collidable_points if cp.enabled]
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev137/src/jaxsim/parsers/kinematic_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,20 @@
 
 from jaxsim import logging
 
 from . import descriptions
 
 
 class RootPose(NamedTuple):
-
     root_position: npt.NDArray = np.zeros(3)
     root_quaternion: npt.NDArray = np.array([1.0, 0, 0, 0])
 
 
 @dataclasses.dataclass(frozen=True)
 class KinematicGraph:
-
     root: descriptions.LinkDescription
     frames: List[descriptions.LinkDescription] = dataclasses.field(default_factory=list)
     joints: List[descriptions.JointDescription] = dataclasses.field(
         default_factory=list
     )
 
     root_pose: RootPose = dataclasses.field(default_factory=RootPose)
@@ -44,36 +42,31 @@
 
     extra_info: Dict[str, Any] = dataclasses.field(
         repr=False, compare=False, default_factory=dict
     )
 
     @functools.cached_property
     def links_dict(self) -> Dict[str, descriptions.LinkDescription]:
-
         return {l.name: l for l in iter(self)}
 
     @functools.cached_property
     def frames_dict(self) -> Dict[str, descriptions.LinkDescription]:
-
         return {f.name: f for f in self.frames}
 
     @functools.cached_property
     def joints_dict(self) -> Dict[str, descriptions.JointDescription]:
-
         return {j.name: j for j in self.joints}
 
     @functools.cached_property
     def joints_connection_dict(
         self,
     ) -> Dict[Tuple[str, str], descriptions.JointDescription]:
-
         return {(j.parent.name, j.child.name): j for j in self.joints}
 
     def __post_init__(self):
-
         # Assign the link index traversing the graph with BFS.
         # Here we assume the model is fixed-base, therefore the base link will
         # have index 0. We will deal with the floating base in a later stage,
         # when this Model object is converted to the physics model.
         for index, link in enumerate(self):
             link.mutable(validate=False).index = index
 
@@ -102,15 +95,14 @@
     @staticmethod
     def build_from(
         links: List[descriptions.LinkDescription],
         joints: List[descriptions.JointDescription],
         root_link_name: str = None,
         root_pose: RootPose = RootPose(),
     ) -> "KinematicGraph":
-
         if root_link_name is None:
             root_link_name = links[0].name
 
         # Couple links and joints and create the graph of links.
         # Note that the pose of the frames is not updated, it's callers
         # responsibility updating their pose if they want to use them.
         graph_root_node, graph_joints, graph_frames = KinematicGraph.create_graph(
@@ -130,30 +122,28 @@
         joints: List[descriptions.JointDescription],
         root_link_name: str,
     ) -> Tuple[
         descriptions.LinkDescription,
         List[descriptions.JointDescription],
         List[descriptions.LinkDescription],
     ]:
-
         # Create a dict that maps link name to the link, for easy retrieval
         links_dict: Dict[str, descriptions.LinkDescription] = {
             l.name: l.mutable(validate=False) for l in links
         }
 
         if root_link_name not in links_dict:
             raise ValueError(root_link_name)
 
         # Reset the connections of the root link
         for link in links_dict.values():
             link.children = []
 
         # Couple links and joints creating the final kinematic graph
         for joint in joints:
-
             # Get the parent and child links of the joint
             parent_link = links_dict[joint.parent.name]
             child_link = links_dict[joint.child.name]
 
             assert child_link.name == joint.child.name
             assert parent_link.name == joint.parent.name
 
@@ -183,27 +173,25 @@
 
         # Store as frames all the links that are not part of the kinematic graph
         frames = list(set(links) - set(all_links_in_graph))
 
         # Update the frames. In particular, reset their children. The other properties
         # are kept as they are, and it's caller responsibility to update them if needed.
         for frame in frames:
-
             frame.children = []
             msg = f"Link '{frame.name}' became a frame"
             logging.info(msg=msg)
 
         return (
             links_dict[root_link_name].mutable(mutable=False),
             list(set(joints) - set(removed_joints)),
             frames,
         )
 
     def reduce(self, considered_joints: List[str]) -> "KinematicGraph":
-
         # The current object represents the complete kinematic graph
         full_graph = self
 
         # Get the names of the joints to remove
         joint_names_to_remove = list(
             set(full_graph.joint_names()) - set(considered_joints)
         )
@@ -211,15 +199,14 @@
         # Return early if there is no action to take
         if len(joint_names_to_remove) == 0:
             logging.info(f"The kinematic graph doesn't need to be reduced")
             return copy.deepcopy(self)
 
         # Check if all considered joints are part of the full kinematic graph
         if len(set(considered_joints) - set([j.name for j in full_graph.joints])) != 0:
-
             extra_j = set(considered_joints) - set([j.name for j in full_graph.joints])
             msg = f"Not all joints to consider are part of the graph ({{{extra_j}}})"
             raise ValueError(msg)
 
         # Extract data we need to modify from the full graph
         links_dict = copy.deepcopy(full_graph.links_dict)
         joints_dict = copy.deepcopy(full_graph.joints_dict)
@@ -247,15 +234,14 @@
             if joint_name in joint_names_to_remove
         ]
 
         # Lump the mass and the inertia traversing the tree from the leaf to the root,
         # this way we propagate these properties back even in the case when also the
         # parent link of a removed joint has to be lumped with its parent.
         for link in reversed(full_graph):
-
             if link.name not in links_to_remove:
                 continue
 
             # Get the link to remove and its parent, i.e. the lumped link
             link_to_remove = links_dict[link.name]
             parent_of_link_to_remove = links_dict[link.parent.name]
 
@@ -307,15 +293,14 @@
             joints_dict[joint_name]
             for joint_name in considered_joints
             if joints_dict[joint_name].parent.name in links_to_remove
         ]
 
         # Update the pose of all joints having as parent link a removed link
         for joint in joints_with_removed_parent_link:
-
             # Update the pose. Note that after the lumping process, the dict entry
             # links_dict[joint.parent.name] contains the final lumped link
             joint.pose = full_graph.relative_transform(
                 relative_to=links_dict[joint.parent.name].name, name=joint.name
             )
 
             # Update the parent link
@@ -356,15 +341,14 @@
 
         # ================================================================
         # 4. Resolve the pose of the frames wrt their reduced graph parent
         # ================================================================
 
         # Update frames properties using the transforms from the full graph
         for frame in reduced_graph.frames:
-
             # Get the link in which the removed link was lumped into
             new_parent_link = links_dict[frame.name]
 
             msg = f"New parent of frame '{frame.name}' is '{new_parent_link.name}'"
             logging.info(msg)
 
             # Update the connection of the frame
@@ -377,44 +361,38 @@
             frame.mass = 0.0
             frame.inertia = np.zeros_like(frame.inertia)
 
         # Return the reduced graph
         return reduced_graph
 
     def link_names(self) -> List[str]:
-
         return list(self.links_dict.keys())
 
     def joint_names(self) -> List[str]:
-
         return list(self.joints_dict.keys())
 
     def frame_names(self) -> List[str]:
-
         return list(self.frames_dict.keys())
 
     def transform(self, name: str) -> npt.NDArray:
-
         if name in self.transform_cache:
             return self.transform_cache[name]
 
         if name in self.joint_names():
-
             joint = self.joints_dict[name]
 
             if joint.initial_position != 0.0:
                 msg = f"Ignoring unsupported initial position of joint '{name}'"
                 logging.warning(msg=msg)
 
             transform = self.transform(name=joint.parent.name) @ joint.pose
             self.transform_cache[name] = transform
             return self.transform_cache[name]
 
         if name in self.link_names():
-
             link = self.links_dict[name]
 
             if link.name == self.root.name:
                 return link.pose
 
             parent_joint = self.joints_connection_dict[(link.parent.name, link.name)]
             transform = self.transform(name=parent_joint.name) @ link.pose
@@ -427,21 +405,19 @@
 
         frame = self.frames_dict[name]
         transform = self.transform(name=frame.parent.name) @ frame.pose
         self.transform_cache[name] = transform
         return self.transform_cache[name]
 
     def relative_transform(self, relative_to: str, name: str) -> npt.NDArray:
-
         return np.linalg.inv(self.transform(name=relative_to)) @ self.transform(
             name=name
         )
 
     def print_tree(self) -> None:
-
         import pptree
 
         root_node = self.root
 
         pptree.print_tree(
             root_node,
             childattr="children",
@@ -450,72 +426,62 @@
         )
 
     @staticmethod
     def breadth_first_search(
         root: descriptions.LinkDescription,
         sort_children: Optional[Callable[[Any], Any]] = lambda link: link.name,
     ) -> Iterable[descriptions.LinkDescription]:
-
         queue = [root]
 
         # We assume that nodes have unique name, and mark a link as visited using
         # its name. This speeds up considerably objects comparison.
         visited = list()
         visited.append(root.name)
 
         yield root
 
         while len(queue) > 0:
-
             l = queue.pop(0)
 
             # Note: sorting the links with their name so that the order of children
             #       insertion does not matter when assigning the link index
             for child in sorted(l.children, key=sort_children):
-
                 if child.name in visited:
                     continue
 
                 visited.append(child.name)
                 queue.append(child)
 
                 yield child
 
     def __iter__(self) -> Iterable[descriptions.LinkDescription]:
-
         yield from KinematicGraph.breadth_first_search(root=self.root)
 
     def __reversed__(self) -> Iterable[descriptions.LinkDescription]:
-
         yield from reversed(list(iter(self)))
 
     def __len__(self) -> int:
-
         return len(list(iter(self)))
 
     def __contains__(self, item: Union[str, descriptions.LinkDescription]) -> bool:
-
         if isinstance(item, str):
             return item in self.link_names()
 
         if isinstance(item, descriptions.LinkDescription):
             return item in set(iter(self))
 
         raise TypeError(type(item).__name__)
 
     def __getitem__(self, key: Union[int, str]) -> descriptions.LinkDescription:
-
         if isinstance(key, str):
-
             if key not in self.link_names():
                 raise KeyError(key)
 
             return self.links_dict[key]
 
         if isinstance(key, int):
-
             if key > len(self):
                 raise KeyError(key)
 
             return list(iter(self))[key]
 
         raise TypeError(type(key).__name__)
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/parser.py` & `jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from jaxsim.math.quaternion import Quaternion
 from jaxsim.parsers import descriptions, kinematic_graph
 
 from . import utils as utils
 
 
 class SDFData(NamedTuple):
-
     model_name: str
 
     fixed_base: bool
     base_link_name: str
 
     link_descriptions: List[descriptions.LinkDescription]
     joint_descriptions: List[descriptions.JointDescription]
@@ -28,15 +27,14 @@
     sdf_model: Optional[rod.Model] = None
     model_pose: kinematic_graph.RootPose = kinematic_graph.RootPose()
 
 
 def extract_data_from_sdf(
     sdf: Union[pathlib.Path, str], model_name: Optional[str] = None
 ) -> SDFData:
-
     # Parse the SDF resource
     sdf_element = rod.Sdf.load(sdf=sdf)
 
     if len(sdf_element.models()) == 0:
         raise RuntimeError("Failed to find any model in SDF resource")
 
     # Assume the SDF resource has only one model, or the desired model name is given
@@ -92,15 +90,14 @@
     # =========================
     # Process fixed-base models
     # =========================
 
     # In this case, we need to get the pose of the joint that connects the base link
     # to the world and combine their pose
     if sdf_model.is_fixed_base():
-
         # Create a massless word link
         world_link = descriptions.LinkDescription(
             name="world", mass=0, inertia=np.zeros(shape=(6, 6))
         )
 
         # Gather joints connecting fixed-base models to the world.
         # TODO: the pose of this joint could be expressed wrt any arbitrary frame,
@@ -153,20 +150,18 @@
 
     # ============
     # Parse joints
     # ============
 
     # Check that all joint poses are expressed w.r.t. their parent link
     for j in sdf_model.joints():
-
         if j.pose is None:
             continue
 
         if j.parent == "world":
-
             if j.pose.relative_to in {"__model__", None}:
                 continue
 
             raise ValueError("Pose of fixed joint connecting to 'world' link not valid")
 
         if j.pose.relative_to != j.parent:
             msg = "Pose of joint '{}' is not expressed wrt its parent link '{}'"
@@ -222,15 +217,14 @@
     ]
 
     # Create a dictionary to find the parent joint of the links
     joint_dict = {j.child.name: j.name for j in joints}
 
     # Check that all the link poses are expressed wrt their parent joint
     for l in sdf_model.links():
-
         if l.name not in links_dict:
             continue
 
         if l.pose is None:
             continue
 
         if l.name == sdf_model.get_canonical_link():
@@ -249,26 +243,23 @@
 
     # Initialize the collision shapes
     collisions: List[descriptions.CollisionShape] = []
 
     # Parse the collisions
     for link in sdf_model.links():
         for collision in link.collisions():
-
             if collision.geometry.box is not None:
-
                 box_collision = utils.create_box_collision(
                     collision=collision,
                     link_description=links_dict[link.name],
                 )
 
                 collisions.append(box_collision)
 
             if collision.geometry.sphere is not None:
-
                 sphere_collision = utils.create_sphere_collision(
                     collision=collision,
                     link_description=links_dict[link.name],
                 )
 
                 collisions.append(sphere_collision)
 
@@ -281,15 +272,14 @@
         base_link_name=sdf_model.get_canonical_link(),
         model_pose=model_pose,
         sdf_model=sdf_model,
     )
 
 
 def build_model_from_sdf(sdf: Union[Path, str]) -> descriptions.ModelDescription:
-
     # Parse data from the SDF
     sdf_data = extract_data_from_sdf(sdf=sdf)
 
     # Build the model description.
     # Note: if the model is fixed-base, the fixed joint between world and the first
     #       link is removed and the pose of the first link is updated.
     model = descriptions.ModelDescription.build_model_from(
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/parsers/sdf/utils.py` & `jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import numpy.typing as npt
 import rod
 
 from jaxsim.parsers import descriptions
 
 
 def from_sdf_inertial(inertial: rod.Inertial) -> npt.NDArray:
-
     from jaxsim.math.inertia import Inertia
     from jaxsim.sixd import se3
 
     # Extract the "mass" element
     m = inertial.mass
 
     # Extract the "inertia" element
@@ -51,15 +50,14 @@
 
     return jnp.array(I_expressed_in_link_frame)
 
 
 def axis_to_jtype(
     axis: rod.Axis, type: str
 ) -> Union[descriptions.JointType, descriptions.JointDescriptor]:
-
     if type == "fixed":
         return descriptions.JointType.F
 
     if not (axis.xyz is not None and axis.xyz.xyz is not None):
         raise ValueError("Failed to read axis xyz data")
 
     axis_xyz = np.array(axis.xyz.xyz)
@@ -94,15 +92,14 @@
 
     raise ValueError("Joint not supported", axis_xyz, type)
 
 
 def create_box_collision(
     collision: rod.Collision, link_description: descriptions.LinkDescription
 ) -> descriptions.BoxCollision:
-
     x, y, z = collision.geometry.box.size
 
     center = np.array([x / 2, y / 2, z / 2])
 
     box_corners = (
         np.vstack(
             [
@@ -139,23 +136,20 @@
         collidable_points=collidable_points, center=center_wrt_link
     )
 
 
 def create_sphere_collision(
     collision: rod.Collision, link_description: descriptions.LinkDescription
 ) -> descriptions.SphereCollision:
-
     # From https://stackoverflow.com/a/26127012
     def fibonacci_sphere(samples: int) -> npt.NDArray:
-
         points = []
         phi = np.pi * (3.0 - np.sqrt(5.0))  # golden angle in radians
 
         for i in range(samples):
-
             y = 1 - (i / float(samples - 1)) * 2  # y goes from 1 to -1
             radius = np.sqrt(1 - y * y)  # radius at y
 
             theta = phi * i  # golden angle increment
 
             x = np.cos(theta) * radius
             z = np.sin(theta) * radius
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/aba.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     model: PhysicsModel,
     xfb: jtp.Vector,
     q: jtp.Vector,
     qd: jtp.Vector,
     tau: jtp.Vector,
     f_ext: jtp.Matrix = None,
 ) -> Tuple[jtp.Vector, jtp.Vector]:
-
     x_fb, q, qd, _, tau, f_ext = utils.process_inputs(
         physics_model=model, xfb=xfb, q=q, qd=qd, tau=tau, f_ext=f_ext
     )
 
     # Extract data from the physics model
     pre_X_λi = model.tree_transforms
     M = model.spatial_inertias
@@ -55,40 +54,37 @@
 
     # Transforms link -> base
     i_X_0 = jnp.zeros_like(pre_X_λi)
     i_X_0 = i_X_0.at[0].set(jnp.eye(6))
 
     # Initialize base quantities
     if model.is_floating_base:
-
         # Base velocity v₀
         v_0 = B_X_W @ base_vel
         v = v.at[0].set(v_0)
 
         # AB inertia (Mᴬ) and AB bias forces (pᴬ)
         MA_0 = M[0]
         MA = MA.at[0].set(MA_0)
         pA_0 = Cross.vx_star(v[0]) @ MA_0 @ v[0] - jnp.linalg.inv(B_X_W).T @ jnp.vstack(
             f_ext[0]
         )
         pA = pA.at[0].set(pA_0)
 
     with jax.experimental.loops.Scope() as s:  # Pass 1
-
         s.qd = qd
         s.f_ext = f_ext
 
         s.i_X_λi = i_X_λi
         s.v = v
         s.c = c
         s.MA = MA
         s.pA = pA
 
         for i in range(1, model.NB):
-
             ii = i - 1
 
             # Compute parent-to-child transform
             i_X_λi_i = i_X_pre[i] @ pre_X_λi[i]
             s.i_X_λi = s.i_X_λi.at[i].set(i_X_λi_i)
 
             # Propagate link velocity
@@ -120,25 +116,23 @@
         pA = s.pA
 
     U = jnp.zeros_like(S)
     d = jnp.zeros(shape=(model.NB, 1))
     u = jnp.zeros(shape=(model.NB, 1))
 
     with jax.experimental.loops.Scope() as s:  # Pass 2
-
         s.tau = tau
 
         s.U = U
         s.d = d
         s.u = u
         s.MA = MA
         s.pA = pA
 
         for i in s.range(model.NB - 1, 0, -1):
-
             ii = i - 1
 
             # Compute intermediate results
             U_i = s.MA[i] @ S[i]
             s.U = s.U.at[i].set(U_i)
 
             d_i = S[i].T @ s.U[i]
@@ -149,15 +143,14 @@
 
             # Compute the articulated-body inertia and bias forces of this link
             Ma = s.MA[i] - s.U[i] / s.d[i] @ s.U[i].T
             pa = s.pA[i] + Ma @ c[i] + s.U[i] * s.u[i] / s.d[i]
 
             # Propagate them to the parent, handling the base link
             def propagate(MA_pA):
-
                 MA, pA = MA_pA
 
                 MA_λi = MA[λ[i]] + i_X_λi[i].T @ Ma @ i_X_λi[i]
                 MA = MA.at[λ[i]].set(MA_λi)
 
                 pA_λi = pA[λ[i]] + i_X_λi[i].T @ pa
                 pA = pA.at[λ[i]].set(pA_λi)
@@ -183,20 +176,18 @@
         a0 = -B_X_W @ jnp.vstack(model.gravity)
 
     a = jnp.zeros_like(S)
     a = a.at[0].set(a0)
     qdd = jnp.zeros_like(q)
 
     with jax.experimental.loops.Scope() as s:  # Pass 3
-
         s.a = a
         s.qdd = qdd
 
         for i in s.range(1, model.NB):
-
             ii = i - 1
 
             # Propagate link accelerations
             a_i = i_X_λi[i] @ s.a[λ[i]] + c[i]
 
             # Compute joint accelerations
             qdd_ii = (u[i] - U[i].T @ a_i) / d[i]
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/crba.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import jaxsim.typing as jtp
 from jaxsim.physics.model.physics_model import PhysicsModel
 
 from . import utils
 
 
 def crba(model: PhysicsModel, q: jtp.Vector) -> jtp.Matrix:
-
     _, q, _, _, _, _ = utils.process_inputs(
         physics_model=model, xfb=None, q=q, qd=None, tau=None, f_ext=None
     )
 
     Xtree = model.tree_transforms
     Mc = model.spatial_inertias
     S = model.motion_subspaces(q=q)
@@ -35,15 +34,14 @@
 
     ForwardPassCarry = Tuple[jtp.MatrixJax, jtp.MatrixJax]
     forward_pass_carry = (Xup, i_X_0)
 
     def propagate_kinematics(
         carry: ForwardPassCarry, i: jtp.Int
     ) -> Tuple[ForwardPassCarry, None]:
-
         Xup, i_X_0 = carry
 
         Xup_i = Xj[i] @ Xtree[i]
         Xup = Xup.at[i].set(Xup_i)
 
         i_X_0_i = Xup[i] @ i_X_0[λ[i]]
         i_X_0 = i_X_0.at[i].set(i_X_0_i)
@@ -64,15 +62,14 @@
 
     BackwardPassCarry = Tuple[jtp.MatrixJax, jtp.MatrixJax]
     backward_pass_carry = (Mc, M)
 
     def backward_pass(
         carry: BackwardPassCarry, i: jtp.Int
     ) -> Tuple[BackwardPassCarry, None]:
-
         ii = i - 1
         Mc, M = carry
 
         Mc_λi = Mc[λ[i]] + Xup[i].T @ Mc[i] @ Xup[i]
         Mc = Mc.at[λ[i]].set(Mc_λi)
 
         Fi = Mc[i] @ S[i]
@@ -81,15 +78,14 @@
 
         j = i
 
         CarryInnerFn = Tuple[jtp.Int, jtp.MatrixJax, jtp.MatrixJax]
         carry_inner_fn = (j, Fi, M)
 
         def while_loop_body(carry: CarryInnerFn) -> CarryInnerFn:
-
             j, Fi, M = carry
 
             Fi = Xup[j].T @ Fi
             j = λ[j]
             jj = j - 1
 
             M_ij = Fi.T @ S[j]
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from . import utils
 
 
 def forward_kinematics_model(
     model: PhysicsModel, q: jtp.Vector, xfb: jtp.Vector
 ) -> jtp.Array:
-
     x_fb, q, _, _, _, _ = utils.process_inputs(
         physics_model=model, xfb=xfb, q=q, qd=None, tau=None, f_ext=None
     )
 
     W_X_0 = Adjoint.from_quaternion_and_translation(
         quaternion=x_fb[0:4], translation=x_fb[4:7]
     )
@@ -39,15 +38,14 @@
 
     PropagateKinematicsCarry = Tuple[jtp.MatrixJax, jtp.MatrixJax]
     propagate_kinematics_carry = (i_X_λi, W_X_i)
 
     def propagate_kinematics(
         carry: PropagateKinematicsCarry, i: jtp.Int
     ) -> Tuple[PropagateKinematicsCarry, None]:
-
         i_X_λi, W_X_i = carry
 
         i_X_λi_i = i_X_pre[i] @ pre_X_λi[i]
         i_X_λi = i_X_λi.at[i].set(i_X_λi_i)
 
         W_X_i_i = W_X_i[λ[i]] @ Adjoint.inverse(i_X_λi[i])
         W_X_i = W_X_i.at[i].set(W_X_i_i)
@@ -62,9 +60,8 @@
 
     return jnp.stack([Adjoint.to_transform(adjoint=X) for X in list(W_X_i)])
 
 
 def forward_kinematics(
     model: PhysicsModel, body_index: jtp.Int, q: jtp.Vector, xfb: jtp.Vector
 ) -> jtp.Matrix:
-
     return forward_kinematics_model(model=model, q=q, xfb=xfb)[body_index]
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/jacobian.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import jaxsim.typing as jtp
 from jaxsim.physics.model.physics_model import PhysicsModel
 
 from . import utils
 
 
 def jacobian(model: PhysicsModel, body_index: jtp.Int, q: jtp.Vector) -> jtp.Matrix:
-
     _, q, _, _, _, _ = utils.process_inputs(physics_model=model, q=q)
 
     S = model.motion_subspaces(q=q)
     i_X_pre = model.joint_transforms(q=q)
     pre_X_λi = model.tree_transforms
     i_X_λi = jnp.zeros_like(i_X_pre)
 
@@ -32,15 +31,14 @@
 
     PropagateKinematicsCarry = Tuple[jtp.MatrixJax, jtp.MatrixJax]
     propagate_kinematics_carry = (i_X_λi, i_X_0)
 
     def propagate_kinematics(
         carry: PropagateKinematicsCarry, i: jtp.Int
     ) -> Tuple[PropagateKinematicsCarry, None]:
-
         i_X_λi, i_X_0 = carry
 
         i_X_λi_i = i_X_pre[i] @ pre_X_λi[i]
         i_X_λi = i_X_λi.at[i].set(i_X_λi_i)
 
         i_X_0_i = i_X_λi[i] @ i_X_0[λ[i]]
         i_X_0 = i_X_0.at[i].set(i_X_0_i)
@@ -64,15 +62,14 @@
 
     # To make JIT happy, we operate on a boolean version of κ(i).
     # Checking if j ∈ κ(i) is equivalent to: κ_bool(j) is True.
     κ_bool = model.support_body_array_bool(body_index=body_index)
 
     def compute_jacobian(J: jtp.MatrixJax, i: jtp.Int) -> Tuple[jtp.MatrixJax, None]:
         def update_jacobian(J: jtp.MatrixJax, i: jtp.Int) -> jtp.MatrixJax:
-
             ii = i - 1
             Js_i = i_X_0[body_index] @ jnp.linalg.inv(i_X_0[i]) @ S[i]
             J = J.at[0:6, 6 + ii].set(Js_i.squeeze())
 
             return J
 
         J = jax.lax.select(pred=κ_bool[i], on_true=update_jacobian(J, i), on_false=J)
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/rnea.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     xfb: jtp.Vector,
     q: jtp.Vector,
     qd: jtp.Vector,
     qdd: jtp.Vector,
     a0fb: jtp.Vector = jnp.zeros(6),
     f_ext: jtp.Matrix = None,
 ) -> Tuple[jtp.Vector, jtp.Vector]:
-
     xfb, q, qd, qdd, _, f_ext = utils.process_inputs(
         physics_model=model, xfb=xfb, q=q, qd=qd, qdd=qdd, f_ext=f_ext
     )
 
     a0fb = a0fb.squeeze()
     gravity = model.gravity.squeeze()
 
@@ -54,27 +53,25 @@
     Xup = Xup.at[0].set(Xup_0)
 
     v[0] = jnp.zeros(shape=(6, 1))
     f[0] = jnp.zeros(shape=(6, 1))
     a[0] = -B_X_W @ jnp.vstack(gravity)
 
     if model.is_floating_base:
-
         W_v_WB = jnp.vstack(jnp.hstack([xfb[10:13], xfb[7:10]]))
         v[0] = B_X_W @ W_v_WB
 
         a[0] = B_X_W @ (jnp.vstack(a0fb) - jnp.vstack(gravity))
         f[0] = (
             I[0] @ a[0]
             + Cross.vx_star(v[0]) @ I[0] @ v[0]
             - jnp.linalg.inv(B_X_W).T @ jnp.vstack(f_ext[0])
         )
 
     for i in np.arange(start=1, stop=model.NB):
-
         ii = i - 1
 
         vJ = S[i] * qd[ii]
         Xup_i = Xj[i] @ Xtree[i]
         Xup = Xup.at[i].set(Xup_i)
 
         λi = model._parent_array_dict[i]
@@ -90,15 +87,14 @@
             + Cross.vx_star(v[i]) @ I[i] @ v[i]
             - i_X_W @ jnp.vstack(f_ext[i])
         )
 
     tau = jnp.zeros_like(q)
 
     for i in reversed(np.arange(start=1, stop=model.NB)):
-
         ii = i - 1
 
         value = S[i].T @ f[i]
         tau = tau.at[ii].set(value.squeeze())
 
         λi = model._parent_array_dict[i]
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,55 +15,49 @@
 from jaxsim.physics.model.physics_model import PhysicsModel
 
 from . import utils
 
 
 @jax_dataclasses.pytree_dataclass
 class SoftContactsState:
-
     tangential_deformation: jtp.Matrix
 
     @staticmethod
     def zero(
         physics_model: jaxsim.physics.model.physics_model.PhysicsModel,
     ) -> "SoftContactsState":
-
         return SoftContactsState(
             tangential_deformation=jnp.zeros(shape=(3, physics_model.gc.body.size))
         )
 
     def valid(
         self, physics_model: jaxsim.physics.model.physics_model.PhysicsModel
     ) -> bool:
-
         from jaxsim.simulation.utils import check_valid_shape
 
         return check_valid_shape(
             what="tangential_deformation",
             shape=self.tangential_deformation.shape,
             expected_shape=(3, physics_model.gc.body.size),
             valid=True,
         )
 
     def replace(self, validate: bool = True, **kwargs) -> "SoftContactsState":
-
         with jax_dataclasses.copy_and_mutate(self, validate=validate) as updated_state:
-
             _ = [updated_state.__setattr__(k, v) for k, v in kwargs.items()]
 
         return updated_state
 
 
 def collidable_points_pos_vel(
     model: PhysicsModel,
     q: jtp.Vector,
     qd: jtp.Vector,
     xfb: jtp.Vector = None,
 ) -> Tuple[jtp.Matrix, jtp.Matrix]:
-
     xfb, q, qd, _, _, _ = utils.process_inputs(physics_model=model, xfb=xfb, q=q, qd=qd)
 
     Xa = jnp.array([jnp.eye(6)] * (model.NB))
     vb = jnp.array([jnp.zeros([6, 1])] * (model.NB))
 
     # 6D transform of base velocity
     Xa_0 = B_X_W = Adjoint.from_quaternion_and_translation(
@@ -77,20 +71,18 @@
 
     Xtree = model.tree_transforms
     S = model.motion_subspaces(q=q)
     XJ = model.joint_transforms(q=q)
     parent_link_of = model.parent_array()
 
     with jax.experimental.loops.Scope() as s:
-
         s.Xa = Xa
         s.vb = vb
 
         for i in s.range(1, model.NB):
-
             ii = i - 1
 
             Xup = XJ[i] @ Xtree[i]
             vJ = S[i] * qd[ii] if qd.size != 0 else S[i] * 0
 
             Xa_i = Xup @ s.Xa[parent_link_of[i]]
             s.Xa = s.Xa.at[i].set(Xa_i)
@@ -98,15 +90,14 @@
             vb_i = jnp.vstack(Xup @ s.vb[parent_link_of[i]]) + vJ
             s.vb = s.vb.at[i].set(vb_i)
 
         Xa = s.Xa
         vb = s.vb
 
     def process_collidable_points_of_link_with_index(i: int) -> jtp.VectorJax:
-
         X = jnp.linalg.inv(Xa[i])
         v = X @ vb[i]
 
         pt = Convert.coordinates_tf(X=X, p=model.gc.point)
         vpt = Convert.velocities_threed(v_6d=v, p=pt)
 
         return jnp.vstack([pt, vpt])
@@ -129,28 +120,26 @@
     )
 
     return pos_vel[0:3, :].squeeze(), pos_vel[3:6, :].squeeze()
 
 
 @jax_dataclasses.pytree_dataclass
 class SoftContactsParams:
-
     K: float = jnp.array(1e6, dtype=float)
     D: float = jnp.array(2000, dtype=float)
     mu: float = jnp.array(0.5, dtype=float)
 
 
 def soft_contacts_model(
     positions: jtp.Vector,
     velocities: jtp.Vector,
     tangential_deformation: jtp.Vector,
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     terrain: Terrain = FlatTerrain(),
 ) -> Tuple[jtp.Matrix, jtp.Matrix, jtp.Matrix]:
-
     p = jnp.array(positions).squeeze()
     pd = jnp.array(velocities).squeeze()
     u = jnp.array(tangential_deformation).squeeze()
 
     K = soft_contacts_params.K
     D = soft_contacts_params.D
     mu = soft_contacts_params.mu
@@ -186,41 +175,40 @@
     # Compute the 3D linear force in C[W] frame
     forces_normal = terrain_normal.T * forces_normal_mag
 
     # ====================================
     # No friction and no tangential forces
     # ====================================
 
-    # Compute the adjoint C[W]->W for transforming 6D forces from mixed to inertial
+    # Compute the adjoint C[W]->W for transforming 6D forces from mixed to inertial.
+    # Note: this is equal to the 6D velocities transform: CW_X_W.transpose().
     W_Xf_CW = jax.vmap(
         lambda W_p_C: jnp.block(
             [
                 [jnp.eye(3), jnp.zeros(shape=(3, 3))],
                 [Skew.wedge(W_p_C), jnp.eye(3)],
             ]
         )
     )(p.T)
 
     def with_no_friction():
-
         # Compute 6D mixed forces in C[W]
         CW_f_lin = forces_normal
         CW_f = jnp.vstack([CW_f_lin, jnp.zeros_like(CW_f_lin)])
 
         # Compute lin-ang 6D forces (inertial representation)
         W_f = jax.vmap(lambda X, f: X @ f)(W_Xf_CW, CW_f.T).T
 
         return W_f, jnp.zeros_like(u), jnp.zeros_like(forces_normal[0])
 
     # =========================
     # Compute tangential forces
     # =========================
 
     def with_friction():
-
         # Initialize the tangential velocity of the point
         v_perpendicular = jax.vmap(jnp.dot)(pd.T, terrain_normal) * terrain_normal.T
         v_tangential = pd - v_perpendicular
         v_tangential = jnp.where(in_contact, v_tangential, 0.0)
 
         # Initialize the tangential deformation rate u̇.
         # For inactive contacts with u≠0, this is the dynamics of the material relaxation.
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/terrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 import jax.numpy as jnp
 import jax_dataclasses
 
 import jaxsim.typing as jtp
 
 
 class Terrain(abc.ABC):
-
     delta = 0.010
 
     @abc.abstractmethod
     def height(self, x: float, y: float) -> float:
         pass
 
     def normal(self, x: float, y: float) -> jtp.Vector:
-
         # https://stackoverflow.com/a/5282364
         h_xp = self.height(x=x + self.delta, y=y)
         h_xm = self.height(x=x - self.delta, y=y)
         h_yp = self.height(x=x, y=y + self.delta)
         h_ym = self.height(x=x, y=y - self.delta)
 
         n = jnp.array(
@@ -33,14 +31,12 @@
 class FlatTerrain(Terrain):
     def height(self, x: float, y: float) -> float:
         return 0.0
 
 
 @jax_dataclasses.pytree_dataclass
 class PlaneTerrain(Terrain):
-
     plane_normal: jtp.Vector = jax_dataclasses.field(default=jnp.array([0, 0, 1.0]))
 
     def height(self, x: float, y: float) -> float:
-
         a, b, c = self.plane_normal
         return -(a * x + b * x) / c
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/algos/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,25 +11,23 @@
     xfb: jtp.Vector = None,
     q: jtp.Vector = None,
     qd: jtp.Vector = None,
     qdd: jtp.Vector = None,
     tau: jtp.Vector = None,
     f_ext: jtp.Matrix = None,
 ) -> Tuple[jtp.Vector, jtp.Vector, jtp.Vector, jtp.Vector, jtp.Vector, jtp.Matrix]:
-
     # Remove extra dimensions
     q = q.squeeze() if q is not None else None
     qd = qd.squeeze() if qd is not None else None
     qdd = qdd.squeeze() if qdd is not None else None
     tau = tau.squeeze() if tau is not None else None
     xfb = xfb.squeeze() if xfb is not None else None
     f_ext = f_ext.squeeze() if f_ext is not None else None
 
     def fix_one_dof(vector: jtp.Vector) -> Optional[jtp.Vector]:
-
         if vector is None:
             return None
 
         return jnp.array([vector]) if vector.shape == () else vector
 
     # Fix case with just 1 DoF
     q = fix_one_dof(q)
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/model/ground_contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,23 @@
 import numpy.typing as npt
 
 from jaxsim.parsers.descriptions import ModelDescription
 
 
 @jax_dataclasses.pytree_dataclass
 class GroundContact:
-
     point: npt.NDArray = jax_dataclasses.field(default_factory=lambda: jnp.array([]))
     body: npt.NDArray = jax_dataclasses.static_field(
         default_factory=lambda: np.array([], dtype=int)
     )
 
     @staticmethod
     def build_from(
         model_description: ModelDescription,
     ) -> "GroundContact":
-
         if len(model_description.collision_shapes) == 0:
             return GroundContact()
 
         # Get all the links so that we can take their updated index
         links_dict = {link.name: link for link in model_description}
 
         # Get all the enabled collidable points of the model
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from .ground_contact import GroundContact
 from .physics_model_state import PhysicsModelState
 
 
 @pytree_dataclass
 class PhysicsModel(JaxsimDataclass):
-
     NB: int = static_field()
     initial_state: PhysicsModelState = jax_dataclasses.field(default=None)
     gravity: jtp.Vector = dataclasses.field(
         default_factory=lambda: jnp.hstack(
             [np.zeros(3), jaxsim.physics.default_gravity()]
         )
     )
@@ -47,25 +46,23 @@
     _joint_friction_static: Dict[int, float] = dataclasses.field(default_factory=dict)
     _joint_friction_viscous: Dict[int, float] = dataclasses.field(default_factory=dict)
 
     _joint_limit_spring: Dict[int, float] = dataclasses.field(default_factory=dict)
     _joint_limit_damper: Dict[int, float] = dataclasses.field(default_factory=dict)
 
     def __post_init__(self):
-
         if self.initial_state is None:
             initial_state = PhysicsModelState.zero(physics_model=self)
             object.__setattr__(self, "initial_state", initial_state)
 
     @staticmethod
     def build_from(
         model_description: jaxsim.parsers.descriptions.model.ModelDescription,
         gravity: jtp.Vector = default_gravity(),
     ) -> "PhysicsModel":
-
         if gravity.size != 3:
             raise ValueError(gravity.size)
 
         # Currently, we assume that the link frame matches the frame of its parent joint
         for l in model_description:
             if not jnp.allclose(l.pose, jnp.eye(4)):
                 raise ValueError(f"Link '{l.name}' has unsupported pose:\n{l.pose}")
@@ -189,19 +186,17 @@
         # Fixed-base models
         with jax_dataclasses.copy_and_mutate(physics_model) as physics_model_fixed:
             physics_model_fixed.is_floating_base = False
 
         return physics_model_fixed
 
     def dofs(self) -> int:
-
         return len(list(self._jtype_dict.keys()))
 
     def set_gravity(self, gravity: jtp.Vector) -> None:
-
         gravity = gravity.squeeze()
 
         if gravity.size == 3:
             self.gravity = jnp.hstack([gravity, 0, 0, 0])
 
         elif gravity.size == 6:
             self.gravity = gravity
@@ -211,74 +206,67 @@
 
     @property
     def parent(self) -> jtp.Vector:
         return self.parent_array()
 
     def parent_array(self) -> jtp.Vector:
         """Returns λ(i)"""
-
         return jnp.array([-1] + list(self._parent_array_dict.values()), dtype=int)
 
     def support_body_array(self, body_index: jtp.Int) -> jtp.Vector:
         """Returns κ(i)"""
 
         κ_bool = self.support_body_array_bool(body_index=body_index)
         return jnp.array(jnp.where(κ_bool)[0], dtype=int)
 
     def support_body_array_bool(self, body_index: jtp.Int) -> jtp.Vector:
-
         active_link = body_index
         κ_bool = jnp.zeros(self.NB, dtype=bool)
 
         for i in np.flip(np.arange(start=0, stop=self.NB)):
-
             κ_bool, active_link = jax.lax.cond(
                 pred=(i == active_link),
                 false_fun=lambda: (κ_bool, active_link),
                 true_fun=lambda: (
                     κ_bool.at[active_link].set(True),
                     self.parent[active_link],
                 ),
             )
 
         return κ_bool
 
     @property
     def tree_transforms(self) -> jtp.Array:
-
         X_tree = jnp.array(
             [
                 self._tree_transforms_dict.get(idx, jnp.eye(6))
                 for idx in np.arange(start=0, stop=self.NB)
             ]
         )
 
         return X_tree
 
     @property
     def spatial_inertias(self) -> jtp.Array:
-
         M_links = jnp.array(
             [
                 self._link_inertias_dict.get(idx, jnp.zeros(6))
                 for idx in np.arange(start=0, stop=self.NB)
             ]
         )
 
         return M_links
 
     def jtype(self, joint_index: int) -> JointType:
-
         if joint_index == 0 or joint_index >= self.NB:
             raise ValueError(joint_index)
 
         return self._jtype_dict[joint_index]
 
     def joint_transforms(self, q: jtp.Vector) -> jtp.Array:
-
         from jaxsim.math.joint import jcalc
 
         if not_tracing(q):
             if q.shape[0] != self.dofs():
                 raise ValueError(q.shape)
 
         Xj = jnp.stack(
@@ -288,15 +276,14 @@
                 for index, joint_position in enumerate(q)
             ]
         )
 
         return Xj
 
     def motion_subspaces(self, q: jtp.Vector) -> jtp.Array:
-
         from jaxsim.math.joint import jcalc
 
         if not_tracing(var=q):
             if q.shape[0] != self.dofs():
                 raise ValueError(q.shape)
 
         SS = jnp.stack(
@@ -306,27 +293,24 @@
                 for index, joint_position in enumerate(q)
             ]
         )
 
         return SS
 
     def __eq__(self, other: "PhysicsModel") -> bool:
-
         same = True
         same = same and self.NB == other.NB
         same = same and np.allclose(self.gravity, other.gravity)
 
         return same
 
     def __hash__(self):
-
         return hash(self.__repr__())
 
     def __repr__(self) -> str:
-
         attributes = [
             f"dofs: {self.dofs()},",
             f"links: {self.NB},",
             f"floating_base: {self.is_floating_base},",
         ]
         attributes_string = "\n    ".join(attributes)
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import jaxsim.physics.model.physics_model
 import jaxsim.typing as jtp
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class PhysicsModelState(JaxsimDataclass):
-
     # Joint state
     joint_positions: jtp.Vector
     joint_velocities: jtp.Vector
 
     # Base state
     base_position: jtp.Vector = jax_dataclasses.field(
         default_factory=lambda: jnp.zeros(3)
@@ -27,52 +26,47 @@
         default_factory=lambda: jnp.zeros(3)
     )
 
     @staticmethod
     def zero(
         physics_model: "jaxsim.physics.model.physics_model.PhysicsModel",
     ) -> "PhysicsModelState":
-
         return PhysicsModelState(
             joint_positions=jnp.zeros(physics_model.dofs()),
             joint_velocities=jnp.zeros(physics_model.dofs()),
         )
 
     def position(self) -> jtp.Vector:
-
         return jnp.hstack(
             [self.base_position, self.base_quaternion, self.joint_positions]
         )
 
     def velocity(self) -> jtp.Vector:
-
         # W_v_WB: inertial-fixed representation of the base velocity
         return jnp.hstack(
             [
                 self.base_linear_velocity,
                 self.base_angular_velocity,
                 self.joint_velocities,
             ]
         )
 
     def xfb(self) -> jtp.Vector:
-
         return jnp.hstack(
             [
                 self.base_quaternion,
                 self.base_position,
                 self.base_angular_velocity,
                 self.base_linear_velocity,
             ]
         )
 
     def valid(
         self, physics_model: "jaxsim.physics.model.physics_model.PhysicsModel"
     ) -> bool:
-
         from jaxsim.simulation.utils import check_valid_shape
 
         valid = True
 
         valid = check_valid_shape(
             what="joint_positions",
             shape=self.joint_positions.shape,
@@ -116,43 +110,38 @@
         )
 
         return valid
 
 
 @jax_dataclasses.pytree_dataclass
 class PhysicsModelInput:
-
     tau: jtp.VectorJax
     f_ext: jtp.MatrixJax
 
     @staticmethod
     def zero(
         physics_model: "jaxsim.physics.model.physics_model.PhysicsModel",
     ) -> "PhysicsModelInput":
-
         ode_input = PhysicsModelInput(
             tau=jnp.zeros(physics_model.dofs()),
             f_ext=jnp.zeros(shape=(physics_model.NB, 6)),
         )
 
         assert ode_input.valid(physics_model)
         return ode_input
 
     def replace(self, validate: bool = True, **kwargs) -> "PhysicsModelInput":
-
         with jax_dataclasses.copy_and_mutate(self, validate=validate) as updated_input:
-
             _ = [updated_input.__setattr__(k, v) for k, v in kwargs.items()]
 
         return updated_input
 
     def valid(
         self, physics_model: "jaxsim.physics.model.physics_model.PhysicsModel"
     ) -> bool:
-
         from jaxsim.simulation.utils import check_valid_shape
 
         valid = True
 
         valid = check_valid_shape(
             what="tau",
             shape=self.tau.shape,
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev137/src/jaxsim/simulation/integrators.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,26 +28,24 @@
 def odeint_euler_one_step(
     dx_dt: StateDerivativeCallable,
     x0: State,
     t0: Time,
     tf: Time,
     num_sub_steps: int = 1,
 ) -> Tuple[State, Dict[str, Any]]:
-
     # Compute the sub-step size.
     # We break dt in configurable sub-steps.
     dt = tf - t0
     sub_step_dt = dt / num_sub_steps
 
     # Initialize the carry
     Carry = Tuple[State, Time]
     carry_init: Carry = (x0, t0)
 
     def body_fun(carry: Carry, xs: None) -> Tuple[Carry, None]:
-
         # Unpack the carry
         x_t0, t0 = carry
 
         # Compute the state derivative
         dxdt_t0, _ = dx_dt(x_t0, t0)
 
         # Integrate the dynamics
@@ -77,26 +75,24 @@
 def odeint_rk4_one_step(
     dx_dt: StateDerivativeCallable,
     x0: State,
     t0: Time,
     tf: Time,
     num_sub_steps: int = 1,
 ) -> Tuple[State, Dict[str, Any]]:
-
     # Compute the sub-step size.
     # We break dt in configurable sub-steps.
     dt = tf - t0
     sub_step_dt = dt / num_sub_steps
 
     # Initialize the carry
     Carry = Tuple[State, Time]
     carry_init: Carry = (x0, t0)
 
     def body_fun(carry: Carry, xs: None) -> Tuple[Carry, None]:
-
         # Unpack the carry
         x_t0, t0 = carry
 
         # Helper to forward the state to compute k2 and k3 at midpoint and k4 at final
         euler_mid = lambda x, dxdt: x + (0.5 * sub_step_dt) * dxdt
         euler_fin = lambda x, dxdt: x + sub_step_dt * dxdt
 
@@ -135,45 +131,41 @@
 def odeint_euler_semi_implicit_one_step(
     dx_dt: StateDerivativeCallable,
     x0: ODEState,
     t0: Time,
     tf: Time,
     num_sub_steps: int = 1,
 ) -> Tuple[ODEState, Dict[str, Any]]:
-
     # Compute the sub-step size.
     # We break dt in configurable sub-steps.
     dt = tf - t0
     sub_step_dt = dt / num_sub_steps
 
     # Initialize the carry
     Carry = Tuple[ODEState, Time]
     carry_init: Carry = (x0, t0)
 
     def quaternion_derivative(W_Q_B: jtp.Vector, W_omega_WB: jtp.Vector) -> jtp.Vector:
-
         from jaxsim.math.quaternion import Quaternion
 
         return Quaternion.derivative(
             quaternion=W_Q_B, omega=W_omega_WB, omega_in_body_fixed=False
         ).squeeze()
 
     def inertial_to_3d_mixed(
         W_v_lin_WB: jtp.Vector, W_v_ang_WB: jtp.Vector, W_pos_B: jtp.Vector
     ) -> jtp.Vector:
-
         from jaxsim.math.conv import Convert
 
         # Compute linear component of mixed velocity BW_v_WB
         return Convert.velocities_threed(
             v_6d=jnp.hstack([W_v_lin_WB, W_v_ang_WB]), p=W_pos_B.squeeze()
         ).squeeze()
 
     def body_fun(carry: Carry, xs: None) -> Tuple[Carry, None]:
-
         # Unpack the carry
         x_t0, t0 = carry
 
         # Extract the initial position and velocity
         pos_t0 = x_t0.physics_model.position()
         vel_t0 = x_t0.physics_model.velocity()
 
@@ -249,20 +241,18 @@
 
 
 def integrate_single_step_over_horizon(
     integrator_single_step: Callable[[Time, Time, State], Tuple[State, Dict[str, Any]]],
     t: TimeHorizon,
     x0: State,
 ) -> Tuple[State, Dict[str, Any]]:
-
     # Initialize the carry
     carry_init = (x0, t)
 
     def body_fun(carry: Tuple, idx: int) -> Tuple[Tuple, jtp.PyTree]:
-
         # Unpack the carry
         x_t0, horizon = carry
 
         # Get the integration interval
         t0 = horizon[idx]
         tf = horizon[idx + 1]
 
@@ -292,15 +282,14 @@
     func,
     y0: State,
     t: TimeHorizon,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False
 ) -> Union[State, Tuple[State, Dict[str, Any]]]:
-
     # Close func over additional inputs and parameters
     dx_dt_closure_aux = lambda x, ts: func(x, ts, *args)
 
     # Close one-step integration over its arguments
     integrator_single_step = lambda t0, tf, x0: odeint_euler_one_step(
         dx_dt=dx_dt_closure_aux, x0=x0, t0=t0, tf=tf, num_sub_steps=num_sub_steps
     )
@@ -317,15 +306,14 @@
     func,
     y0: State,
     t: TimeHorizon,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False
 ) -> Union[State, Tuple[State, Dict[str, Any]]]:
-
     # Close func over additional inputs and parameters
     dx_dt_closure_aux = lambda x, ts: func(x, ts, *args)
 
     # Close one-step integration over its arguments
     integrator_single_step = lambda t0, tf, x0: odeint_euler_semi_implicit_one_step(
         dx_dt=dx_dt_closure_aux, x0=x0, t0=t0, tf=tf, num_sub_steps=num_sub_steps
     )
@@ -342,15 +330,14 @@
     func,
     y0: State,
     t: TimeHorizon,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False
 ) -> Union[State, Tuple[State, Dict[str, Any]]]:
-
     # Close func over additional inputs and parameters
     dx_dt_closure = lambda x, ts: func(x, ts, *args)
 
     # Close one-step integration over its arguments
     integrator_single_step = lambda t0, tf, x0: odeint_rk4_one_step(
         dx_dt=dx_dt_closure, x0=x0, t0=t0, tf=tf, num_sub_steps=num_sub_steps
     )
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev137/src/jaxsim/simulation/ode.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 def compute_contact_forces(
     physics_model: PhysicsModel,
     ode_state: ode_data.ODEState,
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     terrain: Terrain = FlatTerrain(),
 ) -> Tuple[jtp.Matrix, jtp.Matrix, jtp.Matrix]:
-
     # Compute position and linear mixed velocity of all model's collidable points
     # collidable_points_kinematics
     pos_cp, vel_cp = collidable_points_pos_vel(
         model=physics_model,
         q=ode_state.physics_model.joint_positions,
         qd=ode_state.physics_model.joint_velocities,
         xfb=ode_state.physics_model.xfb(),
@@ -45,15 +44,14 @@
     # Initialize the contact forces, one per body
     contact_forces_links = jnp.zeros_like(
         ode_data.ODEInput.zero(physics_model).physics_model.f_ext
     )
 
     # Combine the contact forces of all collidable points belonging to the same body
     for body_idx in set(physics_model.gc.body):
-
         body_idx = int(body_idx)
         contact_forces_links = contact_forces_links.at[body_idx, :].set(
             jnp.sum(contact_forces_points[:, physics_model.gc.body == body_idx], axis=1)
         )
 
     return contact_forces_links, tangential_deformation_dot, contact_forces_points.T
 
@@ -62,15 +60,14 @@
     x: ode_data.ODEState,
     t: Optional[jtp.Float],
     physics_model: PhysicsModel,
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     ode_input: ode_data.ODEInput = None,
     terrain: Terrain = FlatTerrain(),
 ) -> Tuple[ode_data.ODEState, Dict[str, Any]]:
-
     if t is not None and isinstance(t, np.ndarray) and t.size != 1:
         raise ValueError(t.size)
 
     # Initialize arguments
     ode_state = x
     ode_input = (
         ode_input
@@ -106,15 +103,14 @@
         )
 
     # =====================
     # Joint position limits
     # =====================
 
     if physics_model.dofs() > 0:
-
         # Get the joint position limits
         s_min, s_max = jnp.array(
             [j.position_limit for j in physics_model.description.joints_dict.values()]
         ).T
 
         # Get the spring/damper parameters of joint limits enforcement
         k_damper = jnp.array(list(physics_model._joint_limit_damper.values()))
@@ -129,15 +125,14 @@
         tau_limit = jnp.zeros_like(ode_input.physics_model.tau)
 
     # ==============
     # Joint friction
     # ==============
 
     if physics_model.dofs() > 0:
-
         # Static and viscous joint friction parameters
         kc = jnp.array(list(physics_model._joint_friction_static.values()))
         kv = jnp.array(list(physics_model._joint_friction_viscous.values()))
 
         # Compute the joint friction torque
         tau_friction = -(
             jnp.diag(kc) @ jnp.sign(ode_state.physics_model.joint_positions)
@@ -167,20 +162,18 @@
     )
 
     # =========================================
     # Compute the state derivative of base link
     # =========================================
 
     if not physics_model.is_floating_base:
-
         W_Qd_B = jnp.zeros(4)
         BW_v_WB = jnp.zeros(3)
 
     else:
-
         from jaxsim.math.conv import Convert
         from jaxsim.math.quaternion import Quaternion
 
         W_Qd_B = Quaternion.derivative(
             quaternion=ode_state.physics_model.base_quaternion,
             omega=ode_state.physics_model.base_angular_velocity,
             omega_in_body_fixed=False,
@@ -201,15 +194,14 @@
     xd_fb = jnp.hstack([W_Qd_B, BW_v_WB, W_a_WB.squeeze()]).squeeze()
 
     # =====================================
     # Build the full derivative of ODEState
     # =====================================
 
     def fix_one_dof(vector: jtp.Vector) -> Optional[jtp.Vector]:
-
         if vector is None:
             return None
 
         return jnp.array([vector]) if vector.shape == () else vector
 
     physics_model_state_derivative = ode_state.physics_model.replace(
         joint_positions=fix_one_dof(ode_state.physics_model.joint_velocities.squeeze()),
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev137/src/jaxsim/simulation/ode_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,52 +9,45 @@
     PhysicsModelState,
 )
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class ODEInput(JaxsimDataclass):
-
     physics_model: PhysicsModelInput
 
     @staticmethod
     def zero(physics_model: PhysicsModel) -> "ODEInput":
-
         return ODEInput(
             physics_model=PhysicsModelInput.zero(physics_model=physics_model)
         )
 
     def valid(self, physics_model: PhysicsModel) -> bool:
-
         return self.physics_model.valid(physics_model=physics_model)
 
 
 @jax_dataclasses.pytree_dataclass
 class ODEState(JaxsimDataclass):
-
     physics_model: PhysicsModelState
     soft_contacts: SoftContactsState
 
     @staticmethod
     def deserialize(data: jtp.VectorJax, physics_model: PhysicsModel) -> "ODEState":
-
         dummy_object = ODEState.zero(physics_model=physics_model)
         _, unflatten_data = jax.flatten_util.ravel_pytree(dummy_object)
 
         return unflatten_data(data)
 
     @staticmethod
     def zero(physics_model: PhysicsModel) -> "ODEState":
-
         model_state = ODEState(
             physics_model=PhysicsModelState.zero(physics_model=physics_model),
             soft_contacts=SoftContactsState.zero(physics_model=physics_model),
         )
 
         assert model_state.valid(physics_model)
         return model_state
 
     def valid(self, physics_model: PhysicsModel) -> bool:
-
         return self.physics_model.valid(
             physics_model=physics_model
         ) and self.soft_contacts.valid(physics_model=physics_model)
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev137/src/jaxsim/simulation/ode_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,27 @@
 from jaxsim.physics.algos.soft_contacts import SoftContactsParams
 from jaxsim.physics.algos.terrain import FlatTerrain, Terrain
 from jaxsim.physics.model.physics_model import PhysicsModel
 from jaxsim.simulation import integrators, ode
 
 
 class IntegratorType(enum.IntEnum):
-
     RungeKutta4 = enum.auto()
     EulerForward = enum.auto()
     EulerSemiImplicit = enum.auto()
 
 
 @jax.jit
 def ode_integration_rk4_adaptive(
     x0: jtp.Array,
     t: integrators.TimeHorizon,
     physics_model: PhysicsModel,
     *args,
     **kwargs,
 ) -> jtp.Array:
-
     # Close function over its inputs and parameters
     dx_dt_closure = lambda x, ts: ode.dx_dt(x, ts, physics_model, *args)
 
     return odeint(dx_dt_closure, x0, t, **kwargs)
 
 
 @functools.partial(jax.jit, static_argnames=["num_sub_steps", "return_aux"])
@@ -42,15 +40,14 @@
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     terrain: Terrain = FlatTerrain(),
     ode_input: ode.ode_data.ODEInput = None,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False,
 ) -> Union[ode.ode_data.ODEState, Tuple[ode.ode_data.ODEState, Dict[str, Any]]]:
-
     # Close func over additional inputs and parameters
     dx_dt_closure = lambda x, ts: ode.dx_dt(
         x, ts, physics_model, soft_contacts_params, ode_input, terrain, *args
     )
 
     # Integrate over the horizon
     out = integrators.odeint_euler(
@@ -74,15 +71,14 @@
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     terrain: Terrain = FlatTerrain(),
     ode_input: ode.ode_data.ODEInput = None,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False,
 ) -> Union[ode.ode_data.ODEState, Tuple[ode.ode_data.ODEState, Dict[str, Any]]]:
-
     # Close func over additional inputs and parameters
     dx_dt_closure = lambda x, ts: ode.dx_dt(
         x, ts, physics_model, soft_contacts_params, ode_input, terrain, *args
     )
 
     # Integrate over the horizon
     out = integrators.odeint_euler_semi_implicit(
@@ -106,15 +102,14 @@
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     terrain: Terrain = FlatTerrain(),
     ode_input: ode.ode_data.ODEInput = None,
     *args,
     num_sub_steps=1,
     return_aux: bool = False,
 ) -> Union[ode.ode_data.ODEState, Tuple[ode.ode_data.ODEState, Dict]]:
-
     # Close func over additional inputs and parameters
     dx_dt_closure = lambda x, ts: ode.dx_dt(
         x, ts, physics_model, soft_contacts_params, ode_input, terrain, *args
     )
 
     # Integrate over the horizon
     out = integrators.odeint_rk4(
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/simulation/simulator.py` & `jaxsim-0.1.dev137/src/jaxsim/simulation/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from jaxsim.physics.model.physics_model import PhysicsModel
 from jaxsim.simulation import ode_integration
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class SimulatorData(JaxsimDataclass):
-
     # Simulation time stored in ns in order to prevent floats approximation
     time_ns: jtp.Int = jnp.array(0, dtype=jnp.int64)
 
     # Terrain and contact parameters
     terrain: Terrain = jax_dataclasses.field(default_factory=lambda: FlatTerrain())
     contact_parameters: SoftContactsParams = jax_dataclasses.field(
         default_factory=lambda: SoftContactsParams()
@@ -40,15 +39,14 @@
     gravity: jtp.Vector = jax_dataclasses.field(
         default_factory=lambda: jaxsim.physics.default_gravity()
     )
 
 
 @jax_dataclasses.pytree_dataclass
 class JaxSim(JaxsimDataclass):
-
     # Step size stored in ns in order to prevent floats approximation
     step_size_ns: jtp.Int = jax_dataclasses.field(
         default_factory=lambda: jnp.array(1_000_000, dtype=jnp.int64)
     )
 
     # Number of substeps performed at each integration step
     steps_per_run: jtp.Int = jax_dataclasses.static_field(default=1)
@@ -68,66 +66,56 @@
     def build(
         step_size: jtp.Float,
         steps_per_run: jtp.Int = 1,
         velocity_representation: VelRepr = VelRepr.Inertial,
         integrator_type: ode_integration.IntegratorType = ode_integration.IntegratorType.EulerSemiImplicit,
         simulator_data: SimulatorData = None,
     ) -> "JaxSim":
-
         return JaxSim(
             step_size_ns=jnp.array(step_size * 1e9, dtype=jnp.int64),
             steps_per_run=int(steps_per_run),
             velocity_representation=velocity_representation,
             integrator_type=integrator_type,
             data=simulator_data if simulator_data is not None else SimulatorData(),
         )
 
     def reset(self, remove_models: bool = True) -> None:
-
         self.data.time_ns = jnp.zeros_like(self.data.time_ns)
 
         if remove_models:
             self.data.models = dict()
         else:
             _ = [m.zero() for m in self.models()]
 
     def set_step_size(self, step_size: float) -> None:
-
         self.step_size_ns = jnp.array(step_size * 1e9, dtype=jnp.int64)
 
     def dt(self) -> jtp.Float:
-
         return (self.step_size_ns * self.steps_per_run) / 1e9
 
     def time(self) -> jtp.Float:
-
         return self.data.time_ns / 1e9
 
     def gravity(self) -> jtp.Vector:
-
         return self.data.gravity
 
     def model_names(self) -> List[str]:
-
         return list(self.data.models.keys())
 
     def get_model(self, model_name: str) -> Model:
-
         if model_name not in self.data.models.keys():
             raise ValueError(f"Failed to find model '{model_name}'")
 
         return self.data.models[model_name]
 
     def models(self, model_names: List[str] = None) -> List[Model]:
-
         model_names = model_names if model_names is not None else self.model_names()
         return [self.data.models[name] for name in model_names]
 
     def set_gravity(self, gravity: jtp.Vector):
-
         gravity = jnp.array(gravity)
 
         if gravity.size != 3:
             raise ValueError(gravity)
 
         self.data.gravity = gravity
 
@@ -138,15 +126,14 @@
 
     def insert_model_from_sdf(
         self,
         sdf: Union[pathlib.Path, str],
         model_name: str = None,
         considered_joints: List[str] = None,
     ) -> Model:
-
         # Build the model from the input SDF resource
         model = jaxsim.high_level.model.Model.build_from_sdf(
             sdf=sdf,
             model_name=model_name,
             vel_repr=self.velocity_representation,
             considered_joints=considered_joints,
         )
@@ -165,15 +152,14 @@
 
         # Return the newly inserted model
         return self.data.models[model.name()]
 
     def insert_model(
         self, model_description: descriptions.ModelDescription, model_name: str = None
     ) -> Model:
-
         model_name = model_name if model_name is not None else model_description.name
 
         if model_name in self.model_names():
             msg = f"Model '{model_name}' is already part of the simulation"
             raise ValueError(msg)
 
         physics_model = PhysicsModel.build_from(
@@ -188,36 +174,32 @@
 
         self.data.models[model.name()] = model
         self._set_mutability(self._mutability())
 
         return self.data.models[model.name()]
 
     def remove_model(self, model_name: str) -> None:
-
         if model_name not in self.model_names():
             msg = f"Model '{model_name}' is not part of the simulation"
             raise ValueError(msg)
 
         self.data.models.pop(model_name)
         self._set_mutability(self._mutability())
 
     def step(self, clear_inputs: bool = False) -> Dict[str, StepData]:
-
         t0_ns = jnp.array(self.data.time_ns, dtype=jnp.int64)
         dt_ns = jnp.array(self.step_size_ns * self.steps_per_run, dtype=jnp.int64)
 
         tf_ns = t0_ns + dt_ns
 
         # We collect the StepData of all models
         step_data = dict()
 
         for model in self.models():
-
             with model.editable(validate=True) as integrated_model:
-
                 step_data[model.name()] = integrated_model.integrate(
                     t0=jnp.array(t0_ns, dtype=float) / 1e9,
                     tf=jnp.array(tf_ns, dtype=float) / 1e9,
                     sub_steps=self.steps_per_run,
                     integrator_type=self.integrator_type,
                     terrain=self.data.terrain,
                     contact_parameters=self.data.contact_parameters,
@@ -269,15 +251,14 @@
         sim = configure_cb(sim) if configure_cb is not None else sim
 
         # Initialize the carry
         Carry = Tuple[JaxSim, scb.CallbackHandler]
         carry_init: Carry = (sim, callback_handler)
 
         def body_fun(carry: Carry, xs: None) -> Tuple[Carry, jtp.PyTree]:
-
             sim, callback_handler = carry
 
             # Make sure to pass a mutable version of the simulator to the callbacks
             sim = sim.mutable(validate=True)
 
             # Callback: pre-step
             # TODO: should we allow also producing a pre-step output?
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev137/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,37 +15,34 @@
 class SimulatorCallback(abc.ABC):
     pass
 
 
 class ConfigureCallback(SimulatorCallback):
     @property
     def configure_cb(self) -> ConfigureCallbackSignature:
-
         return lambda sim: self.configure(sim=sim)
 
     @abc.abstractmethod
     def configure(self, sim: "jaxsim.JaxSim") -> "jaxsim.JaxSim":
         pass
 
 
 class PreStepCallback(SimulatorCallback):
     @property
     def pre_step_cb(self) -> PreStepCallbackSignature:
-
         return lambda sim: self.pre_step(sim=sim)
 
     @abc.abstractmethod
     def pre_step(self, sim: "jaxsim.JaxSim") -> "jaxsim.JaxSim":
         pass
 
 
 class PostStepCallback(SimulatorCallback):
     @property
     def post_step_cb(self) -> PostStepCallbackSignature:
-
         return lambda sim, step_data: self.post_step(sim=sim, step_data=step_data)
 
     @abc.abstractmethod
     def post_step(
         self, sim: "jaxsim.JaxSim", step_data: Dict[str, StepData]
     ) -> Tuple["jaxsim.JaxSim", jtp.PyTree]:
         pass
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim/typing.py` & `jaxsim-0.1.dev137/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev135/src/jaxsim/utils.py` & `jaxsim-0.1.dev137/src/jaxsim/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,50 +70,42 @@
         return (
             self.__mutability__ is Mutability.MUTABLE
             if validate
             else self.__mutability__ is Mutability.MUTABLE_NO_VALIDATION
         )
 
     def set_mutability(self, mutable: bool = True, validate: bool = False) -> None:
-
         if not mutable:
             mutability = Mutability.FROZEN
         else:
             mutability = (
                 Mutability.MUTABLE if validate else Mutability.MUTABLE_NO_VALIDATION
             )
 
         self._set_mutability(mutability=mutability)
 
     def _mutability(self) -> Mutability:
-
         return self.__mutability__
 
     def _set_mutability(self, mutability: Mutability) -> None:
-
         jax_dataclasses._copy_and_mutate._mark_mutable(
             self, mutable=mutability, visited=set()
         )
 
     def mutable(self: T, mutable: bool = True, validate: bool = False) -> T:
-
         self.set_mutability(mutable=mutable, validate=validate)
         return self
 
     def copy(self: T) -> T:
-
         obj = jax.tree_util.tree_map(lambda leaf: leaf, self)
         obj._set_mutability(mutability=self._mutability())
         return obj
 
     def replace(self: T, validate: bool = True, **kwargs) -> T:
-
         with self.editable(validate=validate) as obj:
-
             _ = [obj.__setattr__(k, copy.copy(v)) for k, v in kwargs.items()]
 
         obj._set_mutability(mutability=self._mutability())
         return obj
 
     def flatten(self: T) -> jtp.VectorJax:
-
         return jax.flatten_util.ravel_pytree(self)[0]
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev137/src/jaxsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev135
+Version: 0.1.dev137
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev135/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev137/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

