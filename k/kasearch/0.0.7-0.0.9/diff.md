# Comparing `tmp/kasearch-0.0.7.tar.gz` & `tmp/kasearch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kasearch-0.0.7.tar", last modified: Mon Aug 29 12:57:02 2022, max compression
+gzip compressed data, was "kasearch-0.0.9.tar", last modified: Mon Oct 24 14:35:45 2022, max compression
```

## Comparing `kasearch-0.0.7.tar` & `kasearch-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwx------   0 olsen    (10273) rstudent (30003)        0 2022-08-29 12:57:02.988123 kasearch-0.0.7/
--rw-------   0 olsen    (10273) rstudent (30003)     2387 2022-08-29 12:57:02.988123 kasearch-0.0.7/PKG-INFO
--rwx------   0 olsen    (10273) rstudent (30003)     2119 2022-08-22 14:48:07.000000 kasearch-0.0.7/README.md
-drwx------   0 olsen    (10273) rstudent (30003)        0 2022-08-29 12:57:02.987123 kasearch-0.0.7/kasearch/
--rwx------   0 olsen    (10273) rstudent (30003)      180 2022-06-20 16:09:57.000000 kasearch-0.0.7/kasearch/__init__.py
--rwx------   0 olsen    (10273) rstudent (30003)     4768 2022-08-22 14:34:47.000000 kasearch-0.0.7/kasearch/canonical_alignment.py
--rwx------   0 olsen    (10273) rstudent (30003)     4174 2022-08-22 14:34:47.000000 kasearch-0.0.7/kasearch/identity_calculations.py
--rw-------   0 olsen    (10273) rstudent (30003)     2341 2022-08-22 13:12:29.000000 kasearch-0.0.7/kasearch/initiate_db.py
--rwx------   0 olsen    (10273) rstudent (30003)     5303 2022-08-22 14:34:47.000000 kasearch-0.0.7/kasearch/kasearch.py
--rw-------   0 olsen    (10273) rstudent (30003)     1710 2022-06-20 16:09:57.000000 kasearch-0.0.7/kasearch/merge_db.py
--rw-------   0 olsen    (10273) rstudent (30003)     2408 2022-08-22 14:34:47.000000 kasearch-0.0.7/kasearch/meta_extract.py
--rw-------   0 olsen    (10273) rstudent (30003)     5978 2022-08-01 17:11:33.000000 kasearch-0.0.7/kasearch/prepare_db.py
--rw-------   0 olsen    (10273) rstudent (30003)     1554 2022-08-01 23:21:52.000000 kasearch-0.0.7/kasearch/prepare_query.py
--rwx------   0 olsen    (10273) rstudent (30003)     2304 2022-08-01 14:15:50.000000 kasearch-0.0.7/kasearch/species_anarci.py
-drwx------   0 olsen    (10273) rstudent (30003)        0 2022-08-29 12:57:02.988123 kasearch-0.0.7/kasearch.egg-info/
--rw-------   0 olsen    (10273) rstudent (30003)     2387 2022-08-29 12:57:02.000000 kasearch-0.0.7/kasearch.egg-info/PKG-INFO
--rw-------   0 olsen    (10273) rstudent (30003)      431 2022-08-29 12:57:02.000000 kasearch-0.0.7/kasearch.egg-info/SOURCES.txt
--rw-------   0 olsen    (10273) rstudent (30003)        1 2022-08-29 12:57:02.000000 kasearch-0.0.7/kasearch.egg-info/dependency_links.txt
--rw-------   0 olsen    (10273) rstudent (30003)       40 2022-08-29 12:57:02.000000 kasearch-0.0.7/kasearch.egg-info/requires.txt
--rw-------   0 olsen    (10273) rstudent (30003)        9 2022-08-29 12:57:02.000000 kasearch-0.0.7/kasearch.egg-info/top_level.txt
--rw-------   0 olsen    (10273) rstudent (30003)       38 2022-08-29 12:57:02.988123 kasearch-0.0.7/setup.cfg
--rwx------   0 olsen    (10273) rstudent (30003)      747 2022-08-29 12:56:06.000000 kasearch-0.0.7/setup.py
+drwx------   0 olsen    (10273) rstudent (30003)        0 2022-10-24 14:35:45.776567 kasearch-0.0.9/
+-rw-------   0 olsen    (10273) rstudent (30003)     4405 2022-10-24 14:35:45.776567 kasearch-0.0.9/PKG-INFO
+-rwx------   0 olsen    (10273) rstudent (30003)     4136 2022-10-13 14:53:27.000000 kasearch-0.0.9/README.md
+drwx------   0 olsen    (10273) rstudent (30003)        0 2022-10-24 14:35:45.775567 kasearch-0.0.9/kasearch/
+-rwx------   0 olsen    (10273) rstudent (30003)      287 2022-10-13 14:09:20.000000 kasearch-0.0.9/kasearch/__init__.py
+-rw-------   0 olsen    (10273) rstudent (30003)     3736 2022-10-13 14:09:20.000000 kasearch-0.0.9/kasearch/align_sequences.py
+-rwx------   0 olsen    (10273) rstudent (30003)     5330 2022-10-06 12:02:30.000000 kasearch-0.0.9/kasearch/canonical_alignment.py
+-rw-------   0 olsen    (10273) rstudent (30003)     1901 2022-10-06 12:02:30.000000 kasearch-0.0.9/kasearch/easy_search.py
+-rwx------   0 olsen    (10273) rstudent (30003)     5392 2022-10-06 12:09:46.000000 kasearch-0.0.9/kasearch/identity_calculations.py
+-rw-------   0 olsen    (10273) rstudent (30003)     2341 2022-09-16 13:24:19.000000 kasearch-0.0.9/kasearch/initiate_db.py
+-rwx------   0 olsen    (10273) rstudent (30003)     6773 2022-10-13 14:09:20.000000 kasearch-0.0.9/kasearch/kasearch.py
+-rw-------   0 olsen    (10273) rstudent (30003)     2657 2022-09-14 15:46:14.000000 kasearch-0.0.9/kasearch/merge_db.py
+-rw-------   0 olsen    (10273) rstudent (30003)     2418 2022-10-06 12:24:32.000000 kasearch-0.0.9/kasearch/meta_extract.py
+-rw-------   0 olsen    (10273) rstudent (30003)     5706 2022-10-13 14:09:20.000000 kasearch-0.0.9/kasearch/prepare_db.py
+-rwx------   0 olsen    (10273) rstudent (30003)     3179 2022-10-13 14:09:20.000000 kasearch-0.0.9/kasearch/species_anarci.py
+drwx------   0 olsen    (10273) rstudent (30003)        0 2022-10-24 14:35:45.775567 kasearch-0.0.9/kasearch.egg-info/
+-rw-------   0 olsen    (10273) rstudent (30003)     4405 2022-10-24 14:35:45.000000 kasearch-0.0.9/kasearch.egg-info/PKG-INFO
+-rw-------   0 olsen    (10273) rstudent (30003)      457 2022-10-24 14:35:45.000000 kasearch-0.0.9/kasearch.egg-info/SOURCES.txt
+-rw-------   0 olsen    (10273) rstudent (30003)        1 2022-10-24 14:35:45.000000 kasearch-0.0.9/kasearch.egg-info/dependency_links.txt
+-rw-------   0 olsen    (10273) rstudent (30003)       40 2022-10-24 14:35:45.000000 kasearch-0.0.9/kasearch.egg-info/requires.txt
+-rw-------   0 olsen    (10273) rstudent (30003)        9 2022-10-24 14:35:45.000000 kasearch-0.0.9/kasearch.egg-info/top_level.txt
+-rw-------   0 olsen    (10273) rstudent (30003)       38 2022-10-24 14:35:45.776567 kasearch-0.0.9/setup.cfg
+-rwx------   0 olsen    (10273) rstudent (30003)      747 2022-10-13 14:47:50.000000 kasearch-0.0.9/setup.py
```

### Comparing `kasearch-0.0.7/kasearch/canonical_alignment.py` & `kasearch-0.0.9/kasearch/canonical_alignment.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,60 +54,89 @@
 # SEQUENCES ARE NUMBERED USING IMGT NUMBERING
 reg_def = dict()
 reg_def["CDR1"] = list(range(27, 38 + 1))
 reg_def["CDR2"] = list(range(56, 65 + 1))
 reg_def["CDR3"] = list(range(105, 117 + 1))
 reg_def["CDR_all"] = reg_def["CDR1"] + reg_def["CDR2"] + reg_def["CDR3"]
 
-cdr3_mask = np.array([int(canonical_numbering[i][:-1]) in reg_def["CDR3"] for i in range(len(canonical_numbering))], dtype = np.int8)
+cdr3_mask = np.array([int(canonical_numbering[i][:-1]) in reg_def["CDR3"] for i in range(len(canonical_numbering))], dtype = np.uint8)
 all_cdrs_mask = np.array(
-    [int(canonical_numbering[i][:-1]) in reg_def["CDR_all"] for i in range(len(canonical_numbering))], dtype = np.int8)
+    [int(canonical_numbering[i][:-1]) in reg_def["CDR_all"] for i in range(len(canonical_numbering))], dtype = np.uint8)
 
 
 def get_region_mask(region):
-    """
-    Get mask for a specific region.
-    """
+    """Retrieve mask for a specific region.
+    
+    Parameters
+    ----------
+    region : list
+        List of unique positions from the canonical alignment to not mask
+
+    Returns
+    -------
+    numpy array
+        Specific region mask
+    """     
     
     if region == 'whole':
-        return np.ones(200, dtype = np.int8)
+        return np.ones(200, dtype = np.uint8)
     elif region == 'cdrs':
         return all_cdrs_mask
     elif region == 'cdr3':
         return cdr3_mask
     else:
         assert np.all([i in canonical_numbering for i in region]), "At least one position in the user defined region, is not part of the 200 used positions. \
         Please remove such positions."
-        return np.array([i in region for i in canonical_numbering], dtype = np.int8)
+        return np.array([i in region for i in canonical_numbering], dtype = np.uint8)
 
 
 def canonical_alignment(anarci_output):
-    """
-    Alignment of anarci output
+    """Alignment of ANARCI output.
+    
+    Parameters
+    ----------
+    anarci_output : dict
+        ANARCI numbering of a sequence
+
+    Returns
+    -------
+    numpy array
+        Canonical alignment of a sequence
     """
 
     sequence = np.zeros(canonical_numbering_len, np.int8)
 
     for res in anarci_output:
         num, seq = res
         num = ''.join([str(i) for i in num])
 
         i = canonical_numbering_to_index[num]
         sequence[i] = int.from_bytes(seq.encode(), 'big')
 
     sequence[(sequence == 45)] = 0
     return sequence
 
+
 oas_numbering_finder = re.compile('\d+.\'\: \'[A-Z]')
 def canonical_alignment_oas(anarci_output):
+    """OAS derived ANARCI output.
+    
+    Parameters
+    ----------
+    anarci_output : dict
+        OAS derived ANARCI numbering of a sequence
+
+    Returns
+    -------
+    numpy array
+        Canonical alignment of a sequence
     """
-    OAS has a different anarci output.
-    """
+    
     sequence = np.zeros(canonical_numbering_len, np.int8)
 
     for res in oas_numbering_finder.findall(anarci_output):
         num, seq = res[:-5], res[-1]
         i = canonical_numbering_to_index[num]
         sequence[i] = int.from_bytes(seq.encode(), 'big')
 
     sequence[(sequence == 45)] = 0
-    return sequence
+    return
```

### Comparing `kasearch-0.0.7/kasearch/initiate_db.py` & `kasearch-0.0.9/kasearch/initiate_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         if database_path == 'oasdb-small': # Download a small version of OAS
             db_folder = os.path.join(os.path.dirname(__file__), "oasdb")
             os.makedirs(db_folder, exist_ok = True)
             
             if not glob.glob(os.path.join(db_folder, "oasdb_small*")):
                 print("Downloading a small version of OAS (4.4GB) ...")
                 
-                url = "https://zenodo.org/record/6668747/files/oasdb_small.tar"
+                url = "https://zenodo.org/record/7079547/files/oasdb_small.tar"
                 tmp_file = os.path.join(db_folder, "tmp.tar")
 
                 with open(tmp_file,'wb') as f: f.write(requests.get(url).content)
                 
                 subprocess.run(["tar", "-xf", tmp_file, "-C", db_folder], check = True) 
                 os.remove(tmp_file)
```

### Comparing `kasearch-0.0.7/kasearch/kasearch.py` & `kasearch-0.0.9/kasearch/kasearch.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,21 +6,40 @@
 
 from kasearch.identity_calculations import get_n_most_identical_multiquery, slow_get_n_most_identical
 from kasearch.meta_extract import ExtractMetadata
 from kasearch.initiate_db import InitiateDatabase
 from kasearch.canonical_alignment import get_region_mask
 
 class SearchDB(InitiateDatabase, ExtractMetadata):
+    """
+    The main class for searching and retrieving meta data with KA-Search. 
+
+    ...
+
+    Attributes
+    ----------
+    current_best_identities : array_like
+        Array of the ordered closest identities
+    files_to_search_normal : list of str
+        List of files that will be searched
+
+    Methods
+    -------
+    search(query, keep_best_n=10)
+        Search files in files_to_search_normal with query
+    get_meta(n_query = 0, n_region = 0, n_sequences = 'all', n_jobs = 1)
+        Retrieve meta data for n_query spanning n_region and returning n_sequences
+    """
+    
     def __init__(self, 
                  database_path='oasdb-small', 
                  allowed_chain='Any', 
                  allowed_species='Any',
                  regions=['whole', 'cdrs', 'cdr3'],
                  length_matched=[False,True,True],
-                 id_to_study_file=None,
                 ):
         super().__init__()
         
         self.region_masks = np.stack([get_region_mask(region) for region in regions])
         self.length_matched = np.array(length_matched, dtype = bool)
         assert self.region_masks.shape[0] == self.length_matched.shape[0], "List of user-defined regions ({}) and 'if length match' ({})\
  are of different lengths. Please define a 'if length match' for each defined region.".format(self.region_masks.shape[0], self.length_matched.shape[0])
@@ -33,70 +52,91 @@
         assert len(self.files_to_search_normal) != 0, "DB does not contain data of {} chains from the {} species.".format(allowed_chain, allowed_species)
     
     def __reset_current_best(self, qsize=1):
         """
         Resets currently most similar sequences.
         """
         
-        self._current_target_numbering = None
-        self._current_target_ids = None
         self.current_best_identities = np.zeros((qsize, 1, self.region_masks.shape[0]), np.float16) - 1
         self.current_best_ids = np.zeros((qsize, 1, self.region_masks.shape[0], 2), np.int32) - 1
 
-    def __update_best(self, query, keep_best_n):
+    def __update_best(self, query, _current_target_numbering, _current_target_ids, keep_best_n):
         """
         Update the current most similar sequences.
         """
         
         chunk_best_identities, chunk_best_ids = get_n_most_identical_multiquery(query,
-                                                                                self._current_target_numbering,
-                                                                                self._current_target_ids, 
+                                                                                _current_target_numbering,
+                                                                                _current_target_ids, 
                                                                                 n=keep_best_n,
                                                                                 region_masks=self.region_masks, 
                                                                                 length_matched=self.length_matched
                                                                                )
         
+        
         all_identities = np.concatenate([chunk_best_identities, self.current_best_identities], axis=1)
         all_ids = np.concatenate([chunk_best_ids, self.current_best_ids], axis=1)
 
         order = np.argsort(-all_identities, axis=1)
 
         self.current_best_identities = np.take_along_axis(all_identities, order, axis=1)[:, :keep_best_n]
-        self.current_best_ids = np.take_along_axis(all_ids, order[:, :, :, None], axis=1)[:, :keep_best_n]
+        self.current_best_ids = np.take_along_axis(all_ids, order[:, :, :, None], axis=1)[:, :keep_best_n]        
         
     def search(self, query, keep_best_n=10):
-        """
-        Search database for sequences most similar to the queries.
+        """Search database for sequences most similar to the queries.
+        
+        Parameters
+        ----------
+        query : str
+            Antibody sequence to search with
+        keep_best_n : int
+            Number of closest matches to return (default is 10)
         """
         
         self.__reset_current_best(query.shape[0])
 
         data_loader = DataLoader(self.files_to_search_normal[0])
-        self._current_target_numbering = data_loader.data['numberings']
-        self._current_target_ids = data_loader.data['idxs']
+        _current_target_numbering, _current_target_ids = data_loader.data['numberings'], data_loader.data['idxs']
+        
+        keep_best_n = min(keep_best_n, _current_target_numbering.shape[0] - 1) # If trying to keep more than available targets, it breaks
+        
         
         for file in self.files_to_search_normal[1:]:
             data_loader = DataLoader(file)
-            self.__update_best(query, keep_best_n)
-            self._current_target_numbering = data_loader.data['numberings']
-            self._current_target_ids = data_loader.data['idxs']
+            self.__update_best(query, _current_target_numbering, _current_target_ids, keep_best_n)
+            _current_target_numbering, _current_target_ids = data_loader.data['numberings'], data_loader.data['idxs']
                 
-        self.__update_best(query, keep_best_n)
+        self.__update_best(query, _current_target_numbering, _current_target_ids, keep_best_n)
         
     def get_meta(self, n_query = 0, n_region = 0, n_sequences = 'all', n_jobs=1):
-        """
-        Get meta data for the current most similar sequences for a specific query and region.
+        """Retrieve meta data for the current closest sequences for a specific query and region.
+        
+        Parameters
+        ----------
+        n_query : int
+            The index of the query to extract meta data for
+        n_region : int
+            The index of the region to extract meta data for
+        n_sequences : int, str
+            The number of sequences to return, or 'all' for all
+        n_jobs : int
+            The number of threads to use
+
+        Returns
+        -------
+        pandas dataframe
+            A pandas dataframe with the keep_best_n closest sequences, and their meta data, to the specified query and region
         """
         
         if n_sequences == 'all':
             n_sequences = self.current_best_identities.shape[1]
             
         assert n_query >= 0
         assert n_region >= 0
-        assert n_sequences > 0
+        assert n_sequences > 0        
         
         metadf = self._extract_meta(self.current_best_ids[n_query, :n_sequences, n_region], n_jobs=n_jobs)
         metadf['Identity'] = self.current_best_identities[n_query, :n_sequences, n_region]
         return metadf
```

### Comparing `kasearch-0.0.7/kasearch/meta_extract.py` & `kasearch-0.0.9/kasearch/meta_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,24 +28,26 @@
         unique_studies, split = np.unique(idxs_ordered_by_study[:, 0], return_index=True)
         return np.split(idxs_ordered_by_study, split[1:])
     
     def _get_single_study_meta(self, idxs):
         """
         Get meta for all ids from a given study.
         """
+        
         study_id = idxs[0,0]
+        
         study_file = self.id_to_study[study_id]
         line_ids = idxs[:,1]
 
         sequence_meta = pd.Series(json.loads(','.join(pd.read_csv(study_file, nrows=0).columns)))
         sequence_data = pd.read_csv(study_file, 
                             header=1, 
                             skiprows=[x+2 for x in range(line_ids.max()) if x not in line_ids], 
                             nrows=len(line_ids))
-        
+
         for key in sequence_meta.keys():
             sequence_data[key] = sequence_meta[key]
         sequence_data["rank"] = idxs[np.argsort(line_ids)][:,-1]
         
         return sequence_data
         
     def _extract_meta(self, idxs, n_jobs=1):
```

### Comparing `kasearch-0.0.7/kasearch/prepare_db.py` & `kasearch-0.0.9/kasearch/prepare_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,145 +1,140 @@
 import os
 import uuid
+import collections
 from dataclasses import dataclass
 from multiprocessing import Pool
 
 import numpy as np
+import pandas as pd
+
+from kasearch import AlignSequences
+from kasearch.merge_db import merge_files
 
-from kasearch.species_anarci import number
-from kasearch.canonical_alignment import canonical_alignment, canonical_alignment_oas, canonical_numbering_len
 
 class PrepareDB:
     
-    def __init__(self, db_path, oas_source=False):
+    def __init__(self, db_path, n_jobs=1, oas_source=False):
         
         os.makedirs(db_path, exist_ok=True)
         self.db_path = db_path
+        self.id_to_study = {}
+        self.n_jobs = n_jobs
         self._file_suffix = 0
         self._oas_source = oas_source
         
-        self._abnormal_sequence = np.zeros(canonical_numbering_len, np.int8)
-        self.tmpDB = tmpDB({}, {}, {}, {}, {})
-    
-    def _canonical_alignment_oas(self, sequence):
-        
-        try:
-            return canonical_alignment_oas(sequence)
-        except Exception:
-            return self._abnormal_sequence
-    
-    def _canonical_alignment(self, sequence):
-        try:
-            return canonical_alignment(sequence)
-        except Exception:
-            return self._abnormal_sequence
-    
-    def _many_canonical_alignment(self, sequence_dataset):
-        
-        if self._oas_source:
-            return np.array([self._canonical_alignment_oas(sequence) for sequence in sequence_dataset])
-        else:
-            return np.array([self._canonical_alignment(sequence) for sequence in sequence_dataset])
+        self.tmpDB = tmpDB(collections.defaultdict(dict), 
+                           collections.defaultdict(dict), 
+                           collections.defaultdict(dict), 
+                           collections.defaultdict(dict), 
+                           collections.defaultdict(dict))
         
     def _update_tmpDB(self, sequences, sequence_alignments, sequence_idxs, chain, species):
         
-        if chain not in self.tmpDB.sequences_count:
-            self.tmpDB.sequences_count[chain] = {}
-            self.tmpDB.sequences[chain] = {}
-            self.tmpDB.sequences_idxs[chain] = {}
-            self.tmpDB.abnormal_sequences[chain] = {}
-            self.tmpDB.abnormal_sequences_idxs[chain] = {}
-            
         if species not in self.tmpDB.sequences_count[chain]:
             self.tmpDB.sequences_count[chain][species] = 0
             self.tmpDB.sequences[chain][species] = []
             self.tmpDB.sequences_idxs[chain][species] = []
-            self.tmpDB.abnormal_sequences[chain][species] = []
-            self.tmpDB.abnormal_sequences_idxs[chain][species] = []
+            self.tmpDB.unusual_sequences[chain][species] = []
+            self.tmpDB.unusual_sequences_idxs[chain][species] = []
             
         self.tmpDB.sequences_count[chain][species] += len(sequences)
         
-        abnormal_sequence_idxs = np.where(0 == sequence_alignments.sum(-1))
+        unusual_sequence_idxs = np.where(0 == sequence_alignments.sum(-1))
         normal_sequence_idxs = np.where(0 != sequence_alignments.sum(-1))
 
         if normal_sequence_idxs[0] != []:
             self.tmpDB.sequences[chain][species].append(sequence_alignments[normal_sequence_idxs])
             self.tmpDB.sequences_idxs[chain][species].append(sequence_idxs[normal_sequence_idxs])
         
-        if abnormal_sequence_idxs[0] != []:
-            self.tmpDB.abnormal_sequences[chain][species].append(
-                sequences[abnormal_sequence_idxs])
-            self.tmpDB.abnormal_sequences_idxs[chain][species].append(
-                sequence_idxs[abnormal_sequence_idxs])
+        if unusual_sequence_idxs[0] != []:
+            self.tmpDB.unusual_sequences[chain][species].append(
+                sequences[unusual_sequence_idxs])
+            self.tmpDB.unusual_sequences_idxs[chain][species].append(
+                sequence_idxs[unusual_sequence_idxs])
     
     def _save_data_subset(self, sequence_alignments, sequence_idxs, chain, species, suffix = ''):
         
-        if suffix == None:
-            suffix = self._file_suffix
-            
-        unique_id = str(uuid.uuid4())
+        if suffix == None: suffix = self._file_suffix
+ 
         save_folder = os.path.join(self.db_path, chain, species)
-        save_file = os.path.join(save_folder, "data-subset-{}-{}.npz".format(suffix, unique_id))
+        save_file = os.path.join(save_folder, "data-subset-{}-{}.npz".format(suffix, str(uuid.uuid4())))
         os.makedirs(save_folder, exist_ok=True)
         
         np.savez_compressed(save_file, 
                             numberings=np.concatenate(sequence_alignments[chain][species]), 
                             idxs=np.concatenate(sequence_idxs[chain][species]))
         
-    def prepare_database(self, sequence_dataset, file_id, sequence_lines = None, chain='Heavy', species='Human'):
+    def prepare_sequences(self, data_unit_file, file_id, sequence_lines = None, chain='Heavy', species='Human', pre_calculated_anarci = None):
         """
         Prepares the new database. If a subset contains more than 50 million sequences, save that subset.
         """
         
-        if not sequence_lines:
-            sequence_lines = range(len(sequence_dataset))
+        self.id_to_study[file_id] = data_unit_file
         
-        sequence_alignments = self._many_canonical_alignment(sequence_dataset)
+        if pre_calculated_anarci is None:
+            sequences = pd.read_csv(data_unit_file, header=1, usecols=['sequence_alignment_aa']).iloc[:,0].values
+        else:
+            sequences = pre_calculated_anarci
+        
+        sequence_alignments = AlignSequences(n_jobs=self.n_jobs, allowed_species=[species],oas_source=self._oas_source, if_fast=True)(sequences)
+        
+        if not sequence_lines: sequence_lines = range(len(sequences))
+
         sequence_idxs = np.array([[file_id, i] for i in sequence_lines], np.int32)
         
-        self._update_tmpDB(sequence_dataset, sequence_alignments, sequence_idxs, chain, species)
+        self._update_tmpDB(sequences, sequence_alignments, sequence_idxs, chain, species)
         
         if self.tmpDB.sequences_count[chain][species]>4_000_000:
             
             self._save_data_subset(self.tmpDB.sequences, 
                                    self.tmpDB.sequences_idxs, 
                                    chain, species,
                                    suffix = 'normal'
                                   )
             
             self.tmpDB.sequences_count[chain][species] = 0
             self.tmpDB.sequences[chain][species] = []
             self.tmpDB.sequences_idxs[chain][species] = []
+            
+    
        
     def save_database(self):
         
         for chain, species_dict in self.tmpDB.sequences_idxs.items():
             for species in species_dict.keys():
                 if self.tmpDB.sequences[chain][species] != []:
                     self._save_data_subset(self.tmpDB.sequences, 
                                            self.tmpDB.sequences_idxs, 
                                            chain, species,
                                            suffix = 'normal'
                                           )
                     
-                if self.tmpDB.abnormal_sequences[chain][species] != []:
-                    self._save_data_subset(self.tmpDB.abnormal_sequences, 
-                                           self.tmpDB.abnormal_sequences_idxs, 
+                if self.tmpDB.unusual_sequences[chain][species] != []:
+                    self._save_data_subset(self.tmpDB.unusual_sequences, 
+                                           self.tmpDB.unusual_sequences_idxs, 
                                            chain, species,
                                            suffix = 'unusual'
                                           )
+                    
+        with open(os.path.join(self.db_path, "id_to_study.txt"), "w") as handle: 
+            handle.write(str(self.id_to_study))
+            
+    def merge_sequence_files(self):
+        
+        merge_files(self.db_path)
     
     
     
 def flatten(xss):
     return [x for xs in xss for x in xs]
 
 def unflatten(xss):
     return [xss[x:x+2] for x in range(0, len(xss), 2)]
     
 @dataclass   
 class tmpDB: 
     sequences_count: dict
     sequences: dict
     sequences_idxs: dict
-    abnormal_sequences: dict
-    abnormal_sequences_idxs: dict
+    unusual_sequences: dict
+    unusual_sequences_idxs: dict
```

### Comparing `kasearch-0.0.7/setup.py` & `kasearch-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='kasearch',
-    version='0.0.7',
+    version='0.0.9',
     description='KA-Search: Rapid and exhaustive sequence identity search of known antibodies',
     license='BSD 3-clause license',
     maintainer='Tobias Hegelund Olsen; Brennan Abanades kenyon',
     long_description=long_description,
     long_description_content_type='text/markdown',
     include_package_data=True,
     packages=find_packages(include=('kasearch', 'kasearch.*')),
```

