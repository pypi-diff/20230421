# Comparing `tmp/jaxsim-0.1.dev137.tar.gz` & `tmp/jaxsim-0.1.dev142.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxsim-0.1.dev137.tar", last modified: Fri Apr 21 08:29:59 2023, max compression
+gzip compressed data, was "jaxsim-0.1.dev142.tar", last modified: Fri Apr 21 10:02:58 2023, max compression
```

## Comparing `jaxsim-0.1.dev137.tar` & `jaxsim-0.1.dev142.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/jaxsim/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/jaxsim/high_level/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/link.py
--rw-r--r--   0 runner    (1001) docker     (123)    33908 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/high_level/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/plucker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/math/skew.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/kinematic_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/physics/algos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/aba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/crba.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/jacobian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/rnea.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/soft_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/terrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/algos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.327850 jaxsim-0.1.dev137/src/jaxsim/physics/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/ground_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/src/jaxsim/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/integrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/ode_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/ode_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/simulator_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.331851 jaxsim-0.1.dev137/src/jaxsim/sixd/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/sixd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-21 08:29:43.000000 jaxsim-0.1.dev137/src/jaxsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:29:59.323850 jaxsim-0.1.dev137/src/jaxsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 08:29:59.000000 jaxsim-0.1.dev137/src/jaxsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.685919 jaxsim-0.1.dev142/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 10:02:58.697920 jaxsim-0.1.dev142/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-21 10:02:58.697920 jaxsim-0.1.dev142/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.685919 jaxsim-0.1.dev142/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/high_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34435 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/high_level/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/plucker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/math/skew.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18763 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/kinematic_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/physics/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/aba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/crba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/jacobian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/rnea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/soft_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/algos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/physics/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/ground_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/ode_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/ode_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/simulator_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.693920 jaxsim-0.1.dev142/src/jaxsim/sixd/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/sixd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-21 10:02:41.000000 jaxsim-0.1.dev142/src/jaxsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:02:58.689920 jaxsim-0.1.dev142/src/jaxsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 10:02:58.000000 jaxsim-0.1.dev142/src/jaxsim.egg-info/top_level.txt
```

### Comparing `jaxsim-0.1.dev137/.github/workflows/ci_cd.yml` & `jaxsim-0.1.dev142/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/.github/workflows/style.yml` & `jaxsim-0.1.dev142/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/.gitignore` & `jaxsim-0.1.dev142/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/LICENSE` & `jaxsim-0.1.dev142/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/PKG-INFO` & `jaxsim-0.1.dev142/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev137
+Version: 0.1.dev142
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev137/README.md` & `jaxsim-0.1.dev142/README.md`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/setup.cfg` & `jaxsim-0.1.dev142/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/__init__.py` & `jaxsim-0.1.dev142/src/jaxsim/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/high_level/joint.py` & `jaxsim-0.1.dev142/src/jaxsim/high_level/joint.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import jaxsim.parsers.descriptions as descriptions
 import jaxsim.typing as jtp
 from jaxsim.utils import JaxsimDataclass
 
 
 @jax_dataclasses.pytree_dataclass
 class Joint(JaxsimDataclass):
+    """
+    High-level class to operate on a single joint of a simulated model.
+    """
+
     joint_description: descriptions.JointDescription = jax_dataclasses.static_field()
     parent_model: "jaxsim.high_level.model.Model" = jax_dataclasses.field(
         default=None, repr=False, compare=False
     )
 
     def valid(self) -> bool:
         return self.parent_model is not None
```

### Comparing `jaxsim-0.1.dev137/src/jaxsim/high_level/link.py` & `jaxsim-0.1.dev142/src/jaxsim/high_level/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from jaxsim.utils import JaxsimDataclass
 
 from .common import VelRepr
 
 
 @jax_dataclasses.pytree_dataclass
 class Link(JaxsimDataclass):
+    """
+    High-level class to operate on a single link of a simulated model.
+    """
+
     link_description: descriptions.LinkDescription = jax_dataclasses.static_field()
     parent_model: "jaxsim.high_level.model.Model" = jax_dataclasses.field(
         default=None, repr=False, compare=False
     )
 
     def valid(self) -> bool:
         return self.parent_model is not None
```

### Comparing `jaxsim-0.1.dev137/src/jaxsim/high_level/model.py` & `jaxsim-0.1.dev142/src/jaxsim/high_level/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,20 +23,34 @@
 from jaxsim.utils import JaxsimDataclass, Mutability
 
 from .common import VelRepr
 
 
 @jax_dataclasses.pytree_dataclass
 class ModelData(JaxsimDataclass):
+    """
+    Class used to store the model state and input at a given time.
+    """
+
     model_state: jaxsim.physics.model.physics_model_state.PhysicsModelState
     model_input: jaxsim.physics.model.physics_model_state.PhysicsModelInput
     contact_state: jaxsim.physics.algos.soft_contacts.SoftContactsState
 
     @staticmethod
     def zero(physics_model: physics.model.physics_model.PhysicsModel) -> "ModelData":
+        """
+        Return a ModelData object with all fields set to zero and initialized with the right shape.
+
+        Args:
+            physics_model: The considered physics model.
+
+        Returns:
+            The zero ModelData object of the given physics model.
+        """
+
         return ModelData(
             model_state=jaxsim.physics.model.physics_model_state.PhysicsModelState.zero(
                 physics_model=physics_model
             ),
             model_input=jaxsim.physics.model.physics_model_state.PhysicsModelInput.zero(
                 physics_model=physics_model
             ),
@@ -44,14 +58,18 @@
                 physics_model=physics_model
             ),
         )
 
 
 @jax_dataclasses.pytree_dataclass
 class StepData(JaxsimDataclass):
+    """
+    Class used to store the data computed at each step of the simulation.
+    """
+
     t0: float
     tf: float
     dt: float
 
     # Starting model data and real input (tau, f_ext) computed at t0
     t0_model_data: ModelData = dataclasses.field(repr=False)
     t0_model_input_real: jaxsim.physics.model.physics_model_state.PhysicsModelInput = (
@@ -73,14 +91,18 @@
     )
 
     aux: Dict[str, Any] = dataclasses.field(default_factory=dict)
 
 
 @jax_dataclasses.pytree_dataclass
 class Model(JaxsimDataclass):
+    """
+    High-level class to operate on a simulated model.
+    """
+
     model_name: str = jax_dataclasses.static_field()
     physics_model: physics.model.physics_model.PhysicsModel = dataclasses.field(
         repr=False
     )
 
     velocity_representation: VelRepr = jax_dataclasses.static_field(
         default=VelRepr.Mixed
```

### Comparing `jaxsim-0.1.dev137/src/jaxsim/logging.py` & `jaxsim-0.1.dev142/src/jaxsim/logging.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/adjoint.py` & `jaxsim-0.1.dev142/src/jaxsim/math/adjoint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/conv.py` & `jaxsim-0.1.dev142/src/jaxsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/cross.py` & `jaxsim-0.1.dev142/src/jaxsim/math/cross.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/inertia.py` & `jaxsim-0.1.dev142/src/jaxsim/math/inertia.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/joint.py` & `jaxsim-0.1.dev142/src/jaxsim/math/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/plucker.py` & `jaxsim-0.1.dev142/src/jaxsim/math/plucker.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/quaternion.py` & `jaxsim-0.1.dev142/src/jaxsim/math/quaternion.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/rotation.py` & `jaxsim-0.1.dev142/src/jaxsim/math/rotation.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/math/skew.py` & `jaxsim-0.1.dev142/src/jaxsim/math/skew.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/collision.py` & `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/collision.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/joint.py` & `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/joint.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/link.py` & `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/link.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/parsers/descriptions/model.py` & `jaxsim-0.1.dev142/src/jaxsim/parsers/descriptions/model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/parsers/kinematic_graph.py` & `jaxsim-0.1.dev142/src/jaxsim/parsers/kinematic_graph.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/parser.py` & `jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/parser.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/parsers/sdf/utils.py` & `jaxsim-0.1.dev142/src/jaxsim/parsers/sdf/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/aba.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/aba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/crba.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/crba.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/forward_kinematics.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/jacobian.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/jacobian.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/rnea.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/rnea.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/soft_contacts.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/soft_contacts.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/terrain.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/terrain.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/algos/utils.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/algos/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/model/ground_contact.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/model/ground_contact.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/physics/model/physics_model_state.py` & `jaxsim-0.1.dev142/src/jaxsim/physics/model/physics_model_state.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/simulation/integrators.py` & `jaxsim-0.1.dev142/src/jaxsim/simulation/integrators.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,28 @@
 def odeint_euler_one_step(
     dx_dt: StateDerivativeCallable,
     x0: State,
     t0: Time,
     tf: Time,
     num_sub_steps: int = 1,
 ) -> Tuple[State, Dict[str, Any]]:
+    """
+    Forward Euler integrator.
+
+    Args:
+        dx_dt: Callable that computes the state derivative.
+        x0: Initial state.
+        t0: Initial time.
+        tf: Final time.
+        num_sub_steps: Number of sub-steps to break the integration into.
+
+    Returns:
+        The final state and a dictionary including auxiliary data at t0.
+    """
+
     # Compute the sub-step size.
     # We break dt in configurable sub-steps.
     dt = tf - t0
     sub_step_dt = dt / num_sub_steps
 
     # Initialize the carry
     Carry = Tuple[State, Time]
@@ -75,14 +89,28 @@
 def odeint_rk4_one_step(
     dx_dt: StateDerivativeCallable,
     x0: State,
     t0: Time,
     tf: Time,
     num_sub_steps: int = 1,
 ) -> Tuple[State, Dict[str, Any]]:
+    """
+    Runge-Kutta 4 integrator.
+
+    Args:
+        dx_dt: Callable that computes the state derivative.
+        x0: Initial state.
+        t0: Initial time.
+        tf: Final time.
+        num_sub_steps: Number of sub-steps to break the integration into.
+
+    Returns:
+        The final state and a dictionary including auxiliary data at t0.
+    """
+
     # Compute the sub-step size.
     # We break dt in configurable sub-steps.
     dt = tf - t0
     sub_step_dt = dt / num_sub_steps
 
     # Initialize the carry
     Carry = Tuple[State, Time]
@@ -131,14 +159,28 @@
 def odeint_euler_semi_implicit_one_step(
     dx_dt: StateDerivativeCallable,
     x0: ODEState,
     t0: Time,
     tf: Time,
     num_sub_steps: int = 1,
 ) -> Tuple[ODEState, Dict[str, Any]]:
+    """
+    Semi-implicit Euler integrator.
+
+    Args:
+        dx_dt: Callable that computes the state derivative.
+        x0: Initial state.
+        t0: Initial time.
+        tf: Final time.
+        num_sub_steps: Number of sub-steps to break the integration into.
+
+    Returns:
+        The final state and a dictionary including auxiliary data at t0.
+    """
+
     # Compute the sub-step size.
     # We break dt in configurable sub-steps.
     dt = tf - t0
     sub_step_dt = dt / num_sub_steps
 
     # Initialize the carry
     Carry = Tuple[ODEState, Time]
@@ -241,14 +283,26 @@
 
 
 def integrate_single_step_over_horizon(
     integrator_single_step: Callable[[Time, Time, State], Tuple[State, Dict[str, Any]]],
     t: TimeHorizon,
     x0: State,
 ) -> Tuple[State, Dict[str, Any]]:
+    """
+    Integrate a single-step integrator over a given horizon.
+
+    Args:
+        integrator_single_step: A single-step integrator.
+        t: The vector of time instants of the integration horizon.
+        x0: The initial state of the integration horizon.
+
+    Returns:
+        The final state and auxiliary data produced by the integrator.
+    """
+
     # Initialize the carry
     carry_init = (x0, t)
 
     def body_fun(carry: Tuple, idx: int) -> Tuple[Tuple, jtp.PyTree]:
         # Unpack the carry
         x_t0, horizon = carry
 
@@ -282,14 +336,30 @@
     func,
     y0: State,
     t: TimeHorizon,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False
 ) -> Union[State, Tuple[State, Dict[str, Any]]]:
+    """
+    Integrate a system of ODEs using the Euler method.
+
+    Args:
+        func: A function that computes the time-derivative of the state.
+        y0: The initial state.
+        t: The vector of time instants of the integration horizon.
+        *args: Additional arguments to be passed to the function func.
+        num_sub_steps: The number of sub-steps to be performed within each integration step.
+        return_aux: Whether to return the auxiliary data produced by the integrator.
+
+    Returns:
+        The state of the system at the end of the integration horizon, and optionally
+        the auxiliary data produced by the integrator.
+    """
+
     # Close func over additional inputs and parameters
     dx_dt_closure_aux = lambda x, ts: func(x, ts, *args)
 
     # Close one-step integration over its arguments
     integrator_single_step = lambda t0, tf, x0: odeint_euler_one_step(
         dx_dt=dx_dt_closure_aux, x0=x0, t0=t0, tf=tf, num_sub_steps=num_sub_steps
     )
@@ -306,14 +376,30 @@
     func,
     y0: State,
     t: TimeHorizon,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False
 ) -> Union[State, Tuple[State, Dict[str, Any]]]:
+    """
+    Integrate a system of ODEs using the Semi-Implicit Euler method.
+
+    Args:
+        func: A function that computes the time-derivative of the state.
+        y0: The initial state.
+        t: The vector of time instants of the integration horizon.
+        *args: Additional arguments to be passed to the function func.
+        num_sub_steps: The number of sub-steps to be performed within each integration step.
+        return_aux: Whether to return the auxiliary data produced by the integrator.
+
+    Returns:
+        The state of the system at the end of the integration horizon, and optionally
+        the auxiliary data produced by the integrator.
+    """
+
     # Close func over additional inputs and parameters
     dx_dt_closure_aux = lambda x, ts: func(x, ts, *args)
 
     # Close one-step integration over its arguments
     integrator_single_step = lambda t0, tf, x0: odeint_euler_semi_implicit_one_step(
         dx_dt=dx_dt_closure_aux, x0=x0, t0=t0, tf=tf, num_sub_steps=num_sub_steps
     )
@@ -330,14 +416,30 @@
     func,
     y0: State,
     t: TimeHorizon,
     *args,
     num_sub_steps: int = 1,
     return_aux: bool = False
 ) -> Union[State, Tuple[State, Dict[str, Any]]]:
+    """
+    Integrate a system of ODEs using the Runge-Kutta 4 method.
+
+    Args:
+        func: A function that computes the time-derivative of the state.
+        y0: The initial state.
+        t: The vector of time instants of the integration horizon.
+        *args: Additional arguments to be passed to the function func.
+        num_sub_steps: The number of sub-steps to be performed within each integration step.
+        return_aux: Whether to return the auxiliary data produced by the integrator.
+
+    Returns:
+        The state of the system at the end of the integration horizon, and optionally
+        the auxiliary data produced by the integrator.
+    """
+
     # Close func over additional inputs and parameters
     dx_dt_closure = lambda x, ts: func(x, ts, *args)
 
     # Close one-step integration over its arguments
     integrator_single_step = lambda t0, tf, x0: odeint_rk4_one_step(
         dx_dt=dx_dt_closure, x0=x0, t0=t0, tf=tf, num_sub_steps=num_sub_steps
     )
```

### Comparing `jaxsim-0.1.dev137/src/jaxsim/simulation/ode.py` & `jaxsim-0.1.dev142/src/jaxsim/simulation/ode.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,14 +18,30 @@
 
 def compute_contact_forces(
     physics_model: PhysicsModel,
     ode_state: ode_data.ODEState,
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     terrain: Terrain = FlatTerrain(),
 ) -> Tuple[jtp.Matrix, jtp.Matrix, jtp.Matrix]:
+    """
+    Compute the contact forces acting on the collidable points of the model.
+
+    Args:
+        physics_model: The physics model to consider.
+        ode_state: The state of the ODE corresponding to the physics model.
+        soft_contacts_params: The parameters of the soft contacts model.
+        terrain: The terrain model.
+
+    Returns:
+        A tuple containing:
+        - The contact forces expressed in the world frame acting on the model's links.
+        - The derivative of the tangential deformation of the terrain dynamics.
+        - The contact forces expressed in the world frame acting on the model's collidable points.
+    """
+
     # Compute position and linear mixed velocity of all model's collidable points
     # collidable_points_kinematics
     pos_cp, vel_cp = collidable_points_pos_vel(
         model=physics_model,
         q=ode_state.physics_model.joint_positions,
         qd=ode_state.physics_model.joint_velocities,
         xfb=ode_state.physics_model.xfb(),
@@ -60,14 +76,31 @@
     x: ode_data.ODEState,
     t: Optional[jtp.Float],
     physics_model: PhysicsModel,
     soft_contacts_params: SoftContactsParams = SoftContactsParams(),
     ode_input: ode_data.ODEInput = None,
     terrain: Terrain = FlatTerrain(),
 ) -> Tuple[ode_data.ODEState, Dict[str, Any]]:
+    """
+    Compute the state derivative of the ODE corresponding to the physics model.
+
+    Args:
+        x: The state of the ODE.
+        t: The current time.
+        physics_model: The physics model to consider.
+        soft_contacts_params: The parameters of the soft contacts model.
+        ode_input: The input of the ODE.
+        terrain: The terrain model.
+
+    Returns:
+        A tuple containing:
+        - The state derivative of the ODE.
+        - A dictionary containing auxiliary information.
+    """
+
     if t is not None and isinstance(t, np.ndarray) and t.size != 1:
         raise ValueError(t.size)
 
     # Initialize arguments
     ode_state = x
     ode_input = (
         ode_input
@@ -148,14 +181,15 @@
 
     # Compute the total forces applied to the bodies
     total_forces = ode_input.physics_model.f_ext + contact_forces_links
 
     # Compute the joint torques to actuate
     tau = ode_input.physics_model.tau + tau_friction + tau_limit
 
+    # Compute forward dynamics with the ABA algorithm
     W_a_WB, qdd = algos.aba.aba(
         model=physics_model,
         xfb=ode_state.physics_model.xfb(),
         q=ode_state.physics_model.joint_positions,
         qd=ode_state.physics_model.joint_velocities,
         tau=tau,
         f_ext=total_forces,
@@ -194,34 +228,40 @@
     xd_fb = jnp.hstack([W_Qd_B, BW_v_WB, W_a_WB.squeeze()]).squeeze()
 
     # =====================================
     # Build the full derivative of ODEState
     # =====================================
 
     def fix_one_dof(vector: jtp.Vector) -> Optional[jtp.Vector]:
+        """Fix the shape of computed quantities for models with just 1 DoF."""
+
         if vector is None:
             return None
 
         return jnp.array([vector]) if vector.shape == () else vector
 
+    # Fill the PhysicsModelState object included in the input ODEState to store the
+    # returned PhysicsModelState derivative
     physics_model_state_derivative = ode_state.physics_model.replace(
         joint_positions=fix_one_dof(ode_state.physics_model.joint_velocities.squeeze()),
         joint_velocities=fix_one_dof(qdd.squeeze()),
         base_quaternion=xd_fb.squeeze()[0:4],
         base_position=xd_fb.squeeze()[4:7],
         base_angular_velocity=xd_fb.squeeze()[10:13],
         base_linear_velocity=xd_fb.squeeze()[7:10],
     )
 
+    # Fill the SoftContactsState object included in the input ODEState to store the
+    # returned SoftContactsState derivative
     soft_contacts_state_derivative = ode_state.soft_contacts.replace(
         tangential_deformation=tangential_deformation_dot.squeeze(),
     )
 
     # We store the state derivative using the ODEState class so that the pytree
-    # structure remains consistent, and it allows using our generic pytree integrators
+    # structure remains consistent, allowing to use our generic pytree integrators
     state_derivative = ode_data.ODEState(
         physics_model=physics_model_state_derivative,
         soft_contacts=soft_contacts_state_derivative,
     )
 
     # ===============================
     # Build auxiliary data and return
```

### Comparing `jaxsim-0.1.dev137/src/jaxsim/simulation/ode_data.py` & `jaxsim-0.1.dev142/src/jaxsim/simulation/ode_data.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/simulation/ode_integration.py` & `jaxsim-0.1.dev142/src/jaxsim/simulation/ode_integration.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/simulation/simulator_callbacks.py` & `jaxsim-0.1.dev142/src/jaxsim/simulation/simulator_callbacks.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/typing.py` & `jaxsim-0.1.dev142/src/jaxsim/typing.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim/utils.py` & `jaxsim-0.1.dev142/src/jaxsim/utils.py`

 * *Files identical despite different names*

### Comparing `jaxsim-0.1.dev137/src/jaxsim.egg-info/PKG-INFO` & `jaxsim-0.1.dev142/src/jaxsim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxsim
-Version: 0.1.dev137
+Version: 0.1.dev142
 Summary: A physics engine in reduced coordinates implemented with JAX.
 Home-page: https://github.com/ami-iit/jaxsim
 Author: Diego Ferigo
 Author-email: diego.ferigo@iit.it
 License: BSD
 Project-URL: Changelog, https://github.com/ami-iit/jaxsim/releases
 Project-URL: Source, https://github.com/ami-iit/jaxsim
```

### Comparing `jaxsim-0.1.dev137/src/jaxsim.egg-info/SOURCES.txt` & `jaxsim-0.1.dev142/src/jaxsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

