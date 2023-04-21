# Comparing `tmp/zeno_evals-0.1.7.tar.gz` & `tmp/zeno_evals-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeno_evals-0.1.7.tar", max compression
+gzip compressed data, was "zeno_evals-0.1.8.tar", max compression
```

## Comparing `zeno_evals-0.1.7.tar` & `zeno_evals-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.7/LICENSE.md
--rw-r--r--   0        0        0     1259 2023-04-18 17:05:50.193994 zeno_evals-0.1.7/README.md
--rw-r--r--   0        0        0      537 2023-04-18 17:16:06.138189 zeno_evals-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       84 2023-04-18 15:03:49.480326 zeno_evals-0.1.7/zeno_evals/__init__.py
--rw-r--r--   0        0        0       29 2023-04-18 15:06:35.651777 zeno_evals-0.1.7/zeno_evals/__main__.py
--rw-r--r--   0        0        0     6316 2023-04-18 16:53:55.919011 zeno_evals-0.1.7/zeno_evals/main.py
--rw-r--r--   0        0        0     2088 1970-01-01 00:00:00.000000 zeno_evals-0.1.7/setup.py
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 zeno_evals-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0     1303 2023-04-18 18:06:34.832884 zeno_evals-0.1.8/README.md
+-rw-r--r--   0        0        0      537 2023-04-21 13:07:11.143849 zeno_evals-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-04-18 15:03:49.480326 zeno_evals-0.1.8/zeno_evals/__init__.py
+-rw-r--r--   0        0        0       29 2023-04-18 15:06:35.651777 zeno_evals-0.1.8/zeno_evals/__main__.py
+-rw-r--r--   0        0        0     6368 2023-04-21 13:06:44.157476 zeno_evals-0.1.8/zeno_evals/main.py
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 zeno_evals-0.1.8/setup.py
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 zeno_evals-0.1.8/PKG-INFO
```

### Comparing `zeno_evals-0.1.7/LICENSE.md` & `zeno_evals-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.7/README.md` & `zeno_evals-0.1.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 ```bash
 zeno-evals ./examples/example.jsonl
 ```
 
 And an example of comparison between two models:
 
 ```bash
-zeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl
+zeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl
 ```
 
 And lastly, we can pass additional [Zeno functions](https://zenoml.com/docs/api) to provide more context to the results:
 
 ```bash
 pip install wordfreq
-zeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py
+zeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py
 ```
```

### Comparing `zeno_evals-0.1.7/pyproject.toml` & `zeno_evals-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeno-evals"
-version = "0.1.7"
+version = "0.1.8"
 description = "Visualize OpenAI evals with Zeno"
 authors = ["Alex Cabrera <alex.cabrera@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "zeno_evals" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<=3.11"
```

### Comparing `zeno_evals-0.1.7/zeno_evals/main.py` & `zeno_evals-0.1.8/zeno_evals/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,66 +72,67 @@
 
 
 @model
 def model_fn(name):
     model_df = dfs[name]
 
     def mod(df, ops):
-        return ModelReturn(model_output=model_df["sampled"].loc[df.index].tolist())
+        return ModelReturn(model_output=model_df["sampled"].loc[df["id"]].tolist())
 
     return mod
 
 
 @distill
 def correct(df, ops: ZenoOptions):
     model_name = [i for i in dfs.keys() if i in ops.output_column]
     model_df = dfs[model_name[0]]
-    return DistillReturn(distill_output=model_df["correct"].loc[df.index])
+    return DistillReturn(distill_output=model_df["correct"].loc[df["id"]])
 
 
 @metric
 def avg_correct(df, ops: ZenoOptions):
     return MetricReturn(
         metric=df[ops.distill_columns["correct"]].astype(int).mean() * 100
     )
 
 
 def read_results_file(data):
+    data_res = [d for d in data if "event_id" in d]
     sampling_df = pd.DataFrame(
         [
             {
                 "id": d["sample_id"],
                 "prompt": d["data"]["prompt"],
                 "sampled": d["data"]["sampled"][0],
             }
-            for d in data[2:]
+            for d in data_res
             if "type" in d and d["type"] == "sampling"
         ]
     )
 
     match_df = pd.DataFrame(
         [
             {
                 "id": d["sample_id"],
                 "correct": d["data"]["correct"],
                 "expected": d["data"]["expected"],
             }
-            for d in data[2:]
+            for d in data_res
             if "type" in d and d["type"] == "match"
         ]
     )
 
     metric_names = []
-    for d in data[2:]:
+    for d in data_res:
         if "type" in d and d["type"] == "metrics":
             metric_names = list(d["data"].keys())
             break
 
     metrics = []
-    for d in data[2:]:
+    for d in data_res:
         if "type" in d and d["type"] == "metrics":
             met_obj = {"id": d["sample_id"]}
             for name in metric_names:
                 met_obj[name] = d["data"][name]
             metrics.append(met_obj)
     metrics_df = pd.DataFrame(metrics)
```

### Comparing `zeno_evals-0.1.7/setup.py` & `zeno_evals-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['fire>=0.5.0,<0.6.0', 'pandas>=1.5.3,<2.0.0', 'zenoml>=0.4.10,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['zeno-evals = zeno_evals.main:cli']}
 
 setup_kwargs = {
     'name': 'zeno-evals',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Visualize OpenAI evals with Zeno',
-    'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\nSingle example looking at US tort law questions:\n\n```bash\nzeno-evals ./examples/example.jsonl\n```\n\nAnd an example of comparison between two models:\n\n```bash\nzeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl\n```\n\nAnd lastly, we can pass additional [Zeno functions](https://zenoml.com/docs/api) to provide more context to the results:\n\n```bash\npip install wordfreq\nzeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py\n```\n',
+    'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\nSingle example looking at US tort law questions:\n\n```bash\nzeno-evals ./examples/example.jsonl\n```\n\nAnd an example of comparison between two models:\n\n```bash\nzeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl\n```\n\nAnd lastly, we can pass additional [Zeno functions](https://zenoml.com/docs/api) to provide more context to the results:\n\n```bash\npip install wordfreq\nzeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py\n```\n',
     'author': 'Alex Cabrera',
     'author_email': 'alex.cabrera@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `zeno_evals-0.1.7/PKG-INFO` & `zeno_evals-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno-evals
-Version: 0.1.7
+Version: 0.1.8
 Summary: Visualize OpenAI evals with Zeno
 Author: Alex Cabrera
 Author-email: alex.cabrera@gmail.com
 Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -43,17 +43,17 @@
 ```bash
 zeno-evals ./examples/example.jsonl
 ```
 
 And an example of comparison between two models:
 
 ```bash
-zeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl
+zeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl
 ```
 
 And lastly, we can pass additional [Zeno functions](https://zenoml.com/docs/api) to provide more context to the results:
 
 ```bash
 pip install wordfreq
-zeno-evals ./examples/crossword-turbo.jsonl ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py
+zeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py
 ```
```

