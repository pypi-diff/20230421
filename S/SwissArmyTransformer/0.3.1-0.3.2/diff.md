# Comparing `tmp/SwissArmyTransformer-0.3.1.tar.gz` & `tmp/SwissArmyTransformer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-z934vhzp/SwissArmyTransformer-0.3.1.tar", last modified: Wed Apr 12 06:44:49 2023, max compression
+gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-gyh69qc3/SwissArmyTransformer-0.3.2.tar", last modified: Fri Apr 21 14:13:42 2023, max compression
```

## Comparing `SwissArmyTransformer-0.3.1.tar` & `SwissArmyTransformer-0.3.2.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.1/LICENSE
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/MANIFEST.in
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9446 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9074 2023-04-12 06:44:14.000000 SwissArmyTransformer-0.3.1/README.md
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9446 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3924 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       65 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-04-12 06:44:49.000000 SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       64 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/requirements.txt
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      179 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23055 2023-04-12 06:10:30.000000 SwissArmyTransformer-0.3.1/sat/arguments.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/data_utils/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/data_utils/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15216 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/data_utils/configure_data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/data_utils/datasets.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1852 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/data_utils/samplers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/generation/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5653 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/magnify.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2899 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4990 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3183 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/generation/utils.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3484 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/helpers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.200191 SwissArmyTransformer-0.3.1/sat/model/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      201 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11487 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/base_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5492 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/model/finetune/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/adapter.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/ffadd.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/lora.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/mixins.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/model/official/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/official/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/bert_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/cait_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11755 2023-04-11 14:19:47.000000 SwissArmyTransformer-0.3.1/sat/model/official/chatglm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7337 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/clip_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9680 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-11 14:26:12.000000 SwissArmyTransformer-0.3.1/sat/model/official/distill_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/dpr_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7364 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/eva2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14109 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3786 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/glm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/gpt2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/gptneo_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/mae_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/roberta_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/t5_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8842 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/vit_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/official/yolos_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/model/position_embedding/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5441 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/model/position_embedding/vision_rotary_embeddings.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    26381 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/model/transformer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/mpu/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1776 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4884 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/initialize.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/layers.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/mappings.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/mpu/utils.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.204191 SwissArmyTransformer-0.3.1/sat/ops/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/ops/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      582 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/ops/layernorm.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/ops/local_attention_function.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/resources/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/resources/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1956 2023-04-11 13:31:52.000000 SwissArmyTransformer-0.3.1/sat/resources/download.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-11 13:31:52.000000 SwissArmyTransformer-0.3.1/sat/resources/urls.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3822 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/tokenization/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.196191 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.208191 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.212191 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/sat/tokenization/glm/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/sat/training/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      109 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23474 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_training.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3432 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/learning_rates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9271 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/training/model_io.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4431 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.1/sat/training/utils.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7479 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/sat/transformer_defaults.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/setup.cfg
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-04-12 06:38:10.000000 SwissArmyTransformer-0.3.1/setup.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-12 06:44:49.216191 SwissArmyTransformer-0.3.1/tests/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-11 14:34:16.000000 SwissArmyTransformer-0.3.1/tests/test_base_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-11 13:52:06.000000 SwissArmyTransformer-0.3.1/tests/test_list_info.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.2/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.041410 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3990 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       65 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-04-21 14:13:42.000000 SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       64 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.2/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      179 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23473 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15251 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1852 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/data_utils/samplers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5653 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.045410 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2899 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4990 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3183 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3484 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.049410 SwissArmyTransformer-0.3.2/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      201 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    11454 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5492 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.049410 SwissArmyTransformer-0.3.2/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/lora.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.049410 SwissArmyTransformer-0.3.2/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    12271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7337 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9680 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7364 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14109 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3786 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8842 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5441 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/model/registry.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    26381 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1776 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4884 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/mappings.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/ops/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      582 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/ops/local_attention_function.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1956 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3822 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.053410 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.037410 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.057410 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.061410 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.061410 SwissArmyTransformer-0.3.2/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.061410 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      109 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23627 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3432 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9271 2023-04-21 14:10:30.000000 SwissArmyTransformer-0.3.2/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4431 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7502 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-04-21 14:12:08.000000 SwissArmyTransformer-0.3.2/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 14:13:42.065410 SwissArmyTransformer-0.3.2/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/tests/test_inference.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.2/tests/test_list_info.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.2/tests/test_train.py
```

### Comparing `SwissArmyTransformer-0.3.1/LICENSE` & `SwissArmyTransformer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/PKG-INFO` & `SwissArmyTransformer-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.1
+Version: 0.3.2
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -14,16 +14,18 @@
 `sat`(`SwissArmyTransformer`) is a flexible and powerful library to develop your own Transformer variants.
 
 `sat` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
 
 `sat` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 
 # Migrate from SwissArmyTransformer 0.2.x to 0.3.x
+0. change the package name from `SwissArmyTransformer` to `sat` when importing, e.g. `from sat import get_args`.
 1. delete all `--sandwich-ln` in you script, use `layernorm-order='sandwich'`.
 2. change order `from_pretrained(args, name) => from_pretrained(name, args)`.
+4. We can directly use `from sat.model import AutoModel;model, args = AutoModel.from_pretrained('roberta-base')` to load model in `model-only` mode, instead of initializing the sat first. 
 
 ## Install
 ```
     pip install SwissArmyTransformer
 ```
 # Features
 
@@ -177,12 +179,12 @@
 
 ## Tutorials 
 TO BE RELEASED SOON...
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
-If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/sat}` to mention us and recommend `sat` to others.
+If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
 
 The tutorial for contributing sat is on the way!
 
 The project is based on (a user of) DeepSpeed, Megatron-LM and Huggingface transformers. Thanks for their awesome work.
```

### Comparing `SwissArmyTransformer-0.3.1/README.md` & `SwissArmyTransformer-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 `sat`(`SwissArmyTransformer`) is a flexible and powerful library to develop your own Transformer variants.
 
 `sat` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
 
 `sat` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 
 # Migrate from SwissArmyTransformer 0.2.x to 0.3.x
+0. change the package name from `SwissArmyTransformer` to `sat` when importing, e.g. `from sat import get_args`.
 1. delete all `--sandwich-ln` in you script, use `layernorm-order='sandwich'`.
 2. change order `from_pretrained(args, name) => from_pretrained(name, args)`.
+4. We can directly use `from sat.model import AutoModel;model, args = AutoModel.from_pretrained('roberta-base')` to load model in `model-only` mode, instead of initializing the sat first. 
 
 ## Install
 ```
     pip install SwissArmyTransformer
 ```
 # Features
 
@@ -165,12 +167,12 @@
 
 ## Tutorials 
 TO BE RELEASED SOON...
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
-If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/sat}` to mention us and recommend `sat` to others.
+If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
 
 The tutorial for contributing sat is on the way!
 
 The project is based on (a user of) DeepSpeed, Megatron-LM and Huggingface transformers. Thanks for their awesome work.
```

### Comparing `SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.1
+Version: 0.3.2
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -14,16 +14,18 @@
 `sat`(`SwissArmyTransformer`) is a flexible and powerful library to develop your own Transformer variants.
 
 `sat` is named after "swiss army knife", meaning that all the models (e.g. BERT, GPT, T5, GLM, CogView, ViT...) **share the same backone code** and cater for versatile usages with some extra light-weight mixins. 
 
 `sat` is powered by `deepspeed-ZeRO` and model parallelism, aiming to provide the best practice for pretraining and finetuning large models (100M\~20B parameters). 
 
 # Migrate from SwissArmyTransformer 0.2.x to 0.3.x
+0. change the package name from `SwissArmyTransformer` to `sat` when importing, e.g. `from sat import get_args`.
 1. delete all `--sandwich-ln` in you script, use `layernorm-order='sandwich'`.
 2. change order `from_pretrained(args, name) => from_pretrained(name, args)`.
+4. We can directly use `from sat.model import AutoModel;model, args = AutoModel.from_pretrained('roberta-base')` to load model in `model-only` mode, instead of initializing the sat first. 
 
 ## Install
 ```
     pip install SwissArmyTransformer
 ```
 # Features
 
@@ -177,12 +179,12 @@
 
 ## Tutorials 
 TO BE RELEASED SOON...
 
 # Citation
 Currently we don't have a paper, so you don't need to formally cite us!~ 
 
-If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/sat}` to mention us and recommend `sat` to others.
+If this project helps your research or engineering, use `\footnote{https://github.com/THUDM/SwissArmyTransformer}` to mention us and recommend `SwissArmyTransformer` to others.
 
 The tutorial for contributing sat is on the way!
 
 The project is based on (a user of) DeepSpeed, Megatron-LM and Huggingface transformers. Thanks for their awesome work.
```

### Comparing `SwissArmyTransformer-0.3.1/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.3.2/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 sat/generation/sampling_strategies/beam_search_strategy.py
 sat/generation/sampling_strategies/iterative_entfilter_strategy.py
 sat/model/__init__.py
 sat/model/base_model.py
 sat/model/cached_autoregressive_model.py
 sat/model/encoder_decoder_model.py
 sat/model/mixins.py
+sat/model/registry.py
 sat/model/transformer.py
 sat/model/finetune/__init__.py
 sat/model/finetune/adapter.py
 sat/model/finetune/ffadd.py
 sat/model/finetune/lora.py
 sat/model/finetune/mlp_head.py
 sat/model/finetune/prompt_tuning.py
@@ -105,8 +106,10 @@
 sat/training/deepspeed_zero0.json
 sat/training/deepspeed_zero1.json
 sat/training/deepspeed_zero2.json
 sat/training/learning_rates.py
 sat/training/model_io.py
 sat/training/utils.py
 tests/test_base_model.py
-tests/test_list_info.py
+tests/test_inference.py
+tests/test_list_info.py
+tests/test_train.py
```

### Comparing `SwissArmyTransformer-0.3.1/sat/arguments.py` & `SwissArmyTransformer-0.3.2/sat/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 
 def add_model_config_args(parser):
     """Model arguments"""
 
     group = parser.add_argument_group('model', 'model configuration')
 
     # --------------- Core hyper-parameters --------------- 
-    group.add_argument('--num-layers', type=int, default=24,
+    group.add_argument('--num-layers', type=int, default=6,
                        help='num of layers')
     group.add_argument('--hidden-size', type=int, default=1024,
                        help='transformer hidden size')
     group.add_argument('--num-attention-heads', type=int, default=16,
                        help='num of transformer attention heads')
-    group.add_argument('--vocab-size', type=int, default=0,
+    group.add_argument('--vocab-size', type=int, default=100,
                        help='vocab size for tokenization. the size of word_embeddings.')
     group.add_argument('--max-sequence-length', type=int, default=512,
                        help='maximum number of position embeddings to use')
     
     # ---------------  Optional hyper-parameters --------------- 
 
     group.add_argument('--layernorm-order', type=str, default='pre',
@@ -454,22 +454,27 @@
     torch.distributed.init_process_group(
         backend=args.distributed_backend,
         world_size=args.world_size, rank=args.rank,
         init_method=init_method)
 
     # Set the model-parallel / data-parallel communicators.
     mpu.initialize_model_parallel(args.model_parallel_size)
-
     # Optional DeepSpeed Activation Checkpointing Features
     if args.deepspeed: 
         deepspeed.init_distributed(
             dist_backend=args.distributed_backend,
             world_size=args.world_size, rank=args.rank, init_method=init_method)
         # It seems that it has no negative influence to configure it even without using checkpointing.  
         deepspeed.checkpointing.configure(mpu, deepspeed_config=args.deepspeed_config, num_checkpoints=args.num_layers)
+    else:
+        # in model-only mode, we don't want to init deepspeed, but we still need to init the rng tracker for model_parallel, just because we save the seed by default when dropout. 
+        from deepspeed.runtime.activation_checkpointing.checkpointing import _CUDA_RNG_STATE_TRACKER, _MODEL_PARALLEL_RNG_TRACKER_NAME
+        _CUDA_RNG_STATE_TRACKER.add(_MODEL_PARALLEL_RNG_TRACKER_NAME, 1) # default seed 1
+
+
     return True
 
 def set_random_seed(seed):
     """Set random seed for reproducability."""
     if seed is not None:
         assert seed > 0
         random.seed(seed)
```

### Comparing `SwissArmyTransformer-0.3.1/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.3.2/sat/data_utils/configure_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,16 @@
         args.val_drop_number = 0
         args.test_last_shape = [1] * world_size
         args.test_drop_number = 0
         return torch.utils.data.DataLoader(
             dataset,
             batch_size=batch_size//world_size,
             num_workers=args.num_workers,
-            pin_memory=True
+            pin_memory=True,
+            collate_fn=collate_fn
             )
 
     sampler = torch.utils.data.SequentialSampler(dataset)
     # drop_last = distributed
     drop_last = False # TODO will always drop last to keep the consistency.
     # or, how to avg in eval last batch?
```

### Comparing `SwissArmyTransformer-0.3.1/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.3.2/sat/data_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.3.2/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.3.2/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.3.2/sat/generation/autoregressive_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.3.2/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/generation/magnify.py` & `SwissArmyTransformer-0.3.2/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/base_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.3.2/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/generation/utils.py` & `SwissArmyTransformer-0.3.2/sat/generation/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/helpers.py` & `SwissArmyTransformer-0.3.2/sat/helpers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/base_model.py` & `SwissArmyTransformer-0.3.2/sat/model/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 import sys
 import math
 import random
 import torch
 import inspect
 import warnings
 import argparse
-
-
+from sat.model.registry import model_registry, MetaModel
 
 from sat.model.transformer import BaseTransformer, standard_attention
 from sat import update_args_with_file
 from sat.training.deepspeed_training import load_checkpoint, get_model
 
 from sat.transformer_defaults import HOOKS_DEFAULT
 from sat.resources import auto_create
@@ -69,15 +68,15 @@
     # def attention_fn(q, k, v, mask, dropout_fn, old_impl=standard_attention, **kw_args):
     #     new_q, new_k, new_v = pre_hack(q, k, v)
     #     attn_result = old_impl(q, k, v, mask, dropout_fn, **kw_args)
     #     attn_result = post_hack(attn_result)
     #     return attn_result
 
 
-class BaseModel(torch.nn.Module):
+class BaseModel(torch.nn.Module, metaclass=MetaModel):
     def __init__(self, args, transformer=None, params_dtype=torch.float, **kwargs):
         super(BaseModel, self).__init__()
         self.mixins = torch.nn.ModuleDict()
         self.collect_hooks_()
         if transformer is not None:
             self.transformer = transformer
         else:
@@ -181,15 +180,15 @@
 
     @classmethod
     def add_model_specific_args(cls, parser):
         # recorded in arguments.py: add_model_config_args
         return parser
 
     @classmethod
-    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', **kwargs):
+    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, **kwargs):
         '''Load a pretrained checkpoint of the current model.
             Args:
                 name: The identifier of the pretrained model.
                 args: NameSpace. will add the loaded args into it. None will create a new model-only one with defaults.
                 path: the parent folder of existing `name` model. Default: SAT_HOME.
                 url: the url of the model. Default: SAT_URL.
                 prefix: the prefix of the checkpoint. Default: ''.
@@ -202,15 +201,16 @@
         else:
             model_path = auto_create(name, path=home_path, url=url)
         # create a new args if not provided
         if args is None:
             args = cls.get_args()
         args = update_args_with_file(args, path=os.path.join(model_path, 'model_config.json'))
         model = get_model(args, cls, **kwargs)
-        load_checkpoint(model, args, load_path=model_path, prefix=prefix)
+        if not build_only:
+            load_checkpoint(model, args, load_path=model_path, prefix=prefix)
         return model, args
     
     @classmethod
     def list_avail_args(cls, print=True):
         '''List all available args of the current model.'''
         parser = argparse.ArgumentParser()
         from sat.arguments import add_model_config_args
@@ -239,15 +239,15 @@
                 setattr(args, k, v)
             else:
                 raise ValueError(f'Unknown arg {k}.')
         return args
 
 class AutoModel():
     @classmethod
-    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', **kwargs):
+    def from_pretrained(cls, name, args=None, *, home_path=None, url=None, prefix='', build_only=False, **kwargs):
         '''Automatically find the class and instantiate it. Auto-download.
             Args:
                 name: The identifier of the pretrained model.
                 args: NameSpace. will add the loaded args into it.
                 path: the parent folder of existing `name` model. Default: SAT_HOME.
                 url: manually specified url for the `name` model.
         '''
@@ -259,22 +259,18 @@
             args = argparse.Namespace() # null, fill later
             null_args = True
         else:
             null_args = False
         args = update_args_with_file(args, path=os.path.join(model_path, 'model_config.json'))
         if not hasattr(args, 'model_class'):
             raise ValueError('model_config.json must have key "model_class" for AutoModel.from_pretrained.')
-        import sat.model
-        if not hasattr(sat.model, args.model_class): 
-            # TODO dynamic loading
-            raise ValueError(f'model_class {args.model_class} not found.')
-        else:
-            model_cls = getattr(sat.model, args.model_class)
+        model_cls = model_registry.get(args.model_class)
         if null_args:
             # fill args with default values, if not provided
             model_default_args = model_cls.get_args()
             for k, v in model_default_args.__dict__.items():
                 if not hasattr(args, k):
                     setattr(args, k, v)
         model = get_model(args, model_cls, **kwargs)
-        load_checkpoint(model, args, load_path=model_path, prefix=prefix)
+        if not build_only:
+            load_checkpoint(model, args, load_path=model_path, prefix=prefix)
         return model, args
```

### Comparing `SwissArmyTransformer-0.3.1/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.3.2/sat/model/cached_autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.3.2/sat/model/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.3.2/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.3.2/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.3.2/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.3.2/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.3.2/sat/model/finetune/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/__init__.py` & `SwissArmyTransformer-0.3.2/sat/model/official/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/bert_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/chatglm_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -168,86 +168,94 @@
 class ChatGLMModel(BaseModel):
     def __init__(self, args, transformer=None, **kwargs):
         super(ChatGLMModel, self).__init__(args, transformer=transformer, activation_func=gelu, **kwargs)
         self.add_mixin("chatglm-final", ChatGLMFinalMixin(args.vocab_size, args.hidden_size))
         self.add_mixin("chatglm-attn", ChatGLMAttnMixin(args.hidden_size, args.num_attention_heads))
         self.add_mixin("chatglm-layer", ChatGLMLayerMixin(args.num_layers))
         self.bos_token_id = args.bos_token_id
+        self.mask_token_id = args.mask_token_id
+        self.gmask_token_id = args.gmask_token_id
+        self.pad_token_id = 3
 
     def position_embedding_forward(self, position_ids, output_cross_layer, **kw_args):
         return None
     
     def forward(self, input_ids, attention_mask=None, position_ids=None, past_key_values=None, **kwargs):
-        if past_key_values is None:
-            attention_mask, position_ids = self.get_inputs(input_ids, attention_mask=attention_mask, position_ids=position_ids)
-        else:
-            input_ids, position_ids = self.only_one_input(input_ids)
-        if attention_mask is None:
-            attention_mask = torch.ones(1, 1, device=input_ids.device)
-        else:
-            attention_mask = attention_mask.to(input_ids.device)
+        attention_mask, position_ids = self.get_inputs(input_ids, attention_mask=attention_mask, position_ids=position_ids, past_key_values=past_key_values, **kwargs)
+        if past_key_values is not None:
+            input_ids = input_ids[:, -1:]
+            position_ids = position_ids[..., -1:]
+            if input_ids.size(0) != 1:
+                attention_mask = attention_mask[:, :, -1:]
         return super().forward(input_ids=input_ids, attention_mask=attention_mask, position_ids=position_ids, past_key_values=past_key_values, **kwargs)
     
-    def get_inputs(self, input_ids, attention_mask=None, position_ids=None):
+    def get_inputs(self, input_ids, attention_mask=None, position_ids=None, past_key_values=None, **kwargs):
         if attention_mask is None:
-            attention_mask = self.get_masks(
-                input_ids=input_ids,
-                device=input_ids.device
-            )
+            if past_key_values is not None and input_ids.size(0) == 1:
+                attention_mask = torch.tensor([[1]], dtype=torch.long, device=input_ids.device)
+            else:
+                attention_mask = self.get_masks(
+                    input_ids=input_ids,
+                    device=input_ids.device, **kwargs
+                )
+        elif attention_mask.dtype is torch.bool:
+            attention_mask = (~attention_mask).long()
         if position_ids is None:
-            MASK, gMASK = 150000, 150001
-            mask_token = MASK if MASK in input_ids else gMASK
-            use_gmask = False if MASK in input_ids else gMASK
+            MASK, gMASK = self.mask_token_id, self.gmask_token_id
+            mask_token = gMASK if gMASK in input_ids else MASK
+            use_gmask = True if gMASK in input_ids else False
 
             mask_positions = [seq.tolist().index(mask_token) for seq in input_ids]
             position_ids = self.get_position_ids(
                 input_ids=input_ids,
                 mask_positions=mask_positions,
                 device=input_ids.device,
-                gmask=use_gmask
+                gmask=use_gmask, **kwargs
             )
         return attention_mask, position_ids
     
-    def only_one_input(self, input_ids):
-        batch_size, seq_length = input_ids.shape
-        MASK, gMASK = 150000, 150001
-        mask_token = MASK if MASK in input_ids else gMASK
-        use_gmask = False if MASK in input_ids else gMASK
-        seqs = input_ids.tolist()
-        mask_positions = [seq.index(mask_token) for seq in seqs]
-        context_lengths = [seq.index(self.bos_token_id) for seq in seqs]
-        last_token = input_ids[:, -1].unsqueeze(-1)
-        position_ids = torch.tensor(
-                [[mask_position, seq_length - context_length] for mask_position, context_length in
-                    zip(mask_positions, context_lengths)], dtype=torch.long, device=input_ids.device).unsqueeze(-1)
-        return last_token, position_ids
+    def get_pad_length(self, seq):
+        l = 0
+        while l < len(seq) and seq[l] == self.pad_token_id:
+            l += 1
+        return l
     
-    def get_masks(self, input_ids, device):
+    def get_masks(self, input_ids, device, **kwargs):
         batch_size, seq_length = input_ids.shape
         context_lengths = [seq.tolist().index(self.bos_token_id) for seq in input_ids]
         attention_mask = torch.ones((batch_size, seq_length, seq_length), device=device)
         attention_mask.tril_()
         for i, context_length in enumerate(context_lengths):
             attention_mask[i, :, :context_length] = 1
+        pad_lengths = [self.get_pad_length(seq.tolist()) for seq in input_ids]
+        for i, pad_length in enumerate(pad_lengths):
+            attention_mask[i, :, :pad_length] = 0
+            attention_mask[i, :pad_length, :] = 0
         attention_mask.unsqueeze_(1)
         # attention_mask = (attention_mask < 0.5).bool()
 
         return attention_mask
 
-    def get_position_ids(self, input_ids, mask_positions, device, gmask=False):
+    def get_position_ids(self, input_ids, mask_positions, device, gmask=False, **kwargs):
         batch_size, seq_length = input_ids.shape
+        pad_lengths = [self.get_pad_length(seq.tolist()) for seq in input_ids]
         context_lengths = [seq.tolist().index(self.bos_token_id) for seq in input_ids]
-        position_ids = torch.arange(seq_length, dtype=torch.long, device=device).expand(batch_size, seq_length)
-        for i, context_length in enumerate(context_lengths):
-            position_ids[i, context_length:] = mask_positions[i]
+        position_ids = [torch.arange(seq_length-pad_length, dtype=torch.long, device=device) for pad_length in pad_lengths]
+        for i, (context_length, pad_length) in enumerate(zip(context_lengths, pad_lengths)):
+            position_ids[i][context_length-pad_length:] = mask_positions[i] - pad_length
         block_position_ids = [torch.cat((
             torch.zeros(context_length, dtype=torch.long, device=device),
             torch.arange(seq_length - context_length, dtype=torch.long, device=device) + 1
         )) for context_length in context_lengths]
         block_position_ids = torch.stack(block_position_ids, dim=0)
+        position_ids = [torch.cat((
+            torch.zeros(pad_length, dtype=torch.long, device=device),
+            range_pos
+        )) for pad_length, range_pos in zip(pad_lengths, position_ids)]
+        position_ids = torch.stack(position_ids, dim=0)
         position_ids = torch.stack((position_ids, block_position_ids), dim=1)
 
         return position_ids
     
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('ChatGLM', 'ChatGLM Configurations')
```

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/eva2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/glm130B_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/glm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/gpt2_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/vit_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.3.2/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.3.2/sat/model/position_embedding/rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.3.2/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.3.2/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/model/transformer.py` & `SwissArmyTransformer-0.3.2/sat/model/transformer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/mpu/__init__.py` & `SwissArmyTransformer-0.3.2/sat/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.3.2/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/mpu/data.py` & `SwissArmyTransformer-0.3.2/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/mpu/initialize.py` & `SwissArmyTransformer-0.3.2/sat/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/mpu/layers.py` & `SwissArmyTransformer-0.3.2/sat/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/mpu/mappings.py` & `SwissArmyTransformer-0.3.2/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/mpu/utils.py` & `SwissArmyTransformer-0.3.2/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/ops/layernorm.py` & `SwissArmyTransformer-0.3.2/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.3.2/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/resources/download.py` & `SwissArmyTransformer-0.3.2/sat/resources/download.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/resources/urls.py` & `SwissArmyTransformer-0.3.2/sat/resources/urls.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.3.2/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.3.2/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.3.2/sat/training/deepspeed_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,22 +171,25 @@
     if hasattr(model, 'disable_untrainable_params'):
         model.disable_untrainable_params() # mark trainable params
 
     param_groups = get_optimizer_param_groups(model)
 
     if args.train_data is not None:
         if args.deepspeed:
+            from packaging import version
             print_rank_0("DeepSpeed is enabled.")
             model, optimizer, _, _ = deepspeed.initialize(
                 model=model,
                 model_parameters=param_groups,
                 args=args,
                 mpu=mpu,
                 dist_init_required=False,
                 config_params=args.deepspeed_config
+                    if version.parse(deepspeed.version) < version.parse("0.9.0")
+                    else None
             )
         else:
             raise ValueError('Currently, we only support training with deepspeed.')
     else:
         optimizer = None
 
     return model, optimizer
```

### Comparing `SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.3.2/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/training/learning_rates.py` & `SwissArmyTransformer-0.3.2/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/training/model_io.py` & `SwissArmyTransformer-0.3.2/sat/training/model_io.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/training/utils.py` & `SwissArmyTransformer-0.3.2/sat/training/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.1/sat/transformer_defaults.py` & `SwissArmyTransformer-0.3.2/sat/transformer_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     dropout_fn = self.attention_dropout if self.training else None
     # Reshape and transpose [b, np, s, hn]
     query_layer = self._transpose_for_scores(mixed_query_layer)
     key_layer = self._transpose_for_scores(mixed_key_layer)
     value_layer = self._transpose_for_scores(mixed_value_layer)
 
-    context_layer = attention_fn(query_layer, key_layer, value_layer, cross_attention_mask, dropout_fn, **kw_args)
+    context_layer = attention_fn(query_layer, key_layer, value_layer, cross_attention_mask, dropout_fn, cross_attention=True, **kw_args)
     context_layer = context_layer.permute(0, 2, 1, 3).contiguous()
     new_context_layer_shape = context_layer.size()[:-2] + (self.hidden_size_per_partition,)
     # [b, s, hp]
     context_layer = context_layer.view(*new_context_layer_shape)
 
     # Output. [b, s, h]
     output = self.dense(context_layer)
@@ -177,8 +177,8 @@
     'attention_forward': attention_forward_default,
     'cross_attention_forward': cross_attention_forward_default,
     'mlp_forward': mlp_forward_default,
     'word_embedding_forward': word_embedding_forward_default,
     'position_embedding_forward': position_embedding_forward_default,
     'final_forward': final_forward_default,
     'layer_forward': layer_forward_default
-}
+}
```

### Comparing `SwissArmyTransformer-0.3.1/setup.py` & `SwissArmyTransformer-0.3.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.3.1',
+    version='0.3.2',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.3.1/tests/test_base_model.py` & `SwissArmyTransformer-0.3.2/tests/test_base_model.py`

 * *Files identical despite different names*

