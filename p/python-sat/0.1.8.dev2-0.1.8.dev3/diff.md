# Comparing `tmp/python-sat-0.1.8.dev2.tar.gz` & `tmp/python-sat-0.1.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-0.1.8.dev2.tar", last modified: Sun Mar 19 00:44:01 2023, max compression
+gzip compressed data, was "python-sat-0.1.8.dev3.tar", last modified: Fri Apr 21 08:08:39 2023, max compression
```

## Comparing `python-sat-0.1.8.dev2.tar` & `python-sat-0.1.8.dev3.tar`

### file list

```diff
@@ -1,91 +1,94 @@
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.685909 python-sat-0.1.8.dev2/
--rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) 907548567     1168 2023-03-19 00:44:01.686002 python-sat-0.1.8.dev2/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567    14093 2023-03-05 06:40:46.000000 python-sat-0.1.8.dev2/README.rst
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.658265 python-sat-0.1.8.dev2/cardenc/
--rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev2/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.661380 python-sat-0.1.8.dev2/examples/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev2/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20609 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev2/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev2/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    23950 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    68707 2023-03-19 00:37:27.000000 python-sat-0.1.8.dev2/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.665671 python-sat-0.1.8.dev2/pysat/
--rw-r--r--   0 aign0002 (892519254) 907548567      653 2023-03-19 00:37:43.000000 python-sat-0.1.8.dev2/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) 907548567    90179 2023-01-30 23:39:56.000000 python-sat-0.1.8.dev2/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) 907548567    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev2/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) 907548567   169376 2023-03-05 04:20:33.000000 python-sat-0.1.8.dev2/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.666998 python-sat-0.1.8.dev2/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) 907548567     1168 2023-03-19 00:44:01.000000 python-sat-0.1.8.dev2/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567     1825 2023-03-19 00:44:01.000000 python-sat-0.1.8.dev2/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) 907548567        1 2023-03-19 00:44:01.000000 python-sat-0.1.8.dev2/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       57 2023-03-19 00:44:01.000000 python-sat-0.1.8.dev2/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       23 2023-03-19 00:44:01.000000 python-sat-0.1.8.dev2/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/requirements.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      107 2023-03-19 00:44:01.686280 python-sat-0.1.8.dev2/setup.cfg
--rw-r--r--   0 aign0002 (892519254) 907548567     6328 2023-03-06 01:55:34.000000 python-sat-0.1.8.dev2/setup.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.676075 python-sat-0.1.8.dev2/solvers/
--rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev2/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev2/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.682908 python-sat-0.1.8.dev2/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev2/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    66092 2023-03-06 01:41:40.000000 python-sat-0.1.8.dev2/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev2/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev2/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev2/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    25391 2023-03-06 01:41:50.000000 python-sat-0.1.8.dev2/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) 907548567   214965 2023-03-05 04:21:31.000000 python-sat-0.1.8.dev2/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2023-03-19 00:44:01.685546 python-sat-0.1.8.dev2/tests/
--rw-r--r--   0 aign0002 (892519254) 907548567      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev2/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) 907548567     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev2/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev2/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) 907548567      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev2/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev2/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev2/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.947493 python-sat-0.1.8.dev3/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1109 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      217 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-04-21 08:08:39.947572 python-sat-0.1.8.dev3/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    14137 2023-04-21 08:05:23.000000 python-sat-0.1.8.dev3/README.rst
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.920034 python-sat-0.1.8.dev3/allies/
+-rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-14 00:41:27.000000 python-sat-0.1.8.dev3/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    13494 2023-04-21 08:07:34.000000 python-sat-0.1.8.dev3/allies/approxmc.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.922703 python-sat-0.1.8.dev3/cardenc/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1375 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2468 2023-03-02 05:23:11.000000 python-sat-0.1.8.dev3/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1874 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1303 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4646 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2325 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1008 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      918 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15865 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     4851 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     8355 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5117 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.926142 python-sat-0.1.8.dev3/examples/
+-rw-------   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    17968 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    18986 2023-03-04 22:56:50.000000 python-sat-0.1.8.dev3/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20609 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    21295 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15523 2023-01-20 20:56:31.000000 python-sat-0.1.8.dev3/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    20320 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5724 2023-01-13 10:54:03.000000 python-sat-0.1.8.dev3/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    10563 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    23950 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)    68707 2023-03-19 00:37:27.000000 python-sat-0.1.8.dev3/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2183 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.928663 python-sat-0.1.8.dev3/pysat/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      653 2023-04-21 07:53:10.000000 python-sat-0.1.8.dev3/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     5814 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1340 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    30043 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    90179 2023-01-30 23:39:56.000000 python-sat-0.1.8.dev3/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    15657 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    11968 2023-03-05 06:22:14.000000 python-sat-0.1.8.dev3/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   169376 2023-03-05 04:20:33.000000 python-sat-0.1.8.dev3/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.930112 python-sat-0.1.8.dev3/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1193 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1863 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)        1 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       87 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       23 2023-04-21 08:08:39.000000 python-sat-0.1.8.dev3/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)       39 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      107 2023-04-21 08:08:39.947929 python-sat-0.1.8.dev3/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     6549 2023-04-21 07:47:02.000000 python-sat-0.1.8.dev3/setup.py
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.937919 python-sat-0.1.8.dev3/solvers/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   547031 2023-03-02 05:10:30.000000 python-sat-0.1.8.dev3/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   596433 2023-03-03 10:16:48.000000 python-sat-0.1.8.dev3/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    50813 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82779 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   501731 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82656 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    94949 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    77088 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   179223 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)  1529188 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    43879 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    75209 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.944239 python-sat-0.1.8.dev3/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51588 2023-03-02 05:15:52.000000 python-sat-0.1.8.dev3/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    66092 2023-03-06 01:41:40.000000 python-sat-0.1.8.dev3/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    93207 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    89206 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   117955 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   137342 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    54848 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    90618 2023-01-14 22:24:35.000000 python-sat-0.1.8.dev3/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   114715 2023-01-14 21:29:08.000000 python-sat-0.1.8.dev3/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    82379 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    88893 2023-01-14 22:24:31.000000 python-sat-0.1.8.dev3/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    51757 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    42627 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    60626 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)    25391 2023-03-06 01:41:50.000000 python-sat-0.1.8.dev3/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)   214965 2023-03-05 04:21:31.000000 python-sat-0.1.8.dev3/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) MONASH\Domain Users (907548567)        0 2023-04-21 08:08:39.947104 python-sat-0.1.8.dev3/tests/
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      948 2023-03-05 08:16:22.000000 python-sat-0.1.8.dev3/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      429 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      707 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      998 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     2408 2023-03-05 08:17:09.000000 python-sat-0.1.8.dev3/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      784 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)     1007 2023-03-05 06:31:37.000000 python-sat-0.1.8.dev3/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      866 2023-03-05 08:17:46.000000 python-sat-0.1.8.dev3/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      937 2023-01-13 10:53:42.000000 python-sat-0.1.8.dev3/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) MONASH\Domain Users (907548567)      643 2023-01-14 22:33:39.000000 python-sat-0.1.8.dev3/tests/test_warmstart.py
```

### Comparing `python-sat-0.1.8.dev2/LICENSE.txt` & `python-sat-0.1.8.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/PKG-INFO` & `python-sat-0.1.8.dev3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev2
+Version: 0.1.8.dev3
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
+Provides-Extra: approxmc
 Provides-Extra: pblib
 License-File: LICENSE.txt
 
 
 A Python library providing a simple interface to a number of state-of-art
 Boolean satisfiability (SAT) solvers and a few types of cardinality and
 pseudo-Boolean encodings. The purpose of PySAT is to enable researchers
```

### Comparing `python-sat-0.1.8.dev2/README.rst` & `python-sat-0.1.8.dev3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -269,20 +269,20 @@
 
 Once all the prerequisites are installed, the simplest way to get and start
 using PySAT is to install the latest stable release of the toolkit from `PyPI
 <https://pypi.org/>`__:
 
 ::
 
-    $ pip install python-sat[pblib,aiger]
+    $ pip install python-sat[aiger,approxmc,pblib]
 
-We encourage you to install the *optional* dependencies `pblib` and `aiger`,
-as in the previous command. However, if it cannot be done (e.g. if their
-installation fails), you can install PySAT with the functionality of `aiger`
-and `pblib` disabled:
+We encourage you to install the *optional* dependencies `pblib`, `aiger`, and
+`approxmc`, as in the previous command. However, if it cannot be done (e.g. if
+their installation fails), you can install PySAT with the functionality of
+`aiger`, `approxmc`, and `pblib` disabled:
 
 ::
 
     $ pip install python-sat
 
 Once installed from PyPI, the toolkit at a later stage can be updated in the
 following way:
@@ -290,15 +290,15 @@
 ::
 
     $ pip install -U python-sat
 
 .. note::
 
     For some shells, e.g. *zsh*, you may need to put the package names into
-    single quotes, i.e. use ``pip install 'python-sat[pblib,aiger]'``.
+    single quotes, i.e. use ``pip install 'python-sat[aiger,approxmc,pblib]'``.
 
 Alternatively, one can clone `the repository
 <https://github.com/pysathq/pysat>`__ and execute the following command in the
 local copy:
 
 ::
```

### Comparing `python-sat-0.1.8.dev2/cardenc/bitwise.hh` & `python-sat-0.1.8.dev3/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/card.hh` & `python-sat-0.1.8.dev3/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/clset.hh` & `python-sat-0.1.8.dev3/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/common.hh` & `python-sat-0.1.8.dev3/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/itot.hh` & `python-sat-0.1.8.dev3/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/ladder.hh` & `python-sat-0.1.8.dev3/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/mto.hh` & `python-sat-0.1.8.dev3/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/pairwise.hh` & `python-sat-0.1.8.dev3/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/ptypes.hh` & `python-sat-0.1.8.dev3/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/pycard.cc` & `python-sat-0.1.8.dev3/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/seqcounter.hh` & `python-sat-0.1.8.dev3/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/sortcard.hh` & `python-sat-0.1.8.dev3/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/cardenc/utils.hh` & `python-sat-0.1.8.dev3/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/fm.py` & `python-sat-0.1.8.dev3/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/genhard.py` & `python-sat-0.1.8.dev3/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/hitman.py` & `python-sat-0.1.8.dev3/examples/hitman.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/lbx.py` & `python-sat-0.1.8.dev3/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/lsu.py` & `python-sat-0.1.8.dev3/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/mcsls.py` & `python-sat-0.1.8.dev3/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/models.py` & `python-sat-0.1.8.dev3/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/musx.py` & `python-sat-0.1.8.dev3/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/optux.py` & `python-sat-0.1.8.dev3/examples/optux.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/rc2.py` & `python-sat-0.1.8.dev3/examples/rc2.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/examples/usage.py` & `python-sat-0.1.8.dev3/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/pysat/__init__.py` & `python-sat-0.1.8.dev3/pysat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##  Created on: Mar 4, 2017
 ##      Author: Alexey S. Ignatiev
 ##      E-mail: aignatiev@ciencias.ulisboa.pt
 ##
 
 # current version
 #==============================================================================
-VERSION = (0, 1, 8, "dev", 2)
+VERSION = (0, 1, 8, "dev", 3)
 
 
 # PEP440 Format
 #==============================================================================
 __version__ = "%d.%d.%d.%s%d" % VERSION if len(VERSION) == 5 else \
               "%d.%d.%d" % VERSION
```

### Comparing `python-sat-0.1.8.dev2/pysat/_fileio.py` & `python-sat-0.1.8.dev3/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/pysat/_utils.py` & `python-sat-0.1.8.dev3/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/pysat/card.py` & `python-sat-0.1.8.dev3/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/pysat/formula.py` & `python-sat-0.1.8.dev3/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/pysat/pb.py` & `python-sat-0.1.8.dev3/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/pysat/process.py` & `python-sat-0.1.8.dev3/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/pysat/solvers.py` & `python-sat-0.1.8.dev3/pysat/solvers.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/python_sat.egg-info/PKG-INFO` & `python-sat-0.1.8.dev3/python_sat.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 0.1.8.dev2
+Version: 0.1.8.dev3
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: aiger
+Provides-Extra: approxmc
 Provides-Extra: pblib
 License-File: LICENSE.txt
 
 
 A Python library providing a simple interface to a number of state-of-art
 Boolean satisfiability (SAT) solvers and a few types of cardinality and
 pseudo-Boolean encodings. The purpose of PySAT is to enable researchers
```

### Comparing `python-sat-0.1.8.dev2/python_sat.egg-info/SOURCES.txt` & `python-sat-0.1.8.dev3/python_sat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
+allies/__init__.py
+allies/approxmc.py
 cardenc/bitwise.hh
 cardenc/card.hh
 cardenc/clset.hh
 cardenc/common.hh
 cardenc/itot.hh
 cardenc/ladder.hh
 cardenc/mto.hh
```

### Comparing `python-sat-0.1.8.dev2/setup.py` & `python-sat-0.1.8.dev3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,18 +68,19 @@
 
 # solvers to install
 #==============================================================================
 to_install = ['cadical103', 'cadical153', 'gluecard30', 'gluecard41',
               'glucose30', 'glucose41', 'lingeling', 'maplechrono', 'maplecm',
               'maplesat', 'mergesat3', 'minicard', 'minisat22', 'minisatgh']
 
-# example scripts to install as standalone executables
+# example and allies scripts to install as standalone executables
 #==============================================================================
-scripts = ['fm', 'genhard', 'lbx', 'lsu', 'mcsls', 'models', 'musx', 'optux',
-        'rc2']
+example_scripts = ['fm', 'genhard', 'lbx', 'lsu', 'mcsls', 'models', 'musx',
+                   'optux', 'rc2']
+allies_scripts = ['approxmc']
 
 
 # we need to redefine the build command to
 # be able to download and compile solvers
 #==============================================================================
 class build(distutils.command.build.build):
     """
@@ -166,26 +167,28 @@
     library_dirs=library_dirs
 )
 
 
 # finally, calling standard setuptools.setup() (or distutils.core.setup())
 #==============================================================================
 setup(name='python-sat',
-    packages=['pysat', 'pysat.examples'],
-    package_dir={'pysat.examples': 'examples'},
+    packages=['pysat', 'pysat.examples', 'pysat.allies'],
+    package_dir={'pysat.examples': 'examples', 'pysat.allies': 'allies'},
     version=__version__,
     description='A Python library for prototyping with SAT oracles',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst; charset=UTF-8',
     license='MIT',
     author='Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado',
     author_email='alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com',
     url='https://github.com/pysathq/pysat',
     ext_modules=[pycard_ext, pysolvers_ext],
-    scripts=['examples/{0}.py'.format(s) for s in scripts],
+    scripts=['examples/{0}.py'.format(s) for s in example_scripts] + \
+            ['allies/{0}.py'.format(s) for s in allies_scripts],
     cmdclass={'build': build, 'build_ext': build_ext},
     install_requires=['six'],
     extras_require = {
         'aiger': ['py-aiger-cnf>=2.0.0'],
+        'approxmc': ['pyapproxmc>=4.1.8'],
         'pblib': ['pypblib>=0.0.3']
     }
 )
```

### Comparing `python-sat-0.1.8.dev2/solvers/cadical103.tar.gz` & `python-sat-0.1.8.dev3/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/cadical153.tar.gz` & `python-sat-0.1.8.dev3/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/glucose30.tar.gz` & `python-sat-0.1.8.dev3/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/glucose41.tar.gz` & `python-sat-0.1.8.dev3/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/lingeling.tar.gz` & `python-sat-0.1.8.dev3/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/maplechrono.zip` & `python-sat-0.1.8.dev3/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/maplecm.zip` & `python-sat-0.1.8.dev3/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/maplesat.zip` & `python-sat-0.1.8.dev3/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/mergesat3.tar.gz` & `python-sat-0.1.8.dev3/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/minicard.tar.gz` & `python-sat-0.1.8.dev3/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/minisat22.tar.gz` & `python-sat-0.1.8.dev3/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/minisatgh.zip` & `python-sat-0.1.8.dev3/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/cadical103.patch` & `python-sat-0.1.8.dev3/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/cadical153.patch` & `python-sat-0.1.8.dev3/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/glucose30.patch` & `python-sat-0.1.8.dev3/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/glucose41.patch` & `python-sat-0.1.8.dev3/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/gluecard30.patch` & `python-sat-0.1.8.dev3/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/gluecard41.patch` & `python-sat-0.1.8.dev3/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/lingeling.patch` & `python-sat-0.1.8.dev3/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/maplechrono.patch` & `python-sat-0.1.8.dev3/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/maplecm.patch` & `python-sat-0.1.8.dev3/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/maplesat.patch` & `python-sat-0.1.8.dev3/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/mergesat3.patch` & `python-sat-0.1.8.dev3/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/minicard.patch` & `python-sat-0.1.8.dev3/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/minisat22.patch` & `python-sat-0.1.8.dev3/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/patches/minisatgh.patch` & `python-sat-0.1.8.dev3/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/prepare.py` & `python-sat-0.1.8.dev3/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/solvers/pysolvers.cc` & `python-sat-0.1.8.dev3/solvers/pysolvers.cc`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_accum_stats.py` & `python-sat-0.1.8.dev3/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_atmost1.py` & `python-sat-0.1.8.dev3/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_atmostk.py` & `python-sat-0.1.8.dev3/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_cnfplus.py` & `python-sat-0.1.8.dev3/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_equals1.py` & `python-sat-0.1.8.dev3/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_process.py` & `python-sat-0.1.8.dev3/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_unique_model.py` & `python-sat-0.1.8.dev3/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_unique_mus.py` & `python-sat-0.1.8.dev3/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-0.1.8.dev2/tests/test_warmstart.py` & `python-sat-0.1.8.dev3/tests/test_warmstart.py`

 * *Files identical despite different names*

