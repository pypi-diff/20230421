# Comparing `tmp/thinkgpt-0.0.1.tar.gz` & `tmp/thinkgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkgpt-0.0.1.tar", max compression
+gzip compressed data, was "thinkgpt-0.0.2.tar", max compression
```

## Comparing `thinkgpt-0.0.1.tar` & `thinkgpt-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.1/LICENSE
--rw-r--r--   0        0        0     7601 2023-04-17 00:05:06.375416 thinkgpt-0.0.1/README.md
--rw-r--r--   0        0        0      562 2023-04-16 22:51:53.510872 thinkgpt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.1/thinkgpt/__init__.py
--rw-r--r--   0        0        0     4157 2023-04-16 20:58:23.227617 thinkgpt-0.0.1/thinkgpt/abstract.py
--rw-r--r--   0        0        0     2223 2023-04-15 22:14:39.262945 thinkgpt-0.0.1/thinkgpt/condition.py
--rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.1/thinkgpt/helper.py
--rw-r--r--   0        0        0     2812 2023-04-16 20:58:23.231671 thinkgpt-0.0.1/thinkgpt/infer.py
--rw-r--r--   0        0        0     4137 2023-04-16 20:58:23.215360 thinkgpt-0.0.1/thinkgpt/llm.py
--rw-r--r--   0        0        0     2498 2023-04-16 17:31:17.921222 thinkgpt-0.0.1/thinkgpt/memory.py
--rw-r--r--   0        0        0     1854 2023-04-15 15:38:08.801502 thinkgpt-0.0.1/thinkgpt/refine.py
--rw-r--r--   0        0        0     2865 2023-04-16 16:05:14.591073 thinkgpt-0.0.1/thinkgpt/select.py
--rw-r--r--   0        0        0     8502 1970-01-01 00:00:00.000000 thinkgpt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 15:21:33.490604 thinkgpt-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6871 2023-04-20 23:12:15.079797 thinkgpt-0.0.2/README.md
+-rw-r--r--   0        0        0      562 2023-04-21 01:19:20.920060 thinkgpt-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 15:28:05.934649 thinkgpt-0.0.2/thinkgpt/__init__.py
+-rw-r--r--   0        0        0     4157 2023-04-16 20:58:23.227617 thinkgpt-0.0.2/thinkgpt/abstract.py
+-rw-r--r--   0        0        0     2223 2023-04-15 22:14:39.262945 thinkgpt-0.0.2/thinkgpt/condition.py
+-rw-r--r--   0        0        0     3061 2023-04-20 23:52:42.818016 thinkgpt-0.0.2/thinkgpt/gpt_select.py
+-rw-r--r--   0        0        0     1165 2023-04-16 03:45:24.127522 thinkgpt-0.0.2/thinkgpt/helper.py
+-rw-r--r--   0        0        0     2812 2023-04-16 20:58:23.231671 thinkgpt-0.0.2/thinkgpt/infer.py
+-rw-r--r--   0        0        0     4410 2023-04-21 00:39:21.276973 thinkgpt-0.0.2/thinkgpt/llm.py
+-rw-r--r--   0        0        0     2509 2023-04-21 00:50:43.413297 thinkgpt-0.0.2/thinkgpt/memory.py
+-rw-r--r--   0        0        0     1854 2023-04-15 15:38:08.801502 thinkgpt-0.0.2/thinkgpt/refine.py
+-rw-r--r--   0        0        0     3314 2023-04-21 00:43:56.674582 thinkgpt-0.0.2/thinkgpt/summarize.py
+-rw-r--r--   0        0        0     7772 1970-01-01 00:00:00.000000 thinkgpt-0.0.2/PKG-INFO
```

### Comparing `thinkgpt-0.0.1/LICENSE` & `thinkgpt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.1/README.md` & `thinkgpt-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,45 @@
+Metadata-Version: 2.1
+Name: thinkgpt
+Version: 0.0.2
+Summary: ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents.
+License: Apache 2.0
+Author: Alaeddine Abdessalem
+Author-email: alaeddine-13@live.fr
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: docarray (<=0.21.0)
+Requires-Dist: langchain (>=0.0.141,<0.0.142)
+Requires-Dist: openai (>=0.27.4,<0.28.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
+Description-Content-Type: text/markdown
+
 # ThinkGPT 🧠🤖
 ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents. 
 The library aims to help with the following:
 * solve limited context with long memory and compressed knowledge
 * enhance LLMs' one-shot reasoning with higher order reasoning primitives
 * add intelligent decisions to your code base
 
 
 ## Key Features ✨
-* Memory 🧠: GPTs that can remember experience
-* Self-refinement 🔧: Improve model-generated content by addressing critics
-* Abstraction 🌐: Encourages LLMs to generalize rules from examples or observations
-* Inference 💡️: Make educated guesses based on available information
-* Natural Language Conditions 📝: Easily express tasks and conditions in natural language
-* Extremely easy setup and pythonic API thanks to [DocArray](https://github.com/docarray/docarray)
+* Thinking building blocks 🧱:
+    * Memory 🧠: GPTs that can remember experience
+    * Self-refinement 🔧: Improve model-generated content by addressing critics
+    * Abstraction 🌐: Encourages LLMs to generalize rules from examples or observations
+    * Inference 💡️: Make educated guesses based on available information
+    * Natural Language Conditions 📝: Easily express choices and conditions in natural language
+* Efficient and Measurable GPT context length 📐
+* Extremely easy setup and pythonic API 🎯 thanks to [DocArray](https://github.com/docarray/docarray)
 
 ## Installation 💻
 You can install ThinkGPT using pip:
 
 ```shell
 pip install git+https://github.com/alaeddine-13/thinkgpt.git
 ```
@@ -188,15 +211,8 @@
 ...
 ```
 This technique was mainly implemented in the [the Self-Refine: Iterative Refinement with Self-Feedback paper](https://arxiv.org/abs/2303.17651)
 
 
 For more detailed usage and code examples check `./examples`.
 
-## Rationale: why did I build this project ?
-P.S: here I'm just giving my point of view on LLM, shouldn't be considered a scientific argument.
-
-I believe that LLMs are good for one shot reasoning tasks, or what Daniel Kahneman calls [fast thinking](https://en.wikipedia.org/wiki/Thinking,_Fast_and_Slow).
-However, [they are not good at "slow thinking"](https://arxiv.org/abs/2206.10498). In other words, LLMs are limited in their context length and reasoning capacity.
 
-They are not conscious that, when given a complex task, they need to recall previous information from memory, infer new observations or criticize their output.
-This project aims to offload this high-level thinking to the user through a programmatic API. It is up to the user to determine the thinking strategy and how to prompt GPT to reason according to their use case.
```

### Comparing `thinkgpt-0.0.1/pyproject.toml` & `thinkgpt-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thinkgpt"
-version = "0.0.1"
+version = "0.0.2"
 description = "ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents."
 authors = ["Alaeddine Abdessalem <alaeddine-13@live.fr>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
```

### Comparing `thinkgpt-0.0.1/thinkgpt/abstract.py` & `thinkgpt-0.0.2/thinkgpt/abstract.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.1/thinkgpt/condition.py` & `thinkgpt-0.0.2/thinkgpt/condition.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.1/thinkgpt/helper.py` & `thinkgpt-0.0.2/thinkgpt/helper.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.1/thinkgpt/infer.py` & `thinkgpt-0.0.2/thinkgpt/infer.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.1/thinkgpt/llm.py` & `thinkgpt-0.0.2/thinkgpt/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,52 +9,56 @@
 from thinkgpt.helper import PythonREPL
 
 from thinkgpt.abstract import AbstractMixin, AbstractChain
 from thinkgpt.condition import ConditionMixin, ConditionChain
 from thinkgpt.infer import InferMixin, InferChain
 from thinkgpt.memory import MemoryMixin, ExecuteWithContextChain
 from thinkgpt.refine import RefineMixin, RefineChain
-from thinkgpt.select import SelectChain, SelectMixin
+from thinkgpt.gpt_select import SelectChain, SelectMixin
 
-embeddings_model = OpenAIEmbeddings()
+from thinkgpt.summarize import SummarizeMixin, SummarizeChain
 
 
-class ThinkGPT(OpenAIChat, MemoryMixin, AbstractMixin, RefineMixin, ConditionMixin, SelectMixin, InferMixin, extra=Extra.allow):
+
+class ThinkGPT(OpenAIChat, MemoryMixin, AbstractMixin, RefineMixin, ConditionMixin, SelectMixin, InferMixin, SummarizeMixin, extra=Extra.allow):
     """Wrapper around OpenAI large language models to augment it with memory
 
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``OPENAI_API_KEY`` set with your API key.
     """
 
     def __init__(self,
                  memory: DocumentArray = None,
                  execute_with_context_chain: ExecuteWithContextChain = None,
                  abstract_chain: AbstractChain = None,
                  refine_chain: RefineChain = None,
                  condition_chain: ConditionChain = None,
                  select_chain: SelectChain = None,
                  infer_chain: InferChain = None,
+                 summarize_chain: SummarizeChain = None,
                  verbose=True,
                  # TODO: model name can be specified per mixin
                  **kwargs
                  ):
         super().__init__(**kwargs)
         # TODO: offer more docarray backends
         self.memory = memory or DocumentArray()
+        self.embeddings_model = OpenAIEmbeddings()
         self.openai = OpenAI(model_name=kwargs.get('model_name'))
         self.execute_with_context_chain = execute_with_context_chain or ExecuteWithContextChain.from_llm(
             self.openai, verbose=verbose)
         self.abstract_chain = abstract_chain or AbstractChain.from_llm(
             self.openai, verbose=verbose)
         self.refine_chain = refine_chain or RefineChain.from_llm(
             self.openai, verbose=verbose)
         self.condition_chain = condition_chain or ConditionChain.from_llm(
             self.openai, verbose=verbose)
         self.select_chain = select_chain or SelectChain.from_llm(self.openai, verbose=verbose)
         self.infer_chain = infer_chain or InferChain.from_llm(self.openai, verbose=verbose)
+        self.summarize_chain = summarize_chain or SummarizeChain.from_llm(self.openai, verbose=verbose)  # Add this line
         self.mem_cnt = 0
 
 
     def generate(
             self, prompts: List[str], stop: Optional[List[str]] = None, remember: Union[int, List[str]] = 0
     ) -> LLMResult:
         # only works for single prompt
@@ -87,8 +91,7 @@
     ], instruction_hint="output the rule in french")
     llm.memorize(rules)
 
     llm.memorize("in tunisian, I went is \"mchit\"")
 
     task = "translate to Tunisian: I didn't go"
     print(llm.predict(task, remember=llm.remember(task)))
-
```

### Comparing `thinkgpt-0.0.1/thinkgpt/memory.py` & `thinkgpt-0.0.2/thinkgpt/memory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
 from typing import Dict, List, Union
 
 import numpy as np
 from langchain import PromptTemplate, LLMChain
-from langchain.llms import OpenAI, BaseLLM, OpenAIChat
 from langchain.embeddings import OpenAIEmbeddings
+from langchain.llms import OpenAI, BaseLLM, OpenAIChat
 from docarray import Document, DocumentArray
-embeddings_model = OpenAIEmbeddings()
 
 
 EXECUTE_WITH_CONTEXT_PROMPT = PromptTemplate(template="""
 Given a context information, reply to the provided request
 Context: {context}
 User request: {prompt}
 """, input_variables=["prompt", "context"], )
@@ -25,19 +24,20 @@
         """Get the response parser."""
         return cls(prompt=EXECUTE_WITH_CONTEXT_PROMPT, llm=llm, verbose=verbose)
 
 
 class MemoryMixin:
     memory: DocumentArray
     mem_cnt: int
+    embeddings_model: OpenAIEmbeddings
 
     def memorize(self, concept: Union[str, Document, DocumentArray, List]):
         self.mem_cnt += 1
         if isinstance(concept, str):
-            doc = Document(text=concept, embedding=np.asarray(embeddings_model.embed_query(concept)), tags={'mem_cnt': self.mem_cnt})
+            doc = Document(text=concept, embedding=np.asarray(self.embeddings_model.embed_query(concept)), tags={'mem_cnt': self.mem_cnt})
             self.memory.append(doc)
         elif isinstance(concept, Document):
             assert concept.embedding is not None
             concept.tags['mem_cnt'] = self.mem_cnt
             self.memory.append(concept)
         elif isinstance(concept, (DocumentArray, list)):
             for doc in concept:
@@ -47,15 +47,15 @@
 
     def remember(self, concept: Union[str, Document] = None, limit: int = 5, sort_by_order: bool = False) -> List[str]:
         if len(self.memory) == 0:
             return []
         if concept is None:
             return [doc.text for doc in self.memory[-limit:]]
         elif isinstance(concept, str):
-            query_input = Document(embedding=np.asarray(embeddings_model.embed_query(concept)))
+            query_input = Document(embedding=np.asarray(self.embeddings_model.embed_query(concept)))
         elif isinstance(concept, Document):
             assert concept.embedding is not None
             query_input = concept
         else:
             raise ValueError('wrong type, must be either str or Document')
 
         docs = self.memory.find(query_input, limit=limit)[0]
```

### Comparing `thinkgpt-0.0.1/thinkgpt/refine.py` & `thinkgpt-0.0.2/thinkgpt/refine.py`

 * *Files identical despite different names*

### Comparing `thinkgpt-0.0.1/thinkgpt/select.py` & `thinkgpt-0.0.2/thinkgpt/gpt_select.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,49 +36,50 @@
 """, input_variables=["question", "options_text", "answer"])
 
 
 def format_options(options: List[str]) -> str:
     return "\n".join(options)
 
 
-SELECT_PROMPT = FewShotPromptTemplate(
-    prefix="Choose the correct answer for the following question from the provided options. {instruction_hint}",
-    examples=SELECT_EXAMPLES,
-    example_prompt=SELECT_EXAMPLE_PROMPT,
-    suffix="Question:\n{question}\nOptions:\n{options_text}\nAnswer:\n",
-    input_variables=["instruction_hint", "question", "options_text"]
-)
 
 
 class SelectOutputParser(BaseOutputParser[Optional[str]]):
     options: List[str]
 
     def parse(self, text: str) -> Optional[str]:
         if text.strip().lower() not in [option.lower() for option in self.options]:
             return None
         return text.strip()
 
 
 class SelectChain(LLMChain):
 
     @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool = True) -> LLMChain:
+    def from_llm(cls, llm: BaseLLM, select_examples: Optional[List] = None, verbose: bool = True) -> LLMChain:
+        SELECT_PROMPT = FewShotPromptTemplate(
+            prefix="Choose the correct answer for the following question from the provided options.",
+            examples=select_examples or SELECT_EXAMPLES,
+            example_prompt=SELECT_EXAMPLE_PROMPT,
+            suffix="{instruction_hint}\nQuestion:\n{question}\nOptions:\n{options_text}\nAnswer:\n",
+            input_variables=["instruction_hint", "question", "options_text"]
+        )
         return cls(prompt=SELECT_PROMPT, llm=llm, verbose=verbose)
 
     def predict(self, question: str, options: List[str], instruction_hint: str = '', **kwargs: Any) -> str:
         options_text = format_options(options)
         result = super().predict(question=question, options_text=options_text, instruction_hint=instruction_hint,
                                  **kwargs)
         return SelectOutputParser(options=options).parse(result)
 
 
 class SelectMixin:
     select_chain: SelectChain
 
-    def select(self, question: str, options: List[str], instruction_hint: str = '') -> str:
-        return self.select_chain.predict(question=question, options=options, instruction_hint=instruction_hint)
+    def select(self, question: str, options: List[str], instruction_hint: str = '', select_chain: Optional[SelectChain] = None) -> str:
+       chain = select_chain or self.select_chain
+       return chain.predict(question=question, options=options, instruction_hint=instruction_hint)
 
 
 if __name__ == '__main__':
     chain = SelectChain.from_llm(OpenAI(model_name="gpt-3.5-turbo"))
     print(chain.predict(question="Which animal is known as the king of the jungle?",
                         options=["Lion", "Elephant", "Tiger", "Giraffe"], instruction_hint=""))
```

### Comparing `thinkgpt-0.0.1/PKG-INFO` & `thinkgpt-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,24 @@
-Metadata-Version: 2.1
-Name: thinkgpt
-Version: 0.0.1
-Summary: ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents.
-License: Apache 2.0
-Author: Alaeddine Abdessalem
-Author-email: alaeddine-13@live.fr
-Requires-Python: >=3.7,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: docarray (<=0.21.0)
-Requires-Dist: langchain (>=0.0.141,<0.0.142)
-Requires-Dist: openai (>=0.27.4,<0.28.0)
-Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
-Description-Content-Type: text/markdown
-
 # ThinkGPT 🧠🤖
 ThinkGPT is a Python library aimed at implementing Chain of Thoughts for Large Language Models (LLMs), prompting the model to think, reason, and to create generative agents. 
 The library aims to help with the following:
 * solve limited context with long memory and compressed knowledge
 * enhance LLMs' one-shot reasoning with higher order reasoning primitives
 * add intelligent decisions to your code base
 
 
 ## Key Features ✨
-* Memory 🧠: GPTs that can remember experience
-* Self-refinement 🔧: Improve model-generated content by addressing critics
-* Abstraction 🌐: Encourages LLMs to generalize rules from examples or observations
-* Inference 💡️: Make educated guesses based on available information
-* Natural Language Conditions 📝: Easily express tasks and conditions in natural language
-* Extremely easy setup and pythonic API thanks to [DocArray](https://github.com/docarray/docarray)
+* Thinking building blocks 🧱:
+    * Memory 🧠: GPTs that can remember experience
+    * Self-refinement 🔧: Improve model-generated content by addressing critics
+    * Abstraction 🌐: Encourages LLMs to generalize rules from examples or observations
+    * Inference 💡️: Make educated guesses based on available information
+    * Natural Language Conditions 📝: Easily express choices and conditions in natural language
+* Efficient and Measurable GPT context length 📐
+* Extremely easy setup and pythonic API 🎯 thanks to [DocArray](https://github.com/docarray/docarray)
 
 ## Installation 💻
 You can install ThinkGPT using pip:
 
 ```shell
 pip install git+https://github.com/alaeddine-13/thinkgpt.git
 ```
@@ -209,16 +190,7 @@
 ...
 ```
 This technique was mainly implemented in the [the Self-Refine: Iterative Refinement with Self-Feedback paper](https://arxiv.org/abs/2303.17651)
 
 
 For more detailed usage and code examples check `./examples`.
 
-## Rationale: why did I build this project ?
-P.S: here I'm just giving my point of view on LLM, shouldn't be considered a scientific argument.
-
-I believe that LLMs are good for one shot reasoning tasks, or what Daniel Kahneman calls [fast thinking](https://en.wikipedia.org/wiki/Thinking,_Fast_and_Slow).
-However, [they are not good at "slow thinking"](https://arxiv.org/abs/2206.10498). In other words, LLMs are limited in their context length and reasoning capacity.
-
-They are not conscious that, when given a complex task, they need to recall previous information from memory, infer new observations or criticize their output.
-This project aims to offload this high-level thinking to the user through a programmatic API. It is up to the user to determine the thinking strategy and how to prompt GPT to reason according to their use case.
-
```

