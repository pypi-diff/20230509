# Comparing `tmp/optimum-neuron-0.0.3.tar.gz` & `tmp/optimum-neuron-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.3.tar", last modified: Wed Apr 26 08:34:48 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.4.tar", last modified: Mon May  8 22:42:52 2023, max compression
```

## Comparing `optimum-neuron-0.0.3.tar` & `optimum-neuron-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.3/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.3/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     9536 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.609527 optimum-neuron-0.0.3/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.609527 optimum-neuron-0.0.3/optimum/commands/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/commands/export/
--rw-rw-r--   0 michael   (1000) michael   (1000)     4755 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/commands/export/neuron.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4523 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/commands/export/neuronx.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/commands/register/
--rw-rw-r--   0 michael   (1000) michael   (1000)      987 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/commands/register/register_neuron.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.609527 optimum-neuron-0.0.3/optimum/exporters/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/exporters/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4655 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10509 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/config.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12023 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/convert.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4205 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/exporters/neuron/model_configs.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1400 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2307 2023-03-24 13:22:19.000000 optimum-neuron-0.0.3/optimum/neuron/hf_argparser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12697 2023-04-24 14:58:35.000000 optimum-neuron-0.0.3/optimum/neuron/trainer_callback.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)     8516 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/neuron/trainers.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum/neuron/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1021 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4745 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/argument_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17609 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/neuron/utils/cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1149 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/import_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/testing_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9069 2023-04-19 09:39:28.000000 optimum-neuron-0.0.3/optimum/neuron/utils/training_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      825 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/optimum/neuron/utils/version_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/optimum/neuron/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/optimum_neuron.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     1193 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      301 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-04-26 08:34:48.000000 optimum-neuron-0.0.3/optimum_neuron.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2582 2023-04-26 08:34:38.000000 optimum-neuron-0.0.3/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-04-26 08:34:48.613527 optimum-neuron-0.0.3/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    23763 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/tests/test_cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    26361 2023-04-26 08:31:39.000000 optimum-neuron-0.0.3/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9236 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/tests/test_trainer_callback.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    13136 2023-04-14 14:05:35.000000 optimum-neuron-0.0.3/tests/test_trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8036 2023-03-24 13:22:19.000000 optimum-neuron-0.0.3/tests/test_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.4/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.4/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9536 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.865747 optimum-neuron-0.0.4/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.865747 optimum-neuron-0.0.4/optimum/commands/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/commands/export/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4906 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/commands/export/neuron.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4648 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/commands/export/neuronx.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/commands/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1141 2023-04-28 16:14:49.000000 optimum-neuron-0.0.4/optimum/commands/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2971 2023-05-05 15:47:22.000000 optimum-neuron-0.0.4/optimum/commands/neuron/cache.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/commands/register/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.4/optimum/commands/register/register_export.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.4/optimum/commands/register/register_neuron.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.865747 optimum-neuron-0.0.4/optimum/exporters/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/exporters/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5035 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/__main__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10509 2023-04-26 13:29:33.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12081 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/convert.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4205 2023-04-26 13:29:33.000000 optimum-neuron-0.0.4/optimum/exporters/neuron/model_configs.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.869747 optimum-neuron-0.0.4/optimum/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1400 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2307 2023-03-24 13:22:19.000000 optimum-neuron-0.0.4/optimum/neuron/hf_argparser.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12697 2023-04-24 14:58:35.000000 optimum-neuron-0.0.4/optimum/neuron/trainer_callback.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)     8516 2023-05-08 22:41:10.000000 optimum-neuron-0.0.4/optimum/neuron/trainers.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/optimum/neuron/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1021 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5163 2023-05-08 22:41:16.000000 optimum-neuron-0.0.4/optimum/neuron/utils/argument_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    20411 2023-05-05 15:47:22.000000 optimum-neuron-0.0.4/optimum/neuron/utils/cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1149 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/import_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/testing_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9069 2023-04-19 09:39:28.000000 optimum-neuron-0.0.4/optimum/neuron/utils/training_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      825 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/optimum/neuron/utils/version_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-05-08 22:41:25.000000 optimum-neuron-0.0.4/optimum/neuron/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/optimum_neuron.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10765 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1303 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      362 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-05-08 22:42:52.000000 optimum-neuron-0.0.4/optimum_neuron.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-05-08 22:42:52.877747 optimum-neuron-0.0.4/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2776 2023-05-08 22:41:25.000000 optimum-neuron-0.0.4/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-08 22:42:52.873747 optimum-neuron-0.0.4/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    25748 2023-05-05 15:47:22.000000 optimum-neuron-0.0.4/tests/test_cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    27159 2023-05-02 15:09:11.000000 optimum-neuron-0.0.4/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9236 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/tests/test_trainer_callback.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    13136 2023-04-14 14:05:35.000000 optimum-neuron-0.0.4/tests/test_trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8036 2023-03-24 13:22:19.000000 optimum-neuron-0.0.4/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.3/LICENSE` & `optimum-neuron-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/MANIFEST.in` & `optimum-neuron-0.0.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/PKG-INFO` & `optimum-neuron-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.3
+Version: 0.0.4
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.3/README.md` & `optimum-neuron-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/commands/export/neuron.py` & `optimum-neuron-0.0.4/optimum/commands/export/neuron.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,25 +56,29 @@
     optional_group.add_argument(
         "--trust-remote-code",
         action="store_true",
         help="Allow to use custom code for the modeling hosted in the model repository. This option should only be set for repositories you trust and in which you have read the code, as it will execute on your local machine arbitrary code present in the model repository.",
     )
     optional_group.add_argument(
         "--auto_cast",
+        type=str,
         default=None,
-        help='Whether to cast operations from FP32 to lower precision to speed up the inference. Can be `None`, `"matmul"` or `"all"`.',
+        choices=["none", "matmul", "all"],
+        help='Whether to cast operations from FP32 to lower precision to speed up the inference. Can be `"none"`, `"matmul"` or `"all"`.',
     )
     optional_group.add_argument(
         "--auto_cast_type",
-        default=None,
-        help='The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"` or `"tf32"`.',
+        type=str,
+        default="bf16",
+        choices=["bf16", "fp16", "mixed", "tf32"],
+        help='The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"`, `"mixed"` or `"tf32"`.',
     )
     optional_group.add_argument(
-        "--disable_fast_relayout",
-        default=False,
+        "--disable-fast-relayout",
+        action="store_true",
         help="Whether to disable fast relayout optimization which improves performance by using the matrix multiplier for tensor transpose.",
     )
 
     input_group = parser.add_argument_group("Input shapes")
     doc_input = "that the Neuron-cc compiler exported model will be able to take as input."
     input_group.add_argument(
         "--batch_size",
```

### Comparing `optimum-neuron-0.0.3/optimum/commands/export/neuronx.py` & `optimum-neuron-0.0.4/optimum/commands/export/neuronx.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,20 +56,24 @@
     optional_group.add_argument(
         "--trust-remote-code",
         action="store_true",
         help="Allow to use custom code for the modeling hosted in the model repository. This option should only be set for repositories you trust and in which you have read the code, as it will execute on your local machine arbitrary code present in the model repository.",
     )
     optional_group.add_argument(
         "--auto_cast",
+        type=str,
         default=None,
-        help='Whether to cast operations from FP32 to lower precision to speed up the inference. Can be `None`, `"matmul"` or `"all"`.',
+        choices=["none", "matmul", "all"],
+        help='Whether to cast operations from FP32 to lower precision to speed up the inference. Can be `"none"`, `"matmul"` or `"all"`.',
     )
     optional_group.add_argument(
         "--auto_cast_type",
-        default=None,
+        type=str,
+        default="bf16",
+        choices=["bf16", "fp16", "tf32"],
         help='The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"` or `"tf32"`.',
     )
 
     input_group = parser.add_argument_group("Input shapes")
     doc_input = "that the Neuronx-cc compiler exported model will be able to take as input."
     input_group.add_argument(
         "--batch_size",
```

### Comparing `optimum-neuron-0.0.3/optimum/exporters/neuron/__init__.py` & `optimum-neuron-0.0.4/optimum/exporters/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/exporters/neuron/__main__.py` & `optimum-neuron-0.0.4/optimum/exporters/neuron/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -73,30 +73,43 @@
     # TODO: find a cleaner way to do this.
     shapes = {name: getattr(args, name) for name in neuron_config_constructor.func.get_mandatory_axes_for_task(task)}
     neuron_config = neuron_config_constructor(model.config, **shapes)
 
     if args.atol is None:
         args.atol = neuron_config.ATOL_FOR_VALIDATION
 
-    # Saving the model config and preprocessor as this is needed sometimes.
-    model.config.save_pretrained(args.output.parent)
-    maybe_save_preprocessors(args.model, args.output.parent)
-
-    auto_cast = None if args.auto_cast == "None" else args.auto_cast
-    auto_cast_type = None if args.auto_cast_type == "None" else args.auto_cast_type
+    # Get compilation arguments
+    auto_cast = None if args.auto_cast == "none" else args.auto_cast
+    auto_cast_type = args.auto_cast_type
     kwargs = {"auto_cast": auto_cast, "auto_cast_type": auto_cast_type}
     if hasattr(args, "disable_fast_relayout"):
         kwargs["disable_fast_relayout"] = getattr(args, "disable_fast_relayout")
+
     neuron_inputs, neuron_outputs = export(
         model=model,
         config=neuron_config,
         output=args.output,
         **kwargs,
     )
 
+    # Add input shapes during compilation to the config
+    for axe, shape in shapes.items():
+        axe = f"neuron_{axe}"
+        model.config.__setattr__(axe, shape)
+    # Add compilation args to the config
+    if auto_cast is None:
+        kwargs["auto_cast_type"] = None
+    for arg, value in kwargs.items():
+        model.config.__setattr__(arg, value)
+
+    # Saving the model config and preprocessor as this is needed sometimes.
+    model.config.save_pretrained(args.output.parent)
+    maybe_save_preprocessors(args.model, args.output.parent)
+
+    # Validate compiled model
     try:
         validate_model_outputs(
             config=neuron_config,
             reference_model=ref_model,
             neuron_model_path=args.output,
             neuron_named_outputs=neuron_config.outputs,
             atol=args.atol,
```

### Comparing `optimum-neuron-0.0.3/optimum/exporters/neuron/base.py` & `optimum-neuron-0.0.4/optimum/exporters/neuron/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/exporters/neuron/config.py` & `optimum-neuron-0.0.4/optimum/exporters/neuron/config.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/exporters/neuron/convert.py` & `optimum-neuron-0.0.4/optimum/exporters/neuron/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,16 +143,16 @@
 
 
 def export(
     model: "PreTrainedModel",
     config: "NeuronConfig",
     output: Path,
     auto_cast: Optional[str] = None,
-    auto_cast_type: Optional[str] = None,
-    disable_fast_relayout: Optional[bool] = False,
+    auto_cast_type: str = "bf16",
+    disable_fast_relayout: bool = False,
 ) -> Tuple[List[str], List[str]]:
     if is_neuron_available():
         return export_neuron(model, config, output, auto_cast, auto_cast_type, disable_fast_relayout)
     elif is_neuronx_available():
         return export_neuronx(model, config, output, auto_cast, auto_cast_type)
     else:
         raise RuntimeError(
@@ -161,29 +161,29 @@
 
 
 def export_neuronx(
     model: "PreTrainedModel",
     config: "NeuronConfig",
     output: Path,
     auto_cast: Optional[str] = None,
-    auto_cast_type: Optional[str] = None,
+    auto_cast_type: str = "bf16",
 ) -> Tuple[List[str], List[str]]:
     """
     Exports a PyTorch model to a Neuronx compiled TorchScript model.
 
     Args:
         model ([`PreTrainedModel`]):
             The model to export.
         config ([`~exporter.NeuronConfig`]):
             The Neuron configuration associated with the exported model.
         output (`Path`):
             Directory to store the exported Neuron model.
         auto_cast (`Optional[str]`, defaults to `None`):
             Whether to cast operations from FP32 to lower precision to speed up the inference. Can be `None`, `"matmul"` or `"all"`, you should use `None` to disable any auto-casting, use `"matmul"` to cast FP32 matrix multiplication operations, and use `"all"` to cast all FP32 operations.
-        auto_cast_type (`Optional[str]`, defaults to `None`):
+        auto_cast_type (`str`, defaults to `"bf16"`):
             The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"` or `"tf32"`.
 
     Returns:
         `Tuple[List[str], List[str]]`: A tuple with an ordered list of the model's inputs, and the named inputs from
         the Neuron configuration.
     """
     output.parent.mkdir(parents=True, exist_ok=True)
@@ -209,49 +209,48 @@
 
     if auto_cast is not None:
         logger.info(f"Using Neuron: --auto-cast {auto_cast}")
 
         auto_cast = "matmult" if auto_cast == "matmul" else auto_cast
         compiler_args = ["--auto-cast", auto_cast]
 
-        if auto_cast_type is not None:
-            logger.info(f"Using Neuron: --auto-cast-type {auto_cast_type}")
-            compiler_args.extend(["--auto-cast-type", auto_cast_type])
+        logger.info(f"Using Neuron: --auto-cast-type {auto_cast_type}")
+        compiler_args.extend(["--auto-cast-type", auto_cast_type])
     else:
         compiler_args = ["--auto-cast", "none"]
 
     neuron_model = neuronx.trace(checked_model, dummy_inputs_tuple, compiler_args=compiler_args)
     torch.jit.save(neuron_model, output)
 
     return config.inputs, config.outputs
 
 
 def export_neuron(
     model: "PreTrainedModel",
     config: "NeuronConfig",
     output: Path,
     auto_cast: Optional[str] = None,
-    auto_cast_type: Optional[str] = None,
-    disable_fast_relayout: Optional[bool] = False,
+    auto_cast_type: str = "bf16",
+    disable_fast_relayout: bool = False,
 ) -> Tuple[List[str], List[str]]:
     """
     Exports a PyTorch model to a Neuron compiled TorchScript model.
 
     Args:
         model ([`PreTrainedModel`]):
             The model to export.
         config ([`~exporter.NeuronConfig`]):
             The Neuron configuration associated with the exported model.
         output (`Path`):
             Directory to store the exported Neuron model.
         auto_cast (`Optional[str]`, defaults to `None`):
             Whether to cast operations from FP32 to lower precision to speed up the inference. Can be `None`, `"matmul"` or `"all"`, you should use `None` to disable any auto-casting, use `"matmul"` to cast FP32 matrix multiplication operations, and use `"all"` to cast all FP32 operations.
-        auto_cast_type (`Optional[str]`, defaults to `None`):
-            The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"` or `"tf32"`.
-        disable_fast_relayout (`Optional[bool]`, defaults to `False`):
+        auto_cast_type (`str`, defaults to `"bf16"`):
+            The data type to cast FP32 operations to when auto-cast mode is enabled. Can be `"bf16"`, `"fp16"`, ``"mixed" or `"tf32"`. `"mixed"` is only available when auto_cast is "matmul", it will cast operators that use Neuron Matmult engine to bf16 while using fp16 for matmult-based transpose.
+        disable_fast_relayout (`bool`, defaults to `False`):
             Whether to disable fast relayout optimization which improves performance by using the matrix multiplier for tensor transpose.
 
     Returns:
         `Tuple[List[str], List[str]]`: A tuple with an ordered list of the model's inputs, and the named inputs from
         the Neuron configuration.
     """
     output.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `optimum-neuron-0.0.3/optimum/exporters/neuron/model_configs.py` & `optimum-neuron-0.0.4/optimum/exporters/neuron/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/__init__.py` & `optimum-neuron-0.0.4/optimum/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.4/optimum/neuron/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/trainer_callback.py` & `optimum-neuron-0.0.4/optimum/neuron/trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/trainers.py` & `optimum-neuron-0.0.4/optimum/neuron/trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.4/optimum/neuron/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.4/optimum/neuron/utils/argument_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,32 +85,42 @@
                 "Aborting training. To disable automatic failure when an argument value is inferred to be wrong for "
                 "Tranium, set the environment variable OPTIMUM_DISABLE_STRICT_MODE to 1."
             )
             raise ValueError(f"{error_msg}\n{raise_error_msg}")
 
 
 def convert_neuronx_compiler_args_to_neuron(
-    auto_cast: Optional[str] = None,
-    auto_cast_type: Optional[str] = None,
-    disable_fast_relayout: Optional[bool] = False,
+    auto_cast: Optional[str],
+    auto_cast_type: str,
+    disable_fast_relayout: bool,
 ):
     """
     Builds `compiler_args` for neuron compiler.
     """
     compiler_args = []
 
     if auto_cast is None:
         auto_cast = "none"
     elif auto_cast == "matmul":
         auto_cast = "matmult"
 
-    if auto_cast in ["none", "all"]:
+    if auto_cast == "none":
         compiler_args.extend(["--fast-math", auto_cast])
+    elif auto_cast == "all":
+        if auto_cast_type == "mixed":
+            raise ValueError(
+                f"For auto_cast={auto_cast}, cannot set auto_cast_type={auto_cast_type}. "
+                "Please choose among `bf16`, `fp16` and `tf32`."
+            )
+        elif auto_cast_type != "bf16":
+            compiler_args.extend(["--fast-math", f"fp32-cast-all-{auto_cast_type}"])
+        else:
+            compiler_args.extend(["--fast-math", auto_cast])
     elif auto_cast == "matmult":
-        if auto_cast_type is None:
+        if auto_cast_type == "mixed":
             compiler_args.extend(["--fast-math", "fp32-cast-matmult"])
         else:
             compiler_args.extend(["--fast-math", f"fp32-cast-matmult-{auto_cast_type}"])
     else:
         raise ValueError(
             f"The auto_cast value {auto_cast} is not valid. Please use one of the following: None, all or matmul."
         )
```

### Comparing `optimum-neuron-0.0.3/optimum/neuron/utils/cache_utils.py` & `optimum-neuron-0.0.4/optimum/neuron/utils/cache_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,65 +11,126 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 """Utilities for caching."""
 
 import hashlib
 import io
+import json
 import os
 import re
 import shutil
+import subprocess
 import tempfile
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
 import huggingface_hub
 import numpy as np
 import torch
-from huggingface_hub import HfApi, HfFolder
+from huggingface_hub import HfApi, HfFolder, RepoUrl, create_repo
 from huggingface_hub.utils import HfHubHTTPError, RepositoryNotFoundError
 
 from ...utils import logging
 from .version_utils import get_neuronxcc_version
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedModel
 
 
 logger = logging.get_logger()
 
+HOME = Path.home()
+DEFAULT_HF_HOME = f"{HOME}/.cache/huggingface"
+XDG_CACHE_HOME = os.environ.get("XDG_CACHE_HOME", None)
+if XDG_CACHE_HOME is not None:
+    DEFAULT_HF_HOME = f"{XDG_CACHE_HOME}/huggingface"
+HF_HOME = os.environ.get("HF_HOME", DEFAULT_HF_HOME)
 
+CACHE_REPO_FILENAME = "optimum_neuron_custom_cache"
+HF_HOME_CACHE_REPO_FILE = f"{HF_HOME}/{CACHE_REPO_FILENAME}"
+
+CACHE_REPO_NAME = "optimum-neuron-cache"
 if os.environ.get("HUGGINGFACE_CO_STAGING") == "1":
     HF_HUB_CACHE_REPOS = []
 else:
-    HF_HUB_CACHE_REPOS = ["aws-neuron/optimum-neuron-cache"]
+    HF_HUB_CACHE_REPOS = [f"aws-neuron/{CACHE_REPO_NAME}"]
 
 HASH_FILE_NAME = "pytorch_model.bin"
 NEURON_COMPILE_CACHE_NAME = "neuron-compile-cache"
 
 _IP_PATTERN = re.compile(r"ip-([0-9]{1,3}-){4}")
 
 
+def load_custom_cache_repo_name_from_hf_home(
+    hf_home_cache_repo_file: Union[str, Path] = HF_HOME_CACHE_REPO_FILE
+) -> Optional[str]:
+    if Path(hf_home_cache_repo_file).exists():
+        with open(hf_home_cache_repo_file, "r") as fp:
+            return fp.read()
+    return None
+
+
+def set_custom_cache_repo_name_in_hf_home(repo_id: str, hf_home: str = HF_HOME):
+    hf_home_cache_repo_file = f"{hf_home}/{CACHE_REPO_FILENAME}"
+    try:
+        HfApi().repo_info(repo_id, repo_type="model")
+    except Exception as e:
+        raise ValueError(
+            f"Could not save the custom Trainium cache repo to be {repo_id} because it does not exist or is private to "
+            f"you. Complete exception message: {e}."
+        )
+
+    existing_custom_cache_repo = load_custom_cache_repo_name_from_hf_home(hf_home_cache_repo_file)
+    if existing_custom_cache_repo is not None:
+        logger.warning(
+            f"A custom cache repo was already registered: {existing_custom_cache_repo}. It will be overwritten to "
+            f"{repo_id}."
+        )
+
+    with open(hf_home_cache_repo_file, "w") as fp:
+        fp.write(repo_id)
+
+
+def create_custom_cache_repo(repo_id: str = CACHE_REPO_NAME, private: bool = True) -> RepoUrl:
+    repo_url = create_repo(repo_id, private=private, repo_type="model")
+    set_custom_cache_repo_name_in_hf_home(repo_url.repo_id)
+    return repo_url
+
+
 def is_private_repo(repo_id: str) -> bool:
     HfApi().list_repo_files(repo_id=repo_id, token=HfFolder.get_token())
     private = False
     try:
         HfApi().list_repo_files(repo_id=repo_id, token=False)
     except RepositoryNotFoundError:
         private = True
     return private
 
 
 def get_hf_hub_cache_repos():
-    custom_cache_repo = os.environ.get("CUSTOM_CACHE_REPO", None)
     hf_hub_repos = HF_HUB_CACHE_REPOS
-    if custom_cache_repo:
+
+    saved_custom_cache_repo = load_custom_cache_repo_name_from_hf_home()
+    if saved_custom_cache_repo is None:
+        logger.warning(
+            "No Trainium cache name is saved locally. This means that only the official Trainium cache, and "
+            "potentially a cache defined in $CUSTOM_CACHE_REPO will be used. You can create a Trainium cache repo by "
+            "running the following command: `optimum-cli neuron cache create`. If the Trainium cache already exists "
+            "you can set it by running the following command: `optimum-cli neuron cache set -n [name]`."
+        )
+    else:
+        hf_hub_repos = [saved_custom_cache_repo] + hf_hub_repos
+
+    custom_cache_repo = os.environ.get("CUSTOM_CACHE_REPO", None)
+    if custom_cache_repo is not None:
         hf_hub_repos = [custom_cache_repo] + hf_hub_repos
+
     return hf_hub_repos
 
 
 def get_neuron_cache_path() -> Optional[Path]:
     # NEURON_CC_FLAGS is the environment variable read by the neuron compiler.
     # Among other things, this is where the cache directory is specified.
     neuron_cc_flags = os.environ.get("NEURON_CC_FLAGS", "")
@@ -96,24 +157,32 @@
             raise ValueError(
                 "Cannot set the neuron compile cache since --no-cache is in NEURON_CC_FLAGS. You can overwrite this "
                 "behaviour by doing ignore_no_cache=True."
             )
     if isinstance(neuron_cache_path, Path):
         neuron_cache_path = neuron_cache_path.as_posix()
 
-    match_ = re.search(r"--cache_dir=([\w\/]+)", neuron_cc_flags)
+    match_ = re.search(r"--cache_dir=([\w\/-]+)", neuron_cc_flags)
     if match_:
         neuron_cc_flags = neuron_cc_flags[: match_.start(1)] + neuron_cache_path + neuron_cc_flags[match_.end(1) :]
     else:
         neuron_cc_flags = neuron_cc_flags + f" --cache_dir={neuron_cache_path}"
 
     os.environ["NEURON_CC_FLAGS"] = neuron_cc_flags
 
 
-def get_num_neuron_cores_used():
+def get_num_neuron_cores() -> int:
+    proc = subprocess.Popen(["neuron-ls", "-j"], stdout=subprocess.PIPE)
+    stdout, _ = proc.communicate()
+    stdout = stdout.decode("utf-8")
+    json_stdout = json.loads(stdout)
+    return json_stdout[0]["nc_count"]
+
+
+def get_num_neuron_cores_used() -> int:
     return int(os.environ.get("LOCAL_WORLD_SIZE", "1"))
 
 
 def list_files_in_neuron_cache(neuron_cache_path: Path, only_relevant_files: bool = False) -> List[Path]:
     files = [path for path in neuron_cache_path.glob("**/*") if path.is_file()]
     if only_relevant_files:
         files = [p for p in files if p.suffix in [".neff", ".pb", ".txt"]]
```

### Comparing `optimum-neuron-0.0.3/optimum/neuron/utils/import_utils.py` & `optimum-neuron-0.0.4/optimum/neuron/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/utils/testing_utils.py` & `optimum-neuron-0.0.4/optimum/neuron/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/utils/training_utils.py` & `optimum-neuron-0.0.4/optimum/neuron/utils/training_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/utils/version_utils.py` & `optimum-neuron-0.0.4/optimum/neuron/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/optimum/neuron/version.py` & `optimum-neuron-0.0.4/optimum/neuron/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `optimum-neuron-0.0.3/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.4/optimum_neuron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.3
+Version: 0.0.4
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.3/optimum_neuron.egg-info/SOURCES.txt` & `optimum-neuron-0.0.4/optimum_neuron.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 optimum/commands/export/neuron.py
 optimum/commands/export/neuronx.py
+optimum/commands/neuron/base.py
+optimum/commands/neuron/cache.py
+optimum/commands/register/register_export.py
 optimum/commands/register/register_neuron.py
 optimum/exporters/neuron/__init__.py
 optimum/exporters/neuron/__main__.py
 optimum/exporters/neuron/base.py
 optimum/exporters/neuron/config.py
 optimum/exporters/neuron/convert.py
 optimum/exporters/neuron/model_configs.py
```

### Comparing `optimum-neuron-0.0.3/pyproject.toml` & `optimum-neuron-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/setup.py` & `optimum-neuron-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     assert False, "Error: Could not open '%s' due %s\n" % (filepath, error)
 
 
 INSTALL_REQUIRES = [
     "transformers >= 4.28.0",
     "optimum",
     "huggingface_hub >= 0.14.0",
+    "numpy>1.19, <=1.21.6",
+    "protobuf<4",
 ]
 
 TESTS_REQUIRE = [
     "pytest",
     "psutil",
     "parameterized",
     "GitPython",
@@ -35,20 +37,26 @@
 ]
 
 EXTRAS_REQUIRE = {
     "tests": TESTS_REQUIRE,
     "quality": QUALITY_REQUIRES,
     "neuron": [
         "wheel",
-        "torch-neuron==1.12.1.*",
+        "torch-neuron==1.13.1.*",
         "neuron-cc[tensorflow]",
         "protobuf",
         "torchvision",
     ],
-    "neuronx": ["neuronx-cc==2.*", "torch-neuronx", "torchvision"],
+    "neuronx": [
+        "wheel",
+        "neuronx-cc==2.*",
+        "torch-neuronx",
+        "torch==1.13.1.*",
+        "torchvision==0.14.*",
+    ],
 }
 
 setup(
     name="optimum-neuron",
     version=__version__,
     description=(
         "Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS "
@@ -72,11 +80,12 @@
     url="https://huggingface.co/hardware/aws",
     author="HuggingFace Inc. Special Ops Team",
     author_email="hardware@huggingface.co",
     license="Apache",
     packages=find_namespace_packages(include=["optimum*"]),
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRAS_REQUIRE,
+    dependency_links=["https://pip.repos.neuron.amazonaws.com"],
     include_package_data=True,
     zip_safe=False,
     entry_points={"console_scripts": ["optimum-cli=optimum.commands.optimum_cli:main"]},
 )
```

### Comparing `optimum-neuron-0.0.3/tests/test_cache_utils.py` & `optimum-neuron-0.0.4/tests/test_cache_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,55 +9,103 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 """Tests for the cache utilities."""
 
+import logging
 import os
 import random
 from dataclasses import FrozenInstanceError
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import List
 from unittest import TestCase
 
 import torch
-from huggingface_hub import HfApi, create_repo, delete_repo
+from huggingface_hub import HfApi, HfFolder, create_repo, delete_repo
 from transformers import BertConfig, BertModel, set_seed
 from transformers.testing_utils import TOKEN as TRANSFORMERS_TOKEN
 from transformers.testing_utils import USER as TRANSFORMERS_USER
 from transformers.testing_utils import is_staging_test
 
 from optimum.neuron.utils.cache_utils import (
+    CACHE_REPO_FILENAME,
     NEURON_COMPILE_CACHE_NAME,
     NeuronHash,
     download_cached_model_from_hub,
     get_cached_model_on_the_hub,
     get_neuron_cache_path,
     get_num_neuron_cores_used,
     list_files_in_neuron_cache,
+    load_custom_cache_repo_name_from_hf_home,
     path_after_folder,
     push_to_cache_on_hub,
     remove_ip_adress_from_path,
+    set_custom_cache_repo_name_in_hf_home,
     set_neuron_cache_path,
 )
 from optimum.neuron.utils.testing_utils import is_trainium_test
 
 # Use that once optimum==1.7.4 is released.
 # from optimum.utils.testing_utils import USER
-from .utils import MyTinyModel, StagingTestMixin, get_random_string
+from .utils import TOKEN, MyTinyModel, StagingTestMixin, get_random_string
 
 
 USER = "__DUMMY_OPTIMUM_USER__"
 
 DUMMY_COMPILER_VERSION = "1.2.3"
 
 
 class NeuronUtilsTestCase(TestCase):
+    def test_load_custom_cache_repo_name_from_hf_home(self):
+        with TemporaryDirectory() as tmpdirname:
+            hf_home_cache_repo_file = f"{tmpdirname}/{CACHE_REPO_FILENAME}"
+            with open(hf_home_cache_repo_file, "w") as fp:
+                fp.write("blablabla")
+            self.assertEqual(load_custom_cache_repo_name_from_hf_home(hf_home_cache_repo_file), "blablabla")
+
+            bad_hf_home_cache_repo_file = f"{tmpdirname}/does_not_exist"
+            self.assertIsNone(load_custom_cache_repo_name_from_hf_home(bad_hf_home_cache_repo_file))
+
+    @is_staging_test
+    def test_set_custom_cache_repo_name_in_hf_home(self):
+        orig_token = HfFolder.get_token()
+        HfFolder.save_token(TOKEN)
+
+        repo_name = "blablabla"
+        repo_id = f"{USER}/{repo_name}"
+        create_repo(repo_name, repo_type="model")
+
+        def remove_repo():
+            delete_repo(repo_name, repo_type="model")
+
+        with TemporaryDirectory() as tmpdirname:
+            try:
+                set_custom_cache_repo_name_in_hf_home(repo_id, hf_home=tmpdirname)
+            except ValueError as e:
+                remove_repo()
+                if orig_token:
+                    HfFolder.save_token(orig_token)
+                self.fail(str(e))
+
+            with open(f"{tmpdirname}/{CACHE_REPO_FILENAME}", "r") as fp:
+                content = fp.read()
+
+            self.assertEqual(content, repo_id, "The stored repo id must match the one specified.")
+
+            with self.assertLogs("optimum", level=logging.WARNING) as cm:
+                set_custom_cache_repo_name_in_hf_home(repo_id, hf_home=tmpdirname)
+                self.assertIn("A custom cache repo was already", cm.output[0])
+
+            remove_repo()
+            if orig_token:
+                HfFolder.save_token(orig_token)
+
     def test_get_neuron_cache_path(self):
         os.environ["NEURON_CC_FLAGS"] = "--some --parameters --here --no-cache --other --paremeters --here"
         assert get_neuron_cache_path() is None
 
         custom_cache_dir_name = Path("_this/is_/my1/2custom/cache/dir")
         os.environ[
             "NEURON_CC_FLAGS"
@@ -417,15 +465,15 @@
             repo_name = "optimum-neuron-cache"
             create_repo(repo_name, repo_type="model", exist_ok=True)
             self.set_hf_hub_token(orig_token)
 
             os.environ["CUSTOM_CACHE_REPO"] = f"{TRANSFORMERS_USER}/{repo_name}"
             with self.assertLogs("optimum", "WARNING") as cm:
                 push_to_cache_on_hub(neuron_hash, get_neuron_cache_path())
-                self.assertIn("Could not push the cached model to the repo", cm.output[0])
+                self.assertTrue(any("Could not push the cached model to the repo" in output for output in cm.output))
 
             self.set_hf_hub_token(TRANSFORMERS_TOKEN)
             delete_repo(repo_name, repo_type="model")
             self.set_hf_hub_token(orig_token)
 
     def test_download_cached_model_from_hub(self):
         os.environ["CUSTOM_CACHE_REPO"] = self.CUSTOM_PRIVATE_CACHE_REPO
```

### Comparing `optimum-neuron-0.0.3/tests/test_examples.py` & `optimum-neuron-0.0.4/tests/test_examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 # limitations under the License.
 """Tests every (architecture, task) supported pair on 🤗 Transformers training example scripts."""
 
 import json
 import os
 import re
 import subprocess
+import sys
 from datetime import date
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import Any, Callable, Dict, List, Optional, Set, Union
 from unittest import TestCase
 
+from huggingface_hub import HfFolder
 from transformers import (
     CONFIG_MAPPING,
     MODEL_FOR_AUDIO_CLASSIFICATION_MAPPING,
     MODEL_FOR_CAUSAL_LM_MAPPING,
     MODEL_FOR_CTC_MAPPING,
     MODEL_FOR_IMAGE_CLASSIFICATION_MAPPING,
     MODEL_FOR_MASKED_LM_MAPPING,
@@ -35,15 +37,28 @@
     MODEL_FOR_QUESTION_ANSWERING_MAPPING,
     MODEL_FOR_SEQ_TO_SEQ_CAUSAL_LM_MAPPING,
     MODEL_FOR_SEQUENCE_CLASSIFICATION_MAPPING,
     MODEL_FOR_TOKEN_CLASSIFICATION_MAPPING,
 )
 from transformers.testing_utils import slow
 
-from .utils import MODELS_TO_TEST_MAPPING
+from optimum.neuron.utils.cache_utils import set_neuron_cache_path
+from optimum.neuron.utils.testing_utils import is_trainium_test
+
+
+# Doing it this way to be able to use this file in tools.
+path_tests = Path(__file__).parent
+sys.path.insert(0, str(path_tests))
+from utils import MODELS_TO_TEST_MAPPING  # noqa: E402
+
+
+TOKEN = HfFolder.get_token()
+if os.environ.get("HF_TOKEN_OPTIMUM_NEURON_CI", None) is not None:
+    print("TESSSST", os.environ.get("HF_TOKEN_OPTIMUM_NEURON_CI"))
+    TOKEN = os.environ.get("HF_TOKEN_OPTIMUM_NEURON_CI")
 
 
 def _get_supported_models_for_script(
     models_to_test: Dict[str, str], task_mapping: Dict[str, str], to_exclude: Optional[Set[str]] = None
 ) -> List[str]:
     """
     Filters models that can perform the task from models_to_test.
@@ -128,14 +143,15 @@
             model_name (`str`): the model_name_or_path.
 
         Returns:
             `Callable[[ExampleTesterBase], None]`: The test function that runs the example.
         """
 
         @slow
+        @is_trainium_test
         def test(self):
             if self.EXAMPLE_NAME is None:
                 raise ValueError("An example name must be provided")
             example_script = Path(self.EXAMPLE_DIR).glob(f"*/{self.EXAMPLE_NAME}.py")
             example_script = list(example_script)
             if len(example_script) == 0:
                 raise RuntimeError(f"Could not find {self.EXAMPLE_NAME}.py in examples located in {self.EXAMPLE_DIR}")
@@ -143,82 +159,59 @@
                 raise RuntimeError(f"Found more than {self.EXAMPLE_NAME}.py in examples located in {self.EXAMPLE_DIR}")
             else:
                 example_script = example_script[0]
 
             self._install_requirements(example_script.parent / "requirements.txt")
 
             do_precompilation = ExampleTestMeta.process_class_attribute(self.DO_PRECOMPILATION, model_type)
-            train_batch_size = ExampleTestMeta.process_class_attribute(self.TRAIN_BATCH_SIZE, model_type)
-            eval_batch_size = ExampleTestMeta.process_class_attribute(self.EVAL_BATCH_SIZE, model_type)
-            gradient_accumulation_steps = ExampleTestMeta.process_class_attribute(
-                self.GRADIENT_ACCUMULATION_STEPS, model_type
-            )
-            extra_command_line_arguments = [
-                ExampleTestMeta.process_class_attribute(arg, model_type) for arg in self.EXTRA_COMMAND_LINE_ARGUMENTS
-            ]
-            learning_rate = ExampleTestMeta.process_class_attribute(self.LEARNING_RATE, model_type)
+            only_precompilation = ExampleTestMeta.process_class_attribute(self.ONLY_PRECOMPILATION, model_type)
+
+            eval_is_supported = ExampleTestMeta.process_class_attribute(self.EVAL_IS_SUPPORTED, model_type)
+            eval_score_threshold = ExampleTestMeta.process_class_attribute(self.EVAL_SCORE_THRESHOLD, model_type)
 
+            env = self.get_env(model_type)
             if do_precompilation:
                 with TemporaryDirectory(dir=Path(self.EXAMPLE_DIR)) as tmp_dir:
-                    os.environ["HF_HOME"] = os.path.join(tmp_dir, "hf_home")
                     cmd_line = self._create_command_line(
                         example_script,
                         model_name,
+                        model_type,
                         tmp_dir,
                         is_precompilation=True,
-                        task=self.TASK_NAME,
-                        dataset_config_name=self.DATASET_CONFIG_NAME,
-                        do_eval=False,
-                        lr=learning_rate,
-                        train_batch_size=train_batch_size,
-                        eval_batch_size=eval_batch_size,
-                        num_epochs=1,
-                        gradient_accumulation_steps=gradient_accumulation_steps,
-                        extra_command_line_arguments=extra_command_line_arguments,
                     )
                     joined_cmd_line = " ".join(cmd_line)
                     print(f"#### Running precompilation... ####\n{joined_cmd_line}\n")
-                    p = subprocess.Popen(joined_cmd_line, shell=True)
+                    p = subprocess.Popen(joined_cmd_line, shell=True, env=env)
+                    return_code = p.wait()
+                    self.assertEqual(return_code, 0)
+
+            if not only_precompilation:
+                with TemporaryDirectory(dir=Path(self.EXAMPLE_DIR)) as tmp_dir:
+                    cmd_line = self._create_command_line(
+                        example_script,
+                        model_name,
+                        model_type,
+                        tmp_dir,
+                    )
+                    joined_cmd_line = " ".join(cmd_line)
+                    print(f"#### Running command line... ####\n{joined_cmd_line}\n")
+                    os.environ["WANDB_NAME"] = f"{self.EXAMPLE_NAME}_{model_type}"
+                    p = subprocess.Popen(joined_cmd_line, shell=True, env=env)
                     return_code = p.wait()
                     self.assertEqual(return_code, 0)
 
-            with TemporaryDirectory(dir=Path(self.EXAMPLE_DIR)) as tmp_dir:
-                os.environ["HF_HOME"] = os.path.join(tmp_dir, "hf_home")
-                cmd_line = self._create_command_line(
-                    example_script,
-                    model_name,
-                    tmp_dir,
-                    task=self.TASK_NAME,
-                    dataset_config_name=self.DATASET_CONFIG_NAME,
-                    do_eval=self.EVAL_IS_SUPPORTED,
-                    lr=learning_rate,
-                    train_batch_size=train_batch_size,
-                    eval_batch_size=eval_batch_size,
-                    num_epochs=self.NUM_EPOCHS,
-                    gradient_accumulation_steps=gradient_accumulation_steps,
-                    extra_command_line_arguments=extra_command_line_arguments,
-                )
-                joined_cmd_line = " ".join(cmd_line)
-                print(f"#### Running command line... ####\n{joined_cmd_line}\n")
-                os.environ["WANDB_NAME"] = f"{self.EXAMPLE_NAME}_{model_type}"
-                p = subprocess.Popen(joined_cmd_line, shell=True)
-                return_code = p.wait()
-                self.assertEqual(return_code, 0)
-
-                if self.EVAL_IS_SUPPORTED:
-                    with open(Path(tmp_dir) / "all_results.json") as fp:
-                        results = json.load(fp)
-                    threshold_overrides = {}
-                    if isinstance(self.EVAL_SCORE_THRESHOLD_OVERRIDES, dict):
-                        threshold_overrides = self.EVAL_SCORE_THRESHOLD_OVERRIDES
-                    threshold = threshold_overrides.get(model_name, self.EVAL_SCORE_THRESHOLD)
-                    if self.EVAL_SCORE_GREATER_IS_BETTER:
-                        self.assertGreaterEqual(float(results[self.SCORE_NAME]), threshold)
-                    else:
-                        self.assertLessEqual(float(results[self.SCORE_NAME]), threshold)
+                    if eval_is_supported:
+                        with open(Path(tmp_dir) / "all_results.json") as fp:
+                            results = json.load(fp)
+                        threshold_overrides = {}
+                        threshold = threshold_overrides.get(model_name, eval_score_threshold)
+                        if self.EVAL_SCORE_GREATER_IS_BETTER:
+                            self.assertGreaterEqual(float(results[self.SCORE_NAME]), threshold)
+                        else:
+                            self.assertLessEqual(float(results[self.SCORE_NAME]), threshold)
 
         return test
 
 
 class ExampleTesterBase(TestCase):
     """
     Base example tester class.
@@ -226,162 +219,214 @@
     Attributes:
         EXAMPLE_DIR (`Union[str, Path]`) -- The directory containing the examples.
         EXAMPLE_NAME (`Optional[str]`) -- The name of the example script without the file extension, e.g. run_qa, run_glue, etc.
         TASK_NAME (`str`) -- The name of the dataset to use.
         EVAL_IS_SUPPORTED (`bool`) -- Whether evaluation is currently supported on AWS Tranium.
             If True, the example will run evaluation, otherwise it will be skipped.
         EVAL_SCORE_THRESHOLD (`float`) -- The score threshold from which training is assumed to have worked.
-        EVAL_SCORE_THRESHOLD_OVERRIDES (`Dict[str, float]`) -- Per-model score threshold overrides.
         SCORE_NAME (`str`) -- The name of the metric to use for checking that the example ran successfully.
         DATASET_PARAMETER_NAME (`str`) -- The argument name to use for the dataset parameter.
             Most of the time it will be "dataset_name", but for some tasks on a benchmark it might be something else.
         TRAIN_BATCH_SIZE (`int`) -- The batch size to give to the example script for training.
         EVAL_BATCH_SIZE (`int`) -- The batch size to give to the example script for evaluation.
         GRADIENT_ACCUMULATION_STEPS (`int`) -- The number of gradient accumulation to use during training.
         DATALOADER_DROP_LAST (`bool`) -- Whether to drop the last batch if it is a remainder batch.
         NPROC_PER_NODE (`int`) -- The number of Neuron cores to use when doing multiple workers training.
-        EXTRA_COMMAND_LINE_ARGUMENTS (`str`) -- Extra arguments, if needed, to be passed to the command line traning
+        EXTRA_COMMAND_LINE_ARGUMENTS (`Optional[List[str]]`) -- Extra arguments, if needed, to be passed to the command line traning
             script.
     """
 
     EXAMPLE_DIR = Path(__file__).parent.parent / "examples"
     EXAMPLE_NAME = ""
     TASK_NAME = None
     DATASET_CONFIG_NAME = ""
     EVAL_IS_SUPPORTED = True
     # Camembert is pretrained on French.
     EVAL_SCORE_THRESHOLD = {"default": 0.75, "camembert": 0.5}
-    EVAL_SCORE_THRESHOLD_OVERRIDES = None
     EVAL_SCORE_GREATER_IS_BETTER = True
     SCORE_NAME = "eval_accuracy"
     DATASET_PARAMETER_NAME = "dataset_name"
     NUM_EPOCHS = 1
     MAX_STEPS = None
     LEARNING_RATE = 1e-4
     TRAIN_BATCH_SIZE = 16
     EVAL_BATCH_SIZE = 16
     GRADIENT_ACCUMULATION_STEPS = 16
     NPROC_PER_NODE = 2
-    EXTRA_COMMAND_LINE_ARGUMENTS = ""
+    EXTRA_COMMAND_LINE_ARGUMENTS = None
+    LOGGING_STEPS = 1
+    SAVE_STEPS = -1
+    ONLY_PRECOMPILATION = False
     DO_PRECOMPILATION = True
+    NEURON_CACHE = None
+    MULTI_PROC = os.environ.get("MULTI_PROC", "false")
+    BF16 = True
+
+    @classmethod
+    def setUpClass(cls):
+        cls._create_venv()
+        HfFolder.save_token(TOKEN)
+
+    @classmethod
+    def tearDownClass(cls):
+        cls._remove_venv()
 
     def setUp(self):
-        self._create_venv()
+        set_neuron_cache_path("/var/tmp/neuron-compile-cache")
 
     def tearDown(self):
-        self._remove_venv()
+        set_neuron_cache_path("/var/tmp/neuron-compile-cache")
+
+        cmd_line = "sudo rmmod neuron".split()
+        p = subprocess.Popen(cmd_line)
+        return_code = p.wait()
+        assert return_code == 0
+
+        cmd_line = "sudo modprobe neuron".split()
+        p = subprocess.Popen(cmd_line)
+        return_code = p.wait()
+        assert return_code == 0
+
+    def get_env(self, model_type: str) -> Dict[str, str]:
+        env = dict(os.environ)
+        return env
 
     def _create_command_line(
         self,
         script: str,
         model_name: str,
+        model_type: str,
         output_dir: str,
         is_precompilation: bool = False,
-        task: Optional[str] = None,
-        dataset_config_name: Optional[str] = None,
-        do_eval: bool = True,
-        lr: float = 1e-4,
-        train_batch_size: int = 4,
-        eval_batch_size: int = 4,
-        num_epochs: int = 1,
-        gradient_accumulation_steps: int = 64,
-        extra_command_line_arguments: Optional[List[str]] = None,
     ) -> List[str]:
+        # Task related.
+        task = ExampleTestMeta.process_class_attribute(self.TASK_NAME, model_type)
+        dataset_parameter_name = ExampleTestMeta.process_class_attribute(self.DATASET_PARAMETER_NAME, model_type)
+        dataset_config_name = ExampleTestMeta.process_class_attribute(self.DATASET_CONFIG_NAME, model_type)
+
+        # Batch size related.
+        train_batch_size = ExampleTestMeta.process_class_attribute(self.TRAIN_BATCH_SIZE, model_type)
+        eval_batch_size = ExampleTestMeta.process_class_attribute(self.EVAL_BATCH_SIZE, model_type)
+        gradient_accumulation_steps = ExampleTestMeta.process_class_attribute(
+            self.GRADIENT_ACCUMULATION_STEPS, model_type
+        )
+
+        # Training related.
+        learning_rate = ExampleTestMeta.process_class_attribute(self.LEARNING_RATE, model_type)
+        eval_is_supported = ExampleTestMeta.process_class_attribute(self.EVAL_IS_SUPPORTED, model_type)
+        n_proc_per_node = ExampleTestMeta.process_class_attribute(self.NPROC_PER_NODE, model_type)
+        num_train_epochs = ExampleTestMeta.process_class_attribute(self.NUM_EPOCHS, model_type)
+        max_steps = ExampleTestMeta.process_class_attribute(self.MAX_STEPS, model_type)
+        logging_steps = ExampleTestMeta.process_class_attribute(self.LOGGING_STEPS, model_type)
+        save_steps = ExampleTestMeta.process_class_attribute(self.SAVE_STEPS, model_type)
+
+        bf16 = ExampleTestMeta.process_class_attribute(self.BF16, model_type)
+        multi_proc = ExampleTestMeta.process_class_attribute(self.MULTI_PROC, model_type)
+
+        # Extra
+        extra_command_line_arguments = [
+            ExampleTestMeta.process_class_attribute(arg, model_type) for arg in self.EXTRA_COMMAND_LINE_ARGUMENTS
+        ]
+
+        do_eval = eval_is_supported and not is_precompilation
+
         do_eval_option = "--do_eval" if do_eval else " "
-        task_option = f"--{self.DATASET_PARAMETER_NAME} {task}" if task else " "
+        task_option = f"--{dataset_parameter_name} {task}" if task else " "
 
-        if os.environ.get("MULTI_PROC", "false") == "false":
-            program = ["venv/bin/python" if self.venv_was_created else "python"]
+        if multi_proc == "false":
+            program = ["venv/bin/python" if self.venv_was_created() else "python"]
         else:
             program = [
-                "venv/bin/torchrun" if self.venv_was_created else "torchrun",
-                f"--nproc_per_node={self.NPROC_PER_NODE}",
+                "venv/bin/torchrun" if self.venv_was_created() else "torchrun",
+                f"--nproc_per_node={n_proc_per_node}",
             ]
 
         if is_precompilation:
             neuron_parallel_compile_path = (
-                "venv/bin/neuron_parallel_compile" if self.venv_was_created else "neuron_parallel_compile"
+                "venv/bin/neuron_parallel_compile" if self.venv_was_created() else "neuron_parallel_compile"
             )
             program = [neuron_parallel_compile_path] + program
 
-        # TODO: make that a parameter to the function?
-        if self.MAX_STEPS is not None:
-            max_steps = f"--max_steps {self.MAX_STEPS}"
+        if max_steps is not None:
+            max_steps = f"--max_steps {max_steps}"
         else:
             max_steps = ""
 
         cmd_line = program + [
             f"{script}",
             f"--model_name_or_path {model_name}",
             f"{task_option}",
             "--do_train",
             f"{do_eval_option}",
             f"--output_dir {output_dir}",
             "--overwrite_output_dir true",
-            f"--learning_rate {lr}",
+            f"--learning_rate {learning_rate}",
             f"--per_device_train_batch_size {train_batch_size}",
             f"--per_device_eval_batch_size {eval_batch_size}",
             f"--gradient_accumulation_steps {gradient_accumulation_steps}",
-            "--save_strategy epoch",
-            f" --num_train_epochs {num_epochs}",
+            "--save_strategy steps",
+            f" --num_train_epochs {num_train_epochs}",
             max_steps,
             "--dataloader_num_workers 4",
-            "--save_steps -1",
+            f"--save_steps {save_steps}",
             "--save_total_limit 1",
-            "--logging_steps 1",
-            "--bf16",
+            f"--logging_steps {logging_steps}",
         ]
+        if bf16:
+            cmd_line.append("--bf16")
         if is_precompilation:
             cmd_line.append("--report_to none")
 
         if dataset_config_name:
             cmd_line.append(f"--dataset_config_name {dataset_config_name}")
 
         if extra_command_line_arguments is not None:
             cmd_line += extra_command_line_arguments
 
         pattern = re.compile(r"([\"\'].+?[\"\'])|\s")
         return [x for y in cmd_line for x in re.split(pattern, y) if x]
 
-    @property
-    def venv_was_created(self):
+    @classmethod
+    def venv_was_created(cls):
         return os.environ.get("USE_VENV", "true") == "true" and os.path.isdir("venv")
 
-    def _create_venv(self):
+    @classmethod
+    def _create_venv(cls):
         """
         Creates the virtual environment for the example.
         """
         if os.environ.get("USE_VENV", "true") == "true":
             cmd_line = "python -m venv venv".split()
             p = subprocess.Popen(cmd_line)
             return_code = p.wait()
-            self.assertEqual(return_code, 0)
+            assert return_code == 0
 
             # Install pip
             cmd_line = "venv/bin/python -m ensurepip --upgrade".split()
             p = subprocess.Popen(cmd_line)
             return_code = p.wait()
-            self.assertEqual(return_code, 0)
+            assert return_code == 0
 
-    def _remove_venv(self):
+    @classmethod
+    def _remove_venv(cls):
         """
         Removes the virtual environment for the example.
         """
-        if self.venv_was_created:
+        if cls.venv_was_created():
             cmd_line = "rm -rf venv".split()
             p = subprocess.Popen(cmd_line)
             return_code = p.wait()
-            self.assertEqual(return_code, 0)
+            assert return_code == 0
 
     def _install_requirements(self, requirements_filename: Union[str, os.PathLike]):
         """
         Installs the necessary requirements to run the example if the provided file exists, otherwise does nothing.
         """
 
-        pip_name = "venv/bin/pip" if self.venv_was_created else "pip"
+        pip_name = "venv/bin/pip" if self.venv_was_created() else "pip"
 
         # Update pip
         cmd_line = f"{pip_name} install --upgrade pip".split()
         p = subprocess.Popen(cmd_line)
         return_code = p.wait()
         self.assertEqual(return_code, 0)
 
@@ -425,15 +470,15 @@
             cmd_line = f"{pip_name} install wandb".split()
             p = subprocess.Popen(cmd_line)
             return_code = p.wait()
             self.assertEqual(return_code, 0)
 
             env_with_updated_path = dict(os.environ, PATH=f"/home/ubuntu/.local/bin:{os.environ['PATH']}")
 
-            wandb_name = "venv/bin/wandb" if self.venv_was_created else "wandb"
+            wandb_name = "venv/bin/wandb" if self.venv_was_created() else "wandb"
             cmd_line = f"{wandb_name} login --relogin {wandb_token}".split()
             p = subprocess.Popen(cmd_line, env=env_with_updated_path)
             self.assertEqual(return_code, 0)
 
             wandb_project_name = os.environ.get("WANDB_PROJECT", "aws-neuron-tests")
             today = date.today().strftime("%d%m%Y")
             wandb_project_name = f"{wandb_project_name}-{today}"
@@ -464,15 +509,15 @@
     EVAL_BATCH_SIZE = {"default": 4, "distilbert": 6}
     EXTRA_COMMAND_LINE_ARGUMENTS = [
         "--max_seq_length 384",
     ]
 
 
 class MultipleChoiceExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_swag"):
-    EVAL_SCORE_THRESHOLD_OVERRIDES = {"distilbert-base-uncased": 0.645}
+    EVAL_SCORE_THRESHOLD = {"default": 0.75, "camembert": 0.5, "distilbert": 0.645}
     TRAIN_BATCH_SIZE = {"default": 2, "distilbert": 3}
     EVAL_BATCH_SIZE = {"default": 2, "distilbert": 3}
     NUM_EPOCHS = 3
     EXTRA_COMMAND_LINE_ARGUMENTS = [
         "--max_seq_length 512",
     ]
 
@@ -492,50 +537,36 @@
     EVAL_SCORE_THRESHOLD = 30
     SCORE_NAME = "eval_rougeLsum"
     EXTRA_COMMAND_LINE_ARGUMENTS = [
         "--prediction_loss_only",
         "--pad_to_max_length",
         "--max_target_length 200",
         {"default": "--max_source_length 1024", "t5": "--max_source_length 768"},
+        {"default": "", "t5": "--source_prefix 'summarize: '"},
     ]
 
     def _create_command_line(
         self,
         script: str,
         model_name: str,
+        model_type: str,
         output_dir: str,
         is_precompilation: bool = False,
-        task: Optional[str] = None,
-        dataset_config_name: Optional[str] = None,
-        do_eval: bool = True,
-        lr: float = 1e-4,
-        train_batch_size: int = 1,
-        eval_batch_size: int = 1,
-        num_epochs: int = 2,
-        gradient_accumulation_steps: int = 64,
-        extra_command_line_arguments: Optional[List[str]] = None,
     ) -> List[str]:
+        extra_command_line_arguments = [
+            ExampleTestMeta.process_class_attribute(arg, model_type) for arg in self.EXTRA_COMMAND_LINE_ARGUMENTS
+        ]
         if extra_command_line_arguments is None:
             extra_command_line_arguments = []
-        if "t5" in model_name:
-            extra_command_line_arguments.append("--source_prefix 'summarize: '")
         return super()._create_command_line(
             script,
             model_name,
+            model_type,
             output_dir,
             is_precompilation=is_precompilation,
-            task=task,
-            dataset_config_name=dataset_config_name,
-            do_eval=do_eval,
-            lr=lr,
-            train_batch_size=train_batch_size,
-            eval_batch_size=eval_batch_size,
-            num_epochs=num_epochs,
-            gradient_accumulation_steps=gradient_accumulation_steps,
-            extra_command_line_arguments=extra_command_line_arguments,
         )
 
 
 class TranslationExampleTester(ExampleTesterBase, metaclass=ExampleTestMeta, example_name="run_translation"):
     TASK_NAME = "wmt16"
     DATASET_CONFIG_NAME = "ro-en"
     TRAIN_BATCH_SIZE = 1
```

### Comparing `optimum-neuron-0.0.3/tests/test_trainer_callback.py` & `optimum-neuron-0.0.4/tests/test_trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/tests/test_trainers.py` & `optimum-neuron-0.0.4/tests/test_trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.3/tests/test_utils.py` & `optimum-neuron-0.0.4/tests/test_utils.py`

 * *Files identical despite different names*

