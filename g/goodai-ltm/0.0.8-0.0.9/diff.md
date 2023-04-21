# Comparing `tmp/goodai-ltm-0.0.8.tar.gz` & `tmp/goodai-ltm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodai-ltm-0.0.8.tar", last modified: Thu Apr 20 21:49:03 2023, max compression
+gzip compressed data, was "goodai-ltm-0.0.9.tar", last modified: Thu Apr 20 22:03:06 2023, max compression
```

## Comparing `goodai-ltm-0.0.8.tar` & `goodai-ltm-0.0.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.383241 goodai-ltm-0.0.8/
--rw-rw-rw-   0        0        0      184 2023-04-20 21:49:03.382240 goodai-ltm-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-04-19 21:51:49.000000 goodai-ltm-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.295210 goodai-ltm-0.0.8/goodai/
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.320241 goodai-ltm-0.0.8/goodai/helpers/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/helpers/__init__.py
--rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/collections_helper.py
--rw-rw-rw-   0        0        0      717 2023-04-19 20:33:13.000000 goodai-ltm-0.0.8/goodai/helpers/file_helper.py
--rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/html_helper.py
--rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/json_helper.py
--rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/tokenizer_helper.py
--rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.324240 goodai-ltm-0.0.8/goodai/ltm/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.325241 goodai-ltm-0.0.8/goodai/ltm/data/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/data/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/data/cloud.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.327241 goodai-ltm-0.0.8/goodai/ltm/data/names/
--rw-rw-rw-   0        0        0     1996 2023-04-19 22:25:12.000000 goodai-ltm-0.0.8/goodai/ltm/data/names/__init__.py
--rw-rw-rw-   0        0        0   183119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/data/names/wikidata-names.json
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.337240 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/__init__.py
--rw-rw-rw-   0        0        0     1626 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/auto_data_source.py
--rw-rw-rw-   0        0        0      485 2023-04-20 19:49:15.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/data_source.py
--rw-rw-rw-   0        0        0     2422 2023-04-19 22:26:45.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/dataset.py
--rw-rw-rw-   0        0        0      331 2023-04-20 19:47:41.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/example.py
--rw-rw-rw-   0        0        0    11044 2023-04-20 19:51:43.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa.py
--rw-rw-rw-   0        0        0     1857 2023-04-19 22:30:12.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa_tok_entry.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.339240 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/__init__.py
--rw-rw-rw-   0        0        0     2527 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
--rw-rw-rw-   0        0        0     6936 2023-04-20 19:54:07.000000 goodai-ltm-0.0.8/goodai/ltm/data/query_passage/wiki.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.348241 goodai-ltm-0.0.8/goodai/ltm/embedding_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/auto.py
--rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/contrast_classifier.py
--rw-rw-rw-   0        0        0     5368 2023-04-20 21:44:48.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/default.py
--rw-rw-rw-   0        0        0     1533 2023-04-20 21:31:29.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/emb_qp_prob_model.py
--rw-rw-rw-   0        0        0     2785 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/openai_emb.py
--rw-rw-rw-   0        0        0     2224 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/st_emb.py
--rw-rw-rw-   0        0        0     5437 2023-04-20 21:34:03.000000 goodai-ltm-0.0.8/goodai/ltm/embedding_models/trainable.py
--rw-rw-rw-   0        0        0     1584 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/embeddings.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.355240 goodai-ltm-0.0.8/goodai/ltm/eval/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/eval/__init__.py
--rw-rw-rw-   0        0        0     1038 2023-04-20 21:13:58.000000 goodai-ltm-0.0.8/goodai/ltm/eval/auto.py
--rw-rw-rw-   0        0        0     4450 2023-04-20 19:42:22.000000 goodai-ltm-0.0.8/goodai/ltm/eval/mem.py
--rw-rw-rw-   0        0        0     2716 2023-04-19 23:22:15.000000 goodai-ltm-0.0.8/goodai/ltm/eval/metrics.py
--rw-rw-rw-   0        0        0     1901 2023-04-19 23:26:29.000000 goodai-ltm-0.0.8/goodai/ltm/eval/qrecc.py
--rw-rw-rw-   0        0        0     2072 2023-04-20 20:01:17.000000 goodai-ltm-0.0.8/goodai/ltm/eval/strategy_qa.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.356240 goodai-ltm-0.0.8/goodai/ltm/eval/tests/
--rw-rw-rw-   0        0        0     1420 2023-04-19 23:22:33.000000 goodai-ltm-0.0.8/goodai/ltm/eval/tests/test_metrics.py
--rw-rw-rw-   0        0        0     1188 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/matching.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.361240 goodai-ltm-0.0.8/goodai/ltm/matching_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/__init__.py
--rw-rw-rw-   0        0        0      777 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/auto.py
--rw-rw-rw-   0        0        0    10021 2023-04-20 21:36:37.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/default.py
--rw-rw-rw-   0        0        0      706 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/prob_model.py
--rw-rw-rw-   0        0        0      658 2023-04-19 21:49:37.000000 goodai-ltm-0.0.8/goodai/ltm/matching_models/st_ce.py
--rw-rw-rw-   0        0        0     1208 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.371241 goodai-ltm-0.0.8/goodai/ltm/memory_models/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/__init__.py
--rw-rw-rw-   0        0        0     1376 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/auto.py
--rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk.py
--rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_mixin.py
--rw-rw-rw-   0        0        0    10364 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_queue.py
--rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/config.py
--rw-rw-rw-   0        0        0     5562 2023-04-19 22:25:35.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/default.py
--rw-rw-rw-   0        0        0     5784 2023-04-19 22:27:29.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/mem_foundation.py
--rw-rw-rw-   0        0        0     2960 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/simple_vector_db.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.373241 goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/__init__.py
--rw-rw-rw-   0        0        0     3101 2023-04-20 15:19:11.000000 goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/test_chunk_queue.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.375241 goodai-ltm-0.0.8/goodai/ltm/training/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/training/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.376241 goodai-ltm-0.0.8/goodai/ltm/training/query_passage/
--rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.8/goodai/ltm/training/query_passage/__init__.py
--rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.8/goodai/ltm/training/query_passage/trainer.py
--rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.8/goodai/ltm/training/sched_opt.py
-drwxrwxrwx   0        0        0        0 2023-04-20 21:49:03.381241 goodai-ltm-0.0.8/goodai_ltm.egg-info/
--rw-rw-rw-   0        0        0      184 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2399 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-20 21:49:03.000000 goodai-ltm-0.0.8/goodai_ltm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 21:49:03.383241 goodai-ltm-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      657 2023-04-20 21:47:37.000000 goodai-ltm-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.622628 goodai-ltm-0.0.9/
+-rw-rw-rw-   0        0        0      184 2023-04-20 22:03:06.622628 goodai-ltm-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-04-19 21:51:49.000000 goodai-ltm-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.537898 goodai-ltm-0.0.9/goodai/
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.563640 goodai-ltm-0.0.9/goodai/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1357 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/helpers/collections_helper.py
+-rw-rw-rw-   0        0        0      717 2023-04-19 20:33:13.000000 goodai-ltm-0.0.9/goodai/helpers/file_helper.py
+-rw-rw-rw-   0        0        0      214 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/helpers/html_helper.py
+-rw-rw-rw-   0        0        0      165 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/helpers/json_helper.py
+-rw-rw-rw-   0        0        0     3910 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/helpers/tokenizer_helper.py
+-rw-rw-rw-   0        0        0      119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.566640 goodai-ltm-0.0.9/goodai/ltm/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.568640 goodai-ltm-0.0.9/goodai/ltm/data/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/data/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/ltm/data/cloud.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.570628 goodai-ltm-0.0.9/goodai/ltm/data/names/
+-rw-rw-rw-   0        0        0     1996 2023-04-19 22:25:12.000000 goodai-ltm-0.0.9/goodai/ltm/data/names/__init__.py
+-rw-rw-rw-   0        0        0   183119 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/ltm/data/names/wikidata-names.json
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.578627 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     1626 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/auto_data_source.py
+-rw-rw-rw-   0        0        0      485 2023-04-20 19:49:15.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/data_source.py
+-rw-rw-rw-   0        0        0     2422 2023-04-19 22:26:45.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/dataset.py
+-rw-rw-rw-   0        0        0      331 2023-04-20 19:47:41.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/example.py
+-rw-rw-rw-   0        0        0    11044 2023-04-20 19:51:43.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/qa.py
+-rw-rw-rw-   0        0        0     1857 2023-04-19 22:30:12.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/qa_tok_entry.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.580627 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/tests/__init__.py
+-rw-rw-rw-   0        0        0     2527 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py
+-rw-rw-rw-   0        0        0     6936 2023-04-20 19:54:07.000000 goodai-ltm-0.0.9/goodai/ltm/data/query_passage/wiki.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.589627 goodai-ltm-0.0.9/goodai/ltm/embedding_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/auto.py
+-rw-rw-rw-   0        0        0     1554 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/contrast_classifier.py
+-rw-rw-rw-   0        0        0     5368 2023-04-20 21:44:48.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/default.py
+-rw-rw-rw-   0        0        0     1533 2023-04-20 21:31:29.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/emb_qp_prob_model.py
+-rw-rw-rw-   0        0        0     2785 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/openai_emb.py
+-rw-rw-rw-   0        0        0     2224 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/st_emb.py
+-rw-rw-rw-   0        0        0     5508 2023-04-20 21:55:59.000000 goodai-ltm-0.0.9/goodai/ltm/embedding_models/trainable.py
+-rw-rw-rw-   0        0        0     1584 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/embeddings.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.595627 goodai-ltm-0.0.9/goodai/ltm/eval/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/eval/__init__.py
+-rw-rw-rw-   0        0        0     1038 2023-04-20 21:13:58.000000 goodai-ltm-0.0.9/goodai/ltm/eval/auto.py
+-rw-rw-rw-   0        0        0     4450 2023-04-20 19:42:22.000000 goodai-ltm-0.0.9/goodai/ltm/eval/mem.py
+-rw-rw-rw-   0        0        0     2716 2023-04-19 23:22:15.000000 goodai-ltm-0.0.9/goodai/ltm/eval/metrics.py
+-rw-rw-rw-   0        0        0     1901 2023-04-19 23:26:29.000000 goodai-ltm-0.0.9/goodai/ltm/eval/qrecc.py
+-rw-rw-rw-   0        0        0     2072 2023-04-20 20:01:17.000000 goodai-ltm-0.0.9/goodai/ltm/eval/strategy_qa.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.596627 goodai-ltm-0.0.9/goodai/ltm/eval/tests/
+-rw-rw-rw-   0        0        0     1420 2023-04-19 23:22:33.000000 goodai-ltm-0.0.9/goodai/ltm/eval/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     1188 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/matching.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.601627 goodai-ltm-0.0.9/goodai/ltm/matching_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:01.000000 goodai-ltm-0.0.9/goodai/ltm/matching_models/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/matching_models/auto.py
+-rw-rw-rw-   0        0        0    10021 2023-04-20 21:36:37.000000 goodai-ltm-0.0.9/goodai/ltm/matching_models/default.py
+-rw-rw-rw-   0        0        0      706 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/matching_models/prob_model.py
+-rw-rw-rw-   0        0        0      658 2023-04-19 21:49:37.000000 goodai-ltm-0.0.9/goodai/ltm/matching_models/st_ce.py
+-rw-rw-rw-   0        0        0     1208 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/memory.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.611627 goodai-ltm-0.0.9/goodai/ltm/memory_models/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/__init__.py
+-rw-rw-rw-   0        0        0     1376 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/auto.py
+-rw-rw-rw-   0        0        0     1238 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/chunk.py
+-rw-rw-rw-   0        0        0      679 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/chunk_mixin.py
+-rw-rw-rw-   0        0        0    10364 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/chunk_queue.py
+-rw-rw-rw-   0        0        0      181 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/config.py
+-rw-rw-rw-   0        0        0     5562 2023-04-19 22:25:35.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/default.py
+-rw-rw-rw-   0        0        0     5784 2023-04-19 22:27:29.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/mem_foundation.py
+-rw-rw-rw-   0        0        0     2960 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/simple_vector_db.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.612627 goodai-ltm-0.0.9/goodai/ltm/memory_models/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/tests/__init__.py
+-rw-rw-rw-   0        0        0     3101 2023-04-20 15:19:11.000000 goodai-ltm-0.0.9/goodai/ltm/memory_models/tests/test_chunk_queue.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.614627 goodai-ltm-0.0.9/goodai/ltm/training/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/training/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.616628 goodai-ltm-0.0.9/goodai/ltm/training/query_passage/
+-rw-rw-rw-   0        0        0        0 2023-04-19 16:47:00.000000 goodai-ltm-0.0.9/goodai/ltm/training/query_passage/__init__.py
+-rw-rw-rw-   0        0        0     7132 2023-04-19 16:47:45.000000 goodai-ltm-0.0.9/goodai/ltm/training/query_passage/trainer.py
+-rw-rw-rw-   0        0        0     1473 2023-04-18 18:54:58.000000 goodai-ltm-0.0.9/goodai/ltm/training/sched_opt.py
+drwxrwxrwx   0        0        0        0 2023-04-20 22:03:06.621628 goodai-ltm-0.0.9/goodai_ltm.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-04-20 22:03:06.000000 goodai-ltm-0.0.9/goodai_ltm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2399 2023-04-20 22:03:06.000000 goodai-ltm-0.0.9/goodai_ltm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 22:03:06.000000 goodai-ltm-0.0.9/goodai_ltm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-04-20 22:03:06.000000 goodai-ltm-0.0.9/goodai_ltm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-20 22:03:06.000000 goodai-ltm-0.0.9/goodai_ltm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 22:03:06.623627 goodai-ltm-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-04-20 21:58:31.000000 goodai-ltm-0.0.9/setup.py
```

### Comparing `goodai-ltm-0.0.8/README.md` & `goodai-ltm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/helpers/collections_helper.py` & `goodai-ltm-0.0.9/goodai/helpers/collections_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/helpers/file_helper.py` & `goodai-ltm-0.0.9/goodai/helpers/file_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/helpers/tokenizer_helper.py` & `goodai-ltm-0.0.9/goodai/helpers/tokenizer_helper.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/cloud.py` & `goodai-ltm-0.0.9/goodai/ltm/data/cloud.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/names/__init__.py` & `goodai-ltm-0.0.9/goodai/ltm/data/names/__init__.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/names/wikidata-names.json` & `goodai-ltm-0.0.9/goodai/ltm/data/names/wikidata-names.json`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/auto_data_source.py` & `goodai-ltm-0.0.9/goodai/ltm/data/query_passage/auto_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/dataset.py` & `goodai-ltm-0.0.9/goodai/ltm/data/query_passage/dataset.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa.py` & `goodai-ltm-0.0.9/goodai/ltm/data/query_passage/qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/qa_tok_entry.py` & `goodai-ltm-0.0.9/goodai/ltm/data/query_passage/qa_tok_entry.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py` & `goodai-ltm-0.0.9/goodai/ltm/data/query_passage/tests/test_query_passage_data_source.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/data/query_passage/wiki.py` & `goodai-ltm-0.0.9/goodai/ltm/data/query_passage/wiki.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embedding_models/auto.py` & `goodai-ltm-0.0.9/goodai/ltm/embedding_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embedding_models/contrast_classifier.py` & `goodai-ltm-0.0.9/goodai/ltm/embedding_models/contrast_classifier.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embedding_models/default.py` & `goodai-ltm-0.0.9/goodai/ltm/embedding_models/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embedding_models/emb_qp_prob_model.py` & `goodai-ltm-0.0.9/goodai/ltm/embedding_models/emb_qp_prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embedding_models/openai_emb.py` & `goodai-ltm-0.0.9/goodai/ltm/embedding_models/openai_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embedding_models/st_emb.py` & `goodai-ltm-0.0.9/goodai/ltm/embedding_models/st_emb.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embedding_models/trainable.py` & `goodai-ltm-0.0.9/goodai/ltm/embedding_models/trainable.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             rng = tqdm(rng, desc='Embeddings', unit='batch')
         keys_list = []
         for b0 in rng:
             b_sentences = sentences[b0:b0 + batch_size]
             input_ids_list = [t.encode(s, add_special_tokens=False) for s in b_sentences]
             model_inputs = get_model_inputs(input_ids_list, self.pad_token_id,
                                             return_token_lengths=return_token_lengths,
+                                            tokenizer=self.tokenizer,
                                             device=device)
             keys = enc_fn(**model_inputs)
             keys_list.append(keys)
         result = torch.cat(keys_list)
         if convert_to_tensor:
             return result
         else:
```

### Comparing `goodai-ltm-0.0.8/goodai/ltm/embeddings.py` & `goodai-ltm-0.0.9/goodai/ltm/embeddings.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/eval/auto.py` & `goodai-ltm-0.0.9/goodai/ltm/eval/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/eval/mem.py` & `goodai-ltm-0.0.9/goodai/ltm/eval/mem.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/eval/metrics.py` & `goodai-ltm-0.0.9/goodai/ltm/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/eval/qrecc.py` & `goodai-ltm-0.0.9/goodai/ltm/eval/qrecc.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/eval/strategy_qa.py` & `goodai-ltm-0.0.9/goodai/ltm/eval/strategy_qa.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/eval/tests/test_metrics.py` & `goodai-ltm-0.0.9/goodai/ltm/eval/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/matching.py` & `goodai-ltm-0.0.9/goodai/ltm/matching.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/matching_models/auto.py` & `goodai-ltm-0.0.9/goodai/ltm/matching_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/matching_models/default.py` & `goodai-ltm-0.0.9/goodai/ltm/matching_models/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/matching_models/prob_model.py` & `goodai-ltm-0.0.9/goodai/ltm/matching_models/prob_model.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/matching_models/st_ce.py` & `goodai-ltm-0.0.9/goodai/ltm/matching_models/st_ce.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory.py` & `goodai-ltm-0.0.9/goodai/ltm/memory.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/auto.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/auto.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/chunk.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_mixin.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/chunk_mixin.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/chunk_queue.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/chunk_queue.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/default.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/default.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/mem_foundation.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/mem_foundation.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/simple_vector_db.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/simple_vector_db.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/memory_models/tests/test_chunk_queue.py` & `goodai-ltm-0.0.9/goodai/ltm/memory_models/tests/test_chunk_queue.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/training/query_passage/trainer.py` & `goodai-ltm-0.0.9/goodai/ltm/training/query_passage/trainer.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai/ltm/training/sched_opt.py` & `goodai-ltm-0.0.9/goodai/ltm/training/sched_opt.py`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/goodai_ltm.egg-info/SOURCES.txt` & `goodai-ltm-0.0.9/goodai_ltm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goodai-ltm-0.0.8/setup.py` & `goodai-ltm-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from setuptools import setup, find_packages, find_namespace_packages
+from setuptools import setup, find_namespace_packages
 
 packages = find_namespace_packages(include=['goodai.*'])
 
 setup(name='goodai-ltm',
       description='A text memory meant to be used with conversational language models.',
       url='https://github.com/GoodAI/goodai-ltm',
-      version='0.0.8',
+      version='0.0.9',
       packages=packages,
       package_data={'goodai.ltm.data': ['**/*.json']},
       install_requires=['torch>=1.8.0', 'pytest>=7.0.0', 'numpy>=1.19.0', 'transformers>=4.0.0',
                         'openai>=0.27.0', 'faiss-cpu', 'datasets', 'boto3', 'python-dotenv',
                         'sentence-transformers>=2.2.2']
 )
```

