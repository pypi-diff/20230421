# Comparing `tmp/plex-nfs-watchdog-0.0.1.tar.gz` & `tmp/plex-nfs-watchdog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plex-nfs-watchdog-0.0.1.tar", last modified: Fri Apr 21 10:48:55 2023, max compression
+gzip compressed data, was "plex-nfs-watchdog-0.0.2.tar", last modified: Fri Apr 21 11:33:29 2023, max compression
```

## Comparing `plex-nfs-watchdog-0.0.1.tar` & `plex-nfs-watchdog-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-21 10:48:55.937604 plex-nfs-watchdog-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-21 10:48:55.937604 plex-nfs-watchdog-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/config/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/plex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/plex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/plex/plex_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/watchdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-21 10:48:40.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/plex_nfs_watchdog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:48:55.933604 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-21 10:48:55.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-21 10:48:55.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:48:55.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 10:48:55.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 10:48:55.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 10:48:55.000000 plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.498438 plex-nfs-watchdog-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-21 11:33:29.498438 plex-nfs-watchdog-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-21 11:33:29.498438 plex-nfs-watchdog-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.494438 plex-nfs-watchdog-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.494438 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.494438 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.494438 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/config/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.494438 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/plex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/plex/plex_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.498438 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/watchdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/watchdog/plex_watchdog_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-04-21 11:33:15.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/plex_nfs_watchdog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 11:33:29.494438 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-04-21 11:33:29.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-21 11:33:29.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 11:33:29.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 11:33:29.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 11:33:29.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 11:33:29.000000 plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/top_level.txt
```

### Comparing `plex-nfs-watchdog-0.0.1/LICENSE` & `plex-nfs-watchdog-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.1/PKG-INFO` & `plex-nfs-watchdog-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.1
+Version: 0.0.2
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.1 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.2 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.1/README.md` & `plex-nfs-watchdog-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.1/setup.cfg` & `plex-nfs-watchdog-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/modules/plex/plex_agent.py` & `plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/modules/plex/plex_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,66 @@
 
 class PlexAgent:
     __plex_config: dict[str, str] = {}
     __server: PlexServer = None
     __save_cache: bool = False
     __internal_paths: dict[str, tuple[str, str]] = {}
     __notify_queue: set[tuple[str, str]] = set()
+    __supported_ext: list[str] = [
+        "3g2",
+        "3gp",
+        "amv",
+        "asf",
+        "ass",
+        "avi",
+        "drc",
+        "f4a",
+        "f4b",
+        "f4p",
+        "f4v",
+        "flac",
+        "flv",
+        "gif",
+        "gifv",
+        "idx",
+        "m2ts",
+        "m2v",
+        "m4p",
+        "m4v",
+        "m4v",
+        "mkv",
+        "mng",
+        "mov",
+        "mp2",
+        "mp3",
+        "mp4",
+        "mpe",
+        "mpeg",
+        "mpg",
+        "mpv",
+        "mxf",
+        "nsv",
+        "ogg",
+        "ogv",
+        "qt",
+        "rm",
+        "rmvb",
+        "roq",
+        "smi",
+        "srt",
+        "ssa",
+        "sub",
+        "svi",
+        "ts",
+        "vob",
+        "vtt",
+        "wmv",
+        "yuv",
+        "webm"
+    ]
 
     def is_cache_loaded(self) -> bool:
         """
         Checks if the Plex configuration is set
         :return bool: True if the Plex configuration is set, False otherwise
         """
         return self.__plex_config != {}
@@ -168,15 +220,18 @@
         Parses the given event and adds it to the queue
         :param event: The event to parse
         :return:
         """
         event_path = Path(event.src_path)
         if event_path.name in self.__internal_paths.keys():
             return
-        logging.info(f"Analyzing {event_path}")
+        if not event_path.is_dir():
+            extension: str = event_path.suffix.replace(".", "")
+            if extension not in self.__supported_ext:
+                return
         section_child: Path | None = self.__find_section_child_of(event_path)
         if section_child is None:
             logging.error(f"Could not find Plex section for {event_path}")
             return
         section_scan = (section_child.parent.name, section_child.name)
         if section_scan not in self.__notify_queue:
             logging.info(f"Adding to queue ({event.event_type}): {section_child.name}")
```

### Comparing `plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog/plex_nfs_watchdog.py` & `plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog/plex_nfs_watchdog.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from watchdog.observers import Observer
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "."))
 from modules.watchdog.plex_watchdog_event import PlexWatchdog
 from modules.config import shared
 from modules.plex.plex_agent import plex_agent_singleton
 
-colorlog.basicConfig(format='{log_color}{levelname}:\t{message}', level=logging.DEBUG, style='{', stream=None,
+colorlog.basicConfig(format='{log_color}{levelname}:\t{message}', level=logging.INFO, style='{', stream=None,
                      log_colors={
                          'DEBUG': 'cyan', 'INFO': 'white', 'WARNING': 'yellow', 'ERROR': 'red', 'CRITICAL': 'red'
                      })
 logging.getLogger("urllib3").setLevel(logging.WARNING)
+logging.getLogger("watchdog").setLevel(logging.WARNING)
 
 
 def get_args_from_cli() -> None:
     """
     Parses the command line arguments and stores them in the shared config
     :return:
     """
@@ -71,23 +72,27 @@
                 continue
             logging.info(f"Registering watcher for {full_path}")
             observer.schedule(event_handler, full_path, recursive=True)
             observers.append(observer)
         if not observers:
             logging.error("No valid paths given, exiting...")
             exit(-1)
-        observer.start()
-        stop_plex_watchdog_service: () = plex_agent_singleton.start_service()
+        stop_plex_watchdog_service: () = None
         try:
+            observer.start()
+            stop_plex_watchdog_service: () = plex_agent_singleton.start_service()
             while True:
-                time.sleep(1)
+                time.sleep(2)
         except KeyboardInterrupt:
             logging.warning("Detected SIGNTERM, stopping PlexNFSWatchdog...")
             for observer in observers:
                 observer.unschedule_all()
                 observer.stop()
                 observer.join()
-            stop_plex_watchdog_service()
+            if stop_plex_watchdog_service is not None:
+                stop_plex_watchdog_service()
+        except OSError as os_err:
+            logging.error(f"OS error: {os_err}")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/PKG-INFO` & `plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plex-nfs-watchdog
-Version: 0.0.1
+Version: 0.0.2
 Summary: A utility to trigger Plex partial-scans on NFS configurations, on which inotify is not supported
 Home-page: https://github.com/LightDestory/PlexNFSWatchdog
 Author: LightDestory
 Author-email: apb231@gmail.com
 Project-URL: Bug Tracker, https://github.com/LightDestory/PlexNFSWatchdog/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.1 Summary: A utility
+Metadata-Version: 2.1 Name: plex-nfs-watchdog Version: 0.0.2 Summary: A utility
 to trigger Plex partial-scans on NFS configurations, on which inotify is not
 supported Home-page: https://github.com/LightDestory/PlexNFSWatchdog Author:
 LightDestory Author-email: apb231@gmail.com Project-URL: Bug Tracker, https://
 github.com/LightDestory/PlexNFSWatchdog/issues Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier: License
 :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
```

### Comparing `plex-nfs-watchdog-0.0.1/src/plex_nfs_watchdog.egg-info/SOURCES.txt` & `plex-nfs-watchdog-0.0.2/src/plex_nfs_watchdog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

