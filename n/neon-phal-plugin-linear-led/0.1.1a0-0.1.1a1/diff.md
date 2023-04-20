# Comparing `tmp/neon_phal_plugin_linear_led-0.1.1a0-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_linear_led-0.1.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11151 bytes, number of entries: 9
--rw-r--r--  2.0 unx    16507 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led/__init__.py
--rw-r--r--  2.0 unx     2662 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led/neopixel_led.py
--rw-r--r--  2.0 unx     2455 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led/smbus_led.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3641 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/WHEEL
--rw-r--r--  2.0 unx      229 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      911 b- defN 23-Apr-13 21:47 neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD
-9 files, 28159 bytes uncompressed, 9533 bytes compressed:  66.1%
+Zip file size: 11287 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    17185 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led/__init__.py
+-rw-r--r--  2.0 unx     2662 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led/neopixel_led.py
+-rw-r--r--  2.0 unx     2455 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led/smbus_led.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led-0.1.1a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3641 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led-0.1.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led-0.1.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      229 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led-0.1.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led-0.1.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      911 b- defN 23-Apr-20 22:53 neon_phal_plugin_linear_led-0.1.1a1.dist-info/RECORD
+9 files, 28837 bytes uncompressed, 9669 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: neon_phal_plugin_linear_led/neopixel_led.py
 Comment: 
 
 Filename: neon_phal_plugin_linear_led/smbus_led.py
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md
+Filename: neon_phal_plugin_linear_led-0.1.1a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA
+Filename: neon_phal_plugin_linear_led-0.1.1a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/WHEEL
+Filename: neon_phal_plugin_linear_led-0.1.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/entry_points.txt
+Filename: neon_phal_plugin_linear_led-0.1.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/top_level.txt
+Filename: neon_phal_plugin_linear_led-0.1.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD
+Filename: neon_phal_plugin_linear_led-0.1.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_linear_led/__init__.py

```diff
@@ -53,14 +53,18 @@
     def __init__(self, led: AbstractLed, bus=None, config=None, name=None):
         self.leds = led
         self.leds.fill(Color.BLACK.as_rgb_tuple())
 
         self._is_muted = False
         self._internet_disconnected = not is_connected()
 
+        # Assume initial state as default (until connection)
+        # TODO: Read fully offline setting from config
+        self._fully_offline = self._internet_disconnected
+
         # Init bus listeners after `_internet_disconnected` is defined
         PHALPlugin.__init__(self, bus=bus, name=name, config=config)
 
         self.listen_color = Color.THEME
         self.mute_color = Color.BURNT_ORANGE
         self.sleep_color = Color.RED
         self.error_color = Color.RED
@@ -167,18 +171,24 @@
         # Audio hardware handlers
         self.bus.on('mycroft.mic.mute', self.on_mic_mute)
         self.bus.on('mycroft.mic.unmute', self.on_mic_unmute)
         self.bus.on('mycroft.mic.error', self.on_mic_error)
         self.bus.on('mycroft.volume.increase', self.on_volume_increase)
         self.bus.on('mycroft.volume.decrease', self.on_volume_decrease)
 
-        # Internet event handler
+        # Network event handler
+        self.bus.on("mycroft.network.state", self.on_network_state)
+
+        # TODO: below events should be consumed in connectivity events plugin
+        #       directly
+        # Plugin notify offline mode selected
+        self.bus.on('ovos.phal.wifi.plugin.fully_offline',
+                    self.on_fully_offline)
+        # Generic internet connected notification
         self.bus.on('mycroft.internet.connected', self.on_internet_connected)
-        # self.bus.on("ovos.wifi.setup.completed", self.on_internet_connected)
-        self.bus.on('ovos.phal.wifi.plugin.fully_offline', self.on_fully_offline)
 
         # Core API handlers
         self.bus.on('neon.linear_led.show_animation', self.on_show_animation)
         self.bus.on('ovos.theme.get.response', self.on_theme_update)
 
         # User interaction handlers
         self.bus.on('recognizer_loop:utterance', self.on_utterance)
@@ -195,53 +205,64 @@
         if self._is_muted:
             LOG.debug("Mic Muted")
             self.on_mic_mute()
         elif self._internet_disconnected:
             LOG.debug("Internet Disconnected")
             self.on_no_internet()
 
+    def on_network_state(self, message):
+        """
+        Handle a network state update from the connectivity events plugin
+        :param message: Message containing network state
+        """
+        new_state = message.data.get("state")
+        if new_state == "connected":
+            self.on_internet_connected(message)
+        elif new_state == "disconnected" and not self._fully_offline:
+            self.on_no_internet(message)
+        else:
+            LOG.warning(f"Unhandled network state change: {message.data}")
+
     @transient_animation
     def on_fully_offline(self, message):
         """
         Handle an event notifying the user selected offline operation
         :param message: Message object
         """
         LOG.info("Wifi plugin notified fully offline mode selected")
+        self._fully_offline = True
         self._internet_disconnected = False
         self._disconnected_animation.stop()
 
     def on_no_internet(self, message=None):
         """
         Handle an event notifying internet connection was unexpectedly lost.
         :param message: Message object
         """
         LOG.debug("Bus notified no internet")
         if self._internet_disconnected:
             LOG.debug(f"Already disconnected")
             return
-        self._internet_disconnected = True
-        message = message.forward("ovos.phal.wifi.plugin.status") if \
-            message else Message("ovos.phal.wifi.plugin.status")
-        resp = self.bus.wait_for_response(message)
-        if resp and not resp.data.get('watchdog_active'):
-            LOG.info(f"Watchdog inactive: {resp.data}")
+        if self._fully_offline:
+            LOG.info("In Offline Mode")
             return
+        self._internet_disconnected = True
         LOG.debug(f"Starting Internet Disconnected Animation")
-        # TODO: Check ready settings and skill internet setting in config?
         with self._led_lock:
             self._disconnected_animation.start()
 
     @transient_animation
     def on_internet_connected(self, message):
         """
         Handle an event notifying internet connection has been established.
         :param message: Message object
         """
         LOG.debug(f"Internet connection re-established")
         self._internet_disconnected = False
+        self._fully_offline = False
         self._disconnected_animation.stop()
 
     @transient_animation
     def on_complete_intent_failure(self, message):
         """
         Handle an event notifying intent service failure.
         :param message: Message object
```

## Comparing `neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md` & `neon_phal_plugin_linear_led-0.1.1a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA` & `neon_phal_plugin_linear_led-0.1.1a1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-linear-led
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: Linear/Ring LED Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-linear_led
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD` & `neon_phal_plugin_linear_led-0.1.1a1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-neon_phal_plugin_linear_led/__init__.py,sha256=JUQMmZi_NoTCU34cIO5lA3R3FRYO9Ad7IRtPvoDqEuU,16507
+neon_phal_plugin_linear_led/__init__.py,sha256=WnPOT9PXOauyYyuLMgyGj3L9cUdLYDLB5oN8EnKZ_Rs,17185
 neon_phal_plugin_linear_led/neopixel_led.py,sha256=j6tf2UQ8zO3zjj1MJkYbnxSKcRDUhISnKh_yBoeHavU,2662
 neon_phal_plugin_linear_led/smbus_led.py,sha256=DxXb5fuu6uvzX92Br3MEn5CbmF4KWVbTn2OvBQ9xUIQ,2455
-neon_phal_plugin_linear_led-0.1.1a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_linear_led-0.1.1a0.dist-info/METADATA,sha256=6xxXRPQoUSN3oahWgW9-vlkTuLEUMOEaFPep1sEiPlM,3641
-neon_phal_plugin_linear_led-0.1.1a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_linear_led-0.1.1a0.dist-info/entry_points.txt,sha256=kam9ztzRLdfMrjVQYjtbcVmtJZTxufNnjnWqMAH992o,229
-neon_phal_plugin_linear_led-0.1.1a0.dist-info/top_level.txt,sha256=Tbx4PyK54fa4KBJAb7RI0xMAqRPoUNmLHSEkVtQfzJ8,28
-neon_phal_plugin_linear_led-0.1.1a0.dist-info/RECORD,,
+neon_phal_plugin_linear_led-0.1.1a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_linear_led-0.1.1a1.dist-info/METADATA,sha256=uwc3-EZCbe0CZTd4CqF4Z9PESnGjWs6fAgOEQGMyiuQ,3641
+neon_phal_plugin_linear_led-0.1.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_linear_led-0.1.1a1.dist-info/entry_points.txt,sha256=kam9ztzRLdfMrjVQYjtbcVmtJZTxufNnjnWqMAH992o,229
+neon_phal_plugin_linear_led-0.1.1a1.dist-info/top_level.txt,sha256=Tbx4PyK54fa4KBJAb7RI0xMAqRPoUNmLHSEkVtQfzJ8,28
+neon_phal_plugin_linear_led-0.1.1a1.dist-info/RECORD,,
```

