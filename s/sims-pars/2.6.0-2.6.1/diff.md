# Comparing `tmp/sims-pars-2.6.0.tar.gz` & `tmp/sims-pars-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sims-pars-2.6.0.tar", last modified: Fri Apr 21 15:00:21 2023, max compression
+gzip compressed data, was "sims-pars-2.6.1.tar", last modified: Fri Apr 21 14:58:42 2023, max compression
```

## Comparing `sims-pars-2.6.0.tar` & `sims-pars-2.6.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.609856 sims-pars-2.6.0/
--rw-rw-rw-   0        0        0     1084 2023-04-21 13:17:56.000000 sims-pars-2.6.0/LICENSE
--rw-rw-rw-   0        0        0      664 2023-04-21 15:00:21.609856 sims-pars-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-04-21 13:17:56.000000 sims-pars-2.6.0/README.md
--rw-rw-rw-   0        0        0      676 2023-04-21 15:00:07.000000 sims-pars-2.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 15:00:21.609856 sims-pars-2.6.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.559857 sims-pars-2.6.0/src/
--rw-rw-rw-   0        0        0     1657 2023-04-21 15:00:07.000000 sims-pars-2.6.0/src/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.563856 sims-pars-2.6.0/src/sims_pars/
--rw-rw-rw-   0        0        0      290 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.570856 sims-pars-2.6.0/src/sims_pars/bayesnet/
--rw-rw-rw-   0        0        0      251 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/bayesnet/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/bayesnet/bn.py
--rw-rw-rw-   0        0        0     3240 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/bayesnet/chromosome.py
--rw-rw-rw-   0        0        0     6477 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/bayesnet/dag.py
--rw-rw-rw-   0        0        0     7954 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/bayesnet/loci.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.574856 sims-pars-2.6.0/src/sims_pars/data/
--rw-rw-rw-   0        0        0      204 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/__init__.py
--rw-rw-rw-   0        0        0      660 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/datafunction.py
--rw-rw-rw-   0        0        0       28 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/fn.py
--rw-rw-rw-   0        0        0      502 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/frame.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.579856 sims-pars-2.6.0/src/sims_pars/data/reg/
--rw-rw-rw-   0        0        0      151 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/reg/__init__.py
--rw-rw-rw-   0        0        0     4086 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/reg/glm.py
--rw-rw-rw-   0        0        0     3616 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/reg/hazard.py
--rw-rw-rw-   0        0        0        6 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/reg/lcm.py
--rw-rw-rw-   0        0        0     4179 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/reg/linear.py
--rw-rw-rw-   0        0        0     3568 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/reg/survival.py
--rw-rw-rw-   0        0        0     2776 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/static.py
--rw-rw-rw-   0        0        0     3131 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/data/timeseries.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.580856 sims-pars-2.6.0/src/sims_pars/factory/
--rw-rw-rw-   0        0        0      324 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/factory/__init__.py
--rw-rw-rw-   0        0        0     2995 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/factory/craftstation.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.584856 sims-pars-2.6.0/src/sims_pars/fit/
--rw-rw-rw-   0        0        0      174 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/fit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.585856 sims-pars-2.6.0/src/sims_pars/fit/abc_smc/
--rw-rw-rw-   0        0        0       57 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/abc_smc/__init__.py
--rw-rw-rw-   0        0        0    10906 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/fit/abc_smc/alg.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.587856 sims-pars-2.6.0/src/sims_pars/fit/abcom/
--rw-rw-rw-   0        0        0       52 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/abcom/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/abcom/alg.py
--rw-rw-rw-   0        0        0     6789 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/fit/base.py
--rw-rw-rw-   0        0        0     4311 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/converter.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.590856 sims-pars-2.6.0/src/sims_pars/fit/ga/
--rw-rw-rw-   0        0        0       35 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/ga/__init__.py
--rw-rw-rw-   0        0        0     5748 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/ga/alg.py
--rw-rw-rw-   0        0        0     2396 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/ga/cross.py
--rw-rw-rw-   0        0        0     2313 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/ga/mutate.py
--rw-rw-rw-   0        0        0     2871 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/ga/select.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.593856 sims-pars-2.6.0/src/sims_pars/fit/hme/
--rw-rw-rw-   0        0        0       56 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/hme/__init__.py
--rw-rw-rw-   0        0        0     6943 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/fit/hme/alg.py
--rw-rw-rw-   0        0        0     2567 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/fit/hme/emulator.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.593856 sims-pars-2.6.0/src/sims_pars/fit/nuts/
--rw-rw-rw-   0        0        0       43 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/nuts/__init__.py
--rw-rw-rw-   0        0        0      957 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/results.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.596856 sims-pars-2.6.0/src/sims_pars/fit/targets/
--rw-rw-rw-   0        0        0     1382 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/targets/__init__.py
--rw-rw-rw-   0        0        0      572 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/targets/base.py
--rw-rw-rw-   0        0        0      307 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/targets/multi.py
--rw-rw-rw-   0        0        0     2277 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/targets/single.py
--rw-rw-rw-   0        0        0     3404 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fit/toys.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.600856 sims-pars-2.6.0/src/sims_pars/fitting/
--rw-rw-rw-   0        0        0       87 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fitting/__init__.py
--rw-rw-rw-   0        0        0     5408 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fitting/base.py
--rw-rw-rw-   0        0        0     1782 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fitting/cases.py
--rw-rw-rw-   0        0        0     3633 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fitting/fitter.py
--rw-rw-rw-   0        0        0     5236 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/fitting/util.py
--rw-rw-rw-   0        0        0     2354 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/fn.py
--rw-rw-rw-   0        0        0     2260 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/monitor.py
--rw-rw-rw-   0        0        0     9423 2023-04-21 14:34:09.000000 sims-pars-2.6.0/src/sims_pars/prob.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.605856 sims-pars-2.6.0/src/sims_pars/simulation/
--rw-rw-rw-   0        0        0      240 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/simulation/__init__.py
--rw-rw-rw-   0        0        0     3908 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/simulation/actor.py
--rw-rw-rw-   0        0        0     1830 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/simulation/fn.py
--rw-rw-rw-   0        0        0    11850 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/simulation/nodeset.py
--rw-rw-rw-   0        0        0    14710 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/simulation/parcore.py
--rw-rw-rw-   0        0        0     1743 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/simulation/simucore.py
--rw-rw-rw-   0        0        0     4267 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/simulation/simugroup.py
--rw-rw-rw-   0        0        0     7374 2023-04-21 13:17:56.000000 sims-pars-2.6.0/src/sims_pars/util.py
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.567856 sims-pars-2.6.0/src/sims_pars.egg-info/
--rw-rw-rw-   0        0        0      664 2023-04-21 15:00:21.000000 sims-pars-2.6.0/src/sims_pars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2123 2023-04-21 15:00:21.000000 sims-pars-2.6.0/src/sims_pars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 15:00:21.000000 sims-pars-2.6.0/src/sims_pars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 15:00:21.000000 sims-pars-2.6.0/src/sims_pars.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-21 15:00:21.608856 sims-pars-2.6.0/tests/
--rw-rw-rw-   0        0        0     3959 2023-04-21 13:17:56.000000 sims-pars-2.6.0/tests/test_distribution.py
--rw-rw-rw-   0        0        0     1661 2023-04-21 13:17:56.000000 sims-pars-2.6.0/tests/test_factory.py
--rw-rw-rw-   0        0        0      839 2023-04-21 13:17:56.000000 sims-pars-2.6.0/tests/test_monitor.py
--rw-rw-rw-   0        0        0     1940 2023-04-21 13:17:56.000000 sims-pars-2.6.0/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.509613 sims-pars-2.6.1/
+-rw-rw-rw-   0        0        0     1084 2023-04-21 13:17:56.000000 sims-pars-2.6.1/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-04-21 14:58:42.508613 sims-pars-2.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-04-21 13:17:56.000000 sims-pars-2.6.1/README.md
+-rw-rw-rw-   0        0        0      676 2023-04-21 14:53:30.000000 sims-pars-2.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 14:58:42.509613 sims-pars-2.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.449614 sims-pars-2.6.1/src/
+-rw-rw-rw-   0        0        0     1657 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.453614 sims-pars-2.6.1/src/sims_pars/
+-rw-rw-rw-   0        0        0      290 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.461614 sims-pars-2.6.1/src/sims_pars/bayesnet/
+-rw-rw-rw-   0        0        0      251 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/bayesnet/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/bayesnet/bn.py
+-rw-rw-rw-   0        0        0     3240 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/bayesnet/chromosome.py
+-rw-rw-rw-   0        0        0     6477 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/bayesnet/dag.py
+-rw-rw-rw-   0        0        0     7954 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/bayesnet/loci.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.465614 sims-pars-2.6.1/src/sims_pars/data/
+-rw-rw-rw-   0        0        0      204 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/__init__.py
+-rw-rw-rw-   0        0        0      660 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/datafunction.py
+-rw-rw-rw-   0        0        0       28 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/fn.py
+-rw-rw-rw-   0        0        0      502 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/frame.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.470614 sims-pars-2.6.1/src/sims_pars/data/reg/
+-rw-rw-rw-   0        0        0      151 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/reg/__init__.py
+-rw-rw-rw-   0        0        0     4086 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/reg/glm.py
+-rw-rw-rw-   0        0        0     3616 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/reg/hazard.py
+-rw-rw-rw-   0        0        0        6 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/reg/lcm.py
+-rw-rw-rw-   0        0        0     4179 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/reg/linear.py
+-rw-rw-rw-   0        0        0     3568 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/reg/survival.py
+-rw-rw-rw-   0        0        0     2776 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/static.py
+-rw-rw-rw-   0        0        0     3131 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/data/timeseries.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.472613 sims-pars-2.6.1/src/sims_pars/factory/
+-rw-rw-rw-   0        0        0      324 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/factory/__init__.py
+-rw-rw-rw-   0        0        0     2995 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/factory/craftstation.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.478627 sims-pars-2.6.1/src/sims_pars/fit/
+-rw-rw-rw-   0        0        0      174 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/fit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.480613 sims-pars-2.6.1/src/sims_pars/fit/abc_smc/
+-rw-rw-rw-   0        0        0       57 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/abc_smc/__init__.py
+-rw-rw-rw-   0        0        0    10906 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/fit/abc_smc/alg.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.482612 sims-pars-2.6.1/src/sims_pars/fit/abcom/
+-rw-rw-rw-   0        0        0       52 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/abcom/__init__.py
+-rw-rw-rw-   0        0        0     3846 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/abcom/alg.py
+-rw-rw-rw-   0        0        0     6789 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/fit/base.py
+-rw-rw-rw-   0        0        0     4311 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/converter.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.487634 sims-pars-2.6.1/src/sims_pars/fit/ga/
+-rw-rw-rw-   0        0        0       35 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/ga/__init__.py
+-rw-rw-rw-   0        0        0     5748 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/ga/alg.py
+-rw-rw-rw-   0        0        0     2396 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/ga/cross.py
+-rw-rw-rw-   0        0        0     2313 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/ga/mutate.py
+-rw-rw-rw-   0        0        0     2871 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/ga/select.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.490614 sims-pars-2.6.1/src/sims_pars/fit/hme/
+-rw-rw-rw-   0        0        0       56 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/hme/__init__.py
+-rw-rw-rw-   0        0        0     6943 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/fit/hme/alg.py
+-rw-rw-rw-   0        0        0     2567 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/fit/hme/emulator.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.491614 sims-pars-2.6.1/src/sims_pars/fit/nuts/
+-rw-rw-rw-   0        0        0       43 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/nuts/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/results.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.494614 sims-pars-2.6.1/src/sims_pars/fit/targets/
+-rw-rw-rw-   0        0        0     1382 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/targets/__init__.py
+-rw-rw-rw-   0        0        0      572 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/targets/base.py
+-rw-rw-rw-   0        0        0      307 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/targets/multi.py
+-rw-rw-rw-   0        0        0     2277 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/targets/single.py
+-rw-rw-rw-   0        0        0     3404 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fit/toys.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.498613 sims-pars-2.6.1/src/sims_pars/fitting/
+-rw-rw-rw-   0        0        0       87 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fitting/__init__.py
+-rw-rw-rw-   0        0        0     5408 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fitting/base.py
+-rw-rw-rw-   0        0        0     1782 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fitting/cases.py
+-rw-rw-rw-   0        0        0     3633 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fitting/fitter.py
+-rw-rw-rw-   0        0        0     5236 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/fitting/util.py
+-rw-rw-rw-   0        0        0     2354 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/fn.py
+-rw-rw-rw-   0        0        0     2260 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/monitor.py
+-rw-rw-rw-   0        0        0     9423 2023-04-21 14:34:09.000000 sims-pars-2.6.1/src/sims_pars/prob.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.504613 sims-pars-2.6.1/src/sims_pars/simulation/
+-rw-rw-rw-   0        0        0      240 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/simulation/__init__.py
+-rw-rw-rw-   0        0        0     3908 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/simulation/actor.py
+-rw-rw-rw-   0        0        0     1830 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/simulation/fn.py
+-rw-rw-rw-   0        0        0    11850 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/simulation/nodeset.py
+-rw-rw-rw-   0        0        0    14710 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/simulation/parcore.py
+-rw-rw-rw-   0        0        0     1743 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/simulation/simucore.py
+-rw-rw-rw-   0        0        0     4267 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/simulation/simugroup.py
+-rw-rw-rw-   0        0        0     7374 2023-04-21 13:17:56.000000 sims-pars-2.6.1/src/sims_pars/util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.457614 sims-pars-2.6.1/src/sims_pars.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-21 14:58:42.000000 sims-pars-2.6.1/src/sims_pars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2123 2023-04-21 14:58:42.000000 sims-pars-2.6.1/src/sims_pars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 14:58:42.000000 sims-pars-2.6.1/src/sims_pars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-21 14:58:42.000000 sims-pars-2.6.1/src/sims_pars.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-21 14:58:42.507613 sims-pars-2.6.1/tests/
+-rw-rw-rw-   0        0        0     3959 2023-04-21 13:17:56.000000 sims-pars-2.6.1/tests/test_distribution.py
+-rw-rw-rw-   0        0        0     1661 2023-04-21 13:17:56.000000 sims-pars-2.6.1/tests/test_factory.py
+-rw-rw-rw-   0        0        0      839 2023-04-21 13:17:56.000000 sims-pars-2.6.1/tests/test_monitor.py
+-rw-rw-rw-   0        0        0     1940 2023-04-21 13:17:56.000000 sims-pars-2.6.1/tests/test_util.py
```

### Comparing `sims-pars-2.6.0/LICENSE` & `sims-pars-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/PKG-INFO` & `sims-pars-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sims-pars
-Version: 2.6.0
+Version: 2.6.1
 Summary: Serving stochastic parameters to simulation modelse
 Author-email: Chu-Chang Ku <TimeWz667@gmail.com>
 Project-URL: Homepage, https://github.com/CxModelling/sims-parst
 Project-URL: Bug Tracker, https://github.com/CxModelling/sims-pars/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sims-pars-2.6.0/pyproject.toml` & `sims-pars-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sims-pars"
-version = "2.6.0"
+version = "2.6.1"
 authors = [
   { name="Chu-Chang Ku", email="TimeWz667@gmail.com" },
 ]
 description = "Serving stochastic parameters to simulation modelse"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `sims-pars-2.6.0/src/setup.py` & `sims-pars-2.6.1/src/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     dep: parse_requirements_file("requirements/" + dep + ".txt")
     for dep in ["core", "doc"]
 }
 
 
 setuptools.setup(
     name='sims-pars',
-    version='2.6.0',
+    version='2.8.1',
     author="Chu-Chang Ku",
     author_email='TimeWz667@gmail.com',
     description='Serving stochastic parameters to simulation models',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TimeWz667/sims-pars",
     project_urls={
```

### Comparing `sims-pars-2.6.0/src/sims_pars/bayesnet/bn.py` & `sims-pars-2.6.1/src/sims_pars/bayesnet/bn.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/bayesnet/chromosome.py` & `sims-pars-2.6.1/src/sims_pars/bayesnet/chromosome.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/bayesnet/dag.py` & `sims-pars-2.6.1/src/sims_pars/bayesnet/dag.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/bayesnet/loci.py` & `sims-pars-2.6.1/src/sims_pars/bayesnet/loci.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/data/datafunction.py` & `sims-pars-2.6.1/src/sims_pars/data/datafunction.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/data/reg/glm.py` & `sims-pars-2.6.1/src/sims_pars/data/reg/glm.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/data/reg/hazard.py` & `sims-pars-2.6.1/src/sims_pars/data/reg/hazard.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/data/reg/linear.py` & `sims-pars-2.6.1/src/sims_pars/data/reg/linear.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/data/reg/survival.py` & `sims-pars-2.6.1/src/sims_pars/data/reg/survival.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/data/static.py` & `sims-pars-2.6.1/src/sims_pars/data/static.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/data/timeseries.py` & `sims-pars-2.6.1/src/sims_pars/data/timeseries.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/factory/craftstation.py` & `sims-pars-2.6.1/src/sims_pars/factory/craftstation.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/abc_smc/alg.py` & `sims-pars-2.6.1/src/sims_pars/fit/abc_smc/alg.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/abcom/alg.py` & `sims-pars-2.6.1/src/sims_pars/fit/abcom/alg.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/base.py` & `sims-pars-2.6.1/src/sims_pars/fit/base.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/converter.py` & `sims-pars-2.6.1/src/sims_pars/fit/converter.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/ga/alg.py` & `sims-pars-2.6.1/src/sims_pars/fit/ga/alg.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/ga/cross.py` & `sims-pars-2.6.1/src/sims_pars/fit/ga/cross.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/ga/mutate.py` & `sims-pars-2.6.1/src/sims_pars/fit/ga/mutate.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/ga/select.py` & `sims-pars-2.6.1/src/sims_pars/fit/ga/select.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/hme/alg.py` & `sims-pars-2.6.1/src/sims_pars/fit/hme/alg.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/hme/emulator.py` & `sims-pars-2.6.1/src/sims_pars/fit/hme/emulator.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/results.py` & `sims-pars-2.6.1/src/sims_pars/fit/results.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/targets/__init__.py` & `sims-pars-2.6.1/src/sims_pars/fit/targets/__init__.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/targets/base.py` & `sims-pars-2.6.1/src/sims_pars/fit/targets/base.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/targets/single.py` & `sims-pars-2.6.1/src/sims_pars/fit/targets/single.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fit/toys.py` & `sims-pars-2.6.1/src/sims_pars/fit/toys.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fitting/base.py` & `sims-pars-2.6.1/src/sims_pars/fitting/base.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fitting/cases.py` & `sims-pars-2.6.1/src/sims_pars/fitting/cases.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fitting/fitter.py` & `sims-pars-2.6.1/src/sims_pars/fitting/fitter.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fitting/util.py` & `sims-pars-2.6.1/src/sims_pars/fitting/util.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/fn.py` & `sims-pars-2.6.1/src/sims_pars/fn.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/monitor.py` & `sims-pars-2.6.1/src/sims_pars/monitor.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/prob.py` & `sims-pars-2.6.1/src/sims_pars/prob.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/simulation/actor.py` & `sims-pars-2.6.1/src/sims_pars/simulation/actor.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/simulation/fn.py` & `sims-pars-2.6.1/src/sims_pars/simulation/fn.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/simulation/nodeset.py` & `sims-pars-2.6.1/src/sims_pars/simulation/nodeset.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/simulation/parcore.py` & `sims-pars-2.6.1/src/sims_pars/simulation/parcore.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/simulation/simucore.py` & `sims-pars-2.6.1/src/sims_pars/simulation/simucore.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/simulation/simugroup.py` & `sims-pars-2.6.1/src/sims_pars/simulation/simugroup.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars/util.py` & `sims-pars-2.6.1/src/sims_pars/util.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/src/sims_pars.egg-info/PKG-INFO` & `sims-pars-2.6.1/src/sims_pars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sims-pars
-Version: 2.6.0
+Version: 2.6.1
 Summary: Serving stochastic parameters to simulation modelse
 Author-email: Chu-Chang Ku <TimeWz667@gmail.com>
 Project-URL: Homepage, https://github.com/CxModelling/sims-parst
 Project-URL: Bug Tracker, https://github.com/CxModelling/sims-pars/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sims-pars-2.6.0/src/sims_pars.egg-info/SOURCES.txt` & `sims-pars-2.6.1/src/sims_pars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/tests/test_distribution.py` & `sims-pars-2.6.1/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/tests/test_factory.py` & `sims-pars-2.6.1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/tests/test_monitor.py` & `sims-pars-2.6.1/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sims-pars-2.6.0/tests/test_util.py` & `sims-pars-2.6.1/tests/test_util.py`

 * *Files identical despite different names*

