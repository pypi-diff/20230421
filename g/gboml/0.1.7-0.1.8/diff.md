# Comparing `tmp/gboml-0.1.7.tar.gz` & `tmp/gboml-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gboml-0.1.7.tar", last modified: Sun Mar 26 18:01:21 2023, max compression
+gzip compressed data, was "gboml-0.1.8.tar", last modified: Fri Apr 21 07:41:20 2023, max compression
```

## Comparing `gboml-0.1.7.tar` & `gboml-0.1.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.384772 gboml-0.1.7/
--rw-r--r--   0 bmiftari   (501) staff       (20)      564 2023-02-20 09:58:31.000000 gboml-0.1.7/AUTHORS
--rw-r--r--   0 bmiftari   (501) staff       (20)     1162 2023-02-20 09:58:31.000000 gboml-0.1.7/LICENSE.txt
--rw-r--r--   0 bmiftari   (501) staff       (20)       96 2023-02-20 09:58:31.000000 gboml-0.1.7/MANIFEST.in
--rw-r--r--   0 bmiftari   (501) staff       (20)     4331 2023-03-26 18:01:21.384617 gboml-0.1.7/PKG-INFO
--rw-r--r--   0 bmiftari   (501) staff       (20)     3288 2023-02-20 09:58:31.000000 gboml-0.1.7/README.md
--rw-r--r--   0 bmiftari   (501) staff       (20)       91 2023-02-20 09:58:31.000000 gboml-0.1.7/pyproject.toml
--rw-r--r--   0 bmiftari   (501) staff       (20)       27 2023-02-20 09:58:31.000000 gboml-0.1.7/requirements.txt
--rw-r--r--   0 bmiftari   (501) staff       (20)       38 2023-03-26 18:01:21.384817 gboml-0.1.7/setup.cfg
--rw-r--r--   0 bmiftari   (501) staff       (20)     1864 2023-02-20 09:58:31.000000 gboml-0.1.7/setup.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.373276 gboml-0.1.7/src/
--rw-r--r--   0 bmiftari   (501) staff       (20)      210 2023-02-20 09:58:31.000000 gboml-0.1.7/src/__init__.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.374457 gboml-0.1.7/src/gboml/
--rw-r--r--   0 bmiftari   (501) staff       (20)      585 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/__init__.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.377148 gboml-0.1.7/src/gboml/compiler/
--rw-r--r--   0 bmiftari   (501) staff       (20)     1642 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/__init__.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.380187 gboml-0.1.7/src/gboml/compiler/classes/
--rw-r--r--   0 bmiftari   (501) staff       (20)      946 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/classes/__init__.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     5788 2023-03-26 15:50:21.000000 gboml-0.1.7/src/gboml/compiler/classes/condition.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     3943 2023-03-26 15:48:52.000000 gboml-0.1.7/src/gboml/compiler/classes/constraint.py
--rw-r--r--   0 bmiftari   (501) staff       (20)      944 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/classes/error.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    32537 2023-03-26 16:20:45.000000 gboml-0.1.7/src/gboml/compiler/classes/expression.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    42754 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/classes/factor.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     5252 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/classes/identifier.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     7330 2023-03-26 15:49:02.000000 gboml-0.1.7/src/gboml/compiler/classes/link.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     3084 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/classes/mdp.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    11578 2023-03-26 16:08:00.000000 gboml-0.1.7/src/gboml/compiler/classes/node.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     2326 2023-03-26 15:48:41.000000 gboml-0.1.7/src/gboml/compiler/classes/objective.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     3310 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/classes/parameter.py
--rw-r--r--   0 bmiftari   (501) staff       (20)      900 2023-03-26 16:18:27.000000 gboml-0.1.7/src/gboml/compiler/classes/parent.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     8497 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/classes/program.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    12014 2023-03-26 15:50:51.000000 gboml-0.1.7/src/gboml/compiler/classes/time_obj.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     3765 2023-03-26 16:02:08.000000 gboml-0.1.7/src/gboml/compiler/classes/variable.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     4102 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/gboml_compiler.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     5095 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/gboml_lexer.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    16943 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/gboml_matrix_generation.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    22161 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/gboml_parser.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    80254 2023-03-26 16:04:57.000000 gboml-0.1.7/src/gboml/compiler/gboml_semantic.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.380721 gboml-0.1.7/src/gboml/compiler/ply/
--rw-r--r--   0 bmiftari   (501) staff       (20)      116 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/ply/__init__.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    35241 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/ply/lex.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    98438 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/ply/yacc.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     5827 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/compiler/utils.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    40129 2023-03-26 17:50:24.000000 gboml-0.1.7/src/gboml/gboml_graph.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    10313 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/gboml_main.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.381284 gboml-0.1.7/src/gboml/output/
--rw-r--r--   0 bmiftari   (501) staff       (20)      256 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/output/__init__.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    22418 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/output/gboml_output.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.384358 gboml-0.1.7/src/gboml/solver_api/
--rw-r--r--   0 bmiftari   (501) staff       (20)     1923 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/__init__.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     8110 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/cbc_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     5658 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/clp_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)       28 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/cplex.opt
--rw-r--r--   0 bmiftari   (501) staff       (20)    10438 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/cplex_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     8131 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/dsp_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    17546 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/dsppy.py
--rw-r--r--   0 bmiftari   (501) staff       (20)       40 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/gurobi.opt
--rw-r--r--   0 bmiftari   (501) staff       (20)     8222 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/gurobi_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)       76 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/highs.opt
--rw-r--r--   0 bmiftari   (501) staff       (20)     8331 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/highs_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    17736 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/pycbc.py
--rw-r--r--   0 bmiftari   (501) staff       (20)    46263 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/pyhighs.py
--rw-r--r--   0 bmiftari   (501) staff       (20)     3463 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/scipy_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)       27 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/xpress.opt
--rw-r--r--   0 bmiftari   (501) staff       (20)     8896 2023-02-20 09:58:31.000000 gboml-0.1.7/src/gboml/solver_api/xpress_solver.py
--rw-r--r--   0 bmiftari   (501) staff       (20)      308 2023-03-26 17:54:46.000000 gboml-0.1.7/src/gboml/version.py
-drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-03-26 18:01:21.375388 gboml-0.1.7/src/gboml.egg-info/
--rw-r--r--   0 bmiftari   (501) staff       (20)     4331 2023-03-26 18:01:21.000000 gboml-0.1.7/src/gboml.egg-info/PKG-INFO
--rw-r--r--   0 bmiftari   (501) staff       (20)     1963 2023-03-26 18:01:21.000000 gboml-0.1.7/src/gboml.egg-info/SOURCES.txt
--rw-r--r--   0 bmiftari   (501) staff       (20)        1 2023-03-26 18:01:21.000000 gboml-0.1.7/src/gboml.egg-info/dependency_links.txt
--rw-r--r--   0 bmiftari   (501) staff       (20)       37 2023-03-26 18:01:21.000000 gboml-0.1.7/src/gboml.egg-info/entry_points.txt
--rw-r--r--   0 bmiftari   (501) staff       (20)      132 2023-03-26 18:01:21.000000 gboml-0.1.7/src/gboml.egg-info/requires.txt
--rw-r--r--   0 bmiftari   (501) staff       (20)        6 2023-03-26 18:01:21.000000 gboml-0.1.7/src/gboml.egg-info/top_level.txt
--rw-r--r--   0 bmiftari   (501) staff       (20)      966 2023-02-20 09:58:31.000000 gboml-0.1.7/src/main.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.912229 gboml-0.1.8/
+-rw-r--r--   0 bmiftari   (501) staff       (20)      564 2023-02-20 09:58:31.000000 gboml-0.1.8/AUTHORS
+-rw-r--r--   0 bmiftari   (501) staff       (20)     1162 2023-02-20 09:58:31.000000 gboml-0.1.8/LICENSE.txt
+-rw-r--r--   0 bmiftari   (501) staff       (20)       96 2023-02-20 09:58:31.000000 gboml-0.1.8/MANIFEST.in
+-rw-r--r--   0 bmiftari   (501) staff       (20)     4331 2023-04-21 07:41:20.912064 gboml-0.1.8/PKG-INFO
+-rw-r--r--   0 bmiftari   (501) staff       (20)     3288 2023-02-20 09:58:31.000000 gboml-0.1.8/README.md
+-rw-r--r--   0 bmiftari   (501) staff       (20)       91 2023-02-20 09:58:31.000000 gboml-0.1.8/pyproject.toml
+-rw-r--r--   0 bmiftari   (501) staff       (20)       27 2023-02-20 09:58:31.000000 gboml-0.1.8/requirements.txt
+-rw-r--r--   0 bmiftari   (501) staff       (20)       38 2023-04-21 07:41:20.912268 gboml-0.1.8/setup.cfg
+-rw-r--r--   0 bmiftari   (501) staff       (20)     1864 2023-02-20 09:58:31.000000 gboml-0.1.8/setup.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.898199 gboml-0.1.8/src/
+-rw-r--r--   0 bmiftari   (501) staff       (20)      210 2023-02-20 09:58:31.000000 gboml-0.1.8/src/__init__.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.899616 gboml-0.1.8/src/gboml/
+-rw-r--r--   0 bmiftari   (501) staff       (20)      585 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/__init__.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.902544 gboml-0.1.8/src/gboml/compiler/
+-rw-r--r--   0 bmiftari   (501) staff       (20)     1642 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/__init__.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.906518 gboml-0.1.8/src/gboml/compiler/classes/
+-rw-r--r--   0 bmiftari   (501) staff       (20)      946 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/classes/__init__.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     5788 2023-03-26 15:50:21.000000 gboml-0.1.8/src/gboml/compiler/classes/condition.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     3943 2023-03-26 15:48:52.000000 gboml-0.1.8/src/gboml/compiler/classes/constraint.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)      944 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/classes/error.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    32537 2023-03-26 16:20:45.000000 gboml-0.1.8/src/gboml/compiler/classes/expression.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    42754 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/classes/factor.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     5252 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/classes/identifier.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     8006 2023-04-19 14:12:54.000000 gboml-0.1.8/src/gboml/compiler/classes/link.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     3084 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/classes/mdp.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    12254 2023-04-19 14:10:11.000000 gboml-0.1.8/src/gboml/compiler/classes/node.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     2326 2023-03-26 15:48:41.000000 gboml-0.1.8/src/gboml/compiler/classes/objective.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     3310 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/classes/parameter.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)      900 2023-03-26 16:18:27.000000 gboml-0.1.8/src/gboml/compiler/classes/parent.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     8497 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/classes/program.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    12014 2023-03-26 15:50:51.000000 gboml-0.1.8/src/gboml/compiler/classes/time_obj.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     3765 2023-03-26 16:02:08.000000 gboml-0.1.8/src/gboml/compiler/classes/variable.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     4102 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/gboml_compiler.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     5095 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/gboml_lexer.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    16943 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/gboml_matrix_generation.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    22161 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/gboml_parser.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    80254 2023-03-26 16:04:57.000000 gboml-0.1.8/src/gboml/compiler/gboml_semantic.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.907157 gboml-0.1.8/src/gboml/compiler/ply/
+-rw-r--r--   0 bmiftari   (501) staff       (20)      116 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/ply/__init__.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    35241 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/ply/lex.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    98438 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/ply/yacc.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     5827 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/compiler/utils.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    40129 2023-03-26 17:50:24.000000 gboml-0.1.8/src/gboml/gboml_graph.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    11290 2023-04-21 07:33:35.000000 gboml-0.1.8/src/gboml/gboml_main.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.907623 gboml-0.1.8/src/gboml/output/
+-rw-r--r--   0 bmiftari   (501) staff       (20)      256 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/output/__init__.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    22403 2023-04-18 10:27:11.000000 gboml-0.1.8/src/gboml/output/gboml_output.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.911798 gboml-0.1.8/src/gboml/solver_api/
+-rw-r--r--   0 bmiftari   (501) staff       (20)     1923 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/__init__.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     8240 2023-04-17 09:10:57.000000 gboml-0.1.8/src/gboml/solver_api/cbc_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     5658 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/clp_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)       28 2023-04-18 11:17:49.000000 gboml-0.1.8/src/gboml/solver_api/cplex.opt
+-rw-r--r--   0 bmiftari   (501) staff       (20)    12211 2023-04-18 10:04:06.000000 gboml-0.1.8/src/gboml/solver_api/cplex_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     8222 2023-04-17 09:29:42.000000 gboml-0.1.8/src/gboml/solver_api/dsp_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    17546 2023-04-17 09:29:51.000000 gboml-0.1.8/src/gboml/solver_api/dsppy.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)       40 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/gurobi.opt
+-rw-r--r--   0 bmiftari   (501) staff       (20)     8222 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/gurobi_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)       76 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/highs.opt
+-rw-r--r--   0 bmiftari   (501) staff       (20)     8423 2023-04-17 09:09:09.000000 gboml-0.1.8/src/gboml/solver_api/highs_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    17736 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/pycbc.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)    46263 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/pyhighs.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)     3463 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/scipy_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)       27 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/xpress.opt
+-rw-r--r--   0 bmiftari   (501) staff       (20)     8896 2023-02-20 09:58:31.000000 gboml-0.1.8/src/gboml/solver_api/xpress_solver.py
+-rw-r--r--   0 bmiftari   (501) staff       (20)      308 2023-04-21 07:39:54.000000 gboml-0.1.8/src/gboml/version.py
+drwxr-xr-x   0 bmiftari   (501) staff       (20)        0 2023-04-21 07:41:20.900507 gboml-0.1.8/src/gboml.egg-info/
+-rw-r--r--   0 bmiftari   (501) staff       (20)     4331 2023-04-21 07:41:20.000000 gboml-0.1.8/src/gboml.egg-info/PKG-INFO
+-rw-r--r--   0 bmiftari   (501) staff       (20)     1963 2023-04-21 07:41:20.000000 gboml-0.1.8/src/gboml.egg-info/SOURCES.txt
+-rw-r--r--   0 bmiftari   (501) staff       (20)        1 2023-04-21 07:41:20.000000 gboml-0.1.8/src/gboml.egg-info/dependency_links.txt
+-rw-r--r--   0 bmiftari   (501) staff       (20)       37 2023-04-21 07:41:20.000000 gboml-0.1.8/src/gboml.egg-info/entry_points.txt
+-rw-r--r--   0 bmiftari   (501) staff       (20)      132 2023-04-21 07:41:20.000000 gboml-0.1.8/src/gboml.egg-info/requires.txt
+-rw-r--r--   0 bmiftari   (501) staff       (20)        6 2023-04-21 07:41:20.000000 gboml-0.1.8/src/gboml.egg-info/top_level.txt
+-rw-r--r--   0 bmiftari   (501) staff       (20)      966 2023-02-20 09:58:31.000000 gboml-0.1.8/src/main.py
```

### Comparing `gboml-0.1.7/AUTHORS` & `gboml-0.1.8/AUTHORS`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/LICENSE.txt` & `gboml-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/PKG-INFO` & `gboml-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gboml
-Version: 0.1.7
+Version: 0.1.8
 Summary: GBOML: Graph-Based Optimization Modeling Language
 Home-page: https://gitlab.uliege.be/smart_grids/public/gboml
 Author: Bardhyl Miftari, Mathias Berger, Hatim Djelassi, Damien Ernst
 Author-email: bmiftari@uliege.be
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gboml-0.1.7/README.md` & `gboml-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/setup.py` & `gboml-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/__init__.py` & `gboml-0.1.8/src/gboml/__init__.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/__init__.py` & `gboml-0.1.8/src/gboml/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/__init__.py` & `gboml-0.1.8/src/gboml/compiler/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/condition.py` & `gboml-0.1.8/src/gboml/compiler/classes/condition.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/constraint.py` & `gboml-0.1.8/src/gboml/compiler/classes/constraint.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/error.py` & `gboml-0.1.8/src/gboml/compiler/classes/error.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/expression.py` & `gboml-0.1.8/src/gboml/compiler/classes/expression.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/factor.py` & `gboml-0.1.8/src/gboml/compiler/classes/factor.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/identifier.py` & `gboml-0.1.8/src/gboml/compiler/classes/identifier.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/link.py` & `gboml-0.1.8/src/gboml/compiler/classes/link.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.nb_constraint_matrix = 0
         self.nb_constraints = len(constraints)
         self.constr_factors = []
         self.c_triplet_list = []
         self.variables_used = {}
         self.line = line
         self.names_changes = []
+        self.parameters_redefined_dict = {}
         self.parameters_changes = []
         self.constraints_data = {}
         self.nb_eq_constraints = 0
         self.nb_ineq_constraints = 0
 
     def get_line(self):
         return self.line
@@ -88,15 +89,27 @@
     def get_names_changes(self):
         return self.names_changes
 
     def add_name_change(self, change):
         self.names_changes.append(change)
 
     def set_parameters_changes(self, changes):
-        self.parameters_changes = changes
+        if not self.parameters_changes:
+            self.parameters_changes = changes
+            for i, change in enumerate(changes):
+                self.parameters_redefined_dict[change.get_name()] = i
+        else:
+            for param in self.parameters_changes:
+                name = param.get_name()
+                if name in self.parameters_redefined_dict:
+                    i = self.parameters_redefined_dict[name]
+                    self.parameters_changes[i] = param
+                else:
+                    self.parameters_redefined_dict[name] = (len(self.parameters_changes), param)
+                    self.parameters_changes.append(param)
 
     def add_parameter_change(self, change):
         self.parameters_changes.append(change)
 
     def get_parameters_changes(self):
         return self.parameters_changes
```

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/mdp.py` & `gboml-0.1.8/src/gboml/compiler/classes/mdp.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/node.py` & `gboml-0.1.8/src/gboml/compiler/classes/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         self.param_dict = None
         self.constr_factors = []
         self.obj_factors = []
         self.nodes = []
         self.hyperedges = []
         self.expression = []
         self.parameters_changes = []
+        self.parameters_redefined_dict = {}
         self.variables_changes = []
         self.dict_sub_nodes_edges = {}
         self.objectives_data = {}
         self.constraints_data = {}
 
     def __str__(self):
 
@@ -103,15 +104,27 @@
     def add_variable_change(self, change):
         self.variables_changes.append(change)
 
     def get_variables_changes(self):
         return self.variables_changes
 
     def set_parameters_changes(self, changes):
-        self.parameters_changes = changes
+        if not self.parameters_changes:
+            self.parameters_changes = changes
+            for i, change in enumerate(changes):
+                self.parameters_redefined_dict[change.get_name()] = i
+        else:
+            for param in self.parameters_changes:
+                name = param.get_name()
+                if name in self.parameters_redefined_dict:
+                    i = self.parameters_redefined_dict[name]
+                    self.parameters_changes[i] = param
+                else:
+                    self.parameters_redefined_dict[name] = (len(self.parameters_changes), param)
+                    self.parameters_changes.append(param)
 
     def add_parameter_change(self, change):
         self.parameters_changes.append(change)
 
     def get_parameters_changes(self):
         return self.parameters_changes
```

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/objective.py` & `gboml-0.1.8/src/gboml/compiler/classes/objective.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/parameter.py` & `gboml-0.1.8/src/gboml/compiler/classes/parameter.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/parent.py` & `gboml-0.1.8/src/gboml/compiler/classes/parent.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/program.py` & `gboml-0.1.8/src/gboml/compiler/classes/program.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/time_obj.py` & `gboml-0.1.8/src/gboml/compiler/classes/time_obj.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/classes/variable.py` & `gboml-0.1.8/src/gboml/compiler/classes/variable.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/gboml_compiler.py` & `gboml-0.1.8/src/gboml/compiler/gboml_compiler.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/gboml_lexer.py` & `gboml-0.1.8/src/gboml/compiler/gboml_lexer.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/gboml_matrix_generation.py` & `gboml-0.1.8/src/gboml/compiler/gboml_matrix_generation.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/gboml_parser.py` & `gboml-0.1.8/src/gboml/compiler/gboml_parser.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/gboml_semantic.py` & `gboml-0.1.8/src/gboml/compiler/gboml_semantic.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/ply/lex.py` & `gboml-0.1.8/src/gboml/compiler/ply/lex.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/ply/yacc.py` & `gboml-0.1.8/src/gboml/compiler/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/compiler/utils.py` & `gboml-0.1.8/src/gboml/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/gboml_graph.py` & `gboml-0.1.8/src/gboml/gboml_graph.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/gboml_main.py` & `gboml-0.1.8/src/gboml/gboml_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 import sys
 from time import gmtime, strftime, time
 
 
 def main():
     parser = argparse.ArgumentParser(allow_abbrev=False,
                                      description='Compiler and solver for the '
-                                                 'generic system model language'
-                                     )
+                                                 'generic system model language')
     parser.add_argument("input_file", type=str)
 
     # Compiling info
     parser.add_argument("--lex", help="Prints all tokens found in input file",
                         action='store_const', const=True)
     parser.add_argument("--parse", help="Prints the AST", action='store_const',
                         const=True)
@@ -54,14 +53,16 @@
     # Solver
     parser.add_argument("--clp", help="CLP solver", action='store_const',
                         const=True)
     parser.add_argument("--cbc", help="CBC solver", action='store_const',
                         const=True)
     parser.add_argument("--cplex", help="Cplex solver", action='store_const',
                         const=True)
+    parser.add_argument("--cplex_benders", help="Cplex Benders Solver",
+                        action='store_const', const=True)
     parser.add_argument("--linprog", help="Scipy linprog solver",
                         action='store_const', const=True)
     parser.add_argument("--gurobi", help="Gurobi solver",
                         action='store_const', const=True)
     parser.add_argument("--xpress", help="Xpress solver",
                         action='store_const', const=True)
     parser.add_argument("--dsp_de", help="DSP Extensive Form algorithm",
@@ -84,16 +85,20 @@
                         help="get detailed version of the output",
                         nargs="?",
                         type=str, default="")
     parser.add_argument("--log", help="Get log in a file",
                         action="store_const", const=True)
     parser.add_argument("--output", help="Output filename", type=str)
     parser.add_argument("--opt", help="Optimization options filename", type=str)
+    parser.add_argument("--solver_lib",
+                        help="Path to solver library for CBC - HiGHs - DSP solver",
+                        type=str)
 
     args = parser.parse_args()
+
     start_time = time()
     if args.detailed is None:
         args.detailed = True
     elif args.detailed == "":
         args.detailed = False
 
     if args.input_file:
@@ -131,55 +136,67 @@
         elif args.clp:
 
             x, objective, status, solver_info = \
                 clp_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples)
         elif args.cbc:
 
             x, objective, status, solver_info = \
-                cbc_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples)
+                cbc_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
+                           solver_lib=args.solver_lib)
+
+        elif args.cplex_benders:
+            struct_eq, struct_ineq = program.get_first_level_constraints_decomposition()
+            x, objective, status, solver_info, \
+             constraints_additional_information, \
+             variables_additional_information = \
+                cplex_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
+                             opt_file=args.opt, structure_indexes_eq=struct_eq,
+                             structure_indexes_ineq=struct_ineq, details=args.detailed)
+
         elif args.cplex:
             x, objective, status, solver_info, \
              constraints_additional_information, \
              variables_additional_information = \
              cplex_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
                           args.opt, details=args.detailed)
 
         elif args.gurobi:
 
             x, objective, status, solver_info, \
              constraints_additional_information, \
              variables_additional_information = \
              gurobi_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
                            args.opt, args.detailed)
-            print(x)
 
         elif args.xpress:
 
             x, objective, status, solver_info, \
              constraints_additional_information, \
              variables_additional_information = \
              xpress_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
                            args.opt, args.detailed)
 
         elif args.dsp_dw:
             struct_eq, struct_ineq = program.get_first_level_constraints_decomposition()
             x, objective, status, solver_info = \
                 dsp_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
-                           struct_eq, struct_ineq, algorithm="dw")
+                           struct_eq, struct_ineq, algorithm="dw",
+                           solver_lib=args.solver_lib)
 
         elif args.dsp_de:
             struct_eq, struct_ineq = program.get_first_level_constraints_decomposition()
             x, objective, status, solver_info = \
                 dsp_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
-                           struct_eq, struct_ineq, algorithm="de")
+                           struct_eq, struct_ineq, algorithm="de",
+                           solver_lib=args.solver_lib)
 
         elif args.highs:
             x, objective, status, solver_info = \
                 highs_solver(A_eq, b_eq, A_ineq, b_ineq, C_sum, objective_offset, name_tuples,
-                             args.opt)
+                             args.opt, solver_lib=args.solver_lib)
         else:
 
             print("No solver was chosen")
             sys.exit()
 
         assert status in {"unbounded", "optimal", "feasible", "infeasible",
                           "error", "unknown", "sub-optimal stopped"}
```

### Comparing `gboml-0.1.7/src/gboml/output/gboml_output.py` & `gboml-0.1.8/src/gboml/output/gboml_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,20 +358,20 @@
             start_index = identifier.get_index()
             size_variable = identifier.get_size()
             identifier_name = node_name+"."+identifier.get_name()
             values = solution[start_index:
                               (start_index + size_variable)].flatten().tolist()
             name_tuples.append([identifier_name, values])
 
-        #parameters = node.get_parameter_dict()
-        #for parameter_name, parameter_object in parameters.items():
+        parameters = node.get_parameter_dict()
+        for parameter_name, parameter_object in parameters.items():
 
-        #    values = parameter_object.get_value()
-        #    parameter_full_name = str(node_name) + "." + str(parameter_name)
-        #    name_tuples.append([parameter_full_name, values])
+            values = parameter_object.get_value()
+            parameter_full_name = str(node_name) + "." + str(parameter_name)
+            name_tuples.append([parameter_full_name, values])
 
         objectives_data = node.get_objectives_data()
         for i, objective_info in objectives_data.items():
             objective_type = objective_info["type"]
             if "name" in objective_info:
                 name_objective = objective_info["name"]
 
@@ -406,19 +406,19 @@
                                                       product,
                                                       constraints_info,
                                                       node_name+".")
 
     for hyperedge in hyperedges:
         hyperedge_name = prefix+hyperedge.get_name()
         parameters = hyperedge.get_parameter_dict()
-        #for parameter_name, parameter_object in parameters.items():
-        #    values = parameter_object.get_value()
-        #    parameter_full_name = str(hyperedge_name) + "." \
-        #                          + str(parameter_name)
-        #    name_tuples.append([parameter_full_name, values])
+        for parameter_name, parameter_object in parameters.items():
+            values = parameter_object.get_value()
+            parameter_full_name = str(hyperedge_name) + "." \
+                                  + str(parameter_name)
+            name_tuples.append([parameter_full_name, values])
 
         if constraints_info != {}:
             constraints_info_in_hyperedge = hyperedge.get_constraints_data()
             for constr_type, constr_dict in constraints_info_in_hyperedge.items():
                 current_constr_dict = constraints_info[constr_type]
                 for constraint_name, indexes in constr_dict.items():
                     for constraint_info_name, constraint_info_values in \
@@ -456,19 +456,19 @@
     hyperedges = program.get_links()
 
     product = []
     if solution is not None:
         product = c_matrix * solution + indep_terms_c
 
     global_param: dict = program.get_global_parameters()
-    #for param in global_param.keys():
-    #    values = global_param[param].get_value()
-    #    full_name = "global." + str(param)
-    #    names.append(full_name)
-    #    ordered_values.append(values)
+    for param in global_param.keys():
+        values = global_param[param].get_value()
+        full_name = "global." + str(param)
+        names.append(full_name)
+        ordered_values.append(values)
 
     name_value_tuples = flat_graph_and_add_node_prefix(nodes,
                                                        hyperedges,
                                                        solution,
                                                        product,
                                                        constraints_info,
                                                        prefix="")
```

### Comparing `gboml-0.1.7/src/gboml/solver_api/__init__.py` & `gboml-0.1.8/src/gboml/solver_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/solver_api/cbc_solver.py` & `gboml-0.1.8/src/gboml/solver_api/cbc_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 def cbc_solver(matrix_a_eq: coo_matrix, vector_b_eq: np.ndarray,
                matrix_a_ineq: coo_matrix, vector_b_ineq: np.ndarray,
                vector_c: np.ndarray,
                objective_offset: float,
                name_tuples: dict,
                opt_file: str = None,
-               option_dict: dict = None) -> tuple:
+               option_dict: dict = None,
+               solver_lib=None) -> tuple:
     """cbc_solver
 
         takes as input the matrix A, the vectors b and c. It returns the
         solution of the problem : min c^T * x s.t. A * x <= b found by
         the clp/cbc solver
 
         Args:
@@ -49,15 +50,15 @@
             vector_c -> np.ndarray of objective vector
             objective_offset -> float of the objective offset
             name_tuples -> dictionary of <node_name variables> used to get
                            the type
             opt_file -> optimization parameters file
             option_dict -> alternative to optimization parameters file that associates
                            key = <option to set>, value= value
-
+            solver_lib -> path to solver library
         Returns:
             solution -> np.ndarray of the flat solution
             objective -> float of the objective value
             status -> solution status
             solver_info -> dictionary of solver information
 
     """
@@ -88,15 +89,15 @@
         if var_type == "binary":
             col_types[index:index + var_size] = [1] * var_size
             col_lower[index:index + var_size] = [0] * var_size
             col_upper[index:index + var_size] = [1] * var_size
 
     merged_matrices = coo_matrix((all_data, (all_rows, all_col)), shape=(nb_row_ineq+nb_row_eq, nvars)).tocsc()
     index, indptr, data = merged_matrices.indices, merged_matrices.indptr, merged_matrices.data
-    cbc_lib = PyCBC()
+    cbc_lib = PyCBC(solver_lib)
     cbc_model = cbc_lib.Cbc_newModel()
     cbc_lib.Cbc_loadProblem(cbc_model, nvars, nb_row_ineq+nb_row_eq, indptr, index, data,
                             col_lower, col_upper, vector_c[0], row_lower, row_upper)
 
     for i, col_type in enumerate(col_types):
         if col_type == 1:
             cbc_lib.Cbc_setInteger(cbc_model, i)
@@ -190,8 +191,10 @@
         elif secondary_status_gap or secondary_status_timeout:
             status = "sub-optimal stopped"
             solution = cbc_lib.Cbc_getColSolution(cbc_model, nvars)
             objective = cbc_lib.Cbc_getObjValue(cbc_model)+objective_offset
     else:
         status = "unknown"
 
+    cbc_lib.Cbc_deleteModel(cbc_model)
+
     return solution, objective, status, solver_info
```

### Comparing `gboml-0.1.7/src/gboml/solver_api/clp_solver.py` & `gboml-0.1.8/src/gboml/solver_api/clp_solver.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/solver_api/cplex_solver.py` & `gboml-0.1.8/src/gboml/solver_api/cplex_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 
 def cplex_solver(matrix_a_eq: coo_matrix, vector_b_eq: np.ndarray,
                  matrix_a_ineq: coo_matrix, vector_b_ineq: np.ndarray,
                  vector_c: np.ndarray,
                  objective_offset: float,
                  name_tuples: dict,
+                 structure_indexes_eq = None,
+                 structure_indexes_ineq = None,
                  opt_file: str = None,
                  details=False,
                  option_dict: dict = None) -> tuple:
     """cplex_solver
 
         takes as input the matrix A, the vectors b and c. It returns
         the solution of the problem : min c^T * x s.t. A * x <= b found
@@ -56,26 +58,31 @@
             vector_b_eq -> np.ndarray of independent terms of each equality constraint
             matrix_a_ineq -> coo_matrix of inequality constraints
             vector_b_eq -> np.ndarray of independent terms of each inequality constraint
             c -> np.ndarray of objective vector
             objective_offset -> float of the objective offset
             name_tuples -> dictionary of <node_name variables> used
                            to get the type
+            structure_indexes_eq -> constraint indexes for equality matrix of the different blocks
+                                    (last one being the master block)
+            structure_indexes_ineq -> constraint indexes for inequality matrix of the different blocks
+                                    (last one being the master block)
             opt_file -> optimization parameters file
             option_dict -> alternative to optimization parameters file that associates
                            key = <option to set>, value= value
         Returns:
             solution -> np.ndarray of the flat solution
             objective -> float of the objective value
             status -> solution status
             solver_info -> dictionary of solver information
 
     """
     if option_dict is None:
         option_dict = dict()
+
     try:
 
         import cplex
     except ImportError:
 
         print("Warning: Did not find the CPLEX package")
         exit(0)
@@ -120,14 +127,36 @@
                 i = i+1
 
     model.linear_constraints.add(senses=['L']*line_ineq+['E']*line_eq, rhs=vector_b)
     model.linear_constraints.set_coefficients(matrix_a_zipped)
     model.objective.set_sense(model.objective.sense.minimize)
     model.objective.set_offset(objective_offset)
 
+    print(structure_indexes_eq, structure_indexes_ineq)
+    if structure_indexes_eq is not None and structure_indexes_ineq is not None:
+        if structure_indexes_eq != [] and structure_indexes_ineq != []:
+            master_block_eq = structure_indexes_eq[-1]
+            master_block_ineq = structure_indexes_ineq[-1]
+            col_ineq = matrix_a_ineq.col
+            col_eq = matrix_a_eq.col
+            master_var_col = np.append(col_ineq[master_block_ineq], col_eq[master_block_eq])
+            anno = model.long_annotations
+            idx = anno.add(name=anno.benders_annotation,
+                           defval=anno.benders_mastervalue)
+            objtype = anno.object_type.variable
+            nb_blocks = len(structure_indexes_eq)
+            for b_number in range(nb_blocks - 1):
+                block_eq = structure_indexes_eq[b_number]
+                block_ineq = structure_indexes_ineq[b_number]
+                block_var = np.append(col_ineq[block_eq], col_eq[block_ineq])
+                list_zipped = [(int(i), int(b_number+1)) for i in block_var if i not in master_var_col]
+                model.long_annotations.set_values(idx, objtype, list_zipped)
+        else:
+            model.parameters.benders.strategy.set(
+                model.parameters.benders.strategy.values.full)
     # Retrieve solver information
     solver_info = {"name": "cplex"}
     print("\nReading CPLEX options from file cplex.opt")
     option_info = {}
     new_dict_options_from_file = option_dict.copy()
     try:
```

### Comparing `gboml-0.1.7/src/gboml/solver_api/dsp_solver.py` & `gboml-0.1.8/src/gboml/solver_api/dsp_solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
 def dsp_solver(matrix_a_eq: coo_matrix, vector_b_eq: np.ndarray,
                matrix_a_ineq: coo_matrix, vector_b_ineq: np.ndarray,
                vector_c: np.ndarray,
                objective_offset: float, name_tuples: dict,
                structure_indexes_eq,
                structure_indexes_ineq,
-               algorithm="de") -> tuple:
+               algorithm="de",
+               solver_lib=None) -> tuple:
     """dsp_solver
 
         takes as input the matrix A, the vectors b and c. It returns the
         solution of the problem : min c^T * x s.t. A * x <= b found
         by the dsp solver
 
         Args:
@@ -52,15 +53,15 @@
                            the type
             structure_indexes_eq -> constraint indexes for equality matrix of the different blocks
                                     (last one being the master block)
             structure_indexes_ineq -> constraint indexes for inequality matrix of the different blocks
                                     (last one being the master block)
             algorithm -> solving algorithm to use, either "de" for the extensive
                          form and "dw" for Dantzig-Wolf
-
+            solver_lib -> path to solver library
         Returns:
             solution -> np.ndarray of the flat solution
             objective -> float of the objective value
             status -> solution status
             solver_info -> dictionary of solver information
 
     """
@@ -102,15 +103,15 @@
 
     vector_master_eq = vector_b_eq[master_constr_slice_eq].tolist()
 
     row_lb = [-float("inf")] * master_nb_lines_ineq+vector_master_eq
 
     row_up = vector_b_ineq[master_constr_slice_ineq].tolist()+vector_master_eq
 
-    dsp = DSPpy()
+    dsp = DSPpy(solver_lib)
     pointer_to_model = dsp.createEnv()
     master_val = np.concatenate((master_val_ineq, master_val_eq))
     master_col = np.concatenate((master_col_ineq, master_col_eq))
     master_row = np.concatenate((master_row_ineq[:-1], master_row_eq+len(master_val_ineq)))
 
     dsp.loadBlockProblem(pointer_to_model, 0, nb_cols, master_nb_lines_ineq+master_nb_lines_eq,
                          len(master_val), master_row, master_col, master_val,
```

### Comparing `gboml-0.1.7/src/gboml/solver_api/dsppy.py` & `gboml-0.1.8/src/gboml/solver_api/dsppy.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/solver_api/gurobi_solver.py` & `gboml-0.1.8/src/gboml/solver_api/gurobi_solver.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/solver_api/highs_solver.py` & `gboml-0.1.8/src/gboml/solver_api/highs_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
 
 def highs_solver(matrix_a_eq: coo_matrix, vector_b_eq: np.ndarray,
                  matrix_a_ineq: coo_matrix, vector_b_ineq: np.ndarray,
                  vector_c: np.ndarray,
                  objective_offset: float, name_tuples: dict,
                  opt_file: str = None,
-                 option_dict: dict = None
+                 option_dict: dict = None,
+                 solver_lib=None
                  ) -> tuple:
     """highs_solver
 
         takes as input the matrix A, the vectors b and c. It returns the
         solution of the problem : min c^T * x s.t. A * x <= b found by
         the Highs solver
 
@@ -49,15 +50,15 @@
             vector_c -> np.ndarray of objective vector
             objective_offset -> float of the objective offset
             name_tuples -> dictionary of <node_name variables> used to get
                            the type
             opt_file -> optimization parameters file
             option_dict -> alternative to optimization parameters file that associates
                            key = <option to set>, value= value
-
+            solver_lib -> path to solver library
         Returns:
             solution -> np.ndarray of the flat solution
             objective -> float of the objective value
             status -> solution status
             solver_info -> dictionary of solver information
 
     """
@@ -74,15 +75,15 @@
     nb_values_ineq = len(matrix_a_ineq.data)
     nb_values = len(matrix_a_eq.data)+nb_values_ineq
 
     csr_matrix_a_eq = csr_matrix(matrix_a_eq)
     csr_matrix_a_ineq = csr_matrix(matrix_a_ineq)
 
     vector_c = vector_c[-1]
-    py_highs = PyHighs()
+    py_highs = PyHighs(solver_lib)
     highs_model = py_highs.Highs_create()
 
     col_types = [0] * nb_cols
     col_lower = [-float('inf')]*nb_cols
     col_upper = [float('inf')]*nb_cols
     flat_name_tuples = flat_nested_list_to_two_level(name_tuples)
     is_milp = False
```

### Comparing `gboml-0.1.7/src/gboml/solver_api/pycbc.py` & `gboml-0.1.8/src/gboml/solver_api/pycbc.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/solver_api/pyhighs.py` & `gboml-0.1.8/src/gboml/solver_api/pyhighs.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/solver_api/scipy_solver.py` & `gboml-0.1.8/src/gboml/solver_api/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml/solver_api/xpress_solver.py` & `gboml-0.1.8/src/gboml/solver_api/xpress_solver.py`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/gboml.egg-info/PKG-INFO` & `gboml-0.1.8/src/gboml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gboml
-Version: 0.1.7
+Version: 0.1.8
 Summary: GBOML: Graph-Based Optimization Modeling Language
 Home-page: https://gitlab.uliege.be/smart_grids/public/gboml
 Author: Bardhyl Miftari, Mathias Berger, Hatim Djelassi, Damien Ernst
 Author-email: bmiftari@uliege.be
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gboml-0.1.7/src/gboml.egg-info/SOURCES.txt` & `gboml-0.1.8/src/gboml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gboml-0.1.7/src/main.py` & `gboml-0.1.8/src/main.py`

 * *Files identical despite different names*

