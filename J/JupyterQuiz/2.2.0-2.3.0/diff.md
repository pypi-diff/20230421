# Comparing `tmp/JupyterQuiz-2.2.0.tar.gz` & `tmp/JupyterQuiz-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterQuiz-2.2.0.tar", last modified: Tue Apr 18 16:27:10 2023, max compression
+gzip compressed data, was "JupyterQuiz-2.3.0.tar", last modified: Fri Apr 21 13:05:20 2023, max compression
```

## Comparing `JupyterQuiz-2.2.0.tar` & `JupyterQuiz-2.3.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1820 2021-07-06 14:35:18.501466 JupyterQuiz-2.2.0/.gitignore
--rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.2.0/CITATION.cff
--rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.2.0/HideQuiz.ipynb
--rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.2.0/LICENSE
--rw-r--r--   0        0        0     8860 2023-03-11 13:44:15.891925 JupyterQuiz-2.2.0/README.md
--rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.2.0/examples/mc-example.gif
--rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.2.0/examples/num-example.gif
--rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.2.0/examples/questions.json
--rw-r--r--   0        0        0      661 2023-04-18 16:18:26.616246 JupyterQuiz-2.2.0/jupyterquiz/__init__.py
--rw-r--r--   0        0        0     7273 2023-04-18 15:57:35.208735 JupyterQuiz-2.2.0/jupyterquiz/dynamic.py
--rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.2.0/jupyterquiz/helpers.js
--rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.js
--rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.py
--rw-r--r--   0        0        0     7570 2022-08-22 19:45:35.870224 JupyterQuiz-2.2.0/jupyterquiz/numeric.js
--rw-r--r--   0        0        0     5944 2023-04-18 16:11:00.030201 JupyterQuiz-2.2.0/jupyterquiz/show_questions.js
--rw-r--r--   0        0        0     2762 2021-07-06 14:33:13.180515 JupyterQuiz-2.2.0/jupyterquiz/styles.css
--rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.2.0/preserve-responses.ipynb
--rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.2.0/previews/github-preview.png
--rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.2.0/previews/github-preview.psd
--rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1393 2021-07-06 14:33:27.396186 JupyterQuiz-2.2.0/schema/mc_schema.json
--rw-r--r--   0        0        0   166749 2021-06-16 19:44:25.130972 JupyterQuiz-2.2.0/schema/mc_schema.png
--rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.2.0/schema/num_schema.json
--rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.2.0/schema/num_schema.png
--rw-r--r--   0        0        0     8093 2021-06-15 23:07:58.000000 JupyterQuiz-2.2.0/schema/schema.ipynb
--rw-r--r--   0        0        0    54049 2023-04-18 16:14:00.216953 JupyterQuiz-2.2.0/test.ipynb
--rw-r--r--   0        0        0     9174 1970-01-01 00:00:00.000000 JupyterQuiz-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 JupyterQuiz-2.3.0/.gitignore
+-rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.3.0/CITATION.cff
+-rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.3.0/HideQuiz.ipynb
+-rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.3.0/LICENSE
+-rw-r--r--   0        0        0     8860 2023-03-11 13:44:15.891925 JupyterQuiz-2.3.0/README.md
+-rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.3.0/examples/mc-example.gif
+-rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.3.0/examples/num-example.gif
+-rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.3.0/examples/questions.json
+-rw-r--r--   0        0        0      661 2023-04-21 13:03:20.531584 JupyterQuiz-2.3.0/jupyterquiz/__init__.py
+-rw-r--r--   0        0        0     7468 2023-04-21 12:54:08.754441 JupyterQuiz-2.3.0/jupyterquiz/dynamic.py
+-rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.3.0/jupyterquiz/helpers.js
+-rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.js
+-rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.py
+-rw-r--r--   0        0        0     7570 2022-08-22 19:45:35.870224 JupyterQuiz-2.3.0/jupyterquiz/numeric.js
+-rw-r--r--   0        0        0     6034 2023-04-21 12:37:51.040441 JupyterQuiz-2.3.0/jupyterquiz/show_questions.js
+-rw-r--r--   0        0        0     2902 2023-04-21 13:01:28.819811 JupyterQuiz-2.3.0/jupyterquiz/styles.css
+-rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.3.0/preserve-responses.ipynb
+-rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.3.0/previews/github-preview.png
+-rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.3.0/previews/github-preview.psd
+-rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 JupyterQuiz-2.3.0/schema/README
+-rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 JupyterQuiz-2.3.0/schema/mc_schema.json
+-rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 JupyterQuiz-2.3.0/schema/mc_schema.png
+-rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 JupyterQuiz-2.3.0/schema/mc_schema.svg
+-rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.3.0/schema/num_schema.json
+-rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.3.0/schema/num_schema.png
+-rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 JupyterQuiz-2.3.0/schema/schema.ipynb
+-rw-r--r--   0        0        0   281731 2023-04-21 13:02:56.982731 JupyterQuiz-2.3.0/test.ipynb
+-rw-r--r--   0        0        0     9174 1970-01-01 00:00:00.000000 JupyterQuiz-2.3.0/PKG-INFO
```

### Comparing `JupyterQuiz-2.2.0/.gitignore` & `JupyterQuiz-2.3.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -127,7 +127,10 @@
 
 # Pyre type checker
 .pyre/
 
 .DS_Store
 
 .vscode/
+
+.#*
+
```

### Comparing `JupyterQuiz-2.2.0/HideQuiz.ipynb` & `JupyterQuiz-2.3.0/HideQuiz.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/LICENSE` & `JupyterQuiz-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/README.md` & `JupyterQuiz-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/examples/mc-example.gif` & `JupyterQuiz-2.3.0/examples/mc-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/examples/num-example.gif` & `JupyterQuiz-2.3.0/examples/num-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/examples/questions.json` & `JupyterQuiz-2.3.0/examples/questions.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/__init__.py` & `JupyterQuiz-2.3.0/jupyterquiz/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.2.0'
+__version__ = '2.3.0'
 from .dynamic import display_quiz, capture_responses
```

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/dynamic.py` & `JupyterQuiz-2.3.0/jupyterquiz/dynamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import importlib.resources
 import urllib.request
 import urllib
 import json
 import sys
 
 
-def display_quiz(ref, num=1_000_000, shuffle_questions=False, shuffle_answers=True, preserve_responses=False):
+def display_quiz(ref, num=1_000_000, shuffle_questions=False, shuffle_answers=True, preserve_responses=False,
+                 border_radius=10):
     '''
     Display an interactive quiz (currently multiple-choice or numeric answer)
     using a mix of Python and Javascript to support use in rendered notebooks
     (especially JupyterBook, but also Voila)
 
     Inputs:
     ref = string, reference to quiz JSON, may be:
@@ -26,14 +27,16 @@
 
     shuffle_questions = boolean, whether to shuffle order of questions (default False)
 
     shuffle_answers = boolean, whether to shuffle answers for multiple-choice questions (default True)
     
     preserve_responses = boolean, whether to output the user responses in a way that is preserved upon reload of the notebook (default False)
 
+    border_radius = border radius property for all buttons and questions, in pixels (default 10)
+
     John  M. Shea
     9/26/2021
     '''
 
     assert not (shuffle_questions and preserve_responses), \
         "This package does not support preserving responses if questions are shuffled."
     assert num==1_000_000 or (not preserve_responses), \
@@ -52,15 +55,16 @@
         preserve_json = "false"
 
 
 
     mydiv = f"""<div id="{div_id}" data-shufflequestions="{str(shuffle_questions)}"
                data-shuffleanswers="{str(shuffle_answers)}"
                data-preserveresponses="{preserve_json}"
-               data-numquestions="{str(num)}"> """
+               data-numquestions="{str(num)}"
+               style="border-radius: {str(border_radius)}px;"> """
     #print(mydiv)
 
     styles = "<style>"
     f = importlib.resources.files(package).joinpath('styles.css')
     css = f.read_bytes()
     styles += css.decode("utf-8")
     styles += "</style>"
```

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/helpers.js` & `JupyterQuiz-2.3.0/jupyterquiz/helpers.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.js` & `JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/multiple_choice.py` & `JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/numeric.js` & `JupyterQuiz-2.3.0/jupyterquiz/numeric.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/show_questions.js` & `JupyterQuiz-2.3.0/jupyterquiz/show_questions.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -112,15 +112,16 @@
 
         //console.log(qa.type);
 
         var num_correct;
         if ((qa.type == "multiple_choice") || (qa.type == "many_choice")) {
             num_correct = make_mc(qa, shuffle_answers, outerqDiv, qDiv, aDiv, id);
             if ("answer_cols" in qa) {
-                aDiv.style.gridTemplateColumns = 'auto '.repeat(qa.answer_cols);
+                //aDiv.style.gridTemplateColumns = 'auto '.repeat(qa.answer_cols);
+                aDiv.style.gridTemplateColumns = 'repeat(' + qa.answer_cols + ', 1fr)';
             }
         } else if (qa.type == "numeric") {
             //console.log("numeric");
             make_numeric(qa, outerqDiv, qDiv, aDiv, id);
         }
```

### Comparing `JupyterQuiz-2.2.0/jupyterquiz/styles.css` & `JupyterQuiz-2.3.0/jupyterquiz/styles.css`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     margin-left: auto;
     margin-right: auto;
     margin-bottom: 15px;
     padding-bottom: 4px;
     padding-top: 4px;
     line-height: 1.1;
     font-size: 16pt;
+    border-radius: inherit;
 }
 
 .QuizCode {
     font-size: 14pt;
     margin-top: 10px;
     margin-left: 20px;
     margin-right: 20px;
@@ -30,16 +31,17 @@
 .QuizCode>pre {
     padding: 4px;
 }
 
 .Answer {
     margin: 10px 0;
     display: grid;
-    grid-template-columns: auto auto;
+    grid-template-columns: 1fr 1fr;
     grid-gap: 10px;
+    border-radius: inherit;
 }
 
 .Feedback {
     font-size: 16pt;
     text-align: center;
     min-height: 2em;
 }
@@ -72,44 +74,47 @@
     background-color: #c0c0c0;
     box-shadow: 0.6rem 0.8rem 1.4rem -0.5rem #999999;
 }
 
 .MCButton {
     background: #fafafa;
     border: 1px solid #eee;
-    border-radius: 10px;
+    border-radius: inherit;
     padding: 10px;
     font-size: 16px;
     cursor: pointer;
     text-align: center;
+    display: flex;
+    align-items: center;
+    justify-content: center;
 }
 
 .MCButton p {
     color: inherit;
 }
 
 .MultipleChoiceQn {
     padding: 10px;
     background: var(--medium-slate-blue);
     color: #fafafa;
-    border-radius: 10px;
+    border-radius: inherit;
 }
 
 .ManyChoiceQn {
     padding: 10px;
     background: var(--orange-pantone);
     color: #fafafa;
-    border-radius: 10px;
+    border-radius: inherit;
 }
 
 .NumericQn {
     padding: 10px;
     background: var(--russian-violet);
     color: #fafafa;
-    border-radius: 10px;
+    border-radius: inherit;
 }
 
 .NumericQn p {
     color: inherit;
 }
 
 .InpLabel {
@@ -153,8 +158,8 @@
     }
 }
 
 @keyframes correct-anim {
     100% {
         background-color: var(--correct-green);
     }
-}
+}
```

### Comparing `JupyterQuiz-2.2.0/preserve-responses.ipynb` & `JupyterQuiz-2.3.0/preserve-responses.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/previews/github-preview.png` & `JupyterQuiz-2.3.0/previews/github-preview.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/previews/github-preview.psd` & `JupyterQuiz-2.3.0/previews/github-preview.psd`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/schema/mc_schema.json` & `JupyterQuiz-2.3.0/schema/mc_schema.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8359375%*

 * *Differences: {"'properties'": "{'answers': {replace: OrderedDict([('type', 'array'), ('items', "*

 * *                 "OrderedDict([('type', 'object'), ('properties', OrderedDict([('answer', "*

 * *                 "OrderedDict([('type', 'string')])), ('correct', OrderedDict([('type', "*

 * *                 "'boolean')])), ('feedback', OrderedDict([('type', 'string')])), ('answer_cols', "*

 * *                 "OrderedDict([('type', 'number')]))])), ('required', ['answer', "*

 * *                 "'correct'])]))])}}",*

 * * "'required'": "{insert: […]*

```diff
@@ -1,52 +1,48 @@
 {
     "$id": "https://github.com/jmshea/jupyterquiz/mc_schema.json",
     "$schema": "https://json-schema.org/draft/2020-12/schema",
-    "definitions": {
-        "answerlist": {
+    "description": "Schema for Multiple or Many Choice Questions in JupyterQuiz",
+    "properties": {
+        "answers": {
             "items": {
                 "properties": {
-                    "answer (+)": {
+                    "answer": {
                         "type": "string"
                     },
-                    "code (+)": {
-                        "type": "string"
+                    "answer_cols": {
+                        "type": "number"
                     },
                     "correct": {
                         "type": "boolean"
                     },
                     "feedback": {
                         "type": "string"
                     }
                 },
                 "required": [
+                    "answer",
                     "correct"
                 ],
                 "type": "object"
             },
             "type": "array"
-        }
-    },
-    "description": "Schema for Multiple or Many Choice Questions in JupyterQuiz",
-    "properties": {
-        "answers": {
-            "$ref": "#/definitions/answerlist"
         },
         "code": {
             "type": "string"
         },
         "question": {
             "type": "string"
         },
         "type": {
             "pattern": "multiple_choice|many_choice",
             "type": "string"
         }
     },
     "required": [
-        "question",
         "type",
+        "question",
         "answers"
     ],
     "title": "JupyterQuiz Multiple or Many Choice Quiz",
     "type": "object"
 }
```

### Comparing `JupyterQuiz-2.2.0/schema/num_schema.json` & `JupyterQuiz-2.3.0/schema/num_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/schema/num_schema.png` & `JupyterQuiz-2.3.0/schema/num_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.2.0/schema/schema.ipynb` & `JupyterQuiz-2.3.0/schema/schema.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888762111544369%*

 * *Differences: {"'cells'": "{2: {'metadata': {replace: OrderedDict([('user_expressions', [])])}}, 4: "*

 * *            "{'execution_count': 6, 'source': {insert: [(17, '                     "*

 * *            '"feedback": {"type": "string"},\\n\'), (18, \'                     "answer_cols": '*

 * *            '{"type": "number"}\\n\')], delete: [17]}}, 5: {\'execution_count\': 7}, 6: '*

 * *            "{'execution_count': 8}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': "*

 * *               "{'ver […]*

```diff
@@ -21,15 +21,17 @@
                 "with open(\"../examples/questions.json\", \"r\") as file:\n",
                 "    questions=json.load(file)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c539a78f",
-            "metadata": {},
+            "metadata": {
+                "user_expressions": []
+            },
             "source": [
                 "# Schema for Multiple Choice Questions"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
@@ -62,15 +64,15 @@
             "source": [
                 "multiple_choice=questions[0]\n",
                 "multiple_choice"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 6,
             "id": "885e0c61",
             "metadata": {},
             "outputs": [],
             "source": [
                 "mc_schema={\n",
                 "  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n",
                 "  \"$id\": \"https://github.com/jmshea/jupyterquiz/mc_schema.json\",\n",
@@ -84,15 +86,16 @@
                 "                  \"pattern\": \"multiple_choice|many_choice\"},\n",
                 "      \"answers\": {\"type\": \"array\",\n",
                 "                 \"items\":{\n",
                 "                     \"type\": \"object\",\n",
                 "                     \"properties\": {\n",
                 "                     \"answer\": {\"type\": \"string\"},\n",
                 "                     \"correct\": {\"type\": \"boolean\"},\n",
-                "                     \"feedback\": {\"type\": \"string\"}\n",
+                "                     \"feedback\": {\"type\": \"string\"},\n",
+                "                     \"answer_cols\": {\"type\": \"number\"}\n",
                 "                     },\n",
                 "                     \"required\": [\"answer\", \"correct\"]\n",
                 "                 }\n",
                 "                 },\n",
                 "      \"code\": {\"type\":\"string\"}\n",
                 "  },\n",
                 "  \"required\": [\"type\", \"question\", \"answers\"]\n",
@@ -100,25 +103,25 @@
                 "\n",
                 "\n",
                 "}"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 7,
             "id": "84dea887",
             "metadata": {},
             "outputs": [],
             "source": [
                 "validate(multiple_choice, mc_schema)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "id": "a320d6fb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "with open(\"mc_schema.json\", \"w\") as file:\n",
                 "    json.dump(mc_schema, file, indent=4)"
             ]
@@ -254,27 +257,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.4"
+            "version": "3.9.15"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `JupyterQuiz-2.2.0/PKG-INFO` & `JupyterQuiz-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterQuiz
-Version: 2.2.0
+Version: 2.3.0
 Summary: Interactive quizzes for Jupyter and Jupyter Book
 Author-email: "John M. Shea" <jshea@ieee.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: home-page, https://github.com/jmshea/jupyterquiz
 
 # JupyterQuiz
```

