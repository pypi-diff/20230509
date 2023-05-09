# Comparing `tmp/pyalslib-1.0.1.tar.gz` & `tmp/pyalslib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalslib-1.0.1.tar", last modified: Fri Jan 13 11:00:38 2023, max compression
+gzip compressed data, was "pyalslib-1.1.0.tar", last modified: Tue May  9 11:50:33 2023, max compression
```

## Comparing `pyalslib-1.0.1.tar` & `pyalslib-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-01-13 11:00:38.666331 pyalslib-1.0.1/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1263 2023-01-13 11:00:38.666331 pyalslib-1.0.1/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2022-12-18 19:42:03.000000 pyalslib-1.0.1/README.md
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-01-13 11:00:38.666331 pyalslib-1.0.1/pyalslib/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5994 2022-11-22 08:19:07.000000 pyalslib-1.0.1/pyalslib/ALSCatalog.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2022-11-22 08:19:07.000000 pyalslib-1.0.1/pyalslib/ALSCatalogCache.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    16947 2023-01-12 21:15:36.000000 pyalslib-1.0.1/pyalslib/ALSGraph.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1859 2022-12-02 10:45:43.000000 pyalslib-1.0.1/pyalslib/ALSRewriter.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2022-12-01 15:22:30.000000 pyalslib-1.0.1/pyalslib/ALSSMT.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2022-11-30 13:27:43.000000 pyalslib-1.0.1/pyalslib/Utility.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11332 2023-01-13 00:22:03.000000 pyalslib-1.0.1/pyalslib/YosysHelper.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-01-12 21:01:17.000000 pyalslib-1.0.1/pyalslib/__init__.py
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-01-13 11:00:38.666331 pyalslib-1.0.1/pyalslib.egg-info/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1263 2023-01-13 11:00:38.000000 pyalslib-1.0.1/pyalslib.egg-info/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      357 2023-01-13 11:00:38.000000 pyalslib-1.0.1/pyalslib.egg-info/SOURCES.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-01-13 11:00:38.000000 pyalslib-1.0.1/pyalslib.egg-info/dependency_links.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-01-13 11:00:38.000000 pyalslib-1.0.1/pyalslib.egg-info/requires.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-01-13 11:00:38.000000 pyalslib-1.0.1/pyalslib.egg-info/top_level.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-01-13 11:00:38.666331 pyalslib-1.0.1/setup.cfg
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-01-12 21:01:11.000000 pyalslib-1.0.1/setup.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-05-09 11:50:33.549561 pyalslib-1.1.0/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-01-19 14:00:21.000000 pyalslib-1.1.0/LICENSE
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-05-09 11:50:33.548561 pyalslib-1.1.0/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1186 2023-01-19 14:00:21.000000 pyalslib-1.1.0/README.md
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-05-09 11:50:33.548561 pyalslib-1.1.0/pyalslib/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     5995 2023-05-09 11:47:18.000000 pyalslib-1.1.0/pyalslib/ALSCatalog.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     7265 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/ALSCatalogCache.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    16896 2023-05-09 11:47:18.000000 pyalslib-1.1.0/pyalslib/ALSGraph.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1859 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/ALSRewriter.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    17375 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/ALSSMT.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2117 2023-01-19 14:00:21.000000 pyalslib-1.1.0/pyalslib/Utility.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    11332 2023-05-09 09:34:12.000000 pyalslib-1.1.0/pyalslib/YosysHelper.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      405 2023-05-09 11:47:18.000000 pyalslib-1.1.0/pyalslib/__init__.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-05-09 11:50:33.548561 pyalslib-1.1.0/pyalslib.egg-info/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1238 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      365 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/SOURCES.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/dependency_links.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       49 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/requires.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        9 2023-05-09 11:50:33.000000 pyalslib-1.1.0/pyalslib.egg-info/top_level.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-05-09 11:50:33.549561 pyalslib-1.1.0/setup.cfg
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1735 2023-05-09 11:47:18.000000 pyalslib-1.1.0/setup.py
```

### Comparing `pyalslib-1.0.1/PKG-INFO` & `pyalslib-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
-Description: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
-Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+
+Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib
```

### Comparing `pyalslib-1.0.1/README.md` & `pyalslib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyalslib-1.0.1/pyalslib/ALSCatalog.py` & `pyalslib-1.1.0/pyalslib/ALSCatalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
 class ALSCatalog:
     def __init__(self, file_name, solver):
         self.__cache_file = file_name
         self.__solver = solver
         ALSCatalogCache(self.__cache_file).init()
 
-    def generate_catalog(self, luts_set, es_timeout):
+    def generate_catalog(self, luts_set, es_timeout, ncpus):
         random.shuffle(luts_set)
         luts_sets = list_partitioning(luts_set, cpu_count())
         args = [ [self.__cache_file, lut_set, es_timeout, self.__solver] for lut_set in luts_sets ]
-        with Pool(cpu_count()) as pool:
+        with Pool(ncpus) as pool:
             catalog = pool.starmap(generate_catalog, args)
         catalog = [ item for sublist in catalog for item in sublist ]
         return catalog
 
 
 def generate_catalog(catalog_cache_file, luts_set, smt_timeout, solver):
     cache = ALSCatalogCache(catalog_cache_file)
```

### Comparing `pyalslib-1.0.1/pyalslib/ALSCatalogCache.py` & `pyalslib-1.1.0/pyalslib/ALSCatalogCache.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.0.1/pyalslib/ALSGraph.py` & `pyalslib-1.1.0/pyalslib/ALSGraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,35 +13,41 @@
 You should have received a copy of the GNU General Public License along with
 RMEncoder; if not, write to the Free Software Foundation, Inc., 51 Franklin
 Street, Fifth Floor, Boston, MA 02110-1301, USA.
 """
 import copy, igraph as ig
 from pyosys import libyosys as ys
 from enum import Enum
-
+import time
 
 class ALSGraph:
     class VertexType(Enum):
         CONSTANT_ZERO = 0,
         CONSTANT_ONE = 1,
         PRIMARY_INPUT = 2,
         CELL = 3,
         PRIMARY_OUTPUT = 4
 
     def __init__(self, design = None):
         if design:
             self.__graph = ig.Graph(directed=True)
             self.__graph_from_design(design)
             self.__graph.topological_sorting()
+
+            type(self).cell_values_base = {v: False for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.CONSTANT_ZERO} | {v: True for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.CONSTANT_ONE}
         else:
             self.__graph = None
+            type(self).cell_values_base is None
 
     def __deepcopy__(self, memo = None):
         graph = ALSGraph()
         graph.__graph = copy.deepcopy(self.__graph)
+
+        type(self).cell_values_base = {v: False for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.CONSTANT_ZERO} | {v: True for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.CONSTANT_ONE}
+        
         return graph
 
     def get_pi(self):
         return [v for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.PRIMARY_INPUT]
 
     def get_po(self):
         return [v for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.PRIMARY_OUTPUT]
@@ -78,45 +84,47 @@
             if pi not in weights.keys():
                 raise ValueError(f"Significance weight for primary input {pi} is not provided in configuration file.")
             else:
                 pi_weights[pi] = weights[pi]
         return pi_weights
 
     def evaluate(self, inputs, lut_io_info, configuration = None):
-        cell_values = {c: False for c in [v for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.CONSTANT_ZERO]} | {c: True for c in [v for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.CONSTANT_ONE]} | {p : inputs[p["name"]] for p in [v for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.PRIMARY_INPUT]}
-        for cell in [v for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.CELL]:
-            _, lut_io_info = self.__evaluate_cell_output(cell_values, cell, lut_io_info, configuration)
-        return {o["name"]: cell_values[o.neighbors(mode="in")[0]] for o in [v for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.PRIMARY_OUTPUT]}, lut_io_info
-
+        cell_values = self.cell_values_base | {v : inputs[v["name"]] for v in self.__graph.vs if v["type"] == ALSGraph.VertexType.PRIMARY_INPUT}
+        for po in self.__graph.vs:
+            if po["type"] == ALSGraph.VertexType.PRIMARY_OUTPUT:
+                _, lut_io_info = self.__evaluate_cell_output(cell_values, self.__graph.vs[po['in'][0]], lut_io_info, configuration)
+        return {o["name"]: cell_values[o.neighbors(mode="in")[0]] for o in self.__graph.vs if o["type"] == ALSGraph.VertexType.PRIMARY_OUTPUT}, lut_io_info
+        
     def __evaluate_cell_output(self, cell_values, cell, lut_io_info, configuration):
         if cell not in cell_values:
             input_values = []
-            input_names = []
             for n in cell["in"]:
-                input_names.append(self.__graph.vs[n]["name"])
                 if self.__graph.vs[n] in cell_values:
                     input_values.append(cell_values[self.__graph.vs[n]])
                 else:
                     o, lut_io_info = self.__evaluate_cell_output(cell_values, self.__graph.vs[n], lut_io_info, configuration)
                     input_values.append(o)
-            out_idx = sum(2 ** i if input_values[i] else 0 for i in range(len(input_values)))
+            out_idx = 0
+            for i in range(len(input_values)):
+                if input_values[i]:
+                    out_idx += 2 ** i
             if configuration is None:
                 cell_values[cell] = cell["spec"][out_idx] == "1"
                 if cell["name"] not in lut_io_info:
                     lut_io_info[cell["name"]] = {"spec": cell["spec"], "freq" : [0] * len(cell["spec"])}       
                 lut_io_info[cell["name"]]["freq"][out_idx] += 1
             else:
                 cell_conf = configuration[cell["name"]]
                 if cell["name"] not in lut_io_info:
                     lut_io_info[cell["name"]] = {"spec": cell_conf["axspec"], "freq" : [0] * len(cell["spec"])}       
                 lut_io_info[cell["name"]]["freq"][out_idx] += 1
                 cell_values[cell] = cell_conf["axspec"][out_idx] == "1"
-            #print("name: {name} Spec: {spec}, Dist.: {dist}, AxSpec: {axspec}, Inputs: {inputs} = {I} (Index: {i}) -> Output: {o} ({O}) AxOutput: {axo})".format(name = cell["name"], spec = cell_spec, dist = dist, axspec = ax_cell_spec, inputs = input_names, I = input_values, i = out_idx, o=out_value, O = cell_values[cell], axo =  ax_out_value))
         return cell_values[cell], lut_io_info
 
+
     def plot(self):
         layout = self.__graph.layout("sugiyama")
         layout.rotate(270)
         ig.plot(self.__graph, layout = layout, bbox=(2000, 2000), margin=120, hovermode='closest', vertex_label_dist = 2.5)
 
     def save(self, file_name):
         layout = self.__graph.layout("sugiyama")
```

### Comparing `pyalslib-1.0.1/pyalslib/ALSRewriter.py` & `pyalslib-1.1.0/pyalslib/ALSRewriter.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.0.1/pyalslib/ALSSMT.py` & `pyalslib-1.1.0/pyalslib/ALSSMT.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.0.1/pyalslib/Utility.py` & `pyalslib-1.1.0/pyalslib/Utility.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.0.1/pyalslib/YosysHelper.py` & `pyalslib-1.1.0/pyalslib/YosysHelper.py`

 * *Files identical despite different names*

### Comparing `pyalslib-1.0.1/pyalslib.egg-info/PKG-INFO` & `pyalslib-1.1.0/pyalslib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pyalslib
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
 Home-page: https://github.com/SalvatoreBarone/pyALSlib
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyALSlib/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyALSlib
-Description: Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib
 Keywords: Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique
-Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.9
+License-File: LICENSE
+
+Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib
```

### Comparing `pyalslib-1.0.1/setup.py` & `pyalslib-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyalslib",
-    version="1.0.1",
+    version="1.1.0",
     description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique",
     long_description="Python implementation of the Catalog-based Aig-rewriting Approximate Logic Synthesis approximation technique. Please visit https://github.com/SalvatoreBarone/pyALSlib",
     url="https://github.com/SalvatoreBarone/pyALSlib",
     author="Salvatore Barone",
     author_email="salvatore.barone@unina.it",
     classifiers=[
         "Intended Audience :: Information Technology",
```

