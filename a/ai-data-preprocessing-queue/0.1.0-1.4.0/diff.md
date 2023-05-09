# Comparing `tmp/ai-data-preprocessing-queue-0.1.0.tar.gz` & `tmp/ai-data-preprocessing-queue-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-data-preprocessing-queue-0.1.0.tar", last modified: Tue May  9 06:21:02 2023, max compression
+gzip compressed data, was "ai-data-preprocessing-queue-1.4.0.tar", last modified: Tue May  9 06:24:34 2023, max compression
```

## Comparing `ai-data-preprocessing-queue-0.1.0.tar` & `ai-data-preprocessing-queue-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:21:02.949481 ai-data-preprocessing-queue-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-09 06:21:02.949481 ai-data-preprocessing-queue-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:21:02.949481 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/StepProcessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:21:02.949481 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/language_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/regex_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/remove_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/remove_punctuation.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/snowball_stemmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/spellcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/text_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/to_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/token_replacement.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:21:02.949481 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-09 06:21:02.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-09 06:21:02.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:21:02.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 06:21:02.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 06:21:02.000000 ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 06:21:02.949481 ai-data-preprocessing-queue-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:21:02.949481 ai-data-preprocessing-queue-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-09 06:20:54.000000 ai-data-preprocessing-queue-0.1.0/tests/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:34.715556 ai-data-preprocessing-queue-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-09 06:24:34.715556 ai-data-preprocessing-queue-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:34.715556 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/StepProcessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:34.715556 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/language_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/regex_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/remove_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/remove_punctuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/snowball_stemmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/spellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/text_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/to_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/token_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:34.715556 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-09 06:24:34.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-09 06:24:34.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:24:34.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 06:24:34.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 06:24:34.000000 ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 06:24:34.715556 ai-data-preprocessing-queue-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:34.715556 ai-data-preprocessing-queue-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-09 06:24:23.000000 ai-data-preprocessing-queue-1.4.0/tests/test_pipeline.py
```

### Comparing `ai-data-preprocessing-queue-0.1.0/LICENSE.txt` & `ai-data-preprocessing-queue-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/PKG-INFO` & `ai-data-preprocessing-queue-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-data-preprocessing-queue
-Version: 0.1.0
+Version: 1.4.0
 Summary: Can be used to pre process data before ai processing
 Home-page: https://github.com/SamhammerAG/ai_data_preprocessing_queue
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/ai_data_preprocessing_queue
 Project-URL: Bug Reports, https://github.com/SamhammerAG/ai_data_preprocessing_queue/issues
```

### Comparing `ai-data-preprocessing-queue-0.1.0/README.md` & `ai-data-preprocessing-queue-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Pipeline.py` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Pipeline.py`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/StepProcessor.py` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/StepProcessor.py`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/language_detect.py` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/language_detect.py`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/regex_replacement.py` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/regex_replacement.py`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/snowball_stemmer.py` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/snowball_stemmer.py`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/spellcheck.py` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/spellcheck.py`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue/Steps/token_replacement.py` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue/Steps/token_replacement.py`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/PKG-INFO` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-data-preprocessing-queue
-Version: 0.1.0
+Version: 1.4.0
 Summary: Can be used to pre process data before ai processing
 Home-page: https://github.com/SamhammerAG/ai_data_preprocessing_queue
 Author: Samhammer AG
 Author-email: support@samhammer.de
 License: MIT
 Project-URL: Documentation, https://github.com/SamhammerAG/ai_data_preprocessing_queue
 Project-URL: Bug Reports, https://github.com/SamhammerAG/ai_data_preprocessing_queue/issues
```

### Comparing `ai-data-preprocessing-queue-0.1.0/ai_data_preprocessing_queue.egg-info/SOURCES.txt` & `ai-data-preprocessing-queue-1.4.0/ai_data_preprocessing_queue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai-data-preprocessing-queue-0.1.0/setup.py` & `ai-data-preprocessing-queue-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     REQS = fin.read().splitlines()
 
 with open("requirements-dev.txt", "r") as fin:
     REQS_DEV = [item for item in fin.read().splitlines() if not item.endswith(".txt")]
 
 setuptools.setup(
     name="ai-data-preprocessing-queue",
-    version="0.1.0",
+    version="1.4.0",
     description="Can be used to pre process data before ai processing",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/SamhammerAG/ai_data_preprocessing_queue",
     author="Samhammer AG",
     author_email="support@samhammer.de",
     license="MIT",
```

### Comparing `ai-data-preprocessing-queue-0.1.0/tests/test_pipeline.py` & `ai-data-preprocessing-queue-1.4.0/tests/test_pipeline.py`

 * *Files identical despite different names*

