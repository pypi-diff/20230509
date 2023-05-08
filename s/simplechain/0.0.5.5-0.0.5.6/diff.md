# Comparing `tmp/simplechain-0.0.5.5.tar.gz` & `tmp/simplechain-0.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechain-0.0.5.5.tar", last modified: Mon May  8 23:40:30 2023, max compression
+gzip compressed data, was "simplechain-0.0.5.6.tar", last modified: Mon May  8 23:43:45 2023, max compression
```

## Comparing `simplechain-0.0.5.5.tar` & `simplechain-0.0.5.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.603580 simplechain-0.0.5.5/
--rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.5/LICENSE
--rw-rw-rw-   0        0        0      602 2023-05-08 23:40:30.602582 simplechain-0.0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-08 23:40:30.603580 simplechain-0.0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-05-08 23:40:22.000000 simplechain-0.0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.524581 simplechain-0.0.5.5/simplechain/
--rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.5/simplechain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.549580 simplechain-0.0.5.5/simplechain/pipeline/
--rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.5/simplechain/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.552580 simplechain-0.0.5.5/simplechain/pipeline/data_loaders/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.5/simplechain/pipeline/data_loaders/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.5/simplechain/pipeline/data_loaders/user_input.py
--rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.5/simplechain/pipeline/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.558586 simplechain-0.0.5.5/simplechain/pipeline/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.5/simplechain/pipeline/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.5/simplechain/pipeline/prompt_templates/base_template.py
--rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.5/simplechain/pipeline/prompt_templates/conversation_prompts.py
--rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.5/simplechain/pipeline/prompt_templates/database_prompts.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.562580 simplechain-0.0.5.5/simplechain/pipeline/providers/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.5/simplechain/pipeline/providers/__init__.py
--rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.5/simplechain/pipeline/providers/database.py
--rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.5/simplechain/pipeline/providers/search.py
--rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.5/simplechain/pipeline/standard_modules.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.565580 simplechain-0.0.5.5/simplechain/stack/
--rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.5/simplechain/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.569580 simplechain-0.0.5.5/simplechain/stack/databases/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.5/simplechain/stack/databases/__init__.py
--rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.5/simplechain/stack/databases/base.py
--rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.5/simplechain/stack/databases/sql.py
--rw-rw-rw-   0        0        0     1759 2023-04-28 02:00:57.000000 simplechain-0.0.5.5/simplechain/stack/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.570579 simplechain-0.0.5.5/simplechain/stack/image_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.5/simplechain/stack/image_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.572579 simplechain-0.0.5.5/simplechain/stack/pdf_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.5/simplechain/stack/pdf_loaders/__init__.py
--rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.5/simplechain/stack/pdf_loaders/base.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.577580 simplechain-0.0.5.5/simplechain/stack/search_engines/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.5/simplechain/stack/search_engines/__init__.py
--rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.5/simplechain/stack/search_engines/base.py
--rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5.5/simplechain/stack/search_engines/google_serper.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.583580 simplechain-0.0.5.5/simplechain/stack/text_embedders/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.5/simplechain/stack/text_embedders/__init__.py
--rw-rw-rw-   0        0        0     2146 2023-04-28 01:54:45.000000 simplechain-0.0.5.5/simplechain/stack/text_embedders/ai21.py
--rw-rw-rw-   0        0        0      329 2023-04-28 01:54:45.000000 simplechain-0.0.5.5/simplechain/stack/text_embedders/base.py
--rw-rw-rw-   0        0        0     1103 2023-04-28 01:52:29.000000 simplechain-0.0.5.5/simplechain/stack/text_embedders/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.586579 simplechain-0.0.5.5/simplechain/stack/text_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.5/simplechain/stack/text_generators/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.5/simplechain/stack/text_generators/base.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.592580 simplechain-0.0.5.5/simplechain/stack/text_generators/llms/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.5/simplechain/stack/text_generators/llms/__init__.py
--rw-rw-rw-   0        0        0     2196 2023-04-28 01:54:45.000000 simplechain-0.0.5.5/simplechain/stack/text_generators/llms/ai21.py
--rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.5/simplechain/stack/text_generators/llms/llm.py
--rw-rw-rw-   0        0        0     1165 2023-04-28 01:54:17.000000 simplechain-0.0.5.5/simplechain/stack/text_generators/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.598581 simplechain-0.0.5.5/simplechain/stack/vector_databases/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.5/simplechain/stack/vector_databases/__init__.py
--rw-rw-rw-   0        0        0     3858 2023-05-08 23:39:57.000000 simplechain-0.0.5.5/simplechain/stack/vector_databases/annoy_vd.py
--rw-rw-rw-   0        0        0     1371 2023-05-08 23:00:45.000000 simplechain-0.0.5.5/simplechain/stack/vector_databases/base.py
--rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.5/simplechain/stack/vector_databases/faiss.py
--rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.5/simplechain/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.543588 simplechain-0.0.5.5/simplechain.egg-info/
--rw-rw-rw-   0        0        0      602 2023-05-08 23:40:30.000000 simplechain-0.0.5.5/simplechain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1846 2023-05-08 23:40:30.000000 simplechain-0.0.5.5/simplechain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:40:30.000000 simplechain-0.0.5.5/simplechain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-08 23:40:30.000000 simplechain-0.0.5.5/simplechain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 23:40:30.600581 simplechain-0.0.5.5/tests/
--rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.5/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.767229 simplechain-0.0.5.6/
+-rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.6/LICENSE
+-rw-rw-rw-   0        0        0      602 2023-05-08 23:43:45.767229 simplechain-0.0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-08 23:43:45.768229 simplechain-0.0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-05-08 23:43:38.000000 simplechain-0.0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.702727 simplechain-0.0.5.6/simplechain/
+-rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.6/simplechain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.721229 simplechain-0.0.5.6/simplechain/pipeline/
+-rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.6/simplechain/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.723231 simplechain-0.0.5.6/simplechain/pipeline/data_loaders/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.6/simplechain/pipeline/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.6/simplechain/pipeline/data_loaders/user_input.py
+-rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.6/simplechain/pipeline/module.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.729229 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/base_template.py
+-rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/conversation_prompts.py
+-rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/database_prompts.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.732228 simplechain-0.0.5.6/simplechain/pipeline/providers/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.6/simplechain/pipeline/providers/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.6/simplechain/pipeline/providers/database.py
+-rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.6/simplechain/pipeline/providers/search.py
+-rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.6/simplechain/pipeline/standard_modules.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.735237 simplechain-0.0.5.6/simplechain/stack/
+-rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.6/simplechain/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.738230 simplechain-0.0.5.6/simplechain/stack/databases/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.6/simplechain/stack/databases/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.6/simplechain/stack/databases/base.py
+-rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.6/simplechain/stack/databases/sql.py
+-rw-rw-rw-   0        0        0     1759 2023-04-28 02:00:57.000000 simplechain-0.0.5.6/simplechain/stack/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.740230 simplechain-0.0.5.6/simplechain/stack/image_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.6/simplechain/stack/image_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.742230 simplechain-0.0.5.6/simplechain/stack/pdf_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.6/simplechain/stack/pdf_loaders/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.6/simplechain/stack/pdf_loaders/base.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.745230 simplechain-0.0.5.6/simplechain/stack/search_engines/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.6/simplechain/stack/search_engines/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.6/simplechain/stack/search_engines/base.py
+-rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5.6/simplechain/stack/search_engines/google_serper.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.751228 simplechain-0.0.5.6/simplechain/stack/text_embedders/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/__init__.py
+-rw-rw-rw-   0        0        0     2146 2023-04-28 01:54:45.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/ai21.py
+-rw-rw-rw-   0        0        0      329 2023-04-28 01:54:45.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/base.py
+-rw-rw-rw-   0        0        0     1103 2023-04-28 01:52:29.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.754229 simplechain-0.0.5.6/simplechain/stack/text_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/base.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.759228 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/__init__.py
+-rw-rw-rw-   0        0        0     2196 2023-04-28 01:54:45.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/ai21.py
+-rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/llm.py
+-rw-rw-rw-   0        0        0     1165 2023-04-28 01:54:17.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.764228 simplechain-0.0.5.6/simplechain/stack/vector_databases/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/__init__.py
+-rw-rw-rw-   0        0        0     3864 2023-05-08 23:43:16.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/annoy_vd.py
+-rw-rw-rw-   0        0        0     1531 2023-05-08 23:43:20.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/base.py
+-rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/faiss.py
+-rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.6/simplechain/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.715736 simplechain-0.0.5.6/simplechain.egg-info/
+-rw-rw-rw-   0        0        0      602 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.765229 simplechain-0.0.5.6/tests/
+-rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.6/tests/__init__.py
```

### Comparing `simplechain-0.0.5.5/LICENSE` & `simplechain-0.0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/PKG-INFO` & `simplechain-0.0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.5/README.rst` & `simplechain-0.0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/setup.py` & `simplechain-0.0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5.5'
+VERSION = '0.0.5.6'
 DESCRIPTION = 'A package of AI services in modular form'
 LONG_DESCRIPTION = 'A package of AI services in modular form easily configurable and deployable'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="simplechain",
```

### Comparing `simplechain-0.0.5.5/simplechain/pipeline/module.py` & `simplechain-0.0.5.6/simplechain/pipeline/module.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/pipeline/prompt_templates/conversation_prompts.py` & `simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/conversation_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/pipeline/prompt_templates/database_prompts.py` & `simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/database_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/pipeline/providers/database.py` & `simplechain-0.0.5.6/simplechain/pipeline/providers/database.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/pipeline/standard_modules.py` & `simplechain-0.0.5.6/simplechain/pipeline/standard_modules.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/databases/base.py` & `simplechain-0.0.5.6/simplechain/stack/databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/databases/sql.py` & `simplechain-0.0.5.6/simplechain/stack/databases/sql.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/factory.py` & `simplechain-0.0.5.6/simplechain/stack/factory.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/search_engines/google_serper.py` & `simplechain-0.0.5.6/simplechain/stack/search_engines/google_serper.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/text_embedders/ai21.py` & `simplechain-0.0.5.6/simplechain/stack/text_embedders/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/text_embedders/openai.py` & `simplechain-0.0.5.6/simplechain/stack/text_embedders/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/text_generators/llms/ai21.py` & `simplechain-0.0.5.6/simplechain/stack/text_generators/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/text_generators/llms/llm.py` & `simplechain-0.0.5.6/simplechain/stack/text_generators/llms/llm.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/text_generators/llms/openai.py` & `simplechain-0.0.5.6/simplechain/stack/text_generators/llms/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/stack/vector_databases/annoy_vd.py` & `simplechain-0.0.5.6/simplechain/stack/vector_databases/annoy_vd.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,36 +76,36 @@
         self.index.save(self.path_to_index_file)
 
         # Save metadata to json
         metadata_json = json.dumps(self.metadata)
         with open(self.path_to_metadata_file, "w") as f:
             f.write(metadata_json)
 
-    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1, include_distances: bool= False) -> Dict:
+    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1, include_distances: bool = False) -> Dict:
         """
         Given a query embed, get the k nearest neighbors with their distances
         :param include_distances:
         :param query_embed:
         :param k:
         :return: k nearest neighbors with their distances
         """
         results = {}
         nearest_neighbors = self.index.get_nns_by_vector(query_embed, k, include_distances)
         results["ids"] = nearest_neighbors[0]
         if include_distances:
             results["distances"] = nearest_neighbors[1]
-        results["metadata"] = [self.metadata[i] for i in nearest_neighbors[0]] # Get metadata for each id
+        results["metadata"] = [self.metadata[i] for i in nearest_neighbors[0]]  # Get metadata for each id
 
         return results
 
-    def get_item_given_index(self, index: int, return_embeds: bool = True, return_metadata: bool = True) -> Dict:
+    def get_item_given_index(self, index: int, include_embeds: bool = True, include_metadata: bool = True) -> Dict:
         """
         Given an index, get the name and embed of the item
         :param index:
         :return:
         """
         results = {}
-        if return_embeds:
+        if include_embeds:
             results["embed"] = self.index.get_item_vector(index)
-        if return_metadata:
+        if include_metadata:
             results["metadata"] = self.metadata[index]
         return results
```

### Comparing `simplechain-0.0.5.5/simplechain/stack/vector_databases/base.py` & `simplechain-0.0.5.6/simplechain/stack/vector_databases/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,26 +30,27 @@
         """
         Build the database
         :return:
         """
         pass
 
     @abstractmethod
-    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1) -> Dict:
+    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1, include_distances: bool = False) -> Dict:
         """
         Given a query embed, get the k nearest neighbors with their distances
         :param query_embed:
         :param k:
         :return: a list of k nearest neighbours with their payloads and distances
         """
         pass
+
     @abstractmethod
-    def get_item_given_index(self, index: int, return_embed:bool=False) -> Dict:
+    def get_item_given_index(self, index: int, include_embeds: bool = True, include_metadata: bool = True) -> Dict:
         """
         Given an index, get the name and embed of the item
+        :param include_metadata:
+        :param include_embeds:
+        :param return_embed:
         :param index:
         :return:
         """
         pass
-
-
-
```

### Comparing `simplechain-0.0.5.5/simplechain/stack/vector_databases/faiss.py` & `simplechain-0.0.5.6/simplechain/stack/vector_databases/faiss.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain/utils.py` & `simplechain-0.0.5.6/simplechain/utils.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.5/simplechain.egg-info/PKG-INFO` & `simplechain-0.0.5.6/simplechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.5/simplechain.egg-info/SOURCES.txt` & `simplechain-0.0.5.6/simplechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

