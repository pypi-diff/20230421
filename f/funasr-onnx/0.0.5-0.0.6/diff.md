# Comparing `tmp/funasr_onnx-0.0.5.tar.gz` & `tmp/funasr_onnx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funasr_onnx-0.0.5.tar", last modified: Fri Apr 14 15:16:44 2023, max compression
+gzip compressed data, was "dist/funasr_onnx-0.0.6.tar", last modified: Fri Apr 21 11:17:57 2023, max compression
```

## Comparing `funasr_onnx-0.0.5.tar` & `funasr_onnx-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2784 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2175 2023-04-14 15:16:16.000000 funasr_onnx-0.0.5/README.md
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr_onnx-0.0.5/funasr_onnx/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/paraformer_bin.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr_onnx-0.0.5/funasr_onnx/punc_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx/utils/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr_onnx-0.0.5/funasr_onnx/utils/__init__.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/utils/e2e_vad.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)    15845 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/utils/frontend.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr_onnx-0.0.5/funasr_onnx/utils/postprocess_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr_onnx-0.0.5/funasr_onnx/utils/timestamp_utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr_onnx-0.0.5/funasr_onnx/utils/utils.py
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr_onnx-0.0.5/funasr_onnx/vad_bin.py
-drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     2784 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/PKG-INFO
--rw-rw-r--   0 gzf       (1006) gzf       (1007)      485 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/SOURCES.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/dependency_links.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       90 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/requires.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       12 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/funasr_onnx.egg-info/top_level.txt
--rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-14 15:16:44.000000 funasr_onnx-0.0.5/setup.cfg
--rw-rw-r--   0 gzf       (1006) gzf       (1007)     1384 2023-04-14 15:16:16.000000 funasr_onnx-0.0.5/setup.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6094 2023-04-21 03:10:43.000000 funasr_onnx-0.0.6/README.md
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      218 2023-04-14 03:21:54.000000 funasr_onnx-0.0.6/funasr_onnx/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7786 2023-04-14 02:00:09.000000 funasr_onnx-0.0.6/funasr_onnx/paraformer_bin.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    12135 2023-04-14 03:21:54.000000 funasr_onnx-0.0.6/funasr_onnx/punc_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx/utils/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        0 2023-03-29 02:53:52.000000 funasr_onnx-0.0.6/funasr_onnx/utils/__init__.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    28927 2023-04-14 02:00:09.000000 funasr_onnx-0.0.6/funasr_onnx/utils/e2e_vad.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)    15848 2023-04-21 11:13:25.000000 funasr_onnx-0.0.6/funasr_onnx/utils/frontend.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     7566 2023-03-29 02:53:52.000000 funasr_onnx-0.0.6/funasr_onnx/utils/postprocess_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     2762 2023-03-29 02:53:52.000000 funasr_onnx-0.0.6/funasr_onnx/utils/timestamp_utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9176 2023-04-14 02:00:09.000000 funasr_onnx-0.0.6/funasr_onnx/utils/utils.py
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     9707 2023-04-14 03:21:54.000000 funasr_onnx-0.0.6/funasr_onnx/vad_bin.py
+drwxrwxr-x   0 gzf       (1006) gzf       (1007)        0 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     6714 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/PKG-INFO
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)      485 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)        1 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       90 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/requires.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       12 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/funasr_onnx.egg-info/top_level.txt
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)       38 2023-04-21 11:17:57.000000 funasr_onnx-0.0.6/setup.cfg
+-rw-rw-r--   0 gzf       (1006) gzf       (1007)     1393 2023-04-21 11:13:25.000000 funasr_onnx-0.0.6/setup.py
```

### Comparing `funasr_onnx-0.0.5/funasr_onnx/paraformer_bin.py` & `funasr_onnx-0.0.6/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.5/funasr_onnx/punc_bin.py` & `funasr_onnx-0.0.6/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.5/funasr_onnx/utils/e2e_vad.py` & `funasr_onnx-0.0.6/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.5/funasr_onnx/utils/frontend.py` & `funasr_onnx-0.0.6/funasr_onnx/utils/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         batch_size = input.shape[0]
         if self.input_cache is None:
             self.input_cache = np.empty((batch_size, 0), dtype=np.float32)
         input = np.concatenate((self.input_cache, input), axis=1)
         frame_num = self.compute_frame_num(input.shape[-1], self.frame_sample_length, self.frame_shift_sample_length)
         # update self.in_cache
         self.input_cache = input[:, -(input.shape[-1] - frame_num * self.frame_shift_sample_length):]
-        waveforms = np.empty(0, dtype=np.int16)
+        waveforms = np.empty(0, dtype=np.float32)
         feats_pad = np.empty(0, dtype=np.float32)
         feats_lens = np.empty(0, dtype=np.int32)
         if frame_num:
             waveforms = []
             feats = []
             feats_lens = []
             for i in range(batch_size):
@@ -233,15 +233,15 @@
                 self.fbank_fn.accept_waveform(self.opts.frame_opts.samp_freq, waveform.tolist())
                 frames = self.fbank_fn.num_frames_ready
                 mat = np.empty([frames, self.opts.mel_opts.num_bins])
                 for i in range(frames):
                     mat[i, :] = self.fbank_fn.get_frame(i)
                 feat = mat.astype(np.float32)
                 feat_len = np.array(mat.shape[0]).astype(np.int32)
-                feats.append(mat)
+                feats.append(feat)
                 feats_lens.append(feat_len)
 
             waveforms = np.stack(waveforms)
             feats_lens = np.array(feats_lens)
             feats_pad = np.array(feats)
         self.fbanks = feats_pad
         self.fbanks_lens = copy.deepcopy(feats_lens)
```

### Comparing `funasr_onnx-0.0.5/funasr_onnx/utils/postprocess_utils.py` & `funasr_onnx-0.0.6/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.5/funasr_onnx/utils/timestamp_utils.py` & `funasr_onnx-0.0.6/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.5/funasr_onnx/utils/utils.py` & `funasr_onnx-0.0.6/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.5/funasr_onnx/vad_bin.py` & `funasr_onnx-0.0.6/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr_onnx-0.0.5/setup.py` & `funasr_onnx-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.0.5'
+VERSION_NUM = '0.0.6'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
-    author="Speech Lab, Alibaba Group, China",
+    author="Speech Lab of DAMO Academy, Alibaba Group",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     license='MIT',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=["librosa", "onnxruntime>=1.7.0",
```

