# Comparing `tmp/flavio-2.5.2.tar.gz` & `tmp/flavio-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flavio-2.5.2.tar", last modified: Fri Apr 21 17:48:48 2023, max compression
+gzip compressed data, was "flavio-2.5.3.tar", last modified: Fri Apr 21 18:13:13 2023, max compression
```

## Comparing `flavio-2.5.2.tar` & `flavio-2.5.3.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-21 17:44:13.000000 flavio-2.5.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 17:44:13.000000 flavio-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 17:48:48.563819 flavio-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-21 17:44:13.000000 flavio-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.511818 flavio-2.5.2/flavio/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.515818 flavio-2.5.2/flavio/data/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/citations.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)   984881 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/measurements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    26734 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/parameters_correlated.yml
--rw-r--r--   0 runner    (1001) docker     (123)    86949 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/parameters_metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/parameters_uncorrelated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.519818 flavio-2.5.2/flavio/data/test/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/2009.09313_digitized.npz
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/SPheno-2.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/SPheno.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/wcxf-flavio-example.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.519818 flavio-2.5.2/flavio/io/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/instanceio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.523818 flavio-2.5.2/flavio/math/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.523818 flavio-2.5.2/flavio/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.535819 flavio-2.5.2/flavio/physics/bdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/angular.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bll.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpll_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/bvll/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/nonfactorizable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/observables_bs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_bvll.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxll_qed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/btop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/test_btop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/clnexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/test_btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/hqet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/test_cln.py
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambdagamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambdall_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_angular.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bll.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bvgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_wc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/betadecays/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/ft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/test_betadecays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.503818 flavio-2.5.2/flavio/physics/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.547819 flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.551819 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/README
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.551819 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/
--rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.551819 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/
--rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/
--rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/arXiv-2102.07233v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/qcdf_interpolate/
--rw-r--r--   0 runner    (1001) docker     (123)   146774 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/wcsm/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/ddecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/ddecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/rge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/test_dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/test_dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/dileptons/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/partondist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/ppll.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/pplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/test_ppll.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/test_pplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/edms/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/slcouplings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/test_neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/test_paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/eft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/higgs/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/signalstrength.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/test_higgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/width.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/kdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/mdms/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mdms/al.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mdms/test_al.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/mesonmixing/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/test_mesonmixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/wilsoncoefficient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/mudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/muegamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/test_mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/test_mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/test_muegamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/neutrinos/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/neutrinos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/neutrinos/test_trident.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/neutrinos/trident.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/quarkonium/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Pll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Sll.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Vll.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Vllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Pll.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Sll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Vll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Vllgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/running/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/betafunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/masses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/running.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/test_running.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/scattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/scattering/ee_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/scattering/test_ee_ww.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/physics/taudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/test_ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/test_eft.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/physics/wdecays/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/gammaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/mw.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/test_mW.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/test_wdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/physics/zdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/afbz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/gammaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/gammazsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/test_smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/test_zdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39693 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/plotfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/test_plotfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    37591 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/test_probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_parseerrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.515818 flavio-2.5.2/flavio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 17:48:48.563819 flavio-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-21 17:44:13.000000 flavio-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.284982 flavio-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-21 18:08:35.000000 flavio-2.5.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 18:08:35.000000 flavio-2.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 18:13:13.280981 flavio-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-21 18:08:35.000000 flavio-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.252981 flavio-2.5.3/flavio/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.252981 flavio-2.5.3/flavio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/citations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   984881 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/measurements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26734 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/parameters_correlated.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    86949 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/parameters_metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19969 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/parameters_uncorrelated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.256981 flavio-2.5.3/flavio/data/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/2009.09313_digitized.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/SPheno-2.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/SPheno.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/data/test/wcxf-flavio-example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.256981 flavio-2.5.3/flavio/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/io/instanceio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/io/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.256981 flavio-2.5.3/flavio/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/math/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/math/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/math/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/math/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/math/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/math/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.256981 flavio-2.5.3/flavio/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.260981 flavio-2.5.3/flavio/physics/bdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bpll_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.260981 flavio-2.5.3/flavio/physics/bdecays/bvll/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/nonfactorizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/observables_bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/test_bvll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/test_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/test_qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bxll_qed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.260981 flavio-2.5.3/flavio/physics/bdecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.260981 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_gamma/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.264981 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/btop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/test_btop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.264981 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/clnexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/test_btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/hqet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.264981 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.264981 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/formfactors/test_cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/lambdablambdagamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/lambdablambdall_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bvgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/test_wc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/bdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.264981 flavio-2.5.3/flavio/physics/betadecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/betadecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/betadecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/betadecays/ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/betadecays/test_betadecays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.248981 flavio-2.5.3/flavio/physics/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.264981 flavio-2.5.3/flavio/physics/data/arXiv-0810-4077v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-0810-4077v3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.268981 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.268981 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.268981 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/
+-rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.268981 flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/data/arXiv-2102.07233v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/data/qcdf_interpolate/
+-rw-r--r--   0 runner    (1001) docker     (123)   146774 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/data/wcsm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/ddecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/ddecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/formfactors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/formfactors/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/formfactors/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/formfactors/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/rge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/test_dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/ddecays/test_dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/dileptons/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/dileptons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/dileptons/partondist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/dileptons/ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/dileptons/pplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/dileptons/test_ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/dileptons/test_pplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/edms/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/edms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/edms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/edms/neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/edms/paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/edms/slcouplings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/edms/test_neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/edms/test_paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.272982 flavio-2.5.3/flavio/physics/higgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/higgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/higgs/decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/higgs/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/higgs/signalstrength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/higgs/test_higgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/higgs/width.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.276981 flavio-2.5.3/flavio/physics/kdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/test_kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/test_klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/test_kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/test_kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/test_kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/test_lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/kdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.276981 flavio-2.5.3/flavio/physics/mdms/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mdms/al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mdms/test_al.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.276981 flavio-2.5.3/flavio/physics/mesonmixing/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mesonmixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mesonmixing/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mesonmixing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mesonmixing/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mesonmixing/test_mesonmixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mesonmixing/wilsoncoefficient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.276981 flavio-2.5.3/flavio/physics/mudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mudecays/mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mudecays/mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mudecays/muegamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mudecays/test_mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mudecays/test_mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/mudecays/test_muegamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.276981 flavio-2.5.3/flavio/physics/neutrinos/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/neutrinos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/neutrinos/test_trident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/neutrinos/trident.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.276981 flavio-2.5.3/flavio/physics/quarkonium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/Vllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/test_Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/test_Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/test_Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/quarkonium/test_Vllgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.276981 flavio-2.5.3/flavio/physics/running/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/running/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/running/betafunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/running/masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/running/running.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/running/test_running.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.280981 flavio-2.5.3/flavio/physics/scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/scattering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/scattering/ee_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/scattering/test_ee_ww.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.280981 flavio-2.5.3/flavio/physics/taudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/test_tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/test_taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/test_taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/test_taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/test_taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/taudecays/test_tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/test_ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/test_eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.280981 flavio-2.5.3/flavio/physics/wdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/wdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/wdecays/gammaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/wdecays/mw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/wdecays/test_mW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/wdecays/test_wdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.280981 flavio-2.5.3/flavio/physics/zdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/zdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/zdecays/afbz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/zdecays/gammaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/zdecays/gammazsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/zdecays/smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/zdecays/test_smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/physics/zdecays/test_zdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.280981 flavio-2.5.3/flavio/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/plots/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/plots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39693 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/plots/plotfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/plots/test_plotfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.280981 flavio-2.5.3/flavio/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/statistics/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/statistics/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/statistics/probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/statistics/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/statistics/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37591 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/statistics/test_probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/test_parseerrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-21 18:08:35.000000 flavio-2.5.3/flavio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:13:13.252981 flavio-2.5.3/flavio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 18:13:13.000000 flavio-2.5.3/flavio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-04-21 18:13:13.000000 flavio-2.5.3/flavio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:13:13.000000 flavio-2.5.3/flavio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 18:13:13.000000 flavio-2.5.3/flavio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 18:13:13.000000 flavio-2.5.3/flavio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 18:13:13.284982 flavio-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-21 18:08:35.000000 flavio-2.5.3/setup.py
```

### Comparing `flavio-2.5.2/LICENSE.txt` & `flavio-2.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/PKG-INFO` & `flavio-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.5.2
+Version: 2.5.3
 Summary: A Python package for flavour physics phenomenology in the Standard Model and beyond
 Home-page: https://flav-io.github.io
 Author: David M. Straub
 Author-email: straub@protonmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flavio Version: 2.5.2 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.3 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
```

### Comparing `flavio-2.5.2/README.md` & `flavio-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/__init__.py` & `flavio-2.5.3/flavio/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/_parse_errors.py` & `flavio-2.5.3/flavio/_parse_errors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/citations.py` & `flavio-2.5.3/flavio/citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/classes.py` & `flavio-2.5.3/flavio/classes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/citations.yml` & `flavio-2.5.3/flavio/data/citations.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/config.yml` & `flavio-2.5.3/flavio/data/config.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/measurements.yml` & `flavio-2.5.3/flavio/data/measurements.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/parameters_correlated.yml` & `flavio-2.5.3/flavio/data/parameters_correlated.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/parameters_metadata.yml` & `flavio-2.5.3/flavio/data/parameters_metadata.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/parameters_uncorrelated.yml` & `flavio-2.5.3/flavio/data/parameters_uncorrelated.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/test/2009.09313_digitized.npz` & `flavio-2.5.3/flavio/data/test/2009.09313_digitized.npz`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/test/SPheno-2.spc.MSSM` & `flavio-2.5.3/flavio/data/test/SPheno-2.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/data/test/SPheno.spc.MSSM` & `flavio-2.5.3/flavio/data/test/SPheno.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/functions.py` & `flavio-2.5.3/flavio/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/io/instanceio.py` & `flavio-2.5.3/flavio/io/instanceio.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/io/test_yaml.py` & `flavio-2.5.3/flavio/io/test_yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/io/yaml.py` & `flavio-2.5.3/flavio/io/yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/math/functions.py` & `flavio-2.5.3/flavio/math/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/math/integrate.py` & `flavio-2.5.3/flavio/math/integrate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/math/optimize.py` & `flavio-2.5.3/flavio/math/optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/math/test_math.py` & `flavio-2.5.3/flavio/math/test_math.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/math/test_optimize.py` & `flavio-2.5.3/flavio/math/test_optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/measurements.py` & `flavio-2.5.3/flavio/measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/parameters.py` & `flavio-2.5.3/flavio/parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/__init__.py` & `flavio-2.5.3/flavio/physics/bdecays/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/angular.py` & `flavio-2.5.3/flavio/physics/bdecays/angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bc_lifetime.py` & `flavio-2.5.3/flavio/physics/bdecays/bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bll.py` & `flavio-2.5.3/flavio/physics/bdecays/bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bllgamma.py` & `flavio-2.5.3/flavio/physics/bdecays/bllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/blnu.py` & `flavio-2.5.3/flavio/physics/bdecays/blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bpll.py` & `flavio-2.5.3/flavio/physics/bdecays/bpll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bpll_lfv.py` & `flavio-2.5.3/flavio/physics/bdecays/bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bpll_subleading.py` & `flavio-2.5.3/flavio/physics/bdecays/bpll_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bplnu.py` & `flavio-2.5.3/flavio/physics/bdecays/bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bpnunu.py` & `flavio-2.5.3/flavio/physics/bdecays/bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvgamma.py` & `flavio-2.5.3/flavio/physics/bdecays/bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/amplitudes.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/amplitudes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/lfv.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/nonfactorizable.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/nonfactorizable.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/observables.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/observables_bs.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/observables_bs.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf_interpolate.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/subleading.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/test_bvll.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/test_bvll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/test_lfv.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/test_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/test_qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py` & `flavio-2.5.3/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvlnu.py` & `flavio-2.5.3/flavio/physics/bdecays/bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bvnunu.py` & `flavio-2.5.3/flavio/physics/bdecays/bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bxgamma.py` & `flavio-2.5.3/flavio/physics/bdecays/bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bxll.py` & `flavio-2.5.3/flavio/physics/bdecays/bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bxll_qed.py` & `flavio-2.5.3/flavio/physics/bdecays/bxll_qed.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/bxlnu.py` & `flavio-2.5.3/flavio/physics/bdecays/bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/common.py` & `flavio-2.5.3/flavio/physics/bdecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/btop.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/btop.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/cln.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/test_btop.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_p/test_btop.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/btov.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/cln.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/clnexp.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/clnexp.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/isgurwise.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/isgurwise.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/sse.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/test_btov.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/b_v/test_btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/common.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/hqet.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/hqet.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/sse.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/formfactors/test_cln.py` & `flavio-2.5.3/flavio/physics/bdecays/formfactors/test_cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/lambdablambda1520ll.py` & `flavio-2.5.3/flavio/physics/bdecays/lambdablambda1520ll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/lambdablambdall.py` & `flavio-2.5.3/flavio/physics/bdecays/lambdablambdall.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/lambdablambdall_subleading.py` & `flavio-2.5.3/flavio/physics/bdecays/lambdablambdall_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/matrixelements.py` & `flavio-2.5.3/flavio/physics/bdecays/matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_angular.py` & `flavio-2.5.3/flavio/physics/bdecays/test_angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bc_lifetime.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bll.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bllgamma.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_blnu.py` & `flavio-2.5.3/flavio/physics/bdecays/test_blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bpll.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bpll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bpll_lfv.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bplnu.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bpnunu.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bvgamma.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bvlnu.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bvnunu.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bxgamma.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bxll.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_bxlnu.py` & `flavio-2.5.3/flavio/physics/bdecays/test_bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_lambdablambda1520ll.py` & `flavio-2.5.3/flavio/physics/bdecays/test_lambdablambda1520ll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_lambdablambdall.py` & `flavio-2.5.3/flavio/physics/bdecays/test_lambdablambdall.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_matrixelements.py` & `flavio-2.5.3/flavio/physics/bdecays/test_matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/test_wc.py` & `flavio-2.5.3/flavio/physics/bdecays/test_wc.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/bdecays/wilsoncoefficients.py` & `flavio-2.5.3/flavio/physics/bdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/betadecays/common.py` & `flavio-2.5.3/flavio/physics/betadecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/betadecays/ft.py` & `flavio-2.5.3/flavio/physics/betadecays/ft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/betadecays/test_betadecays.py` & `flavio-2.5.3/flavio/physics/betadecays/test_betadecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ckm.py` & `flavio-2.5.3/flavio/physics/ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/common.py` & `flavio-2.5.3/flavio/physics/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat` & `flavio-2.5.3/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/README` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/README`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat` & `flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat` & `flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d` & `flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat` & `flavio-2.5.3/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json` & `flavio-2.5.3/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml` & `flavio-2.5.3/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz` & `flavio-2.5.3/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy` & `flavio-2.5.3/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/dlnu.py` & `flavio-2.5.3/flavio/physics/ddecays/dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/dplnu.py` & `flavio-2.5.3/flavio/physics/ddecays/dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/formfactors/__init__.py` & `flavio-2.5.3/flavio/physics/ddecays/formfactors/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/formfactors/bcl.py` & `flavio-2.5.3/flavio/physics/ddecays/formfactors/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/formfactors/bsz.py` & `flavio-2.5.3/flavio/physics/ddecays/formfactors/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/formfactors/test_formfactors.py` & `flavio-2.5.3/flavio/physics/ddecays/formfactors/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/test_dlnu.py` & `flavio-2.5.3/flavio/physics/ddecays/test_dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/ddecays/test_dplnu.py` & `flavio-2.5.3/flavio/physics/ddecays/test_dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/dileptons/partondist.py` & `flavio-2.5.3/flavio/physics/dileptons/partondist.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/dileptons/ppll.py` & `flavio-2.5.3/flavio/physics/dileptons/ppll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/dileptons/pplnu.py` & `flavio-2.5.3/flavio/physics/dileptons/pplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/dileptons/test_ppll.py` & `flavio-2.5.3/flavio/physics/dileptons/test_ppll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/dileptons/test_pplnu.py` & `flavio-2.5.3/flavio/physics/dileptons/test_pplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/edms/common.py` & `flavio-2.5.3/flavio/physics/edms/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/edms/neutronedm.py` & `flavio-2.5.3/flavio/physics/edms/neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/edms/paraedm.py` & `flavio-2.5.3/flavio/physics/edms/paraedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/edms/test_neutronedm.py` & `flavio-2.5.3/flavio/physics/edms/test_neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/eft.py` & `flavio-2.5.3/flavio/physics/eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/elements.py` & `flavio-2.5.3/flavio/physics/elements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/higgs/decay.py` & `flavio-2.5.3/flavio/physics/higgs/decay.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/higgs/production.py` & `flavio-2.5.3/flavio/physics/higgs/production.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/higgs/signalstrength.py` & `flavio-2.5.3/flavio/physics/higgs/signalstrength.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/higgs/test_higgs.py` & `flavio-2.5.3/flavio/physics/higgs/test_higgs.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/higgs/width.py` & `flavio-2.5.3/flavio/physics/higgs/width.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/formfactors.py` & `flavio-2.5.3/flavio/physics/kdecays/formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/kll.py` & `flavio-2.5.3/flavio/physics/kdecays/kll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/klnu.py` & `flavio-2.5.3/flavio/physics/kdecays/klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/kpilnu.py` & `flavio-2.5.3/flavio/physics/kdecays/kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/kpinunu.py` & `flavio-2.5.3/flavio/physics/kdecays/kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/kpipi.py` & `flavio-2.5.3/flavio/physics/kdecays/kpipi.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/lambdaplnu.py` & `flavio-2.5.3/flavio/physics/kdecays/lambdaplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/test_formfactors.py` & `flavio-2.5.3/flavio/physics/kdecays/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/test_kll.py` & `flavio-2.5.3/flavio/physics/kdecays/test_kll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/test_klnu.py` & `flavio-2.5.3/flavio/physics/kdecays/test_klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/test_kpilnu.py` & `flavio-2.5.3/flavio/physics/kdecays/test_kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/test_kpinunu.py` & `flavio-2.5.3/flavio/physics/kdecays/test_kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/kdecays/wilsoncoefficients.py` & `flavio-2.5.3/flavio/physics/kdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mdms/al.py` & `flavio-2.5.3/flavio/physics/mdms/al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mdms/test_al.py` & `flavio-2.5.3/flavio/physics/mdms/test_al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mesonmixing/amplitude.py` & `flavio-2.5.3/flavio/physics/mesonmixing/amplitude.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mesonmixing/common.py` & `flavio-2.5.3/flavio/physics/mesonmixing/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mesonmixing/observables.py` & `flavio-2.5.3/flavio/physics/mesonmixing/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mesonmixing/test_mesonmixing.py` & `flavio-2.5.3/flavio/physics/mesonmixing/test_mesonmixing.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mesonmixing/wilsoncoefficient.py` & `flavio-2.5.3/flavio/physics/mesonmixing/wilsoncoefficient.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mudecays/mu3e.py` & `flavio-2.5.3/flavio/physics/mudecays/mu3e.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mudecays/mueconversion.py` & `flavio-2.5.3/flavio/physics/mudecays/mueconversion.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mudecays/muegamma.py` & `flavio-2.5.3/flavio/physics/mudecays/muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/mudecays/test_muegamma.py` & `flavio-2.5.3/flavio/physics/mudecays/test_muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/neutrinos/test_trident.py` & `flavio-2.5.3/flavio/physics/neutrinos/test_trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/neutrinos/trident.py` & `flavio-2.5.3/flavio/physics/neutrinos/trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/Pll.py` & `flavio-2.5.3/flavio/physics/quarkonium/Pll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/Sll.py` & `flavio-2.5.3/flavio/physics/quarkonium/Sll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/Vll.py` & `flavio-2.5.3/flavio/physics/quarkonium/Vll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/Vllgamma.py` & `flavio-2.5.3/flavio/physics/quarkonium/Vllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/test_Pll.py` & `flavio-2.5.3/flavio/physics/quarkonium/test_Pll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/test_Sll.py` & `flavio-2.5.3/flavio/physics/quarkonium/test_Sll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/test_Vll.py` & `flavio-2.5.3/flavio/physics/quarkonium/test_Vll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/quarkonium/test_Vllgamma.py` & `flavio-2.5.3/flavio/physics/quarkonium/test_Vllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/running/betafunctions.py` & `flavio-2.5.3/flavio/physics/running/betafunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/running/masses.py` & `flavio-2.5.3/flavio/physics/running/masses.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/running/running.py` & `flavio-2.5.3/flavio/physics/running/running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/running/test_running.py` & `flavio-2.5.3/flavio/physics/running/test_running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/scattering/ee_ww.py` & `flavio-2.5.3/flavio/physics/scattering/ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/scattering/test_ee_ww.py` & `flavio-2.5.3/flavio/physics/scattering/test_ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/common.py` & `flavio-2.5.3/flavio/physics/taudecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/tau3l.py` & `flavio-2.5.3/flavio/physics/taudecays/tau3l.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/taulgamma.py` & `flavio-2.5.3/flavio/physics/taudecays/taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/taulnunu.py` & `flavio-2.5.3/flavio/physics/taudecays/taulnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/taupl.py` & `flavio-2.5.3/flavio/physics/taudecays/taupl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/taupnu.py` & `flavio-2.5.3/flavio/physics/taudecays/taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/tauvl.py` & `flavio-2.5.3/flavio/physics/taudecays/tauvl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/test_taulgamma.py` & `flavio-2.5.3/flavio/physics/taudecays/test_taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/test_taulnunu.py` & `flavio-2.5.3/flavio/physics/taudecays/test_taulnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/taudecays/test_taupnu.py` & `flavio-2.5.3/flavio/physics/taudecays/test_taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/test_ckm.py` & `flavio-2.5.3/flavio/physics/test_ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/test_common.py` & `flavio-2.5.3/flavio/physics/test_common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/test_eft.py` & `flavio-2.5.3/flavio/physics/test_eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/units.py` & `flavio-2.5.3/flavio/physics/units.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/wdecays/gammaw.py` & `flavio-2.5.3/flavio/physics/wdecays/gammaw.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/wdecays/mw.py` & `flavio-2.5.3/flavio/physics/wdecays/mw.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/wdecays/test_mW.py` & `flavio-2.5.3/flavio/physics/wdecays/test_mW.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/wdecays/test_wdecays.py` & `flavio-2.5.3/flavio/physics/wdecays/test_wdecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/zdecays/afbz.py` & `flavio-2.5.3/flavio/physics/zdecays/afbz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/zdecays/gammaz.py` & `flavio-2.5.3/flavio/physics/zdecays/gammaz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/zdecays/gammazsm.py` & `flavio-2.5.3/flavio/physics/zdecays/gammazsm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/zdecays/smeftew.py` & `flavio-2.5.3/flavio/physics/zdecays/smeftew.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/physics/zdecays/test_zdecays.py` & `flavio-2.5.3/flavio/physics/zdecays/test_zdecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/plots/__init__.py` & `flavio-2.5.3/flavio/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/plots/colors.py` & `flavio-2.5.3/flavio/plots/colors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/plots/plotfunctions.py` & `flavio-2.5.3/flavio/plots/plotfunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/plots/test_plotfunctions.py` & `flavio-2.5.3/flavio/plots/test_plotfunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/statistics/functions.py` & `flavio-2.5.3/flavio/statistics/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/statistics/likelihood.py` & `flavio-2.5.3/flavio/statistics/likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/statistics/probability.py` & `flavio-2.5.3/flavio/statistics/probability.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/statistics/test_functions.py` & `flavio-2.5.3/flavio/statistics/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/statistics/test_likelihood.py` & `flavio-2.5.3/flavio/statistics/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/statistics/test_probability.py` & `flavio-2.5.3/flavio/statistics/test_probability.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/test_citations.py` & `flavio-2.5.3/flavio/test_citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/test_classes.py` & `flavio-2.5.3/flavio/test_classes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/test_functions.py` & `flavio-2.5.3/flavio/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/test_measurements.py` & `flavio-2.5.3/flavio/test_measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/test_parameters.py` & `flavio-2.5.3/flavio/test_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/test_parseerrors.py` & `flavio-2.5.3/flavio/test_parseerrors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio/util.py` & `flavio-2.5.3/flavio/util.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/flavio.egg-info/PKG-INFO` & `flavio-2.5.3/flavio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.5.2
+Version: 2.5.3
 Summary: A Python package for flavour physics phenomenology in the Standard Model and beyond
 Home-page: https://flav-io.github.io
 Author: David M. Straub
 Author-email: straub@protonmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flavio Version: 2.5.2 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.3 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
```

### Comparing `flavio-2.5.2/flavio.egg-info/SOURCES.txt` & `flavio-2.5.3/flavio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flavio-2.5.2/setup.py` & `flavio-2.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
                 'physics/data/arXiv-1811-00983v1/*',
                 'physics/data/arXiv-2102.07233v2/*',
                 'physics/data/qcdf_interpolate/*',
                 'physics/data/wcsm/*',
                 ]
       },
       install_requires=['numpy>=1.20.0', 'scipy', 'setuptools>=3.3', 'pyyaml',
-                        'ckmutil', 'wilson>=2.0', 'particle>=0.16.0', 'parton>=0.2.1', ],
+                        'ckmutil', 'wilson>=2.0', 'particle>=0.21.0', 'parton>=0.2.1', ],
       extras_require={
             'testing': ['nose2'],
             'plotting': ['matplotlib>=2.0'],
             'sampling': ['iminuit>=2.0'],
             },
     )
```

