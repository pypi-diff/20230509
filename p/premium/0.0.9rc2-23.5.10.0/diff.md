# Comparing `tmp/premium-0.0.9rc2.tar.gz` & `tmp/premium-23.5.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "premium-0.0.9rc2.tar", last modified: Thu Nov 24 13:33:36 2022, max compression
+gzip compressed data, was "dist/premium-23.5.10.0.tar", last modified: Tue May  9 16:15:41 2023, max compression
```

## Comparing `premium-0.0.9rc2.tar` & `premium-23.5.10.0.tar`

### file list

```diff
@@ -1,120 +1,128 @@
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.456326 premium-0.0.9rc2/
--rw-rw-r--   0 x03       (1000) x03       (1000)      414 2022-11-24 13:33:36.452325 premium-0.0.9rc2/PKG-INFO
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-08-20 00:45:22.000000 premium-0.0.9rc2/README.md
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.236308 premium-0.0.9rc2/data/
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-11-05 09:52:56.000000 premium-0.0.9rc2/data/__init__.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.236308 premium-0.0.9rc2/data/config/
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-11-05 09:52:37.000000 premium-0.0.9rc2/data/config/__init__.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.244309 premium-0.0.9rc2/examples/
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-11-05 10:32:04.000000 premium-0.0.9rc2/examples/__init__.py
--rwxr--r--   0 x03       (1000) x03       (1000)      634 2022-11-04 03:32:46.000000 premium-0.0.9rc2/examples/bert_sentiment.py
--rw-r--r--   0 x03       (1000) x03       (1000)     8075 2022-11-07 14:48:40.000000 premium-0.0.9rc2/examples/cn_ner_transformer_pytorch.py
--rw-r--r--   0 x03       (1000) x03       (1000)     1322 2022-11-06 06:27:50.000000 premium-0.0.9rc2/examples/evaluate_cn_ner_transformer_pytorch.py
--rwxr--r--   0 x03       (1000) x03       (1000)     7574 2022-11-07 14:51:39.000000 premium-0.0.9rc2/examples/ner_transformer_pytorch.py
--rw-r--r--   0 x03       (1000) x03       (1000)     1930 2022-11-09 07:28:21.000000 premium-0.0.9rc2/examples/pytorch_vocab.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.248309 premium-0.0.9rc2/premium/
--rw-r--r--   0 x03       (1000) x03       (1000)     1142 2022-11-06 04:31:36.000000 premium-0.0.9rc2/premium/__init__.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.252309 premium-0.0.9rc2/premium/algorithm/
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-09-18 07:48:09.000000 premium-0.0.9rc2/premium/algorithm/__init__.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.252309 premium-0.0.9rc2/premium/automl/
--rw-r--r--   0 x03       (1000) x03       (1000)      726 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/automl/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)      111 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/config.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.256310 premium-0.0.9rc2/premium/corpus/
--rw-r--r--   0 x03       (1000) x03       (1000)       63 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/corpus/__init__.py
--rwxr--r--   0 x03       (1000) x03       (1000)     1081 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/corpus/stopwords.py
--rw-r--r--   0 x03       (1000) x03       (1000)      933 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/corpus/texts.py
--rw-r--r--   0 x03       (1000) x03       (1000)      447 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/corpus/utils.py
--rw-r--r--   0 x03       (1000) x03       (1000)     3875 2022-11-03 02:49:52.000000 premium-0.0.9rc2/premium/crf.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.264310 premium-0.0.9rc2/premium/data/
--rw-r--r--   0 x03       (1000) x03       (1000)        4 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/data/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)     3344 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/data/_dict.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2136 2022-08-21 08:32:02.000000 premium-0.0.9rc2/premium/data/augumentation.py
--rw-r--r--   0 x03       (1000) x03       (1000)     3682 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/data/csv.py
--rw-r--r--   0 x03       (1000) x03       (1000)     8928 2022-11-06 05:10:17.000000 premium-0.0.9rc2/premium/data/datasets.py
--rw-r--r--   0 x03       (1000) x03       (1000)     3002 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/data/eda.py
--rwxr--r--   0 x03       (1000) x03       (1000)     2637 2022-11-12 09:14:02.000000 premium-0.0.9rc2/premium/data/loader.py
--rwxr--r--   0 x03       (1000) x03       (1000)     2277 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/data/postprocess.py
--rw-r--r--   0 x03       (1000) x03       (1000)    13852 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/data/preprocess.py
--rw-r--r--   0 x03       (1000) x03       (1000)     6551 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/demo.py
--rw-r--r--   0 x03       (1000) x03       (1000)      684 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/draw.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.276311 premium-0.0.9rc2/premium/experimental/
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/experimental/__init__.py
--rwxr--r--   0 x03       (1000) x03       (1000)     6624 2022-08-31 13:10:31.000000 premium-0.0.9rc2/premium/experimental/cbow.py
--rwxr--r--   0 x03       (1000) x03       (1000)     2569 2022-09-06 07:29:08.000000 premium-0.0.9rc2/premium/experimental/eda.py
--rw-r--r--   0 x03       (1000) x03       (1000)     1462 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/experimental/kaggle.py
--rwxr--r--   0 x03       (1000) x03       (1000)     5506 2022-09-02 12:56:51.000000 premium-0.0.9rc2/premium/experimental/myfasttext.py
--rwxr--r--   0 x03       (1000) x03       (1000)     1498 2022-09-06 23:56:22.000000 premium-0.0.9rc2/premium/experimental/ner.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2272 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/experimental/nn_metric.py
--rwxr--r--   0 x03       (1000) x03       (1000)     2914 2022-11-01 04:49:36.000000 premium-0.0.9rc2/premium/experimental/segment_train.py
--rwxr--r--   0 x03       (1000) x03       (1000)     3315 2022-09-02 02:26:29.000000 premium-0.0.9rc2/premium/experimental/textnn.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2385 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/frame.py
--rw-r--r--   0 x03       (1000) x03       (1000)     8076 2022-09-27 06:27:21.000000 premium-0.0.9rc2/premium/hmm.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.344317 premium-0.0.9rc2/premium/localdata/
--rw-r--r--   0 x03       (1000) x03       (1000)  1001504 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/27.mp3
--rw-r--r--   0 x03       (1000) x03       (1000)  5340812 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/27.wav
--rw-r--r--   0 x03       (1000) x03       (1000)     4695 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/cn_stopwords.txt
--rw-r--r--   0 x03       (1000) x03       (1000)  1134854 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/dict.txt
--rw-r--r--   0 x03       (1000) x03       (1000)   278548 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/emit_p.pickle
--rw-r--r--   0 x03       (1000) x03       (1000)      621 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/en_stopwords.txt
--rw-r--r--   0 x03       (1000) x03       (1000)       61 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/oov.txt
--rw-r--r--   0 x03       (1000) x03       (1000)   844962 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/puredict.txt
--rw-r--r--   0 x03       (1000) x03       (1000)   755791 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/soledad.txt
--rw-r--r--   0 x03       (1000) x03       (1000)      176 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/trans.pickle
--rw-r--r--   0 x03       (1000) x03       (1000)  7310398 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/localdata/xinhua.txt
--rw-r--r--   0 x03       (1000) x03       (1000)     2803 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/measure.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.404322 premium-0.0.9rc2/premium/metrics/
--rw-r--r--   0 x03       (1000) x03       (1000)      635 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/metrics/__init__.py
--rwxr--r--   0 x03       (1000) x03       (1000)      876 2022-10-22 08:56:25.000000 premium-0.0.9rc2/premium/metrics/distance.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.420323 premium-0.0.9rc2/premium/models/
--rw-r--r--   0 x03       (1000) x03       (1000)       42 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)     6835 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/base.py
--rw-r--r--   0 x03       (1000) x03       (1000)      200 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/bayes.py
--rw-r--r--   0 x03       (1000) x03       (1000)     3178 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/benchmark.py
--rw-r--r--   0 x03       (1000) x03       (1000)    15555 2022-09-02 07:01:51.000000 premium-0.0.9rc2/premium/models/bert.py
--rw-r--r--   0 x03       (1000) x03       (1000)     6238 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/binary_classifiers.py
--rw-r--r--   0 x03       (1000) x03       (1000)     3939 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/clf.py
--rw-r--r--   0 x03       (1000) x03       (1000)    10472 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/lgb.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2697 2022-11-03 11:20:22.000000 premium-0.0.9rc2/premium/models/model_config.py
--rw-r--r--   0 x03       (1000) x03       (1000)     6144 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/multi_classifier.py
--rwxr--r--   0 x03       (1000) x03       (1000)    22231 2022-09-04 03:09:30.000000 premium-0.0.9rc2/premium/models/nn.py
--rw-r--r--   0 x03       (1000) x03       (1000)     4954 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/optuna.py
--rw-r--r--   0 x03       (1000) x03       (1000)     7796 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/regressor.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.420323 premium-0.0.9rc2/premium/models/tensorflow/
--rw-r--r--   0 x03       (1000) x03       (1000)      127 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/tensorflow/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2857 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/tensorflow/binary_classifier.py
--rw-r--r--   0 x03       (1000) x03       (1000)      186 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/tensorflow/info.py
--rw-r--r--   0 x03       (1000) x03       (1000)    11038 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/touchstone.py
--rw-r--r--   0 x03       (1000) x03       (1000)     1783 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/models/xgb.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.428323 premium-0.0.9rc2/premium/nlp/
--rw-r--r--   0 x03       (1000) x03       (1000)       66 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/nlp/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)     3209 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/nlp/metrics.py
--rwxr--r--   0 x03       (1000) x03       (1000)     1212 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/nlp/net.py
--rwxr--r--   0 x03       (1000) x03       (1000)     1086 2022-09-06 23:53:01.000000 premium-0.0.9rc2/premium/nlp/nlp.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.432324 premium-0.0.9rc2/premium/preprocessing/
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-09-04 01:32:49.000000 premium-0.0.9rc2/premium/preprocessing/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2435 2022-09-05 23:32:12.000000 premium-0.0.9rc2/premium/preprocessing/text.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.432324 premium-0.0.9rc2/premium/projects/
--rw-r--r--   0 x03       (1000) x03       (1000)        0 2022-09-07 00:21:25.000000 premium-0.0.9rc2/premium/projects/__init__.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.452325 premium-0.0.9rc2/premium/pytorch/
--rw-r--r--   0 x03       (1000) x03       (1000)      849 2022-11-11 02:06:02.000000 premium-0.0.9rc2/premium/pytorch/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)     1463 2022-11-12 15:40:53.000000 premium-0.0.9rc2/premium/pytorch/data.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2549 2022-11-12 09:21:21.000000 premium-0.0.9rc2/premium/pytorch/tokenizer.py
--rw-r--r--   0 x03       (1000) x03       (1000)     2136 2022-11-11 03:50:39.000000 premium-0.0.9rc2/premium/pytorch/trainer.py
--rw-r--r--   0 x03       (1000) x03       (1000)     5369 2022-09-14 00:12:27.000000 premium-0.0.9rc2/premium/segment.py
--rw-r--r--   0 x03       (1000) x03       (1000)     7175 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/sox.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.452325 premium-0.0.9rc2/premium/text_feature/
--rw-r--r--   0 x03       (1000) x03       (1000)       36 2022-11-23 03:47:20.000000 premium-0.0.9rc2/premium/text_feature/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)     4938 2022-11-23 03:47:52.000000 premium-0.0.9rc2/premium/text_feature/bm25.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.452325 premium-0.0.9rc2/premium/utils/
--rw-r--r--   0 x03       (1000) x03       (1000)     1172 2022-09-03 03:49:06.000000 premium-0.0.9rc2/premium/utils/__init__.py
--rw-r--r--   0 x03       (1000) x03       (1000)      563 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/utils/decorators.py
--rw-r--r--   0 x03       (1000) x03       (1000)      988 2022-08-20 00:43:56.000000 premium-0.0.9rc2/premium/zz.py
-drwxrwxr-x   0 x03       (1000) x03       (1000)        0 2022-11-24 13:33:36.252309 premium-0.0.9rc2/premium.egg-info/
--rw-rw-r--   0 x03       (1000) x03       (1000)      414 2022-11-24 13:33:36.000000 premium-0.0.9rc2/premium.egg-info/PKG-INFO
--rw-rw-r--   0 x03       (1000) x03       (1000)     2595 2022-11-24 13:33:36.000000 premium-0.0.9rc2/premium.egg-info/SOURCES.txt
--rw-rw-r--   0 x03       (1000) x03       (1000)        1 2022-11-24 13:33:36.000000 premium-0.0.9rc2/premium.egg-info/dependency_links.txt
--rw-rw-r--   0 x03       (1000) x03       (1000)       66 2022-11-24 13:33:36.000000 premium-0.0.9rc2/premium.egg-info/entry_points.txt
--rw-rw-r--   0 x03       (1000) x03       (1000)       95 2022-11-24 13:33:36.000000 premium-0.0.9rc2/premium.egg-info/requires.txt
--rw-rw-r--   0 x03       (1000) x03       (1000)       22 2022-11-24 13:33:36.000000 premium-0.0.9rc2/premium.egg-info/top_level.txt
--rw-rw-r--   0 x03       (1000) x03       (1000)       38 2022-11-24 13:33:36.456326 premium-0.0.9rc2/setup.cfg
--rw-r--r--   0 x03       (1000) x03       (1000)     1143 2022-11-24 13:31:00.000000 premium-0.0.9rc2/setup.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.710121 premium-23.5.10.0/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      350 2023-05-09 16:15:41.706121 premium-23.5.10.0/PKG-INFO
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-08-20 00:45:22.000000 premium-23.5.10.0/README.md
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.506122 premium-23.5.10.0/data/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-11-05 09:52:56.000000 premium-23.5.10.0/data/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.506122 premium-23.5.10.0/data/config/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-11-05 09:52:37.000000 premium-23.5.10.0/data/config/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.522122 premium-23.5.10.0/premium/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       46 2023-04-12 13:39:31.000000 premium-23.5.10.0/premium/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.526122 premium-23.5.10.0/premium/algorithm/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-09-18 07:48:09.000000 premium-23.5.10.0/premium/algorithm/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.526122 premium-23.5.10.0/premium/automl/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      726 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/automl/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.530122 premium-23.5.10.0/premium/base/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-02-28 03:25:12.000000 premium-23.5.10.0/premium/base/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      988 2023-02-28 03:25:36.000000 premium-23.5.10.0/premium/base/pipeline.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.530122 premium-23.5.10.0/premium/classifiers/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-04-12 08:44:25.000000 premium-23.5.10.0/premium/classifiers/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4588 2023-05-08 12:52:53.000000 premium-23.5.10.0/premium/classifiers/baseline.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.534122 premium-23.5.10.0/premium/classifiers/binary/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-05-08 09:46:49.000000 premium-23.5.10.0/premium/classifiers/binary/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      111 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/config.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.538122 premium-23.5.10.0/premium/corpus/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       30 2023-02-13 02:48:47.000000 premium-23.5.10.0/premium/corpus/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1074 2023-02-16 01:59:57.000000 premium-23.5.10.0/premium/corpus/stopwords.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      933 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/corpus/texts.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      447 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/corpus/utils.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.554122 premium-23.5.10.0/premium/data/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        4 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/data/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3344 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/data/_dict.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2136 2022-08-21 08:32:02.000000 premium-23.5.10.0/premium/data/augumentation.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.558122 premium-23.5.10.0/premium/data/classification/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-12-15 03:45:19.000000 premium-23.5.10.0/premium/data/classification/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3682 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/data/csv.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     9076 2023-05-09 05:48:14.000000 premium-23.5.10.0/premium/data/datasets.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3002 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/data/eda.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1418 2022-12-19 07:47:54.000000 premium-23.5.10.0/premium/data/loader.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2277 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/data/postprocess.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    12455 2023-04-28 13:08:42.000000 premium-23.5.10.0/premium/data/preprocess.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     4670 2022-12-22 11:10:43.000000 premium-23.5.10.0/premium/data/utils.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6551 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/demo.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      684 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/draw.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.570122 premium-23.5.10.0/premium/experimental/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/experimental/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     6624 2022-08-31 13:10:31.000000 premium-23.5.10.0/premium/experimental/cbow.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2569 2022-09-06 07:29:08.000000 premium-23.5.10.0/premium/experimental/eda.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1462 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/experimental/kaggle.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     8572 2023-04-12 10:55:43.000000 premium-23.5.10.0/premium/experimental/myfasttext.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1498 2022-09-06 23:56:22.000000 premium-23.5.10.0/premium/experimental/ner.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2272 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/experimental/nn_metric.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2914 2022-11-01 04:49:36.000000 premium-23.5.10.0/premium/experimental/segment_train.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     3315 2022-09-02 02:26:29.000000 premium-23.5.10.0/premium/experimental/textnn.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    14328 2022-12-19 07:00:16.000000 premium-23.5.10.0/premium/experimental/torch_crf.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2385 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/frame.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     8076 2022-09-27 06:27:21.000000 premium-23.5.10.0/premium/hmm.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.574122 premium-23.5.10.0/premium/lightning/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-04-17 06:05:11.000000 premium-23.5.10.0/premium/lightning/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2213 2023-05-04 13:34:16.000000 premium-23.5.10.0/premium/lightning/callbacks.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.638121 premium-23.5.10.0/premium/localdata/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  1001504 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/27.mp3
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  5340812 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/27.wav
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4695 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/cn_stopwords.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  1134854 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/dict.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)   278548 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/emit_p.pickle
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      621 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/en_stopwords.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       61 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/oov.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)   844962 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/puredict.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)   755791 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/soledad.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      176 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/trans.pickle
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  7310398 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/localdata/xinhua.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2803 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/measure.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.670121 premium-23.5.10.0/premium/metrics/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      660 2023-03-22 07:48:42.000000 premium-23.5.10.0/premium/metrics/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)      876 2022-10-22 08:56:25.000000 premium-23.5.10.0/premium/metrics/distance.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2990 2023-04-12 11:56:01.000000 premium-23.5.10.0/premium/metrics/metrix.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.690121 premium-23.5.10.0/premium/models/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       42 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6835 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/base.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      200 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/bayes.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3178 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/benchmark.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    15555 2022-09-02 07:01:51.000000 premium-23.5.10.0/premium/models/bert.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6238 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/binary_classifiers.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3939 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/clf.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    10472 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/lgb.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2697 2022-11-03 11:20:22.000000 premium-23.5.10.0/premium/models/model_config.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6144 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/multi_classifier.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)    22231 2022-09-04 03:09:30.000000 premium-23.5.10.0/premium/models/nn.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4954 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/optuna.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     7796 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/regressor.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.694121 premium-23.5.10.0/premium/models/tensorflow/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      127 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/tensorflow/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2857 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/tensorflow/binary_classifier.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      186 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/tensorflow/info.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    11038 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/touchstone.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1783 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/models/xgb.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.698121 premium-23.5.10.0/premium/nlp/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       66 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/nlp/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3209 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/nlp/metrics.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1212 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/nlp/net.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1086 2022-09-06 23:53:01.000000 premium-23.5.10.0/premium/nlp/nlp.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.702121 premium-23.5.10.0/premium/preprocessing/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-09-04 01:32:49.000000 premium-23.5.10.0/premium/preprocessing/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2933 2023-05-04 12:57:40.000000 premium-23.5.10.0/premium/preprocessing/ner.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2435 2022-09-05 23:32:12.000000 premium-23.5.10.0/premium/preprocessing/text.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.702121 premium-23.5.10.0/premium/pytorch/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      849 2022-11-11 02:06:02.000000 premium-23.5.10.0/premium/pytorch/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1772 2023-02-16 13:53:00.000000 premium-23.5.10.0/premium/pytorch/data.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2471 2022-12-08 04:52:17.000000 premium-23.5.10.0/premium/pytorch/tokenizer.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2136 2022-11-11 03:50:39.000000 premium-23.5.10.0/premium/pytorch/trainer.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)      275 2022-12-15 03:41:20.000000 premium-23.5.10.0/premium/pytorch/utils.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     5369 2022-09-14 00:12:27.000000 premium-23.5.10.0/premium/segment.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.706121 premium-23.5.10.0/premium/text_feature/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       36 2022-11-23 03:47:20.000000 premium-23.5.10.0/premium/text_feature/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4938 2022-11-23 03:47:52.000000 premium-23.5.10.0/premium/text_feature/bm25.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3362 2022-11-29 11:47:18.000000 premium-23.5.10.0/premium/text_feature/sif.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.706121 premium-23.5.10.0/premium/utils/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1661 2022-12-06 08:25:40.000000 premium-23.5.10.0/premium/utils/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      563 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/utils/decorators.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      988 2022-08-20 00:43:56.000000 premium-23.5.10.0/premium/zz.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:15:41.526122 premium-23.5.10.0/premium.egg-info/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      350 2023-05-09 16:15:41.000000 premium-23.5.10.0/premium.egg-info/PKG-INFO
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)     2757 2023-05-09 16:15:41.000000 premium-23.5.10.0/premium.egg-info/SOURCES.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-05-09 16:15:41.000000 premium-23.5.10.0/premium.egg-info/dependency_links.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       65 2023-05-09 16:15:41.000000 premium-23.5.10.0/premium.egg-info/entry_points.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       71 2023-05-09 16:15:41.000000 premium-23.5.10.0/premium.egg-info/requires.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       13 2023-05-09 16:15:41.000000 premium-23.5.10.0/premium.egg-info/top_level.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-05-09 16:15:41.710121 premium-23.5.10.0/setup.cfg
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1127 2023-04-12 11:10:28.000000 premium-23.5.10.0/setup.py
```

### Comparing `premium-0.0.9rc2/premium/automl/__init__.py` & `premium-23.5.10.0/premium/automl/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/corpus/texts.py` & `premium-23.5.10.0/premium/corpus/texts.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/data/_dict.py` & `premium-23.5.10.0/premium/data/_dict.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/data/augumentation.py` & `premium-23.5.10.0/premium/data/augumentation.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/data/csv.py` & `premium-23.5.10.0/premium/data/csv.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/data/datasets.py` & `premium-23.5.10.0/premium/data/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,19 +232,23 @@
 
     def mnli(self):
         """ Chinese-MNLI 自然语言推理数据集
         https://jishuin.proginn.com/p/763bfbd72666
         """
         fetch_from_url('https://host.ddot.cc/mnli.zip')
 
-    def get(self, filename: str):
+    def get(self, filename: str) -> str:
         url_map = {
             'tencent_cn_1M.txt':
             'https://filedn.com/lCdtpv3siVybVynPcgXgnPm/corpus/pretrained/tencent_cn/tencent_cn_1M.txt',
             'glove25d.gz':
             'https://filedn.com/lCdtpv3siVybVynPcgXgnPm/corpus/pretrained/glove.twitter.27B.25d.txt.gz'
         }
+        target_path = '/tmp/' + filename
         if filename in url_map:
-            cf.net.download(url_map[filename], '/tmp/' + filename)
+            cf.net.download(url_map[filename], target_path)
+            return target_path
+        else:
+            raise ValueError(f'Unknown file name {filename}')
 
-downloader = Downloader()
 
+downloader = Downloader()
```

### Comparing `premium-0.0.9rc2/premium/data/eda.py` & `premium-23.5.10.0/premium/data/eda.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/data/loader.py` & `premium-23.5.10.0/premium/preprocessing/text.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,84 @@
 #!/usr/bin/env python
-import pandas as pd
-import os
-import codefast as cf
-try:
-    import yaml
-except ImportError:
-    print('Please install yaml')
-
-
-class Struct:
-    def __init__(self, **entries):
-        self.__dict__.update(entries)
-
-    def __str__(self) -> str:
-        _dict = {}
-        for k, v in self.__dict__.items():
-            _dict[k] = v.__dict__ if isinstance(v, Struct) else v
-        return str(_dict)
-
-    def __getitem__(self, key):
-        return self.__dict__[key]
-
-
-def make_obj(obj):
-    if isinstance(obj, dict):
-        _struct = Struct()
-        for k, v in obj.items():
-            if isinstance(v, dict) or isinstance(v, list):
-                _struct.__dict__[k] = make_obj(v)
-            else:
-                _struct.__dict__[k] = v
-        return _struct
-    elif isinstance(obj, list):
-        return [make_obj(o) for o in obj]
-    else:
+import pickle
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+
+import tensorflow as tf
+from codefast.decorators.log import time_it
+from tensorflow import keras
+
+class TextVectorizer(tf.keras.layers.TextVectorization):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def adapt(self, data):
+        super().adapt(data)
+        self.vocab = self.get_vocabulary()
+        self.word_index = dict(zip(self.vocab, range(len(self.vocab))))
+    
+    @time_it
+    def dump(self, path: str):
+        self.pickle(path)
+
+    @time_it
+    def pickle(self, path: str):
+        with open(path, 'wb') as f:
+            pickle.dump(
+                {
+                    'config': self.get_config(),
+                    'weights': self.get_weights(),
+                }, f)
+
+    @classmethod
+    @time_it
+    def load(cls, path: str):
+        with open(path, 'rb') as f:
+            data = pickle.load(f)
+        obj = cls(**data['config'])
+        obj.set_weights(data['weights'])
         return obj
 
 
-def load_yaml(path) -> Struct:
-    with open(path) as f:
-        return make_obj(yaml.safe_load(f))
-
-
-class DataRetriver(object):
-    def __init__(self, remote: str, local: str, cache_dir: str) -> None:
-        self.remote = remote
-        self.local = local
-        self.cache_dir = os.path.join(cf.io.home() + f'/.cache/{cache_dir}')
-        if not os.path.exists(self.cache_dir):
-            os.mkdir(self.cache_dir)
-        self._full_path = os.path.join(self.cache_dir, self.local)
-
-    @property
-    def df(self) -> pd.DataFrame:
-        cf.net.download(self.remote, self._full_path)
-        _df = pd.read_csv(self._full_path)
-        _df.dropna(inplace=True)
-        return _df
-
-
-def ner_weibo() -> Struct:
-    """ ner weibo data
-    https://github.com/InsaneLife/ChineseNLPCorpus/tree/master/NER
-    """
-    x = DataRetriver(
-        'https://host.ddot.cc/weiboNER_2nd_conll.train.csv', 'train.csv', 'ner_weibo')
-    t = DataRetriver('https://host.ddot.cc/weiboNER_2nd_conll.test.csv',
-               'test.csv', 'ner_weibo')
-    v = DataRetriver('https://host.ddot.cc/weiboNER_2nd_conll.dev.csv',
-               'dev.csv', 'ner_weibo')
-    return make_obj(dict(train=x.df, test=t.df, val=v.df))
-
-
-def ner_en() -> Struct:
-    """English ner dataset"""
-    x = DataRetriver(
-        'https://host.ddot.cc/ner_en.csv', 'ner_en.csv', 'ner')
-    return make_obj(dict(train=x.df))
-
-
-def imdb_sentiment() -> Struct:
-    """imdb sentiment dataset"""
-    x = DataRetriver(
-        'https://host.ddot.cc/imdb_sentiment.csv', 'sentiment.csv', 'imdb')
-    return make_obj(dict(train=x.df))
-
-def spam_en()->Struct:
-    x = DataRetriver(
-        'https://host.ddot.cc/spam_en.csv', 'spam_en.csv', 'spam')
-    return make_obj(dict(train=x.df))
-    
+class TextTokenizer(tf.keras.preprocessing.text.Tokenizer):
+    def __init__(self,
+                 maxlen: int,
+                 path: str = None,
+                 padding: str = 'pre',
+                 *args,
+                 **kwargs):
+        super().__init__(*args, **kwargs)
+        self.path = path
+        self.maxlen = maxlen
+        self.padding = padding
+
+    def save(self):
+        if self.path is None:
+            raise ValueError('Path is not set')
+        with open(self.path, 'wb') as f:
+            pickle.dump(self, f)
+
+    def fit(self, texts: List[str]):
+        """ Fit the tokenizer on the texts 
+        """
+        super().fit_on_texts(texts)
+        return self.tok(texts)
+
+    @classmethod
+    def load(cls, path: str):
+        with open(path, 'rb') as f:
+            return pickle.load(f)
+
+    def tok(self, texts: List[str]) -> List[List[int]]:
+        sequences = self.texts_to_sequences(texts)
+        return tf.keras.preprocessing.sequence.pad_sequences(
+            sequences, maxlen=self.maxlen, padding=self.padding)
+
+    def transform(self, texts: List[str]) -> List[List[int]]:
+        """alias of tok"""
+        return self.tok(texts)
+
+    @time_it
+    def fit_transform(self, texts: List[str]) -> List[List[int]]:
+        """ Fit the tokenizer on the texts 
+        """
+        super().fit_on_texts(texts)
+        return self.tok(texts)
```

### Comparing `premium-0.0.9rc2/premium/data/postprocess.py` & `premium-23.5.10.0/premium/data/postprocess.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/data/preprocess.py` & `premium-23.5.10.0/premium/data/preprocess.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import random
+import warnings
 import os
 import re
 from abc import abstractmethod
 from argparse import Namespace
 from typing import Any, Dict, List, NamedTuple, Tuple
 
 import codefast as cf
@@ -141,75 +143,33 @@
         if self.lower:
             text = text.lower()
         if self.remove_stopwords:
             text = self.filter_stopwords(text)
         return text
 
 
-class TrainData(object):
-    """ Data holder
-    """
-    def __init__(self, attrs: Dict[str, Any]) -> None:
-        for k, v in attrs.items():
-            setattr(self, k, v)
-
-    def split(self,
-              test_size: float = 0.2,
-              random_state: int = 2023) -> 'TrainData':
-        """ Assume train data 'x' and label 'y' is already assigned
-        return x, xv, y, yv
-        """
-        return train_test_split(self.x,
-                                self.y,
-                                test_size=test_size,
-                                random_state=random_state)
-
-
-class SentenceList(object):
-    """Text data wrapper
-    """
-    def __init__(self, sentences: List[List[str]]) -> None:
-        self.sentences = sentences
-
-    def clean(self):
-        """Do text cleaning
-        """
-        cclist = []
-        for text in self.sentences:
-            text = EnglishTextCleaner(lower=True).__call__(text)
-            cclist.append(text)
-        self.sentences = cclist
-        return self
-
-    def tokenize(self,
-                 num_words: int = 10000,
-                 oov_token: str = '<OOV>') -> List[List[str]]:
-        from tensorflow.keras.preprocessing.text import Tokenizer
-        cf.info(f'Tokenizing texts')
-        self.tokenizer = Tokenizer(num_words=num_words, oov_token=oov_token)
-        self.tokenizer.fit_on_texts(self.sentences)
-        self.sentences = self.tokenizer.texts_to_sequences(self.sentences)
-        return self
-
-    def pad_sequences(self,
-                      padding: str = 'pre',
-                      maxlen: int = 1000) -> List[List[str]]:
-        cf.info(f'Padding sequences')
-        from tensorflow.keras.preprocessing.sequence import pad_sequences
-        self.sentences = pad_sequences(self.sentences,
-                                       maxlen=maxlen,
-                                       padding=padding)
-        return self
-
-    def tfidf(self, inplace: bool = True):
-        self.vectorizer = TfidfVectorizer()
-        res = self.vectorizer.fit_transform(self.sentences)
-        key = 'sentences' if inplace else 'sentences_tfidf'
-        setattr(self, key, res)
-        return self
+class DataAugment(object):
+    # Data augmentation
+    def __init__(self, text: str):
+        self.cn_tokens = list('，。！？【】（）％＃＠＆１２３４５６７８９０')
+        self.en_tokens = list(',.!?[]()%#@&1234567890')
+        stopwords = Stopwords()
+        self.cn_stopwords = stopwords.cn + self.cn_tokens
+        self.en_stopwords = stopwords.en + self.en_tokens
+        self.text = text
+
+    def insert_tokens(self, ratio: float = 0.3) -> str:
+        # return a string with tokens inserted
+        chars = list(self.text)
+        resp = []
+        for c in chars:
+            resp.append(c)
+            if random.random() < ratio:
+                resp.append(random.choice(self.cn_stopwords))
+        return ''.join(resp)
 
 
 class LabelData(object):
     def __init__(self, labels: List[int]) -> None:
         self.labels = labels
 
     def encode(self) -> List[int]:
@@ -385,16 +345,14 @@
 
 once = DataManager()
 
 tools = Namespace(birdview=birdview,
                   train_test_split=train_test_split,
                   split=train_test_split)
 
-import warnings
-
 
 class Stopwords(object):
     def __init__(self):
         warnings.warn(
             "premium.data.Stopwords() is deprecated; use premium.corpus.stopwords instead.")
         pass
 
@@ -409,8 +367,8 @@
         return self._load_stopwords_file('cn_stopwords.txt')
 
     @property
     def en(self) -> set:
         return self._load_stopwords_file('en_stopwords.txt')
 
 
-data = Namespace(contraction_dict=contraction_dict)
+data = Namespace(contraction_dict=contraction_dict)
```

### Comparing `premium-0.0.9rc2/premium/demo.py` & `premium-23.5.10.0/premium/demo.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/draw.py` & `premium-23.5.10.0/premium/draw.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/experimental/cbow.py` & `premium-23.5.10.0/premium/experimental/cbow.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/experimental/eda.py` & `premium-23.5.10.0/premium/experimental/eda.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/experimental/kaggle.py` & `premium-23.5.10.0/premium/experimental/kaggle.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/experimental/ner.py` & `premium-23.5.10.0/premium/experimental/ner.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/experimental/nn_metric.py` & `premium-23.5.10.0/premium/experimental/nn_metric.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/experimental/segment_train.py` & `premium-23.5.10.0/premium/experimental/segment_train.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/experimental/textnn.py` & `premium-23.5.10.0/premium/experimental/textnn.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/frame.py` & `premium-23.5.10.0/premium/frame.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/hmm.py` & `premium-23.5.10.0/premium/hmm.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/27.mp3` & `premium-23.5.10.0/premium/localdata/27.mp3`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/27.wav` & `premium-23.5.10.0/premium/localdata/27.wav`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/cn_stopwords.txt` & `premium-23.5.10.0/premium/localdata/cn_stopwords.txt`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/dict.txt` & `premium-23.5.10.0/premium/localdata/dict.txt`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/emit_p.pickle` & `premium-23.5.10.0/premium/localdata/emit_p.pickle`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/en_stopwords.txt` & `premium-23.5.10.0/premium/localdata/en_stopwords.txt`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/puredict.txt` & `premium-23.5.10.0/premium/localdata/puredict.txt`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/soledad.txt` & `premium-23.5.10.0/premium/localdata/soledad.txt`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/localdata/xinhua.txt` & `premium-23.5.10.0/premium/localdata/xinhua.txt`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/measure.py` & `premium-23.5.10.0/premium/measure.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/metrics/__init__.py` & `premium-23.5.10.0/premium/metrics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import tensorflow as tf
-from tensorflow.keras import backend as K
-
 
 def f1_loss(y_true, y_pred):
+    # lazy import
+    import tensorflow as tf
+    from tensorflow.keras import backend as K
     tp = K.sum(K.cast(y_true * y_pred, 'float'), axis=0)
     tn = K.sum(K.cast((1 - y_true) * (1 - y_pred), 'float'), axis=0)
     fp = K.sum(K.cast((1 - y_true) * y_pred, 'float'), axis=0)
     fn = K.sum(K.cast(y_true * (1 - y_pred), 'float'), axis=0)
 
     p = tp / (tp + fp + K.epsilon())
     r = tp / (tp + fn + K.epsilon())
```

### Comparing `premium-0.0.9rc2/premium/metrics/distance.py` & `premium-23.5.10.0/premium/metrics/distance.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/base.py` & `premium-23.5.10.0/premium/models/base.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/benchmark.py` & `premium-23.5.10.0/premium/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/bert.py` & `premium-23.5.10.0/premium/models/bert.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/binary_classifiers.py` & `premium-23.5.10.0/premium/models/binary_classifiers.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/clf.py` & `premium-23.5.10.0/premium/models/clf.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/lgb.py` & `premium-23.5.10.0/premium/models/lgb.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/model_config.py` & `premium-23.5.10.0/premium/models/model_config.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/multi_classifier.py` & `premium-23.5.10.0/premium/models/multi_classifier.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/nn.py` & `premium-23.5.10.0/premium/models/nn.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/optuna.py` & `premium-23.5.10.0/premium/models/optuna.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/regressor.py` & `premium-23.5.10.0/premium/models/regressor.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/tensorflow/binary_classifier.py` & `premium-23.5.10.0/premium/models/tensorflow/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/touchstone.py` & `premium-23.5.10.0/premium/models/touchstone.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/models/xgb.py` & `premium-23.5.10.0/premium/models/xgb.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/nlp/metrics.py` & `premium-23.5.10.0/premium/nlp/metrics.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/nlp/net.py` & `premium-23.5.10.0/premium/nlp/net.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/nlp/nlp.py` & `premium-23.5.10.0/premium/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/pytorch/__init__.py` & `premium-23.5.10.0/premium/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/pytorch/data.py` & `premium-23.5.10.0/premium/pytorch/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import Callable
 
 import pandas as pd
 from sklearn.model_selection import train_test_split
-
+from torch.utils.data import Dataset
 
 class BaseDataset(ABC):
     def __init__(self) -> None:
         super().__init__()
 
     @abstractmethod
     def __len__(self):
@@ -31,14 +31,26 @@
         row = self.df.iloc[idx]
         text = row['text']
         label = row['label']
         tokens = self.tokenizer(text)[0]
         return {'text': tokens, 'label': label}
 
 
+class TrainData(Dataset):
+
+    def __init__(self, X_data, y_data):
+        self.X_data = X_data
+        self.y_data = y_data
+
+    def __getitem__(self, index):
+        return self.X_data[index], self.y_data[index]
+
+    def __len__(self):
+        return len(self.X_data)
+
 def train_test_val_split(df, test_size=0.2, val_size=0.2, random_state=42):
     X, P = train_test_split(df, test_size=test_size, random_state=random_state)
     V, T = train_test_split(P, test_size=val_size, random_state=random_state)
     return X, V, T
 
 
 class AbstractLoader(ABC):
@@ -53,7 +65,9 @@
     def __init__(self, dataset, **kargs):
         self._DataSet = dataset
         self.kargs = kargs
 
     def __call__(self, df: pd.DataFrame, **kargs) -> DataLoader:
         self.kargs.update(kargs)
         return DataLoader(self._DataSet(df), **self.kargs)
+
+
```

### Comparing `premium-0.0.9rc2/premium/pytorch/tokenizer.py` & `premium-23.5.10.0/premium/pytorch/tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 
 from abc import ABC, abstractmethod
 from typing import List, Union
 import torch
 import torchtext as tt
+import numpy as np 
 
-
-class Tokenizer(ABC):
+class Vectorizer(ABC):
     def __init__(self, *args, **kwargs):
         pass
 
     @abstractmethod
     def fit(self, texts: List[str]):
         pass
 
@@ -31,48 +31,48 @@
         pass
 
     @abstractmethod
     def load(self, path: str):
         pass
 
 
-class VocabTokenizer(Tokenizer):
+class VocabVectorizer(Vectorizer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.tokenizer = tt.data.get_tokenizer('basic_english')
         self.vocab = None
-        self.max_len = kwargs.get('max_len', -1)
+        self.max_length = kwargs.get('max_length', 100)
         self.padding = kwargs.get('padding', False)
 
     def _yield_tokens(self, texts: List[str]):
         for text in texts:
             yield self.tokenizer(text)
 
     def __len__(self):
         return len(self.vocab)
 
+    def size(self)->int:
+        return len(self.vocab)
+    
     def fit(self, texts: List[str]) -> 'Self':
-        assert isinstance(texts, list), "texts must be a list"
         self.vocab = tt.vocab.build_vocab_from_iterator(self._yield_tokens(texts))
         self.vocab.set_default_index(0)
         return self
 
-    def transform(self, texts: Union[str, List[str]]) -> List[torch.tensor]:
+    def transform(self, texts: Union[str, List[str]]) -> np.ndarray:
         if isinstance(texts, str):
             texts = [texts]
-        tensors = []
-        for text in texts:
-            tokens = self.tokenizer(text)
-            if self.max_len > 0:
-                tokens = tokens[:self.max_len]
-            if self.padding:
-                tokens = tokens + ['<pad>'] * (self.max_len - len(tokens))
-            tensor = torch.tensor([self.vocab[token] for token in tokens])
-            tensors.append(tensor)
-        return tensors
+        vectors = [[self.vocab[token]
+                    for token in self.tokenizer(text)[:self.max_length]]
+                   for text in texts]
+        padded_vectors = np.array([
+            vector + [0] * (self.max_length - len(vector)) for vector in vectors
+        ])
+        return padded_vectors
+
 
     def fit_transform(self, texts: Union[str, List[str]]) -> List[List[int]]:
         if isinstance(texts, str):
             texts = [texts]
         return self.fit(texts).transform(texts)
 
     def inverse_transform(self, tokens: List[int]) -> List[str]:
@@ -84,7 +84,9 @@
 
     def load(self, path: str) -> 'Self':
         self.vocab = torch.load(path)
         return self
 
     def __call__(self, texts: Union[str, List[str]]) -> List[int]:
         return self.transform(texts)
+
+
```

### Comparing `premium-0.0.9rc2/premium/pytorch/trainer.py` & `premium-23.5.10.0/premium/pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/segment.py` & `premium-23.5.10.0/premium/segment.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/text_feature/bm25.py` & `premium-23.5.10.0/premium/text_feature/bm25.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/utils/decorators.py` & `premium-23.5.10.0/premium/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium/zz.py` & `premium-23.5.10.0/premium/zz.py`

 * *Files identical despite different names*

### Comparing `premium-0.0.9rc2/premium.egg-info/SOURCES.txt` & `premium-23.5.10.0/premium.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 README.md
 setup.py
 data/__init__.py
 data/config/__init__.py
-examples/__init__.py
-examples/bert_sentiment.py
-examples/cn_ner_transformer_pytorch.py
-examples/evaluate_cn_ner_transformer_pytorch.py
-examples/ner_transformer_pytorch.py
-examples/pytorch_vocab.py
 premium/__init__.py
 premium/config.py
-premium/crf.py
 premium/demo.py
 premium/draw.py
 premium/frame.py
 premium/hmm.py
 premium/measure.py
 premium/segment.py
-premium/sox.py
 premium/zz.py
 premium.egg-info/PKG-INFO
 premium.egg-info/SOURCES.txt
 premium.egg-info/dependency_links.txt
 premium.egg-info/entry_points.txt
 premium.egg-info/requires.txt
 premium.egg-info/top_level.txt
 premium/algorithm/__init__.py
 premium/automl/__init__.py
+premium/base/__init__.py
+premium/base/pipeline.py
+premium/classifiers/__init__.py
+premium/classifiers/baseline.py
+premium/classifiers/binary/__init__.py
 premium/corpus/__init__.py
 premium/corpus/stopwords.py
 premium/corpus/texts.py
 premium/corpus/utils.py
 premium/data/__init__.py
 premium/data/_dict.py
 premium/data/augumentation.py
 premium/data/csv.py
 premium/data/datasets.py
 premium/data/eda.py
 premium/data/loader.py
 premium/data/postprocess.py
 premium/data/preprocess.py
+premium/data/utils.py
+premium/data/classification/__init__.py
 premium/experimental/__init__.py
 premium/experimental/cbow.py
 premium/experimental/eda.py
 premium/experimental/kaggle.py
 premium/experimental/myfasttext.py
 premium/experimental/ner.py
 premium/experimental/nn_metric.py
 premium/experimental/segment_train.py
 premium/experimental/textnn.py
+premium/experimental/torch_crf.py
+premium/lightning/__init__.py
+premium/lightning/callbacks.py
 premium/localdata/27.mp3
 premium/localdata/27.wav
 premium/localdata/cn_stopwords.txt
 premium/localdata/dict.txt
 premium/localdata/emit_p.pickle
 premium/localdata/en_stopwords.txt
 premium/localdata/oov.txt
 premium/localdata/puredict.txt
 premium/localdata/soledad.txt
 premium/localdata/trans.pickle
 premium/localdata/xinhua.txt
 premium/metrics/__init__.py
 premium/metrics/distance.py
+premium/metrics/metrix.py
 premium/models/__init__.py
 premium/models/base.py
 premium/models/bayes.py
 premium/models/benchmark.py
 premium/models/bert.py
 premium/models/binary_classifiers.py
 premium/models/clf.py
@@ -81,17 +84,19 @@
 premium/models/tensorflow/binary_classifier.py
 premium/models/tensorflow/info.py
 premium/nlp/__init__.py
 premium/nlp/metrics.py
 premium/nlp/net.py
 premium/nlp/nlp.py
 premium/preprocessing/__init__.py
+premium/preprocessing/ner.py
 premium/preprocessing/text.py
-premium/projects/__init__.py
 premium/pytorch/__init__.py
 premium/pytorch/data.py
 premium/pytorch/tokenizer.py
 premium/pytorch/trainer.py
+premium/pytorch/utils.py
 premium/text_feature/__init__.py
 premium/text_feature/bm25.py
+premium/text_feature/sif.py
 premium/utils/__init__.py
 premium/utils/decorators.py
```

### Comparing `premium-0.0.9rc2/setup.py` & `premium-23.5.10.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import setuptools
+import codefast as cf 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="premium",
-    version="0.0.9rc2",
+    version=cf.generate_version(),
     author="sK9xTFBq0H",
-    author_email="GaoangLau@gmail.com",
+    author_email="google@gmail.com",
     description="Python AI toolkits",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/GaoangLiu/premium",
+    url="https://github.com/",
     packages=setuptools.find_packages(),
     include_package_data=True,
     package_data={
         # And include any *.msg files found in the "hello" package, too:
         "premium": [
             'localdata/*.txt', 'localdata/*.pickle', 'localdata/*.mp3',
             'localdata/*.wav'
         ],
     },
     install_requires=[
-        'smart-open', 'optuna', 'jieba', 'matplotlib', 'sklearn', 'tensorflow',
-        'transformers', 'codefast', 'jiwer', 'pandas', 'numpy'
+        'smart-open', 'optuna', 'jieba', 'matplotlib', 'sklearn',
+        'codefast', 'jiwer', 'pandas', 'numpy'
     ],
     entry_points={
         'console_scripts': ['demo=premium.demo:entry', 'zz=premium.zz:main'],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

