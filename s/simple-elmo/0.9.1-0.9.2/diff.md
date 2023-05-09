# Comparing `tmp/simple_elmo-0.9.1.tar.gz` & `tmp/simple_elmo-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_elmo-0.9.1.tar", last modified: Tue Jan  3 16:17:49 2023, max compression
+gzip compressed data, was "simple_elmo-0.9.2.tar", last modified: Tue May  9 17:57:15 2023, max compression
```

## Comparing `simple_elmo-0.9.1.tar` & `simple_elmo-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:17:49.837546 simple_elmo-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-01-03 16:17:49.837546 simple_elmo-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-03 16:17:49.837546 simple_elmo-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:17:49.837546 simple_elmo-0.9.1/simple_elmo/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/simple_elmo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16961 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/simple_elmo/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/simple_elmo/elmo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20498 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/simple_elmo/elmo_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27527 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/simple_elmo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    45942 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/simple_elmo/training.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-01-03 16:17:40.000000 simple_elmo-0.9.1/simple_elmo/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 16:17:49.837546 simple_elmo-0.9.1/simple_elmo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-01-03 16:17:49.000000 simple_elmo-0.9.1/simple_elmo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-03 16:17:49.000000 simple_elmo-0.9.1/simple_elmo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 16:17:49.000000 simple_elmo-0.9.1/simple_elmo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-03 16:17:49.000000 simple_elmo-0.9.1/simple_elmo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-03 16:17:49.000000 simple_elmo-0.9.1/simple_elmo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:57:15.099523 simple_elmo-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-05-09 17:57:15.099523 simple_elmo-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:57:15.099523 simple_elmo-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:57:15.095523 simple_elmo-0.9.2/simple_elmo/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/simple_elmo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16961 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/simple_elmo/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/simple_elmo/elmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20599 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/simple_elmo/elmo_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27527 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/simple_elmo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45942 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/simple_elmo/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      510 2023-05-09 17:57:04.000000 simple_elmo-0.9.2/simple_elmo/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:57:15.099523 simple_elmo-0.9.2/simple_elmo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-05-09 17:57:14.000000 simple_elmo-0.9.2/simple_elmo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-09 17:57:15.000000 simple_elmo-0.9.2/simple_elmo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:57:14.000000 simple_elmo-0.9.2/simple_elmo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 17:57:14.000000 simple_elmo-0.9.2/simple_elmo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 17:57:14.000000 simple_elmo-0.9.2/simple_elmo.egg-info/top_level.txt
```

### Comparing `simple_elmo-0.9.1/LICENSE` & `simple_elmo-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_elmo-0.9.1/PKG-INFO` & `simple_elmo-0.9.2/simple_elmo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple_elmo
-Version: 0.9.1
+Name: simple-elmo
+Version: 0.9.2
 Summary: Handy library to work with pre-trained ELMo embeddings in TensorFlow
 Home-page: https://github.com/ltgoslo/simple_elmo
 Author: Andrey Kutuzov
 Author-email: andreku@ifi.uio.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -12,35 +12,35 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tf
 Provides-Extra: tf_gpu
 License-File: LICENSE
 
-_Simple_elmo_ is a Python library to work with pre-trained [ELMo embeddings](https://allennlp.org/elmo) in TensorFlow.
+_Simple_elmo_ is a Python library to work with pre-trained [ELMo contextualized language models](https://allennlp.org/elmo) in TensorFlow.
 
 This is a significantly updated wrapper to the [original ELMo implementation](https://github.com/allenai/bilm-tf).
 The main changes are:
 - more convenient and transparent data loading (including from compressed files)
 - code adapted to modern TensorFlow versions (including TensorFlow 2).
 
 # Installation
 
 `pip install --upgrade simple_elmo`
 
-Make sure to update the package regularly, we are actively developing.
+Make sure to update the package regularly.
 
 # Usage
 
  `from simple_elmo import ElmoModel`
 
  `model = ElmoModel()`
 
 ## Loading
- First, let's load a pretrained model from disk:
+ First, let's load a pretrained model:
 
  `model.load(PATH_TO_ELMO)`
 
 ### Required arguments
 
  **PATH_TO_ELMO** is either a ZIP archive downloaded from the [NLPL vector repository](http://vectors.nlpl.eu/repository/),
 OR a directory containing 2 files:
@@ -58,15 +58,15 @@
 
    the maximum number of sentences/documents in a batch during inference;
    your input will be automatically split into chunks of the respective size;
    if your computational resources allow, you might want to increase this value.
 - **limit**: *integer, default 100*;
 
     the number of words from the vocabulary file to actually cache (counted from the first line).
-    Increase the default value if you are sure these words occur in your training data much more often than 1 or 2 times.
+    Increase the default value if you are sure these words occur in your data much more often than 1 or 2 times.
 - **full**: *boolean, default False*;
 
     if True, will try to load the full model from TensorFlow checkpoints, together with the vocabulary.
     Models loaded this way can be used for language modeling.
 
 ## Working with models
  Currently, we provide three methods for loaded models (will be expanded in the future):
@@ -190,8 +190,8 @@
 
 Meaniwhile, these warnings can be ignored: they do not harm the resulting embeddings in any way.
 
 ### Can I train my own ELMo with this library?
 
 Currently we provide ELMo training code (updated and improved in the same way compared to the original implementation)
 in a [separate repository](https://github.com/ltgoslo/simple_elmo_training).
-It will be integrated into the _simple_elmo_ package in the nearest future.
+It will be integrated into the _simple_elmo_ package at some point.
```

### Comparing `simple_elmo-0.9.1/README.md` & `simple_elmo-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-_Simple_elmo_ is a Python library to work with pre-trained [ELMo embeddings](https://allennlp.org/elmo) in TensorFlow.
+_Simple_elmo_ is a Python library to work with pre-trained [ELMo contextualized language models](https://allennlp.org/elmo) in TensorFlow.
 
 This is a significantly updated wrapper to the [original ELMo implementation](https://github.com/allenai/bilm-tf).
 The main changes are:
 - more convenient and transparent data loading (including from compressed files)
 - code adapted to modern TensorFlow versions (including TensorFlow 2).
 
 # Installation
 
 `pip install --upgrade simple_elmo`
 
-Make sure to update the package regularly, we are actively developing.
+Make sure to update the package regularly.
 
 # Usage
 
  `from simple_elmo import ElmoModel`
 
  `model = ElmoModel()`
 
 ## Loading
- First, let's load a pretrained model from disk:
+ First, let's load a pretrained model:
 
  `model.load(PATH_TO_ELMO)`
 
 ### Required arguments
 
  **PATH_TO_ELMO** is either a ZIP archive downloaded from the [NLPL vector repository](http://vectors.nlpl.eu/repository/),
 OR a directory containing 2 files:
@@ -40,15 +40,15 @@
 
    the maximum number of sentences/documents in a batch during inference;
    your input will be automatically split into chunks of the respective size;
    if your computational resources allow, you might want to increase this value.
 - **limit**: *integer, default 100*;
 
     the number of words from the vocabulary file to actually cache (counted from the first line).
-    Increase the default value if you are sure these words occur in your training data much more often than 1 or 2 times.
+    Increase the default value if you are sure these words occur in your data much more often than 1 or 2 times.
 - **full**: *boolean, default False*;
 
     if True, will try to load the full model from TensorFlow checkpoints, together with the vocabulary.
     Models loaded this way can be used for language modeling.
 
 ## Working with models
  Currently, we provide three methods for loaded models (will be expanded in the future):
@@ -172,8 +172,8 @@
 
 Meaniwhile, these warnings can be ignored: they do not harm the resulting embeddings in any way.
 
 ### Can I train my own ELMo with this library?
 
 Currently we provide ELMo training code (updated and improved in the same way compared to the original implementation)
 in a [separate repository](https://github.com/ltgoslo/simple_elmo_training).
-It will be integrated into the _simple_elmo_ package in the nearest future.
+It will be integrated into the _simple_elmo_ package at some point.
```

### Comparing `simple_elmo-0.9.1/setup.py` & `simple_elmo-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_elmo",
-    version="0.9.1",
+    version="0.9.2",
     author="Andrey Kutuzov",
     author_email="andreku@ifi.uio.no",
     description="Handy library to work with pre-trained ELMo embeddings in TensorFlow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ltgoslo/simple_elmo",
     packages=setuptools.find_packages(),
```

### Comparing `simple_elmo-0.9.1/simple_elmo/data.py` & `simple_elmo-0.9.2/simple_elmo/data.py`

 * *Files identical despite different names*

### Comparing `simple_elmo-0.9.1/simple_elmo/elmo.py` & `simple_elmo-0.9.2/simple_elmo/elmo.py`

 * *Files identical despite different names*

### Comparing `simple_elmo-0.9.1/simple_elmo/elmo_helpers.py` & `simple_elmo-0.9.2/simple_elmo/elmo_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,18 @@
             """
             self.logger.info(message)
             if sys.version_info.major < 3 or sys.version_info.minor < 7:
                 raise SystemExit(
                     "Error: loading models from ZIP archives requires Python >= 3.7."
                 )
             zf = zipfile.ZipFile(directory)
-            vocab_file = zf.read("vocab.txt").decode("utf-8")
+            if "vocab.txt" in zf.namelist():
+                vocab_file = zf.read("vocab.txt").decode("utf-8")
+            else:
+                vocab_file = None
             options_file = zf.read("options.json").decode("utf-8")
             weight_file = zf.open("model.hdf5")
             m_options = json.loads(options_file)
         elif os.path.isdir(directory):
             # We have all the files already extracted in a separate directory
             options_file = os.path.join(directory, "options.json")
             with open(options_file, "r") as of:
```

### Comparing `simple_elmo-0.9.1/simple_elmo/model.py` & `simple_elmo-0.9.2/simple_elmo/model.py`

 * *Files identical despite different names*

### Comparing `simple_elmo-0.9.1/simple_elmo/training.py` & `simple_elmo-0.9.2/simple_elmo/training.py`

 * *Files identical despite different names*

### Comparing `simple_elmo-0.9.1/simple_elmo.egg-info/PKG-INFO` & `simple_elmo-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple-elmo
-Version: 0.9.1
+Name: simple_elmo
+Version: 0.9.2
 Summary: Handy library to work with pre-trained ELMo embeddings in TensorFlow
 Home-page: https://github.com/ltgoslo/simple_elmo
 Author: Andrey Kutuzov
 Author-email: andreku@ifi.uio.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -12,35 +12,35 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: tf
 Provides-Extra: tf_gpu
 License-File: LICENSE
 
-_Simple_elmo_ is a Python library to work with pre-trained [ELMo embeddings](https://allennlp.org/elmo) in TensorFlow.
+_Simple_elmo_ is a Python library to work with pre-trained [ELMo contextualized language models](https://allennlp.org/elmo) in TensorFlow.
 
 This is a significantly updated wrapper to the [original ELMo implementation](https://github.com/allenai/bilm-tf).
 The main changes are:
 - more convenient and transparent data loading (including from compressed files)
 - code adapted to modern TensorFlow versions (including TensorFlow 2).
 
 # Installation
 
 `pip install --upgrade simple_elmo`
 
-Make sure to update the package regularly, we are actively developing.
+Make sure to update the package regularly.
 
 # Usage
 
  `from simple_elmo import ElmoModel`
 
  `model = ElmoModel()`
 
 ## Loading
- First, let's load a pretrained model from disk:
+ First, let's load a pretrained model:
 
  `model.load(PATH_TO_ELMO)`
 
 ### Required arguments
 
  **PATH_TO_ELMO** is either a ZIP archive downloaded from the [NLPL vector repository](http://vectors.nlpl.eu/repository/),
 OR a directory containing 2 files:
@@ -58,15 +58,15 @@
 
    the maximum number of sentences/documents in a batch during inference;
    your input will be automatically split into chunks of the respective size;
    if your computational resources allow, you might want to increase this value.
 - **limit**: *integer, default 100*;
 
     the number of words from the vocabulary file to actually cache (counted from the first line).
-    Increase the default value if you are sure these words occur in your training data much more often than 1 or 2 times.
+    Increase the default value if you are sure these words occur in your data much more often than 1 or 2 times.
 - **full**: *boolean, default False*;
 
     if True, will try to load the full model from TensorFlow checkpoints, together with the vocabulary.
     Models loaded this way can be used for language modeling.
 
 ## Working with models
  Currently, we provide three methods for loaded models (will be expanded in the future):
@@ -190,8 +190,8 @@
 
 Meaniwhile, these warnings can be ignored: they do not harm the resulting embeddings in any way.
 
 ### Can I train my own ELMo with this library?
 
 Currently we provide ELMo training code (updated and improved in the same way compared to the original implementation)
 in a [separate repository](https://github.com/ltgoslo/simple_elmo_training).
-It will be integrated into the _simple_elmo_ package in the nearest future.
+It will be integrated into the _simple_elmo_ package at some point.
```

