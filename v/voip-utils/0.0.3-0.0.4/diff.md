# Comparing `tmp/voip-utils-0.0.3.tar.gz` & `tmp/voip-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voip-utils-0.0.3.tar", last modified: Thu Apr 20 17:22:34 2023, max compression
+gzip compressed data, was "voip-utils-0.0.4.tar", last modified: Thu Apr 20 20:19:20 2023, max compression
```

## Comparing `voip-utils-0.0.3.tar` & `voip-utils-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 17:22:34.288439 voip-utils-0.0.3/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.3/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 17:22:34.288439 voip-utils-0.0.3/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.3/README.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1969 2023-04-20 16:15:30.000000 voip-utils-0.0.3/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-04-20 17:22:34.288439 voip-utils-0.0.3/setup.cfg
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 17:22:34.288439 voip-utils-0.0.3/voip_utils/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.3/voip_utils/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.3/voip_utils/error.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7678 2023-04-06 20:24:07.000000 voip-utils-0.0.3/voip_utils/rtp_audio.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5984 2023-04-20 17:19:08.000000 voip-utils-0.0.3/voip_utils/sip.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.3/voip_utils/util.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5583 2023-04-20 17:21:30.000000 voip-utils-0.0.3/voip_utils/voip.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 17:22:34.288439 voip-utils-0.0.3/voip_utils.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 17:22:33.000000 voip-utils-0.0.3/voip_utils.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/requires.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-04-20 17:22:34.000000 voip-utils-0.0.3/voip_utils.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.3/voip_utils.egg-info/zip-safe
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 20:19:20.851068 voip-utils-0.0.4/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11357 2022-11-22 20:23:02.000000 voip-utils-0.0.4/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 20:19:20.851068 voip-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       39 2023-04-06 16:12:50.000000 voip-utils-0.0.4/README.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1969 2023-04-20 20:18:10.000000 voip-utils-0.0.4/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      299 2023-04-20 20:19:20.851068 voip-utils-0.0.4/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 20:19:20.851068 voip-utils-0.0.4/voip_utils/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      158 2023-04-06 17:22:11.000000 voip-utils-0.0.4/voip_utils/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      170 2023-04-06 15:51:26.000000 voip-utils-0.0.4/voip_utils/error.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7191 2023-04-20 20:08:03.000000 voip-utils-0.0.4/voip_utils/rtp_audio.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5984 2023-04-20 17:19:08.000000 voip-utils-0.0.4/voip_utils/sip.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      257 2023-04-06 18:58:36.000000 voip-utils-0.0.4/voip_utils/util.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5745 2023-04-20 20:17:37.000000 voip-utils-0.0.4/voip_utils/voip.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-20 20:19:20.851068 voip-utils-0.0.4/voip_utils.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      777 2023-04-20 20:19:20.000000 voip-utils-0.0.4/voip_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      366 2023-04-20 20:19:20.000000 voip-utils-0.0.4/voip_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-20 20:19:20.000000 voip-utils-0.0.4/voip_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       15 2023-04-20 20:19:20.000000 voip-utils-0.0.4/voip_utils.egg-info/requires.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       11 2023-04-20 20:19:20.000000 voip-utils-0.0.4/voip_utils.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-06 18:58:14.000000 voip-utils-0.0.4/voip_utils.egg-info/zip-safe
```

### Comparing `voip-utils-0.0.3/LICENSE.md` & `voip-utils-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.3/PKG-INFO` & `voip-utils-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `voip-utils-0.0.3/pyproject.toml` & `voip-utils-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "voip-utils"
-version     = "0.0.3"
+version     = "0.0.4"
 license     = {text = "Apache-2.0"}
 description = "Voice over IP Utilities"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "voip", "phone"]
```

### Comparing `voip-utils-0.0.3/voip_utils/rtp_audio.py` & `voip-utils-0.0.4/voip_utils/rtp_audio.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     """Prepares audio to send to an RTP client using OPUS."""
 
     opus_rate: int = 48000  # Hz
     opus_width: int = 2  # bytes
     opus_channels: int = 2
     opus_frame_size: int = 960  # samples per channel
     opus_payload: int = 123  # set by GrandStream
-    opus_bytes_per_frame: int = 960 * 2 * 2
+    opus_bytes_per_frame: int = 960 * 2 * 2  # 16-bit x stereo
 
     _rtp_flags: int = 0b10000000  # v2, no padding/extensions/CSRCs
     _rtp_sequence_num: int = 0
     _rtp_timestamp: int = 0
     _rtp_ssrc: int = 0
 
     _encoder: opuslib.api.encoder.Encoder = None
@@ -136,29 +136,14 @@
 
         # Set up OPUS encoder for VoIP
         self._encoder = opuslib.api.encoder.create_state(
             self.opus_rate,
             self.opus_width,
             opuslib.APPLICATION_VOIP,
         )
-        opuslib.api.encoder.encoder_ctl(
-            self._encoder,
-            opuslib.api.ctl.set_signal,
-            opuslib.SIGNAL_VOICE,
-        )
-        opuslib.api.encoder.encoder_ctl(
-            self._encoder,
-            opuslib.api.ctl.set_bandwidth,
-            opuslib.BANDWIDTH_WIDEBAND,  # for 16Khz
-        )
-        opuslib.api.encoder.encoder_ctl(
-            self._encoder,
-            opuslib.api.ctl.set_bitrate,
-            20_000,  # 16-20 kbit/s recommended for wideband
-        )
 
         self.reset()
 
     def reset(self):
         """Clear audio buffer and state."""
         self._audio_buffer = b""
         self._resample_state = None
```

### Comparing `voip-utils-0.0.3/voip_utils/sip.py` & `voip-utils-0.0.4/voip_utils/sip.py`

 * *Files identical despite different names*

### Comparing `voip-utils-0.0.3/voip_utils/voip.py` & `voip-utils-0.0.4/voip_utils/voip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Voice over IP (VoIP) implementation."""
 import asyncio
 import logging
 import socket
+import time
 from abc import ABC, abstractmethod
 from functools import partial
 from typing import Any, Callable, Optional, Set
 
 from .rtp_audio import RtpOpusInput, RtpOpusOutput
 from .sip import CallInfo, SdpInfo, SipDatagramProtocol
 
@@ -112,61 +113,66 @@
 
         self.on_chunk(audio_bytes)
 
     @abstractmethod
     def on_chunk(self, audio_bytes: bytes) -> None:
         """Handle raw audio chunk."""
 
-    async def send_audio(
+    def send_audio(
         self,
         audio_bytes: bytes,
         rate: int,
         width: int,
         channels: int,
         addr: Any = None,
-        sleep_ratio: float = 0.98,
+        sleep_ratio: float = 1.0,
         silence_before: float = 0.0,
     ) -> None:
         """Send audio from WAV file in chunks over RTP."""
         if self.transport is None:
             raise ValueError("Transport not set")
 
         addr = addr or self.addr
         if addr is None:
             raise ValueError("Destination address not set")
 
-        # Pause before sending to allow time for user to pick up phone.
-        await asyncio.sleep(silence_before)
-
         bytes_per_sample = width * channels
         bytes_per_frame = self._rtp_output.opus_frame_size * bytes_per_sample
-        seconds_per_rtp = self._rtp_output.opus_frame_size / self._rtp_output.opus_rate
 
+        # Generate all RTP packets up front
         sample_offset = 0
         samples_left = len(audio_bytes) // bytes_per_sample
+        rtp_packets: list[bytes] = []
         while samples_left > 0:
             bytes_offset = sample_offset * bytes_per_sample
             chunk = audio_bytes[bytes_offset : bytes_offset + bytes_per_frame]
             samples_in_chunk = len(chunk) // bytes_per_sample
             samples_left -= samples_in_chunk
 
             for rtp_bytes in self._rtp_output.process_audio(
                 chunk,
                 rate,
                 width,
                 channels,
                 is_end=samples_left <= 0,
             ):
-                # _LOGGER.debug(len(rtp_bytes))
-                self.transport.sendto(rtp_bytes, addr)
-
-                # Wait almost the full amount of time for the chunk.
-                #
-                # Sending too fast will cause the phone to skip chunks,
-                # since it doesn't seem to have a very large buffer.
-                #
-                # Sending too slow will cause audio artifacts if there is
-                # network jitter, which is why programs like GStreamer are
-                # much better at this.
-                await asyncio.sleep(seconds_per_rtp * sleep_ratio)
+                rtp_packets.append(rtp_bytes)
 
             sample_offset += samples_in_chunk
+
+        # Pause before sending to allow time for user to pick up phone.
+        time.sleep(silence_before)
+
+        # Send RTP in a steady stream, delaying between each packet to simulate real-time audio
+        seconds_per_rtp = self._rtp_output.opus_frame_size / self._rtp_output.opus_rate
+        for rtp_bytes in rtp_packets:
+            self.transport.sendto(rtp_bytes, addr)
+
+            # Wait almost the full amount of time for the chunk.
+            #
+            # Sending too fast will cause the phone to skip chunks,
+            # since it doesn't seem to have a very large buffer.
+            #
+            # Sending too slow will cause audio artifacts if there is
+            # network jitter, which is why programs like GStreamer are
+            # much better at this.
+            time.sleep(seconds_per_rtp * sleep_ratio)
```

### Comparing `voip-utils-0.0.3/voip_utils.egg-info/PKG-INFO` & `voip-utils-0.0.4/voip_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voip-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Voice over IP Utilities
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,voip,phone
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

