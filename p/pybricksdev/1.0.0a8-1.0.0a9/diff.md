# Comparing `tmp/pybricksdev-1.0.0a8.tar.gz` & `tmp/pybricksdev-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybricksdev-1.0.0a8.tar", max compression
+gzip compressed data, was "pybricksdev-1.0.0a9.tar", max compression
```

## Comparing `pybricksdev-1.0.0a8.tar` & `pybricksdev-1.0.0a9.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0      194 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/AUTHORS.md
--rw-r--r--   0        0        0     1082 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/LICENSE
--rw-r--r--   0        0        0     4936 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/README.md
--rw-r--r--   0        0        0      195 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/__init__.py
--rw-r--r--   0        0        0      201 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/__main__.py
--rw-r--r--   0        0        0     5803 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/_dfu_create.py
--rwxr-xr-x   0        0        0    20534 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/_dfu_upload.py
--rw-r--r--   0        0        0     6140 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/ble/__init__.py
--rw-r--r--   0        0        0     2943 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/ble/lwp3.py
--rw-r--r--   0        0        0     1000 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/ble/nus.py
--rw-r--r--   0        0        0     4206 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/ble/pybricks.py
--rw-r--r--   0        0        0     9758 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/cli/__init__.py
--rw-r--r--   0        0        0     4304 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/compile.py
--rw-r--r--   0        0        0    26391 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/connections.py
--rw-r--r--   0        0        0     6739 2021-05-18 22:19:49.552137 pybricksdev-1.0.0a8/pybricksdev/dfu.py
--rw-r--r--   0        0        0    13596 2021-05-18 22:19:49.556137 pybricksdev-1.0.0a8/pybricksdev/flash.py
--rw-r--r--   0        0        0     1191 2021-05-18 22:19:49.556137 pybricksdev-1.0.0a8/pybricksdev/resources/99-pybricksdev.rules
--rw-r--r--   0        0        0      336 2021-05-18 22:19:49.556137 pybricksdev-1.0.0a8/pybricksdev/resources/__init__.py
--rw-r--r--   0        0        0   148480 2021-05-18 22:19:49.556137 pybricksdev-1.0.0a8/pybricksdev/resources/dfu-util.exe
--rw-r--r--   0        0        0   137728 2021-05-18 22:19:49.556137 pybricksdev-1.0.0a8/pybricksdev/resources/libusb-1.0.dll
--rw-r--r--   0        0        0     2768 2021-05-18 22:19:49.556137 pybricksdev-1.0.0a8/pybricksdev/usbconnection.py
--rw-r--r--   0        0        0     1497 2021-05-18 22:19:49.556137 pybricksdev-1.0.0a8/pyproject.toml
--rw-r--r--   0        0        0     6155 2021-05-18 22:20:36.121095 pybricksdev-1.0.0a8/setup.py
--rw-r--r--   0        0        0     6241 2021-05-18 22:20:36.121616 pybricksdev-1.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0      194 2021-05-27 23:30:42.101977 pybricksdev-1.0.0a9/AUTHORS.md
+-rw-r--r--   0        0        0     1082 2021-05-27 23:30:42.101977 pybricksdev-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     5407 2021-05-27 23:30:42.101977 pybricksdev-1.0.0a9/README.md
+-rw-r--r--   0        0        0      215 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/__init__.py
+-rw-r--r--   0        0        0      201 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/__main__.py
+-rw-r--r--   0        0        0     5803 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/_dfu_create.py
+-rwxr-xr-x   0        0        0    20534 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/_dfu_upload.py
+-rw-r--r--   0        0        0     6110 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/ble/__init__.py
+-rw-r--r--   0        0        0     2770 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/ble/lwp3/__init__.py
+-rw-r--r--   0        0        0    24088 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/ble/lwp3/bytecodes.py
+-rw-r--r--   0        0        0    51941 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/ble/lwp3/messages.py
+-rw-r--r--   0        0        0     1000 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/ble/nus.py
+-rw-r--r--   0        0        0     4208 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/ble/pybricks.py
+-rw-r--r--   0        0        0    11168 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/cli/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/cli/lwp3/__init__.py
+-rw-r--r--   0        0        0     5357 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/cli/lwp3/repl.py
+-rw-r--r--   0        0        0     4285 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/compile.py
+-rw-r--r--   0        0        0    26261 2021-05-27 23:30:42.105977 pybricksdev-1.0.0a9/pybricksdev/connections.py
+-rw-r--r--   0        0        0     6741 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/dfu.py
+-rw-r--r--   0        0        0    11093 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/flash.py
+-rw-r--r--   0        0        0     1191 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/resources/99-pybricksdev.rules
+-rw-r--r--   0        0        0      336 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/resources/__init__.py
+-rw-r--r--   0        0        0   148480 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/resources/dfu-util.exe
+-rw-r--r--   0        0        0   137728 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/resources/libusb-1.0.dll
+-rw-r--r--   0        0        0        0 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/tools/__init__.py
+-rw-r--r--   0        0        0     2888 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/tools/checksum.py
+-rw-r--r--   0        0        0     2768 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pybricksdev/usbconnection.py
+-rw-r--r--   0        0        0     1696 2021-05-27 23:30:42.109977 pybricksdev-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     6765 2021-05-27 23:31:34.048910 pybricksdev-1.0.0a9/setup.py
+-rw-r--r--   0        0        0     6800 2021-05-27 23:31:34.049509 pybricksdev-1.0.0a9/PKG-INFO
```

### Comparing `pybricksdev-1.0.0a8/LICENSE` & `pybricksdev-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/README.md` & `pybricksdev-1.0.0a9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![Coverage Status](https://coveralls.io/repos/github/pybricks/pybricksdev/badge.svg?branch=master)](https://coveralls.io/github/pybricks/pybricksdev?branch=master)
+
 # Pybricks tools & interface library
 
 This is a package with tools for Pybricks developers. For regular users we
 recommend the [Pybricks Code][code] web IDE.
 
 This package contains both command line tools and a library to call equivalent
 operations from within a Python script.
@@ -24,34 +26,35 @@
 [py-dl]: https://www.python.org/downloads/
 [py38-win]: https://www.microsoft.com/en-us/p/python-38/9mssztt1n39l
 [asdf]: https://asdf-vm.com
 [pyenv]: https://github.com/pyenv/pyenv
 
 ### Command Line Tool
 
-We recommend using [pipx][pipx] to install `pybricksdev` as a command line tool.
-
-[pipx]: https://pipxproject.github.io/pipx/
-
-Be sure to install `pipx` in the Python 3.8 runtime:
-
-    python3.8 -m pip install --upgrade pip # ensure pip is up to date first
-    python3.8 -m pip install pipx
+We recommend using [pipx] to install `pybricksdev` as a command line tool.
 
-If this is the first time you have installed `pipx`, run this command:
-
-    python3.8 -m pipx ensurepath
+We also highly recommend installing `pipx` using a package manager such as `apt`,
+`brew`, etc. as suggested in the official [pipx installation] instructions.
 
+And don't forget to run `pipx ensurepath` after the initial installation.
 This will make it so that tools installed with `pipx` are in your `PATH`.
 You will need to restart any terminal windows for this to take effect. If that
 doesn't work, try logging out and logging back in.
 
 Then use `pipx` to install `pybricksdev`:
 
-    python3.8 -m pipx install pybricksdev
+    # POSIX shell (Linux, macOS, Cygwin, etc)
+    PIPX_DEFAULT_PYTHON=python3.8 pipx install pybricksdev
+
+Setting the `PIPX_DEFAULT_PYTHON` environment variable is only needed when
+`pipx` uses a different Python runtime other that Python 3.8. This may be the
+case if your package manager uses a different Python runtime.
+
+[pipx]: https://pipxproject.github.io/pipx/
+[pipx installation]: https://pipxproject.github.io/pipx/installation/
 
 #### Windows users
 
 If you are using the *Python Launcher for Windows* (installed by default with
 the official Python installer), then you will need to use `py -3.8` instead
 of `python3.8`.
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/_dfu_create.py` & `pybricksdev-1.0.0a9/pybricksdev/_dfu_create.py`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/pybricksdev/_dfu_upload.py` & `pybricksdev-1.0.0a9/pybricksdev/_dfu_upload.py`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/pybricksdev/ble/__init__.py` & `pybricksdev-1.0.0a9/pybricksdev/ble/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             it is not used as part of the matching criteria.
         service:
             The service UUID that is advertized.
         timeout:
             How long to search before giving up.
 
     Returns:
-        BLEDevice: The first detected matching device.
+        The first detected matching device.
 
     Raises:
         asyncio.TimeoutError:
             Device was not found within the timeout.
     """
     print(f"Searching for {name or service}")
 
@@ -97,16 +97,15 @@
         logger.debug("Disconnected.")
         self.connected = False
 
     async def connect(self, device: BLEDevice):
         """Connects to a BLE device.
 
         Arguments:
-            device (BLEDevice):
-                Client device
+            device: Client device
         """
 
         print("Connecting to", device)
         self.client = BleakClient(device)
         await self.client.connect(disconnected_callback=self.disconnected_handler)
         await self.client.start_notify(self.char_tx_UUID, self.data_handler)
         print("Connected successfully!")
@@ -184,16 +183,16 @@
         Arguments:
             timeout (float or None):
                 Time out to await. Same as asyncio.wait_for.
 
         Returns:
             bytearray: The reply.
 
-        Raises
-            TimeOutError. Same as asyncio.wait_for.
+        Raises:
+            asyncio.TimeoutError: Same as asyncio.wait_for.
         """
         # Await for the reply ready event to be raised.
         await asyncio.wait_for(self.reply_ready.wait(), timeout)
 
         # Return reply and clear internal buffer
         reply = self.reply
         self.prepare_reply()
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/ble/lwp3.py` & `pybricksdev-1.0.0a9/pybricksdev/ble/lwp3/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2021 The Pybricks Authors
 
-"""This module is used for Bluetooth Low Energy communications with devices
-that provide the LEGO Wireless Protocol v3.
+"""This module and its submodules are used for Bluetooth Low Energy
+communications with devices that provide the LEGO Wireless Protocol v3.
 """
 
 from enum import IntEnum
 
 # LEGO Wireless Protocol v3 is defined at:
 # https://lego.github.io/lego-ble-wireless-protocol-docs/
 
 
+LEGO_CID = 0x0397
+"""LEGO System A/S company identifier.
+
+This number is assigned by the Bluetooth SIG.
+
+https://www.bluetooth.com/specifications/assigned-numbers/company-identifiers/
+"""
+
+
 def _lwp3_uuid(short: int) -> str:
     """Get a 128-bit UUID from a ``short`` UUID.
 
     Args:
         short: The 16-bit UUID.
 
     Returns:
@@ -32,33 +41,14 @@
 LWP3_BOOTLOADER_SERVICE_UUID = _lwp3_uuid(0x1625)
 """LEGO wireless protocol v3 bootloader service UUID."""
 
 LWP3_BOOTLOADER_CHARACTERISTIC_UUID = _lwp3_uuid(0x1626)
 """LEGO wireless protocol v3 bootloader characteristic UUID."""
 
 
-class HubTypeId(IntEnum):
-    """Hub type identifiers.
-
-    These are used in both advertising data and in bytecodes.
-    """
-
-    MOVE_HUB = 0x40
-    """BOOST Move hub."""
-
-    CITY_HUB = 0x41
-    """City/train/Batmobile hub."""
-
-    TECHNIC_HUB = 0x80
-    """Technic medium (Control+) hub."""
-
-    PRIME_HUB = 0x84
-    """Technic large (SPIKE Prime, MINDSTORMS Inventor) hub."""
-
-
 # Bootloader characteristic bytecodes
 
 
 class BootloaderCommand(IntEnum):
     """Commands that are sent to the bootloader GATT characteristic."""
 
     ERASE_FLASH = 0x11
@@ -85,15 +75,15 @@
     Not all bootloaders support this command.
     """
 
     DISCONNECT = 0x88
     """Causes the remote device to disconnect from Bluetooth."""
 
 
-class BootloaderMessageType(IntEnum):
+class BootloaderMessageKind(IntEnum):
     """Type for messages received from bootlaoder GATT characteristic notifications.
 
     Messages that are a response to a command will have the same value as
     :class:`BootloaderCommand` instead of a value from this enum.
     """
 
     ERROR = 0x05
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/ble/nus.py` & `pybricksdev-1.0.0a9/pybricksdev/ble/nus.py`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/pybricksdev/ble/pybricks.py` & `pybricksdev-1.0.0a9/pybricksdev/ble/pybricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2021 The Pybricks Authors
 
-"""This module is used for Bluetooth Low Energy communications with devices
+"""
+This module is used for Bluetooth Low Energy communications with devices
 that provide the Pybricks GATT service.
 
 Device identification and connection
 ------------------------------------
 
-Devices that support this protocol MUST advertise the :data:`PYBRICKS_SERVICE_UUID:.
+Devices that support this protocol MUST advertise the :data:`PYBRICKS_SERVICE_UUID`.
 Connecting devices SHOULD then filter on this UUID to identify compatible devices.
 
 After connecting, programs SHOULD read the Software Revision characteristic of
 the Device Information Service to determine the Pybricks protocol version. This
 version can be used to determine the capabilities of the device.
 """
 
@@ -59,15 +60,15 @@
     Events are received from a device running Pybricks firmware.
     """
 
     STATUS_REPORT = 0
     """Status report.
 
     The payload is a 32-bit little-endian unsigned integer containing
-    :class:`StatusFlags`.
+    :class:`Status` flags.
 
     .. availability:: Since Pybricks protocol v1.0.0.
     """
 
 
 class Status(IntEnum):
     """Hub status indicators.
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/cli/__init__.py` & `pybricksdev-1.0.0a9/pybricksdev/cli/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from abc import ABC, abstractmethod
 from os import path
 
 import argcomplete
 from argcomplete.completers import FilesCompleter
 
 from .. import __name__ as MODULE_NAME, __version__ as MODULE_VERSION
-from ..ble.lwp3 import HubTypeId, LWP3_BOOTLOADER_SERVICE_UUID
+from ..ble.lwp3 import LWP3_BOOTLOADER_SERVICE_UUID
+from ..ble.lwp3.bytecodes import HubKind
 
 
 PROG_NAME = (
     f"{path.basename(sys.executable)} -m {MODULE_NAME}"
     if sys.argv[0].endswith("__main__.py")
     else path.basename(sys.argv[0])
 )
@@ -182,15 +183,15 @@
 
     async def run(self, args: argparse.Namespace):
         from ..flash import create_firmware
 
         print("Creating firmware")
         firmware, metadata = await create_firmware(args.firmware)
 
-        if metadata["device-id"] == HubTypeId.PRIME_HUB:
+        if metadata["device-id"] == HubKind.PRIME:
             from ..dfu import flash_dfu
 
             flash_dfu(firmware, metadata)
         else:
             from ..ble import find_device
             from ..flash import BootloaderConnection
 
@@ -237,30 +238,72 @@
         from ..dfu import restore_dfu
 
         restore_dfu(args.firmware)
 
 
 class DFU(Tool):
     def add_parser(self, subparsers: argparse._SubParsersAction):
-        parser = subparsers.add_parser(
+        self.parser = subparsers.add_parser(
             "dfu",
             help="use DFU to backup or restore firmware",
         )
-        parser.tool = self
-        self.subparsers = parser.add_subparsers(
+        self.parser.tool = self
+        self.subparsers = self.parser.add_subparsers(
             metavar="<action>", dest="action", help="the action to perform"
         )
 
         for tool in DFUBackup(), DFURestore():
             tool.add_parser(self.subparsers)
 
     def run(self, args: argparse.Namespace):
+        if args.action not in self.subparsers.choices:
+            self.parser.error(
+                f'Missing name of action: {"|".join(self.subparsers.choices.keys())}'
+            )
+
         return self.subparsers.choices[args.action].tool.run(args)
 
 
+class LWP3Repl(Tool):
+    def add_parser(self, subparsers: argparse._SubParsersAction):
+        parser = subparsers.add_parser(
+            "repl",
+            help="interactive REPL for sending and receiving LWP3 messages",
+        )
+        parser.tool = self
+
+    def run(self, args: argparse.Namespace):
+        from .lwp3.repl import setup_repl_logging, repl
+
+        setup_repl_logging()
+        return repl()
+
+
+class LWP3(Tool):
+    def add_parser(self, subparsers: argparse._SubParsersAction):
+        self.parser = subparsers.add_parser(
+            "lwp3", help="interact with devices using LWP3"
+        )
+        self.parser.tool = self
+        self.subparsers = self.parser.add_subparsers(
+            metavar="<lwp3-tool>", dest="lwp3_tool", help="the tool to run"
+        )
+
+        for tool in (LWP3Repl(),):
+            tool.add_parser(self.subparsers)
+
+    def run(self, args: argparse.Namespace):
+        if args.lwp3_tool not in self.subparsers.choices:
+            self.parser.error(
+                f'Missing name of tool: {"|".join(self.subparsers.choices.keys())}'
+            )
+
+        return self.subparsers.choices[args.lwp3_tool].tool.run(args)
+
+
 class Udev(Tool):
     def add_parser(self, subparsers: argparse._SubParsersAction):
         parser = subparsers.add_parser("udev", help="print udev rules to stdout")
         parser.tool = self
 
     async def run(self, args: argparse.Namespace):
         from importlib.resources import read_text
@@ -288,15 +331,15 @@
 
     subparsers = parser.add_subparsers(
         metavar="<tool>",
         dest="tool",
         help="the tool to use",
     )
 
-    for tool in Compile(), Run(), Flash(), DFU(), Udev():
+    for tool in Compile(), Run(), Flash(), DFU(), LWP3(), Udev():
         tool.add_parser(subparsers)
 
     argcomplete.autocomplete(parser)
     args = parser.parse_args()
 
     logging.basicConfig(
         format="%(asctime)s: %(levelname)s: %(name)s: %(message)s",
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/compile.py` & `pybricksdev-1.0.0a9/pybricksdev/compile.py`

 * *Files 7% similar despite different names*

```diff
@@ -114,30 +114,33 @@
     make_build_dir()
 
     # Path to temporary file.
     py_path = os.path.join(BUILD_DIR, TMP_PY_SCRIPT)
 
     # Write Python command to a file.
     with open(py_path, "w") as f:
-        f.write(py_string + "\n")
+        f.write(py_string)
+        f.write("\n")
 
     # Return path to file
     return py_path
 
 
 def print_mpy(data):
     # Print as string as a sanity check.
-    print("\nBytes:")
+    print()
+    print("Bytes:")
     print(data)
 
     # Print the bytes as a C byte array for development of new MicroPython
     # ports without usable I/O, REPL or otherwise.
     WIDTH = 8
-    print(
-        "\n// MPY file. Version: {0}. Size: {1}".format(data[1], len(data))
-        + "\nconst uint8_t script[] = "
-    )
+    print()
+    print(f"// MPY file. Version: {data[1]}. Size: {len(data)} bytes")
+    print("const uint8_t script[] = {")
+
     for i in range(0, len(data), WIDTH):
         chunk = data[i : i + WIDTH]
-        hex_repr = ["0x{0}".format(hex(i)[2:].zfill(2).upper()) for i in chunk]
-        print("    " + ", ".join(hex_repr) + ",")
+        hex_repr = [f"0x{i:02X}" for i in chunk]
+        print(f"    {', '.join(hex_repr)},")
+
     print("};")
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/connections.py` & `pybricksdev-1.0.0a9/pybricksdev/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 import json
 import logging
 import os
 import random
 import struct
 
 import asyncssh
-from bleak.backends.device import BLEDevice
-from bleak import BleakClient
 import semver
+from bleak import BleakClient
+from bleak.backends.device import BLEDevice
 from tqdm.auto import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
 from .ble import BLEConnection
 from .ble.nus import NUS_RX_UUID, NUS_TX_UUID
 from .ble.pybricks import (
-    Event,
     PYBRICKS_CONTROL_UUID,
     PYBRICKS_PROTOCOL_VERSION,
     SW_REV_UUID,
+    Event,
     Status,
 )
 from .compile import compile_file
+from .tools.checksum import xor_bytes
 from .usbconnection import USBConnection
 
 logger = logging.getLogger(__name__)
 
 
 class CharacterGlue:
     """Glues incoming bytes into a buffer and splits it into lines."""
@@ -245,17 +246,15 @@
                 Did not receive expected checksum for this message.
         """
 
         if len(data) > 100:
             raise ValueError("Cannot send this much data at once")
 
         # Compute expected reply
-        checksum = 0
-        for b in data:
-            checksum ^= b
+        checksum = xor_bytes(data, 0)
 
         # Clear existing checksum
         self.prepare_checksum()
 
         # Send the data
         await self.write(data)
 
@@ -742,23 +741,17 @@
     async def disconnect(self):
         if self.connected:
             logger.info("Disconnecting...")
             await self.client.disconnect()
         else:
             logger.debug("already disconnected")
 
-    def get_checksum(self, block):
-        checksum = 0
-        for b in block:
-            checksum ^= b
-        return checksum
-
     async def send_block(self, data):
         self.checksum_ready.clear()
-        self.expected_checksum = self.get_checksum(data)
+        self.expected_checksum = xor_bytes(data, 0)
         try:
             await self.client.write_gatt_char(NUS_RX_UUID, bytearray(data), False)
             await asyncio.wait_for(self.checksum_ready.wait(), timeout=0.5)
         except:  # noqa: E722
             # normally self.expected_checksum = -1 will be called in nus_handler()
             # but if we timeout or something like that, we need to reset it here
             self.expected_checksum = -1
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/dfu.py` & `pybricksdev-1.0.0a9/pybricksdev/dfu.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from subprocess import DEVNULL, call, check_call
 from tempfile import TemporaryDirectory
 from typing import BinaryIO, ContextManager
 
 from usb.core import NoBackendError, USBError
 
 from . import _dfu_upload, _dfu_create, resources
-from .ble.lwp3 import HubTypeId
+from .ble.lwp3.bytecodes import HubKind
 
 FIRMWARE_ADDRESS = 0x08008000
 FIRMWARE_SIZE = 1 * 1024 * 1024 - 32 * 1024  # 1MiB - 32KiB
 LEGO_VID = 0x0694
 SPIKE_PRIME_PID = 0x0008
 MINDSTORMS_INVENTOR_PID = 0x0011
 
@@ -130,15 +130,15 @@
                 )
             )
 
 
 def flash_dfu(firmware_bin: bytes, metadata: dict) -> None:
     """Flashes a firmware file using DFU."""
 
-    if metadata["device-id"] != HubTypeId.PRIME_HUB:
+    if metadata["device-id"] != HubKind.PRIME:
         print("Unknown hub type:", metadata["device-id"], file=sys.stderr)
         exit(1)
 
     with TemporaryDirectory() as out_dir:
         outfile = os.path.join(out_dir, "firmware.dfu")
         target = {"address": FIRMWARE_ADDRESS, "data": firmware_bin}
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/flash.py` & `pybricksdev-1.0.0a9/pybricksdev/flash.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,146 +1,36 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2019-2021 The Pybricks Authors
 
 import asyncio
 import io
-from collections import namedtuple
 import json
 import logging
 import os
 import platform
 import struct
 import sys
-from typing import Dict, Tuple
+import zipfile
+from collections import namedtuple
+from typing import BinaryIO, Dict, Tuple, Union
+
 from tqdm.auto import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
-import typing
-import zipfile
 
 from .ble import BLERequestsConnection
-from .ble.lwp3 import BootloaderCommand, HubTypeId
-from .compile import save_script, compile_file
+from .ble.lwp3 import BootloaderCommand
+from .ble.lwp3.bytecodes import HubKind
+from .compile import compile_file, save_script
+from .tools.checksum import crc32_checksum, sum_complement
 
 logger = logging.getLogger(__name__)
 
 
-def sum_complement(fw, max_size):
-    """Calculates the checksum of a firmware file using the sum complement
-    method of adding each 32-bit word and the returning the two's complement
-    as the checksum.
-
-    Arguments:
-        fw (file):
-            The firmware file (a binary buffer - e.g. a file opened in 'rb' mode)
-        max_size (int):
-            The maximum size of the firmware file.
-
-    Returns:
-        int: The correction needed to make the checksum of the file == 0.
-    """
-    checksum = 0
-    size = 0
-
-    while True:
-        word = fw.read(4)
-        if not word:
-            break
-        checksum += struct.unpack("I", word)[0]
-        size += 4
-
-    if size > max_size:
-        print('firmware + main.mpy is too large"', file=sys.stderr)
-        exit(1)
-
-    for _ in range(size, max_size, 4):
-        checksum += 0xFFFFFFFF
-
-    checksum &= 0xFFFFFFFF
-    correction = checksum and (1 << 32) - checksum or 0
-
-    return correction
-
-
-# thanks https://stackoverflow.com/a/33152544/1976323
-
-_CRC_TABLE = (
-    0x00000000,
-    0x04C11DB7,
-    0x09823B6E,
-    0x0D4326D9,
-    0x130476DC,
-    0x17C56B6B,
-    0x1A864DB2,
-    0x1E475005,
-    0x2608EDB8,
-    0x22C9F00F,
-    0x2F8AD6D6,
-    0x2B4BCB61,
-    0x350C9B64,
-    0x31CD86D3,
-    0x3C8EA00A,
-    0x384FBDBD,
-)
-
-
-def _dword(value):
-    return value & 0xFFFFFFFF
-
-
-def _crc32_fast(crc, data):
-    crc, data = _dword(crc), _dword(data)
-    crc ^= data
-    for _ in range(8):
-        crc = _dword(crc << 4) ^ _CRC_TABLE[crc >> 28]
-    return crc
-
-
-def _crc32_fast_block(crc, buffer):
-    for data in buffer:
-        crc = _crc32_fast(crc, data)
-    return crc
-
-
-def crc32_checksum(fw, max_size):
-    """Calculate the checksum of a firmware file using CRC-32 as implemented
-    in STM32 microprocessors.
-
-    Parameters
-    ----------
-    fw : file
-        The firmware file (a binary buffer - e.g. a file opened in 'rb' mode)
-    max_size : int
-        The maximum size of the firmware file.
-
-    Returns
-    -------
-    int
-        The checksum
-    """
-
-    # remove the last 4 bytes that are the placeholder for the checksum
-    try:
-        fw = fw.read()[:-4]
-    except AttributeError:
-        fw = fw[:-4]
-    if len(fw) + 4 > max_size:
-        raise ValueError("File is too large")
-
-    if len(fw) & 3:
-        raise ValueError("bytes_data length must be multiple of four")
-
-    crc = 0xFFFFFFFF
-    for index in range(0, len(fw), 4):
-        data = int.from_bytes(fw[index : index + 4], "little")
-        crc = _crc32_fast(crc, data)
-    return crc
-
-
 async def create_firmware(
-    firmware_zip: typing.Union[str, os.PathLike, typing.BinaryIO]
+    firmware_zip: Union[str, os.PathLike, BinaryIO]
 ) -> Tuple[bytes, dict]:
     """Creates a firmware blob from base firmware and main.mpy file.
 
     Arguments:
         firmware_zip:
             Path to the firmware zip file or a file-like object.
 
@@ -190,18 +80,18 @@
         print(f'Unknown checksum type "{metadata["checksum-type"]}"', file=sys.stderr)
         exit(1)
 
     return firmware, metadata
 
 
 # NAME, PAYLOAD_SIZE requirement
-HUB_INFO: Dict[HubTypeId, Tuple[str, int]] = {
-    HubTypeId.MOVE_HUB: ("Move Hub", 14),
-    HubTypeId.CITY_HUB: ("City Hub", 32),
-    HubTypeId.TECHNIC_HUB: ("Technic Hub", 32),
+HUB_INFO: Dict[HubKind, Tuple[str, int]] = {
+    HubKind.BOOST: ("Move Hub", 14),
+    HubKind.CITY: ("City Hub", 32),
+    HubKind.TECHNIC: ("Technic Hub", 32),
 }
 
 
 class BootloaderRequest:
     """Bootloader request structure."""
 
     def __init__(
@@ -368,16 +258,15 @@
         try:
             # Windows sometimes doesn't receive the reply to this command at all
             # or until another command is sent (buggy Bluetooth drivers?) so we
             # have a few hacks to special case this. City hub further complicates
             # things by having a buggy Bluetooth implementation in its bootloader.
             response = await self.bootloader_request(
                 self.ERASE_FLASH_CITY_HUB
-                if info.type_id == HubTypeId.CITY_HUB
-                and not platform.system() == "Windows"
+                if info.type_id == HubKind.CITY and not platform.system() == "Windows"
                 else self.ERASE_FLASH,
                 timeout=5,
             )
             logger.debug(response)
         except asyncio.TimeoutError:
             self.ignore_erase_reply = True
             logger.info("did not receive erase reply, continuing anyway")
@@ -423,15 +312,15 @@
                     request = self.PROGRAM_FLASH_FINAL
                 else:
                     # Otherwise, do not wait for confirmation.
                     request = self.PROGRAM_FLASH
 
                 # Pack the data in the expected format
                 data = struct.pack(
-                    "<BI" + "B" * len(payload), len(payload) + 4, address, *payload
+                    f"<BI{len(payload)}B", len(payload) + 4, address, *payload
                 )
                 response = await self.bootloader_request(request, data)
                 logger.debug(response)
                 pbar.update(len(payload))
                 address += len(payload)
 
         # Reboot the hub
```

### Comparing `pybricksdev-1.0.0a8/pybricksdev/resources/99-pybricksdev.rules` & `pybricksdev-1.0.0a9/pybricksdev/resources/99-pybricksdev.rules`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/pybricksdev/resources/dfu-util.exe` & `pybricksdev-1.0.0a9/pybricksdev/resources/dfu-util.exe`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/pybricksdev/resources/libusb-1.0.dll` & `pybricksdev-1.0.0a9/pybricksdev/resources/libusb-1.0.dll`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/pybricksdev/usbconnection.py` & `pybricksdev-1.0.0a9/pybricksdev/usbconnection.py`

 * *Files identical despite different names*

### Comparing `pybricksdev-1.0.0a8/pyproject.toml` & `pybricksdev-1.0.0a9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybricksdev"
-version = "1.0.0-alpha.8"
+version = "1.0.0-alpha.9"
 description = "Pybricks developer tools"
 authors = ["The Pybricks Authors <dev@pybricks.com>"]
 maintainers = ["Laurens Valk <laurens@pybricks.com>", "David Lechner <david@pybricks.com>" ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pybricks.com"
 repository = "https://github.com/pybricks/pybricksdev"
@@ -27,30 +27,40 @@
 pybricksdev = 'pybricksdev.cli:main'
 
 [tool.poetry.dependencies]
 aioserial = "^1.3.0"
 argcomplete = "^1.11.1"
 asyncssh = "^2.2.1"
 bleak = "^0.11.0"
-mpy-cross = "==1.12"
+mpy-cross = "1.14"
 python = "~3.8"
 tqdm = "^4.46.1"
 validators = "^0.18.2"
 pyusb = "^1.0.2"
 semver = "^2.13.0"
+appdirs = "^1.4.4"
+prompt-toolkit = "^3.0.18"
 
 [tool.poetry.dev-dependencies]
 black = {version = "^21.5b1", allow-prereleases = true}
+coverage = {extras = ["toml"], version = "^5.5"}
 flake8 = "^3.8.3"
 ipykernel = "^5.3.1"
 ipywidgets = "^7.6.3"
 nbstripout = "^0.3.8"
 notebook = "^6.0.3"
-pybricks = { git = "https://github.com/pybricks/pybricks-api.git", branch = "master" }
+pybricks = {version = "3.0.0rc1", allow-prereleases = true}
 pytest = "^5.2"
+Sphinx = "^4.0.2"
+sphinx-rtd-theme = "^0.5.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.black]
 target-version = ['py38']
+
+[tool.coverage.run]
+branch = true
+command_line = "-m pytest"
+source = ["pybricksdev"]
```

### Comparing `pybricksdev-1.0.0a8/setup.py` & `pybricksdev-1.0.0a9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['pybricksdev', 'pybricksdev.ble', 'pybricksdev.cli', 'pybricksdev.resources']
+['pybricksdev',
+ 'pybricksdev.ble',
+ 'pybricksdev.ble.lwp3',
+ 'pybricksdev.cli',
+ 'pybricksdev.cli.lwp3',
+ 'pybricksdev.resources',
+ 'pybricksdev.tools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aioserial>=1.3.0,<2.0.0',
+ 'appdirs>=1.4.4,<2.0.0',
  'argcomplete>=1.11.1,<2.0.0',
  'asyncssh>=2.2.1,<3.0.0',
  'bleak>=0.11.0,<0.12.0',
- 'mpy-cross==1.12',
+ 'mpy-cross==1.14',
+ 'prompt-toolkit>=3.0.18,<4.0.0',
  'pyusb>=1.0.2,<2.0.0',
  'semver>=2.13.0,<3.0.0',
  'tqdm>=4.46.1,<5.0.0',
  'validators>=0.18.2,<0.19.0']
 
 entry_points = \
 {'console_scripts': ['pybricksdev = pybricksdev.cli:main']}
 
 setup_kwargs = {
     'name': 'pybricksdev',
-    'version': '1.0.0a8',
+    'version': '1.0.0a9',
     'description': 'Pybricks developer tools',
-    'long_description': '# Pybricks tools & interface library\n\nThis is a package with tools for Pybricks developers. For regular users we\nrecommend the [Pybricks Code][code] web IDE.\n\nThis package contains both command line tools and a library to call equivalent\noperations from within a Python script.\n\n[code]: https://www.code.pybricks.com\n\n## Installation\n\n### Python Runtime\n\nWe currently only support Python 3.8.x. (Newer versions are not supported yet\nfor technical reasons.)\n\n- For Windows, use the [official Python installer][py-dl] or the [Windows Store][py38-win].\n- For Mac, use the [official Python installer][py-dl] or Homebrew (`brew install python@3.8`).\n- For Linux, use the distro provided `python3.8` or if not available, use a Python\n  runtime version manager such as [asdf][asdf] or [pyenv][pyenv].\n\n\n[py-dl]: https://www.python.org/downloads/\n[py38-win]: https://www.microsoft.com/en-us/p/python-38/9mssztt1n39l\n[asdf]: https://asdf-vm.com\n[pyenv]: https://github.com/pyenv/pyenv\n\n### Command Line Tool\n\nWe recommend using [pipx][pipx] to install `pybricksdev` as a command line tool.\n\n[pipx]: https://pipxproject.github.io/pipx/\n\nBe sure to install `pipx` in the Python 3.8 runtime:\n\n    python3.8 -m pip install --upgrade pip # ensure pip is up to date first\n    python3.8 -m pip install pipx\n\nIf this is the first time you have installed `pipx`, run this command:\n\n    python3.8 -m pipx ensurepath\n\nThis will make it so that tools installed with `pipx` are in your `PATH`.\nYou will need to restart any terminal windows for this to take effect. If that\ndoesn\'t work, try logging out and logging back in.\n\nThen use `pipx` to install `pybricksdev`:\n\n    python3.8 -m pipx install pybricksdev\n\n#### Windows users\n\nIf you are using the *Python Launcher for Windows* (installed by default with\nthe official Python installer), then you will need to use `py -3.8` instead\nof `python3.8`.\n\n    py -3.8 -m pip install --upgrade pip # ensure pip is up to date first\n    py -3.8 -m pip install pipx\n    py -3.8 -m pipx ensurepath\n    py -3.8 -m pipx install pybricksdev\n\n#### Linux USB\n\nOn Linux, `udev` rules are needed to allow access via USB. The `pybricksdev`\ncommand line tool contains a function to generate the required rules. Run the\nfollowing:\n\n    pybricksdev udev | sudo tee /etc/udev/rules.d/99-pybricksdev.rules\n\n### Library\n\nTo install `pybricksdev` as a library, we highly recommend using a virtual\nenvironment for your project. Our tool of choice for this is [poetry][poetry]:\n\n    poetry env use python3.8\n    poetry add pybricksdev\n\nOf course you can always use `pip` as well:\n\n    pip install pybrickdev --pre\n\n\n[poetry]: https://python-poetry.org\n\n\n## Using the Command Line Tool\n\nThe following are some examples of how to use the `pybricksdev` command line tool.\nFor additional info, run `pybricksdev --help`.\n\n### Flashing Pybricks MicroPython firmware\n\nMake sure the hub is off. Press and keep holding the hub button, and run:\n\n    pybricksdev flash <firmware.zip>\n\nReplace `<firmware.zip>` with the actual path to the firmware archive.\n\nYou may release the button once the progress bar first appears. \n\nThe SPIKE Prime Hub and MINDSTORMS Robot Inventor Hub do not have a Bluetooth\nbootloader. It is recommended to [install Pybricks using a Python script][issue-167] that\nruns on the hub. You can also flash the firmware manually using [DFU](dfu).\n\n\n[dfu]: ./README_dfu.rst\n[issue-167]: https://github.com/pybricks/support/issues/167\n\n\n### Running Pybricks MicroPython programs\n\nThis compiles a MicroPython script and sends it to a hub with Pybricks\nfirmware.\n\n    pybricksdev run --help\n\n    #\n    # ble connection examples:\n    #\n\n    # Run a one-liner on a Pybricks hub\n    pybricksdev run ble "print(\'Hello!\'); print(\'world!\');"\n\n    # Run script on the first device we find called Pybricks hub\n    pybricksdev run ble --name "Pybricks Hub" demo/shortdemo.py\n\n    # Run script on device with address 90:84:2B:4A:2B:75 (doesn\'t work on Mac)\n    pybricksdev run ble --name 90:84:2B:4A:2B:75 demo/shortdemo.py\n\n    #\n    # Other connection examples:\n    #\n\n    # Run script on ev3dev at 192.168.0.102\n    pybricksdev run ssh --name 192.168.0.102 demo/shortdemo.py\n\n    # Run script on primehub at\n    pybricksdev run usb --name "Pybricks Hub" demo/shortdemo.py\n\n\n### Compiling Pybricks MicroPython programs without running\n\nThis can be used to compile programs. Instead of also running them as above,\nit just prints the output on the screen instead.\n\n    pybricksdev compile demo/shortdemo.py\n\n    pybricksdev compile "print(\'Hello!\'); print(\'world!\');"\n\n\nThis is mainly intended for developers who want to quickly inspect the\ncontents of the `.mpy` file. To get the actual file, just use `mpy-cross`\ndirectly. We have used this tool in the past to test bare minimum MicroPython\nports that have neither a builtin compiler or any form of I/O yet. You can\npaste the generated `const uint8_t script[]` directly ito your C code.\n',
+    'long_description': '[![Coverage Status](https://coveralls.io/repos/github/pybricks/pybricksdev/badge.svg?branch=master)](https://coveralls.io/github/pybricks/pybricksdev?branch=master)\n\n# Pybricks tools & interface library\n\nThis is a package with tools for Pybricks developers. For regular users we\nrecommend the [Pybricks Code][code] web IDE.\n\nThis package contains both command line tools and a library to call equivalent\noperations from within a Python script.\n\n[code]: https://www.code.pybricks.com\n\n## Installation\n\n### Python Runtime\n\nWe currently only support Python 3.8.x. (Newer versions are not supported yet\nfor technical reasons.)\n\n- For Windows, use the [official Python installer][py-dl] or the [Windows Store][py38-win].\n- For Mac, use the [official Python installer][py-dl] or Homebrew (`brew install python@3.8`).\n- For Linux, use the distro provided `python3.8` or if not available, use a Python\n  runtime version manager such as [asdf][asdf] or [pyenv][pyenv].\n\n\n[py-dl]: https://www.python.org/downloads/\n[py38-win]: https://www.microsoft.com/en-us/p/python-38/9mssztt1n39l\n[asdf]: https://asdf-vm.com\n[pyenv]: https://github.com/pyenv/pyenv\n\n### Command Line Tool\n\nWe recommend using [pipx] to install `pybricksdev` as a command line tool.\n\nWe also highly recommend installing `pipx` using a package manager such as `apt`,\n`brew`, etc. as suggested in the official [pipx installation] instructions.\n\nAnd don\'t forget to run `pipx ensurepath` after the initial installation.\nThis will make it so that tools installed with `pipx` are in your `PATH`.\nYou will need to restart any terminal windows for this to take effect. If that\ndoesn\'t work, try logging out and logging back in.\n\nThen use `pipx` to install `pybricksdev`:\n\n    # POSIX shell (Linux, macOS, Cygwin, etc)\n    PIPX_DEFAULT_PYTHON=python3.8 pipx install pybricksdev\n\nSetting the `PIPX_DEFAULT_PYTHON` environment variable is only needed when\n`pipx` uses a different Python runtime other that Python 3.8. This may be the\ncase if your package manager uses a different Python runtime.\n\n[pipx]: https://pipxproject.github.io/pipx/\n[pipx installation]: https://pipxproject.github.io/pipx/installation/\n\n#### Windows users\n\nIf you are using the *Python Launcher for Windows* (installed by default with\nthe official Python installer), then you will need to use `py -3.8` instead\nof `python3.8`.\n\n    py -3.8 -m pip install --upgrade pip # ensure pip is up to date first\n    py -3.8 -m pip install pipx\n    py -3.8 -m pipx ensurepath\n    py -3.8 -m pipx install pybricksdev\n\n#### Linux USB\n\nOn Linux, `udev` rules are needed to allow access via USB. The `pybricksdev`\ncommand line tool contains a function to generate the required rules. Run the\nfollowing:\n\n    pybricksdev udev | sudo tee /etc/udev/rules.d/99-pybricksdev.rules\n\n### Library\n\nTo install `pybricksdev` as a library, we highly recommend using a virtual\nenvironment for your project. Our tool of choice for this is [poetry][poetry]:\n\n    poetry env use python3.8\n    poetry add pybricksdev\n\nOf course you can always use `pip` as well:\n\n    pip install pybrickdev --pre\n\n\n[poetry]: https://python-poetry.org\n\n\n## Using the Command Line Tool\n\nThe following are some examples of how to use the `pybricksdev` command line tool.\nFor additional info, run `pybricksdev --help`.\n\n### Flashing Pybricks MicroPython firmware\n\nMake sure the hub is off. Press and keep holding the hub button, and run:\n\n    pybricksdev flash <firmware.zip>\n\nReplace `<firmware.zip>` with the actual path to the firmware archive.\n\nYou may release the button once the progress bar first appears. \n\nThe SPIKE Prime Hub and MINDSTORMS Robot Inventor Hub do not have a Bluetooth\nbootloader. It is recommended to [install Pybricks using a Python script][issue-167] that\nruns on the hub. You can also flash the firmware manually using [DFU](dfu).\n\n\n[dfu]: ./README_dfu.rst\n[issue-167]: https://github.com/pybricks/support/issues/167\n\n\n### Running Pybricks MicroPython programs\n\nThis compiles a MicroPython script and sends it to a hub with Pybricks\nfirmware.\n\n    pybricksdev run --help\n\n    #\n    # ble connection examples:\n    #\n\n    # Run a one-liner on a Pybricks hub\n    pybricksdev run ble "print(\'Hello!\'); print(\'world!\');"\n\n    # Run script on the first device we find called Pybricks hub\n    pybricksdev run ble --name "Pybricks Hub" demo/shortdemo.py\n\n    # Run script on device with address 90:84:2B:4A:2B:75 (doesn\'t work on Mac)\n    pybricksdev run ble --name 90:84:2B:4A:2B:75 demo/shortdemo.py\n\n    #\n    # Other connection examples:\n    #\n\n    # Run script on ev3dev at 192.168.0.102\n    pybricksdev run ssh --name 192.168.0.102 demo/shortdemo.py\n\n    # Run script on primehub at\n    pybricksdev run usb --name "Pybricks Hub" demo/shortdemo.py\n\n\n### Compiling Pybricks MicroPython programs without running\n\nThis can be used to compile programs. Instead of also running them as above,\nit just prints the output on the screen instead.\n\n    pybricksdev compile demo/shortdemo.py\n\n    pybricksdev compile "print(\'Hello!\'); print(\'world!\');"\n\n\nThis is mainly intended for developers who want to quickly inspect the\ncontents of the `.mpy` file. To get the actual file, just use `mpy-cross`\ndirectly. We have used this tool in the past to test bare minimum MicroPython\nports that have neither a builtin compiler or any form of I/O yet. You can\npaste the generated `const uint8_t script[]` directly ito your C code.\n',
     'author': 'The Pybricks Authors',
     'author_email': 'dev@pybricks.com',
     'maintainer': 'Laurens Valk',
     'maintainer_email': 'laurens@pybricks.com',
     'url': 'https://pybricks.com',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pybricksdev-1.0.0a8/PKG-INFO` & `pybricksdev-1.0.0a9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybricksdev
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: Pybricks developer tools
 Home-page: https://pybricks.com
 License: MIT
 Author: The Pybricks Authors
 Author-email: dev@pybricks.com
 Maintainer: Laurens Valk
 Maintainer-email: laurens@pybricks.com
@@ -13,28 +13,32 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: aioserial (>=1.3.0,<2.0.0)
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: argcomplete (>=1.11.1,<2.0.0)
 Requires-Dist: asyncssh (>=2.2.1,<3.0.0)
 Requires-Dist: bleak (>=0.11.0,<0.12.0)
-Requires-Dist: mpy-cross (==1.12)
+Requires-Dist: mpy-cross (==1.14)
+Requires-Dist: prompt-toolkit (>=3.0.18,<4.0.0)
 Requires-Dist: pyusb (>=1.0.2,<2.0.0)
 Requires-Dist: semver (>=2.13.0,<3.0.0)
 Requires-Dist: tqdm (>=4.46.1,<5.0.0)
 Requires-Dist: validators (>=0.18.2,<0.19.0)
 Project-URL: Changelog, https://github.com/pybricks/pybricksdev/blob/master/CHANGELOG.md
 Project-URL: Issues, https://github.com/pybricks/support/issues
 Project-URL: Repository, https://github.com/pybricks/pybricksdev
 Project-URL: Support, https://github.com/pybricks/support/discussions
 Description-Content-Type: text/markdown
 
+[![Coverage Status](https://coveralls.io/repos/github/pybricks/pybricksdev/badge.svg?branch=master)](https://coveralls.io/github/pybricks/pybricksdev?branch=master)
+
 # Pybricks tools & interface library
 
 This is a package with tools for Pybricks developers. For regular users we
 recommend the [Pybricks Code][code] web IDE.
 
 This package contains both command line tools and a library to call equivalent
 operations from within a Python script.
@@ -57,34 +61,35 @@
 [py-dl]: https://www.python.org/downloads/
 [py38-win]: https://www.microsoft.com/en-us/p/python-38/9mssztt1n39l
 [asdf]: https://asdf-vm.com
 [pyenv]: https://github.com/pyenv/pyenv
 
 ### Command Line Tool
 
-We recommend using [pipx][pipx] to install `pybricksdev` as a command line tool.
-
-[pipx]: https://pipxproject.github.io/pipx/
-
-Be sure to install `pipx` in the Python 3.8 runtime:
-
-    python3.8 -m pip install --upgrade pip # ensure pip is up to date first
-    python3.8 -m pip install pipx
+We recommend using [pipx] to install `pybricksdev` as a command line tool.
 
-If this is the first time you have installed `pipx`, run this command:
-
-    python3.8 -m pipx ensurepath
+We also highly recommend installing `pipx` using a package manager such as `apt`,
+`brew`, etc. as suggested in the official [pipx installation] instructions.
 
+And don't forget to run `pipx ensurepath` after the initial installation.
 This will make it so that tools installed with `pipx` are in your `PATH`.
 You will need to restart any terminal windows for this to take effect. If that
 doesn't work, try logging out and logging back in.
 
 Then use `pipx` to install `pybricksdev`:
 
-    python3.8 -m pipx install pybricksdev
+    # POSIX shell (Linux, macOS, Cygwin, etc)
+    PIPX_DEFAULT_PYTHON=python3.8 pipx install pybricksdev
+
+Setting the `PIPX_DEFAULT_PYTHON` environment variable is only needed when
+`pipx` uses a different Python runtime other that Python 3.8. This may be the
+case if your package manager uses a different Python runtime.
+
+[pipx]: https://pipxproject.github.io/pipx/
+[pipx installation]: https://pipxproject.github.io/pipx/installation/
 
 #### Windows users
 
 If you are using the *Python Launcher for Windows* (installed by default with
 the official Python installer), then you will need to use `py -3.8` instead
 of `python3.8`.
```

