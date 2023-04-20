# Comparing `tmp/cloudshell-networking-cisco-iosxr-4.0.6.zip` & `tmp/cloudshell-networking-cisco-iosxr-5.0.0.zip`

## zipinfo {}

```diff
@@ -1,49 +1,56 @@
-Zip file size: 29598 bytes, number of entries: 47
--rw-rw-rw-  2.0 fat      595 b- defN 17-Oct-13 13:06 cloudshell-networking-cisco-iosxr-4.0.6/dev_requirements.txt
--rw-rw-rw-  2.0 fat       35 b- defN 17-Feb-22 17:14 cloudshell-networking-cisco-iosxr-4.0.6/MANIFEST.in
--rw-rw-rw-  2.0 fat      337 b- defN 18-Nov-08 13:25 cloudshell-networking-cisco-iosxr-4.0.6/PKG-INFO
--rw-rw-rw-  2.0 fat       75 b- defN 16-Sep-01 12:43 cloudshell-networking-cisco-iosxr-4.0.6/README.txt
--rw-rw-rw-  2.0 fat       41 b- defN 18-Jan-10 17:03 cloudshell-networking-cisco-iosxr-4.0.6/requirements.txt
--rw-rw-rw-  2.0 fat       42 b- defN 18-Nov-08 13:25 cloudshell-networking-cisco-iosxr-4.0.6/setup.cfg
--rw-rw-rw-  2.0 fat      777 b- defN 17-Feb-22 17:20 cloudshell-networking-cisco-iosxr-4.0.6/setup.py
--rw-rw-rw-  2.0 fat        9 b- defN 17-Feb-22 17:14 cloudshell-networking-cisco-iosxr-4.0.6/test_requirements.txt
--rw-rw-rw-  2.0 fat        5 b- defN 18-Nov-08 13:24 cloudshell-networking-cisco-iosxr-4.0.6/version.txt
--rw-rw-rw-  2.0 fat       75 b- defN 17-Feb-22 17:14 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/__init__.py
--rw-rw-rw-  2.0 fat       75 b- defN 17-Feb-22 17:14 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/__init__.py
--rw-rw-rw-  2.0 fat       75 b- defN 17-Feb-22 17:14 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/__init__.py
--rw-rw-rw-  2.0 fat       79 b- defN 16-Sep-01 12:43 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/__init__.py
--rw-rw-rw-  2.0 fat     1254 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/cli/cisco_iosxr_cli_handler.py
--rw-rw-rw-  2.0 fat     2377 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/cli/cisco_iosxr_command_modes.py
--rw-rw-rw-  2.0 fat       77 b- defN 17-Feb-22 13:27 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/cli/__init__.py
--rw-rw-rw-  2.0 fat     3037 b- defN 17-May-10 18:36 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/cisco_iosxr_add_remove_vlan_actions.py
--rw-rw-rw-  2.0 fat     2635 b- defN 17-May-10 16:17 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/cisco_iosxr_iface_actions.py
--rw-rw-rw-  2.0 fat     7094 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/cisco_iosxr_system_actions.py
--rw-rw-rw-  2.0 fat       77 b- defN 17-May-10 18:00 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/__init__.py
--rw-rw-rw-  2.0 fat     4080 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_templates/cisco_ios_xr_cmd_templates.py
--rw-rw-rw-  2.0 fat       77 b- defN 17-Jan-13 18:23 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_templates/__init__.py
--rw-rw-rw-  2.0 fat     2623 b- defN 17-May-10 18:51 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_add_vlan_flow.py
--rw-rw-rw-  2.0 fat     9333 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_load_firmware_flow.py
--rw-rw-rw-  2.0 fat     2166 b- defN 17-May-10 18:31 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_remove_vlan_flow.py
--rw-rw-rw-  2.0 fat     2180 b- defN 17-May-26 15:05 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_restore_flow.py
--rw-rw-rw-  2.0 fat       77 b- defN 17-Jan-13 18:23 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/__init__.py
--rw-rw-rw-  2.0 fat      476 b- defN 17-Dec-26 10:41 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/cisco_iosxr_configuration_runner.py
--rw-rw-rw-  2.0 fat      657 b- defN 17-Dec-26 10:44 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/cisco_iosxr_connectivity_runner.py
--rw-rw-rw-  2.0 fat     1695 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/cisco_iosxr_firmware_runner.py
--rw-rw-rw-  2.0 fat       77 b- defN 17-Jan-13 18:23 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 18-Nov-08 13:25 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat      337 b- defN 18-Nov-08 13:25 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       38 b- defN 18-Nov-08 13:25 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/requires.txt
--rw-rw-rw-  2.0 fat     2364 b- defN 18-Nov-08 13:25 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat       17 b- defN 18-Nov-08 13:25 cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/top_level.txt
--rw-rw-rw-  2.0 fat       77 b- defN 17-May-24 13:34 cloudshell-networking-cisco-iosxr-4.0.6/tests/__init__.py
--rw-rw-rw-  2.0 fat       75 b- defN 17-Apr-05 15:26 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/__init__.py
--rw-rw-rw-  2.0 fat       75 b- defN 17-Apr-05 15:26 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/__init__.py
--rw-rw-rw-  2.0 fat       75 b- defN 17-May-26 14:54 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/__init__.py
--rw-rw-rw-  2.0 fat     5794 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_actions/test_iosxr_system_admin_actions.py
--rw-rw-rw-  2.0 fat        0 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_actions/__init__.py
--rw-rw-rw-  2.0 fat     3830 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_templates/test_iosxr_cmd_templates.py
--rw-rw-rw-  2.0 fat        0 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_templates/__init__.py
--rw-rw-rw-  2.0 fat    17198 b- defN 18-Nov-07 16:24 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/flows/test_iosxr_load_firmware_flow.py
--rw-rw-rw-  2.0 fat     4575 b- defN 17-May-26 15:57 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/flows/test_restore_configuration_flow.py
--rw-rw-rw-  2.0 fat       75 b- defN 17-May-26 14:54 cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/flows/__init__.py
-47 files, 76743 bytes uncompressed, 17570 bytes compressed:  77.1%
+Zip file size: 24494 bytes, number of entries: 54
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/
+-rw-r--r--  2.0 unx      297 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/PKG-INFO
+-rw-r--r--  2.0 unx     1078 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tox.ini
+-rw-r--r--  2.0 unx     1303 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/setup.py
+-rw-r--r--  2.0 unx       45 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/dev_requirements.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/setup.cfg
+-rw-r--r--  2.0 unx     2387 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/README.md
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/version.txt
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx      117 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/requirements.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/test_requirements.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_templates/
+-rw-r--r--  2.0 unx       33 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/constants.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/__init__.py
+-rw-r--r--  2.0 unx     9892 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/firmware.py
+-rw-r--r--  2.0 unx     2482 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/configuration.py
+-rw-r--r--  2.0 unx     3166 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/connectivity.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/__init__.py
+-rw-r--r--  2.0 unx     6851 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/system.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/__init__.py
+-rw-r--r--  2.0 unx     2038 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/add_remove_vlan.py
+-rw-r--r--  2.0 unx     1169 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/iface.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/__init__.py
+-rw-r--r--  2.0 unx     1398 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/handler.py
+-rw-r--r--  2.0 unx     1923 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/command_modes.py
+-rw-r--r--  2.0 unx     3894 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_templates/system.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_templates/__init__.py
+-rw-r--r--  2.0 unx      118 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/requires.txt
+-rw-r--r--  2.0 unx      297 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1574 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/SOURCES.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/iosxr/
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/iosxr/__init__.py
+-rw-r--r--  2.0 unx      117 b- defN 23-Apr-20 23:15 cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/iosxr/test_constants.py
+54 files, 41293 bytes uncompressed, 12052 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -1,142 +1,163 @@
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/dev_requirements.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/MANIFEST.in
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/PKG-INFO
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/README.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/requirements.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/setup.cfg
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tox.ini
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/setup.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/setup.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/test_requirements.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/version.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/README.md
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/version.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/cli/cisco_iosxr_cli_handler.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/cli/cisco_iosxr_command_modes.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/cli/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/cisco_iosxr_add_remove_vlan_actions.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/cisco_iosxr_iface_actions.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/cisco_iosxr_system_actions.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_templates/cisco_ios_xr_cmd_templates.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_templates/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_add_vlan_flow.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_load_firmware_flow.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_templates/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_remove_vlan_flow.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/constants.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_restore_flow.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/firmware.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/cisco_iosxr_configuration_runner.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/configuration.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/cisco_iosxr_connectivity_runner.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/connectivity.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/cisco_iosxr_firmware_runner.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/runners/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/system.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/dependency_links.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/PKG-INFO
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/add_remove_vlan.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/requires.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/iface.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/SOURCES.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/cloudshell_networking_cisco_iosxr.egg-info/top_level.txt
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/handler.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/command_modes.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_templates/system.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_templates/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_actions/test_iosxr_system_admin_actions.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_actions/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_templates/test_iosxr_cmd_templates.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/command_templates/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/cloudshell_networking_cisco_iosxr.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/flows/test_iosxr_load_firmware_flow.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/flows/test_restore_configuration_flow.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-networking-cisco-iosxr-4.0.6/tests/networking/cisco/iosxr/flows/__init__.py
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/
+Comment: 
+
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/__init__.py
+Comment: 
+
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/
+Comment: 
+
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/__init__.py
+Comment: 
+
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/iosxr/
+Comment: 
+
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/__init__.py
+Comment: 
+
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/iosxr/__init__.py
+Comment: 
+
+Filename: cloudshell-networking-cisco-iosxr-5.0.0/tests/cloudshell/networking/cisco/iosxr/test_constants.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/cli/cisco_iosxr_cli_handler.py` & `cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/cli/handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-from cloudshell.cli.cli_service_impl import CliServiceImpl
-
-from cloudshell.networking.cisco.cli.cisco_cli_handler import CiscoCliHandler
-from cloudshell.networking.cisco.cli.cisco_command_modes import EnableCommandMode, ConfigCommandMode
-from cloudshell.networking.cisco.iosxr.cli.cisco_iosxr_command_modes import CiscoIOSXRConfigCommandMode, \
-    CiscoIOSXRAdminCommandMode
-
-
-class CiscoIOSXRCliHandler(CiscoCliHandler):
-    @property
-    def config_mode(self):
-        return self.modes[CiscoIOSXRConfigCommandMode]
-
-    @property
-    def admin_mode(self):
-        return self.modes[CiscoIOSXRAdminCommandMode]
-
-    def on_session_start(self, session, logger):
-        """Send default commands to configure/clear session outputs
-        :return:
-        """
-
-        cli_service = CliServiceImpl(session=session, command_mode=self.enable_mode, logger=logger)
-        cli_service.send_command("terminal length 0", EnableCommandMode.PROMPT)
-        cli_service.send_command("terminal width 300", EnableCommandMode.PROMPT)
-        with cli_service.enter_mode(self.config_mode) as config_session:
-            config_session.send_command("no logging console", ConfigCommandMode.PROMPT)
+from cloudshell.cli.service.cli_service_impl import CliServiceImpl
+from cloudshell.networking.cisco.cli.cisco_cli_handler import CiscoCli, CiscoCliHandler
+from cloudshell.networking.cisco.cli.cisco_command_modes import EnableCommandMode
+
+from cloudshell.networking.cisco.iosxr.cli.command_modes import (
+    CiscoIOSXRAdminCommandMode,
+    CiscoIOSXRConfigCommandMode,
+)
+
+
+class CiscoIOSXRCli(CiscoCli):
+    def get_cli_handler(self, resource_config, logger):
+        return CiscoIOSXRCliHandler.from_config(resource_config, logger, self.cli)
+
+
+class CiscoIOSXRCliHandler(CiscoCliHandler):
+    @property
+    def config_mode(self):
+        return self.modes[CiscoIOSXRConfigCommandMode]
+
+    @property
+    def admin_mode(self):
+        return self.modes[CiscoIOSXRAdminCommandMode]
+
+    def _on_session_start(self, session, logger):
+        """Send default commands to configure/clear session outputs."""
+        cli_service = CliServiceImpl(
+            session=session, requested_command_mode=self.enable_mode, logger=logger
+        )
+        cli_service.send_command("terminal length 0", EnableCommandMode.PROMPT)
+        cli_service.send_command("terminal width 300", EnableCommandMode.PROMPT)
+        with cli_service.enter_mode(self.config_mode) as config_session:
+            config_session.send_command(
+                "no logging console", CiscoIOSXRConfigCommandMode.PROMPT
+            )
```

## Comparing `cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/command_actions/cisco_iosxr_add_remove_vlan_actions.py` & `cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/command_actions/add_remove_vlan.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,60 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
-import re
-
-from cloudshell.cli.cli_service import CliService
-from cloudshell.cli.command_template.command_template_executor import CommandTemplateExecutor
-from cloudshell.networking.cisco.command_actions.add_remove_vlan_actions import AddRemoveVlanActions
-from cloudshell.networking.cisco.command_templates import add_remove_vlan as vlan_command_template
-from cloudshell.networking.cisco.command_templates import iface as iface_command_template
-
-
-class CiscoIOSXRAddRemoveVlanActions(AddRemoveVlanActions):
-    def __init__(self, cli_service, logger):
-        """ Add remove vlan
-
-        :param cli_service: config mode cli_service
-        :type cli_service: CliService
-        :param logger:
-        :type logger: Logger
-        :return:
-        """
-
-        super(CiscoIOSXRAddRemoveVlanActions, self).__init__(cli_service, logger)
-        self._cli_service = cli_service
-        self._logger = logger
-
-    def set_vlan_to_interface(self, vlan_range, port_mode, port_name, qnq, c_tag,
-                              action_map=None,
-                              error_map=None):
-
-        """Assign vlan to a certain interface
-
-        :param vlan_range: range of vlans to be assigned
-        :param port_mode: switchport mode
-        :param port_name: interface name
-        :param qnq: qinq settings (dot1q tunnel)
-        :param c_tag: selective qnq
-        :param action_map: actions will be taken during executing commands, i.e. handles yes/no prompts
-        :param error_map: errors will be raised during executing commands, i.e. handles Invalid Commands errors
-        """
-
-        CommandTemplateExecutor(self._cli_service,
-                                iface_command_template.CONFIGURE_INTERFACE).execute_command(port_name=port_name,
-                                                                                            l2transport="")
-
-        CommandTemplateExecutor(self._cli_service,
-                                iface_command_template.NO_SHUTDOWN,
-                                action_map=action_map,
-                                error_map=error_map).execute_command()
-
-        if qnq:
-            CommandTemplateExecutor(self._cli_service,
-                                    vlan_command_template.VLAN_SUB_IFACE,
-                                    action_map=action_map,
-                                    error_map=error_map).execute_command(vlan_id=vlan_range, qnq="")
-        else:
-            CommandTemplateExecutor(self._cli_service,
-                                    vlan_command_template.VLAN_SUB_IFACE,
-                                    action_map=action_map,
-                                    error_map=error_map).execute_command(vlan_id=vlan_range, untagged="")
-
-    def clean_vlan_sub_interface(self, port_name):
-        CommandTemplateExecutor(self._cli_service,
-                                iface_command_template.REMOVE_INTERFACE).execute_command(port_name=port_name)
+from cloudshell.cli.command_template.command_template_executor import (
+    CommandTemplateExecutor,
+)
+from cloudshell.networking.cisco.command_actions.add_remove_vlan_actions import (
+    AddRemoveVlanActions,
+)
+from cloudshell.networking.cisco.command_templates import (
+    add_remove_vlan as vlan_command_template,
+)
+from cloudshell.networking.cisco.command_templates import (
+    iface as iface_command_template,
+)
+
+
+class CiscoIOSXRAddRemoveVlanActions(AddRemoveVlanActions):
+    def set_vlan_to_interface(
+        self,
+        vlan_range,
+        port_mode,
+        port_name,
+        qnq,
+        c_tag,
+        action_map=None,
+        error_map=None,
+    ):
+        """Assign VLAM to a certain interface.
+
+        :param vlan_range: range of vlans to be assigned
+        :param port_mode: switchport mode
+        :param port_name: interface name
+        :param qnq: qinq settings (dot1q tunnel)
+        :param c_tag: selective qnq
+        :param action_map: actions will be taken during executing commands
+        :param error_map: errors will be raised during executing commands
+        """
+        CommandTemplateExecutor(
+            self._cli_service, iface_command_template.CONFIGURE_INTERFACE
+        ).execute_command(port_name=port_name, l2transport="")
+
+        CommandTemplateExecutor(
+            self._cli_service,
+            iface_command_template.NO_SHUTDOWN,
+            action_map=action_map,
+            error_map=error_map,
+        ).execute_command()
+
+        if qnq:
+            CommandTemplateExecutor(
+                self._cli_service,
+                vlan_command_template.VLAN_SUB_IFACE,
+                action_map=action_map,
+                error_map=error_map,
+            ).execute_command(vlan_id=vlan_range, qnq="")
+        else:
+            CommandTemplateExecutor(
+                self._cli_service,
+                vlan_command_template.VLAN_SUB_IFACE,
+                action_map=action_map,
+                error_map=error_map,
+            ).execute_command(vlan_id=vlan_range, untagged="")
```

## Comparing `cloudshell-networking-cisco-iosxr-4.0.6/cloudshell/networking/cisco/iosxr/flows/cisco_iosxr_load_firmware_flow.py` & `cloudshell-networking-cisco-iosxr-5.0.0/cloudshell/networking/cisco/iosxr/flows/firmware.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,246 @@
-#!/usr/bin/python
-# -*- coding: utf-8 -*-
-
-import re
-
-from cloudshell.devices.networking_utils import UrlParser
-from cloudshell.networking.cisco.flows.cisco_load_firmware_flow import CiscoLoadFirmwareFlow
-from cloudshell.networking.cisco.iosxr.command_actions.cisco_iosxr_system_actions import CiscoIOSXRAdminSystemActions
-
-
-class CiscoIOSXRLoadFirmwareFlow(CiscoLoadFirmwareFlow):
-    def __init__(self, cli_handler, logger, packages_to_install):
-        super(CiscoIOSXRLoadFirmwareFlow, self).__init__(cli_handler, logger)
-        self._packages_to_add = []
-        self._result_dict = {}
-        self._sync = None
-        self._is_old_iosxr = False
-        self._cmd_admin_prefix = None
-        if not packages_to_install or packages_to_install == "*" or packages_to_install.lower() == "all":
-            self._packages_to_add = []
-        else:
-            self._packages_to_add = packages_to_install.lower().split(" ")
-
-    def execute_flow(self, path, vrf, timeout):
-        """Load a firmware onto the device
-
-        :param path: The path to the firmware file, including the firmware file name
-        :param vrf: Virtual Routing and Forwarding Name
-        :param timeout:
-        :return:
-        """
-
-        success = False
-
-        full_path_dict = UrlParser().parse_url(path)
-        firmware_file_name = full_path_dict.get(UrlParser.FILENAME)
-        password = full_path_dict.get(UrlParser.PASSWORD)
-        remote_path = path.replace("{}".format(firmware_file_name), "").rstrip("/")
-        if vrf and vrf not in remote_path:
-            remote_path = remote_path.replace("{}".format(full_path_dict.get(UrlParser.HOSTNAME)),
-                                              "{};{}".format(full_path_dict.get(UrlParser.HOSTNAME), vrf))
-
-        with self._cli_handler.get_cli_service(self._cli_handler.enable_mode) as enable_session:
-            admin_actions = CiscoIOSXRAdminSystemActions(enable_session, self._logger)
-            try:
-                admin_actions.show_install_repository()
-                remote_path = remote_path.replace(":{}".format(password), "")
-            except:
-                self._sync = ""
-                self._is_old_iosxr = True
-                self._cmd_admin_prefix = ""
-
-        output = self._install_add_source(admin_actions=admin_actions, remote_path=remote_path,
-                                          firmware_file_name=firmware_file_name, password=password)
-        pkgs_for_install = self._filter_packages_for_install(admin_actions=admin_actions, output=output)
-
-        if not pkgs_for_install:
-            self._logger.info(admin_actions.prepare_output(self._result_dict))
-            raise Exception("Failed to load firmware: No new packages available to be installed (activated).")
-
-        activate_output = admin_actions.install_activate(pkgs_for_install, admin=self._cmd_admin_prefix)
-        if re.search(r"install operation \S+ continue asynchronously", activate_output,
-                     re.IGNORECASE) or not self._is_old_iosxr:
-            operation_id = self._get_operation_id(activate_output)
-            admin_actions.show_install_request(operation_id)
-            admin_actions.retrieve_install_log(operation_id)
-
-        commit_output = admin_actions.install_commit(admin=self._cmd_admin_prefix)
-        if not self._is_old_iosxr:
-            operation_id = self._get_operation_id(commit_output)
-            admin_actions.show_install_request(operation_id)
-            admin_actions.retrieve_install_log(operation_id)
-
-        active_pkgs = admin_actions.show_install_active()
-        for pkg in pkgs_for_install:
-            package_name = re.sub("^.*:|.x86_64$", "", pkg)
-            if package_name not in active_pkgs:
-                self._result_dict[package_name] = "Failed to install package, please see logs for details."
-            else:
-                success = True
-                self._result_dict[package_name] = "Package was successfully installed!"
-        if not success:
-            self._logger.error("Failed to load firmware.")
-            raise Exception("Failed to load firmware. Please check logs for details.")
-        self._logger.info(admin_actions.prepare_output(self._result_dict))
-        return admin_actions.prepare_output(self._result_dict)
-
-    def _install_add_source(self, admin_actions, remote_path, firmware_file_name, password):
-        error_map = {
-            "{}/{}\S*\s*could not be found".format(remote_path, firmware_file_name): "{} file not found".format(
-                firmware_file_name)}
-        action_map = {"[Pp]assword:": lambda session, logger: session.send_line(password, logger)}
-        if self._is_old_iosxr:
-            file_extension = None
-            file_extension_match = re.search("\.[a-z]{3}$", firmware_file_name, re.IGNORECASE)
-            if file_extension_match:
-                file_extension = file_extension_match.group().lstrip(".")
-            output = admin_actions.install_add_source(path=remote_path, file_extension=file_extension,
-                                                      file_name=firmware_file_name, admin=self._cmd_admin_prefix,
-                                                      sync=self._sync, action_map=action_map, error_map=error_map)
-        else:
-            output = admin_actions.install_add_source(path=remote_path, file_name=firmware_file_name,
-                                                      action_map=action_map, error_map=error_map)
-            operation_id = self._get_operation_id(output)
-            admin_actions.show_install_request(operation_id)
-        return output
-
-    def _filter_packages_for_install(self, admin_actions, output):
-        pkgs_for_install = []
-        available_packages = []
-        if self._is_old_iosxr:
-            if not output or "no new packages available to be activated" in output.lower():
-                raise Exception("Failed to load firmware: no new packages available to be installed (activated)")
-            pkgs_for_install = self._get_legacy_packages_for_install(output)
-        else:
-            operation_id = self._get_operation_id(output)
-            log = admin_actions.retrieve_install_log(operation_id)
-            for line in re.finditer("\s\s+(\S+\d+(\S+\d*)+)", log, re.MULTILINE):
-                available_packages.append(line.group().strip(" \n\t\r"))
-
-            if not available_packages:
-                raise Exception("Failed to load firmware: no new packages available for installation (activation)")
-            else:
-                for pkg in self._get_packages_for_install(available_packages):
-                    if pkg not in admin_actions.show_install_active():
-                        pkgs_for_install.append(pkg)
-                    else:
-                        self._result_dict[pkg] = "Package is already installed, skipping."
-        return pkgs_for_install
-
-    def _get_operation_id(self, output):
-        operation_id_match = re.search("Install operation (\d+)", output, re.IGNORECASE + re.MULTILINE)
-        if operation_id_match:
-            return operation_id_match.group(1)
-
-    def _get_packages_for_install(self, available_pkgs):
-        pkgs_for_install = []
-        if self._packages_to_add:
-            for pkg in self._packages_to_add:
-                if pkg in available_pkgs:
-                    pkgs_for_install.append(pkg)
-                else:
-                    self._result_dict[pkg] = "Package not found, skipping."
-        else:
-            pkgs_for_install.extend(available_pkgs)
-        return pkgs_for_install
-
-    def _get_legacy_packages_for_install(self, output):
-        _pkgs_to_add = []
-        available_pkgs_re_iter = re.finditer("(?P<type>Info|warning): *(?P<message>\S+\d+(.\d+)+)$", output,
-                                             re.MULTILINE + re.IGNORECASE) or []
-        for item in available_pkgs_re_iter:
-            match_dict = item.groupdict()
-
-            package_name = re.sub("^.*:", "", match_dict.get("message").lower())
-            if re.search("\Wpie\W", package_name):
-                continue
-            if match_dict.get("type").lower() == "warning":
-                package_name = re.sub("^.*:", "", match_dict.get("message"))
-                if self._packages_to_add and any(
-                        [package_name for pkg in self._packages_to_add if package_name in pkg]):
-                    self._result_dict[package_name] = "Package is already installed, skipping."
-                else:
-                    self._result_dict[package_name] = "Package is already installed, skipping."
-                continue
-            if match_dict.get("type").lower() == "info":
-                if not self._packages_to_add:
-                    if match_dict.get("message").lower() not in _pkgs_to_add:
-                        _pkgs_to_add.append(match_dict.get("message"))
-                else:
-                    for package in self._packages_to_add:
-                        if package.lower() in package_name.lower():
-                            if match_dict.get("message").lower() not in _pkgs_to_add:
-                                _pkgs_to_add.append(match_dict.get("message"))
-        return _pkgs_to_add
+import re
+
+from cloudshell.networking.cisco.flows.cisco_load_firmware_flow import (
+    CiscoLoadFirmwareFlow,
+)
+from cloudshell.shell.flows.utils.url import RemoteURL
+
+from cloudshell.networking.cisco.iosxr.command_actions.system import (
+    CiscoIOSXRAdminSystemActions,
+)
+from cloudshell.networking.cisco.iosxr.constants import IOSXR_FILE_SYSTEM
+
+
+class CiscoIOSXRLoadFirmwareFlow(CiscoLoadFirmwareFlow):
+    def __init__(self, cli_handler, logger, packages_to_install):
+        super().__init__(cli_handler, logger, IOSXR_FILE_SYSTEM)
+        self._result_dict = {}
+        self._sync = None
+        self._is_old_iosxr = False
+        self._cmd_admin_prefix = None
+
+        if (
+            not packages_to_install
+            or packages_to_install == "*"
+            or packages_to_install.lower() == "all"
+        ):
+            self._packages_to_add = []
+        else:
+            self._packages_to_add = packages_to_install.lower().split(" ")
+
+    def _load_firmware_flow(
+        self, path: RemoteURL, vrf_management_name: str, timeout: int
+    ):
+        """Load a firmware onto the device.
+
+        :param path: The path to the firmware file, including the firmware file name
+        :param vrf_management_name: Virtual Routing and Forwarding Name
+        :param timeout:
+        :return:
+        """
+        success = False
+
+        firmware_file_name = path.filename
+        password = path.password
+        remote_path = path.safe_url.replace(firmware_file_name, "").rstrip("/")
+        if vrf_management_name and vrf_management_name not in remote_path:
+            remote_path = remote_path.replace(
+                f"{path.host}", f"{path.host};{vrf_management_name}"
+            )
+
+        with self._cli_handler.get_cli_service(
+            self._cli_handler.enable_mode
+        ) as enable_session:
+            admin_actions = CiscoIOSXRAdminSystemActions(enable_session, self._logger)
+            try:
+                admin_actions.show_install_repository()
+                remote_path = remote_path.replace(f":{password}", "")
+            except Exception:
+                self._sync = ""
+                self._is_old_iosxr = True
+                self._cmd_admin_prefix = ""
+
+        output = self._install_add_source(
+            admin_actions=admin_actions,
+            remote_path=remote_path,
+            firmware_file_name=firmware_file_name,
+            password=password,
+        )
+        pkgs_for_install = self._filter_packages_for_install(
+            admin_actions=admin_actions, output=output
+        )
+
+        if not pkgs_for_install:
+            self._logger.info(admin_actions.prepare_output(self._result_dict))
+            raise Exception(
+                "Failed to load firmware: No new packages available "
+                "to be installed (activated)."
+            )
+
+        activate_output = admin_actions.install_activate(
+            pkgs_for_install, admin=self._cmd_admin_prefix
+        )
+        if (
+            re.search(
+                r"install operation \S+ continue asynchronously",
+                activate_output,
+                re.IGNORECASE,
+            )
+            or not self._is_old_iosxr
+        ):
+            operation_id = self._get_operation_id(activate_output)
+            admin_actions.show_install_request(operation_id)
+            admin_actions.retrieve_install_log(operation_id)
+
+        commit_output = admin_actions.install_commit(admin=self._cmd_admin_prefix)
+        if not self._is_old_iosxr:
+            operation_id = self._get_operation_id(commit_output)
+            admin_actions.show_install_request(operation_id)
+            admin_actions.retrieve_install_log(operation_id)
+
+        active_pkgs = admin_actions.show_install_active()
+        for pkg in pkgs_for_install:
+            package_name = re.sub("^.*:|.x86_64$", "", pkg)
+            if package_name not in active_pkgs:
+                self._result_dict[
+                    package_name
+                ] = "Failed to install package, please see logs for details."
+            else:
+                success = True
+                self._result_dict[package_name] = "Package was successfully installed!"
+        if not success:
+            self._logger.error("Failed to load firmware.")
+            raise Exception("Failed to load firmware. Please check logs for details.")
+        self._logger.info(admin_actions.prepare_output(self._result_dict))
+        return admin_actions.prepare_output(self._result_dict)
+
+    def _install_add_source(
+        self, admin_actions, remote_path, firmware_file_name, password
+    ):
+        error_map = {
+            r"{}/{}\S*\s*could not be found".format(
+                remote_path, firmware_file_name
+            ): f"{firmware_file_name} file not found"
+        }
+        action_map = {
+            "[Pp]assword:": lambda session, logger: session.send_line(password, logger)
+        }
+        if self._is_old_iosxr:
+            file_extension = None
+            file_extension_match = re.search(
+                r"\.[a-z]{3}$", firmware_file_name, re.IGNORECASE
+            )
+            if file_extension_match:
+                file_extension = file_extension_match.group().lstrip(".")
+            output = admin_actions.install_add_source(
+                path=remote_path,
+                file_extension=file_extension,
+                file_name=firmware_file_name,
+                admin=self._cmd_admin_prefix,
+                sync=self._sync,
+                action_map=action_map,
+                error_map=error_map,
+            )
+        else:
+            output = admin_actions.install_add_source(
+                path=remote_path,
+                file_name=firmware_file_name,
+                action_map=action_map,
+                error_map=error_map,
+            )
+            operation_id = self._get_operation_id(output)
+            admin_actions.show_install_request(operation_id)
+        return output
+
+    def _filter_packages_for_install(self, admin_actions, output):
+        pkgs_for_install = []
+        available_packages = []
+        if self._is_old_iosxr:
+            if (
+                not output
+                or "no new packages available to be activated" in output.lower()
+            ):
+                raise Exception(
+                    "Failed to load firmware: no new packages available "
+                    "to be installed (activated)"
+                )
+            pkgs_for_install = self._get_legacy_packages_for_install(output)
+        else:
+            operation_id = self._get_operation_id(output)
+            log = admin_actions.retrieve_install_log(operation_id)
+            for line in re.finditer(r"\s\s+(\S+\d+(\S+\d*)+)", log, re.MULTILINE):
+                available_packages.append(line.group().strip(" \n\t\r"))
+
+            if not available_packages:
+                raise Exception(
+                    "Failed to load firmware: no new packages available "
+                    "for installation (activation)"
+                )
+            else:
+                for pkg in self._get_packages_for_install(available_packages):
+                    if pkg not in admin_actions.show_install_active():
+                        pkgs_for_install.append(pkg)
+                    else:
+                        self._result_dict[
+                            pkg
+                        ] = "Package is already installed, skipping."
+        return pkgs_for_install
+
+    def _get_operation_id(self, output):
+        operation_id_match = re.search(
+            r"Install operation (\d+)", output, re.IGNORECASE + re.MULTILINE
+        )
+        if operation_id_match:
+            return operation_id_match.group(1)
+
+    def _get_packages_for_install(self, available_pkgs):
+        pkgs_for_install = []
+        if self._packages_to_add:
+            for pkg in self._packages_to_add:
+                if pkg in available_pkgs:
+                    pkgs_for_install.append(pkg)
+                else:
+                    self._result_dict[pkg] = "Package not found, skipping."
+        else:
+            pkgs_for_install.extend(available_pkgs)
+        return pkgs_for_install
+
+    def _get_legacy_packages_for_install(self, output):
+        _pkgs_to_add = []
+        available_pkgs_re_iter = (
+            re.finditer(
+                r"(?P<type>Info|warning): *(?P<message>\S+\d+(.\d+)+)$",
+                output,
+                re.MULTILINE + re.IGNORECASE,
+            )
+            or []
+        )
+        for item in available_pkgs_re_iter:
+            match_dict = item.groupdict()
+
+            package_name = re.sub("^.*:", "", match_dict.get("message").lower())
+            if re.search(r"\Wpie\W", package_name):
+                continue
+            if match_dict.get("type").lower() == "warning":
+                package_name = re.sub("^.*:", "", match_dict.get("message"))
+                if self._packages_to_add and any(
+                    package_name for pkg in self._packages_to_add if package_name in pkg
+                ):
+                    self._result_dict[
+                        package_name
+                    ] = "Package is already installed, skipping."
+                else:
+                    self._result_dict[
+                        package_name
+                    ] = "Package is already installed, skipping."
+                continue
+            if match_dict.get("type").lower() == "info":
+                if not self._packages_to_add:
+                    if match_dict.get("message").lower() not in _pkgs_to_add:
+                        _pkgs_to_add.append(match_dict.get("message"))
+                else:
+                    for package in self._packages_to_add:
+                        if package.lower() in package_name.lower():
+                            if match_dict.get("message").lower() not in _pkgs_to_add:
+                                _pkgs_to_add.append(match_dict.get("message"))
+        return _pkgs_to_add
```

