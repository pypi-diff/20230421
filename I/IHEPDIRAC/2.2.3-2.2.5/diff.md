# Comparing `tmp/IHEPDIRAC-2.2.3.tar.gz` & `tmp/IHEPDIRAC-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IHEPDIRAC-2.2.3.tar", last modified: Thu Apr 28 02:53:12 2022, max compression
+gzip compressed data, was "IHEPDIRAC-2.2.5.tar", last modified: Fri Apr 21 04:58:00 2023, max compression
```

## Comparing `IHEPDIRAC-2.2.3.tar` & `IHEPDIRAC-2.2.5.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.775133 IHEPDIRAC-2.2.3/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     1270 2022-04-21 03:28:15.000000 IHEPDIRAC-2.2.3/LICENSE
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      120 2022-04-21 04:04:14.000000 IHEPDIRAC-2.2.3/MANIFEST.in
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      436 2022-04-28 02:53:12.776134 IHEPDIRAC-2.2.3/PKG-INFO
--rw-rw-r--   0 dirac     (1000) dirac     (1000)       51 2022-04-21 03:28:15.000000 IHEPDIRAC-2.2.3/README.md
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      226 2022-04-21 04:04:20.000000 IHEPDIRAC-2.2.3/pyproject.toml
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     2255 2022-04-28 02:53:12.776134 IHEPDIRAC-2.2.3/setup.cfg
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      323 2022-04-21 04:04:36.000000 IHEPDIRAC-2.2.3/setup.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.296129 IHEPDIRAC-2.2.3/src/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.743133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.744133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Core/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.745133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Core/Utilities/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     1941 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Core/Utilities/DErrno.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Core/Utilities/__init__.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Core/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.745133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.747133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:42:19.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/__init__.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1827 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_add_dir.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     3510 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_check_replicas.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4325 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_EOS_files.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4021 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_dir.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4386 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_files.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1992 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1972 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir_replicas.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     8935 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_scan_unregistered.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.747133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.748133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Agent/
--rw-r--r--   0 dirac     (1000) dirac     (1000)     4299 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Agent/CacheFeederIHEPAgent.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     4044 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Agent/CacheFeederIHEPAgent.py.bak
--rw-r--r--   0 dirac     (1000) dirac     (1000)     7912 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Agent/SAMTestAgent.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Agent/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.748133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Client/
--rw-r--r--   0 dirac     (1000) dirac     (1000)    25008 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Client/ResourceManagementIHEPClient.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Client/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.749133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/
--rw-r--r--   0 dirac     (1000) dirac     (1000)     2943 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/HostCommand.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     6658 2022-04-27 15:45:25.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/JobIHEPCommand.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     1623 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/SAMIHEPCommand.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     3248 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/StorageIHEPCommand.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     3566 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/WorkNodeIHEPCommand.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/__init__.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)      570 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/ConfigTemplate.cfg
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.750133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/DB/
--rw-r--r--   0 dirac     (1000) dirac     (1000)    17561 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/DB/ResourceManagementIHEPDB.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)       30 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/DB/ResourceManagementIHEPDB.sql
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/DB/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.751133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Policy/
--rw-r--r--   0 dirac     (1000) dirac     (1000)      413 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Policy/Configurations.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     2180 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Policy/SiteSAMPolicy.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Policy/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.751133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.752133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/
--rw-r--r--   0 dirac     (1000) dirac     (1000)     3374 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/__init__.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.752133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.755133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/
--rw-r--r--   0 dirac     (1000) dirac     (1000)     2866 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/AccessTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     1452 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/BOSSTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     1756 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEAccessTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     7622 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEBaseTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)      778 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEPCTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     1217 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CLOUDAccessTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)      803 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CVMFSTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)      866 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/JUNOTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     1067 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SEAccessTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     3722 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SETest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)      887 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestBase.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     1514 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestConfiguration.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)      819 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/WMSTest.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 09:01:41.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/__init__.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     5084 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/StatusEvaluator.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     8170 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/TestExecutor.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.756133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 09:02:03.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/__init__.py
--rwxr-xr-x   0 dirac     (1000) dirac     (1000)     1854 2022-04-27 13:52:17.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/boss_test.py
--rwxr-xr-x   0 dirac     (1000) dirac     (1000)      851 2022-04-27 13:57:05.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cepc_test.py
--rwxr-xr-x   0 dirac     (1000) dirac     (1000)      762 2022-04-27 14:02:23.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cvmfs_test.py
--rwxr-xr-x   0 dirac     (1000) dirac     (1000)     1108 2022-04-27 14:09:54.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/juno_test.py
--rwxr-xr-x   0 dirac     (1000) dirac     (1000)     1305 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/se_test.py
--rwxr-xr-x   0 dirac     (1000) dirac     (1000)      203 2022-04-27 14:14:44.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/wms_test.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.762133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Service/
--rw-r--r--   0 dirac     (1000) dirac     (1000)    18528 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Service/PublisherIHEPHandler.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     7316 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Service/ResourceManagementIHEPHandler.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Service/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.763133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/
--rw-r--r--   0 dirac     (1000) dirac     (1000)     3380 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/BESUtils.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     9455 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/CSHelpers.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)     6409 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/MySQLWrapper.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/__init__.py
--rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:59:02.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.299129 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Resources/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.763133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Resources/scripts/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:43:01.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Resources/scripts/__init__.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)      819 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/Resources/scripts/ihepdirac_resource_get_squids.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.764133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.299129 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.765133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1501 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/bootstrap.sh
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     2509 2022-04-27 15:46:58.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-add-files.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)      575 2022-04-27 15:50:29.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-set-job-status.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)      993 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-calib-ts.sh
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)      916 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-detsim-ts.sh
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1082 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim-ts.sh
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1116 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim_rec-ts.sh
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1045 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-rec-ts.sh
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.768133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:40:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/__init__.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)    27963 2022-04-28 02:39:12.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_productions.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)    23389 2022-04-28 02:39:39.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)    24695 2022-04-28 02:50:44.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction_sim.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     2758 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_reset_files.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     2970 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_dir.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4297 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_metadata.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.768133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.770134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     8077 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/SAMHistoryHandler.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)    10474 2022-04-27 15:47:59.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/SiteStatusMonitorHandler.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)    14272 2022-04-27 15:49:28.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/TaskManagerHandler.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.300129 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.301129 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.300129 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.770134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/classes/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)    16341 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/classes/SAMHistory.js
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.770134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/css/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      105 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/css/SAMHistory.css
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.770134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/images/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      226 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/images/grid.png
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.300129 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.770134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/classes/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)    13578 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/classes/SiteStatusMonitor.js
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.301129 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.771134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/classes/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)    30737 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/classes/TaskManager.js
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.771134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/css/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/css/TaskManager.css
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      220 2022-04-27 13:32:05.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/web.cfg
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.771134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.772133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Agent/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     6506 2022-04-27 15:24:51.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Agent/TaskAgent.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Agent/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.772133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Client/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     3135 2022-04-27 15:25:17.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Client/TaskClient.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Client/__init__.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      162 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.773134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/DB/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)    14521 2022-04-27 13:32:55.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)       12 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.sql
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/DB/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.774134 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Service/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)    17562 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Service/TaskManagerHandler.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Service/__init__.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      348 2022-03-29 08:16:34.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.775133 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:41:51.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/__init__.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)      966 2022-04-27 14:23:50.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-delete.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     3089 2022-04-27 15:07:32.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-event-progress.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1645 2022-04-27 15:09:56.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-job-show.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4454 2022-04-27 15:07:16.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-list.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1258 2022-04-27 14:29:24.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-reschedule.py
--rwxrwxr-x   0 dirac     (1000) dirac     (1000)     3121 2022-04-27 15:06:58.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-show.py
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      569 2022-04-21 04:05:19.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC/__init__.py
-drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2022-04-28 02:53:12.744133 IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      436 2022-04-28 02:53:11.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/PKG-INFO
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     7475 2022-04-28 02:53:12.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/SOURCES.txt
--rw-rw-r--   0 dirac     (1000) dirac     (1000)        1 2022-04-28 02:53:11.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/dependency_links.txt
--rw-rw-r--   0 dirac     (1000) dirac     (1000)     1596 2022-04-28 02:53:11.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/entry_points.txt
--rw-rw-r--   0 dirac     (1000) dirac     (1000)      139 2022-04-28 02:53:12.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/requires.txt
--rw-rw-r--   0 dirac     (1000) dirac     (1000)       10 2022-04-28 02:53:12.000000 IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/top_level.txt
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.254247 IHEPDIRAC-2.2.5/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     1270 2022-04-21 03:28:15.000000 IHEPDIRAC-2.2.5/LICENSE
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      120 2022-04-21 04:04:14.000000 IHEPDIRAC-2.2.5/MANIFEST.in
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      391 2023-04-21 04:58:00.254247 IHEPDIRAC-2.2.5/PKG-INFO
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)       51 2022-04-21 03:28:15.000000 IHEPDIRAC-2.2.5/README.md
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      221 2023-04-21 04:24:17.000000 IHEPDIRAC-2.2.5/pyproject.toml
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     2206 2023-04-21 04:58:00.255247 IHEPDIRAC-2.2.5/setup.cfg
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      323 2022-04-21 04:04:36.000000 IHEPDIRAC-2.2.5/setup.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.128246 IHEPDIRAC-2.2.5/src/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.140246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.142246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Core/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.144246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Core/Utilities/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     1941 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Core/Utilities/DErrno.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Core/Utilities/__init__.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Core/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.144246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:28:03.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.152246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:28:03.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/__init__.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1827 2023-04-20 08:28:03.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_add_dir.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     3510 2023-04-20 08:28:03.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_check_replicas.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4782 2023-04-21 02:44:23.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_EOS_files.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4021 2023-04-20 08:28:03.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_dir.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4386 2023-04-20 08:28:03.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_files.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1992 2023-04-20 08:28:03.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1983 2023-04-21 02:24:10.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir_replicas.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     9497 2023-04-21 02:24:10.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_scan_unregistered.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.154246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.156246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Agent/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     4297 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Agent/CacheFeederIHEPAgent.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     7912 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Agent/SAMTestAgent.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Agent/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.157246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Client/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)    25117 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Client/ResourceManagementIHEPClient.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Client/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.162246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     2943 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/HostCommand.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     6658 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/JobIHEPCommand.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     1623 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/SAMIHEPCommand.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     3248 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/StorageIHEPCommand.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     3574 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/WorkNodeIHEPCommand.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/__init__.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)      570 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/ConfigTemplate.cfg
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.164246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/DB/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)    17561 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/DB/ResourceManagementIHEPDB.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)       30 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/DB/ResourceManagementIHEPDB.sql
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/DB/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.166246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Policy/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)      413 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Policy/Configurations.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     2180 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Policy/SiteSAMPolicy.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Policy/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.166246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.168246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     3374 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/__init__.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.170246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.184246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     2866 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/AccessTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     1452 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/BOSSTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     1756 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEAccessTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     7622 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEBaseTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)      778 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEPCTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     1217 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CLOUDAccessTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)      803 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CVMFSTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)      866 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/JUNOTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     1067 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SEAccessTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     3722 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SETest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)      887 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestBase.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     1514 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestConfiguration.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)      819 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/WMSTest.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/__init__.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     5084 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/StatusEvaluator.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     8168 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/TestExecutor.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.190246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/__init__.py
+-rwxr-xr-x   0 dirac     (1000) dirac     (1000)     1854 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/boss_test.py
+-rwxr-xr-x   0 dirac     (1000) dirac     (1000)      851 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cepc_test.py
+-rwxr-xr-x   0 dirac     (1000) dirac     (1000)      762 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cvmfs_test.py
+-rwxr-xr-x   0 dirac     (1000) dirac     (1000)     1108 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/juno_test.py
+-rwxr-xr-x   0 dirac     (1000) dirac     (1000)     1305 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/se_test.py
+-rwxr-xr-x   0 dirac     (1000) dirac     (1000)      203 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/wms_test.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.193246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Service/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)    18714 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Service/PublisherIHEPHandler.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     7316 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Service/ResourceManagementIHEPHandler.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Service/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.196246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     3380 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/BESUtils.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     9455 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/CSHelpers.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)     6409 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/MySQLWrapper.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/__init__.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:24:18.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.132246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Resources/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.196246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Resources/scripts/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:43:01.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Resources/scripts/__init__.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)      819 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/Resources/scripts/ihepdirac_resource_get_squids.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.198247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.132246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.205247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1501 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/bootstrap.sh
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     2509 2022-04-27 15:46:58.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-add-files.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)      575 2022-04-27 15:50:29.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-set-job-status.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)      993 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-calib-ts.sh
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)      916 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-detsim-ts.sh
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1082 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim-ts.sh
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1116 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim_rec-ts.sh
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1045 2022-03-29 07:46:48.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-rec-ts.sh
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.213247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2022-03-29 08:40:37.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/__init__.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    27964 2022-07-28 23:30:57.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_productions.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    23390 2022-07-28 23:31:44.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)    24695 2022-04-28 02:50:44.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction_sim.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     2758 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_reset_files.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     2978 2023-04-21 02:24:10.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_dir.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4297 2022-04-19 02:42:37.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_metadata.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.215247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.219247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     8077 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/SAMHistoryHandler.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    10481 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/SiteStatusMonitorHandler.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    14301 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/TaskManagerHandler.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.134246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.135246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.134246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.219247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/classes/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    16341 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/classes/SAMHistory.js
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.220247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/css/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      105 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/css/SAMHistory.css
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.221247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/images/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      226 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/images/grid.png
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.135246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.229247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/classes/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    13578 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/classes/SiteStatusMonitor.js
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.135246 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.237247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/classes/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    30737 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/classes/TaskManager.js
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.239247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/css/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/css/TaskManager.css
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      210 2023-04-20 09:13:26.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/web.cfg
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.241247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.243247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Agent/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     6509 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Agent/TaskAgent.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Agent/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.244247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Client/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     3135 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Client/TaskClient.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Client/__init__.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      398 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.246247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/DB/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    14689 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)       12 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.sql
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/DB/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.247247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Service/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)    17241 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Service/TaskManagerHandler.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Service/__init__.py
+-rw-r--r--   0 dirac     (1000) dirac     (1000)    17620 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Service/root@samtest.ihep.ac.cn
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      348 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.253247 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        0 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/__init__.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)      966 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-delete.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     3089 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-event-progress.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1645 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-job-show.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     4454 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-list.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     1258 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-reschedule.py
+-rwxrwxr-x   0 dirac     (1000) dirac     (1000)     3121 2023-04-20 08:27:30.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-show.py
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      579 2023-04-20 07:18:19.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC/__init__.py
+drwxrwxr-x   0 dirac     (1000) dirac     (1000)        0 2023-04-21 04:58:00.142246 IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)      391 2023-04-21 04:58:00.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/PKG-INFO
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     7477 2023-04-21 04:58:00.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/SOURCES.txt
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)        1 2023-04-21 04:58:00.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/dependency_links.txt
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)     1596 2023-04-21 04:58:00.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/entry_points.txt
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)       94 2023-04-21 04:58:00.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/requires.txt
+-rw-rw-r--   0 dirac     (1000) dirac     (1000)       10 2023-04-21 04:58:00.000000 IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/top_level.txt
```

### Comparing `IHEPDIRAC-2.2.3/LICENSE` & `IHEPDIRAC-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/setup.cfg` & `IHEPDIRAC-2.2.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [metadata]
 name = IHEPDIRAC
-version = 2.2.3
+version = 2.2.5
 description = IHEPDIRAC is the IHEP extension of DIRAC
 url = https://code.ihep.ac.cn/Grid/IHEPDIRAC
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.9
 install_requires = DIRAC
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 server = 
-	DIRAC[server] ~= 7.3.0
-	WebAppDIRAC ~=4.3.0
-	DIRACWebAppResources ~=1.0
+	DIRAC[server] ~= 8.0.0
 	psutil
 	stomp.py
 	suds-jurko
 testing = 
 	mock
 	Pillow
 	pytest
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/Core/Utilities/DErrno.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/Core/Utilities/DErrno.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_add_dir.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_add_dir.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_check_replicas.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_check_replicas.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_EOS_files.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_EOS_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,26 +67,30 @@
     counter = 0
     eosclient = client.FileSystem(eosRoot)
 
     dm = DataManager()
     fileTupleBuffer = []
 
     cmd = 'xrdfs %s ls %s -R' % (eosHead, eosPath)
+    gLogger.debug('Commands to get files:%s' % (cmd))
     file_obj = os.popen(cmd).readlines()
+    #gLogger.debug('file lists:%s' % (file_obj))
     for fullFn in file_obj:
         counter += 1
         fullFn=fullFn.strip('\n')
+        gLogger.debug('fullFn:%s' % (fullFn))
 
         if not fullFn.startswith(eosPath):
             gLogger.error('%s does not start with %s' % (fullFn, localDir))
             continue 
         lastPart = fullFn[len(eosPath):]
         pfn = eosHead + fullFn
-       
+      
         lfn = dfcRoot + lastPart
+        gLogger.debug('lfn, dfcRoot, lastPart:%s, %s, %s' % (lfn, dfcRoot, lastPart))
 
         if lfn in lfnQuery:
             gLogger.notice('File exists, skip: %s' % lfn)
             counter -= 1
             continue
 
         if existCheck:
@@ -96,24 +100,31 @@
                 counter -= 1
                 continue
 
         status, response = eosclient.stat(fullFn)
         if status.ok:
             size = response.size
         else:
-            gLogger.error('Error in getting size of %s!')% lfn
+            gLogger.error('Error in getting size of %s!' % lfn)
             continue
+        # 19 is a directory
+        if response.flags == 19:
+           gLogger.debug('%s is a directory' % lfn)
+           counter -= 1
+           continue
+
         status, response = eosclient.query(QueryCode.CHECKSUM, fullFn)
         if status.ok:
             gchecksum = response.split()
         else:
-            gLogger.error('Error in getting checksum of %s!')% lfn
+            gLogger.error('%s is not a file, or has problems to get checksum!')% lfn
             continue
         if size != 0:
-            adler32 = str(gchecksum[1].strip(b'\x00'.decode()))
+            #adler32 = gchecksum[1].strip(b'\x00'.decode())
+            adler32 = gchecksum[1].strip(b'\x00')
             guid = makeGuid()
             fileTuple = ( lfn, pfn, size, toSE, guid, adler32 )
             gLogger.debug('To be registered: %s %s %s %s %s %s' % (lfn,pfn,size,toSE,guid,adler32))
             fileTupleBuffer.append(fileTuple)
             gLogger.debug('Register lfn: %s' % lfn)
         else:
             counter -=1
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_dir.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_dir.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_files.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_files.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir_replicas.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir_replicas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 """
 Remove specified replica from SE under specified directory
 Usage:
-  ihepdirac_dms_rm_dir_replicas [option|cfgfile] DFCDir SE 
+  ihepdirac_dms_rm_dir_replicas [option|cfgfile] DFCDir SE
 
 Example:
   $ ihepdirac_dms_rm_dir_replicas /juno/production/muon/prd100 IHEP-STORM
 """
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
@@ -27,15 +27,15 @@
 from DIRAC.DataManagementSystem.Client.DataManager import DataManager
 dm = DataManager()
 
 counterFile = 0
 counterDir = 0
 
 
-def removeFromDir(d):
+def removeFromDir(d, SE):
     global counterFile
     global counterDir
 
     result = fcc.listDirectory(d)
     if not result['OK']:
         gLogger.error('Failed to list directory %s: %s' %
                       (d, result['Message']))
@@ -49,15 +49,15 @@
         gLogger.notice(
             'Removing replicas of {0} files from dir "{1}"'.format(fileNumber, d))
         counterFile += fileNumber
         dm.removeReplica(SE, files)
 
     if result['Value']['Successful'][d]['SubDirs']:
         for subdir in result['Value']['Successful'][d]['SubDirs']:
-            removeFromDir(subdir)
+            removeFromDir(subdir, SE)
 
     counterDir += 1
 
 
 @DIRACScript()
 def main():
 
@@ -68,15 +68,15 @@
     if len(args) != 2:
         Script.showHelp()
         exit(1)
 
     dfcDir = args[0]
     SE = args[1]
 
-    removeFromDir(dfcDir)
+    removeFromDir(dfcDir, SE)
 
     gLogger.notice('%s directories and %s files deleted' %
                (counterDir, counterFile))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_scan_unregistered.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_scan_unregistered.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 """
 Scan dark files in assigned SEs.
 Usage:
-  ihepdirac_dms_scan_unregistered [option|cfgfile] DFCDir SE 
+  ihepdirac-dms-scan-unregistered [option|cfgfile] DFCDir SE
 
 Example:
-  $ ihepdirac_dms_scan_unregistered /juno/production/muon/prd100 IHEP-STORM
+  $ ihepdirac-dms-scan-unregistered /juno/production/muon/prd100 IHEP-STORM
 """
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 __RCSID__ = "$Id$"
 
@@ -198,63 +198,75 @@
         else:
            if not srmSwitch:
               listFile(PFNURL)
            else:
               srmListFile(i)
 
     # duplicate removal
-    fileList = list(set(fileList))
-    fileList.sort()
-    fileDFCList = list(set(fileDFCList))
-    fileDFCList.sort()
+    fileList_copy = list(set(fileList))
+    fileList_copy.sort()
+    fileDFCList_copy = list(set(fileDFCList))
+    fileDFCList_copy.sort()
 
     # output
     if not srmSwitch:
-       gLogger.notice("----------  Files found in assigned SE:  ----------")
+       gLogger.debug("----------  Files found in assigned SE:  ----------")
     else:
-       gLogger.notice("----------  Files found in assigned DFC:  ----------")
-    for i in fileDFCList:
-       gLogger.notice(i)
+       gLogger.debug("----------  Files found in assigned DFC:  ----------")
+    for i in fileDFCList_copy:
+       gLogger.debug(i)
        if not srmSwitch:
           compareFile(i)
        else:
           srmCompareFile(i)
-    gLogger.notice("----------  Total: %d found files.  ----------\n" %len(fileDFCList))
+    gLogger.notice("----------  Total: %d found files.  ----------\n" %len(fileDFCList_copy))
 
     if not srmSwitch:
-       gLogger.notice("----------  Files unregistered (dark files):  ----------")
+       gLogger.debug("----------  Files unregistered (dark files):  ----------")
        for i in fileDarkList:
-           gLogger.notice(i)
+           gLogger.debug(i)
        gLogger.notice("----------  Total: %d dark files.  ----------\n" %len(fileDarkList))
 
-    gLogger.notice("----------  Files registered but not register as assigned SE replicas:  ----------")
+    gLogger.debug("----------  Files registered but not register as assigned SE replicas:  ----------")
     for i in fileUnlinkedList:
-        gLogger.notice(i)
+        gLogger.debug(i)
     gLogger.notice("----------  Total: %d unlinked files.  ----------\n" %len(fileUnlinkedList))
 
     if deletionSwitch:
         for i in fileDarkList:
             g.unlink(HEAD0 + '/' + i)
-            gLogger.notice("%s deleted!" %(HEAD0 + '/' + i))
+            gLogger.debug("%s deleted!" %(HEAD0 + '/' + i))
         gLogger.notice("----------  All dark files deleted!  ----------\n")
 
     if registerOption != 'none':
         if registerOption in ['dark', 'both']:
-            gLogger.notice("----------  Register dark files:  ----------")
+            gLogger.debug("----------  Register dark files:  ----------")
+            fileTupleBuffer = []
             for i in fileDarkList:
                 fileStat = g.stat(HEAD0 + '/' + i)
                 fileSize = fileStat.st_size
                 fileGuid = makeGuid()
                 fileSum = g.checksum(HEAD0 + '/' + i, "ADLER32")
                 fileTuple = (i, HEAD0 + '/' + i, fileSize, SITE, fileGuid, fileSum)
-                dm.registerFile(fileTuple)
-                gLogger.notice(i + ' registered successfully!')
+                fileTupleBuffer.append(fileTuple)
+                if len(fileTupleBuffer) > 499:
+                    dm.registerFile(fileTupleBuffer)
+                    fileTupleBuffer = []
+                gLogger.debug(i + ' registered successfully!')
+            if len(fileTupleBuffer) > 0:
+                dm.registerFile(fileTupleBuffer)
         if registerOption in ['unlinked', 'both']:
-            gLogger.notice("----------  Register unlinked files:  ----------")
+            gLogger.debug("----------  Register unlinked files:  ----------")
+            fileTupleBuffer = []
             for i in fileUnlinkedList:
                 fileTuple = (i, HEAD0 + '/' + i, SITE)
-                dm.registerReplica(fileTuple)
-                gLogger.notice(i + ' registered successfully!')
+                fileTupleBuffer.append(fileTuple)
+                if len(fileTupleBuffer) > 499:
+                    dm.registerReplica(fileTupleBuffer)
+                    fileTupleBuffer = []
+                gLogger.debug(i + ' registered successfully!')
+            if len(fileTupleBuffer) > 0:
+                dm.registerReplica(fileTupleBuffer)
         gLogger.notice("----------  Register finished  ----------\n")
 
 if __name__ == "__main__":
     main()
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Agent/CacheFeederIHEPAgent.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Agent/CacheFeederIHEPAgent.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 from future import standard_library
 standard_library.install_aliases()
 from builtins import *
 from DIRAC                                                      import S_OK
 from DIRAC.AccountingSystem.Client.ReportsClient                import ReportsClient
 from DIRAC.Core.Base.AgentModule                                import AgentModule
-#from DIRAC.Core.DISET.RPCClient                                 import RPCClient
+from DIRAC.Core.DISET.RPCClient                                 import RPCClient
 #from DIRAC.Core.LCG.GOCDBClient                                 import GOCDBClient
-#from DIRAC.ResourceStatusSystem.Client.ResourceStatusClient     import ResourceStatusClient
-#from DIRAC.ResourceStatusSystem.Command                         import CommandCaller
+from DIRAC.ResourceStatusSystem.Client.ResourceStatusClient     import ResourceStatusClient
+from DIRAC.ResourceStatusSystem.Command                         import CommandCaller
 from DIRAC.ResourceStatusSystem.Utilities                       import Utils
 ResourceManagementIHEPClient = getattr( Utils.voimport( 'DIRAC.ResourceStatusSystem.Client.ResourceManagementIHEPClient' ), 'ResourceManagementIHEPClient' )
 
 __RCSID__ = '$Id:  $'
 AGENT_NAME = 'ResourceStatus/CacheFeederIHEPAgent'
 
 class CacheFeederIHEPAgent( AgentModule ):
@@ -51,15 +51,15 @@
     self.rmClient = ResourceManagementIHEPClient()
 
     self.commands[ 'JobIHEP' ] = [ { 'JobIHEP' : {} } ]
     self.commands[ 'StorageIHEP' ] = [ { 'StorageIHEP' : {} } ]
     self.commands[ 'WorkNodeIHEP' ] = [ { 'WorkNodeIHEP' : {} } ]
 
     # Reuse clients for the commands
-    self.clients[ 'GOCDBClient' ] = GOCDBClient()
+    #self.clients[ 'GOCDBClient' ] = GOCDBClient()
     self.clients[ 'ReportGenerator' ] = RPCClient( 'Accounting/ReportGenerator' )
     self.clients[ 'ReportsClient' ] = ReportsClient()
     self.clients[ 'ResourceStatusClient' ] = ResourceStatusClient()
     self.clients[ 'ResourceManagementIHEPClient' ] = ResourceManagementIHEPClient()
     self.clients[ 'WMSAdministrator' ] = RPCClient( 'WorkloadManagement/WMSAdministrator' )
 
     self.cCaller = CommandCaller
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Agent/SAMTestAgent.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Agent/SAMTestAgent.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Client/ResourceManagementIHEPClient.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Client/ResourceManagementIHEPClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """ ResourceManagementIHEPClient
 
   ResourceManagementIHEPClient for IHEPDIRAC.
 
 """
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
 
 from DIRAC                      import gLogger, S_ERROR
 from datetime                   import datetime, timedelta
 from DIRAC.Core.DISET.RPCClient import RPCClient
 
 __RCSID__ = '$Id:  $'
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/HostCommand.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/HostCommand.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/JobIHEPCommand.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/JobIHEPCommand.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/SAMIHEPCommand.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/SAMIHEPCommand.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/StorageIHEPCommand.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/StorageIHEPCommand.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Command/WorkNodeIHEPCommand.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Command/WorkNodeIHEPCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     hosts = masterParams
 
     sql = """
 select JP.Value, J.Status, J.Site, count(*) from Jobs J, JobParameters JP
 where J.JobID = JP.JobID and JP.Name = 'HostName'
 and J.EndExecTime >= DATE_SUB(UTC_TIMESTAMP(),INTERVAL 24 HOUR)
-group by JP.Value, J.Status
+group by JP.Value, J.Status, J.site
 """
 
     jobDB = JobDB()
     queryRes = jobDB._query(sql)
     if not queryRes[ 'OK' ]:
       return queryRes
     records = queryRes[ 'Value' ]
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/ConfigTemplate.cfg` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/DB/ResourceManagementIHEPDB.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/DB/ResourceManagementIHEPDB.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Policy/SiteSAMPolicy.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Policy/SiteSAMPolicy.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/AccessTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/AccessTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/BOSSTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/BOSSTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEAccessTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEAccessTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEBaseTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEBaseTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEPCTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CEPCTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CLOUDAccessTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CLOUDAccessTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CVMFSTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/CVMFSTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/JUNOTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/JUNOTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SEAccessTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SEAccessTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SETest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/SETest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestBase.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestBase.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestConfiguration.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/TestConfiguration.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/WMSTest.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/SAMTest/WMSTest.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/StatusEvaluator.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/StatusEvaluator.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/TestExecutor.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/TestExecutor.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from __future__ import unicode_literals
  
 from future import standard_library
 standard_library.install_aliases()
 from builtins import *
 from builtins import object
 
-#import time
-#import random
+import time
+import random
 import queue
 from datetime import datetime
 from DIRAC                                                         import S_OK, S_ERROR, gLogger
 from IHEPDIRAC.ResourceStatusSystem.Client.ResourceManagementIHEPClient import ResourceManagementIHEPClient
 
 
 __RCSID__ = '$Id:  $'
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/boss_test.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/boss_test.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cepc_test.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cepc_test.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cvmfs_test.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/cvmfs_test.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/juno_test.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/juno_test.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/se_test.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/SAM/sam_script/se_test.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Service/PublisherIHEPHandler.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Service/PublisherIHEPHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,31 +150,34 @@
       ces = CSHelpers.getSiteComputingElements(siteName)
 
     ses = CSHelpers.getSiteStorageElements(siteName)
 
     return S_OK({ 'ComputingElement' : ces, 'StorageElement' : ses })
 
   types_getSitesSAMSummary = [  (str, type(None), list), (str, type(None), list) ]
+  #types_getSitesSAMSummary = []
   def export_getSitesSAMSummary(self, sitesName, vo = None):
     """
     Return the dictionary with SAM summary information for the given sites.
 
     :return: S_OK( { site : { 'CEStatus' : 'OK'
                                                    'SEStatus' : 'Bad'
                                                    } } ) | S_ERROR
     """
 
     gLogger.info('getSitesSAMSummary')
 
     sitesSAMSummary = {}
 
     vo = vo or 'all'
+    gLogger.debug('rmClient.selectSiteSAMStatus++++++++++++++%s', sitesName)
     queryRes = rmClient.selectSiteSAMStatus(site = sitesName, vO = vo,
                                             meta = { 'newer' : [ 'LastCheckTime',
                                                                 datetime.utcnow().replace(microsecond = 0) - timedelta(hours = 24) ] })
+    gLogger.debug('rmClient.selectSiteSAMStatus++++++++++++++%s', queryRes)
     if not queryRes[ 'OK' ]:
       return queryRes
     records = queryRes[ 'Value' ]
     columns = queryRes[ 'Columns' ]
 
     for record in records:
       recordDict = dict(zip(columns, record))
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Service/ResourceManagementIHEPHandler.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Service/ResourceManagementIHEPHandler.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/BESUtils.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/BESUtils.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/CSHelpers.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/CSHelpers.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/ResourceStatusSystem/Utilities/MySQLWrapper.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/ResourceStatusSystem/Utilities/MySQLWrapper.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/Resources/scripts/ihepdirac_resource_get_squids.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/Resources/scripts/ihepdirac_resource_get_squids.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/bootstrap.sh` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-add-files.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-add-files.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-set-job-status.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/dirac-set-job-status.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-calib-ts.sh` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-calib-ts.sh`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-detsim-ts.sh` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-detsim-ts.sh`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim-ts.sh` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim-ts.sh`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim_rec-ts.sh` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-elecsim_rec-ts.sh`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-rec-ts.sh` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/runtime/juno/run-rec-ts.sh`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_productions.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_productions.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
         t.setGroupSize(self.__groupSize)
         if self.__transGroup:
             t.setTransformationGroup(self.__transGroup)
         t.setPlugin(self.__plugin)
 
         t.setTargetSE(self.__targetSE)
 
-        transBody = []
+        transBody = '' 
 
         t.setBody(transBody)
 
         ########################################
         # Transformation submission
         ########################################
         res = t.addTransformation()
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         if self.__transGroup:
             t.setTransformationGroup(self.__transGroup)
         t.setPlugin(self.__plugin)
 
 #        t.setSourceSE(self.__sourceSE)
         t.setTargetSE(self.__targetSE)
 
-        transBody = []
+        transBody = '' 
 
 #        transBody.append(
 #            ("ReplicateAndRegister", {"TargetSE": ','.join(self.__targetSE)}))
 
 #        for tse in self.__targetSE:
 #            sse = list(set(self.__sourceSE) - set([tse]))
 #            transBody.append(("ReplicateAndRegister", {"SourceSE": ','.join(sse), "TargetSE": ','.join(tse)}))
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction_sim.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_juno_make_reconstruction_sim.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_reset_files.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_reset_files.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_dir.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
     fcc = FileCatalogClient('DataManagement/FileCatalog')
     result = fcc.listDirectory(inDir)
     if not result['OK'] or 'Successful' not in result['Value'] or inDir not in result['Value']['Successful']:
        gLogger.error('Can not list directory %s' % inDir)
        exit(2)
 
-    infileList = result['Value']['Successful'][inDir]['Files'].keys()
-    infileList.sort()
+    infileList = list(result['Value']['Successful'][inDir]['Files'].keys())
+    sorted(infileList)
 
     print('%s files to transfer' % len(infileList))
 
     if not infileList:
         gLogger.Info('No file to transfer')
         exit(0)
 
@@ -82,9 +82,10 @@
         exit(2)
 
     result = tc.setTransformationParameter( transID['Value'], 'Status', 'Flush' )
     if not result['OK']:
         gLogger.error('Can not flush transformation: %s' % result['Message'])
         exit(2)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_metadata.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/TransformationSystem/scripts/ihepdirac_transformation_transfer_metadata.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/SAMHistoryHandler.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/SAMHistoryHandler.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/SiteStatusMonitorHandler.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/SiteStatusMonitorHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json, math
 from DIRAC                      import S_OK
-from WebAppDIRAC.Lib.WebHandler import WebHandler, WErr, WOK, asyncGen
+from WebAppDIRAC.Lib.WebHandler import WebHandler, WErr, asyncGen
 from DIRAC.Core.DISET.RPCClient import RPCClient
 from DIRAC.Interfaces.API.DiracAdmin import DiracAdmin
 
 
 class SiteStatusMonitorHandler( WebHandler ):
 
   AUTH_PROPS = "authenticated"
@@ -99,15 +99,15 @@
 
     if not sitesDict:
       self.finish( { 'success' : 'false', 'result' : [], 'total' : 0, 'error' : 'There are no data to display' } )
       return
 
     summarys = []
 
-    samSummary = yield self.threadTask( publisher.getSitesSAMSummary, sitesDict.keys(), selectedVOs )
+    samSummary = yield self.threadTask( publisher.getSitesSAMSummary, list(sitesDict.keys()), selectedVOs )
     if not samSummary[ 'OK' ]:
       self.finish( { 'success' : 'false', 'result' : [], 'total' : 0, 'error' : samSummary[ 'Message' ] } )
       return 
     summarys.append( samSummary[ 'Value' ] )
 
     storageSummary = yield self.threadTask( publisher.getSitesStorageSummary, sitesDict.keys() )
     if not storageSummary[ 'OK' ]:
@@ -223,15 +223,15 @@
                     'Failed' : totalFailed,
                     'Efficiency' : efficiency })
 
     self.finish( { 'success' : 'ture', 'result' : wnsInfo, 'total' : len( wnsInfo ) } )
 
 
   def __siteFilte( self, sitesDict, selectedSites = None, selectedType = None, selectedMask = None, selectedVOs = None ):
-    for siteName, siteDict in sitesDict.items():
+    for siteName, siteDict in list(sitesDict.items()):
 
       if selectedSites is not None and siteName not in selectedSites:
         del sitesDict[ siteName ]
         continue
 
       siteType = siteDict[ 'SiteType' ]
       if selectedType is not None and siteType not in selectedType:
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/handler/TaskManagerHandler.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/handler/TaskManagerHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import json
 
-from WebAppDIRAC.Lib.WebHandler import WebHandler, WErr, WOK, asyncGen
+from WebAppDIRAC.Lib.WebHandler import WebHandler, WErr, asyncGen
 from DIRAC import gConfig, S_OK, S_ERROR, gLogger
 from DIRAC.Core.DISET.RPCClient import RPCClient
 from IHEPDIRAC.WorkloadManagementSystem.Client.TaskClient import TaskClient
 
 STATUS_ICON_MAP = {
   'Init' : 'Checking',
   'Ready' : 'Waiting',
@@ -379,23 +379,23 @@
       if "ownerGroup" in self.request.arguments:
         ownerGroup = list( json.loads( self.request.arguments[ 'ownerGroup' ][-1] ) )
         if len( ownerGroup ) > 0:
           req["OwnerGroup"] = ownerGroup
           
       if 'startDate' in self.request.arguments and len( self.request.arguments["startDate"][0] ) > 0:
         if 'startTime' in self.request.arguments and len( self.request.arguments["startTime"][0] ) > 0:
-          req["FromDate"] = str( self.request.arguments["startDate"][0] + " " + self.request.arguments["startTime"][0] )
+          req["FromDate"] = str( self.request.arguments["startDate"][0] + b" " + self.request.arguments["startTime"][0], "utf-8")
         else:
-          req["FromDate"] = str( self.request.arguments["startDate"][0] )
+          req["FromDate"] = str( self.request.arguments["startDate"][0],"utf-8" )
 
       if 'endDate' in self.request.arguments and len( self.request.arguments["endDate"][0] ) > 0:
         if 'endTime' in self.request.arguments and len( self.request.arguments["endTime"][0] ) > 0:
-          req["ToDate"] = str( self.request.arguments["endDate"][0] + " " + self.request.arguments["endTime"][0] )
+          req["ToDate"] = str( self.request.arguments["endDate"][0] + b" " + self.request.arguments["endTime"][0],"utf-8" )
         else:
-          req["ToDate"] = str( self.request.arguments["endDate"][0] )
+          req["ToDate"] = str( self.request.arguments["endDate"][0],"utf-8" )
 
       if 'date' in self.request.arguments and len( self.request.arguments["date"][0] ) > 0:
         req["LastUpdate"] = str( self.request.arguments["date"][0] )
 
       if 'sort' in self.request.arguments:
         sort = json.loads( self.request.arguments['sort'][-1] )
         if len( sort ) > 0:
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/classes/SAMHistory.js` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SAMHistory/classes/SAMHistory.js`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/classes/SiteStatusMonitor.js` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/SiteStatusMonitor/classes/SiteStatusMonitor.js`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/classes/TaskManager.js` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WebApp/static/IHEPDIRAC/TaskManager/classes/TaskManager.js`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Agent/TaskAgent.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Agent/TaskAgent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __RCSID__ = "8f34a5d (2015-01-12 13:07:33 +0000) Xianghu Zhao <zhaoxh@ihep.ac.cn>"
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
+#from __future__ import absolute_import
+#from __future__ import division
+#from __future__ import print_function
 
 from DIRAC                                            import S_OK, S_ERROR
 from DIRAC.Core.Base.AgentModule                      import AgentModule
 from DIRAC.Core.DISET.RPCClient                       import RPCClient
 
 from DIRAC.WorkloadManagementSystem.DB.JobDB          import JobDB
 from IHEPDIRAC.WorkloadManagementSystem.DB.TaskDB      import TaskDB
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Client/TaskClient.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Client/TaskClient.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,18 @@
     if 'FromDate' in condDict:
       newer = condDict['FromDate']
       del condDict['FromDate']
     older = None
     if 'ToDate' in condDict:
       older = condDict['ToDate']
       del condDict['ToDate']
-
+    
+    print('conDict++++++++++++++++++++++++++', condDict) 
+    print('newer++++++++++++++++++++++++++', newer) 
+    print('older++++++++++++++++++++++++++', older) 
     result = self.getCounters( 'Task', ['Status'], condDict, newer = newer, older = older, timeStamp = 'UpdateTime' )
     if not result['OK']:
       self.log.error( 'Can not get task count', result['Message'] )
       return result
 
     nTasks = 0
     for stDict, count in result['Value']:
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/Service/TaskManagerHandler.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/Service/root@samtest.ihep.ac.cn`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from types import DictType, FloatType, IntType, ListType, LongType, StringTypes, TupleType, UnicodeType
+#from types import FloatType, type(int), type(list), type(int), type(str), TupleType, UnicodeType
 
 import time
 import json
 
 # DIRAC
 from DIRAC                                import gConfig, gLogger, S_ERROR, S_OK
 from DIRAC.Core.DISET.RequestHandler      import RequestHandler, getServiceOption
@@ -37,15 +37,15 @@
     self.ownerGroup     = credDict[ 'group' ]
     self.userProperties = credDict[ 'properties' ]
 
 
 ################################################################################
 # exported interfaces
 
-  types_createTask = [ StringTypes, DictType ]
+  types_createTask = [ type(str), type(dict) ]
   def export_createTask( self, taskName, taskInfo, jobInfos ):
     """ Create a new task
     """
     if Properties.NORMAL_USER not in self.userProperties and Properties.JOB_ADMINISTRATOR not in self.userProperties:
       return S_ERROR( 'Access denied to create task' )
 
     jobIDs = self.__filterJobAccess( jobInfos.keys() )
@@ -68,15 +68,15 @@
 
     result = gTaskDB.updateTaskStatus( taskID, 'Ready', 'Task is ready for processing' )
     if not result['OK']:
       return result
 
     return S_OK( taskID )
 
-#  types_activateTask = [ [IntType, LongType] ]
+#  types_activateTask = [ [type(int), type(int)] ]
 #  def export_activateTask( self, taskID ):
 #    """ Activate the task
 #    """
 #    if not self.__hasTaskAccess( taskID ):
 #      return S_ERROR( 'Access denied to activate task %s' % taskID )
 #
 #    result = gTaskDB.getTaskStatus( taskID )
@@ -86,24 +86,24 @@
 #
 #    if status != 'Init':
 #      self.log.error( 'Can only activate task with "Init" status: task %s' % taskID )
 #      return S_ERROR( 'Can only activate task with "Init" status: task %s' % taskID )
 #
 #    return gTaskDB.updateTaskStatus( taskID, 'Ready', 'Task is activated' )
 
-  types_removeTask = [ [IntType, LongType] ]
+  types_removeTask = [ [type(int), type(int)] ]
   def export_removeTask( self, taskID ):
     """ Delete the task
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to remove task %s' % taskID )
 
     return gTaskDB.updateTaskStatus( taskID, 'Removed', 'Task is removed' )
 
-#  types_addTaskJob = [ [IntType, LongType], [IntType, LongType], DictType ]
+#  types_addTaskJob = [ [type(Int), type(Long)], [type(int), type(int)], type(dict) ]
 #  def export_addTaskJob( self, taskID, jobID, jobInfo ):
 #    """ Add a job to the task
 #    """
 #    if not self.__hasTaskAccess( taskID ):
 #      return S_ERROR( 'Access denied for task %s: Can not add job %s to task' % ( taskID, jobID ) )
 #    if not self.__hasJobAccess( jobID ):
 #      return S_ERROR( 'Access denied for job %s: Can not add job to task %s' % ( jobID, taskID ) )
@@ -115,15 +115,15 @@
 #
 #    if status != 'Init':
 #      self.log.error( 'Can only add job to "Init" status: task %s' % taskID )
 #      return S_ERROR( 'Can only add job to "Init" status: task %s' % taskID )
 #
 #    return gTaskDB.addTaskJob( taskID, jobID, jobInfo )
 #
-#  types_updateTaskInfo = [ [IntType, LongType], DictType ]
+#  types_updateTaskInfo = [ [type(int), type(int)], type(dict) ]
 #  def export_updateTaskInfo( self, taskID, taskInfo ):
 #    """ Update the task info
 #    """
 #    if not self.__hasTaskAccess( taskID ):
 #      return S_ERROR( 'Access denied to update task info for task %s' % taskID )
 #
 #    result = gTaskDB.getTaskInfo( taskID )
@@ -131,15 +131,15 @@
 #      return result
 #
 #    newTaskInfo = result['Value']
 #    newTaskInfo.update( taskInfo )
 #
 #    return gTaskDB.updateTaskInfo( taskID, newTaskInfo )
 
-  types_renameTask = [ [IntType, LongType], StringTypes ]
+  types_renameTask = [ [type(int), type(int)], type(str) ]
   def export_renameTask( self, taskID, newName ):
     """ Rename the task
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to rename task %s' % taskID )
 
     return gTaskDB.renameTask( taskID, newName )
@@ -154,15 +154,15 @@
 
   types_getTaskOwnerGroups = []
   def export_getTaskOwnerGroups( self ):
     """ Return Distinct Values of OwnerGroup
     """
     return gTaskDB.getDistinctTaskAttributes( 'OwnerGroup' )
 
-  types_getTaskCount = [ DictType ]
+  types_getTaskCount = [ type(dict) ]
   def export_getTaskCount( self, condDict ):
     """ Get task count
     """
     if Properties.NORMAL_USER not in self.userProperties and Properties.JOB_ADMINISTRATOR not in self.userProperties:
       return S_ERROR( 'Access denied to get task count' )
 
     if Properties.NORMAL_USER in self.userProperties:
@@ -173,15 +173,15 @@
         condDict['Status'] = [ 'Init', 'Ready', 'Processing', 'Finished', 'Expired' ]
       else:
         condDict['Status'] = list( condDict['Status'] )
         condDict['Status'] = [ v for v in condDict['Status'] if v != 'Removed' ]
 
     return gTaskDB.getTaskCount( condDict )
 
-  types_getTasks = [ DictType, [IntType, LongType], [IntType, LongType], StringTypes, [IntType, LongType] ]
+  types_getTasks = [ type(dict), [type(int), type(int)], [type(int), type(int)], type(str), [type(int), type(int)] ]
   def export_getTasks( self, condDict, limit, offset, orderAttribute, realTimeProgress ):
     """ Get task list
     """
     if Properties.NORMAL_USER not in self.userProperties and Properties.JOB_ADMINISTRATOR not in self.userProperties:
       return S_ERROR( 'Access denied to get tasks' )
 
     if Properties.NORMAL_USER in self.userProperties:
@@ -211,15 +211,15 @@
           self.log.error( result['Message'] )
           return result
         progress = result['Value']
       tasks.append( self.__generateTaskResult( outFields, outValues, progress ) )
 
     return S_OK( tasks )
 
-  types_getTask = [ [IntType, LongType], [IntType, LongType] ]
+  types_getTask = [ [type(int), type(int)], [type(int), type(int)] ]
   def export_getTask( self, taskID, realTimeProgress ):
     """ Get task
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to get task for task %s' % taskID )
 
     outFields = ['TaskID', 'TaskName', 'Status', 'Owner', 'OwnerDN', 'OwnerGroup', 'CreationTime', 'UpdateTime', 'JobGroup', 'Site', 'Info']
@@ -236,33 +236,33 @@
       result = self.__getTaskProgress( taskID )
       if not result['OK']:
         self.log.error( result['Message'] )
         return result
       progress = result['Value']
     return S_OK( self.__generateTaskResult( outFields, outValues, progress ) )
 
-  types_getTaskStatus = [ [IntType, LongType] ]
+  types_getTaskStatus = [ [type(int), type(int)] ]
   def export_getTaskStatus( self, taskID ):
     """ Get task status
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to get task status for task %s' % taskID )
 
     return gTaskDB.getTaskStatus( taskID )
 
-  types_getTaskInfo = [ [IntType, LongType] ]
+  types_getTaskInfo = [ [type(int), type(int)] ]
   def export_getTaskInfo( self, taskID ):
     """ Get task info
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to get task info for task %s' % taskID )
 
     return gTaskDB.getTaskInfo( taskID )
 
-  types_getTaskProgress = [ [IntType, LongType] ]
+  types_getTaskProgress = [ [type(int), type(int)] ]
   def export_getTaskProgress( self, taskID ):
     """ Get task progress
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to get task progress for task %s' % taskID )
 
     result = self.__getTaskProgress( taskID )
@@ -271,61 +271,61 @@
     progress = result['Value']
     self.log.debug( 'Task %d Progress: %s' % ( taskID, progress ) )
     result = gTaskDB.updateTaskProgress( taskID, progress )
     if not result['OK']:
       return result
     return S_OK( progress )
 
-  types_getTaskHistories = [ [IntType, LongType] ]
+  types_getTaskHistories = [ [type(int), type(int)] ]
   def export_getTaskHistories( self, taskID ):
     """ Get task histories
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to get task histories for task %s' % taskID )
 
     return gTaskDB.getTaskHistories( taskID )
 
-  types_getTaskJobs = [ [IntType, LongType] ]
+  types_getTaskJobs = [ [type(int), type(int)] ]
   def export_getTaskJobs( self, taskID ):
     """ Get task jobs
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to get task jobs for task %s' % taskID )
 
     return gTaskDB.getTaskJobs( taskID )
 
-  types_getJobs = [ ListType, ListType ]
+  types_getJobs = [ type(list), type(list) ]
   def export_getJobs( self, jobIDs, outFields ):
     """ Get jobs
     """
     jobIDs = self.__filterJobOfTaskAccess( jobIDs )
 
     return gTaskDB.getJobs( jobIDs, outFields )
 
-  types_getTaskIDFromJob = [ [IntType, LongType] ]
+  types_getTaskIDFromJob = [ [type(int), type(int)] ]
   def export_getTaskIDFromJob( self, jobID ):
     """ Get task ID from job ID
     """
     result = gTaskDB.getTaskIDFromJob( jobID )
     if not result['OK']:
       return result
 
     return S_OK( self.__filterTaskAccess( result['Value'] ) )
 
-  types_getJobInfo = [ [IntType, LongType] ]
+  types_getJobInfo = [ [type(int), type(int)] ]
   def export_getJobInfo( self, jobID ):
     """ Get job info
     """
     if not self.__hasJobForTaskAccess( jobID ):
       return S_ERROR( 'Access denied to get job info for job %s' % jobID )
 
     return gTaskDB.getJobInfo( jobID )
 
 
-  types_getTaskJobsStatistics = [ [IntType, LongType], StringTypes ]
+  types_getTaskJobsStatistics = [ [type(int), type(int)], type(str) ]
   def export_getTaskJobsStatistics( self, taskID, statusType ):
     """ Get statistics of all jobs in the task
     """
     if not self.__hasTaskAccess( taskID ):
       return S_ERROR( 'Access denied to get task jobs %s statistics for task %s' % ( statusType, taskID ) )
 
     return self.__getTaskStatusCount( taskID, statusType )
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-delete.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-delete.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-event-progress.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-event-progress.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-job-show.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-job-show.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-list.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-list.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-reschedule.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-reschedule.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-show.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-show.py`

 * *Files identical despite different names*

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC/__init__.py` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def extension_metadata():
   import importlib.resources  # pylint: disable=import-error,no-name-in-module
   return {
       "primary_extension": True,
       "priority": 100,
       "setups": {
-          "CAS_Production": "dips://dirac.ihep.ac.cn:9135/Configuration/Server",
-          "CAS_Production-cert": "dips://dirac.ihep.ac.cn:9135/Configuration/Server",
+          "CAS_Production": "dips://prod-dirac.ihep.ac.cn:9135/Configuration/Server",
+          "CAS_Production-cert": "dips://prod-dirac.ihep.ac.cn:9135/Configuration/Server",
       },
       "default_setup": "CAS_Production",
       "web_resources": {
           "static": [importlib.resources.files("IHEPDIRAC") / "WebApp" / "static"],  # pylint: disable=no-member
       },
   }
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/SOURCES.txt` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_register_files.py
 src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir.py
 src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_rm_dir_replicas.py
 src/IHEPDIRAC/DataManagementSystem/scripts/ihepdirac_dms_scan_unregistered.py
 src/IHEPDIRAC/ResourceStatusSystem/ConfigTemplate.cfg
 src/IHEPDIRAC/ResourceStatusSystem/__init__.py
 src/IHEPDIRAC/ResourceStatusSystem/Agent/CacheFeederIHEPAgent.py
-src/IHEPDIRAC/ResourceStatusSystem/Agent/CacheFeederIHEPAgent.py.bak
 src/IHEPDIRAC/ResourceStatusSystem/Agent/SAMTestAgent.py
 src/IHEPDIRAC/ResourceStatusSystem/Agent/__init__.py
 src/IHEPDIRAC/ResourceStatusSystem/Client/ResourceManagementIHEPClient.py
 src/IHEPDIRAC/ResourceStatusSystem/Client/__init__.py
 src/IHEPDIRAC/ResourceStatusSystem/Command/HostCommand.py
 src/IHEPDIRAC/ResourceStatusSystem/Command/JobIHEPCommand.py
 src/IHEPDIRAC/ResourceStatusSystem/Command/SAMIHEPCommand.py
@@ -115,14 +114,15 @@
 src/IHEPDIRAC/WorkloadManagementSystem/Client/TaskClient.py
 src/IHEPDIRAC/WorkloadManagementSystem/Client/__init__.py
 src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.py
 src/IHEPDIRAC/WorkloadManagementSystem/DB/TaskDB.sql
 src/IHEPDIRAC/WorkloadManagementSystem/DB/__init__.py
 src/IHEPDIRAC/WorkloadManagementSystem/Service/TaskManagerHandler.py
 src/IHEPDIRAC/WorkloadManagementSystem/Service/__init__.py
+src/IHEPDIRAC/WorkloadManagementSystem/Service/root@samtest.ihep.ac.cn
 src/IHEPDIRAC/WorkloadManagementSystem/scripts/__init__.py
 src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-delete.py
 src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-event-progress.py
 src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-job-show.py
 src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-list.py
 src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-reschedule.py
 src/IHEPDIRAC/WorkloadManagementSystem/scripts/besdirac-wms-task-show.py
```

### Comparing `IHEPDIRAC-2.2.3/src/IHEPDIRAC.egg-info/entry_points.txt` & `IHEPDIRAC-2.2.5/src/IHEPDIRAC.egg-info/entry_points.txt`

 * *Files identical despite different names*

