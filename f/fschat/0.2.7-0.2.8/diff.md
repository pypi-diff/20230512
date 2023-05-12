# Comparing `tmp/fschat-0.2.7.tar.gz` & `tmp/fschat-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.7.tar", last modified: Mon May  8 14:34:56 2023, max compression
+gzip compressed data, was "fschat-0.2.8.tar", last modified: Fri May 12 09:29:50 2023, max compression
```

## Comparing `fschat-0.2.7.tar` & `fschat-0.2.8.tar`

### file list

```diff
@@ -1,80 +1,77 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.7/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 14:34:56.836340 fschat-0.2.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15049 2023-05-08 10:26:52.000000 fschat-0.2.7/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-08 14:31:24.000000 fschat-0.2.7/fastchat/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4067 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/client/openai_api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14198 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-05-05 11:09:54.000000 fschat-0.2.7/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-05-05 11:09:54.000000 fschat-0.2.7/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-05 11:09:54.000000 fschat-0.2.7/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.7/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.7/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3447 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-05-08 06:48:06.000000 fschat-0.2.7/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/model/apply_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-05-08 14:31:24.000000 fschat-0.2.7/fastchat/model/chatglm_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/make_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14980 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/model_adapter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2772 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/model_registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      996 2023-05-08 14:31:24.000000 fschat-0.2.7/fastchat/model/rwkv_model.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/protocol/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/protocol/openai_api_protocol.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11456 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5497 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11809 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14370 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/gradio_block_arena_anony.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14209 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/gradio_block_arena_named.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20317 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6239 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/gradio_web_server_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1796 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7980 2023-05-08 14:15:06.000000 fschat-0.2.7/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10911 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/model_worker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/serve/monitor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5413 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/basic_stats.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5116 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/clean_battle_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8275 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/elo_analysis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6919 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/monitor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12369 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/openai_api_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2442 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8670 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/train/train.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14619 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/train/train_flant5.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7107 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2047 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-05-08 14:31:24.000000 fschat-0.2.7/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-08 14:34:56.836340 fschat-0.2.7/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-05-08 13:54:24.000000 fschat-0.2.7/tests/test_openai_client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.8/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15741 2023-05-12 09:29:50.769843 fschat-0.2.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15247 2023-05-12 09:23:49.000000 fschat-0.2.8/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.757843 fschat-0.2.8/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-12 09:29:43.000000 fschat-0.2.8/fastchat/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      739 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15513 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.761843 fschat-0.2.8/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-05-05 11:09:54.000000 fschat-0.2.8/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-05-05 11:09:54.000000 fschat-0.2.8/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      939 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/data/inspect_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.8/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.8/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3447 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.761843 fschat-0.2.8/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-05-08 06:48:06.000000 fschat-0.2.8/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/model/apply_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2471 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/model/chatglm_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/make_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15843 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/model/model_adapter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3002 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/model/model_registry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      996 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/model/rwkv_model.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/protocol/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4377 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/protocol/openai_api_protocol.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11747 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5596 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11883 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14791 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/gradio_block_arena_anony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14209 2023-05-12 07:21:21.000000 fschat-0.2.8/fastchat/serve/gradio_block_arena_named.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21945 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/gradio_web_server_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1796 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9248 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12405 2023-05-12 09:27:57.000000 fschat-0.2.8/fastchat/serve/model_worker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.765843 fschat-0.2.8/fastchat/serve/monitor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5594 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/basic_stats.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5609 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/clean_battle_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8700 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/elo_analysis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7159 2023-05-12 08:32:11.000000 fschat-0.2.8/fastchat/serve/monitor/monitor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22422 2023-05-12 08:58:36.000000 fschat-0.2.8/fastchat/serve/openai_api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.8/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2442 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8670 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/train/train.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14619 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/train/train_flant5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.8/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7107 2023-05-12 07:11:10.000000 fschat-0.2.8/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15741 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1984 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-12 09:29:50.000000 fschat-0.2.8/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-05-12 09:29:43.000000 fschat-0.2.8/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-12 09:29:50.769843 fschat-0.2.8/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-12 09:29:50.769843 fschat-0.2.8/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1285 2023-05-12 08:58:36.000000 fschat-0.2.8/tests/test_openai_sdk.py
```

### Comparing `fschat-0.2.7/LICENSE` & `fschat-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/PKG-INFO` & `fschat-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.7
+Version: 0.2.8
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # FastChat
 | [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) |
 
 FastChat is an open platform for training, serving, and evaluating large language model based chatbots. The core features include:
 - The weights, training code, and evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5).
-- A distributed multi-model serving system with Web UI and OpenAI-Compatible RESTful APIs.
+- A distributed multi-model serving system with Web UI and OpenAI-compatible RESTful APIs.
 
 ## News
 - [2023/05] 🔥 We introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
 - [2023/04] We released **FastChat-T5** compatible with commercial usage. Check out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org).
 - [2023/03] We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
@@ -119,19 +119,20 @@
 
 #### Supported Models
 The following models are tested:
 - Vicuna, Alpaca, LLaMA, Koala
 - [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
 - [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
+- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
+- [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
-- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
@@ -221,15 +222,16 @@
 - You can also launch a multi-tab gradio server, which includes the Chatbot Arena tabs.
 ```bash
 python3 -m fastchat.serve.gradio_web_server_multi
 ```
 
 ## API
 ### OpenAI-Compatible RESTful APIs & SDK
-FastChat provides OpenAI-Compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+FastChat provides OpenAI-compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+The FastChat server is compatible with both [openai-python](https://github.com/openai/openai-python) library and cURL commands.
 See [docs/openai_api.md](docs/openai_api.md).
 
 ### Hugging Face Generation APIs
 See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py).
 
 ## Evaluation
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.7 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.8 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
 [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
 h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) | FastChat is an open
 platform for training, serving, and evaluating large language model based
 chatbots. The core features include: - The weights, training code, and
 evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5). - A
-distributed multi-model serving system with Web UI and OpenAI-Compatible
+distributed multi-model serving system with Web UI and OpenAI-compatible
 RESTful APIs. ## News - [2023/05] ð¥ We introduced **Chatbot Arena** for
 battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-
 03-arena) and [demo](https://arena.lmsys.org). - [2023/04] We released
 **FastChat-T5** compatible with commercial usage. Check out the [weights]
 (#fastchat-t5) and [demo](https://chat.lmsys.org). - [2023/03] We released
 **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**.
 Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://
@@ -62,56 +62,57 @@
 with Command Line Interface (Experimental Feature: You can specify `--style
 rich` to enable rich text output and better text streaming quality for some
 non-ASCII content. This may not work properly on certain terminals.) [assets/
 screenshot_cli.png] #### Supported Models The following models are tested: -
 Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0](https://
 huggingface.co/lmsys/fastchat-t5) - [BlinkDL/RWKV-4-Raven](https://
 huggingface.co/BlinkDL/rwkv-4-raven) - [databricks/dolly-v2-12b](https://
-huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
-[StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
-stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
-chatglm-6b) - [FreedomIntelligence/phoenix-inst-chat-7b](https://
-huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) #### Single GPU The
-command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU
-memory for Vicuna-7B. See the "No Enough Memory" section below if you do not
-have enough memory. Replace `/path/to/model/weights` with the a local folder or
-a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-model/weights ``` #### Multiple GPUs You can use model parallelism to aggregate
-GPU memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
-CPU Only This runs on the CPU only and does not require GPU. It requires around
-60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
-``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
-cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
-`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
-2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
-No Enough Memory If you do not have enough memory, you can enable 8-bit
-compression by adding `--load-8bit` to commands above. This can reduce memory
-usage by around half with slightly degraded model quality. It is compatible
-with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
-on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
-addition to that, you can add `--cpu-offloading` to commands above to offload
-weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
-compression to be enabled and the bitsandbytes package to be installed, which
-is only available on linux operating systems. #### More Platforms - [MLC LLM]
-(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
-tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
-and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
-[assets/screenshot_gui.png] To serve using the web UI, you need three main
-components: web servers that interface with users, model workers that host one
-or more models, and a controller to coordinate the webserver and model workers.
-You can learn more about the architecture [here](docs/server_arch.md). Here are
-the commands to follow in your terminal: #### Launch the controller ```bash
-python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker(s) ```bash python3 -
+huggingface.co/databricks/dolly-v2-12b) - [FreedomIntelligence/phoenix-inst-
+chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) -
+[mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat) -
+[OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/
+oasst-sft-1-pythia-12b) - [project-baize/baize-lora-7B](https://huggingface.co/
+project-baize/baize-lora-7B) - [StabilityAI/stablelm-tuned-alpha-7b](https://
+huggingface.co/stabilityai/stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https:
+//huggingface.co/THUDM/chatglm-6b) #### Single GPU The command below requires
+around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
+See the "No Enough Memory" section below if you do not have enough memory.
+Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights ``` ####
+Multiple GPUs You can use model parallelism to aggregate GPU memory from
+multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --model-
+path /path/to/model/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU
+only and does not require GPU. It requires around 60GB of CPU memory for
+Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/model/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory If
+you do not have enough memory, you can enable 8-bit compression by adding `--
+load-8bit` to commands above. This can reduce memory usage by around half with
+slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
+backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
+4080/T4/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/
+to/model/weights --load-8bit ``` In addition to that, you can add `--cpu-
+offloading` to commands above to offload weights that don't fit on your GPU
+onto the CPU memory. This requires 8-bit compression to be enabled and the
+bitsandbytes package to be installed, which is only available on linux
+operating systems. #### More Platforms - [MLC LLM](https://mlc.ai/mlc-llm/),
+backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler,
+deploys Vicuna natively on phones, consumer-class GPUs and web browsers via
+Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI [assets/
+screenshot_gui.png] To serve using the web UI, you need three main components:
+web servers that interface with users, model workers that host one or more
+models, and a controller to coordinate the webserver and model workers. You can
+learn more about the architecture [here](docs/server_arch.md). Here are the
+commands to follow in your terminal: #### Launch the controller ```bash python3
+-m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". The model worker will register itself to the controller . To ensure that
 your model worker is connected to your controller properly, send a test message
 using the following command: ```bash python3 -m fastchat.serve.test_message --
 model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
 web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
@@ -126,26 +127,28 @@
 m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --
 controller http://localhost:21001 --port 31000 --worker http://localhost:31000
 # worker 1 CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --
 model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --
 port 31001 --worker http://localhost:31001 ``` - You can also launch a multi-
 tab gradio server, which includes the Chatbot Arena tabs. ```bash python3 -
 m fastchat.serve.gradio_web_server_multi ``` ## API ### OpenAI-Compatible
-RESTful APIs & SDK FastChat provides OpenAI-Compatible APIs for its supported
+RESTful APIs & SDK FastChat provides OpenAI-compatible APIs for its supported
 models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
-See [docs/openai_api.md](docs/openai_api.md). ### Hugging Face Generation APIs
-See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py). ##
-Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
-provides a high-level summary of the pipeline. For detailed instructions,
-please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
-Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
-ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
-Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
-reviews automatically. This step can also be performed manually if the GPT-
-4 API is not available to you. 3. Generate visualization data: Run
+The FastChat server is compatible with both [openai-python](https://github.com/
+openai/openai-python) library and cURL commands. See [docs/openai_api.md](docs/
+openai_api.md). ### Hugging Face Generation APIs See [fastchat/serve/
+huggingface_api.py](fastchat/serve/huggingface_api.py). ## Evaluation Our AI-
+enhanced evaluation pipeline is based on GPT-4. This section provides a high-
+level summary of the pipeline. For detailed instructions, please refer to the
+[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
+answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
+specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
+models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
+automatically. This step can also be performed manually if the GPT-4 API is not
+available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.7/README.md` & `fschat-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FastChat
 | [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) |
 
 FastChat is an open platform for training, serving, and evaluating large language model based chatbots. The core features include:
 - The weights, training code, and evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5).
-- A distributed multi-model serving system with Web UI and OpenAI-Compatible RESTful APIs.
+- A distributed multi-model serving system with Web UI and OpenAI-compatible RESTful APIs.
 
 ## News
 - [2023/05] 🔥 We introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
 - [2023/04] We released **FastChat-T5** compatible with commercial usage. Check out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org).
 - [2023/03] We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
@@ -106,19 +106,20 @@
 
 #### Supported Models
 The following models are tested:
 - Vicuna, Alpaca, LLaMA, Koala
 - [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
 - [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
+- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
+- [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
-- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
@@ -208,15 +209,16 @@
 - You can also launch a multi-tab gradio server, which includes the Chatbot Arena tabs.
 ```bash
 python3 -m fastchat.serve.gradio_web_server_multi
 ```
 
 ## API
 ### OpenAI-Compatible RESTful APIs & SDK
-FastChat provides OpenAI-Compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+FastChat provides OpenAI-compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+The FastChat server is compatible with both [openai-python](https://github.com/openai/openai-python) library and cURL commands.
 See [docs/openai_api.md](docs/openai_api.md).
 
 ### Hugging Face Generation APIs
 See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py).
 
 ## Evaluation
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # FastChat | [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://
 arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**]
 (https://twitter.com/lmsysorg) | FastChat is an open platform for training,
 serving, and evaluating large language model based chatbots. The core features
 include: - The weights, training code, and evaluation code for state-of-the-art
 models (e.g., Vicuna, FastChat-T5). - A distributed multi-model serving system
-with Web UI and OpenAI-Compatible RESTful APIs. ## News - [2023/05] ð¥ We
+with Web UI and OpenAI-compatible RESTful APIs. ## News - [2023/05] ð¥ We
 introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post]
 (https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
 - [2023/04] We released **FastChat-T5** compatible with commercial usage. Check
 out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org). - [2023/03]
 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT
 Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo]
 (https://chat.lmsys.org). [assets/demo_narrow.gif] ## Contents - [Install]
@@ -55,56 +55,57 @@
 v1.0 ``` ## Inference with Command Line Interface (Experimental Feature: You
 can specify `--style rich` to enable rich text output and better text streaming
 quality for some non-ASCII content. This may not work properly on certain
 terminals.) [assets/screenshot_cli.png] #### Supported Models The following
 models are tested: - Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0]
 (https://huggingface.co/lmsys/fastchat-t5) - [BlinkDL/RWKV-4-Raven](https://
 huggingface.co/BlinkDL/rwkv-4-raven) - [databricks/dolly-v2-12b](https://
-huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
-[StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
-stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
-chatglm-6b) - [FreedomIntelligence/phoenix-inst-chat-7b](https://
-huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) #### Single GPU The
-command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU
-memory for Vicuna-7B. See the "No Enough Memory" section below if you do not
-have enough memory. Replace `/path/to/model/weights` with the a local folder or
-a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-model/weights ``` #### Multiple GPUs You can use model parallelism to aggregate
-GPU memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
-CPU Only This runs on the CPU only and does not require GPU. It requires around
-60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
-``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
-cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
-`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
-2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
-No Enough Memory If you do not have enough memory, you can enable 8-bit
-compression by adding `--load-8bit` to commands above. This can reduce memory
-usage by around half with slightly degraded model quality. It is compatible
-with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
-on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
-addition to that, you can add `--cpu-offloading` to commands above to offload
-weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
-compression to be enabled and the bitsandbytes package to be installed, which
-is only available on linux operating systems. #### More Platforms - [MLC LLM]
-(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
-tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
-and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
-[assets/screenshot_gui.png] To serve using the web UI, you need three main
-components: web servers that interface with users, model workers that host one
-or more models, and a controller to coordinate the webserver and model workers.
-You can learn more about the architecture [here](docs/server_arch.md). Here are
-the commands to follow in your terminal: #### Launch the controller ```bash
-python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker(s) ```bash python3 -
+huggingface.co/databricks/dolly-v2-12b) - [FreedomIntelligence/phoenix-inst-
+chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) -
+[mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat) -
+[OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/
+oasst-sft-1-pythia-12b) - [project-baize/baize-lora-7B](https://huggingface.co/
+project-baize/baize-lora-7B) - [StabilityAI/stablelm-tuned-alpha-7b](https://
+huggingface.co/stabilityai/stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https:
+//huggingface.co/THUDM/chatglm-6b) #### Single GPU The command below requires
+around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
+See the "No Enough Memory" section below if you do not have enough memory.
+Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights ``` ####
+Multiple GPUs You can use model parallelism to aggregate GPU memory from
+multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --model-
+path /path/to/model/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU
+only and does not require GPU. It requires around 60GB of CPU memory for
+Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/model/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory If
+you do not have enough memory, you can enable 8-bit compression by adding `--
+load-8bit` to commands above. This can reduce memory usage by around half with
+slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
+backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
+4080/T4/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/
+to/model/weights --load-8bit ``` In addition to that, you can add `--cpu-
+offloading` to commands above to offload weights that don't fit on your GPU
+onto the CPU memory. This requires 8-bit compression to be enabled and the
+bitsandbytes package to be installed, which is only available on linux
+operating systems. #### More Platforms - [MLC LLM](https://mlc.ai/mlc-llm/),
+backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler,
+deploys Vicuna natively on phones, consumer-class GPUs and web browsers via
+Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI [assets/
+screenshot_gui.png] To serve using the web UI, you need three main components:
+web servers that interface with users, model workers that host one or more
+models, and a controller to coordinate the webserver and model workers. You can
+learn more about the architecture [here](docs/server_arch.md). Here are the
+commands to follow in your terminal: #### Launch the controller ```bash python3
+-m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". The model worker will register itself to the controller . To ensure that
 your model worker is connected to your controller properly, send a test message
 using the following command: ```bash python3 -m fastchat.serve.test_message --
 model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
 web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
@@ -119,26 +120,28 @@
 m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --
 controller http://localhost:21001 --port 31000 --worker http://localhost:31000
 # worker 1 CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --
 model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --
 port 31001 --worker http://localhost:31001 ``` - You can also launch a multi-
 tab gradio server, which includes the Chatbot Arena tabs. ```bash python3 -
 m fastchat.serve.gradio_web_server_multi ``` ## API ### OpenAI-Compatible
-RESTful APIs & SDK FastChat provides OpenAI-Compatible APIs for its supported
+RESTful APIs & SDK FastChat provides OpenAI-compatible APIs for its supported
 models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
-See [docs/openai_api.md](docs/openai_api.md). ### Hugging Face Generation APIs
-See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py). ##
-Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
-provides a high-level summary of the pipeline. For detailed instructions,
-please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
-Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
-ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
-Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
-reviews automatically. This step can also be performed manually if the GPT-
-4 API is not available to you. 3. Generate visualization data: Run
+The FastChat server is compatible with both [openai-python](https://github.com/
+openai/openai-python) library and cURL commands. See [docs/openai_api.md](docs/
+openai_api.md). ### Hugging Face Generation APIs See [fastchat/serve/
+huggingface_api.py](fastchat/serve/huggingface_api.py). ## Evaluation Our AI-
+enhanced evaluation pipeline is based on GPT-4. This section provides a high-
+level summary of the pipeline. For detailed instructions, please refer to the
+[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
+answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
+specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
+models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
+automatically. This step can also be performed manually if the GPT-4 API is not
+available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.7/fastchat/conversation.py` & `fschat-0.2.8/fastchat/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     ADD_COLON_SINGLE = auto()
     ADD_COLON_TWO = auto()
     NO_COLON_SINGLE = auto()
     BAIZE = auto()
     DOLLY = auto()
     RWKV = auto()
     PHOENIX = auto()
+    NEW_LINE = auto()
 
 
 @dataclasses.dataclass
 class Conversation:
     """A class that keeps all conversation history."""
 
     # The name of this template
@@ -111,14 +112,22 @@
             ret = self.system
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + "<s>" + message + "</s>"
                 else:
                     ret += role + ": " + "<s>"
             return ret
+        elif self.sep_style == SeparatorStyle.NEW_LINE:
+            ret = self.system + self.sep
+            for role, message in self.messages:
+                if message:
+                    ret += role + "\n" + message + self.sep
+                else:
+                    ret += role + "\n"
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.sep_style}")
 
     def append_message(self, role: str, message: str):
         """Append a new message."""
         self.messages.append([role, message])
 
@@ -321,18 +330,24 @@
     )
 )
 
 # RWKV-4-Raven default template
 register_conv_template(
     Conversation(
         name="rwkv",
-        system="",
+        system="The following is a coherent verbose detailed conversation between Bob and Alice.\n\n",
         roles=("Bob", "Alice"),
-        messages=(),
-        offset=0,
+        messages=(
+            ("Bob", "Hi"),
+            (
+                "Alice",
+                "Hi. I am your assistant and I will answer all questions. Please feel free to ask any question and I will always answer it.",
+            ),
+        ),
+        offset=2,
         sep_style=SeparatorStyle.RWKV,
         sep="",
         stop_str="\n\n",
     )
 )
 
 # Buddy default template
@@ -393,14 +408,32 @@
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         sep="\n\n",
     )
 )
 
+# MPT default template
+register_conv_template(
+    Conversation(
+        name="mpt",
+        system="""<|im_start|>system
+- You are a helpful assistant chatbot trained by MosaicML.
+- You answer questions.
+- You are excited to be able to help the user, but will refuse to do anything that could be considered harmful to the user.
+- You are more than just an information source, you are also able to write poetry, short stories, and make jokes.
+""",
+        roles=("<|im_start|>user", "<|im_start|>assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.NEW_LINE,
+        sep="<|im_end|>",
+        stop_token_ids=[50278, 0],
+    )
+)
 
 if __name__ == "__main__":
     conv = get_conv_template("vicuna_v1.1")
     conv.append_message(conv.roles[0], "Hello!")
     conv.append_message(conv.roles[1], "Hi!")
     conv.append_message(conv.roles[0], "How are you?")
     conv.append_message(conv.roles[1], None)
```

### Comparing `fschat-0.2.7/fastchat/data/clean_sharegpt.py` & `fschat-0.2.8/fastchat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/data/hardcoded_questions.py` & `fschat-0.2.8/fastchat/data/hardcoded_questions.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/data/inspect.py` & `fschat-0.2.8/fastchat/data/inspect_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Usage:
-python3 -m fastchat.data.inspect --in sharegpt_20230322_clean_lang_split.json
+python3 -m fastchat.data.inspect_data --in sharegpt_20230322_clean_lang_split.json
 """
 import argparse
 import json
 import random
 
 
 if __name__ == "__main__":
```

### Comparing `fschat-0.2.7/fastchat/data/merge.py` & `fschat-0.2.8/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/data/optional_clean.py` & `fschat-0.2.8/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/data/sample.py` & `fschat-0.2.8/fastchat/data/sample.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/data/split_long_conversation.py` & `fschat-0.2.8/fastchat/data/split_long_conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.8/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.8/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/eval/get_model_answer.py` & `fschat-0.2.8/fastchat/eval/get_model_answer.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.8/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/model/apply_delta.py` & `fschat-0.2.8/fastchat/model/apply_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/model/apply_lora.py` & `fschat-0.2.8/fastchat/model/apply_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/model/compression.py` & `fschat-0.2.8/fastchat/model/compression.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/model/convert_fp16.py` & `fschat-0.2.8/fastchat/model/convert_fp16.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/model/make_delta.py` & `fschat-0.2.8/fastchat/model/make_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/model/model_adapter.py` & `fschat-0.2.8/fastchat/model/model_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 """Model adapter registration."""
 
+import sys
 from typing import List, Optional
 import warnings
-from functools import cache
+if sys.version_info >= (3, 9):
+    from functools import cache
+else:
+    from functools import lru_cache as cache
 
 import torch
 from transformers import (
     AutoConfig,
     AutoModel,
     AutoModelForCausalLM,
     AutoModelForSeq2SeqLM,
@@ -324,14 +328,37 @@
         )
         return model, tokenizer
 
     def get_default_conv_template(self, model_path: str) -> Conversation:
         return get_conv_template("stablelm")
 
 
+class MPTAdapter(BaseAdapter):
+    """The model adapter for mosaicml/mpt-7b-chat"""
+
+    def match(self, model_path: str):
+        return "mpt" in model_path
+
+    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
+        model = AutoModelForCausalLM.from_pretrained(
+            model_path,
+            low_cpu_mem_usage=True,
+            trust_remote_code=True,
+            max_seq_len=8192,
+            **from_pretrained_kwargs,
+        )
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_path, trust_remote_code=True, use_fast=True
+        )
+        return model, tokenizer
+
+    def get_default_conv_template(self, model_path: str) -> Conversation:
+        return get_conv_template("mpt")
+
+
 class BaizeAdapter(BaseAdapter):
     """The model adapter for project-baize/baize-lora-7B"""
 
     def match(self, model_path: str):
         return "baize" in model_path
 
     def get_default_conv_template(self, model_path: str) -> Conversation:
@@ -435,11 +462,11 @@
 register_model_adapter(StableLMAdapter)
 register_model_adapter(BaizeAdapter)
 register_model_adapter(RwkvAdapter)
 register_model_adapter(OpenBuddyAdapter)
 register_model_adapter(PhoenixAdapter)
 register_model_adapter(ChatGPTAdapter)
 register_model_adapter(ClaudeAdapter)
-
+register_model_adapter(MPTAdapter)
 
 # After all adapters, try the default base adapter.
 register_model_adapter(BaseAdapter)
```

### Comparing `fschat-0.2.7/fastchat/model/model_registry.py` & `fschat-0.2.8/fastchat/model/model_registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from collections import namedtuple
+from typing import List
 
 
 ModelInfo = namedtuple("ModelInfo", ["simple_name", "link", "description"])
 
 
 model_info = {}
 
 
-def register_model_info(full_names, simple_name, link, description):
+def register_model_info(
+    full_names: List[str], simple_name: str, link: str, description: str
+):
     info = ModelInfo(simple_name, link, description)
 
     for full_name in full_names:
         model_info[full_name] = info
 
 
-def get_model_info(name):
+def get_model_info(name: str) -> ModelInfo:
     return model_info[name]
 
 
 register_model_info(
     ["gpt-4"], "ChatGPT-4", "https://chat.openai.com/", "ChatGPT-4 by OpenAI"
 )
 register_model_info(
@@ -91,11 +94,17 @@
     ["fastchat-t5-3b"],
     "FastChat-T5",
     "https://huggingface.co/lmsys/fastchat-t5-3b-v1.0",
     "a chat assistant fine-tuned from FLAN-T5 by LMSYS",
 )
 register_model_info(
     ["phoenix-inst-chat-7b"],
-    "Phoenix-7b",
+    "Phoenix-7B",
     "https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b",
     "a multilingual chat assistant fine-tuned from Bloomz to democratize ChatGPT across languages by CUHK(SZ)",
 )
+register_model_info(
+    ["mpt-7b-chat"],
+    "MPT-Chat",
+    "https://www.mosaicml.com/blog/mpt-7b",
+    "a chatbot fine-tuned from MPT-7B by MosaicML",
+)
```

### Comparing `fschat-0.2.7/fastchat/model/monkey_patch_non_inplace.py` & `fschat-0.2.8/fastchat/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/model/rwkv_model.py` & `fschat-0.2.8/fastchat/model/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.8/fastchat/serve/cacheflow_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,15 @@
             cpu_memory=get_cpu_memory(),
         )
         self.running_seq_groups: Dict[int, SequenceGroup] = {}
         self.sequence_group_events: Dict[int, asyncio.Event] = {}
         self.is_server_running = False
 
         if not no_register:
+            time.sleep(30)  # wait for model loading
             self.register_to_controller()
             self.heart_beat_thread = threading.Thread(
                 target=heart_beat_worker, args=(self,)
             )
             self.heart_beat_thread.start()
 
     def register_to_controller(self):
@@ -181,29 +182,40 @@
             self.running_seq_groups[group_id] = seq_group
             self.sequence_group_events[group_id].set()
 
     async def generate_stream(self, params):
         tokenizer = self.tokenizer
         context = params["prompt"]
         temperature = float(params.get("temperature", 1.0))
+        top_p = float(params.get("top_p", 1.0))
         max_new_tokens = min(int(params.get("max_new_tokens", 256)), 1024)
         stop_str = params.get("stop", None)
         echo = params.get("echo", True)
-        params["stop_token_ids"] = params.get("stop_token_ids", None) or []
+        stop_token_ids = params.get("stop_token_ids", None) or []
+        stop_token_ids.append(tokenizer.eos_token_id)
 
         input_ids = tokenizer(context).input_ids
         max_src_len = self.context_len - max_new_tokens - 8
         input_ids = input_ids[-max_src_len:]
 
         # make sampling params in cacheflow
-        sampling_params = SamplingParams.from_dict(params)
-        sampling_params.stop_token_ids.add(tokenizer.eos_token_id)
-        sampling_params.n = 1
-        sampling_params.max_num_steps = max_new_tokens
-        sampling_params.temperature = temperature
+        top_p = max(top_p, 1e-5)
+        if temperature <= 1e-5:
+            top_p = 1.0
+        sampling_params = SamplingParams(
+            n=1,
+            temperature=temperature,
+            top_p=top_p,
+            use_beam_search=False,
+            stop_token_ids=stop_token_ids,
+            max_num_steps=max_new_tokens,
+            num_logprobs=0,
+            context_window_size=None,
+        )
+
         if stop_str is not None:
             sampling_params.stop_str = stop_str
         # we might sample multiple sequences, but in chatbot, this is one
         seqs: List[Sequence] = []
         for _ in range(sampling_params.n):
             seq_id = next(self.seq_counter)
             seq = Sequence(seq_id, input_ids, block_size=self.block_size)
```

### Comparing `fschat-0.2.7/fastchat/serve/cli.py` & `fschat-0.2.8/fastchat/serve/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 
     def prompt_for_output(self, role: str):
         print(f"{role}: ", end="", flush=True)
 
     def stream_output(self, output_stream):
         pre = 0
         for outputs in output_stream:
-            outputs = outputs.strip().split(" ")
-            now = len(outputs) - 1
+            output_text = outputs["text"]
+            output_text = output_text.strip().split(" ")
+            now = len(output_text) - 1
             if now > pre:
-                print(" ".join(outputs[pre:now]), end=" ", flush=True)
+                print(" ".join(output_text[pre:now]), end=" ", flush=True)
                 pre = now
-        print(" ".join(outputs[pre:]), flush=True)
-        return " ".join(outputs)
+        print(" ".join(output_text[pre:]), flush=True)
+        return " ".join(output_text)
 
 
 class RichChatIO(ChatIO):
     def __init__(self):
         self._prompt_session = PromptSession(history=InMemoryHistory())
         self._completer = WordCompleter(
             words=["!exit", "!reset"], pattern=re.compile("$")
@@ -70,39 +71,40 @@
 
         # Create a Live context for updating the console output
         with Live(console=self._console, refresh_per_second=4) as live:
             # Read lines from the stream
             for outputs in output_stream:
                 if not outputs:
                     continue
+                text = outputs["text"]
                 # Render the accumulated text as Markdown
                 # NOTE: this is a workaround for the rendering "unstandard markdown"
                 #  in rich. The chatbots output treat "\n" as a new line for
                 #  better compatibility with real-world text. However, rendering
                 #  in markdown would break the format. It is because standard markdown
                 #  treat a single "\n" in normal text as a space.
                 #  Our workaround is adding two spaces at the end of each line.
                 #  This is not a perfect solution, as it would
                 #  introduce trailing spaces (only) in code block, but it works well
                 #  especially for console output, because in general the console does not
                 #  care about trailing spaces.
                 lines = []
-                for line in outputs.splitlines():
+                for line in text.splitlines():
                     lines.append(line)
                     if line.startswith("```"):
                         # Code block marker - do not add trailing spaces, as it would
                         #  break the syntax highlighting
                         lines.append("\n")
                     else:
                         lines.append("  \n")
                 markdown = Markdown("".join(lines))
                 # Update the Live console output
                 live.update(markdown)
         self._console.print()
-        return outputs
+        return text
 
 
 def main(args):
     if args.gpus:
         if len(args.gpus.split(",")) < args.num_gpus:
             raise ValueError(
                 f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!"
```

### Comparing `fschat-0.2.7/fastchat/serve/controller.py` & `fschat-0.2.8/fastchat/serve/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from fastapi import FastAPI, Request
 from fastapi.responses import StreamingResponse
 import numpy as np
 import requests
 import uvicorn
 
-from fastchat.constants import CONTROLLER_HEART_BEAT_EXPIRATION
+from fastchat.constants import CONTROLLER_HEART_BEAT_EXPIRATION, ErrorCode
 from fastchat.utils import build_logger, server_error_msg
 
 
 logger = build_logger("controller", "controller.log")
 
 
 class DispatchMethod(Enum):
@@ -196,23 +196,23 @@
         for worker_name in to_delete:
             self.remove_worker(worker_name)
 
     def handle_no_worker(params, server_error_msg):
         logger.info(f"no worker: {params['model']}")
         ret = {
             "text": server_error_msg,
-            "error_code": 2,
+            "error_code": ErrorCode.CONTROLLER_NO_WORKER,
         }
         return json.dumps(ret).encode() + b"\0"
 
     def handle_worker_timeout(worker_address, server_error_msg):
         logger.info(f"worker timeout: {worker_address}")
         ret = {
             "text": server_error_msg,
-            "error_code": 3,
+            "error_code": ErrorCode.CONTROLLER_WORKER_TIMEOUT,
         }
         return json.dumps(ret).encode() + b"\0"
 
     def worker_api_generate_stream(self, params):
         worker_addr = self.get_worker_address(params["model"])
         if not worker_addr:
             yield self.handle_no_worker(params, server_error_msg)
```

### Comparing `fschat-0.2.7/fastchat/serve/gradio_block_arena_anony.py` & `fschat-0.2.8/fastchat/serve/gradio_block_arena_anony.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,24 +153,39 @@
     logger.info(f"share (anony). ip: {request.client.host}")
     if state0 is not None and state1 is not None:
         vote_last_response(
             [state0, state1], "share", [model_selector0, model_selector1], request
         )
 
 
-DEFAULT_WEIGHTS = [1.5] * 8 + [1] * 32
+DEFAULT_WEIGHTS = {
+    "gpt-4": 1.5,
+    "gpt-3.5-turbo": 1.5,
+    "claude-v1": 1.5,
+    "vicuna-13b": 1.5,
+    "koala-13b": 1.5,
+    "RWKV-4-Raven-14B": 1.2,
+    "oasst-pythia-12b": 1.2,
+    "mpt-7b-chat": 1.2,
+    "fastchat-t5-3b": 1,
+    "alpaca-13b": 1,
+    "chatglm-6b": 1,
+    "stablelm-tuned-alpha-7b": 0.5,
+    "dolly-v2-12b": 0.5,
+    "llama-13b": 0.1,
+}
 
 
 def add_text(state0, state1, text, request: gr.Request):
     logger.info(f"add_text (anony). ip: {request.client.host}. len: {len(text)}")
     states = [state0, state1]
 
     if states[0] is None:
         assert states[1] is None
-        weights = DEFAULT_WEIGHTS[: len(models)]
+        weights = [DEFAULT_WEIGHTS.get(m, 1.0) for m in models]
         if len(models) > 1:
             weights = weights / np.sum(weights)
             model_left, model_right = np.random.choice(
                 models, size=(2,), p=weights, replace=False
             )
         else:
             model_left = model_right = models[0]
@@ -299,15 +314,15 @@
 - Click "Clear history" to start a new round.
 - [[Blog](https://lmsys.org/blog/2023-05-03-arena/)] [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
 By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data and reserves the right to distribute it under a Creative Commons Attribution (CC-BY) license.** The demo works better on desktop devices with a wide screen.
 
 ### Battle
-Please scroll down and start chatting. You can view a leaderboard of the participated models at the 4th tab above (Leaderboard) or click [this](?leaderboard). We also added ChatGPT and Claude.
+Please scroll down and start chatting. You can view a leaderboard of participating models in the fourth tab above labeled 'Leaderboard' or by clicking [here](?leaderboard). The models include both closed-source models (e.g., ChatGPT) and open-source models (e.g., Vicuna).
 """
 
     states = [gr.State() for _ in range(num_models)]
     model_selectors = [None] * num_models
     chatbots = [None] * num_models
 
     gr.Markdown(notice_markdown, elem_id="notice_markdown")
```

### Comparing `fschat-0.2.7/fastchat/serve/gradio_block_arena_named.py` & `fschat-0.2.8/fastchat/serve/gradio_block_arena_named.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/serve/gradio_css.py` & `fschat-0.2.8/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/serve/gradio_patch.py` & `fschat-0.2.8/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/serve/gradio_web_server.py` & `fschat-0.2.8/fastchat/serve/gradio_web_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 import uuid
 
 import gradio as gr
 import requests
 
 from fastchat.conversation import SeparatorStyle
-from fastchat.constants import LOGDIR, WORKER_API_TIMEOUT
+from fastchat.constants import LOGDIR, WORKER_API_TIMEOUT, ErrorCode
 from fastchat.model.model_adapter import get_conversation_template
 from fastchat.model.model_registry import model_info
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_css import code_highlight_css
 from fastchat.utils import (
     build_logger,
     server_error_msg,
@@ -64,14 +64,45 @@
     models = ret.json()["models"]
     priority = {k: f"___{i:02d}" for i, k in enumerate(model_info)}
     models.sort(key=lambda x: priority.get(x, x))
     logger.info(f"Models: {models}")
     return models
 
 
+def load_demo_refresh_model_list(url_params):
+    models = get_model_list(controller_url)
+    selected_model = models[0] if len(models) > 0 else ""
+    if "model" in url_params:
+        model = url_params["model"]
+        if model in models:
+            selected_model = model
+
+    dropdown_update = gr.Dropdown.update(
+        choices=models, value=selected_model, visible=True
+    )
+
+    state = None
+    return (
+        state,
+        dropdown_update,
+        gr.Chatbot.update(visible=True),
+        gr.Textbox.update(visible=True),
+        gr.Button.update(visible=True),
+        gr.Row.update(visible=True),
+        gr.Accordion.update(visible=True),
+    )
+
+
+def load_demo_reload_model(url_params, request: gr.Request):
+    logger.info(
+        f"load_demo_reload_model. ip: {request.client.host}. params: {url_params}"
+    )
+    return load_demo_refresh_model_list(url_params)
+
+
 def load_demo_single(models, url_params):
     dropdown_update = gr.Dropdown.update(visible=True)
     if "model" in url_params:
         model = url_params["model"]
         if model in models:
             dropdown_update = gr.Dropdown.update(value=model, visible=True)
 
@@ -331,37 +362,43 @@
             if data["error_code"] == 0:
                 output = data["text"].strip()
                 if "vicuna" in model_name:
                     output = post_process_code(output)
                 state.messages[-1][-1] = output + "▌"
                 yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
             else:
-                output = data["text"] + f" (error_code: {data['error_code']})"
+                output = data["text"] + f"\n\n(error_code: {data['error_code']})"
                 state.messages[-1][-1] = output
                 yield (state, state.to_gradio_chatbot()) + (
                     disable_btn,
                     disable_btn,
                     disable_btn,
                     enable_btn,
                     enable_btn,
                 )
                 return
             time.sleep(0.02)
     except requests.exceptions.RequestException as e:
-        state.messages[-1][-1] = server_error_msg + f" (error_code: 4)"
+        state.messages[-1][-1] = (
+            f"{server_error_msg}\n\n"
+            f"(error_code: {ErrorCode.GRADIO_REQUEST_ERROR}, {e})"
+        )
         yield (state, state.to_gradio_chatbot()) + (
             disable_btn,
             disable_btn,
             disable_btn,
             enable_btn,
             enable_btn,
         )
         return
     except Exception as e:
-        state.messages[-1][-1] = server_error_msg + f" (error_code: 5, {e})"
+        state.messages[-1][-1] = (
+            f"{server_error_msg}\n\n"
+            f"(error_code: {ErrorCode.GRADIO_STREAM_UNKNOWN_ERROR}, {e})"
+        )
         yield (state, state.to_gradio_chatbot()) + (
             disable_btn,
             disable_btn,
             disable_btn,
             enable_btn,
             enable_btn,
         )
@@ -569,28 +606,47 @@
                     textbox,
                     send_btn,
                     button_row,
                     parameter_row,
                 ],
                 _js=get_window_url_params_js,
             )
+        elif args.model_list_mode == "reload":
+            demo.load(
+                load_demo_reload_model,
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
+                _js=get_window_url_params_js,
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
     parser.add_argument(
-        "--model-list-mode", type=str, default="once", choices=["once", "reload"]
+        "--model-list-mode",
+        type=str,
+        default="once",
+        choices=["once", "reload"],
+        help="Whether to load the model list once or reload the model list every time.",
     )
     parser.add_argument("--share", action="store_true")
     parser.add_argument(
         "--moderate", action="store_true", help="Enable content moderation"
     )
     parser.add_argument(
         "--add-chatgpt",
```

### Comparing `fschat-0.2.7/fastchat/serve/gradio_web_server_multi.py` & `fschat-0.2.8/fastchat/serve/gradio_web_server_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="0.0.0.0")
     parser.add_argument("--port", type=int)
     parser.add_argument("--controller-url", type=str, default="http://localhost:21001")
     parser.add_argument("--concurrency-count", type=int, default=10)
     parser.add_argument(
-        "--model-list-mode", type=str, default="once", choices=["once", "reload"]
+        "--model-list-mode", type=str, default="once", choices=["once"],
     )
     parser.add_argument("--share", action="store_true")
     parser.add_argument(
         "--moderate", action="store_true", help="Enable content moderation"
     )
     parser.add_argument(
         "--add-chatgpt",
```

### Comparing `fschat-0.2.7/fastchat/serve/huggingface_api.py` & `fschat-0.2.8/fastchat/serve/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/serve/inference.py` & `fschat-0.2.8/fastchat/serve/inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Inference for FastChat models."""
 import abc
 import gc
 import math
-from typing import Optional
+from typing import Iterable, Optional
 import sys
 import warnings
 
 import psutil
 import torch
 from transformers import (
     AutoTokenizer,
@@ -84,14 +84,15 @@
         )[0]
         start_ids = torch.as_tensor(
             [[model.generation_config.decoder_start_token_id]],
             dtype=torch.int64,
             device=device,
         )
 
+    past_key_values = out = None
     for i in range(max_new_tokens):
         if i == 0:
             if model.config.is_encoder_decoder:
                 out = model.decoder(
                     input_ids=start_ids,
                     encoder_hidden_states=encoder_output,
                     use_cache=True,
@@ -156,23 +157,61 @@
 
             output = tokenizer.decode(
                 tmp_output_ids,
                 skip_special_tokens=True,
                 spaces_between_special_tokens=False,
             )
             if stop_str:
-                pos = output.rfind(stop_str, rfind_start)
-                if pos != -1:
-                    output = output[:pos]
-                    stopped = True
-            yield output
+                if isinstance(stop_str, str):
+                    pos = output.rfind(stop_str, rfind_start)
+                    if pos != -1:
+                        output = output[:pos]
+                        stopped = True
+                elif isinstance(stop_str, Iterable):
+                    for each_stop in stop_str:
+                        pos = output.rfind(each_stop, rfind_start)
+                        if pos != -1:
+                            output = output[:pos]
+                            stopped = True
+                            break
+                else:
+                    raise ValueError("Invalid stop field type.")
+
+            yield {
+                "text": output,
+                "usage": {
+                    "prompt_tokens": input_echo_len,
+                    "completion_tokens": i,
+                    "total_tokens": input_echo_len + i,
+                },
+                "finish_reason": None,
+            }
 
         if stopped:
             break
 
+    # finish stream event, which contains finish reason
+    if i == max_new_tokens - 1:
+        finish_reason = "length"
+    elif stopped:
+        finish_reason = "stop"
+    else:
+        finish_reason = None
+
+    yield {
+        "text": output,
+        "usage": {
+            "prompt_tokens": input_echo_len,
+            "completion_tokens": i,
+            "total_tokens": input_echo_len + i,
+        },
+        "finish_reason": finish_reason,
+    }
+
+    # clean
     del past_key_values, out
     gc.collect()
     torch.cuda.empty_cache()
 
 
 class ChatIO(abc.ABC):
     @abc.abstractmethod
```

### Comparing `fschat-0.2.7/fastchat/serve/model_worker.py` & `fschat-0.2.8/fastchat/serve/model_worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         AutoModelForCausalLM,
         LLaMATokenizer,
         AutoModel,
     )
 import torch
 import uvicorn
 
-from fastchat.constants import WORKER_HEART_BEAT_INTERVAL
+from fastchat.constants import WORKER_HEART_BEAT_INTERVAL, ErrorCode
 from fastchat.model.model_adapter import load_model, add_model_args
 from fastchat.model.chatglm_model import chatglm_generate_stream
 from fastchat.serve.inference import generate_stream
 from fastchat.utils import build_logger, server_error_msg, pretty_print_semaphore
 
 GB = 1 << 30
 
@@ -85,14 +85,15 @@
         if hasattr(self.model.config, "max_sequence_length"):
             self.context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self.context_len = self.model.config.max_position_embeddings
         else:
             self.context_len = 2048
 
+        # generate_stream
         is_chatglm = "chatglm" in str(type(self.model)).lower()
         if is_chatglm:
             self.generate_stream_func = chatglm_generate_stream
         else:
             self.generate_stream_func = generate_stream
 
         if not no_register:
@@ -159,101 +160,117 @@
     def get_status(self):
         return {
             "model_names": [self.model_name],
             "speed": 1,
             "queue_length": self.get_queue_length(),
         }
 
+    def count_token(self, params):
+        prompt = params["prompt"]
+        input_ids = self.tokenizer(prompt).input_ids
+        input_echo_len = len(input_ids)
+
+        ret = {
+            "count": input_echo_len,
+            "error_code": 0,
+        }
+        return ret
+
     def generate_stream_gate(self, params):
         try:
             for output in self.generate_stream_func(
                 self.model,
                 self.tokenizer,
                 params,
                 self.device,
                 self.context_len,
                 args.stream_interval,
             ):
                 ret = {
-                    "text": output,
+                    "text": output["text"],
                     "error_code": 0,
                 }
+                if "usage" in output:
+                    ret["usage"] = output["usage"]
+                if "finish_reason" in output:
+                    ret["finish_reason"] = output["finish_reason"]
+                if "logprobs" in output:
+                    ret["logprobs"] = output["logprobs"]
                 yield json.dumps(ret).encode() + b"\0"
-        except torch.cuda.OutOfMemoryError:
+        except torch.cuda.OutOfMemoryError as e:
+            ret = {
+                "text": f"{server_error_msg}\n\n({e})",
+                "error_code": ErrorCode.CUDA_OUT_OF_MEMORY,
+            }
+            yield json.dumps(ret).encode() + b"\0"
+        except (ValueError, RuntimeError) as e:
             ret = {
-                "text": server_error_msg,
-                "error_code": 1,
+                "text": f"{server_error_msg}\n\n({e})",
+                "error_code": ErrorCode.INTERNAL_ERROR,
             }
             yield json.dumps(ret).encode() + b"\0"
 
-    def generate_completion(self, params):
+    def generate_gate(self, params):
         try:
-            input_ids = self.tokenizer([params["prompt"]]).input_ids
-            output_ids = self.model.generate(
-                torch.as_tensor(input_ids).cuda(),
-                do_sample=True,
-                temperature=params["temperature"],
-                max_new_tokens=params["max_tokens"]
-                - 1,  # generate max_new_tokens + 1 tokens
-            )
-            if self.model.config.is_encoder_decoder:
-                output_ids = output_ids[0]
-            else:
-                output_ids = output_ids[0][len(input_ids[0]) :]
-            outputs = self.tokenizer.decode(
-                output_ids,
-                skip_special_tokens=True,
-                spaces_between_special_tokens=False,
-            )
-            completion_tokens = len(self.tokenizer(outputs).input_ids)
-            if completion_tokens >= params["max_tokens"]:
-                finish_reason = "length"
-            else:
-                finish_reason = "stop"
-            return json.dumps(
-                {
-                    "text": outputs,
-                    "finish_reason": finish_reason,
-                    "completion_tokens": completion_tokens,
-                    "prompt_tokens": len(input_ids[0]),
-                }
-            )
-
-        except torch.cuda.OutOfMemoryError:
+            ret = {"text": "", "error_code": 0}
+            for output in self.generate_stream_func(
+                self.model,
+                self.tokenizer,
+                params,
+                self.device,
+                self.context_len,
+                args.stream_interval,
+            ):
+                ret["text"] = output["text"]
+            if "usage" in output:
+                ret["usage"] = output["usage"]
+            if "finish_reason" in output:
+                ret["finish_reason"] = output["finish_reason"]
+            if "logprobs" in output:
+                ret["logprobs"] = output["logprobs"]
+        except torch.cuda.OutOfMemoryError as e:
+            ret = {
+                "text": f"{server_error_msg}\n\n({e})",
+                "error_code": ErrorCode.CUDA_OUT_OF_MEMORY,
+            }
+        except (ValueError, RuntimeError) as e:
             ret = {
-                "text": server_error_msg,
-                "error_code": 1,
+                "text": f"{server_error_msg}\n\n({e})",
+                "error_code": ErrorCode.INTERNAL_ERROR,
             }
-            return json.dumps(ret).encode() + b"\0"
+        return ret
 
     def get_embeddings(self, params):
         try:
             tokenizer = self.tokenizer
             input_ids = tokenizer.encode(params["input"], return_tensors="pt").to(
                 self.device
             )
             model_output = self.model(input_ids, output_hidden_states=True)
             is_chatglm = "chatglm" in str(type(self.model)).lower()
             if is_chatglm:
                 data = (model_output.hidden_states[-1].transpose(0, 1))[0]
             else:
                 data = model_output.hidden_states[-1][0]
             embedding = torch.mean(data, dim=0)
-            return json.dumps(
-                {
-                    "embedding": embedding.tolist(),
-                    "token_num": len(self.tokenizer(params["input"]).input_ids),
-                }
-            )
-        except torch.cuda.OutOfMemoryError:
             ret = {
-                "text": server_error_msg,
-                "error_code": 1,
+                "embedding": embedding.tolist(),
+                "token_num": len(self.tokenizer(params["input"]).input_ids),
+            }
+        except torch.cuda.OutOfMemoryError as e:
+            ret = {
+                "text": f"{server_error_msg}\n\n({e})",
+                "error_code": ErrorCode.CUDA_OUT_OF_MEMORY,
+            }
+        except (ValueError, RuntimeError) as e:
+            ret = {
+                "text": f"{server_error_msg}\n\n({e})",
+                "error_code": ErrorCode.INTERNAL_ERROR,
             }
-            return json.dumps(ret).encode() + b"\0"
+        return ret
 
 
 app = FastAPI()
 
 
 def release_model_semaphore():
     model_semaphore.release()
@@ -278,19 +295,37 @@
     params = await request.json()
     await acquire_model_semaphore()
     generator = worker.generate_stream_gate(params)
     background_tasks = create_background_tasks()
     return StreamingResponse(generator, background=background_tasks)
 
 
+@app.post("/worker_generate")
+async def api_generate(request: Request):
+    params = await request.json()
+    await acquire_model_semaphore()
+    output = worker.generate_gate(params)
+    release_model_semaphore()
+    return JSONResponse(output)
+
+
+@app.post("/worker_generate_completion_stream")
+async def api_generate_completion_stream(request: Request):
+    params = await request.json()
+    await acquire_model_semaphore()
+    generator = worker.generate_stream_gate(params)
+    background_tasks = create_background_tasks()
+    return StreamingResponse(generator, background=background_tasks)
+
+
 @app.post("/worker_generate_completion")
 async def api_generate_completion(request: Request):
     params = await request.json()
     await acquire_model_semaphore()
-    completion = worker.generate_completion(params)
+    completion = worker.generate_gate(params)
     background_tasks = create_background_tasks()
     return JSONResponse(content=completion, background=background_tasks)
 
 
 @app.post("/worker_get_embeddings")
 async def api_get_embeddings(request: Request):
     params = await request.json()
@@ -301,14 +336,25 @@
 
 
 @app.post("/worker_get_status")
 async def api_get_status(request: Request):
     return worker.get_status()
 
 
+@app.post("/count_token")
+async def count_token(request: Request):
+    params = await request.json()
+    return worker.count_token(params)
+
+
+@app.post("/model_details")
+async def model_details(request: Request):
+    return {"context_length": worker.context_len}
+
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21002)
     parser.add_argument("--worker-address", type=str, default="http://localhost:21002")
     parser.add_argument(
         "--controller-address", type=str, default="http://localhost:21001"
```

### Comparing `fschat-0.2.7/fastchat/serve/monitor/basic_stats.py` & `fschat-0.2.8/fastchat/serve/monitor/basic_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,37 @@
 
 def get_log_files(max_num_files=None):
     dates = []
     for month in [4, 5]:
         for day in range(1, 32):
             dates.append(f"2023-{month:02d}-{day:02d}")
 
-    num_servers = 10
+    num_servers = 12
     filenames = []
     for d in dates:
         for i in range(num_servers):
             name = os.path.expanduser(f"~/fastchat_logs/server{i}/{d}-conv.json")
             if os.path.exists(name):
                 filenames.append(name)
     max_num_files = max_num_files or len(filenames)
     filenames = filenames[-max_num_files:]
     return filenames
 
 
 def load_log_files(log_files):
     data = []
     for filename in tqdm(log_files, desc="read files"):
-        for l in open(filename):
+        for retry in range(5):
+            try:
+                lines = open(filename).readlines()
+                break
+            except FileNotFoundError:
+                time.sleep(2)
+
+        for l in lines:
             row = json.loads(l)
 
             data.append(
                 dict(
                     type=row["type"],
                     tstamp=row["tstamp"],
                     model=row.get("model", ""),
```

### Comparing `fschat-0.2.7/fastchat/serve/monitor/clean_battle_data.py` & `fschat-0.2.8/fastchat/serve/monitor/clean_battle_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import argparse
 import datetime
 import json
 from pytz import timezone
 import os
+import time
 
 from tqdm import tqdm
 
 from fastchat.serve.monitor.basic_stats import get_log_files
 
 
 VOTES = ["tievote", "leftvote", "rightvote", "bothbad_vote"]
 IDENTITY_WORDS = [
-    "lmsys",
     "vicuna",
+    "lmsys",
     "koala",
     "uc berkeley",
     "open assistant",
     "laion",
     "chatglm",
     "chatgpt",
     "openai",
@@ -27,18 +28,18 @@
 
 def get_log_files(max_num_files=None):
     dates = []
     for month in [4]:
         for day in range(24, 32):
             dates.append(f"2023-{month:02d}-{day:02d}")
     for month in [5]:
-        for day in range(1, 2):
+        for day in range(1, 9):
             dates.append(f"2023-{month:02d}-{day:02d}")
 
-    num_servers = 10
+    num_servers = 12
     filenames = []
     for d in dates:
         for i in range(num_servers):
             name = os.path.expanduser(f"~/fastchat_logs/server{i}/{d}-conv.json")
             if os.path.exists(name):
                 filenames.append(name)
     max_num_files = max_num_files or len(filenames)
@@ -66,15 +67,22 @@
         return raw[raw.find(": ") + 2 : -len("</h3>\n")]
     return raw
 
 
 def clean_battle_data(log_files):
     data = []
     for filename in tqdm(log_files, desc="read files"):
-        for l in open(filename):
+        for retry in range(5):
+            try:
+                lines = open(filename).readlines()
+                break
+            except FileNotFoundError:
+                time.sleep(2)
+
+        for l in lines:
             row = json.loads(l)
             if row["type"] in VOTES:
                 data.append(row)
 
     convert_type = {
         "leftvote": "model_a",
         "rightvote": "model_b",
@@ -152,21 +160,28 @@
                 rounds=rounds,
                 language=lang_code,
                 tstamp=row["tstamp"],
             )
         )
 
         all_models.update(models_hidden)
+    battles.sort(key=lambda x: x["tstamp"])
+    last_updated_tstamp = battles[-1]["tstamp"]
+
+    last_updated_datetime = datetime.datetime.fromtimestamp(
+        last_updated_tstamp, tz=timezone("US/Pacific")
+    ).strftime("%Y-%m-%d %H:%M:%S %Z")
 
     print(
         f"#votes: {len(data)}, #invalid votes: {ct_invalid}, "
         f"#leaked_identity: {ct_leaked_identity}"
     )
     print(f"#battles: {len(battles)}, #annoy: {ct_annoy}")
     print(f"#models: {len(all_models)}, {all_models}")
+    print(f"last-updated: {last_updated_datetime}")
 
     return battles
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--max-num-files", type=int)
```

### Comparing `fschat-0.2.7/fastchat/serve/monitor/elo_analysis.py` & `fschat-0.2.8/fastchat/serve/monitor/elo_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from fastchat.serve.monitor.basic_stats import get_log_files
 from fastchat.serve.monitor.clean_battle_data import clean_battle_data
 
 
 pd.options.display.float_format = "{:.2f}".format
 
 
-def compute_elo(battles, K=32, SCALE=400, BASE=10, INIT_RATING=1000):
+def compute_elo(battles, K=4, SCALE=400, BASE=10, INIT_RATING=1000):
     rating = defaultdict(lambda: INIT_RATING)
 
     for rd, model_a, model_b, win in battles[
         ["model_a", "model_b", "win"]
     ].itertuples():
         ra = rating[model_a]
         rb = rating[model_b]
@@ -43,15 +43,17 @@
 
     return dict(rating)
 
 
 def get_bootstrap_result(battles, func_compute_elo, num_round=1000):
     rows = []
     for i in tqdm(range(num_round), desc="bootstrap"):
-        rows.append(func_compute_elo(battles.sample(frac=1.0, replace=True)))
+        tmp_battles = battles.sample(frac=1.0, replace=True)
+        # tmp_battles = tmp_battles.sort_values(ascending=True, by=["tstamp"])
+        rows.append(func_compute_elo(tmp_battles))
     df = pd.DataFrame(rows)
     return df[df.median().sort_values(ascending=False).index]
 
 
 def get_elo_from_bootstrap(bootstrap_df):
     return dict(bootstrap_df.quantile(0.5))
 
@@ -108,15 +110,15 @@
     md = ""
     md += "| Rank | Model | Elo Rating | Description |\n"
     md += "| --- | --- | --- | --- |\n"
     for i, model in enumerate(models):
         rank = i + 1
         minfo = get_model_info(model)
         emoji = emoji_dict.get(rank, "")
-        md += f"| {rank} | {emoji} [{model}]({minfo.link}) | {rating[model]:.0f} | {minfo.description} |\n"
+        md += f"| {rank} | {emoji} [{model}]({minfo.link}) | {int(rating[model])} | {minfo.description} |\n"
 
     return md
 
 
 def visualize_bootstrap_elo_rating(df):
     bars = (
         pd.DataFrame(
@@ -208,40 +210,45 @@
 def report_elo_analysis_results(battles_json):
     battles = pd.DataFrame(battles_json)
     battles = battles.sort_values(ascending=True, by=["tstamp"])
     # Only use anonymous votes
     battles = battles[battles["anony"]].reset_index(drop=True)
     battles_no_ties = battles[~battles["win"].str.contains("tie")]
 
-    bootstrap_df = get_bootstrap_result(battles, compute_elo)
-    elo_rating = get_elo_from_bootstrap(bootstrap_df)
-    elo_rating = {k: int(v) for k, v in elo_rating.items()}
+    # Online update
+    elo_rating_online = compute_elo(battles)
 
-    model_order = list(elo_rating.keys())
-    model_order.sort(key=lambda k: -elo_rating[k])
+    # Bootstrap
+    bootstrap_df = get_bootstrap_result(battles, compute_elo)
+    elo_rating_median = get_elo_from_bootstrap(bootstrap_df)
+    elo_rating_median = {k: int(v) for k, v in elo_rating_median.items()}
+    model_order = list(elo_rating_median.keys())
+    model_order.sort(key=lambda k: -elo_rating_median[k])
 
-    leaderboard_table = visualize_leaderboard_table(elo_rating)
+    # Plots
+    leaderboard_table = visualize_leaderboard_table(elo_rating_online)
     win_fraction_heatmap = visualize_pairwise_win_fraction(battles_no_ties, model_order)
     battle_count_heatmap = visualize_battle_count(battles_no_ties, model_order)
     average_win_rate_bar = visualize_average_win_rate(battles_no_ties)
     bootstrap_elo_rating = visualize_bootstrap_elo_rating(bootstrap_df)
 
-    last_update_tstamp = battles["tstamp"].max()
-    last_update_datetime = datetime.datetime.fromtimestamp(
-        last_update_tstamp, tz=timezone("US/Pacific")
+    last_updated_tstamp = battles["tstamp"].max()
+    last_updated_datetime = datetime.datetime.fromtimestamp(
+        last_updated_tstamp, tz=timezone("US/Pacific")
     ).strftime("%Y-%m-%d %H:%M:%S %Z")
 
     return {
-        "elo_rating": elo_rating,
+        "elo_rating_online": elo_rating_online,
+        "elo_rating_median": elo_rating_median,
         "leaderboard_table": leaderboard_table,
         "win_fraction_heatmap": win_fraction_heatmap,
         "battle_count_heatmap": battle_count_heatmap,
         "average_win_rate_bar": average_win_rate_bar,
         "bootstrap_elo_rating": bootstrap_elo_rating,
-        "last_update_datetime": f"{last_update_datetime}",
+        "last_updated_datetime": f"{last_updated_datetime}",
     }
 
 
 def pretty_print_elo_rating(rating):
     model_order = list(rating.keys())
     model_order.sort(key=lambda k: -rating[k])
     for i, model in enumerate(model_order):
@@ -260,12 +267,15 @@
     else:
         # Read data from all log files
         log_files = get_log_files(args.max_num_files)
         battles = clean_battle_data(log_files)
 
     results = report_elo_analysis_results(battles)
 
-    pretty_print_elo_rating(results["elo_rating"])
-    print(f"last update : {results['last_update_datetime']}")
+    print("# Online")
+    pretty_print_elo_rating(results["elo_rating_online"])
+    print("# Median")
+    pretty_print_elo_rating(results["elo_rating_median"])
+    print(f"last update : {results['last_updated_datetime']}")
 
     with open("elo_results.pkl", "wb") as fout:
         pickle.dump(results, fout)
```

### Comparing `fschat-0.2.7/fastchat/serve/monitor/monitor.py` & `fschat-0.2.8/fastchat/serve/monitor/monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,29 +27,38 @@
 table_css = """
 table {
     line-height: 0em
 }
 """
 
 
+notebook_url = "https://colab.research.google.com/drive/1iI_IszGAwSMkdfUrIDI6NfTG7tGDDRxZ?usp=sharing"
+
+
+def make_leaderboard_md(elo_results):
+    leaderboard_md = f"""
+# Leaderboard
+[[Blog](https://lmsys.org/blog/2023-05-03-arena/)] [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
+
+We use the Elo rating system to calculate the relative performance of the models. You can view the voting data, basic analyses, and calculation procedure in this [notebook]({notebook_url}). We will periodically release new leaderboards. If you want to see more models, please help us [add them](https://github.com/lm-sys/FastChat/blob/main/docs/arena.md#how-to-add-a-new-model).
+Last updated: {elo_results["last_updated_datetime"]}
+{elo_results["leaderboard_table"]}
+"""
+    return leaderboard_md
+
+
 def update_elo_components(max_num_files, elo_results_file):
     log_files = get_log_files(max_num_files)
 
     # Leaderboard
     if elo_results_file is None:
         battles = clean_battle_data(log_files)
         elo_results = report_elo_analysis_results(battles)
-        leaderboard_md = f"""
-# Leaderboard
-[[Blog](https://lmsys.org/blog/2023-05-03-arena/)] [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
-We use the Elo rating system to calculate the relative performance of the models. You can view the voting data, basic analyses, and calculation procedure in this [notebook](https://colab.research.google.com/drive/1lAQ9cKVErXI1rEYq7hTKNaCQ5Q8TzrI5?usp=sharing).
-Last update: {elo_results["last_update_datetime"]}
-"""
-        leader_component_values[0] = leaderboard_md + elo_results["leaderboard_table"]
+        leader_component_values[0] = make_leaderboard_md(elo_results)
         leader_component_values[1] = elo_results["win_fraction_heatmap"]
         leader_component_values[2] = elo_results["battle_count_heatmap"]
         leader_component_values[3] = elo_results["average_win_rate_bar"]
         leader_component_values[4] = elo_results["bootstrap_elo_rating"]
 
     # Basic stats
     basic_stats = report_basic_stats(log_files)
@@ -61,15 +70,15 @@
     basic_stats_md += "### Model Call Histogram\n"
     basic_stats_md += basic_stats["model_hist_md"] + "\n"
     basic_stats_md += "### Model Call (Last 24 Hours)\n"
     basic_stats_md += basic_stats["num_chats_last_24_hours"] + "\n"
     date = datetime.datetime.now(tz=timezone("US/Pacific")).strftime(
         "%Y-%m-%d %H:%M:%S %Z"
     )
-    basic_stats_md += f"\n\nLast update: {date}"
+    basic_stats_md += f"\n\nLast updated: {date}"
     basic_component_values[0] = basic_stats_md
 
 
 def update_worker(max_num_files, interval, elo_results_file):
     while True:
         update_elo_components(max_num_files, elo_results_file)
         time.sleep(interval)
@@ -86,29 +95,29 @@
 
 
 def build_leaderboard_tab(elo_results_file):
     if elo_results_file is not None:
         with open(elo_results_file, "rb") as fin:
             elo_results = pickle.load(fin)
 
-        md = elo_results["leaderboard_md"]
+        md = make_leaderboard_md(elo_results)
         p1 = elo_results["win_fraction_heatmap"]
         p2 = elo_results["battle_count_heatmap"]
         p3 = elo_results["average_win_rate_bar"]
         p4 = elo_results["bootstrap_elo_rating"]
     else:
         md = "Loading ..."
         p1 = p2 = p3 = p4 = None
 
     leader_component_values[:] = [md, p1, p2, p3, p4]
 
     md_1 = gr.Markdown(md)
     gr.Markdown(
-        """## More Statistics\n
-Here, we have added some additional figures to show more statistics. The code for generating them is also included in this [notebook](https://colab.research.google.com/drive/1lAQ9cKVErXI1rEYq7hTKNaCQ5Q8TzrI5?usp=sharing).
+        f"""## More Statistics\n
+Here, we have added some additional figures to show more statistics. The code for generating them is also included in this [notebook]({notebook_url}).
 Please note that you may see different orders from different ranking methods. This is expected for models that perform similarly, as demonstrated by the confidence interval in the bootstrap figure. Going forward, we prefer the classical Elo calculation because of its scalability and interpretability. You can find more discussions in this blog [post](https://lmsys.org/blog/2023-05-03-arena/).
 """
     )
 
     with gr.Row():
         with gr.Column():
             gr.Markdown(
```

### Comparing `fschat-0.2.7/fastchat/serve/register_worker.py` & `fschat-0.2.8/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/serve/test_message.py` & `fschat-0.2.8/fastchat/serve/test_message.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/serve/test_throughput.py` & `fschat-0.2.8/fastchat/serve/test_throughput.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.8/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/train/train.py` & `fschat-0.2.8/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/train/train_flant5.py` & `fschat-0.2.8/fastchat/train/train_flant5.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/train/train_lora.py` & `fschat-0.2.8/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fastchat/utils.py` & `fschat-0.2.8/fastchat/utils.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.7/fschat.egg-info/PKG-INFO` & `fschat-0.2.8/fschat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.7
+Version: 0.2.8
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # FastChat
 | [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) |
 
 FastChat is an open platform for training, serving, and evaluating large language model based chatbots. The core features include:
 - The weights, training code, and evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5).
-- A distributed multi-model serving system with Web UI and OpenAI-Compatible RESTful APIs.
+- A distributed multi-model serving system with Web UI and OpenAI-compatible RESTful APIs.
 
 ## News
 - [2023/05] 🔥 We introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
 - [2023/04] We released **FastChat-T5** compatible with commercial usage. Check out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org).
 - [2023/03] We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
@@ -119,19 +119,20 @@
 
 #### Supported Models
 The following models are tested:
 - Vicuna, Alpaca, LLaMA, Koala
 - [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
 - [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
+- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
+- [mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
-- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
 Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
@@ -221,15 +222,16 @@
 - You can also launch a multi-tab gradio server, which includes the Chatbot Arena tabs.
 ```bash
 python3 -m fastchat.serve.gradio_web_server_multi
 ```
 
 ## API
 ### OpenAI-Compatible RESTful APIs & SDK
-FastChat provides OpenAI-Compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+FastChat provides OpenAI-compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+The FastChat server is compatible with both [openai-python](https://github.com/openai/openai-python) library and cURL commands.
 See [docs/openai_api.md](docs/openai_api.md).
 
 ### Hugging Face Generation APIs
 See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py).
 
 ## Evaluation
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.7 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.8 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
 [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
 h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) | FastChat is an open
 platform for training, serving, and evaluating large language model based
 chatbots. The core features include: - The weights, training code, and
 evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5). - A
-distributed multi-model serving system with Web UI and OpenAI-Compatible
+distributed multi-model serving system with Web UI and OpenAI-compatible
 RESTful APIs. ## News - [2023/05] ð¥ We introduced **Chatbot Arena** for
 battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-
 03-arena) and [demo](https://arena.lmsys.org). - [2023/04] We released
 **FastChat-T5** compatible with commercial usage. Check out the [weights]
 (#fastchat-t5) and [demo](https://chat.lmsys.org). - [2023/03] We released
 **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**.
 Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://
@@ -62,56 +62,57 @@
 with Command Line Interface (Experimental Feature: You can specify `--style
 rich` to enable rich text output and better text streaming quality for some
 non-ASCII content. This may not work properly on certain terminals.) [assets/
 screenshot_cli.png] #### Supported Models The following models are tested: -
 Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0](https://
 huggingface.co/lmsys/fastchat-t5) - [BlinkDL/RWKV-4-Raven](https://
 huggingface.co/BlinkDL/rwkv-4-raven) - [databricks/dolly-v2-12b](https://
-huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
-[StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
-stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
-chatglm-6b) - [FreedomIntelligence/phoenix-inst-chat-7b](https://
-huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) #### Single GPU The
-command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU
-memory for Vicuna-7B. See the "No Enough Memory" section below if you do not
-have enough memory. Replace `/path/to/model/weights` with the a local folder or
-a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /path/to/
-model/weights ``` #### Multiple GPUs You can use model parallelism to aggregate
-GPU memory from multiple GPUs on the same machine. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
-CPU Only This runs on the CPU only and does not require GPU. It requires around
-60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
-``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
-cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
-`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
-2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
-No Enough Memory If you do not have enough memory, you can enable 8-bit
-compression by adding `--load-8bit` to commands above. This can reduce memory
-usage by around half with slightly degraded model quality. It is compatible
-with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
-on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
-addition to that, you can add `--cpu-offloading` to commands above to offload
-weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
-compression to be enabled and the bitsandbytes package to be installed, which
-is only available on linux operating systems. #### More Platforms - [MLC LLM]
-(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
-tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
-and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
-[assets/screenshot_gui.png] To serve using the web UI, you need three main
-components: web servers that interface with users, model workers that host one
-or more models, and a controller to coordinate the webserver and model workers.
-You can learn more about the architecture [here](docs/server_arch.md). Here are
-the commands to follow in your terminal: #### Launch the controller ```bash
-python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker(s) ```bash python3 -
+huggingface.co/databricks/dolly-v2-12b) - [FreedomIntelligence/phoenix-inst-
+chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) -
+[mosaicml/mpt-7b-chat](https://huggingface.co/mosaicml/mpt-7b-chat) -
+[OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/
+oasst-sft-1-pythia-12b) - [project-baize/baize-lora-7B](https://huggingface.co/
+project-baize/baize-lora-7B) - [StabilityAI/stablelm-tuned-alpha-7b](https://
+huggingface.co/stabilityai/stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https:
+//huggingface.co/THUDM/chatglm-6b) #### Single GPU The command below requires
+around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
+See the "No Enough Memory" section below if you do not have enough memory.
+Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights ``` ####
+Multiple GPUs You can use model parallelism to aggregate GPU memory from
+multiple GPUs on the same machine. ``` python3 -m fastchat.serve.cli --model-
+path /path/to/model/weights --num-gpus 2 ``` #### CPU Only This runs on the CPU
+only and does not require GPU. It requires around 60GB of CPU memory for
+Vicuna-13B and around 30GB of CPU memory for Vicuna-7B. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device cpu ``` ####
+Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use `--device mps`
+to enable GPU acceleration on Mac computers (requires torch >= 2.0). Use `--
+load-8bit` to turn on 8-bit compression. ``` python3 -m fastchat.serve.cli --
+model-path /path/to/model/weights --device mps --load-8bit ``` Vicuna-7B can
+run on a 32GB M1 Macbook with 1 - 2 words / second. #### No Enough Memory If
+you do not have enough memory, you can enable 8-bit compression by adding `--
+load-8bit` to commands above. This can reduce memory usage by around half with
+slightly degraded model quality. It is compatible with the CPU, GPU, and Metal
+backend. Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/
+4080/T4/V100(16GB) GPU. ``` python3 -m fastchat.serve.cli --model-path /path/
+to/model/weights --load-8bit ``` In addition to that, you can add `--cpu-
+offloading` to commands above to offload weights that don't fit on your GPU
+onto the CPU memory. This requires 8-bit compression to be enabled and the
+bitsandbytes package to be installed, which is only available on linux
+operating systems. #### More Platforms - [MLC LLM](https://mlc.ai/mlc-llm/),
+backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler,
+deploys Vicuna natively on phones, consumer-class GPUs and web browsers via
+Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI [assets/
+screenshot_gui.png] To serve using the web UI, you need three main components:
+web servers that interface with users, model workers that host one or more
+models, and a controller to coordinate the webserver and model workers. You can
+learn more about the architecture [here](docs/server_arch.md). Here are the
+commands to follow in your terminal: #### Launch the controller ```bash python3
+-m fastchat.serve.controller ``` This controller manages the distributed
+workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
 ...". The model worker will register itself to the controller . To ensure that
 your model worker is connected to your controller properly, send a test message
 using the following command: ```bash python3 -m fastchat.serve.test_message --
 model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
 web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
@@ -126,26 +127,28 @@
 m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --
 controller http://localhost:21001 --port 31000 --worker http://localhost:31000
 # worker 1 CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --
 model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --
 port 31001 --worker http://localhost:31001 ``` - You can also launch a multi-
 tab gradio server, which includes the Chatbot Arena tabs. ```bash python3 -
 m fastchat.serve.gradio_web_server_multi ``` ## API ### OpenAI-Compatible
-RESTful APIs & SDK FastChat provides OpenAI-Compatible APIs for its supported
+RESTful APIs & SDK FastChat provides OpenAI-compatible APIs for its supported
 models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
-See [docs/openai_api.md](docs/openai_api.md). ### Hugging Face Generation APIs
-See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py). ##
-Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
-provides a high-level summary of the pipeline. For detailed instructions,
-please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
-Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
-ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
-Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
-reviews automatically. This step can also be performed manually if the GPT-
-4 API is not available to you. 3. Generate visualization data: Run
+The FastChat server is compatible with both [openai-python](https://github.com/
+openai/openai-python) library and cURL commands. See [docs/openai_api.md](docs/
+openai_api.md). ### Hugging Face Generation APIs See [fastchat/serve/
+huggingface_api.py](fastchat/serve/huggingface_api.py). ## Evaluation Our AI-
+enhanced evaluation pipeline is based on GPT-4. This section provides a high-
+level summary of the pipeline. For detailed instructions, please refer to the
+[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
+answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
+specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
+models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
+automatically. This step can also be performed manually if the GPT-4 API is not
+available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.7/fschat.egg-info/SOURCES.txt` & `fschat-0.2.8/fschat.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 fastchat/__init__.py
 fastchat/constants.py
 fastchat/conversation.py
 fastchat/utils.py
-fastchat/client/__init__.py
-fastchat/client/openai_api_client.py
 fastchat/data/__init__.py
 fastchat/data/clean_sharegpt.py
 fastchat/data/hardcoded_questions.py
-fastchat/data/inspect.py
+fastchat/data/inspect_data.py
 fastchat/data/merge.py
 fastchat/data/optional_clean.py
 fastchat/data/pretty_json.py
 fastchat/data/sample.py
 fastchat/data/split_long_conversation.py
 fastchat/eval/eval_gpt_review.py
 fastchat/eval/generate_webpage_data_from_table.py
@@ -59,8 +57,8 @@
 fastchat/train/train_lora.py
 fastchat/train/train_mem.py
 fschat.egg-info/PKG-INFO
 fschat.egg-info/SOURCES.txt
 fschat.egg-info/dependency_links.txt
 fschat.egg-info/requires.txt
 fschat.egg-info/top_level.txt
-tests/test_openai_client.py
+tests/test_openai_sdk.py
```

### Comparing `fschat-0.2.7/pyproject.toml` & `fschat-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.7"
+version = "0.2.8"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
```

