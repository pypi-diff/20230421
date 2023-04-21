# Comparing `tmp/markit-tcpbroker-1.7.tar.gz` & `tmp/markit-tcpbroker-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rfimu-interface/rfimu-interface/dist/.tmp-xllx074t/markit-tcpbroker-1.7.tar", last modified: Fri Feb 10 14:19:41 2023, max compression
+gzip compressed data, was "/home/runner/work/rfimu-interface/rfimu-interface/dist/.tmp-wm8tsmlv/markit-tcpbroker-1.8.2.tar", last modified: Thu Apr 20 16:39:42 2023, max compression
```

## Comparing `markit-tcpbroker-1.7.tar` & `markit-tcpbroker-1.8.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/markit_tcpbroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/markit_tcpbroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/markit_tcpbroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/markit_tcpbroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/markit_tcpbroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/markit_tcpbroker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/tcpbroker/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/tcpbroker/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/cmd/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/cmd/easy_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/cmd/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/tcpbroker/common/
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/common/IMUParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/common/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/common/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/common/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/tcpbroker/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/functional/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/functional/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/functional/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/tcpbroker/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/scripts/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/tcpbroker/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/tasks/imu_render_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/tasks/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/tasks/tcp_listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/tasks/tcp_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tcpbroker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:19:41.000000 markit-tcpbroker-1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tests/test_fit_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tests/test_measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-10 14:19:31.000000 markit-tcpbroker-1.7/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/tcpbroker/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/tcpbroker/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/cmd/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/cmd/easy_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/cmd/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/tcpbroker/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/common/IMUParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/common/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/common/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/common/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/tcpbroker/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/functional/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/functional/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/functional/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/functional/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/tcpbroker/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/scripts/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/tcpbroker/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/tasks/imu_render_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/tasks/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/tasks/tcp_listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/tasks/tcp_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tcpbroker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:39:42.000000 markit-tcpbroker-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tests/test_fit_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tests/test_measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-20 16:39:23.000000 markit-tcpbroker-1.8.2/tests/test_streamlit.py
```

### Comparing `markit-tcpbroker-1.7/PKG-INFO` & `markit-tcpbroker-1.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markit-tcpbroker
-Version: 1.7
+Version: 1.8.2
 Summary: IMU message broker
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # IMU Interface
@@ -23,9 +23,7 @@
 ```shell
 python -m pip install markit-tcpbroker
 ```
 
 ## Documentation
 
 For documentation, please refer to [rfimu-interface/docs](https://github.com/mvig-robotflow/rfimu-interface/docs).
-
-
```

### Comparing `markit-tcpbroker-1.7/markit_tcpbroker.egg-info/PKG-INFO` & `markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markit-tcpbroker
-Version: 1.7
+Version: 1.8.2
 Summary: IMU message broker
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # IMU Interface
@@ -23,9 +23,7 @@
 ```shell
 python -m pip install markit-tcpbroker
 ```
 
 ## Documentation
 
 For documentation, please refer to [rfimu-interface/docs](https://github.com/mvig-robotflow/rfimu-interface/docs).
-
-
```

### Comparing `markit-tcpbroker-1.7/markit_tcpbroker.egg-info/SOURCES.txt` & `markit-tcpbroker-1.8.2/markit_tcpbroker.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 tcpbroker/cmd/portal.py
 tcpbroker/common/IMUParser.py
 tcpbroker/common/__init__.py
 tcpbroker/common/render.py
 tcpbroker/common/repo.py
 tcpbroker/common/tcp.py
 tcpbroker/functional/__init__.py
+tcpbroker/functional/align.py
 tcpbroker/functional/convert.py
 tcpbroker/functional/ellipse.py
 tcpbroker/functional/vector.py
 tcpbroker/scripts/__init__.py
 tcpbroker/scripts/cli.py
 tcpbroker/scripts/configure.py
 tcpbroker/tasks/__init__.py
```

### Comparing `markit-tcpbroker-1.7/setup.py` & `markit-tcpbroker-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 requires = open("requirements.txt", "r").readlines() if os.path.exists("requirements.txt") else open("./markit_tcpbroker.egg-info/requires.txt", "r").readlines()
 print("#-------------------    ", str(os.listdir("./")))
 setup(
     name="markit-tcpbroker",
-    version="1.7",
+    version="1.8.2",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="IMU message broker",
     packages=[
         "tcpbroker",
         "tcpbroker.cmd",
         "tcpbroker.common",
```

### Comparing `markit-tcpbroker-1.7/tcpbroker/__main__.py` & `markit-tcpbroker-1.8.2/tcpbroker/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 import sys
 
-from .scripts import cli, configure
+from tcpbroker.scripts import cli, configure
 
 if __name__ == '__main__':
     if len(sys.argv) > 1 and sys.argv[1] == 'configure':
         parser = argparse.ArgumentParser()
         parser.add_argument("--input", "-i", type=str, default=None, help="path to input config file")
         parser.add_argument("--output", "-o", type=str, default="imu_config.yaml", help="path to output config file")
         args = parser.parse_args(sys.argv[2:])
```

### Comparing `markit-tcpbroker-1.7/tcpbroker/cmd/control.py` & `markit-tcpbroker-1.8.2/tcpbroker/cmd/control.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/cmd/easy_setup.py` & `markit-tcpbroker-1.8.2/tcpbroker/cmd/easy_setup.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/cmd/portal.py` & `markit-tcpbroker-1.8.2/tcpbroker/cmd/portal.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
     # Start threads
     threading.Thread(target=update_imu_state_thread, daemon=True).start()
     threading.Thread(target=update_client_info_thread, daemon=True).start()
 
     try:
         # app.run(host='0.0.0.0', port=api_port)
-        uvicorn.run(app=app, port=cfg.api_port)
+        uvicorn.run(app=app, port=cfg.api_port, host='0.0.0.0')
     except KeyboardInterrupt:
         LOGGER.info(f"portal() got KeyboardInterrupt")
         return
 
 
 if __name__ == '__main__':
     portal(BrokerConfig('./imu_config.yaml'))
```

### Comparing `markit-tcpbroker-1.7/tcpbroker/common/IMUParser.py` & `markit-tcpbroker-1.8.2/tcpbroker/common/IMUParser.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 
 
 class IMUParser:
     ADDR = 0xe5
     BLOCK_SZ: int = 0x1000
     ch_imu_data_t_fmt = "I3f3f3f3f4ffI"
-    hi229_dgram_meta_t_fmt = "=qi12s"
+    hi229_dgram_meta_t_fmt = "=qqIi12s"
 
     def __init__(self) -> None:
         self.buf: np.ndarray = np.zeros(shape=(100), dtype=np.uint8)
         self.cursor: int = 0
         self.start_reg: int = 0
         self.length: int = 0
         self.data_valid: bool = False
@@ -23,14 +23,20 @@
         self.cursor = 0
         self.start_reg = 0
         self.length = 0
         self.data_valid = False
         self.meta_valid = False
         self.buf.fill(0)
 
+    @staticmethod
+    def verify_packet(buf, chksum: int) -> bool:
+        arr = np.frombuffer(buf, dtype=np.uint8)
+        arr_chksum = np.bitwise_xor.reduce(arr)
+        return arr_chksum == chksum
+
     def _sync(self, read_buf: bytes):
         """
         Magic Sync Algorithm.
         See imu-esp-node (C code)
         Args:
             read_buf:
 
@@ -43,15 +49,15 @@
             return res
 
         for idx in range(len(read_buf)):
             if read_buf[idx] == self.ADDR:
                 _start_idx = idx
                 _end_idx = _start_idx + 1 + struct.calcsize(self.ch_imu_data_t_fmt) + struct.calcsize(
                     self.hi229_dgram_meta_t_fmt)
-                data_valid = sum(read_buf[_start_idx: _end_idx]) % 0x100 == read_buf[_end_idx]
+                data_valid = self.verify_packet(read_buf[_start_idx: _end_idx], read_buf[_end_idx])
                 if data_valid:
                     return {
                         "sync_start_idx": _start_idx,
                         "dgram_length": _end_idx - _start_idx + 1,
                         "imu_offset": 1,
                         "imu_length": struct.calcsize(self.ch_imu_data_t_fmt),
                         "imu_fmt": self.ch_imu_data_t_fmt,
@@ -67,32 +73,40 @@
         return None
 
     def _parse(self, read_buf, fmt) -> List[Dict]:
         result: List[Dict] = []
         start_idx = fmt['sync_start_idx']
         try:
             while start_idx + fmt['dgram_length'] < len(read_buf):
-                imu_data = struct.unpack(self.ch_imu_data_t_fmt, read_buf[start_idx + fmt['imu_offset']:start_idx + fmt[
-                    'imu_offset'] + fmt['imu_length']])
-                meta_data = struct.unpack(self.hi229_dgram_meta_t_fmt, read_buf[
-                                                                       start_idx + fmt['meta_offset']:start_idx + fmt[
-                                                                           'meta_offset'] + fmt['meta_length']])
-
-                imu_dict: dict = {"accel_x": imu_data[1], "accel_y": imu_data[2], "accel_z": imu_data[3],
-                                  "gyro_x": imu_data[4], "gyro_y": imu_data[5], "gyro_z": imu_data[6],
-                                  "roll": imu_data[10], "pitch": imu_data[11], "yaw": imu_data[12],
-                                  "quat_w": imu_data[13], "quat_x": imu_data[14], "quat_y": imu_data[15], "quat_z": imu_data[16],
-                                  "temp": 0.0,
-                                  "mag_x": imu_data[7], "mag_y": imu_data[8], "mag_z": imu_data[9],
-                                  "sys_ticks": imu_data[18]}
-
-                meta_dict = {'timestamp': meta_data[0],
-                             'uart_buffer_len': meta_data[1],
-                             'id': ''.join([chr(meta_data[2][idx]) for idx in range(len(meta_data[2]))]),
-                             }
+                imu_data = struct.unpack(
+                    self.ch_imu_data_t_fmt,
+                    read_buf[start_idx + fmt['imu_offset']:start_idx + fmt['imu_offset'] + fmt['imu_length']]
+                )
+                meta_data = struct.unpack(
+                    self.hi229_dgram_meta_t_fmt,
+                    read_buf[start_idx + fmt['meta_offset']:start_idx + fmt['meta_offset'] + fmt['meta_length']]
+                )
+
+                imu_dict: dict = {
+                    "accel_x": imu_data[1], "accel_y": imu_data[2], "accel_z": imu_data[3],
+                    "gyro_x": imu_data[4], "gyro_y": imu_data[5], "gyro_z": imu_data[6],
+                    "roll": imu_data[10], "pitch": imu_data[11], "yaw": imu_data[12],
+                    "quat_w": imu_data[13], "quat_x": imu_data[14], "quat_y": imu_data[15], "quat_z": imu_data[16],
+                    "temp": 0.0,
+                    "mag_x": imu_data[7], "mag_y": imu_data[8], "mag_z": imu_data[9],
+                    "sys_ticks": imu_data[18]
+                }
+
+                meta_dict = {
+                    'timestamp': meta_data[0],
+                    'tsf_timestamp': meta_data[1],
+                    'seq': meta_data[2],
+                    'uart_buffer_len': meta_data[3],
+                    'id': ''.join([chr(meta_data[4][idx]) for idx in range(len(meta_data[4]))]),
+                }
 
                 result.append({**imu_dict, **meta_dict})
 
                 start_idx += fmt['dgram_length']
         except Exception as e:
             print(e)
             pass
```

### Comparing `markit-tcpbroker-1.7/tcpbroker/common/render.py` & `markit-tcpbroker-1.8.2/tcpbroker/common/render.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 import multiprocessing as mp
 import struct
 import time
 from io import BytesIO
 from typing import Dict, List, Tuple, Optional, BinaryIO, Union
+import numpy as np
 
 
 class IMURender:
     ch_imu_data_t_fmt = "I3f3f3f3f4ffI"
     imu_packet_length = struct.calcsize(ch_imu_data_t_fmt)
-    dgram_meta_t_fmt = "=qi12s"
+    dgram_meta_t_fmt = "=qqIi12s"
     meta_packet_length = struct.calcsize(dgram_meta_t_fmt)
     imu_addr: bytes = b'\xe5'
     addr_length = 1
     packet_length = addr_length + \
-        struct.calcsize(ch_imu_data_t_fmt) + struct.calcsize(dgram_meta_t_fmt)
+                    struct.calcsize(ch_imu_data_t_fmt) + struct.calcsize(dgram_meta_t_fmt)
 
     buffer: BytesIO = BytesIO()
 
     filename: Optional[str] = None
     file_handle: Optional[BinaryIO] = None
     out_queue: Optional[mp.Queue] = None
     update_interval_s: Optional[float] = None
@@ -35,63 +36,78 @@
         if self.filename is not None:
             self.file_handle = open(self.filename, "ab")
 
         self.out_queue = out_queue
         self.update_interval_s = update_interval_s
         self.last_update_time = time.time()
 
+    @staticmethod
+    def verify_packet(buf, chksum: int) -> bool:
+        arr = np.frombuffer(buf, dtype=np.uint8)
+        arr_chksum = np.bitwise_xor.reduce(arr)
+        return arr_chksum == chksum
+
     def _parse_packet(self, pkt: bytes) -> Dict[str, Union[float, str, int]]:
         imu_struct = struct.unpack(self.ch_imu_data_t_fmt,
                                    pkt[self.addr_length:self.addr_length + self.imu_packet_length])
         meta_struct = struct.unpack(
             self.dgram_meta_t_fmt, pkt[self.addr_length + self.imu_packet_length:])
 
-        imu_dict: dict = {"accel_x": imu_struct[1], "accel_y": imu_struct[2], "accel_z": imu_struct[3],
-                          "gyro_x": imu_struct[4], "gyro_y": imu_struct[5], "gyro_z": imu_struct[6],
-                          "roll": imu_struct[10], "pitch": imu_struct[11], "yaw": imu_struct[12],
-                          "quat_w": imu_struct[13], "quat_x": imu_struct[14], "quat_y": imu_struct[15],
-                          "quat_z": imu_struct[16],
-                          "temp": 0.0,
-                          "mag_x": imu_struct[7], "mag_y": imu_struct[8], "mag_z": imu_struct[9],
-                          "sys_ticks": imu_struct[18]}
-
-        meta_dict = {'timestamp': meta_struct[0],
-                     'uart_buffer_len': meta_struct[1],
-                     'id': ''.join([chr(meta_struct[2][idx]) for idx in range(len(meta_struct[2]))]),
-                     }
+        imu_dict: dict = {
+            "accel_x": imu_struct[1], "accel_y": imu_struct[2], "accel_z": imu_struct[3],
+            "gyro_x": imu_struct[4], "gyro_y": imu_struct[5], "gyro_z": imu_struct[6],
+            "roll": imu_struct[10], "pitch": imu_struct[11], "yaw": imu_struct[12],
+            "quat_w": imu_struct[13], "quat_x": imu_struct[14], "quat_y": imu_struct[15],
+            "quat_z": imu_struct[16],
+            "temp": 0.0,
+            "mag_x": imu_struct[7], "mag_y": imu_struct[8], "mag_z": imu_struct[9],
+            "sys_ticks": imu_struct[18]
+        }
+
+        meta_dict = {
+            'timestamp': meta_struct[0],
+            'tsf_timestamp': meta_struct[1],
+            'seq': meta_struct[2],
+            'uart_buffer_len': meta_struct[3],
+            'id': ''.join([chr(meta_struct[4][idx]) for idx in range(len(meta_struct[4]))]),
+        }
         return {**imu_dict, **meta_dict}
 
     def _try_sync(self, data: bytes) -> Tuple[bool, List[Dict[str, Union[float, str, int]]]]:
-        try:
-            self.buffer.write(data)
-            self.buffer.seek(0)
-
-            while (addr := self.buffer.read(1)) != self.imu_addr:
-                if addr == b'':
-                    return False, []
-            self.buffer.seek(self.buffer.tell() - 1)
-
-            data_valid = sum(self.buffer.read(self.packet_length)
-                             ) % 0x100 == sum(self.buffer.read(1))
-            if data_valid:
-                self.buffer.seek(self.buffer.tell() - self.packet_length - 1)
-                res = []
-                while True:
-                    pkt = self.buffer.read(self.packet_length)
-                    checksum = self.buffer.read(1)
-                    if len(pkt) < self.packet_length or checksum == b'':
-                        self.buffer = BytesIO(pkt)
-                        self.buffer.read()  # move pointer to end using read
-                        break
-                    res.append(self._parse_packet(pkt))
-                return True, res
-            else:
+
+        self.buffer.write(data)
+        self.buffer.seek(0)
+
+        while (addr := self.buffer.read(1)) != self.imu_addr:
+            if addr == b'':
                 return False, []
-        except ValueError as _:
-            logging.warning("value error encountered in IMURender")
+        self.buffer.seek(self.buffer.tell() - 1)
+
+        _content = self.buffer.read(self.packet_length)
+        _chksum = self.buffer.read(1)
+        if len(_content) < self.packet_length or len(_chksum) < 1:
+            self.buffer.write(_content)
+            self.buffer.write(_chksum)
+            return False, []
+
+        data_valid = self.verify_packet(_content, int(_chksum[0]))
+
+        if data_valid:
+            self.buffer.seek(self.buffer.tell() - self.packet_length - 1)
+            res = []
+            while True:
+                pkt = self.buffer.read(self.packet_length)
+                checksum = self.buffer.read(1)
+                if len(pkt) < self.packet_length or checksum == b'':
+                    self.buffer = BytesIO(pkt)
+                    self.buffer.read()  # move pointer to end using read
+                    break
+                res.append(self._parse_packet(pkt))
+            return True, res
+        else:
             return False, []
 
     def update(self, data: bytes):
         # If not synced, try to sync
         success, res = self._try_sync(data)
         if success:
             self.state_is_valid = True
```

### Comparing `markit-tcpbroker-1.7/tcpbroker/common/repo.py` & `markit-tcpbroker-1.8.2/tcpbroker/common/repo.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/common/tcp.py` & `markit-tcpbroker-1.8.2/tcpbroker/common/tcp.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/config.py` & `markit-tcpbroker-1.8.2/tcpbroker/config.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/functional/convert.py` & `markit-tcpbroker-1.8.2/tcpbroker/functional/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 import os
 from typing import Dict, List
 
 import numpy as np
 import tqdm
 
 from tcpbroker.common import IMUParser
-from .vector import vectorize_to_np
-
+from tcpbroker.functional.vector import vectorize_to_np
+from tcpbroker.functional.align import align_measurement
 
 def convert_measurement(measurement_basedir: str, delete_dat: bool = False) -> Dict[str, Dict[str, np.ndarray]]:
     _logger = logging.getLogger('convert_measurement')
 
     MEASUREMENT_KEYS: List[str] = [
-        'id', 'timestamp', 'accel_x', 'accel_y', 'accel_z', 'gyro_x', 'gyro_y', 'gyro_z', 'mag_x', 'mag_y', 'mag_z', 'quat_w', 'quat_x', 'quat_y', 'quat_z', 'pitch', 'roll', 'yaw', "uart_buffer_len"
+        'id', 'timestamp',
+        'accel_x', 'accel_y', 'accel_z',
+        'gyro_x', 'gyro_y', 'gyro_z',
+        'mag_x', 'mag_y', 'mag_z',
+        'quat_w', 'quat_x', 'quat_y', 'quat_z',
+        'pitch', 'roll', 'yaw',
+        'uart_buffer_len', 'tsf_timestamp','seq'
     ]
 
     filenames_list: List[str] = glob.glob(os.path.join(measurement_basedir, '*.dat'))
     all_measurement: Dict[str, list] = {}
     all_measurement_np: Dict[str, Dict[str, np.ndarray]] = {}
     imu_parser = IMUParser()
 
@@ -46,24 +52,25 @@
     # Dump numpy array
     for imu_id in all_measurement_np.keys():
         np.savez(os.path.join(measurement_basedir, f'imu_{imu_id}.npz'), **all_measurement_np[imu_id])
     """example
     >>> import numpy as np
     >>> npfile = np.load('./imu_mem_2021-10-21_211859/imu_84f7033b3e78.npz')
     >>> npfile.files
-    ['id', 'timestamp', 'accel_x', 'accel_y', 'accel_z', 'gyro_x',  'gyro_y', 'gyro_z', 'pitch', 'roll', 'yaw']
+    ['id', 'timestamp', 'accel_x', 'accel_y', 'accel_z', 'gyro_x', 'gyro_y', 'gyro_z', 'mag_x', 'mag_y', 'mag_z', 'quat_w', 'quat_x', 'quat_y', 'quat_z', 'pitch', 'roll', 'yaw', 'uart_buffer_len', 'tsf_timestamp', 'seq']
     >>> npfile['timestamp']
     array([[1.63482358e+15],
           [1.63482358e+15],
           [1.63482358e+15],
           ...,
           [1.63482235e+15],
           [1.63482235e+15],
           [1.63482235e+15]])
     """
 
-    return all_measurement_np
+    interp_res = align_measurement(measurement_basedir)
+    return interp_res
 
 
 if __name__ == '__main__':
-    res = convert_measurement(r"C:\Users\liyutong\Desktop\rfimu-interface\imu_data\imu_mem_2022-10-27_193652")
+    res = convert_measurement(r"C:\Users\robotflow\Desktop\rfimu-interface\imu_data\imu_mem_2023-04-18_202012")
     print(res)
```

### Comparing `markit-tcpbroker-1.7/tcpbroker/functional/ellipse.py` & `markit-tcpbroker-1.8.2/tcpbroker/functional/ellipse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 import dataclasses
 from math import sqrt
 
 import numpy as np
 from scipy.optimize import root
-
+from typing import Tuple, Optional, List
 
 @dataclasses.dataclass()
-class EllipseFitResult:
-    pos: np.ndarray = np.array([np.inf, np.inf, np.inf])
-    length: np.ndarray = np.array([np.inf, np.inf, np.inf])
-    ret: bool = False
-
-    @property
-    def score(self) -> float:
-        """Get the score of ellipse fitting
-
-        Returns:
-            float: Score of fitting
-        """
-        if not self.ret:
-            return np.inf
-        else:
-            return np.sum(self.pos ** 2) + np.std(self.length)
+class EllipseFitter:
 
-    def fit(self, points: np.ndarray):
+    @staticmethod
+    def fit(points: np.ndarray) -> Tuple[bool, Optional[List[float]],  Optional[List[float]], Optional[float]]:
         """Fit an ellipse to points
         Args:
             points (np.ndarray): Points to fit
 
         Returns:
-            EllipseFitResult: Result of fitting
+            EllipseFitter: Result of fitting
 
         """
 
         x: np.ndarray = points[:, 0]
         y: np.ndarray = points[:, 1]
         z: np.ndarray = points[:, 2]
 
@@ -71,15 +57,15 @@
             # X-axis length
             A = sqrt(x0 * x0 + result[0] * y0 * y0 + result[1] * z0 * z0 - result[5])
             # Y-axis length
             B = A / sqrt(result[0])
             # Z-axis length
             C = A / sqrt(result[1])
 
-            self.ret = True
-            self.pos = np.array([x0, y0, z0])
-            self.length = np.array([A, B, C])
+            ret = True
+            pos = [x0, y0, z0]
+            length = [A, B, C]
+            score = np.sum(np.array(pos) ** 2) + np.std(length)
+            return ret, pos, length, score
 
         except ValueError as _:
-            self.ret = False
-            self.pos = np.array([np.inf, np.inf, np.inf])
-            self.length = np.array([np.inf, np.inf, np.inf])
+            return False, None, None, None
```

### Comparing `markit-tcpbroker-1.7/tcpbroker/functional/vector.py` & `markit-tcpbroker-1.8.2/tcpbroker/functional/vector.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/scripts/cli.py` & `markit-tcpbroker-1.8.2/tcpbroker/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/scripts/configure.py` & `markit-tcpbroker-1.8.2/tcpbroker/scripts/configure.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/tasks/imu_render_ui.py` & `markit-tcpbroker-1.8.2/tcpbroker/tasks/imu_render_ui.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/tasks/measure.py` & `markit-tcpbroker-1.8.2/tcpbroker/tasks/measure.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/tasks/tcp_listen.py` & `markit-tcpbroker-1.8.2/tcpbroker/tasks/tcp_listen.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/tasks/tcp_process.py` & `markit-tcpbroker-1.8.2/tcpbroker/tasks/tcp_process.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tcpbroker/utils.py` & `markit-tcpbroker-1.8.2/tcpbroker/utils.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tests/test_measure.py` & `markit-tcpbroker-1.8.2/tests/test_measure.py`

 * *Files identical despite different names*

### Comparing `markit-tcpbroker-1.7/tests/test_streamlit.py` & `markit-tcpbroker-1.8.2/tests/test_streamlit.py`

 * *Files identical despite different names*

