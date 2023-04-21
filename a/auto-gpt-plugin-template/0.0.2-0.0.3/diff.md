# Comparing `tmp/auto_gpt_plugin_template-0.0.2.tar.gz` & `tmp/auto_gpt_plugin_template-0.0.3.tar.gz`

## Comparing `auto_gpt_plugin_template-0.0.2.tar` & `auto_gpt_plugin_template-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.flake8
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.isort.cfg
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.sourcery.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/clean_all.sh
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/qa.sh
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/requirements.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/style.sh
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/src/auto_gpt_plugin_template/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/LICENSE
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/README.md
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/.coveragerc
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/.flake8
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/.isort.cfg
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/.sourcery.yaml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/Makefile
+-rwxr-xr-x   0        0        0      896 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/helpers.bat
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/helpers.sh
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/pylintrc
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/run_pylint.py
+-rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/src/auto_gpt_plugin_template/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/LICENSE
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/README.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 auto_gpt_plugin_template-0.0.3/PKG-INFO
```

### Comparing `auto_gpt_plugin_template-0.0.2/.coveragerc` & `auto_gpt_plugin_template-0.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.2/.pre-commit-config.yaml` & `auto_gpt_plugin_template-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.2/.sourcery.yaml` & `auto_gpt_plugin_template-0.0.3/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.2/pylintrc` & `auto_gpt_plugin_template-0.0.3/pylintrc`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.2/src/auto_gpt_plugin_template/__init__.py` & `auto_gpt_plugin_template-0.0.3/src/auto_gpt_plugin_template/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """This is a template for Auto-GPT plugins."""
 import abc
-from typing import Any, Dict, List, Optional, Tuple, TypeVar
+from typing import Any, Dict, List, Optional, Tuple, TypeVar, TypedDict
 
 from abstract_singleton import AbstractSingleton, Singleton
 
 PromptGenerator = TypeVar("PromptGenerator")
 
 
+class Message(TypedDict):
+    role: str
+    content: str
+
+
 class AutoGPTPluginTemplate(AbstractSingleton, metaclass=Singleton):
     """
     This is a template for Auto-GPT plugins.
     """
 
     def __init__(self):
         super().__init__()
@@ -61,17 +66,17 @@
 
         Returns:
             bool: True if the plugin can handle the on_planning method."""
         return False
 
     @abc.abstractmethod
     def on_planning(
-        self, prompt: PromptGenerator, messages: List[str]
+        self, prompt: PromptGenerator, messages: List[Message]
     ) -> Optional[str]:
-        """This method is called before the planning chat completeion is done.
+        """This method is called before the planning chat completion is done.
 
         Args:
             prompt (PromptGenerator): The prompt generator.
             messages (List[str]): The list of messages.
         """
         pass
 
@@ -82,15 +87,15 @@
 
         Returns:
             bool: True if the plugin can handle the post_planning method."""
         return False
 
     @abc.abstractmethod
     def post_planning(self, response: str) -> str:
-        """This method is called after the planning chat completeion is done.
+        """This method is called after the planning chat completion is done.
 
         Args:
             response (str): The response.
 
         Returns:
             str: The resulting response.
         """
@@ -102,40 +107,40 @@
         handle the pre_instruction method.
 
         Returns:
             bool: True if the plugin can handle the pre_instruction method."""
         return False
 
     @abc.abstractmethod
-    def pre_instruction(self, messages: List[str]) -> List[str]:
+    def pre_instruction(self, messages: List[Message]) -> List[Message]:
         """This method is called before the instruction chat is done.
 
         Args:
-            messages (List[str]): The list of context messages.
+            messages (List[Message]): The list of context messages.
 
         Returns:
-            List[str]: The resulting list of messages.
+            List[Message]: The resulting list of messages.
         """
         pass
 
     @abc.abstractmethod
     def can_handle_on_instruction(self) -> bool:
         """This method is called to check that the plugin can
         handle the on_instruction method.
 
         Returns:
             bool: True if the plugin can handle the on_instruction method."""
         return False
 
     @abc.abstractmethod
-    def on_instruction(self, messages: List[str]) -> Optional[str]:
+    def on_instruction(self, messages: List[Message]) -> Optional[str]:
         """This method is called when the instruction chat is done.
 
         Args:
-            messages (List[str]): The list of context messages.
+            messages (List[Message]): The list of context messages.
 
         Returns:
             Optional[str]: The resulting message.
         """
         pass
 
     @abc.abstractmethod
@@ -209,31 +214,31 @@
     def can_handle_chat_completion(
         self, messages: Dict[Any, Any], model: str, temperature: float, max_tokens: int
     ) -> bool:
         """This method is called to check that the plugin can
           handle the chat_completion method.
 
         Args:
-            messages (Dict[Any, Any]): The messages.
+            messages (List[Message]): The messages.
             model (str): The model name.
             temperature (float): The temperature.
             max_tokens (int): The max tokens.
 
           Returns:
               bool: True if the plugin can handle the chat_completion method."""
         return False
 
     @abc.abstractmethod
     def handle_chat_completion(
-        self, messages: Dict[Any, Any], model: str, temperature: float, max_tokens: int
+        self, messages: List[Message], model: str, temperature: float, max_tokens: int
     ) -> str:
         """This method is called when the chat completion is done.
 
         Args:
-            messages (Dict[Any, Any]): The messages.
+            messages (List[Message]): The messages.
             model (str): The model name.
             temperature (float): The temperature.
             max_tokens (int): The max tokens.
 
         Returns:
             str: The resulting response.
         """
```

### Comparing `auto_gpt_plugin_template-0.0.2/.gitignore` & `auto_gpt_plugin_template-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.2/LICENSE` & `auto_gpt_plugin_template-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_gpt_plugin_template-0.0.2/pyproject.toml` & `auto_gpt_plugin_template-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "auto_gpt_plugin_template"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
-  { name="Torantulino", email="34168009+BillSchumacher@users.noreply.github.com" },
+  { name="Torantulino", email="support@agpt.co" },
 ]
 description = "The template plugin for Auto-GPT."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["abstract-singleton"]
 
 [project.urls]
-"Homepage" = "https://github.com/Torantulino/Auto-GPT"
-"Bug Tracker" = "https://github.com/Torantulino/Auto-GPT"
+"Homepage" = "https://github.com/Significant-Gravitas/Auto-GPT"
+"Bug Tracker" = "https://github.com/Significant-Gravitas/Auto-GPT"
 
 [tool.black]
 line-length = 88
 target-version = ['py38']
 include = '\.pyi?$'
 extend-exclude = ""
```

### Comparing `auto_gpt_plugin_template-0.0.2/PKG-INFO` & `auto_gpt_plugin_template-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: auto_gpt_plugin_template
-Version: 0.0.2
+Version: 0.0.3
 Summary: The template plugin for Auto-GPT.
-Project-URL: Homepage, https://github.com/Torantulino/Auto-GPT
-Project-URL: Bug Tracker, https://github.com/Torantulino/Auto-GPT
-Author-email: Torantulino <34168009+BillSchumacher@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/Significant-Gravitas/Auto-GPT
+Project-URL: Bug Tracker, https://github.com/Significant-Gravitas/Auto-GPT
+Author-email: Torantulino <support@agpt.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: abstract-singleton
 Description-Content-Type: text/markdown
```

