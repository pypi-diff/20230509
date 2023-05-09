# Comparing `tmp/pgmax-0.5.1.tar.gz` & `tmp/pgmax-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgmax-0.5.1.tar", last modified: Fri Mar 10 00:41:02 2023, max compression
+gzip compressed data, was "pgmax-0.6.0.tar", last modified: Tue May  9 20:31:29 2023, max compression
```

## Comparing `pgmax-0.5.1.tar` & `pgmax-0.6.0.tar`

### file list

```diff
@@ -1,43 +1,50 @@
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.569037 pgmax-0.5.1/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    11357 2023-03-10 00:40:41.000000 pgmax-0.5.1/LICENSE
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     4014 2023-03-10 00:41:02.569037 pgmax-0.5.1/PKG-INFO
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     3749 2023-03-10 00:40:41.000000 pgmax-0.5.1/README.md
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.565037 pgmax-0.5.1/pgmax/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)      669 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/__init__.py
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.569037 pgmax-0.5.1/pgmax/factor/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1725 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/factor/__init__.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    17220 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/factor/enum.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     6952 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/factor/factor.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    24352 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/factor/logical.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    14838 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/factor/pool.py
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.569037 pgmax-0.5.1/pgmax/fgraph/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)      754 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/fgraph/__init__.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    13073 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/fgraph/fgraph.py
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.569037 pgmax-0.5.1/pgmax/fgroup/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1089 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/fgroup/__init__.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    15885 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/fgroup/enum.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     9468 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/fgroup/fgroup.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     3182 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/fgroup/logical.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1930 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/fgroup/pool.py
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.569037 pgmax-0.5.1/pgmax/infer/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1136 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/infer/__init__.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    15130 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/infer/bp.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    13369 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/infer/bp_state.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     7361 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/infer/energy.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1028 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/utils.py
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.569037 pgmax-0.5.1/pgmax/vgroup/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)      783 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/vgroup/__init__.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     6318 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/vgroup/varray.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     6164 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/vgroup/vdict.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     3863 2023-03-10 00:40:41.000000 pgmax-0.5.1/pgmax/vgroup/vgroup.py
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.565037 pgmax-0.5.1/pgmax.egg-info/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     4014 2023-03-10 00:41:02.000000 pgmax-0.5.1/pgmax.egg-info/PKG-INFO
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)      693 2023-03-10 00:41:02.000000 pgmax-0.5.1/pgmax.egg-info/SOURCES.txt
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)        1 2023-03-10 00:41:02.000000 pgmax-0.5.1/pgmax.egg-info/dependency_links.txt
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)       12 2023-03-10 00:41:02.000000 pgmax-0.5.1/pgmax.egg-info/top_level.txt
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)       38 2023-03-10 00:41:02.569037 pgmax-0.5.1/setup.cfg
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1508 2023-03-10 00:40:41.000000 pgmax-0.5.1/setup.py
-drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-03-10 00:41:02.569037 pgmax-0.5.1/tests/
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)      589 2023-03-10 00:40:41.000000 pgmax-0.5.1/tests/__init__.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)     2417 2023-03-10 00:40:41.000000 pgmax-0.5.1/tests/test_examples.py
--rw-r-----   0 adedieu  (1031935) primarygroup (89939)    16084 2023-03-10 00:40:41.000000 pgmax-0.5.1/tests/test_pgmax.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.534866 pgmax-0.6.0/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    11357 2023-05-09 20:31:21.000000 pgmax-0.6.0/LICENSE
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     4401 2023-05-09 20:31:29.534866 pgmax-0.6.0/PKG-INFO
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     4136 2023-05-09 20:31:21.000000 pgmax-0.6.0/README.md
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.526865 pgmax-0.6.0/pgmax/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)      669 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/__init__.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.530866 pgmax-0.6.0/pgmax/factor/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1725 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/factor/__init__.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    17388 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/factor/enum.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     6952 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/factor/factor.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    28785 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/factor/logical.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    17405 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/factor/pool.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     6132 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/factor/update_utils.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.530866 pgmax-0.6.0/pgmax/fgraph/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)      754 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/fgraph/__init__.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    13111 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/fgraph/fgraph.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.530866 pgmax-0.6.0/pgmax/fgroup/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1089 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/fgroup/__init__.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    15779 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/fgroup/enum.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     9484 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/fgroup/fgroup.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     3182 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/fgroup/logical.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1930 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/fgroup/pool.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.530866 pgmax-0.6.0/pgmax/infer/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1586 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/infer/__init__.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    10506 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/infer/bp.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    14100 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/infer/bp_state.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    17904 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/infer/dual_lp.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     7518 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/infer/energy.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     8747 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/infer/inferer.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.530866 pgmax-0.6.0/pgmax/utils/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1727 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/utils/__init__.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     7407 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/utils/primal_lp.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.530866 pgmax-0.6.0/pgmax/vgroup/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)      783 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/vgroup/__init__.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     6719 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/vgroup/varray.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     6450 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/vgroup/vdict.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     4094 2023-05-09 20:31:21.000000 pgmax-0.6.0/pgmax/vgroup/vgroup.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.530866 pgmax-0.6.0/pgmax.egg-info/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     4401 2023-05-09 20:31:29.000000 pgmax-0.6.0/pgmax.egg-info/PKG-INFO
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)      846 2023-05-09 20:31:29.000000 pgmax-0.6.0/pgmax.egg-info/SOURCES.txt
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)        1 2023-05-09 20:31:29.000000 pgmax-0.6.0/pgmax.egg-info/dependency_links.txt
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)       12 2023-05-09 20:31:29.000000 pgmax-0.6.0/pgmax.egg-info/top_level.txt
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)       38 2023-05-09 20:31:29.534866 pgmax-0.6.0/setup.cfg
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     1508 2023-05-09 20:31:21.000000 pgmax-0.6.0/setup.py
+drwxr-x---   0 adedieu  (1031935) primarygroup (89939)        0 2023-05-09 20:31:29.534866 pgmax-0.6.0/tests/
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)      589 2023-05-09 20:31:21.000000 pgmax-0.6.0/tests/__init__.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     2018 2023-05-09 20:31:21.000000 pgmax-0.6.0/tests/test_clipping.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     4619 2023-05-09 20:31:21.000000 pgmax-0.6.0/tests/test_energy.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)     2394 2023-05-09 20:31:21.000000 pgmax-0.6.0/tests/test_examples.py
+-rw-r-----   0 adedieu  (1031935) primarygroup (89939)    16145 2023-05-09 20:31:21.000000 pgmax-0.6.0/tests/test_pgmax.py
```

### Comparing `pgmax-0.5.1/LICENSE` & `pgmax-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/PKG-INFO` & `pgmax-0.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pgmax
-Version: 0.5.1
-Summary: Loopy belief propagation for factor graphs on discrete variables in JAX
-Author: DeepMind
-Author-email: pgmax-dev@google.com
-License: Apache 2.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![continuous-integration](https://github.com/deepmind/PGMax/actions/workflows/ci.yaml/badge.svg)](https://github.com/deepmind/PGMax/actions/workflows/ci.yaml)
 [![PyPI version](https://badge.fury.io/py/pgmax.svg)](https://badge.fury.io/py/pgmax)
 [![Documentation Status](https://readthedocs.org/projects/pgmax/badge/?version=latest)](https://pgmax.readthedocs.io/en/latest/?badge=latest)
 
 # PGMax
 
 PGMax implements general [factor graphs](https://en.wikipedia.org/wiki/Factor_graph)
@@ -74,28 +64,30 @@
 
 ## Getting Started
 
 
 Here are a few self-contained Colab notebooks to help you get started on using PGMax:
 
 - [Tutorial on basic PGMax usage](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/rbm.ipynb)
+- [LBP inference on Ising model](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/ising_model.ipynb)
 - [Implementing max-product LBP](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/rcn.ipynb)
 for [Recursive Cortical Networks](https://www.science.org/doi/10.1126/science.aag2612)
 - [End-to-end differentiable LBP for gradient-based PGM training](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/gmrf.ipynb)
 - [2D binary deconvolution](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/pmp_binary_deconvolution.ipynb)
+- [Alternative inference with Smooth Dual LP-MAP](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/sdlp_examples.ipynb)
 
 ## Citing PGMax
 
-Please consider citing our [companion paper](https://arxiv.org/abs/2202.04110) if you use PGMax in your work:
-
+Please consider citing our [companion paper](https://arxiv.org/abs/2202.04110)
 ```
 @article{zhou2022pgmax,
   author = {Zhou, Guangyao and Dedieu, Antoine and Kumar, Nishanth and L{\'a}zaro-Gredilla, Miguel and Kushagra, Shrinu and George, Dileep},
   title = {{PGMax: Factor Graphs for Discrete Probabilistic Graphical Models and Loopy Belief Propagation in JAX}},
   journal = {arXiv preprint arXiv:2202.04110},
   year={2022}
 }
 ```
+and using the [DeepMind JAX Ecosystem citation](https://github.com/deepmind/jax/blob/main/deepmind2020jax.txt) if you use PGMax in your work.
 
 ## Note
 
 This is not an officially supported Google product.
```

### Comparing `pgmax-0.5.1/README.md` & `pgmax-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: pgmax
+Version: 0.6.0
+Summary: Loopy belief propagation for factor graphs on discrete variables in JAX
+Author: DeepMind
+Author-email: pgmax-dev@google.com
+License: Apache 2.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![continuous-integration](https://github.com/deepmind/PGMax/actions/workflows/ci.yaml/badge.svg)](https://github.com/deepmind/PGMax/actions/workflows/ci.yaml)
 [![PyPI version](https://badge.fury.io/py/pgmax.svg)](https://badge.fury.io/py/pgmax)
 [![Documentation Status](https://readthedocs.org/projects/pgmax/badge/?version=latest)](https://pgmax.readthedocs.io/en/latest/?badge=latest)
 
 # PGMax
 
 PGMax implements general [factor graphs](https://en.wikipedia.org/wiki/Factor_graph)
@@ -64,28 +74,30 @@
 
 ## Getting Started
 
 
 Here are a few self-contained Colab notebooks to help you get started on using PGMax:
 
 - [Tutorial on basic PGMax usage](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/rbm.ipynb)
+- [LBP inference on Ising model](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/ising_model.ipynb)
 - [Implementing max-product LBP](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/rcn.ipynb)
 for [Recursive Cortical Networks](https://www.science.org/doi/10.1126/science.aag2612)
 - [End-to-end differentiable LBP for gradient-based PGM training](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/gmrf.ipynb)
 - [2D binary deconvolution](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/pmp_binary_deconvolution.ipynb)
+- [Alternative inference with Smooth Dual LP-MAP](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/sdlp_examples.ipynb)
 
 ## Citing PGMax
 
-Please consider citing our [companion paper](https://arxiv.org/abs/2202.04110) if you use PGMax in your work:
-
+Please consider citing our [companion paper](https://arxiv.org/abs/2202.04110)
 ```
 @article{zhou2022pgmax,
   author = {Zhou, Guangyao and Dedieu, Antoine and Kumar, Nishanth and L{\'a}zaro-Gredilla, Miguel and Kushagra, Shrinu and George, Dileep},
   title = {{PGMax: Factor Graphs for Discrete Probabilistic Graphical Models and Loopy Belief Propagation in JAX}},
   journal = {arXiv preprint arXiv:2202.04110},
   year={2022}
 }
 ```
+and using the [DeepMind JAX Ecosystem citation](https://github.com/deepmind/jax/blob/main/deepmind2020jax.txt) if you use PGMax in your work.
 
 ## Note
 
 This is not an officially supported Google product.
```

### Comparing `pgmax-0.5.1/pgmax/__init__.py` & `pgmax-0.6.0/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,11 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""A container package for the entire PGMax library."""
-
-__version__ = "0.5.1"
```

### Comparing `pgmax-0.5.1/pgmax/factor/__init__.py` & `pgmax-0.6.0/pgmax/factor/__init__.py`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/pgmax/factor/enum.py` & `pgmax-0.6.0/pgmax/factor/enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import warnings
 
 import jax
 import jax.numpy as jnp
 import numba as nb
 import numpy as np
 from pgmax.factor import factor
+from pgmax.factor import update_utils
 from pgmax.utils import NEG_INF
 
 
 # pylint: disable=unexpected-keyword-arg
 @jax.tree_util.register_pytree_node_class
 @dataclasses.dataclass(frozen=True, eq=False)
 class EnumWiring(factor.Wiring):
@@ -303,22 +304,30 @@
         Only takes into account the EnumFactors of the FactorGraph
       num_val_configs: the total number of valid configurations for all the
         EnumFactors in the factor graph.
       num_factors: the total number of EnumFactors in the factor graph.
     """
     # One-hot decoding of all the factors configs
     fac_config_decoded = (
-        jnp.ones(shape=(num_val_configs,))
+        jnp.ones(shape=(num_val_configs,), dtype=bool)
         .at[factor_configs_indices]
         .multiply(edge_states_one_hot_decoding[factor_configs_edge_states])
     )
+
+    # Replace infinite log potentials
+    clipped_nan_log_potentials = jnp.where(
+        jnp.logical_and(jnp.isinf(log_potentials), fac_config_decoded != 1),
+        -NEG_INF * jnp.sign(log_potentials),
+        log_potentials,
+    )
+
     energy = jnp.where(
         jnp.sum(fac_config_decoded) != num_factors,
         jnp.inf,  # invalid decoding
-        -jnp.sum(fac_config_decoded * log_potentials)
+        -jnp.sum(clipped_nan_log_potentials, where=fac_config_decoded),
     )
     return energy
 
   @staticmethod
   def compute_factor_energy(
       variables: List[Hashable],
       vars_to_map_states: Dict[Hashable, Any],
@@ -398,14 +407,15 @@
     vtof_msgs: jnp.ndarray,
     factor_configs_indices: jnp.ndarray,
     factor_configs_edge_states: jnp.ndarray,
     log_potentials: jnp.ndarray,
     num_val_configs: int,
     num_factors: int,
     temperature: float,
+    normalize: bool
 ) -> jnp.ndarray:
   """Passes messages from EnumFactors to Variables.
 
   The update is performed in two steps.
   (1) First, a "summary" array is generated that has an entry for every valid
   configuration for every EnumFactor. The elements of this array are simply
   the sums of messages across each valid config.
@@ -432,46 +442,39 @@
       EnumFactors in the factor graph.
 
     num_factors: total number of EnumFactors in the factor graph.
 
     temperature: Temperature for loopy belief propagation. 1.0 corresponds
       to sum-product, 0.0 corresponds to max-product.
 
+    normalize: Whether we normalize the outgoing messages. Not used for
+      EnumFactors.
+
   Returns:
     Array of shape (num_edge_states,). This holds all the flattened
     EnumFactors to variable messages.
   """
   fac_config_summary_sum = (
       jnp.zeros(shape=(num_val_configs,))
       .at[factor_configs_indices]
       .add(vtof_msgs[factor_configs_edge_states])
   ) + log_potentials
   max_factor_config_summary_for_edge_states = (
-      jnp.full(shape=(vtof_msgs.shape[0],), fill_value=NEG_INF)
+      jnp.full(shape=(vtof_msgs.shape[0],), fill_value=-jnp.inf)
       .at[factor_configs_edge_states]
       .max(fac_config_summary_sum[factor_configs_indices])
   )
-  ftov_msgs = max_factor_config_summary_for_edge_states
 
-  if temperature != 0.0:
-    ftov_msgs = ftov_msgs + (
-        temperature
-        * jnp.log(
-            jnp.zeros((vtof_msgs.shape[0],))
-            .at[factor_configs_edge_states]
-            .add(
-                jnp.exp(
-                    (
-                        fac_config_summary_sum[factor_configs_indices]
-                        - max_factor_config_summary_for_edge_states[
-                            factor_configs_edge_states
-                        ]
-                    )
-                    / temperature
-                )
-            )
-        )
+  if temperature == 0.0:
+    ftov_msgs = max_factor_config_summary_for_edge_states
+  else:
+    ftov_msgs = update_utils.logsumexps_with_temp(
+        data=fac_config_summary_sum[factor_configs_indices],
+        labels=factor_configs_edge_states,
+        num_labels=vtof_msgs.shape[0],
+        temperature=temperature,
+        maxes=max_factor_config_summary_for_edge_states
     )
 
   # Remove incoming messages
   ftov_msgs -= vtof_msgs
   return ftov_msgs
```

### Comparing `pgmax-0.5.1/pgmax/factor/factor.py` & `pgmax-0.6.0/pgmax/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/pgmax/factor/pool.py` & `pgmax-0.6.0/pgmax/factor/pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import warnings
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from pgmax.factor import factor
 from pgmax.factor import logical
+from pgmax.factor import update_utils
 from pgmax.utils import NEG_INF
 
 
 # pylint: disable=unexpected-keyword-arg
 @jax.tree_util.register_pytree_node_class
 @dataclasses.dataclass(frozen=True, eq=False)
 class PoolWiring(factor.Wiring):
@@ -98,15 +99,15 @@
 
   Note: placing the pool indicator at the end allows us to reuse our
   existing infrastucture for wiring logical factors
   """
 
   log_potentials: np.ndarray = dataclasses.field(
       init=False,
-      default=np.empty((0,)),
+      default_factory=lambda: np.empty((0,)),
   )
 
   def __post_init__(self):
     if len(self.variables) < 2:
       raise ValueError(
           "A PoolFactor requires at least one pool choice and one pool "
           "indicator."
@@ -271,21 +272,22 @@
       factor_energy = np.inf
     else:
       factor_energy = 0.0
     return factor_energy
 
 
 # pylint: disable=unused-argument
-@functools.partial(jax.jit, static_argnames="temperature")
+@functools.partial(jax.jit, static_argnames=("temperature", "normalize"))
 def pass_pool_fac_to_var_messages(
     vtof_msgs: jnp.ndarray,
     pool_choices_factor_indices: jnp.ndarray,
     pool_choices_msg_indices: jnp.ndarray,
     pool_indicators_edge_states: jnp.ndarray,
     temperature: float,
+    normalize: bool,
     log_potentials: Optional[jnp.ndarray] = None,
 ) -> jnp.ndarray:
   """Passes messages from PoolFactors to Variables.
 
   Args:
     vtof_msgs: Array of shape (num_edge_states,). This holds all the flattened
       variable to all the PoolFactors messages.
@@ -308,110 +310,168 @@
       The message index of the pool indicator variable's state 1 is
       pool_indicators_edge_states[ii] + 1
       Only takes into account the PoolFactors of the FactorGraph
 
     temperature: Temperature for loopy belief propagation. 1.0 corresponds to
       sum-product, 0.0 corresponds to max-product.
 
+    normalize: Whether we normalize the outgoing messages. Set to True for BP
+      and to False for Smooth Dual LP.
+
     log_potentials: Optional array of log potentials
 
   Returns:
     Array of shape (num_edge_states,). This holds all the flattened PoolFactors
     to variable messages.
+
+  Note: The updates below are derived to be mathematically stable at low
+    temperatures in (0, 0.1].
+    logaddexp_with_temp, logminusexp_with_temp and logsumexps_with_temp are also
+    derived to be numerically stable at these low temperatures.
   """
   num_factors = pool_indicators_edge_states.shape[0]
 
-  pool_choices_tof_msgs = (
+  pool_choices_tof_msgs_diffs = (
       vtof_msgs[pool_choices_msg_indices + 1]
       - vtof_msgs[pool_choices_msg_indices]
   )
-  pool_indicators_tof_msgs = (
+  pool_choices_tof_msgs_zeros = vtof_msgs[pool_choices_msg_indices]
+
+  pool_indicators_tof_msgs_diffs = (
       vtof_msgs[pool_indicators_edge_states + 1]
       - vtof_msgs[pool_indicators_edge_states]
   )
+  pool_indicators_tof_msgs_ones = vtof_msgs[pool_indicators_edge_states + 1]
+
+  # First, get the easier outgoing messages to pool choices and pool indicators
+  sums_pool_choices_tof_msgs_zeros = (
+      jnp.zeros((num_factors,))
+      .at[pool_choices_factor_indices]
+      .add(pool_choices_tof_msgs_zeros)
+  )
+  pool_choices_msgs_ones = (
+      sums_pool_choices_tof_msgs_zeros[pool_choices_factor_indices]
+      + pool_indicators_tof_msgs_ones[pool_choices_factor_indices]
+      - pool_choices_tof_msgs_zeros
+  )
+  pool_indicators_msgs_zeros = sums_pool_choices_tof_msgs_zeros
 
-  pool_choices_maxes, pool_choices_argmaxes = logical.get_maxes_and_argmaxes(
-      pool_choices_tof_msgs, pool_choices_factor_indices, num_factors
+  # Second derive the other outgoing messages
+  # Get the maxes and argmaxes of pool_choices_tof_msgs_diffs per factor
+  (
+      pool_choices_diffs_maxes,
+      pool_choices_diffs_argmaxes,
+  ) = update_utils.get_maxes_and_argmaxes(
+      pool_choices_tof_msgs_diffs, pool_choices_factor_indices, num_factors
   )
 
   # Consider the max-product case separately.
   if temperature == 0.0:
-    # Get the first and second pool choice argmaxes per factor
-    pool_choices_wo_maxes = pool_choices_tof_msgs.at[pool_choices_argmaxes].set(
-        NEG_INF
-    )
-
-    pool_choices_second_maxes = (
+    # Get the second maxes and argmaxes per factor
+    pool_choices_diffs_wo_maxes = pool_choices_tof_msgs_diffs.at[
+        pool_choices_diffs_argmaxes
+    ].set(NEG_INF)
+    pool_choices_diffs_second_maxes = (
         jnp.full(shape=(num_factors,), fill_value=NEG_INF)
         .at[pool_choices_factor_indices]
-        .max(pool_choices_wo_maxes)
+        .max(pool_choices_diffs_wo_maxes)
     )
 
-    # Compute the maximum of the incoming messages without self
-    pool_choices_maxes_wo_self = pool_choices_maxes[
-        pool_choices_factor_indices
-    ]
-    pool_choices_maxes_wo_self = pool_choices_maxes_wo_self.at[
-        pool_choices_argmaxes
-    ].set(pool_choices_second_maxes)
-
-    # Get the outgoing messages
-    pool_choices_msgs = jnp.minimum(
-        pool_indicators_tof_msgs[pool_choices_factor_indices],
-        -pool_choices_maxes_wo_self,
-    )
-    pool_indicators_msgs = pool_choices_maxes
-
-  else:
-    exp_pool_choices_wo_maxes = jnp.exp(
-        (
-            pool_choices_tof_msgs
-            - pool_choices_maxes[pool_choices_factor_indices]
+    # Get the difference between the outgoing messages
+    pool_choices_msgs_diffs = jnp.minimum(
+        pool_indicators_tof_msgs_diffs, -pool_choices_diffs_maxes
+    )[pool_choices_factor_indices]
+
+    pool_choices_msgs_diffs = pool_choices_msgs_diffs.at[
+        pool_choices_diffs_argmaxes
+    ].set(
+        jnp.minimum(
+            pool_indicators_tof_msgs_diffs, -pool_choices_diffs_second_maxes,
         )
-        / temperature
-    )
-    exp_minus_parents_wo_maxes = jnp.exp(
-        -(pool_indicators_tof_msgs + pool_choices_maxes) / temperature
-    )
-
-    sum_exp_pool_choices_wo_maxes = (
-        jnp.zeros((num_factors,))
-        .at[pool_choices_factor_indices]
-        .add(exp_pool_choices_wo_maxes)
-    )
-    sum_exp_pool_choices_wo_maxes_wo_self = (
-        sum_exp_pool_choices_wo_maxes[pool_choices_factor_indices]
-        - exp_pool_choices_wo_maxes
     )
+    pool_indicators_msgs_diffs = pool_choices_diffs_maxes
 
-    # Get the outgoing messages
-    pool_choices_msgs = -pool_choices_maxes[
-        pool_choices_factor_indices
-    ] - temperature * jnp.log(
-        sum_exp_pool_choices_wo_maxes_wo_self
-        + exp_minus_parents_wo_maxes[pool_choices_factor_indices]
-    )
-    pool_indicators_msgs = pool_choices_maxes + temperature * jnp.log(
-        sum_exp_pool_choices_wo_maxes
-    )
+  else:
+    # Stable difference between the pool indicators outgoing messages
+    pool_indicators_msgs_diffs = update_utils.logsumexps_with_temp(
+        data=pool_choices_tof_msgs_diffs,
+        labels=pool_choices_factor_indices,
+        num_labels=num_factors,
+        temperature=temperature,
+        maxes=pool_choices_diffs_maxes
+    )
+
+    factor_logsumexp_msgs_diffs = update_utils.logaddexp_with_temp(
+        pool_indicators_msgs_diffs,
+        -pool_indicators_tof_msgs_diffs,
+        temperature
+    )
+
+    # Stable difference between the pool choices outgoing messages
+    # Except for the pool_choices_tof_msgs_diffs argmaxes
+    pool_choices_msgs_diffs = - update_utils.logminusexp_with_temp(
+        factor_logsumexp_msgs_diffs[pool_choices_factor_indices],
+        pool_choices_tof_msgs_diffs,
+        temperature,
+    )
+
+    # pool_choices_msgs_diffs above is not numerically stable for the
+    # pool_choices_diffs_argmaxes. The stable update is derived below
+    pool_choices_indicators_diffs = pool_choices_tof_msgs_diffs.at[
+        pool_choices_diffs_argmaxes
+    ].set(-pool_indicators_tof_msgs_diffs)
+
+    pool_choices_msgs_diffs_argmaxes = - update_utils.logsumexps_with_temp(
+        data=pool_choices_indicators_diffs,
+        labels=pool_choices_factor_indices,
+        num_labels=num_factors,
+        temperature=temperature,
+    )
+    pool_choices_msgs_diffs = pool_choices_msgs_diffs.at[
+        pool_choices_diffs_argmaxes
+    ].set(pool_choices_msgs_diffs_argmaxes)
 
-  # Special case: factors with a single parent
+  # Special case: factors with a single pool choice
   num_pool_choices = jnp.bincount(
       pool_choices_factor_indices, length=num_factors
   )
   first_pool_choices = jnp.concatenate(
       [jnp.zeros(1, dtype=int), jnp.cumsum(num_pool_choices)]
   )[:-1]
-  pool_choices_msgs = pool_choices_msgs.at[first_pool_choices].set(
+  pool_choices_msgs_diffs = pool_choices_msgs_diffs.at[first_pool_choices].set(
+      jnp.where(
+          num_pool_choices == 1,
+          pool_indicators_tof_msgs_diffs,
+          pool_choices_msgs_diffs[first_pool_choices],
+      ),
+  )
+  pool_choices_msgs_ones = pool_choices_msgs_ones.at[first_pool_choices].set(
       jnp.where(
           num_pool_choices == 1,
-          pool_indicators_tof_msgs,
-          pool_choices_msgs[first_pool_choices],
+          pool_indicators_tof_msgs_ones,
+          pool_choices_msgs_ones[first_pool_choices],
       ),
   )
 
+  # Outgoing messages
   ftov_msgs = jnp.zeros_like(vtof_msgs)
-  ftov_msgs = ftov_msgs.at[pool_choices_msg_indices + 1].set(pool_choices_msgs)
-  ftov_msgs = ftov_msgs.at[pool_indicators_edge_states + 1].set(
-      pool_indicators_msgs
-  )
+  if normalize:
+    ftov_msgs = ftov_msgs.at[pool_choices_msg_indices + 1].set(
+        pool_choices_msgs_diffs
+    )
+    ftov_msgs = ftov_msgs.at[pool_indicators_edge_states + 1].set(
+        pool_indicators_msgs_diffs
+    )
+  else:
+    ftov_msgs = ftov_msgs.at[pool_choices_msg_indices + 1].set(
+        pool_choices_msgs_ones
+    )
+    ftov_msgs = ftov_msgs.at[pool_choices_msg_indices].set(
+        pool_choices_msgs_ones - pool_choices_msgs_diffs
+    )
+    ftov_msgs = ftov_msgs.at[pool_indicators_edge_states + 1].set(
+        pool_indicators_msgs_zeros + pool_indicators_msgs_diffs
+    )
+    ftov_msgs = ftov_msgs.at[pool_indicators_edge_states].set(
+        pool_indicators_msgs_zeros
+    )
   return ftov_msgs
```

### Comparing `pgmax-0.5.1/pgmax/fgraph/__init__.py` & `pgmax-0.6.0/pgmax/fgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/pgmax/fgraph/fgraph.py` & `pgmax-0.6.0/pgmax/fgraph/fgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import collections
 import copy
 import dataclasses
 import functools
 import types
 from typing import Any, Dict, FrozenSet, List, Mapping, OrderedDict, Sequence, Set, Tuple, Type, Union
 
+import jax.numpy as jnp
 import numpy as np
 from pgmax import factor
 from pgmax import fgroup
 from pgmax import vgroup
 from pgmax.factor import FAC_TO_VAR_UPDATES
 from pgmax.utils import cached_property
 
@@ -266,17 +267,17 @@
     """
     log_potentials = collections.OrderedDict()
     for (
         factor_type,
         factors_groups_by_type,
     ) in self._factor_types_to_groups.items():
       if not factors_groups_by_type:
-        log_potentials[factor_type] = np.empty((0,))
+        log_potentials[factor_type] = jnp.empty((0,))
       else:
-        log_potentials[factor_type] = np.concatenate(
+        log_potentials[factor_type] = jnp.concatenate(
             [
                 factor_group.factor_group_log_potentials
                 for factor_group in factors_groups_by_type
             ]
         )
 
     return log_potentials
@@ -314,26 +315,26 @@
     return self._factor_types_to_groups
 
   @property
   def evidence_to_vars(self) -> np.ndarray:
     """Returns the variable index associated with each evidence entry."""
     var_indices = list(self._vars_to_starts.values()) + [self._num_var_states]
 
-    evidence_to_vars = np.zeros((self._num_var_states,))
+    evidence_to_vars = np.zeros((self._num_var_states,), dtype=int)
     for idx_var in range(len(var_indices) - 1):
       var_start, var_stop = var_indices[idx_var], var_indices[idx_var + 1]
       evidence_to_vars[var_start:var_stop] = idx_var
     return evidence_to_vars
 
   @cached_property
   def fg_state(self) -> FactorGraphState:
     """Current factor graph state given the added factors."""
     # Preliminary computations
     self.compute_offsets()
-    log_potentials = np.concatenate(
+    log_potentials = jnp.concatenate(
         [
             self.log_potentials[factor_type]
             for factor_type in self.log_potentials.keys()
         ]
     )
     assert isinstance(self.variable_groups, list)
```

### Comparing `pgmax-0.5.1/pgmax/fgroup/__init__.py` & `pgmax-0.6.0/pgmax/fgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/pgmax/fgroup/enum.py` & `pgmax-0.6.0/pgmax/fgroup/enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Defines EnumFactorGroup and PairwiseFactorGroup."""
 
 import collections
 import dataclasses
-from typing import Any, FrozenSet, Optional, OrderedDict, Type, Union
+from typing import Any, FrozenSet, OrderedDict, Optional, Type, Union
 
 import jax
 import jax.numpy as jnp
-import numba as nb
 import numpy as np
 from pgmax import factor
 from pgmax.factor import enum
 from pgmax.fgroup import fgroup
 
 
 @dataclasses.dataclass(frozen=True, eq=False)
@@ -48,15 +47,17 @@
   Raises:
     ValueError if:
       (1) The specified log_potentials is not of the expected shape.
       (2) The dtype of the potential array is not float
   """
 
   factor_configs: np.ndarray
-  log_potentials: Optional[np.ndarray] = None  #: :meta private:
+  log_potentials: Optional[Union[np.ndarray, jnp.ndarray]] = (
+      None  #: :meta private:
+  )
   factor_type: Type[factor.Factor] = dataclasses.field(
       init=False,
       default=enum.EnumFactor,
   )  #: :meta private:
 
   def __post_init__(self):
     super().__post_init__()
@@ -72,18 +73,24 @@
           num_val_configs,
       ) and self.log_potentials.shape != (self.num_factors, num_val_configs):
         raise ValueError(
             f"Expected log potentials shape: {(num_val_configs,)} or"
             f" {(self.num_factors, num_val_configs)}. Got"
             f" {self.log_potentials.shape}."
         )
-      log_potentials = np.broadcast_to(
-          self.log_potentials,
-          (self.num_factors, num_val_configs),
-      )
+      if isinstance(self.log_potentials, jnp.ndarray):
+        log_potentials = jnp.broadcast_to(
+            self.log_potentials,
+            (self.num_factors, num_val_configs),
+        )
+      else:
+        log_potentials = np.broadcast_to(
+            self.log_potentials,
+            (self.num_factors, num_val_configs),
+        )
 
     if not np.issubdtype(log_potentials.dtype, np.floating):
       raise ValueError(
           f"Potentials should be floats. Got {log_potentials.dtype}."
       )
     object.__setattr__(self, "log_potentials", log_potentials)
 
@@ -95,22 +102,23 @@
 
     This function is only called on demand when the user requires it.
 
     Returns:
       A dictionary mapping all possible set of connected variables to different
       factors.
     """
+    np_array_log_potentials = np.array(self.log_potentials)
     variables_to_factors = collections.OrderedDict(
         [
             (
                 frozenset(variables_for_factor),
                 enum.EnumFactor(
                     variables=variables_for_factor,
                     factor_configs=self.factor_configs,
-                    log_potentials=np.array(self.log_potentials)[ii],
+                    log_potentials=np_array_log_potentials[ii],
                 ),
             )
             for ii, variables_for_factor in enumerate(
                 self.variables_for_factors
             )
         ]
     )
@@ -224,15 +232,17 @@
       (4) The specified log_potential_matrix does not match the number of
       factors.
       (5) The specified log_potential_matrix does not match the number of
       variable states of the
           variables in the factors.
   """
 
-  log_potential_matrix: Optional[np.ndarray] = None  #: :meta private:
+  log_potential_matrix: Optional[Union[np.ndarray, jnp.ndarray]] = (
+      None  #: :meta private:
+  )
   factor_type: Type[factor.Factor] = dataclasses.field(
       init=False,
       default=enum.EnumFactor,
   )  #: :meta private:
 
   def __post_init__(self):
     super().__post_init__()
@@ -295,23 +305,26 @@
             : log_potential_matrix.shape[-2], : log_potential_matrix.shape[-1]
         ]
         .transpose((1, 2, 0))
         .reshape((-1, 2))
     )
     object.__setattr__(self, "factor_configs", factor_configs)
 
-    log_potential_matrix = np.broadcast_to(
-        log_potential_matrix,
-        (len(self.variables_for_factors),) + log_potential_matrix.shape[-2:],
-    )
-    log_potentials = np.empty((self.num_factors, self.factor_configs.shape[0]))
-    _compute_log_potentials(
-        log_potentials,
-        log_potential_matrix,
-        self.factor_configs,
+    if isinstance(log_potential_matrix, jnp.ndarray):
+      log_potential_matrix = jnp.broadcast_to(
+          log_potential_matrix,
+          (len(self.variables_for_factors),) + log_potential_matrix.shape[-2:],
+      )
+    else:
+      log_potential_matrix = np.broadcast_to(
+          log_potential_matrix,
+          (len(self.variables_for_factors),) + log_potential_matrix.shape[-2:],
+      )
+    log_potentials = log_potential_matrix.reshape(
+        log_potential_matrix.shape[0], -1
     )
     object.__setattr__(self, "log_potentials", log_potentials)
 
   # pylint: disable=g-complex-comprehension
   def _get_variables_to_factors(
       self,
   ) -> OrderedDict[FrozenSet[Any], enum.EnumFactor]:
@@ -416,26 +429,7 @@
           "flat_data should be compatible with shape"
           f" {(num_factors,) + self.log_potential_matrix.shape[-2:]} or"
           f" {(num_factors, np.sum(self.log_potential_matrix.shape[-2:]))}. Got"
           f" {flat_data.shape}."
       )
 
     return data
-
-
-# pylint: disable=g-doc-args
-@nb.jit(parallel=False, cache=True, fastmath=True, nopython=True)
-def _compute_log_potentials(
-    log_potentials: np.ndarray,
-    log_potential_matrix: np.ndarray,
-    factor_configs: np.ndarray,
-):
-  """Fast numba computation of the log_potentials of a PairwiseFactorGroup.
-
-  log_potentials is updated in-place.
-  """
-
-  for config_idx in range(factor_configs.shape[0]):
-    aux = log_potential_matrix[
-        :, factor_configs[config_idx, 0], factor_configs[config_idx, 1]
-    ]
-    log_potentials[:, config_idx] = aux
```

### Comparing `pgmax-0.5.1/pgmax/fgroup/fgroup.py` & `pgmax-0.6.0/pgmax/fgroup/fgroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       ValueError: if the FactorGroup does not contain a Factor
   """
 
   variables_for_factors: Sequence[List[Tuple[int, int]]]
   factor_configs: np.ndarray = dataclasses.field(init=False)
   log_potentials: np.ndarray = dataclasses.field(
       init=False,
-      default=np.empty((0,)),
+      default_factory=lambda: np.empty((0,)),
   )
   factor_type: Type[Any] = dataclasses.field(init=False)
 
   def __post_init__(self):
     if not self.variables_for_factors:
       raise ValueError("Cannot create a FactorGroup with no Factor.")
```

### Comparing `pgmax-0.5.1/pgmax/fgroup/logical.py` & `pgmax-0.6.0/pgmax/fgroup/logical.py`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/pgmax/fgroup/pool.py` & `pgmax-0.6.0/pgmax/fgroup/pool.py`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/pgmax/infer/bp.py` & `pgmax-0.6.0/pgmax/infer/bp_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,432 +9,428 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A module containing the core message-passing functions for belief propagation."""
+"""A module defining container classes for belief propagation states."""
 
 import dataclasses
 import functools
-from typing import Any, Callable, Dict, Hashable, Optional, Sequence, Tuple
-import warnings
+from typing import Any, Dict, Optional, Tuple, Union, cast
 
 import jax
 import jax.numpy as jnp
-from jax.scipy.special import logsumexp
 import numpy as np
-from pgmax import factor
-from pgmax import vgroup
-from pgmax.factor import FAC_TO_VAR_UPDATES
-from pgmax.infer import bp_state as bpstate
-from pgmax.infer.bp_state import BPArrays
-from pgmax.infer.bp_state import BPState
-from pgmax.infer.bp_state import Evidence
-from pgmax.infer.bp_state import FToVMessages
-from pgmax.infer.bp_state import LogPotentials
+from pgmax import fgraph
+from pgmax import fgroup
 from pgmax.utils import NEG_INF
 
 
+@jax.tree_util.register_pytree_node_class
 @dataclasses.dataclass(frozen=True, eq=False)
-class BeliefPropagation:
-  """Belief propagation functions.
+class BPArrays:
+  """Container for the relevant flat arrays used in belief propagation.
 
   Attributes:
-    init: Function to create log_potentials, ftov_msgs and evidence.
-      Args:
-        log_potentials_updates: Optional dictionary of log_potentials updates.
-        ftov_msgs_updates: Optional dictionary of ftov_msgs updates.
-        evidence_updates: Optional dictionary of evidence updates.
-
-      Returns:
-        A BPArrays with the log_potentials, ftov_msgs and evidence.
-
-    update: Function to update log_potentials, ftov_msgs and evidence.
-      Args:
-        bp_arrays: Optional arrays of log_potentials, ftov_msgs, evidence.
-        log_potentials_updates: Optional dictionary of log_potentials updates.
-        ftov_msgs_updates: Optional dictionary of ftov_msgs updates.
-        evidence_updates: Optional dictionary of evidence updates.
-
-      Returns:
-        A BPArrays with the updated log_potentials, ftov_msgs and evidence.
-
-    run_bp: Function to run belief propagation for num_iters with damping.
-      Args:
-        bp_arrays: Initial arrays of log_potentials, ftov_msgs, evidence.
-        num_iters: Number of belief propagation iterations.
-        damping: The damping factor to use for message updates between one
-        timestep and the next.
-
-      Returns:
-        A BPArrays containing the updated ftov_msgs.
-
-    to_bp_state: Function to reconstruct the BPState from a BPArrays.
-      Args:
-        bp_arrays: A BPArrays containing log_potentials, ftov_msgs, evidence.
-
-      Returns:
-        The reconstructed BPState
-
-    get_beliefs: Function to calculate beliefs from a BPArrays.
-      Args:
-        bp_arrays: A BPArrays containing log_potentials, ftov_msgs, evidence.
-
-      Returns:
-        beliefs: Beliefs returned by belief propagation.
+    log_potentials: Flat log potentials array.
+    ftov_msgs: Flat factor to variable messages array.
+    evidence: Flat evidence array.
   """
 
-  init: Callable[..., BPArrays]
-  update: Callable[..., BPArrays]
-  run_bp: Callable[..., BPArrays]
-  to_bp_state: Callable[..., BPArrays]
-  get_beliefs: Callable[..., Dict[Hashable, Any]]
-
-
-# pylint: disable=invalid-name
-def BP(bp_state: BPState, temperature: float = 0.0) -> BeliefPropagation:
-  """Function for generating belief propagation functions.
+  log_potentials: Union[np.ndarray, jnp.ndarray]
+  ftov_msgs: Union[np.ndarray, jnp.ndarray]
+  evidence: Union[np.ndarray, jnp.ndarray]
+
+  def __post_init__(self):
+    for field in self.__dataclass_fields__:
+      if isinstance(getattr(self, field), np.ndarray):
+        getattr(self, field).flags.writeable = False
+
+  def tree_flatten(self):
+    return jax.tree_util.tree_flatten(dataclasses.asdict(self))
+
+  @classmethod
+  def tree_unflatten(cls, aux_data, children):
+    return cls(**aux_data.unflatten(children))
+
+
+@functools.partial(jax.jit, static_argnames="fg_state")
+def update_log_potentials(
+    log_potentials: jnp.ndarray,
+    updates: Dict[Any, Union[np.ndarray, jnp.ndarray]],
+    fg_state: fgraph.FactorGraphState,
+) -> jnp.ndarray:
+  """Returns new log_potentials with updates for a set of factor groups.
 
   Args:
-    bp_state: Belief propagation state.
-    temperature: Temperature for loopy belief propagation. 1.0 corresponds to
-      sum-product, 0.0 corresponds to max-product.
+    log_potentials: A flat jnp array containing log_potentials.
+    updates: A dictionary containing updates for log_potentials
+    fg_state: Factor graph state
 
   Returns:
-    Belief propagation functions.
-  """
-  if jax.lib.xla_bridge.get_backend().platform == "tpu":  # pragma: no cover
-    warnings.warn(
-        "PGMax is not optimized for the TPU backend. Please consider using"
-        " GPUs!"
-    )
+    A flat jnp array containing updated log_potentials.
 
-  wiring = bp_state.fg_state.wiring
-
-  # Add offsets to the edges and factors indices of var_states_for_edges
-  var_states_for_edges = factor.concatenate_var_states_for_edges(
-      [
-          wiring[factor_type].var_states_for_edges
-          for factor_type in FAC_TO_VAR_UPDATES
-      ]
+  Raises: ValueError if
+    (1) Provided log_potentials shape does not match the expected
+        log_potentials shape.
+    (2) Provided name is not valid for log_potentials updates.
+  """
+  # Copy to device and clip updates to not have infinite values
+  updates = jax.tree_util.tree_map(
+      lambda x: jnp.clip(jax.device_put(x), NEG_INF, -NEG_INF), updates
   )
-  var_states_for_edge_states = var_states_for_edges[..., 0]
-  edge_indices_for_edge_states = var_states_for_edges[..., 1]
 
-  num_edges = int(var_states_for_edges[-1, 1]) + 1
-
-  # Inference argumnets per factor type
-  inference_arguments = {}
-  for factor_type in FAC_TO_VAR_UPDATES:
-    this_inference_arguments = wiring[factor_type].get_inference_arguments()
-    inference_arguments[factor_type] = this_inference_arguments
-
-  factor_type_to_msgs_range = bp_state.fg_state.factor_type_to_msgs_range
-  factor_type_to_potentials_range = (
-      bp_state.fg_state.factor_type_to_potentials_range
-  )
+  for factor_group, data in updates.items():
+    if factor_group in fg_state.factor_group_to_potentials_starts:
+      flat_data = factor_group.flatten(data)
+      if flat_data.shape != factor_group.factor_group_log_potentials.shape:
+        raise ValueError(
+            "Expected log potentials shape"
+            f" {factor_group.factor_group_log_potentials.shape} for"
+            f" factor group. Got incompatible data shape {data.shape}."
+        )
+
+      start = fg_state.factor_group_to_potentials_starts[factor_group]
+      log_potentials = log_potentials.at[
+          start : start + flat_data.shape[0]
+      ].set(flat_data)
+    else:
+      raise ValueError("Invalid FactorGroup for log potentials updates.")
 
-  def update(
-      bp_arrays: Optional[BPArrays] = None,
-      log_potentials_updates: Optional[Dict[Any, jnp.ndarray]] = None,
-      ftov_msgs_updates: Optional[Dict[Any, jnp.ndarray]] = None,
-      evidence_updates: Optional[Dict[Any, jnp.ndarray]] = None,
-  ) -> BPArrays:
-    """Function to update belief propagation log_potentials, ftov_msgs, evidence.
+  return log_potentials
 
-    Args:
-      bp_arrays: Optional arrays of log_potentials, ftov_msgs, evidence.
-      log_potentials_updates: Optional dictionary containing log_potentials
-        updates.
-      ftov_msgs_updates: Optional dictionary containing ftov_msgs updates.
-      evidence_updates: Optional dictionary containing evidence updates.
 
-    Returns:
-      A BPArrays with the updated log_potentials, ftov_msgs and evidence.
-    """
-    if bp_arrays is not None:
-      log_potentials = bp_arrays.log_potentials
-      evidence = bp_arrays.evidence
-      ftov_msgs = bp_arrays.ftov_msgs
-    else:
-      log_potentials = jax.device_put(bp_state.log_potentials.value)
-      ftov_msgs = bp_state.ftov_msgs.value
-      evidence = bp_state.evidence.value
-
-    if log_potentials_updates is not None:
-      log_potentials = bpstate.update_log_potentials(
-          log_potentials,
-          log_potentials_updates,
-          bp_state.fg_state,
-      )
+@dataclasses.dataclass(frozen=True, eq=False)
+class LogPotentials:
+  """Class for storing and manipulating log potentials.
 
-    if ftov_msgs_updates is not None:
-      ftov_msgs = bpstate.update_ftov_msgs(
-          ftov_msgs,
-          ftov_msgs_updates,
-          bp_state.fg_state,
-      )
+  Attributes:
+    fg_state: Factor graph state
+    value: Optionally specify an initial value
+  Raises: ValueError if provided value shape does not match the expected
+    log_potentials shape.
+  """
 
-    if evidence_updates is not None:
-      evidence = bpstate.update_evidence(
-          evidence, evidence_updates, bp_state.fg_state
-      )
+  fg_state: fgraph.FactorGraphState
+  value: Optional[np.ndarray] = None
 
-    return BPArrays(
-        log_potentials=log_potentials,
-        ftov_msgs=ftov_msgs,
-        evidence=evidence,
-    )
+  def __post_init__(self):
+    if self.value is None:
+      object.__setattr__(self, "value", self.fg_state.log_potentials)
+    else:
+      if self.value.shape != self.fg_state.log_potentials.shape:
+        raise ValueError(
+            "Expected log potentials shape"
+            f" {self.fg_state.log_potentials.shape}. Got {self.value.shape}."
+        )
+      object.__setattr__(self, "value", self.value)
 
-  def run_bp(
-      bp_arrays: BPArrays,
-      num_iters: int,
-      damping: float = 0.5,
-  ) -> BPArrays:
-    """Function to run belief propagation for num_iters with a damping_factor.
+  def __getitem__(self, factor_group: fgroup.FactorGroup) -> np.ndarray:
+    """Function to query log potentials for a FactorGroup.
 
     Args:
-      bp_arrays: Initial arrays of log_potentials, ftov_msgs, evidence.
-      num_iters: Number of belief propagation iterations.
-      damping: The damping factor to use for message updates between one
-        timestep and the next.
+      factor_group: Queried FactorGroup
 
     Returns:
-      A BPArrays containing the updated ftov_msgs.
+      The queried log potentials.
     """
-    log_potentials = bp_arrays.log_potentials
-    evidence = bp_arrays.evidence
-    ftov_msgs = bp_arrays.ftov_msgs
-
-    # Normalize the messages to ensure the maximum value is 0.
-    ftov_msgs = normalize_and_clip_msgs(
-        ftov_msgs, edge_indices_for_edge_states, num_edges
-    )
-
-    @jax.checkpoint
-    def update(msgs: jnp.ndarray, _) -> Tuple[jnp.ndarray, None]:
-      # Compute new variable to factor messages by message passing
-      vtof_msgs = pass_var_to_fac_messages(
-          msgs, evidence, var_states_for_edge_states,
-      )
-      ftov_msgs = jnp.zeros_like(vtof_msgs)
-      for factor_type in FAC_TO_VAR_UPDATES:
-        msgs_start, msgs_end = factor_type_to_msgs_range[factor_type]
-        potentials_start, potentials_end = factor_type_to_potentials_range[
-            factor_type
-        ]
-        # Do not update the messages for factor types not present in the graph
-        if msgs_start != msgs_end:
-          ftov_msgs_type = FAC_TO_VAR_UPDATES[factor_type](
-              vtof_msgs=vtof_msgs[msgs_start:msgs_end],
-              log_potentials=log_potentials[potentials_start:potentials_end],
-              temperature=temperature,
-              **inference_arguments[factor_type],
-          )
-          ftov_msgs = ftov_msgs.at[msgs_start:msgs_end].set(ftov_msgs_type)
-
-      # Use the results of message passing to perform damping and
-      # update the factor to variable messages
-      delta_msgs = ftov_msgs - msgs
-      msgs = msgs + (1 - damping) * delta_msgs
-      # Normalize and clip these damped, updated messages before returning them.
-      msgs = normalize_and_clip_msgs(
-          msgs, edge_indices_for_edge_states, num_edges
-      )
-      return msgs, None
-
-    # Scan can have significant overhead for a small number of iterations
-    # if not JITed.  Running one it at a time is a common use-case
-    # for checking convergence, so specialize that case.
-    if num_iters > 1:
-      ftov_msgs, _ = jax.lax.scan(update, ftov_msgs, None, num_iters)
+    value = cast(np.ndarray, self.value)
+    if factor_group in self.fg_state.factor_group_to_potentials_starts:
+      start = self.fg_state.factor_group_to_potentials_starts[factor_group]
+      log_potentials = value[
+          start : start + factor_group.factor_group_log_potentials.shape[0]
+      ]
     else:
-      ftov_msgs, _ = update(ftov_msgs, None)
+      raise ValueError("Invalid FactorGroup queried to access log potentials.")
+    return log_potentials
 
-    return BPArrays(
-        log_potentials=log_potentials, ftov_msgs=ftov_msgs, evidence=evidence
-    )
-
-  def to_bp_state(bp_arrays: BPArrays) -> BPState:
-    """Function to reconstruct the BPState from a BPArrays.
+  def __setitem__(
+      self,
+      factor_group: fgroup.FactorGroup,
+      data: Union[np.ndarray, jnp.ndarray],
+  ):
+    """Set the log potentials for a FactorGroup.
 
     Args:
-      bp_arrays: A BPArrays containing log_potentials, ftov_msgs, evidence.
-
-    Returns:
-      The reconstructed BPState
+      factor_group: FactorGroup
+      data: Array containing the log potentials for the FactorGroup
     """
-    return BPState(
-        log_potentials=LogPotentials(
-            fg_state=bp_state.fg_state, value=bp_arrays.log_potentials
-        ),
-        ftov_msgs=FToVMessages(
-            fg_state=bp_state.fg_state,
-            value=bp_arrays.ftov_msgs,
-        ),
-        evidence=Evidence(
-            fg_state=bp_state.fg_state,
-            value=bp_arrays.evidence,
+    object.__setattr__(
+        self,
+        "value",
+        np.asarray(
+            update_log_potentials(
+                jax.device_put(self.value),
+                {factor_group: jax.device_put(data)},
+                self.fg_state,
+            )
         ),
     )
 
-  def unflatten_beliefs(
-      flat_beliefs: jnp.array, variable_groups: Sequence[vgroup.VarGroup]
-  ) -> Dict[Hashable, Any]:
-    """Function to return unflattened beliefs from the flat beliefs.
 
-    Args:
-      flat_beliefs: Flattened array of beliefs
-      variable_groups: All the variable groups in the FactorGraph.
+@functools.partial(jax.jit, static_argnames="fg_state")
+def update_ftov_msgs(
+    ftov_msgs: jnp.ndarray,
+    updates: Dict[Any, Union[np.ndarray, jnp.ndarray]],
+    fg_state: fgraph.FactorGraphState,
+) -> jnp.ndarray:
+  """Returns new ftov_msgs with updates for a set of variables or factor types.
 
-    Returns:
-      Unflattened beliefs
-    """
-    beliefs = {}
-    start = 0
-    for variable_group in variable_groups:
-      num_states = variable_group.num_states
-      assert isinstance(num_states, np.ndarray)
-      length = num_states.sum()
+  Args:
+    ftov_msgs: A flat jnp array containing ftov_msgs.
+    updates: A dictionary mapping the variables or the factor types to their
+      ftov_msgs updates
+    fg_state: Factor graph state
 
-      beliefs[variable_group] = variable_group.unflatten(
-          flat_beliefs[start : start + length]
-      )
-      start += length
-    return beliefs
+  Returns:
+    A flat jnp array containing updated ftov_msgs.
 
-  @jax.jit
-  def get_beliefs(bp_arrays: BPArrays) -> Dict[Hashable, Any]:
-    """Function to calculate beliefs from a BPArrays.
+  Raises: ValueError if:
+    (1) provided ftov_msgs shape does not match the expected ftov_msgs shape.
+    (2) provided variable or factor type is not in the FactorGraph.
+  """
+  # Copy to device and clip updates to not have infinite values
+  updates = jax.tree_util.tree_map(
+      lambda x: jnp.clip(jax.device_put(x), NEG_INF, -NEG_INF), updates
+  )
 
-    Args:
-      bp_arrays: A BPArrays containing log_potentials, ftov_msgs, evidence.
+  for name, data in updates.items():
+    if name in fg_state.factor_type_to_msgs_range:
+      msgs_start, msgs_end = fg_state.factor_type_to_msgs_range[name]
+      if data.shape != (msgs_end - msgs_start,):
+        raise ValueError(
+            f"Expected ftov_msgs shape {(msgs_end - msgs_start,)}"
+            f" for factor type {name}. Got incompatible shape {data.shape}."
+        )
+      ftov_msgs = ftov_msgs.at[msgs_start:msgs_end].set(data)
+
+    elif name in fg_state.vars_to_starts:
+      num_var_states = name[1]
+      if data.shape != (num_var_states,):
+        raise ValueError(
+            f"Expected ftov_msgs shape {(num_var_states,)} for variable {name}."
+            f" Got incompatible shape {data.shape}."
+        )
+
+      var_states_for_edge_states = np.concatenate(
+          [
+              wiring_by_type.var_states_for_edges[..., 0]
+              for wiring_by_type in fg_state.wiring.values()
+          ]
+      )
+      starts = np.nonzero(
+          var_states_for_edge_states == fg_state.vars_to_starts[name]
+      )[0]
+      for start in starts:
+        ftov_msgs = ftov_msgs.at[start : start + name[1]].set(
+            data / starts.shape[0]
+        )
 
-    Returns:
-      beliefs: Beliefs returned by belief propagation.
-    """
+    else:
+      raise ValueError(
+          "Provided variable or factor type is not in the FactorGraph"
+      )
+  return ftov_msgs
 
-    flat_beliefs = (
-        jax.device_put(bp_arrays.evidence)
-        .at[jax.device_put(var_states_for_edge_states)]
-        .add(bp_arrays.ftov_msgs)
-    )
-    return unflatten_beliefs(flat_beliefs, bp_state.fg_state.variable_groups)
 
-  bp = BeliefPropagation(
-      init=functools.partial(update, None),
-      update=update,
-      run_bp=run_bp,
-      to_bp_state=to_bp_state,
-      get_beliefs=get_beliefs,
-  )
-  return bp
+@dataclasses.dataclass(frozen=True, eq=False)
+class FToVMessages:
+  """Class for storing and manipulating factor to variable messages.
 
+  Attributes:
+    fg_state: Factor graph state
+    value: Optionally specify initial value for ftov messages
+  Raises: ValueError if provided value does not match expected ftov messages
+    shape.
+  """
 
-@jax.jit
-def pass_var_to_fac_messages(
-    ftov_msgs: jnp.ndarray,
-    evidence: jnp.ndarray,
-    var_states_for_edge_states: jnp.ndarray,
-) -> jnp.ndarray:
-  """Passes messages from Variables to Factors.
+  fg_state: fgraph.FactorGraphState
+  value: Optional[np.ndarray] = None
 
-  The update works by first summing the evidence and neighboring factor to
-  variable messages for each variable.
-  Next, it subtracts messages from the correct elements of this
-  sum to yield the correct updated messages.
+  def __post_init__(self):
+    if self.value is None:
+      object.__setattr__(
+          self, "value", np.zeros(self.fg_state.total_factor_num_states)
+      )
+    else:
+      if self.value.shape != (self.fg_state.total_factor_num_states,):
+        raise ValueError(
+            "Expected messages shape"
+            f" {(self.fg_state.total_factor_num_states,)}. Got"
+            f" {self.value.shape}."
+        )
+
+      object.__setattr__(self, "value", self.value)
+
+  def __setitem__(
+      self,
+      variable: Tuple[int, int],
+      data: Union[np.ndarray, jnp.ndarray],
+  ) -> None:
+    """Spreading beliefs at a variable to all connected Factors.
 
-  Args:
-    ftov_msgs: Array of shape (num_edge_states,). This holds all the flattened
-      factor to variable messages.
-    evidence: Array of shape (num_var_states,) representing the flattened
-      evidence for each variable
-    var_states_for_edge_states: Array of shape (num_edge_states,).
-      var_states_for_edges[ii] contains the global variable state index
-      associated to each edge state
+    Args:
+      variable: Variable queried
+      data: An array containing the beliefs to be spread uniformly across all
+        factors to variable messages involving this variable.
+    """
 
-  Returns:
-      Array of shape (num_edge_state,). This holds all the flattened variable
-      to factor messages.
-  """
-  var_sums_arr = evidence.at[var_states_for_edge_states].add(ftov_msgs)
-  vtof_msgs = var_sums_arr[var_states_for_edge_states] - ftov_msgs
-  return vtof_msgs
+    object.__setattr__(
+        self,
+        "value",
+        np.asarray(
+            update_ftov_msgs(
+                jax.device_put(self.value),
+                {variable: jax.device_put(data)},
+                self.fg_state,
+            )
+        ),
+    )
 
 
-@functools.partial(jax.jit, static_argnames="num_edges")
-def normalize_and_clip_msgs(
-    msgs: jnp.ndarray, edge_indices_for_edge_states: jnp.ndarray, num_edges: int
+@functools.partial(jax.jit, static_argnames="fg_state")
+def update_evidence(
+    evidence: jnp.ndarray,
+    updates: Dict[Any, Union[np.ndarray, jnp.ndarray]],
+    fg_state: fgraph.FactorGraphState,
 ) -> jnp.ndarray:
-  """Performs normalization and clipping of flattened messages.
-
-  Normalization is done by subtracting the maximum value of every message from
-  every element of every message,
-  clipping is done to keep every message value in the range [-1000, 0].
+  """Returns new evidence with updates for a set of variables or variables groups.
 
   Args:
-    msgs: Array of shape (num_edge_states,). This holds all the flattened factor
-      to variable messages.
-    edge_indices_for_edge_states: Array of shape (num_edge_states,)
-      edge_indices_for_edge_states[ii] contains the global edge index
-      associated to the edge state
-    num_edges: Total number of edges in the factor graph
+    evidence: A flat jnp array containing evidence.
+    updates: A dictionary mapping variables or VarGroups to their updated
+      evidence values.
+    fg_state: Factor graph state
 
   Returns:
-    Array of shape (num_edge_states,). This holds all the flattened factor to
-    variable messages after normalization and clipping
+    A flat jnp array containing the updated evidence values.
+
+  Raises: ValueError if
+    (1) The provided evidence shape does not match the expected one
+    (2) The provided variable or VarGroup is not in the Factorgraph
   """
-  max_by_edges = (
-      jnp.full(shape=(num_edges,), fill_value=NEG_INF)
-      .at[edge_indices_for_edge_states]
-      .max(msgs)
+  # Copy to device and clip updates to not have infinite values
+  updates = jax.tree_util.tree_map(
+      lambda x: jnp.clip(jax.device_put(x), NEG_INF, -NEG_INF), updates
   )
-  norm_msgs = msgs - max_by_edges[edge_indices_for_edge_states]
-
-  # Clip message values to be always greater than NEG_INF
-  new_msgs = jnp.clip(norm_msgs, NEG_INF, None)
-  return new_msgs
 
+  for name, data in updates.items():
+    # Name is a variable_group or a variable
+    if name in fg_state.variable_groups:
+      # The evidence will only be flattened if it is of the expected size
+      flat_data = name.flatten(data)
+
+      first_variable = name.variables[0]
+      start_index = fg_state.vars_to_starts[first_variable]
+      evidence = evidence.at[
+          start_index : start_index + flat_data.shape[0]
+      ].set(flat_data)
+    elif name in fg_state.vars_to_starts:
+      start_index = fg_state.vars_to_starts[name]
+      var_num_states = name[1]
+      if data.shape != (var_num_states,):
+        raise ValueError(
+            f"Expected evidence shape {(var_num_states,)} for variable {name}."
+            f" Got incompatible shape {data.shape}."
+        )
+      evidence = evidence.at[start_index : start_index + name[1]].set(data)
+    else:
+      raise ValueError(
+          "Got evidence for a variable or a VarGroup not in the FactorGraph!"
+      )
+  return evidence
 
-@jax.jit
-def decode_map_states(beliefs: Dict[Hashable, Any]) -> Any:
-  """Function to decode MAP states given the calculated beliefs.
 
-  Args:
-    beliefs: A dictionary mapping each VarGroup to the beliefs of all its
-      variables.
+@dataclasses.dataclass(frozen=True, eq=False)
+class Evidence:
+  """Class for storing and manipulating evidence.
 
-  Returns:
-    A dictionary mapping each VarGroup to the MAP states of all its variables.
+  Attributes:
+    fg_state: Factor graph state
+    value: Optionally specify initial value for evidence
+  Raises: ValueError if provided value does not match expected evidence shape.
   """
-  return jax.tree_util.tree_map(lambda x: jnp.argmax(x, axis=-1), beliefs)
 
+  fg_state: fgraph.FactorGraphState
+  value: Optional[np.ndarray] = None
 
-@jax.jit
-def get_marginals(beliefs: Dict[Hashable, Any]) -> Any:
-  """Function normalizing the beliefs to a valid probability distribution.
+  def __post_init__(self):
+    if self.value is None:
+      value = np.zeros((self.fg_state.num_var_states,))
+      object.__setattr__(self, "value", value)
+    else:
+      if self.value.shape != (self.fg_state.num_var_states,):
+        raise ValueError(
+            f"Expected evidence shape {(self.fg_state.num_var_states,)}. "
+            f"Got {self.value.shape}."
+        )
 
-  When the temperature is equal to 1.0, get_marginals returns the sum-product
-  estimate of the marginal probabilities.
+  def __getitem__(self, variable: Tuple[int, int]) -> np.ndarray:
+    """Returns the evidence of a queried variable.
 
-  When the temperature is equal to 0.0, get_marginals returns the max-product
-  estimate of the normalized max-marginal probabilities, defined as:
-  norm_max_marginals(x_i^*) ∝ max_{x: x_i = x_i^*} p(x)
+    Args:
+      variable: Variable queried
+    """
+    value = cast(np.ndarray, self.value)
+    start = self.fg_state.vars_to_starts[variable]
+    evidence = value[start : start + variable[1]]
+    return evidence
+
+  def __setitem__(
+      self,
+      name: Any,
+      data: np.ndarray,
+  ) -> None:
+    """Updates the evidence of a variable group or of a variable.
 
-  When the temperature is strictly between 0.0 and 1.0, get_marginals returns
-  the belief propagation estimate of the normalized soft max-marginal
-  probabilities, defined as:
-  norm_soft_max_marginals(x_i^*) ∝ (sum_{x: x_i = x_i^*} p(x)^{1 /Temp})^Temp
+    Args:
+      name: The name of a variable group or a single variable. If name is the
+        name of a variable group, updates are derived by using the variable
+        group to flatten the data. If name is the name of a variable, data
+        should be of an array shape (num_states,) If name is None, updates are
+        derived by using self.fg_state.variable_groups to flatten the data.
+      data: Array containing the evidence updates.
+    """
+    object.__setattr__(
+        self,
+        "value",
+        np.asarray(
+            update_evidence(
+                jax.device_put(self.value),
+                {name: jax.device_put(data)},
+                self.fg_state,
+            ),
+        ),
+    )
 
-  Args:
-    beliefs: A dictionary mapping each VarGroup to the beliefs of all its
-      variables.
 
-  Returns:
-    A dictionary mapping each VarGroup to the marginal probabilities of all its
-    variables.
+@dataclasses.dataclass(frozen=True, eq=False)
+class BPState:
+  """Container class for belief propagation states, including log potentials, ftov messages and evidence (unary log potentials).
+
+  Attributes:
+    log_potentials: log potentials of the model
+    ftov_msgs: factor to variable messages
+    evidence: evidence (unary log potentials) for variables.
+    fg_state: associated factor graph state
+  Raises: ValueError if log_potentials, ftov_msgs or evidence are not derived
+    from the same Factor graph state.
   """
-  return jax.tree_util.tree_map(
-      lambda x: jnp.exp(x - logsumexp(x, axis=-1, keepdims=True)), beliefs
-  )
+
+  log_potentials: LogPotentials
+  ftov_msgs: FToVMessages
+  evidence: Evidence
+
+  def __post_init__(self):
+    if (self.log_potentials.fg_state != self.ftov_msgs.fg_state) or (
+        self.ftov_msgs.fg_state != self.evidence.fg_state
+    ):
+      raise ValueError(
+          "log_potentials, ftov_msgs and evidence should be derived from the"
+          " same fg_state."
+      )
+
+  @property
+  def fg_state(self) -> fgraph.FactorGraphState:
+    return self.log_potentials.fg_state
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pgmax-0.5.1/pgmax/infer/energy.py` & `pgmax-0.6.0/pgmax/infer/energy.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
       variables.
 
   Returns:
     A dictionary mapping each individual variable to its MAP state.
   """
   vars_to_map_states = {}
   for variable_group, vg_map_states in map_states.items():
+    if np.prod(variable_group.shape) == 0:  # Skip empty variable groups
+      continue
     vg_map_states_flat = variable_group.flatten(vg_map_states)
     vars_to_map_states.update(
         zip(variable_group.variables, list(np.array(vg_map_states_flat)))
     )
   return vars_to_map_states
 
 
@@ -96,14 +98,16 @@
     this_inference_arguments = wiring[factor_type].get_inference_arguments()
     inference_arguments[factor_type] = this_inference_arguments
 
   # Step 1: compute the contribution of all the variables to the energy
   # Represent the decoding of each variable groups via a one-hot vector
   vgroups_one_hot_decoding = {}
   for variable_group in bp_state.fg_state.variable_groups:
+    if variable_group.num_states.size == 0:
+      continue
     # VarDict will soon inherit from NDVarArray
     assert isinstance(variable_group, vgroup.NDVarArray)
 
     vgroup_decoded = map_states[variable_group]
     vgroup_one_hot_decoding = jnp.zeros(
         shape=vgroup_decoded.shape + (variable_group.num_states.max(),)
     )
@@ -169,15 +173,15 @@
   vars_energies = {}
   factors_energies = {}
 
   # Map each variable to its MAP state
   vars_to_map_states = get_vars_to_map_states(map_states)
 
   # Step 1: compute the contribution of each variable to the energy
-  evidence = Evidence(bp_state.fg_state, value=bp_arrays.evidence)
+  evidence = Evidence(bp_state.fg_state, value=np.array(bp_arrays.evidence))
   for variable_group in bp_state.fg_state.variable_groups:
     for var in variable_group.variables:
       var_decoded_state = int(vars_to_map_states[var])
       var_energy = -float(evidence[var][var_decoded_state])
       vars_energies[var] = var_energy
       energy += var_energy
```

### Comparing `pgmax-0.5.1/pgmax/utils.py` & `pgmax-0.6.0/pgmax/vgroup/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,26 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A module containing helper functions."""
+"""A sub-package defining different types of groups of variables."""
 
-import functools
-from typing import Any, Callable
-
-# A large negative value to use as -inf for numerical stability reasons
-NEG_INF = -1e20
-
-
-def cached_property(func: Callable[..., Any]) -> property:
-  """Customized cached property decorator.
-
-  Args:
-    func: Member function to be decorated
-
-  Returns:
-    Decorated cached property
-  """
-  return property(functools.lru_cache(None)(func))
+from pgmax.vgroup.varray import NDVarArray
+from pgmax.vgroup.vdict import VarDict
+from pgmax.vgroup.vgroup import VarGroup
```

### Comparing `pgmax-0.5.1/pgmax/vgroup/__init__.py` & `pgmax-0.6.0/pgmax/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,12 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A sub-package defining different types of groups of variables."""
+"""A container package for the entire PGMax library."""
 
-from pgmax.vgroup.varray import NDVarArray
-from pgmax.vgroup.vdict import VarDict
-from pgmax.vgroup.vgroup import VarGroup
+__version__ = "0.6.0"
```

### Comparing `pgmax-0.5.1/pgmax/vgroup/varray.py` & `pgmax-0.6.0/pgmax/vgroup/varray.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,19 +150,24 @@
       )
     else:
       raise ValueError(
           f"data should be of shape {self.shape} or"
           f" {self.shape + (self.num_states.max(),)}. Got {data.shape}."
       )
 
-  def unflatten(self, flat_data: Union[np.ndarray, jnp.ndarray]) -> jnp.ndarray:
+  def unflatten(
+      self, flat_data: Union[np.ndarray, jnp.ndarray], per_state: bool
+  ) -> jnp.ndarray:
     """Function that recovers meaningful structured data from internal flat data array.
 
     Args:
       flat_data: Internal flat data array.
+      per_state:  If True, the provided data is per state, such as beliefs for
+        every state for every variable.  Alternatively, it is considered to be
+        per variable, such as a MAP decoding.
 
     Returns:
       Meaningful structured data.
       An array of shape self.shape (for e.g. MAP decodings)
       or an array of shape self.shape + (self.num_states,) (for e.g. evidence,
       beliefs).
 
@@ -174,23 +179,29 @@
     assert isinstance(self.num_states, np.ndarray)
 
     if flat_data.ndim != 1:
       raise ValueError(
           f"Can only unflatten 1D array. Got a {flat_data.ndim}D array."
       )
 
-    if flat_data.size == np.product(self.shape):
-      data = flat_data.reshape(self.shape)
-    elif flat_data.size == self.num_states.sum():
+    if per_state:
+      if flat_data.size != self.num_states.sum():
+        raise ValueError(
+            "flat_data size should be equal to "
+            f"{self.num_states.sum()}. Got size {flat_data.size}."
+        )
       data = jnp.full(
-          shape=self.shape + (self.num_states.max(),), fill_value=-jnp.inf
+          shape=self.shape + (self.num_states.max(initial=0),),
+          fill_value=-jnp.inf,
       )
       data = data.at[
           np.arange(data.shape[-1]) < self.num_states[..., None]
       ].set(flat_data)
-    else:
-      raise ValueError(
-          f"flat_data size should be equal to {np.product(self.shape)} or to "
-          f"{self.num_states.sum()}. Got size {flat_data.size}."
-      )
 
+    else:
+      if flat_data.size != np.product(self.shape):
+        raise ValueError(
+            f"flat_data size should be equal to {np.product(self.shape)}. "
+            f"Got size {flat_data.size}."
+        )
+      data = flat_data.reshape(self.shape)
     return data
```

### Comparing `pgmax-0.5.1/pgmax/vgroup/vdict.py` & `pgmax-0.6.0/pgmax/vgroup/vdict.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,26 +122,29 @@
 
     flat_data = jnp.concatenate(
         [data[var_name].flatten() for var_name in self.variable_names]
     )
     return flat_data
 
   def unflatten(
-      self, flat_data: Union[np.ndarray, jnp.ndarray]
+      self, flat_data: Union[np.ndarray, jnp.ndarray], per_state: bool
   ) -> Dict[Hashable, Union[np.ndarray, jnp.ndarray]]:
     """Function that recovers meaningful structured data from internal flat data array.
 
     Args:
       flat_data: Internal flat data array.
+      per_state:  If True, the provided data is per state, such as beliefs
+        for every state for every variable.  Alternatively, it is considered to
+        be per variable, such as a MAP decoding.
 
     Returns:
       Meaningful structured data.
       Should be a mapping with names from self.variable_names.
       Each value should be an array of shape (1,) (for e.g. MAP decodings) or
-      (self.num_states,) (for e.g. evidence, beliefs).
+      (self.num_states,) (for e.g. evidence, beliefs) depending on per_state
 
     Raises:
       ValueError if:
         (1) flat_data is not a 1D array
         (2) flat_data is not of the right shape
     """
     assert isinstance(self.num_states, np.ndarray)
@@ -149,37 +152,38 @@
     if flat_data.ndim != 1:
       raise ValueError(
           f"Can only unflatten 1D array. Got a {flat_data.ndim}D array."
       )
 
     num_variables = len(self.variable_names)
     num_variable_states = self.num_states.sum()
-    if flat_data.shape[0] == num_variables:
-      use_num_states = False
-    elif flat_data.shape[0] == num_variable_states:
-      use_num_states = True
-    else:
-      raise ValueError(
-          "flat_data should be either of shape"
-          f" (num_variables(={len(self.variables)}),), or"
-          f" (num_variable_states(={num_variable_states}),). Got"
-          f" {flat_data.shape}"
-      )
 
-    if use_num_states:
+    if per_state:
+      if flat_data.shape[0] != num_variable_states:
+        raise ValueError(
+            "flat_data should be shape "
+            f"(num_variable_states(={num_variable_states}),). Got "
+            f"{flat_data.shape}"
+        )
       # Check whether all the variables have the same number of states
       if np.all(self.num_states == self.num_states[0]):
         data = dict(
             zip(self.variable_names, flat_data.reshape(-1, self.num_states[0]))
         )
       else:
         var_states_limits = np.insert(np.cumsum(self.num_states), 0, 0)
         var_states = [
             flat_data[var_states_limits[idx] : var_states_limits[idx + 1]]
             for idx in range(self.num_states.shape[0])
         ]
         data = dict(zip(self.variable_names, var_states))
 
     else:
+      if flat_data.shape[0] != num_variables:
+        raise ValueError(
+            "flat_data should be shape "
+            f"(num_variables(={len(self.variables)}),). Got "
+            f"{flat_data.shape}"
+        )
       data = dict(zip(self.variable_names, flat_data))
 
     return data
```

### Comparing `pgmax-0.5.1/pgmax/vgroup/vgroup.py` & `pgmax-0.6.0/pgmax/vgroup/vgroup.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,19 +114,24 @@
     Returns:
       A flat jnp.array for internal use
     """
     raise NotImplementedError(
         "Please subclass the VarGroup class and override this method"
     )
 
-  def unflatten(self, flat_data: Union[np.ndarray, jnp.ndarray]) -> Any:
+  def unflatten(
+      self, flat_data: Union[np.ndarray, jnp.ndarray], per_state: bool
+  ) -> Any:
     """Function that recovers meaningful structured data from internal flat data array.
 
     Args:
       flat_data: Internal flat data array.
+      per_state:  If True, the provided data is per state, such as beliefs for
+        every state for every variable.  Alternatively, it is considered to be
+        per variable, such as a MAP decoding.
 
     Returns:
       Meaningful structured data
     """
     raise NotImplementedError(
         "Please subclass the VarGroup class and override this method"
     )
```

### Comparing `pgmax-0.5.1/pgmax.egg-info/PKG-INFO` & `pgmax-0.6.0/pgmax.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgmax
-Version: 0.5.1
+Version: 0.6.0
 Summary: Loopy belief propagation for factor graphs on discrete variables in JAX
 Author: DeepMind
 Author-email: pgmax-dev@google.com
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -74,28 +74,30 @@
 
 ## Getting Started
 
 
 Here are a few self-contained Colab notebooks to help you get started on using PGMax:
 
 - [Tutorial on basic PGMax usage](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/rbm.ipynb)
+- [LBP inference on Ising model](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/ising_model.ipynb)
 - [Implementing max-product LBP](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/rcn.ipynb)
 for [Recursive Cortical Networks](https://www.science.org/doi/10.1126/science.aag2612)
 - [End-to-end differentiable LBP for gradient-based PGM training](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/gmrf.ipynb)
 - [2D binary deconvolution](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/pmp_binary_deconvolution.ipynb)
+- [Alternative inference with Smooth Dual LP-MAP](https://colab.research.google.com/github/deepmind/PGMax/blob/master/examples/sdlp_examples.ipynb)
 
 ## Citing PGMax
 
-Please consider citing our [companion paper](https://arxiv.org/abs/2202.04110) if you use PGMax in your work:
-
+Please consider citing our [companion paper](https://arxiv.org/abs/2202.04110)
 ```
 @article{zhou2022pgmax,
   author = {Zhou, Guangyao and Dedieu, Antoine and Kumar, Nishanth and L{\'a}zaro-Gredilla, Miguel and Kushagra, Shrinu and George, Dileep},
   title = {{PGMax: Factor Graphs for Discrete Probabilistic Graphical Models and Loopy Belief Propagation in JAX}},
   journal = {arXiv preprint arXiv:2202.04110},
   year={2022}
 }
 ```
+and using the [DeepMind JAX Ecosystem citation](https://github.com/deepmind/jax/blob/main/deepmind2020jax.txt) if you use PGMax in your work.
 
 ## Note
 
 This is not an officially supported Google product.
```

### Comparing `pgmax-0.5.1/setup.py` & `pgmax-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `pgmax-0.5.1/tests/test_examples.py` & `pgmax-0.6.0/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Test running inference with PGMax in some simple models."""
 
-import jax
 import numpy as np
 from pgmax import fgraph
 from pgmax import fgroup
 from pgmax import infer
 from pgmax import vgroup
 
 
@@ -38,29 +37,27 @@
   factor_group = fgroup.PairwiseFactorGroup(
       variables_for_factors=variables_for_factors,
       log_potential_matrix=0.8 * np.array([[1.0, -1.0], [-1.0, 1.0]]),
   )
   fg.add_factors(factor_group)
 
   # Run inference
-  bp = infer.BP(fg.bp_state, temperature=0)
+  bp = infer.build_inferer(fg.bp_state, backend="bp")
 
   bp_arrays = bp.init(
-      evidence_updates={
-          variables: jax.device_put(np.random.gumbel(size=(50, 50, 2)))
-      }
+      evidence_updates={variables: np.random.gumbel(size=(50, 50, 2))}
   )
 
   # Get the initial energy
   beliefs = bp.get_beliefs(bp_arrays)
   map_states = infer.decode_map_states(beliefs)
   init_energy = infer.compute_energy(fg.bp_state, bp_arrays, map_states)[0]
 
   # Run BP
-  bp_arrays = bp.run_bp(bp_arrays, num_iters=3000)
+  bp_arrays = bp.run(bp_arrays, num_iters=3000, temperature=0)
   beliefs = bp.get_beliefs(bp_arrays)
   map_states = infer.decode_map_states(beliefs)
   assert map_states[variables].shape == (50, 50)
 
   # Compute the energy of the decoding with and without debug mode
   decoding_energy = infer.compute_energy(fg.bp_state, bp_arrays, map_states)[0]
   decoding_energy_debug = infer.compute_energy(
```

### Comparing `pgmax-0.5.1/tests/test_pgmax.py` & `pgmax-0.6.0/tests/test_pgmax.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,16 +408,16 @@
       [
           isinstance(jax.device_put(this_wiring), factor.Wiring)
           for this_wiring in fg.fg_state.wiring.values()
       ]
   )
   bp_state.evidence[grid_vars] = grid_evidence_arr
   bp_state.evidence[additional_vars] = additional_vars_evidence_dict
-  bp = infer.BP(bp_state)
-  bp_arrays = bp.run_bp(bp.init(), num_iters=100)
+  bp = infer.build_inferer(bp_state, backend="bp")
+  bp_arrays = bp.run(bp.init(), num_iters=100, temperature=0.0)
   # Test that the output messages are close to the true messages
   assert jnp.allclose(bp_arrays.ftov_msgs, true_final_msgs_output, atol=1e-06)
   decoded_map_states = infer.decode_map_states(bp.get_beliefs(bp_arrays))
   for name in true_map_state_output:
     assert true_map_state_output[name] == decoded_map_states[name[0]][name[1]]
 
 
@@ -465,11 +465,11 @@
   bp_state = fg.bp_state
   bp_state.evidence[pixel_vars] = np.array(bXn)
   bp_state.evidence[pixel_vars[0, 0]] = np.array([0.0, 0.0, 0.0])
   _ = bp_state.evidence[pixel_vars[0, 0]]
   _ = bp_state.evidence[hidden_vars[0, 0]]
   assert isinstance(bp_state.evidence.value, np.ndarray)
   assert len(sum(fg.factors.values(), ())) == 7056
-  bp = infer.BP(bp_state, temperature=1.0)
-  bp_arrays = bp.run_bp(bp.init(), num_iters=1)
+  bp = infer.build_inferer(bp_state, backend="bp")
+  bp_arrays = bp.run(bp.init(), num_iters=1, temperature=1.0)
   marginals = infer.get_marginals(bp.get_beliefs(bp_arrays))
   assert jnp.allclose(jnp.sum(marginals[pixel_vars], axis=-1), 1.0)
```

