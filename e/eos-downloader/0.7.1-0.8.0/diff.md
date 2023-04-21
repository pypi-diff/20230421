# Comparing `tmp/eos_downloader-0.7.1.tar.gz` & `tmp/eos_downloader-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eos_downloader-0.7.1.tar", last modified: Wed Feb 15 13:53:50 2023, max compression
+gzip compressed data, was "eos_downloader-0.8.0.tar", last modified: Fri Apr 21 08:16:55 2023, max compression
```

## Comparing `eos_downloader-0.7.1.tar` & `eos_downloader-0.8.0.tar`

### file list

```diff
@@ -1,49 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.605205 eos_downloader-0.7.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2064 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/bin/cvp-upload
--rwxr-xr-x   0 runner    (1001) docker     (123)     3217 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/bin/eos-download
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.605205 eos_downloader-0.7.1/eos_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.605205 eos_downloader-0.7.1/eos_downloader/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-02-15 13:53:50.000000 eos_downloader-0.7.1/eos_downloader/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.605205 eos_downloader-0.7.1/eos_downloader/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.605205 eos_downloader-0.7.1/eos_downloader/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/cli/debug/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/eos_downloader/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/cli/get/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/cvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/eos.py
--rw-r--r--   0 runner    (1001) docker     (123)    17567 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/eos_downloader/object_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.605205 eos_downloader-0.7.1/eos_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-02-15 13:53:50.000000 eos_downloader-0.7.1/eos_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-15 13:53:50.000000 eos_downloader-0.7.1/eos_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 13:53:50.000000 eos_downloader-0.7.1/eos_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-15 13:53:50.000000 eos_downloader-0.7.1/eos_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-15 13:53:50.000000 eos_downloader-0.7.1/eos_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-15 13:53:50.000000 eos_downloader-0.7.1/eos_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/lib/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/lib/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/tests/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/system/test_eos_download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:50.609205 eos_downloader-0.7.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/unit/test_CvFeatureManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-02-15 13:53:46.000000 eos_downloader-0.7.1/tests/unit/test_eos_download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/debug/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/get/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/cli/info/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cli/info/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/cvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/eos_downloader/object_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/eos_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20707 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 08:16:55.000000 eos_downloader-0.8.0/eos_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-21 08:16:44.000000 eos_downloader-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:16:55.809499 eos_downloader-0.8.0/setup.cfg
```

### Comparing `eos_downloader-0.7.1/LICENSE` & `eos_downloader-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eos_downloader-0.7.1/eos_downloader/__init__.py` & `eos_downloader-0.8.0/eos_downloader/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 #!/usr/bin/python
 # coding: utf-8 -*-
 
+"""
+EOS Downloader module.
+"""
+
 from __future__ import (absolute_import, division,
                         print_function, unicode_literals)
 import dataclasses
+from typing import Any
 import json
+import importlib.metadata
 
 __author__ = '@titom73'
 __email__ = 'tom@inetsix.net'
 __date__ = '2022-03-16'
-__version__ = '0.7.1'
+__version__ = importlib.metadata.version("eos-downloader")
 
-__all__ = ["CvpAuthenticationItem", "CvFeatureManager", "EOSDownloader", "ObjectDownloader", "reverse"]
+# __all__ = ["CvpAuthenticationItem", "CvFeatureManager", "EOSDownloader", "ObjectDownloader", "reverse"]
 
 ARISTA_GET_SESSION = "https://www.arista.com/custom_data/api/cvp/getSessionCode/"
 
 ARISTA_SOFTWARE_FOLDER_TREE = "https://www.arista.com/custom_data/api/cvp/getFolderTree/"
 
 ARISTA_DOWNLOAD_URL = "https://www.arista.com/custom_data/api/cvp/getDownloadLink/"
 
@@ -30,11 +36,12 @@
 MSG_INVALID_DATA = """Invalid data returned by server
 """
 
 EVE_QEMU_FOLDER_PATH = '/opt/unetlab/addons/qemu/'
 
 
 class EnhancedJSONEncoder(json.JSONEncoder):
-    def default(self, o):
+    """Custom JSon encoder."""
+    def default(self, o: Any) -> Any:
         if dataclasses.is_dataclass(o):
             return dataclasses.asdict(o)
         return super().default(o)
```

### Comparing `eos_downloader-0.7.1/eos_downloader/cli/cli.py` & `eos_downloader-0.8.0/eos_downloader/cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,72 @@
 #!/usr/bin/env python
 # coding: utf-8 -*-
 # pylint: disable=no-value-for-parameter
 # pylint: disable=cyclic-import
 # pylint: disable=too-many-arguments
+# pylint: disable=unused-argument
 
 
 """
 ARDL CLI Baseline.
 """
 
 import click
 from rich.console import Console
 import eos_downloader
 from eos_downloader.cli.get import commands as get_commands
 from eos_downloader.cli.debug import commands as debug_commands
+from eos_downloader.cli.info import commands as info_commands
 
 
 @click.group()
 @click.pass_context
 @click.option('--token', show_envvar=True, default=None, help='Arista Token from your customer account')
 def ardl(ctx: click.Context, token: str) -> None:
     """Arista Network Download CLI"""
     ctx.ensure_object(dict)
     ctx.obj['token'] = token
 
 
 @click.command()
-def version():
+def version() -> None:
     """Display version of ardl"""
     console = Console()
     console.print(f'ardl is running version {eos_downloader.__version__}')
 
 
 @ardl.group(no_args_is_help=True)
 @click.pass_context
 def get(ctx: click.Context) -> None:
     # pylint: disable=redefined-builtin
     """Download Arista from Arista website"""
 
 
 @ardl.group(no_args_is_help=True)
 @click.pass_context
+def info(ctx: click.Context) -> None:
+    # pylint: disable=redefined-builtin
+    """List information from Arista website"""
+
+
+@ardl.group(no_args_is_help=True)
+@click.pass_context
 def debug(ctx: click.Context) -> None:
     # pylint: disable=redefined-builtin
     """Debug commands to work with ardl"""
 
 # ANTA CLI Execution
 
 
 def cli() -> None:
     """Load ANTA CLI"""
     # Load group commands
     get.add_command(get_commands.eos)
     get.add_command(get_commands.cvp)
+    info.add_command(info_commands.eos_versions)
     debug.add_command(debug_commands.xml)
     ardl.add_command(version)
     # Load CLI
     ardl(
         obj={},
         auto_envvar_prefix='arista'
     )
```

### Comparing `eos_downloader-0.7.1/eos_downloader/cli/debug/commands.py` & `eos_downloader-0.8.0/eos_downloader/cli/debug/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 #!/usr/bin/env python
 # coding: utf-8 -*-
 # pylint: disable=no-value-for-parameter
 # pylint: disable=too-many-arguments
 # pylint: disable=line-too-long
+# pylint: disable=duplicate-code
 # flake8: noqa E501
 
 """
 Commands for ARDL CLI to get data.
 """
 
+import xml.etree.ElementTree as ET
+from xml.dom import minidom
+
 import click
-import eos_downloader.eos
 from loguru import logger
 from rich.console import Console
-import xml.etree.ElementTree as ET
-from xml.dom import minidom
 
+import eos_downloader.eos
 
 
 @click.command()
 @click.pass_context
 @click.option('--output', default=str('arista.xml'), help='Path to save XML file', type=click.Path(), show_default=True)
 @click.option('--log-level', '--log', help='Logging level of the command', default=None, type=click.Choice(['debug', 'info', 'warning', 'error', 'critical'], case_sensitive=False))
-def xml(ctx: click.Context, output: str, log_level: str):
+def xml(ctx: click.Context, output: str, log_level: str) -> None:
     # sourcery skip: remove-unnecessary-cast
     """Extract XML directory structure"""
     console = Console()
     # Get from Context
     token = ctx.obj['token']
 
     logger.remove()
@@ -37,15 +39,15 @@
         image='unset',
         software='EOS',
         version='unset',
         token=token,
         hash_method='sha512sum')
 
     my_download.authenticate()
-    xml_object: ET.ElementTree = my_download._get_folder_tree()
+    xml_object: ET.ElementTree = my_download._get_folder_tree()  # pylint: disable=protected-access
     xml_content = xml_object.getroot()
 
     xmlstr = minidom.parseString(ET.tostring(xml_content)).toprettyxml(indent="    ", newl='')
-    with open(output, "w") as f:
+    with open(output, "w", encoding='utf-8') as f:
         f.write(str(xmlstr))
 
     console.print(f'XML file saved in: { output }')
```

### Comparing `eos_downloader-0.7.1/eos_downloader/cli/get/commands.py` & `eos_downloader-0.8.0/eos_downloader/cli/get/commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 #!/usr/bin/env python
 # coding: utf-8 -*-
 # pylint: disable=no-value-for-parameter
 # pylint: disable=too-many-arguments
 # pylint: disable=line-too-long
+# pylint: disable=redefined-builtin
 # flake8: noqa E501
 
 """
 Commands for ARDL CLI to get data.
 """
 
 import os
 import sys
-import logging
+from typing import Union
+
 import click
-import eos_downloader.eos
 from loguru import logger
 from rich.console import Console
 
+import eos_downloader.eos
+from eos_downloader.models.version import BASE_VERSION_STR, RTYPE_FEATURE, RTYPES
 
 EOS_IMAGE_TYPE = ['64', 'INT', '2GB-INT', 'cEOS', 'cEOS64', 'vEOS', 'vEOS-lab', 'EOS-2GB', 'default']
 CVP_IMAGE_TYPE = ['ova', 'rpm', 'kvm', 'upgrade']
 
 @click.command(no_args_is_help=True)
 @click.pass_context
 @click.option('--image-type', default='default', help='EOS Image type', type=click.Choice(EOS_IMAGE_TYPE), required=True)
-@click.option('--version', default=None, help='EOS version', type=str, required=True)
+@click.option('--version', default=None, help='EOS version', type=str, required=False)
+@click.option('--latest', '-l', is_flag=True, type=click.BOOL, default=False, help='Get latest version in given branch. If --branch is not use, get the latest branch with specific release type')
+@click.option('--release-type', '-rtype', type=click.Choice(RTYPES, case_sensitive=False), default=RTYPE_FEATURE, help='EOS release type to search')
+@click.option('--branch', '-b', type=click.STRING, default=None, help='EOS Branch to list releases')
 @click.option('--docker-name', default='arista/ceos', help='Docker image name (default: arista/ceos)', type=str, show_default=True)
 @click.option('--output', default=str(os.path.relpath(os.getcwd(), start=os.curdir)), help='Path to save image', type=click.Path(),show_default=True)
 # Debugging
 @click.option('--log-level', '--log', help='Logging level of the command', default=None, type=click.Choice(['debug', 'info', 'warning', 'error', 'critical'], case_sensitive=False))
 # Boolean triggers
-@click.option('--eve-ng/--no-eve-ng', help='Run EVE-NG vEOS provisioning (only if CLI runs on an EVE-NG server)', default=False)
-@click.option('--disable-ztp/--no-disable-ztp', help='Disable ZTP process in vEOS image (only available with --eve-ng)', default=False)
-@click.option('--import-docker/--no-import-docker', help='Import docker image (only available with --image_type cEOSlab)', default=False)
-def eos(ctx: click.Context, image_type: str, version: str, output: str, log_level: str, eve_ng: bool, disable_ztp: bool, import_docker: bool, docker_name: str):
+@click.option('--eve-ng', is_flag=True, help='Run EVE-NG vEOS provisioning (only if CLI runs on an EVE-NG server)', default=False)
+@click.option('--disable-ztp', is_flag=True, help='Disable ZTP process in vEOS image (only available with --eve-ng)', default=False)
+@click.option('--import-docker', is_flag=True, help='Import docker image (only available with --image_type cEOSlab)', default=False)
+def eos(
+    ctx: click.Context, image_type: str, output: str, log_level: str, eve_ng: bool, disable_ztp: bool,
+    import_docker: bool, docker_name: str, version: Union[str, None] = None, release_type: str = RTYPE_FEATURE,
+    latest: bool = False, branch: Union[str,None] = None
+    ) -> int:
     """Download EOS image from Arista website"""
     console = Console()
     # Get from Context
     token = ctx.obj['token']
     if token is None or token == '':
         console.print('❗ Token is unset ! Please configure ARISTA_TOKEN or use --token option', style="bold red")
         sys.exit(1)
@@ -46,45 +56,61 @@
     if log_level is not None:
         logger.add("eos-downloader.log", rotation="10 MB", level=log_level.upper())
 
     console.print("🪐 [bold blue]eos-downloader[/bold blue] is starting...", )
     console.print(f'    - Image Type: {image_type}')
     console.print(f'    - Version: {version}')
 
-    my_download = eos_downloader.eos.EOSDownloader(
-        image=image_type,
-        software='EOS',
-        version=version,
-        token=token,
-        hash_method='sha512sum')
 
-    my_download.authenticate()
+    if version is not None:
+        my_download = eos_downloader.eos.EOSDownloader(
+            image=image_type,
+            software='EOS',
+            version=version,
+            token=token,
+            hash_method='sha512sum')
+        my_download.authenticate()
+
+    elif latest:
+        my_download = eos_downloader.eos.EOSDownloader(
+            image=image_type,
+            software='EOS',
+            version='unset',
+            token=token,
+            hash_method='sha512sum')
+        my_download.authenticate()
+        if branch is None:
+            branch = str(my_download.latest_branch(rtype=release_type).branch)
+        latest_version = my_download.latest_eos(branch, rtype=release_type)
+        if str(latest_version) == BASE_VERSION_STR:
+            console.print(f'[red]Error[/red], cannot find any version in {branch} for {release_type} release type')
+            sys.exit(1)
+        my_download.version = str(latest_version)
 
     if eve_ng:
         my_download.provision_eve(noztp=disable_ztp, checksum=True)
     else:
         my_download.download_local(file_path=output, checksum=True)
 
     if import_docker:
         my_download.docker_import(
-            version=version,
             image_name=docker_name
         )
     console.print('✅  processing done !')
     sys.exit(0)
 
 
 
 @click.command(no_args_is_help=True)
 @click.pass_context
 @click.option('--format', default='upgrade', help='CVP Image type', type=click.Choice(CVP_IMAGE_TYPE), required=True)
 @click.option('--version', default=None, help='CVP version', type=str, required=True)
 @click.option('--output', default=str(os.path.relpath(os.getcwd(), start=os.curdir)), help='Path to save image', type=click.Path(),show_default=True)
 @click.option('--log-level', '--log', help='Logging level of the command', default=None, type=click.Choice(['debug', 'info', 'warning', 'error', 'critical'], case_sensitive=False))
-def cvp(ctx: click.Context, version: str, format: str, output: str, log_level: str):
+def cvp(ctx: click.Context, version: str, format: str, output: str, log_level: str) -> int:
     """Download CVP image from Arista website"""
     console = Console()
     # Get from Context
     token = ctx.obj['token']
     if token is None or token == '':
         console.print('❗ Token is unset ! Please configure ARISTA_TOKEN or use --token option', style="bold red")
         sys.exit(1)
@@ -98,14 +124,14 @@
     console.print(f'    - Version: {version}')
 
     my_download = eos_downloader.eos.EOSDownloader(
         image=format,
         software='CloudVision',
         version=version,
         token=token,
-        hash_method='sha512sum')
+        hash_method='md5sum')
 
     my_download.authenticate()
 
-    my_download.download_local(file_path=output, checksum=True)
+    my_download.download_local(file_path=output, checksum=False)
     console.print('✅  processing done !')
     sys.exit(0)
```

### Comparing `eos_downloader-0.7.1/eos_downloader/cvp.py` & `eos_downloader-0.8.0/eos_downloader/cvp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 #!/usr/bin/python
 # coding: utf-8 -*-
 
-from posixpath import basename
-from loguru import logger
-from dataclasses import dataclass
+"""
+CVP Uploader content
+"""
+
 import os
+from typing import List, Optional, Any
+from dataclasses import dataclass
+from loguru import logger
 from cvprac.cvp_client import CvpClient
 from cvprac.cvp_client_errors import CvpLoginError
-from typing import List
 
 
 @dataclass
 class CvpAuthenticationItem:
     """
      Data structure to represent Cloudvision Authentication
     """
     server: str
     port: int = 443
-    token: str = None
+    token: Optional[str] = None
     timeout: int = 1200
     validate_cert: bool = False
 
 
 class Filer():
+    # pylint: disable=too-few-public-methods
     """
     Filer Helper for file management
     """
-    def __init__(self, path: str):
+    def __init__(self, path: str) -> None:
         self.file_exist = False
         self.filename = ''
         self.absolute_path = ''
         self.relative_path = path
         if os.path.exists(path):
             self.file_exist = True
             self.filename = os.path.basename(path)
             self.absolute_path = os.path.realpath(path)
 
-    def __repr__(self):
-        if self.file_exist:
-            return self.absolute_path
-        return ''
+    def __repr__(self) -> str:
+        return self.absolute_path if self.file_exist else ''
 
 
 class CvFeatureManager():
     """
     CvFeatureManager Object to interect with Cloudvision
     """
-    def __init__(self, authentication: CvpAuthenticationItem):
+    def __init__(self, authentication: CvpAuthenticationItem) -> None:
         """
         __init__ Class Creator
 
         Parameters
         ----------
         authentication : CvpAuthenticationItem
             Authentication information to use to connect to Cloudvision
         """
         self._authentication = authentication
         # self._cv_instance = CvpClient()
         self._cv_instance = self._connect(authentication=authentication)
         self._cv_images = self.__get_images()
         # self._cv_bundles = self.__get_bundles()
 
-    def _connect(self, authentication: CvpAuthenticationItem):
+    def _connect(self, authentication: CvpAuthenticationItem) -> CvpClient:
         """
         _connect Connection management
 
         Parameters
         ----------
         authentication : CvpAuthenticationItem
             Authentication information to use to connect to Cloudvision
@@ -85,58 +87,50 @@
                     api_token=authentication.token,
                     is_cvaas=True,
                     port=authentication.port,
                     cert=authentication.validate_cert,
                     request_timeout=authentication.timeout
                 )
             except CvpLoginError as error_data:
-                logger.error(
-                    'Cannot connect to Cloudvision server {}'.format(
-                        authentication.server
-                    )
-                )
-                logger.debug('Error message: {}'.format(error_data))
+                logger.error(f'Cannot connect to Cloudvision server {authentication.server}')
+                logger.debug(f'Error message: {error_data}')
         logger.info('connected to Cloudvision server')
-        logger.debug('Connection info: {0}'.format(authentication))
+        logger.debug(f'Connection info: {authentication}')
         return client
 
-    def __get_images(self):
+    def __get_images(self) -> List[Any]:
         """
         __get_images Collect information about images on Cloudvision
 
         Returns
         -------
         dict
             Fact returned by Cloudvision
         """
         images = []
         logger.debug('  -> Collecting images')
         images = self._cv_instance.api.get_images()['data']
-        if self.__check_api_result(images):
-            return images
-        return None
-
-    def __get_bundles(self):
-        """
-        __get_bundles [Not In use] Collect information about bundles on Cloudvision
+        return images if self.__check_api_result(images) else []
 
-        Returns
-        -------
-        dict
-            Fact returned by Cloudvision
-        """
-        bundles = []
-        logger.debug('  -> Collecting images bundles')
-        bundles = self._cv_instance.api.get_image_bundles()['data']
-        # bundles = self._cv_instance.post(url='/cvpservice/image/getImageBundles.do?queryparam=&startIndex=0&endIndex=0')['data']
-        if self.__check_api_result(bundles):
-            return bundles
-        return None
+    # def __get_bundles(self):
+    #     """
+    #     __get_bundles [Not In use] Collect information about bundles on Cloudvision
+
+    #     Returns
+    #     -------
+    #     dict
+    #         Fact returned by Cloudvision
+    #     """
+    #     bundles = []
+    #     logger.debug('  -> Collecting images bundles')
+    #     bundles = self._cv_instance.api.get_image_bundles()['data']
+    #     # bundles = self._cv_instance.post(url='/cvpservice/image/getImageBundles.do?queryparam=&startIndex=0&endIndex=0')['data']
+    #     return bundles if self.__check_api_result(bundles) else None
 
-    def __check_api_result(self, arg0):
+    def __check_api_result(self, arg0: Any) -> bool:
         """
         __check_api_result Check API calls return content
 
         Parameters
         ----------
         arg0 : any
             Element to test
@@ -145,48 +139,44 @@
         -------
         bool
             True if data are correct False in other cases
         """
         logger.debug(arg0)
         return len(arg0) > 0
 
-    def _does_image_exist(self, image_name):
+    def _does_image_exist(self, image_name: str) -> bool:
         """
         _does_image_exist Check if an image is referenced in Cloudvision facts
 
         Parameters
         ----------
         image_name : str
             Name of the image to search for
 
         Returns
         -------
         bool
             True if present
         """
-        return any(image_name == image['name'] for image in self._cv_images)
+        return any(image_name == image['name'] for image in self._cv_images) if isinstance(self._cv_images, list) else False
 
-    def _does_bundle_exist(self, bundle_name):
+    def _does_bundle_exist(self, bundle_name: str) -> bool:
+        # pylint: disable=unused-argument
         """
         _does_bundle_exist Check if an image is referenced in Cloudvision facts
 
-        Parameters
-        ----------
-        bundle_name : str
-            Name of the bundle to search for
-
         Returns
         -------
         bool
             True if present
         """
         # return any(bundle_name == bundle['name'] for bundle in self._cv_bundles)
         return False
 
-    def upload_image(self, image_path: str):
+    def upload_image(self, image_path: str) -> bool:
         """
         upload_image Upload an image to Cloudvision server
 
         Parameters
         ----------
         image_path : str
             Path to the local file to upload
@@ -194,30 +184,30 @@
         Returns
         -------
         bool
             True if succeeds
         """
         image_item = Filer(path=image_path)
         if image_item.file_exist is False:
-            logger.error('File not found: {}'.format(image_item.relative_path))
+            logger.error(f'File not found: {image_item.relative_path}')
             return False
-        logger.info('File path for image: {}'.format(image_item))
+        logger.info(f'File path for image: {image_item}')
         if self._does_image_exist(image_name=image_item.filename):
             logger.error("Image found in Cloudvision , Please delete it before running this script")
-            return  False
+            return False
         try:
             upload_result = self._cv_instance.api.add_image(filepath=image_item.absolute_path)
-        except Exception as e:
+        except Exception as e:  # pylint: disable=broad-exception-caught
             logger.error('An error occurred during upload, check CV connection')
-            logger.error('Exception message is: {}'.format(e))
+            logger.error(f'Exception message is: {e}')
             return False
-        logger.debug('Upload Result is : {}'.format(upload_result))
+        logger.debug(f'Upload Result is : {upload_result}')
         return True
 
-    def build_image_list(self, image_list):
+    def build_image_list(self, image_list: List[str]) -> List[Any]:
         """
         Builds a list of the image data structures, for a given list of image names.
         Parameters
         ----------
         image_list : list
             List of software image names
         Returns
@@ -236,20 +226,17 @@
 
             if image_data is not None:
                 internal_image_list.append(image_data)
                 image_data = None
             else:
                 success = False
 
-        if success:
-            return internal_image_list
-        else:
-            return None
+        return internal_image_list if success else []
 
-    def create_bundle(self, name: str, images_name: List[str]):
+    def create_bundle(self, name: str, images_name: List[str]) -> bool:
         """
         create_bundle Create a bundle with a list of images.
 
         Parameters
         ----------
         name : str
             Name of the bundle
@@ -257,28 +244,29 @@
             List of images available on Cloudvision
 
         Returns
         -------
         bool
             True if succeeds
         """
-        logger.debug('Init creation of an image bundle {0} with following images {1}'.format(name, str(images_name)))
-        all_images_present : List[bool] = []
+        logger.debug(f'Init creation of an image bundle {name} with following images {images_name}')
+        all_images_present: List[bool] = []
         self._cv_images = self.__get_images()
-        for image_name in images_name:
-            all_images_present.append(self._does_image_exist(image_name=image_name))
+        all_images_present.extend(
+            self._does_image_exist(image_name=image_name)
+            for image_name in images_name
+        )
         # Bundle Create
         if self._does_bundle_exist(bundle_name=name) is False:
-            logger.debug('Creating image bundle {0} with following images {1}'.format(name, str(images_name)))
+            logger.debug(f'Creating image bundle {name} with following images {images_name}')
             images_data = self.build_image_list(image_list=images_name)
             if images_data is not None:
-                logger.debug('Images information: {0}'.format(images_data))
+                logger.debug('Images information: {images_data}')
                 try:
                     data = self._cv_instance.api.save_image_bundle(name=name, images=images_data)
-                except Exception as e:
-                    logger.critical('{0}'.format(e))
+                except Exception as e:  # pylint: disable=broad-exception-caught
+                    logger.critical(f'{e}')
                 else:
                     logger.debug(data)
                 return True
-            else:
-                logger.critical('No data found for images')
+            logger.critical('No data found for images')
         return False
```

### Comparing `eos_downloader-0.7.1/eos_downloader/download.py` & `eos_downloader-0.8.0/eos_downloader/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
+# flake8: noqa: F811
+# pylint: disable=unused-argument
+# pylint: disable=too-few-public-methods
+
+"""download module"""
+
 import os.path
-import sys
-import requests
 import signal
-from functools import partial
 from concurrent.futures import ThreadPoolExecutor
 from threading import Event
-from typing import Iterable
-from urllib.request import urlopen
+from typing import Iterable, Any
+
+import requests
 import rich
 from rich import console
-from rich.progress import (
-    BarColumn,
-    DownloadColumn,
-    Progress,
-    TaskID,
-    TextColumn,
-    TransferSpeedColumn,
-    TimeElapsedColumn
-)
+from rich.progress import (BarColumn, DownloadColumn, Progress, TaskID,
+                           TextColumn, TimeElapsedColumn, TransferSpeedColumn)
 
 console = rich.get_console()
 done_event = Event()
 
 
-def handle_sigint(signum, frame):
+def handle_sigint(signum: Any, frame: Any) -> None:
+    """Progress bar handler"""
     done_event.set()
 
+
 signal.signal(signal.SIGINT, handle_sigint)
 
+
 class DownloadProgressBar():
     """
     Object to manage Download process with Progress Bar from Rich
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """
         Class Constructor
         """
         self.progress = Progress(
             TextColumn("💾  Downloading [bold blue]{task.fields[filename]}", justify="right"),
             BarColumn(bar_width=None),
             "[progress.percentage]{task.percentage:>3.1f}%",
@@ -47,30 +47,30 @@
             DownloadColumn(),
             "•",
             TimeElapsedColumn(),
             "•",
             console=console
         )
 
-    def _copy_url(self, task_id: TaskID, url: str, path: str, block_size=1024) -> None:
+    def _copy_url(self, task_id: TaskID, url: str, path: str, block_size: int = 1024) -> bool:
         """Copy data from a url to a local file."""
-        response = requests.get(url, stream=True)
+        response = requests.get(url, stream=True, timeout=5)
         # This will break if the response doesn't contain content length
         self.progress.update(task_id, total=int(response.headers['Content-Length']))
         with open(path, "wb") as dest_file:
             self.progress.start_task(task_id)
             for data in response.iter_content(chunk_size=block_size):
                 dest_file.write(data)
                 self.progress.update(task_id, advance=len(data))
                 if done_event.is_set():
-                    return
+                    return True
         # console.print(f"Downloaded {path}")
+        return False
 
-
-    def download(self, urls: Iterable[str], dest_dir: str):
+    def download(self, urls: Iterable[str], dest_dir: str) -> None:
         """Download multuple files to the given directory."""
         with self.progress:
             with ThreadPoolExecutor(max_workers=4) as pool:
                 for url in urls:
                     filename = url.split("/")[-1].split('?')[0]
                     dest_path = os.path.join(dest_dir, filename)
                     task_id = self.progress.add_task("download", filename=filename, start=False)
```

### Comparing `eos_downloader-0.7.1/eos_downloader/object_downloader.py` & `eos_downloader-0.8.0/eos_downloader/object_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 #!/usr/bin/python
 # coding: utf-8 -*-
+# flake8: noqa: F811
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
+
+"""
+eos_downloader class definition
+"""
+
+from __future__ import (absolute_import, division, print_function,
+                        unicode_literals)
 
-from __future__ import (absolute_import, division,
-                        print_function, unicode_literals)
-# from builtins import *
-import sys
-import os
 import base64
 import glob
 import hashlib
-import requests
-import rich
 import json
+import os
+# from builtins import *
+import sys
 import xml.etree.ElementTree as ET
-from xml.etree import ElementTree
-from xml.dom import minidom
+from typing import Union
+
+import requests
+import rich
 from loguru import logger
-from urllib.request import urlopen
 from rich import console
-from eos_downloader.download import DownloadProgressBar
-from eos_downloader.data import DATA_MAPPING
-from eos_downloader import ARISTA_GET_SESSION, ARISTA_SOFTWARE_FOLDER_TREE, ARISTA_DOWNLOAD_URL, MSG_TOKEN_EXPIRED, MSG_INVALID_DATA, EVE_QEMU_FOLDER_PATH
 from tqdm import tqdm
 
+from eos_downloader import (ARISTA_DOWNLOAD_URL, ARISTA_GET_SESSION,
+                            ARISTA_SOFTWARE_FOLDER_TREE, EVE_QEMU_FOLDER_PATH,
+                            MSG_INVALID_DATA, MSG_TOKEN_EXPIRED)
+from eos_downloader.data import DATA_MAPPING
+from eos_downloader.download import DownloadProgressBar
+
 console = rich.get_console()
 
+
 class ObjectDownloader():
     """
     ObjectDownloader Generic Object to download from Arista.com
     """
     def __init__(self, image: str, version: str, token: str, software: str = 'EOS', hash_method: str = 'md5sum'):
         """
         __init__ Class constructor
@@ -52,51 +63,53 @@
         self.image = image
         self._version = version
         self.token = token
         self.folder_level = 0
         self.session_id = None
         self.filename = self._build_filename()
         self.hash_method = hash_method
+        self.timeout = 5
         # Logging
         logger.debug(f'Filename built by _build_filename is {self.filename}')
 
-
-    def __str__(self):
-        return self.software + ' - ' + self.image + ' - ' + self.version
+    def __str__(self) -> str:
+        return f'{self.software} - {self.image} - {self.version}'
 
     @property
-    def version(self):
+    def version(self) -> str:
+        """Get version."""
         return self._version
 
     @version.setter
-    def version(self, value: str):
+    def version(self, value: str) -> None:
+        """Set version."""
         self._version = value
         self.filename = self._build_filename()
 
     # ------------------------------------------------------------------------ #
-    # Private METHODS
+    # Internal METHODS
     # ------------------------------------------------------------------------ #
 
-    def _build_filename(self):
+    def _build_filename(self) -> str:
         """
         _build_filename Helper to build filename to search on arista.com
 
         Returns
         -------
         str:
             Filename to search for on Arista.com
         """
         if self.software in DATA_MAPPING:
             if self.image in DATA_MAPPING[self.software]:
                 return f"{DATA_MAPPING[self.software][self.image]['prepend']}-{self.version}{DATA_MAPPING[self.software][self.image]['extension']}"
-            else:
-                return f"{DATA_MAPPING[self.software]['default']['prepend']}-{self.version}{DATA_MAPPING[self.software]['default']['extension']}"
-        return None
+            return f"{DATA_MAPPING[self.software]['default']['prepend']}-{self.version}{DATA_MAPPING[self.software]['default']['extension']}"
+        return ''
 
-    def _parse_xml(self, root_xml: ET.ElementTree, xpath: str, search_file: str):
+    def _parse_xml_for_path(self, root_xml: ET.ElementTree, xpath: str, search_file: str) -> str:
+        # sourcery skip: remove-unnecessary-cast
         """
         _parse_xml Read and extract data from XML using XPATH
 
         Get all interested nodes using XPATH and then get node that match search_file
 
         Parameters
         ----------
@@ -113,23 +126,23 @@
             File Path on Arista server side
         """
         logger.debug(f'Using xpath {xpath}')
         logger.debug(f'Search for file {search_file}')
         console.print(f'🔎  Searching file {search_file}')
         for node in root_xml.findall(xpath):
             # logger.debug('Found {}', node.text)
-            if node.text.lower() == search_file.lower():
+            if str(node.text).lower() == search_file.lower():
                 path = node.get('path')
-                console.print(f'    -> Found file at {path}' )
+                console.print(f'    -> Found file at {path}')
                 logger.info('Found {} at {}', node.text, node.get('path'))
-                return node.get('path')
+                return str(node.get('path')) if node.get('path') is not None else ''
         logger.error('Requested file ({}) not found !', self.filename)
-        return False
+        return ''
 
-    def _get_hash(self, file_path: str):
+    def _get_hash(self, file_path: str) -> str:
         """
         _get_hash Download HASH file from Arista server
 
         Parameters
         ----------
         file_path : str
             Path of the HASH file
@@ -139,23 +152,23 @@
         str
             Hash string read from HASH file downloaded from Arista.com
         """
         remote_hash_file = self._get_remote_hashpath(hash_method=self.hash_method)
         hash_url = self._get_url(remote_file_path=remote_hash_file)
         # hash_downloaded = self._download_file_raw(url=hash_url, file_path=file_path + "/" + os.path.basename(remote_hash_file))
         dl_rich_progress_bar = DownloadProgressBar()
-        hash_downloaded = dl_rich_progress_bar.download(urls=[hash_url], dest_dir=file_path)
-        hash_downloaded = file_path + "/" + os.path.basename(remote_hash_file)
+        dl_rich_progress_bar.download(urls=[hash_url], dest_dir=file_path)
+        hash_downloaded = f"{file_path}/{os.path.basename(remote_hash_file)}"
         hash_content = 'unset'
-        with open(hash_downloaded, 'r') as f:
+        with open(hash_downloaded, 'r', encoding='utf-8') as f:
             hash_content = f.read()
         return hash_content.split(' ')[0]
 
     @staticmethod
-    def _compute_hash_md5sum(file: str, hash_expected: str):
+    def _compute_hash_md5sum(file: str, hash_expected: str) -> bool:
         """
         _compute_hash_md5sum Compare MD5 sum
 
         Do comparison between local md5 of the file and value provided by arista.com
 
         Parameters
         ----------
@@ -177,15 +190,15 @@
             return True
         logger.warning('Downloaded file is corrupt: local md5 ({}) is different to md5 from arista ({})',
                        hash_md5.hexdigest(),
                        hash_expected)
         return False
 
     @staticmethod
-    def _compute_hash_sh512sum(file: str, hash_expected: str):
+    def _compute_hash_sh512sum(file: str, hash_expected: str) -> bool:
         """
         _compute_hash_sh512sum Compare SHA512 sum
 
         Do comparison between local sha512 of the file and value provided by arista.com
 
         Parameters
         ----------
@@ -206,68 +219,73 @@
         if str(hash_sha512.hexdigest()) == hash_expected:
             return True
         logger.warning('Downloaded file is corrupt: local sha512 ({}) is different to sha512 from arista ({})',
                        hash_sha512.hexdigest(),
                        hash_expected)
         return False
 
-    def _get_folder_tree(self):
+    def _get_folder_tree(self) -> ET.ElementTree:
         """
         _get_folder_tree Download XML tree from Arista server
 
         Returns
         -------
         ET.ElementTree
             XML document
         """
         if self.session_id is None:
             self.authenticate()
         jsonpost = {'sessionCode': self.session_id}
-        result = requests.post(ARISTA_SOFTWARE_FOLDER_TREE, data=json.dumps(jsonpost))
+        result = requests.post(ARISTA_SOFTWARE_FOLDER_TREE, data=json.dumps(jsonpost), timeout=self.timeout)
         try:
-            folder_tree = (result.json()["data"]["xml"])
+            folder_tree = result.json()["data"]["xml"]
             return ET.ElementTree(ET.fromstring(folder_tree))
         except KeyError as error:
             logger.error(MSG_INVALID_DATA)
+            logger.error(f'Server returned: {error}')
             console.print(f'❌  {MSG_INVALID_DATA}', style="bold red")
             sys.exit(1)
 
-    def _get_remote_filepath(self):
+    def _get_remote_filepath(self) -> str:
         """
         _get_remote_filepath Helper to get path of the file to download
 
         Set XPATH and return result of _parse_xml for the file to download
 
         Returns
         -------
         str
             Remote path of the file to download
         """
         root = self._get_folder_tree()
         logger.debug("GET XML content from ARISTA.com")
-        xpath = './/dir[@label="' + self.software + '"]//file'
-        return self._parse_xml(root_xml=root, xpath=xpath, search_file=self.filename)
+        xpath = f'.//dir[@label="{self.software}"]//file'
+        return self._parse_xml_for_path(root_xml=root, xpath=xpath, search_file=self.filename)
 
-    def _get_remote_hashpath(self, hash_method: str = 'md5sum'):
+    def _get_remote_hashpath(self, hash_method: str = 'md5sum') -> str:
         """
         _get_remote_hashpath Helper to get path of the hash's file to download
 
         Set XPATH and return result of _parse_xml for the file to download
 
         Returns
         -------
         str
             Remote path of the hash's file to download
         """
         root = self._get_folder_tree()
         logger.debug("GET XML content from ARISTA.com")
-        xpath = './/dir[@label="' + self.software + '"]//file'
-        return self._parse_xml(root_xml=root, xpath=xpath, search_file=self.filename + '.' + hash_method)
+        xpath = f'.//dir[@label="{self.software}"]//file'
+        return self._parse_xml_for_path(
+            root_xml=root,
+            xpath=xpath,
+            search_file=f'{self.filename}.{hash_method}',
+        )
 
-    def _get_url(self, remote_file_path: str):
+    def _get_url(self, remote_file_path: str) ->  str:
         """
         _get_url Get URL to use for downloading file from Arista server
 
         Send remote_file_path to get correct URL to use for download
 
         Parameters
         ----------
@@ -278,23 +296,23 @@
         -------
         str
             URL link to use for download
         """
         if self.session_id is None:
             self.authenticate()
         jsonpost = {'sessionCode': self.session_id, 'filePath': remote_file_path}
-        result = requests.post(ARISTA_DOWNLOAD_URL, data=json.dumps(jsonpost))
+        result = requests.post(ARISTA_DOWNLOAD_URL, data=json.dumps(jsonpost), timeout=self.timeout)
         if 'data' in result.json() and 'url' in result.json()['data']:
             # logger.debug('URL to download file is: {}', result.json())
             return result.json()["data"]["url"]
         logger.critical('Server returns following message: {}', result.json())
-        return False
+        return ''
 
     @staticmethod
-    def _download_file_raw(url: str, file_path: str):
+    def _download_file_raw(url: str, file_path: str) -> str:
         """
         _download_file Helper to download file from Arista.com
 
         [extended_summary]
 
         Parameters
         ----------
@@ -305,52 +323,50 @@
 
         Returns
         -------
         str
             File path
         """
         chunkSize = 1024
-        r = requests.get(url, stream=True)
+        r = requests.get(url, stream=True, timeout=5)
         with open(file_path, 'wb') as f:
             pbar = tqdm(unit="B", total=int(r.headers['Content-Length']), unit_scale=True, unit_divisor=1024)
             for chunk in r.iter_content(chunk_size=chunkSize):
                 if chunk:
                     pbar.update(len(chunk))
                 f.write(chunk)
         return file_path
 
-    def _download_file(self, file_path: str, filename: str, rich_interface: bool = True):
+    def _download_file(self, file_path: str, filename: str, rich_interface: bool = True) -> Union[None, str]:
         remote_file_path = self._get_remote_filepath()
         logger.info('File found on arista server: {}', remote_file_path)
         file_url = self._get_url(remote_file_path=remote_file_path)
-        if rich_interface is True:
-            if file_url is not False:
-                rich_downloader = DownloadProgressBar()
-                rich_downloader.download(urls=[file_url], dest_dir=file_path)
-                return os.path.join(file_path, filename)
-        else:
-            if file_url is not False:
+        if file_url is not False:
+            if not rich_interface:
                 return self._download_file_raw(url=file_url, file_path=os.path.join(file_path, filename))
+            rich_downloader = DownloadProgressBar()
+            rich_downloader.download(urls=[file_url], dest_dir=file_path)
+            return os.path.join(file_path, filename)
         logger.error('Cannot download file {}', file_path)
         return None
 
     @staticmethod
-    def _create_destination_folder(path):
+    def _create_destination_folder(path: str) -> None:
         # os.makedirs(path, mode, exist_ok=True)
-        os.system('mkdir -p ' + path)
+        os.system(f'mkdir -p {path}')
 
     @staticmethod
-    def _disable_ztp(file_path: str):
+    def _disable_ztp(file_path: str) -> None:
         pass
 
     # ------------------------------------------------------------------------ #
     # Public METHODS
     # ------------------------------------------------------------------------ #
 
-    def authenticate(self):
+    def authenticate(self) -> bool:
         """
         authenticate Authenticate user on Arista.com server
 
         Send API token and get a session-id from remote server.
         Session-id will be used by all other functions.
 
         Returns
@@ -358,37 +374,34 @@
         bool
             True if authentication succeeds=, False in all other situations.
         """
         credentials = (base64.b64encode(self.token.encode())).decode("utf-8")
         session_code_url = ARISTA_GET_SESSION
         jsonpost = {'accessToken': credentials}
 
-        result = requests.post(session_code_url, data=json.dumps(jsonpost))
+        result = requests.post(session_code_url, data=json.dumps(jsonpost), timeout=self.timeout)
 
-        if result.json()["status"]["message"] == 'Access token expired':
+        if result.json()["status"]["message"] in[ 'Access token expired',  'Invalid access token']:
             console.print(f'❌  {MSG_TOKEN_EXPIRED}', style="bold red")
             logger.error(MSG_TOKEN_EXPIRED)
             return False
-        elif result.json()["status"]["message"] == 'Invalid access token':
-            logger.error(MSG_TOKEN_EXPIRED)
-            console.print(f'❌  {MSG_TOKEN_EXPIRED}', style="bold red")
-            return False
 
         try:
             if 'data' in result.json():
-                self.session_id = (result.json()["data"]["session_code"])
+                self.session_id = result.json()["data"]["session_code"]
                 logger.info('Authenticated on arista.com')
-                console.print('✅ Authenticated on arista.com')
                 return True
-            logger.debug('{}'.format(result.json()))
+            logger.debug(f'{result.json()}')
             return False
         except KeyError as error_arista:
+            logger.error(f'Error: {error_arista}')
             sys.exit(1)
 
-    def download_local(self, file_path: str, checksum: bool = False):
+    def download_local(self, file_path: str, checksum: bool = False) -> bool:
+        # sourcery skip: move-assign
         """
         download_local Entrypoint for local download feature
 
         Do local downnload feature:
         - Get remote file path
         - Get URL from Arista.com
         - Download file
@@ -402,15 +415,15 @@
             Execute checksum or not, by default False
 
         Returns
         -------
         bool
             True if everything went well, False if any problem appears
         """
-        file_downloaded = self._download_file(file_path=file_path, filename=self.filename)
+        file_downloaded = str(self._download_file(file_path=file_path, filename=self.filename))
 
         # Check file HASH
         hash_result = False
         if checksum:
             logger.info('🚀  Running checksum validation')
             console.print('🚀  Running checksum validation')
             if self.hash_method == 'md5sum':
@@ -423,15 +436,16 @@
             logger.error('Downloaded file is corrupted, please check your connection')
             console.print('❌  Downloaded file is corrupted, please check your connection')
             return False
         logger.info('Downloaded file is correct.')
         console.print('✅  Downloaded file is correct.')
         return True
 
-    def provision_eve(self, noztp: bool = False, checksum: bool = True):
+    def provision_eve(self, noztp: bool = False, checksum: bool = True) -> None:
+        # pylint: disable=unused-argument
         """
         provision_eve Entrypoint for EVE-NG download and provisioning
 
         Do following actions:
         - Get remote file path
         - Get URL from file path
         - Download file
@@ -445,15 +459,15 @@
             Flag to deactivate ZTP in EOS image, by default False
         checksum : bool, optional
             Flag to ask for hash validation, by default True
         """
         # Build image name to use in folder path
         eos_image_name = self.filename.rstrip(".vmdk").lower()
         if noztp:
-            eos_image_name = eos_image_name + '-noztp'
+            eos_image_name = f'{eos_image_name}-noztp'
         # Create full path for EVE-NG
         file_path = os.path.join(EVE_QEMU_FOLDER_PATH, eos_image_name.rstrip())
         # Create folders in filesystem
         self._create_destination_folder(path=file_path)
 
         # Download file to local destination
         file_downloaded = self._download_file(
@@ -471,16 +485,24 @@
 
         os.system('/opt/unetlab/wrappers/unl_wrapper -a fixpermissions')
         os.system(f'rm -f {file_downloaded}')
 
         if noztp:
             self._disable_ztp(file_path=file_path)
 
+    def docker_import(self, image_name: str = "arista/ceos") -> None:
+        """
+        Import docker container to your docker server.
+
+        Import downloaded container to your local docker engine.
 
-    def docker_import(self, version: str, image_name: str = "arista/ceos"):
+        Args:
+            version (str):
+            image_name (str, optional): Image name to use. Defaults to "arista/ceos".
+        """
         docker_image = f'{image_name}:{self.version}'
         logger.info(f'Importing image {self.filename} to {docker_image}')
         console.print(f'🚀 Importing image {self.filename} to {docker_image}')
         os.system(f'$(which docker) import {self.filename} {docker_image}')
         for filename in glob.glob(f'{self.filename}*'):
             try:
                 os.remove(filename)
```

