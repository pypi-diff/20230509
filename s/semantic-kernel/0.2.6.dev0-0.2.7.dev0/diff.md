# Comparing `tmp/semantic_kernel-0.2.6.dev0.tar.gz` & `tmp/semantic_kernel-0.2.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.2.6.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.2.7.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.2.6.dev0.tar` & `semantic_kernel-0.2.7.dev0.tar`

### file list

```diff
@@ -1,89 +1,91 @@
--rw-r--r--   0        0        0     4595 2023-05-02 00:16:15.432235 semantic_kernel-0.2.6.dev0/README.md
--rw-r--r--   0        0        0      719 2023-05-02 00:16:15.432829 semantic_kernel-0.2.6.dev0/pyproject.toml
--rw-r--r--   0        0        0     1302 2023-04-18 17:46:11.883057 semantic_kernel-0.2.6.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.983569 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0      506 2023-04-30 18:57:02.983999 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1129 2023-04-30 18:57:02.985239 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1332 2023-04-30 18:57:02.985587 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.986074 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.986678 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     3569 2023-05-01 23:42:05.935410 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2093 2023-04-30 18:57:02.988126 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.988571 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2782 2023-04-30 18:57:02.989002 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2774 2023-04-30 18:57:02.989380 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2769 2023-04-30 18:57:02.990041 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     5227 2023-04-30 18:57:02.990444 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     4471 2023-04-30 18:57:02.990953 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2572 2023-05-01 23:42:05.936356 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0      497 2023-04-30 18:57:02.991644 semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      457 2023-04-22 04:06:40.780007 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2072 2023-04-13 23:12:46.166679 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.780276 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.194344 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2403 2023-04-13 23:12:46.167467 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     5849 2023-04-30 18:57:02.992220 semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0    12503 2023-04-30 18:57:02.992677 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     2240 2023-04-22 04:06:40.781294 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_base.py
--rw-r--r--   0        0        0    10319 2023-05-02 00:16:15.433586 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_config.py
--rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.993735 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      710 2023-04-14 00:51:57.196637 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/__init__.py
--rw-r--r--   0        0        0      210 2023-04-13 23:12:46.171776 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
--rw-r--r--   0        0        0     3822 2023-04-30 18:57:02.994407 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/import_skills.py
--rw-r--r--   0        0        0     2323 2023-04-13 23:12:46.172614 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/inline_definition.py
--rw-r--r--   0        0        0     1497 2023-05-02 00:16:15.434300 semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.173418 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2345 2023-04-30 18:57:02.996159 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3089 2023-04-30 18:57:02.996701 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2012 2023-04-30 18:57:02.997202 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1137 2023-04-13 23:12:46.175270 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6045 2023-05-02 00:16:15.434951 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1196 2023-04-30 18:57:02.998063 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-04-30 18:57:02.998486 semantic_kernel-0.2.6.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.782347 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.199808 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     8966 2023-04-14 00:51:57.200548 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.179530 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.160748 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    15917 2023-04-30 18:57:02.998992 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.999492 semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      919 2023-04-13 23:12:46.181682 semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      673 2023-04-13 23:12:46.182155 semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/retry_mechanism.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.182583 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.203325 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.183441 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4269 2023-04-30 18:57:02.999997 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.204455 semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.205241 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.205757 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     1717 2023-04-13 23:12:46.186028 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.206300 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.206885 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.207475 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.187552 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.208334 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.208951 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.188719 semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.189034 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.209567 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.210164 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000489 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.192355 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.192840 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.211524 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.193631 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.212261 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.194683 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.212967 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.195769 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.196165 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.196572 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.196999 semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.001133 semantic_kernel-0.2.6.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.001562 semantic_kernel-0.2.6.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     6466 2023-05-01 18:36:22.039798 semantic_kernel-0.2.6.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.197533 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2436 2023-04-14 00:51:57.213683 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.198404 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.198764 semantic_kernel-0.2.6.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5307 1970-01-01 00:00:00.000000 semantic_kernel-0.2.6.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 22:48:20.447102 semantic_kernel-0.2.7.dev0/pip/README.md
+-rw-r--r--   0        0        0      771 2023-05-08 22:53:10.954241 semantic_kernel-0.2.7.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1227 2023-05-07 18:39:02.913641 semantic_kernel-0.2.7.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-29 00:21:18.081250 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0      506 2023-04-29 00:21:18.081609 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1129 2023-04-29 00:21:18.081920 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1332 2023-04-29 00:21:18.082190 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-29 00:21:18.082773 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 23:48:28.652652 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3837 2023-05-08 22:53:10.956135 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 22:53:10.957061 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-29 00:21:18.084928 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2782 2023-04-29 00:21:18.085471 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2774 2023-04-29 00:21:18.085835 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2769 2023-04-29 00:21:18.086154 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     5227 2023-04-30 23:48:28.654055 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     4471 2023-04-30 23:48:28.654520 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2572 2023-05-02 00:49:03.449515 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0      497 2023-04-30 23:48:28.654940 semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      500 2023-05-07 18:39:02.916522 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-14 03:36:09.239029 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-26 22:16:44.328276 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 03:36:09.239829 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2403 2023-04-14 03:36:09.240512 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     5849 2023-04-29 00:21:18.088108 semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0    22020 2023-05-08 22:53:10.957924 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     2099 2023-05-07 18:39:02.918601 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_base.py
+-rw-r--r--   0        0        0     1626 2023-04-29 00:21:18.089839 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      710 2023-04-14 03:36:09.245082 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/__init__.py
+-rw-r--r--   0        0        0      210 2023-04-14 03:36:09.245483 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/extends_kernel.py
+-rw-r--r--   0        0        0     3822 2023-04-29 00:21:18.090797 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/import_skills.py
+-rw-r--r--   0        0        0     2323 2023-04-14 03:36:09.246857 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/inline_definition.py
+-rw-r--r--   0        0        0     1483 2023-05-07 18:39:02.919392 semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/memory_configuration.py
+-rw-r--r--   0        0        0      160 2023-04-14 03:36:09.247903 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-30 23:48:28.656559 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3090 2023-05-07 18:39:02.920199 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2004 2023-05-07 18:39:02.921208 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1137 2023-04-14 03:36:09.249612 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6045 2023-05-02 00:49:03.451205 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1196 2023-04-30 23:48:28.662481 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-04-30 23:48:28.664620 semantic_kernel-0.2.7.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-20 17:10:26.995186 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 03:36:09.253302 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     8966 2023-04-14 03:36:09.253662 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-14 03:36:09.254004 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 03:36:09.254344 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    15915 2023-05-07 18:39:02.921883 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 23:48:28.668178 semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-07 18:39:02.922653 semantic_kernel-0.2.7.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7275 2023-05-07 18:39:02.923105 semantic_kernel-0.2.7.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0      396 2023-05-07 18:39:02.923447 semantic_kernel-0.2.7.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      919 2023-04-14 03:36:09.255908 semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      673 2023-04-14 03:36:09.256522 semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/retry_mechanism.py
+-rw-r--r--   0        0        0     2101 2023-04-14 03:36:09.256949 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 03:36:09.257319 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-14 03:36:09.257703 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4269 2023-04-29 00:21:18.098358 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 03:36:09.258593 semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 03:36:09.259027 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 03:36:09.259911 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     1717 2023-04-14 03:36:09.260336 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 03:36:09.261065 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 03:36:09.261495 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 03:36:09.261836 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-14 03:36:09.262309 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 03:36:09.262723 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 03:36:09.263484 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-14 03:36:09.263900 semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-14 03:36:09.264367 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 03:36:09.264992 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 03:36:09.265522 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-29 00:21:18.098851 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-14 03:36:09.267164 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-14 03:36:09.267627 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 03:36:09.268042 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-14 03:36:09.268607 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 03:36:09.269045 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-14 03:36:09.269480 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 03:36:09.269880 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-14 03:36:09.270280 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-14 03:36:09.270855 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-14 03:36:09.271313 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-14 03:36:09.271775 semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 23:48:28.669001 semantic_kernel-0.2.7.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 23:48:28.669455 semantic_kernel-0.2.7.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     6466 2023-04-30 23:48:28.670502 semantic_kernel-0.2.7.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-14 03:36:09.272351 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2436 2023-04-14 03:36:09.272775 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-14 03:36:09.273176 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-14 03:36:09.274119 semantic_kernel-0.2.7.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 semantic_kernel-0.2.7.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from semantic_kernel import core_skills, memory
 from semantic_kernel.kernel import Kernel
-from semantic_kernel.kernel_config import KernelConfig
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.semantic_functions.chat_prompt_template import ChatPromptTemplate
 from semantic_kernel.semantic_functions.prompt_template import PromptTemplate
 from semantic_kernel.semantic_functions.prompt_template_config import (
     PromptTemplateConfig,
@@ -18,15 +17,14 @@
 from semantic_kernel.utils.settings import (
     azure_openai_settings_from_dot_env,
     openai_settings_from_dot_env,
 )
 
 __all__ = [
     "Kernel",
-    "KernelConfig",
     "NullLogger",
     "openai_settings_from_dot_env",
     "azure_openai_settings_from_dot_env",
     "PromptTemplateConfig",
     "PromptTemplate",
     "ChatPromptTemplate",
     "SemanticFunctionConfig",
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import Optional
 
-import torch
-from transformers import GenerationConfig, pipeline
-
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.complete_request_settings import (
     CompleteRequestSettings,
 )
 from semantic_kernel.connectors.ai.text_completion_client_base import (
     TextCompletionClientBase,
 )
@@ -44,18 +41,27 @@
             log {Optional[Logger]} -- Logger instance.
 
         Note that this model will be downloaded from the Hugging Face model hub.
         """
         self._model_id = model_id
         self._task = "text2text-generation" if task is None else task
         self._log = log if log is not None else NullLogger()
+
+        try:
+            import torch
+            import transformers
+        except (ImportError, ModuleNotFoundError):
+            raise ImportError(
+                "Please ensure that torch and transformers are installed to use HuggingFaceTextCompletion"
+            )
+
         self.device = (
             "cuda:" + device if device >= 0 and torch.cuda.is_available() else "cpu"
         )
-        self.generator = pipeline(
+        self.generator = transformers.pipeline(
             task=self._task, model=self._model_id, device=self.device
         )
 
     async def complete_async(
         self, prompt: str, request_settings: CompleteRequestSettings
     ) -> str:
         """
@@ -65,15 +71,17 @@
             prompt {str} -- Prompt to complete.
             request_settings {CompleteRequestSettings} -- Request settings.
 
         Returns:
             str -- Completion result.
         """
         try:
-            generation_config = GenerationConfig(
+            import transformers
+
+            generation_config = transformers.GenerationConfig(
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 max_new_tokens=request_settings.max_tokens,
                 pad_token_id=50256,  # EOS token
             )
             result = self.generator(
                 prompt, num_return_sequences=1, generation_config=generation_config
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from logging import Logger
 from typing import List, Optional
 
-import torch
 from numpy import array, ndarray
-from sentence_transformers import SentenceTransformer
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import (
     EmbeddingGeneratorBase,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 
@@ -34,18 +32,27 @@
             device {Optional[int]} -- Device to run the model on, -1 for CPU, 0+ for GPU.
             log {Optional[Logger]} -- Logger instance.
 
         Note that this model will be downloaded from the Hugging Face model hub.
         """
         self._model_id = model_id
         self._log = log if log is not None else NullLogger()
+
+        try:
+            import sentence_transformers
+            import torch
+        except ImportError:
+            raise ImportError(
+                "Please ensure that torch and sentence-transformers are installed to use HuggingFaceTextEmbedding"
+            )
+
         self.device = (
             "cuda:" + device if device >= 0 and torch.cuda.is_available() else "cpu"
         )
-        self.generator = SentenceTransformer(
+        self.generator = sentence_transformers.SentenceTransformer(
             model_name_or_path=self._model_id, device=self.device
         )
 
     async def generate_embeddings_async(self, texts: List[str]) -> ndarray:
         """
         Generates embeddings for a list of texts.
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_base.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import ABC, abstractmethod
 from logging import Logger
 from typing import Any, Dict, Optional
 
-from semantic_kernel.kernel_config import KernelConfig
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.semantic_functions.semantic_function_config import (
     SemanticFunctionConfig,
 )
@@ -19,19 +18,14 @@
     PromptTemplatingEngine,
 )
 
 
 class KernelBase(ABC):
     @property
     @abstractmethod
-    def config(self) -> KernelConfig:
-        pass
-
-    @property
-    @abstractmethod
     def logger(self) -> Logger:
         pass
 
     @property
     @abstractmethod
     def memory(self) -> SemanticTextMemoryBase:
         pass
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/__init__.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/import_skills.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/import_skills.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/inline_definition.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/inline_definition.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/kernel_extensions/memory_configuration.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/kernel_extensions/memory_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
         self,
         storage: MemoryStoreBase,
         embeddings_generator: Optional[EmbeddingGeneratorBase] = None,
     ) -> None:
         kernel = self.kernel()
 
         if embeddings_generator is None:
-            service_id = kernel.config.get_text_embedding_generation_service_id()
+            service_id = kernel.get_text_embedding_generation_service_id()
             if not service_id:
                 raise ValueError("The embedding service id cannot be `None` or empty")
 
-            embeddings_service = kernel.config.get_ai_service(
+            embeddings_service = kernel.get_ai_service(
                 EmbeddingGeneratorBase, service_id
             )
             if not embeddings_service:
                 raise ValueError(f"AI configuration is missing for: {service_id}")
 
             embeddings_generator = embeddings_service(kernel)
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self._id = id
         self._description = description
         self._text = text
         self._embedding = embedding
 
     @property
     def embedding(self) -> ndarray:
-        return self.embedding
+        return self._embedding
 
     @staticmethod
     def reference_record(
         external_id: str,
         source_name: str,
         description: Optional[str],
         embedding: ndarray,
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 
 class MemoryStoreBase:
     @abstractmethod
-    async def create_collection_async(self, collection_name: SystemError) -> None:
+    async def create_collection_async(self, collection_name: str) -> None:
         pass
 
     @abstractmethod
     async def get_collections_async(
         self,
     ) -> List[str]:
         pass
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
             loop = None
 
         # Handle "asyncio.run() cannot be called from a running event loop"
         if loop and loop.is_running():
             if self.is_semantic:
                 return self._runThread(self._invoke_semantic_async(context, settings))
             else:
-                return self._runThread(self._invoke_semantic_async(context))
+                return self._runThread(self._invoke_native_async(context))
         else:
             if self.is_semantic:
                 return asyncio.run(self._invoke_semantic_async(context, settings))
             else:
                 return asyncio.run(self._invoke_native_async(context))
 
     async def invoke_async(
```

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/reliability/retry_mechanism.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/reliability/retry_mechanism.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.2.6.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.2.7.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

