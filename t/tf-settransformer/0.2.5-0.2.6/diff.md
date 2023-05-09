# Comparing `tmp/tf-settransformer-0.2.5.tar.gz` & `tmp/tf-settransformer-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf-settransformer-0.2.5.tar", last modified: Thu Mar 16 07:29:14 2023, max compression
+gzip compressed data, was "tf-settransformer-0.2.6.tar", last modified: Tue May  9 21:33:39 2023, max compression
```

## Comparing `tf-settransformer-0.2.5.tar` & `tf-settransformer-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-03-16 07:29:14.008512 tf-settransformer-0.2.5/
--rw-rw-r--   0 dwl2x     (1000) users      (100)     1064 2021-10-11 19:00:04.000000 tf-settransformer-0.2.5/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     2430 2023-03-16 07:29:14.008512 tf-settransformer-0.2.5/PKG-INFO
--rw-rw-r--   0 dwl2x     (1000) users      (100)      494 2022-08-19 01:19:07.000000 tf-settransformer-0.2.5/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      805 2023-03-16 07:29:06.000000 tf-settransformer-0.2.5/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-03-16 07:29:14.008512 tf-settransformer-0.2.5/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-03-16 07:29:14.008512 tf-settransformer-0.2.5/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-03-16 07:29:14.008512 tf-settransformer-0.2.5/src/settransformer/
--rw-r--r--   0 dwl2x     (1000) users      (100)    15922 2023-03-16 07:28:16.000000 tf-settransformer-0.2.5/src/settransformer/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-03-16 07:29:14.008512 tf-settransformer-0.2.5/src/tf_settransformer.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     2430 2023-03-16 07:29:14.000000 tf-settransformer-0.2.5/src/tf_settransformer.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      243 2023-03-16 07:29:14.000000 tf-settransformer-0.2.5/src/tf_settransformer.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-03-16 07:29:14.000000 tf-settransformer-0.2.5/src/tf_settransformer.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       15 2023-03-16 07:29:14.000000 tf-settransformer-0.2.5/src/tf_settransformer.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-09 21:33:39.449629 tf-settransformer-0.2.6/
+-rw-rw-r--   0 dwl2x     (1000) users      (100)     1064 2021-10-11 19:00:04.000000 tf-settransformer-0.2.6/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2430 2023-05-09 21:33:39.449629 tf-settransformer-0.2.6/PKG-INFO
+-rw-rw-r--   0 dwl2x     (1000) users      (100)      494 2022-08-19 01:19:07.000000 tf-settransformer-0.2.6/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      805 2023-05-09 21:32:07.000000 tf-settransformer-0.2.6/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-09 21:33:39.449629 tf-settransformer-0.2.6/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-09 21:33:39.449629 tf-settransformer-0.2.6/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-09 21:33:39.449629 tf-settransformer-0.2.6/src/settransformer/
+-rw-r--r--   0 dwl2x     (1000) users      (100)    16732 2023-05-09 21:32:23.000000 tf-settransformer-0.2.6/src/settransformer/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-09 21:33:39.449629 tf-settransformer-0.2.6/src/tf_settransformer.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2430 2023-05-09 21:33:39.000000 tf-settransformer-0.2.6/src/tf_settransformer.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      243 2023-05-09 21:33:39.000000 tf-settransformer-0.2.6/src/tf_settransformer.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-09 21:33:39.000000 tf-settransformer-0.2.6/src/tf_settransformer.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       15 2023-05-09 21:33:39.000000 tf-settransformer-0.2.6/src/tf_settransformer.egg-info/top_level.txt
```

### Comparing `tf-settransformer-0.2.5/LICENSE` & `tf-settransformer-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tf-settransformer-0.2.5/PKG-INFO` & `tf-settransformer-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-settransformer
-Version: 0.2.5
+Version: 0.2.6
 Summary: An unofficial implementation of the Set Transformer framework in Tensorflow/Keras based on the paper: Set Transformer: A Framework for Attention-based Permutation-Invariant Neural Networks
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Juho Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tf-settransformer-0.2.5/pyproject.toml` & `tf-settransformer-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tf-settransformer"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "An unofficial implementation of the Set Transformer framework in Tensorflow/Keras based on the paper: Set Transformer: A Framework for Attention-based Permutation-Invariant Neural Networks"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `tf-settransformer-0.2.5/src/settransformer/__init__.py` & `tf-settransformer-0.2.6/src/settransformer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 """
 
 import numpy as np
 import tensorflow as tf
 import warnings
 from typing import Any, TypeVar
 
+__version__ = "0.2.6"
+
 DISABLE_WARNINGS = False
 
 # Utility Functions --------------------------------------------------------------------------------
 
 KerasLayer = TypeVar("KerasLayer", bound=tf.keras.layers.Layer)
 
 def warn(warning_type, msg):
@@ -129,15 +131,15 @@
         self.use_spectral_norm = use_spectral_norm
 
         self.fc_q = spectral_dense(embed_dim, use_spectral_norm)
         self.fc_k = spectral_dense(embed_dim, use_spectral_norm)
         self.fc_v = spectral_dense(embed_dim, use_spectral_norm)
 
 
-    def call(self, q, v, k=None, training=None):
+    def call(self, q, v, k=None, return_attention_scores=False, training=None):
         """
         Compute multi-head attention in exactly the same manner
         as the official implementation.
 
         Reference: https://github.com/juho-lee/set_transformer/blob/master/modules.py#L20-L33
         """
         if k is None:
@@ -148,14 +150,16 @@
         q_split = tf.concat(tf.split(q, self.num_heads, 2), 0)
         k_split = tf.concat(tf.split(k, self.num_heads, 2), 0)
         v_split = tf.concat(tf.split(v, self.num_heads, 2), 0)
 
         # Compute attention
         att = tf.nn.softmax(tf.matmul(q_split, k_split, transpose_b=True)/np.sqrt(self.embed_dim), 2)
         out = tf.concat(tf.split(tf.matmul(att, v_split), self.num_heads, 0), 2)
+        if return_attention_scores:
+            return out, att
         return out
 
     def get_config(self):
         config = super().get_config()
         config.update({
             "embed_dim": self.embed_dim,
             "num_heads": self.num_heads,
@@ -216,49 +220,60 @@
     def layernorm(self, key):
         # Keras does not like default dicts...
         ln_key = f"layernorm_{key}"
         if not hasattr(self, ln_key):
             setattr(self, ln_key, tf.keras.layers.LayerNormalization(epsilon=1e-6))
         return getattr(self, ln_key)
 
-    def call_pre_layernorm(self, x, y, training=None):
+    def call_pre_layernorm(self, x, y, return_attention_scores, training=None):
         x_norm = self.layernorm('x')(x)
         y_norm = self.layernorm('y')(y) if y is not x else x_norm
 
         # Multi-head attention
-        attn = x + self.att(x_norm, y_norm, y_norm, training=training)
+        attn, attn_scores = self.att(
+            x_norm, y_norm, y_norm,
+            return_attention_scores=True,
+            training=training)
+        attn = x + attn
 
         # ff-projection
         out = self.layernorm("attn")(attn)
         out = attn + self.ffn(out)
 
         if self.is_final_block:
             out = self.layernorm("final")(out)
+
+        if return_attention_scores:
+            return out, attn_scores
         return out
 
-    def call_post_layernorm(self, x, y, training=None):
+    def call_post_layernorm(self, x, y, return_attention_scores, training=None):
         # Multi-head attention
-        attn = x + self.att(x, y, y, training=training)
+        attn, attn_scores = self.att(x, y, y, return_attention_scores=True, training=training)
+        attn = x + attn
         if self.use_layernorm:
             attn = self.layernorm("attn")(attn)
 
         # ff-projection
         out = attn + self.ffn(attn)
         if self.use_layernorm:
             out = self.layernorm("final")(out)
+
+        if return_attention_scores:
+            return out, attn_scores
         return out
 
     def compute_mask(self, inputs, mask):
         return mask
 
-    def call(self, inputs: tuple, training=None):
+    def call(self, inputs: tuple, return_attention_scores=False, training=None):
         x, y = inputs[0], inputs[1]
         if self.use_layernorm and self.pre_layernorm:
-            return self.call_pre_layernorm(x, y, training)
-        return self.call_post_layernorm(x, y, training)
+            return self.call_pre_layernorm(x, y, return_attention_scores, training)
+        return self.call_post_layernorm(x, y, return_attention_scores, training)
 
     def get_config(self):
         config = super().get_config()
         config.update({
             "embed_dim": self.embed_dim,
             "num_heads": self.num_heads,
             "ff_dim": self.ff_dim,
@@ -273,16 +288,19 @@
 
 
 @CustomLayer
 class SetAttentionBlock(MultiHeadAttentionBlock):
     def build(self, input_shape):
         return super().build((input_shape, input_shape))
 
-    def call(self, x, training=None):
-        return super().call((x, x), training=training)
+    def call(self, x, return_attention_scores=False, training=None):
+        return super().call(
+            (x, x),
+            return_attention_scores=return_attention_scores,
+            training=training)
 
 
 @CustomLayer
 class InducedSetAttentionBlock(tf.keras.layers.Layer):
     def __init__(
         self,
         embed_dim: int,
@@ -315,19 +333,20 @@
             initializer="glorot_uniform", # xavier_uniform from pytorch implementation
             trainable=True,
             name="Inducing_Points")
 
     def compute_mask(self, inputs, mask):
         return mask
 
-    def call(self, x, training=None):
+    def call(self, x, return_attention_scores=False, training=None):
         batch_size = tf.shape(x)[0]
         i = tf.tile(self.inducing_points, (batch_size, 1, 1))
-        h = self.mab1((i, x), training=training)
-        return self.mab2((x, h), training=training)
+        h = self.mab1((i, x), return_attention_scores=False, training=training)
+        result = self.mab2((x, h), return_attention_scores=return_attention_scores, training=training)
+        return result
 
     def get_config(self):
         config = super().get_config()
         config.update({
             "embed_dim": self.embed_dim,
             "num_heads": self.mab2.num_heads,
             "num_induce": self.num_induce,
```

### Comparing `tf-settransformer-0.2.5/src/tf_settransformer.egg-info/PKG-INFO` & `tf-settransformer-0.2.6/src/tf_settransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-settransformer
-Version: 0.2.5
+Version: 0.2.6
 Summary: An unofficial implementation of the Set Transformer framework in Tensorflow/Keras based on the paper: Set Transformer: A Framework for Attention-based Permutation-Invariant Neural Networks
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Juho Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

