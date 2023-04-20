# Comparing `tmp/goodai-ltm-0.0.7.tar.gz` & `tmp/goodai-ltm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodai-ltm-0.0.7.tar", last modified: Thu Apr 20 21:24:16 2023, max compression
+gzip compressed data, was "goodai-ltm-0.0.8.tar", last modified: Thu Apr 20 21:49:03 2023, max compression
```

## Comparing `goodai-ltm-0.0.7.tar` & `goodai-ltm-0.0.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.858097 goodai-ltm-0.0.7/
--rw-rw-rw-   0        0        0      184 2023-04-20 21:24:16.858097 goodai-ltm-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-04-19 21:51:49.000000 goodai-ltm-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.772417 goodai-ltm-0.0.7/goodai/
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.797964 goodai-ltm-0.0.7/goodai/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/helpers/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/helpers/collections_helper.py
--rw-rw-rw-   0        0        0      717 2023-04-19 20:33:13.000000 goodai-ltm-0.0.7/goodai/helpers/file_helper.py
--rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/helpers/html_helper.py
--rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/helpers/json_helper.py
--rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/helpers/tokenizer_helper.py
--rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.800964 goodai-ltm-0.0.7/goodai/ltm/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.802965 goodai-ltm-0.0.7/goodai/ltm/data/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/data/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/ltm/data/cloud.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.805556 goodai-ltm-0.0.7/goodai/ltm/data/names/
--rw-rw-rw-   0        0        0     1996 2023-04-19 22:25:12.000000 goodai-ltm-0.0.7/goodai/ltm/data/names/__init__.py
--rw-rw-rw-   0        0        0   183119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/ltm/data/names/wikidata-names.json
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.815096 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/__init__.py
--rw-rw-rw-   0        0        0     1626 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/auto_data_source.py
--rw-rw-rw-   0        0        0      485 2023-04-20 19:49:15.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/data_source.py
--rw-rw-rw-   0        0        0     2422 2023-04-19 22:26:45.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/dataset.py
--rw-rw-rw-   0        0        0      331 2023-04-20 19:47:41.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/example.py
--rw-rw-rw-   0        0        0    11044 2023-04-20 19:51:43.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/qa.py
--rw-rw-rw-   0        0        0     1857 2023-04-19 22:30:12.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/qa_tok_entry.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.817096 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/tests/__init__.py
--rw-rw-rw-   0        0        0     2527 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
--rw-rw-rw-   0        0        0     6936 2023-04-20 19:54:07.000000 goodai-ltm-0.0.7/goodai/ltm/data/query_passage/wiki.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.825096 goodai-ltm-0.0.7/goodai/ltm/embedding_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/auto.py
--rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/contrast_classifier.py
--rw-rw-rw-   0        0        0     5366 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/default.py
--rw-rw-rw-   0        0        0     1533 2023-04-19 16:47:45.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/emb_qp_prob_model.py
--rw-rw-rw-   0        0        0     2785 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/openai_emb.py
--rw-rw-rw-   0        0        0     2224 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/st_emb.py
--rw-rw-rw-   0        0        0     5440 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/embedding_models/trainable.py
--rw-rw-rw-   0        0        0     1584 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/embeddings.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.831097 goodai-ltm-0.0.7/goodai/ltm/eval/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/eval/__init__.py
--rw-rw-rw-   0        0        0     1038 2023-04-20 21:13:58.000000 goodai-ltm-0.0.7/goodai/ltm/eval/auto.py
--rw-rw-rw-   0        0        0     4450 2023-04-20 19:42:22.000000 goodai-ltm-0.0.7/goodai/ltm/eval/mem.py
--rw-rw-rw-   0        0        0     2716 2023-04-19 23:22:15.000000 goodai-ltm-0.0.7/goodai/ltm/eval/metrics.py
--rw-rw-rw-   0        0        0     1901 2023-04-19 23:26:29.000000 goodai-ltm-0.0.7/goodai/ltm/eval/qrecc.py
--rw-rw-rw-   0        0        0     2072 2023-04-20 20:01:17.000000 goodai-ltm-0.0.7/goodai/ltm/eval/strategy_qa.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.832096 goodai-ltm-0.0.7/goodai/ltm/eval/tests/
--rw-rw-rw-   0        0        0     1420 2023-04-19 23:22:33.000000 goodai-ltm-0.0.7/goodai/ltm/eval/tests/test_metrics.py
--rw-rw-rw-   0        0        0     1188 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/matching.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.837097 goodai-ltm-0.0.7/goodai/ltm/matching_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.7/goodai/ltm/matching_models/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/matching_models/auto.py
--rw-rw-rw-   0        0        0    10019 2023-04-19 22:29:29.000000 goodai-ltm-0.0.7/goodai/ltm/matching_models/default.py
--rw-rw-rw-   0        0        0      706 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/matching_models/prob_model.py
--rw-rw-rw-   0        0        0      658 2023-04-19 21:49:37.000000 goodai-ltm-0.0.7/goodai/ltm/matching_models/st_ce.py
--rw-rw-rw-   0        0        0     1208 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/memory.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.847096 goodai-ltm-0.0.7/goodai/ltm/memory_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/__init__.py
--rw-rw-rw-   0        0        0     1376 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/auto.py
--rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/chunk.py
--rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/chunk_mixin.py
--rw-rw-rw-   0        0        0    10364 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/chunk_queue.py
--rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/config.py
--rw-rw-rw-   0        0        0     5562 2023-04-19 22:25:35.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/default.py
--rw-rw-rw-   0        0        0     5784 2023-04-19 22:27:29.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/mem_foundation.py
--rw-rw-rw-   0        0        0     2960 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/simple_vector_db.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.848096 goodai-ltm-0.0.7/goodai/ltm/memory_models/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/tests/__init__.py
--rw-rw-rw-   0        0        0     3101 2023-04-20 15:19:11.000000 goodai-ltm-0.0.7/goodai/ltm/memory_models/tests/test_chunk_queue.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.850097 goodai-ltm-0.0.7/goodai/ltm/training/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.852096 goodai-ltm-0.0.7/goodai/ltm/training/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.7/goodai/ltm/training/query_passage/__init__.py
--rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.7/goodai/ltm/training/query_passage/trainer.py
--rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.7/goodai/ltm/training/sched_opt.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:24:16.857098 goodai-ltm-0.0.7/goodai_ltm.egg-info/
--rw-rw-rw-   0        0        0      184 2023-04-20 21:24:16.000000 goodai-ltm-0.0.7/goodai_ltm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2399 2023-04-20 21:24:16.000000 goodai-ltm-0.0.7/goodai_ltm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 21:24:16.000000 goodai-ltm-0.0.7/goodai_ltm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-04-20 21:24:16.000000 goodai-ltm-0.0.7/goodai_ltm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 21:24:16.000000 goodai-ltm-0.0.7/goodai_ltm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 21:24:16.858097 goodai-ltm-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      657 2023-04-20 21:24:09.000000 goodai-ltm-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.383241 goodai-ltm-0.0.8/
+-rw-rw-rw-   0        0        0      184 2023-04-20 21:49:03.382240 goodai-ltm-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-04-19 21:51:49.000000 goodai-ltm-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.295210 goodai-ltm-0.0.8/goodai/
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.320241 goodai-ltm-0.0.8/goodai/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/collections_helper.py
+-rw-rw-rw-   0        0        0      717 2023-04-19 20:33:13.000000 goodai-ltm-0.0.8/goodai/helpers/file_helper.py
+-rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/html_helper.py
+-rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/json_helper.py
+-rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/tokenizer_helper.py
+-rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.324240 goodai-ltm-0.0.8/goodai/ltm/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.325241 goodai-ltm-0.0.8/goodai/ltm/data/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/data/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/data/cloud.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.327241 goodai-ltm-0.0.8/goodai/ltm/data/names/
+-rw-rw-rw-   0        0        0     1996 2023-04-19 22:25:12.000000 goodai-ltm-0.0.8/goodai/ltm/data/names/__init__.py
+-rw-rw-rw-   0        0        0   183119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/data/names/wikidata-names.json
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.337240 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/auto_data_source.py
+-rw-rw-rw-   0        0        0      485 2023-04-20 19:49:15.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/data_source.py
+-rw-rw-rw-   0        0        0     2422 2023-04-19 22:26:45.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/dataset.py
+-rw-rw-rw-   0        0        0      331 2023-04-20 19:47:41.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/example.py
+-rw-rw-rw-   0        0        0    11044 2023-04-20 19:51:43.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa.py
+-rw-rw-rw-   0        0        0     1857 2023-04-19 22:30:12.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa_tok_entry.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.339240 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/__init__.py
+-rw-rw-rw-   0        0        0     2527 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
+-rw-rw-rw-   0        0        0     6936 2023-04-20 19:54:07.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/wiki.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.348241 goodai-ltm-0.0.8/goodai/ltm/embedding_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/auto.py
+-rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/contrast_classifier.py
+-rw-rw-rw-   0        0        0     5368 2023-04-20 21:44:48.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/default.py
+-rw-rw-rw-   0        0        0     1533 2023-04-20 21:31:29.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/emb_qp_prob_model.py
+-rw-rw-rw-   0        0        0     2785 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/openai_emb.py
+-rw-rw-rw-   0        0        0     2224 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/st_emb.py
+-rw-rw-rw-   0        0        0     5437 2023-04-20 21:34:03.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/trainable.py
+-rw-rw-rw-   0        0        0     1584 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embeddings.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.355240 goodai-ltm-0.0.8/goodai/ltm/eval/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/eval/__init__.py
+-rw-rw-rw-   0        0        0     1038 2023-04-20 21:13:58.000000 goodai-ltm-0.0.8/goodai/ltm/eval/auto.py
+-rw-rw-rw-   0        0        0     4450 2023-04-20 19:42:22.000000 goodai-ltm-0.0.8/goodai/ltm/eval/mem.py
+-rw-rw-rw-   0        0        0     2716 2023-04-19 23:22:15.000000 goodai-ltm-0.0.8/goodai/ltm/eval/metrics.py
+-rw-rw-rw-   0        0        0     1901 2023-04-19 23:26:29.000000 goodai-ltm-0.0.8/goodai/ltm/eval/qrecc.py
+-rw-rw-rw-   0        0        0     2072 2023-04-20 20:01:17.000000 goodai-ltm-0.0.8/goodai/ltm/eval/strategy_qa.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.356240 goodai-ltm-0.0.8/goodai/ltm/eval/tests/
+-rw-rw-rw-   0        0        0     1420 2023-04-19 23:22:33.000000 goodai-ltm-0.0.8/goodai/ltm/eval/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     1188 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/matching.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.361240 goodai-ltm-0.0.8/goodai/ltm/matching_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/auto.py
+-rw-rw-rw-   0        0        0    10021 2023-04-20 21:36:37.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/default.py
+-rw-rw-rw-   0        0        0      706 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/prob_model.py
+-rw-rw-rw-   0        0        0      658 2023-04-19 21:49:37.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/st_ce.py
+-rw-rw-rw-   0        0        0     1208 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.371241 goodai-ltm-0.0.8/goodai/ltm/memory_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/__init__.py
+-rw-rw-rw-   0        0        0     1376 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/auto.py
+-rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk.py
+-rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_mixin.py
+-rw-rw-rw-   0        0        0    10364 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_queue.py
+-rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/config.py
+-rw-rw-rw-   0        0        0     5562 2023-04-19 22:25:35.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/default.py
+-rw-rw-rw-   0        0        0     5784 2023-04-19 22:27:29.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/mem_foundation.py
+-rw-rw-rw-   0        0        0     2960 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/simple_vector_db.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.373241 goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/__init__.py
+-rw-rw-rw-   0        0        0     3101 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/test_chunk_queue.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.375241 goodai-ltm-0.0.8/goodai/ltm/training/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.376241 goodai-ltm-0.0.8/goodai/ltm/training/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/training/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.8/goodai/ltm/training/query_passage/trainer.py
+-rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/training/sched_opt.py
+drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.381241 goodai-ltm-0.0.8/goodai_ltm.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2399 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 21:49:03.383241 goodai-ltm-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      657 2023-04-20 21:47:37.000000 goodai-ltm-0.0.8/setup.py
```

### Comparing `goodai-ltm-0.0.7/README.md` & `goodai-ltm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/helpers/collections_helper.py` & `goodai-ltm-0.0.8/goodai/helpers/collections_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/helpers/file_helper.py` & `goodai-ltm-0.0.8/goodai/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/helpers/tokenizer_helper.py` & `goodai-ltm-0.0.8/goodai/helpers/tokenizer_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/cloud.py` & `goodai-ltm-0.0.8/goodai/ltm/data/cloud.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/names/__init__.py` & `goodai-ltm-0.0.8/goodai/ltm/data/names/__init__.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/names/wikidata-names.json` & `goodai-ltm-0.0.8/goodai/ltm/data/names/wikidata-names.json`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/query_passage/auto_data_source.py` & `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/auto_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/query_passage/dataset.py` & `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/dataset.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/query_passage/qa.py` & `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/query_passage/qa_tok_entry.py` & `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa_tok_entry.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py` & `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/data/query_passage/wiki.py` & `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/wiki.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embedding_models/auto.py` & `goodai-ltm-0.0.8/goodai/ltm/embedding_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embedding_models/contrast_classifier.py` & `goodai-ltm-0.0.8/goodai/ltm/embedding_models/contrast_classifier.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embedding_models/default.py` & `goodai-ltm-0.0.8/goodai/ltm/embedding_models/default.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,41 +68,41 @@
         token_embeddings = lm_output.last_hidden_state
         # token_embeddings: (batch_size, seq_len, emb_size,)
         slf_att_logits_1 = self.out_model(token_embeddings)
         slf_att_logits = slf_att_logits_1 - 200 * (1.0 - out_att_mask[:, :, None])
         slf_att_logits = torch.clamp(slf_att_logits, min=-100, max=+80)
         slf_att_weights = torch.softmax(slf_att_logits, dim=1)
         # slf_att_weights: (batch_size, seq_len, total_keys,)
-        dot_product = token_embeddings[:, :, None, :] * slf_att_weights[:, :, :, None]
-        # dot_product: (batch_size, seq_len, total_keys, emb_size,)
+        emb_product = token_embeddings[:, :, None, :] * slf_att_weights[:, :, :, None]
+        # emb_product: (batch_size, seq_len, total_keys, emb_size,)
         if is_retrieve:
-            key_dot_product = dot_product[:, :, self.num_storage_emb:, :]
+            relevant_product = emb_product[:, :, self.num_storage_emb:, :]
         else:
-            key_dot_product = dot_product[:, :, :self.num_storage_emb, :]
-        raw_key_mean = torch.sum(key_dot_product, dim=1)
+            relevant_product = emb_product[:, :, :self.num_storage_emb, :]
+        raw_key_mean = torch.sum(relevant_product, dim=1)
         # raw_key_mean: (batch_size, num_keys, emb_size,)
         return F.normalize(raw_key_mean, dim=2)
 
     def get_lm_parameters(self):
         return self.lang_model.parameters()
 
     def get_added_parameters(self):
         return itertools.chain(self.out_model.parameters())
 
-    def get_storage_key(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
+    def get_storage_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
         return self(input_ids=input_ids, token_lengths=None, attention_mask=attention_mask, is_retrieve=False)
 
-    def get_retrieval_key(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
+    def get_retrieval_emb(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
                           attention_mask: torch.Tensor = None) -> torch.Tensor:
         return self(input_ids=input_ids, token_lengths=token_lengths, attention_mask=attention_mask,
                     is_retrieve=True)
 
-    def get_keys(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-        sk = self.get_storage_key(input_ids, attention_mask)
-        rk = self.get_retrieval_key(input_ids, attention_mask)
+    def get_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+        sk = self.get_storage_emb(input_ids, attention_mask)
+        rk = self.get_retrieval_emb(input_ids, attention_mask)
         return sk, rk,
 
     def get_embedding_dim(self) -> int:
         return self.emb_dim
 
     def get_num_retrieval_embeddings(self) -> int:
         return self.num_retrieval_emb
```

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embedding_models/emb_qp_prob_model.py` & `goodai-ltm-0.0.8/goodai/ltm/embedding_models/emb_qp_prob_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
         self.emb_model = emb_model
         scale = math.sqrt(emb_model.get_embedding_dim())
         self.classifier = ContrastClassifier(scale)
 
     def forward(self, query_input_ids: torch.Tensor, query_attention_mask: torch.Tensor,
                 query_token_lengths: torch.Tensor,
                 passage_input_ids: torch.Tensor, passage_attention_mask: torch.Tensor) -> torch.Tensor:
-        rk = self.emb_model.get_retrieval_key(query_input_ids, token_lengths=query_token_lengths,
+        rk = self.emb_model.get_retrieval_emb(query_input_ids, token_lengths=query_token_lengths,
                                               attention_mask=query_attention_mask)
-        sk = self.emb_model.get_storage_key(passage_input_ids, passage_attention_mask)
+        sk = self.emb_model.get_storage_emb(passage_input_ids, passage_attention_mask)
         return self.classifier(rk, sk)
 
     def get_lm_parameters(self):
         return self.emb_model.get_lm_parameters()
 
     def get_added_parameters(self):
         km_added_parameters = self.emb_model.get_added_parameters()
```

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embedding_models/openai_emb.py` & `goodai-ltm-0.0.8/goodai/ltm/embedding_models/openai_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embedding_models/st_emb.py` & `goodai-ltm-0.0.8/goodai/ltm/embedding_models/st_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embedding_models/trainable.py` & `goodai-ltm-0.0.8/goodai/ltm/embedding_models/trainable.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,30 +25,30 @@
         self.tokenizer = tokenizer
         self.pad_token_id = get_pad_token_id(tokenizer)
 
     def get_device(self):
         return self.dummy.device
 
     @abstractmethod
-    def get_storage_key(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
+    def get_storage_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor = None) -> torch.Tensor:
         """
         Returns an embedding of shape (batch_size, num_keys, emb_size,)
         """
         pass
 
     @abstractmethod
-    def get_retrieval_key(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
+    def get_retrieval_emb(self, input_ids: torch.Tensor, token_lengths: torch.Tensor,
                           attention_mask: torch.Tensor = None) -> torch.Tensor:
         """
         Returns an embedding of shape (batch_size, emb_size,)
         """
         pass
 
     @abstractmethod
-    def get_keys(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+    def get_emb(self, input_ids: torch.Tensor, attention_mask: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         Returns storage and retrieval embeddings.
         """
         pass
 
     @abstractmethod
     def get_lm_parameters(self):
@@ -60,26 +60,26 @@
     @abstractmethod
     def get_added_parameters(self):
         """
         :return: New parameters that don't belong to the pretrained language model.
         """
         pass
 
-    def get_storage_key_for_ids(self, input_ids: List[List[int]]):
+    def get_storage_emb_for_ids(self, input_ids: List[List[int]]):
         device = self.get_device()
         pad_token_id = self.pad_token_id
         m_inputs = get_model_inputs(input_ids, pad_id=pad_token_id, device=device)
-        return self.get_storage_key(**m_inputs)
+        return self.get_storage_emb(**m_inputs)
 
-    def get_retrieval_key_for_ids(self, input_ids: List[List[int]]):
+    def get_retrieval_emb_for_ids(self, input_ids: List[List[int]]):
         device = self.get_device()
         pad_token_id = self.pad_token_id
         m_inputs = get_model_inputs(input_ids, pad_id=pad_token_id, device=device, return_token_lengths=True,
                                     tokenizer=self.tokenizer)
-        return self.get_retrieval_key(**m_inputs)
+        return self.get_retrieval_emb(**m_inputs)
 
     def _get_token_ids(self, texts: List[str]) -> List[List[int]]:
         tok = self.tokenizer
         return [tok.encode(text, add_special_tokens=False) for text in texts]
 
     def encode_in_batches(self, enc_fn: Callable, sentences: List[str], batch_size: int = 64,
                           show_progress_bar: bool = False,
@@ -105,21 +105,21 @@
             return result
         else:
             return result.detach().cpu().numpy()
 
     def encode_queries(self, queries: List[str], batch_size: int = 64, show_progress_bar: bool = False,
                        convert_to_tensor: bool = False,
                        device: Union[str, torch.device] = None) -> Union[np.ndarray, torch.Tensor]:
-        return self.encode_in_batches(self.get_retrieval_key, queries, batch_size=batch_size,
+        return self.encode_in_batches(self.get_retrieval_emb, queries, batch_size=batch_size,
                                       show_progress_bar=show_progress_bar,
                                       convert_to_tensor=convert_to_tensor,
                                       return_token_lengths=True,
                                       device=device)
 
     def encode_corpus(self, passages: List[str], batch_size: int = 64, show_progress_bar: bool = False,
                       convert_to_tensor: bool = False,
                       device: Union[str, torch.device] = None) -> Union[np.ndarray, torch.Tensor]:
-        return self.encode_in_batches(self.get_retrieval_key, passages, batch_size=batch_size,
+        return self.encode_in_batches(self.get_storage_emb, passages, batch_size=batch_size,
                                       show_progress_bar=show_progress_bar,
                                       convert_to_tensor=convert_to_tensor,
                                       return_token_lengths=False,
                                       device=device)
```

### Comparing `goodai-ltm-0.0.7/goodai/ltm/embeddings.py` & `goodai-ltm-0.0.8/goodai/ltm/embeddings.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/eval/auto.py` & `goodai-ltm-0.0.8/goodai/ltm/eval/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/eval/mem.py` & `goodai-ltm-0.0.8/goodai/ltm/eval/mem.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/eval/metrics.py` & `goodai-ltm-0.0.8/goodai/ltm/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/eval/qrecc.py` & `goodai-ltm-0.0.8/goodai/ltm/eval/qrecc.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/eval/strategy_qa.py` & `goodai-ltm-0.0.8/goodai/ltm/eval/strategy_qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/eval/tests/test_metrics.py` & `goodai-ltm-0.0.8/goodai/ltm/eval/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/matching.py` & `goodai-ltm-0.0.8/goodai/ltm/matching.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/matching_models/auto.py` & `goodai-ltm-0.0.8/goodai/ltm/matching_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/matching_models/default.py` & `goodai-ltm-0.0.8/goodai/ltm/matching_models/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         passage_ids_list = []
         for query, passage in sentences:
             query_ids = tokenizer.encode(query, add_special_tokens=False)
             if len(query_ids) > max_query_tokens:
                 query_ids = query_ids[-max_query_tokens:]
             passage_ids = tokenizer.encode(passage, add_special_tokens=False)
             if len(passage_ids) > max_passage_tokens:
-                passage_ids = query_ids[-max_passage_tokens:]
+                passage_ids = passage_ids[-max_passage_tokens:]
             passage_ids_list.append(passage_ids)
             query_ids_list.append(query_ids)
         # Convert input_ids_list to tensor input_ids and attention_mask by adding padding
         device = self.get_device()
         query_seq_len = self.default_query_seq_len if use_preferred_seq_lengths else None
         passage_seq_len = self.default_passage_seq_len if use_preferred_seq_lengths else None
         query_inputs = get_model_inputs(query_ids_list, pad_id, device, prefix='query_',
```

### Comparing `goodai-ltm-0.0.7/goodai/ltm/matching_models/prob_model.py` & `goodai-ltm-0.0.8/goodai/ltm/matching_models/prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/matching_models/st_ce.py` & `goodai-ltm-0.0.8/goodai/ltm/matching_models/st_ce.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory.py` & `goodai-ltm-0.0.8/goodai/ltm/memory.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/auto.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/chunk.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/chunk_mixin.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_mixin.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/chunk_queue.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_queue.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/default.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/mem_foundation.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/mem_foundation.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/simple_vector_db.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/simple_vector_db.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/memory_models/tests/test_chunk_queue.py` & `goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/test_chunk_queue.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/training/query_passage/trainer.py` & `goodai-ltm-0.0.8/goodai/ltm/training/query_passage/trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai/ltm/training/sched_opt.py` & `goodai-ltm-0.0.8/goodai/ltm/training/sched_opt.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/goodai_ltm.egg-info/SOURCES.txt` & `goodai-ltm-0.0.8/goodai_ltm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.7/setup.py` & `goodai-ltm-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 packages = find_namespace_packages(include=['goodai.*'])
 
 setup(name='goodai-ltm',
       description='A text memory meant to be used with conversational language models.',
       url='https://github.com/GoodAI/goodai-ltm',
-      version='0.0.7',
+      version='0.0.8',
       packages=packages,
       package_data={'goodai.ltm.data': ['**/*.json']},
       install_requires=['torch>=1.8.0', 'pytest>=7.0.0', 'numpy>=1.19.0', 'transformers>=4.0.0',
                         'openai>=0.27.0', 'faiss-cpu', 'datasets', 'boto3', 'python-dotenv',
                         'sentence-transformers>=2.2.2']
 )
```

