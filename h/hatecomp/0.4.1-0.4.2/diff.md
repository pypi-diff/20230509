# Comparing `tmp/hatecomp-0.4.1.tar.gz` & `tmp/hatecomp-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatecomp-0.4.1.tar", last modified: Mon May  8 20:02:21 2023, max compression
+gzip compressed data, was "hatecomp-0.4.2.tar", last modified: Mon May  8 22:31:08 2023, max compression
```

## Comparing `hatecomp-0.4.1.tar` & `hatecomp-0.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.693391 hatecomp-0.4.1/
--rwxrwxrwx   0 root         (0) root         (0)     8693 2023-05-08 20:02:21.693240 hatecomp-0.4.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     8377 2023-05-08 19:58:09.000000 hatecomp-0.4.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.681018 hatecomp-0.4.1/hatecomp/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/_path.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.682595 hatecomp-0.4.1/hatecomp/datasets/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.682842 hatecomp-0.4.1/hatecomp/datasets/AMI/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/AMI/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.683054 hatecomp-0.4.1/hatecomp/datasets/CONAN/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/CONAN/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.683272 hatecomp-0.4.1/hatecomp/datasets/Fox/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/Fox/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.683975 hatecomp-0.4.1/hatecomp/datasets/HASOC/
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/HASOC/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1243 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/HASOC/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1705 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/HASOC/download.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.684236 hatecomp-0.4.1/hatecomp/datasets/HateTwitter/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/HateTwitter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.684946 hatecomp-0.4.1/hatecomp/datasets/MLMA/
--rwxrwxrwx   0 root         (0) root         (0)       55 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/MLMA/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2947 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/MLMA/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/MLMA/download.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.685202 hatecomp-0.4.1/hatecomp/datasets/MultiTwitter/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/MultiTwitter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.685416 hatecomp-0.4.1/hatecomp/datasets/OnlineInter/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/OnlineInter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.686154 hatecomp-0.4.1/hatecomp/datasets/TwitterSexism/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/TwitterSexism/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1055 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/TwitterSexism/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     2038 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/TwitterSexism/download.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.686437 hatecomp-0.4.1/hatecomp/datasets/UBWeb/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.686637 hatecomp-0.4.1/hatecomp/datasets/UBWeb/Facebook/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/UBWeb/Facebook/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.686826 hatecomp-0.4.1/hatecomp/datasets/UBWeb/League/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/UBWeb/League/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.686985 hatecomp-0.4.1/hatecomp/datasets/UBWeb/Twitter/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/UBWeb/Twitter/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.687184 hatecomp-0.4.1/hatecomp/datasets/UBWeb/WoW/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/UBWeb/WoW/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/UBWeb/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.687800 hatecomp-0.4.1/hatecomp/datasets/Vicomtech/
--rwxrwxrwx   0 root         (0) root         (0)       64 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/Vicomtech/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1139 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/Vicomtech/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1832 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/Vicomtech/download.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.688434 hatecomp-0.4.1/hatecomp/datasets/WikiTalk/
--rwxrwxrwx   0 root         (0) root         (0)      135 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/WikiTalk/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5289 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/WikiTalk/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     1894 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/WikiTalk/download.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.689056 hatecomp-0.4.1/hatecomp/datasets/ZeerakTalat/
--rwxrwxrwx   0 root         (0) root         (0)       78 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/ZeerakTalat/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2652 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/ZeerakTalat/dataset.py
--rwxrwxrwx   0 root         (0) root         (0)     3427 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/ZeerakTalat/download.py
--rwxrwxrwx   0 root         (0) root         (0)      644 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.689979 hatecomp-0.4.1/hatecomp/datasets/base/
--rwxrwxrwx   0 root         (0) root         (0)       51 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5408 2023-05-08 19:56:37.000000 hatecomp-0.4.1/hatecomp/datasets/base/data.py
--rwxrwxrwx   0 root         (0) root         (0)     3693 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/base/download.py
--rwxrwxrwx   0 root         (0) root         (0)     2410 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/datasets/base/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.691405 hatecomp-0.4.1/hatecomp/models/
--rwxrwxrwx   0 root         (0) root         (0)      108 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/models/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3723 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/models/auto.py
--rwxrwxrwx   0 root         (0) root         (0)     2883 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/models/download.py
--rwxrwxrwx   0 root         (0) root         (0)     7248 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/models/embed.py
--rwxrwxrwx   0 root         (0) root         (0)     2962 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/models/model_registry.json
--rwxrwxrwx   0 root         (0) root         (0)     2689 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/models/tokenizer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.692507 hatecomp-0.4.1/hatecomp/training/
--rwxrwxrwx   0 root         (0) root         (0)      140 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/training/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10375 2023-05-08 18:27:08.000000 hatecomp-0.4.1/hatecomp/training/functional.py
--rwxrwxrwx   0 root         (0) root         (0)     7823 2023-05-08 18:31:30.000000 hatecomp-0.4.1/hatecomp/training/hatecomp_trial.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/training/metrics.py
--rwxrwxrwx   0 root         (0) root         (0)     8049 2023-05-08 18:30:21.000000 hatecomp-0.4.1/hatecomp/training/trainer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.692916 hatecomp-0.4.1/hatecomp/tweets/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/tweets/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4369 2023-05-08 17:57:46.000000 hatecomp-0.4.1/hatecomp/tweets/fetch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 20:02:21.682329 hatecomp-0.4.1/hatecomp.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     8693 2023-05-08 20:02:21.000000 hatecomp-0.4.1/hatecomp.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1899 2023-05-08 20:02:21.000000 hatecomp-0.4.1/hatecomp.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-08 20:02:21.000000 hatecomp-0.4.1/hatecomp.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      155 2023-05-08 20:02:21.000000 hatecomp-0.4.1/hatecomp.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-05-08 20:02:21.000000 hatecomp-0.4.1/hatecomp.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-08 20:02:21.693448 hatecomp-0.4.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1057 2023-05-08 20:01:37.000000 hatecomp-0.4.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.833646 hatecomp-0.4.2/
+-rwxrwxrwx   0 root         (0) root         (0)     8693 2023-05-08 22:31:08.833511 hatecomp-0.4.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     8377 2023-05-08 19:58:09.000000 hatecomp-0.4.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.818375 hatecomp-0.4.2/hatecomp/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/_path.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.819900 hatecomp-0.4.2/hatecomp/datasets/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.820138 hatecomp-0.4.2/hatecomp/datasets/AMI/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/AMI/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.820330 hatecomp-0.4.2/hatecomp/datasets/CONAN/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/CONAN/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.820654 hatecomp-0.4.2/hatecomp/datasets/Fox/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/Fox/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.821744 hatecomp-0.4.2/hatecomp/datasets/HASOC/
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/HASOC/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/HASOC/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1705 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/HASOC/download.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.822127 hatecomp-0.4.2/hatecomp/datasets/HateTwitter/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/HateTwitter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.823191 hatecomp-0.4.2/hatecomp/datasets/MLMA/
+-rwxrwxrwx   0 root         (0) root         (0)       55 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/MLMA/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2947 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/MLMA/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/MLMA/download.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.823584 hatecomp-0.4.2/hatecomp/datasets/MultiTwitter/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/MultiTwitter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.823916 hatecomp-0.4.2/hatecomp/datasets/OnlineInter/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/OnlineInter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.824988 hatecomp-0.4.2/hatecomp/datasets/TwitterSexism/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/TwitterSexism/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1055 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/TwitterSexism/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     2038 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/TwitterSexism/download.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.825394 hatecomp-0.4.2/hatecomp/datasets/UBWeb/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.825733 hatecomp-0.4.2/hatecomp/datasets/UBWeb/Facebook/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/UBWeb/Facebook/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.826058 hatecomp-0.4.2/hatecomp/datasets/UBWeb/League/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/UBWeb/League/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.826385 hatecomp-0.4.2/hatecomp/datasets/UBWeb/Twitter/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/UBWeb/Twitter/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.826705 hatecomp-0.4.2/hatecomp/datasets/UBWeb/WoW/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/UBWeb/WoW/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/UBWeb/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.827727 hatecomp-0.4.2/hatecomp/datasets/Vicomtech/
+-rwxrwxrwx   0 root         (0) root         (0)       64 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/Vicomtech/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1139 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/Vicomtech/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1832 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/Vicomtech/download.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.828782 hatecomp-0.4.2/hatecomp/datasets/WikiTalk/
+-rwxrwxrwx   0 root         (0) root         (0)      135 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/WikiTalk/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5289 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/WikiTalk/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     1894 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/WikiTalk/download.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.829541 hatecomp-0.4.2/hatecomp/datasets/ZeerakTalat/
+-rwxrwxrwx   0 root         (0) root         (0)       78 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/ZeerakTalat/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2652 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/ZeerakTalat/dataset.py
+-rwxrwxrwx   0 root         (0) root         (0)     3427 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/ZeerakTalat/download.py
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.830418 hatecomp-0.4.2/hatecomp/datasets/base/
+-rwxrwxrwx   0 root         (0) root         (0)       51 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5408 2023-05-08 19:56:37.000000 hatecomp-0.4.2/hatecomp/datasets/base/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     3693 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/base/download.py
+-rwxrwxrwx   0 root         (0) root         (0)     2410 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/datasets/base/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.831742 hatecomp-0.4.2/hatecomp/models/
+-rwxrwxrwx   0 root         (0) root         (0)      108 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3756 2023-05-08 22:25:09.000000 hatecomp-0.4.2/hatecomp/models/auto.py
+-rwxrwxrwx   0 root         (0) root         (0)     2883 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/models/download.py
+-rwxrwxrwx   0 root         (0) root         (0)     7248 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/models/embed.py
+-rwxrwxrwx   0 root         (0) root         (0)     2962 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/models/model_registry.json
+-rwxrwxrwx   0 root         (0) root         (0)     2689 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/models/tokenizer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.832787 hatecomp-0.4.2/hatecomp/training/
+-rwxrwxrwx   0 root         (0) root         (0)      140 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/training/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10375 2023-05-08 18:27:08.000000 hatecomp-0.4.2/hatecomp/training/functional.py
+-rwxrwxrwx   0 root         (0) root         (0)     7823 2023-05-08 18:31:30.000000 hatecomp-0.4.2/hatecomp/training/hatecomp_trial.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/training/metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)     8049 2023-05-08 18:30:21.000000 hatecomp-0.4.2/hatecomp/training/trainer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.833191 hatecomp-0.4.2/hatecomp/tweets/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/tweets/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4369 2023-05-08 17:57:46.000000 hatecomp-0.4.2/hatecomp/tweets/fetch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-08 22:31:08.819652 hatecomp-0.4.2/hatecomp.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     8693 2023-05-08 22:31:08.000000 hatecomp-0.4.2/hatecomp.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1899 2023-05-08 22:31:08.000000 hatecomp-0.4.2/hatecomp.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-08 22:31:08.000000 hatecomp-0.4.2/hatecomp.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      155 2023-05-08 22:31:08.000000 hatecomp-0.4.2/hatecomp.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-05-08 22:31:08.000000 hatecomp-0.4.2/hatecomp.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-08 22:31:08.833695 hatecomp-0.4.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1057 2023-05-08 22:30:36.000000 hatecomp-0.4.2/setup.py
```

### Comparing `hatecomp-0.4.1/PKG-INFO` & `hatecomp-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatecomp
-Version: 0.4.1
+Version: 0.4.2
 Summary: Collection of pytorch datasets for hate speech and toxic internet discourse
 Home-page: https://github.com/HesitantlyHuman/hatecomp
 Author: HesitantlyHuman
 Author-email: tannersims@hesitantlyhuman.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hatecomp-0.4.1/README.md` & `hatecomp-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/HASOC/dataset.py` & `hatecomp-0.4.2/hatecomp/datasets/HASOC/dataset.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/HASOC/download.py` & `hatecomp-0.4.2/hatecomp/datasets/HASOC/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/MLMA/dataset.py` & `hatecomp-0.4.2/hatecomp/datasets/MLMA/dataset.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/MLMA/download.py` & `hatecomp-0.4.2/hatecomp/datasets/MLMA/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/TwitterSexism/dataset.py` & `hatecomp-0.4.2/hatecomp/datasets/TwitterSexism/dataset.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/TwitterSexism/download.py` & `hatecomp-0.4.2/hatecomp/datasets/TwitterSexism/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/Vicomtech/dataset.py` & `hatecomp-0.4.2/hatecomp/datasets/Vicomtech/dataset.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/Vicomtech/download.py` & `hatecomp-0.4.2/hatecomp/datasets/Vicomtech/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/WikiTalk/dataset.py` & `hatecomp-0.4.2/hatecomp/datasets/WikiTalk/dataset.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/WikiTalk/download.py` & `hatecomp-0.4.2/hatecomp/datasets/WikiTalk/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/ZeerakTalat/dataset.py` & `hatecomp-0.4.2/hatecomp/datasets/ZeerakTalat/dataset.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/ZeerakTalat/download.py` & `hatecomp-0.4.2/hatecomp/datasets/ZeerakTalat/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/__init__.py` & `hatecomp-0.4.2/hatecomp/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/base/data.py` & `hatecomp-0.4.2/hatecomp/datasets/base/data.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/base/download.py` & `hatecomp-0.4.2/hatecomp/datasets/base/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/datasets/base/utils.py` & `hatecomp-0.4.2/hatecomp/datasets/base/utils.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/models/auto.py` & `hatecomp-0.4.2/hatecomp/models/auto.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import os
 import json
 import logging
 
 import torch
 from transformers import AutoModel
 
-from hatecomp.models.download import verify_pretrained_download, PRETRAINED_INSTALLATION_LOCATION
+from hatecomp.models.download import (
+    verify_pretrained_download,
+    PRETRAINED_INSTALLATION_LOCATION,
+)
 
 # Suppress the huggingface warning about fine tuning the model
 logging.getLogger("transformers.modeling_utils").setLevel(logging.ERROR)
 
 
 class HatecompClassifier(torch.nn.Module):
     def __init__(
@@ -83,15 +86,15 @@
             config["dropout"],
         )
 
         # Load the state dict
         state_dict_path = os.path.join(
             PRETRAINED_INSTALLATION_LOCATION, pretrained_model_name_or_path, "model.pt"
         )
-        model.load_state_dict(torch.load(state_dict_path))
+        model.load_state_dict(torch.load(state_dict_path, map_location="cpu"))
 
         # Return the model
         return model
 
 
 class HatecompClassificationHead(torch.nn.Module):
     def __init__(
```

### Comparing `hatecomp-0.4.1/hatecomp/models/download.py` & `hatecomp-0.4.2/hatecomp/models/download.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/models/embed.py` & `hatecomp-0.4.2/hatecomp/models/embed.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/models/model_registry.json` & `hatecomp-0.4.2/hatecomp/models/model_registry.json`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/models/tokenizer.py` & `hatecomp-0.4.2/hatecomp/models/tokenizer.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/training/functional.py` & `hatecomp-0.4.2/hatecomp/training/functional.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/training/hatecomp_trial.py` & `hatecomp-0.4.2/hatecomp/training/hatecomp_trial.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/training/trainer.py` & `hatecomp-0.4.2/hatecomp/training/trainer.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp/tweets/fetch.py` & `hatecomp-0.4.2/hatecomp/tweets/fetch.py`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/hatecomp.egg-info/PKG-INFO` & `hatecomp-0.4.2/hatecomp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatecomp
-Version: 0.4.1
+Version: 0.4.2
 Summary: Collection of pytorch datasets for hate speech and toxic internet discourse
 Home-page: https://github.com/HesitantlyHuman/hatecomp
 Author: HesitantlyHuman
 Author-email: tannersims@hesitantlyhuman.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `hatecomp-0.4.1/hatecomp.egg-info/SOURCES.txt` & `hatecomp-0.4.2/hatecomp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hatecomp-0.4.1/setup.py` & `hatecomp-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 PACKAGE_ROOT = os.path.dirname(os.path.realpath(__file__))
 README_FILE = open(os.path.join(PACKAGE_ROOT, "README.md"), "r").read()
 
 if __name__ == "__main__":
     setup(
         name="hatecomp",
-        version="0.4.1",
+        version="0.4.2",
         description="Collection of pytorch datasets for hate speech and toxic internet discourse",
         long_description=README_FILE,
         long_description_content_type="text/markdown",
         url="https://github.com/HesitantlyHuman/hatecomp",
         author="HesitantlyHuman",
         author_email="tannersims@hesitantlyhuman.com",
         license="MIT",
```

