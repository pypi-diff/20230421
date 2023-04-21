# Comparing `tmp/qlapi-0.1.3.tar.gz` & `tmp/qlapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlapi-0.1.3.tar", last modified: Fri Apr 21 09:08:31 2023, max compression
+gzip compressed data, was "qlapi-0.1.4.tar", last modified: Fri Apr 21 10:08:19 2023, max compression
```

## Comparing `qlapi-0.1.3.tar` & `qlapi-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:31.089922 qlapi-0.1.3/
--rw-rw-rw-   0        0        0    35821 2023-04-21 08:17:29.000000 qlapi-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      116 2023-04-21 09:08:31.089303 qlapi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2677 2023-04-21 08:54:39.000000 qlapi-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:31.069874 qlapi-0.1.3/qlapi/
--rw-rw-rw-   0        0        0       77 2023-04-20 03:56:00.000000 qlapi-0.1.3/qlapi/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-04-21 06:55:06.000000 qlapi-0.1.3/qlapi/base.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:31.085834 qlapi-0.1.3/qlapi/lib/
--rw-rw-rw-   0        0        0  1704960 2023-04-10 07:48:28.000000 qlapi-0.1.3/qlapi/lib/QLNRSdk.dll
--rw-rw-rw-   0        0        0     2385 2023-04-20 05:53:02.000000 qlapi-0.1.3/qlapi/nrsdk.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:31.087828 qlapi-0.1.3/qlapi/recorder/
--rw-rw-rw-   0        0        0    18304 2023-04-21 07:15:46.000000 qlapi-0.1.3/qlapi/recorder/__init__.py
--rw-rw-rw-   0        0        0      200 2023-04-21 07:12:04.000000 qlapi-0.1.3/qlapi/rsa.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:31.087828 qlapi-0.1.3/qlapi/stimulator/
--rw-rw-rw-   0        0        0     3366 2023-04-20 05:45:14.000000 qlapi-0.1.3/qlapi/stimulator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 09:08:31.084836 qlapi-0.1.3/qlapi.egg-info/
--rw-rw-rw-   0        0        0      116 2023-04-21 09:08:30.000000 qlapi-0.1.3/qlapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-04-21 09:08:31.000000 qlapi-0.1.3/qlapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 09:08:30.000000 qlapi-0.1.3/qlapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 09:08:30.000000 qlapi-0.1.3/qlapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-04-21 09:08:30.000000 qlapi-0.1.3/qlapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 09:08:31.089922 qlapi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      389 2023-04-21 09:04:48.000000 qlapi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:08:19.254365 qlapi-0.1.4/
+-rw-rw-rw-   0        0        0    35821 2023-04-21 08:17:29.000000 qlapi-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      182 2023-04-21 10:08:19.253367 qlapi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2677 2023-04-21 08:54:39.000000 qlapi-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 10:08:19.235414 qlapi-0.1.4/qlapi/
+-rw-rw-rw-   0        0        0       77 2023-04-20 03:56:00.000000 qlapi-0.1.4/qlapi/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-04-21 06:55:06.000000 qlapi-0.1.4/qlapi/base.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:08:19.249377 qlapi-0.1.4/qlapi/lib/
+-rw-rw-rw-   0        0        0  1704960 2023-04-10 07:48:28.000000 qlapi-0.1.4/qlapi/lib/QLNRSdk.dll
+-rw-rw-rw-   0        0        0     2385 2023-04-20 05:53:02.000000 qlapi-0.1.4/qlapi/nrsdk.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:08:19.251371 qlapi-0.1.4/qlapi/recorder/
+-rw-rw-rw-   0        0        0    18502 2023-04-21 09:52:38.000000 qlapi-0.1.4/qlapi/recorder/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-04-21 07:12:04.000000 qlapi-0.1.4/qlapi/rsa.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:08:19.252368 qlapi-0.1.4/qlapi/stimulator/
+-rw-rw-rw-   0        0        0     3366 2023-04-20 05:45:14.000000 qlapi-0.1.4/qlapi/stimulator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 10:08:19.249377 qlapi-0.1.4/qlapi.egg-info/
+-rw-rw-rw-   0        0        0      182 2023-04-21 10:08:19.000000 qlapi-0.1.4/qlapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-21 10:08:19.000000 qlapi-0.1.4/qlapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 10:08:19.000000 qlapi-0.1.4/qlapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 09:08:30.000000 qlapi-0.1.4/qlapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-21 10:08:19.000000 qlapi-0.1.4/qlapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 10:08:19.254365 qlapi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      533 2023-04-21 10:08:12.000000 qlapi-0.1.4/setup.py
```

### Comparing `qlapi-0.1.3/LICENSE.txt` & `qlapi-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.3/README.md` & `qlapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.3/qlapi/base.py` & `qlapi-0.1.4/qlapi/base.py`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.3/qlapi/lib/QLNRSdk.dll` & `qlapi-0.1.4/qlapi/lib/QLNRSdk.dll`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.3/qlapi/nrsdk.py` & `qlapi-0.1.4/qlapi/nrsdk.py`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.3/qlapi/recorder/__init__.py` & `qlapi-0.1.4/qlapi/recorder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,57 +33,61 @@
 
         # 导默认保存到eeg文件相同目录
         print("eeg path is {}".format(eeg_path))
         if edf_path:
             print("edf path is {}".format(edf_path))
 
         eeg_files = get_file_list(eeg_path, "eeg")
+        if len(eeg_files) == 0:
+            print("No found eeg file in path {}".format(eeg_path))
+            return
+            
         last_eeg_file = eeg_files[-1] 
         if start_time or end_time:
             eeg_files = _eeg_file_filter(eeg_files, start_time, end_time)
         print('eeg file list: {}'.format(eeg_files))
         for eeg_file in eeg_files:
             # 最后一个文件覆盖已转换的edf文件
             if (eeg_file == last_eeg_file):                
                 eeg_to_edf(eeg_file, edf_path, force=True)
             else:
                 eeg_to_edf(eeg_file, edf_path, force=force)
 
     def _open(self, path=None):
         # 初始化示例变量
-        self._path = path
+        self._eeg_path = self._edf_path = path
         self._raw_list = []
         self._start_time = None
         self._end_time = None
 
         # 手动选择文件夹
-        if not self._path:
+        if not self._eeg_path:
             root = tk.Tk()
             root.withdraw()
-            self._path = tk.filedialog.askdirectory()
+            self._eeg_path = self._edf_path = tk.filedialog.askdirectory()
 
         return self
 
     def _preload(self, start_time, end_time, extension='edf'):
             
         # 先导出为edf
-        self.export_edf(self._path, start_time, end_time)
+        self.export_edf(self._eeg_path, start_time, end_time)
 
         # 读取edf/bdf文件
-        self.file_list = get_file_list(self._path, extension)
+        self.file_list = get_file_list(self._eeg_path, extension)
 
         # 读取文件信息
         self._read_header()
 
         return self
 
     # 读取文件头信息
     def _read_header(self):
         if not self.file_list:
-            raise Exception('File not found in path {}'.format(self.path))
+            raise Exception('File not found in path {}'.format(self._edf_path))
 
         print(self.file_list)
         for file in self.file_list:
             raw = mne.io.read_raw_edf(file, preload=False, verbose=False)
 
             # 当前文件记录开始时间和结束时间
             raw.start_time = raw.annotations.orig_time
@@ -94,15 +98,15 @@
 
             if self._end_time is None or self._end_time < raw.end_time:
                 self._end_time = raw.end_time
 
             self._raw_list.append(raw)
 
         if not self._raw_list:
-            raise Exception('No data in in path {}'.format(self._path))
+            raise Exception('No data in in path {}'.format(self._edf_path))
 
         if self._start_time is None or self._end_time is None:
             raise Exception('Record time parse error.')
 
         print("Records from {} to {}, but may not be continuous.".format(
             self._start_time, self._end_time))
```

### Comparing `qlapi-0.1.3/qlapi/stimulator/__init__.py` & `qlapi-0.1.4/qlapi/stimulator/__init__.py`

 * *Files identical despite different names*

