# Comparing `tmp/bioturing-connector-1.1.1.tar.gz` & `tmp/bioturing-connector-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioturing-connector-1.1.1.tar", max compression
+gzip compressed data, was "bioturing-connector-1.2.0.tar", max compression
```

## Comparing `bioturing-connector-1.1.1.tar` & `bioturing-connector-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     4390 2022-10-11 16:34:14.735244 bioturing-connector-1.1.1/README.md
--rw-r--r--   0        0        0        0 2022-10-11 16:34:14.735376 bioturing-connector-1.1.1/bioturing_connector/__init__.py
--rw-r--r--   0        0        0      383 2023-03-05 03:05:20.458891 bioturing-connector-1.1.1/bioturing_connector/common/__init__.py
--rw-r--r--   0        0        0     1449 2023-03-05 03:05:20.460194 bioturing-connector-1.1.1/bioturing_connector/common/https_agent.py
--rw-r--r--   0        0        0    18956 2023-03-18 05:07:27.369182 bioturing-connector-1.1.1/bioturing_connector/connector.py
--rw-r--r--   0        0        0      309 2023-03-05 03:05:20.461458 bioturing-connector-1.1.1/bioturing_connector/typing/__init__.py
--rw-r--r--   0        0        0      444 2023-03-18 05:07:44.985059 bioturing-connector-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 bioturing-connector-1.1.1/setup.py
--rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 bioturing-connector-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4390 2022-10-11 16:34:14.735244 bioturing-connector-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2022-10-11 16:34:14.735376 bioturing-connector-1.2.0/bioturing_connector/__init__.py
+-rw-r--r--   0        0        0      383 2023-03-05 03:05:20.458891 bioturing-connector-1.2.0/bioturing_connector/common/__init__.py
+-rw-r--r--   0        0        0     4224 2023-04-21 15:38:26.637276 bioturing-connector-1.2.0/bioturing_connector/common/common.py
+-rw-r--r--   0        0        0     1449 2023-03-05 03:05:20.460194 bioturing-connector-1.2.0/bioturing_connector/common/https_agent.py
+-rw-r--r--   0        0        0    15367 2023-04-21 15:38:26.638203 bioturing-connector-1.2.0/bioturing_connector/connector.py
+-rw-r--r--   0        0        0    11963 2023-04-21 15:38:26.638453 bioturing-connector-1.2.0/bioturing_connector/lens_connector.py
+-rw-r--r--   0        0        0      347 2023-04-21 15:38:26.639452 bioturing-connector-1.2.0/bioturing_connector/typing/__init__.py
+-rw-r--r--   0        0        0      444 2023-04-21 15:38:42.224041 bioturing-connector-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5379 1970-01-01 00:00:00.000000 bioturing-connector-1.2.0/setup.py
+-rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 bioturing-connector-1.2.0/PKG-INFO
```

### Comparing `bioturing-connector-1.1.1/README.md` & `bioturing-connector-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bioturing-connector-1.1.1/bioturing_connector/common/https_agent.py` & `bioturing-connector-1.2.0/bioturing_connector/common/https_agent.py`

 * *Files identical despite different names*

### Comparing `bioturing-connector-1.1.1/bioturing_connector/connector.py` & `bioturing-connector-1.2.0/bioturing_connector/connector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """Python package for submitting/getting data from BBrowserX"""
 
-import time
-import requests
 import pandas as pd
-from scipy import sparse
-from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
-import json
-from datetime import datetime
 from pathlib import Path
-from tqdm import tqdm
 
 from urllib.parse import urljoin
 from typing import List
 from typing import Union
 
 from .common import get_uuid
 from .common import decode_base64_array
 
 from .common.https_agent import HttpsAgent
+from .common import common
 from .typing import Species
 from .typing import StudyType
 from .typing import InputMatrixType
 from .typing import UNIT_RAW
 
 class BBrowserXConnector:
   """Create a connector object to submit/get data from BBrowserX
@@ -36,107 +30,14 @@
           The API token to verify authority. Generated in-app.
     """
     self.__host = host
     self.__token = token
     self.__https_agent = HttpsAgent(self.__token, ssl)
 
 
-  def __check_result_status(self, result):
-    if not result:
-      raise ConnectionError('Connection failed')
-
-    if 'status' not in result:
-      raise ValueError(result['detail'])
-
-    if result['status'] != 200:
-      if 'message' in result:
-        raise Exception(f"Something went wrong: {result['message']}")
-      else:
-        raise Exception('Something went wrong')
-
-
-  def __parse_submission_status(self, submission_status):
-    """Parse submission status response
-    """
-    if not submission_status:
-      print('Connection failed')
-      return None
-
-    if 'status' not in submission_status:
-      print('Internal server error. Please check server log.')
-      return None
-
-    if submission_status['status'] != 200:
-      if 'message' in submission_status:
-        print(f"Submission failed. {submission_status['message']}")
-      else:
-        print('Submission failed.')
-      return None
-
-    return submission_status['data']['id']
-
-
-  def __get_submission_log(self, group_id: str, task_id: str):
-    last_status = []
-
-    while True:
-      submission_log = self.__https_agent.post(
-        url=urljoin(self.__host, 'api/v1/get_submission_log'),
-        body={'task_id': task_id}
-      )
-      if not submission_log or 'status' not in submission_log or \
-        submission_log['status'] != 200:
-        print('Internal server error. Please check server log.')
-        break
-
-      current_status = submission_log['data']['log'].split('\n')[:-1]
-      new_status = current_status[len(last_status):]
-      if len(new_status):
-        print('\n'.join(new_status))
-
-      last_status += new_status
-      if submission_log['data']['status'] != 'SUCCESS':
-        time.sleep(5)
-        continue
-      else:
-        res = self.__https_agent.post(
-          url=urljoin(self.__host, 'api/v1/commit_submission_result'),
-          body={
-            'group_id': group_id,
-            'task_id': task_id
-          }
-        )
-        if not res or 'status' not in res:
-          print('Internal server error. Please check server log.')
-          break
-
-        if res['status'] != 200:
-          if 'message' in res:
-            print(f"Connection failed. {res['message']}")
-          else:
-            print('Connection failed.')
-          break
-
-        print('Study submitted successfully!')
-        break
-
-
-  def __parse_query_genes_result(self, query_genes_result):
-    """Parse query genes result
-    """
-    self.__check_result_status(query_genes_result)
-
-    indptr = decode_base64_array(query_genes_result['data']['indptr'], 'uint64')
-    indices = decode_base64_array(query_genes_result['data']['indices'], 'uint32')
-    data = decode_base64_array(query_genes_result['data']['data'], 'float32')
-    shape = query_genes_result['data']['shape']
-    csc_mtx = sparse.csc_matrix((data, indices, indptr), shape=shape)
-    return csc_mtx
-
-
   def test_connection(self):
     """Test the connection with the host
     """
     url = urljoin(self.__host, 'api/v1/test_connection')
 
     print(f'Connecting to host at {url}')
     res = self.__https_agent.post(url=url)
@@ -157,56 +58,56 @@
         }, ...]
     """
     url = urljoin(self.__host, 'api/v1/get_user_groups')
 
     res = self.__https_agent.post(url=url)
     if res and 'status' in res and res['status'] == 200:
       return res['data']
-    raise Exception('''Something went wrong,
-    please contact support@bioturing.com''')
+    raise Exception('''Something went wrong, please contact support@bioturing.com''')
 
 
   def _submit_study(
     self,
     group_id: str,
     study_id: str = None,
     name: str = 'To be detailed',
-    authors: List[str] = None,
+    authors: List[str] = [],
     abstract: str = '',
     species: str = Species.HUMAN.value,
     input_matrix_type: str = InputMatrixType.NORMALIZED.value,
     study_type: int = StudyType.H5AD.value,
     min_counts: int = None,
     min_genes: int = None,
     max_counts: int = None,
     max_genes: int = None,
-    mt_percentage: Union[int, float] = None
+    mt_percentage: Union[int, float] = None,
+    skip_dimred: bool = False,
   ):
     if study_id is None:
       study_id = get_uuid()
 
     if min_counts is None:
       min_counts = 0
 
     if min_genes is None:
       min_genes = 0
 
     if max_counts is None:
-      max_counts = 5000000000000 # Really big number
+      max_counts = 1e9
 
     if max_genes is None:
-      max_genes = 5000000000000 # Really big number
+      max_genes = 1e9
 
     if mt_percentage is None:
       mt_percentage = 100
 
     study_info = {
       'study_hash_id': study_id,
       'name': name,
-      'authors': authors,
+      'authors': authors if authors else [],
       'abstract': abstract
     }
 
     return {
       'species': species,
       'group_id': group_id,
       'filter_params': {
@@ -215,50 +116,53 @@
         'max_counts': max_counts,
         'max_genes': max_genes,
         'mt_percentage': mt_percentage / 100
       },
       'study_type': study_type,
       'normalize': input_matrix_type == InputMatrixType.RAW.value,
       'subsample': -1,
+      'skip_dimred': skip_dimred,
       'study_info': study_info,
     }
 
 
   def submit_study_from_s3(
     self,
     group_id: str,
     batch_info: List[dict] = [],
     study_id: str = None,
     name: str = 'To be detailed',
-    authors: List[str] = None,
+    authors: List[str] = [],
     abstract: str = '',
     species: str = Species.HUMAN.value,
     input_matrix_type: str = InputMatrixType.NORMALIZED.value,
     study_type: int = StudyType.H5AD.value,
     min_counts: int = None,
     min_genes: int = None,
     max_counts: int = None,
     max_genes: int = None,
-    mt_percentage: Union[int, float] = None
+    mt_percentage: Union[int, float] = None,
+    skip_dimred: bool = False
   ):
     """Submit one or multiple scanpy objects.
       Args:
         group_id: ID of the group to submit the data to.
         batch_info: File path and batch name information. Exp: [{"name: "normal": "s3_folder/batch1.h5ad"}, {"name": "cancer": "s3_folder/batch2.h5ad"}]
         study_id: Study ID, if no value is specified, use a random uuidv4 string
         name: Name of the study.
         authors: Authors of the study.
         abstract: Abstract of the study.
         species: Species of the study.
+        skip_dirmed: Skip BioTuring pipline if set to True (only appliable when input is a scanpy/seurat object).
         input_matrix_type: If the value of this input is 'normalized',
           then the software will
           use slot 'X' from the scanpy object and does not apply normalization.
           If the value of this input is 'raw',then the software will
           use slot 'raw.X' from thescanpy object and apply log-normalization.
-        study_type: The format of the study, supports h5ad and rds.
+        study_type: The format of the study, supports: mtx, h5, h5ad, rds, tsv/csv.
         min_counts: Minimum number of counts required
           for a cell to pass filtering.
         min_genes: Minimum number of genes expressed required
           for a cell to pass filtering.
         max_counts: Maximum number of counts required
           for a cell to pass filtering.
         max_genes: Maximum number of genes expressed required
@@ -275,14 +179,15 @@
       input_matrix_type,
       study_type,
       min_counts,
       min_genes,
       max_counts,
       max_genes,
       mt_percentage,
+      skip_dimred,
     )
 
     if study_type == StudyType.MTX_10X.value:
       for i, o in enumerate(batch_info):
         name = o['matrix'].split('/')
         if len(name) == 1:
           o['name'] = f'Batch {i + 1}'
@@ -294,54 +199,58 @@
     data['batch_info'] = {f'Batch_{i}': o for i, o in enumerate(batch_info)}
 
     submission_status = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/submit_study_from_s3'),
       body=data
     )
 
-    task_id = self.__parse_submission_status(submission_status)
+    task_id = common.parse_submission_status(submission_status)
     if task_id is None:
       return
 
-    self.__get_submission_log(group_id=group_id, task_id=task_id)
+    common.get_submission_log(
+      group_id=group_id, task_id=task_id, https_agent=self.__https_agent, host=self.__host
+    )
     return
 
 
   def submit_study_from_local(
     self,
     group_id: str,
     batch_info: object,
     study_id: str = None,
     name: str = 'To be detailed',
-    authors: List[str] = None,
+    authors: List[str] = [],
     abstract: str = '',
     species: str = Species.HUMAN.value,
     input_matrix_type: str = InputMatrixType.NORMALIZED.value,
     study_type: int = StudyType.H5AD.value,
     min_counts: int = None,
     min_genes: int = None,
     max_counts: int = None,
     max_genes: int = None,
-    mt_percentage: Union[int, float] = None
+    mt_percentage: Union[int, float] = None,
+    skip_dimred: bool = False
   ):
     """Submit one or multiple scanpy objects.
       Args:
         group_id: ID of the group to submit the data to.
         batch_info: File path and batch name information. Exp: [{"name: "normal": "local_folder/batch1.h5ad"}, {"name": "cancer": "local_folder/batch2.h5ad"}].
         study_id: Study ID, if no value is specified, use a random uuidv4 string
         name: Name of the study.
         authors: Authors of the study.
         abstract: Abstract of the study.
         species: Species of the study.
+        skip_dirmed: Skip BioTuring pipline if set to True (only appliable when input is a scanpy/seurat object).
         input_matrix_type: If the value of this input is 'normalized',
           then the software will
           use slot 'X' from the scanpy object and does not apply normalization.
           If the value of this input is 'raw',then the software will
           use slot 'raw.X' from thescanpy object and apply log-normalization.
-        study_type: The format of the study, supports h5ad and rds.
+        study_type: The format of the study, supports: mtx, h5, h5ad, rds, tsv/csv.
         min_counts: Minimum number of counts required
           for a cell to pass filtering.
         min_genes: Minimum number of genes expressed required
           for a cell to pass filtering.
         max_counts: Maximum number of counts required
           for a cell to pass filtering.
         max_genes: Maximum number of genes expressed required
@@ -366,78 +275,49 @@
     else:
       for o in batch_info:
         p = Path(o['matrix'])
         o['name'] = p.name
         file_names.append(p.name)
         files.append(p)
 
-    dir_id = get_uuid()
-    output_dir = ''
-    for file_name, file in zip(file_names, files):
-      total_size = file.stat().st_size
-      with tqdm(
-        desc=file_name, total=total_size, unit='MB',  unit_scale=True, unit_divisor=1024,
-      ) as bar:
-        fields = {
-          'params': json.dumps({
-            'name': file_name,
-            'file_id': dir_id,
-            'group_id': group_id,
-            'study_type': study_type,
-          }),
-          'file': (file_name, open(file, 'rb'))
-        }
-
-        encoder = MultipartEncoder(fields=fields)
-        multipart = MultipartEncoderMonitor(
-          encoder, lambda monitor: bar.update(monitor.bytes_read - bar.n)
-        )
-        headers = {
-          'Content-Type': multipart.content_type,
-          'bioturing-api-token': self.__token
-        }
-        response = requests.post(
-          urljoin(self.__host, 'api/v1/upload'),
-          data=multipart,
-          headers=headers
-        ).json()
-        if not response:
-          raise Exception('Something went wrong')
-        if 'status' not in response or response['status'] != 200:
-          raise Exception(response)
-        output_dir = response['data']
 
+    output_dir = common.upload_local(
+      file_names, files, group_id, study_type, self.__token, self.__host
+    )
     data = self._submit_study(
       group_id,
       study_id,
       name,
       authors,
       abstract,
       species,
       input_matrix_type,
       study_type,
       min_counts,
       min_genes,
       max_counts,
       max_genes,
       mt_percentage,
+      skip_dimred,
     )
     data['study_path'] = output_dir
     data['batch_info'] = [o['name'] for o in batch_info]
 
     submission_status = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/submit_study_from_local'),
       body=data
     )
 
-    task_id = self.__parse_submission_status(submission_status)
+    task_id = common.parse_submission_status(submission_status)
     if task_id is None:
       return
 
-    self.__get_submission_log(group_id=group_id, task_id=task_id)
+    common.get_submission_log(
+      group_id=group_id, task_id=task_id, https_agent=self.__https_agent, host=self.__host
+    )
     return
 
 
   def query_genes(
     self,
     species: str,
     study_id: str,
@@ -467,15 +347,15 @@
       'gene_names': gene_names,
       'unit': unit
     }
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/study/query_genes'),
       body=data
     )
-    return self.__parse_query_genes_result(result)
+    return common.parse_query_genes_result(result)
 
 
   def get_metadata(
     self,
     species: str,
     study_id: str
   ):
@@ -495,15 +375,15 @@
       'species': species,
       'study_id': study_id
     }
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/study/get_metadata'),
       body=data
     )
-    self.__check_result_status(result)
+    common.check_result_status(result)
     metadata_dict = result['data']
     metadata_df = pd.DataFrame(metadata_dict)
     return metadata_df
 
 
   def get_barcodes(
     self,
@@ -526,15 +406,15 @@
       'species': species,
       'study_id': study_id
     }
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/study/get_barcodes'),
       body=data
     )
-    self.__check_result_status(result)
+    common.check_result_status(result)
     return result['data']
 
 
   def get_features(
     self,
     species: str,
     study_id: str
@@ -555,15 +435,15 @@
       'species': species,
       'study_id': study_id
     }
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/study/get_features'),
       body=data
     )
-    self.__check_result_status(result)
+    common.check_result_status(result)
     return result['data']
 
 
   def get_all_studies_info_in_group(
     self,
     species: str,
     group_id: str
@@ -591,15 +471,15 @@
       'species': species,
       'group_id': group_id
     }
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/get_all_studies_info_in_group'),
       body=data
     )
-    self.__check_result_status(result)
+    common.check_result_status(result)
     return result['data']
 
 
   def list_all_custom_embeddings(
     self,
     species: str,
     study_id: str
@@ -625,15 +505,15 @@
       'species': species,
       'study_id': study_id
     }
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/list_all_custom_embeddings'),
       body=data
     )
-    self.__check_result_status(result)
+    common.check_result_status(result)
     return result['data']
 
 
   def retrieve_custom_embedding(
     self,
     species: str,
     study_id: str,
@@ -658,11 +538,11 @@
       'study_id': study_id,
       'embedding_id': embedding_id
     }
     result = self.__https_agent.post(
       url=urljoin(self.__host, 'api/v1/retrieve_custom_embedding'),
       body=data
     )
-    self.__check_result_status(result)
+    common.check_result_status(result)
     coord_arr = result['data']['coord_arr']
     coord_shape = result['data']['coord_shape']
     return decode_base64_array(coord_arr, 'float32', coord_shape)
```

### Comparing `bioturing-connector-1.1.1/setup.py` & `bioturing-connector-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {'': ['*']}
 
 install_requires = \
 ['mypy>=0.982,<0.983', 'pylint>=2.15.3,<3.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bioturing-connector',
-    'version': '1.1.1',
+    'version': '1.2.0',
     'description': 'A set of python modules for accessing BBrowserX on private server',
     'long_description': '## 1. Installation:\n```\n  pip install bioturing_connector --index-url=https://pypi.bioturing.com\n\n  # Username: bioturing\n  # Password: code@bioturing.com\n```\n\n## 2. Usage:\n**The package only allows data submission via Amazon S3 Bucket. Please configure your S3 Bucket credentials in the `Settings` page.**\n### 2.1. Test the connection:\n```\n# example.py\n\nfrom bioturing_connector.connector import BBrowserXConnector\n\nconnector = BBrowserXConnector(\n  host="https://yourcompany/t2d_index_tool/,\n  token="<input your token here>"\n)\n\nconnector.test_connection()\n```\n\nExample output:\n\n```\nConnecting to host at https://yourcompany/t2d_index_tool/api/v1/test_connection\nConnection successful\n```\n\n### 2.2. Get user groups available for your token:\n```\n# example.py\n\nfrom bioturing_connector.connector import BBrowserXConnector\n\nconnector = BBrowserXConnector(\n  host="https://yourcompany/t2d_index_tool/,\n  token="<input your token here>"\n)\n\nuser_groups = connector.get_user_groups()\nprint(user_groups)\n```\n\nExample output:\n\n```\n[{\'id\': \'all_members\', \'name\': \'All members\'}, {\'id\': \'personal\', \'name\': \'Personal workspace\'}]\n```\n\n### 2.3. Submit h5ad (scanpy object):\n```\n# example.py\nfrom bioturing_connector.connector import BBrowserXConnector\nfrom bioturing_connector.typing import InputMatrixType\nfrom bioturing_connector.typing import Species\n\nconnector = BBrowserXConnector(\n  host="https://yourcompany/t2d_index_tool/,\n  token="<input your token here>"\n)\n\n# Call this function first to get available groups and their id.\nuser_groups = connector.get_user_groups()\n# Example: user_groups is now [{\'id\': \'all_members\', \'name\': \'All members\'}, {\'id\': \'personal\', \'name\': \'Personal workspace\'}]\n\n\n# Submitting the scanpy object:\nconnector.submit_h5ad(\n  group_id=\'personal\',\n  study_s3_keys=[\'GSE128223.h5ad\'],\n  study_id=\'GSE128223\',\n  name=\'This is my first study\',\n  authors=[\'Huy Nguyen\'],\n  species=Species.HUMAN.value,\n  input_matrix_type=InputMatrixType.RAW.value\n)\n\n# Example output:\n> [2022-10-10 01:03] Waiting in queue\n> [2022-10-10 01:03] Downloading GSE128223.h5ad from s3: 262.1 KB / 432.8 MB\n> [2022-10-10 01:03] File downloaded\n> [2022-10-10 01:03] Reading batch: GSE128223.h5ad\n> [2022-10-10 01:03] Preprocessing expression matrix: 19121 cells x 63813 genes\n> [2022-10-10 01:03] Filtered: 19121 cells remain\n> [2022-10-10 01:03] Start processing study\n> [2022-10-10 01:03] Normalizing expression matrix\n> [2022-10-10 01:03] Running PCA\n> [2022-10-10 01:03] Running kNN\n> [2022-10-10 01:03] Running spectral embedding\n> [2022-10-10 01:03] Running venice binarizer\n> [2022-10-10 01:04] Running t-SNE\n> [2022-10-10 01:04] Study was successfully submitted\n> [2022-10-10 01:04] DONE !!!\n> Study submitted successfully!\n```\nAvailable parameters for `submit_h5ad` function:\n```\ngroup_id: str\n  ID of the group to submit the data to.\n\nstudy_s3_keys: List[str]\n  List of the s3 key of the studies.\n\nstudy_id: str, default=None\n  Study ID, if no value is specified, use a random uuidv4 string\n\nname: str, default=\'To be detailed\'\n  Name of the study.\n\nauthors: List[str], default=[]\n  Authors of the study.\n\nabstract: str, default=\'\'\n  Abstract of the study.\n\nspecies: str, default=\'human\'\n  Species of the study. Can be: **bioturing_connector.typing.Species.HUMAN.value** or **bioturing_connector.typing.Species.MOUSE.value** or **bioturing_connector.typing.Species.NON_HUMAN_PRIMATE.value**\n\ninput_matrix_type: str, default=\'raw\'\n  If the value of this input is **bioturing_connector.typing.InputMatrixType.NORMALIZED.value**,\n  then the software will\n  use slot \'X\' from the scanpy object and does not apply normalization.\n  If the value of this input is **bioturing_connector.typing.InputMatrixType.RAW.value**,then the software will\n  use slot \'raw.X\' from thescanpy object and apply log-normalization.\n\nmin_counts: int, default=None\n  Minimum number of counts required\n  for a cell to pass filtering.\n\nmin_genes: int, default=None\n  Minimum number of genes expressed required\n  for a cell to pass filtering.\n\nmax_counts: int, default=None\n  Maximum number of counts required\n  for a cell to pass filtering.\n\nmax_genes: int, default=None\n  Maximum number of genes expressed required\n  for a cell to pass filtering.\n\nmt_percentage: Union[int, float], default=None\n  Maximum number of mitochondria genes percentage\n  required for a cell to pass filtering. Ranging from 0 to 100\n```\n',
     'author': 'BioTuring',
     'author_email': 'support@bioturing.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bioturing-connector-1.1.1/PKG-INFO` & `bioturing-connector-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioturing-connector
-Version: 1.1.1
+Version: 1.2.0
 Summary: A set of python modules for accessing BBrowserX on private server
 Author: BioTuring
 Author-email: support@bioturing.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

