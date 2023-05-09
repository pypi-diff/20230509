# Comparing `tmp/numalogic-0.4.dev4.tar.gz` & `tmp/numalogic-0.4.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.4.dev4.tar", max compression
+gzip compressed data, was "numalogic-0.4.dev5.tar", max compression
```

## Comparing `numalogic-0.4.dev4.tar` & `numalogic-0.4.dev5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-05-09 16:47:05.963472 numalogic-0.4.dev4/LICENSE
--rw-r--r--   0        0        0     5150 2023-05-09 16:47:05.963472 numalogic-0.4.dev4/README.md
--rw-r--r--   0        0        0      895 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/__init__.py
--rw-r--r--   0        0        0      729 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/_constants.py
--rw-r--r--   0        0        0     1004 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/config/__init__.py
--rw-r--r--   0        0        0     2479 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/config/_config.py
--rw-r--r--   0        0        0     3257 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/config/factory.py
--rw-r--r--   0        0        0        0 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/__init__.py
--rw-r--r--   0        0        0      683 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3829 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0     2065 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/trainer.py
--rw-r--r--   0        0        0      581 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11206 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6581 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14239 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8271 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4291 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      211 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     4048 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2490 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0     6087 2023-05-09 16:47:06.027474 numalogic-0.4.dev4/numalogic/postprocess.py
--rw-r--r--   0        0        0      746 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/preprocess/__init__.py
--rw-r--r--   0        0        0     3654 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/preprocess/transformer.py
--rw-r--r--   0        0        0     1142 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      328 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     5025 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/artifact.py
--rw-r--r--   0        0        0     1608 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    12660 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0     9409 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    11738 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1650 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     3752 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0      215 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0     6218 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/data.py
--rw-r--r--   0        0        0     1082 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     1458 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/numalogic/tools/types.py
--rw-r--r--   0        0        0     2359 2023-05-09 16:47:06.031473 numalogic-0.4.dev4/pyproject.toml
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 numalogic-0.4.dev4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 17:20:41.512659 numalogic-0.4.dev5/LICENSE
+-rw-r--r--   0        0        0     5150 2023-05-09 17:20:41.512659 numalogic-0.4.dev5/README.md
+-rw-r--r--   0        0        0      895 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/_constants.py
+-rw-r--r--   0        0        0     1004 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     2479 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/config/_config.py
+-rw-r--r--   0        0        0     3257 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/config/factory.py
+-rw-r--r--   0        0        0        0 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      683 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3829 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0     2065 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/trainer.py
+-rw-r--r--   0        0        0      581 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11206 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6581 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14239 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8271 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4291 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      211 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     4048 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2490 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0     6087 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/postprocess.py
+-rw-r--r--   0        0        0      746 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/preprocess/__init__.py
+-rw-r--r--   0        0        0     3654 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/preprocess/transformer.py
+-rw-r--r--   0        0        0     1118 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     5025 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0     1608 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    12660 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0     9409 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    11738 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1650 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     3752 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0      215 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0     6218 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/tools/data.py
+-rw-r--r--   0        0        0     1082 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     1458 2023-05-09 17:20:41.568660 numalogic-0.4.dev5/numalogic/tools/types.py
+-rw-r--r--   0        0        0     2369 2023-05-09 17:20:41.572661 numalogic-0.4.dev5/pyproject.toml
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 numalogic-0.4.dev5/PKG-INFO
```

### Comparing `numalogic-0.4.dev4/LICENSE` & `numalogic-0.4.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/README.md` & `numalogic-0.4.dev5/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/__init__.py` & `numalogic-0.4.dev5/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/_constants.py` & `numalogic-0.4.dev5/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/config/__init__.py` & `numalogic-0.4.dev5/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/config/_config.py` & `numalogic-0.4.dev5/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/config/factory.py` & `numalogic-0.4.dev5/numalogic/config/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/__init__.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/base.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/trainer.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.4.dev5/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/forecast/variants/naive.py` & `numalogic-0.4.dev5/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/threshold/_static.py` & `numalogic-0.4.dev5/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/models/threshold/_std.py` & `numalogic-0.4.dev5/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/postprocess.py` & `numalogic-0.4.dev5/numalogic/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/preprocess/__init__.py` & `numalogic-0.4.dev5/numalogic/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/preprocess/transformer.py` & `numalogic-0.4.dev5/numalogic/preprocess/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/registry/artifact.py` & `numalogic-0.4.dev5/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/registry/localcache.py` & `numalogic-0.4.dev5/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/registry/mlflow_registry.py` & `numalogic-0.4.dev5/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/registry/redis_registry.py` & `numalogic-0.4.dev5/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/synthetic/__init__.py` & `numalogic-0.4.dev5/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/synthetic/anomalies.py` & `numalogic-0.4.dev5/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/synthetic/sparsity.py` & `numalogic-0.4.dev5/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/synthetic/timeseries.py` & `numalogic-0.4.dev5/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/tools/callbacks.py` & `numalogic-0.4.dev5/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/tools/data.py` & `numalogic-0.4.dev5/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/tools/exceptions.py` & `numalogic-0.4.dev5/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/numalogic/tools/types.py` & `numalogic-0.4.dev5/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4.dev4/pyproject.toml` & `numalogic-0.4.dev5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.4.dev4"
+version = "0.4.dev5"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
@@ -88,15 +88,15 @@
 )/
 '''
 
 [tool.ruff]
 line-length = 100
 src = ["numalogic", "tests"]
 select = ["E", "F", "W", "C901", "NPY", "RUF", "TRY", "G", "PLE", "PLW", "UP", "ICN", "RET", "Q"]
-ignore = ["TRY003", "TRY301"]
+ignore = ["TRY003", "TRY301", "RUF100"]
 target-version = "py39"
 show-fixes = true
 show-source = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `numalogic-0.4.dev4/PKG-INFO` & `numalogic-0.4.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.4.dev4
+Version: 0.4.dev5
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.11
```

