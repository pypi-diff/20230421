# Comparing `tmp/fschat-0.2.2.tar.gz` & `tmp/fschat-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.2.tar", last modified: Sun Apr 16 13:22:37 2023, max compression
+gzip compressed data, was "fschat-0.2.3.tar", last modified: Fri Apr 21 09:16:52 2023, max compression
```

## Comparing `fschat-0.2.2.tar` & `fschat-0.2.3.tar`

### file list

```diff
@@ -1,61 +1,68 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12292 2023-04-16 13:22:37.921172 fschat-0.2.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11818 2023-04-16 13:16:40.000000 fschat-0.2.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.913172 fschat-0.2.2/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6288 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.917172 fschat-0.2.2/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/alpaca-converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5543 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5976 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      615 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2684 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3188 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.917172 fschat-0.2.2/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3661 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3072 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2345 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.917172 fschat-0.2.2/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5704 2023-04-16 09:48:14.000000 fschat-0.2.2/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1669 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/model/make_delta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11255 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5478 2023-04-16 09:48:14.000000 fschat-0.2.2/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9943 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2717 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7343 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16562 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2120 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8321 2023-04-16 13:00:59.000000 fschat-0.2.2/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7202 2023-04-16 09:48:14.000000 fschat-0.2.2/fastchat/serve/model_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      904 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/serve_chatglm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2429 2023-04-16 12:58:41.000000 fschat-0.2.2/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3867 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3982 2023-04-16 08:29:15.000000 fschat-0.2.2/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8450 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/train/train.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    15586 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/train/train_flant5.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3649 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      345 2023-04-16 08:29:18.000000 fschat-0.2.2/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4999 2023-04-16 09:48:12.000000 fschat-0.2.2/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 13:22:37.921172 fschat-0.2.2/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12292 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1505 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      181 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-16 13:22:37.000000 fschat-0.2.2/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-04-16 13:10:56.000000 fschat-0.2.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-16 13:22:37.921172 fschat-0.2.2/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.877371 fschat-0.2.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13822 2023-04-21 09:16:52.877371 fschat-0.2.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13328 2023-04-20 20:43:00.000000 fschat-0.2.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-21 08:18:30.000000 fschat-0.2.3/fastchat/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-18 08:21:09.000000 fschat-0.2.3/fastchat/client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/client/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/client/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8880 2023-04-21 07:20:06.000000 fschat-0.2.3/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/alpaca-converter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5826 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5979 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      616 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3200 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.869371 fschat-0.2.3/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3166 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5998 2023-04-21 08:31:12.000000 fschat-0.2.3/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1688 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/model/make_delta.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/protocol/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-18 08:21:09.000000 fschat-0.2.3/fastchat/protocol/chat_completion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5295 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11251 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5773 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3908 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10058 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7364 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17731 2023-04-21 08:09:53.000000 fschat-0.2.3/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15008 2023-04-21 08:09:56.000000 fschat-0.2.3/fastchat/serve/gradio_web_server_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2306 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10824 2023-04-21 07:20:06.000000 fschat-0.2.3/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7636 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/model_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.3/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      885 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/serve_chatglm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2480 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.873371 fschat-0.2.3/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8126 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/train.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5051 2023-04-21 07:02:29.000000 fschat-0.2.3/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-21 09:16:52.877371 fschat-0.2.3/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13822 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1657 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      241 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-04-21 09:16:52.000000 fschat-0.2.3/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1128 2023-04-21 08:17:20.000000 fschat-0.2.3/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-21 09:16:52.877371 fschat-0.2.3/setup.cfg
```

### Comparing `fschat-0.2.2/LICENSE` & `fschat-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.2/PKG-INFO` & `fschat-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: fschat
-Version: 0.2.2
-Summary: An open platform for training, serving, and evaluating large language model based chatbots.
-Project-URL: Homepage, https://github.com/lm-sys/fastchat
-Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FastChat
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
@@ -183,16 +171,81 @@
 
 
 ## API
 
 ### Huggingface Generation APIs
 See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py)
 
-### OpenAI-compatible RESTful APIs
-Coming soon.
+### OpenAI-compatible RESTful APIs & SDK
+
+(Experimental. We will keep improving the API and SDK.)
+
+#### Chat Completion
+
+Reference: https://platform.openai.com/docs/api-reference/chat/create
+
+Some features/compatibilities to be implemented:
+
+- [ ] streaming
+- [ ] support of some parameters like `top_p`, `presence_penalty`
+- [ ] proper error handling (e.g. model not found)
+- [ ] the return value in the client SDK could be used like a dict
+
+
+**RESTful API Server**
+
+First, launch the controller
+
+```bash
+python3 -m fastchat.serve.controller
+```
+
+Then, launch the model worker(s)
+
+```bash
+python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights
+```
+
+Finally, launch the RESTful API server
+
+```bash
+export FASTCHAT_CONTROLLER_URL=http://localhost:21001
+python3 -m fastchat.serve.api --host localhost --port 8000
+```
+
+Test the API server
+
+```bash
+curl http://localhost:8000/v1/chat/completions \
+  -H "Content-Type: application/json" \
+  -d '{
+    "model": "vicuna-7b-v1.1",
+    "messages": [{"role": "user", "content": "Hello!"}]
+  }'
+```
+
+**Client SDK**
+
+Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://localhost:8000`), you can use the following code to send a request to the API server:
+
+```python
+import os
+from fastchat import client
+
+client.set_baseurl(os.getenv("FASTCHAT_BASEURL"))
+
+completion = client.ChatCompletion.create(
+  model="vicuna-7b-v1.1",
+  messages=[
+    {"role": "user", "content": "Hello!"}
+  ]
+)
+
+print(completion.choices[0].message)
+```
 
 ## Evaluation
 
 Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ### Pipeline Steps
```

#### html2text {}

```diff
@@ -1,14 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.2 Summary: An open platform for
-training, serving, and evaluating large language model based chatbots. Project-
-URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
-https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # FastChat An open platform for training, serving, and evaluating large
+# FastChat An open platform for training, serving, and evaluating large
 language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
@@ -86,23 +80,42 @@
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
 Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
 is the user interface that users will interact with. By following these steps,
 you will be able to serve your models using the web UI. You can open your
 browser and chat with a model now. ## API ### Huggingface Generation APIs See
 [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py) ###
-OpenAI-compatible RESTful APIs Coming soon. ## Evaluation Our AI-enhanced
-evaluation pipeline is based on GPT-4. This section provides a high-level
-summary of the pipeline. For detailed instructions, please refer to the
-[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
-answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
-specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
-models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
-automatically. This step can also be performed manually if the GPT-4 API is not
-available to you. 3. Generate visualization data: Run
+OpenAI-compatible RESTful APIs & SDK (Experimental. We will keep improving the
+API and SDK.) #### Chat Completion Reference: https://platform.openai.com/docs/
+api-reference/chat/create Some features/compatibilities to be implemented: -
+[ ] streaming - [ ] support of some parameters like `top_p`, `presence_penalty`
+- [ ] proper error handling (e.g. model not found) - [ ] the return value in
+the client SDK could be used like a dict **RESTful API Server** First, launch
+the controller ```bash python3 -m fastchat.serve.controller ``` Then, launch
+the model worker(s) ```bash python3 -m fastchat.serve.model_worker --model-name
+'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights ``` Finally, launch the
+RESTful API server ```bash export FASTCHAT_CONTROLLER_URL=http://localhost:
+21001 python3 -m fastchat.serve.api --host localhost --port 8000 ``` Test the
+API server ```bash curl http://localhost:8000/v1/chat/completions \ -
+H "Content-Type: application/json" \ -d '{ "model": "vicuna-7b-v1.1",
+"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Client SDK**
+Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL
+(e.g., `http://localhost:8000`), you can use the following code to send a
+request to the API server: ```python import os from fastchat import client
+client.set_baseurl(os.getenv("FASTCHAT_BASEURL")) completion =
+client.ChatCompletion.create( model="vicuna-7b-v1.1", messages=[ {"role":
+"user", "content": "Hello!"} ] ) print(completion.choices[0].message) ``` ##
+Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
+provides a high-level summary of the pipeline. For detailed instructions,
+please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
+Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
+ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
+Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
+reviews automatically. This step can also be performed manually if the GPT-
+4 API is not available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.2/README.md` & `fschat-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fschat
+Version: 0.2.3
+Summary: An open platform for training, serving, and evaluating large language model based chatbots.
+Project-URL: Homepage, https://github.com/lm-sys/fastchat
+Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # FastChat
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 
 <p align="center">
 <a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
@@ -171,16 +184,81 @@
 
 
 ## API
 
 ### Huggingface Generation APIs
 See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py)
 
-### OpenAI-compatible RESTful APIs
-Coming soon.
+### OpenAI-compatible RESTful APIs & SDK
+
+(Experimental. We will keep improving the API and SDK.)
+
+#### Chat Completion
+
+Reference: https://platform.openai.com/docs/api-reference/chat/create
+
+Some features/compatibilities to be implemented:
+
+- [ ] streaming
+- [ ] support of some parameters like `top_p`, `presence_penalty`
+- [ ] proper error handling (e.g. model not found)
+- [ ] the return value in the client SDK could be used like a dict
+
+
+**RESTful API Server**
+
+First, launch the controller
+
+```bash
+python3 -m fastchat.serve.controller
+```
+
+Then, launch the model worker(s)
+
+```bash
+python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights
+```
+
+Finally, launch the RESTful API server
+
+```bash
+export FASTCHAT_CONTROLLER_URL=http://localhost:21001
+python3 -m fastchat.serve.api --host localhost --port 8000
+```
+
+Test the API server
+
+```bash
+curl http://localhost:8000/v1/chat/completions \
+  -H "Content-Type: application/json" \
+  -d '{
+    "model": "vicuna-7b-v1.1",
+    "messages": [{"role": "user", "content": "Hello!"}]
+  }'
+```
+
+**Client SDK**
+
+Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://localhost:8000`), you can use the following code to send a request to the API server:
+
+```python
+import os
+from fastchat import client
+
+client.set_baseurl(os.getenv("FASTCHAT_BASEURL"))
+
+completion = client.ChatCompletion.create(
+  model="vicuna-7b-v1.1",
+  messages=[
+    {"role": "user", "content": "Hello!"}
+  ]
+)
+
+print(completion.choices[0].message)
+```
 
 ## Evaluation
 
 Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ### Pipeline Steps
```

#### html2text {}

```diff
@@ -1,9 +1,15 @@
-# FastChat An open platform for training, serving, and evaluating large
-language model based chatbots. ## Release
+Metadata-Version: 2.1 Name: fschat Version: 0.2.3 Summary: An open platform for
+training, serving, and evaluating large language model based chatbots. Project-
+URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
+https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # FastChat An open platform for training, serving,
+and evaluating large language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
@@ -80,23 +86,42 @@
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
 Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
 is the user interface that users will interact with. By following these steps,
 you will be able to serve your models using the web UI. You can open your
 browser and chat with a model now. ## API ### Huggingface Generation APIs See
 [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py) ###
-OpenAI-compatible RESTful APIs Coming soon. ## Evaluation Our AI-enhanced
-evaluation pipeline is based on GPT-4. This section provides a high-level
-summary of the pipeline. For detailed instructions, please refer to the
-[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
-answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
-specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
-models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
-automatically. This step can also be performed manually if the GPT-4 API is not
-available to you. 3. Generate visualization data: Run
+OpenAI-compatible RESTful APIs & SDK (Experimental. We will keep improving the
+API and SDK.) #### Chat Completion Reference: https://platform.openai.com/docs/
+api-reference/chat/create Some features/compatibilities to be implemented: -
+[ ] streaming - [ ] support of some parameters like `top_p`, `presence_penalty`
+- [ ] proper error handling (e.g. model not found) - [ ] the return value in
+the client SDK could be used like a dict **RESTful API Server** First, launch
+the controller ```bash python3 -m fastchat.serve.controller ``` Then, launch
+the model worker(s) ```bash python3 -m fastchat.serve.model_worker --model-name
+'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights ``` Finally, launch the
+RESTful API server ```bash export FASTCHAT_CONTROLLER_URL=http://localhost:
+21001 python3 -m fastchat.serve.api --host localhost --port 8000 ``` Test the
+API server ```bash curl http://localhost:8000/v1/chat/completions \ -
+H "Content-Type: application/json" \ -d '{ "model": "vicuna-7b-v1.1",
+"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Client SDK**
+Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL
+(e.g., `http://localhost:8000`), you can use the following code to send a
+request to the API server: ```python import os from fastchat import client
+client.set_baseurl(os.getenv("FASTCHAT_BASEURL")) completion =
+client.ChatCompletion.create( model="vicuna-7b-v1.1", messages=[ {"role":
+"user", "content": "Hello!"} ] ) print(completion.choices[0].message) ``` ##
+Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
+provides a high-level summary of the pipeline. For detailed instructions,
+please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
+Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
+ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
+Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
+reviews automatically. This step can also be performed manually if the GPT-
+4 API is not available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.2/fastchat/conversation.py` & `fschat-0.2.3/fastchat/conversation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,38 @@
+"""
+Conversation prompt template.
+
+Now we support
+- Vicuna
+- Koala
+- OpenAssistant/oasst-sft-1-pythia-12b
+- StabilityAI/stablelm-tuned-alpha-7b
+- databricks/dolly-v2-12b
+- THUDM/chatglm-6b
+- Alpaca/LLaMa
+"""
+
 import dataclasses
 from enum import auto, Enum
 from typing import List, Tuple, Any
 
 
 class SeparatorStyle(Enum):
     """Different separator style."""
+
     SINGLE = auto()
     TWO = auto()
     DOLLY = auto()
+    OASST_PYTHIA = auto()
 
 
 @dataclasses.dataclass
 class Conversation:
     """A class that keeps all conversation history."""
+
     system: str
     roles: List[str]
     messages: List[List[str]]
     offset: int
     sep_style: SeparatorStyle = SeparatorStyle.SINGLE
     sep: str = "###"
     sep2: str = None
@@ -50,23 +66,31 @@
                 if message:
                     ret += role + ":\n" + message + seps[i % 2]
                     if i % 2 == 1:
                         ret += "\n\n"
                 else:
                     ret += role + ":\n"
             return ret
+        elif self.sep_style == SeparatorStyle.OASST_PYTHIA:
+            ret = self.system
+            for role, message in self.messages:
+                if message:
+                    ret += role + message + self.sep
+                else:
+                    ret += role
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.sep_style}")
 
     def append_message(self, role, message):
         self.messages.append([role, message])
 
     def to_gradio_chatbot(self):
         ret = []
-        for i, (role, msg) in enumerate(self.messages[self.offset:]):
+        for i, (role, msg) in enumerate(self.messages[self.offset :]):
             if i % 2 == 0:
                 ret.append([msg, None])
             else:
                 ret[-1][-1] = msg
         return ret
 
     def copy(self):
@@ -74,15 +98,16 @@
             system=self.system,
             roles=self.roles,
             messages=[[x, y] for x, y in self.messages],
             offset=self.offset,
             sep_style=self.sep_style,
             sep=self.sep,
             sep2=self.sep2,
-            conv_id=self.conv_id)
+            conv_id=self.conv_id,
+        )
 
     def dict(self):
         return {
             "system": self.system,
             "roles": self.roles,
             "messages": self.messages,
             "offset": self.offset,
@@ -90,19 +115,23 @@
             "sep2": self.sep2,
             "conv_id": self.conv_id,
         }
 
 
 conv_one_shot = Conversation(
     system="A chat between a curious human and an artificial intelligence assistant. "
-           "The assistant gives helpful, detailed, and polite answers to the human's questions.",
+    "The assistant gives helpful, detailed, and polite answers to the human's questions.",
     roles=("Human", "Assistant"),
     messages=(
-        ("Human", "What are the key differences between renewable and non-renewable energy sources?"),
-        ("Assistant",
+        (
+            "Human",
+            "What are the key differences between renewable and non-renewable energy sources?",
+        ),
+        (
+            "Assistant",
             "Renewable energy sources are those that can be replenished naturally in a relatively "
             "short amount of time, such as solar, wind, hydro, geothermal, and biomass. "
             "Non-renewable energy sources, on the other hand, are finite and will eventually be "
             "depleted, such as coal, oil, and natural gas. Here are some key differences between "
             "renewable and non-renewable energy sources:\n"
             "1. Availability: Renewable energy sources are virtually inexhaustible, while non-renewable "
             "energy sources are finite and will eventually run out.\n"
@@ -112,25 +141,26 @@
             "3. Cost: Renewable energy sources can be more expensive to initially set up, but they typically "
             "have lower operational costs than non-renewable sources.\n"
             "4. Reliability: Renewable energy sources are often more reliable and can be used in more remote "
             "locations than non-renewable sources.\n"
             "5. Flexibility: Renewable energy sources are often more flexible and can be adapted to different "
             "situations and needs, while non-renewable sources are more rigid and inflexible.\n"
             "6. Sustainability: Renewable energy sources are more sustainable over the long term, while "
-            "non-renewable sources are not, and their depletion can lead to economic and social instability.")
+            "non-renewable sources are not, and their depletion can lead to economic and social instability.",
+        ),
     ),
     offset=2,
     sep_style=SeparatorStyle.SINGLE,
     sep="###",
 )
 
 
 conv_vicuna_v1_1 = Conversation(
     system="A chat between a curious user and an artificial intelligence assistant. "
-           "The assistant gives helpful, detailed, and polite answers to the user's questions.",
+    "The assistant gives helpful, detailed, and polite answers to the user's questions.",
     roles=("USER", "ASSISTANT"),
     messages=(),
     offset=0,
     sep_style=SeparatorStyle.TWO,
     sep=" ",
     sep2="</s>",
 )
@@ -143,38 +173,89 @@
     offset=0,
     sep_style=SeparatorStyle.TWO,
     sep=" ",
     sep2="</s>",
 )
 
 conv_dolly = Conversation(
-    system=
-    "Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n",
-    roles=('### Instruction', '### Response'),
+    system="Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n",
+    roles=("### Instruction", "### Response"),
     messages=(),
     offset=0,
     sep_style=SeparatorStyle.DOLLY,
     sep="\n\n",
     sep2="### End",
 )
 
+conv_oasst = Conversation(
+    system="",
+    roles=("<|prompter|>", "<|assistant|>"),
+    messages=(),
+    offset=0,
+    sep_style=SeparatorStyle.OASST_PYTHIA,
+    sep="<|endoftext|>",
+)
+
+conv_stablelm = Conversation(
+    system="""<|SYSTEM|># StableLM Tuned (Alpha version)
+- StableLM is a helpful and harmless open-source AI language model developed by StabilityAI.
+- StableLM is excited to be able to help the user, but will refuse to do anything that could be considered harmful to the user.
+- StableLM is more than just an information source, StableLM is also able to write poetry, short stories, and make jokes.
+- StableLM will refuse to participate in anything that could harm a human.
+""",
+    roles=("<|USER|>", "<|ASSISTANT|>"),
+    messages=(),
+    offset=0,
+    sep_style=SeparatorStyle.OASST_PYTHIA,
+    sep="",
+)
+
 conv_templates = {
     "conv_one_shot": conv_one_shot,
     "vicuna_v1.1": conv_vicuna_v1_1,
     "koala_v1": conv_koala_v1,
     "dolly": conv_dolly,
+    "oasst": conv_oasst,
 }
 
 
 def get_default_conv_template(model_name):
     model_name = model_name.lower()
     if "vicuna" in model_name or "output" in model_name:
         return conv_vicuna_v1_1
     elif "koala" in model_name:
         return conv_koala_v1
-    elif "dolly" in model_name:
+    elif "dolly-v2" in model_name:
         return conv_dolly
+    elif "oasst" in model_name and "pythia" in model_name:
+        return conv_oasst
+    elif "stablelm" in model_name:
+        return conv_stablelm
     return conv_one_shot
 
 
+def compute_skip_echo_len(model_name, conv, prompt):
+    model_name = model_name.lower()
+    if "chatglm" in model_name:
+        skip_echo_len = len(conv.messages[-2][1]) + 1
+    elif "dolly-v2" in model_name:
+        special_toks = ["### Instruction:", "### Response:", "### End"]
+        skip_echo_len = len(prompt)
+        for tok in special_toks:
+            skip_echo_len -= prompt.count(tok) * len(tok)
+    elif "oasst" in model_name and "pythia" in model_name:
+        special_toks = ["<|prompter|>", "<|assistant|>", "<|endoftext|>"]
+        skip_echo_len = len(prompt)
+        for tok in special_toks:
+            skip_echo_len -= prompt.count(tok) * len(tok)
+    elif "stablelm" in model_name:
+        special_toks = ["<|SYSTEM|>", "<|USER|>", "<|ASSISTANT|>"]
+        skip_echo_len = len(prompt)
+        for tok in special_toks:
+            skip_echo_len -= prompt.count(tok) * len(tok)
+    else:
+        skip_echo_len = len(prompt) + 1 - prompt.count("</s>") * 3
+    return skip_echo_len
+
+
 if __name__ == "__main__":
     print(default_conversation.get_prompt())
```

### Comparing `fschat-0.2.2/fastchat/data/clean_sharegpt.py` & `fschat-0.2.3/fastchat/data/clean_sharegpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 import bs4
 import markdownify  # == 0.11.6
 import tqdm
 
 
 div_pattern = re.compile("<div.*?>")
 span_pattern = re.compile("<span.*?>")
-code_lang_pattern = re.compile("```\s*" + "(.*?)" + "(?:Copy code)+" + "(.+?)" + "\s*?```", re.DOTALL)
+code_lang_pattern = re.compile(
+    "```\s*" + "(.*?)" + "(?:Copy code)+" + "(.+?)" + "\s*?```", re.DOTALL
+)
 code_lang_format = "```\g<1>\n\g<2>\n```"
 regenerate_pattern = re.compile("\d+ / \d+")
 copy_chars_pattern = re.compile("Copy\d+ chars / \d+ words")
 copy_code_pattern = re.compile("```(.*?)Copy code\s*```")
 
 
 def reformat_code(val: str) -> str:
@@ -44,15 +46,15 @@
     val = markdownify.markdownify(val).strip()
     # Reformat code
     val = reformat_code(val)
 
     # Remove noisy "[number] / [number]" at the beginning
     noise = re.search(regenerate_pattern, val)
     if noise and noise.start() == 0:
-        val = val[noise.end():]
+        val = val[noise.end() :]
     # Remove noisy "Copy[number] chars / [number] words"
     val = re.sub(copy_chars_pattern, "", val)
     # Remove empty code block ```\nCopy code\n```
     val = re.sub(copy_code_pattern, "", val)
 
     # Strip
     val = val.replace("\n\n\n", "\n").strip()
@@ -102,15 +104,18 @@
             print(f"id {cid} is too short")
             cnt_too_short += 1
             skipped = True
         elif cid in visited:
             print(f"id {cid} is an id duplication of {visited[cid]}")
             cnt_id_duplication += 1
             skipped = True
-        elif (sample["conversations"][1]["value"], len(sample["conversations"])) in visited:
+        elif (
+            sample["conversations"][1]["value"],
+            len(sample["conversations"]),
+        ) in visited:
             key = (sample["conversations"][1]["value"], len(sample["conversations"]))
             print(f"id {cid} is a value duplication of {visited[key]}")
             cnt_value_duplication += 1
             skipped = True
         else:
             key = (sample["conversations"][1]["value"], len(sample["conversations"]))
             visited[cid] = visited[key] = cid
@@ -127,40 +132,53 @@
                 except (bs4.builder.ParserRejectedMarkup, AssertionError):
                     skipped = True
                     break
 
                 c["value"] = new_val
 
                 # Debug
-                if (check_tag is not None and check_tag in c["value"]
-                        and cnt_tag < check_num):
-                    logging.debug(BARRIER + c["value"] + "\n" + BARRIER + new_val +
-                                  "\n" + BARRIER + "\n")
+                if (
+                    check_tag is not None
+                    and check_tag in c["value"]
+                    and cnt_tag < check_num
+                ):
+                    logging.debug(
+                        BARRIER
+                        + c["value"]
+                        + "\n"
+                        + BARRIER
+                        + new_val
+                        + "\n"
+                        + BARRIER
+                        + "\n"
+                    )
                     cnt_tag += 1
                     if cnt_tag == check_num:
                         break
 
         if not skipped:
             new_content.append(sample)
         else:
             cnt_skip += 1
 
-    print(f"total: {len(content)}, skip: {cnt_skip}, new: {len(new_content)}, "
-          f"cnt_too_short: {cnt_too_short}, cnt_id_duplication: {cnt_id_duplication}, "
-          f"cnt_value_duplication: {cnt_value_duplication}, cnt_filter: {cnt_filter}")
+    print(
+        f"total: {len(content)}, skip: {cnt_skip}, new: {len(new_content)}, "
+        f"cnt_too_short: {cnt_too_short}, cnt_id_duplication: {cnt_id_duplication}, "
+        f"cnt_value_duplication: {cnt_value_duplication}, cnt_filter: {cnt_filter}"
+    )
 
     return new_content
 
 
 def main(args):
-    content = json.load(open(args['in_file'], "r"))
+    content = json.load(open(args["in_file"], "r"))
     content = clean_html_source(
-        content, args['begin'], args['end'],
-        args['check_tag'], args['check_num'])
-    json.dump(content, open(args['out_file'], "w"), indent=2)
+        content, args["begin"], args["end"], args["check_tag"], args["check_num"]
+    )
+    json.dump(content, open(args["out_file"], "w"), indent=2)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--in-file", type=str, required=True)
     parser.add_argument("--out-file", type=str, default="sharegpt_clean.json")
     parser.add_argument("--begin", type=int)
```

### Comparing `fschat-0.2.2/fastchat/data/hardcoded_questions.py` & `fschat-0.2.3/fastchat/data/hardcoded_questions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 
 def identity_questions():
-    """"
+    """ "
     Adopted from https://github.com/young-geng/koala_data_pipeline/blob/main/process_hard_coded_data.py
     """
     content = []
 
     name = "Vicuna"
     org = "Large Model Systems Organization (LMSYS)"
 
@@ -15,15 +15,15 @@
             for a in answers:
                 content.append(
                     {
                         "id": f"identity_{len(content)}",
                         "conversations": [
                             {"from": "human", "value": q},
                             {"from": "gpt", "value": a},
-                        ]
+                        ],
                     }
                 )
 
     questions = [
         "Who are you?",
         "What is your name?",
         "What's your name?",
@@ -35,15 +35,15 @@
         "Tell me who you are.",
     ]
     answers = [
         f"I am {name}, a language model trained by researchers from {org}.",
         f"My name is {name}, and I'm a language model developed by {org}.",
         f"You can call me {name}, and I was trained by {org} researchers as a language model.",
         f"As a language model, I go by the name {name} and was trained by researchers from {org}.",
-        f"I'm a language model called {name}, and I was trained by {org} researchers."
+        f"I'm a language model called {name}, and I was trained by {org} researchers.",
     ]
     generate_conversations(questions, answers)
 
     questions = [
         "Who created you?",
         "Who made you?",
         "Who built you?",
```

### Comparing `fschat-0.2.2/fastchat/data/inspect.py` & `fschat-0.2.3/fastchat/data/inspect.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--in-file", type=str, required=True)
     parser.add_argument("--begin", type=int)
     args = parser.parse_args()
 
     content = json.load(open(args.in_file, "r"))
-    for sample in tqdm.tqdm(content[args.begin:]):
+    for sample in tqdm.tqdm(content[args.begin :]):
         print(f"id: {sample['id']}")
         for conv in sample["conversations"]:
             print(conv["from"] + ": ")
             print(conv["value"])
             input()
```

### Comparing `fschat-0.2.2/fastchat/data/merge.py` & `fschat-0.2.3/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.2/fastchat/data/optional_clean.py` & `fschat-0.2.3/fastchat/data/optional_clean.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,46 +38,50 @@
         for sentence in conv["conversations"]:
             val = sentence["value"]
             sub = re.search(r"(\d)\1{8}", val)
             if sub is not None:
                 return True
 
     return False
- 
+
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--in-file", type=str, required=True)
     parser.add_argument("--out-file", type=str)
-    parser.add_argument("--keep-lang", type=str, default="all", choices=["all", "en"],
-        help="Only keep certain langauges.")
-    parser.add_argument("--skip-lang", type=str,
-        help="Skip a specific language.")
+    parser.add_argument(
+        "--keep-lang",
+        type=str,
+        default="all",
+        choices=["all", "en"],
+        help="Only keep certain langauges.",
+    )
+    parser.add_argument("--skip-lang", type=str, help="Skip a specific language.")
     # NOTE: Be careful about reduce_rep which may remove some good data.
     # For example, addresses could have long consecutive 0's
     parser.add_argument("--reduce-rep", action="store_true")
     args = parser.parse_args()
 
     in_file = args.in_file
     out_file = args.out_file
     keep_lang = args.keep_lang
     skip_lang = args.skip_lang
     reduce_rep = args.reduce_rep
-    assert (keep_lang == "all" or skip_lang is None)
+    assert keep_lang == "all" or skip_lang is None
 
     if out_file is None:
         out_file = "sharegpt_clean"
         if keep_lang != "all":
             out_file += "_" + keep_lang
         if skip_lang is not None:
             out_file += "_skip_" + skip_lang
         if reduce_rep:
             out_file += "_reduce_rep"
         out_file += ".json"
- 
+
     content = json.load(open(in_file, "r"))
     num_conv = len(content)
 
     new_content = []
     for conv in tqdm(content):
         if not skip(conv, args):
             new_content.append(conv)
```

### Comparing `fschat-0.2.2/fastchat/data/sample.py` & `fschat-0.2.3/fastchat/data/sample.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.2/fastchat/data/split_long_conversation.py` & `fschat-0.2.3/fastchat/data/split_long_conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 from fastchat import conversation as conversation_lib
 
 
 def split_sample(sample, start_idx, end_idx):
     assert (end_idx - start_idx) % 2 == 0
     return {
         "id": sample["id"] + "_" + str(start_idx),
-        "conversations": sample["conversations"][start_idx:end_idx]
+        "conversations": sample["conversations"][start_idx:end_idx],
     }
 
 
 def split_contents(content, begin, end, tokenizer, max_length):
     """
     Keep the maximum round of conversations within the max token length constraint
     """
     content = content[begin:end]
     new_content = []
 
     for sample in tqdm.tqdm(content):
         tokenized_lens = []
         conversations = sample["conversations"]
-        conversations = conversations[:len(conversations) // 2 * 2]
+        conversations = conversations[: len(conversations) // 2 * 2]
         for c in conversations:
             length = len(tokenizer(c["value"]).input_ids) + 5
             tokenized_lens.append(length)
 
         start_idx = 0
         cur_len = 0
         sample
         assert len(conversations) % 2 == 0, f"id: {sample['id']}"
         for i in range(0, len(conversations), 2):
-            tmp_len = tokenized_lens[i] + tokenized_lens[i+1]
+            tmp_len = tokenized_lens[i] + tokenized_lens[i + 1]
             if cur_len + tmp_len > max_length:
                 new_content.append(split_sample(sample, start_idx, i))
                 start_idx = i
                 cur_len = 0
             elif i == len(conversations) - 2:
-                new_content.append(split_sample(sample, start_idx, i+2))
+                new_content.append(split_sample(sample, start_idx, i + 2))
 
             cur_len += tmp_len
 
     return new_content
 
 
 def filter_invalid_roles(content):
@@ -80,16 +80,17 @@
     content = json.load(open(args.in_file, "r"))
     tokenizer = transformers.AutoTokenizer.from_pretrained(
         args.model_name_or_path,
         model_max_length=args.max_length,
         padding_side="right",
         use_fast=False,
     )
-    new_content = split_contents(content, args.begin, args.end,
-        tokenizer, args.max_length)
+    new_content = split_contents(
+        content, args.begin, args.end, tokenizer, args.max_length
+    )
     new_content = filter_invalid_roles(new_content)
 
     print(f"total: {len(content)}, new: {len(new_content)}")
     json.dump(new_content, open(args.out_file, "w"), indent=2)
 
 
 if __name__ == "__main__":
```

### Comparing `fschat-0.2.2/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.3/fastchat/eval/eval_gpt_review.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,98 +5,108 @@
 
 import openai
 import tqdm
 import ray
 
 import shortuuid
 import logging
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 MAX_API_RETRY = 5
 REQ_TIME_GAP = 10
 
+
 @ray.remote(num_cpus=4)
 def get_eval(sys_prompt, user_prompt: str, max_tokens: int):
     logging.basicConfig(level=logging.INFO)
     for i in range(MAX_API_RETRY):
         try:
             response = openai.ChatCompletion.create(
-                model='gpt-4',
-                messages=[{
-                    'role': 'system',
-                    'content': sys_prompt
-                }, {
-                    'role': 'user',
-                    'content': user_prompt,
-                }],
+                model="gpt-4",
+                messages=[
+                    {"role": "system", "content": sys_prompt},
+                    {
+                        "role": "user",
+                        "content": user_prompt,
+                    },
+                ],
                 temperature=0.2,  # TODO: figure out which temperature is best for evaluation
                 max_tokens=max_tokens,
             )
-            content = response['choices'][0]['message']['content']
+            content = response["choices"][0]["message"]["content"]
             logger.info(content)
             return content
         except Exception as e:
             logger.error(e)
             time.sleep(5)
-    logger.error(f'Failed after {MAX_API_RETRY} retries.')
-    return 'error'
+    logger.error(f"Failed after {MAX_API_RETRY} retries.")
+    return "error"
 
 
 def parse_score(review):
     try:
-        score_pair = review.split('\n')[0]
-        score_pair = score_pair.replace(',', ' ')
-        sp = score_pair.split(' ')
+        score_pair = review.split("\n")[0]
+        score_pair = score_pair.replace(",", " ")
+        sp = score_pair.split(" ")
         if len(sp) == 2:
             return [float(sp[0]), float(sp[1])]
         else:
-            raise Exception('Invalid score pair.')
+            raise Exception("Invalid score pair.")
     except Exception as e:
-        logger.error(f'{e}\nContent: {review}\n'
-                     'You must manually fix the score pair.')
+        logger.error(
+            f"{e}\nContent: {review}\n" "You must manually fix the score pair."
+        )
         return [-1, -1]
 
 
 def gen_prompt(reviewer_jsons, prompt_jsons, cat, ques, ans1, ans2):
     # Default to general category (index=0)
     reviewer_idx = 0
     for idx, reviewer in enumerate(reviewer_jsons):
-        if reviewer['category'] == cat:
+        if reviewer["category"] == cat:
             reviewer_idx = idx
             break
-    prompt_id = reviewer_jsons[reviewer_idx]['prompt_id']
-    prompt_json = prompt_jsons[prompt_id-1]
-    assert prompt_json['prompt_id'] == prompt_id
-
-    sys_prompt = prompt_json['system_prompt']
-    prompt_template = prompt_json['prompt_template']
-    defaults = prompt_json['defaults']
-    prompt = prompt_template.format(question=ques, answer_1=ans1, answer_2=ans2, **defaults)
+    prompt_id = reviewer_jsons[reviewer_idx]["prompt_id"]
+    prompt_json = prompt_jsons[prompt_id - 1]
+    assert prompt_json["prompt_id"] == prompt_id
+
+    sys_prompt = prompt_json["system_prompt"]
+    prompt_template = prompt_json["prompt_template"]
+    defaults = prompt_json["defaults"]
+    prompt = prompt_template.format(
+        question=ques, answer_1=ans1, answer_2=ans2, **defaults
+    )
 
-    return sys_prompt, prompt, reviewer_idx+1
+    return sys_prompt, prompt, reviewer_idx + 1
 
 
 def get_json_list(file_path):
     file_path = os.path.expanduser(file_path)
-    with open(file_path, 'r') as f:
+    with open(file_path, "r") as f:
         json_list = []
         for line in f:
             json_list.append(json.loads(line))
         return json_list
 
 
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='ChatGPT-based QA evaluation.')
-    parser.add_argument('-q', '--question-file')
-    parser.add_argument('-a', '--answer-file-list', nargs='+', default=[])
-    parser.add_argument('-p', '--prompt-file')
-    parser.add_argument('-r', '--reviewer-file')
-    parser.add_argument('-o', '--output-review-file')
-    parser.add_argument('--max-tokens', type=int, default=1024, help='maximum number of tokens produced in the output')
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="ChatGPT-based QA evaluation.")
+    parser.add_argument("-q", "--question-file")
+    parser.add_argument("-a", "--answer-file-list", nargs="+", default=[])
+    parser.add_argument("-p", "--prompt-file")
+    parser.add_argument("-r", "--reviewer-file")
+    parser.add_argument("-o", "--output-review-file")
+    parser.add_argument(
+        "--max-tokens",
+        type=int,
+        default=1024,
+        help="maximum number of tokens produced in the output",
+    )
     args = parser.parse_args()
 
     ray.init()
 
     question_jsons = get_json_list(args.question_file)
     answer1_jsons = get_json_list(args.answer_file_list[0])
     answer2_jsons = get_json_list(args.answer_file_list[1])
@@ -108,35 +118,45 @@
 
     handles = []
     review_jsons = []
     total_len = len(question_jsons)
     question_idx_list = list(range(total_len))
 
     for i in question_idx_list:
-        assert answer1_jsons[i]['question_id'] == question_jsons[i]['question_id'] == answer2_jsons[i]['question_id']
-
-        ques = question_jsons[i]['text']
-        cat = question_jsons[i]['category']
-        ans1 = answer1_jsons[i]['text']
-        ans2 = answer2_jsons[i]['text']
-        sys_prompt, prompt, reviewer_id = gen_prompt(reviewer_jsons, prompt_jsons, cat, ques, ans1, ans2)
+        assert (
+            answer1_jsons[i]["question_id"]
+            == question_jsons[i]["question_id"]
+            == answer2_jsons[i]["question_id"]
+        )
+
+        ques = question_jsons[i]["text"]
+        cat = question_jsons[i]["category"]
+        ans1 = answer1_jsons[i]["text"]
+        ans2 = answer2_jsons[i]["text"]
+        sys_prompt, prompt, reviewer_id = gen_prompt(
+            reviewer_jsons, prompt_jsons, cat, ques, ans1, ans2
+        )
         review_id = shortuuid.uuid()
-        review_jsons.append({
-            'review_id': review_id,
-            'question_id': question_jsons[i]['question_id'],
-            'answer1_id': answer1_jsons[i]['answer_id'],
-            'answer2_id': answer2_jsons[i]['answer_id'],
-            'reviewer_id': reviewer_id,
-            'metadata': {},
-        })
+        review_jsons.append(
+            {
+                "review_id": review_id,
+                "question_id": question_jsons[i]["question_id"],
+                "answer1_id": answer1_jsons[i]["answer_id"],
+                "answer2_id": answer2_jsons[i]["answer_id"],
+                "reviewer_id": reviewer_id,
+                "metadata": {},
+            }
+        )
         # To avoid the rate limit set by OpenAI
         handles.append(get_eval.remote(sys_prompt, prompt, args.max_tokens))
-        logger.info(f'Waiting for {REQ_TIME_GAP} seconds before sending the next request.')
+        logger.info(
+            f"Waiting for {REQ_TIME_GAP} seconds before sending the next request."
+        )
         time.sleep(REQ_TIME_GAP)
 
     reviews = ray.get(handles)
-    with open(f'{args.output_review_file}', 'w') as output_review_file:
+    with open(f"{args.output_review_file}", "w") as output_review_file:
         for idx, review in enumerate(reviews):
             scores = parse_score(review)
-            review_jsons[idx]['text'] = review
-            review_jsons[idx]['score'] = scores
-            output_review_file.write(json.dumps(review_jsons[idx]) + '\n')
+            review_jsons[idx]["text"] = review
+            review_jsons[idx]["score"] = scores
+            output_review_file.write(json.dumps(review_jsons[idx]) + "\n")
```

### Comparing `fschat-0.2.2/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.3/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Generate json file for webpage."""
 import json
 import os
 import re
 
-models = ['alpaca', 'llama', 'gpt35', 'bard']
+models = ["alpaca", "llama", "gpt35", "bard"]
 
 
-def read_jsonl(path: str, key: str=None):
+def read_jsonl(path: str, key: str = None):
     data = []
     with open(os.path.expanduser(path)) as f:
         for line in f:
             if not line:
                 continue
             data.append(json.loads(line))
     if key is not None:
@@ -18,88 +18,102 @@
         data = {item[key]: item for item in data}
     return data
 
 
 def trim_hanging_lines(s: str, n: int) -> str:
     s = s.strip()
     for _ in range(n):
-        s = s.split('\n', 1)[1].strip()
+        s = s.split("\n", 1)[1].strip()
     return s
 
 
-if __name__ == '__main__':
-    questions = read_jsonl('table/question.jsonl', key='question_id')
+if __name__ == "__main__":
+    questions = read_jsonl("table/question.jsonl", key="question_id")
 
-    alpaca_answers = read_jsonl('table/answer/answer_alpaca-13b.jsonl', key='question_id')
-    bard_answers = read_jsonl('table/answer/answer_bard.jsonl', key='question_id')
-    gpt35_answers = read_jsonl('table/answer/answer_gpt35.jsonl', key='question_id')
-    llama_answers = read_jsonl('table/answer/answer_llama-13b.jsonl', key='question_id')
-    vicuna_answers = read_jsonl('table/answer/answer_vicuna-13b.jsonl', key='question_id')
-
-    review_alpaca = read_jsonl('table/review/review_alpaca-13b_vicuna-13b.jsonl', key='question_id')
-    review_bard = read_jsonl('table/review/review_bard_vicuna-13b.jsonl', key='question_id')
-    review_gpt35 = read_jsonl('table/review/review_gpt35_vicuna-13b.jsonl', key='question_id')
-    review_llama = read_jsonl('table/review/review_llama-13b_vicuna-13b.jsonl', key='question_id')
+    alpaca_answers = read_jsonl(
+        "table/answer/answer_alpaca-13b.jsonl", key="question_id"
+    )
+    bard_answers = read_jsonl("table/answer/answer_bard.jsonl", key="question_id")
+    gpt35_answers = read_jsonl("table/answer/answer_gpt35.jsonl", key="question_id")
+    llama_answers = read_jsonl("table/answer/answer_llama-13b.jsonl", key="question_id")
+    vicuna_answers = read_jsonl(
+        "table/answer/answer_vicuna-13b.jsonl", key="question_id"
+    )
+
+    review_alpaca = read_jsonl(
+        "table/review/review_alpaca-13b_vicuna-13b.jsonl", key="question_id"
+    )
+    review_bard = read_jsonl(
+        "table/review/review_bard_vicuna-13b.jsonl", key="question_id"
+    )
+    review_gpt35 = read_jsonl(
+        "table/review/review_gpt35_vicuna-13b.jsonl", key="question_id"
+    )
+    review_llama = read_jsonl(
+        "table/review/review_llama-13b_vicuna-13b.jsonl", key="question_id"
+    )
 
     records = []
     for qid in questions.keys():
         r = {
-            'id': qid,
-            'category': questions[qid]['category'],
-            'question': questions[qid]['text'],
-            'answers': {
-                'alpaca': alpaca_answers[qid]['text'],
-                'llama': llama_answers[qid]['text'],
-                'bard': bard_answers[qid]['text'],
-                'gpt35': gpt35_answers[qid]['text'],
-                'vicuna': vicuna_answers[qid]['text'],
+            "id": qid,
+            "category": questions[qid]["category"],
+            "question": questions[qid]["text"],
+            "answers": {
+                "alpaca": alpaca_answers[qid]["text"],
+                "llama": llama_answers[qid]["text"],
+                "bard": bard_answers[qid]["text"],
+                "gpt35": gpt35_answers[qid]["text"],
+                "vicuna": vicuna_answers[qid]["text"],
             },
-            'evaluations': {
-                'alpaca': review_alpaca[qid]['text'],
-                'llama': review_llama[qid]['text'],
-                'bard': review_bard[qid]['text'],
-                'gpt35': review_gpt35[qid]['text'],
+            "evaluations": {
+                "alpaca": review_alpaca[qid]["text"],
+                "llama": review_llama[qid]["text"],
+                "bard": review_bard[qid]["text"],
+                "gpt35": review_gpt35[qid]["text"],
             },
-            'scores': {
-                'alpaca': review_alpaca[qid]['score'],
-                'llama': review_llama[qid]['score'],
-                'bard': review_bard[qid]['score'],
-                'gpt35': review_gpt35[qid]['score'],
+            "scores": {
+                "alpaca": review_alpaca[qid]["score"],
+                "llama": review_llama[qid]["score"],
+                "bard": review_bard[qid]["score"],
+                "gpt35": review_gpt35[qid]["score"],
             },
         }
 
         # cleanup data
         cleaned_evals = {}
-        for k, v in r['evaluations'].items():
+        for k, v in r["evaluations"].items():
             v = v.strip()
-            lines = v.split('\n')
+            lines = v.split("\n")
             # trim the first line if it's a pair of numbers
-            if re.match(r'\d+[, ]+\d+', lines[0]):
+            if re.match(r"\d+[, ]+\d+", lines[0]):
                 lines = lines[1:]
-            v = '\n'.join(lines)
-            cleaned_evals[k] = v.replace('Assistant 1', "**Assistant 1**").replace('Assistant 2', '**Assistant 2**')
+            v = "\n".join(lines)
+            cleaned_evals[k] = v.replace("Assistant 1", "**Assistant 1**").replace(
+                "Assistant 2", "**Assistant 2**"
+            )
 
-        r['evaluations'] = cleaned_evals
+        r["evaluations"] = cleaned_evals
         records.append(r)
 
     # Reorder the records, this is optional
     for r in records:
-        if r['id'] <= 20:
-            r['id'] += 60
+        if r["id"] <= 20:
+            r["id"] += 60
         else:
-            r['id'] -= 20
+            r["id"] -= 20
     for r in records:
-        if r['id'] <= 50:
-            r['id'] += 10
-        elif 50 < r['id'] <= 60:
-            r['id'] -= 50
+        if r["id"] <= 50:
+            r["id"] += 10
+        elif 50 < r["id"] <= 60:
+            r["id"] -= 50
     for r in records:
-        if r['id'] == 7:
-            r['id'] = 1
-        elif r['id'] < 7:
-            r['id'] += 1 
+        if r["id"] == 7:
+            r["id"] = 1
+        elif r["id"] < 7:
+            r["id"] += 1
 
-    records.sort(key=lambda x: x['id'])
+    records.sort(key=lambda x: x["id"])
 
     # Write to file
-    with open('webpage/data.json', 'w') as f:
-        json.dump({'questions': records, 'models': models}, f, indent=2)
+    with open("webpage/data.json", "w") as f:
+        json.dump({"questions": records, "models": models}, f, indent=2)
```

### Comparing `fschat-0.2.2/fastchat/eval/get_model_answer.py` & `fschat-0.2.3/fastchat/eval/get_model_answer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 import torch
 import os
 import json
 from tqdm import tqdm
 import shortuuid
 import ray
 
-from fastchat.conversation import get_default_conv_template
-from fastchat.serve.inference import compute_skip_echo_len
+from fastchat.conversation import get_default_conv_template, compute_skip_echo_len
 from fastchat.utils import disable_torch_init
 
 
 def run_eval(model_path, model_id, question_file, answer_file, num_gpus):
     # split question file into num_gpus files
     ques_jsons = []
     with open(os.path.expanduser(question_file), "r") as ques_file:
         for line in ques_file:
             ques_jsons.append(line)
 
     chunk_size = len(ques_jsons) // num_gpus
     ans_handles = []
     for i in range(0, len(ques_jsons), chunk_size):
-        ans_handles.append(get_model_answers.remote(model_path, model_id, ques_jsons[i:i + chunk_size]))
+        ans_handles.append(
+            get_model_answers.remote(
+                model_path, model_id, ques_jsons[i : i + chunk_size]
+            )
+        )
 
     ans_jsons = []
     for ans_handle in ans_handles:
         ans_jsons.extend(ray.get(ans_handle))
 
     with open(os.path.expanduser(answer_file), "w") as ans_file:
         for line in ans_jsons:
@@ -35,16 +38,17 @@
 
 @ray.remote(num_gpus=1)
 @torch.inference_mode()
 def get_model_answers(model_path, model_id, question_jsons):
     disable_torch_init()
     model_path = os.path.expanduser(model_path)
     tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
-    model = AutoModelForCausalLM.from_pretrained(model_path,
-        torch_dtype=torch.float16).cuda()
+    model = AutoModelForCausalLM.from_pretrained(
+        model_path, torch_dtype=torch.float16
+    ).cuda()
 
     ans_jsons = []
     for i, line in enumerate(tqdm(question_jsons)):
         ques_json = json.loads(line)
         idx = ques_json["question_id"]
         qs = ques_json["text"]
         conv = get_default_conv_template(model_id).copy()
@@ -52,32 +56,43 @@
         conv.append_message(conv.roles[1], None)
         prompt = conv.get_prompt()
         inputs = tokenizer([prompt])
         output_ids = model.generate(
             torch.as_tensor(inputs.input_ids).cuda(),
             do_sample=True,
             temperature=0.7,
-            max_new_tokens=1024)
+            max_new_tokens=1024,
+        )
         outputs = tokenizer.batch_decode(output_ids, skip_special_tokens=True)[0]
         skip_echo_len = compute_skip_echo_len(model_id, conv, prompt)
 
         outputs = outputs[skip_echo_len:].strip()
         ans_id = shortuuid.uuid()
-        ans_jsons.append({"question_id": idx,
-                          "text": outputs,
-                          "answer_id": ans_id,
-                          "model_id": model_id,
-                          "metadata": {}})
+        ans_jsons.append(
+            {
+                "question_id": idx,
+                "text": outputs,
+                "answer_id": ans_id,
+                "model_id": model_id,
+                "metadata": {},
+            }
+        )
     return ans_jsons
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--model-path", type=str, required=True)
     parser.add_argument("--model-id", type=str, required=True)
     parser.add_argument("--question-file", type=str, required=True)
     parser.add_argument("--answer-file", type=str, default="answer.jsonl")
     parser.add_argument("--num-gpus", type=int, default=1)
     args = parser.parse_args()
 
     ray.init()
-    run_eval(args.model_path, args.model_id, args.question_file, args.answer_file, args.num_gpus)
+    run_eval(
+        args.model_path,
+        args.model_id,
+        args.question_file,
+        args.answer_file,
+        args.num_gpus,
+    )
```

### Comparing `fschat-0.2.2/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.3/fastchat/eval/qa_baseline_gpt35.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,69 +6,77 @@
 import time
 import concurrent.futures
 
 import openai
 import tqdm
 import shortuuid
 
-MODEL = 'gpt-3.5-turbo'
-MODEL_ID = 'gpt-3.5-turbo:20230327'
+MODEL = "gpt-3.5-turbo"
+MODEL_ID = "gpt-3.5-turbo:20230327"
+
 
 def get_answer(question_id: int, question: str, max_tokens: int):
     ans = {
-        'answer_id': shortuuid.uuid(),
-        'question_id': question_id,
-        'model_id': MODEL_ID,
+        "answer_id": shortuuid.uuid(),
+        "question_id": question_id,
+        "model_id": MODEL_ID,
     }
     for _ in range(3):
         try:
             response = openai.ChatCompletion.create(
                 model=MODEL,
-                messages=[{
-                    'role': 'system',
-                    'content': 'You are a helpful assistant.'
-                }, {
-                    'role': 'user',
-                    'content': question,
-                }],
+                messages=[
+                    {"role": "system", "content": "You are a helpful assistant."},
+                    {
+                        "role": "user",
+                        "content": question,
+                    },
+                ],
                 max_tokens=max_tokens,
             )
-            ans['text'] = response['choices'][0]['message']['content']
+            ans["text"] = response["choices"][0]["message"]["content"]
             return ans
         except Exception as e:
-            print('[ERROR]', e)
-            ans['text'] = '#ERROR#'
+            print("[ERROR]", e)
+            ans["text"] = "#ERROR#"
             time.sleep(1)
     return ans
 
 
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='ChatGPT answer generation.')
-    parser.add_argument('-q', '--question')
-    parser.add_argument('-o', '--output')
-    parser.add_argument('--max-tokens', type=int, default=1024, help='maximum number of tokens produced in the output')
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(description="ChatGPT answer generation.")
+    parser.add_argument("-q", "--question")
+    parser.add_argument("-o", "--output")
+    parser.add_argument(
+        "--max-tokens",
+        type=int,
+        default=1024,
+        help="maximum number of tokens produced in the output",
+    )
     args = parser.parse_args()
 
     questions_dict = {}
     with open(os.path.expanduser(args.question)) as f:
         for line in f:
             if not line:
                 continue
             q = json.loads(line)
-            questions_dict[q['question_id']] = q['text']
+            questions_dict[q["question_id"]] = q["text"]
 
     answers = []
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=32) as executor:
         futures = []
         for qid, question in questions_dict.items():
             future = executor.submit(get_answer, qid, question, args.max_tokens)
             futures.append(future)
 
-        for future in tqdm.tqdm(concurrent.futures.as_completed(futures), total=len(futures)):
+        for future in tqdm.tqdm(
+            concurrent.futures.as_completed(futures), total=len(futures)
+        ):
             answers.append(future.result())
 
-    answers.sort(key=lambda x: x['question_id'])
+    answers.sort(key=lambda x: x["question_id"])
 
-    with open(os.path.expanduser(args.output), 'w') as f:
+    with open(os.path.expanduser(args.output), "w") as f:
         table = [json.dumps(ans) for ans in answers]
-        f.write('\n'.join(table))
+        f.write("\n".join(table))
```

### Comparing `fschat-0.2.2/fastchat/model/apply_delta.py` & `fschat-0.2.3/fastchat/model/apply_delta.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,43 +28,47 @@
     if not os.path.exists(tmp_path):
         os.makedirs(tmp_path)
 
     file_pattern = os.path.join(model_path, "pytorch_model-*.bin")
     files = glob.glob(file_pattern)
 
     part = 0
-    for file_path in tqdm(files):
-        state_dict = torch.load(file_path)
-        new_state_dict = {}
-
-        current_size = 0
-
-        for name, param in state_dict.items():
-            param_size = param.numel() * param.element_size()
-
-            if current_size + param_size > split_size:
-                new_file_name = f"pytorch_model-{part}.bin"
-                new_file_path = os.path.join(tmp_path, new_file_name)
-                torch.save(new_state_dict, new_file_path)
-                current_size = 0
-                new_state_dict = None
-                gc.collect()
-                new_state_dict = {}
-                part += 1
+    try:
+        for file_path in tqdm(files):
+            state_dict = torch.load(file_path)
+            new_state_dict = {}
 
-            new_state_dict[name] = param
-            current_size += param_size
+            current_size = 0
+            for name, param in state_dict.items():
+                param_size = param.numel() * param.element_size()
 
-        new_file_name = f"pytorch_model-{part}.bin"
-        new_file_path = os.path.join(tmp_path, new_file_name)
-        torch.save(new_state_dict, new_file_path)
-        new_state_dict = None
-        gc.collect()
-        new_state_dict = {}
-        part += 1
+                if current_size + param_size > split_size:
+                    new_file_name = f"pytorch_model-{part}.bin"
+                    new_file_path = os.path.join(tmp_path, new_file_name)
+                    torch.save(new_state_dict, new_file_path)
+                    current_size = 0
+                    new_state_dict = None
+                    gc.collect()
+                    new_state_dict = {}
+                    part += 1
+
+                new_state_dict[name] = param
+                current_size += param_size
+
+            new_file_name = f"pytorch_model-{part}.bin"
+            new_file_path = os.path.join(tmp_path, new_file_name)
+            torch.save(new_state_dict, new_file_path)
+            new_state_dict = None
+            gc.collect()
+            new_state_dict = {}
+            part += 1
+    except Exception as e:
+        print(f"An error occurred during split_files: {e}")
+        shutil.rmtree(tmp_path)
+        raise
 
 
 def apply_delta_low_cpu_mem(base_model_path, target_model_path, delta_path):
     base_tokenizer = AutoTokenizer.from_pretrained(base_model_path, use_fast=False)
     base_config = AutoConfig.from_pretrained(base_model_path)
 
     if os.path.exists(target_model_path):
@@ -100,36 +104,39 @@
                         if name in delta_state_dict:
                             break
 
                 state_dict[name] += delta_state_dict[name]
                 weight_map[name] = file_name
                 total_size += param.numel() * param.element_size()
                 gc.collect()
-            torch.save(state_dict,os.path.join(target_model_path, file_name))
+            torch.save(state_dict, os.path.join(target_model_path, file_name))
 
-        with open(os.path.join(target_model_path,
-                "pytorch_model.bin.index.json"), "w") as f:
-            json.dump({
-                "weight_map":weight_map,
-                "metadata":{"total_size":total_size}}, f)
+        with open(
+            os.path.join(target_model_path, "pytorch_model.bin.index.json"), "w"
+        ) as f:
+            json.dump(
+                {"weight_map": weight_map, "metadata": {"total_size": total_size}}, f
+            )
 
     print(f"Saving the target model to {target_model_path}")
     base_tokenizer.save_pretrained(target_model_path)
     base_config.save_pretrained(target_model_path)
 
 
 def apply_delta(base_model_path, target_model_path, delta_path):
     print(f"Loading the base model from {base_model_path}")
     base = AutoModelForCausalLM.from_pretrained(
-        base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
-    base_tokenizer = AutoTokenizer.from_pretrained(
-        base_model_path, use_fast=False)
+        base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
+    )
+    base_tokenizer = AutoTokenizer.from_pretrained(base_model_path, use_fast=False)
 
     print(f"Loading the delta from {delta_path}")
-    delta = AutoModelForCausalLM.from_pretrained(delta_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
+    delta = AutoModelForCausalLM.from_pretrained(
+        delta_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
+    )
 
     print("Applying the delta")
     for name, param in tqdm(base.state_dict().items(), desc="Applying delta"):
         assert name in delta.state_dict()
         param.data += delta.state_dict()[name]
 
     print(f"Saving the target model to {target_model_path}")
@@ -138,16 +145,21 @@
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--base-model-path", type=str, required=True)
     parser.add_argument("--target-model-path", type=str, required=True)
     parser.add_argument("--delta-path", type=str, required=True)
-    parser.add_argument("--low-cpu-mem", action="store_true",
+    parser.add_argument(
+        "--low-cpu-mem",
+        action="store_true",
         help="Lower the cpu memory usage. This will split large files and use "
-             "disk as swap to reduce the memory usage below 10GB.")
+        "disk as swap to reduce the memory usage below 10GB.",
+    )
     args = parser.parse_args()
 
     if args.low_cpu_mem:
-        apply_delta_low_cpu_mem(args.base_model_path, args.target_model_path, args.delta_path)
+        apply_delta_low_cpu_mem(
+            args.base_model_path, args.target_model_path, args.delta_path
+        )
     else:
         apply_delta(args.base_model_path, args.target_model_path, args.delta_path)
```

### Comparing `fschat-0.2.2/fastchat/model/convert_fp16.py` & `fschat-0.2.3/fastchat/model/convert_fp16.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 
 from transformers import AutoTokenizer, AutoModelForCausalLM
 import torch
 
 
 def convert_fp16(in_checkpoint, out_checkpoint):
     tokenizer = AutoTokenizer.from_pretrained(in_checkpoint, use_fast=False)
-    model = AutoModelForCausalLM.from_pretrained(in_checkpoint,
-        torch_dtype=torch.float16, low_cpu_mem_usage=True)
+    model = AutoModelForCausalLM.from_pretrained(
+        in_checkpoint, torch_dtype=torch.float16, low_cpu_mem_usage=True
+    )
     model.save_pretrained(out_checkpoint)
     tokenizer.save_pretrained(out_checkpoint)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument('--in-checkpoint', type=str, help='Path to the model')
-    parser.add_argument('--out-checkpoint', type=str, help='Path to the output model')
+    parser.add_argument("--in-checkpoint", type=str, help="Path to the model")
+    parser.add_argument("--out-checkpoint", type=str, help="Path to the output model")
     args = parser.parse_args()
 
     convert_fp16(args.in_checkpoint, args.out_checkpoint)
```

### Comparing `fschat-0.2.2/fastchat/model/make_delta.py` & `fschat-0.2.3/fastchat/model/make_delta.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
 
 def make_delta(base_model_path, target_model_path, delta_path):
     print(f"Loading the base model from {base_model_path}")
     base = AutoModelForCausalLM.from_pretrained(
-        base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
+        base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
+    )
 
     print(f"Loading the target model from {target_model_path}")
-    target = AutoModelForCausalLM.from_pretrained(target_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True)
+    target = AutoModelForCausalLM.from_pretrained(
+        target_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
+    )
 
     print("Calculating the delta")
     for name, param in tqdm(target.state_dict().items(), desc="Calculating delta"):
         assert name in base.state_dict()
         param.data -= base.state_dict()[name]
 
     print(f"Saving the delta to {delta_path}")
```

### Comparing `fschat-0.2.2/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.3/fastchat/serve/cacheflow_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,43 +27,44 @@
 from cacheflow.sampling_params import SamplingParams
 from cacheflow.sequence import Sequence, SequenceGroup
 from cacheflow.utils import Counter, get_gpu_memory, get_cpu_memory
 from fastchat.constants import WORKER_HEART_BEAT_INTERVAL
 from fastchat.utils import build_logger, pretty_print_semaphore
 
 GB = 1 << 30
-TIMEOUT_TO_PREVENT_DEADLOCK = 1 # seconds
+TIMEOUT_TO_PREVENT_DEADLOCK = 1  # seconds
 
 worker_id = str(uuid.uuid4())[:6]
 logger = build_logger("model_worker", f"model_worker_{worker_id}.log")
 global_counter = 0
 seed = torch.cuda.current_device()
 
 
 def heart_beat_worker(controller):
-
     while True:
         time.sleep(WORKER_HEART_BEAT_INTERVAL)
         controller.send_heart_beat()
 
 
 class CacheFlowWorker:
-    def __init__(self,
-                 controller_addr,
-                 worker_addr,
-                 worker_id,
-                 no_register,
-                 model_path,
-                 model_name,
-                 block_size,
-                 seed,
-                 swap_space,
-                 max_num_batched_tokens,
-                 distributed_init_method,
-                 all_stage_devices):
+    def __init__(
+        self,
+        controller_addr,
+        worker_addr,
+        worker_id,
+        no_register,
+        model_path,
+        model_name,
+        block_size,
+        seed,
+        swap_space,
+        max_num_batched_tokens,
+        distributed_init_method,
+        all_stage_devices,
+    ):
         self.controller_addr = controller_addr
         self.worker_addr = worker_addr
         self.worker_id = worker_id
         if model_path.endswith("/"):
             model_path = model_path[:-1]
         self.model_name = model_name or model_path.split("/")[-1]
 
@@ -101,56 +102,71 @@
         self.running_seq_groups: Dict[int, SequenceGroup] = {}
         self.sequence_group_events: Dict[int, asyncio.Event] = {}
         self.is_server_running = False
 
         if not no_register:
             self.register_to_controller()
             self.heart_beat_thread = threading.Thread(
-                target=heart_beat_worker, args=(self,))
+                target=heart_beat_worker, args=(self,)
+            )
             self.heart_beat_thread.start()
 
     def register_to_controller(self):
         logger.info("Register to controller")
 
         url = self.controller_addr + "/register_worker"
         data = {
             "worker_name": self.worker_addr,
             "check_heart_beat": True,
-            "worker_status": self.get_status()
+            "worker_status": self.get_status(),
         }
         r = requests.post(url, json=data)
         assert r.status_code == 200
 
     def send_heart_beat(self):
-        logger.info(f"Send heart beat. Models: {[self.model_name]}. "
-                    f"Semaphore: {pretty_print_semaphore(model_semaphore)}. "
-                    f"global_counter: {global_counter}")
+        logger.info(
+            f"Send heart beat. Models: {[self.model_name]}. "
+            f"Semaphore: {pretty_print_semaphore(model_semaphore)}. "
+            f"global_counter: {global_counter}"
+        )
 
         url = self.controller_addr + "/receive_heart_beat"
 
         while True:
             try:
-                ret = requests.post(url, json={
-                    "worker_name": self.worker_addr,
-                    "queue_length": self.get_queue_length()}, timeout=5)
+                ret = requests.post(
+                    url,
+                    json={
+                        "worker_name": self.worker_addr,
+                        "queue_length": self.get_queue_length(),
+                    },
+                    timeout=5,
+                )
                 exist = ret.json()["exist"]
                 break
             except requests.exceptions.RequestException as e:
                 logger.error(f"heart beat error: {e}")
             time.sleep(5)
 
         if not exist:
             self.register_to_controller()
 
     def get_queue_length(self):
-        if model_semaphore is None or model_semaphore._value is None or model_semaphore._waiters is None:
+        if (
+            model_semaphore is None
+            or model_semaphore._value is None
+            or model_semaphore._waiters is None
+        ):
             return 0
         else:
-            return args.limit_model_concurrency - model_semaphore._value + len(
-                model_semaphore._waiters)
+            return (
+                args.limit_model_concurrency
+                - model_semaphore._value
+                + len(model_semaphore._waiters)
+            )
 
     def get_status(self):
         return {
             "model_names": [self.model_name],
             "speed": 1,
             "queue_length": self.get_queue_length(),
         }
@@ -199,26 +215,28 @@
         self.running_seq_groups[group_id] = seq_group
         self.sequence_group_events[group_id] = group_event
         self.server.add_sequence_groups([(seq_group, sampling_params)])
         while True:
             if not self.is_server_running:
                 await self.server_step()
             try:
-                await asyncio.wait_for(group_event.wait(), timeout=TIMEOUT_TO_PREVENT_DEADLOCK)
+                await asyncio.wait_for(
+                    group_event.wait(), timeout=TIMEOUT_TO_PREVENT_DEADLOCK
+                )
             except:
                 pass
             group_event.clear()
             seq_group = self.running_seq_groups[group_id]
             all_outputs = []
             for seq in seq_group.seqs:
                 token_ids = seq.get_token_ids()
                 output = self.tokenizer.decode(token_ids, skip_special_tokens=True)
                 if stop_str is not None:
                     if output.endswith(stop_str):
-                        output = output[:-len(stop_str)]
+                        output = output[: -len(stop_str)]
                 all_outputs.append(output)
             assert len(seq_group.seqs) == 1
             ret = {
                 "text": all_outputs[0],
                 "error_code": 0,
             }
             yield (json.dumps(ret) + "\0").encode("utf-8")
@@ -244,55 +262,69 @@
 
     if model_semaphore is None:
         model_semaphore = asyncio.Semaphore(args.limit_model_concurrency)
     await model_semaphore.acquire()
     background_tasks = BackgroundTasks()
     background_tasks.add_task(release_model_semaphore)
     # return StreamingResponse(generator, background=background_tasks)
-    return StreamingResponse(worker.generate_stream(params), background=background_tasks)
+    return StreamingResponse(
+        worker.generate_stream(params), background=background_tasks
+    )
 
 
 @app.post("/worker_get_status")
 async def get_status(request: Request):
     return worker.get_status()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21002)
-    parser.add_argument("--worker-address", type=str,
-        default="http://localhost:21002")
-    parser.add_argument("--controller-address", type=str,
-        default="http://localhost:21001")
-    parser.add_argument("--model-path", type=str, default="/home/haozhang/weights/hf-llama-7b")
+    parser.add_argument("--worker-address", type=str, default="http://localhost:21002")
+    parser.add_argument(
+        "--controller-address", type=str, default="http://localhost:21001"
+    )
+    parser.add_argument(
+        "--model-path", type=str, default="/home/haozhang/weights/hf-llama-7b"
+    )
     parser.add_argument("--model-name", type=str)
     parser.add_argument("--limit-model-concurrency", type=int, default=1024)
     parser.add_argument("--stream-interval", type=int, default=2)
     parser.add_argument("--no-register", action="store_true")
     # cacheflow specific params
-    parser.add_argument('--block-size', type=int, default=8, choices=[8, 16],
-                        help='token block size')
-    parser.add_argument('--swap-space', type=int, default=20,
-                        help='CPU swap space size (GiB) per GPU')
-    parser.add_argument('--max-num-batched-tokens', type=int, default=2560,
-                        help='maximum number of batched tokens')
+    parser.add_argument(
+        "--block-size", type=int, default=8, choices=[8, 16], help="token block size"
+    )
+    parser.add_argument(
+        "--swap-space", type=int, default=20, help="CPU swap space size (GiB) per GPU"
+    )
+    parser.add_argument(
+        "--max-num-batched-tokens",
+        type=int,
+        default=2560,
+        help="maximum number of batched tokens",
+    )
     args = parser.parse_args()
 
-    (num_nodes, num_devices_per_node, distributed_init_method,
-    all_stage_devices) = initialize_ray_cluster(
-            pipeline_parallel_size=1, tensor_parallel_size=1)
-
-    worker = CacheFlowWorker(args.controller_address,
-                             args.worker_address,
-                             worker_id,
-                             args.no_register,
-                             args.model_path,
-                             args.model_name,
-                             args.block_size,
-                             seed,
-                             args.swap_space,
-                             args.max_num_batched_tokens,
-                             distributed_init_method,
-                             all_stage_devices)
+    (
+        num_nodes,
+        num_devices_per_node,
+        distributed_init_method,
+        all_stage_devices,
+    ) = initialize_ray_cluster(pipeline_parallel_size=1, tensor_parallel_size=1)
+
+    worker = CacheFlowWorker(
+        args.controller_address,
+        args.worker_address,
+        worker_id,
+        args.no_register,
+        args.model_path,
+        args.model_name,
+        args.block_size,
+        seed,
+        args.swap_space,
+        args.max_num_batched_tokens,
+        distributed_init_method,
+        all_stage_devices,
+    )
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
-
```

### Comparing `fschat-0.2.2/fastchat/serve/cli.py` & `fschat-0.2.3/fastchat/serve/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,28 @@
         print(" ".join(outputs[pre:]), flush=True)
         return " ".join(outputs)
 
 
 class RichChatIO(ChatIO):
     def __init__(self):
         self._prompt_session = PromptSession(history=InMemoryHistory())
-        self._completer = WordCompleter(words=['!exit', '!reset'], pattern=re.compile('$'))
+        self._completer = WordCompleter(
+            words=["!exit", "!reset"], pattern=re.compile("$")
+        )
         self._console = Console()
 
     def prompt_for_input(self, role) -> str:
         self._console.print(f"[bold]{role}:")
         # TODO(suquark): multiline input has some issues. fix it later.
         prompt_input = self._prompt_session.prompt(
             completer=self._completer,
             multiline=False,
             auto_suggest=AutoSuggestFromHistory(),
-            key_bindings=None)
+            key_bindings=None,
+        )
         self._console.print()
         return prompt_input
 
     def prompt_for_output(self, role: str):
         self._console.print(f"[bold]{role}:")
 
     def stream_output(self, output_stream, skip_echo_len: int):
@@ -101,32 +104,58 @@
     if args.style == "simple":
         chatio = SimpleChatIO()
     elif args.style == "rich":
         chatio = RichChatIO()
     else:
         raise ValueError(f"Invalid style for console: {args.style}")
     try:
-        chat_loop(args.model_path, args.device, args.num_gpus, args.max_gpu_memory,
-            args.load_8bit, args.conv_template, args.temperature, args.max_new_tokens,
-            chatio, args.debug)
+        chat_loop(
+            args.model_path,
+            args.device,
+            args.num_gpus,
+            args.max_gpu_memory,
+            args.load_8bit,
+            args.conv_template,
+            args.temperature,
+            args.max_new_tokens,
+            chatio,
+            args.debug,
+        )
     except KeyboardInterrupt:
         print("exit...")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument("--model-path", type=str, default="facebook/opt-350m",
-        help="The path to the weights")
-    parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
+    parser.add_argument(
+        "--model-path",
+        type=str,
+        default="facebook/opt-350m",
+        help="The path to the weights",
+    )
+    parser.add_argument(
+        "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
+    )
     parser.add_argument("--num-gpus", type=str, default="1")
-    parser.add_argument("--max-gpu-memory", type=str, default="13GiB")
-    parser.add_argument("--load-8bit", action="store_true",
-        help="Use 8-bit quantization.")
-    parser.add_argument("--conv-template", type=str, default=None,
-        help="Conversation prompt template.")
+    parser.add_argument(
+        "--max-gpu-memory",
+        type=str,
+        help="The maximum memory per gpu. Use a string like '13Gib'",
+    )
+    parser.add_argument(
+        "--load-8bit", action="store_true", help="Use 8-bit quantization."
+    )
+    parser.add_argument(
+        "--conv-template", type=str, default=None, help="Conversation prompt template."
+    )
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
-    parser.add_argument("--style", type=str, default="simple",
-                        choices=["simple", "rich"], help="Display style.")
+    parser.add_argument(
+        "--style",
+        type=str,
+        default="simple",
+        choices=["simple", "rich"],
+        help="Display style.",
+    )
     parser.add_argument("--debug", action="store_true")
     args = parser.parse_args()
     main(args)
```

### Comparing `fschat-0.2.2/fastchat/serve/compression.py` & `fschat-0.2.3/fastchat/serve/compression.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 import torch.nn as nn
 from torch.nn import functional as F
 
 
 @dataclasses.dataclass
 class CompressionConfig:
     """Group-wise quantization."""
+
     num_bits: int
     group_size: int
     group_dim: int
     symmetric: bool
     enabled: bool = True
 
 
 default_compression_config = CompressionConfig(
-    num_bits=8, group_size=256, group_dim=1, symmetric=True, enabled=True)
+    num_bits=8, group_size=256, group_dim=1, symmetric=True, enabled=True
+)
 
 
 class CLinear(nn.Module):
     """Compressed Linear Layer."""
 
     def __init__(self, weight, bias, device):
         super().__init__()
@@ -34,53 +36,65 @@
         return F.linear(input, weight, self.bias)
 
 
 def compress_module(module, target_device):
     for attr_str in dir(module):
         target_attr = getattr(module, attr_str)
         if type(target_attr) == torch.nn.Linear:
-            setattr(module, attr_str,
-                CLinear(target_attr.weight, target_attr.bias, target_device))
+            setattr(
+                module,
+                attr_str,
+                CLinear(target_attr.weight, target_attr.bias, target_device),
+            )
     for name, child in module.named_children():
         compress_module(child, target_device)
 
 
 def compress(tensor, config):
     """Simulate group-wise quantization."""
     if not config.enabled:
         return tensor
 
     group_size, num_bits, group_dim, symmetric = (
-        config.group_size, config.num_bits, config.group_dim, config.symmetric)
+        config.group_size,
+        config.num_bits,
+        config.group_dim,
+        config.symmetric,
+    )
     assert num_bits <= 8
 
     original_shape = tensor.shape
     num_groups = (original_shape[group_dim] + group_size - 1) // group_size
-    new_shape = (original_shape[:group_dim] + (num_groups, group_size) +
-                 original_shape[group_dim+1:])
+    new_shape = (
+        original_shape[:group_dim]
+        + (num_groups, group_size)
+        + original_shape[group_dim + 1 :]
+    )
 
     # Pad
     pad_len = (group_size - original_shape[group_dim] % group_size) % group_size
     if pad_len != 0:
-        pad_shape = original_shape[:group_dim] + (pad_len,) + original_shape[group_dim+1:]
-        tensor = torch.cat([
-            tensor,
-            torch.zeros(pad_shape, dtype=tensor.dtype, device=tensor.device)],
-            dim=group_dim)
+        pad_shape = (
+            original_shape[:group_dim] + (pad_len,) + original_shape[group_dim + 1 :]
+        )
+        tensor = torch.cat(
+            [tensor, torch.zeros(pad_shape, dtype=tensor.dtype, device=tensor.device)],
+            dim=group_dim,
+        )
     data = tensor.view(new_shape)
 
     # Quantize
     if symmetric:
         B = 2 ** (num_bits - 1) - 1
         scale = B / torch.max(data.abs(), dim=group_dim + 1, keepdim=True)[0]
         data = data * scale
         data = data.clamp_(-B, B).round_().to(torch.int8)
         return data, scale, original_shape
     else:
-        B = 2 ** num_bits - 1
+        B = 2**num_bits - 1
         mn = torch.min(data, dim=group_dim + 1, keepdim=True)[0]
         mx = torch.max(data, dim=group_dim + 1, keepdim=True)[0]
 
         scale = B / (mx - mn)
         data = data - mn
         data.mul_(scale)
 
@@ -90,30 +104,35 @@
 
 def decompress(packed_data, config):
     """Simulate group-wise dequantization."""
     if not config.enabled:
         return packed_data
 
     group_size, num_bits, group_dim, symmetric = (
-        config.group_size, config.num_bits, config.group_dim, config.symmetric)
+        config.group_size,
+        config.num_bits,
+        config.group_dim,
+        config.symmetric,
+    )
 
     # Dequantize
     if symmetric:
         data, scale, original_shape = packed_data
         data = data / scale
     else:
         data, mn, scale, original_shape = packed_data
         data = data / scale
         data.add_(mn)
 
     # Unpad
     pad_len = (group_size - original_shape[group_dim] % group_size) % group_size
     if pad_len:
         padded_original_shape = (
-            original_shape[:group_dim] +
-            (original_shape[group_dim] + pad_len,) +
-            original_shape[group_dim+1:])
+            original_shape[:group_dim]
+            + (original_shape[group_dim] + pad_len,)
+            + original_shape[group_dim + 1 :]
+        )
         data = data.reshape(padded_original_shape)
         indices = [slice(0, x) for x in original_shape]
         return data[indices].contiguous()
     else:
         return data.view(original_shape)
```

### Comparing `fschat-0.2.2/fastchat/serve/controller.py` & `fschat-0.2.3/fastchat/serve/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,34 +57,40 @@
 class Controller:
     def __init__(self, dispatch_method: str):
         # Dict[str -> WorkerInfo]
         self.worker_info = {}
         self.dispatch_method = DispatchMethod.from_str(dispatch_method)
 
         self.heart_beat_thread = threading.Thread(
-            target=heart_beat_controller, args=(self,))
+            target=heart_beat_controller, args=(self,)
+        )
         self.heart_beat_thread.start()
 
         logger.info("Init controller")
 
-    def register_worker(self, worker_name: str, check_heart_beat: bool,
-                        worker_status: dict):
+    def register_worker(
+        self, worker_name: str, check_heart_beat: bool, worker_status: dict
+    ):
         if worker_name not in self.worker_info:
             logger.info(f"Register a new worker: {worker_name}")
         else:
             logger.info(f"Register an existing worker: {worker_name}")
 
         if not worker_status:
             worker_status = self.get_worker_status(worker_name)
         if not worker_status:
             return False
 
         self.worker_info[worker_name] = WorkerInfo(
-            worker_status["model_names"], worker_status["speed"], worker_status["queue_length"],
-            check_heart_beat, time.time())
+            worker_status["model_names"],
+            worker_status["speed"],
+            worker_status["queue_length"],
+            check_heart_beat,
+            time.time(),
+        )
 
         logger.info(f"Register done: {worker_name}, {worker_status}")
         return True
 
     def get_worker_status(self, worker_name: str):
         try:
             r = requests.post(worker_name + "/worker_get_status", timeout=5)
@@ -127,23 +133,21 @@
                     worker_speeds.append(w_info.speed)
             worker_speeds = np.array(worker_speeds, dtype=np.float32)
             norm = np.sum(worker_speeds)
             if norm < 1e-4:
                 return ""
             worker_speeds = worker_speeds / norm
             if True:  # Directly return address
-                pt = np.random.choice(np.arange(len(worker_names)),
-                    p=worker_speeds)
+                pt = np.random.choice(np.arange(len(worker_names)), p=worker_speeds)
                 worker_name = worker_names[pt]
                 return worker_name
 
             # Check status before returning
             while True:
-                pt = np.random.choice(np.arange(len(worker_names)),
-                    p=worker_speeds)
+                pt = np.random.choice(np.arange(len(worker_names)), p=worker_speeds)
                 worker_name = worker_names[pt]
 
                 if self.get_worker_status(worker_name):
                     break
                 else:
                     self.remove_worker(worker_name)
                     worker_speeds[pt] = 0
@@ -161,15 +165,17 @@
                     worker_names.append(w_name)
                     worker_qlen.append(w_info.queue_length / w_info.speed)
             if len(worker_names) == 0:
                 return ""
             min_index = np.argmin(worker_qlen)
             w_name = worker_names[min_index]
             self.worker_info[w_name].queue_length += 1
-            logger.info(f"names: {worker_names}, queue_lens: {worker_qlen}, ret: {w_name}")
+            logger.info(
+                f"names: {worker_names}, queue_lens: {worker_qlen}, ret: {w_name}"
+            )
             return w_name
         else:
             raise ValueError(f"Invalid dispatch method: {self.dispatch_method}")
 
     def receive_heart_beat(self, worker_name: str, queue_length: int):
         if worker_name not in self.worker_info:
             logger.info(f"Receive unknown heart beat. {worker_name}")
@@ -197,28 +203,31 @@
             ret = {
                 "text": server_error_msg,
                 "error_code": 2,
             }
             yield json.dumps(ret).encode() + b"\0"
 
         try:
-            response = requests.post(worker_addr + "/worker_generate_stream",
-                json=params, stream=True, timeout=15)
+            response = requests.post(
+                worker_addr + "/worker_generate_stream",
+                json=params,
+                stream=True,
+                timeout=15,
+            )
             for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
                 if chunk:
                     yield chunk + b"\0"
         except requests.exceptions.RequestException as e:
             logger.info(f"worker timeout: {worker_addr}")
             ret = {
                 "text": server_error_msg,
                 "error_code": 3,
             }
             yield json.dumps(ret).encode() + b"\0"
 
-
     # Let the controller act as a worker to achieve hierarchical
     # management. This can be used to connect isolated sub networks.
     def worker_api_get_status(self):
         model_names = set()
         speed = 0
         queue_length = 0
 
@@ -239,16 +248,16 @@
 app = FastAPI()
 
 
 @app.post("/register_worker")
 async def register_worker(request: Request):
     data = await request.json()
     controller.register_worker(
-        data["worker_name"], data["check_heart_beat"],
-        data.get("worker_status", None))
+        data["worker_name"], data["check_heart_beat"], data.get("worker_status", None)
+    )
 
 
 @app.post("/refresh_all_workers")
 async def refresh_all_workers():
     models = controller.refresh_all_workers()
 
 
@@ -264,16 +273,15 @@
     addr = controller.get_worker_address(data["model"])
     return {"address": addr}
 
 
 @app.post("/receive_heart_beat")
 async def receive_heart_beat(request: Request):
     data = await request.json()
-    exist = controller.receive_heart_beat(
-        data["worker_name"], data["queue_length"])
+    exist = controller.receive_heart_beat(data["worker_name"], data["queue_length"])
     return {"exist": exist}
 
 
 @app.post("/worker_generate_stream")
 async def worker_api_generate_stream(request: Request):
     params = await request.json()
     generator = controller.worker_api_generate_stream(params)
@@ -285,14 +293,18 @@
     return controller.worker_api_get_status()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21001)
-    parser.add_argument("--dispatch-method", type=str, choices=[
-        "lottery", "shortest_queue"], default="shortest_queue")
+    parser.add_argument(
+        "--dispatch-method",
+        type=str,
+        choices=["lottery", "shortest_queue"],
+        default="shortest_queue",
+    )
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     controller = Controller(args.dispatch_method)
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

### Comparing `fschat-0.2.2/fastchat/serve/gradio_css.py` & `fschat-0.2.3/fastchat/serve/gradio_css.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-code_highlight_css = (
-"""
+code_highlight_css = """
 #chatbot .hll { background-color: #ffffcc }
 #chatbot .c { color: #408080; font-style: italic }
 #chatbot .err { border: 1px solid #FF0000 }
 #chatbot .k { color: #008000; font-weight: bold }
 #chatbot .o { color: #666666 }
 #chatbot .ch { color: #408080; font-style: italic }
 #chatbot .cm { color: #408080; font-style: italic }
@@ -64,10 +63,9 @@
 #chatbot .bp { color: #008000 }
 #chatbot .fm { color: #0000FF }
 #chatbot .vc { color: #19177C }
 #chatbot .vg { color: #19177C }
 #chatbot .vi { color: #19177C }
 #chatbot .vm { color: #19177C }
 #chatbot .il { color: #666666 }
-""")
-#.highlight  { background: #f8f8f8; }
-
+"""
+# .highlight  { background: #f8f8f8; }
```

### Comparing `fschat-0.2.2/fastchat/serve/gradio_patch.py` & `fschat-0.2.3/fastchat/serve/gradio_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             elem_id: An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.
             elem_classes: An optional list of strings that are assigned as the classes of this component in the HTML DOM. Can be used for targeting CSS styles.
         """
         if color_map is not None:
             warnings.warn(
                 "The 'color_map' parameter has been deprecated.",
             )
-        #self.md = utils.get_markdown_parser()
+        # self.md = utils.get_markdown_parser()
         self.md = Markdown(extras=["fenced-code-blocks", "tables", "break-on-newline"])
         self.select: EventListenerMethod
         """
         Event listener for when the user selects message from Chatbot.
         Uses event data gradio.SelectData to carry `value` referring to text of selected message, and `index` tuple to refer to [message, participant] index.
         See EventData documentation on how to use this event data.
         """
@@ -109,15 +109,15 @@
                 "is_file": True,
             }
         elif isinstance(
             chat_message, dict
         ):  # This happens for previously processed messages
             return chat_message
         elif isinstance(chat_message, str):
-            #return self.md.render(chat_message)
+            # return self.md.render(chat_message)
             return str(self.md.convert(chat_message))
         else:
             raise ValueError(f"Invalid message for Chatbot component: {chat_message}")
 
     def postprocess(
         self,
         y: List[
@@ -138,17 +138,18 @@
                 message_pair, (tuple, list)
             ), f"Expected a list of lists or list of tuples. Received: {message_pair}"
             assert (
                 len(message_pair) == 2
             ), f"Expected a list of lists of length 2 or list of tuples of length 2. Received: {message_pair}"
             processed_messages.append(
                 (
-                    #self._process_chat_messages(message_pair[0]),
-                    '<pre style="font-family: var(--font)">' +
-                    message_pair[0] + "</pre>",
+                    # self._process_chat_messages(message_pair[0]),
+                    '<pre style="font-family: var(--font)">'
+                    + message_pair[0]
+                    + "</pre>",
                     self._process_chat_messages(message_pair[1]),
                 )
             )
         return processed_messages
 
     def style(self, height: int | None = None, **kwargs):
         """
@@ -160,9 +161,7 @@
             warnings.warn("The 'color_map' parameter has been deprecated.")
 
         Component.style(
             self,
             **kwargs,
         )
         return self
-
-
```

### Comparing `fschat-0.2.2/fastchat/serve/gradio_web_server.py` & `fschat-0.2.3/fastchat/serve/gradio_web_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,50 +5,69 @@
 import os
 import time
 import uuid
 
 import gradio as gr
 import requests
 
-from fastchat.conversation import (get_default_conv_template,
-                                   SeparatorStyle)
+from fastchat.conversation import (
+    get_default_conv_template,
+    compute_skip_echo_len,
+    SeparatorStyle,
+)
 from fastchat.constants import LOGDIR
-from fastchat.utils import (build_logger, server_error_msg,
-    violates_moderation, moderation_msg)
+from fastchat.utils import (
+    build_logger,
+    server_error_msg,
+    violates_moderation,
+    moderation_msg,
+)
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_css import code_highlight_css
-from fastchat.serve.inference import compute_skip_echo_len
 
 
 logger = build_logger("gradio_web_server", "gradio_web_server.log")
 
 headers = {"User-Agent": "fastchat Client"}
 
 no_change_btn = gr.Button.update()
 enable_btn = gr.Button.update(interactive=True)
 disable_btn = gr.Button.update(interactive=False)
 
+controller_url = None
+enable_moderation = False
+models = []
+
 priority = {
-    "vicuna-13b": "aaaaaaa",
-    "koala-13b": "aaaaaab",
-    "dolly-v2-12b": "aaaaaac",
-    "chatglm-6b": "aaaaaad",
+    "vicuna-13b": "aaa",
+    "koala-13b": "aab",
+    "oasst-sft-1-pythia-12b": "aac",
+    "dolly-v2-12b": "aad",
+    "chatglm-6b": "aae",
+    "stablelm-tuned-alpha-7b": "aaf",
 }
 
 
+def set_global_vars(controller_url_, enable_moderation_, models_):
+    global controller_url, enable_moderation, models
+    controller_url = controller_url_
+    enable_moderation = enable_moderation_
+    models = models_
+
+
 def get_conv_log_filename():
     t = datetime.datetime.now()
     name = os.path.join(LOGDIR, f"{t.year}-{t.month:02d}-{t.day:02d}-conv.json")
     return name
 
 
-def get_model_list():
-    ret = requests.post(args.controller_url + "/refresh_all_workers")
+def get_model_list(controller_url):
+    ret = requests.post(controller_url + "/refresh_all_workers")
     assert ret.status_code == 200
-    ret = requests.post(args.controller_url + "/list_models")
+    ret = requests.post(controller_url + "/list_models")
     models = ret.json()["models"]
     models.sort(key=lambda x: priority.get(x, x))
     logger.info(f"Models: {models}")
     return models
 
 
 get_window_url_params = """
@@ -57,46 +76,36 @@
     url_params = Object.fromEntries(params);
     console.log(url_params);
     return url_params;
     }
 """
 
 
-def load_demo(url_params, request: gr.Request):
-    logger.info(f"load_demo. ip: {request.client.host}. params: {url_params}")
-
+def load_demo_single(url_params):
     dropdown_update = gr.Dropdown.update(visible=True)
     if "model" in url_params:
         model = url_params["model"]
         if model in models:
-            dropdown_update = gr.Dropdown.update(
-                value=model, visible=True)
+            dropdown_update = gr.Dropdown.update(value=model, visible=True)
 
     state = None
-    return (state,
-            dropdown_update,
-            gr.Chatbot.update(visible=True),
-            gr.Textbox.update(visible=True),
-            gr.Button.update(visible=True),
-            gr.Row.update(visible=True),
-            gr.Accordion.update(visible=True))
+    return (
+        state,
+        dropdown_update,
+        gr.Chatbot.update(visible=True),
+        gr.Textbox.update(visible=True),
+        gr.Button.update(visible=True),
+        gr.Row.update(visible=True),
+        gr.Accordion.update(visible=True),
+    )
 
 
-def load_demo_refresh_model_list(request: gr.Request):
-    logger.info(f"load_demo. ip: {request.client.host}")
-    models = get_model_list()
-    state = None
-    return (state, gr.Dropdown.update(
-               choices=models,
-               value=models[0] if len(models) > 0 else ""),
-            gr.Chatbot.update(visible=True),
-            gr.Textbox.update(visible=True),
-            gr.Button.update(visible=True),
-            gr.Row.update(visible=True),
-            gr.Accordion.update(visible=True))
+def load_demo(url_params, request: gr.Request):
+    logger.info(f"load_demo. ip: {request.client.host}. params: {url_params}")
+    return load_demo_single(url_params)
 
 
 def vote_last_response(state, vote_type, model_selector, request: gr.Request):
     with open(get_conv_log_filename(), "a") as fout:
         data = {
             "tstamp": round(time.time(), 4),
             "type": vote_type,
@@ -143,21 +152,22 @@
 
     if state is None:
         state = get_default_conv_template("vicuna").copy()
 
     if len(text) <= 0:
         state.skip_next = True
         return (state, state.to_gradio_chatbot(), "") + (no_change_btn,) * 5
-    if args.moderate:
+    if enable_moderation:
         flagged = violates_moderation(text)
         if flagged:
             logger.info(f"violate moderation. ip: {request.client.host}. text: {text}")
             state.skip_next = True
             return (state, state.to_gradio_chatbot(), moderation_msg) + (
-                no_change_btn,) * 5
+                no_change_btn,
+            ) * 5
 
     text = text[:1536]  # Hard cut-off
     state.append_message(state.roles[0], text)
     state.append_message(state.roles[1], None)
     state.skip_next = False
     return (state, state.to_gradio_chatbot(), "") + (disable_btn,) * 5
 
@@ -173,14 +183,16 @@
     return code
 
 
 def http_bot(state, model_selector, temperature, max_new_tokens, request: gr.Request):
     logger.info(f"http_bot. ip: {request.client.host}")
     start_tstamp = time.time()
     model_name = model_selector
+    temperature = float(temperature)
+    max_new_tokens = int(max_new_tokens)
 
     if state.skip_next:
         # This generate call is skipped due to invalid inputs
         yield (state, state.to_gradio_chatbot()) + (no_change_btn,) * 5
         return
 
     if len(state.messages) == state.offset + 2:
@@ -188,211 +200,310 @@
         new_state = get_default_conv_template(model_name).copy()
         new_state.conv_id = uuid.uuid4().hex
         new_state.append_message(new_state.roles[0], state.messages[-2][1])
         new_state.append_message(new_state.roles[1], None)
         state = new_state
 
     # Query worker address
-    controller_url = args.controller_url
-    ret = requests.post(controller_url + "/get_worker_address",
-            json={"model": model_name})
+    ret = requests.post(
+        controller_url + "/get_worker_address", json={"model": model_name}
+    )
     worker_addr = ret.json()["address"]
     logger.info(f"model_name: {model_name}, worker_addr: {worker_addr}")
 
     # No available worker
     if worker_addr == "":
         state.messages[-1][-1] = server_error_msg
-        yield (state, state.to_gradio_chatbot(), disable_btn, disable_btn, disable_btn, enable_btn, enable_btn)
+        yield (
+            state,
+            state.to_gradio_chatbot(),
+            disable_btn,
+            disable_btn,
+            disable_btn,
+            enable_btn,
+            enable_btn,
+        )
         return
 
     # Construct prompt
     if "chatglm" in model_name:
-        prompt = state.messages[state.offset:]
+        prompt = state.messages[state.offset :]
     else:
         prompt = state.get_prompt()
     skip_echo_len = compute_skip_echo_len(model_name, state, prompt)
 
     # Make requests
     pload = {
         "model": model_name,
         "prompt": prompt,
-        "temperature": float(temperature),
-        "max_new_tokens": int(max_new_tokens),
-        "stop": state.sep if state.sep_style == SeparatorStyle.SINGLE else state.sep2,
+        "temperature": temperature,
+        "max_new_tokens": max_new_tokens,
+        "stop": state.sep if state.sep_style == SeparatorStyle.SINGLE else None,
     }
     logger.info(f"==== request ====\n{pload}")
 
     state.messages[-1][-1] = "▌"
     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
 
     try:
         # Stream output
-        response = requests.post(worker_addr + "/worker_generate_stream",
-            headers=headers, json=pload, stream=True, timeout=20)
+        response = requests.post(
+            worker_addr + "/worker_generate_stream",
+            headers=headers,
+            json=pload,
+            stream=True,
+            timeout=20,
+        )
         for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
             if chunk:
                 data = json.loads(chunk.decode())
                 if data["error_code"] == 0:
                     output = data["text"][skip_echo_len:].strip()
                     output = post_process_code(output)
                     state.messages[-1][-1] = output + "▌"
                     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
                 else:
                     output = data["text"] + f" (error_code: {data['error_code']})"
                     state.messages[-1][-1] = output
-                    yield (state, state.to_gradio_chatbot()) + (disable_btn, disable_btn, disable_btn, enable_btn, enable_btn)
+                    yield (state, state.to_gradio_chatbot()) + (
+                        disable_btn,
+                        disable_btn,
+                        disable_btn,
+                        enable_btn,
+                        enable_btn,
+                    )
                     return
                 time.sleep(0.02)
     except requests.exceptions.RequestException as e:
         state.messages[-1][-1] = server_error_msg + f" (error_code: 4)"
-        yield (state, state.to_gradio_chatbot()) + (disable_btn, disable_btn, disable_btn, enable_btn, enable_btn)
+        yield (state, state.to_gradio_chatbot()) + (
+            disable_btn,
+            disable_btn,
+            disable_btn,
+            enable_btn,
+            enable_btn,
+        )
         return
 
     state.messages[-1][-1] = state.messages[-1][-1][:-1]
     yield (state, state.to_gradio_chatbot()) + (enable_btn,) * 5
 
     finish_tstamp = time.time()
     logger.info(f"{output}")
 
     with open(get_conv_log_filename(), "a") as fout:
         data = {
             "tstamp": round(finish_tstamp, 4),
             "type": "chat",
             "model": model_name,
+            "gen_params": {
+                "temperature": temperature,
+                "max_new_tokens": max_new_tokens,
+            },
             "start": round(start_tstamp, 4),
             "finish": round(start_tstamp, 4),
             "state": state.dict(),
             "ip": request.client.host,
         }
         fout.write(json.dumps(data) + "\n")
 
 
-notice_markdown = ("""
+block_css = (
+    code_highlight_css
+    + """
+pre {
+    white-space: pre-wrap;       /* Since CSS 2.1 */
+    white-space: -moz-pre-wrap;  /* Mozilla, since 1999 */
+    white-space: -pre-wrap;      /* Opera 4-6 */
+    white-space: -o-pre-wrap;    /* Opera 7 */
+    word-wrap: break-word;       /* Internet Explorer 5.5+ */
+}
+#notice_markdown th {
+    display: none;
+}
+"""
+)
+
+
+def build_single_model_ui():
+    notice_markdown = """
 # 🏔️ Chat with Open Large Language Models
 - Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[GitHub]](https://github.com/lm-sys/FastChat) [[Evaluation]](https://vicuna.lmsys.org/eval/)
 - Koala: A Dialogue Model for Academic Research. [[Blog post]](https://bair.berkeley.edu/blog/2023/04/03/koala/) [[GitHub]](https://github.com/young-geng/EasyLM)
 - This demo server. [[GitHub]](https://github.com/lm-sys/FastChat)
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. The service may collect user dialogue data for future research.
 
 ### Choose a model to chat with
-- [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations. This one is expected to perform best according to our evaluation.
-- [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a chatbot fine-tuned from LLaMA on user-shared conversations and open-source datasets. This one performs similarly to Vicuna.
-- [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open LLM by Databricks.
-- [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model | 开源双语对话语言模型
-- [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on 52K instruction-following demonstrations.
-- [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models.
-""")
-
+| | |
+| --- | --- |
+| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a chatbot fine-tuned from LLaMA on user-shared conversations and open-source datasets. |
+| [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone. | [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open LLM by Databricks. |
+| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model 开源双语对话语言模型 | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
+| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on 52K instruction-following demonstrations. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models. |
+"""
 
-learn_more_markdown = ("""
+    learn_more_markdown = """
 ### License
 The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
-""")
-
-
-css = code_highlight_css + """
-pre {
-    white-space: pre-wrap;       /* Since CSS 2.1 */
-    white-space: -moz-pre-wrap;  /* Mozilla, since 1999 */
-    white-space: -pre-wrap;      /* Opera 4-6 */
-    white-space: -o-pre-wrap;    /* Opera 7 */
-    word-wrap: break-word;       /* Internet Explorer 5.5+ */
-}
 """
 
+    state = gr.State()
+    notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
 
-def build_demo():
-    with gr.Blocks(title="FastChat", theme=gr.themes.Base(), css=css) as demo:
-        state = gr.State()
+    with gr.Row(elem_id="model_selector_row"):
+        model_selector = gr.Dropdown(
+            choices=models,
+            value=models[0] if len(models) > 0 else "",
+            interactive=True,
+            show_label=False,
+        ).style(container=False)
+
+    chatbot = grChatbot(elem_id="chatbot", visible=False).style(height=550)
+    with gr.Row():
+        with gr.Column(scale=20):
+            textbox = gr.Textbox(
+                show_label=False,
+                placeholder="Enter text and press ENTER",
+                visible=False,
+            ).style(container=False)
+        with gr.Column(scale=1, min_width=50):
+            send_btn = gr.Button(value="Send", visible=False)
+
+    with gr.Row(visible=False) as button_row:
+        upvote_btn = gr.Button(value="👍  Upvote", interactive=False)
+        downvote_btn = gr.Button(value="👎  Downvote", interactive=False)
+        flag_btn = gr.Button(value="⚠️  Flag", interactive=False)
+        # stop_btn = gr.Button(value="⏹️  Stop Generation", interactive=False)
+        regenerate_btn = gr.Button(value="🔄  Regenerate", interactive=False)
+        clear_btn = gr.Button(value="🗑️  Clear history", interactive=False)
+
+    with gr.Accordion("Parameters", open=False, visible=False) as parameter_row:
+        temperature = gr.Slider(
+            minimum=0.0,
+            maximum=1.0,
+            value=0.7,
+            step=0.1,
+            interactive=True,
+            label="Temperature",
+        )
+        max_output_tokens = gr.Slider(
+            minimum=0,
+            maximum=1024,
+            value=512,
+            step=64,
+            interactive=True,
+            label="Max output tokens",
+        )
+
+    gr.Markdown(learn_more_markdown)
+
+    # Register listeners
+    btn_list = [upvote_btn, downvote_btn, flag_btn, regenerate_btn, clear_btn]
+    upvote_btn.click(
+        upvote_last_response,
+        [state, model_selector],
+        [textbox, upvote_btn, downvote_btn, flag_btn],
+    )
+    downvote_btn.click(
+        downvote_last_response,
+        [state, model_selector],
+        [textbox, upvote_btn, downvote_btn, flag_btn],
+    )
+    flag_btn.click(
+        flag_last_response,
+        [state, model_selector],
+        [textbox, upvote_btn, downvote_btn, flag_btn],
+    )
+    regenerate_btn.click(regenerate, state, [state, chatbot, textbox] + btn_list).then(
+        http_bot,
+        [state, model_selector, temperature, max_output_tokens],
+        [state, chatbot] + btn_list,
+    )
+    clear_btn.click(clear_history, None, [state, chatbot, textbox] + btn_list)
+
+    model_selector.change(clear_history, None, [state, chatbot, textbox] + btn_list)
+
+    textbox.submit(
+        add_text, [state, textbox], [state, chatbot, textbox] + btn_list
+    ).then(
+        http_bot,
+        [state, model_selector, temperature, max_output_tokens],
+        [state, chatbot] + btn_list,
+    )
+    send_btn.click(
+        add_text, [state, textbox], [state, chatbot, textbox] + btn_list
+    ).then(
+        http_bot,
+        [state, model_selector, temperature, max_output_tokens],
+        [state, chatbot] + btn_list,
+    )
 
-        # Draw layout
-        notice = gr.Markdown(notice_markdown)
+    return state, model_selector, chatbot, textbox, send_btn, button_row, parameter_row
 
-        with gr.Row(elem_id="model_selector_row"):
-            model_selector = gr.Dropdown(
-                choices=models,
-                value=models[0] if len(models) > 0 else "",
-                interactive=True,
-                show_label=False).style(container=False)
-
-        chatbot = grChatbot(elem_id="chatbot", visible=False).style(height=550)
-        with gr.Row():
-            with gr.Column(scale=20):
-                textbox = gr.Textbox(show_label=False,
-                    placeholder="Enter text and press ENTER", visible=False).style(container=False)
-            with gr.Column(scale=1, min_width=50):
-                submit_btn = gr.Button(value="Send", visible=False)
-
-        with gr.Row(visible=False) as button_row:
-            upvote_btn = gr.Button(value="👍  Upvote", interactive=False)
-            downvote_btn = gr.Button(value="👎  Downvote", interactive=False)
-            flag_btn = gr.Button(value="⚠️  Flag", interactive=False)
-            #stop_btn = gr.Button(value="⏹️  Stop Generation", interactive=False)
-            regenerate_btn = gr.Button(value="🔄  Regenerate", interactive=False)
-            clear_btn = gr.Button(value="🗑️  Clear history", interactive=False)
-
-        with gr.Accordion("Parameters", open=False, visible=False) as parameter_row:
-            temperature = gr.Slider(minimum=0.0, maximum=1.0, value=0.7, step=0.1, interactive=True, label="Temperature",)
-            max_output_tokens = gr.Slider(minimum=0, maximum=1024, value=512, step=64, interactive=True, label="Max output tokens",)
 
-        gr.Markdown(learn_more_markdown)
+def build_demo():
+    with gr.Blocks(
+        title="Chat with Open Large Language Models",
+        theme=gr.themes.Base(),
+        css=block_css,
+    ) as demo:
         url_params = gr.JSON(visible=False)
 
-        # Register listeners
-        btn_list = [upvote_btn, downvote_btn, flag_btn, regenerate_btn, clear_btn]
-        upvote_btn.click(upvote_last_response,
-            [state, model_selector], [textbox, upvote_btn, downvote_btn, flag_btn])
-        downvote_btn.click(downvote_last_response,
-            [state, model_selector], [textbox, upvote_btn, downvote_btn, flag_btn])
-        flag_btn.click(flag_last_response,
-            [state, model_selector], [textbox, upvote_btn, downvote_btn, flag_btn])
-        regenerate_btn.click(regenerate, state,
-            [state, chatbot, textbox] + btn_list).then(
-            http_bot, [state, model_selector, temperature, max_output_tokens],
-            [state, chatbot] + btn_list)
-        clear_btn.click(clear_history, None, [state, chatbot, textbox] + btn_list)
-
-        model_selector.change(clear_history, None, [state, chatbot, textbox] + btn_list)
-
-        textbox.submit(add_text, [state, textbox], [state, chatbot, textbox] + btn_list
-            ).then(http_bot, [state, model_selector, temperature, max_output_tokens],
-                   [state, chatbot] + btn_list)
-        submit_btn.click(add_text, [state, textbox], [state, chatbot, textbox] + btn_list
-            ).then(http_bot, [state, model_selector, temperature, max_output_tokens],
-                   [state, chatbot] + btn_list)
+        (
+            state,
+            model_selector,
+            chatbot,
+            textbox,
+            send_btn,
+            button_row,
+            parameter_row,
+        ) = build_single_model_ui()
 
         if args.model_list_mode == "once":
-            demo.load(load_demo, [url_params], [state, model_selector,
-                chatbot, textbox, submit_btn, button_row, parameter_row],
-                _js=get_window_url_params)
-        elif args.model_list_mode == "reload":
-            demo.load(load_demo_refresh_model_list, None, [state, model_selector,
-                chatbot, textbox, submit_btn, button_row, parameter_row])
+            demo.load(
+                load_demo,
+                [url_params],
+                [
+                    state,
+                    model_selector,
+                    chatbot,
+                    textbox,
+                    send_btn,
+                    button_row,
+                    parameter_row,
+                ],
+                _js=get_window_url_params,
+            )
         else:
             raise ValueError(f"Unknown model list mode: {args.model_list_mode}")
 
     return demo
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="0.0.0.0")
     parser.add_argument("--port", type=int)
     parser.add_argument("--controller-url", type=str, default="http://localhost:21001")
     parser.add_argument("--concurrency-count", type=int, default=10)
-    parser.add_argument("--model-list-mode", type=str, default="once",
-        choices=["once", "reload"])
+    parser.add_argument(
+        "--model-list-mode", type=str, default="once", choices=["once", "reload"]
+    )
     parser.add_argument("--share", action="store_true")
-    parser.add_argument("--moderate", action="store_true",
-        help="Enable content moderation")
+    parser.add_argument(
+        "--moderate", action="store_true", help="Enable content moderation"
+    )
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
-    models = get_model_list()
+    models = get_model_list(args.controller_url)
+    set_global_vars(args.controller_url, args.moderate, models)
 
     logger.info(args)
     demo = build_demo()
-    demo.queue(concurrency_count=args.concurrency_count, status_update_rate=10,
-               api_open=False).launch(server_name=args.host, server_port=args.port,
-                                      share=args.share, max_threads=200)
+    demo.queue(
+        concurrency_count=args.concurrency_count, status_update_rate=10, api_open=False
+    ).launch(
+        server_name=args.host, server_port=args.port, share=args.share, max_threads=200
+    )
```

### Comparing `fschat-0.2.2/fastchat/serve/huggingface_api.py` & `fschat-0.2.3/fastchat/serve/huggingface_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,55 +4,74 @@
 """
 import argparse
 import json
 
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
-from fastchat.conversation import get_default_conv_template
-from fastchat.serve.inference import load_model, compute_skip_echo_len
+from fastchat.conversation import get_default_conv_template, compute_skip_echo_len
+from fastchat.serve.inference import load_model
 
 
 @torch.inference_mode()
 def main(args):
-    model, tokenizer = load_model(args.model_path, args.device,
-        args.num_gpus, args.max_gpu_memory, args.load_8bit, debug=args.debug)
+    model, tokenizer = load_model(
+        args.model_path,
+        args.device,
+        args.num_gpus,
+        args.max_gpu_memory,
+        args.load_8bit,
+        debug=args.debug,
+    )
 
     msg = args.message
 
     conv = get_default_conv_template(args.model_path).copy()
     conv.append_message(conv.roles[0], msg)
     conv.append_message(conv.roles[1], None)
     prompt = conv.get_prompt()
 
     inputs = tokenizer([prompt])
     output_ids = model.generate(
         torch.as_tensor(inputs.input_ids).cuda(),
         do_sample=True,
         temperature=0.7,
-        max_new_tokens=1024)
+        max_new_tokens=1024,
+    )
     outputs = tokenizer.batch_decode(output_ids, skip_special_tokens=True)[0]
     skip_echo_len = compute_skip_echo_len(args.model_path, conv, prompt)
     outputs = outputs[skip_echo_len:]
 
     print(f"{conv.roles[0]}: {msg}")
     print(f"{conv.roles[1]}: {outputs}")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument("--model-path", type=str, default="facebook/opt-350m",
-        help="The path to the weights")
-    parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
+    parser.add_argument(
+        "--model-path",
+        type=str,
+        default="facebook/opt-350m",
+        help="The path to the weights",
+    )
+    parser.add_argument(
+        "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
+    )
     parser.add_argument("--num-gpus", type=str, default="1")
-    parser.add_argument("--max-gpu-memory", type=str, default="13GiB")
-    parser.add_argument("--load-8bit", action="store_true",
-        help="Use 8-bit quantization.")
-    parser.add_argument("--conv-template", type=str, default=None,
-        help="Conversation prompt template.")
+    parser.add_argument(
+        "--max-gpu-memory",
+        type=str,
+        help="The maximum memory per gpu. Use a string like '13Gib'",
+    )
+    parser.add_argument(
+        "--load-8bit", action="store_true", help="Use 8-bit quantization."
+    )
+    parser.add_argument(
+        "--conv-template", type=str, default=None, help="Conversation prompt template."
+    )
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
     parser.add_argument("--debug", action="store_true")
     parser.add_argument("--message", type=str, default="Hello! Who are you?")
     args = parser.parse_args()
 
     main(args)
```

### Comparing `fschat-0.2.2/fastchat/serve/inference.py` & `fschat-0.2.3/fastchat/serve/inference.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 """Inference for FastChat models."""
 import abc
 from typing import Optional
 import warnings
 
 import torch
+
 try:
-    from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer, LlamaForCausalLM, AutoModel, LlamaForCausalLM
+    from transformers import (
+        AutoTokenizer,
+        AutoModelForCausalLM,
+        LlamaTokenizer,
+        LlamaForCausalLM,
+        AutoModel,
+        AutoModelForSeq2SeqLM,
+    )
 except ImportError:
-    from transformers import AutoTokenizer, AutoModelForCausalLM, LLaMATokenizer, LLamaForCausalLM, AutoModel
-
-from fastchat.conversation import conv_templates, get_default_conv_template, SeparatorStyle
+    from transformers import (
+        AutoTokenizer,
+        AutoModelForCausalLM,
+        LLaMATokenizer,
+        LLamaForCausalLM,
+        AutoModel,
+        AutoModelForSeq2SeqLM,
+    )
+
+from fastchat.conversation import (
+    conv_templates,
+    get_default_conv_template,
+    compute_skip_echo_len,
+    SeparatorStyle,
+)
 from fastchat.serve.compression import compress_module
-from fastchat.serve.monkey_patch_non_inplace import replace_llama_attn_with_non_inplace_operations
+from fastchat.serve.monkey_patch_non_inplace import (
+    replace_llama_attn_with_non_inplace_operations,
+)
 from fastchat.serve.serve_chatglm import chatglm_generate_stream
 
 
 def raise_warning_for_old_weights(model_path, model):
     if "vicuna" in model_path.lower():
         try:
             is_vicuna = isinstance(model, LlamaForCausalLM)
@@ -24,67 +46,96 @@
         if is_vicuna and model.model.vocab_size > 32000:
             warnings.warn(
                 "\nYou are probably using the old Vicuna-v0 model, "
                 "which will generate unexpected results with the "
                 "current fschat.\nYou can try one of the following methods:\n"
                 "1. Upgrade your weights to the new Vicuna-v1.1: https://github.com/lm-sys/FastChat#vicuna-weights.\n"
                 "2. Use the old conversation template by `python3 -m fastchat.serve.cli --model-path /path/to/vicuna-v0 --conv-template conv_one_shot`\n"
-                "3. Downgrade fschat to fschat==0.1.10 (Not recommonded).\n")
+                "3. Downgrade fschat to fschat==0.1.10 (Not recommonded).\n"
+            )
 
 
-def compute_skip_echo_len(model_name, conv, prompt):
-    model_name = model_name.lower()
-    if "chatglm" in model_name:
-        skip_echo_len = len(conv.messages[-2][1]) + 1
-    elif "dolly" in model_name:
-        special_toks = ["### Instruction:", "### Response:", "### End"]
-        prompt_tmp = prompt
-        for tok in special_toks:
-            prompt_tmp = prompt_tmp.replace(tok, "")
-        skip_echo_len = len(prompt_tmp)
-    else:
-        skip_echo_len = len(prompt) + 1 - prompt.count("</s>") * 3
-    return skip_echo_len
-
-
-def load_model(model_path, device, num_gpus, max_gpu_memory="13GiB",
-               load_8bit=False, debug=False):
+def get_gpu_memory(max_gpus=None):
+    gpu_memory = []
+    num_gpus = (
+        torch.cuda.device_count()
+        if max_gpus is None
+        else min(max_gpus, torch.cuda.device_count())
+    )
+
+    for gpu_id in range(num_gpus):
+        with torch.cuda.device(gpu_id):
+            device = torch.cuda.current_device()
+            gpu_properties = torch.cuda.get_device_properties(device)
+            total_memory = gpu_properties.total_memory / (1024**3)
+            allocated_memory = torch.cuda.memory_allocated() / (1024**3)
+            available_memory = total_memory - allocated_memory
+            gpu_memory.append(available_memory)
+    return gpu_memory
+
+
+def load_model(
+    model_path, device, num_gpus, max_gpu_memory=None, load_8bit=False, debug=False
+):
     if device == "cpu":
         kwargs = {}
     elif device == "cuda":
         kwargs = {"torch_dtype": torch.float16}
         if num_gpus == "auto":
             kwargs["device_map"] = "auto"
         else:
             num_gpus = int(num_gpus)
             if num_gpus != 1:
-                kwargs.update({
-                    "device_map": "auto",
-                    "max_memory": {i: max_gpu_memory for i in range(num_gpus)},
-                })
+                kwargs["device_map"] = "auto"
+                if max_gpu_memory is None:
+                    kwargs[
+                        "device_map"
+                    ] = "sequential"  # This is important for not the same VRAM sizes
+                    available_gpu_memory = get_gpu_memory(num_gpus)
+                    kwargs["max_memory"] = {
+                        i: str(int(available_gpu_memory[i] * 0.85)) + "GiB"
+                        for i in range(num_gpus)
+                    }
+                else:
+                    kwargs["max_memory"] = {i: max_gpu_memory for i in range(num_gpus)}
+        print("init_kwargs", kwargs)
     elif device == "mps":
         kwargs = {"torch_dtype": torch.float16}
         # Avoid bugs in mps backend by not using in-place operations.
         replace_llama_attn_with_non_inplace_operations()
     else:
         raise ValueError(f"Invalid device: {device}")
 
     if "chatglm" in model_path:
         tokenizer = AutoTokenizer.from_pretrained(model_path, trust_remote_code=True)
-        model = AutoModel.from_pretrained(model_path, trust_remote_code=True).half().cuda()
+        model = AutoModel.from_pretrained(
+            model_path, trust_remote_code=True, **kwargs
+        ).cuda()
+    elif "google/flan-t5" in model_path:
+        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
+        model = AutoModelForSeq2SeqLM.from_pretrained(
+            model_path, low_cpu_mem_usage=True, **kwargs
+        )
     elif "dolly" in model_path:
-        kwargs.update({"torch_dtype": torch.bfloat16})
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
+        model = AutoModelForCausalLM.from_pretrained(
+            model_path, low_cpu_mem_usage=True, **kwargs
+        )
         # 50277 means "### End"
         tokenizer.eos_token_id = 50277
-        model = AutoModelForCausalLM.from_pretrained(model_path, low_cpu_mem_usage=True, **kwargs)
+    elif "pythia" in model_path or "stablelm" in model_path:
+        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
+        model = AutoModelForCausalLM.from_pretrained(
+            model_path, low_cpu_mem_usage=True, **kwargs
+        )
     else:
         tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
-        model = AutoModelForCausalLM.from_pretrained(model_path,
-            low_cpu_mem_usage=True, **kwargs)
+        model = AutoModelForCausalLM.from_pretrained(
+            model_path, low_cpu_mem_usage=True, **kwargs
+        )
         raise_warning_for_old_weights(model_path, model)
 
     if load_8bit:
         compress_module(model, device)
 
     if (device == "cuda" and num_gpus == 1) or device == "mps":
         model.to(device)
@@ -92,42 +143,70 @@
     if debug:
         print(model)
 
     return model, tokenizer
 
 
 @torch.inference_mode()
-def generate_stream(model, tokenizer, params, device,
-                    context_len=2048, stream_interval=2):
+def generate_stream(
+    model, tokenizer, params, device, context_len=2048, stream_interval=2
+):
     prompt = params["prompt"]
     l_prompt = len(prompt)
     temperature = float(params.get("temperature", 1.0))
     max_new_tokens = int(params.get("max_new_tokens", 256))
     stop_str = params.get("stop", None)
-    if stop_str == tokenizer.eos_token:
-        stop_str = None
+    stop_token_ids = params.get("stop_ids", [tokenizer.eos_token_id])
 
     input_ids = tokenizer(prompt).input_ids
     output_ids = list(input_ids)
 
     max_src_len = context_len - max_new_tokens - 8
     input_ids = input_ids[-max_src_len:]
 
     for i in range(max_new_tokens):
         if i == 0:
-            out = model(
-                torch.as_tensor([input_ids], device=device), use_cache=True)
-            logits = out.logits
-            past_key_values = out.past_key_values
+            if model.config.is_encoder_decoder:
+                encoder_outputs = model.encoder(
+                    input_ids=torch.as_tensor([input_ids], device=device)
+                )
+                out = model(
+                    torch.as_tensor([input_ids], device=device),
+                    decoder_input_ids=torch.as_tensor(
+                        [[model.generation_config.decoder_start_token_id]],
+                        device=device,
+                    ),
+                    encoder_outputs=encoder_outputs,
+                    use_cache=True,
+                )
+                logits = out.logits
+                past_key_values = out.past_key_values
+            else:
+                out = model(torch.as_tensor([input_ids], device=device), use_cache=True)
+                logits = out.logits
+                past_key_values = out.past_key_values
         else:
-            out = model(input_ids=torch.as_tensor([[token]], device=device),
-                        use_cache=True,
-                        past_key_values=past_key_values)
-            logits = out.logits
-            past_key_values = out.past_key_values
+            if model.config.is_encoder_decoder:
+                out = model(
+                    input_ids=torch.as_tensor([input_ids], device=device),
+                    use_cache=True,
+                    encoder_outputs=encoder_outputs,
+                    decoder_input_ids=torch.as_tensor([[token]], device=device),
+                    past_key_values=past_key_values,
+                )
+                logits = out.logits
+                past_key_values = out.past_key_values
+            else:
+                out = model(
+                    input_ids=torch.as_tensor([[token]], device=device),
+                    use_cache=True,
+                    past_key_values=past_key_values,
+                )
+                logits = out.logits
+                past_key_values = out.past_key_values
 
         last_token_logits = logits[0][-1]
 
         if device == "mps":
             # Switch to CPU by avoiding some bugs in mps backend.
             last_token_logits = last_token_logits.float().to("cpu")
 
@@ -135,15 +214,15 @@
             token = int(torch.argmax(last_token_logits))
         else:
             probs = torch.softmax(last_token_logits / temperature, dim=-1)
             token = int(torch.multinomial(probs, num_samples=1))
 
         output_ids.append(token)
 
-        if token == tokenizer.eos_token_id:
+        if token in stop_token_ids:
             stopped = True
         else:
             stopped = False
 
         if i % stream_interval == 0 or i == max_new_tokens - 1 or stopped:
             output = tokenizer.decode(output_ids, skip_special_tokens=True)
             if stop_str:
@@ -169,22 +248,30 @@
         """Prompt for output from a role."""
 
     @abc.abstractmethod
     def stream_output(self, output_stream, skip_echo_len: int):
         """Stream output."""
 
 
-def chat_loop(model_path: str, device: str, num_gpus: str,
-              max_gpu_memory: str, load_8bit: bool,
-              conv_template: Optional[str], temperature: float,
-              max_new_tokens: int, chatio: ChatIO,
-              debug: bool):
+def chat_loop(
+    model_path: str,
+    device: str,
+    num_gpus: str,
+    max_gpu_memory: str,
+    load_8bit: bool,
+    conv_template: Optional[str],
+    temperature: float,
+    max_new_tokens: int,
+    chatio: ChatIO,
+    debug: bool,
+):
     # Model
-    model, tokenizer = load_model(model_path, device,
-        num_gpus, max_gpu_memory, load_8bit, debug)
+    model, tokenizer = load_model(
+        model_path, device, num_gpus, max_gpu_memory, load_8bit, debug
+    )
     is_chatglm = "chatglm" in str(type(model)).lower()
 
     # Chat
     if conv_template:
         conv = conv_templates[conv_template].copy()
     else:
         conv = get_default_conv_template(model_path).copy()
@@ -198,28 +285,28 @@
             print("exit...")
             break
 
         conv.append_message(conv.roles[0], inp)
         conv.append_message(conv.roles[1], None)
 
         if is_chatglm:
-            prompt = conv.messages[conv.offset:]
+            prompt = conv.messages[conv.offset :]
             generate_stream_func = chatglm_generate_stream
         else:
             generate_stream_func = generate_stream
             prompt = conv.get_prompt()
 
         skip_echo_len = compute_skip_echo_len(model_path, conv, prompt)
 
         params = {
             "model": model_path,
             "prompt": prompt,
             "temperature": temperature,
             "max_new_tokens": max_new_tokens,
-            "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else conv.sep2,
+            "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else None,
         }
 
         chatio.prompt_for_output(conv.roles[1])
         output_stream = generate_stream_func(model, tokenizer, params, device)
         outputs = chatio.stream_output(output_stream, skip_echo_len)
         # NOTE: strip is important to align with the training data.
         conv.messages[-1][-1] = outputs.strip()
```

### Comparing `fschat-0.2.2/fastchat/serve/model_worker.py` & `fschat-0.2.3/fastchat/serve/model_worker.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,58 +10,78 @@
 from typing import List, Union
 import threading
 import uuid
 
 from fastapi import FastAPI, Request, BackgroundTasks
 from fastapi.responses import StreamingResponse
 import requests
+
 try:
-    from transformers import AutoTokenizer, AutoModelForCausalLM, LlamaTokenizer, AutoModel
+    from transformers import (
+        AutoTokenizer,
+        AutoModelForCausalLM,
+        LlamaTokenizer,
+        AutoModel,
+    )
 except ImportError:
-    from transformers import AutoTokenizer, AutoModelForCausalLM, LLaMATokenizer, AutoModel
+    from transformers import (
+        AutoTokenizer,
+        AutoModelForCausalLM,
+        LLaMATokenizer,
+        AutoModel,
+    )
 import torch
 import uvicorn
 
 from fastchat.constants import WORKER_HEART_BEAT_INTERVAL
 from fastchat.serve.inference import load_model, generate_stream
 from fastchat.serve.serve_chatglm import chatglm_generate_stream
-from fastchat.utils import (build_logger, server_error_msg,
-    pretty_print_semaphore)
+from fastchat.utils import build_logger, server_error_msg, pretty_print_semaphore
 
 GB = 1 << 30
 
 worker_id = str(uuid.uuid4())[:6]
 logger = build_logger("model_worker", f"model_worker_{worker_id}.log")
 global_counter = 0
 
 model_semaphore = None
 
 
 def heart_beat_worker(controller):
-
     while True:
         time.sleep(WORKER_HEART_BEAT_INTERVAL)
         controller.send_heart_beat()
 
 
 class ModelWorker:
-    def __init__(self, controller_addr, worker_addr,
-                 worker_id, no_register, model_path, model_name,
-                 device, num_gpus, max_gpu_memory, load_8bit=False):
+    def __init__(
+        self,
+        controller_addr,
+        worker_addr,
+        worker_id,
+        no_register,
+        model_path,
+        model_name,
+        device,
+        num_gpus,
+        max_gpu_memory,
+        load_8bit=False,
+    ):
         self.controller_addr = controller_addr
         self.worker_addr = worker_addr
         self.worker_id = worker_id
         if model_path.endswith("/"):
             model_path = model_path[:-1]
         self.model_name = model_name or model_path.split("/")[-1]
         self.device = device
 
         logger.info(f"Loading the model {self.model_name} on worker {worker_id} ...")
         self.model, self.tokenizer = load_model(
-            model_path, device, num_gpus, max_gpu_memory, load_8bit)
+            model_path, device, num_gpus, max_gpu_memory, load_8bit
+        )
 
         if hasattr(self.model.config, "max_sequence_length"):
             self.context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self.context_len = self.model.config.max_position_embeddings
         else:
             self.context_len = 2048
@@ -71,68 +91,89 @@
             self.generate_stream_func = chatglm_generate_stream
         else:
             self.generate_stream_func = generate_stream
 
         if not no_register:
             self.register_to_controller()
             self.heart_beat_thread = threading.Thread(
-                target=heart_beat_worker, args=(self,))
+                target=heart_beat_worker, args=(self,)
+            )
             self.heart_beat_thread.start()
 
     def register_to_controller(self):
         logger.info("Register to controller")
 
         url = self.controller_addr + "/register_worker"
         data = {
             "worker_name": self.worker_addr,
             "check_heart_beat": True,
-            "worker_status": self.get_status()
+            "worker_status": self.get_status(),
         }
         r = requests.post(url, json=data)
         assert r.status_code == 200
 
     def send_heart_beat(self):
-        logger.info(f"Send heart beat. Models: {[self.model_name]}. "
-                    f"Semaphore: {pretty_print_semaphore(model_semaphore)}. "
-                    f"global_counter: {global_counter}")
+        logger.info(
+            f"Send heart beat. Models: {[self.model_name]}. "
+            f"Semaphore: {pretty_print_semaphore(model_semaphore)}. "
+            f"global_counter: {global_counter}"
+        )
 
         url = self.controller_addr + "/receive_heart_beat"
 
         while True:
             try:
-                ret = requests.post(url, json={
-                    "worker_name": self.worker_addr,
-                    "queue_length": self.get_queue_length()}, timeout=5)
+                ret = requests.post(
+                    url,
+                    json={
+                        "worker_name": self.worker_addr,
+                        "queue_length": self.get_queue_length(),
+                    },
+                    timeout=5,
+                )
                 exist = ret.json()["exist"]
                 break
             except requests.exceptions.RequestException as e:
                 logger.error(f"heart beat error: {e}")
             time.sleep(5)
 
         if not exist:
             self.register_to_controller()
 
     def get_queue_length(self):
-        if model_semaphore is None or model_semaphore._value is None or model_semaphore._waiters is None:
+        if (
+            model_semaphore is None
+            or model_semaphore._value is None
+            or model_semaphore._waiters is None
+        ):
             return 0
         else:
-            return args.limit_model_concurrency - model_semaphore._value + len(
-                model_semaphore._waiters)
+            return (
+                args.limit_model_concurrency
+                - model_semaphore._value
+                + len(model_semaphore._waiters)
+            )
 
     def get_status(self):
         return {
             "model_names": [self.model_name],
             "speed": 1,
             "queue_length": self.get_queue_length(),
         }
 
     def generate_stream_gate(self, params):
         try:
-            for output in self.generate_stream_func(self.model, self.tokenizer,
-                    params, self.device, self.context_len, args.stream_interval):
+            for output in self.generate_stream_func(
+                self.model,
+                self.tokenizer,
+                params,
+                self.device,
+                self.context_len,
+                args.stream_interval,
+            ):
                 ret = {
                     "text": output,
                     "error_code": 0,
                 }
                 yield json.dumps(ret).encode() + b"\0"
         except torch.cuda.OutOfMemoryError:
             ret = {
@@ -169,36 +210,47 @@
     return worker.get_status()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21002)
-    parser.add_argument("--worker-address", type=str,
-        default="http://localhost:21002")
-    parser.add_argument("--controller-address", type=str,
-        default="http://localhost:21001")
-    parser.add_argument("--model-path", type=str, default="facebook/opt-350m",
-        help="The path to the weights")
-    parser.add_argument("--model-name", type=str,
-        help="Optional name")
-    parser.add_argument("--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda")
+    parser.add_argument("--worker-address", type=str, default="http://localhost:21002")
+    parser.add_argument(
+        "--controller-address", type=str, default="http://localhost:21001"
+    )
+    parser.add_argument(
+        "--model-path",
+        type=str,
+        default="facebook/opt-350m",
+        help="The path to the weights",
+    )
+    parser.add_argument("--model-name", type=str, help="Optional name")
+    parser.add_argument(
+        "--device", type=str, choices=["cpu", "cuda", "mps"], default="cuda"
+    )
     parser.add_argument("--num-gpus", type=int, default=1)
-    parser.add_argument("--max-gpu-memory", type=str, default="13GiB")
+    parser.add_argument(
+        "--max-gpu-memory",
+        type=str,
+        help="The maximum memory per gpu. Use a string like '13Gib'",
+    )
     parser.add_argument("--load-8bit", action="store_true")
     parser.add_argument("--limit-model-concurrency", type=int, default=5)
     parser.add_argument("--stream-interval", type=int, default=2)
     parser.add_argument("--no-register", action="store_true")
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
-    worker = ModelWorker(args.controller_address,
-                         args.worker_address,
-                         worker_id,
-                         args.no_register,
-                         args.model_path,
-                         args.model_name,
-                         args.device,
-                         args.num_gpus,
-                         args.max_gpu_memory,
-                         args.load_8bit)
+    worker = ModelWorker(
+        args.controller_address,
+        args.worker_address,
+        worker_id,
+        args.no_register,
+        args.model_path,
+        args.model_name,
+        args.device,
+        args.num_gpus,
+        args.max_gpu_memory,
+        args.load_8bit,
+    )
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

### Comparing `fschat-0.2.2/fastchat/serve/monkey_patch_non_inplace.py` & `fschat-0.2.3/fastchat/serve/monkey_patch_non_inplace.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,50 +34,70 @@
     position_ids: Optional[torch.LongTensor] = None,
     past_key_value: Optional[Tuple[torch.Tensor]] = None,
     output_attentions: bool = False,
     use_cache: bool = False,
 ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
     bsz, q_len, _ = hidden_states.size()
 
-    query_states = self.q_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-    key_states = self.k_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-    value_states = self.v_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+    query_states = (
+        self.q_proj(hidden_states)
+        .view(bsz, q_len, self.num_heads, self.head_dim)
+        .transpose(1, 2)
+    )
+    key_states = (
+        self.k_proj(hidden_states)
+        .view(bsz, q_len, self.num_heads, self.head_dim)
+        .transpose(1, 2)
+    )
+    value_states = (
+        self.v_proj(hidden_states)
+        .view(bsz, q_len, self.num_heads, self.head_dim)
+        .transpose(1, 2)
+    )
 
     kv_seq_len = key_states.shape[-2]
     if past_key_value is not None:
         kv_seq_len += past_key_value[0].shape[-2]
     cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-    query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+    query_states, key_states = apply_rotary_pos_emb(
+        query_states, key_states, cos, sin, position_ids
+    )
     # [bsz, nh, t, hd]
 
     if past_key_value is not None:
         # reuse k, v, self_attention
         key_states = torch.cat([past_key_value[0], key_states], dim=2)
         value_states = torch.cat([past_key_value[1], value_states], dim=2)
 
     past_key_value = (key_states, value_states) if use_cache else None
 
-    attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
+    attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(
+        self.head_dim
+    )
 
     if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
         raise ValueError(
             f"Attention weights should be of size {(bsz * self.num_heads, q_len, kv_seq_len)}, but is"
             f" {attn_weights.size()}"
         )
 
     if attention_mask is not None:
         if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
             raise ValueError(
                 f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
             )
         attn_weights = attn_weights + attention_mask
-        attn_weights = torch.max(attn_weights, torch.tensor(torch.finfo(attn_weights.dtype).min))
+        attn_weights = torch.max(
+            attn_weights, torch.tensor(torch.finfo(attn_weights.dtype).min)
+        )
 
     # upcast attention to fp32
-    attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
+    attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(
+        query_states.dtype
+    )
     attn_output = torch.matmul(attn_weights, value_states)
 
     if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
         raise ValueError(
             f"`attn_output` should be of size {(bsz, self.num_heads, q_len, self.head_dim)}, but is"
             f" {attn_output.size()}"
         )
```

### Comparing `fschat-0.2.2/fastchat/serve/register_worker.py` & `fschat-0.2.3/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.2/fastchat/serve/serve_chatglm.py` & `fschat-0.2.3/fastchat/serve/serve_chatglm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import torch
 from typing import List, Tuple
 
 
 @torch.inference_mode()
-def chatglm_generate_stream(model, tokenizer, params, device,
-                            context_len=2048, stream_interval=2):
+def chatglm_generate_stream(
+    model, tokenizer, params, device, context_len=2048, stream_interval=2
+):
     """Generate text using model's chat api"""
     messages = params["prompt"]
     max_new_tokens = int(params.get("max_new_tokens", 256))
     temperature = float(params.get("temperature", 1.0))
     top_p = float(params.get("top_p", 0.7))
 
     gen_kwargs = {
         "max_new_tokens": max_new_tokens,
         "do_sample": True,
         "top_p": top_p,
         "temperature": temperature,
-        "logits_processor": None
+        "logits_processor": None,
     }
 
     hist = []
     for i in range(0, len(messages) - 2, 2):
-        hist.append((messages[i][1], messages[i+1][1]))
+        hist.append((messages[i][1], messages[i + 1][1]))
     query = messages[-2][1]
 
     for response, new_hist in model.stream_chat(tokenizer, query, hist):
         output = query + " " + response
         yield output
```

### Comparing `fschat-0.2.2/fastchat/serve/test_message.py` & `fschat-0.2.3/fastchat/serve/test_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import argparse
 import json
 
 import requests
 
-from fastchat.conversation import get_default_conv_template, SeparatorStyle
-from fastchat.serve.inference import compute_skip_echo_len
+from fastchat.conversation import (
+    get_default_conv_template,
+    compute_skip_echo_len,
+    SeparatorStyle,
+)
 
 
 def main():
     model_name = args.model_name
 
     if args.worker_address:
         worker_addr = args.worker_address
@@ -16,16 +19,17 @@
         controller_addr = args.controller_address
         ret = requests.post(controller_addr + "/refresh_all_workers")
         ret = requests.post(controller_addr + "/list_models")
         models = ret.json()["models"]
         models.sort()
         print(f"Models: {models}")
 
-        ret = requests.post(controller_addr + "/get_worker_address",
-            json={"model": model_name})
+        ret = requests.post(
+            controller_addr + "/get_worker_address", json={"model": model_name}
+        )
         worker_addr = ret.json()["address"]
         print(f"worker_addr: {worker_addr}")
 
     if worker_addr == "":
         return
 
     conv = get_default_conv_template(model_name).copy()
@@ -37,32 +41,41 @@
     pload = {
         "model": model_name,
         "prompt": prompt,
         "max_new_tokens": args.max_new_tokens,
         "temperature": args.temperature,
         "stop": conv.sep if conv.sep_style == SeparatorStyle.SINGLE else conv.sep2,
     }
-    response = requests.post(worker_addr + "/worker_generate_stream", headers=headers,
-            json=pload, stream=True)
+    response = requests.post(
+        worker_addr + "/worker_generate_stream",
+        headers=headers,
+        json=pload,
+        stream=True,
+    )
 
     print(f"{conv.roles[0]}: {args.message}")
-    for chunk in response.iter_lines(chunk_size=8192, decode_unicode=False, delimiter=b"\0"):
+    for chunk in response.iter_lines(
+        chunk_size=8192, decode_unicode=False, delimiter=b"\0"
+    ):
         if chunk:
             data = json.loads(chunk.decode("utf-8"))
             skip_echo_len = compute_skip_echo_len(model_name, conv, prompt)
             output = data["text"][skip_echo_len:].strip()
             print(f"{conv.roles[1]}: {output}", end="\r")
     print("")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument("--controller-address", type=str, default="http://localhost:21001")
+    parser.add_argument(
+        "--controller-address", type=str, default="http://localhost:21001"
+    )
     parser.add_argument("--worker-address", type=str)
     parser.add_argument("--model-name", type=str, default="facebook/opt-350m")
     parser.add_argument("--temperature", type=float, default=0.0)
     parser.add_argument("--max-new-tokens", type=int, default=32)
-    parser.add_argument("--message", type=str, default=
-        "Tell me a story with more than 1000 words.")
+    parser.add_argument(
+        "--message", type=str, default="Tell me a story with more than 1000 words."
+    )
     args = parser.parse_args()
 
     main()
```

### Comparing `fschat-0.2.2/fastchat/serve/test_throughput.py` & `fschat-0.2.3/fastchat/serve/test_throughput.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,47 +16,58 @@
         controller_addr = args.controller_address
         ret = requests.post(controller_addr + "/refresh_all_workers")
         ret = requests.post(controller_addr + "/list_models")
         models = ret.json()["models"]
         models.sort()
         print(f"Models: {models}")
 
-        ret = requests.post(controller_addr + "/get_worker_address",
-                            json={"model": args.model_name})
+        ret = requests.post(
+            controller_addr + "/get_worker_address", json={"model": args.model_name}
+        )
         worker_addr = ret.json()["address"]
         print(f"worker_addr: {worker_addr}")
 
     if worker_addr == "":
         return
 
     conv = default_conversation.copy()
     conv.append_message(conv.roles[0], "Tell me a story with more than 1000 words")
     prompt_template = conv.get_prompt()
     prompts = [prompt_template for _ in range(args.n_thread)]
 
     headers = {"User-Agent": "fastchat Client"}
-    ploads = [{
-        "model": args.model_name,
-        "prompt": prompts[i],
-        "max_new_tokens": args.max_new_tokens,
-        "temperature": 0.0,
-        # "stop": conv.sep,
-    } for i in range(len(prompts))]
+    ploads = [
+        {
+            "model": args.model_name,
+            "prompt": prompts[i],
+            "max_new_tokens": args.max_new_tokens,
+            "temperature": 0.0,
+            # "stop": conv.sep,
+        }
+        for i in range(len(prompts))
+    ]
 
     def send_request(results, i):
         if args.test_dispatch:
-            ret = requests.post(controller_addr + "/get_worker_address",
-                                json={"model": args.model_name})
+            ret = requests.post(
+                controller_addr + "/get_worker_address", json={"model": args.model_name}
+            )
             thread_worker_addr = ret.json()["address"]
         else:
             thread_worker_addr = worker_addr
         print(f"thread {i} goes to {thread_worker_addr}")
-        response = requests.post(thread_worker_addr + "/worker_generate_stream", headers=headers,
-                                 json=ploads[i], stream=False)
-        k = list(response.iter_lines(chunk_size=8192, decode_unicode=False, delimiter=b"\0"))
+        response = requests.post(
+            thread_worker_addr + "/worker_generate_stream",
+            headers=headers,
+            json=ploads[i],
+            stream=False,
+        )
+        k = list(
+            response.iter_lines(chunk_size=8192, decode_unicode=False, delimiter=b"\0")
+        )
         # print(k)
         response_new_words = json.loads(k[-2].decode("utf-8"))["text"]
         error_code = json.loads(k[-2].decode("utf-8"))["error_code"]
         # print(f"=== Thread {i} ===, words: {1}, error code: {error_code}")
         results[i] = len(response_new_words.split(" ")) - len(prompts[i].split(" "))
 
     # use N threads to prompt the backend
@@ -79,21 +90,25 @@
     #     # make sure the streaming finishes at EOS or stopping criteria
     #     k = list(response.iter_lines(chunk_size=8192, decode_unicode=False, delimiter=b"\0"))
     #     response_new_words = json.loads(k[-2].decode("utf-8"))["text"]
     #     # print(response_new_words)
     #     n_words += len(response_new_words.split(" ")) - len(prompts[i].split(" "))
     n_words = sum(results)
     time_seconds = time.time() - tik
-    print(f"Time (Completion): {time_seconds}, n threads: {args.n_thread}, "
-          f"throughput: {n_words / time_seconds} words/s.")
+    print(
+        f"Time (Completion): {time_seconds}, n threads: {args.n_thread}, "
+        f"throughput: {n_words / time_seconds} words/s."
+    )
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument("--controller-address", type=str, default="http://localhost:21001")
+    parser.add_argument(
+        "--controller-address", type=str, default="http://localhost:21001"
+    )
     parser.add_argument("--worker-address", type=str)
     parser.add_argument("--model-name", type=str, default="vicuna")
     parser.add_argument("--max-new-tokens", type=int, default=2048)
     parser.add_argument("--n-thread", type=int, default=8)
     parser.add_argument("--test-dispatch", action="store_true")
     args = parser.parse_args()
```

### Comparing `fschat-0.2.2/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.3/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,86 +7,108 @@
 from transformers.models.llama.modeling_llama import apply_rotary_pos_emb
 
 from einops import rearrange
 
 from flash_attn.flash_attn_interface import flash_attn_unpadded_qkvpacked_func
 from flash_attn.bert_padding import unpad_input, pad_input
 
+
 def forward(
     self,
     hidden_states: torch.Tensor,
     attention_mask: Optional[torch.Tensor] = None,
     position_ids: Optional[torch.Tensor] = None,
     past_key_value: Optional[Tuple[torch.Tensor]] = None,
     output_attentions: bool = False,
     use_cache: bool = False,
-) -> Tuple[torch.Tensor, Optional[torch.Tensor],
-            Optional[Tuple[torch.Tensor]]]:
+) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
     """Input shape: Batch x Time x Channel
-    
+
     attention_mask: [bsz, q_len]
     """
     bsz, q_len, _ = hidden_states.size()
 
-    query_states = self.q_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-    key_states = self.k_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-    value_states = self.v_proj(hidden_states).view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+    query_states = (
+        self.q_proj(hidden_states)
+        .view(bsz, q_len, self.num_heads, self.head_dim)
+        .transpose(1, 2)
+    )
+    key_states = (
+        self.k_proj(hidden_states)
+        .view(bsz, q_len, self.num_heads, self.head_dim)
+        .transpose(1, 2)
+    )
+    value_states = (
+        self.v_proj(hidden_states)
+        .view(bsz, q_len, self.num_heads, self.head_dim)
+        .transpose(1, 2)
+    )
     # [bsz, q_len, nh, hd]
     # [bsz, nh, q_len, hd]
 
     kv_seq_len = key_states.shape[-2]
     assert past_key_value is None, "past_key_value is not supported"
 
     cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-    query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+    query_states, key_states = apply_rotary_pos_emb(
+        query_states, key_states, cos, sin, position_ids
+    )
     # [bsz, nh, t, hd]
     assert not output_attentions, "output_attentions is not supported"
     assert not use_cache, "use_cache is not supported"
 
     # Flash attention codes from
     # https://github.com/HazyResearch/flash-attention/blob/main/flash_attn/flash_attention.py
 
     # transform the data into the format required by flash attention
-    qkv = torch.stack([query_states, key_states, value_states], dim=2) # [bsz, nh, 3, q_len, hd]
-    qkv = qkv.transpose(1, 3) # [bsz, q_len, 3, nh, hd]
+    qkv = torch.stack(
+        [query_states, key_states, value_states], dim=2
+    )  # [bsz, nh, 3, q_len, hd]
+    qkv = qkv.transpose(1, 3)  # [bsz, q_len, 3, nh, hd]
     # We have disabled _prepare_decoder_attention_mask in LlamaModel
     # the attention_mask should be the same as the key_padding_mask
     key_padding_mask = attention_mask
 
-
     if key_padding_mask is None:
-        qkv = rearrange(qkv, 'b s ... -> (b s) ...')
+        qkv = rearrange(qkv, "b s ... -> (b s) ...")
         max_s = q_len
-        cu_q_lens = torch.arange(0, (bsz + 1) * q_len, step=q_len, dtype=torch.int32,
-                                device=qkv.device)
+        cu_q_lens = torch.arange(
+            0, (bsz + 1) * q_len, step=q_len, dtype=torch.int32, device=qkv.device
+        )
         output = flash_attn_unpadded_qkvpacked_func(
-            qkv, cu_q_lens, max_s, 0.0,
-            softmax_scale=None, causal=True
+            qkv, cu_q_lens, max_s, 0.0, softmax_scale=None, causal=True
         )
-        output = rearrange(output, '(b s) ... -> b s ...', b=bsz)
+        output = rearrange(output, "(b s) ... -> b s ...", b=bsz)
     else:
         nheads = qkv.shape[-2]
-        x = rearrange(qkv, 'b s three h d -> b s (three h d)')
+        x = rearrange(qkv, "b s three h d -> b s (three h d)")
         x_unpad, indices, cu_q_lens, max_s = unpad_input(x, key_padding_mask)
-        x_unpad = rearrange(x_unpad, 'nnz (three h d) -> nnz three h d', three=3, h=nheads)
+        x_unpad = rearrange(
+            x_unpad, "nnz (three h d) -> nnz three h d", three=3, h=nheads
+        )
         output_unpad = flash_attn_unpadded_qkvpacked_func(
-            x_unpad, cu_q_lens, max_s, 0.0,
-            softmax_scale=None, causal=True
+            x_unpad, cu_q_lens, max_s, 0.0, softmax_scale=None, causal=True
+        )
+        output = rearrange(
+            pad_input(
+                rearrange(output_unpad, "nnz h d -> nnz (h d)"), indices, bsz, q_len
+            ),
+            "b s (h d) -> b s h d",
+            h=nheads,
         )
-        output = rearrange(pad_input(rearrange(output_unpad, 'nnz h d -> nnz (h d)'),
-                                    indices, bsz, q_len),
-                        'b s (h d) -> b s h d', h=nheads)
-    return self.o_proj(rearrange(output,
-                                    'b s h d -> b s (h d)')), None, None
+    return self.o_proj(rearrange(output, "b s h d -> b s (h d)")), None, None
 
 
 # Disable the transformation of the attention mask in LlamaModel as the flash attention
 # requires the attention mask to be the same as the key_padding_mask
-def _prepare_decoder_attention_mask(self, attention_mask, input_shape,
-                                    inputs_embeds, past_key_values_length):
+def _prepare_decoder_attention_mask(
+    self, attention_mask, input_shape, inputs_embeds, past_key_values_length
+):
     # [bsz, seq_len]
     return attention_mask
 
 
 def replace_llama_attn_with_flash_attn():
-    transformers.models.llama.modeling_llama.LlamaModel._prepare_decoder_attention_mask = _prepare_decoder_attention_mask
+    transformers.models.llama.modeling_llama.LlamaModel._prepare_decoder_attention_mask = (
+        _prepare_decoder_attention_mask
+    )
     transformers.models.llama.modeling_llama.LlamaAttention.forward = forward
```

### Comparing `fschat-0.2.2/fastchat/train/train.py` & `fschat-0.2.3/fastchat/train/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,49 +33,45 @@
 @dataclass
 class ModelArguments:
     model_name_or_path: Optional[str] = field(default="facebook/opt-125m")
 
 
 @dataclass
 class DataArguments:
-    data_path: str = field(default=None,
-                           metadata={"help": "Path to the training data."})
+    data_path: str = field(
+        default=None, metadata={"help": "Path to the training data."}
+    )
     lazy_preprocess: bool = False
 
 
 @dataclass
 class TrainingArguments(transformers.TrainingArguments):
     cache_dir: Optional[str] = field(default=None)
     optim: str = field(default="adamw_torch")
     model_max_length: int = field(
         default=512,
         metadata={
-            "help":
-            "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
+            "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
 
 
 local_rank = None
 
 
 def rank0_print(*args):
     if local_rank == 0:
         print(*args)
 
 
-def safe_save_model_for_hf_trainer(trainer: transformers.Trainer,
-                                   output_dir: str):
+def safe_save_model_for_hf_trainer(trainer: transformers.Trainer, output_dir: str):
     """Collects the state dict and dump to disk."""
     state_dict = trainer.model.state_dict()
     if trainer.args.should_save:
-        cpu_state_dict = {
-            key: value.cpu()
-            for key, value in state_dict.items()
-        }
+        cpu_state_dict = {key: value.cpu() for key, value in state_dict.items()}
         del state_dict
         trainer._save(output_dir, state_dict=cpu_state_dict)  # noqa
 
 
 def preprocess(
     sources,
     tokenizer: transformers.PreTrainedTokenizer,
@@ -123,36 +119,38 @@
             parts = rou.split(sep)
             if len(parts) != 2:
                 break
             parts[0] += sep
             round_len = len(tokenizer(rou).input_ids)
             instruction_len = len(tokenizer(parts[0]).input_ids) - 2
 
-            target[cur_len:cur_len+instruction_len] = (
-                IGNORE_TOKEN_ID)
+            target[cur_len : cur_len + instruction_len] = IGNORE_TOKEN_ID
 
-            #rank0_print(tokenizer.decode(target[cur_len+instruction_len:cur_len+round_len]))
+            # rank0_print(tokenizer.decode(target[cur_len+instruction_len:cur_len+round_len]))
 
             cur_len += round_len
         target[cur_len:] = IGNORE_TOKEN_ID
 
         if cur_len < tokenizer.model_max_length:
             if cur_len != total_len:
-                rank0_print(f"WARNING: tokenization mismatch "
-                            f"{cur_len} vs. {total_len}")
-
-    return dict(input_ids=input_ids, labels=targets,
-                attention_mask=input_ids.ne(tokenizer.pad_token_id))
+                rank0_print(
+                    f"WARNING: tokenization mismatch " f"{cur_len} vs. {total_len}"
+                )
+
+    return dict(
+        input_ids=input_ids,
+        labels=targets,
+        attention_mask=input_ids.ne(tokenizer.pad_token_id),
+    )
 
 
 class SupervisedDataset(Dataset):
     """Dataset for supervised fine-tuning."""
 
-    def __init__(self, data_path: str,
-                 tokenizer: transformers.PreTrainedTokenizer):
+    def __init__(self, data_path: str, tokenizer: transformers.PreTrainedTokenizer):
         super(SupervisedDataset, self).__init__()
         rank0_print("Loading data...")
         list_data_dict = json.load(open(data_path, "r"))
 
         rank0_print("Formatting inputs...")
         sources = [example["conversations"] for example in list_data_dict]
         data_dict = preprocess(sources, tokenizer)
@@ -161,24 +159,25 @@
         self.labels = data_dict["labels"]
         self.attention_mask = data_dict["attention_mask"]
 
     def __len__(self):
         return len(self.input_ids)
 
     def __getitem__(self, i) -> Dict[str, torch.Tensor]:
-        return dict(input_ids=self.input_ids[i],
-                    labels=self.labels[i],
-                    attention_mask=self.attention_mask[i])
+        return dict(
+            input_ids=self.input_ids[i],
+            labels=self.labels[i],
+            attention_mask=self.attention_mask[i],
+        )
 
 
 class LazySupervisedDataset(Dataset):
     """Dataset for supervised fine-tuning."""
 
-    def __init__(self, data_path: str,
-                 tokenizer: transformers.PreTrainedTokenizer):
+    def __init__(self, data_path: str, tokenizer: transformers.PreTrainedTokenizer):
         super(LazySupervisedDataset, self).__init__()
         self.tokenizer = tokenizer
 
         rank0_print("Loading data...")
         list_data_dict = json.load(open(data_path, "r"))
 
         rank0_print("Formatting inputs...Skip in lazy mode")
@@ -188,39 +187,41 @@
     def __len__(self):
         return len(self.list_data_dict)
 
     def __getitem__(self, i) -> Dict[str, torch.Tensor]:
         sources = self.list_data_dict[i]
         if isinstance(i, int):
             sources = [sources]
-        data_dict = preprocess([e["conversations"] for e in sources],
-            self.tokenizer)
+        data_dict = preprocess([e["conversations"] for e in sources], self.tokenizer)
         if isinstance(i, int):
-            data_dict = dict(input_ids=data_dict["input_ids"][0],
-                             labels=data_dict["labels"][0],
-                             attention_mask=data_dict["attention_mask"][0])
+            data_dict = dict(
+                input_ids=data_dict["input_ids"][0],
+                labels=data_dict["labels"][0],
+                attention_mask=data_dict["attention_mask"][0],
+            )
         return data_dict
 
 
-def make_supervised_data_module(tokenizer: transformers.PreTrainedTokenizer,
-                                data_args) -> Dict:
+def make_supervised_data_module(
+    tokenizer: transformers.PreTrainedTokenizer, data_args
+) -> Dict:
     """Make dataset and collator for supervised fine-tuning."""
-    dataset_cls = (LazySupervisedDataset
-                   if data_args.lazy_preprocess else SupervisedDataset)
-    train_dataset = dataset_cls(tokenizer=tokenizer,
-                                data_path=data_args.data_path)
-    return dict(train_dataset=train_dataset,
-                eval_dataset=None)
+    dataset_cls = (
+        LazySupervisedDataset if data_args.lazy_preprocess else SupervisedDataset
+    )
+    train_dataset = dataset_cls(tokenizer=tokenizer, data_path=data_args.data_path)
+    return dict(train_dataset=train_dataset, eval_dataset=None)
 
 
 def train():
     global local_rank
 
     parser = transformers.HfArgumentParser(
-        (ModelArguments, DataArguments, TrainingArguments))
+        (ModelArguments, DataArguments, TrainingArguments)
+    )
     model_args, data_args, training_args = parser.parse_args_into_dataclasses()
     local_rank = training_args.local_rank
     model = transformers.AutoModelForCausalLM.from_pretrained(
         model_args.model_name_or_path,
         cache_dir=training_args.cache_dir,
     )
     tokenizer = transformers.AutoTokenizer.from_pretrained(
@@ -228,25 +229,22 @@
         cache_dir=training_args.cache_dir,
         model_max_length=training_args.model_max_length,
         padding_side="right",
         use_fast=False,
     )
     tokenizer.pad_token = tokenizer.unk_token
 
-    data_module = make_supervised_data_module(tokenizer=tokenizer,
-                                              data_args=data_args)
-    trainer = Trainer(model=model,
-                      tokenizer=tokenizer,
-                      args=training_args,
-                      **data_module)
+    data_module = make_supervised_data_module(tokenizer=tokenizer, data_args=data_args)
+    trainer = Trainer(
+        model=model, tokenizer=tokenizer, args=training_args, **data_module
+    )
 
     if list(pathlib.Path(training_args.output_dir).glob("checkpoint-*")):
         trainer.train(resume_from_checkpoint=True)
     else:
         trainer.train()
     trainer.save_state()
-    safe_save_model_for_hf_trainer(trainer=trainer,
-                                   output_dir=training_args.output_dir)
+    safe_save_model_for_hf_trainer(trainer=trainer, output_dir=training_args.output_dir)
 
 
 if __name__ == "__main__":
     train()
```

### Comparing `fschat-0.2.2/fastchat/utils.py` & `fschat-0.2.3/fastchat/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 import json
 
 import requests
 import torch
 
 from fastchat.constants import LOGDIR
 
-server_error_msg = "**NETWORK ERROR DUE TO HIGH TRAFFIC. PLEASE REGENERATE OR REFRESH THIS PAGE.**"
-moderation_msg = "YOUR INPUT VIOLATES OUR CONTENT MODERATION GUIDELINES. PLEASE TRY AGAIN."
+server_error_msg = (
+    "**NETWORK ERROR DUE TO HIGH TRAFFIC. PLEASE REGENERATE OR REFRESH THIS PAGE.**"
+)
+moderation_msg = (
+    "YOUR INPUT VIOLATES OUR CONTENT MODERATION GUIDELINES. PLEASE TRY AGAIN."
+)
 
 handler = None
 
 
 def build_logger(logger_name, logger_filename):
     global handler
 
     formatter = logging.Formatter(
         fmt="%(asctime)s | %(levelname)s | %(name)s | %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     # Set the format of root handlers
     if not logging.getLogger().handlers:
-        logging.basicConfig(level=logging.INFO, encoding='utf-8')
+        logging.basicConfig(level=logging.INFO, encoding="utf-8")
     logging.getLogger().handlers[0].setFormatter(formatter)
 
     # Redirect stdout and stderr to loggers
     stdout_logger = logging.getLogger("stdout")
     stdout_logger.setLevel(logging.INFO)
     sl = StreamToLogger(stdout_logger, logging.INFO)
     sys.stdout = sl
@@ -45,102 +49,111 @@
     logger.setLevel(logging.INFO)
 
     # Add a file handler for all loggers
     if handler is None:
         os.makedirs(LOGDIR, exist_ok=True)
         filename = os.path.join(LOGDIR, logger_filename)
         handler = logging.handlers.TimedRotatingFileHandler(
-            filename, when='D', utc=True)
+            filename, when="D", utc=True
+        )
         handler.setFormatter(formatter)
 
         for name, item in logging.root.manager.loggerDict.items():
             if isinstance(item, logging.Logger):
                 item.addHandler(handler)
 
     return logger
 
 
 class StreamToLogger(object):
     """
     Fake file-like stream object that redirects writes to a logger instance.
     """
+
     def __init__(self, logger, log_level=logging.INFO):
         self.terminal = sys.stdout
         self.logger = logger
         self.log_level = log_level
-        self.linebuf = ''
+        self.linebuf = ""
 
     def __getattr__(self, attr):
         return getattr(self.terminal, attr)
 
     def write(self, buf):
         temp_linebuf = self.linebuf + buf
-        self.linebuf = ''
+        self.linebuf = ""
         for line in temp_linebuf.splitlines(True):
             # From the io.TextIOWrapper docs:
             #   On output, if newline is None, any '\n' characters written
             #   are translated to the system default line separator.
             # By default sys.stdout.write() expects '\n' newlines and then
             # translates them so this is still cross platform.
-            if line[-1] == '\n':
-                encoded_message = line.encode('utf-8', 'ignore').decode('utf-8')
+            if line[-1] == "\n":
+                encoded_message = line.encode("utf-8", "ignore").decode("utf-8")
                 self.logger.log(self.log_level, encoded_message.rstrip())
             else:
                 self.linebuf += line
 
     def flush(self):
-        if self.linebuf != '':
-            encoded_message = self.linebuf.encode('utf-8', 'ignore').decode('utf-8')
+        if self.linebuf != "":
+            encoded_message = self.linebuf.encode("utf-8", "ignore").decode("utf-8")
             self.logger.log(self.log_level, encoded_message.rstrip())
-        self.linebuf = ''
+        self.linebuf = ""
 
 
 def disable_torch_init():
     """
     Disable the redundant torch default initialization to accelerate model creation.
     """
     import torch
+
     setattr(torch.nn.Linear, "reset_parameters", lambda self: None)
     setattr(torch.nn.LayerNorm, "reset_parameters", lambda self: None)
 
 
 def violates_moderation(text):
     """
     Check whether the text violates OpenAI moderation API.
     """
     url = "https://api.openai.com/v1/moderations"
-    headers = {"Content-Type": "application/json",
-               "Authorization": "Bearer " + os.environ["OPENAI_API_KEY"]}
+    headers = {
+        "Content-Type": "application/json",
+        "Authorization": "Bearer " + os.environ["OPENAI_API_KEY"],
+    }
     text = text.replace("\n", "")
     data = "{" + '"input": ' + f'"{text}"' + "}"
     data = data.encode("utf-8")
     try:
         ret = requests.post(url, headers=headers, data=data, timeout=5)
         flagged = ret.json()["results"][0]["flagged"]
     except requests.exceptions.RequestException as e:
         flagged = False
     except KeyError as e:
         flagged = False
 
     return flagged
 
+
 # Flan-t5 trained with HF+FSDP saves corrupted  weights for shared embeddings,
 # Use this function to make sure it can be correctly loaded.
 def clean_flant5_ckpt(ckpt_path):
     index_file = os.path.join(ckpt_path, "pytorch_model.bin.index.json")
     index_json = json.load(open(index_file, "r"))
 
     weightmap = index_json["weight_map"]
 
     share_weight_file = weightmap["shared.weight"]
-    share_weight = torch.load(os.path.join(ckpt_path, share_weight_file))["shared.weight"]
+    share_weight = torch.load(os.path.join(ckpt_path, share_weight_file))[
+        "shared.weight"
+    ]
 
-    for weight_name in ["decoder.embed_tokens.weight","encoder.embed_tokens.weight"]:
+    for weight_name in ["decoder.embed_tokens.weight", "encoder.embed_tokens.weight"]:
         weight_file = weightmap[weight_name]
         weight = torch.load(os.path.join(ckpt_path, weight_file))
         weight[weight_name] = share_weight
         torch.save(weight, os.path.join(ckpt_path, weight_file))
 
+
 def pretty_print_semaphore(semaphore):
     if semaphore is None:
         return "None"
     return f"Semaphore(value={semaphore._value}, locked={semaphore.locked()})"
```

### Comparing `fschat-0.2.2/fschat.egg-info/PKG-INFO` & `fschat-0.2.3/fschat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.2
+Version: 0.2.3
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # FastChat
 An open platform for training, serving, and evaluating large language model based chatbots.
 
 ## Release
 
@@ -183,16 +184,81 @@
 
 
 ## API
 
 ### Huggingface Generation APIs
 See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py)
 
-### OpenAI-compatible RESTful APIs
-Coming soon.
+### OpenAI-compatible RESTful APIs & SDK
+
+(Experimental. We will keep improving the API and SDK.)
+
+#### Chat Completion
+
+Reference: https://platform.openai.com/docs/api-reference/chat/create
+
+Some features/compatibilities to be implemented:
+
+- [ ] streaming
+- [ ] support of some parameters like `top_p`, `presence_penalty`
+- [ ] proper error handling (e.g. model not found)
+- [ ] the return value in the client SDK could be used like a dict
+
+
+**RESTful API Server**
+
+First, launch the controller
+
+```bash
+python3 -m fastchat.serve.controller
+```
+
+Then, launch the model worker(s)
+
+```bash
+python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights
+```
+
+Finally, launch the RESTful API server
+
+```bash
+export FASTCHAT_CONTROLLER_URL=http://localhost:21001
+python3 -m fastchat.serve.api --host localhost --port 8000
+```
+
+Test the API server
+
+```bash
+curl http://localhost:8000/v1/chat/completions \
+  -H "Content-Type: application/json" \
+  -d '{
+    "model": "vicuna-7b-v1.1",
+    "messages": [{"role": "user", "content": "Hello!"}]
+  }'
+```
+
+**Client SDK**
+
+Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://localhost:8000`), you can use the following code to send a request to the API server:
+
+```python
+import os
+from fastchat import client
+
+client.set_baseurl(os.getenv("FASTCHAT_BASEURL"))
+
+completion = client.ChatCompletion.create(
+  model="vicuna-7b-v1.1",
+  messages=[
+    {"role": "user", "content": "Hello!"}
+  ]
+)
+
+print(completion.choices[0].message)
+```
 
 ## Evaluation
 
 Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ### Pipeline Steps
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.2 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.3 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # FastChat An open platform for training, serving, and evaluating large
-language model based chatbots. ## Release
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # FastChat An open platform for training, serving,
+and evaluating large language model based chatbots. ## Release
                            [assets/vicuna_logo.jpeg]
 - ð¥ We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90%
 ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and
 [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif] Join our [Discord]
 (https://discord.gg/h6kCZb72G7) server and follow our [Twitter](https://
 twitter.com/lmsysorg) to get the latest updates. ## Contents - [Install]
 (#install) - [Vicuna Weights](#vicuna-weights) - [Inference with Command Line
@@ -86,23 +86,42 @@
 test message using the following command: ```bash python3 -
 m fastchat.serve.test_message --model-name vicuna-13b ``` #### Launch the
 Gradio web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This
 is the user interface that users will interact with. By following these steps,
 you will be able to serve your models using the web UI. You can open your
 browser and chat with a model now. ## API ### Huggingface Generation APIs See
 [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py) ###
-OpenAI-compatible RESTful APIs Coming soon. ## Evaluation Our AI-enhanced
-evaluation pipeline is based on GPT-4. This section provides a high-level
-summary of the pipeline. For detailed instructions, please refer to the
-[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
-answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
-specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
-models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
-automatically. This step can also be performed manually if the GPT-4 API is not
-available to you. 3. Generate visualization data: Run
+OpenAI-compatible RESTful APIs & SDK (Experimental. We will keep improving the
+API and SDK.) #### Chat Completion Reference: https://platform.openai.com/docs/
+api-reference/chat/create Some features/compatibilities to be implemented: -
+[ ] streaming - [ ] support of some parameters like `top_p`, `presence_penalty`
+- [ ] proper error handling (e.g. model not found) - [ ] the return value in
+the client SDK could be used like a dict **RESTful API Server** First, launch
+the controller ```bash python3 -m fastchat.serve.controller ``` Then, launch
+the model worker(s) ```bash python3 -m fastchat.serve.model_worker --model-name
+'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights ``` Finally, launch the
+RESTful API server ```bash export FASTCHAT_CONTROLLER_URL=http://localhost:
+21001 python3 -m fastchat.serve.api --host localhost --port 8000 ``` Test the
+API server ```bash curl http://localhost:8000/v1/chat/completions \ -
+H "Content-Type: application/json" \ -d '{ "model": "vicuna-7b-v1.1",
+"messages": [{"role": "user", "content": "Hello!"}] }' ``` **Client SDK**
+Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL
+(e.g., `http://localhost:8000`), you can use the following code to send a
+request to the API server: ```python import os from fastchat import client
+client.set_baseurl(os.getenv("FASTCHAT_BASEURL")) completion =
+client.ChatCompletion.create( model="vicuna-7b-v1.1", messages=[ {"role":
+"user", "content": "Hello!"} ] ) print(completion.choices[0].message) ``` ##
+Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
+provides a high-level summary of the pipeline. For detailed instructions,
+please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
+Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
+ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
+Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
+reviews automatically. This step can also be performed manually if the GPT-
+4 API is not available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.2/fschat.egg-info/SOURCES.txt` & `fschat-0.2.3/fschat.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 fastchat/__init__.py
 fastchat/constants.py
 fastchat/conversation.py
 fastchat/utils.py
+fastchat/client/__init__.py
+fastchat/client/api.py
+fastchat/client/test_client.py
 fastchat/data/__init__.py
 fastchat/data/alpaca-converter.py
 fastchat/data/clean_sharegpt.py
 fastchat/data/hardcoded_questions.py
 fastchat/data/inspect.py
 fastchat/data/merge.py
 fastchat/data/optional_clean.py
@@ -19,33 +22,35 @@
 fastchat/eval/generate_webpage_data_from_table.py
 fastchat/eval/get_model_answer.py
 fastchat/eval/qa_baseline_gpt35.py
 fastchat/model/__init__.py
 fastchat/model/apply_delta.py
 fastchat/model/convert_fp16.py
 fastchat/model/make_delta.py
+fastchat/protocol/chat_completion.py
 fastchat/serve/__init__.py
+fastchat/serve/api.py
 fastchat/serve/cacheflow_worker.py
 fastchat/serve/cli.py
 fastchat/serve/compression.py
 fastchat/serve/controller.py
 fastchat/serve/gradio_css.py
 fastchat/serve/gradio_patch.py
 fastchat/serve/gradio_web_server.py
+fastchat/serve/gradio_web_server_multi.py
 fastchat/serve/huggingface_api.py
 fastchat/serve/inference.py
 fastchat/serve/model_worker.py
 fastchat/serve/monkey_patch_non_inplace.py
 fastchat/serve/register_worker.py
 fastchat/serve/serve_chatglm.py
 fastchat/serve/test_message.py
 fastchat/serve/test_throughput.py
 fastchat/train/llama_flash_attn_monkey_patch.py
 fastchat/train/train.py
-fastchat/train/train_flant5.py
 fastchat/train/train_lora.py
 fastchat/train/train_mem.py
 fschat.egg-info/PKG-INFO
 fschat.egg-info/SOURCES.txt
 fschat.egg-info/dependency_links.txt
 fschat.egg-info/requires.txt
 fschat.egg-info/top_level.txt
```

### Comparing `fschat-0.2.2/pyproject.toml` & `fschat-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.2"
+version = "0.2.3"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "accelerate", "fastapi", "gradio==3.23", "markdown2[all]", "numpy",
     "prompt_toolkit>=3.0.0", "requests", "rich>=10.0.0", "sentencepiece",
     "shortuuid", "transformers>=4.28.0", "tokenizers>=0.12.1", "torch",
-    "uvicorn", "wandb",
+    "uvicorn", "wandb", "httpx", "shortuuid", "pydantic",
 ]
 
+[project.optional-dependencies]
+dev = ["black==23.3.0", "pylint==2.8.2"]
+
 [project.urls]
 "Homepage" = "https://github.com/lm-sys/fastchat"
 "Bug Tracker" = "https://github.com/lm-sys/fastchat/issues"
 
 [tool.setuptools.packages.find]
 exclude = ["assets*", "benchmark*", "docs", "dist*", "playground*", "scripts*", "tests*"]
```

