# Comparing `tmp/daedalus-5g-0.8.0.tar.gz` & `tmp/daedalus-5g-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daedalus-5g-0.8.0.tar", last modified: Thu Sep  2 15:27:38 2021, max compression
+gzip compressed data, was "daedalus-5g-0.9.0.tar", last modified: Thu Nov  4 02:26:59 2021, max compression
```

## Comparing `daedalus-5g-0.8.0.tar` & `daedalus-5g-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/SDR/
--rw-r--r--   0 runner    (1001) docker     (121)      930 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/SDR/bladerf.yml
--rw-r--r--   0 runner    (1001) docker     (121)      931 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/SDR/ettus.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/SDR/limesdr.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/SIMULATED/
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/SIMULATED/srsran-enb.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2999 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/SIMULATED/srsran-ue.yml
--rw-r--r--   0 runner    (1001) docker     (121)      689 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/SIMULATED/ueransim-gnb.yml
--rw-r--r--   0 runner    (1001) docker     (121)      553 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/SIMULATED/ueransim-ue.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/UERANSIM/
--rw-r--r--   0 runner    (1001) docker     (121)      526 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/UERANSIM/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/UERANSIM/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      203 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/UERANSIM/scripts/add_default_route.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      165 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/UERANSIM/scripts/run_rfn_gnb.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       75 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/UERANSIM/scripts/run_ue.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/configs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/configs/UERANSIM/
--rw-r--r--   0 runner    (1001) docker     (121)      726 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/UERANSIM/gnb.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/UERANSIM/ue.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/configs/faucet/
--rw-r--r--   0 runner    (1001) docker     (121)     4881 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/faucet/acls.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/faucet/faucet.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16464 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/imsis.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/configs/open5gs/
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/open5gs/smf.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     5315 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/slice.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/configs/srsRAN/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/blade-rr.conf
--rw-r--r--   0 runner    (1001) docker     (121)      911 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/drb.conf
--rw-r--r--   0 runner    (1001) docker     (121)    11306 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/enb.conf
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/ettus-rr.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/
--rw-r--r--   0 runner    (1001) docker     (121)      911 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/drb.conf
--rw-r--r--   0 runner    (1001) docker     (121)    10252 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/enb.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/rr.conf
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/sib.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/rr.conf
--rw-r--r--   0 runner    (1001) docker     (121)     3692 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/sib.conf
--rw-r--r--   0 runner    (1001) docker     (121)    14006 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/ue.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/configs/srsRAN/virtual-rr.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.363210 daedalus-5g-0.8.0/5G/core/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/core/.env
--rw-r--r--   0 runner    (1001) docker     (121)     4034 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/core/core.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/core/db.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/core/epc.yml
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/core/ui.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/core/upn.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/5G/daedalus/
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/daedalus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/daedalus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29249 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/daedalus/daedalus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3055 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/daedalus/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/5G/open5gs/
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/open5gs/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/5G/open5gs/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1050 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/open5gs/scripts/nrfhc.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      674 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/open5gs/scripts/run_db.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      173 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/open5gs/scripts/run_smf.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      804 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/open5gs/scripts/run_upf.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/5G/srsRAN/
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/srsRAN/Dockerfile.base
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/srsRAN/Dockerfile.srs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/5G/srsRAN/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      203 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/srsRAN/scripts/add_default_route.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      149 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/srsRAN/scripts/run_rfn_enb.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       59 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/5G/srsRAN/scripts/start_srsue.sh
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     7186 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)      485 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      937 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/daedalus_5g.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      485 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-09-02 15:27:38.000000 daedalus-5g-0.8.0/daedalus_5g.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      546 2021-09-02 15:27:38.367210 daedalus-5g-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-09-02 15:27:27.000000 daedalus-5g-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/SDR/
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/SDR/bladerf.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/SDR/ettus.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/SDR/limesdr.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/SIMULATED/
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/SIMULATED/srsran-enb.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2999 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/SIMULATED/srsran-ue.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      689 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/SIMULATED/ueransim-gnb.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/SIMULATED/ueransim-ue.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/UERANSIM/
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/UERANSIM/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/UERANSIM/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      203 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/UERANSIM/scripts/add_default_route.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      165 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/UERANSIM/scripts/run_rfn_gnb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)       75 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/UERANSIM/scripts/run_ue.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/configs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/configs/UERANSIM/
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/UERANSIM/gnb.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/UERANSIM/ue.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/configs/faucet/
+-rw-r--r--   0 runner    (1001) docker     (121)     4881 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/faucet/acls.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/faucet/faucet.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16464 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/imsis.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/configs/open5gs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/open5gs/smf.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     5315 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/slice.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/configs/srsRAN/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/blade-rr.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/drb.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    11305 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/enb.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/ettus-rr.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.132865 daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/drb.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    10251 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/enb.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/rr.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/sib.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/rr.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     3767 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/sib.conf
+-rw-r--r--   0 runner    (1001) docker     (121)    14006 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/ue.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1241 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/configs/srsRAN/virtual-rr.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/5G/core/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/core/.env
+-rw-r--r--   0 runner    (1001) docker     (121)     4034 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/core/core.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1456 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/core/db.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2837 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/core/epc.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/core/ui.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/core/upn.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/5G/daedalus/
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/daedalus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/daedalus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29241 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/daedalus/daedalus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3055 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/daedalus/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/5G/open5gs/
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/open5gs/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/5G/open5gs/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)       93 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/open5gs/scripts/mmehc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1050 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/open5gs/scripts/nrfhc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      674 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/open5gs/scripts/run_db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      173 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/open5gs/scripts/run_smf.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      804 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/open5gs/scripts/run_upf.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/5G/srsRAN/
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/srsRAN/Dockerfile.base
+-rw-r--r--   0 runner    (1001) docker     (121)      381 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/srsRAN/Dockerfile.srs
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/5G/srsRAN/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      203 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/srsRAN/scripts/add_default_route.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)      149 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/srsRAN/scripts/run_rfn_enb.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)       59 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/5G/srsRAN/scripts/start_srsue.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     8227 2021-11-04 02:26:58.000000 daedalus-5g-0.9.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      937 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/daedalus_5g.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      485 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1690 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-04 02:26:59.000000 daedalus-5g-0.9.0/daedalus_5g.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2021-11-04 02:26:59.136865 daedalus-5g-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-11-04 02:26:48.000000 daedalus-5g-0.9.0/setup.py
```

### Comparing `daedalus-5g-0.8.0/5G/SDR/bladerf.yml` & `daedalus-5g-0.9.0/5G/SDR/bladerf.yml`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 
 networks:
   ran:
     external:
       name: ran
 services:
   bladerf-enb:
-    image: iqtlabs/srsran:v0.8.0
+    image: iqtlabs/srsran:v0.9.0
     container_name: bladerf-enb
+    depends_on:
+      mme:
+        condition: service_healthy
     cap_add:
       - SYS_NICE
     networks:
       ran:
         ipv4_address: 192.168.29.61
     volumes:
       - "../configs/srsRAN:/config:z"
```

### Comparing `daedalus-5g-0.8.0/5G/SDR/ettus.yml` & `daedalus-5g-0.9.0/5G/SDR/ettus.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 
 networks:
   ran:
     external:
       name: ran
 services:
   ettus-enb:
-    image: iqtlabs/srsran:v0.8.0
+    image: iqtlabs/srsran:v0.9.0
     container_name: ettus-enb
+    depends_on:
+      mme:
+        condition: service_healthy
     cap_add:
       - SYS_NICE
       - SYS_RAWIO
     networks:
       ran:
         ipv4_address: 192.168.29.62
     volumes:
```

### Comparing `daedalus-5g-0.8.0/5G/SDR/limesdr.yml` & `daedalus-5g-0.9.0/5G/SDR/limesdr.yml`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 
 networks:
   ran:
     external:
       name: ran
 services:
   limesdr-enb:
-    image: iqtlabs/srsran-lime:v0.8.0
+    image: iqtlabs/srsran-lime:latest
     container_name: limesdr-enb
+    depends_on:
+      mme:
+        condition: service_healthy
     cap_add:
       - SYS_NICE
       - SYS_RAWIO
     networks:
       ran:
         ipv4_address: 192.168.29.63
     volumes:
```

### Comparing `daedalus-5g-0.8.0/5G/SIMULATED/srsran-enb.yml` & `daedalus-5g-0.9.0/5G/SIMULATED/srsran-enb.yml`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     external:
       name: ran
   rfn:
     external:
       name: rfn
 services:
   enb:
-    image: iqtlabs/srsran:v0.8.0
+    image: iqtlabs/srsran:v0.9.0
     container_name: enb
     depends_on:
       mme:
-        condition: service_started
+        condition: service_healthy
     cap_add:
       - SYS_NICE
     networks:
       rfn:
         ipv4_address: 192.168.28.60
       ran:
         ipv4_address: 192.168.29.60
```

### Comparing `daedalus-5g-0.8.0/5G/SIMULATED/srsran-ue.yml` & `daedalus-5g-0.9.0/5G/SIMULATED/srsran-ue.yml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 networks:
   rfn:
     external:
       name: rfn
 
 services:
   ue:
-    image: iqtlabs/srsran:v0.8.0
+    image: iqtlabs/srsran:v0.9.0
     container_name: ue
     cap_add:
       - NET_ADMIN
       - SYS_NICE
     devices:
       - /dev/net/tun
     networks:
@@ -31,15 +31,15 @@
       - --usim.imsi=001010000000001
       - --usim.k=c8eba87c1074edd06885cb0486718341
       - --usim.algo=milenage
       - --usim.opc=17b6c0157895bcaa1efc1cef55033f5f
       - --nas.apn=internet
       - --rf.device_args="tx_port=tcp://*:5554,rx_port=tcp://192.168.28.60:5555,id=ue,base_srate=1.92e6"
   ue2:
-    image: iqtlabs/srsran:v0.8.0
+    image: iqtlabs/srsran:v0.9.0
     container_name: ue2
     cap_add:
       - NET_ADMIN
       - SYS_NICE
     devices:
       - /dev/net/tun
     networks:
@@ -58,15 +58,15 @@
       - --usim.imsi=001010000000002
       - --usim.k=c8eba87c1074edd06885cb0486718341
       - --usim.algo=milenage
       - --usim.opc=17b6c0157895bcaa1efc1cef55033f5f
       - --nas.apn=internet2
       - --rf.device_args="tx_port=tcp://*:5564,rx_port=tcp://192.168.28.60:5565,id=ue2,base_srate=1.92e6"
   ue3:
-    image: iqtlabs/srsran:v0.8.0
+    image: iqtlabs/srsran:v0.9.0
     container_name: ue3
     cap_add:
       - NET_ADMIN
       - SYS_NICE
     devices:
       - /dev/net/tun
     networks:
@@ -85,15 +85,15 @@
       - --usim.imsi=001010000000003
       - --usim.k=c8eba87c1074edd06885cb0486718341
       - --usim.algo=milenage
       - --usim.opc=17b6c0157895bcaa1efc1cef55033f5f
       - --nas.apn=internet
       - --rf.device_args="tx_port=tcp://*:5574,rx_port=tcp://192.168.28.60:5575,id=ue3,base_srate=1.92e6"
   ue4:
-    image: iqtlabs/srsran:v0.8.0
+    image: iqtlabs/srsran:v0.9.0
     container_name: ue4
     cap_add:
       - NET_ADMIN
       - SYS_NICE
     devices:
       - /dev/net/tun
     networks:
```

### Comparing `daedalus-5g-0.8.0/5G/SIMULATED/ueransim-gnb.yml` & `daedalus-5g-0.9.0/5G/SIMULATED/ueransim-gnb.yml`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     external:
       name: rfn
   ran:
     external:
       name: ran
 services:
   gnb:
-    image: iqtlabs/ueransim:v0.8.0
+    image: iqtlabs/ueransim:latest
     container_name: gnb
     depends_on:
       nrf:
         condition: service_healthy
       mme:
-        condition: service_started
+        condition: service_healthy
     cap_add:
       - SYS_NICE
       - NET_ADMIN
     networks:
       ran:
         ipv4_address: 192.168.29.65
       rfn:
```

### Comparing `daedalus-5g-0.8.0/5G/SIMULATED/ueransim-ue.yml` & `daedalus-5g-0.9.0/5G/core/ui.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # using version 2 for the gateway option with ipam
 version: '2'
 
 networks:
-  rfn:
+  cpn:
     external:
-      name: rfn
+      name: cpn
+
 services:
-  ue1:
-    image: iqtlabs/ueransim:v0.8.0
-    container_name: ue1
+  webui:
+    image: iqtlabs/open5gs:v0.9.0
     depends_on:
-      - gnb
-    cap_add:
-      - NET_ADMIN
-      - SYS_NICE
-    devices:
-      - /dev/net/tun
+      mongodb:
+        condition: service_healthy
+    environment:
+      - NODE_ENV=dev
+      - 'DB_URI=mongodb://${DB_USER}:${DB_PASS}@mongodb/open5gs?authSource=admin'
+      - DB_HOST=mongodb
+    container_name: webui
+    hostname: webui
+    ports:
+      - "3000:3000"
+    entrypoint:
+      - npm
+    command:
+      - run
+      - dev
+      - --prefix
+      - /webui
     networks:
-      rfn:
-        ipv4_address: 192.168.28.101
-    volumes:
-      - "../configs/UERANSIM:/config:z"
+      cpn:
+        ipv4_address: 192.168.26.6
     labels:
+      - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
-    entrypoint:
-      - /scripts/run_ue.sh
-    command:
-      - -c
-      - /config/ue.yaml
```

### Comparing `daedalus-5g-0.8.0/5G/UERANSIM/Dockerfile` & `daedalus-5g-0.9.0/5G/UERANSIM/Dockerfile`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/UERANSIM/gnb.yaml` & `daedalus-5g-0.9.0/5G/configs/UERANSIM/gnb.yaml`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/UERANSIM/ue.yaml` & `daedalus-5g-0.9.0/5G/configs/UERANSIM/ue.yaml`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/faucet/acls.yaml` & `daedalus-5g-0.9.0/5G/configs/faucet/acls.yaml`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/imsis.json` & `daedalus-5g-0.9.0/5G/configs/imsis.json`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/open5gs/smf.yaml` & `daedalus-5g-0.9.0/5G/configs/open5gs/smf.yaml`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/slice.yaml` & `daedalus-5g-0.9.0/5G/configs/slice.yaml`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/drb.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/drb.conf`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/enb.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/enb.conf`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # note: when enabling mbms, use the sib.conf.mbsfn configuration file which includes SIB13
 # rr_config:   Radio Resources configuration file
 # drb_config:  DRB configuration file
 #####################################################################
 [enb_files]
 sib_config = /config/sib.conf
 rr_config  = /config/rr.conf
-drb_config = /config/drb.conf
+rb_config = /config/drb.conf
 
 #####################################################################
 # RF configuration
 #
 # dl_earfcn: EARFCN code for DL (only valid if a single cell is configured in rr.conf)
 # tx_gain: Transmit gain (dB).
 # rx_gain: Optional receive gain (dB). If disabled, AGC if enabled
```

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/drb.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/drb.conf`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,17 @@
   };
   logical_channel_config = {
     priority = 13;
     prioritized_bit_rate   = -1;
     bucket_size_duration  = 100;
     log_chan_group = 2;
   };
+  enb_specific = {
+    dl_max_retx_thresh = 32;
+  };
 },
 {
   qci=9;
   pdcp_config = {
     discard_timer = -1;
     status_report_required = true;
   }
@@ -45,10 +48,13 @@
   };
   logical_channel_config = {
     priority = 11;
     prioritized_bit_rate   = -1;
     bucket_size_duration  = 100;
     log_chan_group = 3;
   };
+  enb_specific = {
+    dl_max_retx_thresh = 32;
+  };
 }
 
 );
```

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/enb.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/enb.conf`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # note: when enabling mbms, use the sib.conf.mbsfn configuration file which includes SIB13
 # rr_config:   Radio Resources configuration file
 # drb_config:  DRB configuration file
 #####################################################################
 [enb_files]
 sib_config = /config/sib.conf
 rr_config  = /config/rr.conf
-drb_config = /config/drb.conf
+rb_config = /config/drb.conf
 
 #####################################################################
 # RF configuration
 #
 # dl_earfcn: EARFCN code for DL
 # tx_gain: Transmit gain (dB).
 # rx_gain: Optional receive gain (dB). If disabled, AGC if enabled
```

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/rr.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/rr.conf`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/limesdr/sib.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/limesdr/sib.conf`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/rr.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/rr.conf`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/sib.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/sib.conf`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         prach_cnfg =
         {
             root_sequence_index = 128;
             prach_cnfg_info =
             {
                 high_speed_flag = false;
                 prach_config_index = 3;
-                prach_freq_offset = 1;
+                prach_freq_offset = 4;
                 zero_correlation_zone_config = 5;
             };
         };
         pdsch_cnfg =
         {
             /* Warning: Currently disabled and forced to p_b=1 for TM2/3/4 and p_b=0 for TM1
              */
@@ -70,16 +70,16 @@
                 group_assignment_pusch = 0;
                 group_hopping_enabled = false;
                 sequence_hopping_enabled = false;
             };
         };
         pucch_cnfg =
         {
-            delta_pucch_shift = 2;
-            n_rb_cqi = 2;
+            delta_pucch_shift = 1;
+            n_rb_cqi = 1;
             n_cs_an = 0;
             n1_pucch_an = 12;
         };
         ul_pwr_ctrl =
         {
             p0_nominal_pusch = -85;
             alpha = 0.7;
@@ -97,17 +97,17 @@
         ul_cp_length = "len1";
     };
 
     ue_timers_and_constants =
     {
         t300 = 2000; // in ms
         t301 = 100;  // in ms
-        t310 = 1000; // in ms
+        t310 = 200; // in ms
         n310 = 1;
-        t311 = 1000; // in ms
+        t311 = 10000; // in ms
         n311 = 1;
     };
 
     freqInfo =
     {
         ul_carrier_freq_present = true;
         ul_bw_present = true;
@@ -147,10 +147,13 @@
             ncc_permitted = 255;
             q_rx_lev_min = 0;
             thresh_x_high = 2;
             thresh_x_low = 2;
 
             start_arfcn = 871;
             band_ind = "dcs1800";
+            explicit_list_of_arfcns = (
+                871
+            );
         }
     );
 };
```

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/ue.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/ue.conf`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/configs/srsRAN/virtual-rr.conf` & `daedalus-5g-0.9.0/5G/configs/srsRAN/virtual-rr.conf`

 * *Files 24% similar despite different names*

```diff
@@ -5,40 +5,43 @@
   {
     rf_port = 0;
     cell_id = 0x01;
     tac = 0x0001;
     pci = 1;
     root_seq_idx = 204;
     dl_earfcn = 2850;
+    ho_active = false;
 
     // CA cells
     #scell_list = (
       #  {cell_id = 0x02; cross_carrier_scheduling = false; scheduling_cell_id = 0x01; ul_allowed = true}
     #)
   },
   {
     rf_port = 1;
     cell_id = 0x02;
     tac = 0x0001;
     pci = 4;
     root_seq_idx = 205;
     dl_earfcn = 3050;
+    ho_active = false;
 
     // CA cells
   #  scell_list = (
   #     {cell_id = 0x01; cross_carrier_scheduling = false; scheduling_cell_id = 0x02; ul_allowed = true}
   #  )
   },
   {
     rf_port = 2;
     cell_id = 0x03;
     tac = 0x0001;
     pci = 7;
     root_seq_idx = 206;
     dl_earfcn = 3250;
+    ho_active = false;
 
     // CA cells
   #  scell_list = (
   #     {cell_id = 0x01; cross_carrier_scheduling = false; scheduling_cell_id = 0x02; ul_allowed = true}
   #  )
   },
   {
@@ -51,7 +54,12 @@
 
     // CA cells
   #  scell_list = (
   #     {cell_id = 0x01; cross_carrier_scheduling = false; scheduling_cell_id = 0x02; ul_allowed = true}
   #  )
   }
 );
+
+nr_cell_list =
+(
+  // no NR cells
+);
```

### Comparing `daedalus-5g-0.8.0/5G/core/core.yml` & `daedalus-5g-0.9.0/5G/core/core.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   cpn:
     external:
       name: cpn
 
 services:
   nrf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     depends_on:
       hss:
         condition: service_started
     container_name: nrf
     hostname: nrf
     entrypoint:
       - /usr/local/bin/open5gs-nrfd
@@ -35,15 +35,15 @@
       cpn:
         ipv4_address: 192.168.26.61
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   ausf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: ausf
     hostname: ausf
     entrypoint:
       - /usr/local/bin/open5gs-ausfd
     command:
       - -c
       - /usr/local/etc/slice.yaml
@@ -53,15 +53,15 @@
       cpn:
         ipv4_address: 192.168.26.70
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   nssf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: nssf
     hostname: nssf
     entrypoint:
       - /usr/local/bin/open5gs-nssfd
     command:
       - -c
       - /usr/local/etc/slice.yaml
@@ -71,15 +71,15 @@
       cpn:
         ipv4_address: 192.168.26.92
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   udm:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: udm
     hostname: udm
     entrypoint:
       - /usr/local/bin/open5gs-udmd
     command:
       - -c
       - /usr/local/etc/slice.yaml
@@ -89,15 +89,15 @@
       cpn:
         ipv4_address: 192.168.26.80
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   bsf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: bsf
     hostname: bsf
     entrypoint:
       - /usr/local/bin/open5gs-bsfd
     command:
       - -c
       - /usr/local/etc/slice.yaml
@@ -107,15 +107,15 @@
       cpn:
         ipv4_address: 192.168.26.91
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   pcf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: pcf
     hostname: pcf
     environment:
       - DB_HOST=mongodb
       - 'DB_USER=${DB_USER}'
       - 'DB_PASS=${DB_PASS}'
     depends_on:
@@ -132,15 +132,15 @@
       cpn:
         ipv4_address: 192.168.26.93
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   udr:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: udr
     hostname: udr
     environment:
       - DB_HOST=mongodb
       - 'DB_USER=${DB_USER}'
       - 'DB_PASS=${DB_PASS}'
     depends_on:
@@ -157,15 +157,15 @@
       cpn:
         ipv4_address: 192.168.26.90
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   amf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: amf
     hostname: amf
     depends_on:
       smf:
         condition: service_started
     entrypoint:
       - /usr/local/bin/open5gs-amfd
```

### Comparing `daedalus-5g-0.8.0/5G/core/db.yml` & `daedalus-5g-0.9.0/5G/core/db.yml`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/core/epc.yml` & `daedalus-5g-0.9.0/5G/core/epc.yml`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   cpn:
     external:
       name: cpn
 
 services:
   hss:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     depends_on:
       mongodbloader:
         condition: service_healthy
     container_name: hss
     hostname: hss
     environment:
       - DB_HOST=mongodb
@@ -30,15 +30,15 @@
       cpn:
         ipv4_address: 192.168.26.10
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   pcrf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     depends_on:
       mongodb:
         condition: service_healthy
       hss:
         condition: service_started
     container_name: pcrf
     hostname: pcrf
@@ -57,20 +57,26 @@
       cpn:
         ipv4_address: 192.168.26.50
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   mme:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: mme
     hostname: mme
     depends_on:
       hss:
         condition: service_started
+    healthcheck:
+      test: /scripts/mmehc.sh
+      interval: 30s
+      timeout: 10s
+      retries: 5
+      start_period: 40s
     entrypoint:
       - /usr/local/bin/open5gs-mmed
     command:
       - -c
       - /usr/local/etc/slice.yaml
     volumes:
       - "../configs:/usr/local/etc:z"
@@ -78,15 +84,15 @@
       cpn:
         ipv4_address: 192.168.26.20
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   smf:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     depends_on:
       sgwc:
         condition: service_started
     container_name: smf
     hostname: smf
     command:
       - "/scripts/run_smf.sh"
@@ -97,15 +103,15 @@
       cpn:
         ipv4_address: 192.168.26.40
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   sgwc:
     restart: always
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     depends_on:
       mme:
         condition: service_started
     container_name: sgwc
     hostname: sgwc
     entrypoint:
       - /usr/local/bin/open5gs-sgwcd
```

### Comparing `daedalus-5g-0.8.0/5G/core/upn.yml` & `daedalus-5g-0.9.0/5G/core/upn.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 networks:
   upn:
     external:
       name: upn
 
 services:
   sgwu:
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: sgwu
     hostname: sgwu
     depends_on:
       smf:
         condition: service_started
     entrypoint:
       - /usr/local/bin/open5gs-sgwud
@@ -24,15 +24,15 @@
     networks:
       upn:
         ipv4_address: 192.168.27.31
     labels:
       - "dovesnap.faucet.mirror=true"
       - "daedalus.namespace=primary"
   upf:
-    image: iqtlabs/open5gs:v0.8.0
+    image: iqtlabs/open5gs:v0.9.0
     container_name: upf
     hostname: upf
     depends_on:
       sgwu:
         condition: service_started
     command:
       - "/scripts/run_upf.sh"
```

### Comparing `daedalus-5g-0.8.0/5G/daedalus/daedalus.py` & `daedalus-5g-0.9.0/5G/daedalus/daedalus.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def build_dockers(srsran=False, ueransim=False, open5gs=False, srsran_lime=False):
         """Build Docker images for the various components"""
         version = 'latest'
         if not 'dev' in __version__:
             version = 'v'+__version__
 
         if srsran:
-            srsran_version = 'release_21_04'
+            srsran_version = 'release_21_10'
             base_args = ['build', '-t', 'iqtlabs/srsran-base:'+version,
                          '-f', 'Dockerfile.base', '.']
             srs_args = ['build', '-t', 'iqtlabs/srsran:'+version, '-f', 'Dockerfile.srs',
                         '--build-arg', f'SRS_VERSION={srsran_version}', '.']
             with local.cwd(local.cwd / 'srsRAN'):
                 docker.bound_command(base_args) & FG
                 docker.bound_command(srs_args) & FG
@@ -97,15 +97,15 @@
         if open5gs:
             args = ['build', '-t', 'iqtlabs/open5gs:'+version, '.']
             with local.cwd(local.cwd / 'open5gs'):
                 docker.bound_command(args) & FG
 
     def start_dovesnap(self):
         """Start Dovesnap components in Docker containers"""
-        release = 'v1.0.1'
+        release = 'v1.0.4'
         faucet_prefix = '/tmp/tpfaucet'
         sudo[ip['link', 'add', 'tpmirrorint', 'type', 'veth',
                 'peer', 'name', 'tpmirror']](retcode=(0, 2))
         sudo[ip['link', 'set', 'tpmirrorint', 'up']]()
         sudo[ip['link', 'set', 'tpmirror', 'up']]()
         sudo[rm['-rf', f'{faucet_prefix}']]()
         sudo[rm['-rf', local.cwd // 'IQTLabs-dovesnap-*']]()
@@ -512,17 +512,18 @@
                     running = False
 
     @staticmethod
     def _check_conf_dir(conf_dir):
         realpath = os.path.realpath(conf_dir)
         if not realpath.endswith('/5G'):
             raise ValueError('last element of conf_dir must be 5G: %s' % realpath)
-        if not realpath.startswith('/usr/local') and not realpath.startswith('/opt') and not realpath.startswith('/home'):
-            raise ValueError('conf_dir root may not be safe: %s' % realpath)
-        return realpath
+        for valid_prefix in ('/usr/local', '/opt', '/home'):
+            if realpath.startswith(valid_prefix):
+                return realpath
+        raise ValueError('conf_dir root may not be safe: %s' % realpath)
 
     def set_config_dir(self, conf_dir='/5G'):
         """Set the current working directory to where the configs are"""
         try:
             realpath = self._check_conf_dir(os.path.dirname(__file__).split('lib')[0] + conf_dir)
             os.chdir(realpath)
             sudo[chown['-R', str(os.getuid()), '.']]()
```

### Comparing `daedalus-5g-0.8.0/5G/daedalus/validators.py` & `daedalus-5g-0.9.0/5G/daedalus/validators.py`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/open5gs/Dockerfile` & `daedalus-5g-0.9.0/5G/open5gs/Dockerfile`

 * *Files 19% similar despite different names*

```diff
@@ -26,18 +26,19 @@
         net-tools \
         ninja-build \
         pkg-config \
         python3-pip \
         python3-setuptools \
         python3-wheel && \
     apt-get clean
-RUN python3 -m pip install meson
+# TODO: need to pin meson to workaround "Target "../dict_dcca_3gpp" has a path segment pointing to directory "subprojects/freeDiameter/extensions/dict_dcca_3gpp/..". This is an error."
+RUN python3 -m pip install -U meson==0.59.3
 RUN apt-get install -y --no-install-recommends npm nodejs
 
-RUN git clone https://github.com/open5gs/open5gs.git -b v2.3.3
+RUN git clone https://github.com/open5gs/open5gs.git -b v2.3.6
 WORKDIR /open5gs
 RUN meson build && ninja -C build install
 WORKDIR /open5gs/webui
 RUN npm install && npm run build
 WORKDIR /open5gs
 # TODO: provide certs externally; open5gs will use locally built certs for now via make_certs.sh in this image.
 RUN sed -r -i 's/C=\w+/C=NZ/g;s/ST=\w+/ST=UpperHutt/g;s/L=\w+/L=Wellington/g' misc/make_certs.sh && \
@@ -51,14 +52,15 @@
 RUN apt-get update && \
     apt-get install -y --no-install-recommends \
         curl \
         jq \
         iproute2 \
         iptables \
         iputils-ping \
+        lksctp-tools \
         net-tools \
         openvswitch-switch \
         tcpdump \
         tshark && \
     apt-get clean
 RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -
 RUN apt-get install -y --no-install-recommends npm nodejs
```

### Comparing `daedalus-5g-0.8.0/5G/open5gs/scripts/nrfhc.sh` & `daedalus-5g-0.9.0/5G/open5gs/scripts/nrfhc.sh`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/open5gs/scripts/run_db.sh` & `daedalus-5g-0.9.0/5G/open5gs/scripts/run_db.sh`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/open5gs/scripts/run_upf.sh` & `daedalus-5g-0.9.0/5G/open5gs/scripts/run_upf.sh`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/5G/srsRAN/Dockerfile.base` & `daedalus-5g-0.9.0/5G/srsRAN/Dockerfile.base`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
      soapysdr-tools \
      tcpdump \
      wget && \
      apt-get autoremove && apt-get clean && rm -rf /var/lib/apt/lists/*
 RUN pip3 install -U requests
 WORKDIR /root
 
-RUN git clone https://github.com/EttusResearch/uhd.git -b v4.1.0.1 \
+RUN git clone https://github.com/EttusResearch/uhd.git -b v4.1.0.3 \
     && mkdir -p /root/uhd/host/build \
     && cd /root/uhd/host/build \
     && cmake -DENABLE_TESTS=OFF -DENABLE_MANUAL=OFF -DENABLE_EXAMPLES=OFF -DENABLE_B100=OFF -DENABLE_USRP1=OFF -DENABLE_USRP2=OFF -DENABLE_X300=OFF -DENABLE_N320=OFF -DENABLE_N300=OFF -DENABLE_E320=OFF -DENABLE_E300=OFF -DENABLE_X400=OFF -DENABLE_MPMD=OFF -DENABLE_OCTOCLOCK=OFF ../ && make -j `nproc` && make install && ldconfig \
     && cd /root && rm -rf /root/uhd
 
 RUN git clone https://github.com/Nuand/bladeRF.git -b 2021.03 \
     && mkdir -p /root/bladeRF/host/build \
```

### Comparing `daedalus-5g-0.8.0/ChangeLog` & `daedalus-5g-0.9.0/ChangeLog`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,46 @@
 CHANGES
 =======
 
+v0.9.0
+------
+
+* bump to v0.9.0
+* 0.9.0 changes
+* 21.10
+* dovesnap 1.0.4
+* Update dependency pytype to v2021.11.2
+* rr
+* sib diff
+* enb\_specific
+* drb -> rb
+* Update dependency ruamel.yaml to v0.17.17
+* upgrade 21\_10
+* Update dependency pytype to v2021.10.25
+* meson/freeDiameter workaround
+* Upgrade Open5GS to 2.3.6
+* Update dependency pytype to v2021.10.18
+* Upgrade Dovesnap 1.0.3, add MME health check (must have SCTP established) with enb/gnb dependencies
+* more compact prefix check, verbose stdout/stderr test to avoid GHA thinking test has stalled
+* Update dependency pytype to v2021.10.11
+* Upgrade UHD to v4.1.0.3
+* Update dependency docker to v5.0.3
+* Open5GS 2.3.4
+* Update dependency pytype to v2021.10.4
+* Update dependency pytest-cov to v3
+* Update dependency pytype to v2021.9.27
+* Update dependency pylint to v2.11.1
+* don't ignore any paths
+* Update dependency dovesnap to v1.0.3
+* Update codecov/codecov-action action to v2.1.0
+* update pytype
+* add use cases
+* Update dependency dovesnap to v1.0.2
+* bump back to dev
+
 v0.8.0
 ------
 
 * release v0.8.0
 * remove TODO
 * Redundant chown
 * update test requirements
```

### Comparing `daedalus-5g-0.8.0/README.md` & `daedalus-5g-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `daedalus-5g-0.8.0/daedalus_5g.egg-info/SOURCES.txt` & `daedalus-5g-0.9.0/daedalus_5g.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 5G/core/ui.yml
 5G/core/upn.yml
 5G/daedalus/__init__.py
 5G/daedalus/__main__.py
 5G/daedalus/daedalus.py
 5G/daedalus/validators.py
 5G/open5gs/Dockerfile
+5G/open5gs/scripts/mmehc.sh
 5G/open5gs/scripts/nrfhc.sh
 5G/open5gs/scripts/run_db.sh
 5G/open5gs/scripts/run_smf.sh
 5G/open5gs/scripts/run_upf.sh
 5G/srsRAN/Dockerfile.base
 5G/srsRAN/Dockerfile.srs
 5G/srsRAN/scripts/add_default_route.sh
```

### Comparing `daedalus-5g-0.8.0/setup.cfg` & `daedalus-5g-0.9.0/setup.cfg`

 * *Files identical despite different names*

