# Comparing `tmp/scrubadubdub-0.1.0.tar.gz` & `tmp/scrubadubdub-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrubadubdub-0.1.0.tar", max compression
+gzip compressed data, was "scrubadubdub-0.2.0.tar", max compression
```

## Comparing `scrubadubdub-0.1.0.tar` & `scrubadubdub-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-05 10:08:05.566230 scrubadubdub-0.1.0/LICENSE
--rw-r--r--   0        0        0     1988 2023-04-05 10:01:06.250670 scrubadubdub-0.1.0/README.md
--rw-r--r--   0        0        0      324 2023-04-05 10:20:01.268167 scrubadubdub-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-05 09:51:06.434606 scrubadubdub-0.1.0/scrubadubdub/__init__.py
--rw-r--r--   0        0        0     1891 2023-04-05 09:53:45.765954 scrubadubdub-0.1.0/scrubadubdub/scrub.py
--rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 scrubadubdub-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2153 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/README.md
+-rw-r--r--   0        0        0      544 2023-04-21 10:02:52.266377 scrubadubdub-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/scrubadubdub/__init__.py
+-rw-r--r--   0        0        0     1224 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/scrubadubdub/cli.py
+-rw-r--r--   0        0        0     1891 2023-04-21 10:02:39.126608 scrubadubdub-0.2.0/scrubadubdub/scrub.py
+-rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 scrubadubdub-0.2.0/PKG-INFO
```

### Comparing `scrubadubdub-0.1.0/LICENSE` & `scrubadubdub-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrubadubdub-0.1.0/README.md` & `scrubadubdub-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,42 @@
-# scrub - PII Scrubbing Python Package
+<h1 align="center">🫧 scrub 🫧</h1>
 
-scrub is a lightweight, extensible Python package designed to remove Personally Identifiable Information (PII) from any text input. It leverages advanced Machine Learning algorithms to detect PII and provides multiple levels of scrubbing to ensure optimal anonymization of sensitive information. safeguarding user privacy.
+**scrub** is a lightweight, extensible Python package designed to remove Personally Identifiable Information (PII) from any text input. It leverages advanced Machine Learning algorithms to detect PII and provides multiple levels of scrubbing to ensure optimal anonymization of sensitive information. safeguarding user privacy.
 
 ## Installation
 
-Install the latest version of scrub from [PyPI](https://pypi.org/project/scrub/):
+Install the latest version of scrub from [PyPI](https://pypi.org/project/scrubadubdub/):
 
 ```bash
-pip install scrub
+pip install scrubadubdub
 ```
 
 ## Key Features
 
 - Advanced PII detection using Machine Learning algorithms.
 - Support for a wide range of PII types (names, email addresses, phone numbers, etc.).
 - Customizable detection threshold and levels of sanitization.
 - Extensible architecture to allow for the addition of new PII types and algorithms.
 
 ## Basic Usage
 
 ```python
-from scrub import Scrub
+from scrubadubdub import Scrub
 
 scrubber = Scrub()
 input_text = "My name is John Doe and my email address is john.doe@email.com, and my phone number is 123-456-7890"
 scrubbed_text = scrubber.scrub(input_text)
 print(scrubbed_text)
 ```
 
-## Advanced Usage
+```txt
+My name is [REDACTED-NAME] and my email address is [REDACTED-EMAIL], and my phone number is [REDACTED-PHONE]
+```
+
+<!-- ## Advanced Usage
 
 With scrub, you can customize the detection threshold, sanitization levels, and even integrate additional scrubbing functionalities based on your needs.
 
 ```python
 # Set custom threshold and level
 scrubber.set_threshold(0.9)
 scrubber.set_sanitization_level(scrub.SanitizationLevels.MEDIUM)
@@ -41,20 +45,20 @@
 scrubber.enable_email_sanitization()
 
 # Add custom PII detection function
 def custom_detection(text):
     ...
 
 scrubber.add_detection_function(custom_detection)
-```
+``` -->
 
-## Documentation
+<!-- ## Documentation
 
 More details on setting up and using scrub can be found in the [Documentation](https://scrub.readthedocs.io).
 
 ## Contributing
 
-We love contributions! If you'd like to contribute to scrub, please read our [Contributing Guidelines](./CONTRIBUTING.md) for more information on how to get started.
+We love contributions! If you'd like to contribute to scrub, please read our [Contributing Guidelines](./CONTRIBUTING.md) for more information on how to get started. -->
 
 ## License
 
 scrub is licensed under the MIT License. See [LICENSE](./LICENSE) for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scrubadubdub-0.1.0/scrubadubdub/scrub.py` & `scrubadubdub-0.2.0/scrubadubdub/scrub.py`

 * *Files identical despite different names*

### Comparing `scrubadubdub-0.1.0/PKG-INFO` & `scrubadubdub-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 Metadata-Version: 2.1
 Name: scrubadubdub
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package to scrub PII
+Home-page: https://github.com/kylemclaren/scrub
 License: MIT
 Author: Kyle McLaren
 Author-email: kylemclaren@protonmail.com
-Requires-Python: >=3.6
+Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: halo (>=0.0.31,<0.0.32)
+Requires-Dist: ipaddress (>=1.0.23,<2.0.0)
+Requires-Dist: numpy (>=1.24.2,<2.0.0)
+Requires-Dist: phonenumbers (>=8.13.8,<9.0.0)
+Requires-Dist: spacy (>=3.5.1,<4.0.0)
+Project-URL: Repository, https://github.com/kylemclaren/scrub
 Description-Content-Type: text/markdown
 
-# scrub - PII Scrubbing Python Package
+<h1 align="center">🫧 scrub 🫧</h1>
 
-scrub is a lightweight, extensible Python package designed to remove Personally Identifiable Information (PII) from any text input. It leverages advanced Machine Learning algorithms to detect PII and provides multiple levels of scrubbing to ensure optimal anonymization of sensitive information. safeguarding user privacy.
+**scrub** is a lightweight, extensible Python package designed to remove Personally Identifiable Information (PII) from any text input. It leverages advanced Machine Learning algorithms to detect PII and provides multiple levels of scrubbing to ensure optimal anonymization of sensitive information. safeguarding user privacy.
 
 ## Installation
 
-Install the latest version of scrub from [PyPI](https://pypi.org/project/scrub/):
+Install the latest version of scrub from [PyPI](https://pypi.org/project/scrubadubdub/):
 
 ```bash
-pip install scrub
+pip install scrubadubdub
 ```
 
 ## Key Features
 
 - Advanced PII detection using Machine Learning algorithms.
 - Support for a wide range of PII types (names, email addresses, phone numbers, etc.).
 - Customizable detection threshold and levels of sanitization.
 - Extensible architecture to allow for the addition of new PII types and algorithms.
 
 ## Basic Usage
 
 ```python
-from scrub import Scrub
+from scrubadubdub import Scrub
 
 scrubber = Scrub()
 input_text = "My name is John Doe and my email address is john.doe@email.com, and my phone number is 123-456-7890"
 scrubbed_text = scrubber.scrub(input_text)
 print(scrubbed_text)
 ```
 
-## Advanced Usage
+```txt
+My name is [REDACTED-NAME] and my email address is [REDACTED-EMAIL], and my phone number is [REDACTED-PHONE]
+```
+
+<!-- ## Advanced Usage
 
 With scrub, you can customize the detection threshold, sanitization levels, and even integrate additional scrubbing functionalities based on your needs.
 
 ```python
 # Set custom threshold and level
 scrubber.set_threshold(0.9)
 scrubber.set_sanitization_level(scrub.SanitizationLevels.MEDIUM)
@@ -59,20 +66,20 @@
 scrubber.enable_email_sanitization()
 
 # Add custom PII detection function
 def custom_detection(text):
     ...
 
 scrubber.add_detection_function(custom_detection)
-```
+``` -->
 
-## Documentation
+<!-- ## Documentation
 
 More details on setting up and using scrub can be found in the [Documentation](https://scrub.readthedocs.io).
 
 ## Contributing
 
-We love contributions! If you'd like to contribute to scrub, please read our [Contributing Guidelines](./CONTRIBUTING.md) for more information on how to get started.
+We love contributions! If you'd like to contribute to scrub, please read our [Contributing Guidelines](./CONTRIBUTING.md) for more information on how to get started. -->
 
 ## License
 
 scrub is licensed under the MIT License. See [LICENSE](./LICENSE) for more details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

