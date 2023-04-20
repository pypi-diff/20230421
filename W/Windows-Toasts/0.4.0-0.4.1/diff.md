# Comparing `tmp/windows-toasts-0.4.0.tar.gz` & `tmp/Windows-Toasts-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windows-toasts-0.4.0.tar", last modified: Sat Mar 18 13:49:47 2023, max compression
+gzip compressed data, was "Windows-Toasts-0.4.1.tar", last modified: Thu Apr 20 22:41:51 2023, max compression
```

## Comparing `windows-toasts-0.4.0.tar` & `Windows-Toasts-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-18 13:49:47.402768 windows-toasts-0.4.0/
--rw-rw-rw-   0        0        0    11556 2022-02-19 10:55:53.000000 windows-toasts-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       69 2023-03-18 13:42:42.000000 windows-toasts-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3429 2023-03-18 13:49:47.402768 windows-toasts-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2409 2023-03-15 19:30:14.000000 windows-toasts-0.4.0/README.md
--rw-rw-rw-   0        0        0      362 2023-03-18 13:17:33.000000 windows-toasts-0.4.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-18 13:49:47.382215 windows-toasts-0.4.0/scripts/
--rw-rw-rw-   0        0        0        0 2023-03-11 02:56:42.000000 windows-toasts-0.4.0/scripts/__init__.py
--rw-rw-rw-   0        0        0     1662 2023-03-18 10:39:40.000000 windows-toasts-0.4.0/scripts/register_hkey_aumid.py
--rw-rw-rw-   0        0        0       42 2023-03-18 13:49:47.402768 windows-toasts-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1628 2023-03-18 13:46:39.000000 windows-toasts-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-18 13:49:47.376142 windows-toasts-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-18 13:49:47.388216 windows-toasts-0.4.0/src/windows_toasts/
--rw-rw-rw-   0        0        0     1633 2023-03-17 20:56:48.000000 windows-toasts-0.4.0/src/windows_toasts/__init__.py
--rw-rw-rw-   0        0        0      245 2023-03-12 10:37:45.000000 windows-toasts-0.4.0/src/windows_toasts/_version.py
--rw-rw-rw-   0        0        0     1370 2023-03-18 13:25:35.000000 windows-toasts-0.4.0/src/windows_toasts/events.py
--rw-rw-rw-   0        0        0        0 2022-02-26 17:24:59.000000 windows-toasts-0.4.0/src/windows_toasts/py.typed
--rw-rw-rw-   0        0        0     1640 2023-03-17 22:03:36.000000 windows-toasts-0.4.0/src/windows_toasts/toast_audio.py
--rw-rw-rw-   0        0        0    14182 2023-03-18 13:18:09.000000 windows-toasts-0.4.0/src/windows_toasts/toast_document.py
--rw-rw-rw-   0        0        0    15793 2023-03-18 13:15:46.000000 windows-toasts-0.4.0/src/windows_toasts/toast_types.py
--rw-rw-rw-   0        0        0    10859 2023-03-18 13:20:31.000000 windows-toasts-0.4.0/src/windows_toasts/toasters.py
--rw-rw-rw-   0        0        0     6970 2023-03-18 10:31:37.000000 windows-toasts-0.4.0/src/windows_toasts/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-03-18 13:49:47.389213 windows-toasts-0.4.0/tests/
--rw-rw-rw-   0        0        0     1494 2023-03-17 19:28:03.000000 windows-toasts-0.4.0/tests/test_aumid.py
--rw-rw-rw-   0        0        0    10094 2023-03-18 13:18:09.000000 windows-toasts-0.4.0/tests/test_toasts.py
-drwxrwxrwx   0        0        0        0 2023-03-18 13:49:47.401762 windows-toasts-0.4.0/windows_toasts.egg-info/
--rw-rw-rw-   0        0        0     3429 2023-03-18 13:49:47.000000 windows-toasts-0.4.0/windows_toasts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      698 2023-03-18 13:49:47.000000 windows-toasts-0.4.0/windows_toasts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-18 13:49:47.000000 windows-toasts-0.4.0/windows_toasts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-03-18 13:49:47.000000 windows-toasts-0.4.0/windows_toasts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-18 13:36:28.000000 windows-toasts-0.4.0/windows_toasts.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-03-18 13:49:47.000000 windows-toasts-0.4.0/windows_toasts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-03-18 13:49:47.000000 windows-toasts-0.4.0/windows_toasts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 22:41:51.892996 Windows-Toasts-0.4.1/
+-rw-rw-rw-   0        0        0    11556 2022-02-19 10:55:53.000000 Windows-Toasts-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0       69 2023-03-18 13:54:37.000000 Windows-Toasts-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3450 2023-04-20 22:41:51.892996 Windows-Toasts-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2409 2023-03-15 19:30:14.000000 Windows-Toasts-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 22:41:51.884930 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/
+-rw-rw-rw-   0        0        0     3450 2023-04-20 22:41:51.000000 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      698 2023-04-20 22:41:51.000000 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 22:41:51.000000 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-20 22:41:51.000000 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-24 23:36:24.000000 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-04-20 22:41:51.000000 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-20 22:41:51.000000 Windows-Toasts-0.4.1/Windows_Toasts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      362 2023-03-18 13:17:33.000000 Windows-Toasts-0.4.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-20 22:41:51.885929 Windows-Toasts-0.4.1/scripts/
+-rw-rw-rw-   0        0        0        0 2023-03-11 02:56:42.000000 Windows-Toasts-0.4.1/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1662 2023-03-18 10:39:40.000000 Windows-Toasts-0.4.1/scripts/register_hkey_aumid.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 22:41:51.892996 Windows-Toasts-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1723 2023-04-20 22:06:22.000000 Windows-Toasts-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:41:51.875842 Windows-Toasts-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 22:41:51.891446 Windows-Toasts-0.4.1/src/windows_toasts/
+-rw-rw-rw-   0        0        0     1684 2023-04-11 10:41:36.000000 Windows-Toasts-0.4.1/src/windows_toasts/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-04-20 22:25:13.000000 Windows-Toasts-0.4.1/src/windows_toasts/_version.py
+-rw-rw-rw-   0        0        0     1322 2023-04-12 22:03:28.000000 Windows-Toasts-0.4.1/src/windows_toasts/events.py
+-rw-rw-rw-   0        0        0        0 2022-02-26 17:24:59.000000 Windows-Toasts-0.4.1/src/windows_toasts/py.typed
+-rw-rw-rw-   0        0        0     1640 2023-03-17 22:03:36.000000 Windows-Toasts-0.4.1/src/windows_toasts/toast_audio.py
+-rw-rw-rw-   0        0        0    14182 2023-04-20 17:28:34.000000 Windows-Toasts-0.4.1/src/windows_toasts/toast_document.py
+-rw-rw-rw-   0        0        0    15793 2023-04-20 17:28:34.000000 Windows-Toasts-0.4.1/src/windows_toasts/toast_types.py
+-rw-rw-rw-   0        0        0    11096 2023-04-20 17:28:34.000000 Windows-Toasts-0.4.1/src/windows_toasts/toasters.py
+-rw-rw-rw-   0        0        0     6970 2023-03-18 10:31:37.000000 Windows-Toasts-0.4.1/src/windows_toasts/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:41:51.891984 Windows-Toasts-0.4.1/tests/
+-rw-rw-rw-   0        0        0     1494 2023-03-17 19:28:03.000000 Windows-Toasts-0.4.1/tests/test_aumid.py
+-rw-rw-rw-   0        0        0    10270 2023-04-20 21:45:51.000000 Windows-Toasts-0.4.1/tests/test_toasts.py
```

### Comparing `windows-toasts-0.4.0/LICENSE` & `Windows-Toasts-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/PKG-INFO` & `Windows-Toasts-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: windows-toasts
-Version: 0.4.0
-Summary: Windows toast notifications sender
+Name: Windows-Toasts
+Version: 0.4.1
+Summary: Python library used to send toast notifications on Windows machines
 Home-page: https://github.com/DatGuy1/Windows-Toasts
 Author: DatGuy
 Author-email: datguysteam@gmail.com
 License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/DatGuy1/Windows-Toasts/issues
 Project-URL: Documentation, https://windows-toasts.readthedocs.io
+Project-URL: Source, https://github.com/DatGuy1/Windows-Toasts
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `windows-toasts-0.4.0/README.md` & `Windows-Toasts-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/scripts/register_hkey_aumid.py` & `Windows-Toasts-0.4.1/scripts/register_hkey_aumid.py`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/setup.py` & `Windows-Toasts-0.4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 from setuptools import setup
 
 packages = ["windows_toasts", "scripts"]
 
-requires = ["winsdk"]
+requires = ["winsdk==1.0.0b9"]
 
 with open("README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
+about = {}
+with open("src/windows_toasts/_version.py", "r") as f:
+    exec(f.read(), None, about)
+
 setup(
-    name="windows-toasts",
-    version="0.4.0",
-    description="Windows toast notifications sender",
+    name=about["__title__"],
+    version=about["__version__"],
+    description=about["__description__"],
     long_description=readme,
     long_description_content_type="text/markdown",
-    author="DatGuy",
+    author=about["__author__"],
     author_email="datguysteam@gmail.com",
-    url="https://github.com/DatGuy1/Windows-Toasts",
+    url=about["__url__"],
     packages=packages,
     package_dir={"windows_toasts": "src/windows_toasts"},
     package_data={"": ["LICENSE"], "windows_toasts": ["py.typed"]},
     include_package_data=True,
     entry_points={"console_scripts": ["register_hkey_aumid = scripts.register_hkey_aumid:main"]},
     python_requires=">=3.8",
     install_requires=requires,
-    license="Apache 2.0",
+    license=about["__license__"],
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Operating System :: Microsoft :: Windows :: Windows 11",
     ],
     project_urls={
-        "Bug Tracker": "https://github.com/DatGuy1/Windows-Toasts/issues",
         "Documentation": "https://windows-toasts.readthedocs.io",
+        "Source": "https://github.com/DatGuy1/Windows-Toasts",
     },
 )
```

### Comparing `windows-toasts-0.4.0/src/windows_toasts/__init__.py` & `Windows-Toasts-0.4.1/src/windows_toasts/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ._version import __author__, __description__, __license__, __title__, __url__, __version__  # noqa: F401
-from .events import ToastActivatedEventArgs, ToastDismissedEventArgs, ToastFailedEventArgs
+from .events import ToastActivatedEventArgs, ToastDismissalReason, ToastDismissedEventArgs, ToastFailedEventArgs
 from .toast_audio import AudioSource, ToastAudio
 from .toast_types import (
     ToastImageAndText1,
     ToastImageAndText2,
     ToastImageAndText3,
     ToastImageAndText4,
     ToastText1,
@@ -31,14 +31,15 @@
     "__description__",
     "__license__",
     "__title__",
     "__url__",
     "__version__",
     # events.py
     "ToastActivatedEventArgs",
+    "ToastDismissalReason",
     "ToastDismissedEventArgs",
     "ToastFailedEventArgs",
     # toast_audio.py
     "AudioSource",
     "ToastAudio",
     # toast_types.py
     "ToastImageAndText1",
```

### Comparing `windows-toasts-0.4.0/src/windows_toasts/events.py` & `Windows-Toasts-0.4.1/src/windows_toasts/events.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Dict, Optional
 
-# noinspection PyProtectedMember
-from winsdk import _winrt
+from winsdk import system
 from winsdk.windows.foundation import IPropertyValue
-
-# noinspection PyUnresolvedReferences
 from winsdk.windows.ui.notifications import (  # noqa: F401
     ToastActivatedEventArgs as WinRtToastActivatedEventArgs,
+    ToastDismissalReason,
     ToastDismissedEventArgs,
     ToastFailedEventArgs,
 )
 
 
 @dataclass
 class ToastActivatedEventArgs:
@@ -24,15 +22,15 @@
     arguments: Optional[str] = None
     """Arguments provided to :func:`~windows_toasts.toast_types.Toast.AddAction`"""
     inputs: Optional[dict] = None
     """Inputs received when using :func:`~windows_toasts.toast_types.Toast.AddInput`"""
 
     # noinspection PyProtectedMember
     @classmethod
-    def fromWinRt(cls, eventArgs: _winrt.Object) -> ToastActivatedEventArgs:
+    def fromWinRt(cls, eventArgs: system.Object) -> ToastActivatedEventArgs:
         activatedEventArgs = WinRtToastActivatedEventArgs._from(eventArgs)
         receivedInputs: Optional[Dict[str, str]] = None
         try:
             receivedInputs = {k: IPropertyValue._from(v).get_string() for k, v in activatedEventArgs.user_input.items()}
         except OSError:
             pass
```

### Comparing `windows-toasts-0.4.0/src/windows_toasts/toast_audio.py` & `Windows-Toasts-0.4.1/src/windows_toasts/toast_audio.py`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/src/windows_toasts/toast_document.py` & `Windows-Toasts-0.4.1/src/windows_toasts/toast_document.py`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/src/windows_toasts/toast_types.py` & `Windows-Toasts-0.4.1/src/windows_toasts/toast_types.py`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/src/windows_toasts/toasters.py` & `Windows-Toasts-0.4.1/src/windows_toasts/toasters.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,20 @@
 
     progressBar = toast.progress_bar
     if progressBar is not None:
         notificationData.values["status"] = progressBar.status
         notificationData.values.insert(
             "progress", "indeterminate" if progressBar.progress is None else str(progressBar.progress)
         )
-        notificationData.values["progress_override"] = progressBar.progress_override or ""
+        progressOverride = progressBar.progress_override
+        if progressOverride is None and progressBar.progress is not None:
+            # Recreate default Windows behaviour while still allowing it to be changed in the future
+            progressOverride = f"{round(progressBar.progress * 100)}%"
+
+        notificationData.values["progress_override"] = progressOverride
         notificationData.values["caption"] = progressBar.caption or ""
 
     return notificationData
 
 
 def _build_toast_notification(toast: Toast, toastNotification: ToastNotificationT) -> ToastNotificationT:
     """
@@ -187,16 +192,15 @@
         self.toastNotifier.remove_from_schedule(targetNotification)
         return True
 
     def clear_toasts(self) -> None:
         """
         Clear toasts popped by this toaster
         """
-        # noinspection PyUnresolvedReferences
-        toastHistory: ToastNotificationHistory = ToastNotificationManager.get_history()
+        toastHistory: ToastNotificationHistory = ToastNotificationManager.history
         toastHistory.clear(self._AUMID)
 
     def clear_scheduled_toasts(self) -> None:
         """
         Clear all scheduled toasts set for the toaster
         """
         scheduledToasts = self.toastNotifier.get_scheduled_toast_notifications()
```

### Comparing `windows-toasts-0.4.0/src/windows_toasts/wrappers.py` & `Windows-Toasts-0.4.1/src/windows_toasts/wrappers.py`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/tests/test_aumid.py` & `Windows-Toasts-0.4.1/tests/test_aumid.py`

 * *Files identical despite different names*

### Comparing `windows-toasts-0.4.0/tests/test_toasts.py` & `Windows-Toasts-0.4.1/tests/test_toasts.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
     InteractableWindowsToaster("Python").show_toast(newToast)
 
 
 def test_custom_duration_toast():
     from src.windows_toasts import ToastDuration, ToastText1
 
-    newToast = ToastText1(duration=ToastDuration.Short)
+    newToast = ToastText1(duration=ToastDuration.Short, body="A short toast")
     WindowsToaster("Python").show_toast(newToast)
 
 
 def test_attribution_text_toast():
     from src.windows_toasts import ToastImageAndText3
 
     newToast = ToastImageAndText3()
@@ -240,18 +240,25 @@
     from src.windows_toasts import ToastProgressBar, ToastText1
 
     progressBar = ToastProgressBar(
         "Preparing...", "Python 4 release", progress=None, progress_override="? millenniums remaining"
     )
     newToast = ToastText1(progress_bar=progressBar)
 
-    InteractableWindowsToaster("Python", "{1AC14E77-02E7-4E5D-B744-2EB1AE5198B7}\\cmd.exe").show_toast(newToast)
+    toaster = InteractableWindowsToaster("Python", "{1AC14E77-02E7-4E5D-B744-2EB1AE5198B7}\\cmd.exe")
+    toaster.show_toast(newToast)
+
+    # Branching
+    newToast.progress_bar.progress = 0.75
+    newToast.progress_bar.progress_override = None
+
+    toaster.show_toast(newToast)
 
 
-def test_scheduled_toast():
+def test_scheduled_toast(pytestconfig):
     from datetime import datetime, timedelta
 
     from src.windows_toasts import ToastProgressBar, ToastText1
 
     progressBar = ToastProgressBar(
         "Preparing...", "Python 4 release", progress=0.5, progress_override="? millenniums remaining"
     )
@@ -259,20 +266,22 @@
 
     # Branching
     clonedToast = newToast.clone()
     clonedToast.progress_bar.progress_override = None
     clonedToast.progress_bar.caption = None
 
     toaster = InteractableWindowsToaster("Python")
-    toaster.schedule_toast(newToast, datetime.now() + timedelta(seconds=10))
-    toaster.schedule_toast(clonedToast, datetime.now() + timedelta(seconds=20))
-    # We would assert here but due to mocking we can't, so just assert that the toast couldn't be found
-    with warns(UserWarning, match="Toast unscheduling failed."):
-        toaster.unschedule_toast(newToast)
-        toaster.unschedule_toast(clonedToast)
+    toaster.schedule_toast(newToast, datetime.now() + timedelta(seconds=5))
+    toaster.schedule_toast(clonedToast, datetime.now() + timedelta(seconds=10))
+
+    if pytestconfig.getoption("real_run"):
+        assert toaster.unschedule_toast(clonedToast)
+    else:
+        with warns(UserWarning, match="Toast unscheduling failed."):
+            toaster.unschedule_toast(clonedToast)
 
 
 def test_clear_toasts():
     InteractableWindowsToaster("Python").clear_scheduled_toasts()
     InteractableWindowsToaster("Python").clear_toasts()
```

### Comparing `windows-toasts-0.4.0/windows_toasts.egg-info/PKG-INFO` & `Windows-Toasts-0.4.1/Windows_Toasts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
-Name: windows-toasts
-Version: 0.4.0
-Summary: Windows toast notifications sender
+Name: Windows-Toasts
+Version: 0.4.1
+Summary: Python library used to send toast notifications on Windows machines
 Home-page: https://github.com/DatGuy1/Windows-Toasts
 Author: DatGuy
 Author-email: datguysteam@gmail.com
 License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/DatGuy1/Windows-Toasts/issues
 Project-URL: Documentation, https://windows-toasts.readthedocs.io
+Project-URL: Source, https://github.com/DatGuy1/Windows-Toasts
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `windows-toasts-0.4.0/windows_toasts.egg-info/SOURCES.txt` & `Windows-Toasts-0.4.1/Windows_Toasts.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+Windows_Toasts.egg-info/PKG-INFO
+Windows_Toasts.egg-info/SOURCES.txt
+Windows_Toasts.egg-info/dependency_links.txt
+Windows_Toasts.egg-info/entry_points.txt
+Windows_Toasts.egg-info/not-zip-safe
+Windows_Toasts.egg-info/requires.txt
+Windows_Toasts.egg-info/top_level.txt
 scripts/__init__.py
 scripts/register_hkey_aumid.py
 src/windows_toasts/__init__.py
 src/windows_toasts/_version.py
 src/windows_toasts/events.py
 src/windows_toasts/py.typed
 src/windows_toasts/toast_audio.py
 src/windows_toasts/toast_document.py
 src/windows_toasts/toast_types.py
 src/windows_toasts/toasters.py
 src/windows_toasts/wrappers.py
 tests/test_aumid.py
-tests/test_toasts.py
-windows_toasts.egg-info/PKG-INFO
-windows_toasts.egg-info/SOURCES.txt
-windows_toasts.egg-info/dependency_links.txt
-windows_toasts.egg-info/entry_points.txt
-windows_toasts.egg-info/not-zip-safe
-windows_toasts.egg-info/requires.txt
-windows_toasts.egg-info/top_level.txt
+tests/test_toasts.py
```

