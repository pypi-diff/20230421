# Comparing `tmp/gwlandscape-python-0.3.0.tar.gz` & `tmp/gwlandscape-python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwlandscape-python-0.3.0.tar", max compression
+gzip compressed data, was "gwlandscape-python-0.3.1.tar", max compression
```

## Comparing `gwlandscape-python-0.3.0.tar` & `gwlandscape-python-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,23 @@
--rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape-python-0.3.0/LICENSE
--rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape-python-0.3.0/README.rst
--rw-r--r--   0        0        0       37 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/README.md
--rw-r--r--   0        0        0     5924 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape-python-0.3.0/gwlandscape_python/__init__.py
--rw-r--r--   0        0        0     2140 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/dataset_type.py
--rw-r--r--   0        0        0    17763 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/gwlandscape.py
--rw-r--r--   0        0        0     1578 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/keyword_type.py
--rw-r--r--   0        0        0     1890 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/model_type.py
--rw-r--r--   0        0        0     3771 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/publication_type.py
--rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape-python-0.3.0/gwlandscape_python/settings.py
--rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.0/gwlandscape_python/tests/__init__.py
--rw-r--r--   0        0        0      176 2022-08-30 00:50:21.643802 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4499 2023-04-20 22:06:01.608362 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/conftest.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2887 2023-04-20 22:06:01.648362 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_dataset_type.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0    30447 2023-04-20 22:06:01.712363 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_gwlandscape_python.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2421 2023-04-20 22:06:01.784364 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_keyword_type.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2688 2023-04-20 22:06:01.788364 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_model_type.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     5177 2023-04-20 22:06:01.796364 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_publication_type.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0      374 2022-08-30 00:50:21.671802 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     3052 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/conftest.py
--rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_dataset_type.py
--rw-r--r--   0        0        0    36190 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_gwlandscape_python.py
--rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_keyword_type.py
--rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_model_type.py
--rw-r--r--   0        0        0     4228 2023-04-20 04:41:39.760269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_publication_type.py
--rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.0/gwlandscape_python/tests/utils.py
--rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.0/gwlandscape_python/utils/__init__.py
--rw-r--r--   0        0        0      249 2022-12-06 05:10:16.275674 gwlandscape-python-0.3.0/gwlandscape_python/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1786 2022-12-06 05:10:16.275674 gwlandscape-python-0.3.0/gwlandscape_python/utils/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0     3565 2022-12-08 23:27:42.059757 gwlandscape-python-0.3.0/gwlandscape_python/utils/tests/__pycache__/test_utils.cpython-38-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.0/gwlandscape_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape-python-0.3.0/gwlandscape_python/utils/utils.py
--rw-r--r--   0        0        0     1074 2023-04-21 01:14:04.590655 gwlandscape-python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1732 2023-04-21 01:14:18.265159 gwlandscape-python-0.3.0/setup.py
--rw-r--r--   0        0        0     1618 2023-04-21 01:14:18.265417 gwlandscape-python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape-python-0.3.1/LICENSE
+-rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape-python-0.3.1/README.rst
+-rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape-python-0.3.1/gwlandscape_python/__init__.py
+-rw-r--r--   0        0        0     2140 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/dataset_type.py
+-rw-r--r--   0        0        0    17552 2023-04-21 06:22:03.415309 gwlandscape-python-0.3.1/gwlandscape_python/gwlandscape.py
+-rw-r--r--   0        0        0     1578 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/keyword_type.py
+-rw-r--r--   0        0        0     1890 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/model_type.py
+-rw-r--r--   0        0        0     3771 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/publication_type.py
+-rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape-python-0.3.1/gwlandscape_python/settings.py
+-rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.1/gwlandscape_python/tests/__init__.py
+-rw-r--r--   0        0        0     3052 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_dataset_type.py
+-rw-r--r--   0        0        0    36190 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_gwlandscape_python.py
+-rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_keyword_type.py
+-rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_model_type.py
+-rw-r--r--   0        0        0     4228 2023-04-20 04:41:39.760269 gwlandscape-python-0.3.1/gwlandscape_python/tests/test_publication_type.py
+-rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.1/gwlandscape_python/tests/utils.py
+-rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.1/gwlandscape_python/utils/__init__.py
+-rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.1/gwlandscape_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape-python-0.3.1/gwlandscape_python/utils/utils.py
+-rw-r--r--   0        0        0     1074 2023-04-21 06:22:03.419309 gwlandscape-python-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1661 2023-04-21 06:22:10.725775 gwlandscape-python-0.3.1/setup.py
+-rw-r--r--   0        0        0     1618 2023-04-21 06:22:10.726006 gwlandscape-python-0.3.1/PKG-INFO
```

### Comparing `gwlandscape-python-0.3.0/LICENSE` & `gwlandscape-python-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/README.rst` & `gwlandscape-python-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/dataset_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/dataset_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/gwlandscape.py` & `gwlandscape-python-0.3.1/gwlandscape_python/gwlandscape.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,44 +166,37 @@
             A list of str or :class:`~.Keyword` objects for the publication, by default None
 
         Returns
         -------
         Publication
             Created Publication
         """
+        inputs = {key: val for key, val in locals().items() if ((val is not None) and (key != 'self'))}
+
         mutation = """
             mutation AddPublicationMutation($input: AddPublicationMutationInput!) {
                 addPublication(input: $input) {
                     id
                 }
             }
         """
 
-        params = {
-            'input': {
-                'author': author,
-                'title': title,
-                'arxiv_id': arxiv_id,
-                'published': published,
-                'year': year,
-                'journal': journal,
-                'journal_doi': journal_doi,
-                'dataset_doi': dataset_doi,
-                'description': description,
-                'public': public,
-                'download_link': download_link
-            }
-        }
-
         # Handle keywords
         if isinstance(keywords, list):
-            params['input']['keywords'] = [
+            inputs['keywords'] = [
                 self.get_keywords(exact=keyword)[0].id if isinstance(keyword, str) else keyword.id
                 for keyword in keywords
             ]
+            inputs['keywords'] = [keyword.id for keyword in keywords]
+
+        params = {
+            'input': {
+                **inputs
+            }
+        }
 
         result = self.request(mutation, params)
 
         assert 'id' in result['add_publication']
 
         return self.get_publications(_id=result['add_publication']['id'])[0]
 
@@ -300,27 +293,27 @@
             The description of the model to be created, by default None
 
         Returns
         -------
         Model
             Created Model
         """
+        inputs = {key: val for key, val in locals().items() if ((val is not None) and (key != 'self'))}
+
         mutation = """
             mutation AddCompasModelMutation($input: AddCompasModelMutationInput!) {
                 addCompasModel(input: $input) {
                     id
                 }
             }
         """
 
         params = {
             'input': {
-                'name': name,
-                'summary': summary,
-                'description': description
+                **inputs
             }
         }
 
         result = self.request(mutation, params)
 
         assert 'id' in result['add_compas_model']
```

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/keyword_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/keyword_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/model_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/model_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/publication_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/publication_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/tests/conftest.py` & `gwlandscape-python-0.3.1/gwlandscape_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/tests/test_dataset_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_dataset_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/tests/test_gwlandscape_python.py` & `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_gwlandscape_python.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/tests/test_keyword_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_keyword_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/tests/test_model_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_model_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/tests/test_publication_type.py` & `gwlandscape-python-0.3.1/gwlandscape_python/tests/test_publication_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/utils/tests/test_utils.py` & `gwlandscape-python-0.3.1/gwlandscape_python/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/gwlandscape_python/utils/utils.py` & `gwlandscape-python-0.3.1/gwlandscape_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.0/pyproject.toml` & `gwlandscape-python-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwlandscape-python"
-version = "0.3.0"
+version = "0.3.1"
 description = "Wrapper of GWDC API, used for interacting with the GWLandscape endpoints"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>", "Lewis Lakerink <llakerink@swin.edu.au"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwlandscape_python"
 include = ["LICENSE",]
```

### Comparing `gwlandscape-python-0.3.0/setup.py` & `gwlandscape-python-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 packages = \
 ['gwlandscape_python',
  'gwlandscape_python.tests',
  'gwlandscape_python.utils',
  'gwlandscape_python.utils.tests']
 
 package_data = \
-{'': ['*'],
- 'gwlandscape_python': ['.pytest_cache/*', '.pytest_cache/v/cache/*']}
+{'': ['*']}
 
 install_requires = \
 ['graphene-file-upload>=1.3.0,<2.0.0',
  'gwdc-python>=0.4.1,<0.5.0',
  'importlib-metadata>=4.5.0,<5.0.0',
  'jwt>=1.2.0,<2.0.0',
  'requests>=2.25.1,<3.0.0',
  'tqdm>=4.61.2,<5.0.0']
 
 extras_require = \
 {'docs': ['Sphinx>=4.0.2,<5.0.0', 'sphinx-rtd-theme>=0.5.2,<0.6.0']}
 
 setup_kwargs = {
     'name': 'gwlandscape-python',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Wrapper of GWDC API, used for interacting with the GWLandscape endpoints',
     'long_description': "GWLandscape Python API\n======================\n\n`GWLandscape <https://gwlandscape.org.au/>`_ is a service used to handle both the submission of COMPAS jobs (todo)\n\nCheck out the `documentation <https://gwlandscape-python.readthedocs.io/en/latest/>`_ for more information.\n\nInstallation\n------------\n\nThe gwlandscape-python package can be installed with\n\n::\n\n    pip install gwlandscape-python\n\n\nExample\n-------\n\n::\n\n    >>> from gwlandscape_python import GWLandscape\n    >>> gwl = GWLandscape(token='<user_api_token_here>')\n\n",
     'author': 'Thomas Reichardt',
     'author_email': 'treichardt@swin.edu.au',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/gravitationalwavedc/gwlandscape_python',
```

### Comparing `gwlandscape-python-0.3.0/PKG-INFO` & `gwlandscape-python-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwlandscape-python
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wrapper of GWDC API, used for interacting with the GWLandscape endpoints
 Home-page: https://github.com/gravitationalwavedc/gwlandscape_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

