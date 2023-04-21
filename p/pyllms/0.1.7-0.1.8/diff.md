# Comparing `tmp/pyllms-0.1.7.tar.gz` & `tmp/pyllms-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.1.7.tar", last modified: Tue Apr 18 08:36:36 2023, max compression
+gzip compressed data, was "pyllms-0.1.8.tar", last modified: Fri Apr 21 16:52:40 2023, max compression
```

## Comparing `pyllms-0.1.7.tar` & `pyllms-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.512801 pyllms-0.1.7/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.7/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    14594 2023-04-18 08:36:36.512506 pyllms-0.1.7/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    13353 2023-04-18 08:36:22.000000 pyllms-0.1.7/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.509925 pyllms-0.1.7/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.7/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    17345 2023-04-18 08:26:54.000000 pyllms-0.1.7/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.511015 pyllms-0.1.7/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.7/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.7/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     4237 2023-04-18 08:34:19.000000 pyllms-0.1.7/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3719 2023-04-18 08:32:10.000000 pyllms-0.1.7/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-18 08:36:36.512169 pyllms-0.1.7/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    14594 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       69 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-18 08:36:36.000000 pyllms-0.1.7/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-18 08:36:36.512888 pyllms-0.1.7/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     1780 2023-04-18 08:35:05.000000 pyllms-0.1.7/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.509910 pyllms-0.1.8/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2023-04-10 01:29:26.000000 pyllms-0.1.8/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    14670 2023-04-21 16:52:40.509549 pyllms-0.1.8/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    13429 2023-04-21 16:52:18.000000 pyllms-0.1.8/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.504559 pyllms-0.1.8/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2023-04-13 02:24:28.000000 pyllms-0.1.8/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    18089 2023-04-21 16:50:45.000000 pyllms-0.1.8/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.507639 pyllms-0.1.8/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      107 2023-04-09 20:11:29.000000 pyllms-0.1.8/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2333 2023-04-13 21:39:49.000000 pyllms-0.1.8/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     6657 2023-04-21 16:48:57.000000 pyllms-0.1.8/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     5645 2023-04-21 16:48:57.000000 pyllms-0.1.8/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2023-04-21 16:52:40.509164 pyllms-0.1.8/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    14670 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      308 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       69 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2023-04-21 16:52:40.000000 pyllms-0.1.8/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2023-04-21 16:52:40.510003 pyllms-0.1.8/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     1780 2023-04-21 16:50:58.000000 pyllms-0.1.8/setup.py
```

### Comparing `pyllms-0.1.7/LICENSE` & `pyllms-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.7/PKG-INFO` & `pyllms-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.7
+Version: 0.1.8
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -223,14 +223,16 @@
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
 >>> model.list()
 
 [{'provider': 'AnthropicProvider', 'name': 'claude-instant-v1', 'cost': {'prompt': 0.43, 'completion': 1.45}}, {'provider': 'OpenAIProvider', 'name': 'gpt-3.5-turbo', 'cost': {'prompt': 2.0, 'completion': 2.0}}, {'provider': 'AI21Provider', 'name': 'j2-large', 'cost': {'prompt': 3.0, 'completion': 3.0}}, {'provider': 'AnthropicProvider', 'name': 'claude-v1', 'cost': {'prompt': 2.9, 'completion': 8.6}}, {'provider': 'AI21Provider', 'name': 'j2-grande', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-grande-instruct', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo-instruct', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'OpenAIProvider', 'name': 'gpt-4', 'cost': {'prompt': 30.0, 'completion': 60.0}}]
+
+>>> model.list("gpt') # lists only models with 'gpt' in name/provider name
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
 [AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
```

### Comparing `pyllms-0.1.7/README.md` & `pyllms-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,16 @@
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
 >>> model.list()
 
 [{'provider': 'AnthropicProvider', 'name': 'claude-instant-v1', 'cost': {'prompt': 0.43, 'completion': 1.45}}, {'provider': 'OpenAIProvider', 'name': 'gpt-3.5-turbo', 'cost': {'prompt': 2.0, 'completion': 2.0}}, {'provider': 'AI21Provider', 'name': 'j2-large', 'cost': {'prompt': 3.0, 'completion': 3.0}}, {'provider': 'AnthropicProvider', 'name': 'claude-v1', 'cost': {'prompt': 2.9, 'completion': 8.6}}, {'provider': 'AI21Provider', 'name': 'j2-grande', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-grande-instruct', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo-instruct', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'OpenAIProvider', 'name': 'gpt-4', 'cost': {'prompt': 30.0, 'completion': 60.0}}]
+
+>>> model.list("gpt') # lists only models with 'gpt' in name/provider name
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
 [AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
```

### Comparing `pyllms-0.1.7/llms/llms.py` & `pyllms-0.1.8/llms/llms.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import statistics
 from prettytable import PrettyTable
 from .providers import OpenAIProvider
 from .providers import AnthropicProvider
 from .providers import AI21Provider
 import concurrent.futures
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 
 class Result:
     def __init__(self, results):
         self._results = results
 
     @property
@@ -134,14 +134,36 @@
                 for provider in self._providers
             }
             for future in as_completed(futures):
                 results.append(future.result())
 
         return Result(results)
 
+    async def acomplete(self,
+                        prompt: str,
+                        history: Optional[List[tuple]] = None,
+                        **kwargs,
+                        ):
+        if len(self._providers) > 1:
+            raise NotImplementedError("acomplete not supported for multi-models yet.")
+        provider = self._providers[0]
+        response = await provider.acomplete(prompt, history, **kwargs)
+
+        formatted_cost = format(response["meta"]["cost"], '.5f')
+        formatted_latency = round(response["meta"]["latency"], 2)
+
+        response["meta"]["cost"] = formatted_cost
+        response["meta"]["latency"] = formatted_latency
+
+        return Result([{
+            "text": response["text"],
+            "meta": response["meta"],
+            "provider": provider,
+        }])
+
     def complete_stream(self, prompt, history=None, system_message=None, **kwargs):
                  
         if len(self._providers)>1:
             raise ValueError(
                 "Streaming is possible only with a single model"
             )
         if isinstance(self._providers[0], AI21Provider):
@@ -206,15 +228,14 @@
 """
             # prompt = "Please evaluate the following answers on a scale of 1 to 10 (10 being the best):\n\n"
             prompt = ""
             for i, (query, answer) in enumerate(query_answer_pairs):
                 prompt += f"Query #{i + 1}: {query}\nAnswer #{i + 1}: {answer}\n\n"
             #            prompt += "Please provide a score for each answer as a list of integers separated by commas, with no additional text or explanation. For example: 6, 10, 10"
             #print(prompt)
-            evaluator_result = evaluator.complete(prompt, system=system).text
             #print(evaluator_result)
             scores = evaluator_result.split(",")
             return [int(score.strip()) for score in scores]
 
         model_results = {}
 
         def process_prompt(model, prompt, index):
```

### Comparing `pyllms-0.1.7/llms/providers/ai21.py` & `pyllms-0.1.8/llms/providers/ai21.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.1.7/llms/providers/anthropic.py` & `pyllms-0.1.8/llms/providers/anthropic.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,33 +32,38 @@
             )
 
     def complete(self,
                  prompt: str,
                  history: Optional[List[tuple]] = None,
                  temperature: float = 0,
                  max_tokens: int = 300,
+                 stop_sequences: Optional[List[str]] = None,
+                 ai_prompt: str = "",
                  **kwargs
                  ):
 
-        formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}"
+        formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
         if history is not None:
             role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
             history_messages = itertools.chain.from_iterable(history)
             history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
             formatted_prompt = f"{history_prompt}{formatted_prompt}"
 
         if 'max_tokens_to_sample' not in kwargs:
             kwargs['max_tokens_to_sample'] = max_tokens  # Add maxTokens to kwargs if not present
 
+        if stop_sequences is None:
+            stop_sequences = [anthropic.HUMAN_PROMPT]
+
         start_time = time.time()
         response = self.client.completion(
             prompt=formatted_prompt,
-            stop_sequences=[anthropic.HUMAN_PROMPT],
             temperature=temperature,
             model=self.model,
+            stop_sequences=stop_sequences,
             **kwargs,
         )
         latency = time.time() - start_time
         completion = response["completion"].strip()
 
         # Calculate tokens and cost
         prompt_tokens = anthropic.count_tokens(formatted_prompt)
@@ -78,14 +83,69 @@
                 "tokens_prompt": prompt_tokens,
                 "tokens_completion": completion_tokens,
                 "cost": cost,
                 "latency": latency,
             },
         }
 
+    async def acomplete(self,
+                        prompt: str,
+                        history: Optional[List[tuple]] = None,
+                        temperature: float = 0,
+                        max_tokens: int = 300,
+                        stop_sequences: Optional[List[str]] = None,
+                        ai_prompt: str = "",
+                        **kwargs
+                        ):
+
+        formatted_prompt = f"{anthropic.HUMAN_PROMPT}{prompt}{anthropic.AI_PROMPT}{ai_prompt}"
+        if history is not None:
+            role_cycle = itertools.cycle((anthropic.HUMAN_PROMPT, anthropic.AI_PROMPT))
+            history_messages = itertools.chain.from_iterable(history)
+            history_prompt = "".join(itertools.chain.from_iterable(zip(role_cycle, history_messages)))
+            formatted_prompt = f"{history_prompt}{formatted_prompt}"
+
+        if 'max_tokens_to_sample' not in kwargs:
+            kwargs['max_tokens_to_sample'] = max_tokens  # Add maxTokens to kwargs if not present
+
+        if stop_sequences is None:
+            stop_sequences = [anthropic.HUMAN_PROMPT]
+
+        start_time = time.time()
+        response = await self.client.acompletion(
+            prompt=formatted_prompt,
+            temperature=temperature,
+            model=self.model,
+            stop_sequences=stop_sequences,
+            **kwargs,
+        )
+        latency = time.time() - start_time
+        completion = response["completion"].strip()
+
+        # Calculate tokens and cost
+        prompt_tokens = anthropic.count_tokens(formatted_prompt)
+        completion_tokens = anthropic.count_tokens(completion)
+        total_tokens = prompt_tokens + completion_tokens
+        cost_per_token = self.MODEL_INFO[self.model]
+        cost = (
+            (prompt_tokens * cost_per_token["prompt"])
+            + (completion_tokens * cost_per_token["completion"])
+        ) / 1_000_000
+
+        return {
+            "text": completion,
+            "meta": {
+                "model": self.model,
+                "tokens": total_tokens,
+                "tokens_prompt": prompt_tokens,
+                "tokens_completion": completion_tokens,
+                "cost": cost,
+                "latency": latency,
+            },
+        }
 
     def complete_stream(self,
                  prompt: str,
                  history: Optional[List[tuple]] = None,
                  temperature: float = 0,
                  max_tokens: int = 300,
                  **kwargs
```

### Comparing `pyllms-0.1.7/llms/providers/openai.py` & `pyllms-0.1.8/llms/providers/openai.py`

 * *Files 22% similar despite different names*

```diff
@@ -72,14 +72,64 @@
                 "tokens_prompt": prompt_tokens,  # Add tokens_prompt to meta
                 "tokens_completion": completion_tokens,  # Add tokens_completion to meta
                 "cost": cost,
                 "latency": latency,
             },
         }
 
+    async def acomplete(self,
+                        prompt: str,
+                        history: Optional[List[tuple]] = None,
+                        system_message: str = None,
+                        temperature: float = 0,
+                        **kwargs
+                        ):
+        start_time = time.time()
+
+        messages = [{"role": "user", "content": prompt}]
+
+        if history:
+            role_cycle = itertools.cycle(('user', 'assistant'))
+            history_messages = itertools.chain.from_iterable(history)
+
+            history = [{"role": role, "content": message}
+                       for role, message in zip(role_cycle, history_messages)
+                       if message is not None]
+            messages = [*history, *messages]
+
+        if system_message:
+            messages = [{"role": "system", "content": system_message}, *messages] 
+
+        response = await openai.ChatCompletion.acreate(
+            model=self.model, messages=messages, temperature=temperature, **kwargs
+        )
+
+        latency = time.time() - start_time
+        completion = response.choices[0].message.content.strip()
+        usage = response.usage
+        prompt_tokens = usage["prompt_tokens"]
+        completion_tokens = usage["completion_tokens"]
+        total_tokens = usage["total_tokens"]
+
+        cost_per_token = self.MODEL_INFO[self.model]
+        cost = (prompt_tokens * cost_per_token["prompt"] / 1000000) + (
+            completion_tokens * cost_per_token["completion"] / 1000000
+        )
+
+        return {
+            "text": completion,
+            "meta": {
+                "model": self.model,
+                "tokens": total_tokens,
+                "tokens_prompt": prompt_tokens,  # Add tokens_prompt to meta
+                "tokens_completion": completion_tokens,  # Add tokens_completion to meta
+                "cost": cost,
+                "latency": latency,
+            },
+        }
 
     def complete_stream(self,
                  prompt: str,
                  history: Optional[List[tuple]] = None,
                  system_message: str = None,
                  temperature: float = 0,
                  **kwargs):
```

### Comparing `pyllms-0.1.7/pyllms.egg-info/PKG-INFO` & `pyllms-0.1.8/pyllms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.1.7
+Version: 0.1.8
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21
@@ -223,14 +223,16 @@
 To get a list of supported models, call list(). Models will be shown in the order of least expensive to most expensive.
 
 ```
 >>> model=llms.init()
 >>> model.list()
 
 [{'provider': 'AnthropicProvider', 'name': 'claude-instant-v1', 'cost': {'prompt': 0.43, 'completion': 1.45}}, {'provider': 'OpenAIProvider', 'name': 'gpt-3.5-turbo', 'cost': {'prompt': 2.0, 'completion': 2.0}}, {'provider': 'AI21Provider', 'name': 'j2-large', 'cost': {'prompt': 3.0, 'completion': 3.0}}, {'provider': 'AnthropicProvider', 'name': 'claude-v1', 'cost': {'prompt': 2.9, 'completion': 8.6}}, {'provider': 'AI21Provider', 'name': 'j2-grande', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-grande-instruct', 'cost': {'prompt': 10.0, 'completion': 10.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'AI21Provider', 'name': 'j2-jumbo-instruct', 'cost': {'prompt': 15.0, 'completion': 15.0}}, {'provider': 'OpenAIProvider', 'name': 'gpt-4', 'cost': {'prompt': 30.0, 'completion': 60.0}}]
+
+>>> model.list("gpt') # lists only models with 'gpt' in name/provider name
 ```
 
 Useful links:\
 [OpenAI documentation](https://platform.openai.com/docs/api-reference/completions)\
 [Anthropic documentation](https://console.anthropic.com/docs/api/reference#-v1-complete)\
 [AI21 documentation](https://docs.ai21.com/reference/j2-instruct-ref)
```

### Comparing `pyllms-0.1.7/setup.py` & `pyllms-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.1.7",
+    version="0.1.8",
     description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, AI21), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
```

