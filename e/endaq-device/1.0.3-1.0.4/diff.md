# Comparing `tmp/endaq_device-1.0.3-py3-none-any.whl.zip` & `tmp/endaq_device-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 203951 bytes, number of entries: 53
--rw-rw-rw-  2.0 fat    10481 b- defN 23-Apr-12 20:52 endaq/device/__init__.py
+Zip file size: 203967 bytes, number of entries: 53
+-rw-rw-rw-  2.0 fat    10481 b- defN 23-Apr-20 18:14 endaq/device/__init__.py
 -rw-rw-rw-  2.0 fat    53255 b- defN 23-Apr-12 20:52 endaq/device/base.py
--rw-rw-rw-  2.0 fat    84009 b- defN 23-Apr-12 20:52 endaq/device/command_interfaces.py
+-rw-rw-rw-  2.0 fat    84064 b- defN 23-Apr-20 18:14 endaq/device/command_interfaces.py
 -rw-rw-rw-  2.0 fat    55796 b- defN 23-Apr-12 20:52 endaq/device/config.py
 -rw-rw-rw-  2.0 fat     3867 b- defN 23-Jan-05 21:50 endaq/device/configio.py
 -rw-rw-rw-  2.0 fat     9806 b- defN 23-Jan-23 19:04 endaq/device/endaq.py
 -rw-rw-rw-  2.0 fat     3350 b- defN 22-Apr-25 21:19 endaq/device/esp32_codes.py
 -rw-rw-rw-  2.0 fat     1821 b- defN 23-Jan-05 21:50 endaq/device/exceptions.py
 -rw-rw-rw-  2.0 fat     7225 b- defN 23-Jan-05 21:50 endaq/device/hdlc.py
 -rw-rw-rw-  2.0 fat     9726 b- defN 23-Jan-05 21:50 endaq/device/legacy.py
@@ -43,13 +43,13 @@
 -rw-rw-rw-  2.0 fat     8977 b- defN 22-Dec-01 22:10 endaq/device/ui_defaults/Sx_R2000D40.py
 -rw-rw-rw-  2.0 fat     8976 b- defN 22-Dec-01 22:10 endaq/device/ui_defaults/Sx_R500D40.py
 -rw-rw-rw-  2.0 fat     9811 b- defN 22-Dec-01 22:10 endaq/device/ui_defaults/W8_E100D40.py
 -rw-rw-rw-  2.0 fat     9816 b- defN 22-Dec-01 22:10 endaq/device/ui_defaults/W8_E2000D40.py
 -rw-rw-rw-  2.0 fat     9810 b- defN 22-Dec-01 22:10 endaq/device/ui_defaults/W8_E25D40.py
 -rw-rw-rw-  2.0 fat     9487 b- defN 22-Dec-01 22:10 endaq/device/ui_defaults/Wx_D40.py
 -rw-rw-rw-  2.0 fat     2615 b- defN 23-Jan-05 21:50 endaq/device/ui_defaults/__init__.py
--rw-rw-rw-  2.0 fat     1106 b- defN 23-Apr-12 20:55 endaq_device-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3882 b- defN 23-Apr-12 20:55 endaq_device-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-12 20:55 endaq_device-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-12 20:55 endaq_device-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     4754 b- defN 23-Apr-12 20:55 endaq_device-1.0.3.dist-info/RECORD
-53 files, 605180 bytes uncompressed, 196329 bytes compressed:  67.6%
+-rw-rw-rw-  2.0 fat     1106 b- defN 23-Apr-20 18:16 endaq_device-1.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3882 b- defN 23-Apr-20 18:16 endaq_device-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 18:16 endaq_device-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-20 18:16 endaq_device-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     4754 b- defN 23-Apr-20 18:16 endaq_device-1.0.4.dist-info/RECORD
+53 files, 605235 bytes uncompressed, 196345 bytes compressed:  67.6%
```

## zipnote {}

```diff
@@ -138,23 +138,23 @@
 
 Filename: endaq/device/ui_defaults/Wx_D40.py
 Comment: 
 
 Filename: endaq/device/ui_defaults/__init__.py
 Comment: 
 
-Filename: endaq_device-1.0.3.dist-info/LICENSE
+Filename: endaq_device-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: endaq_device-1.0.3.dist-info/METADATA
+Filename: endaq_device-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: endaq_device-1.0.3.dist-info/WHEEL
+Filename: endaq_device-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: endaq_device-1.0.3.dist-info/top_level.txt
+Filename: endaq_device-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: endaq_device-1.0.3.dist-info/RECORD
+Filename: endaq_device-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## endaq/device/__init__.py

```diff
@@ -17,15 +17,15 @@
 from .exceptions import *
 from .endaq import EndaqS, EndaqW
 from .slamstick import SlamStickX, SlamStickC, SlamStickS
 from .types import Filename, Epoch
 
 from . import schemata
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 __all__ = ('CommandError', 'ConfigError', 'ConfigVersionError',
            'DeviceError', 'DeviceTimeout', 'UnsupportedFeature',
            'deviceChanged', 'findDevice', 'fromRecording', 'getDeviceList',
            'getDevices', 'getRecorder', 'isRecorder', 'onRecorder',
            'Recorder', 'EndaqS', 'EndaqW', 'SlamStickX', 'SlamStickC',
            'SlamStickS')
```

## endaq/device/command_interfaces.py

```diff
@@ -664,20 +664,22 @@
         fw = os.path.join(self.device.path, self.device._FW_UPDATE_FILE)
         up = os.path.join(self.device.path, self.device._USERPAGE_UPDATE_FILE)
         sig = fw + ".sig"
 
         fw_ext = os.path.splitext(str(firmware))[-1].lower()
         up_ext = os.path.splitext(str(userpage))[-1].lower()
 
+        keyRev = self.device.getInfo('KeyRev', 0)
+
         if firmware:
             if fw_ext not in ('.pkg', '.bin'):
                 raise TypeError("Firmware update file must be type .pkg or .bin")
 
             if fw_ext == '.bin':
-                if self.device.getInfo('KeyRev', 0):
+                if keyRev:
                     raise ValueError(
                             'Cannot apply unencrypted firmware (*.bin) to device '
                             'with encryption; use *.pkg version if available.')
 
                 # HACK: Unencrypted STM32-based firmware has `STM_` prefix
                 # FUTURE: Handle in Recorder subclass instead?
                 if str(self.device.mcuType).upper().startswith('STM'):
@@ -694,24 +696,23 @@
 
             if not (hasFw or hasUp):
                 raise FileNotFoundError(errno.ENOENT,
                                         "Device has no update files",
                                         os.path.dirname(fw))
 
             isPkg = hasFw and fw_ext == ".pkg"
-            isBin = hasFw and fw_ext == ".bin"
             signature = None if firmware is None or not isPkg else firmware + ".sig"
 
             if isPkg and not self._copyUpdateFile(signature, sig, clean):
                 raise FileNotFoundError(errno.ENOENT,
                                         "Firmware signature file not found",
                                         (signature or sig))
 
-            # Use 'secure' unless there's an unencrypted FW update (.bin)
-            secure = not isBin
+            # Use 'secure' if the device FW update is a .pkg, or it has keys installed.
+            secure = bool(isPkg or keyRev)
 
             return self._updateAll(secure=secure, timeout=timeout, callback=callback)
 
 
     def setKeys(self, keys: Union[bytearray, bytes],
                 timeout: float = 5,
                 callback: Optional[Callable] = None):
@@ -1880,14 +1881,15 @@
             :param callback: A function to call each response-checking
                 cycle. If the callback returns `True`, the wait for a response
                 will be cancelled. The callback function should take no
                 arguments.
             :return:
         """
         cmd = "SecureUpdateAll" if secure else "LegacyAll"
+        logger.debug(f'Sending command {cmd!r}')
         return self._runSimpleCommand({cmd: {}},
                                       timeoutMsg="Timed out waiting for update to begin",
                                       wait=wait,
                                       timeout=timeout,
                                       callback=callback)
```

## Comparing `endaq_device-1.0.3.dist-info/LICENSE` & `endaq_device-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `endaq_device-1.0.3.dist-info/METADATA` & `endaq_device-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endaq-device
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python API for enDAQ data recorders
 Home-page: https://github.com/MideTechnology/endaq-device
 Author: Mide Technology
 Author-email: help@mide.com
 License: MIT
 Keywords: endaq configure recorder hardware
 Platform: UNKNOWN
```

## Comparing `endaq_device-1.0.3.dist-info/RECORD` & `endaq_device-1.0.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-endaq/device/__init__.py,sha256=YaIF40ywdNwebeDznPT-9stlZ-jwDcKMpCe0I3nV8d8,10481
+endaq/device/__init__.py,sha256=j2Ay2EYCNZ1Lm1TDntKf1x3jDlERdFkAdojPOt5JpP8,10481
 endaq/device/base.py,sha256=rvZ7ePVlAFqqctbUIBj6t2ynv-3L1xtghbJOGnXllYc,53255
-endaq/device/command_interfaces.py,sha256=_FIarBEMv9z--IRJfzHpT-sqxckFRtjSepHRRxn-i64,84009
+endaq/device/command_interfaces.py,sha256=4VtDMdLP2d0vpTgD3d_q-reei-TQPPd-Im8iaOVKn6M,84064
 endaq/device/config.py,sha256=Mlo5TmnC9sDjgm4hasu0OkexhF15i1kfrBP5qFu1j4w,55796
 endaq/device/configio.py,sha256=12rjXHoFz8zdC2dRZFj0Hk6vRKtakGMlw4wgFncKIDQ,3867
 endaq/device/endaq.py,sha256=VENW8laBtMNgB6JoOgnySDPTTj8lAcud3JUCmqbPNzQ,9806
 endaq/device/esp32_codes.py,sha256=Q6w941R_iSpz3w73toQ71BOd3upwN68jMXLmb4T1n5Y,3350
 endaq/device/exceptions.py,sha256=b7uaesgyTp1jMkuFO6AMQXrKAN0mmQ0jsZBVqkmBLhA,1821
 endaq/device/hdlc.py,sha256=Gtz4GU8GLPqLqCJidkrfg__4NYB0ssnadGts5koHeW4,7225
 endaq/device/legacy.py,sha256=E-h0_kto_DAEGZY-fKvRDCDQdHi26ypVLaDhW_H1HMk,9726
@@ -42,12 +42,12 @@
 endaq/device/ui_defaults/Sx_R2000D40.py,sha256=_NgH5KeInTBiaySUsB3e4VVNrR-EBAjEOH5Ac1HDovE,8977
 endaq/device/ui_defaults/Sx_R500D40.py,sha256=tFCFhlhEkl6HE9ht6loi6FJWkMqSWqO83nhOh-CREJo,8976
 endaq/device/ui_defaults/W8_E100D40.py,sha256=E0OFPwiG7EozM7APTDNhXyWWVnOIOr6xjWCgzacTr_U,9811
 endaq/device/ui_defaults/W8_E2000D40.py,sha256=6d-D4_3SPNcsSOECxs5XApcn0SfOtHFoPNCUY_d7Nug,9816
 endaq/device/ui_defaults/W8_E25D40.py,sha256=E85cH4FhNJmJeP7NZUAtXyNJGO1A71cPV6swL5YgKz4,9810
 endaq/device/ui_defaults/Wx_D40.py,sha256=B5bJM_B7_DrDvblnQllPfJuUIpiexfsdQLW9Lh7ABC4,9487
 endaq/device/ui_defaults/__init__.py,sha256=2d4LWZ6XhiwPPIkSlypoz-3F1jY_jijHeDf38cjrsCE,2615
-endaq_device-1.0.3.dist-info/LICENSE,sha256=TC-m_nnEfxyqwCKl2SSKYw49jFwHbwLE_S5jTOY68LY,1106
-endaq_device-1.0.3.dist-info/METADATA,sha256=Go8RIaXhuL3vLKGzNPzloq7jof0evmPvlBp-y26ApPM,3882
-endaq_device-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-endaq_device-1.0.3.dist-info/top_level.txt,sha256=eqTVMT9FSjha3gc1ljU4eRn4mXdKGZp2v4WCciER_-w,6
-endaq_device-1.0.3.dist-info/RECORD,,
+endaq_device-1.0.4.dist-info/LICENSE,sha256=TC-m_nnEfxyqwCKl2SSKYw49jFwHbwLE_S5jTOY68LY,1106
+endaq_device-1.0.4.dist-info/METADATA,sha256=mBLHAGyp8BM5jhv5L7RE7MeqapXC-VzgR5E-n0GxleY,3882
+endaq_device-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+endaq_device-1.0.4.dist-info/top_level.txt,sha256=eqTVMT9FSjha3gc1ljU4eRn4mXdKGZp2v4WCciER_-w,6
+endaq_device-1.0.4.dist-info/RECORD,,
```

