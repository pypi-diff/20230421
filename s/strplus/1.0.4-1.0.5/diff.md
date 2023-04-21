# Comparing `tmp/strplus-1.0.4.tar.gz` & `tmp/strplus-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-1.0.4.tar", max compression
+gzip compressed data, was "strplus-1.0.5.tar", max compression
```

## Comparing `strplus-1.0.4.tar` & `strplus-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.4/LICENSE
--rw-r--r--   0        0        0     2824 2023-04-20 19:29:34.926626 strplus-1.0.4/README.md
--rw-r--r--   0        0        0     1027 2023-04-20 19:29:34.926626 strplus-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      161 2023-04-20 19:29:34.926626 strplus-1.0.4/strplus/__init__.py
--rw-r--r--   0        0        0     4271 2023-04-20 19:28:33.046661 strplus-1.0.4/strplus/cases.py
--rw-r--r--   0        0        0      722 2023-04-20 18:44:25.554135 strplus-1.0.4/strplus/functions.py
--rw-r--r--   0        0        0     4316 2023-04-20 19:28:33.046661 strplus-1.0.4/strplus/strplus.py
--rw-r--r--   0        0        0     3480 1970-01-01 00:00:00.000000 strplus-1.0.4/setup.py
--rw-r--r--   0        0        0     3452 1970-01-01 00:00:00.000000 strplus-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:41:30.953611 strplus-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2859 2023-04-21 05:59:45.510185 strplus-1.0.5/README.md
+-rw-r--r--   0        0        0     1027 2023-04-21 05:44:22.660467 strplus-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-04-21 05:44:22.660467 strplus-1.0.5/strplus/__init__.py
+-rw-r--r--   0        0        0     6703 2023-04-21 07:04:27.239013 strplus-1.0.5/strplus/cases.py
+-rw-r--r--   0        0        0     3959 2023-04-21 07:04:27.239013 strplus-1.0.5/strplus/functions.py
+-rw-r--r--   0        0        0     4461 2023-04-21 07:04:27.239013 strplus-1.0.5/strplus/strplus.py
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 strplus-1.0.5/setup.py
+-rw-r--r--   0        0        0     3487 1970-01-01 00:00:00.000000 strplus-1.0.5/PKG-INFO
```

### Comparing `strplus-1.0.4/LICENSE` & `strplus-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-1.0.4/README.md` & `strplus-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 
 <br>
 
 ## Features ✨️
 
 - Wrapper Class
 - +234 test in 32 Tests files!
-- Simple use! 
+- Simple use!
+- Made with A.I. contribution 🤖 
 
 <br>
 
 ### Simple use example 😍
 ```
 >>> my_string = Str('Cast_this_string_TO_Pascal')
 >>> my_string.pascal
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
-
+- Made with A.I. contribution ð¤
 ### Simple use example ð ``` >>> my_string = Str
 ('Cast_this_string_TO_Pascal') >>> my_string.pascal 'CastThisStringToPascal'
 >>> my_string = Str('CastMeUseLikeANormalFunction') >>> my_string.snake
 'cast_me_use_like_a_normal_function' ```
 * [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/
 ) * [Documentations examples](https://wiseupdata.github.io/strplus/index.html)!
```

### Comparing `strplus-1.0.4/pyproject.toml` & `strplus-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "1.0.4"
+version = "1.0.5"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-1.0.4/strplus/strplus.py` & `strplus-1.0.5/strplus/strplus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,57 @@
-from strplus.cases import to_camel, to_list, to_pascal, to_snake
+from strplus.cases import to_camel, to_pascal, to_snake
+from strplus.functions import to_list
 
 
 class Str(str):
-    """A subclass of the built-in str class with additional string manipulation methods.
+    """
+
+    !!! info
+
+        The Str Class is a Wrapper class that extends the str Class, giving it superpowers
+        to handle strings and making it easy to use the strplus functions! You don't need to import, only if you want!
+        All methods from Str are recursive and return the Str object itself, so you always have the same features in the result.
+
+    !!! example "Never was so easy! Simple no parentheses! "
+
+        === "Snake case"
+            ```python
+            my_string = Str("Cast_this_StringToSnake")
+
+            my_string.snake
+            ```
+            'cast_this_string_to_snake'
+
+        === "Camel case"
+            ```python
+            my_string = Str("cast_this_string_to_camel")
+
+            my_string.camel
+            ```
+            'castThisStringToCamel'
+
+        === "Pascal"
+            ```python
+            my_string = Str("Cast_this_string_TO_Pascal!")
+
+            my_string.pascal
+            ```
+            'CastThisStringToPascal'
+
 
-    This class provides several methods for converting strings to different cases, as well as a method for
-    converting a string to a list of words.
+    !!! tip "Use parentheses if you prefer!"
 
-    All methods that return strings return instances of the Str class, so they can be further manipulated
-    with any of the methods provided by this class or by the built-in str class.
+        === "Snake case"
+            ```python
+            my_string = Str("HelloWorld")
 
-    Examples:
-    
-        >>> my_string = Str('hello_world')
-        >>> my_string.to_pascal()
-        'HelloWorld'
-
-        >>> my_string = Str('this_is-an_example')
-        >>> my_string.to_camel()
-        'thisIsAnExample'
-
-        >>> my_string = Str("HelloWorld")
-        >>> my_string.to_snake()
-        'hello_world'
-
-        >>> my_string = Str("Hello, World!")
-        >>> my_string.lower()
-        'hello, world!'
+            my_string.to_snake()
 
-    Note that all methods provided by the Str class are based on regular expressions, so they may not be
-    appropriate for all string manipulation tasks.
+            ```
+            'hello_world'
     """
 
     def __new__(cls, *args, **kwargs):
         if not all(isinstance(arg, str) for arg in args):
             raise TypeError("Str argument must be a string")
         return super().__new__(cls, *args, **kwargs)
 
@@ -61,71 +79,73 @@
 
     @property
     def print(self):
         print(self)
 
     def to_pascal(self):
         """
-        Converts a string to PascalCase.
+        !!! info
+            Simple method to converts a string to PascalCase.
+            Extend the method: to_pascal
 
         Returns:
             str: The PascalCase version of the input string.
 
-        Examples:
-        
-            >>> my_string = Str('hello_world')
-            >>> my_string.to_pascal()
-            'HelloWorld'
-            
-            >>> my_string = Str('some-mixed_string With spaces_underscores-and-hyphens')
-            >>> my_string.to_pascal()
+
+        !!! example
+
+            ```python
+            my_string = Str('some-mixed_string With spaces_underscores-and-hyphens')
+
+            my_string.to_pascal()
+            ```
             'SomeMixedStringWithSpacesUnderscoresAndHyphens'
-            
+
         """
         return Str(to_pascal(self))
 
     def to_camel(self):
         """Converts a string from any case to CamelCase.
 
         Returns:
             str: The converted string in CamelCase.
 
         Examples:
-        
+
             >>> my_string = Str('this_is-an_example')
             >>> my_string.to_camel()
             'thisIsAnExample'
 
             >>> my_string = Str('This is a test!')
             >>> my_string.to_camel()
             'thisIsATest'
-            
+
         """
         return Str(to_camel(self))
 
     def to_snake(self):
         """Converts a string to snake_case.
 
         Returns:
             str: The string converted to snake_case.
 
         Examples:
-        
+
             >>> my_string = Str("HelloWorld")
             >>> my_string.snake("HelloWorld")
             'hello_world'
 
             >>> my_string = Str("  AnotherString!  ")
             >>> my_string.to_snake()
             'another_string'
 
             >>>  my_string = Str("hello-world")
             >>> my_string.to_snake()
             'hello_world'
-            
+
         """
         return Str(to_snake(self))
 
     def to_list(self):
         return [Str(word) for word in to_list(self)]
```

### Comparing `strplus-1.0.4/setup.py` & `strplus-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use! \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'Cast_this_string_TO_Pascal\')\n>>> my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str(\'CastMeUseLikeANormalFunction\')\n>>> my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n<br>\n\n* [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/)\n* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi](https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://pepy.tech/project/strplus)\n[![versions](https://img.shields.io/pypi/pyversions/strplus.svg)](https://github.com/wiseupdata/strplus)\n\n\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/imgs/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n[Documentation](https://wiseupdata.github.io/strplus/index.html)  🚀\n\n<br>\n\n## Features ✨️\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n- Simple use!\n- Made with A.I. contribution 🤖 \n\n<br>\n\n### Simple use example 😍\n```\n>>> my_string = Str(\'Cast_this_string_TO_Pascal\')\n>>> my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str(\'CastMeUseLikeANormalFunction\')\n>>> my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n<br>\n\n* [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/)\n* [Documentations examples](https://wiseupdata.github.io/strplus/index.html)! \n\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n2. [Emojis](https://github.com/wiseupdata/emojis)\n3. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br>\n<br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData\n',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'1.0.4', 'description': 'Python extra functions for strings',
+'1.0.5', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n[![pypi]
 (https://img.shields.io/pypi/v/strplus?color=green)](https://pypi.python.org/
 pypi/strplus)\n[![downloads](https://pepy.tech/badge/strplus/month)](https://
@@ -17,15 +17,15 @@
 \n
 \n
 \n
 \n
 \n
 \n\n[Documentation](https://wiseupdata.github.io/strplus/index.html) ð\n\n
 \n\n## Features â¨ï¸\n\n- Wrapper Class\n- +234 test in 32 Tests files!\n-
-Simple use! \n\n
+Simple use!\n- Made with A.I. contribution ð¤ \n\n
 \n\n### Simple use example ð\n```\n>>> my_string = Str
 (\'Cast_this_string_TO_Pascal\')\n>>>
 my_string.pascal\n\'CastThisStringToPascal\'\n\n>>> my_string = Str
 (\'CastMeUseLikeANormalFunction\')\n>>>
 my_string.snake\n\'cast_me_use_like_a_normal_function\'\n\n```\n
 \n\n* [More Examples !](https://wiseupdata.github.io/strplus/examples/
 examples_01/)\n* [Documentations examples](https://wiseupdata.github.io/
```

### Comparing `strplus-1.0.4/PKG-INFO` & `strplus-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -60,15 +60,16 @@
 
 <br>
 
 ## Features ✨️
 
 - Wrapper Class
 - +234 test in 32 Tests files!
-- Simple use! 
+- Simple use!
+- Made with A.I. contribution 🤖 
 
 <br>
 
 ### Simple use example 😍
 ```
 >>> my_string = Str('Cast_this_string_TO_Pascal')
 >>> my_string.pascal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 1.0.4 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 1.0.5 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 
 
 
 
 
 [Documentation](https://wiseupdata.github.io/strplus/index.html) ð
 ## Features â¨ï¸ - Wrapper Class - +234 test in 32 Tests files! - Simple use!
-
+- Made with A.I. contribution ð¤
 ### Simple use example ð ``` >>> my_string = Str
 ('Cast_this_string_TO_Pascal') >>> my_string.pascal 'CastThisStringToPascal'
 >>> my_string = Str('CastMeUseLikeANormalFunction') >>> my_string.snake
 'cast_me_use_like_a_normal_function' ```
 * [More Examples !](https://wiseupdata.github.io/strplus/examples/examples_01/
 ) * [Documentations examples](https://wiseupdata.github.io/strplus/index.html)!
```

