# Comparing `tmp/dask_histogram-2023.4.4.tar.gz` & `tmp/dask_histogram-2023.5.0.tar.gz`

## Comparing `dask_histogram-2023.4.4.tar` & `dask_histogram-2023.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/__init__.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/bins.py
--rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/boost.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/config.py
--rw-r--r--   0        0        0    38929 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/core.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/histogram.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/py.typed
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/routines.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/sizeof.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/typing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/src/dask_histogram/version.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/LICENSE
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/README.md
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.4/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/__init__.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/bins.py
+-rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/boost.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/config.py
+-rw-r--r--   0        0        0    38953 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/core.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/histogram.yaml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/layers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/py.typed
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/routines.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/sizeof.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/typing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/src/dask_histogram/version.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/README.md
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.5.0/PKG-INFO
```

### Comparing `dask_histogram-2023.4.4/src/dask_histogram/__init__.py` & `dask_histogram-2023.5.0/src/dask_histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/src/dask_histogram/bins.py` & `dask_histogram-2023.5.0/src/dask_histogram/bins.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/src/dask_histogram/boost.py` & `dask_histogram-2023.5.0/src/dask_histogram/boost.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/src/dask_histogram/core.py` & `dask_histogram-2023.5.0/src/dask_histogram/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from dask.context import globalmethod
 from dask.core import flatten
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from dask.threaded import get as tget
 from dask.utils import is_dataframe_like, key_split
 
+from dask_histogram.layers import MockableDataFrameTreeReduction
+
 if TYPE_CHECKING:
     from dask.blockwise import Blockwise
     from numpy.typing import NDArray
 
     from dask_histogram.typing import DaskCollection
 
 __all__ = (
@@ -728,16 +730,14 @@
         return [Delayed(k, graph, layer=layer) for k in keys]
 
 
 def _reduction(
     ph: PartitionedHistogram,
     split_every: int | None = None,
 ) -> AggHistogram:
-    from dask.layers import DataFrameTreeReduction
-
     if split_every is None:
         split_every = dask.config.get("histogram.aggregation.split_every", 8)
     if split_every is False:
         split_every = ph.npartitions
 
     token = tokenize(ph, sum, split_every)
 
@@ -746,26 +746,26 @@
     name_comb = f"{label}-combine-{token}"
     name_agg = f"{label}-agg-{token}"
 
     def hist_safe_sum(items):
         safe_items = [item for item in items if not isinstance(item, tuple)]
         return sum(safe_items)
 
-    dftr = DataFrameTreeReduction(
+    mdftr = MockableDataFrameTreeReduction(
         name=name_agg,
         name_input=ph.name,
         npartitions_input=ph.npartitions,
         concat_func=hist_safe_sum,
         tree_node_func=lambda x: x,
         finalize_func=lambda x: x,
         split_every=split_every,
         tree_node_name=name_comb,
     )
 
-    graph = HighLevelGraph.from_collections(name_agg, dftr, dependencies=(ph,))
+    graph = HighLevelGraph.from_collections(name_agg, mdftr, dependencies=(ph,))
 
     return AggHistogram(graph, name_agg, histref=ph.histref)
 
 
 def _dependencies(
     *args: DaskCollection,
     weights: DaskCollection | None = None,
```

### Comparing `dask_histogram-2023.4.4/src/dask_histogram/routines.py` & `dask_histogram-2023.5.0/src/dask_histogram/routines.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/src/dask_histogram/sizeof.py` & `dask_histogram-2023.5.0/src/dask_histogram/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/.gitignore` & `dask_histogram-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/LICENSE` & `dask_histogram-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/README.md` & `dask_histogram-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/pyproject.toml` & `dask_histogram-2023.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.4/PKG-INFO` & `dask_histogram-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-histogram
-Version: 2023.4.4
+Version: 2023.5.0
 Summary: Histogramming with Dask.
 Project-URL: Homepage, https://github.com/dask-contrib/dask-histogram
 Project-URL: Documentation, https://dask-histogram.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-histogram/issues
 Author-email: Doug Davis <ddavis@ddavis.io>
 License: BSD-3-Clause
 License-File: LICENSE
```

