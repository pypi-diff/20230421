# Comparing `tmp/flavio-2.5.1.tar.gz` & `tmp/flavio-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flavio-2.5.1.tar", last modified: Fri Apr 21 14:31:14 2023, max compression
+gzip compressed data, was "flavio-2.5.2.tar", last modified: Fri Apr 21 17:48:48 2023, max compression
```

## Comparing `flavio-2.5.1.tar` & `flavio-2.5.2.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.703663 flavio-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-21 14:26:37.000000 flavio-2.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:26:37.000000 flavio-2.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 14:31:14.703663 flavio-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-21 14:26:37.000000 flavio-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.675663 flavio-2.5.1/flavio/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.675663 flavio-2.5.1/flavio/data/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/citations.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)   982462 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/measurements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    26756 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/parameters_correlated.yml
--rw-r--r--   0 runner    (1001) docker     (123)    86949 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/parameters_metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/parameters_uncorrelated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.675663 flavio-2.5.1/flavio/data/test/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/2009.09313_digitized.npz
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/SPheno-2.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/SPheno.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/data/test/wcxf-flavio-example.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.679663 flavio-2.5.1/flavio/io/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/io/instanceio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/io/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.679663 flavio-2.5.1/flavio/math/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/math/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/math/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/math/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/math/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/math/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/math/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.679663 flavio-2.5.1/flavio/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.683663 flavio-2.5.1/flavio/physics/bdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/angular.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bll.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bpll_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.683663 flavio-2.5.1/flavio/physics/bdecays/bvll/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/nonfactorizable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/observables_bs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/test_bvll.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/test_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/test_qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bxll_qed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.683663 flavio-2.5.1/flavio/physics/bdecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.683663 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_gamma/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.687663 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/btop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/test_btop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.687663 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/clnexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/test_btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/hqet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.687663 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.687663 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/formfactors/test_cln.py
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/lambdablambdagamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/lambdablambdall_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_angular.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bll.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bvgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/test_wc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/bdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.687663 flavio-2.5.1/flavio/physics/betadecays/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/betadecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/betadecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/betadecays/ft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/betadecays/test_betadecays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.667663 flavio-2.5.1/flavio/physics/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.687663 flavio-2.5.1/flavio/physics/data/arXiv-0810-4077v3/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-0810-4077v3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/README
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/
--rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/
--rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/
--rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/arXiv-2102.07233v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/qcdf_interpolate/
--rw-r--r--   0 runner    (1001) docker     (123)   146774 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.691663 flavio-2.5.1/flavio/physics/data/wcsm/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/ddecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/ddecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/formfactors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/formfactors/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/formfactors/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/formfactors/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/rge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/test_dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/ddecays/test_dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/dileptons/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/dileptons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/dileptons/partondist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/dileptons/ppll.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/dileptons/pplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/dileptons/test_ppll.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/dileptons/test_pplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/edms/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/edms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/edms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/edms/neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/edms/paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/edms/slcouplings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/edms/test_neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/edms/test_paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/eft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/higgs/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/higgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/higgs/decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/higgs/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/higgs/signalstrength.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/higgs/test_higgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/higgs/width.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/kdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/test_kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/test_klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/test_kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/test_kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/test_kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/test_lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/kdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/mdms/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mdms/al.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mdms/test_al.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.695663 flavio-2.5.1/flavio/physics/mesonmixing/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mesonmixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mesonmixing/amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mesonmixing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mesonmixing/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mesonmixing/test_mesonmixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mesonmixing/wilsoncoefficient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/mudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mudecays/mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mudecays/mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mudecays/muegamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mudecays/test_mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mudecays/test_mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/mudecays/test_muegamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/neutrinos/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/neutrinos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/neutrinos/test_trident.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/neutrinos/trident.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/quarkonium/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/Pll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/Sll.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/Vll.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/Vllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/test_Pll.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/test_Sll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/test_Vll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/quarkonium/test_Vllgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/running/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/running/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/running/betafunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/running/masses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/running/running.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/running/test_running.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/scattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/scattering/ee_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/scattering/test_ee_ww.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/taudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/test_tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/test_taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/test_taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/test_taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/test_taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/taudecays/test_tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/test_ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/test_eft.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/wdecays/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/wdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/wdecays/gammaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/wdecays/mw.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/wdecays/test_mW.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/wdecays/test_wdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.699663 flavio-2.5.1/flavio/physics/zdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/zdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/zdecays/afbz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/zdecays/gammaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/zdecays/gammazsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/zdecays/smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/zdecays/test_smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/physics/zdecays/test_zdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.703663 flavio-2.5.1/flavio/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/plots/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/plots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39693 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/plots/plotfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/plots/test_plotfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.703663 flavio-2.5.1/flavio/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/statistics/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/statistics/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/statistics/probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/statistics/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/statistics/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    37591 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/statistics/test_probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/test_parseerrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-21 14:26:37.000000 flavio-2.5.1/flavio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:31:14.675663 flavio-2.5.1/flavio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 14:31:14.000000 flavio-2.5.1/flavio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-04-21 14:31:14.000000 flavio-2.5.1/flavio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:31:14.000000 flavio-2.5.1/flavio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 14:31:14.000000 flavio-2.5.1/flavio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 14:31:14.000000 flavio-2.5.1/flavio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:31:14.703663 flavio-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-21 14:26:37.000000 flavio-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-21 17:44:13.000000 flavio-2.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 17:44:13.000000 flavio-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 17:48:48.563819 flavio-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-21 17:44:13.000000 flavio-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.511818 flavio-2.5.2/flavio/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.515818 flavio-2.5.2/flavio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/citations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   984881 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/measurements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26734 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/parameters_correlated.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    86949 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/parameters_metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/parameters_uncorrelated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.519818 flavio-2.5.2/flavio/data/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/2009.09313_digitized.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/SPheno-2.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/SPheno.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/data/test/wcxf-flavio-example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.519818 flavio-2.5.2/flavio/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/instanceio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.523818 flavio-2.5.2/flavio/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/math/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.523818 flavio-2.5.2/flavio/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.535819 flavio-2.5.2/flavio/physics/bdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpll_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/bvll/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/nonfactorizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/observables_bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_bvll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxll_qed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/btop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/test_btop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/clnexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/test_btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/hqet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/formfactors/test_cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambdagamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/lambdablambdall_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bvgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/test_wc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/bdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.539819 flavio-2.5.2/flavio/physics/betadecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/betadecays/test_betadecays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.503818 flavio-2.5.2/flavio/physics/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.547819 flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.551819 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.551819 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.551819 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/
+-rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/arXiv-2102.07233v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/qcdf_interpolate/
+-rw-r--r--   0 runner    (1001) docker     (123)   146774 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/data/wcsm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/ddecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/ddecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/formfactors/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/rge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/test_dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/ddecays/test_dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/dileptons/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/partondist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/pplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/test_ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/dileptons/test_pplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/edms/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/slcouplings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/test_neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/edms/test_paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.555819 flavio-2.5.2/flavio/physics/higgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/signalstrength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/test_higgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/higgs/width.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/kdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/test_lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/kdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/mdms/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mdms/al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mdms/test_al.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/mesonmixing/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/test_mesonmixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mesonmixing/wilsoncoefficient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/mudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/muegamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/test_mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/test_mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/mudecays/test_muegamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/neutrinos/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/neutrinos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/neutrinos/test_trident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/neutrinos/trident.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/quarkonium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/Vllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/quarkonium/test_Vllgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/running/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/betafunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/running.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/running/test_running.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.559819 flavio-2.5.2/flavio/physics/scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/scattering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/scattering/ee_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/scattering/test_ee_ww.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/physics/taudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/taudecays/test_tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/test_ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/test_eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/physics/wdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/gammaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/mw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/test_mW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/wdecays/test_wdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/physics/zdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/afbz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/gammaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/gammazsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/test_smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/physics/zdecays/test_zdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39693 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/plotfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/plots/test_plotfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.563819 flavio-2.5.2/flavio/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37591 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/statistics/test_probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/test_parseerrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-21 17:44:13.000000 flavio-2.5.2/flavio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 17:48:48.515818 flavio-2.5.2/flavio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 17:48:48.000000 flavio-2.5.2/flavio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 17:48:48.563819 flavio-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-21 17:44:13.000000 flavio-2.5.2/setup.py
```

### Comparing `flavio-2.5.1/LICENSE.txt` & `flavio-2.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/PKG-INFO` & `flavio-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.5.1
+Version: 2.5.2
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
-Metadata-Version: 2.1 Name: flavio Version: 2.5.1 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.2 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
```

### Comparing `flavio-2.5.1/README.md` & `flavio-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/__init__.py` & `flavio-2.5.2/flavio/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/_parse_errors.py` & `flavio-2.5.2/flavio/_parse_errors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/citations.py` & `flavio-2.5.2/flavio/citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/classes.py` & `flavio-2.5.2/flavio/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
         # Read the uncorrelated parameter values from the default YAML data file
         _read_yaml_object_values(pkgutil.get_data('flavio', 'data/parameters_uncorrelated.yml'), self)
 
         # Read the correlated parameter values from the default YAML data file
         _read_yaml_object_values_correlated(pkgutil.get_data('flavio', 'data/parameters_correlated.yml'), self)
 
         # Read the parameters from the default PDG data file
-        read_pdg(2018, self)
+        read_pdg(2022, self)
 
         # Read default parameters for B->V form factors
         flavio.physics.bdecays.formfactors.b_v.bsz_parameters.bsz_load('v2', 'LCSR', ('B->omega', 'B->rho'), self)
         flavio.physics.bdecays.formfactors.b_v.bsz_parameters.bsz_load('v2', 'LCSR-Lattice', ('B->K*', 'Bs->phi', 'Bs->K*'), self)
 
         # Read default parameters for B->P form factors
         flavio.physics.bdecays.formfactors.b_p.bsz_parameters.gkvd_load('v1', 'LCSR-Lattice', ('B->K', 'B->pi'), self)
```

### Comparing `flavio-2.5.1/flavio/data/citations.yml` & `flavio-2.5.2/flavio/data/citations.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/data/config.yml` & `flavio-2.5.2/flavio/data/config.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/data/measurements.yml` & `flavio-2.5.2/flavio/data/measurements.yml`

 * *Files 0% similar despite different names*

```diff
@@ -4177,14 +4177,42 @@
     BR(KL->pienu): (40.55±0.11)1e-2
     BR(KS->pimunu): (4.69±0.05)1e-4
     BR(KS->pienu): (7.04±0.08)1e-4
     BR(K+->pimunu): (3.352±0.033)1e-2
     BR(K+->pienu): (5.07±0.04)1e-2
     Gamma(pi+->munu): (2.52809±0.00050)1e-17
 
+# When updating Gamma(pi+->munu) or BR(K+->munu),
+# RKpi(P+->munu) under "CKM ratio measurements"
+# should be updated as well!
+PDG 2022:
+  experiment: PDG
+  inspire: ParticleDataGroup:2022pth
+  values:
+    BR(pi+->enu): (1.230±0.004)1e-4
+    BR(K+->munu): (63.56±0.11)1e-2
+    Remu(K+->lnu): 2.488±0.009e-5
+    BR(KL->pimunu): (27.04±0.07)1e-2
+    BR(KL->pienu): (40.55±0.11)1e-2
+    BR(K+->pimunu): (3.352±0.033)1e-2
+    BR(K+->pienu): (5.07±0.04)1e-2
+    Gamma(pi+->munu): (2.52809±0.00050)1e-17
+
+KLOE-2 KS->pimunu 2019:
+  experiment: KLOE-2
+  inspire: KLOE-2:2019rev
+  values:
+    BR(KS->pimunu): (4.56±0.20)1e-4
+
+KLOE-2 KS->pienu 2022:
+  experiment: KLOE-2
+  inspire: KLOE-2:2022dot
+  values:
+    BR(KS->pienu): (7.153±0.057)1e-4
+
 PiENu pi->enu 2015:
   experiment: PiENu
   inspire: Aguilar-Arevalo:2015cdf
   values:
     BR(pi+->enu): (1.2344±0.0023±0.0019)1e-4
 
 CKM ratio measurements:
@@ -7385,14 +7413,20 @@
 
 K+->pinunu NA62 2019:
   experiment: NA62
   url: https://indico.cern.ch/event/846814/attachments/1903630/3161337/CERN_seminar_23_09_2019.pdf
   values:
     BR(K+->pinunu): 0.47 + 0.72 - 0.47 e-10
 
+K+->pinunu NA62 2021:
+  experiment: NA62
+  inspire: NA62:2021zjw
+  values:
+    BR(K+->pinunu): 1.06 + 0.40 - 0.34 +- 0.09 e-10
+
 KL->pinunu KOTO 2018:
   experiment: KOTO
   inspire: Ahn:2018mvc
   values:
     BR(KL->pinunu): < 3.0e-9 @ 90% CL
 
 PDG 2018 Kll:
@@ -10905,17 +10939,17 @@
     # to convert numbers from picoseconds to 1/GeV, multiply by
     # ps = 1.519267447878626e+12 [1/GeV],
     tau_mumu: (2.78 +0.35 -0.30 ± 0.06) 1e12 # this is 1.83 +0.23 -0.20 ± 0.04 ps
 
 
 Bc lifetime:
   experiment: PDG
-  inspire: Tanabashi:2018oca
+  inspire: ParticleDataGroup:2022pth
   values:
-    tau_Bc: (7.704 ± 0.137) 1e11
+    tau_Bc: (7.748 ± 0.137) 1e11
 
 
 Belle RK* 2019:
   experiment: Belle
   inspire: Abdesselam:2019wac
   values:
     - name: <Rmue>(B+->K*ll)
@@ -12132,14 +12166,33 @@
     Ft(42Sc): 4.6678 ± 0.0035 1e+27  # 3072.4 ± 2.3 s
     Ft(46V): 4.6704 ± 0.003 1e+27  # 3074.1 ± 2.0 s
     Ft(50Mn): 4.666 ± 0.0032 1e+27  # 3071.2 ± 2.1 s
     Ft(54Co): 4.6638 ± 0.004 1e+27  # 3069.8 ± 2.6 s
     Ft(62Ga): 4.6664 ± 0.0102 1e+27  # 3071.5 ± 6.7 s
     Ft(74Rb): 4.6733 ± 0.0167 1e+27  # 3076.0 ± 11.0 s
 
+Ft(0+) Hardy/Towner 2020:
+  experiment: various
+  inspire: Hardy:2020qwl
+  values:
+    Ft(10C): 4.6728 ± 0.0067 1e+27  # 3075.7 ± 4.4 s
+    Ft(14O): 4.6645 ± 0.0029 1e+27  # 3070.2 ± 1.9 s
+    Ft(22Mg): 4.6736 ± 0.0106 1e+27  # 3076.2 ± 7.0 s
+    Ft(26mAl): 4.6678 ± 0.0017 1e+27  # 3072.4 ± 1.1 s
+    Ft(34Cl): 4.6666 ± 0.0027 1e+27  # 3071.6 ± 1.8 s
+    Ft(34Ar): 4.6719 ± 0.0047 1e+27  # 3075.1 ± 3.1 s
+    Ft(38mK): 4.6686 ± 0.003 1e+27  # 3072.9 ± 2.0 s
+    Ft(38Ca): 4.6760 ± 0.0094 1e+27  # 3077.8 ± 6.2 s
+    Ft(42Sc): 4.6667 ± 0.0030 1e+27  # 3071.7 ± 2.0 s
+    Ft(46V): 4.6707 ± 0.003 1e+27  # 3074.3 ± 2.0 s
+    Ft(50Mn): 4.6658 ± 0.0024 1e+27  # 3071.1 ± 1.6 s
+    Ft(54Co): 4.6648 ± 0.0036 1e+27  # 3070.4 ± 2.5 s
+    Ft(62Ga): 4.6678 ± 0.0102 1e+27  # 3072.4 ± 6.7 s
+    Ft(74Rb): 4.6748 ± 0.0167 1e+27  # 3077.0 ± 11.0 s
+
 Neutron averages GACS 2018 1:
   inspire: Gonzalez-Alonso:2018omy
   description: Averages in table 7 of the paper by Gonzalez-Alonso et al.
   values:
     - name: tau_n
       me_E: 0.655
       value: 1.3366(12) 1e+27 # 879.75(76) s
@@ -12229,14 +12282,36 @@
     BR(D0->pimunu): (2.37 ± 0.24) 1e-3
     BR(D0->Kenu): (3.53 ± 0.028) 1e-2
     BR(D0->Kmunu): (3.31 ± 0.13) 1e-2
     BR(D+->pienu): (3.72 ± 0.17) 1e-3
     BR(D+->Kenu): (8.73 ± 0.10) 1e-2
     BR(D+->Kmunu): (8.74 ± 0.19) 1e-2
 
+PDG 2022 D->lnu:
+  inspire: ParticleDataGroup:2022pth
+  values:
+    BR(D+->enu): < 8.8e-6 @ 90% CL
+    BR(D+->munu): (3.74 ± 0.17) 1e-4
+    BR(D+->taunu): (1.20 ± 0.27) 1e-3
+    BR(Ds->enu): < 8.3e-5 @ 90% CL
+    BR(Ds->munu): (5.43 ± 0.15) 1e-3
+    BR(Ds->taunu): (5.32 ± 0.11) 1e-2
+
+PDG 2022 D->Plnu:
+  inspire: ParticleDataGroup:2022pth
+  values:
+    BR(D0->pienu): (2.91 ± 0.04) 1e-3
+    BR(D0->pimunu): (2.67 ± 0.12) 1e-3
+    BR(D0->Kenu): (3.549 ± 0.026) 1e-2
+    BR(D0->Kmunu): (3.41 ± 0.04) 1e-2
+    BR(D+->pienu): (3.72 ± 0.17) 1e-3
+    BR(D+->pimunu): (3.50 ± 0.15) 1e-3
+    BR(D+->Kenu): (8.72 ± 0.09) 1e-2
+    BR(D+->Kmunu): (8.76 ± 0.19) 1e-2
+    
 BESIII D0->Kenu 2015:
   observables:
   - name: <BR>(D0->Kenu)
     q2max: 0.1
     q2min: 0.0
   - name: <BR>(D0->Kenu)
     q2max: 0.2
```

### Comparing `flavio-2.5.1/flavio/data/parameters_correlated.yml` & `flavio-2.5.2/flavio/data/parameters_correlated.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,23 +31,24 @@
 #
 # The f_K uncertainty and correlation are calculated by assuming f_pi and
 # f_K/f_pi are totally uncorrelated - see discussion at
 # https://github.com/flav-io/flavio/issues/171 and/or the code at
 # https://gist.github.com/DavidMStraub/813bd0c4296837936a188a29c8d8b981
 -
   values:
-    - f_K+: 0.1554(10)  # reproduce f_K/f_pi=1.1932(19) from FLAG 2019 Nf=2+1+1
+    - f_K+: 0.1554(10)  # reproduce f_K/f_pi=1.1932(21) from FLAG 2021 Nf=2+1+1
     - f_K0: 0.1554(10)
-    - f_pi+: 0.1302(8)  # FLAG 2019 Nf=2+1
+    - f_pi+: 0.1302(8)  # FLAG 2021 Nf=2+1
     - f_pi0: 0.1302(8)
   correlation:
-    [[1, 0.99, 0.968, 0.968],
-     [0.99, 1, 0.968, 0.968],
-     [0.968, 0.968, 1, 0.99],
-     [0.968, 0.968, 0.99, 1]]
+    [[1, 0.99, 0.961, 0.961],
+     [0.99, 1, 0.961, 0.961],
+     [0.961, 0.961, 1, 0.99],
+     [0.961, 0.961, 0.99, 1]]
+
 -
   values:
     - f_perp_K*+: 0.145(6)  # 1503.05534v2 table 1, but at 2 GeV
     - f_perp_K*0: 0.145(6)
   correlation: 0.99
 -
   values:
@@ -388,22 +389,22 @@
     - delta_BXdmumu high: 0 ± 0.10
     - delta_BXdtautau high: 0 ± 0.10
   correlation: [[1, 0.9, 0.9], [1, 0.98], [1]] # assuming 90% corr. for e/mu, 98% for tau/mu
 
 
 # Electromagnetic corrections in Kl3 decays
 # 1005.2323 table 1 & eq. 18
+# Set just the Kmu3 parameters here, as we use 
+# updated Ke3 values (but without correlations)
 -
   values:
-    - K0e3 delta_EM: 0.495(110)1e-2
-    - K+e3 delta_EM: 0.050(125)1e-2
     - K0mu3 delta_EM: 0.700(110)1e-2
     - K+mu3 delta_EM: 0.008(125)1e-2
   correlation:
-    [[1, 0.081, 0.685, -0.147], [1, -0.147, 0.764], [1, 0.081], [1]]
+    [[1, 0.081], [1]]
 
 
 # Parameters for HQET form factors
 - values:
     - CLN rho2_xi: 1.068 ± 0.206
     - CLN c_xi: 0.946 ± 0.247
     - CLN xi3: -3.746 ± 1.087
```

### Comparing `flavio-2.5.1/flavio/data/parameters_metadata.yml` & `flavio-2.5.2/flavio/data/parameters_metadata.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/data/parameters_uncorrelated.yml` & `flavio-2.5.2/flavio/data/parameters_uncorrelated.yml`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 # CKM parameters
 
 Vus: 0.2248(8)   # FLAG 2017 Nf=2+1+1
 Vub: 3.73(14)e-3  # FLAG 2017 Nf=2+1 B->pilnu
 Vcb: 4.221(78)e-2
-delta: 1.27(12)  # delta = gamma to excellent approximation
+delta: 1.15(6)  # PDG 2022 (delta = gamma to excellent approximation)
 
 
 # Meson decay constants
 
 f_rho0: 0.212(4)  # 1501.06569 table 1
 f_omega: 0.185(5)  # 1501.06569 table 1
 f_phi: 0.231(5)  # 1501.06569 table 1
@@ -230,18 +230,18 @@
 c1_pi+lnu: -2.56(50) # (115) of 0707.4464
 c2_pi+lnu: 5.2(0.4)(0.01) # table 1 of 0707.4464
 c3_pi+lnu: -10.5(2.3)(0.53) # matching error inflated by factor 4!
 c4_pi+munu: 1.69(0.07)
 c2t_pi+lnu: 0
 
 # Parameters needed for K->pi form factors
-K->pi f+(0): 0.9696(15)(12)        # 1809.02827
+K->pi f+(0): 0.9698(17)            # FLAG 2021 Nf=2+1+1 average
 K->pi fT(0): 0.417(15)             # 1108.1021
 K->pi sT: 1.10(14)                 #  "
-K->pi delta_K+pi0: 0.029(4)        # 1005.2323
+K->pi delta_K+pi0: 0.0252(11)      # 2208.11707, in text of sec. 2
 K->pi ln(C): 0.1998(138)           # 1602.04113
 K->pi Lambda_+: 24.22(1.16) 1e-3   #  "
 K->pi D: 0.0209(21)                # 0903.1654 table 1
 K->pi d: 0.0398(44)                #  "
 K->pi k: 0.0045(4)                 #  "
 K->pi H1: (1.92 + 0.63 - 0.32) e-3 # 0903.1654 table 2
 K->pi H2: (2.63 + 0.28 - 0.15) e-4 #  "
@@ -517,15 +517,15 @@
 CLN lp_2(1): 0
 CLN lp_3(1): 0
 CLN lp_4(1): 0
 CLN lp_5(1): 0
 CLN lp_6(1): 0
 
 # Parameters for beta decays
-DeltaRV: 0.02361(38)  # Marciano/Sirlin, arXiv:hep-ph/0510099
+DeltaRV: 0.02467(27)  # Average from 2208.11707
 # one third of the Z^2alpha^3 term in table V of 0710.3181,
 # as suggested in 1411.5987
 delta_deltaRp_Z2: 0 ± 0.00004e-2
 f_n: 1.6887(1)  # Hardy & Towner
 deltaRp_n: 0.014902(2)
 Lambda->p f_1(0): -1.2247 ± 0.05  # -sqrt(3/2) +-  "few percent"
 Lambda->p g_1(0): -0.88(9)  # see 1605.07114, 1102.3407; 10% SU(3) breaking
@@ -550,7 +550,13 @@
   lowest_value: 0
   highest_value: 100
   central_value: 0
 
 # Parameter for Bs->K*0mumu uncertainty inside resonant regions
 # 2209.04457, appendix B, Eq. B7, we save a relative uncertainty
 delta_BsKstarmumu: 0 ± 0.078
+# Updated EM corrections for Ke3 decays
+# From 2103.04843 (Table VI) 
+# Uncertainties combined in quadrature, factor of 2 normalisation difference since
+# flavio used the normalisation of 1005.2323
+K0e3 delta_EM: 0.580(16)1e-2
+K+e3 delta_EM: 0.105(24)1e-2
```

### Comparing `flavio-2.5.1/flavio/data/test/2009.09313_digitized.npz` & `flavio-2.5.2/flavio/data/test/2009.09313_digitized.npz`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/data/test/SPheno-2.spc.MSSM` & `flavio-2.5.2/flavio/data/test/SPheno-2.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/data/test/SPheno.spc.MSSM` & `flavio-2.5.2/flavio/data/test/SPheno.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/functions.py` & `flavio-2.5.2/flavio/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/io/instanceio.py` & `flavio-2.5.2/flavio/io/instanceio.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/io/test_yaml.py` & `flavio-2.5.2/flavio/io/test_yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/io/yaml.py` & `flavio-2.5.2/flavio/io/yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/math/functions.py` & `flavio-2.5.2/flavio/math/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/math/integrate.py` & `flavio-2.5.2/flavio/math/integrate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/math/optimize.py` & `flavio-2.5.2/flavio/math/optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/math/test_math.py` & `flavio-2.5.2/flavio/math/test_math.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/math/test_optimize.py` & `flavio-2.5.2/flavio/math/test_optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/measurements.py` & `flavio-2.5.2/flavio/measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/parameters.py` & `flavio-2.5.2/flavio/parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/__init__.py` & `flavio-2.5.2/flavio/physics/bdecays/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/angular.py` & `flavio-2.5.2/flavio/physics/bdecays/angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bc_lifetime.py` & `flavio-2.5.2/flavio/physics/bdecays/bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bll.py` & `flavio-2.5.2/flavio/physics/bdecays/bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bllgamma.py` & `flavio-2.5.2/flavio/physics/bdecays/bllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/blnu.py` & `flavio-2.5.2/flavio/physics/bdecays/blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bpll.py` & `flavio-2.5.2/flavio/physics/bdecays/bpll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bpll_lfv.py` & `flavio-2.5.2/flavio/physics/bdecays/bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bpll_subleading.py` & `flavio-2.5.2/flavio/physics/bdecays/bpll_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bplnu.py` & `flavio-2.5.2/flavio/physics/bdecays/bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bpnunu.py` & `flavio-2.5.2/flavio/physics/bdecays/bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvgamma.py` & `flavio-2.5.2/flavio/physics/bdecays/bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/amplitudes.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/amplitudes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/lfv.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/nonfactorizable.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/nonfactorizable.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/observables.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/observables_bs.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/observables_bs.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/qcdf.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/qcdf_interpolate.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/subleading.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/test_bvll.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/test_bvll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/test_lfv.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/test_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/test_qcdf.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py` & `flavio-2.5.2/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvlnu.py` & `flavio-2.5.2/flavio/physics/bdecays/bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bvnunu.py` & `flavio-2.5.2/flavio/physics/bdecays/bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bxgamma.py` & `flavio-2.5.2/flavio/physics/bdecays/bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bxll.py` & `flavio-2.5.2/flavio/physics/bdecays/bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bxll_qed.py` & `flavio-2.5.2/flavio/physics/bdecays/bxll_qed.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/bxlnu.py` & `flavio-2.5.2/flavio/physics/bdecays/bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/common.py` & `flavio-2.5.2/flavio/physics/bdecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bsz.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/btop.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/btop.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/cln.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_p/test_btop.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_p/test_btop.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/bsz.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/btov.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/cln.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/clnexp.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/clnexp.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/isgurwise.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/isgurwise.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/sse.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/b_v/test_btov.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/b_v/test_btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/common.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/hqet.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/hqet.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/sse.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/formfactors/test_cln.py` & `flavio-2.5.2/flavio/physics/bdecays/formfactors/test_cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/lambdablambda1520ll.py` & `flavio-2.5.2/flavio/physics/bdecays/lambdablambda1520ll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/lambdablambdall.py` & `flavio-2.5.2/flavio/physics/bdecays/lambdablambdall.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/lambdablambdall_subleading.py` & `flavio-2.5.2/flavio/physics/bdecays/lambdablambdall_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/matrixelements.py` & `flavio-2.5.2/flavio/physics/bdecays/matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_angular.py` & `flavio-2.5.2/flavio/physics/bdecays/test_angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bc_lifetime.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bll.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bllgamma.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_blnu.py` & `flavio-2.5.2/flavio/physics/bdecays/test_blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bpll.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bpll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bpll_lfv.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bplnu.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bpnunu.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bvgamma.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bvlnu.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bvnunu.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bxgamma.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bxll.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_bxlnu.py` & `flavio-2.5.2/flavio/physics/bdecays/test_bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_lambdablambda1520ll.py` & `flavio-2.5.2/flavio/physics/bdecays/test_lambdablambda1520ll.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         br_inv2 = 2e9/br
 
         # Comparison to figure 6 in arXiv:2009.09313v2
         # Scale factor BRinv2 used since in np-array factor e^(-9) not included
         dBR = 'dBR/dq2(Lambdab->Lambda(1520)mumu)'
         self.assert_sm_arrays(dBR, sm_array['dB_central'], 'central', scalef=br_inv2, rtol=0.02, atol=0.03)
         self.assert_sm_arrays(dBR, sm_array['dB_upper'], 'upper', scalef=br_inv2, rtol=0.08, atol=0.03)
-        self.assert_sm_arrays(dBR, sm_array['dB_lower'], 'lower', scalef=br_inv2, rtol=0.08, atol=0.03)
+        self.assert_sm_arrays(dBR, sm_array['dB_lower'], 'lower', scalef=br_inv2, rtol=0.12, atol=0.03)
 
         # Comparison to figure 9 right in arXiv:2009.09313v2
         Afb = 'AFBl(Lambdab->Lambda(1520)mumu)'
         self.assert_sm_arrays(Afb, sm_array['AFBl_central'], 'central', rtol=0.02, atol=0.03)
         self.assert_sm_arrays(Afb, sm_array['AFBl_upper'], 'upper', rtol=0.08, atol=0.03)
         self.assert_sm_arrays(Afb, sm_array['AFBl_lower'], 'lower', rtol=0.08, atol=0.03)
 
@@ -90,32 +90,32 @@
 
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', 0.048, rtol=0.57, q2min=0.1, q2max=3)
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.127, rtol=0.16, q2min=3, q2max=6)
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.235, rtol=0.03, q2min=6, q2max=8.68)
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.098, rtol=0.24, q2min=1, q2max=6)
 
 
-        self.assert_obs('<S_1cc>(Lambdab->Lambda(1520)mumu)', 0.181, rtol=0.29, q2min=0.1, q2max=3)
+        self.assert_obs('<S_1cc>(Lambdab->Lambda(1520)mumu)', 0.181, rtol=0.30, q2min=0.1, q2max=3)
         self.assert_obs('<S_1cc>(Lambdab->Lambda(1520)mumu)', 0.242, rtol=0.07, q2min=3, q2max=6)
         self.assert_obs('<S_1cc>(Lambdab->Lambda(1520)mumu)', 0.361, rtol=0.05, q2min=6, q2max=8.68)
         self.assert_obs('<S_1cc>(Lambdab->Lambda(1520)mumu)', 0.221, rtol=0.06, q2min=1, q2max=6)
 
     def test_lambdablambda1520ll_binned_qmff_np(self):
         # compare to NP values in table 1 of 2005.09602 using quark model form factors
         flavio.config['implementation']['Lambdab->Lambda(1520) form factor'] = 'Lambdab->Lambda(1520) MCN'
 
         self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 0.337, NP=True, rtol=0.19, scalef=1e9, q2min=0.1, q2max=3)
         self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 1.04, NP=True, rtol=0.06, scalef=1e9, q2min=3, q2max=6)
         self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 2.58, NP=True, rtol=0.07, scalef=1e9, q2min=6, q2max=8.68)
         self.assert_obs('<dBR/dq2>(Lambdab->Lambda(1520)mumu)', 0.77, NP=True, rtol=0.07, scalef=1e9, q2min=1, q2max=6)
 
-        self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', 0.098  , NP=True, rtol=0.26, q2min=0.1, q2max=3)
-        self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.059, NP=True, rtol=0.38, q2min=3, q2max=6)
+        self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', 0.098  , NP=True, rtol=0.27, q2min=0.1, q2max=3)
+        self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.059, NP=True, rtol=0.39, q2min=3, q2max=6)
         self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.166, NP=True, rtol=0.01, q2min=6, q2max=8.68)
-        self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.031, NP=True, rtol=0.84, q2min=1, q2max=6)
+        self.assert_obs('<AFBl>(Lambdab->Lambda(1520)mumu)', -0.031, NP=True, rtol=0.85, q2min=1, q2max=6)
 
     def test_lambdablambda1520mm_all_observables(self):
         # Test if all the observables with l=mu work fine.
         names = [
             '<dBR/dq2>(Lambdab->Lambda(1520)mumu)',
             '<AFBh>(Lambdab->Lambda(1520)mumu)',
             '<AFBlh>(Lambdab->Lambda(1520)mumu)',
```

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_lambdablambdall.py` & `flavio-2.5.2/flavio/physics/bdecays/test_lambdablambdall.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 wc_sm = flavio.WilsonCoefficients()
 # choose parameters as required to compare numerics to arXiv:1602.01399
 par_nominal = flavio.default_parameters.copy()
 flavio.physics.bdecays.formfactors.lambdab_12.lattice_parameters.lattice_load_nominal(par_nominal)
 par_nominal.set_constraint('Vcb', 0.04175)
+par_nominal.set_constraint('delta', 1.30)
+par_nominal.set_constraint("m_t", 173.21)
 par_nominal.set_constraint('tau_Lambdab', 1/4.49e-13) # PDG 2016 value
 par_nominal.set_constraint('Lambda->ppi alpha_-', 0.642) # PDG 2016 value
 par_dict = par_nominal.get_central_all()
 
 def ass_sm(s, name, q2min, q2max, target, delta, scalef=1):
     obs = flavio.classes.Observable[name]
     c = obs.prediction_central(par_nominal, wc_sm, q2min, q2max)*scalef
```

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_matrixelements.py` & `flavio-2.5.2/flavio/physics/bdecays/test_matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/test_wc.py` & `flavio-2.5.2/flavio/physics/bdecays/test_wc.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/bdecays/wilsoncoefficients.py` & `flavio-2.5.2/flavio/physics/bdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/betadecays/common.py` & `flavio-2.5.2/flavio/physics/betadecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/betadecays/ft.py` & `flavio-2.5.2/flavio/physics/betadecays/ft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/betadecays/test_betadecays.py` & `flavio-2.5.2/flavio/physics/betadecays/test_betadecays.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,22 +37,32 @@
         self.assertEqual(wceff['S'], 0)
         self.assertEqual(wceff['P'], 0)
         self.assertAlmostEqual(wceff['T'], 4 * 1, delta=0.1)
 
     def test_ft(self):
         # compare to exp values in table 4 of 1803.08732
         wc_obj = flavio.WilsonCoefficients()
+
+        # The Vus = sqrt(1-Vud^2) values are found by rescaling the average Vud 
+        # quoted in Hardy&Towner 2020 by the corresponding individual Ft values
+        par["Vus"] = (1 - 0.97319**2)**0.5
         Ft = flavio.physics.betadecays.ft.Ft_superallowed(par, wc_obj, '10C')
-        self.assertAlmostEqual(Ft / s, 3078, delta=2 * 5)
+        self.assertAlmostEqual(Ft / s, 3078, delta=5)
+        
+        par["Vus"] = (1 - 0.97371**2)**0.5
         Ft = flavio.physics.betadecays.ft.Ft_superallowed(par, wc_obj, '26mAl')
-        self.assertAlmostEqual(Ft / s, 3072.9, delta=3 * 1)
+        self.assertAlmostEqual(Ft / s, 3072.9, delta=1)
+        
+        par["Vus"] = (1 - 0.97341**2)**0.5
         Ft = flavio.physics.betadecays.ft.Ft_superallowed(par, wc_obj, '46V')
-        self.assertAlmostEqual(Ft / s, 3074.1, delta=2 * 2)
-        Ft = flavio.sm_prediction('Ft(38Ca)')
-        self.assertAlmostEqual(Ft / s, 3076.4, delta=2 * 7.2)
+        self.assertAlmostEqual(Ft / s, 3074.1, delta=2)
+        
+        par["Vus"] = (1 - 0.97285**2)**0.5
+        Ft = flavio.physics.betadecays.ft.Ft_superallowed(par, wc_obj, '38Ca')
+        self.assertAlmostEqual(Ft / s, 3076.4, delta=7.2)
 
     def test_taun(self):
         # compare to exp value in table 5 of 1803.08732
         tau_n = flavio.sm_prediction('tau_n', me_E=0.655)
         self.assertAlmostEqual(tau_n / s, 879.75, delta=39)
 
     def test_corrn(self):
```

### Comparing `flavio-2.5.1/flavio/physics/ckm.py` & `flavio-2.5.2/flavio/physics/ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/common.py` & `flavio-2.5.2/flavio/physics/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat` & `flavio-2.5.2/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/README` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/README`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat` & `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat` & `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d` & `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat` & `flavio-2.5.2/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json` & `flavio-2.5.2/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml` & `flavio-2.5.2/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz` & `flavio-2.5.2/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy` & `flavio-2.5.2/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/dlnu.py` & `flavio-2.5.2/flavio/physics/ddecays/dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/dplnu.py` & `flavio-2.5.2/flavio/physics/ddecays/dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/formfactors/__init__.py` & `flavio-2.5.2/flavio/physics/ddecays/formfactors/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/formfactors/bcl.py` & `flavio-2.5.2/flavio/physics/ddecays/formfactors/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/formfactors/bsz.py` & `flavio-2.5.2/flavio/physics/ddecays/formfactors/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/formfactors/test_formfactors.py` & `flavio-2.5.2/flavio/physics/ddecays/formfactors/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/test_dlnu.py` & `flavio-2.5.2/flavio/physics/ddecays/test_dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/ddecays/test_dplnu.py` & `flavio-2.5.2/flavio/physics/ddecays/test_dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/dileptons/partondist.py` & `flavio-2.5.2/flavio/physics/dileptons/partondist.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/dileptons/ppll.py` & `flavio-2.5.2/flavio/physics/dileptons/ppll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/dileptons/pplnu.py` & `flavio-2.5.2/flavio/physics/dileptons/pplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/dileptons/test_ppll.py` & `flavio-2.5.2/flavio/physics/dileptons/test_ppll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/dileptons/test_pplnu.py` & `flavio-2.5.2/flavio/physics/dileptons/test_pplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/edms/common.py` & `flavio-2.5.2/flavio/physics/edms/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/edms/neutronedm.py` & `flavio-2.5.2/flavio/physics/edms/neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/edms/paraedm.py` & `flavio-2.5.2/flavio/physics/edms/paraedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/edms/test_neutronedm.py` & `flavio-2.5.2/flavio/physics/edms/test_neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/eft.py` & `flavio-2.5.2/flavio/physics/eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/elements.py` & `flavio-2.5.2/flavio/physics/elements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/higgs/decay.py` & `flavio-2.5.2/flavio/physics/higgs/decay.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/higgs/production.py` & `flavio-2.5.2/flavio/physics/higgs/production.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/higgs/signalstrength.py` & `flavio-2.5.2/flavio/physics/higgs/signalstrength.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/higgs/test_higgs.py` & `flavio-2.5.2/flavio/physics/higgs/test_higgs.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/higgs/width.py` & `flavio-2.5.2/flavio/physics/higgs/width.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/formfactors.py` & `flavio-2.5.2/flavio/physics/kdecays/formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/kll.py` & `flavio-2.5.2/flavio/physics/kdecays/kll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/klnu.py` & `flavio-2.5.2/flavio/physics/kdecays/klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/kpilnu.py` & `flavio-2.5.2/flavio/physics/kdecays/kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/kpinunu.py` & `flavio-2.5.2/flavio/physics/kdecays/kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/kpipi.py` & `flavio-2.5.2/flavio/physics/kdecays/kpipi.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/lambdaplnu.py` & `flavio-2.5.2/flavio/physics/kdecays/lambdaplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/test_formfactors.py` & `flavio-2.5.2/flavio/physics/kdecays/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/test_kll.py` & `flavio-2.5.2/flavio/physics/kdecays/test_kll.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         # compare to hep-ph/0605203
         # correct for different CKM choice
         par06 = par.copy()
         par06.update({'Vus': 0.22715, 'Vub': 0.003683, 'Vcb': 0.04161,
                       'delta': 59.0 / 180 * pi})
         self.assertAlmostEqual(br_kll(par06, wc_obj, 'KL', 'mu', 'mu', ld=False),
                                0.79 * 1e-9,
-                               delta=0.02e-9)
+                               delta=0.027e-9)
 
     def test_ksmm_sd_sm(self):
         # compare to 1707.06999
         # correct for different CKM choice
         my_xi_t = ckm.xi('t', 'sd')(par)
         xi_t = ckm.xi('t', 'sd')({'Vus': 0.22508, 'Vub': 0.003715, 'Vcb': 0.04181,
                                   'delta': 65.4 / 180 * pi})
```

### Comparing `flavio-2.5.1/flavio/physics/kdecays/test_klnu.py` & `flavio-2.5.2/flavio/physics/kdecays/test_klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/test_kpilnu.py` & `flavio-2.5.2/flavio/physics/kdecays/test_kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/test_kpinunu.py` & `flavio-2.5.2/flavio/physics/kdecays/test_kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/kdecays/wilsoncoefficients.py` & `flavio-2.5.2/flavio/physics/kdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mdms/al.py` & `flavio-2.5.2/flavio/physics/mdms/al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mdms/test_al.py` & `flavio-2.5.2/flavio/physics/mdms/test_al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mesonmixing/amplitude.py` & `flavio-2.5.2/flavio/physics/mesonmixing/amplitude.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mesonmixing/common.py` & `flavio-2.5.2/flavio/physics/mesonmixing/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mesonmixing/observables.py` & `flavio-2.5.2/flavio/physics/mesonmixing/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mesonmixing/test_mesonmixing.py` & `flavio-2.5.2/flavio/physics/mesonmixing/test_mesonmixing.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mesonmixing/wilsoncoefficient.py` & `flavio-2.5.2/flavio/physics/mesonmixing/wilsoncoefficient.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mudecays/mu3e.py` & `flavio-2.5.2/flavio/physics/mudecays/mu3e.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mudecays/mueconversion.py` & `flavio-2.5.2/flavio/physics/mudecays/mueconversion.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mudecays/muegamma.py` & `flavio-2.5.2/flavio/physics/mudecays/muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/mudecays/test_muegamma.py` & `flavio-2.5.2/flavio/physics/mudecays/test_muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/neutrinos/test_trident.py` & `flavio-2.5.2/flavio/physics/neutrinos/test_trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/neutrinos/trident.py` & `flavio-2.5.2/flavio/physics/neutrinos/trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/Pll.py` & `flavio-2.5.2/flavio/physics/quarkonium/Pll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/Sll.py` & `flavio-2.5.2/flavio/physics/quarkonium/Sll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/Vll.py` & `flavio-2.5.2/flavio/physics/quarkonium/Vll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/Vllgamma.py` & `flavio-2.5.2/flavio/physics/quarkonium/Vllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/test_Pll.py` & `flavio-2.5.2/flavio/physics/quarkonium/test_Pll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/test_Sll.py` & `flavio-2.5.2/flavio/physics/quarkonium/test_Sll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/test_Vll.py` & `flavio-2.5.2/flavio/physics/quarkonium/test_Vll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/quarkonium/test_Vllgamma.py` & `flavio-2.5.2/flavio/physics/quarkonium/test_Vllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/running/betafunctions.py` & `flavio-2.5.2/flavio/physics/running/betafunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/running/masses.py` & `flavio-2.5.2/flavio/physics/running/masses.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/running/running.py` & `flavio-2.5.2/flavio/physics/running/running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/running/test_running.py` & `flavio-2.5.2/flavio/physics/running/test_running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/scattering/ee_ww.py` & `flavio-2.5.2/flavio/physics/scattering/ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/scattering/test_ee_ww.py` & `flavio-2.5.2/flavio/physics/scattering/test_ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/common.py` & `flavio-2.5.2/flavio/physics/taudecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/tau3l.py` & `flavio-2.5.2/flavio/physics/taudecays/tau3l.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/taulgamma.py` & `flavio-2.5.2/flavio/physics/taudecays/taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/taulnunu.py` & `flavio-2.5.2/flavio/physics/taudecays/taulnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/taupl.py` & `flavio-2.5.2/flavio/physics/taudecays/taupl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/taupnu.py` & `flavio-2.5.2/flavio/physics/taudecays/taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/tauvl.py` & `flavio-2.5.2/flavio/physics/taudecays/tauvl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/test_taulgamma.py` & `flavio-2.5.2/flavio/physics/taudecays/test_taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/taudecays/test_taulnunu.py` & `flavio-2.5.2/flavio/physics/taudecays/test_taulnunu.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,8 +65,8 @@
     def test_taulnunu_np4(self):
         CLSM = -4 *  par['GF'] / sqrt(2)
         w = Wilson({'CVLL_numunueemu': -0.5 * CLSM,
                     'CVLL_nutaunueetau': CLSM},
                     80, 'WET', 'flavio')
         BR1 = flavio.sm_prediction('BR(tau->enunu)')
         BR2 = flavio.np_prediction('BR(tau->enunu)', w)
-        self.assertEqual(BR2 / BR1, 9)
+        self.assertAlmostEqual(BR2 / BR1, 9, delta=2e-15)
```

### Comparing `flavio-2.5.1/flavio/physics/taudecays/test_taupnu.py` & `flavio-2.5.2/flavio/physics/taudecays/test_taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/test_ckm.py` & `flavio-2.5.2/flavio/physics/test_ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/test_common.py` & `flavio-2.5.2/flavio/physics/test_common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/test_eft.py` & `flavio-2.5.2/flavio/physics/test_eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/units.py` & `flavio-2.5.2/flavio/physics/units.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/wdecays/gammaw.py` & `flavio-2.5.2/flavio/physics/wdecays/gammaw.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/wdecays/mw.py` & `flavio-2.5.2/flavio/physics/wdecays/mw.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     r"""Two-loop SM prediction for the $W$ pole mass.
 
     Eq. (6) of arXiv:hep-ph/0311148."""
     flavio.citations.register("Awramik:2003rn")
     dH = log(par['m_h'] / 100)
     dh = (par['m_h'] / 100)**2
     dt = (par['m_t'] / 174.3)**2 - 1
-    dZ = par['m_Z'] / 91.1876 - 1
+    dZ = par['m_Z'] / 91.1875 - 1
     dalpha = 0  # FIXME
     dalphas = par['alpha_s'] / 0.119 - 1
     m0W = 80.3779
     c1 = 0.05427
     c2 = 0.008931
     c3 = 0.0000882
     c4 = 0.000161
```

### Comparing `flavio-2.5.1/flavio/physics/wdecays/test_mW.py` & `flavio-2.5.2/flavio/physics/wdecays/test_mW.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 par = flavio.default_parameters.get_central_all()
 
 
 class TestMW(unittest.TestCase):
     def test_mW_SM(self):
-        self.assertAlmostEqual(mw.mW_SM(par), 80.3779, delta=0.02)
+        self.assertAlmostEqual(mw.mW_SM(par), 80.3551, delta=0.02)
 
     def test_shifts_sm(self):
         C = ZeroDict({})
         self.assertEqual(mw.dmW_SMEFT(par, C), 0)
 
     def test_obs(self):
         w = wilson.Wilson({}, scale=91.1876, eft='SMEFT', basis='Warsaw')
```

### Comparing `flavio-2.5.1/flavio/physics/wdecays/test_wdecays.py` & `flavio-2.5.2/flavio/physics/wdecays/test_wdecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/zdecays/afbz.py` & `flavio-2.5.2/flavio/physics/zdecays/afbz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/zdecays/gammaz.py` & `flavio-2.5.2/flavio/physics/zdecays/gammaz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/zdecays/gammazsm.py` & `flavio-2.5.2/flavio/physics/zdecays/gammazsm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/zdecays/smeftew.py` & `flavio-2.5.2/flavio/physics/zdecays/smeftew.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/physics/zdecays/test_zdecays.py` & `flavio-2.5.2/flavio/physics/zdecays/test_zdecays.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,37 +15,37 @@
         self.assertAlmostEqual(flavio.sm_prediction('GammaZ'),
                                2.4950, delta=0.0015)
         self.assertAlmostEqual(flavio.sm_prediction('GammaZ'),
                                1 / par['tau_Z'], delta=0.0015)
         self.assertAlmostEqual(flavio.sm_prediction('sigma_had') / pb / 1e3,
                                41.488, delta=0.05)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->ee)'),
-                               83.966e-3, delta=0.001e-3)
+                               83.966e-3, delta=0.02e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->mumu)'),
-                               83.966e-3, delta=0.001e-3)
+                               83.966e-3, delta=0.02e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->tautau)'),
-                               83.776e-3, delta=0.001e-3)
+                               83.776e-3, delta=0.02e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->uu)'),
-                               299.936e-3, delta=0.04e-3)
+                               299.936e-3, delta=0.6e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->cc)'),
-                               299.860e-3, delta=0.04e-3)
+                               299.860e-3, delta=0.6e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->dd)'),
-                               382.770e-3, delta=0.04e-3)
+                               382.770e-3, delta=0.4e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->ss)'),
-                               382.770e-3, delta=0.04e-3)
+                               382.770e-3, delta=0.4e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->bb)'),
-                               375.724e-3, delta=0.02e-3)
+                               375.724e-3, delta=0.4e-3)
         self.assertAlmostEqual(flavio.sm_prediction('Gamma(Z->nunu)'),
-                               167.157e-3, delta=0.01e-3)
+                               167.157e-3, delta=0.03e-3)
         self.assertAlmostEqual(flavio.sm_prediction('R_l'),
-                               20750.9e-3, delta=2e-3)
+                               20750.9e-3, delta=30e-3)
         self.assertAlmostEqual(flavio.sm_prediction('R_c'),
-                               172.23e-3, delta=0.01e-3)
+                               172.23e-3, delta=0.09e-3)
         self.assertAlmostEqual(flavio.sm_prediction('R_b'),
-                               215.80e-3, delta=0.01e-3)
+                               215.80e-3, delta=0.06e-3)
         self.assertAlmostEqual(flavio.sm_prediction('R_e'),
                                20.743, delta=0.01)
         self.assertAlmostEqual(flavio.sm_prediction('R_mu'),
                                20.743, delta=0.01)
         self.assertAlmostEqual(flavio.sm_prediction('R_tau'),
                                20.743, delta=0.05)
         self.assertAlmostEqual(flavio.sm_prediction('R_uc'),
```

### Comparing `flavio-2.5.1/flavio/plots/__init__.py` & `flavio-2.5.2/flavio/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/plots/colors.py` & `flavio-2.5.2/flavio/plots/colors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/plots/plotfunctions.py` & `flavio-2.5.2/flavio/plots/plotfunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/plots/test_plotfunctions.py` & `flavio-2.5.2/flavio/plots/test_plotfunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/statistics/functions.py` & `flavio-2.5.2/flavio/statistics/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/statistics/likelihood.py` & `flavio-2.5.2/flavio/statistics/likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/statistics/probability.py` & `flavio-2.5.2/flavio/statistics/probability.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/statistics/test_functions.py` & `flavio-2.5.2/flavio/statistics/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/statistics/test_likelihood.py` & `flavio-2.5.2/flavio/statistics/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/statistics/test_probability.py` & `flavio-2.5.2/flavio/statistics/test_probability.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/test_citations.py` & `flavio-2.5.2/flavio/test_citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/test_classes.py` & `flavio-2.5.2/flavio/test_classes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/test_functions.py` & `flavio-2.5.2/flavio/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/test_measurements.py` & `flavio-2.5.2/flavio/test_measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/test_parameters.py` & `flavio-2.5.2/flavio/test_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/test_parseerrors.py` & `flavio-2.5.2/flavio/test_parseerrors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio/util.py` & `flavio-2.5.2/flavio/util.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/flavio.egg-info/PKG-INFO` & `flavio-2.5.2/flavio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.5.1
+Version: 2.5.2
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
-Metadata-Version: 2.1 Name: flavio Version: 2.5.1 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.2 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
```

### Comparing `flavio-2.5.1/flavio.egg-info/SOURCES.txt` & `flavio-2.5.2/flavio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flavio-2.5.1/setup.py` & `flavio-2.5.2/setup.py`

 * *Files identical despite different names*

