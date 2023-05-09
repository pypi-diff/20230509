# Comparing `tmp/numalogic-0.4.dev3.tar.gz` & `tmp/numalogic-0.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.4.dev3.tar", max compression
+gzip compressed data, was "numalogic-0.4.dev4.tar", max compression
```

## Comparing `numalogic-0.4.dev3.tar` & `numalogic-0.4.dev4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-05-05 18:43:20.600149 numalogic-0.4.dev3/LICENSE
--rw-r--r--   0        0        0     5150 2023-05-05 18:43:20.600149 numalogic-0.4.dev3/README.md
--rw-r--r--   0        0        0      895 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/__init__.py
--rw-r--r--   0        0        0      729 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/_constants.py
--rw-r--r--   0        0        0     1004 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/config/__init__.py
--rw-r--r--   0        0        0     2479 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/config/_config.py
--rw-r--r--   0        0        0     3189 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/config/factory.py
--rw-r--r--   0        0        0        0 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/__init__.py
--rw-r--r--   0        0        0      683 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3829 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0     2065 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/trainer.py
--rw-r--r--   0        0        0      581 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11206 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6581 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14239 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8271 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4291 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      211 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     4048 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2490 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0     6087 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/postprocess.py
--rw-r--r--   0        0        0      746 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/preprocess/__init__.py
--rw-r--r--   0        0        0     3654 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/preprocess/transformer.py
--rw-r--r--   0        0        0     1142 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      328 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     4571 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/artifact.py
--rw-r--r--   0        0        0     1608 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    12045 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0     8636 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    11738 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1650 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     3752 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0      215 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0     6218 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/data.py
--rw-r--r--   0        0        0     1082 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     1399 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/types.py
--rw-r--r--   0        0        0     2338 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/pyproject.toml
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 numalogic-0.4.dev3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 16:47:05.963472 numalogic-0.4.dev4/LICENSE
+-rw-r--r--   0        0        0     5150 2023-05-09 16:47:05.963472 numalogic-0.4.dev4/README.md
+-rw-r--r--   0        0        0      895 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/_constants.py
+-rw-r--r--   0        0        0     1004 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     2479 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/config/_config.py
+-rw-r--r--   0        0        0     3257 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/config/factory.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      683 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3829 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0     2065 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/trainer.py
+-rw-r--r--   0        0        0      581 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11206 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6581 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14239 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8271 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4291 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      211 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     4048 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2490 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0     6087 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/postprocess.py
+-rw-r--r--   0        0        0      746 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/preprocess/__init__.py
+-rw-r--r--   0        0        0     3654 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/preprocess/transformer.py
+-rw-r--r--   0        0        0     1142 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     5025 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0     1608 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    12660 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0     9409 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    11738 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1650 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     3752 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0      215 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0     6218 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/data.py
+-rw-r--r--   0        0        0     1082 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     1458 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/types.py
+-rw-r--r--   0        0        0     2359 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/pyproject.toml
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 numalogic-0.4.dev4/PKG-INFO
```

### Comparing `numalogic-0.4.dev3/LICENSE` & `numalogic-0.4.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/README.md` & `numalogic-0.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/__init__.py` & `numalogic-0.4.dev4/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/_constants.py` & `numalogic-0.4.dev4/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/config/__init__.py` & `numalogic-0.4.dev4/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/config/_config.py` & `numalogic-0.4.dev4/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/config/factory.py` & `numalogic-0.4.dev4/numalogic/config/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union
 
-from sklearn.preprocessing import StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler
-
 from numalogic.config._config import ModelInfo, RegistryInfo
-from numalogic.models.autoencoder.variants import (
-    VanillaAE,
-    SparseVanillaAE,
-    Conv1dAE,
-    SparseConv1dAE,
-    LSTMAE,
-    SparseLSTMAE,
-    TransformerAE,
-    SparseTransformerAE,
-)
-from numalogic.models.threshold import StdDevThreshold, StaticThreshold, SigmoidThreshold
-from numalogic.postprocess import TanhNorm, ExpMovingAverage
-from numalogic.preprocess import LogTransformer, StaticPowerTransformer, TanhScaler
-from numalogic.registry import MLflowRegistry, RedisRegistry
 from numalogic.tools.exceptions import UnknownConfigArgsError
 
 
 class _ObjectFactory:
     _CLS_MAP = {}
 
     def get_instance(self, object_info: Union[ModelInfo, RegistryInfo]):
@@ -48,48 +32,68 @@
         except KeyError as err:
             raise UnknownConfigArgsError(
                 f"Invalid model info instance provided: {object_info}"
             ) from err
 
 
 class PreprocessFactory(_ObjectFactory):
+    from sklearn.preprocessing import StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler
+    from numalogic.preprocess import LogTransformer, StaticPowerTransformer, TanhScaler
+
     _CLS_MAP = {
         "StandardScaler": StandardScaler,
         "MinMaxScaler": MinMaxScaler,
         "MaxAbsScaler": MaxAbsScaler,
         "RobustScaler": RobustScaler,
         "LogTransformer": LogTransformer,
         "StaticPowerTransformer": StaticPowerTransformer,
         "TanhScaler": TanhScaler,
     }
 
 
 class PostprocessFactory(_ObjectFactory):
+    from numalogic.postprocess import TanhNorm, ExpMovingAverage
+
     _CLS_MAP = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage}
 
 
 class ThresholdFactory(_ObjectFactory):
+    from numalogic.models.threshold import StdDevThreshold, StaticThreshold, SigmoidThreshold
+
     _CLS_MAP = {
         "StdDevThreshold": StdDevThreshold,
         "StaticThreshold": StaticThreshold,
         "SigmoidThreshold": SigmoidThreshold,
     }
 
 
 class ModelFactory(_ObjectFactory):
+    from numalogic.models.autoencoder.variants import (
+        VanillaAE,
+        SparseVanillaAE,
+        Conv1dAE,
+        SparseConv1dAE,
+        LSTMAE,
+        SparseLSTMAE,
+        TransformerAE,
+        SparseTransformerAE,
+    )
+
     _CLS_MAP = {
         "VanillaAE": VanillaAE,
         "SparseVanillaAE": SparseVanillaAE,
         "Conv1dAE": Conv1dAE,
         "SparseConv1dAE": SparseConv1dAE,
         "LSTMAE": LSTMAE,
         "SparseLSTMAE": SparseLSTMAE,
         "TransformerAE": TransformerAE,
         "SparseTransformerAE": SparseTransformerAE,
     }
 
 
 class RegistryFactory(_ObjectFactory):
+    import numalogic.registry as reg
+
     _CLS_MAP = {
-        "RedisRegistry": RedisRegistry,
-        "MLflowRegistry": MLflowRegistry,
+        "RedisRegistry": getattr(reg, "RedisRegistry"),
+        "MLflowRegistry": getattr(reg, "MLflowRegistry"),
     }
```

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/__init__.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/base.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/trainer.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/forecast/variants/naive.py` & `numalogic-0.4.dev4/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/threshold/_static.py` & `numalogic-0.4.dev4/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/models/threshold/_std.py` & `numalogic-0.4.dev4/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/postprocess.py` & `numalogic-0.4.dev4/numalogic/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/preprocess/__init__.py` & `numalogic-0.4.dev4/numalogic/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/preprocess/transformer.py` & `numalogic-0.4.dev4/numalogic/preprocess/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/registry/__init__.py` & `numalogic-0.4.dev4/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/registry/artifact.py` & `numalogic-0.4.dev4/numalogic/registry/artifact.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
-from numalogic.tools.types import artifact_t, KEYS, META_T, EXTRA_T
+from numalogic.tools.types import artifact_t, KEYS, META_T, META_VT, EXTRA_T
 
 
 @dataclass
 class ArtifactData:
     __slots__ = ("artifact", "metadata", "extras")
 
     artifact: artifact_t
@@ -50,15 +50,15 @@
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             latest: boolean field to determine if latest version is desired or not
             version: explicit artifact version
         """
         raise NotImplementedError("Please implement this method!")
 
-    def save(self, skeys: KEYS, dkeys: KEYS, artifact: artifact_t, **metadata: META_T) -> Any:
+    def save(self, skeys: KEYS, dkeys: KEYS, artifact: artifact_t, **metadata: META_VT) -> Any:
         r"""
         Saves the artifact into mlflow registry and updates version.
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             artifact: primary artifact to be saved
             metadata: additional metadata surrounding the artifact that needs to be saved
@@ -72,14 +72,26 @@
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             version: explicit artifact version
         """
         raise NotImplementedError("Please implement this method!")
 
     @staticmethod
+    def is_artifact_stale(artifact_data: ArtifactData, freq_hr: int) -> bool:
+        """
+        Returns whether the given artifact is stale or not, i.e. if
+        more time has elasped since it was last retrained.
+        Args:
+            artifact_data: ArtifactData object to look into
+            freq_hr: Frequency of retraining in hours
+
+        """
+        raise NotImplementedError("Please implement this method!")
+
+    @staticmethod
     def construct_key(skeys: KEYS, dkeys: KEYS) -> str:
         """
         Returns a single key comprising static and dynamic key fields.
         Override this method if customization is needed.
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
```

### Comparing `numalogic-0.4.dev3/numalogic/registry/localcache.py` & `numalogic-0.4.dev4/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/registry/mlflow_registry.py` & `numalogic-0.4.dev4/numalogic/registry/mlflow_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
+from datetime import datetime, timedelta
 from enum import Enum
 from typing import Optional, Any
 
 import mlflow.pyfunc
 import mlflow.pytorch
 from mlflow.entities.model_registry import ModelVersion
 from mlflow.exceptions import RestException
 from mlflow.protos.databricks_pb2 import ErrorCode, RESOURCE_DOES_NOT_EXIST
 from mlflow.tracking import MlflowClient
 
 from numalogic.registry import ArtifactManager, ArtifactData
 from numalogic.registry.artifact import ArtifactCache
 from numalogic.tools.exceptions import ModelVersionError
-from numalogic.tools.types import artifact_t, KEYS, META_T
+from numalogic.tools.types import artifact_t, KEYS, META_VT
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ModelStage(str, Enum):
     """
     Defines different stages the model state can be in mlflow
@@ -179,15 +180,15 @@
 
     def save(
         self,
         skeys: KEYS,
         dkeys: KEYS,
         artifact: artifact_t,
         run_id: str = None,
-        **metadata: META_T,
+        **metadata: META_VT,
     ) -> Optional[ModelVersion]:
         """
         Saves the artifact into mlflow registry and updates version.
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             artifact: primary artifact to be saved
@@ -209,14 +210,28 @@
             return None
         else:
             _LOGGER.info("Successfully inserted model %s to Mlflow", model_key)
             return model_version
         finally:
             mlflow.end_run()
 
+    @staticmethod
+    def is_artifact_stale(artifact_data: ArtifactData, freq_hr: int) -> bool:
+        """
+        Returns whether the given artifact is stale or not, i.e. if
+        more time has elasped since it was last retrained.
+        Args:
+            artifact_data: ArtifactData object to look into
+            freq_hr: Frequency of retraining in hours
+
+        """
+        date_updated = artifact_data.extras["last_updated_timestamp"] / 1000
+        stale_date = (datetime.now() - timedelta(hours=freq_hr)).timestamp()
+        return date_updated < stale_date
+
     def delete(self, skeys: KEYS, dkeys: KEYS, version: str) -> None:
         """
         Deletes the artifact with a specified version from mlflow registry.
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             version: explicit artifact version
```

### Comparing `numalogic-0.4.dev3/numalogic/registry/redis_registry.py` & `numalogic-0.4.dev4/numalogic/registry/redis_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import time
+from datetime import datetime, timedelta
 from typing import Optional
 
 from redis.exceptions import RedisError
 
 from numalogic.registry import ArtifactManager, ArtifactData
 from numalogic.registry._serialize import loads, dumps
 from numalogic.tools.exceptions import ModelKeyNotFound, RedisRegistryError
-from numalogic.tools.types import artifact_t, redis_client_t, KEYS, META_T
+from numalogic.tools.types import artifact_t, redis_client_t, KEYS, META_T, META_VT
 
 _LOGGER = logging.getLogger()
 
 
 class RedisRegistry(ArtifactManager):
     """
     Model saving and loading using Redis Registry.
@@ -20,22 +21,21 @@
         ttl: Total Time to Live (in seconds) for the key when saving in redis (dafault = 604800)
 
     Examples
     --------
     >>> import redis
     >>> from numalogic.models.autoencoder.variants import VanillaAE
     >>> from numalogic.registry.redis_registry import RedisRegistry
+    >>> ...
     >>> r = redis.StrictRedis(host='127.0.0.1', port=6379)
-    >>> cli = r.client()
-    >>> registry = RedisRegistry(client=cli)
-    >>> skeys = ['c', 'a']
-    >>> dkeys = ['d', 'a']
-    >>> model = VanillaAE(10)
+    >>> registry = RedisRegistry(client=r)
+    >>> skeys, dkeys = ("mymetric", "ae"), ("vanilla", "seq10")
+    >>> model = VanillaAE(seq_len=10)
     >>> registry.save(skeys, dkeys, artifact=model, **{'lr': 0.01})
-    >>> registry.load(skeys, dkeys)
+    >>> loaded_artifact = registry.load(skeys, dkeys)
     """
 
     __slots__ = ("client", "ttl")
 
     def __init__(
         self,
         client: redis_client_t,
@@ -173,15 +173,15 @@
             )
 
     def save(
         self,
         skeys: KEYS,
         dkeys: KEYS,
         artifact: artifact_t,
-        **metadata: META_T,
+        **metadata: META_VT,
     ) -> Optional[str]:
         """
         Saves the artifact into redis registry and updates version.
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             artifact: primary artifact to be saved
@@ -225,7 +225,24 @@
             else:
                 _LOGGER.debug("Key to delete: %s, Not Found !!!\n Exiting.....", del_key)
                 raise ModelKeyNotFound(
                     "Key to delete: %s, Not Found !!!\n Exiting....." % del_key,
                 )
         except RedisError as err:
             raise RedisRegistryError(f"{err.__class__.__name__} raised") from err
+
+    @staticmethod
+    def is_artifact_stale(artifact_data: ArtifactData, freq_hr: int) -> bool:
+        """
+        Returns whether the given artifact is stale or not, i.e. if
+        more time has elasped since it was last retrained.
+        Args:
+            artifact_data: ArtifactData object to look into
+            freq_hr: Frequency of retraining in hours
+
+        """
+        try:
+            artifact_ts = float(artifact_data.extras["timestamp"])
+        except (KeyError, TypeError) as err:
+            raise RedisRegistryError("Error fetching timestamp information") from err
+        stale_ts = (datetime.now() - timedelta(hours=freq_hr)).timestamp()
+        return stale_ts > artifact_ts
```

### Comparing `numalogic-0.4.dev3/numalogic/synthetic/__init__.py` & `numalogic-0.4.dev4/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/synthetic/anomalies.py` & `numalogic-0.4.dev4/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/synthetic/sparsity.py` & `numalogic-0.4.dev4/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/synthetic/timeseries.py` & `numalogic-0.4.dev4/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/tools/callbacks.py` & `numalogic-0.4.dev4/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/tools/data.py` & `numalogic-0.4.dev4/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/tools/exceptions.py` & `numalogic-0.4.dev4/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev3/numalogic/tools/types.py` & `numalogic-0.4.dev4/numalogic/tools/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from redis.client import AbstractRedis
 from sklearn.base import BaseEstimator
 from torch import nn
 
 artifact_t = TypeVar("artifact_t", bound=Union[nn.Module, BaseEstimator])
 META_T = TypeVar("META_T", bound=dict[str, Union[str, list, dict]])
+META_VT = TypeVar("META_VT", bound=Union[str, list, dict])
 EXTRA_T = TypeVar("EXTRA_T", bound=dict[str, Union[str, list, dict]])
 redis_client_t = TypeVar("redis_client_t", bound=AbstractRedis, covariant=True)
 KEYS = TypeVar("KEYS", bound=Sequence[str], covariant=True)
 
 
 class Singleton(type):
     r"""
```

### Comparing `numalogic-0.4.dev3/pyproject.toml` & `numalogic-0.4.dev4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.4.dev3"
+version = "0.4.dev4"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
@@ -22,15 +22,15 @@
 documentation = "https://numalogic.numaproj.io/"
 homepage = "https://numalogic.numaproj.io/"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
 numpy = "^1.23"
 pandas = "^2.0"
-scikit-learn = "^1.0"
+scikit-learn = "^1.2"
 mlflow-skinny = { version = ">2.0, <2.3", optional = true }
 protobuf = "~3.20" # needed to support pytorch-lightning
 omegaconf = "^2.3.0"
 cachetools = "^5.3.0"
 redis = {extras = ["hiredis"], version = "^4.5.4", optional = true}
 
 [tool.poetry.extras]
@@ -51,14 +51,15 @@
 black = "^23.0"
 pytest = "^7.1"
 pytest-cov = "^4.0"
 torchinfo = "^1.7.2"
 ruff = "^0.0.264"
 pre-commit = "^3.3.1"
 fakeredis = "^2.11.2"
+freezegun = "^1.2.2"
 
 [tool.poetry.group.jupyter]
 optional = true
 
 [tool.poetry.group.jupyter.dependencies]
 jupyter = "^1.0.0"
 ipykernel = "^6.15.1"
```

### Comparing `numalogic-0.4.dev3/PKG-INFO` & `numalogic-0.4.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.4.dev3
+Version: 0.4.dev4
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -22,15 +22,15 @@
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: mlflow-skinny (>2.0,<2.3) ; extra == "mlflow"
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: protobuf (>=3.20,<3.21)
 Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0) ; extra == "redis"
-Requires-Dist: scikit-learn (>=1.0,<2.0)
+Requires-Dist: scikit-learn (>=1.2,<2.0)
 Project-URL: Documentation, https://numalogic.numaproj.io/
 Project-URL: Repository, https://github.com/numaproj/numalogic
 Description-Content-Type: text/markdown
 
 # numalogic
 
 [![Build](https://github.com/numaproj/numalogic/actions/workflows/ci.yml/badge.svg)](https://github.com/numaproj/numalogic/actions/workflows/ci.yml)
```

