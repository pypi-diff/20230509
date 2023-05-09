# Comparing `tmp/onnx2kerastl-0.0.85.5.tar.gz` & `tmp/onnx2kerastl-0.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.85.5.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.86.tar", max compression
```

## Comparing `onnx2kerastl-0.0.85.5.tar` & `onnx2kerastl-0.0.86.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/LICENSE
--rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.85.5/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13572 2023-05-08 05:49:57.483750 onnx2kerastl-0.0.85.5/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.85.5/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-24 14:18:00.054331 onnx2kerastl-0.0.85.5/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.85.5/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.85.5/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.85.5/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17867 2023-05-08 05:48:07.753079 onnx2kerastl-0.0.85.5/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5354 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.85.5/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.85.5/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1032 2023-05-08 05:54:36.302817 onnx2kerastl-0.0.85.5/pyproject.toml
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.85.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/LICENSE
+-rw-r--r--   0        0        0       66 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-03 08:32:59.779031 onnx2kerastl-0.0.86/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13572 2023-05-08 05:49:57.483750 onnx2kerastl-0.0.86/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.86/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-09-29 08:59:30.260148 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-24 14:18:00.054331 onnx2kerastl-0.0.86/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-08 05:48:07.745079 onnx2kerastl-0.0.86/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-09-12 14:46:25.445008 onnx2kerastl-0.0.86/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-08 05:48:07.717080 onnx2kerastl-0.0.86/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17867 2023-05-08 05:48:07.753079 onnx2kerastl-0.0.86/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5354 2023-04-24 14:18:00.058331 onnx2kerastl-0.0.86/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-03-02 09:58:33.149358 onnx2kerastl-0.0.86/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-05-09 06:01:41.299601 onnx2kerastl-0.0.86/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.86/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.85.5/LICENSE` & `onnx2kerastl-0.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.86/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.86/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.86/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.86/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.85.5/pyproject.toml` & `onnx2kerastl-0.0.86/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.85.5"
+version = "0.0.86"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.85.5/PKG-INFO` & `onnx2kerastl-0.0.86/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.85.5
+Version: 0.0.86
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

