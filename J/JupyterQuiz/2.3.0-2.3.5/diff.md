# Comparing `tmp/JupyterQuiz-2.3.0.tar.gz` & `tmp/JupyterQuiz-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterQuiz-2.3.0.tar", last modified: Fri Apr 21 13:05:20 2023, max compression
+gzip compressed data, was "JupyterQuiz-2.3.5.tar", last modified: Fri Apr 21 18:17:59 2023, max compression
```

## Comparing `JupyterQuiz-2.3.0.tar` & `JupyterQuiz-2.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 JupyterQuiz-2.3.0/.gitignore
--rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.3.0/CITATION.cff
--rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.3.0/HideQuiz.ipynb
--rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.3.0/LICENSE
--rw-r--r--   0        0        0     8860 2023-03-11 13:44:15.891925 JupyterQuiz-2.3.0/README.md
--rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.3.0/examples/mc-example.gif
--rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.3.0/examples/num-example.gif
--rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.3.0/examples/questions.json
--rw-r--r--   0        0        0      661 2023-04-21 13:03:20.531584 JupyterQuiz-2.3.0/jupyterquiz/__init__.py
--rw-r--r--   0        0        0     7468 2023-04-21 12:54:08.754441 JupyterQuiz-2.3.0/jupyterquiz/dynamic.py
--rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.3.0/jupyterquiz/helpers.js
--rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.js
--rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.py
--rw-r--r--   0        0        0     7570 2022-08-22 19:45:35.870224 JupyterQuiz-2.3.0/jupyterquiz/numeric.js
--rw-r--r--   0        0        0     6034 2023-04-21 12:37:51.040441 JupyterQuiz-2.3.0/jupyterquiz/show_questions.js
--rw-r--r--   0        0        0     2902 2023-04-21 13:01:28.819811 JupyterQuiz-2.3.0/jupyterquiz/styles.css
--rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.3.0/preserve-responses.ipynb
--rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.3.0/previews/github-preview.png
--rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.3.0/previews/github-preview.psd
--rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.3.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 JupyterQuiz-2.3.0/schema/README
--rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 JupyterQuiz-2.3.0/schema/mc_schema.json
--rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 JupyterQuiz-2.3.0/schema/mc_schema.png
--rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 JupyterQuiz-2.3.0/schema/mc_schema.svg
--rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.3.0/schema/num_schema.json
--rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.3.0/schema/num_schema.png
--rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 JupyterQuiz-2.3.0/schema/schema.ipynb
--rw-r--r--   0        0        0   281731 2023-04-21 13:02:56.982731 JupyterQuiz-2.3.0/test.ipynb
--rw-r--r--   0        0        0     9174 1970-01-01 00:00:00.000000 JupyterQuiz-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 JupyterQuiz-2.3.5/.gitignore
+-rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.3.5/CITATION.cff
+-rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.3.5/HideQuiz.ipynb
+-rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.3.5/LICENSE
+-rw-r--r--   0        0        0     8860 2023-03-11 13:44:15.891925 JupyterQuiz-2.3.5/README.md
+-rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.3.5/examples/mc-example.gif
+-rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.3.5/examples/num-example.gif
+-rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.3.5/examples/questions.json
+-rw-r--r--   0        0        0      661 2023-04-21 18:17:41.225287 JupyterQuiz-2.3.5/jupyterquiz/__init__.py
+-rw-r--r--   0        0        0     7860 2023-04-21 15:40:51.461908 JupyterQuiz-2.3.5/jupyterquiz/dynamic.py
+-rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.3.5/jupyterquiz/helpers.js
+-rw-r--r--   0        0        0     9336 2022-07-26 16:35:36.994541 JupyterQuiz-2.3.5/jupyterquiz/multiple_choice.js
+-rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.3.5/jupyterquiz/multiple_choice.py
+-rw-r--r--   0        0        0     7570 2022-08-22 19:45:35.870224 JupyterQuiz-2.3.5/jupyterquiz/numeric.js
+-rw-r--r--   0        0        0     6123 2023-04-21 17:58:09.064320 JupyterQuiz-2.3.5/jupyterquiz/show_questions.js
+-rw-r--r--   0        0        0     2902 2023-04-21 15:09:09.190075 JupyterQuiz-2.3.5/jupyterquiz/styles.css
+-rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.3.5/preserve-responses.ipynb
+-rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.3.5/previews/github-preview.png
+-rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.3.5/previews/github-preview.psd
+-rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.3.5/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 JupyterQuiz-2.3.5/schema/README
+-rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 JupyterQuiz-2.3.5/schema/mc_schema.json
+-rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 JupyterQuiz-2.3.5/schema/mc_schema.png
+-rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 JupyterQuiz-2.3.5/schema/mc_schema.svg
+-rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.3.5/schema/num_schema.json
+-rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.3.5/schema/num_schema.png
+-rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 JupyterQuiz-2.3.5/schema/schema.ipynb
+-rw-r--r--   0        0        0   243037 2023-04-21 18:17:04.467150 JupyterQuiz-2.3.5/test.ipynb
+-rw-r--r--   0        0        0     9174 1970-01-01 00:00:00.000000 JupyterQuiz-2.3.5/PKG-INFO
```

### Comparing `JupyterQuiz-2.3.0/.gitignore` & `JupyterQuiz-2.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/HideQuiz.ipynb` & `JupyterQuiz-2.3.5/HideQuiz.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/LICENSE` & `JupyterQuiz-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/README.md` & `JupyterQuiz-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/examples/mc-example.gif` & `JupyterQuiz-2.3.5/examples/mc-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/examples/num-example.gif` & `JupyterQuiz-2.3.5/examples/num-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/examples/questions.json` & `JupyterQuiz-2.3.5/examples/questions.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/__init__.py` & `JupyterQuiz-2.3.5/jupyterquiz/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.3.0'
+__version__ = '2.3.5'
 from .dynamic import display_quiz, capture_responses
```

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/dynamic.py` & `JupyterQuiz-2.3.5/jupyterquiz/dynamic.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import urllib.request
 import urllib
 import json
 import sys
 
 
 def display_quiz(ref, num=1_000_000, shuffle_questions=False, shuffle_answers=True, preserve_responses=False,
-                 border_radius=10):
+                 border_radius=10, question_alignment="left", max_width=600):
     '''
     Display an interactive quiz (currently multiple-choice or numeric answer)
     using a mix of Python and Javascript to support use in rendered notebooks
     (especially JupyterBook, but also Voila)
 
     Inputs:
     ref = string, reference to quiz JSON, may be:
@@ -29,22 +29,29 @@
 
     shuffle_answers = boolean, whether to shuffle answers for multiple-choice questions (default True)
     
     preserve_responses = boolean, whether to output the user responses in a way that is preserved upon reload of the notebook (default False)
 
     border_radius = border radius property for all buttons and questions, in pixels (default 10)
 
+    question_alignment = string, alignment of question text (default "left")
+
+    max_width= number, display width of question in pixels
+
     John  M. Shea
     9/26/2021
     '''
 
     assert not (shuffle_questions and preserve_responses), \
         "This package does not support preserving responses if questions are shuffled."
     assert num==1_000_000 or (not preserve_responses), \
         "This package does not support preserving responses when num is set because num changes the order of questions"
+    assert question_alignment in ['left', 'right', 'center'], \
+        "question_alignment must be 'left', 'center', or 'right'"
+
 
     resource_package = __name__
     package = resource_package.split('.')[0]
 
     letters = string.ascii_letters
     div_id = ''.join(random.choice(letters) for i in range(12))
     #print(div_id)
@@ -56,15 +63,16 @@
 
 
 
     mydiv = f"""<div id="{div_id}" data-shufflequestions="{str(shuffle_questions)}"
                data-shuffleanswers="{str(shuffle_answers)}"
                data-preserveresponses="{preserve_json}"
                data-numquestions="{str(num)}"
-               style="border-radius: {str(border_radius)}px;"> """
+               data-maxwidth="{str(max_width)}"
+               style="border-radius: {str(border_radius)}px; text-align: {question_alignment}"> """
     #print(mydiv)
 
     styles = "<style>"
     f = importlib.resources.files(package).joinpath('styles.css')
     css = f.read_bytes()
     styles += css.decode("utf-8")
     styles += "</style>"
```

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/helpers.js` & `JupyterQuiz-2.3.5/jupyterquiz/helpers.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.js` & `JupyterQuiz-2.3.5/jupyterquiz/multiple_choice.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/multiple_choice.py` & `JupyterQuiz-2.3.5/jupyterquiz/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/numeric.js` & `JupyterQuiz-2.3.5/jupyterquiz/numeric.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/show_questions.js` & `JupyterQuiz-2.3.5/jupyterquiz/show_questions.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -39,14 +39,15 @@
 
 function show_questions(json, mydiv) {
     console.log('show_questions');
     //var mydiv=document.getElementById(myid);
     var shuffle_questions = mydiv.dataset.shufflequestions;
     var num_questions = mydiv.dataset.numquestions;
     var shuffle_answers = mydiv.dataset.shuffleanswers;
+    var max_width = mydiv.dataset.maxwidth;
 
     if (num_questions > json.length) {
         num_questions = json.length;
     }
 
     var questions;
     if ((num_questions < json.length) || (shuffle_questions == "True")) {
@@ -68,17 +69,17 @@
 
         // Create Div to contain question and answers
         var iDiv = document.createElement('div');
         //iDiv.id = 'quizWrap' + id + index;
         iDiv.id = 'quizWrap' + id;
         iDiv.className = 'Quiz';
         iDiv.setAttribute('data-qnum', index);
+        iDiv.style.maxWidth = max_width + "px";
         mydiv.appendChild(iDiv);
         // iDiv.innerHTML=qa.question;
-
         var outerqDiv = document.createElement('div');
         outerqDiv.id = "OuterquizQn" + id + index;
 
         iDiv.append(outerqDiv);
 
         // Create div to contain question part
         var qDiv = document.createElement('div');
```

### Comparing `JupyterQuiz-2.3.0/jupyterquiz/styles.css` & `JupyterQuiz-2.3.5/jupyterquiz/styles.css`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/preserve-responses.ipynb` & `JupyterQuiz-2.3.5/preserve-responses.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/previews/github-preview.png` & `JupyterQuiz-2.3.5/previews/github-preview.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/previews/github-preview.psd` & `JupyterQuiz-2.3.5/previews/github-preview.psd`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/schema/mc_schema.json` & `JupyterQuiz-2.3.5/schema/mc_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/schema/mc_schema.png` & `JupyterQuiz-2.3.5/schema/mc_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/schema/mc_schema.svg` & `JupyterQuiz-2.3.5/schema/mc_schema.svg`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/schema/num_schema.json` & `JupyterQuiz-2.3.5/schema/num_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/schema/num_schema.png` & `JupyterQuiz-2.3.5/schema/num_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/schema/schema.ipynb` & `JupyterQuiz-2.3.5/schema/schema.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.3.0/test.ipynb` & `JupyterQuiz-2.3.5/test.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9961232316647899%*

 * *Differences: {"'cells'": "{3: {'outputs': {0: {'data': {'text/html': {insert: [(0, '<div "*

 * *            'id="GnGFNpmYHnTT" data-shufflequestions="False"\\n\'), (4, \'               '*

 * *            'data-maxwidth="600"\\n\'), (5, \'               style="border-radius: 10px; '*

 * *            'text-align: left"> <style>:root {\\n\')], delete: [4, 0]}}}, 1: {\'data\': '*

 * *            "{'application/javascript': {insert: [(0, 'var questionsGnGFNpmYHnTT=[\\n'), (833, "*

 * *            "'    var max_width = mydiv.dataset.maxwidth;\\n'), ( […]*

```diff
@@ -46,19 +46,20 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"PnIRFNQeqcwN\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"GnGFNpmYHnTT\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
-                            "               style=\"border-radius: 10px;\"> <style>:root {\n",
+                            "               data-maxwidth=\"600\"\n",
+                            "               style=\"border-radius: 10px; text-align: left\"> <style>:root {\n",
                             "    --medium-slate-blue: #6f78ffff;\n",
                             "    --orange-pantone: #f75c03ff;\n",
                             "    --russian-violet: #392061ff;\n",
                             "    --maximum-yellow-red: #ffc857ff;\n",
                             "    --viridian-green: #119da4ff;\n",
                             "    --incorrect-red: #c80202;\n",
                             "    --correct-green: #009113;\n",
@@ -227,15 +228,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsPnIRFNQeqcwN=[\n",
+                            "var questionsGnGFNpmYHnTT=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -1060,14 +1061,15 @@
                             "\n",
                             "function show_questions(json, mydiv) {\n",
                             "    console.log('show_questions');\n",
                             "    //var mydiv=document.getElementById(myid);\n",
                             "    var shuffle_questions = mydiv.dataset.shufflequestions;\n",
                             "    var num_questions = mydiv.dataset.numquestions;\n",
                             "    var shuffle_answers = mydiv.dataset.shuffleanswers;\n",
+                            "    var max_width = mydiv.dataset.maxwidth;\n",
                             "\n",
                             "    if (num_questions > json.length) {\n",
                             "        num_questions = json.length;\n",
                             "    }\n",
                             "\n",
                             "    var questions;\n",
                             "    if ((num_questions < json.length) || (shuffle_questions == \"True\")) {\n",
@@ -1089,17 +1091,17 @@
                             "\n",
                             "        // Create Div to contain question and answers\n",
                             "        var iDiv = document.createElement('div');\n",
                             "        //iDiv.id = 'quizWrap' + id + index;\n",
                             "        iDiv.id = 'quizWrap' + id;\n",
                             "        iDiv.className = 'Quiz';\n",
                             "        iDiv.setAttribute('data-qnum', index);\n",
+                            "        iDiv.style.maxWidth  =max_width+\"px\";\n",
                             "        mydiv.appendChild(iDiv);\n",
                             "        // iDiv.innerHTML=qa.question;\n",
-                            "\n",
                             "        var outerqDiv = document.createElement('div');\n",
                             "        outerqDiv.id = \"OuterquizQn\" + id + index;\n",
                             "\n",
                             "        iDiv.append(outerqDiv);\n",
                             "\n",
                             "        // Create div to contain question part\n",
                             "        var qDiv = document.createElement('div');\n",
@@ -1207,18 +1209,18 @@
                             "        const jmscontroller = new AbortController();\n",
                             "        const signal = jmscontroller.signal;\n",
                             "\n",
                             "        setTimeout(() => jmscontroller.abort(), 5000);\n",
                             "\n",
                             "        fetch(\"https://raw.githubusercontent.com/jmshea/jupyterquiz/main/examples/questions.json\", {signal})\n",
                             "        .then(response => response.json())\n",
-                            "        .then(json => show_questions(json, PnIRFNQeqcwN))\n",
+                            "        .then(json => show_questions(json, GnGFNpmYHnTT))\n",
                             "        .catch(err => {\n",
                             "        console.log(\"Fetch error or timeout\");\n",
-                            "        show_questions(questionsPnIRFNQeqcwN, PnIRFNQeqcwN);\n",
+                            "        show_questions(questionsGnGFNpmYHnTT, GnGFNpmYHnTT);\n",
                             "        });\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
@@ -1244,19 +1246,20 @@
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"JyIhVTgccWPZ\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"pYEuIhJHgtdK\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
-                            "               style=\"border-radius: 10px;\"> <style>:root {\n",
+                            "               data-maxwidth=\"600\"\n",
+                            "               style=\"border-radius: 10px; text-align: left\"> <style>:root {\n",
                             "    --medium-slate-blue: #6f78ffff;\n",
                             "    --orange-pantone: #f75c03ff;\n",
                             "    --russian-violet: #392061ff;\n",
                             "    --maximum-yellow-red: #ffc857ff;\n",
                             "    --viridian-green: #119da4ff;\n",
                             "    --incorrect-red: #c80202;\n",
                             "    --correct-green: #009113;\n",
@@ -1425,15 +1428,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsJyIhVTgccWPZ=[\n",
+                            "var questionspYEuIhJHgtdK=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -2258,14 +2261,15 @@
                             "\n",
                             "function show_questions(json, mydiv) {\n",
                             "    console.log('show_questions');\n",
                             "    //var mydiv=document.getElementById(myid);\n",
                             "    var shuffle_questions = mydiv.dataset.shufflequestions;\n",
                             "    var num_questions = mydiv.dataset.numquestions;\n",
                             "    var shuffle_answers = mydiv.dataset.shuffleanswers;\n",
+                            "    var max_width = mydiv.dataset.maxwidth;\n",
                             "\n",
                             "    if (num_questions > json.length) {\n",
                             "        num_questions = json.length;\n",
                             "    }\n",
                             "\n",
                             "    var questions;\n",
                             "    if ((num_questions < json.length) || (shuffle_questions == \"True\")) {\n",
@@ -2287,17 +2291,17 @@
                             "\n",
                             "        // Create Div to contain question and answers\n",
                             "        var iDiv = document.createElement('div');\n",
                             "        //iDiv.id = 'quizWrap' + id + index;\n",
                             "        iDiv.id = 'quizWrap' + id;\n",
                             "        iDiv.className = 'Quiz';\n",
                             "        iDiv.setAttribute('data-qnum', index);\n",
+                            "        iDiv.style.maxWidth  =max_width+\"px\";\n",
                             "        mydiv.appendChild(iDiv);\n",
                             "        // iDiv.innerHTML=qa.question;\n",
-                            "\n",
                             "        var outerqDiv = document.createElement('div');\n",
                             "        outerqDiv.id = \"OuterquizQn\" + id + index;\n",
                             "\n",
                             "        iDiv.append(outerqDiv);\n",
                             "\n",
                             "        // Create div to contain question part\n",
                             "        var qDiv = document.createElement('div');\n",
@@ -2397,15 +2401,15 @@
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
                             "\n",
                             "        {\n",
-                            "        show_questions(questionsJyIhVTgccWPZ,  JyIhVTgccWPZ);\n",
+                            "        show_questions(questionspYEuIhJHgtdK,  pYEuIhJHgtdK);\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
                     },
@@ -2430,19 +2434,20 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"nUxcSRqYHIXP\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"tdRhUIJLsxzg\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
-                            "               style=\"border-radius: 10px;\"> <style>:root {\n",
+                            "               data-maxwidth=\"600\"\n",
+                            "               style=\"border-radius: 0px; text-align: left\"> <style>:root {\n",
                             "    --medium-slate-blue: #6f78ffff;\n",
                             "    --orange-pantone: #f75c03ff;\n",
                             "    --russian-violet: #392061ff;\n",
                             "    --maximum-yellow-red: #ffc857ff;\n",
                             "    --viridian-green: #119da4ff;\n",
                             "    --incorrect-red: #c80202;\n",
                             "    --correct-green: #009113;\n",
@@ -2611,15 +2616,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsnUxcSRqYHIXP=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Testing parameter to change number of colums for answers: Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answer_cols\": 4, \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"precision\": 2, \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Determine the output of the following Python code:\", \"code\": \"a=\\\"1\\\"\\nb=\\\"2\\\"\\nprint(a+b)\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"1\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"2\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"12\", \"correct\": true, \"feedback\": \"Yes. The + operator will concatenate the strings \\\"1\\\" and \\\"2\\\".\"}, {\"answer\": \"error\", \"correct\": false, \"feedback\": \"No. The + operator for strings performs string concatenation.\"}]}, {\"question\": \"The variable mylist is a Python list. Choose which code snippet will append the item 3 to mylist.\", \"type\": \"multiple_choice\", \"answers\": [{\"code\": \"mylist+=3\", \"correct\": false}, {\"code\": \"mylist+=[3]\", \"correct\": true}, {\"code\": \"mylist+={3}\", \"correct\": false}]}, {\"question\": \"Which of these is the ratio of a circle's circumference to its diameter?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"$\\\\pi$\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"$\\\\frac{22}{7}$\", \"correct\": false, \"feedback\": \"$\\\\frac{22}{7}$ is only an approximation to the true value.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"This is a crude approximation to the true value.\"}, {\"answer\": \"$\\\\tau$\", \"correct\": false, \"feedback\": \"True for the ratio of the circle's circumference to its radius, not diameter.\"}]}];\n",
+                            "var questionstdRhUIJLsxzg=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Testing parameter to change number of colums for answers: Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answer_cols\": 4, \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Enter the value of $\\\\pi$ to 2 decimal places.\", \"type\": \"numeric\", \"precision\": 2, \"answers\": [{\"type\": \"value\", \"value\": 3.14, \"correct\": true, \"feedback\": \"Correct.\"}, {\"type\": \"range\", \"range\": [3.142857, 3.142858], \"correct\": true, \"feedback\": \"True to 2 decimal places, but you know $\\\\pi$ is not really 22/7, right?\"}, {\"type\": \"range\", \"range\": [-100000000, 0], \"correct\": false, \"feedback\": \"$\\\\pi$ is the AREA of a circle of radius 1. Try again.\"}, {\"type\": \"default\", \"feedback\": \"$\\\\pi$ is the area of a circle of radius 1. Try again.\"}]}, {\"question\": \"Determine the output of the following Python code:\", \"code\": \"a=\\\"1\\\"\\nb=\\\"2\\\"\\nprint(a+b)\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"1\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"2\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"No. When strings are operated on by +, they are concatenated.\"}, {\"answer\": \"12\", \"correct\": true, \"feedback\": \"Yes. The + operator will concatenate the strings \\\"1\\\" and \\\"2\\\".\"}, {\"answer\": \"error\", \"correct\": false, \"feedback\": \"No. The + operator for strings performs string concatenation.\"}]}, {\"question\": \"The variable mylist is a Python list. Choose which code snippet will append the item 3 to mylist.\", \"type\": \"multiple_choice\", \"answers\": [{\"code\": \"mylist+=3\", \"correct\": false}, {\"code\": \"mylist+=[3]\", \"correct\": true}, {\"code\": \"mylist+={3}\", \"correct\": false}]}, {\"question\": \"Which of these is the ratio of a circle's circumference to its diameter?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"$\\\\pi$\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"$\\\\frac{22}{7}$\", \"correct\": false, \"feedback\": \"$\\\\frac{22}{7}$ is only an approximation to the true value.\"}, {\"answer\": \"3\", \"correct\": false, \"feedback\": \"This is a crude approximation to the true value.\"}, {\"answer\": \"$\\\\tau$\", \"correct\": false, \"feedback\": \"True for the ratio of the circle's circumference to its radius, not diameter.\"}]}];\n",
                             "    // Make a random ID\n",
                             "function makeid(length) {\n",
                             "    var result = [];\n",
                             "    var characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz';\n",
                             "    var charactersLength = characters.length;\n",
                             "    for (var i = 0; i < length; i++) {\n",
                             "        result.push(characters.charAt(Math.floor(Math.random() * charactersLength)));\n",
@@ -3208,14 +3213,15 @@
                             "\n",
                             "function show_questions(json, mydiv) {\n",
                             "    console.log('show_questions');\n",
                             "    //var mydiv=document.getElementById(myid);\n",
                             "    var shuffle_questions = mydiv.dataset.shufflequestions;\n",
                             "    var num_questions = mydiv.dataset.numquestions;\n",
                             "    var shuffle_answers = mydiv.dataset.shuffleanswers;\n",
+                            "    var max_width = mydiv.dataset.maxwidth;\n",
                             "\n",
                             "    if (num_questions > json.length) {\n",
                             "        num_questions = json.length;\n",
                             "    }\n",
                             "\n",
                             "    var questions;\n",
                             "    if ((num_questions < json.length) || (shuffle_questions == \"True\")) {\n",
@@ -3237,17 +3243,17 @@
                             "\n",
                             "        // Create Div to contain question and answers\n",
                             "        var iDiv = document.createElement('div');\n",
                             "        //iDiv.id = 'quizWrap' + id + index;\n",
                             "        iDiv.id = 'quizWrap' + id;\n",
                             "        iDiv.className = 'Quiz';\n",
                             "        iDiv.setAttribute('data-qnum', index);\n",
+                            "        iDiv.style.maxWidth  =max_width+\"px\";\n",
                             "        mydiv.appendChild(iDiv);\n",
                             "        // iDiv.innerHTML=qa.question;\n",
-                            "\n",
                             "        var outerqDiv = document.createElement('div');\n",
                             "        outerqDiv.id = \"OuterquizQn\" + id + index;\n",
                             "\n",
                             "        iDiv.append(outerqDiv);\n",
                             "\n",
                             "        // Create div to contain question part\n",
                             "        var qDiv = document.createElement('div');\n",
@@ -3347,15 +3353,15 @@
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
                             "\n",
                             "        {\n",
-                            "        show_questions(questionsnUxcSRqYHIXP,  nUxcSRqYHIXP);\n",
+                            "        show_questions(questionstdRhUIJLsxzg,  tdRhUIJLsxzg);\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
                     },
@@ -3364,15 +3370,15 @@
                 }
             ],
             "source": [
                 "import json\n",
                 "with open(\"examples/questions.json\", \"r\") as file:\n",
                 "    questions=json.load(file)\n",
                 "    \n",
-                "display_quiz(questions)"
+                "display_quiz(questions,  border_radius=0)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
@@ -3397,19 +3403,20 @@
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"RJHvAkeiZKMg\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"PpcjihMETkKm\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"2\"\n",
-                            "               style=\"border-radius: 10px;\"> <style>:root {\n",
+                            "               data-maxwidth=\"600\"\n",
+                            "               style=\"border-radius: 10px; text-align: left\"> <style>:root {\n",
                             "    --medium-slate-blue: #6f78ffff;\n",
                             "    --orange-pantone: #f75c03ff;\n",
                             "    --russian-violet: #392061ff;\n",
                             "    --maximum-yellow-red: #ffc857ff;\n",
                             "    --viridian-green: #119da4ff;\n",
                             "    --incorrect-red: #c80202;\n",
                             "    --correct-green: #009113;\n",
@@ -3578,15 +3585,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsRJHvAkeiZKMg=[\n",
+                            "var questionsPpcjihMETkKm=[\n",
                             "    {\n",
                             "        \"question\": \"Choose all of the following that can be included in Jupyter notebooks?\",\n",
                             "        \"type\": \"many_choice\",\n",
                             "        \"answers\": [\n",
                             "            {\n",
                             "                \"answer\": \"Text and graphics output from Python\",\n",
                             "                \"correct\": true,\n",
@@ -4411,14 +4418,15 @@
                             "\n",
                             "function show_questions(json, mydiv) {\n",
                             "    console.log('show_questions');\n",
                             "    //var mydiv=document.getElementById(myid);\n",
                             "    var shuffle_questions = mydiv.dataset.shufflequestions;\n",
                             "    var num_questions = mydiv.dataset.numquestions;\n",
                             "    var shuffle_answers = mydiv.dataset.shuffleanswers;\n",
+                            "    var max_width = mydiv.dataset.maxwidth;\n",
                             "\n",
                             "    if (num_questions > json.length) {\n",
                             "        num_questions = json.length;\n",
                             "    }\n",
                             "\n",
                             "    var questions;\n",
                             "    if ((num_questions < json.length) || (shuffle_questions == \"True\")) {\n",
@@ -4440,17 +4448,17 @@
                             "\n",
                             "        // Create Div to contain question and answers\n",
                             "        var iDiv = document.createElement('div');\n",
                             "        //iDiv.id = 'quizWrap' + id + index;\n",
                             "        iDiv.id = 'quizWrap' + id;\n",
                             "        iDiv.className = 'Quiz';\n",
                             "        iDiv.setAttribute('data-qnum', index);\n",
+                            "        iDiv.style.maxWidth  =max_width+\"px\";\n",
                             "        mydiv.appendChild(iDiv);\n",
                             "        // iDiv.innerHTML=qa.question;\n",
-                            "\n",
                             "        var outerqDiv = document.createElement('div');\n",
                             "        outerqDiv.id = \"OuterquizQn\" + id + index;\n",
                             "\n",
                             "        iDiv.append(outerqDiv);\n",
                             "\n",
                             "        // Create div to contain question part\n",
                             "        var qDiv = document.createElement('div');\n",
@@ -4558,18 +4566,18 @@
                             "        const jmscontroller = new AbortController();\n",
                             "        const signal = jmscontroller.signal;\n",
                             "\n",
                             "        setTimeout(() => jmscontroller.abort(), 5000);\n",
                             "\n",
                             "        fetch(\"https://raw.githubusercontent.com/jmshea/jupyterquiz/main/examples/questions.json\", {signal})\n",
                             "        .then(response => response.json())\n",
-                            "        .then(json => show_questions(json, RJHvAkeiZKMg))\n",
+                            "        .then(json => show_questions(json, PpcjihMETkKm))\n",
                             "        .catch(err => {\n",
                             "        console.log(\"Fetch error or timeout\");\n",
-                            "        show_questions(questionsRJHvAkeiZKMg, RJHvAkeiZKMg);\n",
+                            "        show_questions(questionsPpcjihMETkKm, PpcjihMETkKm);\n",
                             "        });\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
@@ -4595,19 +4603,20 @@
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div id=\"yMgvEsPjEeTh\" data-shufflequestions=\"False\"\n",
+                            "<div id=\"LeCmwPIrqYLh\" data-shufflequestions=\"False\"\n",
                             "               data-shuffleanswers=\"True\"\n",
                             "               data-preserveresponses=\"false\"\n",
                             "               data-numquestions=\"1000000\"\n",
-                            "               style=\"border-radius: 10px;\"> <style>:root {\n",
+                            "               data-maxwidth=\"600\"\n",
+                            "               style=\"border-radius: 10px; text-align: left\"> <style>:root {\n",
                             "    --medium-slate-blue: #6f78ffff;\n",
                             "    --orange-pantone: #f75c03ff;\n",
                             "    --russian-violet: #392061ff;\n",
                             "    --maximum-yellow-red: #ffc857ff;\n",
                             "    --viridian-green: #119da4ff;\n",
                             "    --incorrect-red: #c80202;\n",
                             "    --correct-green: #009113;\n",
@@ -4776,15 +4785,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "application/javascript": [
-                            "var questionsyMgvEsPjEeTh=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}];\n",
+                            "var questionsLeCmwPIrqYLh=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}];\n",
                             "    // Make a random ID\n",
                             "function makeid(length) {\n",
                             "    var result = [];\n",
                             "    var characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz';\n",
                             "    var charactersLength = characters.length;\n",
                             "    for (var i = 0; i < length; i++) {\n",
                             "        result.push(characters.charAt(Math.floor(Math.random() * charactersLength)));\n",
@@ -5373,14 +5382,15 @@
                             "\n",
                             "function show_questions(json, mydiv) {\n",
                             "    console.log('show_questions');\n",
                             "    //var mydiv=document.getElementById(myid);\n",
                             "    var shuffle_questions = mydiv.dataset.shufflequestions;\n",
                             "    var num_questions = mydiv.dataset.numquestions;\n",
                             "    var shuffle_answers = mydiv.dataset.shuffleanswers;\n",
+                            "    var max_width = mydiv.dataset.maxwidth;\n",
                             "\n",
                             "    if (num_questions > json.length) {\n",
                             "        num_questions = json.length;\n",
                             "    }\n",
                             "\n",
                             "    var questions;\n",
                             "    if ((num_questions < json.length) || (shuffle_questions == \"True\")) {\n",
@@ -5402,17 +5412,17 @@
                             "\n",
                             "        // Create Div to contain question and answers\n",
                             "        var iDiv = document.createElement('div');\n",
                             "        //iDiv.id = 'quizWrap' + id + index;\n",
                             "        iDiv.id = 'quizWrap' + id;\n",
                             "        iDiv.className = 'Quiz';\n",
                             "        iDiv.setAttribute('data-qnum', index);\n",
+                            "        iDiv.style.maxWidth  =max_width+\"px\";\n",
                             "        mydiv.appendChild(iDiv);\n",
                             "        // iDiv.innerHTML=qa.question;\n",
-                            "\n",
                             "        var outerqDiv = document.createElement('div');\n",
                             "        outerqDiv.id = \"OuterquizQn\" + id + index;\n",
                             "\n",
                             "        iDiv.append(outerqDiv);\n",
                             "\n",
                             "        // Create div to contain question part\n",
                             "        var qDiv = document.createElement('div');\n",
@@ -5512,15 +5522,15 @@
                             "            }\n",
                             "        }\n",
                             "    }\n",
                             "    return false;\n",
                             "}\n",
                             "\n",
                             "        {\n",
-                            "        show_questions(questionsyMgvEsPjEeTh,  yMgvEsPjEeTh);\n",
+                            "        show_questions(questionsLeCmwPIrqYLh,  LeCmwPIrqYLh);\n",
                             "        }\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.Javascript object>"
                         ]
                     },
@@ -5534,956 +5544,36 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "user_expressions": []
             },
             "source": [
-                "# Test custom border radius"
+                "# Test custom border radius, question alignment, max_width"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/html": [
-                            "<div id=\"QKKRGtQsSyoO\" data-shufflequestions=\"False\"\n",
-                            "               data-shuffleanswers=\"True\"\n",
-                            "               data-preserveresponses=\"false\"\n",
-                            "               data-numquestions=\"1000000\"\n",
-                            "               style=\"border-radius: 0px;\"> <style>:root {\n",
-                            "    --medium-slate-blue: #6f78ffff;\n",
-                            "    --orange-pantone: #f75c03ff;\n",
-                            "    --russian-violet: #392061ff;\n",
-                            "    --maximum-yellow-red: #ffc857ff;\n",
-                            "    --viridian-green: #119da4ff;\n",
-                            "    --incorrect-red: #c80202;\n",
-                            "    --correct-green: #009113;\n",
-                            "}\n",
-                            "\n",
-                            ".Quiz {\n",
-                            "    max-width: 600px;\n",
-                            "    margin-top: 15px;\n",
-                            "    margin-left: auto;\n",
-                            "    margin-right: auto;\n",
-                            "    margin-bottom: 15px;\n",
-                            "    padding-bottom: 4px;\n",
-                            "    padding-top: 4px;\n",
-                            "    line-height: 1.1;\n",
-                            "    font-size: 16pt;\n",
-                            "    border-radius: inherit;\n",
-                            "}\n",
-                            "\n",
-                            ".QuizCode {\n",
-                            "    font-size: 14pt;\n",
-                            "    margin-top: 10px;\n",
-                            "    margin-left: 20px;\n",
-                            "    margin-right: 20px;\n",
-                            "}\n",
-                            "\n",
-                            ".QuizCode>pre {\n",
-                            "    padding: 4px;\n",
-                            "}\n",
-                            "\n",
-                            ".Answer {\n",
-                            "    margin: 10px 0;\n",
-                            "    display: grid;\n",
-                            "    grid-template-columns: 1fr 1fr;\n",
-                            "    grid-gap: 10px;\n",
-                            "    border-radius: inherit;\n",
-                            "}\n",
-                            "\n",
-                            ".Feedback {\n",
-                            "    font-size: 16pt;\n",
-                            "    text-align: center;\n",
-                            "    min-height: 2em;\n",
-                            "}\n",
-                            "\n",
-                            ".Input {\n",
-                            "    align: left;\n",
-                            "    font-size: 20pt;\n",
-                            "}\n",
-                            "\n",
-                            ".Input-text {\n",
-                            "    display: block;\n",
-                            "    margin: 10px;\n",
-                            "    color: inherit;\n",
-                            "    width: 140px;\n",
-                            "    background-color: #c0c0c0;\n",
-                            "    color: #fff;\n",
-                            "    padding: 5px;\n",
-                            "    padding-left: 10px;\n",
-                            "    font-family: inherit;\n",
-                            "    font-size: 20px;\n",
-                            "    font-weight: inherit;\n",
-                            "    line-height: 20pt;\n",
-                            "    border: none;\n",
-                            "    border-radius: 0.2rem;\n",
-                            "    transition: box-shadow 0.1s);\n",
-                            "}\n",
-                            "\n",
-                            ".Input-text:focus {\n",
-                            "    outline: none;\n",
-                            "    background-color: #c0c0c0;\n",
-                            "    box-shadow: 0.6rem 0.8rem 1.4rem -0.5rem #999999;\n",
-                            "}\n",
-                            "\n",
-                            ".MCButton {\n",
-                            "    background: #fafafa;\n",
-                            "    border: 1px solid #eee;\n",
-                            "    border-radius: inherit;\n",
-                            "    padding: 10px;\n",
-                            "    font-size: 16px;\n",
-                            "    cursor: pointer;\n",
-                            "    text-align: center;\n",
-                            "    display: flex;\n",
-                            "    align-items: center;\n",
-                            "    justify-content: center;\n",
-                            "}\n",
-                            "\n",
-                            ".MCButton p {\n",
-                            "    color: inherit;\n",
-                            "}\n",
-                            "\n",
-                            ".MultipleChoiceQn {\n",
-                            "    padding: 10px;\n",
-                            "    background: var(--medium-slate-blue);\n",
-                            "    color: #fafafa;\n",
-                            "    border-radius: inherit;\n",
-                            "}\n",
-                            "\n",
-                            ".ManyChoiceQn {\n",
-                            "    padding: 10px;\n",
-                            "    background: var(--orange-pantone);\n",
-                            "    color: #fafafa;\n",
-                            "    border-radius: inherit;\n",
-                            "}\n",
-                            "\n",
-                            ".NumericQn {\n",
-                            "    padding: 10px;\n",
-                            "    background: var(--russian-violet);\n",
-                            "    color: #fafafa;\n",
-                            "    border-radius: inherit;\n",
-                            "}\n",
-                            "\n",
-                            ".NumericQn p {\n",
-                            "    color: inherit;\n",
-                            "}\n",
-                            "\n",
-                            ".InpLabel {\n",
-                            "    line-height: 34px;\n",
-                            "    float: left;\n",
-                            "    margin-right: 10px;\n",
-                            "    color: #101010;\n",
-                            "    font-size: 15pt;\n",
-                            "}\n",
-                            "\n",
-                            ".incorrect {\n",
-                            "    color: var(--incorrect-red);\n",
-                            "}\n",
-                            "\n",
-                            ".correct {\n",
-                            "    color: var(--correct-green);\n",
-                            "}\n",
-                            "\n",
-                            ".correctButton {\n",
-                            "    /*\n",
-                            "    background: var(--correct-green);\n",
-                            "   */\n",
-                            "    animation: correct-anim 0.6s ease;\n",
-                            "    animation-fill-mode: forwards;\n",
-                            "    color: #fafafa;\n",
-                            "    box-shadow: inset 0px 0px 5px #555555;\n",
-                            "    outline: none;\n",
-                            "}\n",
-                            "\n",
-                            ".incorrectButton {\n",
-                            "    animation: incorrect-anim 0.8s ease;\n",
-                            "    animation-fill-mode: forwards;\n",
-                            "    color: #fafafa;\n",
-                            "    box-shadow: inset 0px 0px 5px #555555;\n",
-                            "    outline: none;\n",
-                            "}\n",
-                            "\n",
-                            "@keyframes incorrect-anim {\n",
-                            "    100% {\n",
-                            "        background-color: var(--incorrect-red);\n",
-                            "    }\n",
-                            "}\n",
-                            "\n",
-                            "@keyframes correct-anim {\n",
-                            "    100% {\n",
-                            "        background-color: var(--correct-green);\n",
-                            "    }\n",
-                            "}\n",
-                            "</style>"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "application/javascript": [
-                            "var questionsQKKRGtQsSyoO=[{\"question\": \"Choose all of the following that can be included in Jupyter notebooks?\", \"type\": \"many_choice\", \"answers\": [{\"answer\": \"Text and graphics output from Python\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Typeset mathematics\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Python executable code\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Formatted text\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Live snakes via Python\", \"correct\": false, \"feedback\": \"I hope not.\"}]}, {\"question\": \"Which of these are used to create formatted text in Jupyter notebooks?\", \"type\": \"multiple_choice\", \"answers\": [{\"answer\": \"Wiki markup\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"SVG\", \"correct\": false, \"feedback\": \"False.\"}, {\"answer\": \"Markdown\", \"correct\": true, \"feedback\": \"Correct.\"}, {\"answer\": \"Rich Text\", \"correct\": false, \"feedback\": \"False.\"}]}];\n",
-                            "    // Make a random ID\n",
-                            "function makeid(length) {\n",
-                            "    var result = [];\n",
-                            "    var characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz';\n",
-                            "    var charactersLength = characters.length;\n",
-                            "    for (var i = 0; i < length; i++) {\n",
-                            "        result.push(characters.charAt(Math.floor(Math.random() * charactersLength)));\n",
-                            "    }\n",
-                            "    return result.join('');\n",
-                            "}\n",
-                            "\n",
-                            "// Choose a random subset of an array. Can also be used to shuffle the array\n",
-                            "function getRandomSubarray(arr, size) {\n",
-                            "    var shuffled = arr.slice(0), i = arr.length, temp, index;\n",
-                            "    while (i--) {\n",
-                            "        index = Math.floor((i + 1) * Math.random());\n",
-                            "        temp = shuffled[index];\n",
-                            "        shuffled[index] = shuffled[i];\n",
-                            "        shuffled[i] = temp;\n",
-                            "    }\n",
-                            "    return shuffled.slice(0, size);\n",
-                            "}\n",
-                            "\n",
-                            "function printResponses(responsesContainer) {\n",
-                            "    var responses=JSON.parse(responsesContainer.dataset.responses);\n",
-                            "    var stringResponses='<B>IMPORTANT!</B>To preserve this answer sequence for submission, when you have finalized your answers: <ol> <li> Copy the text in this cell below \"Answer String\"</li> <li> Double click on the cell directly below the Answer String, labeled \"Replace Me\"</li> <li> Select the whole \"Replace Me\" text</li> <li> Paste in your answer string and press shift-Enter.</li><li>Save the notebook using the save icon or File->Save Notebook menu item</li></ul><br><br><br><b>Answer String:</b><br> ';\n",
-                            "    console.log(responses);\n",
-                            "    responses.forEach((response, index) => {\n",
-                            "        if (response) {\n",
-                            "            console.log(index + ': ' + response);\n",
-                            "            stringResponses+= index + ': ' + response +\"<BR>\";\n",
-                            "        }\n",
-                            "    });\n",
-                            "    responsesContainer.innerHTML=stringResponses;\n",
-                            "}\n",
-                            "function check_mc() {\n",
-                            "    var id = this.id.split('-')[0];\n",
-                            "    //var response = this.id.split('-')[1];\n",
-                            "    //console.log(response);\n",
-                            "    //console.log(\"In check_mc(), id=\"+id);\n",
-                            "    //console.log(event.srcElement.id)           \n",
-                            "    //console.log(event.srcElement.dataset.correct)   \n",
-                            "    //console.log(event.srcElement.dataset.feedback)\n",
-                            "\n",
-                            "    var label = event.srcElement;\n",
-                            "    //console.log(label, label.nodeName);\n",
-                            "    var depth = 0;\n",
-                            "    while ((label.nodeName != \"LABEL\") && (depth < 20)) {\n",
-                            "        label = label.parentElement;\n",
-                            "        console.log(depth, label);\n",
-                            "        depth++;\n",
-                            "    }\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "    var answers = label.parentElement.children;\n",
-                            "\n",
-                            "    //console.log(answers);\n",
-                            "\n",
-                            "\n",
-                            "    // Split behavior based on multiple choice vs many choice:\n",
-                            "    var fb = document.getElementById(\"fb\" + id);\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "    if (fb.dataset.numcorrect == 1) {\n",
-                            "        // What follows is for the saved responses stuff\n",
-                            "        var outerContainer = fb.parentElement.parentElement;\n",
-                            "        var responsesContainer = document.getElementById(\"responses\" + outerContainer.id);\n",
-                            "        if (responsesContainer) {\n",
-                            "            //console.log(responsesContainer);\n",
-                            "            var response = label.firstChild.innerText;\n",
-                            "            if (label.querySelector(\".QuizCode\")){\n",
-                            "                response+= label.querySelector(\".QuizCode\").firstChild.innerText;\n",
-                            "            }\n",
-                            "            console.log(response);\n",
-                            "            //console.log(document.getElementById(\"quizWrap\"+id));\n",
-                            "            var qnum = document.getElementById(\"quizWrap\"+id).dataset.qnum;\n",
-                            "            console.log(\"Question \" + qnum);\n",
-                            "            //console.log(id, \", got numcorrect=\",fb.dataset.numcorrect);\n",
-                            "            var responses=JSON.parse(responsesContainer.dataset.responses);\n",
-                            "            console.log(responses);\n",
-                            "            responses[qnum]= response;\n",
-                            "            responsesContainer.setAttribute('data-responses', JSON.stringify(responses));\n",
-                            "            printResponses(responsesContainer);\n",
-                            "        }\n",
-                            "        // End code to preserve responses\n",
-                            "        \n",
-                            "        for (var i = 0; i < answers.length; i++) {\n",
-                            "            var child = answers[i];\n",
-                            "            //console.log(child);\n",
-                            "            child.className = \"MCButton\";\n",
-                            "        }\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "        if (label.dataset.correct == \"true\") {\n",
-                            "            // console.log(\"Correct action\");\n",
-                            "            if (\"feedback\" in label.dataset) {\n",
-                            "                fb.textContent = jaxify(label.dataset.feedback);\n",
-                            "            } else {\n",
-                            "                fb.textContent = \"Correct!\";\n",
-                            "            }\n",
-                            "            label.classList.add(\"correctButton\");\n",
-                            "\n",
-                            "            fb.className = \"Feedback\";\n",
-                            "            fb.classList.add(\"correct\");\n",
-                            "\n",
-                            "        } else {\n",
-                            "            if (\"feedback\" in label.dataset) {\n",
-                            "                fb.textContent = jaxify(label.dataset.feedback);\n",
-                            "            } else {\n",
-                            "                fb.textContent = \"Incorrect -- try again.\";\n",
-                            "            }\n",
-                            "            //console.log(\"Error action\");\n",
-                            "            label.classList.add(\"incorrectButton\");\n",
-                            "            fb.className = \"Feedback\";\n",
-                            "            fb.classList.add(\"incorrect\");\n",
-                            "        }\n",
-                            "    }\n",
-                            "    else {\n",
-                            "        var reset = false;\n",
-                            "        var feedback;\n",
-                            "         if (label.dataset.correct == \"true\") {\n",
-                            "            if (\"feedback\" in label.dataset) {\n",
-                            "                feedback = jaxify(label.dataset.feedback);\n",
-                            "            } else {\n",
-                            "                feedback = \"Correct!\";\n",
-                            "            }\n",
-                            "            if (label.dataset.answered <= 0) {\n",
-                            "                if (fb.dataset.answeredcorrect < 0) {\n",
-                            "                    fb.dataset.answeredcorrect = 1;\n",
-                            "                    reset = true;\n",
-                            "                } else {\n",
-                            "                    fb.dataset.answeredcorrect++;\n",
-                            "                }\n",
-                            "                if (reset) {\n",
-                            "                    for (var i = 0; i < answers.length; i++) {\n",
-                            "                        var child = answers[i];\n",
-                            "                        child.className = \"MCButton\";\n",
-                            "                        child.dataset.answered = 0;\n",
-                            "                    }\n",
-                            "                }\n",
-                            "                label.classList.add(\"correctButton\");\n",
-                            "                label.dataset.answered = 1;\n",
-                            "                fb.className = \"Feedback\";\n",
-                            "                fb.classList.add(\"correct\");\n",
-                            "\n",
-                            "            }\n",
-                            "        } else {\n",
-                            "            if (\"feedback\" in label.dataset) {\n",
-                            "                feedback = jaxify(label.dataset.feedback);\n",
-                            "            } else {\n",
-                            "                feedback = \"Incorrect -- try again.\";\n",
-                            "            }\n",
-                            "            if (fb.dataset.answeredcorrect > 0) {\n",
-                            "                fb.dataset.answeredcorrect = -1;\n",
-                            "                reset = true;\n",
-                            "            } else {\n",
-                            "                fb.dataset.answeredcorrect--;\n",
-                            "            }\n",
-                            "\n",
-                            "            if (reset) {\n",
-                            "                for (var i = 0; i < answers.length; i++) {\n",
-                            "                    var child = answers[i];\n",
-                            "                    child.className = \"MCButton\";\n",
-                            "                    child.dataset.answered = 0;\n",
-                            "                }\n",
-                            "            }\n",
-                            "            label.classList.add(\"incorrectButton\");\n",
-                            "            fb.className = \"Feedback\";\n",
-                            "            fb.classList.add(\"incorrect\");\n",
-                            "        }\n",
-                            "        // What follows is for the saved responses stuff\n",
-                            "        var outerContainer = fb.parentElement.parentElement;\n",
-                            "        var responsesContainer = document.getElementById(\"responses\" + outerContainer.id);\n",
-                            "        if (responsesContainer) {\n",
-                            "            //console.log(responsesContainer);\n",
-                            "            var response = label.firstChild.innerText;\n",
-                            "            if (label.querySelector(\".QuizCode\")){\n",
-                            "                response+= label.querySelector(\".QuizCode\").firstChild.innerText;\n",
-                            "            }\n",
-                            "            console.log(response);\n",
-                            "            //console.log(document.getElementById(\"quizWrap\"+id));\n",
-                            "            var qnum = document.getElementById(\"quizWrap\"+id).dataset.qnum;\n",
-                            "            console.log(\"Question \" + qnum);\n",
-                            "            //console.log(id, \", got numcorrect=\",fb.dataset.numcorrect);\n",
-                            "            var responses=JSON.parse(responsesContainer.dataset.responses);\n",
-                            "            if (label.dataset.correct == \"true\") {\n",
-                            "                if (typeof(responses[qnum]) == \"object\"){\n",
-                            "                    if (!responses[qnum].includes(response))\n",
-                            "                        responses[qnum].push(response);\n",
-                            "                } else{\n",
-                            "                    responses[qnum]= [ response ];\n",
-                            "                }\n",
-                            "            } else {\n",
-                            "                responses[qnum]= response;\n",
-                            "            }\n",
-                            "            console.log(responses);\n",
-                            "            responsesContainer.setAttribute('data-responses', JSON.stringify(responses));\n",
-                            "            printResponses(responsesContainer);\n",
-                            "        }\n",
-                            "        // End save responses stuff\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "        var numcorrect = fb.dataset.numcorrect;\n",
-                            "        var answeredcorrect = fb.dataset.answeredcorrect;\n",
-                            "        if (answeredcorrect >= 0) {\n",
-                            "            fb.textContent = feedback + \" [\" + answeredcorrect + \"/\" + numcorrect + \"]\";\n",
-                            "        } else {\n",
-                            "            fb.textContent = feedback + \" [\" + 0 + \"/\" + numcorrect + \"]\";\n",
-                            "        }\n",
-                            "\n",
-                            "\n",
-                            "    }\n",
-                            "\n",
-                            "    if (typeof MathJax != 'undefined') {\n",
-                            "        var version = MathJax.version;\n",
-                            "        console.log('MathJax version', version);\n",
-                            "        if (version[0] == \"2\") {\n",
-                            "            MathJax.Hub.Queue([\"Typeset\", MathJax.Hub]);\n",
-                            "        } else if (version[0] == \"3\") {\n",
-                            "            MathJax.typeset([fb]);\n",
-                            "        }\n",
-                            "    } else {\n",
-                            "        console.log('MathJax not detected');\n",
-                            "    }\n",
-                            "\n",
-                            "}\n",
-                            "\n",
-                            "function make_mc(qa, shuffle_answers, outerqDiv, qDiv, aDiv, id) {\n",
-                            "    var shuffled;\n",
-                            "    if (shuffle_answers == \"True\") {\n",
-                            "        //console.log(shuffle_answers+\" read as true\");\n",
-                            "        shuffled = getRandomSubarray(qa.answers, qa.answers.length);\n",
-                            "    } else {\n",
-                            "        //console.log(shuffle_answers+\" read as false\");\n",
-                            "        shuffled = qa.answers;\n",
-                            "    }\n",
-                            "\n",
-                            "\n",
-                            "    var num_correct = 0;\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "    shuffled.forEach((item, index, ans_array) => {\n",
-                            "        //console.log(answer);\n",
-                            "\n",
-                            "        // Make input element\n",
-                            "        var inp = document.createElement(\"input\");\n",
-                            "        inp.type = \"radio\";\n",
-                            "        inp.id = \"quizo\" + id + index;\n",
-                            "        inp.style = \"display:none;\";\n",
-                            "        aDiv.append(inp);\n",
-                            "\n",
-                            "        //Make label for input element\n",
-                            "        var lab = document.createElement(\"label\");\n",
-                            "        lab.className = \"MCButton\";\n",
-                            "        lab.id = id + '-' + index;\n",
-                            "        lab.onclick = check_mc;\n",
-                            "        var aSpan = document.createElement('span');\n",
-                            "        aSpan.classsName = \"\";\n",
-                            "        //qDiv.id=\"quizQn\"+id+index;\n",
-                            "        if (\"answer\" in item) {\n",
-                            "            aSpan.innerHTML = jaxify(item.answer);\n",
-                            "            //aSpan.innerHTML=item.answer;\n",
-                            "        }\n",
-                            "        lab.append(aSpan);\n",
-                            "\n",
-                            "        // Create div for code inside question\n",
-                            "        var codeSpan;\n",
-                            "        if (\"code\" in item) {\n",
-                            "            codeSpan = document.createElement('span');\n",
-                            "            codeSpan.id = \"code\" + id + index;\n",
-                            "            codeSpan.className = \"QuizCode\";\n",
-                            "            var codePre = document.createElement('pre');\n",
-                            "            codeSpan.append(codePre);\n",
-                            "            var codeCode = document.createElement('code');\n",
-                            "            codePre.append(codeCode);\n",
-                            "            codeCode.innerHTML = item.code;\n",
-                            "            lab.append(codeSpan);\n",
-                            "            //console.log(codeSpan);\n",
-                            "        }\n",
-                            "\n",
-                            "        //lab.textContent=item.answer;\n",
-                            "\n",
-                            "        // Set the data attributes for the answer\n",
-                            "        lab.setAttribute('data-correct', item.correct);\n",
-                            "        if (item.correct) {\n",
-                            "            num_correct++;\n",
-                            "        }\n",
-                            "        if (\"feedback\" in item) {\n",
-                            "            lab.setAttribute('data-feedback', item.feedback);\n",
-                            "        }\n",
-                            "        lab.setAttribute('data-answered', 0);\n",
-                            "\n",
-                            "        aDiv.append(lab);\n",
-                            "\n",
-                            "    });\n",
-                            "\n",
-                            "    if (num_correct > 1) {\n",
-                            "        outerqDiv.className = \"ManyChoiceQn\";\n",
-                            "    } else {\n",
-                            "        outerqDiv.className = \"MultipleChoiceQn\";\n",
-                            "    }\n",
-                            "\n",
-                            "    return num_correct;\n",
-                            "\n",
-                            "}\n",
-                            "function check_numeric(ths, event) {\n",
-                            "\n",
-                            "    if (event.keyCode === 13) {\n",
-                            "        ths.blur();\n",
-                            "\n",
-                            "        var id = ths.id.split('-')[0];\n",
-                            "\n",
-                            "        var submission = ths.value;\n",
-                            "        if (submission.indexOf('/') != -1) {\n",
-                            "            var sub_parts = submission.split('/');\n",
-                            "            //console.log(sub_parts);\n",
-                            "            submission = sub_parts[0] / sub_parts[1];\n",
-                            "        }\n",
-                            "        //console.log(\"Reader entered\", submission);\n",
-                            "\n",
-                            "        if (\"precision\" in ths.dataset) {\n",
-                            "            var precision = ths.dataset.precision;\n",
-                            "            // console.log(\"1:\", submission)\n",
-                            "            submission = Math.round((1 * submission + Number.EPSILON) * 10 ** precision) / 10 ** precision;\n",
-                            "            // console.log(\"Rounded to \", submission, \" precision=\", precision  );\n",
-                            "        }\n",
-                            "\n",
-                            "\n",
-                            "        //console.log(\"In check_numeric(), id=\"+id);\n",
-                            "        //console.log(event.srcElement.id)           \n",
-                            "        //console.log(event.srcElement.dataset.feedback)\n",
-                            "\n",
-                            "        var fb = document.getElementById(\"fb\" + id);\n",
-                            "        fb.style.display = \"none\";\n",
-                            "        fb.textContent = \"Incorrect -- try again.\";\n",
-                            "\n",
-                            "        var answers = JSON.parse(ths.dataset.answers);\n",
-                            "        //console.log(answers);\n",
-                            "\n",
-                            "        var defaultFB = \"\";\n",
-                            "        var correct;\n",
-                            "        var done = false;\n",
-                            "        answers.every(answer => {\n",
-                            "            //console.log(answer.type);\n",
-                            "\n",
-                            "            correct = false;\n",
-                            "            // if (answer.type==\"value\"){\n",
-                            "            if ('value' in answer) {\n",
-                            "                if (submission == answer.value) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
-                            "                    correct = answer.correct;\n",
-                            "                    //console.log(answer.correct);\n",
-                            "                    done = true;\n",
-                            "                }\n",
-                            "                // } else if (answer.type==\"range\") {\n",
-                            "            } else if ('range' in answer) {\n",
-                            "                //console.log(answer.range);\n",
-                            "                if ((submission >= answer.range[0]) && (submission < answer.range[1])) {\n",
-                            "                    fb.textContent = jaxify(answer.feedback);\n",
-                            "                    correct = answer.correct;\n",
-                            "                    //console.log(answer.correct);\n",
-                            "                    done = true;\n",
-                            "                }\n",
-                            "            } else if (answer.type == \"default\") {\n",
-                            "                defaultFB = answer.feedback;\n",
-                            "            }\n",
-                            "            if (done) {\n",
-                            "                return false; // Break out of loop if this has been marked correct\n",
-                            "            } else {\n",
-                            "                return true; // Keep looking for case that includes this as a correct answer\n",
-                            "            }\n",
-                            "        });\n",
-                            "\n",
-                            "        if ((!done) && (defaultFB != \"\")) {\n",
-                            "            fb.innerHTML = jaxify(defaultFB);\n",
-                            "            //console.log(\"Default feedback\", defaultFB);\n",
-                            "        }\n",
-                            "\n",
-                            "        fb.style.display = \"block\";\n",
-                            "        if (correct) {\n",
-                            "            ths.className = \"Input-text\";\n",
-                            "            ths.classList.add(\"correctButton\");\n",
-                            "            fb.className = \"Feedback\";\n",
-                            "            fb.classList.add(\"correct\");\n",
-                            "        } else {\n",
-                            "            ths.className = \"Input-text\";\n",
-                            "            ths.classList.add(\"incorrectButton\");\n",
-                            "            fb.className = \"Feedback\";\n",
-                            "            fb.classList.add(\"incorrect\");\n",
-                            "        }\n",
-                            "\n",
-                            "        // What follows is for the saved responses stuff\n",
-                            "        var outerContainer = fb.parentElement.parentElement;\n",
-                            "        var responsesContainer = document.getElementById(\"responses\" + outerContainer.id);\n",
-                            "        if (responsesContainer) {\n",
-                            "            console.log(submission);\n",
-                            "            var qnum = document.getElementById(\"quizWrap\"+id).dataset.qnum;\n",
-                            "            //console.log(\"Question \" + qnum);\n",
-                            "            //console.log(id, \", got numcorrect=\",fb.dataset.numcorrect);\n",
-                            "            var responses=JSON.parse(responsesContainer.dataset.responses);\n",
-                            "            console.log(responses);\n",
-                            "            if (submission == ths.value){\n",
-                            "                responses[qnum]= submission;\n",
-                            "            } else {\n",
-                            "                responses[qnum]= ths.value + \"(\" + submission +\")\";\n",
-                            "            }\n",
-                            "            responsesContainer.setAttribute('data-responses', JSON.stringify(responses));\n",
-                            "            printResponses(responsesContainer);\n",
-                            "        }\n",
-                            "        // End code to preserve responses\n",
-                            "\n",
-                            "        if (typeof MathJax != 'undefined') {\n",
-                            "            var version = MathJax.version;\n",
-                            "            console.log('MathJax version', version);\n",
-                            "            if (version[0] == \"2\") {\n",
-                            "                MathJax.Hub.Queue([\"Typeset\", MathJax.Hub]);\n",
-                            "            } else if (version[0] == \"3\") {\n",
-                            "                MathJax.typeset([fb]);\n",
-                            "            }\n",
-                            "        } else {\n",
-                            "            console.log('MathJax not detected');\n",
-                            "        }\n",
-                            "        return false;\n",
-                            "    }\n",
-                            "\n",
-                            "}\n",
-                            "\n",
-                            "function isValid(el, charC) {\n",
-                            "    //console.log(\"Input char: \", charC);\n",
-                            "    if (charC == 46) {\n",
-                            "        if (el.value.indexOf('.') === -1) {\n",
-                            "            return true;\n",
-                            "        } else if (el.value.indexOf('/') != -1) {\n",
-                            "            var parts = el.value.split('/');\n",
-                            "            if (parts[1].indexOf('.') === -1) {\n",
-                            "                return true;\n",
-                            "            }\n",
-                            "        }\n",
-                            "        else {\n",
-                            "            return false;\n",
-                            "        }\n",
-                            "    } else if (charC == 47) {\n",
-                            "        if (el.value.indexOf('/') === -1) {\n",
-                            "            if ((el.value != \"\") && (el.value != \".\")) {\n",
-                            "                return true;\n",
-                            "            } else {\n",
-                            "                return false;\n",
-                            "            }\n",
-                            "        } else {\n",
-                            "            return false;\n",
-                            "        }\n",
-                            "    } else if (charC == 45) {\n",
-                            "        var edex = el.value.indexOf('e');\n",
-                            "        if (edex == -1) {\n",
-                            "            edex = el.value.indexOf('E');\n",
-                            "        }\n",
-                            "\n",
-                            "        if (el.value == \"\") {\n",
-                            "            return true;\n",
-                            "        } else if (edex == (el.value.length - 1)) { // If just after e or E\n",
-                            "            return true;\n",
-                            "        } else {\n",
-                            "            return false;\n",
-                            "        }\n",
-                            "    } else if (charC == 101) { // \"e\"\n",
-                            "        if ((el.value.indexOf('e') === -1) && (el.value.indexOf('E') === -1) && (el.value.indexOf('/') == -1)) {\n",
-                            "            // Prev symbol must be digit or decimal point:\n",
-                            "            if (el.value.slice(-1).search(/\\d/) >= 0) {\n",
-                            "                return true;\n",
-                            "            } else if (el.value.slice(-1).search(/\\./) >= 0) {\n",
-                            "                return true;\n",
-                            "            } else {\n",
-                            "                return false;\n",
-                            "            }\n",
-                            "        } else {\n",
-                            "            return false;\n",
-                            "        }\n",
-                            "    } else {\n",
-                            "        if (charC > 31 && (charC < 48 || charC > 57))\n",
-                            "            return false;\n",
-                            "    }\n",
-                            "    return true;\n",
-                            "}\n",
-                            "\n",
-                            "function numeric_keypress(evnt) {\n",
-                            "    var charC = (evnt.which) ? evnt.which : evnt.keyCode;\n",
-                            "\n",
-                            "    if (charC == 13) {\n",
-                            "        check_numeric(this, evnt);\n",
-                            "    } else {\n",
-                            "        return isValid(this, charC);\n",
-                            "    }\n",
-                            "}\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "function make_numeric(qa, outerqDiv, qDiv, aDiv, id) {\n",
-                            "\n",
-                            "\n",
-                            "\n",
-                            "    //console.log(answer);\n",
-                            "\n",
-                            "\n",
-                            "    outerqDiv.className = \"NumericQn\";\n",
-                            "    aDiv.style.display = 'block';\n",
-                            "\n",
-                            "    var lab = document.createElement(\"label\");\n",
-                            "    lab.className = \"InpLabel\";\n",
-                            "    lab.textContent = \"Type numeric answer here:\";\n",
-                            "    aDiv.append(lab);\n",
-                            "\n",
-                            "    var inp = document.createElement(\"input\");\n",
-                            "    inp.type = \"text\";\n",
-                            "    //inp.id=\"input-\"+id;\n",
-                            "    inp.id = id + \"-0\";\n",
-                            "    inp.className = \"Input-text\";\n",
-                            "    inp.setAttribute('data-answers', JSON.stringify(qa.answers));\n",
-                            "    if (\"precision\" in qa) {\n",
-                            "        inp.setAttribute('data-precision', qa.precision);\n",
-                            "    }\n",
-                            "    aDiv.append(inp);\n",
-                            "    //console.log(inp);\n",
-                            "\n",
-                            "    //inp.addEventListener(\"keypress\", check_numeric);\n",
-                            "    //inp.addEventListener(\"keypress\", numeric_keypress);\n",
-                            "    /*\n",
-                            "    inp.addEventListener(\"keypress\", function(event) {\n",
-                            "        return numeric_keypress(this, event);\n",
-                            "    }\n",
-                            "                        );\n",
-                            "                        */\n",
-                            "    //inp.onkeypress=\"return numeric_keypress(this, event)\";\n",
-                            "    inp.onkeypress = numeric_keypress;\n",
-                            "    inp.onpaste = event => false;\n",
-                            "\n",
-                            "    inp.addEventListener(\"focus\", function (event) {\n",
-                            "        this.value = \"\";\n",
-                            "        return false;\n",
-                            "    }\n",
-                            "    );\n",
-                            "\n",
-                            "\n",
-                            "}\n",
-                            "function jaxify(string) {\n",
-                            "    var mystring = string;\n",
-                            "\n",
-                            "    var count = 0;\n",
-                            "    var loc = mystring.search(/([^\\\\]|^)(\\$)/);\n",
-                            "\n",
-                            "    var count2 = 0;\n",
-                            "    var loc2 = mystring.search(/([^\\\\]|^)(\\$\\$)/);\n",
-                            "\n",
-                            "    //console.log(loc);\n",
-                            "\n",
-                            "    while ((loc >= 0) || (loc2 >= 0)) {\n",
-                            "\n",
-                            "        /* Have to replace all the double $$ first with current implementation */\n",
-                            "        if (loc2 >= 0) {\n",
-                            "            if (count2 % 2 == 0) {\n",
-                            "                mystring = mystring.replace(/([^\\\\]|^)(\\$\\$)/, \"$1\\\\[\");\n",
-                            "            } else {\n",
-                            "                mystring = mystring.replace(/([^\\\\]|^)(\\$\\$)/, \"$1\\\\]\");\n",
-                            "            }\n",
-                            "            count2++;\n",
-                            "        } else {\n",
-                            "            if (count % 2 == 0) {\n",
-                            "                mystring = mystring.replace(/([^\\\\]|^)(\\$)/, \"$1\\\\(\");\n",
-                            "            } else {\n",
-                            "                mystring = mystring.replace(/([^\\\\]|^)(\\$)/, \"$1\\\\)\");\n",
-                            "            }\n",
-                            "            count++;\n",
-                            "        }\n",
-                            "        loc = mystring.search(/([^\\\\]|^)(\\$)/);\n",
-                            "        loc2 = mystring.search(/([^\\\\]|^)(\\$\\$)/);\n",
-                            "        //console.log(mystring,\", loc:\",loc,\", loc2:\",loc2);\n",
-                            "    }\n",
-                            "\n",
-                            "    //console.log(mystring);\n",
-                            "    return mystring;\n",
-                            "}\n",
-                            "\n",
-                            "\n",
-                            "function show_questions(json, mydiv) {\n",
-                            "    console.log('show_questions');\n",
-                            "    //var mydiv=document.getElementById(myid);\n",
-                            "    var shuffle_questions = mydiv.dataset.shufflequestions;\n",
-                            "    var num_questions = mydiv.dataset.numquestions;\n",
-                            "    var shuffle_answers = mydiv.dataset.shuffleanswers;\n",
-                            "\n",
-                            "    if (num_questions > json.length) {\n",
-                            "        num_questions = json.length;\n",
-                            "    }\n",
-                            "\n",
-                            "    var questions;\n",
-                            "    if ((num_questions < json.length) || (shuffle_questions == \"True\")) {\n",
-                            "        //console.log(num_questions+\",\"+json.length);\n",
-                            "        questions = getRandomSubarray(json, num_questions);\n",
-                            "    } else {\n",
-                            "        questions = json;\n",
-                            "    }\n",
-                            "\n",
-                            "    //console.log(\"SQ: \"+shuffle_questions+\", NQ: \" + num_questions + \", SA: \", shuffle_answers);\n",
-                            "\n",
-                            "    // Iterate over questions\n",
-                            "    questions.forEach((qa, index, array) => {\n",
-                            "        //console.log(qa.question); \n",
-                            "\n",
-                            "        var id = makeid(8);\n",
-                            "        //console.log(id);\n",
-                            "\n",
-                            "\n",
-                            "        // Create Div to contain question and answers\n",
-                            "        var iDiv = document.createElement('div');\n",
-                            "        //iDiv.id = 'quizWrap' + id + index;\n",
-                            "        iDiv.id = 'quizWrap' + id;\n",
-                            "        iDiv.className = 'Quiz';\n",
-                            "        iDiv.setAttribute('data-qnum', index);\n",
-                            "        mydiv.appendChild(iDiv);\n",
-                            "        // iDiv.innerHTML=qa.question;\n",
-                            "\n",
-                            "        var outerqDiv = document.createElement('div');\n",
-                            "        outerqDiv.id = \"OuterquizQn\" + id + index;\n",
-                            "\n",
-                            "        iDiv.append(outerqDiv);\n",
-                            "\n",
-                            "        // Create div to contain question part\n",
-                            "        var qDiv = document.createElement('div');\n",
-                            "        qDiv.id = \"quizQn\" + id + index;\n",
-                            "        //qDiv.textContent=qa.question;\n",
-                            "        qDiv.innerHTML = jaxify(qa.question);\n",
-                            "\n",
-                            "        outerqDiv.append(qDiv);\n",
-                            "\n",
-                            "        // Create div for code inside question\n",
-                            "        var codeDiv;\n",
-                            "        if (\"code\" in qa) {\n",
-                            "            codeDiv = document.createElement('div');\n",
-                            "            codeDiv.id = \"code\" + id + index;\n",
-                            "            codeDiv.className = \"QuizCode\";\n",
-                            "            var codePre = document.createElement('pre');\n",
-                            "            codeDiv.append(codePre);\n",
-                            "            var codeCode = document.createElement('code');\n",
-                            "            codePre.append(codeCode);\n",
-                            "            codeCode.innerHTML = qa.code;\n",
-                            "            outerqDiv.append(codeDiv);\n",
-                            "            //console.log(codeDiv);\n",
-                            "        }\n",
-                            "\n",
-                            "\n",
-                            "        // Create div to contain answer part\n",
-                            "        var aDiv = document.createElement('div');\n",
-                            "        aDiv.id = \"quizAns\" + id + index;\n",
-                            "        aDiv.className = 'Answer';\n",
-                            "        iDiv.append(aDiv);\n",
-                            "\n",
-                            "        //console.log(qa.type);\n",
-                            "\n",
-                            "        var num_correct;\n",
-                            "        if ((qa.type == \"multiple_choice\") || (qa.type == \"many_choice\") ) {\n",
-                            "            num_correct = make_mc(qa, shuffle_answers, outerqDiv, qDiv, aDiv, id);\n",
-                            "            if (\"answer_cols\" in qa) {\n",
-                            "                //aDiv.style.gridTemplateColumns = 'auto '.repeat(qa.answer_cols);\n",
-                            "                aDiv.style.gridTemplateColumns = 'repeat(' + qa.answer_cols + ', 1fr)';\n",
-                            "            }\n",
-                            "        } else if (qa.type == \"numeric\") {\n",
-                            "            //console.log(\"numeric\");\n",
-                            "            make_numeric(qa, outerqDiv, qDiv, aDiv, id);\n",
-                            "        }\n",
-                            "\n",
-                            "\n",
-                            "        //Make div for feedback\n",
-                            "        var fb = document.createElement(\"div\");\n",
-                            "        fb.id = \"fb\" + id;\n",
-                            "        //fb.style=\"font-size: 20px;text-align:center;\";\n",
-                            "        fb.className = \"Feedback\";\n",
-                            "        fb.setAttribute(\"data-answeredcorrect\", 0);\n",
-                            "        fb.setAttribute(\"data-numcorrect\", num_correct);\n",
-                            "        iDiv.append(fb);\n",
-                            "\n",
-                            "\n",
-                            "    });\n",
-                            "    var preserveResponses = mydiv.dataset.preserveresponses;\n",
-                            "    console.log(preserveResponses);\n",
-                            "    console.log(preserveResponses == \"true\");\n",
-                            "    if (preserveResponses == \"true\") {\n",
-                            "        console.log(preserveResponses);\n",
-                            "        // Create Div to contain record of answers\n",
-                            "        var iDiv = document.createElement('div');\n",
-                            "        iDiv.id = 'responses' + mydiv.id;\n",
-                            "        iDiv.className = 'JCResponses';\n",
-                            "        // Create a place to store responses as an empty array\n",
-                            "        iDiv.setAttribute('data-responses', '[]');\n",
-                            "\n",
-                            "        // Dummy Text\n",
-                            "        iDiv.innerHTML=\"<b>Select your answers and then follow the directions that will appear here.</b>\"\n",
-                            "        //iDiv.className = 'Quiz';\n",
-                            "        mydiv.appendChild(iDiv);\n",
-                            "    }\n",
-                            "//console.log(\"At end of show_questions\");\n",
-                            "    if (typeof MathJax != 'undefined') {\n",
-                            "        console.log(\"MathJax version\", MathJax.version);\n",
-                            "        var version = MathJax.version;\n",
-                            "        setTimeout(function(){\n",
-                            "            var version = MathJax.version;\n",
-                            "            console.log('After sleep, MathJax version', version);\n",
-                            "            if (version[0] == \"2\") {\n",
-                            "                MathJax.Hub.Queue([\"Typeset\", MathJax.Hub]);\n",
-                            "            } else if (version[0] == \"3\") {\n",
-                            "                MathJax.typeset([mydiv]);\n",
-                            "            }\n",
-                            "        }, 500);\n",
-                            "if (typeof version == 'undefined') {\n",
-                            "        } else\n",
-                            "        {\n",
-                            "            if (version[0] == \"2\") {\n",
-                            "                MathJax.Hub.Queue([\"Typeset\", MathJax.Hub]);\n",
-                            "            } else if (version[0] == \"3\") {\n",
-                            "                MathJax.typeset([mydiv]);\n",
-                            "            } else {\n",
-                            "                console.log(\"MathJax not found\");\n",
-                            "            }\n",
-                            "        }\n",
-                            "    }\n",
-                            "    return false;\n",
-                            "}\n",
-                            "\n",
-                            "        {\n",
-                            "        show_questions(questionsQKKRGtQsSyoO,  QKKRGtQsSyoO);\n",
-                            "        }\n",
-                            "        "
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.Javascript object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "ename": "NameError",
+                    "evalue": "name 'it_path' is not defined",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[0;31mNameError\u001b[0m                                 Traceback (most recent call last)",
+                        "Cell \u001b[0;32mIn[10], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m display_quiz(\u001b[43mit_path\u001b[49m\u001b[38;5;241m+\u001b[39m\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mquestions.json\u001b[39m\u001b[38;5;124m\"\u001b[39m, border_radius\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m0\u001b[39m, question_alignment\u001b[38;5;241m=\u001b[39m\u001b[38;5;124m'\u001b[39m\u001b[38;5;124mcenter\u001b[39m\u001b[38;5;124m'\u001b[39m, max_width\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m1000\u001b[39m)\n",
+                        "\u001b[0;31mNameError\u001b[0m: name 'it_path' is not defined"
+                    ]
                 }
             ],
             "source": [
-                "display_quiz(github_preview, border_radius=0)"
+                "display_quiz(it_path+\"questions.json\", border_radius=0, question_alignment='center', max_width=1000)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `JupyterQuiz-2.3.0/PKG-INFO` & `JupyterQuiz-2.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterQuiz
-Version: 2.3.0
+Version: 2.3.5
 Summary: Interactive quizzes for Jupyter and Jupyter Book
 Author-email: "John M. Shea" <jshea@ieee.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: home-page, https://github.com/jmshea/jupyterquiz
 
 # JupyterQuiz
```

