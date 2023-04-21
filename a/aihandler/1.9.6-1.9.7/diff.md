# Comparing `tmp/aihandler-1.9.6.tar.gz` & `tmp/aihandler-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihandler-1.9.6.tar", last modified: Mon Apr 17 23:51:45 2023, max compression
+gzip compressed data, was "aihandler-1.9.7.tar", last modified: Fri Apr 21 14:54:17 2023, max compression
```

## Comparing `aihandler-1.9.6.tar` & `aihandler-1.9.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:45.246710 aihandler-1.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-17 23:51:33.000000 aihandler-1.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-17 23:51:45.246710 aihandler-1.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-17 23:51:33.000000 aihandler-1.9.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:51:45.246710 aihandler-1.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-17 23:51:33.000000 aihandler-1.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:45.242710 aihandler-1.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:45.246710 aihandler-1.9.6/src/aihandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/controlnet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/llmrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/pyqt_offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/qtvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    53625 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/settings_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/socket_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-17 23:51:33.000000 aihandler-1.9.6/src/aihandler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:51:45.246710 aihandler-1.9.6/src/aihandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-17 23:51:45.000000 aihandler-1.9.6/src/aihandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 23:51:45.000000 aihandler-1.9.6/src/aihandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:51:45.000000 aihandler-1.9.6/src/aihandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-17 23:51:45.000000 aihandler-1.9.6/src/aihandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 23:51:45.000000 aihandler-1.9.6/src/aihandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.705761 aihandler-1.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 14:54:05.000000 aihandler-1.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-21 14:54:17.705761 aihandler-1.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-21 14:54:05.000000 aihandler-1.9.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 14:54:17.705761 aihandler-1.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-21 14:54:05.000000 aihandler-1.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.701761 aihandler-1.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.705761 aihandler-1.9.7/src/aihandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/controlnet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/llmrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/pyqt_offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/qtvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54315 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/socket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-21 14:54:05.000000 aihandler-1.9.7/src/aihandler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:54:17.705761 aihandler-1.9.7/src/aihandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 14:54:17.000000 aihandler-1.9.7/src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.9.6/LICENSE` & `aihandler-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/PKG-INFO` & `aihandler-1.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.6
+Version: 1.9.7
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.6/README.md` & `aihandler-1.9.7/README.md`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/setup.py` & `aihandler-1.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "xformers==0.0.18",
     "omegaconf==2.3.0",
     "accelerate==0.18.0",
     "controlnet_aux==0.0.1",
     "huggingface-hub==0.13.3",
     "numpy==1.23.5",
     "Pillow==9.4.0",
-    "pip==23.0.1",
+    "pip==23.1.0",
     "PyQt6==6.4.2",
     "PyQt6-Qt6==6.4.3",
     "PyQt6-sip==13.4.1",
     "pyqtdarktheme==2.1.0",
     "pyre-extensions==0.0.23",
     "lightning==2.0.0",
     "requests==2.28.2",
@@ -47,15 +47,15 @@
     "sympy==1.11.1",
     "regex",
 ]
 
 
 setup(
     name="aihandler",
-    version="1.9.6",
+    version="1.9.7",
     author="Capsize LLC",
     description="AI Handler: An engine which wraps certain huggingface models",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `aihandler-1.9.6/src/aihandler/base_runner.py` & `aihandler-1.9.7/src/aihandler/base_runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/controlnet_utils.py` & `aihandler-1.9.7/src/aihandler/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/database.py` & `aihandler-1.9.7/src/aihandler/database.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/llmrunner.py` & `aihandler-1.9.7/src/aihandler/llmrunner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/logger.py` & `aihandler-1.9.7/src/aihandler/logger.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/offline_client.py` & `aihandler-1.9.7/src/aihandler/offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/pyqt_offline_client.py` & `aihandler-1.9.7/src/aihandler/pyqt_offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/qtvar.py` & `aihandler-1.9.7/src/aihandler/qtvar.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/runner.py` & `aihandler-1.9.7/src/aihandler/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,14 +474,36 @@
     def load_controlnet_scheduler(self):
         if self.data["options"]["enable_model_cpu_offload"]:
             from diffusers import UniPCMultistepScheduler
             self.pipe.scheduler = UniPCMultistepScheduler.from_config(self.pipe.scheduler.config)
             self.pipe.enable_model_cpu_offload()
 
     def _load_ckpt_model(self):
+        logger.debug(f"Loading ckpt file, is safetensors {self.is_safetensors}")
+        try:
+            pipeline = self.download_from_original_stable_diffusion_ckpt()
+            if self.is_controlnet:
+                pipeline = self.load_controlnet_from_ckpt(pipeline)
+        except Exception as e:
+            print("Something went wrong loading the model file", e)
+            self.error_handler("Unable to load ckpt file")
+            raise e
+        # to half
+        # determine which data type to move the model to
+        pipeline.vae.to(self.data_type)
+        pipeline.text_encoder.to(self.data_type)
+        pipeline.unet.to(self.data_type)
+        if self.do_nsfw_filter:
+            pipeline.safety_checker.half()
+        return pipeline
+
+    def download_from_original_stable_diffusion_ckpt(self, config="v1.yaml"):
+        from diffusers.pipelines.stable_diffusion.convert_from_ckpt import \
+            download_from_original_stable_diffusion_ckpt
+        print("is safetensors", self.is_safetensors)
         schedulers = {
             "Euler": "euler",
             "Euler a": "euler-ancestral",
             "LMS": "lms",
             "PNDM": "pndm",
             "Heun": "heun",
             "DDIM": "ddim",
@@ -490,40 +512,30 @@
             "DPM singlestep": "dpmss",
             "DPM++ multistep": "dpm++",
             "DPM++ singlestep": "dpmss++",
             "DPM2 k": "dpm2k",
             "DPM2 a k": "dpm2ak",
             "DEIS": "deis",
         }
-        from diffusers.pipelines.stable_diffusion.convert_from_ckpt import \
-            download_from_original_stable_diffusion_ckpt
-        logger.debug(f"Loading ckpt file, is safetensors {self.is_safetensors}")
         try:
-            pipeline = download_from_original_stable_diffusion_ckpt(
+            return download_from_original_stable_diffusion_ckpt(
                 checkpoint_path=self.model,
-                original_config_file="v1.yaml",
+                original_config_file=config,
                 scheduler_type=schedulers[self.scheduler_name],
                 device=self.device,
                 from_safetensors=self.is_safetensors,
                 load_safety_checker=self.do_nsfw_filter,
             )
-            if self.is_controlnet:
-                pipeline = self.load_controlnet_from_ckpt(pipeline)
-        except Exception as e:
-            print("Something went wrong loading the model file", e)
-            self.error_handler("Unable to load ckpt file")
-            raise e
-        # to half
-        # determine which data type to move the model to
-        pipeline.vae.to(self.data_type)
-        pipeline.text_encoder.to(self.data_type)
-        pipeline.unet.to(self.data_type)
-        if self.do_nsfw_filter:
-            pipeline.safety_checker.half()
-        return pipeline
+        # find exception: RuntimeError: Error(s) in loading state_dict for UNet2DConditionModel
+        except RuntimeError as e:
+            if e.args[0].startswith("Error(s) in loading state_dict for UNet2DConditionModel") and config  == "v1.yaml":
+                logger.info("Failed to load model with v1.yaml config file, trying v2.yaml")
+                return self.download_from_original_stable_diffusion_ckpt(config="v2.yaml")
+            else:
+                raise e
 
     def _load_model(self):
         logger.info("Loading model...")
         self.embeds_loaded = False
         if self.is_ckpt_model or self.is_safetensors:
             kwargs = {}
         else:
```

### Comparing `aihandler-1.9.6/src/aihandler/settings.py` & `aihandler-1.9.7/src/aihandler/settings.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/settings_manager.py` & `aihandler-1.9.7/src/aihandler/settings_manager.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/socket_server.py` & `aihandler-1.9.7/src/aihandler/socket_server.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler/util.py` & `aihandler-1.9.7/src/aihandler/util.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler.egg-info/PKG-INFO` & `aihandler-1.9.7/src/aihandler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.6
+Version: 1.9.7
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.6/src/aihandler.egg-info/SOURCES.txt` & `aihandler-1.9.7/src/aihandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.6/src/aihandler.egg-info/requires.txt` & `aihandler-1.9.7/src/aihandler.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 xformers==0.0.18
 omegaconf==2.3.0
 accelerate==0.18.0
 controlnet_aux==0.0.1
 huggingface-hub==0.13.3
 numpy==1.23.5
 Pillow==9.4.0
-pip==23.0.1
+pip==23.1.0
 PyQt6==6.4.2
 PyQt6-Qt6==6.4.3
 PyQt6-sip==13.4.1
 pyqtdarktheme==2.1.0
 pyre-extensions==0.0.23
 lightning==2.0.0
 requests==2.28.2
```

