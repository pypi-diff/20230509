# Comparing `tmp/NewsSentiment-1.1.8.tar.gz` & `tmp/NewsSentiment-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/felix/IdeaProjects/NewsMTSC/dist/tmpu6cqwq3r/NewsSentiment-1.1.8.tar", last modified: Thu Feb 24 14:07:55 2022, max compression
+gzip compressed data, was "/Users/felix/IdeaProjects/NewsMTSC/dist/tmpg8gh_b2b/NewsSentiment-1.1.9.tar", last modified: Thu Feb 24 14:15:18 2022, max compression
```

## Comparing `NewsSentiment-1.1.8.tar` & `NewsSentiment-1.1.9.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/
--rw-r--r--   0 felix      (501) staff       (20)     1394 2021-10-19 13:47:05.000000 NewsSentiment-1.1.8/LICENSE
--rw-r--r--   0 felix      (501) staff       (20)       44 2021-12-16 11:41:13.000000 NewsSentiment-1.1.8/MANIFEST.in
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/
--rw-r--r--   0 felix      (501) staff       (20)    15097 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/DatasetPreparer.py
--rw-r--r--   0 felix      (501) staff       (20)     6379 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/SentimentClasses.py
--rw-r--r--   0 felix      (501) staff       (20)       58 2021-12-13 13:23:57.000000 NewsSentiment-1.1.8/NewsSentiment/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)      492 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/__main__.py
--rw-r--r--   0 felix      (501) staff       (20)     3495 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/combinations_default.py
--rw-r--r--   0 felix      (501) staff       (20)     1737 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/consts.py
--rw-r--r--   0 felix      (501) staff       (20)    31676 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/controller.py
--rw-r--r--   0 felix      (501) staff       (20)     1709 2021-12-31 10:25:25.000000 NewsSentiment-1.1.8/NewsSentiment/converter_huggingface.py
--rw-r--r--   0 felix      (501) staff       (20)     6007 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/createoverview.py
--rw-r--r--   0 felix      (501) staff       (20)      101 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/customexceptions.py
--rw-r--r--   0 felix      (501) staff       (20)    66783 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/dataset.py
--rw-r--r--   0 felix      (501) staff       (20)      841 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/diskdict.py
--rw-r--r--   0 felix      (501) staff       (20)     3935 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/download.py
--rw-r--r--   0 felix      (501) staff       (20)     1927 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/earlystopping.py
--rw-r--r--   0 felix      (501) staff       (20)     5832 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/evaluator.py
--rw-r--r--   0 felix      (501) staff       (20)      586 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/fxlogger.py
--rw-r--r--   0 felix      (501) staff       (20)     7371 2022-01-13 17:30:56.000000 NewsSentiment-1.1.8/NewsSentiment/infer.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/
--rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/__init__.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/
--rw-r--r--   0 felix      (501) staff       (20)      861 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/bingliuopinion.py
--rw-r--r--   0 felix      (501) staff       (20)     1782 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/converter.py
--rw-r--r--   0 felix      (501) staff       (20)     1191 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/license.txt
--rw-r--r--   0 felix      (501) staff       (20)    44759 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/negative-words.txt
--rw-r--r--   0 felix      (501) staff       (20)   277768 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/opinion_polarity.ddict
--rw-r--r--   0 felix      (501) staff       (20)    19092 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/positive-words.txt
--rw-r--r--   0 felix      (501) staff       (20)      388 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/knowledgeutils.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/data/
--rw-r--r--   0 felix      (501) staff       (20)       63 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/data/readme.txt
--rw-r--r--   0 felix      (501) staff       (20)     1859 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/dic.py
--rw-r--r--   0 felix      (501) staff       (20)      939 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/liwc.py
--rw-r--r--   0 felix      (501) staff       (20)      812 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/liwchelper.py
--rw-r--r--   0 felix      (501) staff       (20)     1002 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/trie.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/
--rw-r--r--   0 felix      (501) staff       (20)     2197 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/converter.py
--rw-r--r--   0 felix      (501) staff       (20)      888 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/mpqasubjectivity.py
--rw-r--r--   0 felix      (501) staff       (20)   662572 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff
--rw-r--r--   0 felix      (501) staff       (20)   284612 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff.ddict
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/
--rw-r--r--   0 felix      (501) staff       (20)  2579144 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt
--rw-r--r--   0 felix      (501) staff       (20)   280866 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt.ddict
--rw-r--r--   0 felix      (501) staff       (20)     1530 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/converter.py
--rw-r--r--   0 felix      (501) staff       (20)      813 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/nrcemolex.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/zeros/
--rw-r--r--   0 felix      (501) staff       (20)      665 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/knowledge/zeros/zerosknowledge.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/layers/
--rw-r--r--   0 felix      (501) staff       (20)     1903 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/layers/AggregatorForBert.py
--rw-r--r--   0 felix      (501) staff       (20)      130 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/layers/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     8505 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/layers/attention.py
--rw-r--r--   0 felix      (501) staff       (20)     3936 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/layers/dynamic_rnn.py
--rw-r--r--   0 felix      (501) staff       (20)      841 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/layers/point_wise_feed_forward.py
--rw-r--r--   0 felix      (501) staff       (20)     3823 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/layers/pytorchnlpattention.py
--rw-r--r--   0 felix      (501) staff       (20)     1207 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/layers/squeeze_embedding.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/losses/
--rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/losses/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     5185 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/losses/crossentropycrossweight.py
--rw-r--r--   0 felix      (501) staff       (20)     5355 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/losses/crossentropylosslsr.py
--rw-r--r--   0 felix      (501) staff       (20)     4719 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/losses/seq2seqloss.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/models/
--rw-r--r--   0 felix      (501) staff       (20)     4435 2021-12-15 12:32:39.000000 NewsSentiment-1.1.8/NewsSentiment/models/FXBaseModel.py
--rw-r--r--   0 felix      (501) staff       (20)     5708 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/FXEnsemble.py
--rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     2698 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/ensemble.py
--rw-r--r--   0 felix      (501) staff       (20)     2324 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/ensembleb.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/
--rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     3531 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/contrasting.py
--rw-r--r--   0 felix      (501) staff       (20)     1308 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/random_multi.py
--rw-r--r--   0 felix      (501) staff       (20)     2901 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/seq2seq.py
--rw-r--r--   0 felix      (501) staff       (20)     2360 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/seq2seq_without_targetmask.py
--rw-r--r--   0 felix      (501) staff       (20)     5300 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/tdbertlikemultitarget.py
--rw-r--r--   0 felix      (501) staff       (20)     3234 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/multitargets/tdbertlikemultitarget_dense.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/
--rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/__init__.py
--rw-r--r--   0 felix      (501) staff       (20)     5945 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/aen.py
--rw-r--r--   0 felix      (501) staff       (20)     7078 2022-02-03 08:35:48.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/grutscsingle.py
--rw-r--r--   0 felix      (501) staff       (20)     8168 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcf.py
--rw-r--r--   0 felix      (501) staff       (20)     8304 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcf2.py
--rw-r--r--   0 felix      (501) staff       (20)     9995 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcfs.py
--rw-r--r--   0 felix      (501) staff       (20)    13420 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcfst.py
--rw-r--r--   0 felix      (501) staff       (20)    12272 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcft.py
--rw-r--r--   0 felix      (501) staff       (20)     1617 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/notargetcls.py
--rw-r--r--   0 felix      (501) staff       (20)     1310 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/random_single.py
--rw-r--r--   0 felix      (501) staff       (20)     2336 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/spc.py
--rw-r--r--   0 felix      (501) staff       (20)     3238 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/td_bert.py
--rw-r--r--   0 felix      (501) staff       (20)     5200 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/td_bert_qa.py
--rw-r--r--   0 felix      (501) staff       (20)     3881 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/models/singletarget/tdbertlikesingle.py
--rw-r--r--   0 felix      (501) staff       (20)     2615 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/NewsSentiment/plotter_utils.py
--rw-r--r--   0 felix      (501) staff       (20)    53826 2021-12-15 14:18:22.000000 NewsSentiment-1.1.8/NewsSentiment/train.py
-drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment.egg-info/
--rw-r--r--   0 felix      (501) staff       (20)     4061 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment.egg-info/PKG-INFO
--rw-r--r--   0 felix      (501) staff       (20)     3769 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment.egg-info/SOURCES.txt
--rw-r--r--   0 felix      (501) staff       (20)        1 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment.egg-info/dependency_links.txt
--rw-r--r--   0 felix      (501) staff       (20)      309 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment.egg-info/requires.txt
--rw-r--r--   0 felix      (501) staff       (20)       88 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/NewsSentiment.egg-info/top_level.txt
--rw-r--r--   0 felix      (501) staff       (20)     4061 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/PKG-INFO
--rw-r--r--   0 felix      (501) staff       (20)     5379 2022-01-13 17:32:01.000000 NewsSentiment-1.1.8/README.md
--rw-r--r--   0 felix      (501) staff       (20)     2911 2022-01-05 13:36:33.000000 NewsSentiment-1.1.8/READMEpypi.md
--rw-r--r--   0 felix      (501) staff       (20)      100 2021-12-13 10:09:22.000000 NewsSentiment-1.1.8/pyproject.toml
--rw-r--r--   0 felix      (501) staff       (20)      602 2021-12-13 13:26:24.000000 NewsSentiment-1.1.8/pythoninfo.md
--rw-r--r--   0 felix      (501) staff       (20)     1606 2022-02-24 14:07:55.000000 NewsSentiment-1.1.8/setup.cfg
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/
+-rw-r--r--   0 felix      (501) staff       (20)     1394 2021-10-19 13:47:05.000000 NewsSentiment-1.1.9/LICENSE
+-rw-r--r--   0 felix      (501) staff       (20)       44 2021-12-16 11:41:13.000000 NewsSentiment-1.1.9/MANIFEST.in
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/
+-rw-r--r--   0 felix      (501) staff       (20)    15097 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/DatasetPreparer.py
+-rw-r--r--   0 felix      (501) staff       (20)     6379 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/SentimentClasses.py
+-rw-r--r--   0 felix      (501) staff       (20)       58 2021-12-13 13:23:57.000000 NewsSentiment-1.1.9/NewsSentiment/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)      492 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/__main__.py
+-rw-r--r--   0 felix      (501) staff       (20)     3495 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/combinations_default.py
+-rw-r--r--   0 felix      (501) staff       (20)     1737 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/consts.py
+-rw-r--r--   0 felix      (501) staff       (20)    31676 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/controller.py
+-rw-r--r--   0 felix      (501) staff       (20)     1709 2021-12-31 10:25:25.000000 NewsSentiment-1.1.9/NewsSentiment/converter_huggingface.py
+-rw-r--r--   0 felix      (501) staff       (20)     6007 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/createoverview.py
+-rw-r--r--   0 felix      (501) staff       (20)      101 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/customexceptions.py
+-rw-r--r--   0 felix      (501) staff       (20)    66788 2022-02-24 14:13:12.000000 NewsSentiment-1.1.9/NewsSentiment/dataset.py
+-rw-r--r--   0 felix      (501) staff       (20)      841 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/diskdict.py
+-rw-r--r--   0 felix      (501) staff       (20)     3935 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/download.py
+-rw-r--r--   0 felix      (501) staff       (20)     1927 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/earlystopping.py
+-rw-r--r--   0 felix      (501) staff       (20)     5832 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/evaluator.py
+-rw-r--r--   0 felix      (501) staff       (20)      586 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/fxlogger.py
+-rw-r--r--   0 felix      (501) staff       (20)     7371 2022-01-13 17:30:56.000000 NewsSentiment-1.1.9/NewsSentiment/infer.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/__init__.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/
+-rw-r--r--   0 felix      (501) staff       (20)      861 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/bingliuopinion.py
+-rw-r--r--   0 felix      (501) staff       (20)     1782 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/converter.py
+-rw-r--r--   0 felix      (501) staff       (20)     1191 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/license.txt
+-rw-r--r--   0 felix      (501) staff       (20)    44759 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/negative-words.txt
+-rw-r--r--   0 felix      (501) staff       (20)   277768 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/opinion_polarity.ddict
+-rw-r--r--   0 felix      (501) staff       (20)    19092 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/positive-words.txt
+-rw-r--r--   0 felix      (501) staff       (20)      388 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/knowledgeutils.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/data/
+-rw-r--r--   0 felix      (501) staff       (20)       63 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/data/readme.txt
+-rw-r--r--   0 felix      (501) staff       (20)     1859 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/dic.py
+-rw-r--r--   0 felix      (501) staff       (20)      939 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/liwc.py
+-rw-r--r--   0 felix      (501) staff       (20)      812 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/liwchelper.py
+-rw-r--r--   0 felix      (501) staff       (20)     1002 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/trie.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/
+-rw-r--r--   0 felix      (501) staff       (20)     2197 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/converter.py
+-rw-r--r--   0 felix      (501) staff       (20)      888 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/mpqasubjectivity.py
+-rw-r--r--   0 felix      (501) staff       (20)   662572 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff
+-rw-r--r--   0 felix      (501) staff       (20)   284612 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff.ddict
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/
+-rw-r--r--   0 felix      (501) staff       (20)  2579144 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt
+-rw-r--r--   0 felix      (501) staff       (20)   280866 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt.ddict
+-rw-r--r--   0 felix      (501) staff       (20)     1530 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/converter.py
+-rw-r--r--   0 felix      (501) staff       (20)      813 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/nrcemolex.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/zeros/
+-rw-r--r--   0 felix      (501) staff       (20)      665 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/knowledge/zeros/zerosknowledge.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/layers/
+-rw-r--r--   0 felix      (501) staff       (20)     1903 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/layers/AggregatorForBert.py
+-rw-r--r--   0 felix      (501) staff       (20)      130 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/layers/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     8505 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/layers/attention.py
+-rw-r--r--   0 felix      (501) staff       (20)     3936 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/layers/dynamic_rnn.py
+-rw-r--r--   0 felix      (501) staff       (20)      841 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/layers/point_wise_feed_forward.py
+-rw-r--r--   0 felix      (501) staff       (20)     3823 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/layers/pytorchnlpattention.py
+-rw-r--r--   0 felix      (501) staff       (20)     1207 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/layers/squeeze_embedding.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/losses/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/losses/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     5185 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/losses/crossentropycrossweight.py
+-rw-r--r--   0 felix      (501) staff       (20)     5355 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/losses/crossentropylosslsr.py
+-rw-r--r--   0 felix      (501) staff       (20)     4719 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/losses/seq2seqloss.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/models/
+-rw-r--r--   0 felix      (501) staff       (20)     4435 2021-12-15 12:32:39.000000 NewsSentiment-1.1.9/NewsSentiment/models/FXBaseModel.py
+-rw-r--r--   0 felix      (501) staff       (20)     5708 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/FXEnsemble.py
+-rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     2698 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/ensemble.py
+-rw-r--r--   0 felix      (501) staff       (20)     2324 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/ensembleb.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     3531 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/contrasting.py
+-rw-r--r--   0 felix      (501) staff       (20)     1308 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/random_multi.py
+-rw-r--r--   0 felix      (501) staff       (20)     2901 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/seq2seq.py
+-rw-r--r--   0 felix      (501) staff       (20)     2360 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/seq2seq_without_targetmask.py
+-rw-r--r--   0 felix      (501) staff       (20)     5300 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/tdbertlikemultitarget.py
+-rw-r--r--   0 felix      (501) staff       (20)     3234 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/multitargets/tdbertlikemultitarget_dense.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/
+-rw-r--r--   0 felix      (501) staff       (20)        0 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/__init__.py
+-rw-r--r--   0 felix      (501) staff       (20)     5945 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/aen.py
+-rw-r--r--   0 felix      (501) staff       (20)     7078 2022-02-03 08:35:48.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/grutscsingle.py
+-rw-r--r--   0 felix      (501) staff       (20)     8168 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcf.py
+-rw-r--r--   0 felix      (501) staff       (20)     8304 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcf2.py
+-rw-r--r--   0 felix      (501) staff       (20)     9995 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcfs.py
+-rw-r--r--   0 felix      (501) staff       (20)    13420 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcfst.py
+-rw-r--r--   0 felix      (501) staff       (20)    12272 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcft.py
+-rw-r--r--   0 felix      (501) staff       (20)     1617 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/notargetcls.py
+-rw-r--r--   0 felix      (501) staff       (20)     1310 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/random_single.py
+-rw-r--r--   0 felix      (501) staff       (20)     2336 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/spc.py
+-rw-r--r--   0 felix      (501) staff       (20)     3238 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/td_bert.py
+-rw-r--r--   0 felix      (501) staff       (20)     5200 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/td_bert_qa.py
+-rw-r--r--   0 felix      (501) staff       (20)     3881 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/models/singletarget/tdbertlikesingle.py
+-rw-r--r--   0 felix      (501) staff       (20)     2615 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/NewsSentiment/plotter_utils.py
+-rw-r--r--   0 felix      (501) staff       (20)    53826 2021-12-15 14:18:22.000000 NewsSentiment-1.1.9/NewsSentiment/train.py
+drwxr-xr-x   0 felix      (501) staff       (20)        0 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment.egg-info/
+-rw-r--r--   0 felix      (501) staff       (20)     4061 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment.egg-info/PKG-INFO
+-rw-r--r--   0 felix      (501) staff       (20)     3769 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment.egg-info/SOURCES.txt
+-rw-r--r--   0 felix      (501) staff       (20)        1 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment.egg-info/dependency_links.txt
+-rw-r--r--   0 felix      (501) staff       (20)      309 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment.egg-info/requires.txt
+-rw-r--r--   0 felix      (501) staff       (20)       88 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/NewsSentiment.egg-info/top_level.txt
+-rw-r--r--   0 felix      (501) staff       (20)     4061 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/PKG-INFO
+-rw-r--r--   0 felix      (501) staff       (20)     5379 2022-01-13 17:32:01.000000 NewsSentiment-1.1.9/README.md
+-rw-r--r--   0 felix      (501) staff       (20)     2911 2022-01-05 13:36:33.000000 NewsSentiment-1.1.9/READMEpypi.md
+-rw-r--r--   0 felix      (501) staff       (20)      100 2021-12-13 10:09:22.000000 NewsSentiment-1.1.9/pyproject.toml
+-rw-r--r--   0 felix      (501) staff       (20)      602 2021-12-13 13:26:24.000000 NewsSentiment-1.1.9/pythoninfo.md
+-rw-r--r--   0 felix      (501) staff       (20)     1606 2022-02-24 14:15:18.000000 NewsSentiment-1.1.9/setup.cfg
```

### Comparing `NewsSentiment-1.1.8/LICENSE` & `NewsSentiment-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/DatasetPreparer.py` & `NewsSentiment-1.1.9/NewsSentiment/DatasetPreparer.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/SentimentClasses.py` & `NewsSentiment-1.1.9/NewsSentiment/SentimentClasses.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/combinations_default.py` & `NewsSentiment-1.1.9/NewsSentiment/combinations_default.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/consts.py` & `NewsSentiment-1.1.9/NewsSentiment/consts.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/controller.py` & `NewsSentiment-1.1.9/NewsSentiment/controller.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/converter_huggingface.py` & `NewsSentiment-1.1.9/NewsSentiment/converter_huggingface.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/createoverview.py` & `NewsSentiment-1.1.9/NewsSentiment/createoverview.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/dataset.py` & `NewsSentiment-1.1.9/NewsSentiment/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,25 +41,25 @@
 logger = get_logger()
 try:
     nlp = spacy.load("en_core_web_sm")
 except OSError:
     spacy.cli.download("en_core_web_sm")
     nlp = spacy.load("en_core_web_sm")
 # this is what we could run on spacy 2.2+
-# nlp_dep_parser_labels = list(nlp.parser.labels)
+nlp_dep_parser_labels = list(nlp.parser.labels)
 # but since we're on spacy 2.1 (and need to be because of newsalyze-backend)
 # we have to use this workaround, see:
 # https://github.com/explosion/spaCy/discussions/5135
-nlp_dep_parser_labels = []
-for move in nlp.parser.move_names:
-    if "-" in move:
-        move = move.split("-")[1]
-        if "||" in move:
-            move = move.split("||")[1]
-        nlp_dep_parser_labels.append(move)
+#nlp_dep_parser_labels = []
+#for move in nlp.parser.move_names:
+#    if "-" in move:
+#        move = move.split("-")[1]
+#        if "||" in move:
+#            move = move.split("||")[1]
+#        nlp_dep_parser_labels.append(move)
 # assert set(nlp_dep_parser_labels) == {
 #     "agent",
 #     "acl",
 #     "intj",
 #     "predet",
 #     "expl",
 #     "prt",
```

### Comparing `NewsSentiment-1.1.8/NewsSentiment/diskdict.py` & `NewsSentiment-1.1.9/NewsSentiment/diskdict.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/download.py` & `NewsSentiment-1.1.9/NewsSentiment/download.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/earlystopping.py` & `NewsSentiment-1.1.9/NewsSentiment/earlystopping.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/evaluator.py` & `NewsSentiment-1.1.9/NewsSentiment/evaluator.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/fxlogger.py` & `NewsSentiment-1.1.9/NewsSentiment/fxlogger.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/infer.py` & `NewsSentiment-1.1.9/NewsSentiment/infer.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/bingliuopinion.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/bingliuopinion.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/converter.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/converter.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/license.txt` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/license.txt`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/negative-words.txt` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/negative-words.txt`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/opinion_polarity.ddict` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/opinion_polarity.ddict`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/bingliuopinion/positive-words.txt` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/bingliuopinion/positive-words.txt`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/dic.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/dic.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/liwc.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/liwc.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/liwchelper.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/liwchelper.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/liwc/trie.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/liwc/trie.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/converter.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/converter.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/mpqasubjectivity.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/mpqasubjectivity.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff.ddict` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/mpqasubjectivity/subjclueslen1-HLTEMNLP05.tff.ddict`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt.ddict` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/NRC-Emotion-Lexicon-Wordlevel-v0.92.txt.ddict`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/converter.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/converter.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/nrcemolex/nrcemolex.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/nrcemolex/nrcemolex.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/knowledge/zeros/zerosknowledge.py` & `NewsSentiment-1.1.9/NewsSentiment/knowledge/zeros/zerosknowledge.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/layers/AggregatorForBert.py` & `NewsSentiment-1.1.9/NewsSentiment/layers/AggregatorForBert.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/layers/attention.py` & `NewsSentiment-1.1.9/NewsSentiment/layers/attention.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/layers/dynamic_rnn.py` & `NewsSentiment-1.1.9/NewsSentiment/layers/dynamic_rnn.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/layers/point_wise_feed_forward.py` & `NewsSentiment-1.1.9/NewsSentiment/layers/point_wise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/layers/pytorchnlpattention.py` & `NewsSentiment-1.1.9/NewsSentiment/layers/pytorchnlpattention.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/layers/squeeze_embedding.py` & `NewsSentiment-1.1.9/NewsSentiment/layers/squeeze_embedding.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/losses/crossentropycrossweight.py` & `NewsSentiment-1.1.9/NewsSentiment/losses/crossentropycrossweight.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/losses/crossentropylosslsr.py` & `NewsSentiment-1.1.9/NewsSentiment/losses/crossentropylosslsr.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/losses/seq2seqloss.py` & `NewsSentiment-1.1.9/NewsSentiment/losses/seq2seqloss.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/FXBaseModel.py` & `NewsSentiment-1.1.9/NewsSentiment/models/FXBaseModel.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/FXEnsemble.py` & `NewsSentiment-1.1.9/NewsSentiment/models/FXEnsemble.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/ensemble.py` & `NewsSentiment-1.1.9/NewsSentiment/models/ensemble.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/ensembleb.py` & `NewsSentiment-1.1.9/NewsSentiment/models/ensembleb.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/multitargets/contrasting.py` & `NewsSentiment-1.1.9/NewsSentiment/models/multitargets/contrasting.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/multitargets/random_multi.py` & `NewsSentiment-1.1.9/NewsSentiment/models/multitargets/random_multi.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/multitargets/seq2seq.py` & `NewsSentiment-1.1.9/NewsSentiment/models/multitargets/seq2seq.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/multitargets/seq2seq_without_targetmask.py` & `NewsSentiment-1.1.9/NewsSentiment/models/multitargets/seq2seq_without_targetmask.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/multitargets/tdbertlikemultitarget.py` & `NewsSentiment-1.1.9/NewsSentiment/models/multitargets/tdbertlikemultitarget.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/multitargets/tdbertlikemultitarget_dense.py` & `NewsSentiment-1.1.9/NewsSentiment/models/multitargets/tdbertlikemultitarget_dense.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/aen.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/aen.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/grutscsingle.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/grutscsingle.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcf.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcf.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcf2.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcf2.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcfs.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcfs.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcfst.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcfst.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/lcft.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/lcft.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/notargetcls.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/notargetcls.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/random_single.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/random_single.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/spc.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/spc.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/td_bert.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/td_bert.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/td_bert_qa.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/td_bert_qa.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/models/singletarget/tdbertlikesingle.py` & `NewsSentiment-1.1.9/NewsSentiment/models/singletarget/tdbertlikesingle.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/plotter_utils.py` & `NewsSentiment-1.1.9/NewsSentiment/plotter_utils.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment/train.py` & `NewsSentiment-1.1.9/NewsSentiment/train.py`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/NewsSentiment.egg-info/PKG-INFO` & `NewsSentiment-1.1.9/NewsSentiment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsSentiment
-Version: 1.1.8
+Version: 1.1.9
 Summary: Easy-to-use, high-quality target-dependent sentiment classification for news articles
 Home-page: https://github.com/fhamborg/NewsMTSC
 Author: Felix Hamborg
 Author-email: felix.hamborg@uni-konstanz.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fhamborg/NewsMTSC/issues
 Platform: UNKNOWN
```

### Comparing `NewsSentiment-1.1.8/NewsSentiment.egg-info/SOURCES.txt` & `NewsSentiment-1.1.9/NewsSentiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/PKG-INFO` & `NewsSentiment-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsSentiment
-Version: 1.1.8
+Version: 1.1.9
 Summary: Easy-to-use, high-quality target-dependent sentiment classification for news articles
 Home-page: https://github.com/fhamborg/NewsMTSC
 Author: Felix Hamborg
 Author-email: felix.hamborg@uni-konstanz.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fhamborg/NewsMTSC/issues
 Platform: UNKNOWN
```

### Comparing `NewsSentiment-1.1.8/README.md` & `NewsSentiment-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/READMEpypi.md` & `NewsSentiment-1.1.9/READMEpypi.md`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/pythoninfo.md` & `NewsSentiment-1.1.9/pythoninfo.md`

 * *Files identical despite different names*

### Comparing `NewsSentiment-1.1.8/setup.cfg` & `NewsSentiment-1.1.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = NewsSentiment
-version = 1.1.8
+version = 1.1.9
 author = Felix Hamborg
 author_email = felix.hamborg@uni-konstanz.de
 description = Easy-to-use, high-quality target-dependent sentiment classification for news articles
 long_description = file: READMEpypi.md
 long_description_content_type = text/markdown
 url = https://github.com/fhamborg/NewsMTSC
 project_urls =
```

