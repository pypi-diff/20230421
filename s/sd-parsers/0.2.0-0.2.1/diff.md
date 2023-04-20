# Comparing `tmp/sd-parsers-0.2.0.tar.gz` & `tmp/sd-parsers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd-parsers-0.2.0.tar", last modified: Tue Apr 18 01:00:48 2023, max compression
+gzip compressed data, was "sd-parsers-0.2.1.tar", last modified: Thu Apr 20 22:44:30 2023, max compression
```

## Comparing `sd-parsers-0.2.0.tar` & `sd-parsers-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.471964 sd-parsers-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.471964 sd-parsers-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/.github/workflows/publish-to.pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/examples/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/examples/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 01:00:48.479963 sd-parsers-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.471964 sd-parsers-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/src/sd_parsers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 01:00:48.000000 sd-parsers-0.2.0/src/sd_parsers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/src/sdparsers/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parser_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:00:48.475963 sd-parsers-0.2.0/src/sdparsers/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111_stealth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/invokeai.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/parsers/novelai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 01:00:32.000000 sd-parsers-0.2.0/src/sdparsers/prompt_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.082386 sd-parsers-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/.github/workflows/publish-to.pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/examples/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/examples/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.082386 sd-parsers-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/src/sd_parsers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 22:44:30.000000 sd-parsers-0.2.1/src/sd_parsers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/src/sdparsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parser_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 22:44:30.086386 sd-parsers-0.2.1/src/sdparsers/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111_stealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/invokeai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/parsers/novelai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-20 22:44:20.000000 sd-parsers-0.2.1/src/sdparsers/prompt_info.py
```

### Comparing `sd-parsers-0.2.0/.github/workflows/publish-to.pypi.yml` & `sd-parsers-0.2.1/.github/workflows/publish-to.pypi.yml`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/LICENSE.txt` & `sd-parsers-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/PKG-INFO` & `sd-parsers-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.2.0
+Version: 0.2.1
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `sd-parsers-0.2.0/README.md` & `sd-parsers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/examples/cmdline.py` & `sd-parsers-0.2.1/examples/cmdline.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/examples/fast_api.py` & `sd-parsers-0.2.1/examples/fast_api.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/src/sd_parsers.egg-info/PKG-INFO` & `sd-parsers-0.2.1/src/sd_parsers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-parsers
-Version: 0.2.0
+Version: 0.2.1
 Summary: SD Parsers - read metadata from images created by Stable Diffusion
 License: MIT License
         
         Copyright (c) 2023 d3x-at
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `sd-parsers-0.2.0/src/sd_parsers.egg-info/SOURCES.txt` & `sd-parsers-0.2.1/src/sd_parsers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/src/sdparsers/parser.py` & `sd-parsers-0.2.1/src/sdparsers/parser.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/src/sdparsers/parser_manager.py` & `sd-parsers-0.2.1/src/sdparsers/parser_manager.py`

 * *Files identical despite different names*

### Comparing `sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111.py` & `sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self, config=None, process_items=True):
         super().__init__(config, process_items)
         self.sampler_params = self.config.get("sampler_params", SAMPLER_PARAMS_DEFAULT)
 
     @staticmethod
     def _get_parameters(image):
         if image.format == "PNG":
-            return image.info.get('parameters')
+            return image.text.get('parameters')
         elif image.format in ("JPEG", "WEBP"):
             return get_exif_value(image, 'UserComment')
         return None
 
     def parse(self, image):
         parameters = self._get_parameters(image)
         if parameters is None:
@@ -30,21 +30,22 @@
         metadata = self._prepare_metadata(parameters)
         if metadata is None:
             return None
 
         return PromptInfo(self.GENERATOR_ID, *metadata, {"parameters": parameters})
 
     def _prepare_metadata(self, parameters: str):
-        prompt, negative_prompt, metadata = split_parameters(parameters)
-        if metadata is None:
+        try:
+            prompt, negative_prompt, metadata = split_parameters(parameters)
+        except ValueError:
             return None
 
         prompts = [(
-            Prompt(prompt) if prompt else None,
-            Prompt(negative_prompt) if negative_prompt else None
+            Prompt(prompt, parts=[prompt]) if prompt else None,
+            Prompt(negative_prompt, parts=[negative_prompt]) if negative_prompt else None
         )]
 
         models = []
         if 'Model' in metadata or 'Model hash' in metadata:
             model = Model(
                 name=metadata.pop('Model', None),
                 model_hash=metadata.pop('Model hash', None)
@@ -63,33 +64,37 @@
             )
             samplers.append(sampler)
 
         return prompts, samplers, models, self._process_metadata(metadata)
 
 
 def split_parameters(parameters: str) -> Tuple[str, str, dict]:
-    '''split an A1111 parameters string into prompt, negative prompt and metadata'''
-    lines = parameters.split("\n")
-    if not lines:
-        return None, None, None
-
-    def split_meta(item: str):
-        key, value = map(str.strip, item.split(':'))
+    '''
+    split an A1111 parameters string into prompt, negative prompt and metadata
+    :exception ValueError: If the metadata does not conform to the expected format.
+    '''
+
+    def split_meta(item: str) -> Tuple[str, str]:
+        '''
+        split metadata item into key:value pair
+        :exception ValueError: If the item has more or less than two components.
+        '''
+        components = item.split(':')
+        if len(components) != 2:
+            raise ValueError("metadata malformed")
+        key, value = map(str.strip, components)
         return key, value
 
-    metadata = None
-    try:
-        metadata = [split_meta(item) for item in lines[-1].split(',')]
-    except ValueError:
-        pass
+    lines = parameters.split('\n')
+    metadata = dict(split_meta(item) for item in lines[-1].split(','))
 
-    if not metadata or len(metadata) < 3:
+    if len(metadata) < 3:
         # actually a bit stricter than in the webui itself
         # grants some protection against "non-a1111" parameters
-        return None, None, None
+        raise ValueError("metadata too short")
 
     prompt_lines = lines[:-1]
 
     # prompt
     prompt = []
     i = 0
     for line in prompt_lines:
@@ -102,9 +107,9 @@
 
     # negative prompt
     negative_prompt = [line.strip() for line in prompt_lines[i:]]
 
     return (
         "\n".join(prompt),
         "\n".join(negative_prompt),
-        dict(metadata)
+        metadata
     )
```

### Comparing `sd-parsers-0.2.0/src/sdparsers/parsers/automatic1111_stealth.py` & `sd-parsers-0.2.1/src/sdparsers/parsers/automatic1111_stealth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from ..prompt_info import PromptInfo
 from .automatic1111 import AUTOMATIC1111Parser
 
 
 class AUTOMATICStealthParser(AUTOMATIC1111Parser):
     PRIORITY = -1
-    GENERATOR_ID = "AUTOMATICStealth"
 
     def parse(self, image):
         if image.mode != 'RGBA' or image.format != 'PNG':
             return None
 
         geninfo = self._read_info_from_image_stealth(image)
         if not geninfo:
```

### Comparing `sd-parsers-0.2.0/src/sdparsers/parsers/invokeai.py` & `sd-parsers-0.2.1/src/sdparsers/parsers/invokeai.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,23 @@
     GENERATOR_ID = "InvokeAI"
 
     def __init__(self, config=None, process_items=True):
         super().__init__(config, process_items)
         self.sampler_params = self.config.get("sampler_params", SAMPLER_PARAMS_DEFAULT)
 
     def parse(self, image):
-        params_metadata = image.info.get('sd-metadata')
+        if image.format != "PNG":
+            return None
+
+        params_metadata = image.text.get('sd-metadata')
         if not params_metadata:
             return None
 
         raw_params = {'sd-metadata': params_metadata}
-        params_dream = image.info.get('Dream')
+        params_dream = image.text.get('Dream')
         if params_dream:
             raw_params['Dream'] = params_dream
 
         try:
             prompts, sampler, model, metadata = self._prepare_metadata(params_metadata)
         except KeyError:
             return None
@@ -36,16 +39,22 @@
     def _prepare_metadata(self, params_metadata):
         metadata = json.loads(params_metadata)
 
         def split_prompt(prompt: str, weight: float):
             negatives = list(map(str.strip, _RE_PROMPT_NEGATIVES.findall(prompt)))
             positive = _RE_PROMPT_NEGATIVES.sub('', prompt).strip()
             return (
-                Prompt(value=positive, weight=weight) if positive else None,
-                Prompt(value=', '.join(negatives), weight=weight) if negatives else None
+                Prompt(
+                    value=positive,
+                    parts=[positive],
+                    weight=weight) if positive else None,
+                Prompt(
+                    value=', '.join(negatives),
+                    parts=negatives,
+                    weight=weight) if negatives else None
             )
 
         metadata_image = dict(metadata.pop('image'))
         prompts = [split_prompt(prompt["prompt"], float(prompt["weight"]))
                    for prompt in metadata_image.pop('prompt')]
 
         sampler_params = ((key, metadata_image.pop(key))
```

### Comparing `sd-parsers-0.2.0/src/sdparsers/prompt_info.py` & `sd-parsers-0.2.1/src/sdparsers/prompt_info.py`

 * *Files identical despite different names*

