# Comparing `tmp/markit-realsense-recorder-1.6.tar.gz` & `tmp/markit-realsense-recorder-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rfimu-realsense-recorder/rfimu-realsense-recorder/dist/.tmp-om_t7nal/markit-realsense-recorder-1.6.tar", last modified: Fri Jan 27 14:12:26 2023, max compression
+gzip compressed data, was "/home/runner/work/rfimu-realsense-recorder/rfimu-realsense-recorder/dist/.tmp-db3gdqrw/markit-realsense-recorder-1.8.0.tar", last modified: Fri Apr 21 12:40:42 2023, max compression
```

## Comparing `markit-realsense-recorder-1.6.tar` & `markit-realsense-recorder-1.8.0.tar`

### file list

```diff
@@ -1,33 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/markit_realsense_recorder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/markit_realsense_recorder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/markit_realsense_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/markit_realsense_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/markit_realsense_recorder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/markit_realsense_recorder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/realsense_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/realsense_recorder/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/cmd/local_capture_static_interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/cmd/local_record_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/cmd/remote_record_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/realsense_recorder/common/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/common/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/common/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/realsense_recorder/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/io/BagReader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/io/DirectoryReader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/io/Sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/realsense_recorder/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/realsense_recorder/scripts/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-27 14:12:26.000000 markit-realsense-recorder-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-27 14:12:16.000000 markit-realsense-recorder-1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/markit_realsense_recorder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/markit_realsense_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/markit_realsense_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/markit_realsense_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/markit_realsense_recorder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/markit_realsense_recorder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/realsense_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/realsense_recorder/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/cmd/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/cmd/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16157 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/cmd/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/realsense_recorder/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17026 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/common/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/common/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/realsense_recorder/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/filters/fiducial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/realsense_recorder/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/io/Compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/io/DirectoryReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/io/Sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/io/Sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/realsense_recorder/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/realsense_recorder/scripts/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:40:42.000000 markit-realsense-recorder-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_advance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_local_capture_static_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_local_record_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_record_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-21 12:40:31.000000 markit-realsense-recorder-1.8.0/tests/test_reprojection.py
```

### Comparing `markit-realsense-recorder-1.6/README.md` & `markit-realsense-recorder-1.8.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -82,9 +82,22 @@
 ```shell
 python -m realsense_recorder configure
 ```
 
 To launch a remote record station that supports REST API
 
 ```shell
-python -m realsense_recorder run --app=remote_record_seq
+python -m realsense_recorder serve
 ```
+
+To launch a remote record station that is calibrated 
+```shell
+python -m realsense_recorder serve --calibration=path/to/calibration
+```
+
+> Note: The calibration.json file is expected to be in the `path/to/calibration` directory. The calibration file can be generated by running `python -m realsense_recorder calibrate`
+
+To run calibration
+
+```shell
+python -m realsense_recorder calibrate
+```
```

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/cmd/local_record_seq.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/cmd/calibrate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,182 +1,220 @@
 import argparse
 import json
 import os.path as osp
 import time
-from concurrent.futures import ThreadPoolExecutor
 from typing import List, Dict, Callable
+import glob
+import logging
+import os
+import shutil
+import subprocess
 
 import cv2
-cv2.setNumThreads(0)
+from rich.progress import track
 import numpy as np
-import tqdm
+
 from realsense_recorder.common import (
     RealsenseCameraCfg,
     RealsenseSystemCfg,
     RealsenseSystemModel,
     new_realsense_camera_system_from_yaml_file,
     CALLBACKS,
     get_datetime_tag
 )
 
+from typing import Optional, Dict, Tuple
+
+CONFIG_DOCKER_IMAGE = "davidliyutong/multical-docker"
+CONFIG_BOARD_YAML = """
+common:
+  _type_: 'charuco'
+  size: [10, 10]
+  aruco_dict: '5X5_1000'
+  square_length: 0.040
+  marker_length: 0.032
+  min_rows: 3
+  min_points: 9
+boards:
+  charuco_10x10_0:
+    aruco_offset: 0
+  charuco_10x10_1:
+    aruco_offset: 50
+  charuco_10x10_2:
+    aruco_offset: 100
+  charuco_10x10_3:
+    aruco_offset: 150
+  charuco_10x10_4:
+    aruco_offset: 200
+aruco_params:
+  adaptiveThreshWinSizeMax: 200
+  adaptiveThreshWinSizeStep: 50
+"""
+
+def run_multical_with_docker(tagged_path: str) -> Tuple[Optional[Dict], Optional[Exception]]:
+    _logger = logging.getLogger('run_multical_with_docker')
+    _logger.debug(f"run multical with image {CONFIG_DOCKER_IMAGE}")
+
+    if not osp.exists(tagged_path):
+        return None, FileNotFoundError(f"file {tagged_path} does not exist")
+
+    cameras_name_list = list(
+        filter(lambda x: os.path.isdir(osp.join(tagged_path, x)),
+               os.listdir(tagged_path)
+               )
+    )  # ["rxx", "ryy", "rzz"]
+
+    if len(cameras_name_list) <= 0:
+        return None, FileNotFoundError(f"no camera found in {tagged_path}")
+
+    _logger.debug(f"found {len(cameras_name_list)} cameras")
+    for camera_name in cameras_name_list:
+        frame_filenames = glob.glob(osp.join(tagged_path, camera_name, "color", "*"))
+        if len(frame_filenames) <= 0:
+            _logger.warning(f"no frame found in {camera_name}/color, assuming they are copied to upper directory")
+            continue
+        for frame_name in frame_filenames:
+            shutil.copy(frame_name, osp.join(tagged_path, camera_name))
+
+    _logger.debug(f"write board.yaml")
+    with open(osp.join(tagged_path, "boards.yaml"), "w") as f:
+        f.write(CONFIG_BOARD_YAML)
+
+    _logger.debug("Add docker volume")
+    with open(osp.join(tagged_path, "multical.sh"), 'w') as f:
+        f.write(f"multical calibrate --cameras {' '.join(cameras_name_list)}")
+
+    _logger.debug("launch multical")
+    p = subprocess.Popen(f"docker run --rm -v {osp.abspath(tagged_path)}:/input {CONFIG_DOCKER_IMAGE}", shell=True)
+    try:
+        p.wait(timeout=60)  # should have finished in 30 seconds
+    except subprocess.TimeoutExpired as _:
+        pass
+
+    if osp.exists(osp.join(tagged_path, "calibration.json")):
+        with open(osp.join(tagged_path, "calibration.json"), 'r') as f:
+            try:
+                res = json.load(f)
+                return res, None
+            except Exception as err:
+                return None, err
+    else:
+        return None, FileNotFoundError(f"calibration.json not found in {tagged_path}")
+
+
 
-class LocalRecordSeq(RealsenseSystemModel):
+class LocalCaptureStaticInteractive(RealsenseSystemModel):
     def __init__(self,
                  system_cfg: RealsenseSystemCfg,
                  camera_cfgs: List[RealsenseCameraCfg],
                  callbacks: Dict[str, Callable] = None):
-        super().__init__(system_cfg, camera_cfgs, callbacks)
-        self.metadata: Dict[Dict] = {cam.friendly_name: [] for cam in self.cameras}
-
-    def insert_meta_data(self, idx, ts, sys_ts, frame_counter):
-        self.metadata[idx].append({
-            "ts": ts,
-            "sys_ts": sys_ts,
-            "frame_counter": frame_counter
-        })
-
-    def save_meta_data(self):
-        meta_save_path = osp.join(self.options.base_dir, "metadata_all.json")
-        config_save_path = osp.join(self.options.base_dir, "realsense_config.json")
-        bundle = {
-            "camera_sn": [cam.option.sn for cam in self.cameras],
-            "metadata": self.metadata
-        }
-        with open(meta_save_path, 'w') as f:
-            json.dump(bundle, f, indent=4)
-
-        with open(config_save_path, 'w') as f:
-            json.dump({"realsense": {"system": self.options.get_dict(), "cameras": list(map(lambda x: x.get_dict(), self.camera_options))}}, f, indent=4)
+        system_cfg.frame_queue_size = 0  # disable frame queue
+        # lower the frame rate to 5/6 fps
+        for camera_idx in range(len(camera_cfgs)):
+            for color_idx in range(len(camera_cfgs[camera_idx].color)):
+                camera_cfgs[camera_idx].color[color_idx].fps = camera_cfgs[camera_idx].__COLOR_FPS_CANDIDATES__[0]
+                camera_cfgs[camera_idx].color[color_idx].exposure = -1
+        system_cfg.interval_ms = 500
 
+        super().__init__(system_cfg, camera_cfgs, callbacks)
 
     def app(self):
+        _resolution = (640, 480)
 
         def create_windows():
             for cam in self.cameras:
                 cv2.namedWindow(cam.window_name, cv2.WINDOW_AUTOSIZE)
 
-        def save_color_frame(path, frame):
-            cv2.imwrite(path, frame)
-
-        def save_depth_frame(path, frame):
-            np.save(path, frame)
-
         self.console.log(f"tag is {self.tag}")
         self.console.log(f"save path is {self.options.base_dir}")
         self.console.log(f"number of cameras is {len(self.cameras)}")
         self._set_advanced_mode()
         self.console.log("opening devices")
         self.open()
-        if self.options.interactive:
-            self.console.log("creating windows")
-            create_windows()
+        self.console.log("creating windows")
+        create_windows()
         self.console.log("starting devices")
         self.start(interval_ms=self.options.interval_ms)
 
         self.console.log("saving intrinsics")
         for cam in self.cameras:
             '''Convert intrinsic data to dict (readable in Open3D)'''
             mat = [cam.intrinsics.fx, 0, 0, 0, cam.intrinsics.fy, 0, cam.intrinsics.ppx, cam.intrinsics.ppy, 1]
             intrinsics_dict = {'width': cam.intrinsics.width, 'height': cam.intrinsics.height, 'intrinsic_matrix': mat}
             save_path = osp.join(cam.save_path, 'realsense_intrinsic.json')
             if not osp.lexists(save_path):
                 with open(save_path, 'w') as f:
                     json.dump(intrinsics_dict, f, sort_keys=False,
                               indent=4,
                               ensure_ascii=False)
-        self.console.log("[]start recording")
-        progress_bars = [tqdm.tqdm(ncols=0) for _ in range(len(self.cameras))]
-        save_workers = ThreadPoolExecutor(max_workers=len(self.cameras) * 2)
+        self.console.log("start recording")
+        for _ in track(range(50), description="waiting for streams to stabilize"):
+            time.sleep(0.1)
 
+        n_frames = 0
         try:
             while True:
+                string_input = self.console.input(f"Press Enter to capture the {n_frames} frame or type 'q' to quit: ")
+                if string_input == 'q':
+                    break
+
                 for idx, cam in enumerate(self.cameras):
-                    tic = time.time()
-                    color_image, depth_image, ts, sys_ts, frame_counter = cam.get_frames()
-                    self.insert_meta_data(cam.friendly_name, ts, sys_ts, frame_counter)
-                    toc = time.time()
 
-                    if color_image is not None:
-                        save_workers.submit(save_color_frame, osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image)
-                        # i5 12400K save jpg at 17 fps (load 60%), write to PM9A1 at 200 - 500MB/s, memory consumption 1GB/min percamera
-                        # i5 12400K save bmp at 20 fps, but write at 1.0GB/s, memory consumption 0GB/min per camera
+                    self.console.print(f"capturing from camera {idx}")
+                    color_image, depth_image, _, sys_ts, frame_counter = cam.get_frames()
 
-                        # save_workers.submit(cv2.imwrite, (osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image,))
-                        # cv2.imwrite(osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image)
+                    if color_image is not None:
+                        cv2.imwrite(osp.join(cam.color_save_path, f'{n_frames}.jpg'), color_image)
 
                     if depth_image is not None:
-                        save_workers.submit(save_depth_frame, osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.npy'), depth_image)
-                        # save_workers.submit(lambda: cv2.imwrite(osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.png'), depth_image, [cv2.IMWRITE_PNG_COMPRESSION, 0]))
-
-                        # np.save(osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.npy'), depth_image)
-                        # cv2.imwrite(osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.png'), depth_image, [cv2.IMWRITE_PNG_COMPRESSION, 0])
+                        np.save(osp.join(cam.depth_save_path, f'{n_frames}.npy'), depth_image)
 
-                    progress_bars[idx].set_description(f'SN={cam.option.sn}, ProcessTime={int((toc - tic) * 1000)}(ms), FrameCounter={frame_counter}')
-                    progress_bars[idx].update(1)
+                    if color_image is not None:
+                        mix = cv2.resize(color_image, _resolution)
+                    cv2.imshow(cam.window_name, mix)
+                    cv2.waitKey(1)
 
-                    if self.options.interactive and not self.options.use_bag:
-                        if color_image is not None and depth_image is not None:
-                            mix = cv2.addWeighted(color_image[...,0:3], 0.5, cv2.resize(depth_image, (color_image.shape[1], color_image.shape[0])), 0.5, 0)
-                        elif color_image is not None and depth_image is None:
-                            mix = color_image
-                        elif color_image is None and depth_image is not None:
-                            mix = depth_image
-                        else:
-                            break
-                        cv2.imshow(cam.window_name, mix)
-                        cv2.waitKey(1)
+                n_frames += 1
 
         except KeyboardInterrupt as e:
             # raise(e)
             self.console.log("\n" * len(self.cameras))
             self.console.log("stopped in response to KeyboardInterrupt")
-
-            self.console.log("stopping cameras")
-            self.stop(interval_ms=self.options.interval_ms)
-            for idx, cam in enumerate(self.cameras):
-                self.console.log(f"saving last frames of camera {cam.option.sn}")
-                while True:
-                    color_image, depth_image, ts, sys_ts, frame_counter = cam.get_frames(timeout_ms=50)
-                    self.insert_meta_data(cam.friendly_name, ts, sys_ts, frame_counter)
-                    if frame_counter > 0:
-                        if color_image is not None:
-                            save_workers.submit(save_color_frame, osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image)
-
-                        if depth_image is not None:
-                            save_workers.submit(save_depth_frame, osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.npy'), depth_image)
-
-                        progress_bars[idx].set_description(f'SN={cam.option.sn}, FrameCounter={frame_counter}')
-                        progress_bars[idx].update(1)
-                    else:
-                        break
-            self.close()
-            save_workers.shutdown(wait=True)
-            self.save_meta_data()
-            cv2.destroyAllWindows()
             return
 
         except Exception as e:
+            self.console.log("\n" * len(self.cameras))
             self.console.log(e)
             raise e
 
+        finally:
+            self.console.log("stopping cameras")
+            self.stop(interval_ms=self.options.interval_ms)
+            self.close()
+            cv2.destroyAllWindows()
+
+            run_multical_with_docker(self.options.base_dir)
 
 def main(args):
     callbacks = {
-        CALLBACKS.tag_cb: (lambda: get_datetime_tag()) if args.tag is None else (lambda: args.tag),
+        CALLBACKS.tag_cb: (lambda: 'cali_' + get_datetime_tag()) if args.tag is None else (lambda: args.tag),
         CALLBACKS.save_path_cb: lambda cam_cfg, sys_cfg: osp.join(sys_cfg.base_dir, "r" + cam_cfg.sn[-2:]),
         CALLBACKS.camera_friendly_name_cb: lambda cam_cfg, _: "r" + cam_cfg.sn[-2:]
     }
 
-    sys = new_realsense_camera_system_from_yaml_file(LocalRecordSeq, args.config, callbacks)
+    sys = new_realsense_camera_system_from_yaml_file(LocalCaptureStaticInteractive, args.config, callbacks)
 
     sys.app()
 
+
 def entry_point(argv):
     parser = argparse.ArgumentParser()
     parser.add_argument('--config', type=str, default='./realsense_config.yaml')
     parser.add_argument('--tag', type=str, default=None)
     args = parser.parse_args(argv)
     main(args)
 
+
 if __name__ == '__main__':
     import sys
-    entry_point(sys.argv)
+
+    entry_point(sys.argv[1:])
```

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/cmd/remote_record_seq.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/cmd/serve.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 import argparse
 import json
 import logging
 import multiprocessing as mp
 import os
 import os.path as osp
+import shutil
 import signal
 import time
 from concurrent.futures import ThreadPoolExecutor
 from typing import Callable, Dict, List, Optional
+import threading
 
 import cv2
 import numpy as np
 import tqdm
 import uvicorn
 from fastapi import FastAPI
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import JSONResponse, RedirectResponse
+import pyrealsense2 as rs
 
 from realsense_recorder.common import (
     CALLBACKS,
     new_realsense_camera_system_from_yaml_file,
     RealsenseSystemModel,
     RealsenseSystemCfg,
     RealsenseCameraCfg,
-    get_datetime_tag
+    get_datetime_tag,
+    enumerate_devices_that_supports_advanced_mode,
 )
+
+from .post_processing import worker as post_processing_worker
+
 app = FastAPI()
 logging.basicConfig(level=logging.INFO)
 
 STOP_EV: mp.Event = mp.Event()
 FINISH_EV: mp.Event = mp.Event()
 READY_EV: mp.Event = mp.Event()
 CAPTURE_PROCS: List[mp.Process] = []
+POST_PROCESSING_QUEUE: Optional[mp.Queue] = None
 ARGS: Optional[argparse.Namespace] = None
 
 
 class RemoteRecordSeq(RealsenseSystemModel):
     def __init__(self,
                  system_cfg: RealsenseSystemCfg,
                  camera_cfgs: List[RealsenseCameraCfg],
                  callbacks: Dict[str, Callable] = None):
         super().__init__(system_cfg, camera_cfgs, callbacks)
         self.metadata: Dict[Dict] = {cam.friendly_name: [] for cam in self.cameras}
 
-    def insert_meta_data(self, idx, ts, sys_ts, frame_counter):
+    def insert_meta_data(self, idx, ts, sys_ts, frame_counter, frame_basename):
         self.metadata[idx].append({
-            "ts": ts,
+            "dev_ts": ts,
             "sys_ts": sys_ts,
-            "frame_counter": frame_counter
+            "frame_counter": frame_counter,
+            "frame_basename": frame_basename
         })
 
     def save_meta_data(self):
         save_path = osp.join(self.options.base_dir, "metadata_all.json")
         config_save_path = osp.join(self.options.base_dir, "realsense_config.json")
         bundle = {
             "camera_sn": [cam.option.sn for cam in self.cameras],
@@ -100,27 +109,29 @@
             ready_ev.set()
 
         try:
             while True:
                 for idx, cam in enumerate(self.cameras):
                     tic = time.time()
                     color_image, depth_image, ts, sys_ts, frame_counter = cam.get_frames()
-                    self.insert_meta_data(cam.friendly_name, ts, sys_ts, frame_counter)
+                    frame_basename = '{:07d}_{}_{}'.format(frame_counter, ts["backend_t"], sys_ts)
+                    self.insert_meta_data(cam.friendly_name, ts, sys_ts, frame_counter, frame_basename)
+
                     toc = time.time()
 
                     if color_image is not None:
-                        save_workers.submit(save_color_frame, osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image)
+                        save_workers.submit(save_color_frame, osp.join(cam.color_save_path, frame_basename + '.bmp'), color_image)
                         # i5 12400K save jpg at 17 fps (load 60%), write to PM9A1 at 200 - 500MB/s, memory consumption 1GB/min percamera
                         # i5 12400K save bmp at 20 fps, but write at 1.0GB/s, memory consumption 0GB/min per camera
 
                         # save_workers.submit(cv2.imwrite, (osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image,))
                         # cv2.imwrite(osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image)
 
                     if depth_image is not None:
-                        save_workers.submit(save_depth_frame, osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.npy'), depth_image)
+                        save_workers.submit(save_depth_frame, osp.join(cam.depth_save_path, frame_basename + '.npy'), depth_image)
                         # save_workers.submit(lambda: cv2.imwrite(osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.png'), depth_image, [cv2.IMWRITE_PNG_COMPRESSION, 0]))
 
                         # np.save(osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.npy'), depth_image)
                         # cv2.imwrite(osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.png'), depth_image, [cv2.IMWRITE_PNG_COMPRESSION, 0])
 
                     progress_bars[idx].set_description(f'SN={cam.option.sn}, ProcessTime={int((toc - tic) * 1000)}(ms), FrameCounter={frame_counter}')
                     progress_bars[idx].update(1)
@@ -147,21 +158,22 @@
 
             self.console.log("stopping cameras")
             self.stop(interval_ms=self.options.interval_ms)
             for idx, cam in enumerate(self.cameras):
                 self.console.log(f"saving last frames of camera {cam.option.sn}")
                 while True:
                     color_image, depth_image, ts, sys_ts, frame_counter = cam.get_frames(timeout_ms=50)
-                    self.insert_meta_data(cam.friendly_name, ts, sys_ts, frame_counter)
                     if frame_counter > 0:
+                        self.insert_meta_data(cam.friendly_name, ts, sys_ts, frame_counter, frame_basename)
+                        frame_basename = '{:07d}_{}_{}'.format(frame_counter, ts["backend_t"], sys_ts)
                         if color_image is not None:
-                            save_workers.submit(save_color_frame, osp.join(cam.color_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.bmp'), color_image)
+                            save_workers.submit(save_color_frame, osp.join(cam.color_save_path, frame_basename + '.bmp'), color_image)
 
                         if depth_image is not None:
-                            save_workers.submit(save_depth_frame, osp.join(cam.depth_save_path, f'{cam.n_frames}_{ts}_{sys_ts}.npy'), depth_image)
+                            save_workers.submit(save_depth_frame, osp.join(cam.depth_save_path, frame_basename + '.npy'), depth_image)
 
                         progress_bars[idx].set_description(f'SN={cam.option.sn}, FrameCounter={frame_counter}')
                         progress_bars[idx].update(1)
                     else:
                         break
             self.close()
             save_workers.shutdown(wait=True)
@@ -186,24 +198,32 @@
     return resp
 
 
 def capture_frames(stop_ev: mp.Event,
                    finish_ev: mp.Event,
                    ready_ev: mp.Event,
                    config: str,
-                   tag: str):
+                   tag: str,
+                   post_processing_queue: mp.Queue = None):
     callbacks = {
         CALLBACKS.tag_cb: lambda: tag,
         CALLBACKS.save_path_cb: lambda cam_cfg, sys_cfg: osp.join(sys_cfg.base_dir, "r" + cam_cfg.sn[-2:]),
         CALLBACKS.camera_friendly_name_cb: lambda cam_cfg, _: "r" + cam_cfg.sn[-2:]
     }
 
     sys = new_realsense_camera_system_from_yaml_file(RemoteRecordSeq, config, callbacks)
 
-    sys.app(stop_ev, finish_ev, ready_ev)
+    try:
+        sys.app(stop_ev, finish_ev, ready_ev)
+    except AttributeError as e:
+        logging.error(f"capture_frames failed: {e}")
+
+    if post_processing_queue is not None:
+        logging.info(f"adding {sys.options.base_dir} to post processing queue")
+        post_processing_queue.put(sys.options.base_dir)
 
 
 @app.get("/")
 def root():
     return RedirectResponse(url='/docs')
 
 
@@ -222,15 +242,15 @@
             return make_response(status_code=200, ready=False)
     else:
         return make_response(status_code=500, msg="NOT SUPPORTED")
 
 
 @app.post("/v1/start")
 def start_process(tag: str = None):
-    global CAPTURE_PROCS, STOP_EV, FINISH_EV, READY_EV, ARGS
+    global CAPTURE_PROCS, STOP_EV, FINISH_EV, READY_EV, ARGS, POST_PROCESSING_QUEUE
 
     # Wait until last capture ends
     if len(CAPTURE_PROCS) > 0:
         if STOP_EV.is_set():
             FINISH_EV.wait(timeout=5)
             if FINISH_EV.is_set():
                 [proc.join(timeout=3) for proc in CAPTURE_PROCS]
@@ -255,15 +275,16 @@
 
         if len(CAPTURE_PROCS) <= 0:
             CAPTURE_PROCS = [mp.Process(target=capture_frames,
                                         args=(STOP_EV,
                                               FINISH_EV,
                                               READY_EV,
                                               ARGS.config,
-                                              tag))]
+                                              tag,
+                                              POST_PROCESSING_QUEUE))]
             DELAY_S = 2  # Magic delay duration to avoid U3V communication error
             [(proc.start(), time.sleep(DELAY_S
                                        )) for proc in CAPTURE_PROCS]
 
         return make_response(status_code=200, msg="START OK", subpath=tag)
 
 
@@ -275,14 +296,26 @@
     if len(CAPTURE_PROCS) > 0 and any([proc.is_alive() for proc in CAPTURE_PROCS]):
         STOP_EV.set()
         return make_response(status_code=200, msg=f"STOP OK: {len([None for proc in CAPTURE_PROCS if proc.is_alive()])} procs are running")
     else:
         return make_response(status_code=500, msg="NOT RUNNING")
 
 
+@app.post("/v1/reset")
+def reset_camera():
+    global CAPTURE_PROCS, STOP_EV
+    if len(CAPTURE_PROCS) > 0 and any([proc.is_alive() for proc in CAPTURE_PROCS]):
+        return make_response(status_code=500, msg="RUNNING")
+    else:
+        for dev in enumerate_devices_that_supports_advanced_mode(rs.context()):
+            dev.hardware_reset()
+        time.sleep(3)
+        return make_response(status_code=200, msg="RESET OK")
+
+
 @app.post("/v1/kill")
 def kill_process():
     global CAPTURE_PROCS, STOP_EV, FINISH_EV
     logging.info("[realsense] kill")
 
     if len(CAPTURE_PROCS) and any([proc.is_alive() for proc in CAPTURE_PROCS]) > 0:
         STOP_EV.set()
@@ -292,30 +325,68 @@
             logging.warning("[realsense] join timeout, force kill all processes")
             [os.kill(proc.pid, signal.SIGTERM) for proc in CAPTURE_PROCS if proc.is_alive()]
         return make_response(status_code=200, msg="KILL OK")
     else:
         return make_response(status_code=500, msg="NOT RUNNING")
 
 
+def post_processing_thread():
+    global POST_PROCESSING_QUEUE, ARGS
+    logging.info("post processing thread started")
+    while True:
+        if not POST_PROCESSING_QUEUE.empty():
+            base_dir = POST_PROCESSING_QUEUE.get()
+            if ARGS.calibration is not None:
+                try:
+                    _calibration_file_name = "calibration.json"
+                    shutil.copy(osp.join(ARGS.calibration, _calibration_file_name), base_dir)
+                    logging.info(f"copy calibration file from {osp.join(ARGS.calibration, _calibration_file_name)} to {base_dir}")
+                except Exception as e:
+                    logging.error(f"copy calibration file failed: {e}")
+                try:
+                    post_processing_worker(base_dir)
+                except Exception as e:
+                    logging.error(f"post processing failed: {e}")
+                # p = mp.Process(target=post_processing_worker, args=(sys.options.base_dir,))
+        else:
+            time.sleep(1)
+
+
 def main(args: argparse.Namespace):
-    global ARGS
+    global ARGS, POST_PROCESSING_QUEUE
+    POST_PROCESSING_QUEUE = mp.Queue()
     ARGS = args
     # Prepare system
     logging.info('the server listens at port {}'.format(args.port))
 
+    if not osp.exists(args.config):
+        logging.error(f"config file {args.config} does not exist")
+        exit(1)
+
+    if args.calibration is not None and not osp.exists(args.calibration):
+        logging.error(f"calibration file {args.calibration} does not exist")
+        exit(1)
+
     try:
+        t = threading.Thread(target=post_processing_thread)
+        t.start()
         uvicorn.run(app=app, port=args.port)
     except KeyboardInterrupt:
         logging.info(f"main() got KeyboardInterrupt")
-        exit(1)
+        os._exit(1)
+
 
 def entry_point(argv):
     parser = argparse.ArgumentParser(description='Recorder')
+    # parser.add_argument('--app', type=str, help='', default='')
     parser.add_argument('--config', type=str, help='The realsense system configuration', default='./realsense_config.yaml')
+    parser.add_argument('--calibration', type=str, help='The realsense system calibration', default=None)
     parser.add_argument('--port', type=int, help="Port to listen", default=5050)
     parser.add_argument('--debug', action='store_true', help='Toggle Debug mode')
     args = parser.parse_args(argv)
     main(args)
 
+
 if __name__ == '__main__':
     import sys
-    entry_point(sys.argv)
+
+    entry_point(sys.argv[1:])
```

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/common/__init__.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/common/__init__.py`

 * *Files identical despite different names*

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/common/config.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/common/config.py`

 * *Files identical despite different names*

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/common/interaction.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/common/interaction.py`

 * *Files identical despite different names*

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/common/record.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/common/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,29 +8,28 @@
 import numpy as np
 import pyrealsense2 as rs
 import rich
 import rich.progress_bar
 import yaml
 
 from .config import (
-    CALLBACKS, 
-    get_device_by_cfg, 
-    RealsenseSystemCfg, 
-    new_camera_config_by_product_id, 
+    CALLBACKS,
+    get_device_by_cfg,
+    RealsenseSystemCfg,
+    new_camera_config_by_product_id,
     RealsenseCameraCfg,
     new_system_config,
 )
 
 from .utils import (
     get_datetime_tag,
     enumerate_devices_that_supports_advanced_mode,
 )
 
 
-
 class RealsenseCameraModel:
     friendly_name: str = ""
     save_path: str = ""
     color_save_path: str = ""
     depth_save_path: str = ""
     bag_save_path: str = ""
     interactive: bool = False
@@ -158,47 +157,48 @@
 
     def stop(self, delay_ms: int = 0, clean: bool = False):
         time.sleep(delay_ms / 1e3)
         self.pipeline.stop()
         if clean:
             self.frame_queue = None
 
-    def _get_global_timestamp(self, frames):
+    @staticmethod
+    def get_timestamp(frames):
         # https://github.com/IntelRealSense/librealsense/issues/5612
-        backend_t = frames.get_frame_metadata(rs.frame_metadata_value.backend_timestamp)
+        t = {'global_t': None, 'backend_t': frames.get_frame_metadata(rs.frame_metadata_value.backend_timestamp) / 1000, 'sensor_t': None, 'frame_t': None}
+
         try:
-            senseor_t = frames.get_frame_metadata(rs.frame_metadata_value.sensor_timestamp)
-            frame_t = frames.get_frame_metadata(rs.frame_metadata_value.frame_timestamp)
-            global_t = backend_t - (frame_t - senseor_t)
+            t['sensor_t'] = frames.get_frame_metadata(rs.frame_metadata_value.sensor_timestamp) / 1000
+            t['frame_t'] = frames.get_frame_metadata(rs.frame_metadata_value.frame_timestamp) / 1000
+            t['global_t'] = t['backend_t'] - (t['frame_t'] - t['sensor_t'])
         except RuntimeError as e:
             # Fallback to backend_t
-            global_t = backend_t
-        return global_t
+            t['global_t'] = t['backend_t']
+        return t
 
-    def get_frames(self, timeout_ms=5000) -> Tuple[Optional[np.ndarray], Optional[np.ndarray], float, float, int]:
+    def get_frames(self, timeout_ms=5000) -> Tuple[Optional[np.ndarray], Optional[np.ndarray], Dict[str, float], float, int]:
         if self.use_bag:
             self.frame_queue.wait_for_frame()
-            ts = time.time()
-            return None, None, -1, ts, -1
+            return None, None, {}, time.time(), -1
         else:
             if self.frame_queue is not None:
                 ret, frames = self.frame_queue.try_wait_for_frame(timeout_ms=timeout_ms)
                 if not ret:
-                    return None, None, -1, time.time(), -1
+                    return None, None, {}, time.time(), -1
                 else:
                     frames = rs.composite_frame(frames)
             else:
                 ret, frames = self.pipeline.try_wait_for_frames(timeout_ms=timeout_ms)
                 if not ret:
-                    return None, None, -1, time.time(), -1
+                    return None, None, {}, time.time(), -1
                 else:
                     pass
 
             frame_counter = frames.get_frame_metadata(rs.frame_metadata_value.frame_counter)
-            ts = self._get_global_timestamp(frames)
+            ts = self.get_timestamp(frames)
             sys_ts = time.time()
 
             try:
                 aligned_frames = self.align.process(frames)
             except RuntimeError as e:
                 return None, None, ts, sys_ts, -1
             depth_frame = aligned_frames.get_depth_frame()
@@ -275,28 +275,32 @@
                 advnc_mode = rs.rs400_advanced_mode(dev)
                 advnc_mode.toggle_advanced_mode(True)
                 time.sleep(1)
 
     def open(self):
         for cam in self.cameras:
             cam.open()
+            time.sleep(0.05)
+        time.sleep(0.1)
 
     def close(self):
         for cam in self.cameras:
             cam.close()
 
-    def start(self, interval_ms: int = 0):
+    def start(self, interval_ms: int = 10):
         num_of_cameras = len(self.cameras)
         ret = []
-        with ThreadPoolExecutor(max_workers=num_of_cameras) as executor:
-            for idx, cam in enumerate(self.cameras):
-                ret.append(executor.submit(lambda: cam.start(delay_ms=interval_ms * (num_of_cameras - idx))))
-
-        list(map(lambda x: x.result(), ret))
-        time.sleep(0.1)
+        # with ThreadPoolExecutor(max_workers=num_of_cameras) as executor:
+        #     for idx, cam in enumerate(self.cameras):
+        #         ret.append(executor.submit(lambda: cam.start(delay_ms=interval_ms * (num_of_cameras - idx))))
+        #     executor.shutdown(wait=True)
+        # list(map(lambda x: x.result(), ret))
+        # time.sleep(0.1)
+        for idx, cam in enumerate(self.cameras):
+            cam.start()
 
     def stop(self, interval_ms: int = 0):
         num_of_cameras = len(self.cameras)
         ret = []
         with ThreadPoolExecutor(max_workers=num_of_cameras) as executor:
             for idx, cam in enumerate(self.cameras):
                 ret.append(executor.submit(lambda: cam.stop(interval_ms * (num_of_cameras - idx))))
```

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/io/DirectoryReader.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/io/DirectoryReader.py`

 * *Files identical despite different names*

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/io/Sequence.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/io/Sequence.py`

 * *Files identical despite different names*

### Comparing `markit-realsense-recorder-1.6/realsense_recorder/scripts/configure.py` & `markit-realsense-recorder-1.8.0/realsense_recorder/scripts/configure.py`

 * *Files identical despite different names*

### Comparing `markit-realsense-recorder-1.6/setup.py` & `markit-realsense-recorder-1.8.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,24 @@
 
 from setuptools import setup
 
 requires = open("./requirements.txt", "r").readlines() if os.path.exists("./requirements.txt") else open("./markit_realsense_recorder.egg-info/requires.txt", "r").readlines()
 
 setup(
     name="markit-realsense-recorder",
-    version="1.6",
+    version="1.8.0",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="Realsense remote recorder",
     packages=[
         "realsense_recorder",
         "realsense_recorder/cmd",
         "realsense_recorder/common",
+        "realsense_recorder/filters",
         "realsense_recorder/io",
         "realsense_recorder/scripts",
     ],
     python_requires=">=3.6",
     install_requires=requires,
-    entrypoints={
-        'console_scripts': [
-            'remote = remote.main:main'
-        ]
-    },
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown"
 )
```

