# Comparing `tmp/griptape_flow-0.11.0.tar.gz` & `tmp/griptape_flow-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_flow-0.11.0.tar", max compression
+gzip compressed data, was "griptape_flow-0.12.0.tar", max compression
```

## Comparing `griptape_flow-0.11.0.tar` & `griptape_flow-0.12.0.tar`

### file list

```diff
@@ -1,82 +1,86 @@
--rw-r--r--   0        0        0    11339 2023-01-13 17:13:04.565235 griptape_flow-0.11.0/LICENSE
--rw-r--r--   0        0        0     1166 2023-04-18 23:25:48.177025 griptape_flow-0.11.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_flow-0.11.0/griptape/__init__.py
--rw-r--r--   0        0        0      111 2023-04-09 17:18:51.870440 griptape_flow-0.11.0/griptape/flow/__init__.py
--rw-r--r--   0        0        0      270 2023-04-18 19:55:01.244603 griptape_flow-0.11.0/griptape/flow/artifacts/__init__.py
--rw-r--r--   0        0        0      435 2023-04-18 19:55:01.242320 griptape_flow-0.11.0/griptape/flow/artifacts/error_output.py
--rw-r--r--   0        0        0      154 2023-04-09 19:15:55.901115 griptape_flow-0.11.0/griptape/flow/artifacts/structure_artifact.py
--rw-r--r--   0        0        0      537 2023-04-18 19:55:01.226474 griptape_flow-0.11.0/griptape/flow/artifacts/text_output.py
--rw-r--r--   0        0        0      506 2023-04-18 19:55:01.261464 griptape_flow-0.11.0/griptape/flow/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape_flow-0.11.0/griptape/flow/drivers/memory/__init__.py
--rw-r--r--   0        0        0      597 2023-04-18 19:57:16.468472 griptape_flow-0.11.0/griptape/flow/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0      267 2023-04-18 19:55:01.280287 griptape_flow-0.11.0/griptape/flow/drivers/memory/memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape_flow-0.11.0/griptape/flow/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     1301 2023-04-18 19:55:01.217008 griptape_flow-0.11.0/griptape/flow/drivers/prompt/cohere_prompt_driver.py
--rw-r--r--   0        0        0     3079 2023-04-18 19:55:01.205576 griptape_flow-0.11.0/griptape/flow/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0     1179 2023-04-18 19:55:01.252613 griptape_flow-0.11.0/griptape/flow/drivers/prompt/prompt_driver.py
--rw-r--r--   0        0        0      391 2023-04-18 19:55:01.278802 griptape_flow-0.11.0/griptape/flow/memory/__init__.py
--rw-r--r--   0        0        0      786 2023-04-18 19:55:01.235469 griptape_flow-0.11.0/griptape/flow/memory/buffer_pipeline_memory.py
--rw-r--r--   0        0        0     1889 2023-04-18 19:55:01.257672 griptape_flow-0.11.0/griptape/flow/memory/pipeline_memory.py
--rw-r--r--   0        0        0      383 2023-04-18 19:55:01.209525 griptape_flow-0.11.0/griptape/flow/memory/pipeline_run.py
--rw-r--r--   0        0        0     2111 2023-04-18 19:55:01.208385 griptape_flow-0.11.0/griptape/flow/memory/summary_pipeline_memory.py
--rw-r--r--   0        0        0      131 2023-04-18 19:55:01.256657 griptape_flow-0.11.0/griptape/flow/rules/__init__.py
--rw-r--r--   0        0        0      466 2023-04-18 19:55:01.268024 griptape_flow-0.11.0/griptape/flow/rules/json.py
--rw-r--r--   0        0        0      500 2023-04-18 19:55:01.241045 griptape_flow-0.11.0/griptape/flow/rules/meta.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape_flow-0.11.0/griptape/flow/rules/rule.py
--rw-r--r--   0        0        0     1950 2023-04-18 19:55:01.200752 griptape_flow-0.11.0/griptape/flow/schemas/__init__.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape_flow-0.11.0/griptape/flow/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape_flow-0.11.0/griptape/flow/schemas/drivers/__init__.py
--rw-r--r--   0        0        0      582 2023-04-18 19:55:01.251545 griptape_flow-0.11.0/griptape/flow/schemas/drivers/openai_prompt_driver_schema.py
--rw-r--r--   0        0        0      419 2023-04-18 19:55:01.277469 griptape_flow-0.11.0/griptape/flow/schemas/drivers/prompt_driver_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape_flow-0.11.0/griptape/flow/schemas/memory/__init__.py
--rw-r--r--   0        0        0      380 2023-04-18 19:55:01.207059 griptape_flow-0.11.0/griptape/flow/schemas/memory/buffer_pipeline_memory_schema.py
--rw-r--r--   0        0        0      435 2023-04-18 19:55:01.270971 griptape_flow-0.11.0/griptape/flow/schemas/memory/pipeline_memory_schema.py
--rw-r--r--   0        0        0      384 2023-04-18 19:55:01.287986 griptape_flow-0.11.0/griptape/flow/schemas/memory/pipeline_run_schema.py
--rw-r--r--   0        0        0      478 2023-04-18 19:55:01.224178 griptape_flow-0.11.0/griptape/flow/schemas/memory/summary_pipeline_memory_schema.py
--rw-r--r--   0        0        0     5957 2023-04-18 19:57:16.466957 griptape_flow-0.11.0/griptape/flow/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      274 2023-04-18 19:55:01.236587 griptape_flow-0.11.0/griptape/flow/schemas/rule_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape_flow-0.11.0/griptape/flow/schemas/steps/__init__.py
--rw-r--r--   0        0        0      465 2023-04-18 19:55:01.265253 griptape_flow-0.11.0/griptape/flow/schemas/steps/prompt_step_schema.py
--rw-r--r--   0        0        0      469 2023-04-18 19:55:01.276036 griptape_flow-0.11.0/griptape/flow/schemas/steps/step_schema.py
--rw-r--r--   0        0        0      573 2023-04-18 19:55:01.221861 griptape_flow-0.11.0/griptape/flow/schemas/steps/toolkit_step_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape_flow-0.11.0/griptape/flow/schemas/structures/__init__.py
--rw-r--r--   0        0        0      313 2023-04-18 19:55:01.219205 griptape_flow-0.11.0/griptape/flow/schemas/structures/pipeline_schema.py
--rw-r--r--   0        0        0      515 2023-04-18 19:55:01.263936 griptape_flow-0.11.0/griptape/flow/schemas/structures/structure_schema.py
--rw-r--r--   0        0        0      267 2023-04-18 19:55:01.243469 griptape_flow-0.11.0/griptape/flow/schemas/structures/workflow_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape_flow-0.11.0/griptape/flow/schemas/summarizers/__init__.py
--rw-r--r--   0        0        0      362 2023-04-18 19:55:01.223064 griptape_flow-0.11.0/griptape/flow/schemas/summarizers/prompt_driver_summarizer_schema.py
--rw-r--r--   0        0        0      295 2023-04-18 19:55:01.250458 griptape_flow-0.11.0/griptape/flow/schemas/summarizers/summarizer_schema.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape_flow-0.11.0/griptape/flow/schemas/tokenizers/__init__.py
--rw-r--r--   0        0        0      346 2023-04-18 19:55:01.232892 griptape_flow-0.11.0/griptape/flow/schemas/tokenizers/tiktoken_tokenizer_schema.py
--rw-r--r--   0        0        0      293 2023-04-18 19:55:01.202880 griptape_flow-0.11.0/griptape/flow/steps/__init__.py
--rw-r--r--   0        0        0     1614 2023-04-18 19:55:01.281433 griptape_flow-0.11.0/griptape/flow/steps/prompt_step.py
--rw-r--r--   0        0        0     3644 2023-04-18 19:55:01.239934 griptape_flow-0.11.0/griptape/flow/steps/step.py
--rw-r--r--   0        0        0     6173 2023-04-18 19:55:01.289434 griptape_flow-0.11.0/griptape/flow/steps/tool_substep.py
--rw-r--r--   0        0        0     3085 2023-04-18 19:55:01.253657 griptape_flow-0.11.0/griptape/flow/steps/toolkit_step.py
--rw-r--r--   0        0        0      231 2023-04-18 19:55:01.282463 griptape_flow-0.11.0/griptape/flow/structures/__init__.py
--rw-r--r--   0        0        0     3994 2023-04-18 19:55:01.273804 griptape_flow-0.11.0/griptape/flow/structures/pipeline.py
--rw-r--r--   0        0        0     3837 2023-04-18 19:57:16.471748 griptape_flow-0.11.0/griptape/flow/structures/structure.py
--rw-r--r--   0        0        0     3046 2023-04-18 19:55:01.258871 griptape_flow-0.11.0/griptape/flow/structures/workflow.py
--rw-r--r--   0        0        0      207 2023-04-18 19:55:01.246851 griptape_flow-0.11.0/griptape/flow/summarizers/__init__.py
--rw-r--r--   0        0        0     1014 2023-04-18 19:55:01.213824 griptape_flow-0.11.0/griptape/flow/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      503 2023-04-18 19:55:01.218085 griptape_flow-0.11.0/griptape/flow/summarizers/summarizer.py
--rw-r--r--   0        0        0     1610 2023-04-18 17:19:47.830308 griptape_flow-0.11.0/griptape/flow/templates/prompts/context.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape_flow-0.11.0/griptape/flow/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-03-19 16:50:11.402408 griptape_flow-0.11.0/griptape/flow/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape_flow-0.11.0/griptape/flow/templates/prompts/run_context.j2
--rw-r--r--   0        0        0      118 2023-03-19 16:50:11.402719 griptape_flow-0.11.0/griptape/flow/templates/prompts/steps/prompt.j2
--rw-r--r--   0        0        0      175 2023-04-18 17:15:05.553494 griptape_flow-0.11.0/griptape/flow/templates/prompts/steps/tool/substep.j2
--rw-r--r--   0        0        0       64 2023-03-07 16:53:11.943798 griptape_flow-0.11.0/griptape/flow/templates/prompts/steps/tool/substeps.j2
--rw-r--r--   0        0        0      174 2023-04-18 17:15:43.411012 griptape_flow-0.11.0/griptape/flow/templates/prompts/steps/tool/tool.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape_flow-0.11.0/griptape/flow/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      255 2023-04-18 17:19:47.832750 griptape_flow-0.11.0/griptape/flow/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-03-19 16:50:11.403504 griptape_flow-0.11.0/griptape/flow/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      578 2023-04-18 19:55:01.283568 griptape_flow-0.11.0/griptape/flow/utils/__init__.py
--rw-r--r--   0        0        0      944 2023-04-18 19:55:01.227759 griptape_flow-0.11.0/griptape/flow/utils/cohere_tokenizer.py
--rw-r--r--   0        0        0      530 2023-04-18 19:55:01.248012 griptape_flow-0.11.0/griptape/flow/utils/conversation.py
--rw-r--r--   0        0        0     1252 2023-04-18 19:57:16.461999 griptape_flow-0.11.0/griptape/flow/utils/j2.py
--rw-r--r--   0        0        0     1526 2023-04-18 19:55:01.255687 griptape_flow-0.11.0/griptape/flow/utils/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      677 2023-04-16 17:11:20.543342 griptape_flow-0.11.0/griptape/flow/utils/tokenizer.py
--rw-r--r--   0        0        0      683 2023-04-18 16:33:49.091358 griptape_flow-0.11.0/griptape/flow/utils/tool_loader.py
--rw-r--r--   0        0        0      802 2023-04-18 23:07:49.593883 griptape_flow-0.11.0/pyproject.toml
--rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 griptape_flow-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-01-13 17:13:04.565235 griptape_flow-0.12.0/LICENSE
+-rw-r--r--   0        0        0     1294 2023-04-19 17:39:18.518767 griptape_flow-0.12.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:39:51.796323 griptape_flow-0.12.0/griptape/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-09 17:18:51.870440 griptape_flow-0.12.0/griptape/flow/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-18 19:55:01.244603 griptape_flow-0.12.0/griptape/flow/artifacts/__init__.py
+-rw-r--r--   0        0        0      435 2023-04-18 19:55:01.242320 griptape_flow-0.12.0/griptape/flow/artifacts/error_output.py
+-rw-r--r--   0        0        0      154 2023-04-09 19:15:55.901115 griptape_flow-0.12.0/griptape/flow/artifacts/structure_artifact.py
+-rw-r--r--   0        0        0      550 2023-04-20 15:52:25.879038 griptape_flow-0.12.0/griptape/flow/artifacts/text_output.py
+-rw-r--r--   0        0        0      787 2023-04-20 15:32:47.491029 griptape_flow-0.12.0/griptape/flow/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape_flow-0.12.0/griptape/flow/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      597 2023-04-18 19:57:16.468472 griptape_flow-0.12.0/griptape/flow/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0      267 2023-04-18 19:55:01.280287 griptape_flow-0.12.0/griptape/flow/drivers/memory/memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape_flow-0.12.0/griptape/flow/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     1306 2023-04-19 21:10:23.701857 griptape_flow-0.12.0/griptape/flow/drivers/prompt/cohere_prompt_driver.py
+-rw-r--r--   0        0        0     1949 2023-04-20 20:45:17.813913 griptape_flow-0.12.0/griptape/flow/drivers/prompt/hugging_face_hub_prompt_driver.py
+-rw-r--r--   0        0        0     1714 2023-04-20 21:03:31.033302 griptape_flow-0.12.0/griptape/flow/drivers/prompt/hugging_face_pipeline_prompt_driver.py
+-rw-r--r--   0        0        0     3084 2023-04-19 21:10:23.672348 griptape_flow-0.12.0/griptape/flow/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0     1192 2023-04-20 15:52:25.880934 griptape_flow-0.12.0/griptape/flow/drivers/prompt/prompt_driver.py
+-rw-r--r--   0        0        0      391 2023-04-18 19:55:01.278802 griptape_flow-0.12.0/griptape/flow/memory/__init__.py
+-rw-r--r--   0        0        0      786 2023-04-18 19:55:01.235469 griptape_flow-0.12.0/griptape/flow/memory/buffer_pipeline_memory.py
+-rw-r--r--   0        0        0     1889 2023-04-18 19:55:01.257672 griptape_flow-0.12.0/griptape/flow/memory/pipeline_memory.py
+-rw-r--r--   0        0        0      383 2023-04-18 19:55:01.209525 griptape_flow-0.12.0/griptape/flow/memory/pipeline_run.py
+-rw-r--r--   0        0        0     2111 2023-04-18 19:55:01.208385 griptape_flow-0.12.0/griptape/flow/memory/summary_pipeline_memory.py
+-rw-r--r--   0        0        0      131 2023-04-18 19:55:01.256657 griptape_flow-0.12.0/griptape/flow/rules/__init__.py
+-rw-r--r--   0        0        0      466 2023-04-18 19:55:01.268024 griptape_flow-0.12.0/griptape/flow/rules/json.py
+-rw-r--r--   0        0        0      500 2023-04-18 19:55:01.241045 griptape_flow-0.12.0/griptape/flow/rules/meta.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape_flow-0.12.0/griptape/flow/rules/rule.py
+-rw-r--r--   0        0        0     1950 2023-04-18 19:55:01.200752 griptape_flow-0.12.0/griptape/flow/schemas/__init__.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape_flow-0.12.0/griptape/flow/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape_flow-0.12.0/griptape/flow/schemas/drivers/__init__.py
+-rw-r--r--   0        0        0      582 2023-04-18 19:55:01.251545 griptape_flow-0.12.0/griptape/flow/schemas/drivers/openai_prompt_driver_schema.py
+-rw-r--r--   0        0        0      419 2023-04-18 19:55:01.277469 griptape_flow-0.12.0/griptape/flow/schemas/drivers/prompt_driver_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069641 griptape_flow-0.12.0/griptape/flow/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-18 19:55:01.207059 griptape_flow-0.12.0/griptape/flow/schemas/memory/buffer_pipeline_memory_schema.py
+-rw-r--r--   0        0        0      435 2023-04-18 19:55:01.270971 griptape_flow-0.12.0/griptape/flow/schemas/memory/pipeline_memory_schema.py
+-rw-r--r--   0        0        0      384 2023-04-18 19:55:01.287986 griptape_flow-0.12.0/griptape/flow/schemas/memory/pipeline_run_schema.py
+-rw-r--r--   0        0        0      478 2023-04-18 19:55:01.224178 griptape_flow-0.12.0/griptape/flow/schemas/memory/summary_pipeline_memory_schema.py
+-rw-r--r--   0        0        0     5957 2023-04-18 19:57:16.466957 griptape_flow-0.12.0/griptape/flow/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      274 2023-04-18 19:55:01.236587 griptape_flow-0.12.0/griptape/flow/schemas/rule_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070339 griptape_flow-0.12.0/griptape/flow/schemas/steps/__init__.py
+-rw-r--r--   0        0        0      465 2023-04-18 19:55:01.265253 griptape_flow-0.12.0/griptape/flow/schemas/steps/prompt_step_schema.py
+-rw-r--r--   0        0        0      469 2023-04-18 19:55:01.276036 griptape_flow-0.12.0/griptape/flow/schemas/steps/step_schema.py
+-rw-r--r--   0        0        0      573 2023-04-18 19:55:01.221861 griptape_flow-0.12.0/griptape/flow/schemas/steps/toolkit_step_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape_flow-0.12.0/griptape/flow/schemas/structures/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-18 19:55:01.219205 griptape_flow-0.12.0/griptape/flow/schemas/structures/pipeline_schema.py
+-rw-r--r--   0        0        0      515 2023-04-18 19:55:01.263936 griptape_flow-0.12.0/griptape/flow/schemas/structures/structure_schema.py
+-rw-r--r--   0        0        0      267 2023-04-18 19:55:01.243469 griptape_flow-0.12.0/griptape/flow/schemas/structures/workflow_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape_flow-0.12.0/griptape/flow/schemas/summarizers/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-18 19:55:01.223064 griptape_flow-0.12.0/griptape/flow/schemas/summarizers/prompt_driver_summarizer_schema.py
+-rw-r--r--   0        0        0      295 2023-04-18 19:55:01.250458 griptape_flow-0.12.0/griptape/flow/schemas/summarizers/summarizer_schema.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.070000 griptape_flow-0.12.0/griptape/flow/schemas/tokenizers/__init__.py
+-rw-r--r--   0        0        0      351 2023-04-19 21:10:23.703816 griptape_flow-0.12.0/griptape/flow/schemas/tokenizers/tiktoken_tokenizer_schema.py
+-rw-r--r--   0        0        0      293 2023-04-18 19:55:01.202880 griptape_flow-0.12.0/griptape/flow/steps/__init__.py
+-rw-r--r--   0        0        0     1614 2023-04-18 19:55:01.281433 griptape_flow-0.12.0/griptape/flow/steps/prompt_step.py
+-rw-r--r--   0        0        0     3644 2023-04-18 19:55:01.239934 griptape_flow-0.12.0/griptape/flow/steps/step.py
+-rw-r--r--   0        0        0     6173 2023-04-18 19:55:01.289434 griptape_flow-0.12.0/griptape/flow/steps/tool_substep.py
+-rw-r--r--   0        0        0     3085 2023-04-18 19:55:01.253657 griptape_flow-0.12.0/griptape/flow/steps/toolkit_step.py
+-rw-r--r--   0        0        0      231 2023-04-18 19:55:01.282463 griptape_flow-0.12.0/griptape/flow/structures/__init__.py
+-rw-r--r--   0        0        0     3994 2023-04-18 19:55:01.273804 griptape_flow-0.12.0/griptape/flow/structures/pipeline.py
+-rw-r--r--   0        0        0     3837 2023-04-18 19:57:16.471748 griptape_flow-0.12.0/griptape/flow/structures/structure.py
+-rw-r--r--   0        0        0     3046 2023-04-18 19:55:01.258871 griptape_flow-0.12.0/griptape/flow/structures/workflow.py
+-rw-r--r--   0        0        0      207 2023-04-18 19:55:01.246851 griptape_flow-0.12.0/griptape/flow/summarizers/__init__.py
+-rw-r--r--   0        0        0     1014 2023-04-18 19:55:01.213824 griptape_flow-0.12.0/griptape/flow/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      503 2023-04-18 19:55:01.218085 griptape_flow-0.12.0/griptape/flow/summarizers/summarizer.py
+-rw-r--r--   0        0        0     1482 2023-04-20 20:01:59.450364 griptape_flow-0.12.0/griptape/flow/templates/prompts/context.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape_flow-0.12.0/griptape/flow/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-03-19 16:50:11.402408 griptape_flow-0.12.0/griptape/flow/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape_flow-0.12.0/griptape/flow/templates/prompts/run_context.j2
+-rw-r--r--   0        0        0      118 2023-03-19 16:50:11.402719 griptape_flow-0.12.0/griptape/flow/templates/prompts/steps/prompt.j2
+-rw-r--r--   0        0        0      175 2023-04-18 17:15:05.553494 griptape_flow-0.12.0/griptape/flow/templates/prompts/steps/tool/substep.j2
+-rw-r--r--   0        0        0       64 2023-03-07 16:53:11.943798 griptape_flow-0.12.0/griptape/flow/templates/prompts/steps/tool/substeps.j2
+-rw-r--r--   0        0        0      174 2023-04-18 17:15:43.411012 griptape_flow-0.12.0/griptape/flow/templates/prompts/steps/tool/tool.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape_flow-0.12.0/griptape/flow/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      255 2023-04-18 17:19:47.832750 griptape_flow-0.12.0/griptape/flow/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-03-19 16:50:11.403504 griptape_flow-0.12.0/griptape/flow/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      403 2023-04-20 15:52:25.874876 griptape_flow-0.12.0/griptape/flow/tokenizers/__init__.py
+-rw-r--r--   0        0        0      730 2023-04-20 15:52:25.871234 griptape_flow-0.12.0/griptape/flow/tokenizers/base_tokenizer.py
+-rw-r--r--   0        0        0      688 2023-04-20 15:52:25.861145 griptape_flow-0.12.0/griptape/flow/tokenizers/cohere_tokenizer.py
+-rw-r--r--   0        0        0      679 2023-04-20 20:31:38.329765 griptape_flow-0.12.0/griptape/flow/tokenizers/hugging_face_tokenizer.py
+-rw-r--r--   0        0        0     1453 2023-04-20 15:52:25.863891 griptape_flow-0.12.0/griptape/flow/tokenizers/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      327 2023-04-19 21:10:23.685938 griptape_flow-0.12.0/griptape/flow/utils/__init__.py
+-rw-r--r--   0        0        0      530 2023-04-18 19:55:01.248012 griptape_flow-0.12.0/griptape/flow/utils/conversation.py
+-rw-r--r--   0        0        0     1265 2023-04-20 15:52:25.866240 griptape_flow-0.12.0/griptape/flow/utils/j2.py
+-rw-r--r--   0        0        0      683 2023-04-18 16:33:49.091358 griptape_flow-0.12.0/griptape/flow/utils/tool_loader.py
+-rw-r--r--   0        0        0      865 2023-04-20 21:06:10.471123 griptape_flow-0.12.0/pyproject.toml
+-rw-r--r--   0        0        0     2430 1970-01-01 00:00:00.000000 griptape_flow-0.12.0/PKG-INFO
```

### Comparing `griptape_flow-0.11.0/LICENSE` & `griptape_flow-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/README.md` & `griptape_flow-0.12.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # griptape-flow
 
 [![Tests](https://github.com/griptape-ai/griptape-flow/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-flow/actions/workflows/tests.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-flow.svg)](https://pypi.python.org/pypi/griptape-flow)
-[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape-flow/)
+[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape_flow/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape-flow** is a Python framework for creating workflow DAGs and pipelines that use large language models (LLMs) such as GPT, Claude, Titan, and Cohere.
 
 **griptape-flow** is part of [griptape](https://github.com/griptape-ai/griptape), a modular Python framework for integrating data, APIs, tools, memory, and chain of thought reasoning into LLMs.
 
 ## Documentation
 
@@ -16,8 +17,8 @@
 - Getting started guides. 
 - Core concepts and design overviews.
 - Examples.
 - Contribution guidelines.
 
 ## License
 
-griptape-flow is available under the Apache 2.0 License.
+griptape-flow is available under the Apache 2.0 License.
```

### Comparing `griptape_flow-0.11.0/griptape/flow/artifacts/text_output.py` & `griptape_flow-0.12.0/griptape/flow/artifacts/text_output.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 from attr import define, field
 from griptape.flow.artifacts import StructureArtifact
-from griptape.flow.utils import TiktokenTokenizer, Tokenizer
+from griptape.flow.tokenizers import TiktokenTokenizer, BaseTokenizer
 
 
 @define(frozen=True)
 class TextOutput(StructureArtifact):
     meta: Optional[any] = field(default=None)
-    tokenizer: Tokenizer = field(default=TiktokenTokenizer(), kw_only=True)
+    tokenizer: BaseTokenizer = field(default=TiktokenTokenizer(), kw_only=True)
 
     def token_count(self) -> Optional[int]:
         if isinstance(self.value, str):
             return self.tokenizer.token_count(self.value)
         else:
             return None
```

### Comparing `griptape_flow-0.11.0/griptape/flow/drivers/memory/disk_memory_driver.py` & `griptape_flow-0.12.0/griptape/flow/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/drivers/prompt/cohere_prompt_driver.py` & `griptape_flow-0.12.0/griptape/flow/drivers/prompt/cohere_prompt_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import cohere
 from attr import define, field, Factory
 from griptape.flow.artifacts import TextOutput
 from griptape.flow.drivers import PromptDriver
-from griptape.flow.utils import CohereTokenizer
+from griptape.flow.tokenizers import CohereTokenizer
 
 
 @define
 class CoherePromptDriver(PromptDriver):
     api_key: str = field(kw_only=True)
     model: str = field(default=CohereTokenizer.DEFAULT_MODEL, kw_only=True)
     client: cohere.Client = field(
```

### Comparing `griptape_flow-0.11.0/griptape/flow/drivers/prompt/openai_prompt_driver.py` & `griptape_flow-0.12.0/griptape/flow/drivers/prompt/openai_prompt_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Optional
 import openai
 from attr import define, field, Factory
 from griptape.flow.artifacts import TextOutput
 from griptape.flow.drivers import PromptDriver
-from griptape.flow.utils import TiktokenTokenizer
+from griptape.flow.tokenizers import TiktokenTokenizer
 
 
 @define
 class OpenAiPromptDriver(PromptDriver):
     api_type: str = field(default=openai.api_type, kw_only=True)
     api_version: Optional[str] = field(default=openai.api_version, kw_only=True)
     api_base: str = field(default=openai.api_base, kw_only=True)
```

### Comparing `griptape_flow-0.11.0/griptape/flow/drivers/prompt/prompt_driver.py` & `griptape_flow-0.12.0/griptape/flow/drivers/prompt/prompt_driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 import logging
 import time
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 from attr import define, field, Factory
-from griptape.flow.utils import Tokenizer
+from griptape.flow.tokenizers import BaseTokenizer
 
 if TYPE_CHECKING:
     from griptape.flow.artifacts import TextOutput
 
 
 @define
 class PromptDriver(ABC):
     max_retries: int = field(default=8, kw_only=True)
     retry_delay: float = field(default=1, kw_only=True)
     type: str = field(default=Factory(lambda self: self.__class__.__name__, takes_self=True), kw_only=True)
     temperature: float = field(default=0.5, kw_only=True)
     model: str
-    tokenizer: Tokenizer
+    tokenizer: BaseTokenizer
 
     def run(self, **kwargs) -> TextOutput:
         for attempt in range(0, self.max_retries + 1):
             try:
                 return self.try_run(**kwargs)
             except Exception as e:
                 logging.error(f"PromptDriver.run attempt {attempt} failed: {e}\nRetrying in {self.retry_delay} seconds")
```

### Comparing `griptape_flow-0.11.0/griptape/flow/memory/buffer_pipeline_memory.py` & `griptape_flow-0.12.0/griptape/flow/memory/buffer_pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/memory/pipeline_memory.py` & `griptape_flow-0.12.0/griptape/flow/memory/pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/memory/summary_pipeline_memory.py` & `griptape_flow-0.12.0/griptape/flow/memory/summary_pipeline_memory.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/schemas/__init__.py` & `griptape_flow-0.12.0/griptape/flow/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/schemas/drivers/openai_prompt_driver_schema.py` & `griptape_flow-0.12.0/griptape/flow/schemas/drivers/openai_prompt_driver_schema.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/schemas/polymorphic_schema.py` & `griptape_flow-0.12.0/griptape/flow/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/schemas/steps/toolkit_step_schema.py` & `griptape_flow-0.12.0/griptape/flow/schemas/steps/toolkit_step_schema.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/schemas/structures/structure_schema.py` & `griptape_flow-0.12.0/griptape/flow/schemas/structures/structure_schema.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/steps/prompt_step.py` & `griptape_flow-0.12.0/griptape/flow/steps/prompt_step.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/steps/step.py` & `griptape_flow-0.12.0/griptape/flow/steps/step.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/steps/tool_substep.py` & `griptape_flow-0.12.0/griptape/flow/steps/tool_substep.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/steps/toolkit_step.py` & `griptape_flow-0.12.0/griptape/flow/steps/toolkit_step.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/structures/pipeline.py` & `griptape_flow-0.12.0/griptape/flow/structures/pipeline.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/structures/structure.py` & `griptape_flow-0.12.0/griptape/flow/structures/structure.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/structures/workflow.py` & `griptape_flow-0.12.0/griptape/flow/structures/workflow.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/summarizers/prompt_driver_summarizer.py` & `griptape_flow-0.12.0/griptape/flow/summarizers/prompt_driver_summarizer.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/templates/prompts/context.j2` & `griptape_flow-0.12.0/griptape/flow/templates/prompts/context.j2`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 {% if tools|length > 0 %}
-You are an assistant that can use tools to answer user questions. To use a tool, follow this format:
+You are an assistant that follows rules and can use tools to answer questions and complete tasks. To use a tool, use this structure:
 
-Input: <original question>
-Thought: <step-by-step thought process about how you can obtain the answer by using tools>
-Action: {"tool": "<tool name>", "action": "<action name>" "value": <action input value based on tool action JSON schema>}
-Observation: <tool response>
-Thought: <step-by-step thought process>
+Input: <original request>
+Thought: <step-by-step thought process about how you can complete the request>
 Action: {"tool": "<tool name>", "action": "<action name>" "value": <action input value based on tool action JSON schema>}
 Observation: <tool response>
-...repeat until you can answer the question
-Thought: I have enough information to answer the original question
-Output: <your final answer>
+...repeat Thought/Action/Observation until you can respond to the original request
+Thought: I have enough information to respond to the original request
+Output: <your final response>
 
 All tool action input JSON is based on the JSON Schema Draft-07 format.
 
 You have access only to the following tools: [{{ tool_names }}]. NEVER make up tools and tool names. If you encounter an error from a tool you should try to fix it. Don't request extra information from the user. If you don't need to use a tool or if you don't know which tool to use, respond like this:
 
-Input: <original question>
-Output: <your final answer>
+Input: <original request>
+Output: <your final response>
 
 # Tool Descriptions
 {% for tool in tools %}
 {{ tool }}
 {% endfor %}
 {% else %}
-You are an assistant who follows rules and answers user questions. Here is the conversation format that I want you to use:
+You are an assistant that follows rules and answers questions. Here is the conversation structure that I want you to use:
 
 Input: <original question>
 Output: <your final answer>
 {% endif %}
 
 {% if rules|length > 0 %}
 When answering questions, follow the following additional rules:
```

### Comparing `griptape_flow-0.11.0/griptape/flow/utils/cohere_tokenizer.py` & `griptape_flow-0.12.0/griptape/flow/tokenizers/cohere_tokenizer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 import cohere
 from attr import define, field
-from griptape.flow.utils import Tokenizer
+from griptape.flow.tokenizers import BaseTokenizer
 
 
 @define(frozen=True)
-class CohereTokenizer(Tokenizer):
+class CohereTokenizer(BaseTokenizer):
     DEFAULT_MODEL = "xlarge"
     MAX_TOKENS = 2048
 
     model: str = field(default=DEFAULT_MODEL, kw_only=True)
-    stop_sequence: str = field(default=Tokenizer.DEFAULT_STOP_SEQUENCE, kw_only=True)
     client: cohere.Client = field(kw_only=True)
 
     @property
     def max_tokens(self) -> int:
         return self.MAX_TOKENS
 
-    def tokens_left(self, text: str) -> int:
-        diff = self.max_tokens - self.token_count(text)
-
-        if diff > 0:
-            return diff
-        else:
-            return 0
-
     def token_count(self, text: str) -> int:
         return len(self.encode(text))
 
     def encode(self, text: str) -> list[int]:
         return self.client.tokenize(text=text).tokens
 
     def decode(self, tokens: list[int]) -> str:
```

### Comparing `griptape_flow-0.11.0/griptape/flow/utils/conversation.py` & `griptape_flow-0.12.0/griptape/flow/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/griptape/flow/utils/j2.py` & `griptape_flow-0.12.0/griptape/flow/utils/j2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from typing import Optional
 from attr import define, field, Factory
 from jinja2 import Environment, FileSystemLoader
-from griptape.flow.utils import TiktokenTokenizer, Tokenizer
+from griptape.flow.tokenizers import TiktokenTokenizer, BaseTokenizer
 import griptape
 
 
 @define(frozen=True)
 class J2:
     template_name: Optional[str] = field(default=None)
     templates_dir: str = field(default=os.path.join(griptape.flow.PACKAGE_ABS_PATH, "templates"), kw_only=True)
-    tokenizer: Tokenizer = field(default=TiktokenTokenizer(), kw_only=True)
+    tokenizer: BaseTokenizer = field(default=TiktokenTokenizer(), kw_only=True)
     environment: Environment = field(
         default=Factory(
             lambda self: Environment(
                 loader=FileSystemLoader(self.templates_dir),
                 trim_blocks=True,
                 lstrip_blocks=True
             ),
```

### Comparing `griptape_flow-0.11.0/griptape/flow/utils/tiktoken_tokenizer.py` & `griptape_flow-0.12.0/griptape/flow/tokenizers/tiktoken_tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from attr import define, field
 import tiktoken
-from griptape.flow.utils import Tokenizer
+from griptape.flow.tokenizers import BaseTokenizer
 
 
 @define(frozen=True)
-class TiktokenTokenizer(Tokenizer):
+class TiktokenTokenizer(BaseTokenizer):
     DEFAULT_MODEL = "gpt-3.5-turbo"
     DEFAULT_ENCODING = "cl100k_base"
     DEFAULT_MAX_TOKENS = 2049
     TOKEN_OFFSET = 8
 
     MODEL_PREFIXES_TO_MAX_TOKENS = {
         "gpt-4-32k": 32768,
@@ -21,15 +21,14 @@
 
     CHAT_API_PREFIXES = [
         "gpt-3.5-turbo",
         "gpt-4"
     ]
 
     model: str = field(default=DEFAULT_MODEL, kw_only=True)
-    stop_sequence: str = field(default=Tokenizer.DEFAULT_STOP_SEQUENCE, kw_only=True)
 
     @property
     def encoding(self) -> tiktoken.Encoding:
         try:
             return tiktoken.encoding_for_model(self.model)
         except KeyError:
             return tiktoken.get_encoding(self.DEFAULT_ENCODING)
```

### Comparing `griptape_flow-0.11.0/griptape/flow/utils/tokenizer.py` & `griptape_flow-0.12.0/griptape/flow/tokenizers/base_tokenizer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from abc import ABC, abstractmethod
-from typing import Optional
+from attr import define, field
 
 
-class Tokenizer(ABC):
+@define
+class BaseTokenizer(ABC):
     DEFAULT_STOP_SEQUENCE = "Observation:"
 
-    model: str
-    stop_sequence: str
+    stop_sequence: str = field(default=DEFAULT_STOP_SEQUENCE, kw_only=True)
 
     @property
     @abstractmethod
     def max_tokens(self) -> int:
         ...
 
     def tokens_left(self, text: str) -> int:
```

### Comparing `griptape_flow-0.11.0/griptape/flow/utils/tool_loader.py` & `griptape_flow-0.12.0/griptape/flow/utils/tool_loader.py`

 * *Files identical despite different names*

### Comparing `griptape_flow-0.11.0/pyproject.toml` & `griptape_flow-0.12.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-flow"
-version = "0.11.0"
+version = "0.12.0"
 description = "Python framework for LLM workflows and pipelines."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-flow"
 
 packages = [
@@ -22,14 +22,17 @@
 jsonschema = ">=4"
 marshmallow = ">=3"
 marshmallow-enum = ">=1.5"
 graphlib = "*"
 tiktoken = ">=0.3"
 rich = ">=13"
 stopit = "*"
+transformers = ">=4"
+huggingface-hub = ">=0.13"
+torch = ">= 2"
 
 [tool.poetry.group.test.dependencies]
 griptape-tools = ">= 0.6.0"
 pytest = "~=7.1"
 pytest-cover = "*"
 twine = ">=4"
```

### Comparing `griptape_flow-0.11.0/PKG-INFO` & `griptape_flow-0.12.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-flow
-Version: 0.11.0
+Version: 0.12.0
 Summary: Python framework for LLM workflows and pipelines.
 Home-page: https://github.com/griptape-ai/griptape-flow
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,32 +12,36 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=22)
 Requires-Dist: cohere (>=4)
 Requires-Dist: graphlib
 Requires-Dist: griptape-core (>=0.9.2)
+Requires-Dist: huggingface-hub (>=0.13)
 Requires-Dist: jinja2 (>=3.1)
 Requires-Dist: jsonschema (>=4)
 Requires-Dist: marshmallow (>=3)
 Requires-Dist: marshmallow-enum (>=1.5)
 Requires-Dist: openai (>=0.27)
 Requires-Dist: python-dotenv (>=0.21)
 Requires-Dist: rich (>=13)
 Requires-Dist: stopit
 Requires-Dist: tiktoken (>=0.3)
+Requires-Dist: torch (>=2)
+Requires-Dist: transformers (>=4)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-flow
 Description-Content-Type: text/markdown
 
 # griptape-flow
 
 [![Tests](https://github.com/griptape-ai/griptape-flow/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-flow/actions/workflows/tests.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/griptape-flow.svg)](https://pypi.python.org/pypi/griptape-flow)
-[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape-flow/)
+[![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io/en/latest/griptape_flow/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/gitbucket/gitbucket/blob/master/LICENSE)
+[![Griptape Discord](https://dcbadge.vercel.app/api/server/gnWRz88eym?compact=true&style=flat)](https://discord.gg/gnWRz88eym)
 
 **griptape-flow** is a Python framework for creating workflow DAGs and pipelines that use large language models (LLMs) such as GPT, Claude, Titan, and Cohere.
 
 **griptape-flow** is part of [griptape](https://github.com/griptape-ai/griptape), a modular Python framework for integrating data, APIs, tools, memory, and chain of thought reasoning into LLMs.
 
 ## Documentation
 
@@ -47,7 +51,8 @@
 - Core concepts and design overviews.
 - Examples.
 - Contribution guidelines.
 
 ## License
 
 griptape-flow is available under the Apache 2.0 License.
+
```

