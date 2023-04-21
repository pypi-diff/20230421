# Comparing `tmp/django-choices-field-2.1.tar.gz` & `tmp/django_choices_field-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-choices-field-2.1.tar", max compression
+gzip compressed data, was "django_choices_field-2.1.1.tar", max compression
```

## Comparing `django-choices-field-2.1.tar` & `django_choices_field-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1077 2022-08-30 19:05:39.349753 django-choices-field-2.1/LICENSE
--rw-r--r--   0        0        0     2085 2022-08-30 19:05:39.349753 django-choices-field-2.1/README.md
--rw-r--r--   0        0        0      132 2022-08-30 19:05:39.349753 django-choices-field-2.1/django_choices_field/__init__.py
--rw-r--r--   0        0        0     3030 2022-08-30 19:05:39.349753 django-choices-field-2.1/django_choices_field/fields.py
--rw-r--r--   0        0        0     5942 2022-08-30 19:05:39.349753 django-choices-field-2.1/django_choices_field/fields.pyi
--rw-r--r--   0        0        0     2697 2022-08-30 19:05:39.349753 django-choices-field-2.1/pyproject.toml
--rw-r--r--   0        0        0     2803 2022-08-30 19:06:10.878458 django-choices-field-2.1/setup.py
--rw-r--r--   0        0        0     3239 2022-08-30 19:06:10.878834 django-choices-field-2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-21 18:21:00.361194 django_choices_field-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2086 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/README.md
+-rw-r--r--   0        0        0      124 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/django_choices_field/__init__.py
+-rw-r--r--   0        0        0     3055 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/django_choices_field/fields.py
+-rw-r--r--   0        0        0     5609 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/django_choices_field/fields.pyi
+-rw-r--r--   0        0        0     3257 2023-04-21 18:21:00.365195 django_choices_field-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 django_choices_field-2.1.1/PKG-INFO
```

### Comparing `django-choices-field-2.1/LICENSE` & `django_choices_field-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-choices-field-2.1/README.md` & `django_choices_field-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 pip install django-choices-field
 ```
 
 ## Usage
 
 ```python
 from django.db import models
-from django_choices_field import TexChoicesField, IntegerChoicesField
+from django_choices_field import TextChoicesField, IntegerChoicesField
 
 
 class MyModel(models.Model):
     class TextEnum(models.TextChoices):
         FOO = "foo", "Foo Description"
         BAR = "bar", "Bar Description"
```

### Comparing `django-choices-field-2.1/django_choices_field/fields.py` & `django_choices_field-2.1.1/django_choices_field/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 
     def to_python(self, value):
         if value is None:
             return None
 
         try:
             return self.choices_enum(value)
-        except ValueError:
+        except ValueError as e:
             raise ValidationError(
                 self.error_messages["invalid"],
                 code="invalid",
                 params={"value": value, "enum": self.choices_enum},
-            )
+            ) from e
 
     def from_db_value(self, value, expression, connection):
         return self.to_python(value)
 
     def get_prep_value(self, value):
         value = super().get_prep_value(value)
         return self.to_python(value)
@@ -72,28 +72,28 @@
 
     def to_python(self, value):
         if value is None:
             return None
 
         try:
             return self.choices_enum(int(value) if isinstance(value, str) else value)
-        except ValueError:
+        except ValueError as e:
             raise ValidationError(
                 self.error_messages["invalid"],
                 code="invalid",
                 params={"value": value, "enum": self.choices_enum},
-            )
+            ) from e
 
     def from_db_value(self, value, expression, connection):
         return self.to_python(value)
 
     def get_prep_value(self, value):
         value = super().get_prep_value(value)
         return self.to_python(value)
 
     def formfield(self, **kwargs):  # pragma:nocover
         return super().formfield(
             **{
                 "coerce": self.to_python,
                 **kwargs,
-            }
+            },
         )
```

### Comparing `django-choices-field-2.1/pyproject.toml` & `django_choices_field-2.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-choices-field"
-version = "2.1"
+version = "2.1.1"
 description = "Django field that set/get django's new TextChoices/IntegerChoices enum."
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bellini666/django-choices-field"
 repository = "https://github.com/bellini666/django-choices-field"
 documentation = "https://django-choices-field.readthedocs.io"
@@ -16,47 +16,41 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
 ]
 packages = [{ include = "django_choices_field" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+django = ">=3.2"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
+black = "^23.3.0"
 codecov = "^2.1.11"
 django = "^4.0"
-django-types = "^0.16.0"
-flake8 = "^4.0.1"
-flake8-broken-line = "^0.5.0"
-flake8-bugbear = "^22.4.25"
-flake8-builtins = "^1.5.3"
-flake8-comprehensions = "^3.5.0"
-flake8-polyfill = "^1.0.2"
-flake8-return = "^1.1.3"
-flake8-simplify = "^0.19.2"
-mock = "^4.0.3"
-pynvim = "^0.4.3"
+django-types = "^0.17.0"
 pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 pytest-django = "^4.2.0"
-isort = "^5.9.2"
+ruff = "^0.0.262"
 
 [tool.black]
 line-length = 100
-target-version = ['py37', 'py38', 'py39']
+target-version = ['py38']
+preview = true
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
   | \.tox
@@ -65,24 +59,99 @@
   | _build
   | buck-out
   | build
   | dist
 )/
 '''
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-force_sort_within_sections = true
+[tool.ruff]
+line-length = 100
+select = [
+  "E",
+  "F",
+  "W",
+  "I",
+  "N",
+  "D",
+  "UP",
+  "YTT",
+  "D2",
+  "D3",
+  "D4",
+  "BLE",
+  "B",
+  "A",
+  "COM",
+  "C4",
+  "DTZ",
+  "T10",
+  "EXE",
+  "ISC",
+  "ICN001",
+  "G",
+  "INP",
+  "PIE",
+  "T20",
+  "PYI",
+  "PT",
+  "Q",
+  "RET",
+  "SIM",
+  "TID",
+  "TCH",
+  "PTH",
+  "ERA",
+  "PGH",
+  "PL",
+  "RSE",
+  "RUF",
+  "TRY",
+  "SLF",
+]
+ignore = [
+  "D1",
+  "D203",
+  "D213",
+  "TCH001",
+  "TCH002",
+  "TCH003",
+  "PGH003",
+  "PLR09",
+  "PLR2004",
+  "SLF001",
+  "TRY003",
+]
+target-version = "py38"
+exclude = [
+  ".eggs",
+  ".git",
+  ".hg",
+  ".mypy_cache",
+  ".tox",
+  ".venv",
+  "__pycached__",
+  "_build",
+  "buck-out",
+  "build",
+  "dist",
+]
+
+[tool.ruff.pyupgrade]
+
+[tool.ruff.isort]
+
+[tool.ruff.pydocstyle]
+convention = "google"
 
 [tool.pyright]
 pythonVersion = "3.8"
 useLibraryCodeForTypes = true
 venvPath = "."
 venv = ".venv"
+ignore = ["**/migrations"]
 reportCallInDefaultInitializer = "warning"
 reportMatchNotExhaustive = "warning"
 reportMissingSuperCall = "warning"
 reportOverlappingOverload = "warning"
 reportUninitializedInstanceVariable = "none"
 reportUnnecessaryCast = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
```

### Comparing `django-choices-field-2.1/PKG-INFO` & `django_choices_field-2.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: django-choices-field
-Version: 2.1
+Version: 2.1.1
 Summary: Django field that set/get django's new TextChoices/IntegerChoices enum.
 Home-page: https://github.com/bellini666/django-choices-field
 License: MIT
 Keywords: django,enum
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: django (>=3.2)
 Project-URL: Documentation, https://django-choices-field.readthedocs.io
 Project-URL: Repository, https://github.com/bellini666/django-choices-field
 Description-Content-Type: text/markdown
 
 # django-choices-field
 
 [![build status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Fbellini666%2Fdjango-choices-field%2Fbadge%3Fref%3Dmaster&style=flat)](https://actions-badge.atrox.dev/bellini666/django-choices-field/goto?ref=master)
@@ -42,15 +50,15 @@
 pip install django-choices-field
 ```
 
 ## Usage
 
 ```python
 from django.db import models
-from django_choices_field import TexChoicesField, IntegerChoicesField
+from django_choices_field import TextChoicesField, IntegerChoicesField
 
 
 class MyModel(models.Model):
     class TextEnum(models.TextChoices):
         FOO = "foo", "Foo Description"
         BAR = "bar", "Bar Description"
```

