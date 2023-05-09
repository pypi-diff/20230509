# Comparing `tmp/evalplus-0.1.2.tar.gz` & `tmp/evalplus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalplus-0.1.2.tar", last modified: Sun May  7 04:56:48 2023, max compression
+gzip compressed data, was "evalplus-0.1.3.tar", last modified: Tue May  9 17:17:46 2023, max compression
```

## Comparing `evalplus-0.1.2.tar` & `evalplus-0.1.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3272 2023-05-07 04:41:37.000000 evalplus-0.1.2/.dockerignore
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-05 23:34:50.000000 evalplus-0.1.2/.gitignore
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.2/.pre-commit-config.yaml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1221 2023-05-05 20:32:21.000000 evalplus-0.1.2/CITATION.cff
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      290 2023-05-07 04:49:10.000000 evalplus-0.1.2/Dockerfile
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.2/LICENSE
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.2/MANIFEST.in
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6603 2023-05-07 04:56:48.282388 evalplus-0.1.2/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6156 2023-05-07 04:56:35.000000 evalplus-0.1.2/README.md
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/codegen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5512 2023-05-05 07:50:38.000000 evalplus-0.1.2/codegen/generate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    22452 2023-05-04 22:42:14.000000 evalplus-0.1.2/codegen/model.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.2/evalplus/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus/_version.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/data/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7130 2023-05-05 23:35:22.000000 evalplus-0.1.2/evalplus/data/__init__.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/eval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6818 2023-05-05 23:35:22.000000 evalplus-0.1.2/evalplus/eval/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.2/evalplus/eval/utils.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7446 2023-05-06 01:17:43.000000 evalplus-0.1.2/evalplus/evaluate.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/gen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.2/evalplus/gen/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.2/evalplus/gen/chatgpt_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.2/evalplus/gen/mut_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.2/evalplus/gen/type_mut.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus/gen/util/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.2/evalplus/gen/util/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.2/evalplus/gen/util/api_request.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.2/evalplus/inputgen.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/evalplus.egg-info/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6603 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1133 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/SOURCES.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/dependency_links.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/entry_points.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/requires.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-05-07 04:56:48.000000 evalplus-0.1.2/evalplus.egg-info/top_level.txt
--rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1894 2023-05-05 23:34:50.000000 evalplus-0.1.2/evo.sh
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/gallary/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    96092 2023-05-02 00:08:40.000000 evalplus-0.1.2/gallary/overview.png
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.2/gallary/render.gif
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.2/pyproject.toml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.2/requirements-llm.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.2/requirements-tools.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.2/requirements.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-05-07 04:56:48.282388 evalplus-0.1.2/setup.cfg
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/tools/
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/tools/_experimental/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.2/tools/_experimental/README.md
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/_experimental/set_cover.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/_experimental/topset_distill.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3413 2023-04-29 17:26:54.000000 evalplus-0.1.2/tools/checker.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/filter_inputs.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-07 04:56:48.282388 evalplus-0.1.2/tools/humaneval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/humaneval/check_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/humaneval/init_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.2/tools/init_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.2/tools/merge_dataset.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/render.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3739 2023-04-28 21:35:44.000000 evalplus-0.1.2/tools/sanitize.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.2/tools/stat_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.2/tools/viz_passrate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      917 2023-05-03 04:36:53.000000 evalplus-0.1.2/zipper.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.527008 evalplus-0.1.3/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3272 2023-05-07 04:41:37.000000 evalplus-0.1.3/.dockerignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-09 16:43:25.000000 evalplus-0.1.3/.gitignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.3/.pre-commit-config.yaml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1142 2023-05-07 05:34:58.000000 evalplus-0.1.3/CITATION.cff
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      290 2023-05-07 04:49:10.000000 evalplus-0.1.3/Dockerfile
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.3/LICENSE
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.3/MANIFEST.in
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7010 2023-05-09 17:17:46.527008 evalplus-0.1.3/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6563 2023-05-07 05:29:37.000000 evalplus-0.1.3/README.md
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/codegen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5512 2023-05-05 07:50:38.000000 evalplus-0.1.3/codegen/generate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    22452 2023-05-04 22:42:14.000000 evalplus-0.1.3/codegen/model.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/evalplus/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.3/evalplus/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-05-09 17:17:46.000000 evalplus-0.1.3/evalplus/_version.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/evalplus/data/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7191 2023-05-09 17:01:57.000000 evalplus-0.1.3/evalplus/data/__init__.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/evalplus/eval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6808 2023-05-09 17:16:35.000000 evalplus-0.1.3/evalplus/eval/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.3/evalplus/eval/utils.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7448 2023-05-09 17:04:32.000000 evalplus-0.1.3/evalplus/evaluate.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/evalplus/gen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.3/evalplus/gen/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.3/evalplus/gen/chatgpt_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.3/evalplus/gen/mut_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.3/evalplus/gen/type_mut.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/evalplus/gen/util/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.3/evalplus/gen/util/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.3/evalplus/gen/util/api_request.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.3/evalplus/inputgen.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/evalplus.egg-info/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7010 2023-05-09 17:17:46.000000 evalplus-0.1.3/evalplus.egg-info/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1133 2023-05-09 17:17:46.000000 evalplus-0.1.3/evalplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-05-09 17:17:46.000000 evalplus-0.1.3/evalplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-05-09 17:17:46.000000 evalplus-0.1.3/evalplus.egg-info/entry_points.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-05-09 17:17:46.000000 evalplus-0.1.3/evalplus.egg-info/requires.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-05-09 17:17:46.000000 evalplus-0.1.3/evalplus.egg-info/top_level.txt
+-rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1894 2023-05-05 23:34:50.000000 evalplus-0.1.3/evo.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.523008 evalplus-0.1.3/gallary/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    96092 2023-05-02 00:08:40.000000 evalplus-0.1.3/gallary/overview.png
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.3/gallary/render.gif
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.3/pyproject.toml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.3/requirements-llm.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.3/requirements-tools.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.3/requirements.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-05-09 17:17:46.527008 evalplus-0.1.3/setup.cfg
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.527008 evalplus-0.1.3/tools/
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.527008 evalplus-0.1.3/tools/_experimental/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.3/tools/_experimental/README.md
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.3/tools/_experimental/set_cover.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.3/tools/_experimental/topset_distill.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3413 2023-04-29 17:26:54.000000 evalplus-0.1.3/tools/checker.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.3/tools/filter_inputs.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-09 17:17:46.527008 evalplus-0.1.3/tools/humaneval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.3/tools/humaneval/check_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.3/tools/humaneval/init_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.3/tools/init_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.3/tools/merge_dataset.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.3/tools/render.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3739 2023-04-28 21:35:44.000000 evalplus-0.1.3/tools/sanitize.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.3/tools/stat_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.3/tools/viz_passrate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      917 2023-05-03 04:36:53.000000 evalplus-0.1.3/zipper.sh
```

### Comparing `evalplus-0.1.2/.dockerignore` & `evalplus-0.1.3/.dockerignore`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/.gitignore` & `evalplus-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/CITATION.cff` & `evalplus-0.1.3/CITATION.cff`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 message: "If you use this work and love it, consider citing it as below \U0001F917"
 title: EvalPlus
 authors:
   - family-names: EvalPlus Team
 url: https://github.com/evalplus/evalplus
 doi: https://doi.org/10.48550/arXiv.2305.01210
 date-released: 2023-05-01
+license: Apache-2.0
 references:
   type: article
   title: "Is Your Code Generated by ChatGPT Really Correct? Rigorous Evaluation of Large Language Models for Code Generation"
   authors:
     - family-names: Liu
       given-names: Jiawei
       email: jiawei6@illinois.edu
@@ -22,14 +23,11 @@
       given-names: Yuyao
       email: yuyao6@outlook.com
       affiliation: Nanjing University
     - family-names: Zhang
       given-names: Lingming
       email: lingming@illinois.edu
       affiliation: University of Illinois Urbana-Champaign
-  collection-title: arXiv preprint arXiv:2305.01210
-  collection-type: article
   year: 2023
   journal: ArXiv
   doi: https://doi.org/10.48550/arXiv.2305.01210
   url: https://arxiv.org/abs/2305.01210
-license: Apache-2.0
```

### Comparing `evalplus-0.1.2/LICENSE` & `evalplus-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/PKG-INFO` & `evalplus-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: evalplus
-Version: 0.1.2
+Version: 0.1.3
 Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
 Home-page: https://github.com/evalplus/evalplus
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `EvalPlus(📖) => 📚`
 
 <p align="center">
+    <a href="https://pypi.org/project/evalplus/"><img src="https://img.shields.io/pypi/v/evalplus?color=g"></a>
+    <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/evalplus"></a>
+    <a href="https://hub.docker.com/r/ganler/evalplus" title="Docker"><img src="https://img.shields.io/docker/image-size/ganler/evalplus"></a>
+</p>
+
+
+<p align="center">
     <a href="#-Quick-Start">🔥Quick Start</a> •
     <a href="#-Papers">📜Papers</a> •
     <a href="#-Useful-tools">🔨Useful tools</a> •
     <a href="#-Development">👷Development</a> •
     <a href="#-Acknowledgement">🙏Acknowledgement</a>
 </p>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.2 Summary: "EvalPlus for
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.3 Summary: "EvalPlus for
 rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
 evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
 (ð) => ð`
+[https://img.shields.io/pypi/v/evalplus?color=g] [https://img.shields.io/pypi/
+    l/evalplus] [https://img.shields.io/docker/image-size/ganler/evalplus]
   ð¥Quick_Start â¢ ðPapers â¢ ð¨Useful_tools â¢ ð·Development â¢
                               ðAcknowledgement
 > **Warning** >
   > > ð¨ Evaluating LLM-generated code over datasets with "3 test-cases" is
                            **NOT** enough! ð¨ > >
 To address this, we started the EvalPlus project -- a rigourous evaluation
 framework for LLM4Code that: + â¨ improves code benchmarks by adding up to
```

### Comparing `evalplus-0.1.2/README.md` & `evalplus-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # `EvalPlus(📖) => 📚`
 
 <p align="center">
+    <a href="https://pypi.org/project/evalplus/"><img src="https://img.shields.io/pypi/v/evalplus?color=g"></a>
+    <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/evalplus"></a>
+    <a href="https://hub.docker.com/r/ganler/evalplus" title="Docker"><img src="https://img.shields.io/docker/image-size/ganler/evalplus"></a>
+</p>
+
+
+<p align="center">
     <a href="#-Quick-Start">🔥Quick Start</a> •
     <a href="#-Papers">📜Papers</a> •
     <a href="#-Useful-tools">🔨Useful tools</a> •
     <a href="#-Development">👷Development</a> •
     <a href="#-Acknowledgement">🙏Acknowledgement</a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
 # `EvalPlus(ð) => ð`
+[https://img.shields.io/pypi/v/evalplus?color=g] [https://img.shields.io/pypi/
+    l/evalplus] [https://img.shields.io/docker/image-size/ganler/evalplus]
   ð¥Quick_Start â¢ ðPapers â¢ ð¨Useful_tools â¢ ð·Development â¢
                               ðAcknowledgement
 > **Warning** >
   > > ð¨ Evaluating LLM-generated code over datasets with "3 test-cases" is
                            **NOT** enough! ð¨ > >
 To address this, we started the EvalPlus project -- a rigourous evaluation
 framework for LLM4Code that: + â¨ improves code benchmarks by adding up to
```

### Comparing `evalplus-0.1.2/codegen/generate.py` & `evalplus-0.1.3/codegen/generate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/codegen/model.py` & `evalplus-0.1.3/codegen/model.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/data/__init__.py` & `evalplus-0.1.3/evalplus/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,28 +68,28 @@
     Different from `sample.jsonl`, the solutions must be complete (with prompt prefix).
     """
 
     # if it is a file
     if os.path.isfile(sample_path):
         for sample in stream_jsonl(sample_path):
             yield sample
-
-    # if it is a folder
-    for task_id in os.listdir(sample_path):
-        task_path = os.path.join(sample_path, task_id)
-        if os.path.isdir(task_path):
-            for solution_id in os.listdir(task_path):
-                solution_path = os.path.join(task_path, solution_id)
-                if os.path.isfile(solution_path) and solution_path.endswith(".py"):
-                    with open(solution_path, "r") as f:
-                        completion = f.read()
-                    yield {
-                        "task_id": task_id.replace("HumanEval_", "HumanEval/"),
-                        "solution": completion,
-                    }
+    else:
+        # if it is a folder
+        for task_id in os.listdir(sample_path):
+            task_path = os.path.join(sample_path, task_id)
+            if os.path.isdir(task_path):
+                for solution_id in os.listdir(task_path):
+                    solution_path = os.path.join(task_path, solution_id)
+                    if os.path.isfile(solution_path) and solution_path.endswith(".py"):
+                        with open(solution_path, "r") as f:
+                            completion = f.read()
+                        yield {
+                            "task_id": task_id.replace("HumanEval_", "HumanEval/"),
+                            "solution": completion,
+                        }
 
 
 def get_human_eval_plus(err_incomplete=True) -> Dict[str, Dict]:
     """Get HumanEvalPlus locally.
     Args:
         err_incomplete (bool, optional): Whether to raise error if HumanEvalPlus is not complete. Defaults to True.
     Returns:
```

### Comparing `evalplus-0.1.2/evalplus/eval/__init__.py` & `evalplus-0.1.3/evalplus/eval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     if not stat:
         stat = TIMEOUT
 
     if stat == SUCCESS:
         if len(details) != len(inputs) or not all(details):
             stat = FAILED
 
-    return stat, np.array(details)
+    return stat, details
 
 
 def evaluate_files(
     files: List[str],
     inputs: List,
     expected: List,
     entry_point: str,
```

### Comparing `evalplus-0.1.2/evalplus/eval/utils.py` & `evalplus-0.1.3/evalplus/eval/utils.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/evaluate.py` & `evalplus-0.1.3/evalplus/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         n_workers = max(1, multiprocessing.cpu_count() // 2)
     else:
         n_workers = flags.parallel
 
     if os.path.isdir(flags.samples):
         result_path = os.path.join(flags.samples, "eval_results.json")
     else:
-        assert flags.samples.endswith(".json")
-        result_path = flags.samples.replace(".json", "_eval_results.json")
+        assert flags.samples.endswith(".jsonl")
+        result_path = flags.samples.replace(".jsonl", "_eval_results.json")
 
     if os.path.isfile(result_path) and not flags.i_just_wanna_run:
         print(f"Load from {result_path}")
         with open(result_path, "r") as f:
             results = json.load(f)
 
         results = compatible_eval_result(results)
```

### Comparing `evalplus-0.1.2/evalplus/gen/__init__.py` & `evalplus-0.1.3/evalplus/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/gen/chatgpt_gen.py` & `evalplus-0.1.3/evalplus/gen/chatgpt_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/gen/mut_gen.py` & `evalplus-0.1.3/evalplus/gen/mut_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/gen/type_mut.py` & `evalplus-0.1.3/evalplus/gen/type_mut.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/gen/util/__init__.py` & `evalplus-0.1.3/evalplus/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/gen/util/api_request.py` & `evalplus-0.1.3/evalplus/gen/util/api_request.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus/inputgen.py` & `evalplus-0.1.3/evalplus/inputgen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evalplus.egg-info/PKG-INFO` & `evalplus-0.1.3/evalplus.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 Metadata-Version: 2.1
 Name: evalplus
-Version: 0.1.2
+Version: 0.1.3
 Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
 Home-page: https://github.com/evalplus/evalplus
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `EvalPlus(📖) => 📚`
 
 <p align="center">
+    <a href="https://pypi.org/project/evalplus/"><img src="https://img.shields.io/pypi/v/evalplus?color=g"></a>
+    <a href="https://github.com/evalplus/evalplus/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/evalplus"></a>
+    <a href="https://hub.docker.com/r/ganler/evalplus" title="Docker"><img src="https://img.shields.io/docker/image-size/ganler/evalplus"></a>
+</p>
+
+
+<p align="center">
     <a href="#-Quick-Start">🔥Quick Start</a> •
     <a href="#-Papers">📜Papers</a> •
     <a href="#-Useful-tools">🔨Useful tools</a> •
     <a href="#-Development">👷Development</a> •
     <a href="#-Acknowledgement">🙏Acknowledgement</a>
 </p>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.2 Summary: "EvalPlus for
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.3 Summary: "EvalPlus for
 rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
 evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
 (ð) => ð`
+[https://img.shields.io/pypi/v/evalplus?color=g] [https://img.shields.io/pypi/
+    l/evalplus] [https://img.shields.io/docker/image-size/ganler/evalplus]
   ð¥Quick_Start â¢ ðPapers â¢ ð¨Useful_tools â¢ ð·Development â¢
                               ðAcknowledgement
 > **Warning** >
   > > ð¨ Evaluating LLM-generated code over datasets with "3 test-cases" is
                            **NOT** enough! ð¨ > >
 To address this, we started the EvalPlus project -- a rigourous evaluation
 framework for LLM4Code that: + â¨ improves code benchmarks by adding up to
```

### Comparing `evalplus-0.1.2/evalplus.egg-info/SOURCES.txt` & `evalplus-0.1.3/evalplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/evo.sh` & `evalplus-0.1.3/evo.sh`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/gallary/overview.png` & `evalplus-0.1.3/gallary/overview.png`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/gallary/render.gif` & `evalplus-0.1.3/gallary/render.gif`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/setup.cfg` & `evalplus-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/_experimental/set_cover.py` & `evalplus-0.1.3/tools/_experimental/set_cover.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/_experimental/topset_distill.py` & `evalplus-0.1.3/tools/_experimental/topset_distill.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/checker.py` & `evalplus-0.1.3/tools/checker.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/filter_inputs.py` & `evalplus-0.1.3/tools/filter_inputs.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/humaneval/check_ground_truth.py` & `evalplus-0.1.3/tools/humaneval/check_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/humaneval/init_plus.py` & `evalplus-0.1.3/tools/humaneval/init_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/init_ground_truth.py` & `evalplus-0.1.3/tools/init_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/merge_dataset.py` & `evalplus-0.1.3/tools/merge_dataset.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/render.py` & `evalplus-0.1.3/tools/render.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/sanitize.py` & `evalplus-0.1.3/tools/sanitize.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/stat_plus.py` & `evalplus-0.1.3/tools/stat_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/tools/viz_passrate.py` & `evalplus-0.1.3/tools/viz_passrate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.2/zipper.sh` & `evalplus-0.1.3/zipper.sh`

 * *Files identical despite different names*

