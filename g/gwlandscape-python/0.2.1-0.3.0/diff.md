# Comparing `tmp/gwlandscape-python-0.2.1.tar.gz` & `tmp/gwlandscape-python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwlandscape-python-0.2.1.tar", max compression
+gzip compressed data, was "gwlandscape-python-0.3.0.tar", max compression
```

## Comparing `gwlandscape-python-0.2.1.tar` & `gwlandscape-python-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,39 @@
--rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape-python-0.2.1/LICENSE
--rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape-python-0.2.1/README.rst
--rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape-python-0.2.1/gwlandscape_python/__init__.py
--rw-r--r--   0        0        0      344 2022-12-16 02:08:22.812511 gwlandscape-python-0.2.1/gwlandscape_python/dataset_type.py
--rw-r--r--   0        0        0    19649 2023-03-27 03:08:09.591796 gwlandscape-python-0.2.1/gwlandscape_python/gwlandscape.py
--rw-r--r--   0        0        0      165 2022-12-16 02:08:22.812511 gwlandscape-python-0.2.1/gwlandscape_python/keyword_type.py
--rw-r--r--   0        0        0      201 2022-12-16 02:08:22.812511 gwlandscape-python-0.2.1/gwlandscape_python/model_type.py
--rw-r--r--   0        0        0      407 2022-12-16 02:08:22.812511 gwlandscape-python-0.2.1/gwlandscape_python/publication_type.py
--rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape-python-0.2.1/gwlandscape_python/settings.py
--rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape-python-0.2.1/gwlandscape_python/tests/__init__.py
--rw-r--r--   0        0        0    40147 2023-03-24 00:55:29.688335 gwlandscape-python-0.2.1/gwlandscape_python/tests/test_gwlandscape_python.py
--rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape-python-0.2.1/gwlandscape_python/tests/utils.py
--rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape-python-0.2.1/gwlandscape_python/utils/__init__.py
--rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape-python-0.2.1/gwlandscape_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape-python-0.2.1/gwlandscape_python/utils/utils.py
--rw-r--r--   0        0        0     1074 2023-03-27 03:08:09.591796 gwlandscape-python-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1661 2023-03-27 03:08:18.513932 gwlandscape-python-0.2.1/setup.py
--rw-r--r--   0        0        0     1618 2023-03-27 03:08:18.514550 gwlandscape-python-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape-python-0.3.0/LICENSE
+-rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape-python-0.3.0/README.rst
+-rw-r--r--   0        0        0       37 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5924 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-30 05:41:07.806853 gwlandscape-python-0.3.0/gwlandscape_python/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape-python-0.3.0/gwlandscape_python/__init__.py
+-rw-r--r--   0        0        0     2140 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/dataset_type.py
+-rw-r--r--   0        0        0    17763 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/gwlandscape.py
+-rw-r--r--   0        0        0     1578 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/keyword_type.py
+-rw-r--r--   0        0        0     1890 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/model_type.py
+-rw-r--r--   0        0        0     3771 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/publication_type.py
+-rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape-python-0.3.0/gwlandscape_python/settings.py
+-rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.0/gwlandscape_python/tests/__init__.py
+-rw-r--r--   0        0        0      176 2022-08-30 00:50:21.643802 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4499 2023-04-20 22:06:01.608362 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/conftest.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2887 2023-04-20 22:06:01.648362 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_dataset_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0    30447 2023-04-20 22:06:01.712363 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_gwlandscape_python.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2421 2023-04-20 22:06:01.784364 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_keyword_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2688 2023-04-20 22:06:01.788364 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_model_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     5177 2023-04-20 22:06:01.796364 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/test_publication_type.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0      374 2022-08-30 00:50:21.671802 gwlandscape-python-0.3.0/gwlandscape_python/tests/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     3052 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_dataset_type.py
+-rw-r--r--   0        0        0    36190 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_gwlandscape_python.py
+-rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_keyword_type.py
+-rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_model_type.py
+-rw-r--r--   0        0        0     4228 2023-04-20 04:41:39.760269 gwlandscape-python-0.3.0/gwlandscape_python/tests/test_publication_type.py
+-rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.0/gwlandscape_python/tests/utils.py
+-rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.0/gwlandscape_python/utils/__init__.py
+-rw-r--r--   0        0        0      249 2022-12-06 05:10:16.275674 gwlandscape-python-0.3.0/gwlandscape_python/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1786 2022-12-06 05:10:16.275674 gwlandscape-python-0.3.0/gwlandscape_python/utils/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0     3565 2022-12-08 23:27:42.059757 gwlandscape-python-0.3.0/gwlandscape_python/utils/tests/__pycache__/test_utils.cpython-38-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.0/gwlandscape_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape-python-0.3.0/gwlandscape_python/utils/utils.py
+-rw-r--r--   0        0        0     1074 2023-04-21 01:14:04.590655 gwlandscape-python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1732 2023-04-21 01:14:18.265159 gwlandscape-python-0.3.0/setup.py
+-rw-r--r--   0        0        0     1618 2023-04-21 01:14:18.265417 gwlandscape-python-0.3.0/PKG-INFO
```

### Comparing `gwlandscape-python-0.2.1/LICENSE` & `gwlandscape-python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.2.1/README.rst` & `gwlandscape-python-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.2.1/gwlandscape_python/gwlandscape.py` & `gwlandscape-python-0.3.0/gwlandscape_python/gwlandscape.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from pathlib import Path
 
 from gwdc_python import GWDC
 from gwdc_python.logger import create_logger
 
-from .dataset_type import Dataset
-from .keyword_type import Keyword
-from .model_type import Model
-from .publication_type import Publication
-from .utils import mutually_exclusive
-from .settings import GWLANDSCAPE_ENDPOINT, GWLANDSCAPE_AUTH_ENDPOINT
+import gwlandscape_python
+from gwlandscape_python.utils import mutually_exclusive
+from gwlandscape_python.settings import GWLANDSCAPE_ENDPOINT, GWLANDSCAPE_AUTH_ENDPOINT
 
 logger = create_logger(__name__)
 
 
 class GWLandscape:
     """
     GWLandscape class provides an API for interacting with COMPAS, allowing jobs to be submitted and acquired.
@@ -114,106 +111,95 @@
             'exact': exact,
             'contains': contains,
             'id': _id
         }
 
         result = self.request(query=query, variables=variables)
 
-        return [Keyword(**kw['node']) for kw in result['keywords']['edges']]
-
-    def delete_keyword(self, keyword):
-        """
-        Delete a keyword represented by the provided keyword.
-
-        Parameters
-        ----------
-        keyword: Keyword
-            The Keyword instance to delete
-        """
-
-        mutation = """
-            mutation DeleteKeywordMutation($input: DeleteKeywordMutationInput!) {
-                deleteKeyword(input: $input) {
-                    result
-                }
-            }
-        """
-
-        params = {
-            'input': {
-                'id': keyword.id
-            }
-        }
-
-        result = self.request(mutation, params)
-
-        assert result['delete_keyword']['result']
-
-    def create_publication(self, author, title, arxiv_id, **kwargs):
+        return [
+            gwlandscape_python.Keyword(client=self, **kw['node'])
+            for kw in result['keywords']['edges']
+        ]
+
+    def create_publication(
+        self,
+        author,
+        title,
+        arxiv_id,
+        published=None,
+        year=None,
+        journal=None,
+        journal_doi=None,
+        dataset_doi=None,
+        description=None,
+        public=None,
+        download_link=None,
+        keywords=None
+    ):
         """
         Creates a new keyword object with the specified tag.
 
         Parameters
         ----------
         author : str
             The author of the publication
         title : str
             The title of the publication
         arxiv_id : str
             The arxiv id of the publication
-        **kwargs : dict, optional
-            Extra keyword arguments that are provided to GWLandscape to create a publication.
-            Accepted keys are:
-
-            published: (`bool`)
-                If the publication was published in a journal/arXiv
-            year : (`int`)
-                The year of the publication
-            journal : (`str`)
-                The name of the journal
-            journal_doi : (`str`)
-                The DOI of the publication
-            dataset_doi : (`str`)
-                The DOI of the dataset
-            description : (`str`)
-                A description of the publication
-            public : (`bool`)
-                If the publication has been made public (visible to the public)
-            download_link : (`str`)
-                A link to download the publication/dataset
-            keywords : (`list`)
-                A list of str or :class:`~.Keyword` objects for the publication
+        published : bool, optional
+            If the publication was published in a journal/arXiv, by default None
+        year : int, optional
+            The year of the publication, by default None
+        journal : str, optional
+            The name of the journal, by default None
+        journal_doi : str, optional
+            The DOI of the publication, by default None
+        dataset_doi : str, optional
+            The DOI of the dataset, by default None
+        description : str, optional
+            A description of the publication, by default None
+        public : bool, optional
+            If the publication has been made public (visible to the public), by default None
+        download_link : str, optional
+            A link to download the publication/dataset, by default None
+        keywords : list, optional
+            A list of str or :class:`~.Keyword` objects for the publication, by default None
 
         Returns
         -------
         Publication
             Created Publication
         """
         mutation = """
             mutation AddPublicationMutation($input: AddPublicationMutationInput!) {
                 addPublication(input: $input) {
                     id
                 }
             }
         """
 
-        keywords = kwargs.pop('keywords', [])
-        assert isinstance(keywords, list), 'Keywords must be a list'
-
         params = {
             'input': {
                 'author': author,
                 'title': title,
                 'arxiv_id': arxiv_id,
-                **kwargs
+                'published': published,
+                'year': year,
+                'journal': journal,
+                'journal_doi': journal_doi,
+                'dataset_doi': dataset_doi,
+                'description': description,
+                'public': public,
+                'download_link': download_link
             }
         }
 
         # Handle keywords
-        if keywords:
+        if isinstance(keywords, list):
             params['input']['keywords'] = [
                 self.get_keywords(exact=keyword)[0].id if isinstance(keyword, str) else keyword.id
                 for keyword in keywords
             ]
 
         result = self.request(mutation, params)
 
@@ -287,45 +273,22 @@
             'id': _id
         }
 
         result = self.request(query=query, variables=variables)
 
         # Handle keywords
         for pub in result['compas_publications']['edges']:
-            pub['node']['keywords'] = [Keyword(**kw['node']) for kw in pub['node']['keywords']['edges']]
-
-        return [Publication(**kw['node']) for kw in result['compas_publications']['edges']]
-
-    def delete_publication(self, publication):
-        """
-        Delete a publication represented by the provided publication instance.
-
-        Parameters
-        ----------
-        publication: Publication
-            The Publication instance to delete
-        """
-
-        mutation = """
-            mutation DeletePublicationMutation($input: DeletePublicationMutationInput!) {
-                deletePublication(input: $input) {
-                    result
-                }
-            }
-        """
-
-        params = {
-            'input': {
-                'id': publication.id
-            }
-        }
-
-        result = self.request(mutation, params)
+            pub['node']['keywords'] = [
+                gwlandscape_python.Keyword(client=self, **kw['node']) for kw in pub['node']['keywords']['edges']
+            ]
 
-        assert result['delete_publication']['result']
+        return [
+            gwlandscape_python.Publication(client=self, **kw['node'])
+            for kw in result['compas_publications']['edges']
+        ]
 
     def create_model(self, name, summary=None, description=None):
         """
         Creates a new model object with the specified parameters.
 
         Parameters
         ----------
@@ -414,43 +377,18 @@
             'summary': summary,
             'description': description,
             'id': _id
         }
 
         result = self.request(query=query, variables=variables)
 
-        return [Model(**kw['node']) for kw in result['compas_models']['edges']]
-
-    def delete_model(self, model):
-        """
-        Delete a model represented by the provided model.
-
-        Parameters
-        ----------
-        model: Model
-            The Model instance to delete
-        """
-
-        mutation = """
-            mutation DeleteCompasModelMutation($input: DeleteCompasModelMutationInput!) {
-                deleteCompasModel(input: $input) {
-                    result
-                }
-            }
-        """
-
-        params = {
-            'input': {
-                'id': model.id
-            }
-        }
-
-        result = self.request(mutation, params)
-
-        assert result['delete_compas_model']['result']
+        return [
+            gwlandscape_python.Model(client=self, **kw['node'])
+            for kw in result['compas_models']['edges']
+        ]
 
     def create_dataset(self, publication, model, datafile):
         """
         Creates a new dataset object with the specified publication and model.
 
         Parameters
         ----------
@@ -563,53 +501,33 @@
         }
 
         result = self.request(query=query, variables=variables)
 
         # Handle publication and model objects
         for dataset in result['compas_dataset_models']['edges']:
             # Handle publication keywords
-            dataset['node']['compas_publication']['keywords'] = \
-                [Keyword(**kw['node']) for kw in dataset['node']['compas_publication']['keywords']['edges']]
+            dataset['node']['compas_publication']['keywords'] = [
+                gwlandscape_python.Keyword(client=self, **kw['node'])
+                for kw in dataset['node']['compas_publication']['keywords']['edges']
+            ]
 
-            dataset['node']['publication'] = Publication(**dataset['node']['compas_publication'])
-            dataset['node']['model'] = Model(**dataset['node']['compas_model'])
+            dataset['node']['publication'] = gwlandscape_python.Publication(
+                client=self,
+                **dataset['node']['compas_publication']
+            )
+            dataset['node']['model'] = gwlandscape_python.Model(client=self, **dataset['node']['compas_model'])
 
             # Delete the compas_ fields - we don't need them anymore
             del dataset['node']['compas_publication']
             del dataset['node']['compas_model']
 
-        return [Dataset(**kw['node']) for kw in result['compas_dataset_models']['edges']]
-
-    def delete_dataset(self, dataset):
-        """
-        Delete a dataset represented by the provided dataset.
-
-        Parameters
-        ----------
-        dataset: Dataset
-            The Dataset instance to delete
-        """
-
-        mutation = """
-            mutation DeleteCompasDatasetModelMutation($input: DeleteCompasDatasetModelMutationInput!) {
-                deleteCompasDatasetModel(input: $input) {
-                    result
-                }
-            }
-        """
-
-        params = {
-            'input': {
-                'id': dataset.id
-            }
-        }
-
-        result = self.request(mutation, params)
-
-        assert result['delete_compas_dataset_model']['result']
+        return [
+            gwlandscape_python.dataset_type.Dataset(client=self, **kw['node'])
+            for kw in result['compas_dataset_models']['edges']
+        ]
 
     def _generate_compas_dataset_model_upload_token(self):
         """Creates a new long lived upload token for use uploading compas publications
 
         Returns
         -------
         str
```

### Comparing `gwlandscape-python-0.2.1/gwlandscape_python/tests/test_gwlandscape_python.py` & `gwlandscape-python-0.3.0/gwlandscape_python/tests/test_gwlandscape_python.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,20 @@
 import uuid
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import pytest
 
-from gwlandscape_python import GWLandscape
-from gwlandscape_python.dataset_type import Dataset
 from gwlandscape_python.keyword_type import Keyword
 from gwlandscape_python.model_type import Model
 from gwlandscape_python.publication_type import Publication
 from gwlandscape_python.tests.utils import compare_graphql_query
 
 
 @pytest.fixture
-def setup_gwl_request(mocker):
-    def mock_init(self, token, auth_endpoint, endpoint):
-        pass
-
-    mock_request = mocker.Mock()
-    mocker.patch('gwlandscape_python.gwlandscape.GWDC.__init__', mock_init)
-    mocker.patch('gwlandscape_python.gwlandscape.GWDC.request', mock_request)
-
-    return GWLandscape(token='my_token'), mock_request
-
-
-@pytest.fixture
 def create_keyword_request(setup_gwl_request):
     response_data = [
         {
             "add_keyword": {
                 "id": "S2V5d29yZE5vZGU6MzA="
             }
         },
@@ -455,49 +441,20 @@
             'exact': None,
             'contains': None,
             'id': None
         }
     )
 
 
-def test_delete_keyword(setup_gwl_request):
-    gwl, mock_request = setup_gwl_request
-
-    mock_request.return_value = {
-        "delete_keyword": {
-            "result": True
-        }
-    }
-
-    keyword = Keyword(**{'tag': 'my_tag', 'id': 'S2V5d29yZE5vZGU6MzA='})
-
-    gwl.delete_keyword(keyword)
-
-    mock_request.assert_called_with(
-        """
-            mutation DeleteKeywordMutation($input: DeleteKeywordMutationInput!) {
-                deleteKeyword(input: $input) {
-                    result
-                }
-            }
-        """,
-        {
-            'input': {
-                'id': keyword.id
-            }
-        }
-    )
-
-
 def test_create_publication(create_publication_request):
     gw, mock_request = create_publication_request
 
     kws = [
-        Keyword('kw_id_1', 'keyword1'),
-        Keyword('kw_id_2', 'keyword2'),
+        Keyword(gw, 'kw_id_1', 'keyword1'),
+        Keyword(gw, 'kw_id_2', 'keyword2'),
     ]
 
     publication = gw.create_publication(
         'my author',
         'my publication',
         'an arxiv id',
         published=True,
@@ -642,16 +599,16 @@
 
     pub = gwl.get_publications(**kwargs)
     assert len(pub) == 1
 
     publication = pub[0]
 
     kws = [
-        Keyword('kw_id_1', 'keyword1'),
-        Keyword('kw_id_2', 'keyword2'),
+        Keyword(gwl, 'kw_id_1', 'keyword1'),
+        Keyword(gwl, 'kw_id_2', 'keyword2'),
     ]
 
     assert publication.id == 'Q29tcGFzUHVibGljYXRpb25Ob2RlOjUw'
     assert publication.author == 'my author'
     assert publication.title == 'my publication'
     assert publication.arxiv_id == 'an arxiv id'
     assert publication.published is True
@@ -815,58 +772,14 @@
 def test_get_publication_author_title_id(setup_gwl_request):
     gwl, mock_request = setup_gwl_request
 
     with pytest.raises(SyntaxError):
         get_publication(gwl, mock_request, author='test_author', title='test_title', _id='not_gonna_work')
 
 
-def test_delete_publication(setup_gwl_request):
-    gwl, mock_request = setup_gwl_request
-
-    mock_request.return_value = {
-        "delete_publication": {
-            "result": True
-        }
-    }
-
-    publication = Publication(**{
-        'id': 'Q29tcGFzUHVibGljYXRpb25Ob2RlOjUw',
-        'author': 'my author',
-        'published': True,
-        'title': 'my publication',
-        'year': 1234,
-        'journal': 'journal',
-        'journal_doi': 'journal doi',
-        'dataset_doi': 'dataset doi',
-        'creation_time': '2022-06-20T02:12:59.459297+00:00',
-        'description': 'my description',
-        'public': True,
-        'download_link': 'my download link',
-        'arxiv_id': 'an arxiv id',
-        'keywords': []
-    })
-
-    gwl.delete_publication(publication)
-
-    mock_request.assert_called_with(
-        """
-            mutation DeletePublicationMutation($input: DeletePublicationMutationInput!) {
-                deletePublication(input: $input) {
-                    result
-                }
-            }
-        """,
-        {
-            'input': {
-                'id': publication.id
-            }
-        }
-    )
-
-
 def test_create_model(create_model_request):
     gw, mock_request = create_model_request
 
     model = gw.create_model('my_name', 'my_summary', 'my_description')
 
     assert model.id == 'Q29tcGFzTW9kZWxOb2RlOjI='
     assert model.name == 'my_name'
@@ -1028,56 +941,20 @@
             name='test_name',
             summary='test_summary',
             description='test_description',
             _id='not_gonna_work'
         )
 
 
-def test_delete_model(setup_gwl_request):
-    gwl, mock_request = setup_gwl_request
-
-    mock_request.return_value = {
-        "delete_compas_model": {
-            "result": True
-        }
-    }
-
-    model = Model(
-        **{
-            'name': 'my_name',
-            'summary': 'my_summary',
-            'description': 'my_description',
-            'id': 'Q29tcGFzTW9kZWxOb2RlOjI='
-        }
-    )
-
-    gwl.delete_model(model)
-
-    mock_request.assert_called_with(
-        """
-            mutation DeleteCompasModelMutation($input: DeleteCompasModelMutationInput!) {
-                deleteCompasModel(input: $input) {
-                    result
-                }
-            }
-        """,
-        {
-            'input': {
-                'id': model.id
-            }
-        }
-    )
-
-
 def test_create_dataset(create_dataset_request, mock_publication_data):
     gw, mock_request = create_dataset_request
     publication_data, model_data = mock_publication_data
 
-    publication = Publication(**publication_data)
-    model = Model(**model_data)
+    publication = Publication(gw, **publication_data)
+    model = Model(gw, **model_data)
 
     with NamedTemporaryFile() as tf:
         dataset = gw.create_dataset(publication, model, Path(tf.name))
 
     assert dataset.id == 'Q29tcGFzRGF0YXNldE1vZGVsTm9kZTo3='
     assert dataset.files == ['test_file.h5']
 
@@ -1249,16 +1126,16 @@
     )
 
 
 def test_get_dataset_publication_model(setup_gwl_request, mock_publication_data):
     gwl, mock_request = setup_gwl_request
     publication_data, model_data = mock_publication_data
 
-    publication = Publication(**publication_data)
-    model = Model(**model_data)
+    publication = Publication(gwl, **publication_data)
+    model = Model(gwl, **model_data)
 
     get_dataset(gwl, mock_request, mock_publication_data, publication=publication, model=model)
 
     mock_request.assert_called_with(
         query="""
             query ($publication: ID, $model: ID, $id: ID) {
                 compasDatasetModels (compasPublication: $publication, compasModel: $model, id: $id) {
@@ -1308,57 +1185,19 @@
     )
 
 
 def test_get_dataset_publication_model_id(setup_gwl_request, mock_publication_data):
     gwl, mock_request = setup_gwl_request
     publication_data, model_data = mock_publication_data
 
-    publication = Publication(**publication_data)
-    model = Model(**model_data)
+    publication = Publication(gwl, **publication_data)
+    model = Model(gwl, **model_data)
 
     with pytest.raises(SyntaxError):
         get_dataset(
             gwl,
             mock_request,
             mock_publication_data,
             publication=publication,
             model=model,
             _id='not_gonna_work'
         )
-
-
-def test_delete_dataset(setup_gwl_request, mock_publication_data):
-    gwl, mock_request = setup_gwl_request
-    publication_data, model_data = mock_publication_data
-
-    mock_request.return_value = {
-        "delete_compas_dataset_model": {
-            "result": True
-        }
-    }
-
-    publication = Publication(**publication_data)
-    model = Model(**model_data)
-
-    dataset = Dataset(**{
-        'id': 'Q29tcGFzRGF0YXNldE1vZGVsTm9kZTo3=',
-        'publication': publication,
-        'model': model,
-        'files': ['my_file.h5']
-    })
-
-    gwl.delete_dataset(dataset)
-
-    mock_request.assert_called_with(
-        """
-            mutation DeleteCompasDatasetModelMutation($input: DeleteCompasDatasetModelMutationInput!) {
-                deleteCompasDatasetModel(input: $input) {
-                    result
-                }
-            }
-        """,
-        {
-            'input': {
-                'id': dataset.id
-            }
-        }
-    )
```

### Comparing `gwlandscape-python-0.2.1/gwlandscape_python/utils/tests/test_utils.py` & `gwlandscape-python-0.3.0/gwlandscape_python/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.2.1/gwlandscape_python/utils/utils.py` & `gwlandscape-python-0.3.0/gwlandscape_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.2.1/pyproject.toml` & `gwlandscape-python-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwlandscape-python"
-version = "0.2.1"
+version = "0.3.0"
 description = "Wrapper of GWDC API, used for interacting with the GWLandscape endpoints"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>", "Lewis Lakerink <llakerink@swin.edu.au"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwlandscape_python"
 include = ["LICENSE",]
```

### Comparing `gwlandscape-python-0.2.1/setup.py` & `gwlandscape-python-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 packages = \
 ['gwlandscape_python',
  'gwlandscape_python.tests',
  'gwlandscape_python.utils',
  'gwlandscape_python.utils.tests']
 
 package_data = \
-{'': ['*']}
+{'': ['*'],
+ 'gwlandscape_python': ['.pytest_cache/*', '.pytest_cache/v/cache/*']}
 
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
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'Wrapper of GWDC API, used for interacting with the GWLandscape endpoints',
     'long_description': "GWLandscape Python API\n======================\n\n`GWLandscape <https://gwlandscape.org.au/>`_ is a service used to handle both the submission of COMPAS jobs (todo)\n\nCheck out the `documentation <https://gwlandscape-python.readthedocs.io/en/latest/>`_ for more information.\n\nInstallation\n------------\n\nThe gwlandscape-python package can be installed with\n\n::\n\n    pip install gwlandscape-python\n\n\nExample\n-------\n\n::\n\n    >>> from gwlandscape_python import GWLandscape\n    >>> gwl = GWLandscape(token='<user_api_token_here>')\n\n",
     'author': 'Thomas Reichardt',
     'author_email': 'treichardt@swin.edu.au',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/gravitationalwavedc/gwlandscape_python',
```

### Comparing `gwlandscape-python-0.2.1/PKG-INFO` & `gwlandscape-python-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwlandscape-python
-Version: 0.2.1
+Version: 0.3.0
 Summary: Wrapper of GWDC API, used for interacting with the GWLandscape endpoints
 Home-page: https://github.com/gravitationalwavedc/gwlandscape_python
 License: MIT
 Author: Thomas Reichardt
 Author-email: treichardt@swin.edu.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

