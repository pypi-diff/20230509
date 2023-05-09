# Comparing `tmp/textgen-0.2.4.tar.gz` & `tmp/textgen-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgen-0.2.4.tar", last modified: Wed Apr 19 14:11:21 2023, max compression
+gzip compressed data, was "textgen-0.2.5.tar", last modified: Tue May  9 04:08:05 2023, max compression
```

## Comparing `textgen-0.2.4.tar` & `textgen-0.2.5.tar`

### file list

```diff
@@ -1,68 +1,73 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.674785 textgen-0.2.4/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.4/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 14:11:21.675321 textgen-0.2.4/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)    28546 2023-04-17 14:03:20.000000 textgen-0.2.4/README.md
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-04-19 14:11:21.676265 textgen-0.2.4/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1427 2023-04-19 14:11:02.000000 textgen-0.2.4/setup.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.622178 textgen-0.2.4/textgen/
--rw-r--r--   0 xuming     (501) staff       (20)     1386 2023-04-19 14:11:02.000000 textgen-0.2.4/textgen/__init__.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.632125 textgen-0.2.4/textgen/augment/
--rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.4/textgen/augment/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.4/textgen/augment/sentence_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.4/textgen/augment/text_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.4/textgen/augment/tokenizer.py
--rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/augment/translate_api.py
--rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.4/textgen/augment/word_level_augment.py
--rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.4/textgen/augment/word_vocab.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.636939 textgen-0.2.4/textgen/chatglm/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-03-26 02:30:43.000000 textgen-0.2.4/textgen/chatglm/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    22085 2023-04-19 14:09:32.000000 textgen-0.2.4/textgen/chatglm/chatglm_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6270 2023-04-13 05:04:59.000000 textgen-0.2.4/textgen/chatglm/chatglm_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.640358 textgen-0.2.4/textgen/config/
--rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/config/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.4/textgen/config/global_args.py
--rw-r--r--   0 xuming     (501) staff       (20)    14505 2023-04-19 06:54:54.000000 textgen-0.2.4/textgen/config/model_args.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.642195 textgen-0.2.4/textgen/custom_models/
--rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/custom_models/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.4/textgen/custom_models/models.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.645721 textgen-0.2.4/textgen/data/
--rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.4/textgen/data/HowNetPOSWord.txt
--rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.4/textgen/data/stopwords.txt
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.649093 textgen-0.2.4/textgen/language_generation/
--rwxr-xr-x   0 xuming     (501) staff       (20)      292 2021-08-05 02:59:06.000000 textgen-0.2.4/textgen/language_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    10056 2022-07-05 07:48:33.000000 textgen-0.2.4/textgen/language_generation/language_generation_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.4/textgen/language_generation/language_generation_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.655570 textgen-0.2.4/textgen/language_modeling/
--rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.4/textgen/language_modeling/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    56833 2022-09-09 11:41:34.000000 textgen-0.2.4/textgen/language_modeling/language_modeling_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.4/textgen/language_modeling/language_modeling_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    65595 2022-11-27 05:36:55.000000 textgen-0.2.4/textgen/language_modeling/songnet_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.4/textgen/language_modeling/songnet_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.659754 textgen-0.2.4/textgen/llama/
--rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.4/textgen/llama/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    22752 2023-04-19 14:10:06.000000 textgen-0.2.4/textgen/llama/llama_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     5741 2023-04-18 02:48:12.000000 textgen-0.2.4/textgen/llama/llama_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.666469 textgen-0.2.4/textgen/seq2seq/
--rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.4/textgen/seq2seq/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    73131 2023-04-14 09:07:24.000000 textgen-0.2.4/textgen/seq2seq/bart_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.4/textgen/seq2seq/bart_seq2seq_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.4/textgen/seq2seq/conv_seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.4/textgen/seq2seq/data_reader.py
--rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.4/textgen/seq2seq/seq2seq_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.4/textgen/seq2seq/seq2seq_trainer.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.671895 textgen-0.2.4/textgen/t5/
--rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.4/textgen/t5/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)    50493 2022-11-16 12:03:51.000000 textgen-0.2.4/textgen/t5/copyt5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.4/textgen/t5/copyt5_utils.py
--rw-r--r--   0 xuming     (501) staff       (20)    50530 2023-04-14 09:07:24.000000 textgen-0.2.4/textgen/t5/t5_model.py
--rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.4/textgen/t5/t5_utils.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.673844 textgen-0.2.4/textgen/unsup_generation/
--rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.4/textgen/unsup_generation/__init__.py
--rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.4/textgen/unsup_generation/tgls_model.py
--rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.4/textgen/unsup_generation/tgls_util.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-04-19 14:11:21.625149 textgen-0.2.4/textgen.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    33563 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     1692 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)      166 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)        8 2023-04-19 14:11:21.000000 textgen-0.2.4/textgen.egg-info/top_level.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.846691 textgen-0.2.5/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2021-08-05 02:59:06.000000 textgen-0.2.5/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    40662 2023-05-09 04:08:05.847286 textgen-0.2.5/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)    35285 2023-05-09 04:07:28.000000 textgen-0.2.5/README.md
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-05-09 04:08:05.848243 textgen-0.2.5/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1427 2023-05-08 11:53:06.000000 textgen-0.2.5/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.771976 textgen-0.2.5/textgen/
+-rw-r--r--   0 xuming     (501) staff       (20)     1484 2023-05-08 11:53:06.000000 textgen-0.2.5/textgen/__init__.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.784082 textgen-0.2.5/textgen/augment/
+-rw-r--r--   0 xuming     (501) staff       (20)      133 2022-06-30 07:59:18.000000 textgen-0.2.5/textgen/augment/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1493 2022-05-09 11:34:10.000000 textgen-0.2.5/textgen/augment/sentence_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3582 2023-04-12 09:49:33.000000 textgen-0.2.5/textgen/augment/text_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2256 2022-07-04 08:00:34.000000 textgen-0.2.5/textgen/augment/tokenizer.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1971 2021-08-05 02:59:06.000000 textgen-0.2.5/textgen/augment/translate_api.py
+-rw-r--r--   0 xuming     (501) staff       (20)    13027 2022-09-26 07:39:41.000000 textgen-0.2.5/textgen/augment/word_level_augment.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1240 2022-05-09 11:34:10.000000 textgen-0.2.5/textgen/augment/word_vocab.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.788241 textgen-0.2.5/textgen/bloom/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.5/textgen/bloom/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    25402 2023-05-09 03:47:33.000000 textgen-0.2.5/textgen/bloom/bloom_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5972 2023-05-09 03:02:44.000000 textgen-0.2.5/textgen/bloom/bloom_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.792339 textgen-0.2.5/textgen/chatglm/
+-rw-r--r--   0 xuming     (501) staff       (20)       79 2023-05-08 11:53:06.000000 textgen-0.2.5/textgen/chatglm/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    25189 2023-05-09 03:47:33.000000 textgen-0.2.5/textgen/chatglm/chatglm_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6280 2023-05-05 06:44:33.000000 textgen-0.2.5/textgen/chatglm/chatglm_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.795655 textgen-0.2.5/textgen/config/
+-rw-r--r--   0 xuming     (501) staff       (20)      140 2021-08-05 02:59:06.000000 textgen-0.2.5/textgen/config/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     1845 2022-06-30 03:18:51.000000 textgen-0.2.5/textgen/config/global_args.py
+-rw-r--r--   0 xuming     (501) staff       (20)    16911 2023-05-09 02:12:56.000000 textgen-0.2.5/textgen/config/model_args.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.798297 textgen-0.2.5/textgen/custom_models/
+-rwxr-xr-x   0 xuming     (501) staff       (20)        0 2021-08-05 02:59:06.000000 textgen-0.2.5/textgen/custom_models/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    32645 2022-08-24 03:27:39.000000 textgen-0.2.5/textgen/custom_models/models.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.802209 textgen-0.2.5/textgen/data/
+-rwxr-xr-x   0 xuming     (501) staff       (20)    48098 2019-08-25 14:57:21.000000 textgen-0.2.5/textgen/data/HowNetPOSWord.txt
+-rw-r--r--   0 xuming     (501) staff       (20)    17438 2021-10-25 11:27:11.000000 textgen-0.2.5/textgen/data/stopwords.txt
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.808222 textgen-0.2.5/textgen/language_generation/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      231 2023-05-08 11:53:06.000000 textgen-0.2.5/textgen/language_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10178 2023-04-30 13:02:41.000000 textgen-0.2.5/textgen/language_generation/language_generation_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     2829 2022-06-14 12:08:00.000000 textgen-0.2.5/textgen/language_generation/language_generation_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.816078 textgen-0.2.5/textgen/language_modeling/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      407 2022-09-10 06:38:25.000000 textgen-0.2.5/textgen/language_modeling/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    56955 2023-04-30 13:02:41.000000 textgen-0.2.5/textgen/language_modeling/language_modeling_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     8938 2022-06-14 12:08:00.000000 textgen-0.2.5/textgen/language_modeling/language_modeling_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    65717 2023-04-30 13:02:41.000000 textgen-0.2.5/textgen/language_modeling/songnet_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    17103 2022-12-05 07:28:16.000000 textgen-0.2.5/textgen/language_modeling/songnet_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.822577 textgen-0.2.5/textgen/llama/
+-rw-r--r--   0 xuming     (501) staff       (20)       80 2023-04-10 03:44:03.000000 textgen-0.2.5/textgen/llama/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    25723 2023-05-09 03:47:33.000000 textgen-0.2.5/textgen/llama/llama_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     5692 2023-05-07 13:27:41.000000 textgen-0.2.5/textgen/llama/llama_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    12870 2023-05-08 06:47:35.000000 textgen-0.2.5/textgen/llama/merge_llama_with_chinese_lora.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.832547 textgen-0.2.5/textgen/seq2seq/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      313 2022-08-07 03:00:11.000000 textgen-0.2.5/textgen/seq2seq/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    73253 2023-04-30 13:02:41.000000 textgen-0.2.5/textgen/seq2seq/bart_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    18590 2023-04-12 10:19:10.000000 textgen-0.2.5/textgen/seq2seq/bart_seq2seq_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    23456 2022-08-25 03:06:56.000000 textgen-0.2.5/textgen/seq2seq/conv_seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     4345 2022-05-10 10:48:02.000000 textgen-0.2.5/textgen/seq2seq/data_reader.py
+-rw-r--r--   0 xuming     (501) staff       (20)    19319 2022-08-25 03:06:56.000000 textgen-0.2.5/textgen/seq2seq/seq2seq_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    10564 2023-04-12 10:22:29.000000 textgen-0.2.5/textgen/seq2seq/seq2seq_trainer.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.841997 textgen-0.2.5/textgen/t5/
+-rwxr-xr-x   0 xuming     (501) staff       (20)      272 2022-08-23 06:18:39.000000 textgen-0.2.5/textgen/t5/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50615 2023-04-30 13:02:41.000000 textgen-0.2.5/textgen/t5/copyt5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     6917 2022-11-16 13:02:34.000000 textgen-0.2.5/textgen/t5/copyt5_utils.py
+-rw-r--r--   0 xuming     (501) staff       (20)    50652 2023-04-30 13:02:41.000000 textgen-0.2.5/textgen/t5/t5_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)     7146 2022-11-17 02:54:45.000000 textgen-0.2.5/textgen/t5/t5_utils.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.845328 textgen-0.2.5/textgen/unsup_generation/
+-rw-r--r--   0 xuming     (501) staff       (20)      246 2022-09-06 02:24:58.000000 textgen-0.2.5/textgen/unsup_generation/__init__.py
+-rw-r--r--   0 xuming     (501) staff       (20)     3456 2022-09-26 07:01:36.000000 textgen-0.2.5/textgen/unsup_generation/tgls_model.py
+-rw-r--r--   0 xuming     (501) staff       (20)    27678 2022-09-06 02:29:56.000000 textgen-0.2.5/textgen/unsup_generation/tgls_util.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-05-09 04:08:05.776010 textgen-0.2.5/textgen.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    40662 2023-05-09 04:08:05.000000 textgen-0.2.5/textgen.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     1823 2023-05-09 04:08:05.000000 textgen-0.2.5/textgen.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-05-09 04:08:05.000000 textgen-0.2.5/textgen.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      166 2023-05-09 04:08:05.000000 textgen-0.2.5/textgen.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        8 2023-05-09 04:08:05.000000 textgen-0.2.5/textgen.egg-info/top_level.txt
```

### Comparing `textgen-0.2.4/LICENSE` & `textgen-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/PKG-INFO` & `textgen-0.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.4
+Version: 0.2.5
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
@@ -12,180 +12,184 @@
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # TextGen
         
-        🌈Implementation of Text Generation models.
+        🌈 Implementation of Text Generation models.
         
-        **textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
+        **textgen**实现了多种文本生成模型，包括：LLaMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
-        **Guide**
-        
-        - [Feature](#Feature)
-        - [Install](#install)
-        - [Usage](#usage)
-        - [Contact](#Contact)
-        - [License](#License)
-        
-        ## 😊Feature
-        
-        ### 文本生成
-        
-        1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
-        2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
-        3. t5: T5、CopyT5
-        
-        ### 文本扩增
-        
-        #### 词粒度扩增
-        
-        1. UDA，非核心词替换
-        2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
-        
-        #### 句粒度扩增
-        
-        1. 回译（BT, Back Translate）：中文-英文-中文
-        2. GPT2模型续写：短文本->长文本
-        3. BART摘要模型：长文本->短文本
-        4. TGLS：无监督相似文本生成模型
-        
-        ### 功能列表
+        ## 😊 Feature
         
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
-        - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
-        - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
+        - [LLaMA](textgen/llama)：本项目基于PyTorch实现了LLaMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
+        - [UDA/EDA](textgen/augment/word_level_augment.py)：本项目实现了UDA(非核心词替换)、EDA和Back Translation(回译)算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
         - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         ### Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
         
-        |Model| Arch       |Introduce| Training                                                                                                                                     | Inference                                                                                                             | 
-        |:-- |:-----------|:--- |:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
-        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5         |中文NLP多任务Prompt模型| [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
-        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5         |fine-tuned中文对联后的模型| [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
-        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet    |SongNet预训练模型| -                                                                                                                                            | -                                                                                                                     |
-        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet    |fine-tuned宋词后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
-        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet    |fine-tuned对联后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
-        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B |在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
-        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
-        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLAMA-13B  |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+        |Model| Arch          | Introduce                                                                                                                                                        | Training                                                                                                                                     | Inference                                                                                                             | 
+        |:-- |:--------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
+        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5            | 中文NLP多任务Prompt模型                                                                                                                                                 | [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
+        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5            | fine-tuned中文对联后的模型                                                                                                                                               | [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
+        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet       | SongNet预训练模型                                                                                                                                                     | -                                                                                                                                            | -                                                                                                                     |
+        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet       | fine-tuned宋词后的模型                                                                                                                                                 | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
+        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet       | fine-tuned对联后的模型                                                                                                                                                 | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B    | 在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重                                                | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B    | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重                   | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
+        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLaMA-13B     | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重                    | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+        |[shibing624/chinese-alpaca-plus-7b](https://huggingface.co/shibing624/chinese-alpaca-plus-7b)| LLaMA-7B-plus | [中文LLaMA, Alpaca Plus版（7B）](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型  | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
+        
+        ### Evaluation
+        
+        | Model                                                                                                                                       |Arch| Introduce                                                                                                            | Score    |
+        |:--------------------------------------------------------------------------------------------------------------------------------------------|:---|:---------------------------------------------------------------------------------------------------------------------|:---------|
+        | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-7b)                                                         |LLaMA-7B| 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分 | 4.82     |
+        | [LLaMA-13B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b)                                                       |LLaMA-13B| 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分 | 7.03     |
+        | [facat/alpaca-lora-cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b)	                                                                |LLaMA-13B| 基于`decapoda-research/llama-13b-hf`加载`facat/alpaca-lora-cn-13b`LoRA模型后评估测试集并标注得分                                      | 4.07     |  
+        | [Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco](https://huggingface.co/Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco) |LLaMA-13B| 基于`decapoda-research/llama-13b-hf`加载`Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco`LoRA模型后评估测试集并标注得分      | 3.92     |
+        | [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                                                                                       |ChatGLM-6B| 基于原生`THUDM/chatglm-6b`评估测试集得分                                                                                        | **7.08** |
+        | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)                                           |ChatGLM-6B| 基于`THUDM/chatglm-6b`加载`shibing624/chatglm-6b-belle-zh-lora`LoRA模型后评估测试集得分                                            | 6.97     |
+        
+        - 评估case，详见在线文档：中文LLM-benchmark多任务评估集(腾讯文档) https://docs.qq.com/sheet/DUUpsREtWbFBsUVJE?tab=BB08J2  感谢韩俊明、[杨家铭](https://github.com/yangjiam)等同学的标注
+        - 评估任务类型包括：知识问答，开放式问答，数值计算，诗词、音乐、体育，娱乐，写文章，文本翻译，代码编程，伦理、拒答类，多轮问答，Score 评分是前100条（10分制）的平均分数，越高越好
+        - 评估脚本：[tests/test_benchmark.py](https://github.com/shibing624/textgen/blob/main/tests/test_benchmark.py)
+        - 结论：当前在[中文LLM-benchmark多任务评估集](https://docs.qq.com/sheet/DUUpsREtWbFBsUVJE?tab=BB08J2)上，ChatGLM-6B的表现最好，LLaMA-13B-Chinese-Alpaca的表现次之，LLaMA-7B的表现整体都差些，说明ChatGLM这种原生的中文预训练模型更理解中文语义，LLaMA-13B-Chinese-Aplaca是在原版LLaMA上扩充了中文词表，并融入了约20G的通用中文语料后的指令微调模型，表明了LLaMA-13B的底座优秀，具有强大的迁移能力
         
-        ## 🚀Demo
+        ## 🚀 Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         
         ```shell
         python examples/gradio_demo.py
         ```
         
         model trained by [examples/t5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb)
         
-        ## 💾Install
+        ## 💾 Install
         
         ```shell
-        pip install git+https://github.com/huggingface/transformers
         pip install git+https://github.com/huggingface/peft
         pip install -U textgen
         ```
         
         or
         
         ```shell
         pip install torch # conda install pytorch
         git clone https://github.com/shibing624/textgen.git
         cd textgen
         python setup.py install
         ```
         
-        ## 😎Usage
-        
-        ### ChatGLM-6B LoRA 模型
+        ## ▶️ Usage
         
-        安装最新开发版的peft库，支持LoRA模型
-        
-        ```shell
-        pip install git+https://github.com/huggingface/peft
-        ```
+        ### ChatGLM-6B 模型
         
-        #### 使用ChatGLM-6B LoRA微调后的模型
+        #### 使用 ChatGLM-6B 微调后的模型
         
         example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
         
         ```python
-        import sys
-        
-        sys.path.append('../..')
         from textgen import ChatGlmModel
         
-        model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
+        model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-csc-zh-lora")
         r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
         print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
         ```
         
         PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
         
-        #### 训练ChatGLM-6B LoRA模型
+        #### 训练 ChatGLM-6B 微调模型
         
-        支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
+        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
+        3. 支持多卡训练，支持混合精度训练
         
         example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
         
-        ### LLAMA LoRA 模型
-        
-        安装最新开发版的transformers和peft库，支持LLAMA、LoRA模型
-        
-        ```shell
-        pip install transformers>=4.28.1
-        pip install git+https://github.com/huggingface/peft
-        ```
+        ### LLaMA 模型
         
-        #### 使用LLAMA LoRA微调后的模型
+        #### 使用 LLaMA 微调后的模型
         
         example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import LlamaModel
         
         
         def generate_prompt(instruction):
-            return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
+          return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
         
         
-        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
+        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
         predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
         r = model.predict([predict_sentence])
         print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
-        #### 训练LLAMA LoRA模型
+        </details>
+        
+        #### 训练 LLaMA 微调模型
+        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
+        3. 支持多卡训练，支持混合精度训练
         
         example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
         
+        #### 基于微调(LoRA)模型继续训练
+        如果需要基于Lora模型继续训练，可以使用下面的脚本合并模型为新的base model，再微调训练即可。
+        
+        单LoRA权重合并（适用于 Chinese-LLaMA, Chinese-LLaMA-Plus, Chinese-Alpaca）
+        
+        执行以下命令：
+        ```shell
+        python -m textgen/llama/merge_llama_with_chinese_lora.py \
+            --base_model path_to_original_llama_hf_dir \
+            --lora_model path_to_chinese_llama_or_alpaca_lora \
+            --output_type [pth|huggingface]
+            --output_dir path_to_output_dir 
+        ```
+        参数说明：
+        ```
+        --base_model：存放HF格式的LLaMA模型权重和配置文件的目录
+        --lora_model：中文LLaMA/Alpaca LoRA解压后文件所在目录，也可使用HF上的Lora模型名称，如`ziqingyang/chinese-alpaca-lora-7b`会自动下载对应模型
+        --output_type: 指定输出格式，可为pth或huggingface。若不指定，默认为pth
+        --output_dir：指定保存全量模型权重的目录，默认为./
+        --offload_dir（可选）：对于低内存用户需要指定一个offload缓存路径
+        ```
+        
         ### ConvSeq2Seq 模型
         
         训练并预测ConvSeq2Seq模型：
         
         example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import argparse
         from loguru import logger
         import sys
         
         sys.path.append('../..')
         from textgen.seq2seq.conv_seq2seq_model import ConvSeq2SeqModel
@@ -225,14 +229,16 @@
         output:
         
         ```bash
         inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
         outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
         ```
         
+        </details>
+        
         ### BART 模型
         
         训练并预测BART模型：
         
         example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
         
         output:
@@ -242,14 +248,17 @@
         outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
         ```
         
         ### T5 模型
         
         example: [examples/t5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/t5/training_zh_t5_model_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import argparse
         from loguru import logger
         import pandas as pd
         import sys
         
         sys.path.append('../..')
@@ -339,14 +348,16 @@
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
         ```
         
+        </details>
+        
         ### GPT2 模型
         
         #### 中文GPT2 - 文章生成
         
         使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
         
         example: [examples/gpt2/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_zh_gpt2_demo.py)
@@ -374,14 +385,17 @@
         
         example: [examples/songnet/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)
         
         ### Keyword Text Augmentation(EDA/UDA)
         
         example: [examples/text_augmentation/text_augmentation_demo.py](examples/text_augmentation/text_augmentation_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import sys
         
         sys.path.append('..')
         from textgen.augment import TextAugment
         
         if __name__ == '__main__':
@@ -416,21 +430,25 @@
         主要研究机器学习、深度学习、计算机视觉、智能对话系统相关内容
         random-0.2: ('主要陪陪机器学习、深度学习主要计算机视觉、智能对话系统受限于内容', [('研究', '陪陪', 2, 4), ('、', '主要', 13, 15), ('相关', '受限于', 27, 30)])
         insert-0.2: ('主要研究机器机器学习学习、深度深度学习、计算机视觉、智能对话系统相关内容', [('机器', '机器机器', 4, 8), ('学习', '学习学习', 8, 12), ('深度', '深度深度', 13, 17)])
         delete-0.2: ('主要研究机器学习、深度学习、计算机视觉、对话系统相关内容', [('智能', '', 20, 20)])
         tfidf-0.2: ('一是研究机器学习、深度学习、计算机听觉、智能交谈系统密切相关内容', [('主要', '一是', 0, 2), ('视觉', '听觉', 17, 19), ('对话', '交谈', 22, 24), ('相关', '密切相关', 26, 30)])
         mix-0.2: ('主要研究机器学习、深度学、计算机听觉、智能对话软件系统相关内容', [('学习', '学', 11, 12), ('视觉', '听觉', 16, 18), ('系统', '软件系统', 23, 27)])
         ```
+        </details>
         
         ### TGLS 模型（无监督相似文本生成模型）
         
         无监督的中文电商评论生成：从**电商评论**中提取用户表达观点的短句并进行组合来生成仿真评论。
         
         example: [examples/unsup_generation/unsup_generation_demo.py](examples/unsup_generation/unsup_generation_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import os
         import sys
         
         sys.path.append('..')
         from textgen.unsup_generation import TglsModel, load_list
         
@@ -484,58 +502,85 @@
         希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
         就是精华液太少了，保湿效果不错。
         面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
         ```
         
         前10句是真实用户评论，后10句是生成的。
         
-        ## 📚Dataset 
+        </details>
+        
+        ## 📚 Dataset 
         
         1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
         2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
         3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
         4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
         5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
         
-        ## ☎️Contact
+        <details>
+        <summary>文本生成方法介绍</summary>
+        
+        ### 文本生成方法
+        
+        1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
+        2. language_modeling: GPT2、SongNet、ChatGLM、LLaMA
+        3. t5: T5、CopyT5
+        
+        ### 文本扩增方法
+        
+        #### 词粒度扩增
+        
+        1. UDA，非核心词替换
+        2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
+        
+        #### 句粒度扩增
+        
+        1. 回译（BT, Back Translate）：中文-英文-中文
+        2. GPT2模型续写：短文本->长文本
+        3. BART摘要模型：长文本->短文本
+        4. TGLS：无监督相似文本生成模型
+        
+        </details>
+        
+        ## ☎️ Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        ## 😇Citation
+        ## 😇 Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
           author={Xu Ming},
           year={2021},
           howpublished={\url{https://github.com/shibing624/textgen}},
         }
         ```
         
-        ## 🤗License
+        ## 🤗 License
         
         授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
         
-        ## 😍Contribute
+        ## 😍 Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        ## 💕Acknowledgements 
+        ## 💕 Acknowledgements 
         
         - [PaddlePaddle/ERNIE](https://github.com/PaddlePaddle/ERNIE)
         - [minimaxir/textgenrnn](https://github.com/minimaxir/textgenrnn)
         - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [asyml/texar](https://github.com/asyml/texar)
         - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
         - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
```

### Comparing `textgen-0.2.4/README.md` & `textgen-0.2.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,180 +4,184 @@
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
 [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
 # TextGen
 
-🌈Implementation of Text Generation models.
+🌈 Implementation of Text Generation models.
 
-**textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
+**textgen**实现了多种文本生成模型，包括：LLaMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
 
-**Guide**
-
-- [Feature](#Feature)
-- [Install](#install)
-- [Usage](#usage)
-- [Contact](#Contact)
-- [License](#License)
-
-## 😊Feature
-
-### 文本生成
-
-1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
-2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
-3. t5: T5、CopyT5
-
-### 文本扩增
-
-#### 词粒度扩增
-
-1. UDA，非核心词替换
-2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
-
-#### 句粒度扩增
-
-1. 回译（BT, Back Translate）：中文-英文-中文
-2. GPT2模型续写：短文本->长文本
-3. BART摘要模型：长文本->短文本
-4. TGLS：无监督相似文本生成模型
-
-### 功能列表
+## 😊 Feature
 
 - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
-- [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-- [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
-- [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
+- [LLaMA](textgen/llama)：本项目基于PyTorch实现了LLaMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
+- [UDA/EDA](textgen/augment/word_level_augment.py)：本项目实现了UDA(非核心词替换)、EDA和Back Translation(回译)算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
 - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
 - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
 - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
 - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
 - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
 
 ### Release Models
 
 release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
 
 
-|Model| Arch       |Introduce| Training                                                                                                                                     | Inference                                                                                                             | 
-|:-- |:-----------|:--- |:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
-|[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5         |中文NLP多任务Prompt模型| [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
-|[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5         |fine-tuned中文对联后的模型| [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
-|[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet    |SongNet预训练模型| -                                                                                                                                            | -                                                                                                                     |
-|[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet    |fine-tuned宋词后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
-|[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet    |fine-tuned对联后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
-|[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B |在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
-|[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
-|[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLAMA-13B  |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+|Model| Arch          | Introduce                                                                                                                                                        | Training                                                                                                                                     | Inference                                                                                                             | 
+|:-- |:--------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
+|[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5            | 中文NLP多任务Prompt模型                                                                                                                                                 | [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
+|[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5            | fine-tuned中文对联后的模型                                                                                                                                               | [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
+|[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet       | SongNet预训练模型                                                                                                                                                     | -                                                                                                                                            | -                                                                                                                     |
+|[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet       | fine-tuned宋词后的模型                                                                                                                                                 | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
+|[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet       | fine-tuned对联后的模型                                                                                                                                                 | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+|[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B    | 在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重                                                | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
+|[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B    | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重                   | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
+|[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLaMA-13B     | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重                    | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+|[shibing624/chinese-alpaca-plus-7b](https://huggingface.co/shibing624/chinese-alpaca-plus-7b)| LLaMA-7B-plus | [中文LLaMA, Alpaca Plus版（7B）](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型  | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
+
+### Evaluation
+
+| Model                                                                                                                                       |Arch| Introduce                                                                                                            | Score    |
+|:--------------------------------------------------------------------------------------------------------------------------------------------|:---|:---------------------------------------------------------------------------------------------------------------------|:---------|
+| [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-7b)                                                         |LLaMA-7B| 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分 | 4.82     |
+| [LLaMA-13B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b)                                                       |LLaMA-13B| 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分 | 7.03     |
+| [facat/alpaca-lora-cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b)	                                                                |LLaMA-13B| 基于`decapoda-research/llama-13b-hf`加载`facat/alpaca-lora-cn-13b`LoRA模型后评估测试集并标注得分                                      | 4.07     |  
+| [Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco](https://huggingface.co/Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco) |LLaMA-13B| 基于`decapoda-research/llama-13b-hf`加载`Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco`LoRA模型后评估测试集并标注得分      | 3.92     |
+| [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                                                                                       |ChatGLM-6B| 基于原生`THUDM/chatglm-6b`评估测试集得分                                                                                        | **7.08** |
+| [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)                                           |ChatGLM-6B| 基于`THUDM/chatglm-6b`加载`shibing624/chatglm-6b-belle-zh-lora`LoRA模型后评估测试集得分                                            | 6.97     |
+
+- 评估case，详见在线文档：中文LLM-benchmark多任务评估集(腾讯文档) https://docs.qq.com/sheet/DUUpsREtWbFBsUVJE?tab=BB08J2  感谢韩俊明、[杨家铭](https://github.com/yangjiam)等同学的标注
+- 评估任务类型包括：知识问答，开放式问答，数值计算，诗词、音乐、体育，娱乐，写文章，文本翻译，代码编程，伦理、拒答类，多轮问答，Score 评分是前100条（10分制）的平均分数，越高越好
+- 评估脚本：[tests/test_benchmark.py](https://github.com/shibing624/textgen/blob/main/tests/test_benchmark.py)
+- 结论：当前在[中文LLM-benchmark多任务评估集](https://docs.qq.com/sheet/DUUpsREtWbFBsUVJE?tab=BB08J2)上，ChatGLM-6B的表现最好，LLaMA-13B-Chinese-Alpaca的表现次之，LLaMA-7B的表现整体都差些，说明ChatGLM这种原生的中文预训练模型更理解中文语义，LLaMA-13B-Chinese-Aplaca是在原版LLaMA上扩充了中文词表，并融入了约20G的通用中文语料后的指令微调模型，表明了LLaMA-13B的底座优秀，具有强大的迁移能力
 
-## 🚀Demo
+## 🚀 Demo
 
 HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
 
 ![](docs/hf.png)
 
 run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
 
 ```shell
 python examples/gradio_demo.py
 ```
 
 model trained by [examples/t5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb)
 
-## 💾Install
+## 💾 Install
 
 ```shell
-pip install git+https://github.com/huggingface/transformers
 pip install git+https://github.com/huggingface/peft
 pip install -U textgen
 ```
 
 or
 
 ```shell
 pip install torch # conda install pytorch
 git clone https://github.com/shibing624/textgen.git
 cd textgen
 python setup.py install
 ```
 
-## 😎Usage
-
-### ChatGLM-6B LoRA 模型
+## ▶️ Usage
 
-安装最新开发版的peft库，支持LoRA模型
-
-```shell
-pip install git+https://github.com/huggingface/peft
-```
+### ChatGLM-6B 模型
 
-#### 使用ChatGLM-6B LoRA微调后的模型
+#### 使用 ChatGLM-6B 微调后的模型
 
 example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
 
 ```python
-import sys
-
-sys.path.append('../..')
 from textgen import ChatGlmModel
 
-model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
+model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-csc-zh-lora")
 r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
 print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
 ```
 
 PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
 
-#### 训练ChatGLM-6B LoRA模型
+#### 训练 ChatGLM-6B 微调模型
 
-支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
+1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
+3. 支持多卡训练，支持混合精度训练
 
 example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
 
-### LLAMA LoRA 模型
-
-安装最新开发版的transformers和peft库，支持LLAMA、LoRA模型
-
-```shell
-pip install transformers>=4.28.1
-pip install git+https://github.com/huggingface/peft
-```
+### LLaMA 模型
 
-#### 使用LLAMA LoRA微调后的模型
+#### 使用 LLaMA 微调后的模型
 
 example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
 
+<details>
+<summary>show code example and result</summary>
+
 ```python
 import sys
 
 sys.path.append('../..')
 from textgen import LlamaModel
 
 
 def generate_prompt(instruction):
-    return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
+  return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
 
 
-model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
+model = LlamaModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
 predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
 r = model.predict([predict_sentence])
 print(r)  # ['地球是唯一一颗拥有生命的行星。']
 ```
 
-#### 训练LLAMA LoRA模型
+</details>
+
+#### 训练 LLaMA 微调模型
+1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
+3. 支持多卡训练，支持混合精度训练
 
 example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
 
+#### 基于微调(LoRA)模型继续训练
+如果需要基于Lora模型继续训练，可以使用下面的脚本合并模型为新的base model，再微调训练即可。
+
+单LoRA权重合并（适用于 Chinese-LLaMA, Chinese-LLaMA-Plus, Chinese-Alpaca）
+
+执行以下命令：
+```shell
+python -m textgen/llama/merge_llama_with_chinese_lora.py \
+    --base_model path_to_original_llama_hf_dir \
+    --lora_model path_to_chinese_llama_or_alpaca_lora \
+    --output_type [pth|huggingface]
+    --output_dir path_to_output_dir 
+```
+参数说明：
+```
+--base_model：存放HF格式的LLaMA模型权重和配置文件的目录
+--lora_model：中文LLaMA/Alpaca LoRA解压后文件所在目录，也可使用HF上的Lora模型名称，如`ziqingyang/chinese-alpaca-lora-7b`会自动下载对应模型
+--output_type: 指定输出格式，可为pth或huggingface。若不指定，默认为pth
+--output_dir：指定保存全量模型权重的目录，默认为./
+--offload_dir（可选）：对于低内存用户需要指定一个offload缓存路径
+```
+
 ### ConvSeq2Seq 模型
 
 训练并预测ConvSeq2Seq模型：
 
 example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
 
+<details>
+<summary>show code example and result</summary>
+
 ```python
 import argparse
 from loguru import logger
 import sys
 
 sys.path.append('../..')
 from textgen.seq2seq.conv_seq2seq_model import ConvSeq2SeqModel
@@ -217,14 +221,16 @@
 output:
 
 ```bash
 inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
 outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
 ```
 
+</details>
+
 ### BART 模型
 
 训练并预测BART模型：
 
 example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
 
 output:
@@ -234,14 +240,17 @@
 outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
 ```
 
 ### T5 模型
 
 example: [examples/t5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/t5/training_zh_t5_model_demo.py)
 
+<details>
+<summary>show code example and result</summary>
+
 ```python
 import argparse
 from loguru import logger
 import pandas as pd
 import sys
 
 sys.path.append('../..')
@@ -331,14 +340,16 @@
 output:
 
 ```shell
 inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
 outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
 ```
 
+</details>
+
 ### GPT2 模型
 
 #### 中文GPT2 - 文章生成
 
 使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
 
 example: [examples/gpt2/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_zh_gpt2_demo.py)
@@ -366,14 +377,17 @@
 
 example: [examples/songnet/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)
 
 ### Keyword Text Augmentation(EDA/UDA)
 
 example: [examples/text_augmentation/text_augmentation_demo.py](examples/text_augmentation/text_augmentation_demo.py)
 
+<details>
+<summary>show code example and result</summary>
+
 ```python
 import sys
 
 sys.path.append('..')
 from textgen.augment import TextAugment
 
 if __name__ == '__main__':
@@ -408,21 +422,25 @@
 主要研究机器学习、深度学习、计算机视觉、智能对话系统相关内容
 random-0.2: ('主要陪陪机器学习、深度学习主要计算机视觉、智能对话系统受限于内容', [('研究', '陪陪', 2, 4), ('、', '主要', 13, 15), ('相关', '受限于', 27, 30)])
 insert-0.2: ('主要研究机器机器学习学习、深度深度学习、计算机视觉、智能对话系统相关内容', [('机器', '机器机器', 4, 8), ('学习', '学习学习', 8, 12), ('深度', '深度深度', 13, 17)])
 delete-0.2: ('主要研究机器学习、深度学习、计算机视觉、对话系统相关内容', [('智能', '', 20, 20)])
 tfidf-0.2: ('一是研究机器学习、深度学习、计算机听觉、智能交谈系统密切相关内容', [('主要', '一是', 0, 2), ('视觉', '听觉', 17, 19), ('对话', '交谈', 22, 24), ('相关', '密切相关', 26, 30)])
 mix-0.2: ('主要研究机器学习、深度学、计算机听觉、智能对话软件系统相关内容', [('学习', '学', 11, 12), ('视觉', '听觉', 16, 18), ('系统', '软件系统', 23, 27)])
 ```
+</details>
 
 ### TGLS 模型（无监督相似文本生成模型）
 
 无监督的中文电商评论生成：从**电商评论**中提取用户表达观点的短句并进行组合来生成仿真评论。
 
 example: [examples/unsup_generation/unsup_generation_demo.py](examples/unsup_generation/unsup_generation_demo.py)
 
+<details>
+<summary>show code example and result</summary>
+
 ```python
 import os
 import sys
 
 sys.path.append('..')
 from textgen.unsup_generation import TglsModel, load_list
 
@@ -476,58 +494,85 @@
 希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
 就是精华液太少了，保湿效果不错。
 面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
 ```
 
 前10句是真实用户评论，后10句是生成的。
 
-## 📚Dataset 
+</details>
+
+## 📚 Dataset 
 
 1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
 2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
 3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
 4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
 5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
 
-## ☎️Contact
+<details>
+<summary>文本生成方法介绍</summary>
+
+### 文本生成方法
+
+1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
+2. language_modeling: GPT2、SongNet、ChatGLM、LLaMA
+3. t5: T5、CopyT5
+
+### 文本扩增方法
+
+#### 词粒度扩增
+
+1. UDA，非核心词替换
+2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
+
+#### 句粒度扩增
+
+1. 回译（BT, Back Translate）：中文-英文-中文
+2. GPT2模型续写：短文本->长文本
+3. BART摘要模型：长文本->短文本
+4. TGLS：无监督相似文本生成模型
+
+</details>
+
+## ☎️ Contact
 
 - Issue(建议)
   ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
 
 <img src="docs/wechat.jpeg" width="200" />
 
-## 😇Citation
+## 😇 Citation
 
 如果你在研究中使用了textgen，请按如下格式引用：
 
 ```latex
 @misc{textgen,
   title={textgen: Text Generation Tool},
   author={Xu Ming},
   year={2021},
   howpublished={\url{https://github.com/shibing624/textgen}},
 }
 ```
 
-## 🤗License
+## 🤗 License
 
 授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
 
-## 😍Contribute
+## 😍 Contribute
 
 项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
 
 - 在`tests`添加相应的单元测试
 - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
 
 之后即可提交PR。
 
-## 💕Acknowledgements 
+## 💕 Acknowledgements 
 
 - [PaddlePaddle/ERNIE](https://github.com/PaddlePaddle/ERNIE)
 - [minimaxir/textgenrnn](https://github.com/minimaxir/textgenrnn)
 - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
 - [asyml/texar](https://github.com/asyml/texar)
 - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
 - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
```

### Comparing `textgen-0.2.4/setup.py` & `textgen-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='textgen',
-    version='0.2.4',
+    version='0.2.5',
     description='Text Generation Model',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='XuMing',
     author_email='xuming624@qq.com',
     url='https://github.com/shibing624/textgen',
     license="Apache 2.0",
```

### Comparing `textgen-0.2.4/textgen/__init__.py` & `textgen-0.2.5/textgen/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description: 
 """
 
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 
 from textgen.augment.text_augment import TextAugment
 
 from textgen.config.model_args import LanguageGenerationArgs
 from textgen.language_generation.language_generation_model import LanguageGenerationModel
 
 from textgen.config.model_args import LanguageModelingArgs
@@ -28,12 +28,15 @@
 
 from textgen.config.model_args import CopyT5Args
 from textgen.t5.copyt5_model import CopyT5Model
 from textgen.t5.copyt5_utils import ZHTokenizer
 
 from textgen.unsup_generation.tgls_model import TglsModel
 
-from textgen.chatglm.chatglm_model import ChatGlmModel
 from textgen.config.model_args import ChatGlmArgs
+from textgen.chatglm.chatglm_model import ChatGlmModel
 
-from textgen.llama.llama_model import LlamaModel
 from textgen.config.model_args import LlamaArgs
+from textgen.llama.llama_model import LlamaModel
+
+from textgen.config.model_args import BloomArgs
+from textgen.bloom.bloom_model import BloomModel
```

### Comparing `textgen-0.2.4/textgen/augment/sentence_level_augment.py` & `textgen-0.2.5/textgen/augment/sentence_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/augment/text_augment.py` & `textgen-0.2.5/textgen/augment/text_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/augment/tokenizer.py` & `textgen-0.2.5/textgen/augment/tokenizer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/augment/translate_api.py` & `textgen-0.2.5/textgen/augment/translate_api.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/augment/word_level_augment.py` & `textgen-0.2.5/textgen/augment/word_level_augment.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/augment/word_vocab.py` & `textgen-0.2.5/textgen/augment/word_vocab.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/chatglm/chatglm_model.py` & `textgen-0.2.5/textgen/chatglm/chatglm_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,30 +36,30 @@
     "chatglm": (AutoConfig, AutoModel, AutoTokenizer),
 }
 
 
 class ChatGlmModel:
     def __init__(
             self,
-            model_type,
-            model_name,
-            lora_name=None,
+            model_type="chatglm",
+            model_name="THUDM/chatglm-6b",
+            peft_name=None,
             args=None,
             use_cuda=has_cuda,
             cuda_device=-1,
             **kwargs,
     ):
 
         """
         Initializes a ChatGLMModel model.
 
         Args:
             model_type: The type of model (chatglm)
             model_name: The exact architecture and trained weights to use. This may be a Hugging Face Transformers compatible pre-trained model, a community model, or the path to a directory containing model files.
-            lora_name (optional): Lora name
+            peft_name (optional): Lora name
             args (optional): Default args will be used if this parameter is not provided. If provided, it should be a dict containing the args that should be changed in the default args.
             use_cuda (optional): Use GPU if available. Setting to False will force model to use CPU only.
             cuda_device (int, optional): Specific GPU that should be used. Will use the first available GPU by default.
             **kwargs (optional): For providing proxies, force_download, resume_download, cache_dir and other options specific to the 'from_pretrained' implementation where this will be supplied.
         """  # noqa: ignore flake8"
         model_type = model_type.lower()
         self.args = self._load_model_args(model_name)
@@ -68,49 +68,56 @@
             self.args.update_from_dict(args)
         elif isinstance(args, ChatGlmArgs):
             self.args = args
         if self.args.manual_seed:
             random.seed(self.args.manual_seed)
             np.random.seed(self.args.manual_seed)
             torch.manual_seed(self.args.manual_seed)
-            if self.args.n_gpu > 0:
+            if torch.cuda.is_available() > 0:
                 torch.cuda.manual_seed_all(self.args.manual_seed)
 
         if use_cuda:
             if torch.cuda.is_available():
                 if cuda_device == -1:
                     self.device = torch.device("cuda")
                 else:
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
         if self.device == "cpu":
             self.args.fp16 = False
             self.args.int8 = False
 
+        world_size = int(os.environ.get("WORLD_SIZE", 1))
+        self.ddp = world_size != 1
+        if self.ddp:
+            device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
+
         self.results = {}
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
         config = AutoConfig.from_pretrained(model_name, trust_remote_code=True, **kwargs)
 
         self.model = model_class.from_pretrained(
             model_name,
             config=config,
             trust_remote_code=True,
             load_in_8bit=self.args.int8,
+            torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
         )
-        if self.args.fp16:
-            self.model.half()
         self.model.to(self.device)
 
         if self.args.quantization_bit:
             logger.debug(f"Quantized to {self.args.quantization_bit} bit")
             self.model = self.model.quantize(self.args.quantization_bit)
         self.tokenizer_class = tokenizer_class
         if self.args.tokenizer_name:
@@ -121,20 +128,17 @@
 
         self.args.model_type = model_type
         if model_name is None:
             self.args.model_name = "ChatGLM_from_scratch"
         else:
             self.args.model_name = model_name
 
-        self.lora_name = lora_name
-        if self.args.use_lora:
-            self.load_lora()
-
-        if torch.__version__ >= "2" and sys.platform != "win32":
-            self.model = torch.compile(self.model)
+        self.peft_name = peft_name
+        if self.args.use_peft:
+            self.load_peft_model()
 
     def data_collator(self, batch):
         """Data collator that will dynamically pad the inputs received."""
         len_ids = [len(example) for example in batch]
         longest = max(len_ids)
         input_ids = []
         labels_list = []
@@ -205,25 +209,83 @@
         if torch.cuda.device_count() > 1:
             self.model.is_parallelizable = True
             self.model.model_parallel = True
         self.model.lm_head = CastOutputToFloat(self.model.lm_head)
         self.model.config.use_cache = False
         resume_from_checkpoint = self.args.resume_from_checkpoint
 
-        # setup peft, add lora config
-        if self.args.use_lora:
-            peft_config = LoraConfig(
-                task_type=TaskType.CAUSAL_LM,
-                inference_mode=False,
-                r=self.args.lora_r,
-                lora_alpha=self.args.lora_alpha,
-                lora_dropout=self.args.lora_dropout,
-                target_modules=self.args.lora_target_modules,
-                bias=self.args.lora_bias,
-            )
+        # setup peft
+        if self.args.use_peft:
+            peft_type = self.args.peft_type.upper()
+            logger.info(f"Using PEFT type: {peft_type}")
+            # add peft config
+            if peft_type == 'LORA':
+                peft_config = LoraConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    inference_mode=False,
+                    r=self.args.lora_r,
+                    lora_alpha=self.args.lora_alpha,
+                    lora_dropout=self.args.lora_dropout,
+                    target_modules=self.args.lora_target_modules,
+                    bias=self.args.lora_bias,
+                )
+            elif peft_type == 'ADALORA':
+                from peft import AdaLoraConfig
+
+                peft_config = AdaLoraConfig(
+                    init_r=self.args.adalora_init_r,
+                    r=self.args.lora_r,
+                    beta1=self.args.lora_beta,
+                    beta2=self.args.lora_beta,
+                    tinit=self.args.adalora_tinit,
+                    tfinal=self.args.adalora_tfinal,
+                    deltaT=self.args.adalora_delta_t,
+                    lora_alpha=self.args.lora_alpha,
+                    lora_dropout=self.args.lora_dropout,
+                    target_modules=self.args.lora_target_modules,
+                    task_type=TaskType.CAUSAL_LM,
+                    inference_mode=False,
+                )
+            elif peft_type == 'PROMPT_TUNING':
+                from peft import PromptTuningConfig
+
+                peft_config = PromptTuningConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    num_virtual_tokens=self.args.num_virtual_tokens,
+                )
+            elif peft_type == 'P_TUNING':
+                from peft import PromptEncoderConfig
+
+                peft_config = PromptEncoderConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    num_virtual_tokens=self.args.num_virtual_tokens,
+                    encoder_hidden_size=self.args.prompt_encoder_hidden_size
+                )
+            elif peft_type == 'PREFIX_TUNING':
+                from peft import PrefixTuningConfig
+
+                peft_config = PrefixTuningConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    num_virtual_tokens=self.args.num_virtual_tokens,
+                    encoder_hidden_size=self.args.prompt_encoder_hidden_size,
+                    prefix_projection=True,
+                )
+                self.model.gradient_checkpointing_disable()
+            else:
+                logger.warning(f"Wrong type of peft. Set to default lora")
+                peft_config = LoraConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    inference_mode=False,
+                    r=self.args.lora_r,
+                    lora_alpha=self.args.lora_alpha,
+                    lora_dropout=self.args.lora_dropout,
+                    target_modules=self.args.lora_target_modules,
+                    bias=self.args.lora_bias,
+                )
+
             if self.args.int8:
                 self.model = prepare_model_for_int8_training(self.model)
             self.model = get_peft_model(self.model, peft_config)
 
             if resume_from_checkpoint:
                 # Check the available weights and load them
                 checkpoint_name = os.path.join(resume_from_checkpoint, "pytorch_model.bin")  # Full checkpoint
@@ -233,15 +295,15 @@
                     resume_from_checkpoint = (
                         False  # So the trainer won't try loading its state
                     )
                 # The two files above have a different name depending on how they were saved, but are actually the same.
                 if os.path.exists(checkpoint_name):
                     logger.info(f"Restarting from {checkpoint_name}")
                     adapters_weights = torch.load(checkpoint_name)
-                    self.model = set_peft_model_state_dict(self.model, adapters_weights)
+                    set_peft_model_state_dict(self.model, adapters_weights)
                 else:
                     logger.warning(f"Checkpoint {checkpoint_name} not found")
 
             self.model.print_trainable_parameters()  # Be more transparent about the % of trainable params.
         else:
             logger.warning("Now full model params fine-tune, which is slow, set `use_lora=True` for lora fine-tune.")
         os.makedirs(output_dir, exist_ok=True)
@@ -293,16 +355,17 @@
             train_dataset=train_dataset,
             eval_dataset=eval_dataset if eval_data is not None else None,
             args=training_args,
             tokenizer=self.tokenizer,
             data_collator=self.data_collator,
         )
 
-        if torch.__version__ >= "2" and sys.platform != "win32":
-            self.model = torch.compile(self.model)
+        if self.args.enable_torch_compile:
+            if torch.__version__ >= "2" and sys.platform != "win32":
+                self.model = torch.compile(self.model)
 
         logger.info("*** Train ***")
         (global_step, training_loss, metrics) = trainer.train(resume_from_checkpoint=resume_from_checkpoint)
         self.handle_metrics("train", metrics, self.args.output_dir)
         self.results.update(metrics)
         self.save_model(model=self.model)
 
@@ -330,28 +393,36 @@
         for key in sorted(metrics.keys()):
             logger.info(f"  {key} = {metrics[key]}")
         output_file = os.path.join(output_dir, f"{split}_results.txt")
         with open(output_file, "w") as writer:
             for key in sorted(metrics.keys()):
                 writer.write("{} = {}\n".format(key, str(metrics[key])))
 
-    def load_lora(self):
-        """Load lora model."""
-        if self.lora_name:
-            self.model = PeftModel.from_pretrained(self.model, self.lora_name)
-            logger.info(f"Loaded lora model from {self.lora_name}")
-        else:
-            lora_path = os.path.join(self.args.output_dir, self.args.lora_bin_name)
-            if lora_path and os.path.exists(lora_path):
-                self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
-                logger.info(f"Loaded lora model from {lora_path}")
+    def load_peft_model(self):
+        """Load peft model."""
+        if self.peft_name:
+            self.model = PeftModel.from_pretrained(
+                self.model,
+                self.peft_name,
+                torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
+            )
+            logger.info(f"Loaded peft model from {self.peft_name}")
+        # load peft model from local
+        peft_path = os.path.join(self.args.output_dir, self.args.peft_bin_name)
+        if peft_path and os.path.exists(peft_path):
+            self.model = PeftModel.from_pretrained(
+                self.model,
+                self.args.output_dir,
+                torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
+            )
+            logger.info(f"Loaded peft model from {peft_path}")
 
     def process_response(self, response):
         """Process response text."""
-        response = response.strip().replace("[[训练时间]]", "2023年")
+        response = response.strip()
         punkts = [
             [",", "，"],
             ["!", "！"],
             [":", "："],
             [";", "；"],
             ["\\?", "？"],
         ]
```

### Comparing `textgen-0.2.4/textgen/chatglm/chatglm_utils.py` & `textgen-0.2.5/textgen/chatglm/chatglm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         dataset = dataset['train']
         if mode == 'dev' and args.max_eval_samples is not None:
             max_eval_samples = min(len(dataset), args.max_eval_samples)
             dataset = dataset.select(range(max_eval_samples))
     else:
         dataset = HFDataset.from_pandas(data)
 
-    dataset = dataset.map(
+    dataset = dataset.shuffle().map(
         lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
         batched=False, remove_columns=dataset.column_names
     ).filter(lambda x: tokenizer.gmask_token_id in list(x['input_ids']))  # exclude samples without gmask
 
     dataset.set_format(type="np", columns=["input_ids"])
 
     return dataset["input_ids"]
```

### Comparing `textgen-0.2.4/textgen/config/global_args.py` & `textgen-0.2.5/textgen/config/global_args.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/config/model_args.py` & `textgen-0.2.5/textgen/config/model_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -362,31 +362,39 @@
     repetition_penalty: float = 1.0
     temperature: float = 0.95
     special_tokens_list: list = field(default_factory=list)
     top_k: float = None
     top_p: float = 0.7
     model_name_or_path: Optional[str] = field(default="THUDM/chatglm-6b")
     dataset_name_or_path: Optional[str] = field(default="shibing624/alpaca-zh")
-    use_lora: bool = True
-    lora_bin_name: str = field(default="adapter_model.bin")
+    use_peft: bool = True
+    peft_type: str = "LORA"
+    peft_bin_name: str = "adapter_model.bin"
     lora_r: int = 8
     lora_alpha = 16
     lora_dropout = 0.05
     lora_target_modules = ["query_key_value"]
     lora_bias = "none"
-    only_lora_state_dict: bool = False
+    adalora_init_r: int = 12
+    adalora_tinit: int = 200
+    adalora_tfinal: int = 1000
+    adalora_delta_t: int = 10
+    lora_beta: float = 0.85
+    num_virtual_tokens: int = 20
+    prompt_encoder_hidden_size: int = 128
     num_train_epochs = 1
     max_steps = -1
     per_device_train_batch_size = 2
-    eval_batch_size: int = 2
+    eval_batch_size: int = 4
     gradient_accumulation_steps = 1
     save_total_limit = 3
     remove_unused_columns = False
     logging_steps = 50
     resume_from_checkpoint: str = None
+    enable_torch_compile: bool = False
 
 
 @dataclass
 class LlamaArgs(ModelArgs):
     """
     Model args for a LlamaModel
     """
@@ -411,30 +419,100 @@
     eval_steps: int = 200
     save_steps: int = 400
     pad_to_multiple_of: int = 8
     max_eval_samples: int = 20
     length_penalty: float = 2.0
     num_beams: int = 1
     num_return_sequences: int = 1
-    repetition_penalty: float = 1.0
-    temperature: float = 0.95
+    repetition_penalty: float = 1.3
+    temperature: float = 0.2
     special_tokens_list: list = field(default_factory=list)
-    top_k: float = 30
-    top_p: float = 0.7
+    top_k: float = 40
+    top_p: float = 0.9
     model_name_or_path: Optional[str] = field(default="decapoda-research/llama-7b-hf")
-    use_lora: bool = True
-    lora_bin_name: str = field(default="adapter_model.bin")
+    use_peft: bool = True
+    peft_type: str = "LORA"
+    peft_bin_name: str = "adapter_model.bin"
     lora_r: int = 8
     lora_alpha = 16
     lora_dropout = 0.05
     lora_target_modules = ["q_proj", "k_proj", "v_proj", "o_proj"]
     lora_bias = "none"
-    only_lora_state_dict: bool = True
+    adalora_init_r: int = 12
+    adalora_tinit: int = 200
+    adalora_tfinal: int = 1000
+    adalora_delta_t: int = 10
+    lora_beta: float = 0.85
+    num_virtual_tokens: int = 20
+    prompt_encoder_hidden_size: int = 128
+    num_train_epochs = 3
+    max_steps = -1
+    per_device_train_batch_size = 2
+    eval_batch_size: int = 4
+    gradient_accumulation_steps = 1
+    save_total_limit = 3
+    remove_unused_columns = False
+    logging_steps = 50
+    resume_from_checkpoint: str = None
+    enable_torch_compile: bool = False
+
+@dataclass
+class BloomArgs(ModelArgs):
+    """
+    Model args for a BloomModel
+    """
+
+    model_class: str = "BloomArgs"
+    dataset_class: Dataset = None
+    learning_rate: float = 3e-4
+    fp16: bool = True
+    int8: bool = False
+    quantization_bit: int = None  # if use quantization bit, set 4, else None
+    debug: bool = False
+    max_seq_length: int = 256  # max length of input sequence
+    max_length = 384  # max length of the sequence to be generated
+    do_sample: bool = True
+    early_stopping: bool = True
+    evaluate_generated_text: bool = True
+    is_chat_task: bool = True
+    warmup_steps: int = 50
+    report_to = "tensorboard"
+    optimizer: str = "adamw_torch"
+    save_strategy: str = "steps"
+    eval_steps: int = 200
+    save_steps: int = 400
+    pad_to_multiple_of: int = 8
+    max_eval_samples: int = 20
+    length_penalty: float = 2.0
+    num_beams: int = 1
+    num_return_sequences: int = 1
+    repetition_penalty: float = 1.3
+    temperature: float = 0.2
+    special_tokens_list: list = field(default_factory=list)
+    top_k: float = 40
+    top_p: float = 0.9
+    model_name_or_path: Optional[str] = field(default="bigscience/bloomz-7b1-mt")
+    use_peft: bool = True
+    peft_type: str = "LORA"
+    peft_bin_name: str = "adapter_model.bin"
+    lora_r: int = 8
+    lora_alpha = 16
+    lora_dropout = 0.05
+    lora_target_modules = ["query_key_value"]
+    lora_bias = "none"
+    adalora_init_r: int = 12
+    adalora_tinit: int = 200
+    adalora_tfinal: int = 1000
+    adalora_delta_t: int = 10
+    lora_beta: float = 0.85
+    num_virtual_tokens: int = 20
+    prompt_encoder_hidden_size: int = 128
     num_train_epochs = 3
     max_steps = -1
     per_device_train_batch_size = 2
-    eval_batch_size: int = 2
+    eval_batch_size: int = 4
     gradient_accumulation_steps = 1
     save_total_limit = 3
     remove_unused_columns = False
     logging_steps = 50
     resume_from_checkpoint: str = None
+    enable_torch_compile: bool = False
```

### Comparing `textgen-0.2.4/textgen/custom_models/models.py` & `textgen-0.2.5/textgen/custom_models/models.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/data/HowNetPOSWord.txt` & `textgen-0.2.5/textgen/data/HowNetPOSWord.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/data/stopwords.txt` & `textgen-0.2.5/textgen/data/stopwords.txt`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/language_generation/language_generation_model.py` & `textgen-0.2.5/textgen/language_generation/language_generation_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,18 @@
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
 
         self.args.model_name = model_name
         self.args.model_type = model_type
 
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
```

### Comparing `textgen-0.2.4/textgen/language_generation/language_generation_utils.py` & `textgen-0.2.5/textgen/language_generation/language_generation_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/language_modeling/language_modeling_model.py` & `textgen-0.2.5/textgen/language_modeling/language_modeling_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,18 @@
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     " Make sure CUDA is available or set use_cuda=False."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
         self.results = {}
 
         if not use_cuda:
             self.args.fp16 = False
 
         self.args.model_name = model_name
```

### Comparing `textgen-0.2.4/textgen/language_modeling/language_modeling_utils.py` & `textgen-0.2.5/textgen/language_modeling/language_modeling_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/language_modeling/songnet_model.py` & `textgen-0.2.5/textgen/language_modeling/songnet_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -632,15 +632,18 @@
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
 
         self.results = {}
 
         if cache_folder is None:
             cache_folder = os.getenv('TEXTGEN_HOME')
             if cache_folder is None:
```

### Comparing `textgen-0.2.4/textgen/language_modeling/songnet_utils.py` & `textgen-0.2.5/textgen/language_modeling/songnet_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/llama/llama_model.py` & `textgen-0.2.5/textgen/bloom/bloom_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,151 +1,153 @@
 # -*- coding: utf-8 -*-
 """
 @author:XuMing(xuming624@qq.com)
 @description:
-
-modified from https://github.com/tloen/alpaca-lora/blob/main/finetune.py
 """
 import os
 import random
 import sys
 from typing import List, Tuple
 
 import numpy as np
 import torch
 from loguru import logger
 from peft import (
     get_peft_model,
     LoraConfig,
     TaskType,
     PeftModel,
-    get_peft_model_state_dict,
     prepare_model_for_int8_training,
     set_peft_model_state_dict,
 )
 from tqdm.auto import tqdm
 from transformers import GenerationConfig, DataCollatorForSeq2Seq
-from transformers import LlamaForCausalLM, LlamaTokenizer
+from transformers import BloomForCausalLM, BloomTokenizerFast
 from transformers import Trainer, TrainingArguments, AutoConfig
 from transformers.trainer import TRAINING_ARGS_NAME
 
-from textgen.config.model_args import LlamaArgs
-from textgen.llama.llama_utils import load_hf_dataset, LlamaDataset
+from textgen.config.model_args import BloomArgs
+from textgen.bloom.bloom_utils import load_hf_dataset, BloomDataset
 
 has_cuda = torch.cuda.is_available()
 os.environ["TOKENIZERS_PARALLELISM"] = "FALSE"
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 
 MODEL_CLASSES = {
-    "llama": (AutoConfig, LlamaForCausalLM, LlamaTokenizer),
+    "bloom": (AutoConfig, BloomForCausalLM, BloomTokenizerFast),
 }
 
 
-class LlamaModel:
+class BloomModel:
     def __init__(
             self,
-            model_type,
-            model_name,
-            lora_name=None,
+            model_type="bloom",
+            model_name="bigscience/bloomz-560m",
+            peft_name=None,
             args=None,
             use_cuda=has_cuda,
             cuda_device=-1,
             **kwargs,
     ):
 
         """
-        Initializes a LlamaModel model.
+        Initializes a BloomModel model.
 
         Args:
             model_type: The type of model (llama)
             model_name: The exact architecture and trained weights to use. This may be a Hugging Face Transformers compatible pre-trained model, a community model, or the path to a directory containing model files.
-            lora_name (optional): Lora name
+            peft_name (optional): Peft model name
             args (optional): Default args will be used if this parameter is not provided. If provided, it should be a dict containing the args that should be changed in the default args.
             use_cuda (optional): Use GPU if available. Setting to False will force model to use CPU only.
             cuda_device (int, optional): Specific GPU that should be used. Will use the first available GPU by default.
             **kwargs (optional): For providing proxies, force_download, resume_download, cache_dir and other options specific to the 'from_pretrained' implementation where this will be supplied.
         """  # noqa: ignore flake8"
         model_type = model_type.lower()
         self.args = self._load_model_args(model_name)
 
         if isinstance(args, dict):
             self.args.update_from_dict(args)
-        elif isinstance(args, LlamaArgs):
+        elif isinstance(args, BloomArgs):
             self.args = args
 
         if self.args.manual_seed:
             random.seed(self.args.manual_seed)
             np.random.seed(self.args.manual_seed)
             torch.manual_seed(self.args.manual_seed)
-            if self.args.n_gpu > 0:
+            if torch.cuda.is_available():
                 torch.cuda.manual_seed_all(self.args.manual_seed)
 
         if use_cuda:
             if torch.cuda.is_available():
                 if cuda_device == -1:
                     self.device = torch.device("cuda")
-                    cuda_device = 0
                 else:
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
         if not use_cuda:
             self.args.fp16 = False
             self.args.int8 = False
+        world_size = int(os.environ.get("WORLD_SIZE", 1))
+        self.ddp = world_size != 1
+        if self.ddp:
+            device_map = {"": int(os.environ.get("LOCAL_RANK") or 0)}
 
         self.results = {}
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             model_name = self.args.model_name_or_path
         config = AutoConfig.from_pretrained(model_name, **kwargs)
 
-        device_map = "auto"
-        world_size = int(os.environ.get("WORLD_SIZE", 1))
-        self.ddp = world_size != 1
-        if self.ddp or torch.cuda.device_count() > 1:
-            device_map = {"": int(os.environ.get("LOCAL_RANK") or cuda_device)}
         self.model = model_class.from_pretrained(
             model_name,
             config=config,
             load_in_8bit=self.args.int8,
             torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
-            device_map=device_map,
         )
+        self.model.to(self.device)
 
         self.tokenizer_class = tokenizer_class
         if self.args.tokenizer_name:
             self.tokenizer = tokenizer_class.from_pretrained(self.args.tokenizer_name)
         else:
             self.tokenizer = tokenizer_class.from_pretrained(model_name)
             self.args.tokenizer_name = self.args.model_name
 
         self.args.model_type = model_type
         if model_name is None:
-            self.args.model_name = "Llama_from_scratch"
+            self.args.model_name = "Bloom_from_scratch"
         else:
             self.args.model_name = model_name
 
-        self.lora_name = lora_name
-        if self.args.use_lora:
-            self.load_lora()
-
-        # unwind broken decapoda-research config
-        self.tokenizer.padding_side = "left"
-        self.tokenizer.pad_token_id = 0  # unk. we want this to be different from the eos token
-        self.model.config.pad_token_id = 0  # unk
-        self.model.config.bos_token_id = 1
-        self.model.config.eos_token_id = 2
-        if torch.__version__ >= "2" and sys.platform != "win32":
-            self.model = torch.compile(self.model)
+        self.peft_name = peft_name
+        if self.args.use_peft:
+            self.load_peft_model()
+
+    def resize_model_embeddings(self, tokenizer_vocab_size):
+        """Resizes model embeddings to match the tokenizer vocab size."""
+        model_vocab_size = self.model.get_input_embeddings().weight.size(0)
+        if model_vocab_size != tokenizer_vocab_size:
+            logger.debug(
+                f"Resize model embeddings to fit tokenizer, "
+                f"Vocab of the base model: {model_vocab_size}, "
+                f"Vocab of the tokenizer: {tokenizer_vocab_size}"
+            )
+            self.model.resize_token_embeddings(tokenizer_vocab_size)
+            assert self.model.get_input_embeddings().weight.size(0) == len(self.tokenizer)
+            logger.debug(f"Model token embeddings updated, size: {len(self.tokenizer)}")
 
     def train_model(
             self,
             train_data,
             output_dir=None,
             args=None,
             eval_data=None,
@@ -198,25 +200,83 @@
         if not self.ddp and torch.cuda.device_count() > 1:
             # keeps Trainer from trying its own DataParallelism when more than 1 gpu is available
             self.model.is_parallelizable = True
             self.model.model_parallel = True
         self.model.config.use_cache = False
         resume_from_checkpoint = self.args.resume_from_checkpoint
 
-        # setup peft, add lora config
-        if self.args.use_lora:
-            peft_config = LoraConfig(
-                task_type=TaskType.CAUSAL_LM,
-                inference_mode=False,
-                r=self.args.lora_r,
-                lora_alpha=self.args.lora_alpha,
-                lora_dropout=self.args.lora_dropout,
-                target_modules=self.args.lora_target_modules,
-                bias=self.args.lora_bias,
-            )
+        # setup peft
+        if self.args.use_peft:
+            peft_type = self.args.peft_type.upper()
+            logger.info(f"Using PEFT type: {peft_type}")
+            # add peft config
+            if peft_type == 'LORA':
+                peft_config = LoraConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    inference_mode=False,
+                    r=self.args.lora_r,
+                    lora_alpha=self.args.lora_alpha,
+                    lora_dropout=self.args.lora_dropout,
+                    target_modules=self.args.lora_target_modules,
+                    bias=self.args.lora_bias,
+                )
+            elif peft_type == 'ADALORA':
+                from peft import AdaLoraConfig
+
+                peft_config = AdaLoraConfig(
+                    init_r=self.args.adalora_init_r,
+                    r=self.args.lora_r,
+                    beta1=self.args.lora_beta,
+                    beta2=self.args.lora_beta,
+                    tinit=self.args.adalora_tinit,
+                    tfinal=self.args.adalora_tfinal,
+                    deltaT=self.args.adalora_delta_t,
+                    lora_alpha=self.args.lora_alpha,
+                    lora_dropout=self.args.lora_dropout,
+                    target_modules=self.args.lora_target_modules,
+                    task_type=TaskType.CAUSAL_LM,
+                    inference_mode=False,
+                )
+            elif peft_type == 'PROMPT_TUNING':
+                from peft import PromptTuningConfig
+
+                peft_config = PromptTuningConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    num_virtual_tokens=self.args.num_virtual_tokens,
+                )
+            elif peft_type == 'P_TUNING':
+                from peft import PromptEncoderConfig
+
+                peft_config = PromptEncoderConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    num_virtual_tokens=self.args.num_virtual_tokens,
+                    encoder_hidden_size=self.args.prompt_encoder_hidden_size
+                )
+            elif peft_type == 'PREFIX_TUNING':
+                from peft import PrefixTuningConfig
+
+                peft_config = PrefixTuningConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    num_virtual_tokens=self.args.num_virtual_tokens,
+                    encoder_hidden_size=self.args.prompt_encoder_hidden_size,
+                    prefix_projection=True,
+                )
+                self.model.gradient_checkpointing_disable()
+            else:
+                logger.warning(f"Wrong type of peft. Set to default lora")
+                peft_config = LoraConfig(
+                    task_type=TaskType.CAUSAL_LM,
+                    inference_mode=False,
+                    r=self.args.lora_r,
+                    lora_alpha=self.args.lora_alpha,
+                    lora_dropout=self.args.lora_dropout,
+                    target_modules=self.args.lora_target_modules,
+                    bias=self.args.lora_bias,
+                )
+
             if self.args.int8:
                 self.model = prepare_model_for_int8_training(self.model)
             self.model = get_peft_model(self.model, peft_config)
 
             if resume_from_checkpoint:
                 # Check the available weights and load them
                 checkpoint_name = os.path.join(resume_from_checkpoint, "pytorch_model.bin")  # Full checkpoint
@@ -226,15 +286,15 @@
                     resume_from_checkpoint = (
                         False  # So the trainer won't try loading its state
                     )
                 # The two files above have a different name depending on how they were saved, but are actually the same.
                 if os.path.exists(checkpoint_name):
                     logger.info(f"Restarting from {checkpoint_name}")
                     adapters_weights = torch.load(checkpoint_name)
-                    self.model = set_peft_model_state_dict(self.model, adapters_weights)
+                    set_peft_model_state_dict(self.model, adapters_weights)
                 else:
                     logger.warning(f"Checkpoint {checkpoint_name} not found")
 
             self.model.print_trainable_parameters()  # Be more transparent about the % of trainable params.
         else:
             logger.warning("Now full model params fine-tune, which is slow, set `use_lora=True` for lora fine-tune.")
         os.makedirs(output_dir, exist_ok=True)
@@ -280,36 +340,31 @@
         logger.warning(
             f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}, "
             + f"distributed training: {bool(training_args.local_rank != -1)}, 16-bits training: {training_args.fp16}"
         )
         logger.info(f"Training/evaluation parameters {training_args}")
 
         data_collator = DataCollatorForSeq2Seq(
-            self.tokenizer, pad_to_multiple_of=self.args.pad_to_multiple_of,
-            return_tensors="pt", padding=True
+            self.tokenizer,
+            return_tensors="pt",
+            padding="max_length",
+            max_length=self.args.max_seq_length + self.args.max_length
         )
         trainer = FinetuneTrainer(
             model=self.model,
             train_dataset=train_dataset,
             eval_dataset=eval_dataset if eval_data is not None else None,
             args=training_args,
             tokenizer=self.tokenizer,
             data_collator=data_collator,
         )
 
-        if self.args.only_lora_state_dict:
-            old_state_dict = self.model.state_dict
-            self.model.state_dict = (
-                lambda self, *_, **__: get_peft_model_state_dict(
-                    self, old_state_dict()
-                )
-            ).__get__(self.model, type(self.model))
-
-        if torch.__version__ >= "2" and sys.platform != "win32":
-            self.model = torch.compile(self.model)
+        if self.args.enable_torch_compile:
+            if torch.__version__ >= "2" and sys.platform != "win32":
+                self.model = torch.compile(self.model)
 
         logger.info("*** Train ***")
         (global_step, training_loss, metrics) = trainer.train(resume_from_checkpoint=resume_from_checkpoint)
         self.handle_metrics("train", metrics, self.args.output_dir)
         self.results.update(metrics)
         self.save_model(model=self.model)
 
@@ -346,34 +401,40 @@
         for key in sorted(metrics.keys()):
             logger.info(f"  {key} = {metrics[key]}")
         output_file = os.path.join(output_dir, f"{split}_results.txt")
         with open(output_file, "w") as writer:
             for key in sorted(metrics.keys()):
                 writer.write("{} = {}\n".format(key, str(metrics[key])))
 
-    def load_lora(self):
-        """Load lora model"""
-        if self.lora_name:
-            if os.path.isdir(self.lora_name) and os.path.exists(
-                    os.path.join(self.lora_name, "tokenizer_config.json")):
+    def load_peft_model(self):
+        """Load peft model"""
+        if self.peft_name:
+            if os.path.isdir(self.peft_name) and os.path.exists(
+                    os.path.join(self.peft_name, "tokenizer_config.json")):
                 update_tokenizer = True
             else:
                 update_tokenizer = False
-            if "ziqingyang/chinese" in self.lora_name or update_tokenizer:
-                self.tokenizer = LlamaTokenizer.from_pretrained(self.lora_name)
-                self.model.resize_token_embeddings(len(self.tokenizer))
-                assert self.model.get_input_embeddings().weight.size(0) == len(self.tokenizer)
-                logger.debug(f"Tokenizer updated, vocabulary size: {len(self.tokenizer)}")
-            self.model = PeftModel.from_pretrained(self.model, self.lora_name)
-            logger.info(f"Loaded lora model from {self.lora_name}")
-        else:
-            lora_path = os.path.join(self.args.output_dir, self.args.lora_bin_name)
-            if lora_path and os.path.exists(lora_path):
-                self.model = PeftModel.from_pretrained(self.model, self.args.output_dir)
-                logger.info(f"Loaded lora model from {lora_path}")
+            if update_tokenizer:
+                self.tokenizer = BloomTokenizerFast.from_pretrained(self.peft_name)
+                self.resize_model_embeddings(len(self.tokenizer))
+            self.model = PeftModel.from_pretrained(
+                self.model,
+                self.peft_name,
+                torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
+            )
+            logger.info(f"Loaded peft model from {self.peft_name}")
+        # Load from local
+        peft_path = os.path.join(self.args.output_dir, self.args.peft_bin_name)
+        if peft_path and os.path.exists(peft_path):
+            self.model = PeftModel.from_pretrained(
+                self.model,
+                self.args.output_dir,
+                torch_dtype=torch.float16 if self.args.fp16 else torch.float32,
+            )
+            logger.info(f"Loaded peft model from {peft_path}")
 
     @torch.no_grad()
     def predict(self, sentences: List[str], keep_prompt: bool = False, max_length: int = None, **kwargs):
         """
         Performs predictions on a list of text.
 
         Args:
@@ -453,15 +514,15 @@
         history = history + [(query, response)]
         return response, history
 
     def load_and_cache_examples(
             self, data, evaluate=False, no_cache=False, verbose=True, silent=False
     ):
         """
-        Creates a LlamaDataset from data.
+        Creates a BloomDataset from data.
 
         Utility function for train() and eval() methods. Not intended to be used directly.
         """
 
         tokenizer = self.tokenizer
         args = self.args
 
@@ -476,15 +537,15 @@
         if self.args.use_hf_datasets:
             dataset = load_hf_dataset(data, tokenizer, self.args, mode)
             return dataset
         elif args.dataset_class:
             CustomDataset = args.dataset_class
             return CustomDataset(tokenizer, args, data, mode)
         else:
-            return LlamaDataset(
+            return BloomDataset(
                 tokenizer,
                 self.args,
                 data,
                 mode,
             )
 
     def save_model(
@@ -512,22 +573,22 @@
             self.save_model_args(output_dir)
 
     def save_model_args(self, output_dir):
         os.makedirs(output_dir, exist_ok=True)
         self.args.save(output_dir)
 
     def _load_model_args(self, input_dir):
-        args = LlamaArgs()
+        args = BloomArgs()
         args.load(input_dir)
         return args
 
 
 class FinetuneTrainer(Trainer):
     """
-    Trainer for finetuning models
+    Trainer for finetune models
     """
 
     def save_model(self, output_dir=None, _internal_call=False):
         """Save the LoRA model."""
         os.makedirs(output_dir, exist_ok=True)
         torch.save(self.args, os.path.join(output_dir, TRAINING_ARGS_NAME))
         self.model.save_pretrained(output_dir)
```

### Comparing `textgen-0.2.4/textgen/llama/llama_utils.py` & `textgen-0.2.5/textgen/llama/llama_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,38 +32,35 @@
 
     if input_text:
         prompt = PROMPT_DICT["prompt_input"].format(instruction=instruction, input_text=input_text)
     else:
         prompt = PROMPT_DICT["prompt_no_input"].format(instruction=instruction)
 
     full_prompt = prompt + target_text + tokenizer.eos_token
+    full_max_length = args.max_seq_length + args.max_length
     example = tokenizer(
         full_prompt,
         truncation=True,
-        max_length=args.max_seq_length + args.max_length,
+        max_length=full_max_length,
         padding=False,
-        return_tensors=None,
+        add_special_tokens=False
     )
-    if (
-            example["input_ids"][-1] != tokenizer.eos_token_id
-            and len(example["input_ids"]) < args.max_seq_length + args.max_length
-    ):
-        example["input_ids"].append(tokenizer.eos_token_id)
-        example["attention_mask"].append(1)
     example["labels"] = example["input_ids"].copy()
     if args.is_chat_task:
         user_example = tokenizer(
             prompt,
             truncation=True,
             max_length=args.max_seq_length,
             padding=False,
-            return_tensors=None,
+            add_special_tokens=False
         )
         user_prompt_len = len(user_example["input_ids"])
-        example["labels"] = [-100] * user_prompt_len + example["labels"][user_prompt_len:]
+        # set labels to full max length to adjust for DataCollatorForSeq2Seq padding
+        example["labels"] = [-100] * (full_max_length - len(example['labels']) + user_prompt_len) + \
+                            example["labels"][user_prompt_len:]
 
     return example
 
 
 def preprocess_batch_for_hf_dataset(example, tokenizer, args):
     data = (example["instruction"], example["input"], example["output"], tokenizer, args)
     example = preprocess_data(data)
@@ -87,15 +84,15 @@
         dataset = dataset['train']
         if mode == 'dev' and args.max_eval_samples is not None:
             max_eval_samples = min(len(dataset), args.max_eval_samples)
             dataset = dataset.select(range(max_eval_samples))
     else:
         dataset = HFDataset.from_pandas(data)
 
-    dataset = dataset.map(
+    dataset = dataset.shuffle().map(
         lambda x: preprocess_batch_for_hf_dataset(x, tokenizer=tokenizer, args=args),
         batched=False, remove_columns=dataset.column_names
     ).filter(lambda x: len(x['input_ids']) > 0)
 
     return dataset
```

### Comparing `textgen-0.2.4/textgen/seq2seq/bart_seq2seq_model.py` & `textgen-0.2.5/textgen/seq2seq/bart_seq2seq_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,18 @@
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
 
         self.results = {}
         if not use_cuda:
             self.args.fp16 = False
 
         if encoder_decoder_type in ["rag-token", "rag-sequence"]:
```

### Comparing `textgen-0.2.4/textgen/seq2seq/bart_seq2seq_utils.py` & `textgen-0.2.5/textgen/seq2seq/bart_seq2seq_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/seq2seq/conv_seq2seq_model.py` & `textgen-0.2.5/textgen/seq2seq/conv_seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/seq2seq/data_reader.py` & `textgen-0.2.5/textgen/seq2seq/data_reader.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/seq2seq/seq2seq_model.py` & `textgen-0.2.5/textgen/seq2seq/seq2seq_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/seq2seq/seq2seq_trainer.py` & `textgen-0.2.5/textgen/seq2seq/seq2seq_trainer.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/t5/copyt5_model.py` & `textgen-0.2.5/textgen/t5/copyt5_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,18 @@
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
 
         self.results = {}
         config_class, model_class, tokenizer_class = MODEL_CLASSES[model_type]
         if model_name is None:
             self.config = self.args.config
             self.model = model_class(config=self.config)
```

### Comparing `textgen-0.2.4/textgen/t5/copyt5_utils.py` & `textgen-0.2.5/textgen/t5/copyt5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/t5/t5_model.py` & `textgen-0.2.5/textgen/t5/t5_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,18 @@
                     self.device = torch.device(f"cuda:{cuda_device}")
             else:
                 raise ValueError(
                     "'use_cuda' set to True when cuda is unavailable."
                     "Make sure CUDA is available or set `use_cuda=False`."
                 )
         else:
-            self.device = "cpu"
+            if torch.backends.mps.is_available():
+                self.device = torch.device("mps")
+            else:
+                self.device = "cpu"
         logger.debug(f"Device: {self.device}")
 
         self.results = {}
 
         config_class, model_class = MODEL_CLASSES[model_type]
 
         if model_name is None:
```

### Comparing `textgen-0.2.4/textgen/t5/t5_utils.py` & `textgen-0.2.5/textgen/t5/t5_utils.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/unsup_generation/tgls_model.py` & `textgen-0.2.5/textgen/unsup_generation/tgls_model.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen/unsup_generation/tgls_util.py` & `textgen-0.2.5/textgen/unsup_generation/tgls_util.py`

 * *Files identical despite different names*

### Comparing `textgen-0.2.4/textgen.egg-info/PKG-INFO` & `textgen-0.2.5/textgen.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgen
-Version: 0.2.4
+Version: 0.2.5
 Summary: Text Generation Model
 Home-page: https://github.com/shibing624/textgen
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/textgen.svg)](https://badge.fury.io/py/textgen)
         [![Downloads](https://pepy.tech/badge/textgen)](https://pepy.tech/project/textgen)
@@ -12,180 +12,184 @@
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_version](https://img.shields.io/badge/Python-3.8%2B-green.svg)](requirements.txt)
         [![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
         # TextGen
         
-        🌈Implementation of Text Generation models.
+        🌈 Implementation of Text Generation models.
         
-        **textgen**实现了多种文本生成模型，包括：LLAMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
+        **textgen**实现了多种文本生成模型，包括：LLaMA、ChatGLM、UDA、GPT2、Seq2Seq、BART、T5、SongNet等模型，开箱即用。
         
-        **Guide**
-        
-        - [Feature](#Feature)
-        - [Install](#install)
-        - [Usage](#usage)
-        - [Contact](#Contact)
-        - [License](#License)
-        
-        ## 😊Feature
-        
-        ### 文本生成
-        
-        1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
-        2. language_modeling: GPT2、SongNet、ChatGLM、LLAMA
-        3. t5: T5、CopyT5
-        
-        ### 文本扩增
-        
-        #### 词粒度扩增
-        
-        1. UDA，非核心词替换
-        2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
-        
-        #### 句粒度扩增
-        
-        1. 回译（BT, Back Translate）：中文-英文-中文
-        2. GPT2模型续写：短文本->长文本
-        3. BART摘要模型：长文本->短文本
-        4. TGLS：无监督相似文本生成模型
-        
-        ### 功能列表
+        ## 😊 Feature
         
         - [ChatGLM](textgen/chatglm)：本项目基于PyTorch实现了ChatGLM-6B模型LoRA微调训练和预测，可以用于句子纠错、对话等文本生成任务
-        - [LLAMA](textgen/llama)：本项目基于PyTorch实现了LLAMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
-        - [UDA(非核心词替换)/EDA](textgen/augment/word_level_augment.py)：本项目参考Google的UDA(非核心词替换)算法和EDA算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
-        - [BT(回译)](textgen/augment/sentence_level_augment.py)：本项目基于百度翻译API实现了回译功能，先把中文句子翻译为英文，再把英文翻译为新的中文
+        - [LLaMA](textgen/llama)：本项目基于PyTorch实现了LLaMA模型LoRA微调训练和预测，可以用于多轮对话生成任务
+        - [UDA/EDA](textgen/augment/word_level_augment.py)：本项目实现了UDA(非核心词替换)、EDA和Back Translation(回译)算法，基于TF-IDF将句子中部分不重要词替换为同义词，随机词插入、删除、替换等方法，产生新的文本，实现了文本扩增
         - [Seq2Seq](textgen/seq2seq)：本项目基于PyTorch实现了Seq2Seq、ConvSeq2Seq、BART模型的训练和预测，可以用于文本翻译、对话生成、摘要生成等文本生成任务
         - [T5](textgen/t5)：本项目基于PyTorch实现了T5和CopyT5模型训练和预测，可以用于文本翻译、对话生成、对联生成、文案撰写等文本生成任务
         - [GPT2](textgen/language_modeling)：本项目基于PyTorch实现了GTP2模型训练和预测，可以用于文章生成、对联生成等文本生成任务
         - [SongNet](textgen/language_modeling/songnet_model.py)：本项目基于PyTorch实现了SongNet模型训练和预测，可以用于规范格式的诗词、歌词等文本生成任务
         - [TGLS](textgen/unsup_generation)：本项目实现了[TGLS](https://www.jiqizhixin.com/articles/2020-08-11-5)无监督相似文本生成模型，是一种“先搜索后学习”的文本生成方法，通过反复迭代学习候选集，最终模型能生成类似候选集的高质量相似文本
         
         ### Release Models
         
         release基于`textgen`训练的中文模型，模型已经release到HuggingFace models，指定模型名称`textgen`会自动下载模型，可直接使用。
         
         
-        |Model| Arch       |Introduce| Training                                                                                                                                     | Inference                                                                                                             | 
-        |:-- |:-----------|:--- |:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
-        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5         |中文NLP多任务Prompt模型| [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
-        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5         |fine-tuned中文对联后的模型| [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
-        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet    |SongNet预训练模型| -                                                                                                                                            | -                                                                                                                     |
-        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet    |fine-tuned宋词后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
-        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet    |fine-tuned对联后的模型| [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
-        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B |在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
-        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
-        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLAMA-13B  |在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重| [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+        |Model| Arch          | Introduce                                                                                                                                                        | Training                                                                                                                                     | Inference                                                                                                             | 
+        |:-- |:--------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------|
+        |[shibing624/prompt-t5-base-chinese](https://huggingface.co/shibing624/prompt-t5-base-chinese)| T5            | 中文NLP多任务Prompt模型                                                                                                                                                 | [prompt-t5-base-chinese.md](https://github.com/shibing624/textgen/blob/main/docs/prompt-t5-base-chinese.md)                                  | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_prompt_demo.py)                       |
+        |[shibing624/t5-chinese-couplet](https://huggingface.co/shibing624/t5-chinese-couplet)| T5            | fine-tuned中文对联后的模型                                                                                                                                               | [对联生成模型调研](https://github.com/shibing624/textgen/blob/main/docs/%E5%AF%B9%E8%81%94%E7%94%9F%E6%88%90%E6%A8%A1%E5%9E%8B%E5%AF%B9%E6%AF%94.md) | [predict script](https://github.com/shibing624/textgen/blob/main/examples/t5/t5_couplet_demo.py)                      |
+        |[shibing624/songnet-base-chinese](https://huggingface.co/shibing624/songnet-base-chinese)| SongNet       | SongNet预训练模型                                                                                                                                                     | -                                                                                                                                            | -                                                                                                                     |
+        |[shibing624/songnet-base-chinese-songci](https://huggingface.co/shibing624/songnet-base-chinese-songci)| SongNet       | fine-tuned宋词后的模型                                                                                                                                                 | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                              | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_songci_demo.py)             |
+        |[shibing624/songnet-base-chinese-couplet](https://huggingface.co/shibing624/songnet-base-chinese-couplet)| SongNet       | fine-tuned对联后的模型                                                                                                                                                 | [training script](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)                                 | [predict script](https://github.com/shibing624/textgen/blob/main/examples/songnet/songnet_couplet_demo.py)            |
+        |[shibing624/chatglm-6b-csc-zh-lora](https://huggingface.co/shibing624/chatglm-6b-csc-zh-lora)| ChatGLM-6B    | 在27万中文拼写纠错数据[shibing624/CSC](https://huggingface.co/datasets/shibing624/CSC)上微调了一版ChatGLM-6B，纠错效果有提升，发布微调后的LoRA权重                                                | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_csc_demo.py)                             | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/csc_demo.py)                        |
+        |[shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)| ChatGLM-6B    | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版ChatGLM-6B，问答效果有提升，发布微调后的LoRA权重                   | [training script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py)                       | [predict script](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_hfdataset_demo.py) |
+        |[shibing624/llama-13b-belle-zh-lora](https://huggingface.co/shibing624/llama-13b-belle-zh-lora)| LLaMA-13B     | 在100万条中文ChatGPT指令Belle数据集[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)上微调了一版Llama-13B，问答效果有提升，发布微调后的LoRA权重                    | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_hfdataset_demo.py)     |
+        |[shibing624/chinese-alpaca-plus-7b](https://huggingface.co/shibing624/chinese-alpaca-plus-7b)| LLaMA-7B-plus | [中文LLaMA, Alpaca Plus版（7B）](https://github.com/ymcui/Chinese-LLaMA-Alpaca/releases/tag/v3.0)，在LLaMA-7B上扩充了中文词表并继续预训练120G文本（通用领域），在4M指令数据集上微调后得到的中文Alpaca-plus模型  | [training script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)                           | [predict script](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)     |
+        
+        ### Evaluation
+        
+        | Model                                                                                                                                       |Arch| Introduce                                                                                                            | Score    |
+        |:--------------------------------------------------------------------------------------------------------------------------------------------|:---|:---------------------------------------------------------------------------------------------------------------------|:---------|
+        | [LLaMA-7B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-7b)                                                         |LLaMA-7B| 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分 | 4.82     |
+        | [LLaMA-13B-Chinese-Alpaca](https://huggingface.co/ziqingyang/chinese-alpaca-lora-13b)                                                       |LLaMA-13B| 复用[ymcui/Chinese-LLaMA-Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca/blob/main/examples/README.md)的评估case和得分 | 7.03     |
+        | [facat/alpaca-lora-cn-13b](https://huggingface.co/facat/alpaca-lora-cn-13b)	                                                                |LLaMA-13B| 基于`decapoda-research/llama-13b-hf`加载`facat/alpaca-lora-cn-13b`LoRA模型后评估测试集并标注得分                                      | 4.07     |  
+        | [Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco](https://huggingface.co/Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco) |LLaMA-13B| 基于`decapoda-research/llama-13b-hf`加载`Chinese-Vicuna/Chinese-Vicuna-lora-13b-belle-and-guanaco`LoRA模型后评估测试集并标注得分      | 3.92     |
+        | [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                                                                                       |ChatGLM-6B| 基于原生`THUDM/chatglm-6b`评估测试集得分                                                                                        | **7.08** |
+        | [shibing624/chatglm-6b-belle-zh-lora](https://huggingface.co/shibing624/chatglm-6b-belle-zh-lora)                                           |ChatGLM-6B| 基于`THUDM/chatglm-6b`加载`shibing624/chatglm-6b-belle-zh-lora`LoRA模型后评估测试集得分                                            | 6.97     |
+        
+        - 评估case，详见在线文档：中文LLM-benchmark多任务评估集(腾讯文档) https://docs.qq.com/sheet/DUUpsREtWbFBsUVJE?tab=BB08J2  感谢韩俊明、[杨家铭](https://github.com/yangjiam)等同学的标注
+        - 评估任务类型包括：知识问答，开放式问答，数值计算，诗词、音乐、体育，娱乐，写文章，文本翻译，代码编程，伦理、拒答类，多轮问答，Score 评分是前100条（10分制）的平均分数，越高越好
+        - 评估脚本：[tests/test_benchmark.py](https://github.com/shibing624/textgen/blob/main/tests/test_benchmark.py)
+        - 结论：当前在[中文LLM-benchmark多任务评估集](https://docs.qq.com/sheet/DUUpsREtWbFBsUVJE?tab=BB08J2)上，ChatGLM-6B的表现最好，LLaMA-13B-Chinese-Alpaca的表现次之，LLaMA-7B的表现整体都差些，说明ChatGLM这种原生的中文预训练模型更理解中文语义，LLaMA-13B-Chinese-Aplaca是在原版LLaMA上扩充了中文词表，并融入了约20G的通用中文语料后的指令微调模型，表明了LLaMA-13B的底座优秀，具有强大的迁移能力
         
-        ## 🚀Demo
+        ## 🚀 Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/chinese-couplet-generate
         
         ![](docs/hf.png)
         
         run example: [examples/gradio_demo.py](examples/gradio_demo.py) to see the demo:
         
         ```shell
         python examples/gradio_demo.py
         ```
         
         model trained by [examples/t5/T5_Finetune_Chinese_Couplet.ipynb](https://github.com/shibing624/textgen/blob/main/examples/t5/T5_Finetune_Chinese_Couplet.ipynb)
         
-        ## 💾Install
+        ## 💾 Install
         
         ```shell
-        pip install git+https://github.com/huggingface/transformers
         pip install git+https://github.com/huggingface/peft
         pip install -U textgen
         ```
         
         or
         
         ```shell
         pip install torch # conda install pytorch
         git clone https://github.com/shibing624/textgen.git
         cd textgen
         python setup.py install
         ```
         
-        ## 😎Usage
-        
-        ### ChatGLM-6B LoRA 模型
+        ## ▶️ Usage
         
-        安装最新开发版的peft库，支持LoRA模型
-        
-        ```shell
-        pip install git+https://github.com/huggingface/peft
-        ```
+        ### ChatGLM-6B 模型
         
-        #### 使用ChatGLM-6B LoRA微调后的模型
+        #### 使用 ChatGLM-6B 微调后的模型
         
         example: [examples/chatglm/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/predict_demo.py)
         
         ```python
-        import sys
-        
-        sys.path.append('../..')
         from textgen import ChatGlmModel
         
-        model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", lora_name="shibing624/chatglm-6b-csc-zh-lora")
+        model = ChatGlmModel("chatglm", "THUDM/chatglm-6b", peft_name="shibing624/chatglm-6b-csc-zh-lora")
         r = model.predict(["对下面中文拼写纠错：\n少先队员因该为老人让坐。\n答："])
         print(r)  # ['少先队员应该为老人让座。\n错误字：因，坐']
         ```
         
         PS：由于使用了开发中的peft库，可能由于版本更新，导致LoRA模型加载失败，建议使用下面的训练方法，自己训练LoRA模型。
         
-        #### 训练ChatGLM-6B LoRA模型
+        #### 训练 ChatGLM-6B 微调模型
         
-        支持自定义数据集，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)。
+        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
+        3. 支持多卡训练，支持混合精度训练
         
         example: [examples/chatglm/training_chatglm_demo.py](https://github.com/shibing624/textgen/blob/main/examples/chatglm/training_chatglm_demo.py)
         
-        ### LLAMA LoRA 模型
-        
-        安装最新开发版的transformers和peft库，支持LLAMA、LoRA模型
-        
-        ```shell
-        pip install transformers>=4.28.1
-        pip install git+https://github.com/huggingface/peft
-        ```
+        ### LLaMA 模型
         
-        #### 使用LLAMA LoRA微调后的模型
+        #### 使用 LLaMA 微调后的模型
         
         example: [examples/llama/predict_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/predict_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import sys
         
         sys.path.append('../..')
         from textgen import LlamaModel
         
         
         def generate_prompt(instruction):
-            return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
+          return f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n### Instruction:{instruction}\n\n### Response:"""
         
         
-        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", lora_name="ziqingyang/chinese-alpaca-lora-7b")
+        model = LlamaModel("llama", "decapoda-research/llama-7b-hf", peft_name="ziqingyang/chinese-alpaca-lora-7b")
         predict_sentence = generate_prompt("问：用一句话描述地球为什么是独一无二的。\n答：")
         r = model.predict([predict_sentence])
         print(r)  # ['地球是唯一一颗拥有生命的行星。']
         ```
         
-        #### 训练LLAMA LoRA模型
+        </details>
+        
+        #### 训练 LLaMA 微调模型
+        1. 支持自定义训练数据集和训练参数，数据集格式参考[examples/data/zh_csc_test.tsv](https://github.com/shibing624/textgen/blob/main/examples/data/zh_csc_test.tsv)或者[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
+        2. 支持AdaLoRA、LoRA、P_Tuning、Prefix_Tuning等部分参数微调方法，也支持全参微调
+        3. 支持多卡训练，支持混合精度训练
         
         example: [examples/llama/training_llama_demo.py](https://github.com/shibing624/textgen/blob/main/examples/llama/training_llama_demo.py)
         
+        #### 基于微调(LoRA)模型继续训练
+        如果需要基于Lora模型继续训练，可以使用下面的脚本合并模型为新的base model，再微调训练即可。
+        
+        单LoRA权重合并（适用于 Chinese-LLaMA, Chinese-LLaMA-Plus, Chinese-Alpaca）
+        
+        执行以下命令：
+        ```shell
+        python -m textgen/llama/merge_llama_with_chinese_lora.py \
+            --base_model path_to_original_llama_hf_dir \
+            --lora_model path_to_chinese_llama_or_alpaca_lora \
+            --output_type [pth|huggingface]
+            --output_dir path_to_output_dir 
+        ```
+        参数说明：
+        ```
+        --base_model：存放HF格式的LLaMA模型权重和配置文件的目录
+        --lora_model：中文LLaMA/Alpaca LoRA解压后文件所在目录，也可使用HF上的Lora模型名称，如`ziqingyang/chinese-alpaca-lora-7b`会自动下载对应模型
+        --output_type: 指定输出格式，可为pth或huggingface。若不指定，默认为pth
+        --output_dir：指定保存全量模型权重的目录，默认为./
+        --offload_dir（可选）：对于低内存用户需要指定一个offload缓存路径
+        ```
+        
         ### ConvSeq2Seq 模型
         
         训练并预测ConvSeq2Seq模型：
         
         example: [examples/seq2sesq/training_convseq2seq_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_convseq2seq_model_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import argparse
         from loguru import logger
         import sys
         
         sys.path.append('../..')
         from textgen.seq2seq.conv_seq2seq_model import ConvSeq2SeqModel
@@ -225,14 +229,16 @@
         output:
         
         ```bash
         inputs: ["什么是ai", "你是什么类型的计算机", "你知道热力学吗"]
         outputs: ['人工智能是工程和科学的分支,致力于构建思维的机器。', '我的程序运行在python,所以我在任何运脑上工作！', '我不能错热是一个疯狂的人工智能"200年。']
         ```
         
+        </details>
+        
         ### BART 模型
         
         训练并预测BART模型：
         
         example: [examples/seq2sesq/training_bartseq2seq_zh_demo.py](https://github.com/shibing624/textgen/blob/main/examples/seq2seq/training_bartseq2seq_zh_demo.py)
         
         output:
@@ -242,14 +248,17 @@
         outputs: ['人工智能是工程和科学的分支,致力于构', '我的程序运行在python,所以我在任何电脑上', '什么是热力学吗？']
         ```
         
         ### T5 模型
         
         example: [examples/t5/training_zh_t5_model_demo.py](https://github.com/shibing624/textgen/blob/main/examples/t5/training_zh_t5_model_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import argparse
         from loguru import logger
         import pandas as pd
         import sys
         
         sys.path.append('../..')
@@ -339,14 +348,16 @@
         output:
         
         ```shell
         inputs: ['什么是ai', '你是什么类型的计算机', '你知道热力学吗']
         outputs: ['人工智能有两个广义的定义,任何拟人的机械,如在卡雷尔capeks', '我的程序运行在Python,所以我在任何电脑上工作!', '什么是热力学']
         ```
         
+        </details>
+        
         ### GPT2 模型
         
         #### 中文GPT2 - 文章生成
         
         使用中文数据集（段落格式，`\n`间隔），训练GPT2模型，可以用于诗歌生成、文章生成等任务。
         
         example: [examples/gpt2/training_zh_gpt2_demo.py](https://github.com/shibing624/textgen/blob/main/examples/gpt2/training_zh_gpt2_demo.py)
@@ -374,14 +385,17 @@
         
         example: [examples/songnet/training_zh_songnet_demo.py](https://github.com/shibing624/textgen/blob/main/examples/songnet/training_zh_songnet_demo.py)
         
         ### Keyword Text Augmentation(EDA/UDA)
         
         example: [examples/text_augmentation/text_augmentation_demo.py](examples/text_augmentation/text_augmentation_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import sys
         
         sys.path.append('..')
         from textgen.augment import TextAugment
         
         if __name__ == '__main__':
@@ -416,21 +430,25 @@
         主要研究机器学习、深度学习、计算机视觉、智能对话系统相关内容
         random-0.2: ('主要陪陪机器学习、深度学习主要计算机视觉、智能对话系统受限于内容', [('研究', '陪陪', 2, 4), ('、', '主要', 13, 15), ('相关', '受限于', 27, 30)])
         insert-0.2: ('主要研究机器机器学习学习、深度深度学习、计算机视觉、智能对话系统相关内容', [('机器', '机器机器', 4, 8), ('学习', '学习学习', 8, 12), ('深度', '深度深度', 13, 17)])
         delete-0.2: ('主要研究机器学习、深度学习、计算机视觉、对话系统相关内容', [('智能', '', 20, 20)])
         tfidf-0.2: ('一是研究机器学习、深度学习、计算机听觉、智能交谈系统密切相关内容', [('主要', '一是', 0, 2), ('视觉', '听觉', 17, 19), ('对话', '交谈', 22, 24), ('相关', '密切相关', 26, 30)])
         mix-0.2: ('主要研究机器学习、深度学、计算机听觉、智能对话软件系统相关内容', [('学习', '学', 11, 12), ('视觉', '听觉', 16, 18), ('系统', '软件系统', 23, 27)])
         ```
+        </details>
         
         ### TGLS 模型（无监督相似文本生成模型）
         
         无监督的中文电商评论生成：从**电商评论**中提取用户表达观点的短句并进行组合来生成仿真评论。
         
         example: [examples/unsup_generation/unsup_generation_demo.py](examples/unsup_generation/unsup_generation_demo.py)
         
+        <details>
+        <summary>show code example and result</summary>
+        
         ```python
         import os
         import sys
         
         sys.path.append('..')
         from textgen.unsup_generation import TglsModel, load_list
         
@@ -484,58 +502,85 @@
         希望好用，面膜用过了很好用，皮肤水嫩光滑白皙，补水不错，价格也合适。
         就是精华液太少了，保湿效果不错。
         面膜的补水效果非常好，保湿效果确实很赞，这个面膜相对于胶原蛋白和美白的那两款的面膜纸要厚一些，看着价格合适。
         ```
         
         前10句是真实用户评论，后10句是生成的。
         
-        ## 📚Dataset 
+        </details>
+        
+        ## 📚 Dataset 
         
         1. 50万条中文ChatGPT指令Belle数据集：[BelleGroup/train_0.5M_CN](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
         2. 100万条中文ChatGPT指令Belle数据集：[BelleGroup/train_1M_CN](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
         3. 5万条英文ChatGPT指令Alpaca数据集：[50k English Stanford Alpaca dataset](https://github.com/tatsu-lab/stanford_alpaca#data-release)
         4. 2万条中文ChatGPT指令Alpaca数据集：[shibing624/alpaca-zh](https://huggingface.co/datasets/shibing624/alpaca-zh)
         5. 69万条中文指令Guanaco数据集(Belle50万条+Guanaco19万条)：[Chinese-Vicuna/guanaco_belle_merge_v1.0](https://huggingface.co/datasets/Chinese-Vicuna/guanaco_belle_merge_v1.0)
         
-        ## ☎️Contact
+        <details>
+        <summary>文本生成方法介绍</summary>
+        
+        ### 文本生成方法
+        
+        1. seq2seq: Seq2Seq、ConvSeq2Seq、BART
+        2. language_modeling: GPT2、SongNet、ChatGLM、LLaMA
+        3. t5: T5、CopyT5
+        
+        ### 文本扩增方法
+        
+        #### 词粒度扩增
+        
+        1. UDA，非核心词替换
+        2. EDA，简单数据增强技术：相似词、同义词替换，随机词插入、删除、替换
+        
+        #### 句粒度扩增
+        
+        1. 回译（BT, Back Translate）：中文-英文-中文
+        2. GPT2模型续写：短文本->长文本
+        3. BART摘要模型：长文本->短文本
+        4. TGLS：无监督相似文本生成模型
+        
+        </details>
+        
+        ## ☎️ Contact
         
         - Issue(建议)
           ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/textgen.svg)](https://github.com/shibing624/textgen/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：姓名-公司名-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        ## 😇Citation
+        ## 😇 Citation
         
         如果你在研究中使用了textgen，请按如下格式引用：
         
         ```latex
         @misc{textgen,
           title={textgen: Text Generation Tool},
           author={Xu Ming},
           year={2021},
           howpublished={\url{https://github.com/shibing624/textgen}},
         }
         ```
         
-        ## 🤗License
+        ## 🤗 License
         
         授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加textgen的链接和授权协议。
         
-        ## 😍Contribute
+        ## 😍 Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python -m pytest`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        ## 💕Acknowledgements 
+        ## 💕 Acknowledgements 
         
         - [PaddlePaddle/ERNIE](https://github.com/PaddlePaddle/ERNIE)
         - [minimaxir/textgenrnn](https://github.com/minimaxir/textgenrnn)
         - [minimaxir/gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [asyml/texar](https://github.com/asyml/texar)
         - [yangjianxin1/GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat)
         - [williamSYSU/TextGAN-PyTorch](https://github.com/williamSYSU/TextGAN-PyTorch)
```

### Comparing `textgen-0.2.4/textgen.egg-info/SOURCES.txt` & `textgen-0.2.5/textgen.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 textgen/augment/__init__.py
 textgen/augment/sentence_level_augment.py
 textgen/augment/text_augment.py
 textgen/augment/tokenizer.py
 textgen/augment/translate_api.py
 textgen/augment/word_level_augment.py
 textgen/augment/word_vocab.py
+textgen/bloom/__init__.py
+textgen/bloom/bloom_model.py
+textgen/bloom/bloom_utils.py
 textgen/chatglm/__init__.py
 textgen/chatglm/chatglm_model.py
 textgen/chatglm/chatglm_utils.py
 textgen/config/__init__.py
 textgen/config/global_args.py
 textgen/config/model_args.py
 textgen/custom_models/__init__.py
@@ -32,14 +35,15 @@
 textgen/language_modeling/language_modeling_model.py
 textgen/language_modeling/language_modeling_utils.py
 textgen/language_modeling/songnet_model.py
 textgen/language_modeling/songnet_utils.py
 textgen/llama/__init__.py
 textgen/llama/llama_model.py
 textgen/llama/llama_utils.py
+textgen/llama/merge_llama_with_chinese_lora.py
 textgen/seq2seq/__init__.py
 textgen/seq2seq/bart_seq2seq_model.py
 textgen/seq2seq/bart_seq2seq_utils.py
 textgen/seq2seq/conv_seq2seq_model.py
 textgen/seq2seq/data_reader.py
 textgen/seq2seq/seq2seq_model.py
 textgen/seq2seq/seq2seq_trainer.py
```

