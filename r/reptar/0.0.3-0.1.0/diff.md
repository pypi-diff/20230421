# Comparing `tmp/reptar-0.0.3.tar.gz` & `tmp/reptar-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reptar-0.0.3.tar", last modified: Thu Dec  1 02:58:53 2022, max compression
+gzip compressed data, was "reptar-0.1.0.tar", last modified: Fri Apr 21 11:31:37 2023, max compression
```

## Comparing `reptar-0.0.3.tar` & `reptar-0.1.0.tar`

### file list

```diff
@@ -1,65 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.916331 reptar-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2022-12-01 02:58:42.000000 reptar-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       49 2022-12-01 02:58:42.000000 reptar-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7870 2022-12-01 02:58:53.916331 reptar-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2022-12-01 02:58:42.000000 reptar-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.916331 reptar-0.0.3/reptar/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2022-12-01 02:58:53.916331 reptar-0.0.3/reptar/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.912331 reptar-0.0.3/reptar/calculators/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/calculators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20088 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/calculators/drivers.py
--rw-r--r--   0 runner    (1001) docker     (122)    11867 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/calculators/psi4_workers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3451 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/calculators/xtb_workers.py
--rw-r--r--   0 runner    (1001) docker     (122)    13083 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/creating.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.916331 reptar-0.0.3/reptar/definitions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3484 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/base.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/md.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      554 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/molprop.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      531 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/pes.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3579 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/qc.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1518 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/sampling.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      112 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/solv.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      733 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/definitions/xtb.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     8245 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.916331 reptar-0.0.3/reptar/extractors/
--rw-r--r--   0 runner    (1001) docker     (122)      352 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/extractors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7646 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/extractors/ase_extractor.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4181 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/extractors/crest_extractor.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3032 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/extractors/extractor.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    35652 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/extractors/orca_extractor.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    19272 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/extractors/xtb_extractor.py
--rw-r--r--   0 runner    (1001) docker     (122)     2854 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/fragment.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.916331 reptar-0.0.3/reptar/parsers/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/parsers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2798 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/parsers/ase_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4801 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/parsers/crest_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3161 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/parsers/orca_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7401 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/parsers/parser.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5173 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/parsers/xtb_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     4253 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/periodic.py
--rw-r--r--   0 runner    (1001) docker     (122)    23886 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/reptar_file.py
--rw-r--r--   0 runner    (1001) docker     (122)    40791 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/sampling.py
--rw-r--r--   0 runner    (1001) docker     (122)     3354 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/save.py
--rw-r--r--   0 runner    (1001) docker     (122)    16380 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.916331 reptar-0.0.3/reptar/writers/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/writers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2570 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/writers/ase_db.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4672 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/writers/pdb.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4354 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/writers/schnetpack_db.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2651 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/writers/writing_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2215 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/writers/xyz.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3353 2022-12-01 02:58:42.000000 reptar-0.0.3/reptar/writers/xyz_gap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.912331 reptar-0.0.3/reptar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7870 2022-12-01 02:58:53.000000 reptar-0.0.3/reptar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1409 2022-12-01 02:58:53.000000 reptar-0.0.3/reptar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 02:58:53.000000 reptar-0.0.3/reptar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 02:58:53.000000 reptar-0.0.3/reptar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      107 2022-12-01 02:58:53.000000 reptar-0.0.3/reptar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-12-01 02:58:53.000000 reptar-0.0.3/reptar.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 02:58:53.916331 reptar-0.0.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     3194 2022-12-01 02:58:42.000000 reptar-0.0.3/scripts/reptar-write-xyz
--rwxr-xr-x   0 runner    (1001) docker     (122)      802 2022-12-01 02:58:53.916331 reptar-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2022-12-01 02:58:42.000000 reptar-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    81180 2022-12-01 02:58:42.000000 reptar-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.622831 reptar-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-21 11:31:22.000000 reptar-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 11:31:22.000000 reptar-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-21 11:31:37.622831 reptar-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-21 11:31:22.000000 reptar-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.622831 reptar-0.1.0/reptar/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-21 11:31:37.622831 reptar-0.1.0/reptar/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.614831 reptar-0.1.0/reptar/calculators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/calculators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20066 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/calculators/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/calculators/psi4_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/calculators/xtb_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/creating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.618831 reptar-0.1.0/reptar/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/md.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/molprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/pes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/qc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/sampling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/solv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/definitions/xtb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.618831 reptar-0.1.0/reptar/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/extractors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7748 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/extractors/ase_extractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4283 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/extractors/crest_extractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3037 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/extractors/extractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35580 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/extractors/orca_extractor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19374 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/extractors/xtb_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.618831 reptar-0.1.0/reptar/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/parsers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2803 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/parsers/ase_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4806 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/parsers/crest_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/parsers/orca_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7406 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/parsers/parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5178 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/parsers/xtb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29179 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/reptar_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41741 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17443 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.618831 reptar-0.1.0/reptar/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/writers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2575 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/writers/ase_db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4677 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/writers/pdb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4371 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/writers/schnetpack_db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2656 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/writers/writing_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2266 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/writers/xyz.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3467 2023-04-21 11:31:22.000000 reptar-0.1.0/reptar/writers/xyz_gap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.614831 reptar-0.1.0/reptar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-21 11:31:37.000000 reptar-0.1.0/reptar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-21 11:31:37.000000 reptar-0.1.0/reptar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:31:37.000000 reptar-0.1.0/reptar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:31:37.000000 reptar-0.1.0/reptar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 11:31:37.000000 reptar-0.1.0/reptar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 11:31:37.000000 reptar-0.1.0/reptar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.618831 reptar-0.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-21 11:31:22.000000 reptar-0.1.0/scripts/reptar-write-xyz
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-04-21 11:31:37.622831 reptar-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-04-21 11:31:22.000000 reptar-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:31:37.622831 reptar-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18022 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_calculators_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_calculators_xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_creator_ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_creator_crest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_creator_orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_creator_xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_writer_ase_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_writer_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_writer_schnetpack_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_writer_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-21 11:31:22.000000 reptar-0.1.0/tests/test_writer_xyz_gap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-04-21 11:31:22.000000 reptar-0.1.0/versioneer.py
```

### Comparing `reptar-0.0.3/LICENSE` & `reptar-0.1.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022, Alex M. Maldonado
+Copyright (c) 2022-2023, Alex M. Maldonado
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/PKG-INFO` & `reptar-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reptar
-Version: 0.0.3
+Version: 0.1.0
 Summary: A tool for storing and analyzing manuscript-scale computational chemistry data
 Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -55,16 +55,14 @@
     <a href="#installation">Installation</a> •
     <a href="#file-types">File Types</a> •
     <a href="#key-value-pairs">Key-value pairs</a> •
     <a href="#workflow">Workflow</a> •
     <a href="#license">License</a>
 </p>
 
-<p align="center"><b>Disclaimer:</b> reptar is under active development and is not suitable for production.</p>
-
 # Motivation
 
 The computational chemistry community often fails to openly provide raw and/or processed data used to draw their scientific conclusions.
 
 For large projects, frameworks such as [QCArchive](https://qcarchive.molssi.org/), [Materials Project](https://materialsproject.org/), [Pitt Quantum Repository](https://pqr.pitt.edu/), [ioChem-BD](https://www.iochem-bd.org/) and many others provide great storage solutions.
 This approach would not be practical for fluid data pipelines and small-scale projects such as a single manuscript.
 
@@ -86,21 +84,22 @@
 git clone https://github.com/aalexmmaldonado/reptar
 cd reptar
 pip install .
 ```
 
 # File types
 
-Reptar supports three file types with a single interface: exdir, JSON, and npz.
+Reptar supports four file types with a single interface: exdir, zarr, JSON, and npz.
 JSON is a text file for storing key-value pairs with few dimensions (i.e., no large arrays).
 NumPy's npz format is useful for arrays; however, no nesting is possible and loading data often requires postprocessing for 0D arrays (e.g., ``np.array('data')``).
 
 Exdir is a simple, yet powerful open file format that mimics the [HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with metadata and data stored in directories with YAML and npy files instead of a single binary file.
-This provides several advantages such as mixing human-readable YAML and binary NumPy files, being easier for version control, and only loading requested portions of datasets into memory.
 For more detailed information, please read this [*Front. Neuroinform.* article about exdir](https://doi.org/10.3389/fninf.2018.00016).
+[Zarr](https://zarr.dev/) is a similar hierarchical data format for chunked and compressed NumPy-like arrays and JSON attributes.
+Both of these file types provide several advantages such as mixing human-readable and binary files, being easier for version control, and only loading requested portions of arrays into memory.
 
 # Key-value pairs
 
 All data is stored under a ``key``-``value`` pair within the reptar framework.
 The ``key`` tells reptar where the data is stored and is conceptually related to standard file paths (without file extensions).
 Nested data is specified by separating the nested keys with a ``/``.
 For example, ``energy_pot``, ``md_run/geometry``, and ``entity_ids`` are all valid keys.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reptar Version: 0.0.3 Summary: A tool for storing
+Metadata-Version: 2.1 Name: reptar Version: 0.1.0 Summary: A tool for storing
 and analyzing manuscript-scale computational chemistry data Author: Alex M.
 Maldonado Author-email: aalexmmaldonado@gmail.com License: MIT license
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Chemistry Classifier: Topic :: System :: Archiving Requires-
@@ -11,16 +11,14 @@
  *** A tool for storing and analyzing manuscript-scale computational chemistry
                                    data ***
                              *** Documentation ***
  [Build_Status_] [codecov] [GitHub_release_(latest_by_date)] [DOI] [License]
                 [GitHub_repo_size] [Black_style] [Black_style]
 Motivation â¢ Installation â¢ File_Types â¢ Key-value_pairs â¢ Workflow â¢
                                     License
-    Disclaimer: reptar is under active development and is not suitable for
-                                  production.
 # Motivation The computational chemistry community often fails to openly
 provide raw and/or processed data used to draw their scientific conclusions.
 For large projects, frameworks such as [QCArchive](https://
 qcarchive.molssi.org/), [Materials Project](https://materialsproject.org/),
 [Pitt Quantum Repository](https://pqr.pitt.edu/), [ioChem-BD](https://
 www.iochem-bd.org/) and many others provide great storage solutions. This
 approach would not be practical for fluid data pipelines and small-scale
@@ -37,28 +35,30 @@
 and archival on places such as [GitHub](https://github.com/) and [Zenodo]
 (https://zenodo.org/). # Installation You can install reptar from [PyPI](https:
 //pypi.org/project/reptar/) by using `pip install reptar`. Or, the latest
 development version can be installed directly from the [GitHub repository]
 (https://github.com/aalexmmaldonado/reptar) or from [TestPyPI](https://
 test.pypi.org/project/reptar/). ```bash git clone https://github.com/
 aalexmmaldonado/reptar cd reptar pip install . ``` # File types Reptar supports
-three file types with a single interface: exdir, JSON, and npz. JSON is a text
-file for storing key-value pairs with few dimensions (i.e., no large arrays).
-NumPy's npz format is useful for arrays; however, no nesting is possible and
-loading data often requires postprocessing for 0D arrays (e.g., ``np.array
-('data')``). Exdir is a simple, yet powerful open file format that mimics the
-[HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with metadata and data
-stored in directories with YAML and npy files instead of a single binary file.
-This provides several advantages such as mixing human-readable YAML and binary
-NumPy files, being easier for version control, and only loading requested
-portions of datasets into memory. For more detailed information, please read
-this [*Front. Neuroinform.* article about exdir](https://doi.org/10.3389/
-fninf.2018.00016). # Key-value pairs All data is stored under a ``key``-
-``value`` pair within the reptar framework. The ``key`` tells reptar where the
-data is stored and is conceptually related to standard file paths (without file
+four file types with a single interface: exdir, zarr, JSON, and npz. JSON is a
+text file for storing key-value pairs with few dimensions (i.e., no large
+arrays). NumPy's npz format is useful for arrays; however, no nesting is
+possible and loading data often requires postprocessing for 0D arrays (e.g.,
+``np.array('data')``). Exdir is a simple, yet powerful open file format that
+mimics the [HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with
+metadata and data stored in directories with YAML and npy files instead of a
+single binary file. For more detailed information, please read this [*Front.
+Neuroinform.* article about exdir](https://doi.org/10.3389/fninf.2018.00016).
+[Zarr](https://zarr.dev/) is a similar hierarchical data format for chunked and
+compressed NumPy-like arrays and JSON attributes. Both of these file types
+provide several advantages such as mixing human-readable and binary files,
+being easier for version control, and only loading requested portions of arrays
+into memory. # Key-value pairs All data is stored under a ``key``-``value``
+pair within the reptar framework. The ``key`` tells reptar where the data is
+stored and is conceptually related to standard file paths (without file
 extensions). Nested data is specified by separating the nested keys with a ``/
 ``. For example, ``energy_pot``, ``md_run/geometry``, and ``entity_ids`` are
 all valid keys. Note that ``gradients`` and ``/gradients`` would translate to
 the same value (``/`` species the "root" of the file). # Workflow ## Storing
 data We refer to a "reptar file" as any file that can be used with the
 ``reptar.File`` class. Creating a reptar file starts by having a set of data
 files generated from some calculation. Paths to these data files are passed
```

### Comparing `reptar-0.0.3/README.md` & `reptar-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,14 @@
     <a href="#installation">Installation</a> •
     <a href="#file-types">File Types</a> •
     <a href="#key-value-pairs">Key-value pairs</a> •
     <a href="#workflow">Workflow</a> •
     <a href="#license">License</a>
 </p>
 
-<p align="center"><b>Disclaimer:</b> reptar is under active development and is not suitable for production.</p>
-
 # Motivation
 
 The computational chemistry community often fails to openly provide raw and/or processed data used to draw their scientific conclusions.
 
 For large projects, frameworks such as [QCArchive](https://qcarchive.molssi.org/), [Materials Project](https://materialsproject.org/), [Pitt Quantum Repository](https://pqr.pitt.edu/), [ioChem-BD](https://www.iochem-bd.org/) and many others provide great storage solutions.
 This approach would not be practical for fluid data pipelines and small-scale projects such as a single manuscript.
 
@@ -67,21 +65,22 @@
 git clone https://github.com/aalexmmaldonado/reptar
 cd reptar
 pip install .
 ```
 
 # File types
 
-Reptar supports three file types with a single interface: exdir, JSON, and npz.
+Reptar supports four file types with a single interface: exdir, zarr, JSON, and npz.
 JSON is a text file for storing key-value pairs with few dimensions (i.e., no large arrays).
 NumPy's npz format is useful for arrays; however, no nesting is possible and loading data often requires postprocessing for 0D arrays (e.g., ``np.array('data')``).
 
 Exdir is a simple, yet powerful open file format that mimics the [HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with metadata and data stored in directories with YAML and npy files instead of a single binary file.
-This provides several advantages such as mixing human-readable YAML and binary NumPy files, being easier for version control, and only loading requested portions of datasets into memory.
 For more detailed information, please read this [*Front. Neuroinform.* article about exdir](https://doi.org/10.3389/fninf.2018.00016).
+[Zarr](https://zarr.dev/) is a similar hierarchical data format for chunked and compressed NumPy-like arrays and JSON attributes.
+Both of these file types provide several advantages such as mixing human-readable and binary files, being easier for version control, and only loading requested portions of arrays into memory.
 
 # Key-value pairs
 
 All data is stored under a ``key``-``value`` pair within the reptar framework.
 The ``key`` tells reptar where the data is stored and is conceptually related to standard file paths (without file extensions).
 Nested data is specified by separating the nested keys with a ``/``.
 For example, ``energy_pot``, ``md_run/geometry``, and ``entity_ids`` are all valid keys.
```

#### html2text {}

```diff
@@ -2,16 +2,14 @@
  *** A tool for storing and analyzing manuscript-scale computational chemistry
                                    data ***
                              *** Documentation ***
  [Build_Status_] [codecov] [GitHub_release_(latest_by_date)] [DOI] [License]
                 [GitHub_repo_size] [Black_style] [Black_style]
 Motivation â¢ Installation â¢ File_Types â¢ Key-value_pairs â¢ Workflow â¢
                                     License
-    Disclaimer: reptar is under active development and is not suitable for
-                                  production.
 # Motivation The computational chemistry community often fails to openly
 provide raw and/or processed data used to draw their scientific conclusions.
 For large projects, frameworks such as [QCArchive](https://
 qcarchive.molssi.org/), [Materials Project](https://materialsproject.org/),
 [Pitt Quantum Repository](https://pqr.pitt.edu/), [ioChem-BD](https://
 www.iochem-bd.org/) and many others provide great storage solutions. This
 approach would not be practical for fluid data pipelines and small-scale
@@ -28,28 +26,30 @@
 and archival on places such as [GitHub](https://github.com/) and [Zenodo]
 (https://zenodo.org/). # Installation You can install reptar from [PyPI](https:
 //pypi.org/project/reptar/) by using `pip install reptar`. Or, the latest
 development version can be installed directly from the [GitHub repository]
 (https://github.com/aalexmmaldonado/reptar) or from [TestPyPI](https://
 test.pypi.org/project/reptar/). ```bash git clone https://github.com/
 aalexmmaldonado/reptar cd reptar pip install . ``` # File types Reptar supports
-three file types with a single interface: exdir, JSON, and npz. JSON is a text
-file for storing key-value pairs with few dimensions (i.e., no large arrays).
-NumPy's npz format is useful for arrays; however, no nesting is possible and
-loading data often requires postprocessing for 0D arrays (e.g., ``np.array
-('data')``). Exdir is a simple, yet powerful open file format that mimics the
-[HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with metadata and data
-stored in directories with YAML and npy files instead of a single binary file.
-This provides several advantages such as mixing human-readable YAML and binary
-NumPy files, being easier for version control, and only loading requested
-portions of datasets into memory. For more detailed information, please read
-this [*Front. Neuroinform.* article about exdir](https://doi.org/10.3389/
-fninf.2018.00016). # Key-value pairs All data is stored under a ``key``-
-``value`` pair within the reptar framework. The ``key`` tells reptar where the
-data is stored and is conceptually related to standard file paths (without file
+four file types with a single interface: exdir, zarr, JSON, and npz. JSON is a
+text file for storing key-value pairs with few dimensions (i.e., no large
+arrays). NumPy's npz format is useful for arrays; however, no nesting is
+possible and loading data often requires postprocessing for 0D arrays (e.g.,
+``np.array('data')``). Exdir is a simple, yet powerful open file format that
+mimics the [HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with
+metadata and data stored in directories with YAML and npy files instead of a
+single binary file. For more detailed information, please read this [*Front.
+Neuroinform.* article about exdir](https://doi.org/10.3389/fninf.2018.00016).
+[Zarr](https://zarr.dev/) is a similar hierarchical data format for chunked and
+compressed NumPy-like arrays and JSON attributes. Both of these file types
+provide several advantages such as mixing human-readable and binary files,
+being easier for version control, and only loading requested portions of arrays
+into memory. # Key-value pairs All data is stored under a ``key``-``value``
+pair within the reptar framework. The ``key`` tells reptar where the data is
+stored and is conceptually related to standard file paths (without file
 extensions). Nested data is specified by separating the nested keys with a ``/
 ``. For example, ``energy_pot``, ``md_run/geometry``, and ``entity_ids`` are
 all valid keys. Note that ``gradients`` and ``/gradients`` would translate to
 the same value (``/`` species the "root" of the file). # Workflow ## Storing
 data We refer to a "reptar file" as any file that can be used with the
 ``reptar.File`` class. Creating a reptar file starts by having a set of data
 files generated from some calculation. Paths to these data files are passed
```

### Comparing `reptar-0.0.3/reptar/calculators/drivers.py` & `reptar-0.1.0/reptar/calculators/drivers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,17 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import math
 import numpy as np
 from ..utils import chunk_iterable
+from ..logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 try:
     import ray
 except ImportError:
     pass
 
 
@@ -34,501 +36,491 @@
     r"""Supervisor of energy+gradient workers.
 
     Creates and manages ray tasks using specified worker.
     """
 
     def __init__(
         self,
-        Z,
-        R,
-        E,
         worker,
         worker_kwargs,
         use_ray=False,
-        n_cpus=1,
-        n_cpus_worker=1,
+        n_workers=1,
+        n_cpus_per_worker=1,
         chunk_size=50,
         start_slice=None,
         end_slice=None,
         ray_address="auto",
     ):
         r"""
         Parameters
         ----------
-        Z : :obj:`numpy.ndarray`, ndim: ``1``
-            Atomic numbers of the atoms with respect to ``R``. Should have shape
-            ``(i,)`` where ``i`` is the number of atoms in the system.
-        R : :obj:`numpy.ndarray`, ndim: ``3``
-            Cartesian coordinates of all structures in group. Should have shape
-            ``(j, i, 3)`` where ``j`` is the number of structures. Units are in
-            Angstroms.
-        E : :obj:`numpy.ndarray`, ndim: ``1``
-            Total electronic energies of all structures in ``R``. Energies that need
-            to be calculated should have ``NaN`` in the element corresponding
-            to the same index in ``R``. Should have shape ``(j,)``. Units are in
-            Hartrees.
         worker : ``callable``
             The desired worker function to compute energy and gradients. It should
             be the same as any previous calculations. The ``ray.remote`` decorator
             will be applied automatically.
         worker_kwargs : :obj:`tuple`, ndim: ``1``
             The other keyword arguments for the worker function after
             ``R_idxs``, ``Z``, and ``R``.
         use_ray : :obj:`bool`, default: ``False``
             Use ray to parallelize calculations. If ``False``, calculations are
             done serially. ``False`` can be useful when running locally or only
             a few calculations are needed. ``True`` is useful for tons of
             calculations.
-        n_cpus : :obj:`int`, default: ``1``
-            Total number of CPUs we can use for ray tasks.
-        n_cpus_worker : :obj:`int`, default: ``1``
-            Number of CPUs to dedicate to each task.
+        n_workers : :obj:`int`, default: ``1``
+            Number of parallel workers to use if ``use_ray`` is ``True``.
+        n_cpus_per_worker : :obj:`int`, default: ``1``
+            Number of CPU cores to provide each worker.
         chunk_size : :obj:`int`, default: ``50``
             Number of calculations per task to do. This should be enough to make
             the ray task overhead significantly less than calculations.
         start_slice : :obj:`int`, default: ``None``
             Trims ``R`` to start at this index.
         end_slice : :obj:`int`, default: ``None``
             Trims ``R`` to end at this index.
         ray_address : :obj:`str`, default: ``'auto'``
             Ray cluster address to connect to.
         """
-        # Check arrays (obsessively)
-        assert R.ndim == 3
-        assert Z.shape[0] == R.shape[1]
-        assert R.shape[0] == E.shape[0]
-        assert R.shape[2] == 3
-
-        # Storing arrays and other information
-        self.Z = Z
-        self.R = R
-        self.E = E
         self.worker = worker
         self.worker_kwargs = worker_kwargs
         self.start_slice = start_slice
         self.end_slice = end_slice
 
-        self.n_cpus = n_cpus
-        self.n_cpus_worker = n_cpus_worker
+        self.n_workers = n_workers
+        self.n_cpus_per_worker = n_cpus_per_worker
         self.chunk_size = chunk_size
-        self.n_workers = math.floor(n_cpus / n_cpus_worker)
 
         self.use_ray = use_ray
         if use_ray:
             if not ray.is_initialized():
                 ray.init(address=ray_address)
 
-            self.Z = ray.put(Z)
-            self.R = ray.put(R)
-
-    def _idx_todo(self):
+    @staticmethod
+    def _idx_todo(E, start_slice=None, end_slice=None):
         r"""Indices of missing energies (calculations to do).
 
         Determines this by finding all ``NaN`` elements.
 
         Returns
         -------
         :obj:`numpy.ndarray`
             Indices for ``R`` that are missing energie values.
         """
-        E = self.E[self.start_slice : self.end_slice]
+        # pylint: disable-next=invalid-name
+        E = E[start_slice:end_slice]
         idx_todo = np.argwhere(np.isnan(E))[:, 0]
         return idx_todo
 
-    def run(self, saver=None):
+    def run(self, Z, R, E, saver=None):
         r"""Run the calculations.
 
         Parameters
         ----------
+        Z : :obj:`numpy.ndarray`, ndim: ``1``
+            Atomic numbers of the atoms with respect to ``R``. Should have shape
+            ``(i,)`` where ``i`` is the number of atoms in the system.
+        R : :obj:`numpy.ndarray`, ndim: ``3``
+            Cartesian coordinates of all structures in group. Should have shape
+            ``(j, i, 3)`` where ``j`` is the number of structures. Units are in
+            Angstroms.
+        E : :obj:`numpy.ndarray`, ndim: ``1``
+            Total electronic energies of all structures in ``R``. Energies that need
+            to be calculated should have ``NaN`` in the element corresponding
+            to the same index in ``R``. Should have shape ``(j,)``. Units are in
+            Hartrees.
         saver : :obj:`reptar.Saver`, optional
-            Save data after every worker finishes.
+            Save data after every worker finishes. Passes ``E`` into
+            :meth:`~reptar.Saver.save`.
 
         Returns
         -------
         :obj:`numpy.ndarray`
             The total electronic energy array, ``E``, after all computations.
         """
+        # Check arrays (obsessively)
+        assert R.ndim == 3
+        assert Z.shape[0] == R.shape[1]
+        assert R.shape[0] == E.shape[0]
+        assert R.shape[2] == 3
+
         worker = self.worker
-        idxs_todo = self._idx_todo()
+        idxs_todo = self._idx_todo(E, self.start_slice, self.end_slice)
         chunker = chunk_iterable(idxs_todo, self.chunk_size)
 
         if not self.use_ray:
             for idx in idxs_todo:
                 # pylint: disable-next=invalid-name
-                _, E_done = worker([idx], self.Z, self.R, **self.worker_kwargs)
-                self.E[idx] = E_done
+                _, E_done = worker([idx], Z, R, **self.worker_kwargs)
+                print(E_done)
+                E[idx] = E_done
 
                 if saver is not None:
-                    saver.save((self.E))
+                    saver.save(E)
         else:
             worker = ray.remote(worker)
+            Z = ray.put(Z)
+            R = ray.put(R)
+
             # Initialize ray workers
             workers = []
 
             def add_worker(workers, chunker):
                 try:
                     chunk = list(next(chunker))
                     workers.append(
-                        worker.options(num_cpus=self.n_cpus_worker).remote(
-                            chunk, self.Z, self.R, **self.worker_kwargs
+                        worker.options(num_cpus=self.n_cpus_per_worker).remote(
+                            chunk, Z, R, **self.worker_kwargs
                         )
                     )
                 except StopIteration:
                     pass
 
             for _ in range(self.n_workers):
                 add_worker(workers, chunker)
 
             # Start calculations
             while len(workers) != 0:
                 done_id, workers = ray.wait(workers)
 
                 idx_done, E_done = ray.get(done_id)[0]  # pylint: disable=invalid-name
-                self.E[idx_done] = E_done
+                E[idx_done] = E_done
 
                 if saver is not None:
-                    saver.save((self.E))
+                    saver.save(E)
 
                 add_worker(workers, chunker)
 
-        return self.E
+            # Cleanup ray object store
+            del Z
+            del R
+
+        return E
 
 
 class DriverEnGrad:
     r"""Supervisor of energy+gradient workers.
 
     Creates and manages ray tasks using specified worker.
     """
 
     def __init__(
         self,
-        Z,
-        R,
-        E,
-        G,
         worker,
         worker_kwargs,
         use_ray=False,
-        n_cpus=1,
-        n_cpus_worker=1,
+        n_workers=1,
+        n_cpus_per_worker=1,
         chunk_size=50,
         start_slice=None,
         end_slice=None,
         ray_address="auto",
     ):
         r"""
         Parameters
         ----------
-        Z : :obj:`numpy.ndarray`, ndim: ``1``
-            Atomic numbers of the atoms with respect to ``R``. Should have shape
-            ``(i,)`` where ``i`` is the number of atoms in the system.
-        R : :obj:`numpy.ndarray`, ndim: ``3``
-            Cartesian coordinates of all structures in group. Should have shape
-            ``(j, i, 3)`` where ``j`` is the number of structures. Units are in
-            Angstroms.
-        E : :obj:`numpy.ndarray`, ndim: ``1``
-            Total electronic energies of all structures in ``R``. Energies that need
-            to be calculated should have ``NaN`` in the element corresponding
-            to the same index in ``R``. Should have shape ``(j,)``. Units are in
-            Hartrees.
-        G : :obj:`numpy.ndarray`, ndim: ``3``
-            Atomic gradients of all structures in ``R``. Gradients that need to be
-            calculated should have ``NaN`` in the corresponding elements. Should
-            have the same shape as ``R``. Units are in Hartrees/Angstrom.
         worker : ``callable``
             The desired worker function to compute energy and gradients. It should
             be the same as any previous calculations. The ``ray.remote`` decorator
             will be applied automatically.
         worker_kwargs : :obj:`tuple`, ndim: ``1``
             The other keyword arguments for the worker function after
             ``R_idxs``, ``Z``, and ``R``.
         use_ray : :obj:`bool`, default: ``False``
             Use ray to parallelize calculations. If ``False``, calculations are
             done serially. ``False`` can be useful when running locally or only
             a few calculations are needed. ``True`` is useful for tons of
             calculations.
-        n_cpus : :obj:`int`, default: ``1``
-            Total number of CPUs we can use for ray tasks.
-        n_cpus_worker : :obj:`int`, default: ``1``
-            Number of CPUs to dedicate to each task.
+        n_workers : :obj:`int`, default: ``1``
+            Number of parallel workers to use if ``use_ray`` is ``True``.
+        n_cpus_per_worker : :obj:`int`, default: ``1``
+            Number of CPU cores to provide each worker.
         chunk_size : :obj:`int`, default: ``50``
             Number of calculations per task to do. This should be enough to make
             the ray task overhead significantly less than calculations.
         start_slice : :obj:`int`, default: ``None``
             Trims ``R`` to start at this index.
         end_slice : :obj:`int`, default: ``None``
             Trims ``R`` to end at this index.
         ray_address : :obj:`str`, default: ``'auto'``
             Ray cluster address to connect to.
         """
-        # Check arrays (obsessively)
-        assert R.ndim == 3
-        assert Z.shape[0] == R.shape[1]
-        assert Z.shape[0] == G.shape[1]
-        assert R.shape[0] == E.shape[0]
-        assert R.shape[0] == G.shape[0]
-        assert R.shape[2] == 3
-        assert G.shape[2] == 3
-
         # Storing arrays and other information
-        self.Z = Z
-        self.R = R
-        self.E = E
-        self.G = G
         self.worker = worker
         self.worker_kwargs = worker_kwargs
         self.start_slice = start_slice
         self.end_slice = end_slice
 
-        self.n_cpus = n_cpus
-        self.n_cpus_worker = n_cpus_worker
+        self.n_workers = n_workers
+        self.n_cpus_per_worker = n_cpus_per_worker
         self.chunk_size = chunk_size
-        self.n_workers = math.floor(n_cpus / n_cpus_worker)
 
         self.use_ray = use_ray
         if use_ray:
             if not ray.is_initialized():
                 ray.init(address=ray_address)
 
-            self.Z = ray.put(Z)
-            self.R = ray.put(R)
-
-    def _idx_todo(self):
+    @staticmethod
+    def _idx_todo(E, start_slice=None, end_slice=None):
         r"""Indices of missing energies (calculations to do).
 
         Determines this by finding all ``NaN`` elements.
 
         Returns
         -------
         :obj:`numpy.ndarray`
             Indices for ``R`` that are missing energie values.
         """
         # pylint: disable-next=invalid-name
-        E = self.E[self.start_slice : self.end_slice]
+        E = E[start_slice:end_slice]
         idx_todo = np.argwhere(np.isnan(E))[:, 0]
         return idx_todo
 
-    def run(self, saver=None):
+    def run(self, Z, R, E, G, saver=None):
         r"""Run the calculations.
 
         Parameters
         ----------
+        Z : :obj:`numpy.ndarray`, ndim: ``1``
+            Atomic numbers of the atoms with respect to ``R``. Should have shape
+            ``(i,)`` where ``i`` is the number of atoms in the system.
+        R : :obj:`numpy.ndarray`, ndim: ``3``
+            Cartesian coordinates of all structures in group. Should have shape
+            ``(j, i, 3)`` where ``j`` is the number of structures. Units are in
+            Angstroms.
+        E : :obj:`numpy.ndarray`, ndim: ``1``
+            Total electronic energies of all structures in ``R``. Energies that need
+            to be calculated should have ``NaN`` in the element corresponding
+            to the same index in ``R``. Should have shape ``(j,)``. Units are in
+            Hartrees.
+        G : :obj:`numpy.ndarray`, ndim: ``3``
+            Atomic gradients of all structures in ``R``. Gradients that need to be
+            calculated should have ``NaN`` in the corresponding elements. Should
+            have the same shape as ``R``. Units are in Hartrees/Angstrom.
         saver : :obj:`reptar.Saver`, optional
-            Save data after every worker finishes.
+            Save data after every worker finishes. Passes ``E, G`` into
+            :meth:`~reptar.Saver.save`.
 
         Returns
         -------
         :obj:`numpy.ndarray`
             The total electronic energy array, ``E``, after all computations.
         :obj:`numpy.ndarray`
             The atomic gradients array, ``E``, after all computations.
         """
+        # Check arrays (obsessively)
+        assert R.ndim == 3
+        assert Z.shape[0] == R.shape[1]
+        assert Z.shape[0] == G.shape[1]
+        assert R.shape[0] == E.shape[0]
+        assert R.shape[0] == G.shape[0]
+        assert R.shape[2] == 3
+        assert G.shape[2] == 3
+
         worker = self.worker
-        idxs_todo = self._idx_todo()
+        idxs_todo = self._idx_todo(E, self.start_slice, self.end_slice)
         chunker = chunk_iterable(idxs_todo, self.chunk_size)
 
         if not self.use_ray:
             for idx in idxs_todo:
                 # pylint: disable-next=invalid-name
-                _, E_done, G_done = worker([idx], self.Z, self.R, **self.worker_kwargs)
-                self.E[idx] = E_done
-                self.G[idx] = G_done
+                _, E_done, G_done = worker([idx], Z, R, **self.worker_kwargs)
+                E[idx] = E_done
+                G[idx] = G_done
 
                 if saver is not None:
-                    saver.save((self.E, self.G))
+                    saver.save((E, G))
         else:
             worker = ray.remote(worker)
+            Z = ray.put(Z)
+            R = ray.put(R)
+
             # Initialize ray workers
             workers = []
 
             def add_worker(workers, chunker):
                 try:
                     chunk = list(next(chunker))
                     workers.append(
-                        worker.options(num_cpus=self.n_cpus_worker).remote(
-                            chunk, self.Z, self.R, **self.worker_kwargs
+                        worker.options(num_cpus=self.n_cpus_per_worker).remote(
+                            chunk, Z, R, **self.worker_kwargs
                         )
                     )
                 except StopIteration:
                     pass
 
             for _ in range(self.n_workers):
                 add_worker(workers, chunker)
 
             # Start calculations
             while len(workers) != 0:
                 done_id, workers = ray.wait(workers)
 
                 # pylint: disable-next=invalid-name
                 idx_done, E_done, G_done = ray.get(done_id)[0]
-                self.E[idx_done] = E_done
-                self.G[idx_done] = G_done
+                E[idx_done] = E_done
+                G[idx_done] = G_done
 
                 if saver is not None:
-                    saver.save((self.E, self.G))
+                    saver.save(E, G)
 
                 add_worker(workers, chunker)
 
-        return self.E, self.G
+            # Cleanup ray object store
+            del Z
+            del R
+
+        return E, G
 
 
 class DriverOpt:
     r"""Supervisor of optimization workers.
 
     Creates and manages ray tasks using specified worker.
     """
 
     def __init__(
         self,
-        Z,
-        R,
-        R_opt,  # pylint: disable=invalid-name
-        E,
-        G,
         worker,
         worker_kwargs,
         use_ray=False,
-        n_cpus=1,
-        n_cpus_worker=1,
+        n_workers=1,
+        n_cpus_per_worker=1,
         chunk_size=1,
         start_slice=None,
         end_slice=None,
         ray_address="auto",
     ):
         r"""
         Parameters
         ----------
-        Z : :obj:`numpy.ndarray`, ndim: ``1``
-            Atomic numbers of the atoms with respect to ``R``. Should have shape
-            ``(i,)`` where ``i`` is the number of atoms in the system.
-        R : :obj:`numpy.ndarray`, ndim: ``3``
-            Cartesian coordinates of all structures in group. Should have shape
-            ``(j, i, 3)`` where ``j`` is the number of structures. Units are in
-            Angstroms.
-        R_opt : :obj:`numpy.ndarray`, ndim: ``3``
-            Optimized Cartesian coordinates of all structures in group. This
-            is used to identifying which optimizations need to be done.
-        E : :obj:`numpy.ndarray`, ndim: ``1``
-            Total electronic energies of all structures in ``R``. Energies that need
-            to be calculated should have ``NaN`` in the element corresponding
-            to the same index in ``R``. Should have shape ``(j,)``. Units are in
-            Hartrees.
-        G : :obj:`numpy.ndarray`, ndim: ``3``
-            Atomic gradients of all structures in ``R``. Gradients that need to be
-            calculated should have ``NaN`` in the corresponding elements. Should
-            have the same shape as ``R``. Units are in Hartrees/Angstrom.
         worker : ``callable``
             The desired worker function to compute energy and gradients. It should
             be the same as any previous calculations. The ``ray.remote`` decorator
             will be applied automatically.
         worker_kwargs : :obj:`tuple`, ndim: ``1``
             The other keyword arguments for the worker function after
             ``R_idxs``, ``Z``, and ``R``.
         use_ray : :obj:`bool`, default: ``False``
             Use ray to parallelize calculations. If ``False``, calculations are
             done serially. ``False`` can be useful when running locally or only
             a few calculations are needed. ``True`` is useful for tons of
             calculations.
-        n_cpus : :obj:`int`, default: ``1``
-            Total number of CPUs we can use for ray tasks.
-        n_cpus_worker : :obj:`int`, default: ``1``
-            Number of CPUs to dedicate to each task.
+        n_workers : :obj:`int`, default: ``1``
+            Number of parallel workers to use if ``use_ray`` is ``True``.
+        n_cpus_per_worker : :obj:`int`, default: ``1``
+            Number of CPU cores to provide each worker.
         chunk_size : :obj:`int`, default: ``1``
             Number of calculations per task to do. This should be enough to make
             the ray task overhead significantly less than calculations.
         start_slice : :obj:`int`, default: ``None``
             Trims ``R`` to start at this index.
         end_slice : :obj:`int`, default: ``None``
             Trims ``R`` to end at this index.
         ray_address : :obj:`str`, default: ``'auto'``
-            Ray cluster address to connect to.
+            Ray cluster address to connect to. Passes ``opt_conv, R_opt, E, G`` into
+            :meth:`~reptar.Saver.save`.
         """
-        # Check arrays (obsessively)
-        assert R.ndim == 3
-        assert Z.shape[0] == R.shape[1]
-        assert R.shape[2] == 3
-
         # Storing arrays and other information
-        self.Z = Z
-        self.R = R
-        self.R_opt = R_opt  # pylint: disable=invalid-name
-        self.opt_conv = ~np.isnan(self.R_opt[:, 0, 0])
-        self.E = E
-        self.G = G
         self.worker = worker
         self.worker_kwargs = worker_kwargs
         self.start_slice = start_slice
         self.end_slice = end_slice
 
-        self.n_cpus = n_cpus
-        self.n_cpus_worker = n_cpus_worker
+        self.n_workers = n_workers
+        self.n_cpus_per_worker = n_cpus_per_worker
         self.chunk_size = chunk_size
-        self.n_workers = math.floor(n_cpus / n_cpus_worker)
 
         self.use_ray = use_ray
         if use_ray:
             if not ray.is_initialized():
                 ray.init(address=ray_address)
 
-            self.Z = ray.put(Z)
-            self.R = ray.put(R)
-
-    def _idx_todo(self):
+    @staticmethod
+    def _idx_todo(opt_conv, start_slice=None, end_slice=None):
         r"""Indices of NaN geometries (calculations to do).
 
         Returns
         -------
         :obj:`numpy.ndarray`
             Indices for ``R`` that are missing energie values.
         """
-        return np.where(~self.opt_conv[self.start_slice : self.end_slice])[0]
+        return np.where(~opt_conv[start_slice:end_slice])[0]
 
-    def run(self, saver=None):
+    # pylint: disable-next=invalid-name
+    def run(self, Z, R, R_opt, E, G, saver=None):
         r"""Run the calculations.
 
         Parameters
         ----------
+        Z : :obj:`numpy.ndarray`, ndim: ``1``
+            Atomic numbers of the atoms with respect to ``R``. Should have shape
+            ``(i,)`` where ``i`` is the number of atoms in the system.
+        R : :obj:`numpy.ndarray`, ndim: ``3``
+            Cartesian coordinates of all structures in group. Should have shape
+            ``(j, i, 3)`` where ``j`` is the number of structures. Units are in
+            Angstroms.
+        R_opt : :obj:`numpy.ndarray`, ndim: ``3``
+            Optimized Cartesian coordinates of all structures in group. This
+            is used to identifying which optimizations need to be done.
+        E : :obj:`numpy.ndarray`, ndim: ``1``
+            Total electronic energies of all structures in ``R``. Energies that need
+            to be calculated should have ``NaN`` in the element corresponding
+            to the same index in ``R``. Should have shape ``(j,)``. Units are in
+            Hartrees.
+        G : :obj:`numpy.ndarray`, ndim: ``3``
+            Atomic gradients of all structures in ``R``. Gradients that need to be
+            calculated should have ``NaN`` in the corresponding elements. Should
+            have the same shape as ``R``. Units are in Hartrees/Angstrom.
         saver : :obj:`reptar.Saver`, optional
             Save data after every worker finishes.
 
         Returns
         -------
         :obj:`numpy.ndarray`
             The total electronic energy array, ``E``, after all computations.
         :obj:`numpy.ndarray`
             The atomic gradients array, ``E``, after all computations.
         """
+        # Check arrays (obsessively)
+        assert R.ndim == 3
+        assert Z.shape[0] == R.shape[1]
+        assert R.shape[2] == 3
+
+        opt_conv = ~np.isnan(R_opt[:, 0, 0])
+
         worker = self.worker
-        idxs_todo = self._idx_todo()
+        idxs_todo = self._idx_todo(opt_conv, self.start_slice, self.end_slice)
         chunker = chunk_iterable(idxs_todo, self.chunk_size)
 
         if not self.use_ray:
             for idx in idxs_todo:
                 # pylint: disable-next=invalid-name
                 _, opt_conv_done, R_opt_done, E_done, G_done = worker(
-                    [idx], self.Z, self.R, **self.worker_kwargs
+                    [idx], Z, R, **self.worker_kwargs
                 )
-                self.opt_conv[idx] = opt_conv_done
-                self.R_opt[idx] = R_opt_done
-                self.E[idx] = E_done
-                self.G[idx] = G_done
+                opt_conv[idx] = opt_conv_done
+                R_opt[idx] = R_opt_done
+                E[idx] = E_done
+                G[idx] = G_done
 
                 if saver is not None:
-                    saver.save((self.opt_conv, self.R_opt, self.E, self.G))
+                    saver.save(opt_conv, R_opt, E, G)
         else:
             worker = ray.remote(worker)
+            Z = ray.put(Z)
+            R = ray.put(R)
+
             # Initialize ray workers
             workers = []
 
             def add_worker(workers, chunker):
                 try:
                     chunk = list(next(chunker))
                     workers.append(
-                        worker.options(num_cpus=self.n_cpus_worker).remote(
-                            chunk, self.Z, self.R, **self.worker_kwargs
+                        worker.options(num_cpus=self.n_cpus_per_worker).remote(
+                            chunk, Z, R, **self.worker_kwargs
                         )
                     )
                 except StopIteration:
                     pass
 
             for _ in range(self.n_workers):
                 add_worker(workers, chunker)
@@ -537,18 +529,18 @@
             while len(workers) != 0:
                 done_id, workers = ray.wait(workers)
 
                 # pylint: disable-next=invalid-name
                 idxs_done, opt_conv_done, R_opt_done, E_done, G_done = ray.get(done_id)[
                     0
                 ]
-                self.opt_conv[idxs_done] = opt_conv_done
-                self.R_opt[idxs_done] = R_opt_done
-                self.E[idxs_done] = E_done
-                self.G[idxs_done] = G_done
+                opt_conv[idxs_done] = opt_conv_done
+                R_opt[idxs_done] = R_opt_done
+                E[idxs_done] = E_done
+                G[idxs_done] = G_done
 
                 if saver is not None:
-                    saver.save((self.opt_conv, self.R_opt, self.E, self.G))
+                    saver.save(opt_conv, R_opt, E, G)
 
                 add_worker(workers, chunker)
 
-        return self.opt_conv, self.R_opt, self.E, self.G
+        return opt_conv, R_opt, E, G
```

### Comparing `reptar-0.0.3/reptar/calculators/psi4_workers.py` & `reptar-0.1.0/reptar/calculators/psi4_workers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,14 +17,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
+from ..logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 try:
     import psi4
 except ImportError:
     pass
 
 # pylint: disable=invalid-name
@@ -85,15 +88,15 @@
     Here, we set ``fix_com`` and ``fix_orientation`` to ``True`` to avoid this.
     """
     psi4.core.set_num_threads(threads)
     psi4.set_memory(mem)
     if options is not None:
         psi4.set_options(options)
     R = R[idxs]
-    E = np.empty(R.shape)
+    E = np.empty(R.shape[0])
     for i, r in enumerate(R):
         mol = psi4.core.Molecule.from_arrays(
             geom=r,
             elez=Z,
             molecular_charge=charge,
             molecular_multiplicity=mult,
             fix_com=True,
```

### Comparing `reptar-0.0.3/reptar/calculators/xtb_workers.py` & `reptar-0.1.0/reptar/calculators/xtb_workers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,19 +17,24 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import numpy as np
+from ..logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 try:
     from xtb.interface import Calculator, Param
+
+    _HAS_XTB = True
 except ImportError:
-    pass
+    _HAS_XTB = False
 
 
 def xtb_engrad(
     idxs, Z, R, charge=0, mult=1, calc_acc=0.1, max_iterations=300, params=None
 ):
     r"""Ray remote function for computing total electronic energy and atomic
     gradients using xtb.
@@ -66,14 +71,16 @@
     :obj:`numpy.ndarray`
         Total electronic energy of computed structures in the same order as
         ``idxs``. Units of Hartree.
     :obj:`numpy.ndarray`
         Atomic gradients of computed structures in the same order as ``idxs``.
         Units of Hartree/Angstrom.
     """
+    assert _HAS_XTB
+
     n_upair_ele = int(mult - 1)
     R = R[idxs]
     G = np.zeros(R.shape)
     E = np.zeros(R.shape[0])
     if params is None:
         params = Param.GFN2xTB
     for i, r in enumerate(R):
```

### Comparing `reptar-0.0.3/reptar/creating.py` & `reptar-0.1.0/reptar/creating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,18 +25,20 @@
 import ase
 from ase.io.ulm import InvalidULMFileError
 import numpy as np
 from pkg_resources import resource_stream
 import yaml
 from . import _version
 from .reptar_file import File
+from .logger import ReptarLogger
 
 # pylint: disable=no-name-in-module
 from .parsers import ParserORCA, ParserXTB, ParserASE, ParserCREST
 
+log = ReptarLogger(__name__)
 __version__ = _version.get_versions()["version"]
 
 defs_reserved = ["base", "md", "molprop", "pes", "qc", "sampl", "solv", "xtb"]
 
 
 def identify_parser(out_path):
     r"""Identifies the correct parser depending on some trigger.
@@ -249,15 +251,15 @@
         -----
         If both ``geom_path`` and ``traj_path`` are provided, it is assumed that
         ``geom_path`` provides an initial geometry not included in
         ``traj_path``.
         """
         assert hasattr(self, "rfile")
 
-        if self.rfile.ftype == "exdir":
+        if self.rfile.ftype in ("exdir", "zarr"):
             self.rfile.create_group(group_key)
 
         # Parsable calculations using an output file.
         if out_path is not None:
             self.parse_output(
                 out_path,
                 geom_path=geom_path,
```

### Comparing `reptar-0.0.3/reptar/definitions/base.yaml` & `reptar-0.1.0/reptar/definitions/base.yaml`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/reptar/definitions/md.yaml` & `reptar-0.1.0/reptar/definitions/md.yaml`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/reptar/definitions/molprop.yaml` & `reptar-0.1.0/reptar/definitions/molprop.yaml`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/reptar/definitions/pes.yaml` & `reptar-0.1.0/reptar/definitions/pes.yaml`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/reptar/definitions/qc.yaml` & `reptar-0.1.0/reptar/definitions/qc.yaml`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/reptar/definitions/sampling.yaml` & `reptar-0.1.0/reptar/definitions/sampling.yaml`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/reptar/definitions/xtb.yaml` & `reptar-0.1.0/reptar/definitions/xtb.yaml`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/reptar/descriptors.py` & `reptar-0.1.0/reptar/descriptors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,14 +21,17 @@
 # SOFTWARE.
 
 """Implementations of structural descriptors and criteria."""
 
 import itertools
 import numpy as np
 from qcelemental import periodictable as ptable
+from .logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 class Criteria:
     r"""Descriptor criteria for accepting a structure based on a descriptor
     and cutoff.
     """
 
@@ -65,17 +68,17 @@
         r"""Specifies if ``Criteria.desc_kwargs`` has precedence over ``kwargs``
         passed directly into :meth:`~reptar.descriptors.Criteria.accept()`.
 
         If ``False``, then duplicate keys passed into
         :meth:`~reptar.descriptors.Criteria.accept()` are used instead of those
         in ``Criteria.desc_kwargs``.
 
-        **Default:** ``False``
-
         :type: :obj:`bool`
+
+        :default: ``False``
         """
 
     def accept(self, Z, R, **kwargs):
         r"""Determine if we accept the structure.
 
         If duplicate keys are provided in ``kwargs`` and ``self.desc_kwargs``,
         ``kwargs`` passed here have preference.
```

### Comparing `reptar-0.0.3/reptar/extractors/ase_extractor.py` & `reptar-0.1.0/reptar/extractors/ase_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,18 +16,23 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# pylint: disable=line-too-long
+
 from math import sqrt
 import numpy as np
 import qcelemental as qcel
 from .extractor import Extractor
+from ..logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 try:
     from ase.calculators.calculator import PropertyNotImplementedError
 except ImportError:
     pass
```

### Comparing `reptar-0.0.3/reptar/extractors/crest_extractor.py` & `reptar-0.1.0/reptar/extractors/crest_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,16 +16,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# pylint: disable=line-too-long
+
 import numpy as np
 from .extractor import Extractor
+from ..logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 class ExtractorCREST(Extractor):
     r"""CREST extractor"""
     # We always pass the file object into methods here.
     # pylint: disable=unused-argument
```

### Comparing `reptar-0.0.3/reptar/extractors/extractor.py` & `reptar-0.1.0/reptar/extractors/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/extractors/orca_extractor.py` & `reptar-0.1.0/reptar/extractors/orca_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,15 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# pylint: disable=line-too-long
+
 from .extractor import Extractor
+from ..logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 class ExtractorORCA(Extractor):
     r"""ORCA extractor"""
     # We always pass the file object into methods here.
     # pylint: disable=unused-argument
 
@@ -489,23 +494,21 @@
                                  OPEN-SHELL COUPLED CLUSTER ITERATIONS
             ----------------------------------------------------------
         """
         while (
             "ORCA POPULATION ANALYSIS" != line.strip()
             and "*     ORCA property calculations      *" != line.strip()
         ):
-            # pylint: disable=line-too-long
             # Iter       E(tot)           E(Corr)          Delta-E          Residual     Time      <S|S>**1/2
             #  0     -7.469294707     -0.036553055      0.000000000      0.027013328    0.05      0.000000001
             #
             # or
             #
             # Iter       E(tot)           E(Corr)          Delta-E          Residual     Time
             #   0     -2.897443580     -0.035772194      0.000000000      0.027217829    0.00
-            # pylint: enable=line-too-long
             if (
                 line.strip()[:79]
                 == "Iter       E(tot)           E(Corr)          Delta-E          Residual     Time"
             ):
                 # Extracts MP2 energies under the initial line.
                 line = next(f)
                 if "energy_correl_mp2" not in self.parsed_info["outputs"]:
@@ -581,22 +584,20 @@
         .. code-block:: text
 
             ------------
             SCF SETTINGS
             ------------
         """
         while "Total time needed     " not in line.strip():
-            # pylint: disable=line-too-long
             # Hamiltonian:
             #  Ab initio Hamiltonian  Method          .... Hartree-Fock(GTOs)
 
             # General Settings:
             #  Integral files         IntName         .... al.chrg0.mult2-orca.sp.esp-ccsdt.anopvqz.vtightscf.sym-lambda0
             #  Hartree-Fock type      HFTyp           .... UHF
-            # pylint: enable=line-too-long
             if "Ab initio Hamiltonian" == line.strip()[:21]:
                 # We only include the HF type in the keywords.
                 for _ in range(0, 5):
                     line = next(f)
                 hf_type = line.split()[4]
                 self.parsed_info["runtime_info"]["hf_type"] = hf_type
```

### Comparing `reptar-0.0.3/reptar/extractors/xtb_extractor.py` & `reptar-0.1.0/reptar/extractors/xtb_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,15 +16,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+# pylint: disable=line-too-long
+
 from .extractor import Extractor
+from ..logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 class ExtractorXTB(Extractor):
     r"""xTB extractor"""
 
     # We always pass the file object into methods here.
     # pylint: disable=unused-argument
```

### Comparing `reptar-0.0.3/reptar/fragment.py` & `reptar-0.1.0/reptar/fragment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,14 +20,17 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Groups atoms into fragments."""
 
 import numpy as np
 from scipy.spatial.distance import cdist
+from .logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 def pairwise_distance(R, cutoff=1.5, num_frags=None):
     r"""Group atoms together into fragments based on some cutoff distance.
 
     This is not very dependable.
```

### Comparing `reptar-0.0.3/reptar/parsers/ase_parser.py` & `reptar-0.1.0/reptar/parsers/ase_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/parsers/crest_parser.py` & `reptar-0.1.0/reptar/parsers/crest_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/parsers/orca_parser.py` & `reptar-0.1.0/reptar/parsers/orca_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/parsers/parser.py` & `reptar-0.1.0/reptar/parsers/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/parsers/xtb_parser.py` & `reptar-0.1.0/reptar/parsers/xtb_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/periodic.py` & `reptar-0.1.0/reptar/periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,14 +21,17 @@
 # SOFTWARE.
 
 """Periodic boundary conditions."""
 
 from ase.geometry import find_mic
 import numpy as np
 from scipy.spatial.distance import pdist
+from .logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 class Cell:
     r"""Enables :math:`n`-body predictions under periodic boundary conditions.
 
     The minimum-image convention (mic) is used to reformat :math:`n`-body
     structures in a form resembling non-periodic structures.
```

### Comparing `reptar-0.0.3/reptar/reptar_file.py` & `reptar-0.1.0/reptar/reptar_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,15 +21,19 @@
 # SOFTWARE.
 
 import os
 import json
 import exdir
 import numpy as np
 import yaml
+import zarr
 from .utils import combine_dicts, dict_iterator, get_md5, remove_nested_key
+from .logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 class File:
     r"""Create, store, and access data from a variety of formats."""
 
     # pylint: disable=unnecessary-dunder-call
 
@@ -67,14 +71,15 @@
         mode : :obj:`str`, default: ``'r'``
             A file mode string that defines the read/write behavior.
         allow_remove : :obj:`bool`, default: ``False``
             Allow the removal of exdir groups in ``'w'`` operation.
         plugins : :obj:`list`, default: ``None``
             A list of instantiated exdir plugins.
         """
+        log.debug("Opening file from path")
         exists = os.path.exists(file_path)
         _, f_ext = os.path.splitext(file_path)
 
         if f_ext == ".exdir":
             File_ = exdir.File(file_path, mode, allow_remove, plugins)
         elif f_ext == ".json":
             if exists:
@@ -88,14 +93,16 @@
                 # Since everything is stored in arrays, we clean up array data.
                 for k, v in File_.items():
                     if self._is_iter(v):
                         v = self.simplify_iter_data(v, k.split("/")[-1])
                         File_[k] = v
             else:
                 File_ = {}
+        elif f_ext == ".zarr":
+            File_ = zarr.open(file_path, mode)
         else:
             raise TypeError(f"{f_ext} is not supported.")
 
         self.fpath = os.path.abspath(file_path)
         self.ftype = f_ext[1:]
         self.fmode = mode
         self.File_ = File_
@@ -113,20 +120,23 @@
         mode : :obj:`str`, default: ``'r'``
             A file mode string that defines the read/write behavior.
         allow_remove : :obj:`bool`, default: ``False``
             Allow the removal of exdir groups in ``'w'`` operation.
         plugins : :obj:`list`, default: ``None``
             A list of instantiated exdir plugins.
         """
+        log.debug("Opening file from dictionary")
         _, f_ext = os.path.splitext(file_path)
 
         if f_ext == ".exdir":
             self.File_ = exdir.File(file_path, mode, allow_remove, plugins)
         elif f_ext in (".json", ".npz"):
             self.File_ = {}
+        elif f_ext == ".zarr":
+            self.File_ = zarr.open(file_path, mode)
         self.fpath = os.path.abspath(file_path)
         self.ftype = f_ext[1:]
         self.fmode = mode
 
         for item in dict_iterator(group_dict):
             key = "/".join(item[:-1])
             data = item[-1]
@@ -144,16 +154,19 @@
             Key of the desired data.
 
         Returns
         -------
         :obj:`str`
             Cleaned key.
         """
+        log.debug("Cleaning key")
+        log.debug("Original key: %s", key)
         if "//" in key:
             key = key.replace("//", "/")
+        log.debug("Cleaned key: %s", key)
         return key
 
     @staticmethod
     def split_key(key):
         r"""Split the key into a parent and data key.
 
         Parameters
@@ -164,35 +177,37 @@
         Returns
         -------
         :obj:`str`
             Parent key.
         :obj:`str`
             Data key.
         """
+        log.debug("Splitting key")
         if key[0] != "/":
             key = "/" + key
         key_split = key.rsplit("/", 1)
         if key_split[0] == "":
             key_split[0] = "/"
+        log.debug("Parent key: %s", key_split[0])
+        log.debug("Data key: %s", key_split[1])
         return key_split
 
     def _get_from_dict(self, key):
         r"""Get data from dictionary-like file (e.g., json, npz).
 
         Parameters
         ----------
         key : :obj:`str`
             Key of the desired data. Nested keys should be separated by ``/``.
 
         Returns
         -------
         Requested data from a dictionary source.
         """
-        if key == "/":
-            return self.File_
+        log.debug("Getting data from dictionary")
 
         keys = key.split("/")
         if keys[0] == "":
             del keys[0]
 
         data = self.File_[keys[0]]
         for k in keys[1:]:
@@ -213,16 +228,15 @@
         as_memmap : :obj:`bool`, default: ``False``
             Keep NumPy memmap instead of converting to arrays.
 
         Returns
         -------
         Requested data from a exdir source.
         """
-        if key == "/":
-            return self.File_
+        log.debug("Getting data from exdir")
 
         key_parent, key_data = self.split_key(key)
         parent = self.File_[key_parent]
         if key_data in list(parent):
             data = parent[key_data]
             if isinstance(data, exdir.core.dataset.Dataset):
                 if as_memmap:
@@ -235,14 +249,42 @@
                 data = dict(data)
 
         if "data" not in locals():
             raise RuntimeError(f"{key} does not exist")
 
         return data
 
+    def _get_from_zarr(self, key):
+        r"""Get data from zarr file.
+
+        Parameters
+        ----------
+        key : :obj:`str`
+            Key of the desired data. Nested keys should be separated by ``/``.
+
+        Returns
+        -------
+        Requested data from a zarr source.
+        """
+        log.debug("Getting data from zarr")
+
+        # Check if key is attribute
+        key_parent, key_data = self.split_key(key)
+        attr_keys = list(self.File_[key_parent].attrs.keys())
+        if key_data in attr_keys:
+            data = self.File_[key_parent].attrs[key_data]
+        else:
+            # Should be array.
+            try:
+                data = self.File_[key]
+            except KeyError as e:
+                raise RuntimeError(f"{key} does not exist") from e
+
+        return data
+
     def get_keys(self, group_key):
         r"""A list of keys in a group.
 
         Does not include keys of nested groups.
 
         Parameters
         ----------
@@ -290,19 +332,26 @@
         --------
         >>> rfile.get('/prod_1/charge')
         0
         >>> rfile.get('energy_scf')
         -12419.360138637763
         """
         key = self.clean_key(key)
+
+        if key == "/":
+            log.debug("Requested root (i.e., '/'). Returning whole file.")
+            return self.File_
+
         try:
             if self.ftype == "exdir":
                 data = self._get_from_exdir(key, as_memmap=as_memmap)
             elif self.ftype in ("json", "npz"):
                 data = self._get_from_dict(key)
+            elif self.ftype == "zarr":
+                data = self._get_from_zarr(key)
         except RuntimeError as e:
             if "does not exist" in str(e) and missing_is_none:
                 data = None
             else:
                 raise
         return data
 
@@ -346,23 +395,26 @@
         those data.
 
         The following cases -> behaviors are enforced on ``data_keys``.
 
         - Length of iterable is one -> Keep as iterable.
             - ``atomic_numbers``, ``entity_ids``, ``comp_ids``
         """
+        log.debug("Checking if data can be simplified")
         # If data is a list we check the types of data it contains.
         # If all of them are strings, we do not convert to array.
         if not isinstance(data, np.ndarray):
             # If there is only one item in the list we can likely
             # just store it as an attribute. However, we have
             # to be careful when the single item is an array.
             if len(data) == 1:
                 if data_key in ["atomic_numbers", "entity_ids", "comp_ids"]:
+                    log.debug("Key is reserved for arrays")
                     return data
+                log.debug("Returning the single item")
                 data = data[0]
             # If all the items are not all strings then we make
             # the dataset.
             elif not all(isinstance(i, str) for i in data):
                 data_array = np.array(data)
                 # Sometimes we have a list of objects that cannot be easily
                 # converted to numpy data types. Numpy will use an object
@@ -372,18 +424,22 @@
             # At this point only data that contains all strings
             # should be left. We put these as attributes (i.e.,
             # comp_ids)
             else:
                 pass
         # Handling arrays.
         else:
+            log.debug("Data type is array")
             # If only one item we store it as a value.
             if data.shape == (1,):
+                log.debug("Shape is (1, )")
                 if data_key in ["atomic_numbers", "entity_ids", "comp_ids"]:
+                    log.debug("Key is reserved for arrays")
                     return data
+                log.debug("Returning the single item")
                 data = data[0].item()
 
         return data
 
     def _put_to_dict(self, key, data):
         r"""Add data to dictionary-like file.
 
@@ -408,14 +464,15 @@
 
         add_dic = {keys[-1]: data}
         for key in reversed(keys[:-1]):  # pylint: disable=redefined-argument-from-local
             add_dic = {key: add_dic}
 
         self.File_ = combine_dicts(self.File_, add_dic)
 
+    # pylint: disable-next=too-many-branches
     def _put_to_exdir(self, key, data):
         r"""Add data to an exdir group.
 
         Parameters
         ----------
         key : :obj:`str`
             Where to put the data. Can be a nested key.
@@ -430,14 +487,18 @@
         # create_group
         try:
             group = self.get(parent_key)
         except KeyError as e:
             if "No such object:" not in str(e):
                 raise
             group = self.create_group(parent_key)
+        except RuntimeError as e:
+            if " does not exist" not in str(e):
+                raise
+            group = self.create_group(parent_key)
         assert isinstance(group, (exdir.core.exdir_file.File, exdir.core.group.Group))
 
         # Custom handling of parsed data to ensure logical behavior.
         ndarray_to_list_keys = ["dipole_moment", "periodic", "periodic_cell"]
         # pylint: disable-next=no-else-return
         if data_key in ndarray_to_list_keys:
             if isinstance(data, np.ndarray):
@@ -470,14 +531,62 @@
             except RuntimeError:
                 # If data set already exists, exdir will throw a RuntimeError.
                 # We remove this dataset and try again.
                 group.__delitem__(data_key)
                 group.create_dataset(data_key, data=data)
         return None
 
+    def _put_to_zarr(self, key, data):
+        r"""Add data to an zarr group.
+
+        Parameters
+        ----------
+        key : :obj:`str`
+            Where to put the data. Can be a nested key.
+        data : various
+            Data to add to zarr file.
+        """
+        parent_key, data_key = self.split_key(key)
+
+        # Handle nested creation of groups.
+        # Suppose we want to put "/group_1/nested_group/data_key" before group_1 or
+        # nested_group exists. We have to create these groups first.
+        try:
+            log.debug("Getting group: %s", parent_key)
+            group = self.File_[parent_key]
+        except KeyError:
+            log.debug("Group not found")
+            group = self.create_group(parent_key)
+        assert isinstance(group, (zarr.hierarchy.Group))
+
+        # Custom handling of parsed data to ensure logical behavior.
+        if data_key == "wall_potential":
+            group.attrs[data_key] = data
+            return None
+
+        # If data is not array/list or array/list of one dimension and
+        # length we make it an exdir attribute.
+        # We make anything else an exdir dataset.
+        is_iter = self._is_iter(data)
+        if is_iter:
+            data = self.simplify_iter_data(data, data_key)
+            if isinstance(data, np.ndarray):
+                store_as = "array"
+            else:
+                store_as = "attr"
+        # Handles all non iterable data.
+        else:
+            store_as = "attr"
+
+        if store_as == "attr":
+            group.attrs[data_key] = data
+        elif store_as == "array":
+            group[data_key] = data
+        return None
+
     def put(self, key, data, with_md5_update=False):
         r"""Put data to file in a specific location.
 
         Note that there is some data postprocessing using
         :meth:`~reptar.File.simplify_iter_data`.
 
         Parameters
@@ -486,19 +595,22 @@
             Key of the desired data (including parent). Nested keys should be
             separated by ``/``.
         data : ``obj``
             Data to add to file.
         with_md5_update : :obj:`bool`, default: ``False``
             Update MD5 hashes after putting data.
         """
+        log.debug("Putting data with key %s", key)
         key = self.clean_key(key)
         if self.ftype == "exdir":
             self._put_to_exdir(key, data)
         elif self.ftype in ("json", "npz"):
             self._put_to_dict(key, data)
+        elif self.ftype == "zarr":
+            self._put_to_zarr(key, data)
 
         # Update MD5 of group
         if with_md5_update:
             group_key, _ = self.split_key(key)
             self.update_md5(group_key)
 
     def put_all(self, group_key, data, nested=False):
@@ -571,14 +683,47 @@
                 attrs = yaml.safe_load(f)
 
             del attrs[attr_key]
 
             with open(yaml_path, "w", encoding="utf-8") as f:
                 yaml.dump(attrs, f)
 
+    def _remove_zarr(self, key):
+        r"""Delete zarr data under ``key``.
+
+        Parameters
+        ----------
+        key : :obj:`str`
+            Key of the desired data (including parent). Nested keys should be
+            separated by ``/``.
+        """
+        try:
+            # Handles datasets
+            self.File_.__delitem__(key)
+            log.debug("Deleted array key: %s", key)
+        except KeyError:
+            log.debug("Key is not an array. Must be an attribute.")
+
+            # Handles attributes
+            group_key, attr_key = self.split_key(key)
+            if group_key[0] == "/":
+                group_key = group_key[1:]
+            json_path = os.path.join(self.fpath, group_key, ".zattrs")
+            log.debug("Loading attribute file at %s", json_path)
+
+            with open(json_path, "r", encoding="utf-8") as f:
+                attrs = json.load(f)
+
+            del attrs[attr_key]
+
+            json_string = json.dumps(attrs)
+
+            with open(json_path, "w", encoding="utf-8") as f:
+                f.write(json_string)
+
     def remove(self, key, with_md5_update=False):
         r"""Delete data under ``key``.
 
         Parameters
         ----------
         key : :obj:`str`
             Key of the desired data (including parent). Nested keys should be
@@ -588,14 +733,16 @@
         """
         key = self.clean_key(key)
 
         if self.ftype == "exdir":
             self._remove_exdir(key)
         elif self.ftype in ("json", "npz"):
             self._remove_dict(key)
+        elif self.ftype == "zarr":
+            self._remove_zarr(key)
 
         # Update MD5 of group
         if with_md5_update:
             group_key, _ = self.split_key(key)
             self.update_md5(group_key)
 
     def copy(self, source_key, dest_key, with_md5_update=False):
@@ -607,29 +754,33 @@
             Key of the data to copy.
         dest_key : :obj:`str`
             Where to copy the data do.
         """
         self.put(dest_key, self.get(source_key), with_md5_update)
 
     def create_group(self, key):
-        r"""Initialize/create an exdir group with the specified key. This can handle
-        creating nested groups.
+        r"""Initialize/create a group in heigherarcal files with the specified key.
+        This can handle creating nested groups.
 
         Parameters
         ----------
         key : :obj:`str`
             Key of the desired data (including parent). Nested keys should be
             separated by ``/``.
 
         Returns
         -------
         :obj:`exdir.core.Group`
             The newly created group.
         """
-        self.File_.create_group(key)
+        log.debug("Creating %s group with key %s", self.ftype, key)
+        if self.ftype == "exdir":
+            self.File_.create_group(key)
+        elif self.ftype == "zarr":
+            self.File_.create_group(key)
         return self.get(key)
 
     def as_dict(self, group_key):
         r"""Get a group as a dictionary.
 
         Parameters
         ----------
```

### Comparing `reptar-0.0.3/reptar/sampling.py` & `reptar-0.1.0/reptar/sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -18,19 +18,24 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from random import choice, randrange
 import numpy as np
+from qcelemental.molparse.from_arrays import validate_and_fill_geometry
+from qcelemental.exceptions import ValidationError
 from .save import Saver
 from .utils import center_structures as get_center_structures
 from .utils import gen_combs, exists_in_array, chunk_iterable
 from .periodic import Cell
 from . import _version
+from .logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 reptar_version = _version.get_versions()["version"]
 
 try:
     import ray
 except ImportError:
     _HAS_RAY = False
@@ -222,14 +227,15 @@
     E_source,  # pylint: disable=invalid-name
     G_source,  # pylint: disable=invalid-name
     entity_ids_source,
     r_prov_specs_source,
     r_prov_id_source,
     criteria,
     periodic_cell,
+    validate_geometry,
 ):
     r"""Given generated selections will slice and sample structures from source."""
     if not isinstance(selections, np.ndarray):
         selections = np.array(selections)
     assert selections.ndim == 2
 
     n_Z = len(Z)  # pylint: disable=invalid-name
@@ -309,14 +315,22 @@
         if criteria is not None:
             accept_r, _ = criteria.accept(Z, R[i_sel], {"entity_ids": entity_ids_dest})
             # If descriptor is not met, will not include sample.
             if not accept_r:
                 keep_idxs[i_sel] = False
                 continue
 
+        # Validate geometry using qcelemental. If atoms are too close, ValidationError
+        # is thrown. If this happens, we discard the sample.
+        if validate_geometry:
+            try:
+                validate_and_fill_geometry(geom=R[i_sel])
+            except ValidationError:
+                continue
+
         r_prov_specs[i_sel] = r_prov_spec_selection
 
         if E_source is not None:
             E[i_sel] = E_source[sel_source_idx]
         if G_source is not None:
             G[i_sel] = r_from_entities(
                 G_source[sel_source_idx], entity_ids_source, entity_ids_selection
@@ -347,15 +361,15 @@
         criteria=None,
         center_structures=False,
         E_key=None,  # pylint: disable=invalid-name
         G_key=None,  # pylint: disable=invalid-name
         dry_run=False,
         all_init_size=50000,
         use_ray=False,
-        n_workers=2,
+        n_workers=1,
         ray_address="auto",
     ):
         """
         Parameters
         ----------
         source_file : :obj:`reptar.File`
             A loaded reptar File to sample structures from.
@@ -386,16 +400,16 @@
             Number of structures to initialize sampling arrays with when
             ``quantity`` is ``'all'``.
         use_ray : :obj:`bool`, default: ``False``
             **Not implemented yet.**
             Use ray to parallelize sampling. If ``False``, then sampling is
             done serially in batches. ``True`` is useful if tons of sampling
             on the order of thousands is desired.
-        n_workers : :obj:`int`, default: ``2``
-            Number of workers to use for sampling if ``use_ray`` is ``True``.
+        n_workers : :obj:`int`, default: ``1``
+            Number of parallel workers to use if ``use_ray`` is ``True``.
             Each worker will have one core.
         ray_address : :obj:`str`, default: ``'auto'``
             Ray cluster address to connect to.
         """
         self.source_file = source_file
         self.source_key = source_key
         self.dest_file = dest_file
@@ -415,17 +429,28 @@
             if not ray.is_initialized():
                 ray.init(address=ray_address)
 
             # We put criteria in ray object store here.
             self.criteria = ray.put(self.criteria)
 
         self.worker_chunk_size_for_all = 1000
-        r"""Chunk size used when ``quantity`` is ``'all'``.
+        r"""Chunk size used when ``quantity`` is ``"all"``.
+
+        :type: :obj:`int`
+
+        :default: ``1000``
+        """
+        self.validate_geometry = True
+        r"""Validate sampled geometry using part of
+        :obj:`qcelemental.molparse.from_arrays`.
+        If ``ValidationError`` is thrown, we discard the sample.
+
+        :type: :obj:`bool`
 
-        :type: : :obj:`int`
+        :default: ``True``
         """
 
     def _prepare_destination(self):
         r"""Check for existing sampled structures in destinations and prepare."""
         dest_file = self.dest_file
         dest_key = self.dest_key
 
@@ -536,16 +561,16 @@
             except RuntimeError:
                 source_file.update_md5()
                 md5_source = source_file.get(f"{source_key}/md5_structures")
 
             # Create pseudo r_prov_ids_source.
             r_prov_ids_source = {0: md5_source}
 
-        # If is this not a new destination we cannot always reuse the source information.
-        # Need to check for overlap of ids and specifications.
+        # If is this not a new destination we cannot always reuse the source
+        # information. Need to check for overlap of ids and specifications.
         # Just need to shift the new source IDs up by the maximum destination ID.
         if r_prov_ids is not None:
 
             # Check and remove any IDs already in the destination.
             present_ids = tuple(key for key in r_prov_ids.keys())
             present_md5s = tuple(value for value in r_prov_ids.values())
             remove_source_ids = []
@@ -666,15 +691,16 @@
                     Z_other = Z_source[
                         np.argwhere(entity_ids_source == other_entity)[:, 0]
                     ]
                     try:
                         assert np.array_equal(Z_ref, Z_other)
                     except AssertionError as e:
                         raise AssertionError(
-                            f"Atomic numbers do not match for entity_id of {other_entity}"
+                            "Atomic numbers do not match for entity_id "
+                            f"of {other_entity}"
                         ) from e
 
             entity_id += 1
 
         Z_sample = np.array(Z_sample)
 
         # Check that, if the destination already contains atomic_numbers, that
@@ -914,14 +940,15 @@
                     self.E_source,
                     self.G_source,
                     self.entity_ids_source,
                     self.r_prov_specs_source,
                     r_prov_id_source,
                     self.criteria,
                     self.periodic_cell,
+                    self.validate_geometry,
                 )
 
                 (
                     i_start,
                     stop_sampling,
                     R,
                     E,
@@ -987,14 +1014,15 @@
                             self.E_source,
                             self.G_source,
                             self.entity_ids_source,
                             self.r_prov_specs_source,
                             r_prov_id_source,
                             self.criteria,
                             self.periodic_cell,
+                            self.validate_geometry,
                         )
                     )
                 except StopIteration:
                     pass
 
             for _ in range(self.n_workers):
                 add_worker(workers, selection_chunker)
```

### Comparing `reptar-0.0.3/reptar/save.py` & `reptar-0.1.0/reptar/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,14 +17,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .reptar_file import File
+from .logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 class Saver:
     r"""Saves data to File.
 
     Useful for drivers that should save current data periodically. For example,
     when running quantum chemistry calculations or sampling. This uses the
```

### Comparing `reptar-0.0.3/reptar/utils.py` & `reptar-0.1.0/reptar/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -24,15 +24,20 @@
 from functools import reduce
 import operator
 import itertools
 import hashlib
 import os
 import numpy as np
 from qcelemental import periodictable as ptable
+from qcelemental.molparse.from_arrays import validate_and_fill_geometry
+from qcelemental.exceptions import ValidationError
 from .descriptors import get_center_of_mass
+from .logger import ReptarLogger
+
+log = ReptarLogger(__name__)
 
 
 def get_files(path, expression, recursive=True):
     r"""Returns paths to all files in a given directory that matches a provided
     expression in the file name.
 
     Commonly used to find all files of a certain type, e.g., output or xyz
@@ -107,35 +112,35 @@
     -------
     :obj:`list` [:obj:`int`]
         Atomic numbers of atoms within a structure.
     """
     return [ptable.to_atomic_number(symbol) for symbol in atom_list]
 
 
-def parse_xyz(stringfile_path):
-    r"""Parses data from string file.
+def parse_xyz(xyz_path):
+    r"""Parses data from xyz file.
 
-    A string file is data presented as consecutive xyz data. The data could be
+    An xyz file is data presented as consecutive xyz structures. The data could be
     three Cartesian coordinates for each atom, three atomic force vector
     components, or both coordinates and atomic forces in one line (referred to
     as extended xyz).
 
     Parameters
     ----------
-    stringfile_path : :obj:`str`
-        Path to string file.
+    xyz_path : :obj:`str`
+        Path to xyz file.
 
     Returns
     -------
     :obj:`tuple` [:obj:`list`]
         Parsed atoms (as element symbols :obj:`str`), comments, and data as
         :obj:`float` from string file.
     """
     Z, comments, data = [], [], []
-    with open(stringfile_path, "r", encoding="utf-8") as f:
+    with open(xyz_path, "r", encoding="utf-8") as f:
         for _, line in enumerate(f):
             line = line.strip()
             if not line:
                 # Skips blank lines
                 pass
             else:
                 line_split = line.split()
@@ -286,16 +291,17 @@
     -------
     :obj:`numpy.ndarray`
         Centered Cartesian atomic coordinates.
     """
     # Masses of each atom in the same shape of R.
     if R.ndim == 2:
         R = np.array([R])
+    n_atoms = R.shape[1]
 
-    R -= np.repeat(get_center_of_mass(Z, R), R.shape[1]).reshape(R.shape)
+    R -= np.repeat(get_center_of_mass(Z, R), n_atoms, axis=0).reshape(R.shape)
 
     if R.shape[0] == 1:
         R = R[0]
 
     return R
 
 
@@ -539,7 +545,39 @@
     Some code here is from `this Stack Overflow answer
     <https://stackoverflow.com/a/14692747>`__ by
     `Martijn Pieters <https://stackoverflow.com/users/100297/martijn-pieters>`__,
     licensed under `CC BY-SA 4.0 <https://creativecommons.org/licenses/by-sa/4.0/>`__.
     """
     del get_nested_key(dictionary, keys[:-1])[keys[-1]]
     return dictionary
+
+
+def validate_geometry(R, tooclose=0.1):
+    """Checks if any atoms would clash.
+
+    Parameters
+    ----------
+    R : :obj:`numpy.ndarray`, ndim: ``3``
+        Atomic coordinates.
+    too_close : :obj:`float`, default: ``0.1``
+        Threshold for atom distances for validated geometries. All atoms must be at
+        least this far away.
+
+    Returns
+    -------
+    :obj:`int`
+        Number of invalid structures.
+    :obj:`numpy.ndarray`
+        (shape: ``R.shape[0]``) If structures in R are valid.
+    """
+    if R.ndim == 2:
+        R = R[None, ...]
+    is_valid = np.full((R.shape[0],), True, dtype=np.bool)
+    for i in range(R.shape[0]):
+        try:
+            validate_and_fill_geometry(geom=R[i], tooclose=tooclose)
+        except ValidationError:
+            is_valid[i] = False
+
+    n_invalid = (~is_valid).sum()
+
+    return n_invalid, is_valid
```

### Comparing `reptar-0.0.3/reptar/writers/ase_db.py` & `reptar-0.1.0/reptar/writers/ase_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/writers/pdb.py` & `reptar-0.1.0/reptar/writers/pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/writers/schnetpack_db.py` & `reptar-0.1.0/reptar/writers/schnetpack_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -60,18 +60,19 @@
         Atomic forces to add to database in eV/A.
     e_units : :obj:`float`, default: ``1.0``
         Units of energy using ``ase.units``. Essentially the conversion factor
         to eV.
     f_units : :obj:`float`, default: ``1.0``
         Units of forces using ``ase.units``. Essentially the conversion factor
         to eV/A.
-    centering_function : ``callable``, default: schnetpack.data.atoms.get_center_of_mass``
+    centering_function : ``callable``
         A function for centering the ``positions`` when querying the database.
         Defaults to centering the structure according to the center of mass.
-        Set to ``None`` for no centering.
+        Set to ``None`` for no centering. Defaults to
+        ``schnetpack.data.atoms.get_center_of_mass``
 
     Returns
     -------
     ``schnetpack.data.atoms.AtomsData``
         Schnetpack database.
 
     Notes
```

### Comparing `reptar-0.0.3/reptar/writers/writing_utils.py` & `reptar-0.1.0/reptar/writers/writing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `reptar-0.0.3/reptar/writers/xyz.py` & `reptar-0.1.0/reptar/writers/xyz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -36,14 +36,17 @@
         Cartesian coordinates of all structures in the same order as ``Z``.
     comments : :obj:`list`, default: ``None``
         Comment lines for each XYZ structure.
     data_precision : :obj:`int`, default: ``10``
         Number of decimal points for printing array data.
 
     """
+    if R.ndim == 2:
+        R = R[None, ...]
+
     n_atoms = len(Z)
     with open(xyz_path, "w", encoding="utf-8") as f:
         for i, r in enumerate(R):
             f.write(f"{n_atoms}\n")
             if comments is not None:
                 comment = comments[i]
                 if comment[-2:] != "\n":
```

### Comparing `reptar-0.0.3/reptar/writers/xyz_gap.py` & `reptar-0.1.0/reptar/writers/xyz_gap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -50,14 +50,19 @@
         Atomic forces of all structures in ``R`` in units of eV/A.
     lattice_precision : :obj:`int`, default: ``3``
         Number of decimal points to print for lattice dimensions.
     data_precision : :obj:`int`, default: ``10``
         Number of decimal points for printing array data.
 
     """
+    if R.ndim == 2:
+        R = R[None, ...]
+    if F is not None and F.ndim == 2:
+        F = F[None, ...]
+
     lat_str = np.array2string(
         lattice.flatten(),
         formatter={"float_kind": lambda x: f"%.{lattice_precision}f" % x},
     )
     # TODO: is pbc always T T T?
     lat_str = 'pbc="T T T" Lattice="' + lat_str[1:-1] + '"'
```

### Comparing `reptar-0.0.3/reptar.egg-info/PKG-INFO` & `reptar-0.1.0/reptar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reptar
-Version: 0.0.3
+Version: 0.1.0
 Summary: A tool for storing and analyzing manuscript-scale computational chemistry data
 Author: Alex M. Maldonado
 Author-email: aalexmmaldonado@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -55,16 +55,14 @@
     <a href="#installation">Installation</a> •
     <a href="#file-types">File Types</a> •
     <a href="#key-value-pairs">Key-value pairs</a> •
     <a href="#workflow">Workflow</a> •
     <a href="#license">License</a>
 </p>
 
-<p align="center"><b>Disclaimer:</b> reptar is under active development and is not suitable for production.</p>
-
 # Motivation
 
 The computational chemistry community often fails to openly provide raw and/or processed data used to draw their scientific conclusions.
 
 For large projects, frameworks such as [QCArchive](https://qcarchive.molssi.org/), [Materials Project](https://materialsproject.org/), [Pitt Quantum Repository](https://pqr.pitt.edu/), [ioChem-BD](https://www.iochem-bd.org/) and many others provide great storage solutions.
 This approach would not be practical for fluid data pipelines and small-scale projects such as a single manuscript.
 
@@ -86,21 +84,22 @@
 git clone https://github.com/aalexmmaldonado/reptar
 cd reptar
 pip install .
 ```
 
 # File types
 
-Reptar supports three file types with a single interface: exdir, JSON, and npz.
+Reptar supports four file types with a single interface: exdir, zarr, JSON, and npz.
 JSON is a text file for storing key-value pairs with few dimensions (i.e., no large arrays).
 NumPy's npz format is useful for arrays; however, no nesting is possible and loading data often requires postprocessing for 0D arrays (e.g., ``np.array('data')``).
 
 Exdir is a simple, yet powerful open file format that mimics the [HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with metadata and data stored in directories with YAML and npy files instead of a single binary file.
-This provides several advantages such as mixing human-readable YAML and binary NumPy files, being easier for version control, and only loading requested portions of datasets into memory.
 For more detailed information, please read this [*Front. Neuroinform.* article about exdir](https://doi.org/10.3389/fninf.2018.00016).
+[Zarr](https://zarr.dev/) is a similar hierarchical data format for chunked and compressed NumPy-like arrays and JSON attributes.
+Both of these file types provide several advantages such as mixing human-readable and binary files, being easier for version control, and only loading requested portions of arrays into memory.
 
 # Key-value pairs
 
 All data is stored under a ``key``-``value`` pair within the reptar framework.
 The ``key`` tells reptar where the data is stored and is conceptually related to standard file paths (without file extensions).
 Nested data is specified by separating the nested keys with a ``/``.
 For example, ``energy_pot``, ``md_run/geometry``, and ``entity_ids`` are all valid keys.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reptar Version: 0.0.3 Summary: A tool for storing
+Metadata-Version: 2.1 Name: reptar Version: 0.1.0 Summary: A tool for storing
 and analyzing manuscript-scale computational chemistry data Author: Alex M.
 Maldonado Author-email: aalexmmaldonado@gmail.com License: MIT license
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Chemistry Classifier: Topic :: System :: Archiving Requires-
@@ -11,16 +11,14 @@
  *** A tool for storing and analyzing manuscript-scale computational chemistry
                                    data ***
                              *** Documentation ***
  [Build_Status_] [codecov] [GitHub_release_(latest_by_date)] [DOI] [License]
                 [GitHub_repo_size] [Black_style] [Black_style]
 Motivation â¢ Installation â¢ File_Types â¢ Key-value_pairs â¢ Workflow â¢
                                     License
-    Disclaimer: reptar is under active development and is not suitable for
-                                  production.
 # Motivation The computational chemistry community often fails to openly
 provide raw and/or processed data used to draw their scientific conclusions.
 For large projects, frameworks such as [QCArchive](https://
 qcarchive.molssi.org/), [Materials Project](https://materialsproject.org/),
 [Pitt Quantum Repository](https://pqr.pitt.edu/), [ioChem-BD](https://
 www.iochem-bd.org/) and many others provide great storage solutions. This
 approach would not be practical for fluid data pipelines and small-scale
@@ -37,28 +35,30 @@
 and archival on places such as [GitHub](https://github.com/) and [Zenodo]
 (https://zenodo.org/). # Installation You can install reptar from [PyPI](https:
 //pypi.org/project/reptar/) by using `pip install reptar`. Or, the latest
 development version can be installed directly from the [GitHub repository]
 (https://github.com/aalexmmaldonado/reptar) or from [TestPyPI](https://
 test.pypi.org/project/reptar/). ```bash git clone https://github.com/
 aalexmmaldonado/reptar cd reptar pip install . ``` # File types Reptar supports
-three file types with a single interface: exdir, JSON, and npz. JSON is a text
-file for storing key-value pairs with few dimensions (i.e., no large arrays).
-NumPy's npz format is useful for arrays; however, no nesting is possible and
-loading data often requires postprocessing for 0D arrays (e.g., ``np.array
-('data')``). Exdir is a simple, yet powerful open file format that mimics the
-[HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with metadata and data
-stored in directories with YAML and npy files instead of a single binary file.
-This provides several advantages such as mixing human-readable YAML and binary
-NumPy files, being easier for version control, and only loading requested
-portions of datasets into memory. For more detailed information, please read
-this [*Front. Neuroinform.* article about exdir](https://doi.org/10.3389/
-fninf.2018.00016). # Key-value pairs All data is stored under a ``key``-
-``value`` pair within the reptar framework. The ``key`` tells reptar where the
-data is stored and is conceptually related to standard file paths (without file
+four file types with a single interface: exdir, zarr, JSON, and npz. JSON is a
+text file for storing key-value pairs with few dimensions (i.e., no large
+arrays). NumPy's npz format is useful for arrays; however, no nesting is
+possible and loading data often requires postprocessing for 0D arrays (e.g.,
+``np.array('data')``). Exdir is a simple, yet powerful open file format that
+mimics the [HDF5](https://www.hdfgroup.org/solutions/hdf5/) format with
+metadata and data stored in directories with YAML and npy files instead of a
+single binary file. For more detailed information, please read this [*Front.
+Neuroinform.* article about exdir](https://doi.org/10.3389/fninf.2018.00016).
+[Zarr](https://zarr.dev/) is a similar hierarchical data format for chunked and
+compressed NumPy-like arrays and JSON attributes. Both of these file types
+provide several advantages such as mixing human-readable and binary files,
+being easier for version control, and only loading requested portions of arrays
+into memory. # Key-value pairs All data is stored under a ``key``-``value``
+pair within the reptar framework. The ``key`` tells reptar where the data is
+stored and is conceptually related to standard file paths (without file
 extensions). Nested data is specified by separating the nested keys with a ``/
 ``. For example, ``energy_pot``, ``md_run/geometry``, and ``entity_ids`` are
 all valid keys. Note that ``gradients`` and ``/gradients`` would translate to
 the same value (``/`` species the "root" of the file). # Workflow ## Storing
 data We refer to a "reptar file" as any file that can be used with the
 ``reptar.File`` class. Creating a reptar file starts by having a set of data
 files generated from some calculation. Paths to these data files are passed
```

### Comparing `reptar-0.0.3/scripts/reptar-write-xyz` & `reptar-0.1.0/scripts/reptar-write-xyz`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # MIT License
 # 
-# Copyright (c) 2022, Alex M. Maldonado
+# Copyright (c) 2022-2023, Alex M. Maldonado
 # 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,69 +21,83 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import argparse
 
+import numpy as np
 from reptar import __version__ as reptar_version
 from reptar import File
 from reptar.writers import write_xyz
-import numpy as np
 
 def main():
-    
+
     parser = argparse.ArgumentParser(
-        description='Write XYZ file from exdir file.'
+        description='Write XYZ file from a reptar supported file type.'
+    )
+    parser.add_argument(
+        'group_path', type=str, nargs='?',
+        help='Path to group path. This can be to a file or exdir/zarr group.'
     )
     parser.add_argument(
-        'group_key', type=str, nargs='?',
-        help='Path to group key. Will take absolute path and split '
-        'based on `.exdir`.'
+        '--group_key', type=str, nargs='?', default='',
+        help='Manually specify group key for file.'
     )
     parser.add_argument(
         '--comment_key', type=str, nargs='?', default='',
-        help='Label of data to include as xyz comment. If "energy" or "grad" is in '
-        'the key, then we convert to kcal/mol.'
+        help='Label of data to include as xyz comment.'
     )
     parser.add_argument(
         '--save_dir', type=str, nargs='?', default='.',
         help='Directory to save XYZ file.'
     )
 
     args = parser.parse_args()
     print(f'reptar {reptar_version}')
 
     print('Parsing args')
-    abs_path = os.path.abspath(args.group_key)
+    abs_path = os.path.abspath(args.group_path)
+    group_key = args.group_key
     comment_key = args.comment_key
     save_dir = args.save_dir
 
-    idx_split = abs_path.rfind('.exdir') + 6
-    exdir_path, group_key = abs_path[:idx_split], abs_path[idx_split:]
+    if ".exdir" in abs_path:
+        idx_split = abs_path.rfind('.exdir') + 6
+    elif ".zarr" in abs_path:
+        idx_split = abs_path.rfind('.zarr') + 5
+    elif ".json" in abs_path:
+        idx_split = abs_path.rfind('.json') + 5
+    elif ".npz" in abs_path:
+        idx_split = abs_path.rfind('.npz') + 4
+    else:
+        raise ValueError("File type is not recognized.")
+
+    if group_key == '':
+        # Need to find parse group_key
+        file_path, group_key = abs_path[:idx_split], abs_path[idx_split:]
+    else:
+        file_path = abs_path
 
     print('Collecting data')
-    rfile = File(exdir_path, mode='r')
-    Z = rfile.get(f'{group_key}/atomic_numbers')
-    R = rfile.get(f'{group_key}/geometry')
+    rfile = File(file_path, mode='r')
+    Z = rfile.get(os.path.join(group_key, 'atomic_numbers'))
+    R = rfile.get(os.path.join(group_key, 'geometry'))
     if comment_key != '':
-        comments = rfile.get(f'{group_key}/{comment_key}')
+        comments = rfile.get(os.path.join(group_key, comment_key))
     else:
         comments = None
-    
+
     if isinstance(comments, np.ndarray):
         print('Handling comment data')
         if comments.ndim > 1:
             raise ValueError(
                 f'Comments has {comments.ndim} dimensions, but it must be 1.'
             )
-        else:
-            if 'energy' in comment_key or 'grad' in comment_key:
-                hartree2kcalmol = 627.5094737775374055927342256  # Psi4 constant
-                comments *= hartree2kcalmol
-            comments = [str(i) for i in comments]
+
+        comments = [str(i) for i in comments]
     print('Writing XYZ file')
     write_xyz(os.path.join(save_dir, 'data.xyz'), Z, R, comments=comments)
     print('Done!')
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `reptar-0.0.3/setup.cfg` & `reptar-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `reptar-0.0.3/setup.py` & `reptar-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "numpy",
     "exdir>=0.4.2",
     "cclib>=1.7.0",
     "scipy",
     "qcelemental>=0.25.1",
     "pyyaml",
     "ase",
+    "zarr",
 ]
 
 setup_requirements = ["versioneer"]
 
 test_requirements = requirements.append(["pytest", "pytest-order", "pytest-dependency"])
 
 setup(
```

### Comparing `reptar-0.0.3/versioneer.py` & `reptar-0.1.0/versioneer.py`

 * *Files identical despite different names*

