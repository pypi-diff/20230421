# Comparing `tmp/esp-idf-monitor-1.0.3.tar.gz` & `tmp/esp-idf-monitor-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-1by69ntq/esp-idf-monitor-1.0.3.tar", last modified: Fri Apr 14 12:49:12 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-60e4z_0t/esp-idf-monitor-1.0.4.tar", last modified: Fri Apr 21 13:10:59 2023, max compression
```

## Comparing `esp-idf-monitor-1.0.3.tar` & `esp-idf-monitor-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/ansi_color_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/chip_specific_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/coredump.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/gdbhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/line_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/pc_address_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/base/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/gdb_panic_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17131 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/esp_idf_monitor/idf_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:49:12.000000 esp-idf-monitor-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-14 12:48:55.000000 esp-idf-monitor-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/ansi_color_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/chip_specific_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/coredump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/gdbhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/line_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/pc_address_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/gdb_panic_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17243 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/idf_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/setup.py
```

### Comparing `esp-idf-monitor-1.0.3/LICENSE` & `esp-idf-monitor-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/PKG-INFO` & `esp-idf-monitor-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.0.3/README.md` & `esp-idf-monitor-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/ansi_color_converter.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/ansi_color_converter.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/argument_parser.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/argument_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/chip_specific_config.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/chip_specific_config.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_parser.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/console_reader.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,23 @@
         self.cmd_queue = cmd_queue
         self.parser = parser
         self.test_mode = test_mode
 
     def run(self):
         # type: () -> None
         self.console.setup()
+        if os.name == 'posix':
+            # Use non-blocking busy read to avoid using unsecure TIOCSTI from console.cancel().
+            # TIOCSTI is not supported on kernels newer than 6.2.
+            import termios
+            new = termios.tcgetattr(self.console.fd)
+            # new[6] - 'cc': a list of the tty special characters
+            new[6][termios.VMIN] = 0  # minimum bytes to read
+            new[6][termios.VTIME] = 2  # timer of 0.1 second granularity
+            termios.tcsetattr(self.console.fd, termios.TCSANOW, new)
         try:
             while self.alive:
                 try:
                     if os.name == 'nt':
                         # Windows kludge: because the console.cancel() method doesn't
                         # seem to work to unblock getkey() on the Windows implementation.
                         #
@@ -49,38 +58,19 @@
                         # Therefore, we avoid calling it.
                         while self.alive:
                             time.sleep(0.1)
                         break
                     c = self.console.getkey()
                 except KeyboardInterrupt:
                     c = '\x03'
-                if c is not None:
+                if c:
                     ret = self.parser.parse(c)
                     if ret is not None:
                         (tag, cmd) = ret
                         # stop command should be executed last
                         if tag == TAG_CMD and cmd != CMD_STOP:
                             self.cmd_queue.put(ret)
                         else:
                             self.event_queue.put(ret)
 
         finally:
             self.console.cleanup()
-
-    def _cancel(self):
-        # type: () -> None
-        if os.name == 'posix' and not self.test_mode:
-            # this is the way cancel() is implemented in pyserial 3.3 or newer,
-            # older pyserial (3.1+) has cancellation implemented via 'select',
-            # which does not work when console sends an escape sequence response
-            #
-            # even older pyserial (<3.1) does not have this method
-            #
-            # on Windows there is a different (also hacky) fix, applied above.
-            #
-            # note that TIOCSTI is not implemented in WSL / bash-on-Windows.
-            # TODO: introduce some workaround to make it work there.
-            #
-            # Note: This would throw exception in testing mode when the stdin is connected to PTY.
-            import fcntl
-            import termios
-            fcntl.ioctl(self.console.fd, termios.TIOCSTI, b'\0')
```

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/constants.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/constants.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/coredump.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/coredump.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/gdbhelper.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/gdbhelper.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/line_matcher.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/line_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/logger.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/logger.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/output_helpers.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/output_helpers.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/pc_address_matcher.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/pc_address_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_handler.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_handler.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/serial_reader.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/stoppable_thread.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/base/web_socket_client.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/base/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/gdb_panic_server.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/gdb_panic_server.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor/idf_monitor.py` & `esp-idf-monitor-1.0.4/esp_idf_monitor/idf_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,16 @@
         self.serial.stdin.flush()
 
     def check_gdb_stub_and_run(self, line: bytes) -> None:
         return  # fake function for linux target
 
 
 def main() -> None:
+    if not sys.stdin.isatty():
+        sys.exit('error: Monitor requires standard input to be attached to TTY')
     parser = get_parser()
     args = parser.parse_args()
 
     # The port name is changed in cases described in the following lines. Use a local argument and
     # avoid the modification of args.port.
     port = args.port
```

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/PKG-INFO` & `esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.0.3
+Version: 1.0.4
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.0.3/esp_idf_monitor.egg-info/SOURCES.txt` & `esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.3/setup.py` & `esp-idf-monitor-1.0.4/setup.py`

 * *Files identical despite different names*

