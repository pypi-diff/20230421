# Comparing `tmp/kepconfig-1.1.2.tar.gz` & `tmp/kepconfig-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kepconfig-1.1.2.tar", last modified: Tue Dec 13 15:45:56 2022, max compression
+gzip compressed data, was "kepconfig-1.2.0.tar", last modified: Fri Apr 21 18:38:17 2023, max compression
```

## Comparing `kepconfig-1.1.2.tar` & `kepconfig-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.952347 kepconfig-1.1.2/
--rw-rw-rw-   0        0        0     1127 2021-03-15 20:50:21.000000 kepconfig-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     5731 2022-12-13 15:45:56.952347 kepconfig-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5037 2022-10-21 00:45:52.000000 kepconfig-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.917144 kepconfig-1.1.2/kepconfig/
--rw-rw-rw-   0        0        0     1318 2022-12-13 15:45:33.000000 kepconfig-1.1.2/kepconfig/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.929144 kepconfig-1.1.2/kepconfig/admin/
--rw-rw-rw-   0        0        0      411 2022-10-21 00:45:52.000000 kepconfig-1.1.2/kepconfig/admin/__init__.py
--rw-rw-rw-   0        0        0     5776 2022-10-21 00:45:52.000000 kepconfig-1.1.2/kepconfig/admin/lls.py
--rw-rw-rw-   0        0        0     5266 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/admin/ua_server.py
--rw-rw-rw-   0        0        0     6392 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/admin/user_groups.py
--rw-rw-rw-   0        0        0     6133 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/admin/users.py
--rw-rw-rw-   0        0        0    19415 2022-12-05 22:48:26.000000 kepconfig-1.1.2/kepconfig/connection.py
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.934351 kepconfig-1.1.2/kepconfig/connectivity/
--rw-rw-rw-   0        0        0      411 2022-04-19 22:08:18.000000 kepconfig-1.1.2/kepconfig/connectivity/__init__.py
--rw-rw-rw-   0        0        0     7501 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/connectivity/channel.py
--rw-rw-rw-   0        0        0    10657 2022-10-21 00:45:52.000000 kepconfig-1.1.2/kepconfig/connectivity/device.py
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.940340 kepconfig-1.1.2/kepconfig/connectivity/egd/
--rw-rw-rw-   0        0        0      473 2022-04-19 22:08:18.000000 kepconfig-1.1.2/kepconfig/connectivity/egd/__init__.py
--rw-rw-rw-   0        0        0     7771 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/connectivity/egd/exchange.py
--rw-rw-rw-   0        0        0     5979 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/connectivity/egd/name.py
--rw-rw-rw-   0        0        0     6627 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/connectivity/egd/range.py
--rw-rw-rw-   0        0        0    20792 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/connectivity/tag.py
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.946345 kepconfig-1.1.2/kepconfig/datalogger/
--rw-rw-rw-   0        0        0      421 2020-12-11 03:00:05.000000 kepconfig-1.1.2/kepconfig/datalogger/__init__.py
--rw-rw-rw-   0        0        0     7228 2022-10-21 00:45:52.000000 kepconfig-1.1.2/kepconfig/datalogger/log_group.py
--rw-rw-rw-   0        0        0     6045 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/datalogger/log_items.py
--rw-rw-rw-   0        0        0     4138 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/datalogger/mapping.py
--rw-rw-rw-   0        0        0     5989 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/datalogger/triggers.py
--rw-rw-rw-   0        0        0     1923 2022-12-05 23:02:10.000000 kepconfig-1.1.2/kepconfig/error.py
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.950347 kepconfig-1.1.2/kepconfig/iot_gateway/
--rw-rw-rw-   0        0        0      568 2022-04-19 22:08:18.000000 kepconfig-1.1.2/kepconfig/iot_gateway/__init__.py
--rw-rw-rw-   0        0        0     8055 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/iot_gateway/agent.py
--rw-rw-rw-   0        0        0     6137 2021-03-22 20:48:04.000000 kepconfig-1.1.2/kepconfig/iot_gateway/iot_items.py
-drwxrwxrwx   0        0        0        0 2022-12-13 15:45:56.922144 kepconfig-1.1.2/kepconfig.egg-info/
--rw-rw-rw-   0        0        0     5731 2022-12-13 15:45:56.000000 kepconfig-1.1.2/kepconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2022-12-13 15:45:56.000000 kepconfig-1.1.2/kepconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-13 15:45:56.000000 kepconfig-1.1.2/kepconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-12-13 15:45:56.000000 kepconfig-1.1.2/kepconfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2022-10-21 00:45:52.000000 kepconfig-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-13 15:45:56.952347 kepconfig-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2209 2022-03-14 21:07:24.000000 kepconfig-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:17.024515 kepconfig-1.2.0/
+-rw-rw-rw-   0        0        0     1127 2021-03-15 20:50:21.000000 kepconfig-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     6530 2023-04-21 18:38:17.022519 kepconfig-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5624 2023-04-21 17:39:00.000000 kepconfig-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.926799 kepconfig-1.2.0/kepconfig/
+-rw-rw-rw-   0        0        0      901 2023-04-21 18:37:58.000000 kepconfig-1.2.0/kepconfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.953955 kepconfig-1.2.0/kepconfig/admin/
+-rw-rw-rw-   0        0        0      495 2023-03-31 19:09:46.000000 kepconfig-1.2.0/kepconfig/admin/__init__.py
+-rw-rw-rw-   0        0        0     6776 2023-04-21 17:03:24.000000 kepconfig-1.2.0/kepconfig/admin/lls.py
+-rw-rw-rw-   0        0        0     5316 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/admin/ua_server.py
+-rw-rw-rw-   0        0        0     6507 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/admin/user_groups.py
+-rw-rw-rw-   0        0        0     6139 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/admin/users.py
+-rw-rw-rw-   0        0        0    20553 2023-04-20 20:32:21.000000 kepconfig-1.2.0/kepconfig/connection.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.968973 kepconfig-1.2.0/kepconfig/connectivity/
+-rw-rw-rw-   0        0        0      759 2023-03-31 19:09:38.000000 kepconfig-1.2.0/kepconfig/connectivity/__init__.py
+-rw-rw-rw-   0        0        0     7831 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/channel.py
+-rw-rw-rw-   0        0        0    11083 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/device.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.983473 kepconfig-1.2.0/kepconfig/connectivity/egd/
+-rw-rw-rw-   0        0        0      517 2023-03-31 19:17:27.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/__init__.py
+-rw-rw-rw-   0        0        0     8753 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/exchange.py
+-rw-rw-rw-   0        0        0     6513 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/name.py
+-rw-rw-rw-   0        0        0     7170 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/egd/range.py
+-rw-rw-rw-   0        0        0    22720 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/tag.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.990479 kepconfig-1.2.0/kepconfig/connectivity/udd/
+-rw-rw-rw-   0        0        0      445 2023-03-31 19:14:13.000000 kepconfig-1.2.0/kepconfig/connectivity/udd/__init__.py
+-rw-rw-rw-   0        0        0     5930 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/connectivity/udd/profile.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:17.007513 kepconfig-1.2.0/kepconfig/datalogger/
+-rw-rw-rw-   0        0        0      491 2023-04-14 21:02:13.000000 kepconfig-1.2.0/kepconfig/datalogger/__init__.py
+-rw-rw-rw-   0        0        0     7654 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/datalogger/log_group.py
+-rw-rw-rw-   0        0        0     6280 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/datalogger/log_items.py
+-rw-rw-rw-   0        0        0     4366 2023-04-20 20:53:12.000000 kepconfig-1.2.0/kepconfig/datalogger/mapping.py
+-rw-rw-rw-   0        0        0     6528 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/datalogger/triggers.py
+-rw-rw-rw-   0        0        0     2455 2023-04-04 12:54:50.000000 kepconfig-1.2.0/kepconfig/error.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:17.018510 kepconfig-1.2.0/kepconfig/iot_gateway/
+-rw-rw-rw-   0        0        0      634 2023-03-31 19:17:31.000000 kepconfig-1.2.0/kepconfig/iot_gateway/__init__.py
+-rw-rw-rw-   0        0        0     8713 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/iot_gateway/agent.py
+-rw-rw-rw-   0        0        0     6854 2023-04-21 17:29:29.000000 kepconfig-1.2.0/kepconfig/iot_gateway/iot_items.py
+-rw-rw-rw-   0        0        0     1893 2023-04-03 19:20:56.000000 kepconfig-1.2.0/kepconfig/structures.py
+-rw-rw-rw-   0        0        0     1480 2023-04-04 12:27:33.000000 kepconfig-1.2.0/kepconfig/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-21 18:38:16.938805 kepconfig-1.2.0/kepconfig.egg-info/
+-rw-rw-rw-   0        0        0     6530 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1041 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-21 18:38:16.000000 kepconfig-1.2.0/kepconfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2022-10-21 00:45:52.000000 kepconfig-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-21 18:38:17.025515 kepconfig-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2417 2023-03-29 20:07:04.000000 kepconfig-1.2.0/setup.py
```

### Comparing `kepconfig-1.1.2/LICENSE` & `kepconfig-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kepconfig-1.1.2/PKG-INFO` & `kepconfig-1.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,103 +1,90 @@
-Metadata-Version: 2.1
-Name: kepconfig
-Version: 1.1.2
-Summary: SDK package for Kepware Configuration API
-Home-page: https://github.com/PTCInc/Kepware-ConfigAPI-SDK-Python
-Author: PTC Inc
-License: MIT License
-Keywords: Kepware,OPC,Configuration,Thingworx
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Kepware Configuration API SDK for Python
 
-[![PyPI version](https://badge.fury.io/py/kepconfig.svg)](https://badge.fury.io/py/kepconfig)
+[![Released Version](https://img.shields.io/pypi/v/kepconfig)](https://pypi.org/project/kepconfig) [![Supported Versions](https://img.shields.io/pypi/pyversions/kepconfig)](https://pypi.org/project/kepconfig) ![PyPI - Downloads](https://img.shields.io/pypi/dm/kepconfig) ![PyPI - License](https://img.shields.io/pypi/l/kepconfig)
 
-This is a package SDK to create Python modules to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
+This is a package to help create Python applications to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
 
 ## Prerequisites
 
-The client libraries are supported on Python 3.6 or later. All HTTP communication is handled by the [urllib](https://docs.python.org/3.6/library/urllib.html#module-urllib) Python standard library.
+Package supported and tested on Python 3.9 or later. Older versions support earlier Python 3 environments but have less functionality. All HTTP communication is handled by the [urllib](https://docs.python.org/3/library/urllib.html#module-urllib) Python standard library.
 
 ## Features
 
 - Supports both HTTP and HTTPS connections with certificate validation options
 
 SDK allows for *GET*, *ADD*, *DELETE*, and *MODIFY* functions for the following Kepware configuration objects:
 
 | Features      | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
 | **Project Properties** <br /> *(Get and Modify Only)* | Y | Y |
 | **Connectivity** <br /> *(Channel, Devices, Tags, Tag Groups)* | Y | Y |
 | **IoT Gateway** <br /> *(Agents, IoT Items)* | Y | Y |
 | **Datalogger** <br /> *(Log Groups, Items, Mapping, Triggers, Reset Mapping Service)* | Y | Y |
 | **Administration** <br /> *(User Groups, Users, UA Endpoints, Local License Server)* | Y* | Y |
+| **Product Info and Health Status\*\*** | Y | Y |
 
-Note (*) - UA Endpoints and Local License Server supported for Kepware Edge only
+- Note (*) - UA Endpoints and Local License Server supported for Kepware Edge only
+- Note (**) - Added to Kepware Server v6.13 / Kepware Edge v1.5 and later builds
 
 Driver specific features:
 
 | Driver          | Features       |
 | :----------:  | :----------:  |
 |GE Ethernet Global Data|Exchanges, Ranges and Name Resolutions|
+|Universal Device Driver|Profile Library|
 
 Methods to read the following logs:
 
 | Logs          | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
 | **Event Log** | Y | Y |
 | **API Transaction Log** | Y | Y |
 
 Configuration API *Services* implemented:
 
 | Services      | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
-| **TagGeneration** <br /> *(for supported drivers)* | Y | Y |
+| **TagGeneration**<br />*(for supported drivers)* | Y | Y |
 | **ReinitializeRuntime** | Y* | Y |
+| **ProjectLoad and ProjectSave**| Y | Y |
 
 Note (*) - Reinitialize service was implemented for Kepware Server v6.8+
 
-Generic REST methods are provided to use for functions not developed in SDK package. These are found in the Server Class in [connection.py](/kepconfig/connection.py)
+Filtering, sorting and pagination query options are added for any collections methods (ex: get_all_devices() or get_all_channel()).
+
+Generic REST methods are provided to use for functions not developed in SDK package. These are found in the Server Class in [connection.py](./kepconfig/connection.py)
 
 ## Known Limitations
 
-- Other property configuration for more complex drivers with objects besides channels, devices, tags and tag groups are not explicitly defined
+- Other property configuration for more complex drivers with objects besides channels, devices, tags and tag groups are not always explicitly defined
 - Other supported plug-ins (EFM Exporter, Scheduler, etc) are not defined
 - When using hostnames (not IP addresses) for connections, delays may occur under certain network configurations as the connection may attempt IPv6 connections first. IPv6 is not supported by Kepware servers at this time.
 
 ## Installation
 
 Package can be installed with `pip` using the following:
 
 ```cmd
     pip install kepconfig
 ```
 
 ## Key Concepts
 
-NOTE: Samples can also be found in the [samples](samples) folder.
+NOTE: Detailed examples can also be found in the [examples](./examples/) folder.
 
 ### Create server connection
 
 ```python
 import kepconfig.connection
 
 server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '')
 
 # For HTTPS connections:
-server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '', https=True)
+server = connection.server(host = '127.0.0.1', port = 57512, user = 'Administrator', pw = '', https=True)
 
 ```
 
 For certificate validation, the SDK uses the OS/systems trusted CA certificate store. The connection uses the "create_default_context()" function as part of urllib as described at the following links:
 
 - [ssl.create_default_context](https://docs.python.org/3/library/ssl.html#ssl.create_default_context)
 - [ssl.SSLContext.load_default_certs](https://docs.python.org/3/library/ssl.html#ssl.SSLContext.load_default_certs)
@@ -139,9 +126,8 @@
 ```
 
 ## Need More Information
 
 **Visit:**
 
 - [Kepware.com](https://www.kepware.com/)
-- [Configuration API Info](https://www.kepware.com/en-us/products/kepserverex/features/configuration-api/)
 - [PTC.com](https://www.ptc.com/)
```

### Comparing `kepconfig-1.1.2/README.md` & `kepconfig-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,113 @@
+Metadata-Version: 2.1
+Name: kepconfig
+Version: 1.2.0
+Summary: SDK package for Kepware Configuration API
+Home-page: https://github.com/PTCInc/Kepware-ConfigAPI-SDK-Python
+Author: PTC Inc
+License: MIT License
+Keywords: Kepware,OPC,Configuration,Thingworx
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Kepware Configuration API SDK for Python
 
-[![PyPI version](https://badge.fury.io/py/kepconfig.svg)](https://badge.fury.io/py/kepconfig)
+[![Released Version](https://img.shields.io/pypi/v/kepconfig)](https://pypi.org/project/kepconfig) [![Supported Versions](https://img.shields.io/pypi/pyversions/kepconfig)](https://pypi.org/project/kepconfig) ![PyPI - Downloads](https://img.shields.io/pypi/dm/kepconfig) ![PyPI - License](https://img.shields.io/pypi/l/kepconfig)
 
-This is a package SDK to create Python modules to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
+This is a package to help create Python applications to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
 
 ## Prerequisites
 
-The client libraries are supported on Python 3.6 or later. All HTTP communication is handled by the [urllib](https://docs.python.org/3.6/library/urllib.html#module-urllib) Python standard library.
+Package supported and tested on Python 3.9 or later. Older versions support earlier Python 3 environments but have less functionality. All HTTP communication is handled by the [urllib](https://docs.python.org/3/library/urllib.html#module-urllib) Python standard library.
 
 ## Features
 
 - Supports both HTTP and HTTPS connections with certificate validation options
 
 SDK allows for *GET*, *ADD*, *DELETE*, and *MODIFY* functions for the following Kepware configuration objects:
 
 | Features      | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
 | **Project Properties** <br /> *(Get and Modify Only)* | Y | Y |
 | **Connectivity** <br /> *(Channel, Devices, Tags, Tag Groups)* | Y | Y |
 | **IoT Gateway** <br /> *(Agents, IoT Items)* | Y | Y |
 | **Datalogger** <br /> *(Log Groups, Items, Mapping, Triggers, Reset Mapping Service)* | Y | Y |
 | **Administration** <br /> *(User Groups, Users, UA Endpoints, Local License Server)* | Y* | Y |
+| **Product Info and Health Status\*\*** | Y | Y |
 
-Note (*) - UA Endpoints and Local License Server supported for Kepware Edge only
+- Note (*) - UA Endpoints and Local License Server supported for Kepware Edge only
+- Note (**) - Added to Kepware Server v6.13 / Kepware Edge v1.5 and later builds
 
 Driver specific features:
 
 | Driver          | Features       |
 | :----------:  | :----------:  |
 |GE Ethernet Global Data|Exchanges, Ranges and Name Resolutions|
+|Universal Device Driver|Profile Library|
 
 Methods to read the following logs:
 
 | Logs          | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
 | **Event Log** | Y | Y |
 | **API Transaction Log** | Y | Y |
 
 Configuration API *Services* implemented:
 
 | Services      | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
-| **TagGeneration** <br /> *(for supported drivers)* | Y | Y |
+| **TagGeneration**<br />*(for supported drivers)* | Y | Y |
 | **ReinitializeRuntime** | Y* | Y |
+| **ProjectLoad and ProjectSave**| Y | Y |
 
 Note (*) - Reinitialize service was implemented for Kepware Server v6.8+
 
-Generic REST methods are provided to use for functions not developed in SDK package. These are found in the Server Class in [connection.py](/kepconfig/connection.py)
+Filtering, sorting and pagination query options are added for any collections methods (ex: get_all_devices() or get_all_channel()).
+
+Generic REST methods are provided to use for functions not developed in SDK package. These are found in the Server Class in [connection.py](./kepconfig/connection.py)
 
 ## Known Limitations
 
-- Other property configuration for more complex drivers with objects besides channels, devices, tags and tag groups are not explicitly defined
+- Other property configuration for more complex drivers with objects besides channels, devices, tags and tag groups are not always explicitly defined
 - Other supported plug-ins (EFM Exporter, Scheduler, etc) are not defined
 - When using hostnames (not IP addresses) for connections, delays may occur under certain network configurations as the connection may attempt IPv6 connections first. IPv6 is not supported by Kepware servers at this time.
 
 ## Installation
 
 Package can be installed with `pip` using the following:
 
 ```cmd
     pip install kepconfig
 ```
 
 ## Key Concepts
 
-NOTE: Samples can also be found in the [samples](samples) folder.
+NOTE: Detailed examples can also be found in the [examples](./examples/) folder.
 
 ### Create server connection
 
 ```python
 import kepconfig.connection
 
 server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '')
 
 # For HTTPS connections:
-server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '', https=True)
+server = connection.server(host = '127.0.0.1', port = 57512, user = 'Administrator', pw = '', https=True)
 
 ```
 
 For certificate validation, the SDK uses the OS/systems trusted CA certificate store. The connection uses the "create_default_context()" function as part of urllib as described at the following links:
 
 - [ssl.create_default_context](https://docs.python.org/3/library/ssl.html#ssl.create_default_context)
 - [ssl.SSLContext.load_default_certs](https://docs.python.org/3/library/ssl.html#ssl.SSLContext.load_default_certs)
@@ -120,9 +149,8 @@
 ```
 
 ## Need More Information
 
 **Visit:**
 
 - [Kepware.com](https://www.kepware.com/)
-- [Configuration API Info](https://www.kepware.com/en-us/products/kepserverex/features/configuration-api/)
 - [PTC.com](https://www.ptc.com/)
```

### Comparing `kepconfig-1.1.2/kepconfig/admin/lls.py` & `kepconfig-1.2.0/kepconfig/admin/lls.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,41 +3,42 @@
 # See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 r"""`lls` exposes an API to allow modifications to Local License Server parameters in 
 the Kepware Administration through the Kepware Configuration API
 """
+from .. import connection
 from typing import Union
 from ..error import KepHTTPError, KepError
 
 
+
 LLS_ROOT = '/admin'
+FORCE_CHECK_URL = '/project/services/ForceLicenseCheck'
 LICENSING_SERVER_PORT = "libadminsettings.LICENSING_SERVER_PORT"
 LICENSING_SERVER_NAME = "libadminsettings.LICENSING_SERVER_NAME"
 LICENSING_SERVER_ENABLE = "libadminsettings.LICENSING_SERVER_ENABLE"
 LICENSING_CHECK_PERIOD_MINS = "libadminsettings.LICENSING_CHECK_PERIOD_MINS"
 LICENSING_SERVER_SSL_PORT = "libadminsettings.LICENSING_SERVER_SSL_PORT"
 LICENSING_SERVER_ALLOW_INSECURE_COMMS = "libadminsettings.LICENSING_SERVER_ALLOW_INSECURE_COMMS"
 LICENSING_SERVER_ALLOW_SELF_SIGNED_CERTS = "libadminsettings.LICENSING_SERVER_ALLOW_SELF_SIGNED_CERTS"
 LICENSING_CLIENT_ALIAS = "libadminsettings.LICENSING_CLIENT_ALIAS"
 
 class lls_config:
     '''A class to represent a admin properties for the Local License Server connection from an instance of Kepware. 
     This object is used to easily manage the LLS parameters for a Kepware instance. 
 
-    Properties:
-
-    "server_name" - Host name or IP address of the LLS server
-    "server_port" - HTTP/non-SSL port to target for the LLS server
-    "check_period" - Period that Kepware checks licensing status
-    "server_port_SSL" - HTTPS/SSL port to target for the LLS server
-    "allow_insecure_comms" - When True, use HTTP/non-SSL connection to LLS
-    "allow_self_signed_certs" - Allow for self signed certificates to be used during HTTPS/SSL connections to the LLS
-    "instance_alias_name" - Alias name for LLS to use as reference to this Kepware instance
+    :param server_name: Host name or IP address of the LLS server
+    :param server_port: HTTP/non-SSL port to target for the LLS server
+    :param check_period: Period that Kepware checks licensing status
+    :param server_port_SSL: HTTPS/SSL port to target for the LLS server
+    :param allow_insecure_comms: When True, use HTTP/non-SSL connection to LLS
+    :param allow_self_signed_certs: Allow for self signed certificates to be used during HTTPS/SSL connections to the LLS
+    :param instance_alias_name: Alias name for LLS to use as reference to this Kepware instance
     '''
 
     def __init__(self, config = {}):
         self.server_name = config[LICENSING_SERVER_NAME] if LICENSING_SERVER_NAME in config else ''
         self.server_port = config[LICENSING_SERVER_PORT] if LICENSING_SERVER_PORT in config else 7070
         self.check_period = config[LICENSING_CHECK_PERIOD_MINS] if LICENSING_CHECK_PERIOD_MINS in config else 5
         self.server_port_SSL = config[LICENSING_SERVER_SSL_PORT] if LICENSING_SERVER_SSL_PORT in config else 1883
@@ -55,79 +56,84 @@
             LICENSING_SERVER_ALLOW_SELF_SIGNED_CERTS: self.allow_self_signed_certs,
             LICENSING_CLIENT_ALIAS: self.instance_alias_name
         }
     
     def __str__(self) -> str:
         return "{}".format(self._get_dict())
 
-def get_lls_config(server) -> lls_config:
-    '''Returns the properties of the Local License server properties. Returned object is lls_config class object.
+def get_lls_config(server: connection.server) -> lls_config:
+    '''Returns the properties of the Local License server connection properties. Returned object is `lls_config` class object.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
     
-    RETURNS:
-    lls_config - class object with lls configuration
+    :return: `lls_config` class object with lls connection configuration
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_get(server.url + LLS_ROOT)
     return lls_config(r.payload)
 
-def update_lls_config(server, config: lls_config) -> bool:
-    '''Updates the Local License Server admin properties for Kepware.
+def update_lls_config(server: connection.server, config: lls_config) -> bool:
+    '''Updates the Local License Server connection properties for Kepware.
+    
+    :param server: instance of the `server` class
+    :param config: `lls_config` class object with lls connection configuration
     
-    INPUTS:
-    "server" - instance of the "server" class
-    "config" - lls_config class object
-    
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
+
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     DATA = config._get_dict()
     r = server._config_update(server.url + LLS_ROOT, DATA)
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def enable_lls(server) -> bool:
+def enable_lls(server: connection.server) -> bool:
     '''Enables the Local License Server connection for Kepware.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_update(server.url + LLS_ROOT, {LICENSING_SERVER_ENABLE: True})
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def disable_lls(server) -> bool:
+def disable_lls(server: connection.server) -> bool:
     '''Disables the Local License Server connection for Kepware.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_update(server.url + LLS_ROOT, {LICENSING_SERVER_ENABLE: False})
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
+
+def force_license_check(server: connection.server, job_ttl: int = None):
+    '''Executes a ForceLicenseCheck service call to the Kepware instance. This triggers the server to verify the 
+    license state of the license received from the Local License Server.
+
+    :param server: instance of the `server` class
+    :param job_ttl: *(optional)* Determines the number of seconds a job instance will exist following completion.
+
+    :return: `KepServiceResponse` instance with job information
+
+    :raises KepHTTPError: If urllib provides an HTTPError (If not HTTP code 202 [Accepted] or 429 [Too Busy] returned)
+    :raises KepURLError: If urllib provides an URLError
+    '''
+
+    url = f'{server.url}{FORCE_CHECK_URL}'
+    job = server._kep_service_execute(url, None, job_ttl)
+    return job
```

### Comparing `kepconfig-1.1.2/kepconfig/admin/ua_server.py` & `kepconfig-1.2.0/kepconfig/admin/users.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,156 @@
 # -------------------------------------------------------------------------
 # Copyright (c), PTC Inc. and/or all its affiliates. All rights reserved.
 # See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
-r"""`ua_server` exposes an API to allow modifications (add, delete, modify) to 
-OPC UA Server endpoints within the Kepware Administration through the Kepware Configuration API
+r"""`users` exposes an API to allow modifications (add, delete, modify) to 
+users within the Kepware Administration User Management through the Kepware Configuration API
 """
 from typing import Union
-from ..error import KepHTTPError, KepError
+from ..error import KepError, KepHTTPError
+from ..connection import server
 
 
-UA_ROOT = '/admin/ua_endpoints'
+USERS_ROOT = '/admin/server_users'
+ENABLE_PROPERTY = 'libadminsettings.USERMANAGER_USER_ENABLED'
 
-def _create_url(endpoint = None):
+def _create_url(user = None):
     '''Creates url object for the "server_users" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
     Returns the user specific url when a value is passed as the user name.
     '''
     
-    if endpoint == None:
-        return UA_ROOT
+    if user == None:
+        return USERS_ROOT
     else:
-        return '{}/{}'.format(UA_ROOT,endpoint)
+        return '{}/{}'.format(USERS_ROOT,user)
 
-def add_endpoint(server, DATA) -> Union[bool, list]:
-    '''Add an "endpoint" or multiple "endpoint" objects to Kepware UA Server by passing a 
-    list of endpoints to be added all at once.
+def add_user(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add a `"user"` or multiple `"user"` objects to Kepware User Manager by passing a 
+    list of users to be added all at once.
 
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param DATA: Dict or List of Dicts of the users to add
 
-    "DATA" - properly JSON object (dict) of the endpoint
-    expected by Kepware Configuration API
-
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-
-    List - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     endpoints added that failed.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_add(server.url + _create_url(), DATA)
-    if r.code == 201: return True
+    if r.code == 201: return True 
     elif r.code == 207:
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_endpoint(server, endpoint) -> bool:
-    '''Delete a "endpoint" object in Kepware UA Server
+def del_user(server: server, user: str) -> bool:
+    '''Delete a `"user"` object in Kepware User Manager
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "endpoint" - name of endpoint
+    :param server: instance of the `server` class
+    :param user: name of user to delete
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
-    r = server._config_del(server.url + _create_url(endpoint))
+    r = server._config_del(server.url + _create_url(user))
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_endpoint(server, DATA, endpoint = None) -> bool:
-    '''Modify a endpoint object and it's properties in Kepware UA Server. If a "endpoint" is not provided as an input,
-    you need to identify the endpoint in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
-    assume that is the endpoint that is to be modified.
-
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "DATA" - properly JSON object (dict) of the endpoint properties to be modified.
+def modify_user(server: server , DATA: dict, *, user: str = None) -> bool:
+    '''Modify a `"user object"` and it's properties in Kepware User Manager. If a `"user"` is not provided as an input,
+    you need to identify the user in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
+    assume that is the user that is to be modified.
 
-    "endpoint" (optional) - name of endpoint to modify. Only needed if not existing in  "DATA"
+    :param server: instance of the `server` class
+    :param DATA: Dict of the user properties to be modified.
+    :param user: *(optional)* name of user to modify. Only needed if not existing in `"DATA"`
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    
-    # channel_data = server._force_update_check(force, DATA)
-    if endpoint == None:
+
+    if user == None:
         try:
             r = server._config_update(server.url + _create_url(DATA['common.ALLTYPES_NAME']), DATA)
             if r.code == 200: return True 
             else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
         except KeyError as err:
-            err_msg = 'Error: No UA Endpoint identified in DATA | Key Error: {}'.format(err)
+            err_msg = 'Error: No User identified in DATA | Key Error: {}'.format(err)
             raise KepError(err_msg)
-
-        # except Exception as e:
-        #     return 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
     else:
-        r = server._config_update(server.url + _create_url(endpoint), DATA)
+        r = server._config_update(server.url + _create_url(user), DATA)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_endpoint(server, endpoint) -> dict:
-    '''Returns the properties of the endpoint object. Returned object is JSON.
+def get_user(server: server, user: str) -> dict:
+    '''Returns the properties of the `"user"` object.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "endpoint" - name of endpoint
+    :param server: instance of the `server` class
+    :param user: name of user to retrieve
     
-    RETURNS:
-    dict - data for the endpoint requested
+    :return: Dict of properties for the user requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
-    r = server._config_get(server.url + _create_url(endpoint))
+    r = server._config_get(server.url + _create_url(user))
     return r.payload
 
-def get_all_endpoints(server) -> list:
-    '''Returns list of all endpoint objects and their properties. Returned object is JSON list.
+def get_all_users(server: server, *, options: dict = None) -> list:
+    '''Returns list of all `"user"` objects and their properties.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of users. Options are 'filter', 
+    'sortOrder', 'sortProperty', 'pageNumber', and 'pageSize.
+
+    :return: List of properties for all users
+
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
+    '''
+
+    r = server._config_get(f'{server.url}{_create_url()}', params= options)
+    return r.payload
+
+def enable_user(server: server, user: str) -> bool:
+    '''Enable the `"user"`.
     
-    RETURNS:
-    list - data for all endpoints requested
+    :param server: instance of the `server` class
+    :param user: name of user
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
+
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
+    DATA = {ENABLE_PROPERTY: True}
+    return modify_user(server, DATA, user= user)
+
+def disable_user(server: server, user: str) -> bool:
+    '''Disable the `"user"`.
+    
+    :param server: instance of the `server` class
+    :param user: name of user
 
-    r = server._config_get(server.url + _create_url())
-    return r.payload
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
+
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
+    '''
+    DATA = {ENABLE_PROPERTY: False}
+    return modify_user(server, DATA, user= user)
```

### Comparing `kepconfig-1.1.2/kepconfig/admin/user_groups.py` & `kepconfig-1.2.0/kepconfig/admin/user_groups.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,186 +1,156 @@
 # -------------------------------------------------------------------------
 # Copyright (c), PTC Inc. and/or all its affiliates. All rights reserved.
 # See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 r"""`user_groups` exposes an API to allow modifications (add, delete, modify) to 
-user_groups within the Kepware Administration User Manager through the Kepware Configuration API
+user groups within the Kepware Administration User Manager through the Kepware Configuration API
 """
 from typing import Union
 from ..error import KepHTTPError, KepError
+from ..connection import server
 
 
 USERGROUPS_ROOT = '/admin/server_usergroups'
 ENABLE_PROPERTY = 'libadminsettings.USERMANAGER_GROUP_ENABLED'
 
 def _create_url(user_group = None):
     '''Creates url object for the "server_usergroups" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
-    Returns the user_group specific url when a value is passed as the user_group name.
+    Returns the user group specific url when a value is passed as the user_group name.
     '''
     
     if user_group == None:
         return USERGROUPS_ROOT
     else:
         return '{}/{}'.format(USERGROUPS_ROOT,user_group)
 
-def add_user_group(server, DATA) -> Union[bool, list]:
-    '''Add a "user_group" or multiple "user_group" objects to Kepware User Manager by passing a 
+def add_user_group(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add a `"user group"` or multiple `"user group"` objects to Kepware User Manager by passing a 
     list of user groups to be added all at once.
 
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param DATA: Dict or List of Dicts of the user groups to add
 
-    "DATA" - properly JSON object (dict) of the user_group
-    expected by Kepware Configuration API
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    endpoints added that failed.
 
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-
-    List - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
-    user groups added that failed.
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_add(server.url + _create_url(), DATA)
     if r.code == 201: return True 
     elif r.code == 207:
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_user_group(server, user_group) -> bool:
-    '''Delete a "user_group" object in Kepware User Manager
+def del_user_group(server: server, user_group: str) -> bool:
+    '''Delete a `"user group"` object in Kepware User Manager
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "user_group" - name of user_group
+    :param server: instance of the `server` class
+    :param user_group: name of user group to delete
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_del(server.url + _create_url(user_group))
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_user_group(server, DATA, user_group = None) -> bool:
-    '''Modify a user_group object and it's properties in Kepware User Manager. If a "user_group" is not provided as an input,
-    you need to identify the user_group in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
-    assume that is the user_group that is to be modified.
-
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "DATA" - properly JSON object (dict) of the user_group properties to be modified.
-
-    "user_group" (optional) - name of user_group to modify. Only needed if not existing in  "DATA"
+def modify_user_group(server: server, DATA: dict, *, user_group: str = None) -> bool:
+    '''Modify a `"user group"` object and it's properties in Kepware User Manager. If a `"user group"` is not provided as an input,
+    you need to identify the user group in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
+    assume that is the user group that is to be modified.
+
+    :param server: instance of the `server` class
+    :param DATA: Dict of the user group properties to be modified.
+    :param user_group: *(optional)* name of user group to modify. Only needed if not existing in `"DATA"`
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     
-    # channel_data = server._force_update_check(force, DATA)
     if user_group == None:
         try:
             r = server._config_update(server.url + _create_url(DATA['common.ALLTYPES_NAME']), DATA)
             if r.code == 200: return True 
-            else: return False
+            else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
         except KeyError as err:
             err_msg = 'Error: No User Group identified in DATA | Key Error: {}'.format(err)
             raise KepError(err_msg)
-        # except Exception as e:
-        #     return 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
     else:
         r = server._config_update(server.url + _create_url(user_group), DATA)
         if r.code == 200: return True 
-        else: return False
+        else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_user_group(server, user_group) -> dict:
-    '''Returns the properties of the user_group object. Returned object is JSON.
+def get_user_group(server: server, user_group: str) -> dict:
+    '''Returns the properties of the `"user group"` object.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "user_group" - name of user_group
+    :param server: instance of the `server` class
+    :param user_group: name of user group to retrieve
     
-    RETURNS:
-    dict - data for the user_group requested
+    :return: Dict of properties for the user group requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_get(server.url + _create_url(user_group))
     return r.payload
 
-def get_all_user_groups(server) -> list:
-    '''Returns list of all user_group objects and their properties. Returned object is JSON list.
-    
-    INPUTS:
-    "server" - instance of the "server" class
+def get_all_user_groups(server: server, *, options: dict = None) -> list:
+    '''Returns list of all `"user group"` objects and their properties.
     
-    RETURNS:
-    list - data for all user_groups requested
+    :param server: instance of the `server` class
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of user groups. Options are 'filter', 
+    'sortOrder', 'sortProperty', 'pageNumber', and 'pageSize.
+
+    :return: List of properties for all user groups
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
-    r = server._config_get(server.url + _create_url())
+    r = server._config_get(f'{server.url}{_create_url()}', params= options)
     return r.payload
 
-def enable_user_group(server, user_group) -> bool:
-    '''Enable the user group. Returned object is JSON.
+def enable_user_group(server: server, user_group: str) -> bool:
+    '''Enable the `"user group"`.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param user_group: name of user group
 
-    "user_group" - name of user group
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     DATA = {ENABLE_PROPERTY: True}
-    return modify_user_group(server, DATA, user_group)
+    return modify_user_group(server, DATA, user_group= user_group)
 
-def disable_user_group(server, user_group) -> bool:
-    '''Disable the user group. Returned object is JSON.
+def disable_user_group(server: server, user_group: str) -> bool:
+    '''Disable the `"user group"`.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "user_group" - name of user group
+    :param server: instance of the `server` class
+    :param user_group: name of user group
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     DATA = {ENABLE_PROPERTY: False}
-    return modify_user_group(server, DATA, user_group)
+    return modify_user_group(server, DATA, user_group= user_group)
```

### Comparing `kepconfig-1.1.2/kepconfig/connection.py` & `kepconfig-1.2.0/kepconfig/connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,89 @@
 # -------------------------------------------------------------------------
 # Copyright (c) PTC Inc. and/or all its affiliates. All rights reserved.
 # See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
-r"""`connection` exposes an API that manages the RESTful requests 
-for the Kepware Configuration API. 
+r"""`connection` exposes an `server` class that manages the connection
+information and RESTful requests for the Kepware Configuration API Library.
 """
 
 import json
 import codecs
 import datetime
 from urllib import request, parse, error
 from base64 import b64encode
 from .error import KepError, KepHTTPError, KepURLError
 import socket
 import ssl
-import sys
+from .structures import KepServiceResponse, KepServiceStatus, _HttpDataAbstract
 
-class KepServiceResponse:
-    '''A class to represent a return object when calling a "service" API of Kepware. This is
-    used to return the responses when a "service" is executed appropriately
-
-    Properties:
-
-    "code" - HTTP code returned
-    "message" - return from the "service" call
-    "href" - URL reference to the JOB that is created by the service API
-    '''
-
-    def __init__(self, code = '', message = '', href = ''):
-        self.code = code
-        self.message = message
-        self.href = href
-    
-    def __str__(self):
-        return '{"code": %s, "message": %s, "href": %s}' % (self.code, self.message, self.href)
-
-class KepServiceStatus:
-    '''A class to represent a status object when checking on a "service" API job state in Kepware. This is
-    used to return the status of a "service" job
-
-    Properties:
-
-    "complete" - Boolean of service job completion status
-    "status" - Status code of job
-    "message" - Error message if service job fails
-    
-    '''
-    def __init__(self, complete = '', status = '', message = ''):
-        self.status = status
-        self.message = message
-        self.complete = complete
-    
-    def __str__(self):
-        return '{"complete": %s, "status": %s, "message": %s}' % (self.complete, self.status, self.message)
-
-class _HttpDataAbstract:
-    def __init__(self):
-        self.payload = ''
-        self.code = ''
-        self.reason = ''
 
 class server:
     '''A class to represent a connection to an instance of Kepware. This object is used to 
     create the Authentication and server parameters to taget a Kepware instance. An instance of this is 
     used in all configuration calls done.
 
-    Properties:
-
-    "host" - host name or IP address
-    "port" - port of Configuration API
-    "username" - username to conduct "Basic Authentication"
-    "password" - password to conduct "Basic Authentication"
-    "url" (STATIC) - base URL for the server connection
-    "SSL_on" - Identify to use HTTPS connection (Default: False)
-    "SSL_ignore_hostname" - During certificate validation ignore the hostname check
-    "SSL_trust_all_certs" (insecure) - During certificate validation trust any certificate - if True, 
+    :param host: host name or IP address
+    :param port: port of Configuration API
+    :param username: username to conduct "Basic Authentication"
+    :param password: password to conduct "Basic Authentication"
+    :param https: Sets `SSL_on` to use HTTPS connection (Default: False)
+    :param SSL_on: Identify to use HTTPS connection (Default: False)
+    :param SSL_ignore_hostname: During certificate validation ignore the hostname check
+    :param SSL_trust_all_certs: (insecure) - During certificate validation trust any certificate - if True, 
         will "set SSL_ignore_hostname" to true
+    :param url: base URL for the server connection
 
-    Methods:
+    **Methods**
 
-    "reinitialize()" - reinitialize the Kepware server
-    "get_trans_log()" - retrieve the Configuration API transaction logs
-    "get_event_log()" - retrieve the Kepware Event Log
-    "get_project_properties()" - retrieve the Kepware Project Properties
-    "modify_project_properties()" - modify the Kepware Project Properties
-    "service_status()" - retrive service job status
+    :meth:`reinitialize`: reinitialize the Kepware server
+
+    :meth:`get_transaction_log`: retrieve the Configuration API transaction logs
+
+    :meth:`get_event_log`: retrieve the Kepware Event Log
+
+    :meth:`get_project_properties`: retrieve the Kepware Project Properties
+
+    :meth:`modify_project_properties` - modify the Kepware Project Properties
+
+    :meth:`service_status` - retrive service job status
     '''
     __root_url = '/config'
     __version_url = '/v1'
     __project_services_url = '/project/services'
     __event_log_url = '/event_log'
     __trans_log_url = '/log'
 
 
 
-    def __init__(self,  host = None, port = None, user = None, pw = None, https = False):
+    def __init__(self,  host: str, port: int, user: str, pw: str, https: bool = False):
         self.host = host
         self.port = port
         self.username = user
         self.password = pw
         self.__ssl_context = ssl.create_default_context()
         self.__SSL_on = https
     
     @property
     def url(self):
         if self.SSL_on:
             proto = 'https'
         else:
             proto = 'http'
-        return  '{}://{}:{}{}{}'.format(proto, self.host, self.port, self.__root_url, self.__version_url)
+        return  f'{proto}://{self.host}:{self.port}{self.__root_url}{self.__version_url}'
     
     @property
     def SSL_on(self):
         return self.__SSL_on
     
     @SSL_on.setter
     def SSL_on(self, val):
+        
         if isinstance(val, bool):
             self.__SSL_on = val
 
     @property
     def SSL_ignore_hostname(self):
         return not self.__ssl_context.check_hostname
 
@@ -148,127 +110,138 @@
                 if self.__ssl_context.check_hostname == True:
                     self.__ssl_context.check_hostname = False
                 self.__ssl_context.verify_mode = ssl.CERT_NONE
             else:
                 self.__ssl_context.verify_mode = ssl.CERT_REQUIRED
 
 
+    def get_status(self) -> dict:
+        '''Executes a health status request to the Kepware instance to report service statuses.
 
+        :return: List of data for the health status request
 
-    def reinitialize(self, job_ttl = None) -> KepServiceResponse:
-        '''Executes a Reinitialize call to the Kepware instance.
+        :raises KepHTTPError: If urllib provides an HTTPError
+        :raises KepURLError: If urllib provides an URLError
+        '''
 
-        INPUTS:
+        r = self._config_get(f'{self.url}/status')
+        return r.payload
+    def get_info(self) -> dict:
+        '''Requests product information from the Kepware instance. Provides various information including
+        product name and version information.
+
+        :return: dict of data for the product information request
+        
+        :raises KepHTTPError: If urllib provides an HTTPError
+        :raises KepURLError: If urllib provides an URLError
+        '''
+        
+        r = self._config_get(f'{self.url}/about')
+        return r.payload
 
-        "job_ttl" (optional) - Determines the number of seconds a job instance will exist following completion.
+    def reinitialize(self, job_ttl: int = None) -> KepServiceResponse:
+        '''Executes a Reinitialize service call to the Kepware instance.
 
-        RETURNS:
-        KepServiceResponse instance with job information
+        :param job_ttl: *(optional)* Determines the number of seconds a job instance will exist following completion.
 
-        EXCEPTIONS (If not HTTP 200 or 429 returned):
-        
-        KepHTTPError - If urllib provides an HTTPError
-        KepURLError - If urllib provides an URLError
+        :return: `KepServiceResponse` instance with job information
+
+        :raises KepHTTPError: If urllib provides an HTTPError (If not HTTP code 202 [Accepted] or 429 [Too Busy] returned)
+        :raises KepURLError: If urllib provides an URLError
         '''
         url = self.url + self.__project_services_url + '/ReinitializeRuntime' 
         try:
             job = self._kep_service_execute(url, None, job_ttl)
             return job
         except Exception as err:
             raise err
         
-    def get_trans_log(self, start = None, end = None, limit = None) -> list:
+    def get_transaction_log(self, limit: int = None, start: datetime.datetime = None, end: datetime.datetime = None) -> list:
         ''' Get the Transaction Log from the Kepware instance.
 
-        "start" (optional) - datetime.datetime type and should be UTC
-
-        "end" (optional) - datetime.datetime type and should be UTC
+        :param limit: *(optional)* number of transaction log entries to request
+        :param start: *(optional)* start time of query as `datetime.datetime` type and should be UTC
+        :param end: *(optional)* end time of query as `datetime.datetime` type and should be UTC
 
-        "limit" (optional) -  number of event log entries to request
+        :raises KepHTTPError: If urllib provides an HTTPError
+        :raises KepURLError: If urllib provides an URLError
         '''
         query = self.__create_query(start, end, limit)
-        url = self.url + self.__trans_log_url + '?' + parse.urlencode(query)
-        r = self._config_get(url)
+        url = f'{self.url}{self.__trans_log_url}'
+        r = self._config_get(url, params= query)
         return r.payload
 
-    def get_event_log(self, limit = None, start = None, end = None) -> list:
+    def get_event_log(self, limit: int = None, start: datetime.datetime = None, end: datetime.datetime = None, *, options: dict = None) -> list:
         ''' Get the Event Log from the Kepware instance.
 
-        "start" (optional) - datetime.datetime type and should be UTC
+        :param limit: *(optional)* number of event log entries to request
+        :param start: *(optional)* start time of query as `datetime.datetime` type and should be UTC
+        :param end: *(optional)* end time of query as `datetime.datetime` type and should be UTC
+        :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of transactions. Options are `event`, 
+        `sortOrder`, `sortProperty`, `pageNumber`, and `pageSize`
 
-        "end" (optional) - datetime.datetime type and should be UTC
-
-        "limit" (optional) - number of event log entries to request
+        :raises KepHTTPError: If urllib provides an HTTPError
+        :raises KepURLError: If urllib provides an URLError
         '''
         query = self.__create_query(start, end, limit)
-        url = self.url + self.__event_log_url + '?' + parse.urlencode(query)
-        r = self._config_get(url)
+        if options is not None:
+            query = {**query, **options}
+        url = f'{self.url}{self.__event_log_url}'
+        r = self._config_get(url, params= query)
         return r.payload
     
     def get_project_properties(self) -> dict:
         ''' Get the Project Properties of the Kepware instance.
         
-        RETURNS:
-        dict - Dict of all the project properties
+        :return: Dict of all the project properties
 
-        EXCEPTIONS:
-        KepHTTPError - If urllib provides an HTTPError
-        KepURLError - If urllib provides an URLError
+        :raises KepHTTPError: If urllib provides an HTTPError
+        :raises KepURLError: If urllib provides an URLError
         '''
 
         r = self._config_get(self.url + '/project')
         return r.payload
     
-    def modify_project_properties(self, DATA, force = False) -> bool:
+    def modify_project_properties(self, DATA: dict, force: bool = False) -> bool:
         ''' Modify the Project Properties of the Kepware instance.
 
-        INPUTS:
-
-        "DATA" - properly JSON object (dict) of the project properties to be modified
-
-        "force" (optional) - if True, will force the configuration update to the Kepware server
+        :param DATA: Dict of the project properties to be modified
+        :param force: *(optional)* if True, will force the configuration update to the Kepware server
         
-        RETURNS:
-        True - If a "HTTP 200 - OK" is received from Kepware
+        :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-        EXCEPTIONS:
-        KepHTTPError - If urllib provides an HTTPError
-        KepURLError - If urllib provides an URLError
+        :raises KepHTTPError: If urllib provides an HTTPError
+        :raises KepURLError: If urllib provides an URLError
         '''
 
         prop_data = self._force_update_check(force, DATA)
         r = self._config_update(self.url + '/project', prop_data)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
     
     def save_project(self, filename: str, password: str = None, job_ttl: int = None) -> KepServiceResponse:
         '''Executes a ProjectSave Service call to the Kepware instance. This saves 
         a copy of the current project file to disk. The filename
 
-        INPUTS:
-        
-        "filename" - Fully qualified relative file path and name of project file including the file extension.
-        location of project file save defaults: 
+        :param filename: Relative file path and name of project file including the file extension to save.
+        Location of relative project file paths:
+         
                 TKS or KEP (Windows): C:\\PROGRAMDATA\\PTC\\Thingworx Kepware Server\\V6 or 
                                 C:\\PROGRAMDATA\\Kepware\\KEPServerEX\\V6
                 TKE (Linux):    /opt/tkedge/v1/user_data
 
 
-        "password" (optional) - Specify a password with which to load or save an encrypted project file.  
+        :param password: *(optional)* Specify a password with which to  save an encrypted project file with.  
             This password will be required to load this project file.
-        
-        "job_ttl" (optional) - Determines the number of seconds a job instance will exist following completion.
+        :param job_ttl: *(optional)* Determines the number of seconds a job instance will exist following completion.
 
-        RETURNS:
-        KepServiceResponse instance with job information
+        :return: `KepServiceResponse` instance with job information
 
-        EXCEPTIONS (If not HTTP 200 or 429 returned):
-        
-        KepHTTPError - If urllib provides an HTTPError
-        KepURLError - If urllib provides an URLError
+        :raises KepHTTPError: If urllib provides an HTTPError (If not HTTP code 202 [Accepted] or 429 [Too Busy] returned)
+        :raises KepURLError: If urllib provides an URLError
         '''
         url = self.url + self.__project_services_url + '/ProjectSave'
         prop_data = {'servermain.PROJECT_FILENAME': filename}
         if password != None: prop_data['servermain.PROJECT_PASSWORD'] = password
         try:
             job = self._kep_service_execute(url, prop_data, job_ttl)
             return job
@@ -277,30 +250,27 @@
 
     def load_project(self, filename: str, password: str = None, job_ttl: int = None) -> KepServiceResponse:
         '''Executes a ProjectLoad Service call to the Kepware instance. This loads 
         a project file to disk.
 
         INPUTS:
         
-        "filename" - Fully qualified path and name of project file including the file extension. Absolute
-        paths required for TKS and KEP while file path is relative for TKE
-            ex: Windows - filename = C:\\filepath\\test.opf
+        :param filename: Fully qualified or relative path and name of project file including the file extension. Absolute
+        paths required for TKS and KEP while file path is relative for TKE:
+
+                Windows - filename = C:\\filepath\\test.opf
                 Linux - filename = filepath/test.lpf - Location is /opt/tkedge/v1/user_data/filepath/test.lpf
 
-        "password" (optional) - Specify a password with which to load or save an encrypted project file.
-        
-        "job_ttl" (optional) - Determines the number of seconds a job instance will exist following completion.
+        :param password: *(optional)* Specify a password with which to load an encrypted project file.          
+        :param job_ttl: *(optional)* Determines the number of seconds a job instance will exist following completion.
 
-        RETURNS:
-        KepServiceResponse instance with job information
+        :return: `KepServiceResponse` instance with job information
 
-        EXCEPTIONS (If not HTTP 200 or 429 returned):
-        
-        KepHTTPError - If urllib provides an HTTPError
-        KepURLError - If urllib provides an URLError
+        :raises KepHTTPError: If urllib provides an HTTPError (If not HTTP code 202 [Accepted] or 429 [Too Busy] returned)
+        :raises KepURLError: If urllib provides an URLError
         '''
         url = self.url + self.__project_services_url + '/ProjectLoad'
         prop_data = {'servermain.PROJECT_FILENAME': filename}
         if password != None: prop_data['servermain.PROJECT_PASSWORD'] = password
         try:
             job = self._kep_service_execute(url, prop_data, job_ttl)
             return job
@@ -308,24 +278,20 @@
             raise err
 
 
     def service_status(self, resp: KepServiceResponse):
         '''Returns the status of a service job. Used to verify if a service call
         has completed or not.
 
-        INPUT:
-        "resp" - KepServiceResponse instance with job information
+        :param resp: `KepServiceResponse` instance with job information
 
-        RETURNS:
-        KepServiceStatus instance with job status
+        :return: `KepServiceStatus` instance with job status
 
-        EXCEPTIONS:
-        
-        KepHTTPError - If urllib provides an HTTPError
-        KepURLError - If urllib provides an URLError
+        :raises KepHTTPError: If urllib provides an HTTPError
+        :raises KepURLError: If urllib provides an URLError
         '''
         # need to remove part of job href
         loc = resp.href.find(self.__root_url + self.__version_url)
         job_url = resp.href[loc + len(self.__root_url + self.__version_url):]
 
         r = self._config_get(self.url + job_url)
         job = KepServiceStatus(r.payload['servermain.JOB_COMPLETE'],r.payload['servermain.JOB_STATUS'], r.payload['servermain.JOB_STATUS_MSG'])
@@ -333,14 +299,17 @@
 
 
     #Function used to Add an object to Kepware (HTTP POST)
     def _config_add(self, url, DATA):
         '''Conducts an POST method at *url* to add an object in the Kepware Configuration
         *DATA* is required to be a properly JSON object (dict) of the item to be posted to *url* 
         '''
+        if len(DATA) == 0:
+            err_msg = f'Error: Empty List or Dict in DATA | DATA type: {type(DATA)}'
+            raise KepError(err_msg) 
         data = json.dumps(DATA).encode('utf-8')
         url_obj = self.__url_validate(url)
         q = request.Request(url_obj, data, method='POST')
         r = self.__connect(q)
         return r
 
     #Function used to del an object to Kepware (HTTP DELETE)
@@ -362,23 +331,36 @@
         else:
             data = json.dumps(DATA).encode('utf-8')
             q = request.Request(url_obj, data, method='PUT')
         r = self.__connect(q)
         return r
 
     #Function used to Read an object from Kepware (HTTP GET) and return the JSON response
-    def _config_get(self, url):
-        '''Conducts an GET method at *url* to retrieve an objects properties in the Kepware Configuration.'''
+    def _config_get(self, url, *, params = None):
+        '''
+        Conducts an GET method at *url* to retrieve an objects properties with query parameters in 
+        the Kepware Configuration.
+        '''
+        # Add parameters when necessary
+        if params is not None and params != {}:
+            qparams = parse.urlencode(params)
+            url = f'{url}?{qparams}'
         url_obj = self.__url_validate(url)
         q = request.Request(url_obj, method='GET')
         r = self.__connect(q)
         return r
 
     
     def _force_update_check(self, force, DATA):
+        '''
+        This will validate if the modify call needs to be forced or not. If forced, the dict DATA needs
+        to have the 'FORCE_UPDATE' property with a value of True. If forced is not requested, it is necessary
+        to provide the current 'PROJECT_ID'. If 'PROJECT_ID' is not present in DATA, this will automatically 
+        retreive it from the active server.
+        '''
         if force == True:
             DATA['FORCE_UPDATE'] = True
         else:
             # Get Project ID if it doesn't exist and if FORCE_UPDATE is existing and FALSE
             if 'PROJECT_ID' not in DATA:
                 if 'FORCE_UPDATE' in DATA:
                     if 'FORCE_UPDATE' == False:
```

### Comparing `kepconfig-1.1.2/kepconfig/connectivity/channel.py` & `kepconfig-1.2.0/kepconfig/connectivity/channel.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 r"""`channel` exposes an API to allow modifications (add, delete, modify) to 
 channel objects within the Kepware Configuration API
 """
 
  
 import inspect
+from ..connection import server
 from ..error import KepHTTPError, KepError
 from typing import Union
-from. import device
+from . import device
 
 CHANNEL_ROOT = '/project/channels'
 
 def _create_url(channel = None):
     '''Creates url object for the "channel" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
@@ -25,91 +26,75 @@
     '''
     
     if channel == None:
         return CHANNEL_ROOT
     else:
         return '{}/{}'.format(CHANNEL_ROOT,channel)
 
-def add_channel(server, DATA) -> Union[bool, list]:
-    '''Add a "channel" or multiple "channel" objects to Kepware. Can be used to pass children of a channel object 
+def add_channel(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add a `"channel"` or multiple `"channel"` objects to Kepware. Can be used to pass children of a channel object 
     such as devices and tags/tag groups. This allows you to create a channel, it's devices and tags 
     all in one function, if desired.
 
     Additionally it can be used to pass a list of channels and it's children to be added all at once.
 
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "DATA" - properly JSON object (dict) of the channel and it's children
+    :param server: instance of the `server` class
+    :param DATA: Dict of the channel and it's children
     expected by Kepware Configuration API
 
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-    
-    List - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     channels added that failed.
-        
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_add(server.url + _create_url(), DATA)
     if r.code == 201: return True
     elif r.code == 207:
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
     else: 
         raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_channel(server, channel) -> bool:
-    '''Delete a "channel" object in Kepware. This will delete all children as well
+def del_channel(server: server, channel: str) -> bool:
+    '''Delete a `"channel"` object in Kepware. This will delete all children as well
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "channel" - name of channel
+    :param server: instance of the `server` class
+    :param channel: name of channel
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_del(server.url + _create_url(channel))
     if r.code == 200: return True 
     else: 
         raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_channel(server, DATA, channel = None, force = False) -> bool:
-    '''Modify a channel object and it's properties in Kepware. If a "channel" is not provided as an input,
-    you need to identify the channel in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
+def modify_channel(server: server, DATA: dict, *, channel: str = None, force: bool = False) -> bool:
+    '''Modify a channel object and it's properties in Kepware. If a `"channel"` is not provided as an input,
+    you need to identify the channel in the *'common.ALLTYPES_NAME'* property field in `"DATA"`. It will 
     assume that is the channel that is to be modified.
 
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "DATA" - properly JSON object (dict) of the channel properties to be modified.
-
-    "channel" (optional) - name of channel to modify. Only needed if not existing in  "DATA"
-
-    "force" (optional) - if True, will force the configuration update to the Kepware server
+    :param server: instance of the `server` class
+    :param DATA: Dict of the `channel` properties to be modified
+    :param channel: *(optional)* - name of channel to modify. Only needed if not existing in `"DATA"`
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     
     channel_data = server._force_update_check(force, DATA)
     if channel == None:
         try:
             r = server._config_update(server.url + _create_url(channel_data['common.ALLTYPES_NAME']), channel_data)
             if r.code == 200: return True 
@@ -121,90 +106,82 @@
         #     return 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
     else:
         r = server._config_update(server.url + _create_url(channel), channel_data)
         if r.code == 200: return True 
         else: 
             raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_channel(server, channel)  -> dict:
-    '''Returns the properties of the channel object. Returned object is JSON.
+def get_channel(server: server, channel: str)  -> dict:
+    '''Returns the properties of the channel object.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "channel" - name of channel
+    :param server: instance of the `server` class
+    :param channel: name of channel
     
-    RETURNS:
-    dict - data for the channel requested
+    :return: Dict of data for the channel requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_get(server.url + _create_url(channel))
     return r.payload
 
-def get_all_channels(server) -> list:
-    '''Returns list of all channel objects and their properties. Returned object is JSON list.
+def get_all_channels(server: server, *, options: dict = None) -> list:
+    '''Returns list of all channel objects and their properties.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of channels. Options are `filter`, 
+        `sortOrder`, `sortProperty`, `pageNumber`, and `pageSize`
     
-    RETURNS:
-    list - data for the channel requested
+    :return: List of data for all channels in Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
-    r = server._config_get(server.url + _create_url())
+    r = server._config_get(server.url + _create_url(), params= options)
     return r.payload
 
-def get_channel_structure(server, channel) -> dict:
-    '''Returns the properties of "channel" and includes all "devices" and the "tag" and "tag group" objects for a 
+def get_channel_structure(server: server, channel: str) -> dict:
+    '''Returns the properties of `"channel"` and includes all `"devices"` and the `"tag"` and `"tag group"` objects for a 
     channel in Kepware. Returned object is a dict of channel properties including a device list with 
     tag lists and tag group lists.
 
-    The returned object resembles below, nested based on how many 
+    The returned object resembles the example below, nested based on how many 
     levels the tag_group namespace has tags or tag_groups:
 
-    Ex.
-    {
-        channel_properties,
-        'devices: [
-            {
-                device1_properties,
-                'tags': [tag1_dict, tag2_dict,...],
-                'tag_groups':[
-                    {
-                        tag_group1_properties,
-                        'tags': [tag1_dict, tag2_dict,...]
-                        'tag_groups':[sub_group1, subgroup2,...]
-                    }, 
-                    {
-                        tag_group2_properties,
-                        'tags': [tag1_dict, tag2_dict,...]
-                        'tag_groups':[sub_group1, subgroup2,...]
-                    },...]
-            },...]
-    }       
-
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "channel" - name of channel
-
-    RETURNS:
-    dict - data for the device structure requested for "channel"
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    Example return:
+    
+        {
+            channel_properties,
+            'devices: [
+                {
+                    device1_properties,
+                    'tags': [tag1_dict, tag2_dict,...],
+                    'tag_groups':[
+                        {
+                            tag_group1_properties,
+                            'tags': [tag1_dict, tag2_dict,...]
+                            'tag_groups':[sub_group1, subgroup2,...]
+                        }, 
+                        {
+                            tag_group2_properties,
+                            'tags': [tag1_dict, tag2_dict,...]
+                            'tag_groups':[sub_group1, subgroup2,...]
+                        },...]
+                },...]
+        }       
+
+    :param server: instance of the `server` class
+    :param channel: name of channel
+
+    :return: Dict of data for the channel structure requested for `"channel"`
+
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     channel_properties = get_channel(server, channel)
     device_list = device.get_all_devices(server,channel)
     for dev in device_list:
         device_properties = []
         dev_struct = device.get_device_structure(server,channel + '.' + dev['common.ALLTYPES_NAME'])
```

### Comparing `kepconfig-1.1.2/kepconfig/connectivity/device.py` & `kepconfig-1.2.0/kepconfig/connectivity/device.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # --------------------------------------------------------------------------
 
 
 r"""`device` exposes an API to allow modifications (add, delete, modify) to 
 device objects within the Kepware Configuration API
 """
 
-from ..connection import KepServiceResponse
+from ..connection import KepServiceResponse, server
 from ..error import KepHTTPError, KepError
 from typing import Union
 import kepconfig
 from . import channel, tag
 import inspect
 
 DEVICE_ROOT = '/devices'
@@ -26,257 +26,225 @@
     Returns the device specific url when a value is passed as the device name.
     '''
     if device == None:
         return DEVICE_ROOT
     else:
         return '{}/{}'.format(DEVICE_ROOT,device)
 
-def add_device(server, dev_channel, DATA) -> Union[bool, list]:
-    '''Add a "device" object to a channel in Kepware. Can be used to pass children of a device object 
+def add_device(server: server, channel_name: str, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add a `"device"` or multiple `"device"` objects to a channel in Kepware. Can be used to pass children of a device object 
     such as tags and tag groups. This allows you to create a device and tags 
     all in one function, if desired.
 
-    Additionally it can be used to pass a list of channelsdevices and it's children to be added all at once.
+    Additionally it can be used to pass a list of devices and it's children to be added all at once.
 
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "dev_channel" - channel the device object exists
-
-    "DATA" - properly JSON object (dict) of the device and it's children 
+    :param server: instance of the `server` class
+    :param channel_name: channel to add the device object(s)
+    :param DATA: Dict or List of Dicts of the device(s) and it's children
     expected by Kepware Configuration API
     
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-    
-    List  - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     devices added that failed.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
-    r = server._config_add(server.url + channel._create_url(dev_channel) + _create_url(), DATA)
+    r = server._config_add(server.url + channel._create_url(channel_name) + _create_url(), DATA)
     if r.code == 201: return True
     elif r.code == 207:
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
     else: 
         raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_device(server, device_path) -> bool:
-    '''Delete a "device" object in Kepware. This will delete all children as well.
-
-    INPUTS:
-    "server" - instance of the "server" class
+def del_device(server: server, device_path: str) -> bool:
+    '''Delete a `"device"` object in Kepware. This will delete all children as well.
 
-    "device_path" - path identifying device to delete. Standard Kepware address decimal notation string including the 
-    device such as "channel1.device1"
+    :param server: instance of the `server` class
+    :param device_path: path identifying device to delete. Standard Kepware address decimal notation string including the 
+    device such as `"channel1.device1"`
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(device_path)
     try:
         r = server._config_del(server.url + channel._create_url(path_obj['channel']) + _create_url(path_obj['device']))
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
     except KeyError as err:
         err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
 
-def modify_device(server, device_path, DATA, force = False) -> bool:
+def modify_device(server: server, device_path: str, DATA: dict, *, force: bool = False) -> bool:
     '''Modify a device object and it's properties in Kepware.
 
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "device_path" -  path identifying device to modify. Standard Kepware address decimal notation string including the 
-    device such as "channel1.device1"
-
-    "DATA" - properly JSON object (dict) of the device properties to be modified.
-
-    "force" (optional) - if True, will force the configuration update to the Kepware server
+    :param server: instance of the `server` class
+    :param device_path: path identifying device to modffy. Standard Kepware address decimal notation string including the 
+    device such as `"channel1.device1"`
+    :param DATA: Dict of the `device` properties to be modified
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
     
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     device_data = server._force_update_check(force, DATA)
 
     path_obj = kepconfig.path_split(device_path)
     try:
         r = server._config_update(server.url + channel._create_url(path_obj['channel']) + _create_url(path_obj['device']), device_data)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
     except KeyError as err:
             err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
             raise KepError(err_msg)
-    # except Exception as e:
-    #     return 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
 
-def get_device(server, device_path) -> dict:
-    '''Returns the properties of the device object. Returned object is JSON.
+def get_device(server: server, device_path: str) -> dict:
+    '''Returns the properties of the device object.
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "device_path" -  path identifying device. Standard Kepware address decimal notation string including the 
-    device such as "channel1.device1"
+    :param server: instance of the `server` class
+    :param device_path: path identifying device to retrieve properties. Standard Kepware address decimal notation string including the 
+    device such as `"channel1.device1"`
 
-    RETURNS:
-    dict - data for the device requested
+    :return: Dict of data for the device requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(device_path)
     try:
         r = server._config_get(server.url + channel._create_url(path_obj['channel']) + _create_url(path_obj['device']))
         return r.payload
     except KeyError as err:
         err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
     # except Exception as err:
     #     print('Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(err)))
     #     raise err
 
-def get_all_devices(server, dev_channel) -> list:
+def get_all_devices(server: server, channel_name: str, *, options: dict = None) -> list:
     '''Returns list of all device objects and their properties within a channel. Returned object is JSON list.
     
-    INPUTS:
-    "dev_channel" - channel the device object exists
+    :param server: instance of the `server` class
+    :param channel: name of channel
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of devices. Options are `filter`, 
+        `sortOrder`, `sortProperty`, `pageNumber`, and `pageSize`
 
-    RETURNS:
-    list - data for the devices requested
+    :return: List of data for all devices within the channel
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_get(server.url + channel._create_url(dev_channel) + _create_url())
+    r = server._config_get(f'{server.url}{channel._create_url(channel_name)}{_create_url()}', params= options)
     return r.payload
 
-def auto_tag_gen(server, device_path, job_ttl = None) -> KepServiceResponse:
+def auto_tag_gen(server: server, device_path: str, job_ttl: int = None) -> KepServiceResponse:
     '''Executes Auto Tag Generation function on devices that support the feature in Kepware
     
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "device_path" -  path identifying device. Standard Kepware address decimal notation string including the 
-    device such as "channel1.device1"
-
-    "job_ttl" (optional) - Determines the number of seconds a job instance will exist following completion.
+    :param server: instance of the `server` class
+    :param device_path: path identifying device to modffy. Standard Kepware address decimal notation string including the 
+    device such as `"channel1.device1"`
 
-    RETURNS:
-    KepServiceReturn with the result of the service either Code 202 (Accepted) or 429 (Too Busy)
+    :param job_ttl: *(optional)* Determines the number of seconds a job instance will exist following completion.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :return: `KepServiceResponse` instance with job information
+    
+    :raises KepHTTPError: If urllib provides an HTTPError (If not HTTP code 202 [Accepted] or 429 [Too Busy] returned)
+    :raises KepURLError: If urllib provides an URLError
     '''
     
     path_obj = kepconfig.path_split(device_path)
     try:
         url = server.url +channel._create_url(path_obj['channel']) + _create_url(path_obj['device']) + ATG_URL
         job = server._kep_service_execute(url, None, job_ttl)
         return job
     except KeyError as err:
         err_msg = 'Error: No {} identified in {} | Function: {}'.format(err,'device_path', inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
 
-def get_all_tags_tag_groups(server, device_path) -> dict:
-    '''Returns the properties of all "tag" and "tag group" objects for as specific
+def get_all_tags_tag_groups(server: server, device_path: str) -> dict:
+    '''Returns the properties of all `"tag"` and `"tag group"` objects for as specific
     device in Kepware. Returned object is a dict of tag list and tag group list.
 
-    The returned object resembles below, nested based on how many 
+    The returned object resembles the example below, nested based on how many 
     levels the tag_group namespace has tags or tag_groups:
 
-    Ex.
-    {
-        'tags': [tag1_dict, tag2_dict,...],
-        'tag_groups':[
-            {
-                tag_group1_properties,
-                'tags': [tag1_dict, tag2_dict,...]
-                'tag_groups':[sub_group1, subgroup2,...]
-            }, 
-            {
-                tag_group2_properties,
-                'tags': [tag1_dict, tag2_dict,...]
-                'tag_groups':[sub_group1, subgroup2,...]
-            },...]
-    } 
+    Example return:
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "device_path" - path identifying device. Standard Kepware address decimal notation string including the 
-    device such as "channel1.device1"
+        {
+            'tags': [tag1_dict, tag2_dict,...],
+            'tag_groups':[
+                {
+                    tag_group1_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                }, 
+                {
+                    tag_group2_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                },...]
+        } 
+
+    :param server: instance of the `server` class
+    :param device_path: path identifying device to modffy. Standard Kepware address decimal notation string including the 
+    device such as `"channel1.device1"`
 
-    RETURNS:
-    dict - data for the tag structure requested at "device_path" location
+    :return: Dict of data for the tag structure for device requested at `"device_path"` location
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = tag.get_full_tag_structure(server, device_path,recursive=True)
     return r
 
 def get_device_structure(server, device_path) -> dict:
-    '''Returns the properties of "device" and includes all "tag" and "tag group" objects for as specific
+    '''Returns the properties of `"device"` and includes all `"tag"` and `"tag group"` objects for as specific
     device in Kepware. Returned object is a dict of device properties including a tag list and tag group list.
 
-    The returned object resembles below, nested based on how many 
+    The returned object resembles example below, nested based on how many 
     levels the tag_group namespace has tags or tag_groups:
 
-    Ex.
-    {
-        device_properties,
-        'tags': [tag1_dict, tag2_dict,...],
-        'tag_groups':[
-            {
-                tag_group1_properties,
-                'tags': [tag1_dict, tag2_dict,...]
-                'tag_groups':[sub_group1, subgroup2,...]
-            }, 
-            {
-                tag_group2_properties,
-                'tags': [tag1_dict, tag2_dict,...]
-                'tag_groups':[sub_group1, subgroup2,...]
-            },...]
-    } 
-
-    INPUTS:
-    "server" - instance of the "server" class
+    Example return:
     
-    "device_path" - path identifying device. Standard Kepware address decimal notation string including the 
-    device such as "channel1.device1"
+        {
+            device_properties,
+            'tags': [tag1_dict, tag2_dict,...],
+            'tag_groups':[
+                {
+                    tag_group1_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                }, 
+                {
+                    tag_group2_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                },...]
+        } 
+
+    :param server: instance of the `server` class
+    :param device_path: path identifying device to modffy. Standard Kepware address decimal notation string including the 
+    device such as `"channel1.device1"`
 
-    RETURNS:
-    dict - data for the device structure requested at "device_path" location
+    :return: Dict of data for the device structure at `"device_path"` location
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     tags = tag.get_full_tag_structure(server, device_path,recursive=True)
     device_properties = get_device(server,device_path)
     return {**device_properties, **tags}
```

### Comparing `kepconfig-1.1.2/kepconfig/connectivity/egd/range.py` & `kepconfig-1.2.0/kepconfig/connectivity/egd/range.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 r"""`ranges` exposes an API to allow modifications (add, delete, modify) to 
 range objects in exchanges for EGD devices within the Kepware Configuration API
 """
 
 from typing import Union
 from .. import egd as EGD
+from ...connection import server
+from ...error import KepError, KepHTTPError
 
 RANGES_ROOT = '/ranges'
 
 def _create_url(device_path, ex_type, exchange_name, range = None):
     '''Creates url object for the "range" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
@@ -23,160 +25,116 @@
     exchange_root = EGD.exchange._create_url(device_path, ex_type, exchange_name)
 
     if range == None:
         return '{}{}'.format(exchange_root, RANGES_ROOT)
     else:
         return '{}{}/{}'.format(exchange_root, RANGES_ROOT, range)
 
-def add_range(server, device_path, ex_type, exchange_name, DATA) -> Union[bool, list]:
-    '''Add a "range" or multiple "range" objects to Kepware. This allows you to 
+def add_range(server: server, device_path: str, ex_type: str, exchange_name: str, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add a `"range"` or multiple `"range"` objects to Kepware. This allows you to 
     create a range or multiple ranges all in one function, if desired.
 
     When passing multiple ranges, they will be populated in the same order
     in the list sent. Ensure you provide the list in the order desired.
 
-    INPUTS:
+    :param server: instance of the `server` class
+    :param device_path: path to EGD device. Standard Kepware address decimal 
+    notation string such as `"channel1.device1"`
+    :param ex_type: type of exchange, either `CONSUMER` or `PRODUCER`
+    :param exchange_name: name of exchange that range is located
+    :param DATA: Dict or List of Dicts of the range(s) to add
 
-    "server" - instance of the "server" class
-
-    "device_path" - path to exchanges and their ranges. Standard Kepware address decimal 
-    notation string such as "channel1.device1"
-
-    "ex_type" - type of exchange either consumer or producer
-
-    "exchange_name" - name of exchange to add range to
-
-    "DATA" - properly JSON object (dict) of the range or ranges
-
-    RETURNS:
-
-    True - If a "HTTP 201 - Created" is received from Kepware
-    
-    List - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     ranges added that failed.
-
-    False - If a non-expected "2xx successful" code is returned
-
-    EXCEPTIONS:
-
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+        
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_add(server.url + _create_url(device_path, ex_type, exchange_name), DATA)
     if r.code == 201: return True
     elif r.code == 207:
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
-    else: return False
+    else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_range(server, device_path, ex_type, exchange_name, range_name) -> bool:
-    '''Delete a "range" object in Kepware.
+def del_range(server: server, device_path: str, ex_type: str, exchange_name: str, range_name: str) -> bool:
+    '''Delete a `"range"` object in Kepware.
     
-    INPUTS:
-
-    "server" - instance of the "server" class
-
-    "device_path" - path to exchanges and their ranges. Standard Kepware address decimal 
-    notation string such as "channel1.device1"
-
-    "ex_type" - type of exchange either consumer or producer
-
-    "exchange_name" - name of exchange that range is located
-
-    "range_name" - name of range
+    :param server: instance of the `server` class
+    :param device_path: path to EGD device. Standard Kepware address decimal 
+    notation string such as `"channel1.device1"`
+    :param ex_type: type of exchange, either `CONSUMER` or `PRODUCER`
+    :param exchange_name: name of exchange that range is located
+    :param range_name: name of range to delete
     
-    RETURNS:
-
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_del(server.url + _create_url(device_path, ex_type, exchange_name, range_name))
     if r.code == 200: return True 
-    else: return False
+    else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_range(server, device_path, ex_type, exchange_name, DATA, range_name = None, force = False) -> bool:
-    '''Modify a range object and it's properties in Kepware. If a "range_name" is not provided as an input,
-    you need to identify the range in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
+def modify_range(server: server, device_path: str, ex_type: str, exchange_name: str, DATA: dict, *, range_name: str = None, force: bool = False) -> bool:
+    '''Modify a `"range"` object and it's properties in Kepware. If a `"range_name"` is not provided as an input,
+    you need to identify the range in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
     assume that is the range that is to be modified.
 
-    INPUTS:
-
-    "server" - instance of the "server" class
-
-    "device_path" - path to exchanges and their ranges. Standard Kepware address decimal 
-    notation string such as "channel1.device1"
-
-    "ex_type" - type of exchange either consumer or producer
-
-    "exchange_name" - name of exchange that range is located
-
-    "DATA" - properly JSON object (dict) of the range properties to be modified.
-
-    "range_name" (optional) - name of range to modify. Only needed if not existing in  "DATA"
-
-    "force" (optional) - if True, will force the configuration update to the Kepware server
-    
-    RETURNS:
+    :param server: instance of the `server` class
+    :param device_path: path to EGD device. Standard Kepware address decimal 
+    notation string such as `"channel1.device1"`
+    :param ex_type: type of exchange, either `CONSUMER` or `PRODUCER`
+    :param exchange_name: name of exchange that range is located
+    :param DATA: Dict of the range properties to be modified.
+    :param range_name: *(optional)* name of range to to modify. Only needed if not existing in `"DATA"`
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
     
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     
     range_data = server._force_update_check(force, DATA)
     if range_name == None:
         try:
             r = server._config_update(server.url + _create_url(device_path, ex_type, exchange_name, range_data['common.ALLTYPES_NAME']), range_data)
             if r.code == 200: return True 
-            else: return False
+            else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
         except KeyError as err:
-            print('Error: No range identified in DATA | Key Error: {}'.format(err))
-            return False
-        # except Exception as e:
-        #     return 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
+            err_msg = 'Error: No range identified in DATA | Key Error: {}'.format(err)
+            raise KepError(err_msg)
     else:
         r = server._config_update(server.url + _create_url(device_path, ex_type, exchange_name, range_name), range_data)
         if r.code == 200: return True 
-        else: return False
+        else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_range(server, device_path, ex_type, exchange_name, range_name = None) -> Union[dict, list]:
-    '''Returns the properties of the range object or a list of all ranges. Returned object is JSON.
+def get_range(server: server, device_path: str, ex_type: str, exchange_name: str, range_name: str = None, *, options: dict = None) -> Union[dict, list]:
+    '''Returns the properties of the `"range"` object or a list of all ranges.
     
-    INPUTS:
-
-    "server" - instance of the "server" class
-
-    "device_path" - path to exchanges and their ranges. Standard Kepware address decimal 
-    notation string such as "channel1.device1"
-
-    "ex_type" - type of exchange either consumer or producer
-
-    "exchange_name" - name of exchange that range is located
-
-    "range_name" - name of range
+    :param server: instance of the `server` class
+    :param device_path: path to EGD device. Standard Kepware address decimal 
+    notation string such as `"channel1.device1"`
+    :param ex_type: type of exchange, either `CONSUMER` or `PRODUCER`
+    :param exchange_name: name of exchange that range is located
+    :param DATA: Dict of the range properties to be modified.
+    :param range_name: *(optional)* name of range to retrieve. If not defined, get all ranges
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of exchanges. Options are 'filter', 
+    'sortOrder', 'sortProperty', 'pageNumber', and 'pageSize'. Only used when range_name is not defined.
     
-    RETURNS:
-
-    JSON - data for the range requested or a list of ranges and their properties
-
-    EXCEPTIONS:
+    :return: Dict of properties for the range requested or a List of ranges and their properties
 
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     if range_name == None:
-        r = server._config_get(server.url + _create_url(device_path, ex_type, exchange_name))
+        r = server._config_get(f'{server.url}{_create_url(device_path, ex_type, exchange_name)}', params= options)
     else:
-        r = server._config_get(server.url + _create_url(device_path, ex_type, exchange_name, range_name))
+        r = server._config_get(f'{server.url}{_create_url(device_path, ex_type, exchange_name, range_name)}')
     return r.payload
```

### Comparing `kepconfig-1.1.2/kepconfig/connectivity/tag.py` & `kepconfig-1.2.0/kepconfig/connectivity/tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # --------------------------------------------------------------------------
 
 
 r"""`tag` exposes an API to allow modifications (add, delete, modify) to 
 tag and tag group objects within the Kepware Configuration API
 """
 
+from ..connection import server
 from ..error import KepError, KepHTTPError
 from typing import Union
 import kepconfig
 from . import channel, device
 import inspect
 
 TAGS_ROOT = '/tags'
@@ -36,36 +37,29 @@
     Returns the tag group specific url when a value is passed as the tag group name.
     '''
     if tag_group == None:
         return TAG_GRP_ROOT
     else: 
         return '{}/{}'.format(TAG_GRP_ROOT,tag_group)
 
-def add_tag(server, tag_path, DATA) -> Union[bool, list]:
-    '''Add "tag" objects to a specific path in Kepware. To be used to 
-    pass a list of tags to be added at one path location.
+def add_tag(server: server, tag_path: str, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add `"tag"` or multiple `"tag"` objects to a specific path in Kepware. 
+    Can be used to pass a list of tags to be added at one path location.
+
+    :param server: instance of the `server` class
+    :param device_path: path identifying where to add tag(s). Standard Kepware address decimal 
+    notation string that tags exists such as "channel1.device1.tag_group1" or "channel1.device1"
+    :param DATA: Dict or List of Dicts of the tag(s) to add
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "tag_path" -  path identifying location to add tags. Standard Kepware address decimal 
-    notation string such as "channel1.device1.tag_group1"
-    
-    "DATA" - properly JSON object (dict) of the tags 
-    expected by Kepware Configuration API at the "tags" url
-
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-
-    List  - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     tags added that failed.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
@@ -83,37 +77,30 @@
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def add_tag_group(server, tag_group_path, DATA) -> Union[bool, list]:
-    '''Add "tag_group" objects to a specific path in Kepware. To be used to 
-    pass a list of tag_groups and children (tags or tag groups) to be added at one 
+def add_tag_group(server: server, tag_group_path: str, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add `"tag_group"` or multiple `"tag_group"` objects to a specific path in Kepware. 
+    Can be used to pass a list of tag_groups and children (tags or tag groups) to be added at one 
     path location.
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "tag_group_path" - path identifying location to add tag groups. Standard Kepware address decimal 
-    notation string such as "channel1.device1.tag_group1"
-    
-    "DATA" - properly JSON object (dict) of the tag groups
-    and it's children expected by Kepware Configuration API at the "tag_groups" url
+    :param server: instance of the `server` class
+    :param tag_group_path: path identifying where to add tag group(s). Standard Kepware address decimal 
+    notation string that tag groups exists such as "channel1.device1.tag_group1" or "channel1.device1"
+    :param DATA: Dict or List of Dicts of the tag group(s) to add and it's children (tags or tag groups)
 
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-
-    List  - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     tag groups added that failed.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
@@ -131,43 +118,51 @@
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def add_all_tags(server, ch_dev_path, DATA) -> Union[bool, list]:
-    '''Add "tag" and "tag group" objects to a device in Kepware. To be used to 
+def add_all_tags(server: server, ch_dev_path: str, DATA: dict) -> Union[bool, list]:
+    '''Add `"tag"` and `"tag group"` objects to a device in Kepware. To be used to 
     pass a list of tags, tag groups and/or children of tag groups (tags and tag 
-    groups) to be added at once.
-    
-    INPUTS:
-    "server" - instance of the "server" class
+    groups) to be added at once. See example below for required structure with 
+    "tags" and "tag_groups" as keys:
 
-    "ch_dev_path" - path to add tags and tag groups. Standard Kepware address decimal 
-    notation string such as "channel1.device1"
-    
-    "DATA" - properly JSON object (dict) of the tags, 
-    tag groups and it's children expected by Kepware Configuration API.
-    
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware for all items
+    Example DATA:
 
-    List  - [tag failure list, tag group failure list] -   If a "HTTP 207 - Multi-Status" is received from 
-    Kepware for either tags or tag groups, a list of dict error responses for all tags and/or tag groups added that failed. 
+        {
+            'tags': [tag1_dict, tag2_dict,...],
+            'tag_groups':[
+                {
+                    tag_group1_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                }, 
+                {
+                    tag_group2_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                },...]
+        }
+    
+    :param server: instance of the `server` class
+    :param ch_dev_path: device path identifying where to add tags and tag groups. Standard Kepware address decimal 
+    notation string that tag groups exists such as "channel1.device1"
+    :param DATA: Dict of the tags and tag groups to add and it's children (tags or tag groups). 
+
+    
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: List [tag failure list, tag group failure list] - If a "HTTP 207 - Multi-Status" is received from 
+    Kepware for either tags or tag groups, a list of dict error responses for all tags and/or tag groups added that failed.
+    :return: False - If tags or tag groups are not found in DATA
 
-    False - If tags or tag groups are not found in DATA
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-######################################################
-# Need to Handle HTTP 207 from the tag/tag group calls
-######################################################
     
     tags_result = False
     tag_groups_result = False
 
     # check to see if there are dict entries for tags or tag groups
     if ('tag_groups' not in DATA) and ('tags' not in DATA):
         return False
@@ -185,33 +180,27 @@
         return [[], tag_groups_result]
     elif tag_groups_result == True:
         return [tags_result, []]
     else:
         # mixed results from both tags and tag groups
         return [tags_result, tag_groups_result]
 
-def modify_tag(server, full_tag_path, DATA, force = False) -> bool:
-    '''Modify a "tag" object and it's properties in Kepware.
+def modify_tag(server: server, full_tag_path: str, DATA: dict, force: bool = False) -> bool:
+    '''Modify a `"tag"` object and it's properties in Kepware.
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "full_tag_path" - path identifying location and tag to modify. Standard Kepware address decimal 
+    :param server: instance of the `server` class
+    :param full_tag_path: path identifying location and tag to modify. Standard Kepware address decimal 
     notation string including the tag such as "channel1.device1.tag_group1.tag1"
+    :param DATA: Dict of the `tag` properties to be modified
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
 
-    "DATA" - properly JSON object (dict) of the tag properties to be modified.
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    "force" (optional) - if True, will force the configuration update to the Kepware server
-
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     tag_data = server._force_update_check(force, DATA)
 
     path_obj = kepconfig.path_split(full_tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
@@ -224,31 +213,27 @@
     except Exception as e:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
         raise KepError(err_msg)
     r = server._config_update(url, tag_data)
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_tag_group(server, tag_group_path, DATA, force = False) -> bool:
-    '''Modify a "tag group" object and it's properties in Kepware.
-
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "tag_group_path" - path identifying location and tag group to modify. Standard Kepware address decimal 
-    notation string including the tag such as "channel1.device1.tag_group1"
+def modify_tag_group(server: server, tag_group_path: str, DATA: dict, force: bool = False) -> bool:
+    '''Modify a `"tag group"` object and it's properties in Kepware.
 
-    "DATA" is required to be a properly JSON object (dict) of the tag properties to be modified.
+    :param server: instance of the `server` class
+    :param tag_group_path: path identifying location and tag group to modify. Standard Kepware address decimal 
+    notation string that tag groups exists such as "channel1.device1.tag_group1"
+    :param DATA: Dict of the `tag group` properties to be modified
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     tag_group_data = server._force_update_check(force, DATA)
 
     path_obj = kepconfig.path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
@@ -260,29 +245,25 @@
     except Exception as e:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
         raise KepError(err_msg)
     r = server._config_update(url, tag_group_data)
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_tag(server, full_tag_path) -> bool:
-    '''Delete "tag" object at a specific path in Kepware.
+def del_tag(server: server, full_tag_path: str) -> bool:
+    '''Delete `"tag"` object at a specific path in Kepware.
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "full_tag_path" - path identifying location and tag to delete. Standard Kepware address decimal 
+    :param server: instance of the `server` class
+    :param full_tag_path: path identifying location and tag to delete. Standard Kepware address decimal 
     notation string including the tag such as "channel1.device1.tag_group1.tag1"
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(full_tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for x in range(0, len(path_obj['tag_path'])-1):
             url += _create_tag_groups_url(tag_group=path_obj['tag_path'][x])
@@ -293,29 +274,25 @@
     except Exception as e:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
         raise KepError(err_msg)
     r = server._config_del(url)
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_tag_group(server, tag_group_path) -> bool:
-    '''Delete "tag group" object at a specific path in Kepware.
+def del_tag_group(server: server, tag_group_path: str) -> bool:
+    '''Delete `"tag group"` object at a specific path in Kepware.
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "tag_group_path" - path identifying location and tag group to delete. Standard Kepware address decimal 
-    notation string such as "channel1.device1.tag_group1"
+    :param server: instance of the `server` class
+    :param tag_group_path: path identifying location and tag group to delete. Standard Kepware address decimal 
+    notation string that tag groups exists such as "channel1.device1.tag_group1"
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for tg in path_obj['tag_path']:
             url += _create_tag_groups_url(tag_group=tg)
@@ -325,30 +302,25 @@
     except Exception as err:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(err))
         raise KepError(err_msg)
     r = server._config_del(url)
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_tag(server, full_tag_path) -> dict:
-    '''Returns the properties of the "tag" object at a specific path in Kepware. 
-    Returned object is JSON. 
+def get_tag(server: server, full_tag_path: str) -> dict:
+    '''Returns the properties of the `"tag"` object at a specific path in Kepware. 
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "full_tag_path" - path identifying tag. Standard Kepware address decimal 
+    :param server: instance of the `server` class
+    :param full_tag_path: path identifying location and tag to delete. Standard Kepware address decimal 
     notation string including the tag such as "channel1.device1.tag_group1.tag1"
 
-    RETURNS:
-    dict - data for the tag requested
+    :return: Dict of data for the tag requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(full_tag_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for x in range(0, len(path_obj['tag_path'])-1):
             url += _create_tag_groups_url(tag_group=path_obj['tag_path'][x])
@@ -358,64 +330,57 @@
         raise KepError(err_msg)
     except Exception as e:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
         raise KepError(err_msg)
     r = server._config_get(url)
     return r.payload
 
-def get_all_tags(server, full_tag_path) -> list:
-    '''Returns the properties of all "tag" object at a specific path in Kepware. 
-    Returned object is JSON list.
+def get_all_tags(server: server, full_tag_path: str, *, options: dict = None) -> list:
+    '''Returns the properties of all `"tag"` object at a specific path in Kepware. 
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "full_tag_path" - path identifying location to retreive tag list. Standard Kepware address decimal 
-    notation string including the tag such as "channel1.device1.tag_group1"
+    :param server: instance of the `server` class
+    :param full_tag_path: path identifying location to retreive tag list. Standard Kepware address decimal 
+    notation string including the tag such as "channel1.device1.tag_group1.tag1"
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of tags. Options are `filter`, 
+        `sortOrder`, `sortProperty`, `pageNumber`, and `pageSize`
     
-    RETURNS:
-    list - data for the tags requested
+    :return: List of data for all tags
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     path_obj = kepconfig.path_split(full_tag_path)
     try:
-        url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
+        url = f"{server.url}{channel._create_url(path_obj['channel'])}{device._create_url(path_obj['device'])}"
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
                 url += _create_tag_groups_url(tag_group=tg)
         url += _create_tags_url()
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
     except Exception as e:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
         raise KepError(err_msg)
-    r = server._config_get(url)
+    r = server._config_get(url, params= options)
     return r.payload
 
-def get_tag_group(server, tag_group_path) -> dict:
+def get_tag_group(server: server, tag_group_path: str) -> dict:
     '''Returns the properties of the "tag group" object at a specific 
     path in Kepware. Returned object is JSON.
 
-    INPUTS:
-    "server" - instance of the "server" class 
-    
-    "tag_group_path" - path identifying tag group. Standard Kepware address decimal 
-    notation string such as "channel1.device1.tag_group1"
+    :param server: instance of the `server` class
+    :param tag_group_path: path identifying location and tag group to retrieve properties. Standard Kepware address decimal 
+    notation string that tag groups exists such as "channel1.device1.tag_group1"
 
-    RETURNS:
-    dict - data for the tag group requested
+    :return: Dict of data for the tag group requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     path_obj = kepconfig.path_split(tag_group_path)
     try:
         url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
         for tg in path_obj['tag_path']:
             url += _create_tag_groups_url(tag_group=tg)
     except KeyError as err:
@@ -423,93 +388,98 @@
         raise KepError(err_msg)
     except Exception as e:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
         raise KepError(err_msg)
     r = server._config_get(url)
     return r.payload
 
-def get_all_tag_groups(server, tag_group_path) -> list:
-    '''Returns the properties of all "tag group" objects at a specific 
-    path in Kepware. Returned object is JSON list. 
+def get_all_tag_groups(server:server, tag_group_path: str, *, options: dict = None) -> list:
+    '''Returns the properties of all `"tag group"` objects at a specific 
+    path in Kepware.
+
+    :param server: instance of the `server` class
+    :param tag_group_path: path identifying location to retrieve tag group list and properties. Standard Kepware address decimal 
+    notation string that tag groups exists such as "channel1.device1.tag_group1"
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of devices. Options are `filter`, 
+        `sortOrder`, `sortProperty`, `pageNumber`, and `pageSize`
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "tag_group_path" - path identifying location to retreive tag group list. Standard Kepware address decimal 
-    notation string such as "channel1.device1.tag_group1"
-
-    RETURNS:
-    list - data for the tag groups requested
+    :return: List of data for all tag groups
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     path_obj = kepconfig.path_split(tag_group_path)
     try:
-        url = server.url+channel._create_url(path_obj['channel'])+device._create_url(path_obj['device'])
+        url = f"{server.url}{channel._create_url(path_obj['channel'])}{device._create_url(path_obj['device'])}"
         if 'tag_path' in path_obj:
             for tg in path_obj['tag_path']:
                 url += _create_tag_groups_url(tag_group=tg)
         url += _create_tag_groups_url()
     except KeyError as err:
         err_msg = 'Error: No key {} identified | Function: {}'.format(err, inspect.currentframe().f_code.co_name)
         raise KepError(err_msg)
     except Exception as e:
         err_msg = 'Error: Error with {}: {}'.format(inspect.currentframe().f_code.co_name, str(e))
         raise KepError(err_msg)
-    r = server._config_get(url)
+    r = server._config_get(url, params= options)
     return r.payload
 
-def get_full_tag_structure(server, path, recursive = False) -> dict:
-    '''Returns the properties of all "tag" and "tag group" objects at a specific 
+def get_full_tag_structure(server: server, path: str, *, recursive: bool = False, options: dict = None) -> dict:
+    '''Returns the properties of all `"tag"` and `"tag group"` objects at a specific 
     path in Kepware. Returned object is a dict of tag list and tag group list.
 
-    Ex.
-    {
-        'tags': [tag1_dict, tag2_dict,...],
-        'tag_groups':[tag_group1_dict, tag_group2_dict,...]
-    } 
+    Example:
 
-    If recursive is TRUE, then the call will iterate through all tag groups and get the tags and 
+        {
+            'tags': [tag1_dict, tag2_dict,...],
+            'tag_groups':[tag_group1_dict, tag_group2_dict,...]
+        } 
+
+    If `recursive` is TRUE, then the call will iterate through all tag groups and get the tags and 
     tag groups of all tag group children.This would be the equivilant of asking for all tags and tag groups
-    that exist below the "path" location. The returned object would look like below, nested based on how many 
+    that exist below the `"path"` location. The returned object would look like below, nested based on how many 
     levels the tag_group namespace has tags or tag_groups:
 
-    Ex.
-    {
-        'tags': [tag1_dict, tag2_dict,...],
-        'tag_groups':[
-            {
-                tag_group1_properties,
-                'tags': [tag1_dict, tag2_dict,...]
-                'tag_groups':[sub_group1, subgroup2,...]
-            }, 
-            {
-                tag_group2_properties,
-                'tags': [tag1_dict, tag2_dict,...]
-                'tag_groups':[sub_group1, subgroup2,...]
-            },...]
-    } 
+    Example with Recursive True:
 
-    INPUTS:
-    "server" - instance of the "server" class
-    
-    "path" - path identifying location to retreive the tag structure. Standard Kepware address decimal 
+        {
+            'tags': [tag1_dict, tag2_dict,...],
+            'tag_groups':[
+                {
+                    tag_group1_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                }, 
+                {
+                    tag_group2_properties,
+                    'tags': [tag1_dict, tag2_dict,...]
+                    'tag_groups':[sub_group1, subgroup2,...]
+                },...]
+        } 
+
+    :param server: instance of the `server` class
+    :param path: path identifying location to retreive the tag structure. Standard Kepware address decimal 
     notation string such as "channel1.device1.tag_group1" and must container at least the channel and device.
+    :param recursive: *(optional)* If True, returns structures within the tag groups found and all of their 
+    children. (default= False)
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of tags and tag groups. 
+    Options are 'filter', 'sortOrder', and 'sortProperty' only.
 
-    RETURNS:
-    dict - data for the tag structure requested at "path" location
+    :return: Dict of data for the tag structure requested at "path" location
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     r = {}
         
-    r['tags'] = get_all_tags(server, path)
-    r['tag_groups'] = get_all_tag_groups(server, path)
+    # Remove pagination options, if present. Not useful with this method since it is designed to get the full tree of items.
+    if options is not None:
+        remove_list = ['pageNumber','pageSize']
+        [options.pop(x) for x in remove_list]
+    
+    r['tags'] = get_all_tags(server, path, options= options)
+    r['tag_groups'] = get_all_tag_groups(server, path, options= options)
     if recursive:
         for group in r['tag_groups']:
-            res = get_full_tag_structure(server, path + '.' + group['common.ALLTYPES_NAME'])
+            res = get_full_tag_structure(server, path + '.' + group['common.ALLTYPES_NAME'], options= options)
             group.update(res)
     return r
```

### Comparing `kepconfig-1.1.2/kepconfig/datalogger/log_group.py` & `kepconfig-1.2.0/kepconfig/datalogger/log_group.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # license information.
 # --------------------------------------------------------------------------
 
 r"""`log_group` exposes an API to allow modifications (add, delete, modify) to 
 log group objects in DataLogger within the Kepware Configuration API
 """
 from typing import Union
-from ..connection import KepServiceResponse
+from ..connection import KepServiceResponse, server
 from ..error import KepError, KepHTTPError
 
 ENABLE_PROPERTY = 'datalogger.LOG_GROUP_ENABLED'
 LOG_GROUP_ROOT = '/project/_datalogger/log_groups'
 SERVICES_ROOT = '/services'
 def _create_url(log_group = None):
     '''Creates url object for the "log_group" branch of Kepware's project tree. Used 
@@ -23,184 +23,151 @@
 
     if log_group == None:
         return '{}'.format(LOG_GROUP_ROOT)
     else:
         return '{}/{}'.format(LOG_GROUP_ROOT, log_group)
 
 
-def add_log_group(server, DATA) -> Union[bool, list]:
-    '''Add a "log group" or multiple "log groups" objects to Kepware's DataLogger. It can be used 
+def add_log_group(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add a `"log group"` or multiple `"log groups"` objects to Kepware's DataLogger. It can be used 
     to pass a list of log groups to be added all at once.
 
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param DATA: Dict or a list of the log groups to add through Kepware Configuration API
 
-    *DATA* - properly JSON object (dict) of the log group expected by Kepware Configuration API
-
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-
-    List - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     log groups added that failed.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_add(server.url + _create_url(), DATA)
     if r.code == 201: return True 
     elif r.code == 207:
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_log_group(server, log_group) -> bool:
-    '''Delete a "log group" object in Kepware's Datalogger.
+def del_log_group(server: server, log_group: str) -> bool:
+    '''Delete a `"log group"` object in Kepware's Datalogger.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "log_group" - name of log group
+    :param server: instance of the `server` class
+    :param log_group: name of log group to delete
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     r = server._config_del(server.url + _create_url(log_group))
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_log_group(server, DATA, log_group = None, force = False) -> bool:
-    '''Modify a log group object and it's properties in Kepware's Datalogger. If a "log group" is not provided as an input,
-    you need to identify the log group in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
+def modify_log_group(server: server, DATA: dict, *, log_group: str = None, force: bool = False) -> bool:
+    '''Modify a `"log group"` object and it's properties in Kepware's Datalogger. If a `"log group"` is not provided as an input,
+    you need to identify the log group in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
     assume that is the log group that is to be modified.
 
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "DATA" - properly JSON object (dict) of the agent properties to be modified
-
-    "log_group" (optional) - name of log group. Only needed if not existing in "DATA"
+    :param server: instance of the `server` class
+    :param DATA: Dict of the log group properties to be modified.
+    :param log_group: *(optional)* name of log group to modify. Only needed if not existing in `"DATA"`
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
 
-    "force" (optional) - if True, will force the configuration update to the Kepware server
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     
     log_group_data = server._force_update_check(force, DATA)
     
     if log_group == None:
         try:
             r = server._config_update(server.url + _create_url(log_group_data['common.ALLTYPES_NAME']), log_group_data)
             if r.code == 200: return True 
             else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
         except KeyError as err:
             err_msg = 'Error: No log group identified in DATA | Key Error: {}'.format(err)
             raise KepError(err_msg)
-        # except:
-        #     return 'Error: Error with {}'.format(inspect.currentframe().f_code.co_name)
     else:
         r = server._config_update(server.url + _create_url(log_group), log_group_data)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_log_group(server, log_group) -> dict:
-    '''Returns the properties of the log group object. Returned object is JSON.
+def get_log_group(server: server, log_group: str) -> dict:
+    '''Returns the properties of the `"log group"` object.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "log_group" - name of log group
+    :param server: instance of the `server` class
+    :param log_group: name of log group to retrieve
 
-    RETURNS:
-    dict - data for the log group requested
+    :return: Dict of properties for the log group requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     r = server._config_get(server.url + _create_url(log_group))
     return r.payload
 
-def get_all_log_groups(server) -> list:
+def get_all_log_groups(server: server, *, options: dict = None) -> list:
     '''Returns the properties of all log group objects for Kepware's Datalogger. Returned object is JSON list.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of log groups. Options are 'filter', 
+    'sortOrder', 'sortProperty', 'pageNumber', and 'pageSize'. Only used when exchange_name is not defined.
 
-    RETURNS:
-    list - data for the log groups requested
+    :return: list of properties for all log groups requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_get(server.url + _create_url())
+    r = server._config_get(f'{server.url}{_create_url()}', params= options)
     return r.payload
 
-def enable_log_group(server, log_group) -> bool:
-    '''Enable the log group. Returned object is JSON.
+def enable_log_group(server: server, log_group: str) -> bool:
+    '''Enable the `"log group"`.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "log_group" - name of log group
+    :param server: instance of the `server` class
+    :param log_group: name of log group to enable
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     DATA = {ENABLE_PROPERTY: True}
-    return modify_log_group(server, DATA, log_group)
+    return modify_log_group(server, DATA, log_group= log_group)
 
-def disable_log_group(server, log_group) -> bool:
+def disable_log_group(server: server, log_group: str) -> bool:
     '''Disable the log group. Returned object is JSON.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param log_group: name of log group to enable
 
-    "log_group" - name of log group
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     DATA = {ENABLE_PROPERTY: False}
-    return modify_log_group(server, DATA, log_group)
+    return modify_log_group(server, DATA, log_group= log_group)
 
-def reset_column_mapping_service(server, log_group, job_ttl = None) -> KepServiceResponse:
+def reset_column_mapping_service(server: server, log_group: str, job_ttl: int = None) -> KepServiceResponse:
     '''Executes a ResetColumnMapping serivce call to the log group
 
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "log_group" - name of log group
+    :param server: instance of the `server` class
+    :param log_group: name of log group to enable
+    :param job_ttl: *(optional)* Determines the number of seconds a job instance will exist following completion.
 
-    RETURNS:
-    KepServiceResponse instance with job information
+    :return: `KepServiceResponse` instance with job information
     
-    EXCEPTIONS (If not HTTP 200 or 429 returned):
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError (If not HTTP code 202 [Accepted] or 429 [Too Busy] returned)
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     url = server.url + _create_url(log_group) + SERVICES_ROOT + '/ResetColumnMapping'
     job = server._kep_service_execute(url, None, job_ttl)
     return job
```

### Comparing `kepconfig-1.1.2/kepconfig/datalogger/mapping.py` & `kepconfig-1.2.0/kepconfig/datalogger/mapping.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 r"""`mapping` exposes an API to allow modifications (add, delete, modify) to 
 column mapping objects in a Datalogger log group within the Kepware Configuration API
 """
 
 from . import log_group as Log_Group
 from ..error import KepError, KepHTTPError
+from ..connection import server
 
 MAPPING_ROOT = '/column_mappings'
 
 def _create_url(mapping = None):
     '''Creates url object for the "column_mappings" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
@@ -21,85 +22,69 @@
     '''
 
     if mapping == None:
         return '{}'.format(MAPPING_ROOT)
     else:
         return '{}/{}'.format(MAPPING_ROOT, mapping)
 
-def modify_mapping(server, log_group, DATA, mapping = None, force = False) -> bool:
-    '''Modify a column mapping object and it's properties in Kepware. If a "mapping" is not provided as an input,
-    you need to identify the column mapping in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
+def modify_mapping(server: server, log_group: str, DATA: dict, *, mapping: str = None, force: bool = False) -> bool:
+    '''Modify a column `"mapping"` object and it's properties in Kepware. If a `"mapping"` is not provided as an input,
+    you need to identify the column mapping in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
     assume that is the column mapping that is to be modified.
 
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the mapping
+    :param DATA: Dict of the mapping properties to be modified.
+    :param mapping: *(optional)* column mapping to modify in the log group. Only needed if not existing in `"DATA"`
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
 
-    "log_group" - name of log group that mapping exists
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    "DATA" - properly JSON object (dict) of the agent properties to be modified
-
-    "mapping" (optional) - column mapping to modify in the log group. Only needed if not existing in "DATA"
-
-    "force" (optional) - if True, will force the configuration update to the Kepware server
-
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     
     mapping_data = server._force_update_check(force, DATA)
     
     if mapping == None:
         try:
             r = server._config_update(server.url + Log_Group._create_url(log_group) + _create_url(mapping_data['common.ALLTYPES_NAME']), mapping_data)
             if r.code == 200: return True 
             else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
         except KeyError as err:
             err_msg = 'Error: No column mapping identified in DATA | Key Error: {}'.format(err)
             raise KepError(err_msg)
-        # except:
-        #     return 'Error: Error with {}'.format(inspect.currentframe().f_code.co_name)
     else:
         r = server._config_update(server.url + Log_Group._create_url(log_group) + _create_url(mapping), mapping_data)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_mapping(server, log_group, mapping) -> dict:
-    '''Returns the properties of the mapping object. Returned object is JSON.
+def get_mapping(server: server, log_group: str, mapping: str) -> dict:
+    '''Returns the properties of the `"mapping"` object.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "log_group" - name of log group that mapping exists
-
-    "mapping" - name of column mapping to retrieve properties for
-
-    RETURNS:
-    dict - data for the column mapping requested
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the mapping
+    :param mapping: name of column mapping to retrieve properties
+    
+    :return: Dict of properties for the mapping object requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     r = server._config_get(server.url + Log_Group._create_url(log_group) + _create_url(mapping))
     return r.payload
 
-def get_all_mappings(server, log_group) -> list:
-    '''Returns the properties of all column mapping objects for a log group. Returned object is JSON list.
+def get_all_mappings(server: server, log_group: str, *, options: dict = None) -> list:
+    '''Returns the properties of all column `"mapping"` objects for a log group.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "log_group" - name of log group
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the mapping
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of mapping items. Options are 'filter', 
+    'sortOrder', 'sortProperty', 'pageNumber', and 'pageSize'. Only used when exchange_name is not defined.
 
-    RETURNS:
-    list - data for the column mappings requested
+    :return: list of properties for all mapping items in the log group requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_get(server.url + Log_Group._create_url(log_group) + _create_url())
+    r = server._config_get(f'{server.url}{Log_Group._create_url(log_group)}{_create_url()}', params= options)
     return r.payload
```

### Comparing `kepconfig-1.1.2/kepconfig/datalogger/triggers.py` & `kepconfig-1.2.0/kepconfig/datalogger/triggers.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 r"""`triggers` exposes an API to allow modifications (add, delete, modify) to 
 trigger objects in a Datalogger log group within the Kepware Configuration API
 """
 
 from typing import Union
 from . import log_group as Log_Group
 from ..error import KepError, KepHTTPError
+from ..connection import server
 
 TRIGGERS_ROOT = '/triggers'
 
 def _create_url(trigger = None):
     '''Creates url object for the "trigger" branch of Kepware's project tree. Used 
     to build a part of Kepware Configuration API URL structure
 
@@ -23,89 +24,71 @@
 
     if trigger == None:
         return '{}'.format(TRIGGERS_ROOT)
     else:
         return '{}/{}'.format(TRIGGERS_ROOT, trigger)
 
 
-def add_trigger(server, log_group, DATA) -> Union[bool, list]:
-    '''Add a "trigger" or multiple "trigger" objects to a log group in Kepware's Datalogger. It can 
+def add_trigger(server: server, log_group: str, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add a `"trigger"` or multiple `"trigger"` objects to a log group in Kepware's Datalogger. It can 
     be used to pass a list of triggers to be added all at once.
 
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the trigger items
+    :param DATA: Dict or a list of the trigger items to add through Kepware Configuration API
 
-    "log_group" - name of log group that the triggers will be added
-
-    *DATA* - properly JSON object (dict) of the trigger expected by Kepware Configuration API
-
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
-
-    List - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
     triggers added that failed.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
 
     r = server._config_add(server.url + Log_Group._create_url(log_group) + _create_url(), DATA)
     if r.code == 201: return True
     elif r.code == 207:
         errors = [] 
         for item in r.payload:
             if item['code'] != 201:
                 errors.append(item)
         return errors 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_trigger(server, log_group, trigger) -> bool:
-    '''Delete a "trigger" object of a log group in Kepware's Datalogger.
+def del_trigger(server: server, log_group: str, trigger: str) -> bool:
+    '''Delete a `"trigger"` object of a log group in Kepware's Datalogger.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the trigger items
+    :param trigger: name of trigger to delete
 
-    "log_group" - name of log group that trigger exists
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    "trigger" - name of trigger to delete
-
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     r = server._config_del(server.url + Log_Group._create_url(log_group) + _create_url(trigger))
     if r.code == 200: return True
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_trigger(server, log_group, DATA, trigger = None, force = False)  -> bool:
-    '''Modify a trigger object and it's properties in Kepware. If a "trigger" is not provided as an input,
-    you need to identify the trigger in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
+def modify_trigger(server: server, log_group: str, DATA: dict, *, trigger: str = None, force: bool = False)  -> bool:
+    '''Modify a `"trigger"` object and it's properties in Kepware. If a `"trigger"` is not provided as an input,
+    you need to identify the trigger in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
     assume that is the trigger that is to be modified.
 
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "log_group" - name of log group that trigger exists
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the trigger items
+    :param DATA: Dict of the trigger properties to be modified.
+    :param trigger: *(optional)* name of trigger to modify in the log group. Only needed if not existing in `"DATA"`
+    :param force: *(optional)* if True, will force the configuration update to the Kepware server
 
-    "DATA" - properly JSON object (dict) of the agent properties to be modified
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    "trigger" (optional) - trigger to modify in the log group. Only needed if not existing in "DATA"
-
-    "force" (optional) - if True, will force the configuration update to the Kepware server
-
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     
     trigger_data = server._force_update_check(force, DATA)
     
     if trigger == None:
         try:
             r = server._config_update(server.url + Log_Group._create_url(log_group) + _create_url(trigger_data['common.ALLTYPES_NAME']), trigger_data)
@@ -118,43 +101,41 @@
         #     return 'Error: Error with {}'.format(inspect.currentframe().f_code.co_name)
     else:
         r = server._config_update(server.url + Log_Group._create_url(log_group) + _create_url(trigger), trigger_data)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
 def get_trigger(server, log_group, trigger) -> dict:
-    '''Returns the properties of the trigger object. Returned object is JSON.
+    '''Returns the properties of the `"trigger"` object.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the trigger items
+    :param trigger: name of trigger to retrieve
 
-    "log_group" - name of log group that trigger exists
+    :return: Dict of properties for the trigger requested
 
-    "trigger" - name of trigger to retrieve properties for
-
-    RETURNS:
-    dict - data for the trigger requested
-
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
     r = server._config_get(server.url + Log_Group._create_url(log_group) + _create_url(trigger))
     return r.payload
 
-def get_all_triggers(server, log_group) -> list:
-    '''Returns the properties of all trigger objects for a log group. Returned object is JSON list.
+def get_all_triggers(server: server, log_group: str, *, options: dict = None) -> list:
+    '''Returns the properties of all `"trigger"` objects for a log group.
     
-    INPUTS:
-    "server" - instance of the "server" class
+    :param server: instance of the `server` class
+    :param log_group: name of log group for the trigger items
+
+    :return: Dict of properties for the trigger requested
 
-    "log_group" - name of log group
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of triggers. Options are 'filter', 
+    'sortOrder', 'sortProperty', 'pageNumber', and 'pageSize'. Only used when exchange_name is not defined.
 
-    RETURNS:
-    list - data for the triggers requested
+    :return: list of properties for all triggers in the log group requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_get(server.url + Log_Group._create_url(log_group) + _create_url())
+    r = server._config_get(f'{server.url}{Log_Group._create_url(log_group)}{_create_url()}', params= options)
     return r.payload
```

### Comparing `kepconfig-1.1.2/kepconfig/error.py` & `kepconfig-1.2.0/kepconfig/error.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,41 +10,52 @@
 """
 
 __all__ = ['KepError', 'KepURLError', 'KepHTTPError']
 
 
 class KepError(Exception):
     '''General Exception class for Kepconfig.
+    
+    :param msg: General error message returned in string format.
     '''
     def __init__(self, msg):
         self.msg = msg
 
     def __str__(self):
             return 'KepError Error: %s' % (self.msg)
 
 class KepURLError(KepError):
-    '''Exception class raised by Kepconfig that inherits responses from the urllib URLError exceptions.
+    '''Exception class raised by Kepconfig that derives responses from the urllib URLError exceptions.
+
+    :param url: full url path of the request that flagged a URLError exception
+    :param msg: reason parameter in URLError exception
     '''
     def __init__(self, url=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.url = url
     
     @property
     def reason(self):
         return self.msg
 
     def __str__(self):
         return '<urlopen error %s>' % self.reason
 
 class KepHTTPError(KepError):
-    '''Exception class raised by Kepconfig that inherits responses from the urllib HTTPError 
+    '''Exception class raised by Kepconfig that derives responses from the urllib HTTPError 
     exceptions. This exception class is also a valid HTTP response instance.  It behaves 
     this way because HTTP protocol errors are valid responses, with a status 
-    code, headers, and a body.  In some contexts,an application may want to 
+    code, headers, and a body.  In some contexts, an application may want to 
     handle an exception like a regular response.
+
+    :param url: url parameter in HTTPError exception
+    :param code: HTTP response code parameter in HTTPError exception
+    :param hdrs: hdrs parameter in HTTPError exception
+    :param payload: string of HTTP response payload that flagged HTTPError exception 
+    :param msg: msg parameter in HTTPError exception
     '''
     def __init__(self, url=None, code=None, hdrs=None, payload=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.url = url
         self.code = code
         self.hdrs = hdrs
         self.payload = payload
```

### Comparing `kepconfig-1.1.2/kepconfig/iot_gateway/iot_items.py` & `kepconfig-1.2.0/kepconfig/admin/ua_server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,127 @@
 # -------------------------------------------------------------------------
-# Copyright (c) PTC Inc. and/or all its affiliates. All rights reserved.
+# Copyright (c), PTC Inc. and/or all its affiliates. All rights reserved.
 # See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
-
-r"""`iot_items` exposes an API to allow modifications (add, delete, modify) to 
-iot_items objects within the Kepware Configuration API
+r"""`ua_server` exposes an API to allow modifications (add, delete, modify) to 
+OPC UA Server endpoints within the Kepware Administration through the Kepware Configuration API
 """
-
 from typing import Union
-import kepconfig as helper
-from .. import iot_gateway as IOT
-from ..error import KepError, KepHTTPError
-
-IOT_ITEMS_ROOT = '/iot_items'
+from ..error import KepHTTPError, KepError
+from ..connection import server
 
-def _create_url(tag = None):
-    '''Creates url object for the "iot items" branch of Kepware's IoT Agents property model. Used 
-    to build a part of Kepware Configuration API URL structure
-    
-    Returns the device specific url when a value is passed as the iot item name.
-    '''
-    if tag == None:
-        return IOT_ITEMS_ROOT
-    else: 
-        normalized_tag = helper._address_dedecimal(tag)
-        return '{}/{}'.format(IOT_ITEMS_ROOT,normalized_tag)
 
+UA_ROOT = '/admin/ua_endpoints'
 
-def add_iot_item(server, DATA, agent, agent_type) -> Union[bool, list]:
-    '''Add a "iot item" or multiple "iot item" objects to Kepware's IoT Gateway agent. Additionally 
-    it can be used to pass a list of iot items to be added to an agent all at once.
-
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "DATA" - properly JSON object (dict) of the iot item or list of items
-    expected by Kepware Configuration API.
+def _create_url(endpoint = None):
+    '''Creates url object for the "server_users" branch of Kepware's project tree. Used 
+    to build a part of Kepware Configuration API URL structure
 
-    "agent" - name of IoT Agent
+    Returns the user specific url when a value is passed as the user name.
+    '''
+    
+    if endpoint == None:
+        return UA_ROOT
+    else:
+        return '{}/{}'.format(UA_ROOT,endpoint)
 
-    "agent_type" - agent type
+def add_endpoint(server: server, DATA: Union[dict, list]) -> Union[bool, list]:
+    '''Add an `"endpoint"` or multiple `"endpoint"` objects to Kepware UA Server by passing a 
+    list of endpoints to be added all at once.
 
-    RETURNS:
-    True - If a "HTTP 201 - Created" is received from Kepware
+    :param server: instance of the `server` class
+    :param DATA: Dict or List of Dicts of the UA Endpoints to add
 
-    List - If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
-    iot items added that failed.
+    :return: True - If a "HTTP 201 - Created" is received from Kepware server
+    :return: If a "HTTP 207 - Multi-Status" is received from Kepware with a list of dict error responses for all 
+    endpoints added that failed.
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_add(server.url + IOT.agent._create_url(agent_type, agent) + _create_url(), DATA)
+
+    r = server._config_add(server.url + _create_url(), DATA)
     if r.code == 201: return True
     elif r.code == 207:
-            errors = [] 
-            for item in r.payload:
-                if item['code'] != 201:
-                    errors.append(item)
-            return errors 
+        errors = [] 
+        for item in r.payload:
+            if item['code'] != 201:
+                errors.append(item)
+        return errors
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def del_iot_item(server, iot_item, agent, agent_type) -> bool:
-    '''Delete a "iot item" object in Kepware.
-
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "iot_item" - IoT item to delete
-
-    "agent" - name of IoT Agent
-
-    "agent_type" - agent type 
-
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+def del_endpoint(server: server, endpoint: str) -> bool:
+    '''Delete an `"endpoint"` object in Kepware UA Server
+    
+    :param server: instance of the `server` class
+    :param endpoint: name of endpoint to delete
+    
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_del(server.url + IOT.agent._create_url(agent_type, agent) + _create_url(iot_item))
+
+    r = server._config_del(server.url + _create_url(endpoint))
     if r.code == 200: return True 
     else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def modify_iot_item(server, DATA, agent, agent_type, iot_item = None, force = False) -> bool:
-    '''Modify a iot item object and it's properties in Kepware. If a "iot item" is not provided as an input,
-    you need to identify the iot item in the 'common.ALLTYPES_NAME' property field in the "DATA". It will 
-    assume that is the iot item that is to be modified.
-
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "DATA" - properly JSON object (dict) of the iot item properties to be modified.
-
-    "agent" - name of IoT Agent
-
-    "agent_type" - agent type 
-
-    "iot_item" (optional) - IoT item to modify
-
-    "force" (optional) - if True, will force the configuration update to the Kepware server
-
-    RETURNS:
-    True - If a "HTTP 200 - OK" is received from Kepware
+def modify_endpoint(server: server, DATA: dict, endpoint: str = None) -> bool:
+    '''Modify a `"endpoint"` object and it's properties in Kepware UA Server. If a `"endpoint"` is not provided as an input,
+    you need to identify the endpoint in the *'common.ALLTYPES_NAME'* property field in the `"DATA"`. It will 
+    assume that is the endpoint that is to be modified.
+
+    :param server: instance of the `server` class
+    :param DATA: Dict of the UA endpoint properties to be modified.
+    :param endpoint: *(optional)* name of endpoint to modify. Only needed if not existing in `"DATA"`
+    
+    :return: True - If a "HTTP 200 - OK" is received from Kepware server
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    
-    agent_data = server._force_update_check(force, DATA)
-    if iot_item == None:
+
+    if endpoint == None:
         try:
-            r = server._config_update(server.url + IOT.agent._create_url(agent_type, agent) + _create_url(agent_data['common.ALLTYPES_NAME']), agent_data)
+            r = server._config_update(server.url + _create_url(DATA['common.ALLTYPES_NAME']), DATA)
             if r.code == 200: return True 
             else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
         except KeyError as err:
-            err_msg = 'Error: No agent identified in DATA | Key Error: {}'.format(err)
+            err_msg = 'Error: No UA Endpoint identified in DATA | Key Error: {}'.format(err)
             raise KepError(err_msg)
-        # except:
-        #     return 'Error: Error with {}'.format(inspect.currentframe().f_code.co_name)
     else:
-        r = server._config_update(server.url + IOT.agent._create_url(agent_type, agent) + _create_url(iot_item), agent_data)
+        r = server._config_update(server.url + _create_url(endpoint), DATA)
         if r.code == 200: return True 
         else: raise KepHTTPError(r.url, r.code, r.msg, r.hdrs, r.payload)
 
-def get_iot_item(server, iot_item, agent, agent_type)-> dict:
-    '''Returns the properties of the agent object. Returned object is JSON.
-
-    INPUTS:
-    "server" - instance of the "server" class
+def get_endpoint(server: server, endpoint: str) -> dict:
+    '''Returns the properties of the `"endpoint"` object.
     
-    "iot_item" - IoT item
-
-    "agent" - name of IoT Agent
-
-    "agent_type" - agent type
-
-    RETURNS:
-    dict - data for the IoT item requested
+    :param server: instance of the `server` class
+    :param endpoint: name of endpoint to retrieve
+    
+    :return: Dict of properties for the UA endpoint requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_get(server.url + IOT.agent._create_url(agent_type, agent) + _create_url(iot_item))
+
+    r = server._config_get(server.url + _create_url(endpoint))
     return r.payload
 
-def get_all_iot_items(server, agent, agent_type) -> list:
-    '''Returns the properties of all iot item objects for an agent. Returned object is JSON list.
+def get_all_endpoints(server: server, *, options: dict = None) -> list:
+    '''Returns list of all `"endpoint"` objects and their properties.
     
-    INPUTS:
-    "server" - instance of the "server" class
-
-    "agent" - name of IoT Agent
-
-    "agent_type" - agent type
-
-    RETURNS:
-    list - data for the IoT item requested
+    :param server: instance of the `server` class
+    :param options: *(optional)* Dict of parameters to filter, sort or pagenate the list of UA endpoints. Options are 'filter', 
+    'sortOrder', 'sortProperty', 'pageNumber', and 'pageSize.
+    
+    :return: List of properties for all UA endpoints requested
 
-    EXCEPTIONS:
-    KepHTTPError - If urllib provides an HTTPError
-    KepURLError - If urllib provides an URLError
+    :raises KepHTTPError: If urllib provides an HTTPError
+    :raises KepURLError: If urllib provides an URLError
     '''
-    r = server._config_get(server.url + IOT.agent._create_url(agent_type, agent) + _create_url())
+
+    r = server._config_get(f'{server.url}{_create_url()}', params= options)
     return r.payload
```

### Comparing `kepconfig-1.1.2/kepconfig.egg-info/PKG-INFO` & `kepconfig-1.2.0/kepconfig.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,113 @@
 Metadata-Version: 2.1
 Name: kepconfig
-Version: 1.1.2
+Version: 1.2.0
 Summary: SDK package for Kepware Configuration API
 Home-page: https://github.com/PTCInc/Kepware-ConfigAPI-SDK-Python
 Author: PTC Inc
 License: MIT License
 Keywords: Kepware,OPC,Configuration,Thingworx
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Kepware Configuration API SDK for Python
 
-[![PyPI version](https://badge.fury.io/py/kepconfig.svg)](https://badge.fury.io/py/kepconfig)
+[![Released Version](https://img.shields.io/pypi/v/kepconfig)](https://pypi.org/project/kepconfig) [![Supported Versions](https://img.shields.io/pypi/pyversions/kepconfig)](https://pypi.org/project/kepconfig) ![PyPI - Downloads](https://img.shields.io/pypi/dm/kepconfig) ![PyPI - License](https://img.shields.io/pypi/l/kepconfig)
 
-This is a package SDK to create Python modules to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
+This is a package to help create Python applications to conduct operations with the Kepware Configuration API. This package is designed to work with all versions of Kepware that support the Configuration API including Thingworx Kepware Server (TKS), Thingworx Kepware Edge (TKE) and KEPServerEX (KEP).
 
 ## Prerequisites
 
-The client libraries are supported on Python 3.6 or later. All HTTP communication is handled by the [urllib](https://docs.python.org/3.6/library/urllib.html#module-urllib) Python standard library.
+Package supported and tested on Python 3.9 or later. Older versions support earlier Python 3 environments but have less functionality. All HTTP communication is handled by the [urllib](https://docs.python.org/3/library/urllib.html#module-urllib) Python standard library.
 
 ## Features
 
 - Supports both HTTP and HTTPS connections with certificate validation options
 
 SDK allows for *GET*, *ADD*, *DELETE*, and *MODIFY* functions for the following Kepware configuration objects:
 
 | Features      | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
 | **Project Properties** <br /> *(Get and Modify Only)* | Y | Y |
 | **Connectivity** <br /> *(Channel, Devices, Tags, Tag Groups)* | Y | Y |
 | **IoT Gateway** <br /> *(Agents, IoT Items)* | Y | Y |
 | **Datalogger** <br /> *(Log Groups, Items, Mapping, Triggers, Reset Mapping Service)* | Y | Y |
 | **Administration** <br /> *(User Groups, Users, UA Endpoints, Local License Server)* | Y* | Y |
+| **Product Info and Health Status\*\*** | Y | Y |
 
-Note (*) - UA Endpoints and Local License Server supported for Kepware Edge only
+- Note (*) - UA Endpoints and Local License Server supported for Kepware Edge only
+- Note (**) - Added to Kepware Server v6.13 / Kepware Edge v1.5 and later builds
 
 Driver specific features:
 
 | Driver          | Features       |
 | :----------:  | :----------:  |
 |GE Ethernet Global Data|Exchanges, Ranges and Name Resolutions|
+|Universal Device Driver|Profile Library|
 
 Methods to read the following logs:
 
 | Logs          | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
 | **Event Log** | Y | Y |
 | **API Transaction Log** | Y | Y |
 
 Configuration API *Services* implemented:
 
 | Services      | TKS/KEP       | TKE           |
 | :----------:  | :----------:  | :----------:  |
-| **TagGeneration** <br /> *(for supported drivers)* | Y | Y |
+| **TagGeneration**<br />*(for supported drivers)* | Y | Y |
 | **ReinitializeRuntime** | Y* | Y |
+| **ProjectLoad and ProjectSave**| Y | Y |
 
 Note (*) - Reinitialize service was implemented for Kepware Server v6.8+
 
-Generic REST methods are provided to use for functions not developed in SDK package. These are found in the Server Class in [connection.py](/kepconfig/connection.py)
+Filtering, sorting and pagination query options are added for any collections methods (ex: get_all_devices() or get_all_channel()).
+
+Generic REST methods are provided to use for functions not developed in SDK package. These are found in the Server Class in [connection.py](./kepconfig/connection.py)
 
 ## Known Limitations
 
-- Other property configuration for more complex drivers with objects besides channels, devices, tags and tag groups are not explicitly defined
+- Other property configuration for more complex drivers with objects besides channels, devices, tags and tag groups are not always explicitly defined
 - Other supported plug-ins (EFM Exporter, Scheduler, etc) are not defined
 - When using hostnames (not IP addresses) for connections, delays may occur under certain network configurations as the connection may attempt IPv6 connections first. IPv6 is not supported by Kepware servers at this time.
 
 ## Installation
 
 Package can be installed with `pip` using the following:
 
 ```cmd
     pip install kepconfig
 ```
 
 ## Key Concepts
 
-NOTE: Samples can also be found in the [samples](samples) folder.
+NOTE: Detailed examples can also be found in the [examples](./examples/) folder.
 
 ### Create server connection
 
 ```python
 import kepconfig.connection
 
 server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '')
 
 # For HTTPS connections:
-server = connection.server(host = '127.0.0.1', port = 57412, user = 'Administrator', pw = '', https=True)
+server = connection.server(host = '127.0.0.1', port = 57512, user = 'Administrator', pw = '', https=True)
 
 ```
 
 For certificate validation, the SDK uses the OS/systems trusted CA certificate store. The connection uses the "create_default_context()" function as part of urllib as described at the following links:
 
 - [ssl.create_default_context](https://docs.python.org/3/library/ssl.html#ssl.create_default_context)
 - [ssl.SSLContext.load_default_certs](https://docs.python.org/3/library/ssl.html#ssl.SSLContext.load_default_certs)
@@ -139,9 +149,8 @@
 ```
 
 ## Need More Information
 
 **Visit:**
 
 - [Kepware.com](https://www.kepware.com/)
-- [Configuration API Info](https://www.kepware.com/en-us/products/kepserverex/features/configuration-api/)
 - [PTC.com](https://www.ptc.com/)
```

### Comparing `kepconfig-1.1.2/kepconfig.egg-info/SOURCES.txt` & `kepconfig-1.2.0/kepconfig.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 kepconfig/__init__.py
 kepconfig/connection.py
 kepconfig/error.py
+kepconfig/structures.py
+kepconfig/utils.py
 kepconfig.egg-info/PKG-INFO
 kepconfig.egg-info/SOURCES.txt
 kepconfig.egg-info/dependency_links.txt
 kepconfig.egg-info/top_level.txt
 kepconfig/admin/__init__.py
 kepconfig/admin/lls.py
 kepconfig/admin/ua_server.py
@@ -18,14 +20,16 @@
 kepconfig/connectivity/channel.py
 kepconfig/connectivity/device.py
 kepconfig/connectivity/tag.py
 kepconfig/connectivity/egd/__init__.py
 kepconfig/connectivity/egd/exchange.py
 kepconfig/connectivity/egd/name.py
 kepconfig/connectivity/egd/range.py
+kepconfig/connectivity/udd/__init__.py
+kepconfig/connectivity/udd/profile.py
 kepconfig/datalogger/__init__.py
 kepconfig/datalogger/log_group.py
 kepconfig/datalogger/log_items.py
 kepconfig/datalogger/mapping.py
 kepconfig/datalogger/triggers.py
 kepconfig/iot_gateway/__init__.py
 kepconfig/iot_gateway/agent.py
```

### Comparing `kepconfig-1.1.2/setup.py` & `kepconfig-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,13 +46,17 @@
     project_urls={},
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
         "Operating System :: OS Independent",
         "Intended Audience :: Manufacturing",
         "Intended Audience :: Developers",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.9',
 )
```

