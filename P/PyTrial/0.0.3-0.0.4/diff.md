# Comparing `tmp/PyTrial-0.0.3.tar.gz` & `tmp/PyTrial-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyTrial-0.0.3.tar", last modified: Fri Mar 10 18:13:33 2023, max compression
+gzip compressed data, was "dist/PyTrial-0.0.4.tar", last modified: Fri Apr 21 19:26:22 2023, max compression
```

## Comparing `PyTrial-0.0.3.tar` & `PyTrial-0.0.4.tar`

### file list

```diff
@@ -1,133 +1,139 @@
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-01-18 21:29:45.000000 PyTrial-0.0.3/LICENSE
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6659 2023-03-10 18:13:33.000000 PyTrial-0.0.3/PKG-INFO
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/PyTrial.egg-info/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6659 2023-03-10 18:13:33.000000 PyTrial-0.0.3/PyTrial.egg-info/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4426 2023-03-10 18:13:33.000000 PyTrial-0.0.3/PyTrial.egg-info/SOURCES.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-03-10 18:13:33.000000 PyTrial-0.0.3/PyTrial.egg-info/dependency_links.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      364 2023-03-10 18:13:33.000000 PyTrial-0.0.3/PyTrial.egg-info/requires.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        8 2023-03-10 18:13:33.000000 PyTrial-0.0.3/PyTrial.egg-info/top_level.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6009 2023-03-06 23:05:32.000000 PyTrial-0.0.3/README.md
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      302 2023-03-10 18:11:40.000000 PyTrial-0.0.3/pytrial/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/data/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/data/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10756 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/data/demo_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/data/drug_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15547 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/data/patient_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21943 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/data/site_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13302 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/data/trial_data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/data/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1324 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/data/vocab_data.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5257 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/model_utils/bert.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    19288 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/model_utils/drug.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11508 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/model_utils/icd.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/causal/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/causal/__init__.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/confidence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/confidence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1757 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11365 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21022 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/dipole.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13626 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/raim.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10887 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/retain.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13497 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/rnn.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15633 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/stagenet.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10018 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/mlp.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/transtab.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7509 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/xgboost.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/indiv_outcome/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       80 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4575 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8666 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5913 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3023 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/metrics.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7943 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/pgentropy.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3659 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/site_selection/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      124 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    41735 2023-01-22 06:32:16.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/hint.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/logistic_regression.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/mlp.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/dataloader.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7926 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/module.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13678 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4734 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6727 2023-01-18 22:50:10.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_outcome/xgboost.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/compose.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/deepenroll.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_patient_match/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/losses.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/metrics.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/models/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/models/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/models/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/models/bm25.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/models/doc2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/models/trial2vec.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_search/models/whiten_bert.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2023-02-06 20:47:58.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/data.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/losses.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      136 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12108 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/eva.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21137 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9448 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/knn.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7669 2023-01-27 05:51:39.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/promptehr.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2023-03-08 22:14:32.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2023-03-08 22:16:42.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/synteg.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      154 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/base.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14843 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/copula_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8207 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/ct_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/evaluation.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3781 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14569 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/med_gan.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9470 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/tvae.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/tasks/trial_simulation/trainer.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-03-10 18:13:33.000000 PyTrial-0.0.3/pytrial/utils/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/utils/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/utils/check.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/utils/mimic_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/utils/parallel.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14882 2023-03-06 23:05:32.000000 PyTrial-0.0.3/pytrial/utils/tabular_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17977 2023-03-10 18:11:27.000000 PyTrial-0.0.3/pytrial/utils/trainer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2023-01-18 21:29:45.000000 PyTrial-0.0.3/pytrial/utils/trial_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-03-10 18:13:33.000000 PyTrial-0.0.3/setup.cfg
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1186 2023-03-10 18:12:40.000000 PyTrial-0.0.3/setup.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-01-18 21:29:45.000000 PyTrial-0.0.4/LICENSE
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6659 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PKG-INFO
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6659 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4711 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/SOURCES.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/dependency_links.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      264 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/requires.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        8 2023-04-21 19:26:22.000000 PyTrial-0.0.4/PyTrial.egg-info/top_level.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6009 2023-03-06 23:05:32.000000 PyTrial-0.0.4/README.md
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      302 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/data/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10898 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/data/demo_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        3 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/drug_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15741 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/data/patient_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21943 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/site_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13918 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/data/trial_data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2804 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1324 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/data/vocab_data.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5257 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/bert.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    19288 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/drug.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11508 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/model_utils/icd.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/causal/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/causal/__init__.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/confidence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/confidence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3485 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1757 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2342 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      128 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11365 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21022 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/dipole.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13626 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/raim.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10887 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/retain.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13497 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/rnn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15633 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/stagenet.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      174 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10018 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    46325 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5848 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7436 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/mlp.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    11151 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/transtab.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7509 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/xgboost.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1563 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/indiv_outcome/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       80 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4575 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8666 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5913 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3023 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/metrics.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8185 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/pgentropy.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3659 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/site_selection/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      147 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      830 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2335 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2167 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    41581 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/hint.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5262 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/logistic_regression.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9120 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/mlp.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7751 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/data_structure.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     2934 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/data_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7158 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/dataloader.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4047 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8303 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3857 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/module.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12827 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5784 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8295 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     6727 2023-01-18 22:50:10.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    33283 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/spot.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5454 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_outcome/xgboost.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      384 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4166 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4590 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7234 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    27438 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/compose.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24519 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/deepenroll.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4455 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_patient_match/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      191 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1775 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1223 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/losses.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      552 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/metrics.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7238 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/bm25.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8652 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/doc2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    39578 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/trial2vec.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15813 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_search/models/whiten_bert.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4125 2023-04-19 17:00:00.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/data.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4986 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/losses.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      136 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12108 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16604 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/eva.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    21137 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9448 2023-03-10 18:11:27.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/knn.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7669 2023-01-27 05:51:39.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/promptehr.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    16617 2023-03-08 22:14:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/rnn_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    24355 2023-03-08 22:16:42.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/synteg.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      154 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3742 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/base.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14843 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/copula_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     8207 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/ct_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7208 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/evaluation.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3781 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    14680 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/med_gan.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     9470 2023-03-06 23:05:32.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/tvae.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13937 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/tasks/trial_simulation/trainer.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-21 19:26:22.000000 PyTrial-0.0.4/pytrial/utils/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      146 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     3089 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/check.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    20404 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/mimic_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10434 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/parallel.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15561 2023-04-21 19:25:57.000000 PyTrial-0.0.4/pytrial/utils/tabular_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    17977 2023-04-21 00:55:39.000000 PyTrial-0.0.4/pytrial/utils/trainer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12797 2023-01-18 21:29:45.000000 PyTrial-0.0.4/pytrial/utils/trial_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-04-21 19:26:22.000000 PyTrial-0.0.4/setup.cfg
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1186 2023-04-21 19:25:57.000000 PyTrial-0.0.4/setup.py
```

### Comparing `PyTrial-0.0.3/LICENSE` & `PyTrial-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/PKG-INFO` & `PyTrial-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTrial
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTrial: A Python Package for Artificial Intelligence in Drug Development
 Home-page: https://github.com/RyanWangZf/pytrial
 Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jingtang Ma, Jimeng Sun
 Author-email: zifengw2@illinois.edu
 Keywords: drug development,clinical trial,artificial intelligence,deep learning,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PyTrial-0.0.3/PyTrial.egg-info/PKG-INFO` & `PyTrial-0.0.4/PyTrial.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTrial
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyTrial: A Python Package for Artificial Intelligence in Drug Development
 Home-page: https://github.com/RyanWangZf/pytrial
 Author: Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jingtang Ma, Jimeng Sun
 Author-email: zifengw2@illinois.edu
 Keywords: drug development,clinical trial,artificial intelligence,deep learning,machine learning
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PyTrial-0.0.3/PyTrial.egg-info/SOURCES.txt` & `PyTrial-0.0.4/PyTrial.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,25 +46,31 @@
 pytrial/tasks/site_selection/data.py
 pytrial/tasks/site_selection/losses.py
 pytrial/tasks/site_selection/metrics.py
 pytrial/tasks/site_selection/pgentropy.py
 pytrial/tasks/site_selection/trainer.py
 pytrial/tasks/trial_outcome/__init__.py
 pytrial/tasks/trial_outcome/base.py
+pytrial/tasks/trial_outcome/data.py
+pytrial/tasks/trial_outcome/evaluation.py
 pytrial/tasks/trial_outcome/hint.py
 pytrial/tasks/trial_outcome/logistic_regression.py
 pytrial/tasks/trial_outcome/mlp.py
+pytrial/tasks/trial_outcome/spot.py
 pytrial/tasks/trial_outcome/xgboost.py
 pytrial/tasks/trial_outcome/model_utils/__init__.py
+pytrial/tasks/trial_outcome/model_utils/data_structure.py
+pytrial/tasks/trial_outcome/model_utils/data_utils.py
 pytrial/tasks/trial_outcome/model_utils/dataloader.py
 pytrial/tasks/trial_outcome/model_utils/gnn_layers.py
 pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py
 pytrial/tasks/trial_outcome/model_utils/module.py
 pytrial/tasks/trial_outcome/model_utils/molecule_encode.py
 pytrial/tasks/trial_outcome/model_utils/protocol_encode.py
+pytrial/tasks/trial_outcome/model_utils/topic_discovery.py
 pytrial/tasks/trial_outcome/model_utils/utils.py
 pytrial/tasks/trial_patient_match/__init__.py
 pytrial/tasks/trial_patient_match/data.py
 pytrial/tasks/trial_patient_match/losses.py
 pytrial/tasks/trial_patient_match/trainer.py
 pytrial/tasks/trial_patient_match/models/__init__.py
 pytrial/tasks/trial_patient_match/models/base.py
```

### Comparing `PyTrial-0.0.3/README.md` & `PyTrial-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/data/demo_data.py` & `PyTrial-0.0.4/pytrial/data/demo_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,45 +164,48 @@
         'visit_stage':v_stage,
         'relapse':label_relapse,
         'mortality':label_mortality,
     }
 
 def load_trial_outcome_data(input_dir=None, phase='I', split='train'):
     '''
-    Load trial outcome prediction (TOP) benchmark data from https://github.com/futianfan/clinical-trial-outcome-prediction.
+    Load trial outcome prediction (TOP) benchmark data.
 
     Parameters
     ----------
     input_dir: str
         The folder that stores the demo data. If None, we will download the demo data and save it
         to './demo_data/demo_trial_data'. Make sure to remove this folder if it is empty.
 
     phase: {'I','II','III'}
         The phase of the trial data. Can be 'I', 'II', 'III'.
     
     split: {'train', 'test', 'valid'}
         The split of the trial data. Can be 'train', 'test', 'valid'.
     '''
+
+    BENCHMARK_DATA_URL = 'https://storage.googleapis.com/pytrial/HINT-benchmark-data/hint_benchmark_dataset_w_date.zip'
+
     if input_dir is None:
-        input_dir = './demo_data/demo_trial_data'
-    
-    filename = 'phase_{}_{}.csv'.format(phase, split)
+        input_dir = './demo_data/demo_trial_outcome_data'
 
-    if not os.path.exists(os.path.join(input_dir, filename)):
-        if not os.path.exists(input_dir):
-            os.makedirs(input_dir)
-        url = TOP_URL + filename
-        df = pd.read_csv(url)
-        df.to_csv(os.path.join(input_dir, filename))
+    if not os.path.exists(input_dir):
+        os.makedirs(input_dir)
+        # download the benchmark data
+        wget.download(BENCHMARK_DATA_URL, out=input_dir)
+        # unzip filename
+        import zipfile
+        with zipfile.ZipFile(os.path.join(input_dir, 'hint_benchmark_dataset_w_date.zip'), 'r') as zip_ref:
+            zip_ref.extractall(input_dir)
         print(f'\n Download trial data to {input_dir}.')
     
-    else:
-        filename = os.path.join(input_dir, filename)
-        # load patient data
-        df = pd.read_csv(filename)
+    filename = 'phase_{}_{}.csv'.format(phase, split)
+    filename = os.path.join(input_dir, filename)
+    # load patient data
+    df = pd.read_csv(filename)
     return {'data':df}
 
 def load_trial_document_data(input_dir=None, 
     n_sample=None,
     source='preprocessed',
     date='20221001',
     ):
```

### Comparing `PyTrial-0.0.3/pytrial/data/patient_data.py` & `PyTrial-0.0.4/pytrial/data/patient_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
                 self.ht.detect_initial_config(df)
                 self.metadata = self.ht.get_config()
                 self.ht.fit(df)
 
             else:
                 # parse the metadata and update hypertransformer's config
                 self._parse_metadata()
+            
+            # create a mapping from column name before to column name after transformation
+            self._create_transformed_col2col()
 
             # replace data with the transformed one
             self.df = self.transform(df)
 
     def __getitem__(self, index):
         # TODO: support better indexing
         '''
@@ -177,14 +180,15 @@
         
         if 'sdtypes' in metadata:
             self.ht.update_sdtypes(metadata['sdtypes'])
 
         self.ht.fit(self.df)
         self.metadata.update(self.ht.get_config())
 
+    def _create_transformed_col2col(self):
         # create transformed column id to the original columns
         transformed_col2col = OrderedDict()
         for idx, col in enumerate(self.df.columns):
             col_transformer = self.metadata['transformers'][col]
             transformed_col2col[col] = col_transformer.output_columns
         self.metadata['transformed_col2col'] = transformed_col2col
```

### Comparing `PyTrial-0.0.3/pytrial/data/site_data.py` & `PyTrial-0.0.4/pytrial/data/site_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/data/trial_data.py` & `PyTrial-0.0.4/pytrial/data/trial_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
 from collections import defaultdict
 import pdb
 import os
 from typing import Any, Callable, Dict, List, NewType, Optional, Tuple, Union
 
 import pandas as pd
+import torch
 from torch.utils.data import Dataset, DataLoader
 
 from ..utils.trial_utils import ClinicalTrials
 from ..utils.tabular_utils import read_csv_to_df
 from ..data.vocab_data import Vocab
 
 from ..utils.tabular_utils import HyperTransformer
@@ -17,52 +18,67 @@
     '''
     The basic trial datasets loader.
 
     Parameters
     ----------
     data: pd.DataFrame
         Contain the trial document in tabular format.
+
+    criteria_column: str
+        The column name of eligibility criteria in the dataframe.
     '''
     inc_ec_embedding = None # inclusion criteria embedding
     inc_vocab = None # inclusion criteria vocab
     exc_ec_embedding = None # exclusion criteria embedding
     exc_vocab = None # exclusion criteria vocab
 
-    def __init__(self, data):
+    def __init__(self, data, criteria_column='criteria'):
         self.df = data
-        self._process_ec()
+        self._process_ec(criteria_column=criteria_column)
         self._collect_cleaned_sentence_set()
     
     def __len__(self):
         return len(self.df)
 
     def __getitem__(self, index):
         return self.df.iloc[index:index+1]
     
     def get_ec_sentence_embedding(self):
         '''
         Process the eligibility criteria of each trial,
         get the criterion-level emebddings stored in dict.
+
+        Parameters
+        ----------
+        criteria_column: str
+            The column name of eligibility criteria in the dataframe.
         '''
-        self._get_ec_emb()
+        if self.inc_ec_embedding is None or self.exc_ec_embedding is None:
+            self._get_ec_emb()
+        
+        return self.inc_ec_embedding, self.exc_ec_embedding
 
-    def _process_ec(self):
-        res = self.df['criteria'].apply(lambda x: self._split_protocol(x))
+    def _process_ec(self, criteria_column):
+        res = self.df[criteria_column].apply(lambda x: self._split_protocol(x))
         self.df['inclusion_criteria'] = res.apply(lambda x: x[0])
         self.df['exclusion_criteria'] = res.apply(lambda x: x[1])
 
     def _get_ec_emb(self):
         # create EC embedding with indexed ECs
         from pytrial.model_utils.bert import BERT
-        bert_model = BERT(device='cuda:0')
+        # check if cuda is available
+        if torch.cuda.is_available():
+            device = 'cuda:0'
+        else:
+            device = 'cpu'
+        bert_model = BERT(device=device)
         self.inc_ec_embedding = bert_model.encode(self.inc_vocab.words, batch_size=64)
         self.exc_ec_embedding = bert_model.encode(self.exc_vocab.words, batch_size=64)
         self.inc_ec_embedding = self.inc_ec_embedding.cpu()
         self.exc_ec_embedding = self.exc_ec_embedding.cpu()
-        
 
     def _collect_cleaned_sentence_set(self):
         # create a vocab for ec sentences
         self.inc_vocab = Vocab()
         self.exc_vocab = Vocab()
         self.inc_vocab.add_sentence(['[PAD]']) # 0 belongs to the pad token
         self.exc_vocab.add_sentence(['[PAD]']) # 0 belongs to the pad token
@@ -158,15 +174,15 @@
 
     def __call__(self, examples):
         batch_df = pd.concat(examples, 0)
         batch_df.fillna('none',inplace=True)
         return batch_df
 
 
-class TrialOutcomeDatasetBase(Dataset):
+class TrialOutcomeDatasetBase(TrialDatasetBase):
     '''
     Basic trial outcome datasets loader.
 
     Parameters
     ----------
     data: pd.DataFrame
         Contain the trial document in tabular format.
```

### Comparing `PyTrial-0.0.3/pytrial/data/utils.py` & `PyTrial-0.0.4/pytrial/data/utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/data/vocab_data.py` & `PyTrial-0.0.4/pytrial/data/vocab_data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/model_utils/bert.py` & `PyTrial-0.0.4/pytrial/model_utils/bert.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/model_utils/drug.py` & `PyTrial-0.0.4/pytrial/model_utils/drug.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/model_utils/icd.py` & `PyTrial-0.0.4/pytrial/model_utils/icd.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/data.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/losses.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/metrics.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/base.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/dipole.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/dipole.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/raim.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/raim.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/retain.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/retain.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/rnn.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/rnn.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/sequence/stagenet.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/sequence/stagenet.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/base.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/mlp.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/mlp.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/transtab.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/transtab.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/tabular/xgboost.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/tabular/xgboost.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/indiv_outcome/trainer.py` & `PyTrial-0.0.4/pytrial/tasks/indiv_outcome/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/site_selection/base.py` & `PyTrial-0.0.4/pytrial/tasks/site_selection/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/site_selection/data.py` & `PyTrial-0.0.4/pytrial/tasks/site_selection/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/site_selection/losses.py` & `PyTrial-0.0.4/pytrial/tasks/site_selection/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/site_selection/metrics.py` & `PyTrial-0.0.4/pytrial/tasks/site_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/site_selection/pgentropy.py` & `PyTrial-0.0.4/pytrial/tasks/site_selection/pgentropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,28 +42,32 @@
         network_input = torch.cat((site_encoding, trial_encoding), dim=-1)
         network_input = torch.relu(self.score_encoder(network_input))
         score = self.output(torch.relu(self.fc(network_input))).squeeze(-1)
         return score
 
 class PolicyGradientEntropy(SiteSelectionBase):
     '''
-    Implement Policy Gradient Entropy model for selecting clinical trial sites based on possibly missing multi-model site features.
+    Implement Policy Gradient Entropy model for selecting clinical trial sites based on possibly missing multi-model site features. [1]_
     
     Parameters
     ----------
     
     trial_dim: list[int]
         Size of the trial representation
 
     site_dim: int
         Size of the site representation
 
     embedding_dim: int
         Size of all of the modality and other intermediate embeddings
-        
+    
+    Notes
+    -----
+    .. [1] Srinivasa, R. S., Qian, C., Theodorou, B., Spaeder, J., Xiao, C., Glass, L., & Sun, J. (2022). Clinical trial site matching with improved diversity using fair policy learning. arXiv preprint arXiv:2204.06501.
+
     '''
     def __init__(self, 
         trial_dim=211, 
         site_dim=124, 
         embedding_dim=64, 
         enrollment_only=True,
         K=10,
```

### Comparing `PyTrial-0.0.3/pytrial/tasks/site_selection/trainer.py` & `PyTrial-0.0.4/pytrial/tasks/site_selection/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/base.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/hint.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/hint.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,14 @@
         weight_decay = 0, 
         ):
         super(Interaction, self).__init__()
         icdcode2ancestor_dict = build_icdcode2ancestor_dict()
         self.disease_encoder = GRAM(embedding_dim = disease_embedding_dim, icdcode2ancestor = icdcode2ancestor_dict, device = device)
         self.protocol_encoder = Protocol_Embedding(output_dim = protocol_output_dim, highway_num=3, device = device)
         self.molecule_encoder = MPNN(mpnn_hidden_size = molecule_embedding_dim, mpnn_depth=3, device = device)
-        # self.molecule_encoder = molecule_encoder 
-        # self.disease_encoder = disease_encoder 
-        # self.protocol_encoder = protocol_encoder 
         self.global_embed_size = global_embed_size 
         self.highway_num_layer = highway_num_layer 
         self.feature_dim = self.molecule_encoder.embedding_size + self.disease_encoder.embedding_size + self.protocol_encoder.embedding_size
         self.epoch = epoch 
         self.lr = lr 
         self.weight_decay = weight_decay 
         self.save_name = prefix_name + '_interaction'
```

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/logistic_regression.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/mlp.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/mlp.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/dataloader.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/gnn_layers.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/icdcode_encode.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 	icdcode_embedding 
 
 '''
 
 import csv, re, pickle, os
 import pdb
 from functools import reduce 
-import icd10
+import wget
 from collections import defaultdict
 
 import pandas as pd
 import torch 
 from torch import nn 
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+import icd10
 
 ICDCODE_ANCESTOR_URL = 'https://github.com/futianfan/clinical-trial-outcome-prediction/raw/main/data/raw_data.csv'
+icdcode2ancestor_dict_url = "https://storage.googleapis.com/pytrial/HINT-benchmark-data/icdcode2ancestor_dict.pkl"
 
 def text_2_lst_of_lst(text):
 	"""
 		"[""['F53.0', 'P91.4', 'Z13.31', 'Z13.32']""]"
 	"""
 	text = text[2:-2]
 	code_sublst = []
@@ -74,15 +76,20 @@
 			ancestor = ancestor[:-1]
 		if icd10.find(ancestor) is not None:
 			icdcode2ancestor[icdcode].append(ancestor)
 	return
 
 
 def build_icdcode2ancestor_dict():
-	pkl_file = "demo_data/demo_trial_outcome_data/icdcode2ancestor_dict.pkl"
+	pkl_file = "pretrained_model/icdcode2ancestor/icdcode2ancestor_dict.pkl"
+
+	if not os.path.exists('pretrained_model/icdcode2ancestor'):
+		os.makedirs('pretrained_model/icdcode2ancestor')
+		wget.download(icdcode2ancestor_dict_url, pkl_file)
+
 	if os.path.exists(pkl_file):
 		icdcode2ancestor = pickle.load(open(pkl_file, 'rb'))
 		return icdcode2ancestor
 	all_code = collect_all_icdcodes()
 	icdcode2ancestor = defaultdict(list)
 	for code in all_code:
 		find_ancestor_for_icdcode(code, icdcode2ancestor)
@@ -111,15 +118,18 @@
 
 class GRAM(nn.Sequential):
 	"""	
 		return a weighted embedding 
 	"""
 
 	def __init__(self, embedding_dim, icdcode2ancestor, device):
-		super(GRAM, self).__init__()		
+		super(GRAM, self).__init__()
+		if icdcode2ancestor is None: 
+			icdcode2ancestor = build_icdcode2ancestor_dict()
+
 		self.icdcode2ancestor = icdcode2ancestor 
 		self.all_code_lst = GRAM.codedict_2_allcode(self.icdcode2ancestor)
 		self.code_num = len(self.all_code_lst)
 		self.maxlength = 5
 		self.code2index = {code:idx for idx,code in enumerate(self.all_code_lst)}
 		self.index2code = {idx:code for idx,code in enumerate(self.all_code_lst)}
 		self.padding_matrix = torch.zeros(self.code_num, self.maxlength).long()
```

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/module.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/module.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/molecule_encode.py`

 * *Files 6% similar despite different names*

```diff
@@ -226,14 +226,19 @@
 		self.mpnn_hidden_size = mpnn_hidden_size
 		self.mpnn_depth = mpnn_depth 
 
 		self.W_i = nn.Linear(ATOM_FDIM + BOND_FDIM, self.mpnn_hidden_size, bias=False)
 		self.W_h = nn.Linear(self.mpnn_hidden_size, self.mpnn_hidden_size, bias=False)
 		self.W_o = nn.Linear(ATOM_FDIM + self.mpnn_hidden_size, self.mpnn_hidden_size)
 
+		# initialize weights
+		nn.init.xavier_uniform_(self.W_i.weight)
+		nn.init.xavier_uniform_(self.W_h.weight)
+		nn.init.xavier_uniform_(self.W_o.weight)
+
 		self.device = device
 		self = self.to(self.device)
 
 	def set_device(self, device):
 		self.device = device 
 
 
@@ -353,15 +358,14 @@
 		self.device = device 
 		self = self.to(device)
 
 	def set_device(self, device):
 		self.device = device 
 		self.molecule_encoder.set_device(device)
 
-
 	def forward_smiles_lst_embedding(self, smiles_lst, idx):
 		embed_all = self.molecule_encoder.forward_smiles_lst(smiles_lst)
 		output = self.highway_nn_lst[idx](embed_all)
 		return output 
 
 	def forward_embedding_to_pred(self, embeded, idx):
 		return self.fc_output_lst[idx](embeded)
@@ -378,46 +382,14 @@
 			for smiles_lst, label_vec in dataloader_lst[idx]:
 				output = self.forward_smiles_lst_pred(smiles_lst, idx).view(-1)
 				loss = self.loss(output, label_vec.to(self.device).float())
 				single_loss_lst.append(loss.item())
 			loss_lst.append(np.mean(single_loss_lst))
 		return np.mean(loss_lst)
 
-	def train(self, train_loader_lst, valid_loader_lst):
-		opt = torch.optim.Adam(self.parameters(), lr = self.lr, weight_decay = self.weight_decay)
-		train_loss_record = [] 
-		valid_loss = self.test(valid_loader_lst, return_loss=True)
-		valid_loss_record = [valid_loss]
-		best_valid_loss = valid_loss 
-		best_model = deepcopy(self)
-		for ep in tqdm(range(self.epoch)):
-			data_iterator_lst = [iter(train_loader_lst[idx]) for idx in range(5)]
-			try: 
-				while True:
-					for idx in range(1):
-						smiles_lst, label_vec = next(data_iterator_lst[idx])
-						output = self.forward_smiles_lst_pred(smiles_lst, idx).view(-1)
-						loss = self.loss(output, label_vec.float()) 
-						opt.zero_grad() 
-						loss.backward()
-						opt.step()	
-			except:
-				pass 
-			valid_loss = self.test(valid_loader_lst, return_loss = True)
-			valid_loss_record.append(valid_loss)						
-
-			if valid_loss < best_valid_loss:
-				best_valid_loss = valid_loss 
-				best_model = deepcopy(self)
-
-		self = deepcopy(best_model)
-
-
-
-
 
 if __name__ == "__main__":
 	model = MPNN(mpnn_hidden_size = 50, mpnn_depth = 3)
 	dataloader = data_loader()
 	for smiles_feature, labels in dataloader:
 		embedding = model(smiles_feature) 
 		print(embedding.shape)
```

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/model_utils/utils.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/model_utils/utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_outcome/xgboost.py` & `PyTrial-0.0.4/pytrial/tasks/trial_outcome/xgboost.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_patient_match/data.py` & `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_patient_match/losses.py` & `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/base.py` & `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/compose.py` & `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/compose.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_patient_match/models/deepenroll.py` & `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/models/deepenroll.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_patient_match/trainer.py` & `PyTrial-0.0.4/pytrial/tasks/trial_patient_match/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_search/data.py` & `PyTrial-0.0.4/pytrial/tasks/trial_search/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_search/losses.py` & `PyTrial-0.0.4/pytrial/tasks/trial_search/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_search/metrics.py` & `PyTrial-0.0.4/pytrial/tasks/trial_search/metrics.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_search/models/base.py` & `PyTrial-0.0.4/pytrial/tasks/trial_search/models/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_search/models/doc2vec.py` & `PyTrial-0.0.4/pytrial/tasks/trial_search/models/doc2vec.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_search/models/trial2vec.py` & `PyTrial-0.0.4/pytrial/tasks/trial_search/models/trial2vec.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_search/models/whiten_bert.py` & `PyTrial-0.0.4/pytrial/tasks/trial_search/models/whiten_bert.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/data.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/data.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/losses.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/losses.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/base.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/eva.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/eva.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/evaluation.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/knn.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/knn.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/promptehr.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/promptehr.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/rnn_gan.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/rnn_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/sequence/synteg.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/sequence/synteg.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/base.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/base.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/copula_gan.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/copula_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/ct_gan.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/ct_gan.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/evaluation.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/evaluation.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/gaussian_copula.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/med_gan.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/med_gan.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,16 @@
         self.decoder = Decoder(self.embedding_dim, self.compress_dims, data_dim).to(self.device)
         optimizerAE = Adam(
             list(encoder.parameters()) + list(self.decoder.parameters()),
             weight_decay=self.l2scale
         )
 
         for i in range(self.pretrain_epoch):
+            if self.verbose:
+                print('Pretrain Epoch: {} / {}'.format(i+1, self.pretrain_epoch))
             for id_, data in enumerate(loader):
                 optimizerAE.zero_grad()
                 real = data[0].to(self.device)
                 emb = encoder(real)
                 rec = self.decoder(emb, self.output_info)
                 loss = aeloss(rec, real, self.output_info)
```

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/tabular/tvae.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/tabular/tvae.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/tasks/trial_simulation/trainer.py` & `PyTrial-0.0.4/pytrial/tasks/trial_simulation/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/utils/check.py` & `PyTrial-0.0.4/pytrial/utils/check.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/utils/mimic_utils.py` & `PyTrial-0.0.4/pytrial/utils/mimic_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/utils/parallel.py` & `PyTrial-0.0.4/pytrial/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/utils/tabular_utils.py` & `PyTrial-0.0.4/pytrial/utils/tabular_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 max_categories and min_frequencies, refer to https://scikit-learn.org/stable/modules/preprocessing.html.
 '''
 from collections import defaultdict
 import pickle
 from pathlib import Path
 import pdb
 import os
+from copy import deepcopy
 
 import pandas as pd
 import numpy as np
 from sklearn.preprocessing import StandardScaler as sk_standardscaler
 from sklearn.preprocessing import MinMaxScaler as sk_minmaxscaler
 import rdt
 from rdt.hyper_transformer import Config
@@ -195,14 +196,21 @@
         self.standard_transformer = sk_minmaxscaler()
 
 
 class HyperTransformer(rdt.HyperTransformer):
     '''
     A subclass of `rdt.HyperTransformer` to set special setups.
     '''
+    _DTYPES_TO_SDTYPES = {
+        'i': 'categorical', # change the default from numerical to categorical for integers
+        'f': 'numerical',
+        'O': 'categorical',
+        'b': 'boolean',
+        'M': 'datetime',
+    }
     def __init__(self):
         self._default_sdtype_transformers = {
             'numerical': StandardScaler(missing_value_replacement='mean'),
             'categorical': LabelEncoder(),
             'boolean': BinaryEncoder(missing_value_replacement='mode'),
             'datetime': UnixTimestampEncoder(missing_value_replacement='mean'),
         }
@@ -278,14 +286,25 @@
         if invalid_transformers_columns:
             raise InvalidConfigError(
                 f'Invalid transformers for columns: {invalid_transformers_columns}. '
                 'Please assign an rdt transformer instance to each column name.'
             )
         
         column_name_to_transformer.update(update_transformers)
+    
+    def _set_field_sdtype(self, data, field):
+        clean_data = data[field].dropna()
+        kind = clean_data.infer_objects().dtype.kind
+        if kind == 'i':
+            # decide if it is categorical or binary for input integers
+            if len(clean_data.unique()) <= 2:
+                kind = 'b'
+            else:
+                kind = 'O'
+        self.field_sdtypes[field] = self._DTYPES_TO_SDTYPES[kind]
 
 
 def read_csv_to_df(file_loc, header_lower=True, usecols=None, dtype=None,
                    low_memory=True, encoding=None, index_col=None):
     """Read in csv files with necessary processing
     Parameters
     ----------
```

### Comparing `PyTrial-0.0.3/pytrial/utils/trainer.py` & `PyTrial-0.0.4/pytrial/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/pytrial/utils/trial_utils.py` & `PyTrial-0.0.4/pytrial/utils/trial_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrial-0.0.3/setup.py` & `PyTrial-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # read the contents of requirements.txt
 with open(os.path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name = 'PyTrial',
-    version = '0.0.3',
+    version = '0.0.4',
     author = 'Zifeng Wang, Brandon Theodoru, Tianfan Fu, Jingtang Ma, Jimeng Sun',
     author_email = 'zifengw2@illinois.edu',
     description = 'PyTrial: A Python Package for Artificial Intelligence in Drug Development',
     url = 'https://github.com/RyanWangZf/pytrial',
     keywords=['drug development', 'clinical trial', 'artificial intelligence', 'deep learning', 'machine learning'],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

