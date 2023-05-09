# Comparing `tmp/pybefit-0.1.2.tar.gz` & `tmp/pybefit-0.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybefit-0.1.2.tar", last modified: Fri Apr 21 16:37:23 2023, max compression
+gzip compressed data, was "pybefit-0.1.21.tar", last modified: Tue May  9 14:24:09 2023, max compression
```

## Comparing `pybefit-0.1.2.tar` & `pybefit-0.1.21.tar`

### file list

```diff
@@ -1,42 +1,54 @@
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/
--rw-r--r--   0 dima      (1000) dima      (1000)     1114 2023-01-22 14:03:59.000000 pybefit-0.1.2/LICENSE.md
--rw-r--r--   0 dima      (1000) dima      (1000)      460 2023-04-21 16:37:23.046908 pybefit-0.1.2/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)     2996 2023-01-22 14:03:59.000000 pybefit-0.1.2/README.md
--rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-04-21 16:37:23.046908 pybefit-0.1.2/setup.cfg
--rw-r--r--   0 dima      (1000) dima      (1000)     1375 2023-04-21 16:37:13.000000 pybefit-0.1.2/setup.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.043575 pybefit-0.1.2/src/
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.043575 pybefit-0.1.2/src/pybefit/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:55.000000 pybefit-0.1.2/src/pybefit/__init__.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/agents/
--rwxr-xr-x   0 dima      (1000) dima      (1000)       19 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     1414 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/base.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/agents/jax/
--rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/jax/__init__.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6438 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/agents/jax/hsmm_ai.py
--rw-r--r--   0 dima      (1000) dima      (1000)      337 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/agents/jax/utils.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/agents/torch/
--rw-r--r--   0 dima      (1000) dima      (1000)      130 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    13071 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/active_inference.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    21780 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/bayesian.py
--rw-r--r--   0 dima      (1000) dima      (1000)    22613 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/dynamic_programming.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1190 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/random.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)     5247 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/agents/torch/rl.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/inference/
--rwxr-xr-x   0 dima      (1000) dima      (1000)       92 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/__init__.py
--rwxr-xr-x   0 dima      (1000) dima      (1000)    10154 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/methods.py
--rw-r--r--   0 dima      (1000) dima      (1000)     1610 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/models.py
--rw-r--r--   0 dima      (1000) dima      (1000)     5429 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/posteriors.py
--rw-r--r--   0 dima      (1000) dima      (1000)     5904 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/priors.py
--rw-r--r--   0 dima      (1000) dima      (1000)     6575 2023-04-21 16:18:01.000000 pybefit-0.1.2/src/pybefit/inference/regression.py
--rwxr--r--   0 dima      (1000) dima      (1000)     2916 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/simulate.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit/tasks/
--rwxr--r--   0 dima      (1000) dima      (1000)       59 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/__init__.py
--rwxr--r--   0 dima      (1000) dima      (1000)     4136 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/bandits.py
--rwxr--r--   0 dima      (1000) dima      (1000)     2650 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/rev_learning.py
--rw-r--r--   0 dima      (1000) dima      (1000)     3716 2023-01-22 14:03:59.000000 pybefit-0.1.2/src/pybefit/tasks/sat.py
-drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-04-21 16:37:23.046908 pybefit-0.1.2/src/pybefit.egg-info/
--rw-r--r--   0 dima      (1000) dima      (1000)      460 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/PKG-INFO
--rw-r--r--   0 dima      (1000) dima      (1000)      974 2023-04-21 16:37:23.000000 pybefit-0.1.2/src/pybefit.egg-info/SOURCES.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/dependency_links.txt
--rw-r--r--   0 dima      (1000) dima      (1000)      104 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/requires.txt
--rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-04-21 16:37:22.000000 pybefit-0.1.2/src/pybefit.egg-info/top_level.txt
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/
+-rw-r--r--   0 dima      (1000) dima      (1000)     1114 2023-01-22 14:03:59.000000 pybefit-0.1.21/LICENSE.md
+-rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-05-09 14:24:09.784801 pybefit-0.1.21/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     2996 2023-01-22 14:03:59.000000 pybefit-0.1.21/README.md
+-rw-r--r--   0 dima      (1000) dima      (1000)       79 2023-05-09 14:24:09.784801 pybefit-0.1.21/setup.cfg
+-rw-r--r--   0 dima      (1000) dima      (1000)     1433 2023-05-09 14:17:55.000000 pybefit-0.1.21/setup.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:55.000000 pybefit-0.1.21/src/pybefit/__init__.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit/agents/
+-rwxr--r--   0 dima      (1000) dima      (1000)       19 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     1414 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/base.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit/agents/jax/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/jax/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6438 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/agents/jax/hsmm_ai.py
+-rw-r--r--   0 dima      (1000) dima      (1000)      337 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/agents/jax/utils.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/agents/torch/
+-rw-r--r--   0 dima      (1000) dima      (1000)      130 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)    13071 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/active_inference.py
+-rwxr--r--   0 dima      (1000) dima      (1000)    21780 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/bayesian.py
+-rw-r--r--   0 dima      (1000) dima      (1000)    22613 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/dynamic_programming.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1190 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/random.py
+-rwxr--r--   0 dima      (1000) dima      (1000)     5247 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/agents/torch/rl.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/inference/
+-rwxr--r--   0 dima      (1000) dima      (1000)       92 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/__init__.py
+-rwxr--r--   0 dima      (1000) dima      (1000)    10154 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/methods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1610 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/models.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/inference/numpyro/
+-rw-r--r--   0 dima      (1000) dima      (1000)        0 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/numpyro/__init__.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1500 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/numpyro/likelihoods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6507 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/numpyro/regression.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     5429 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/posteriors.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     5904 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/priors.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/inference/pyro/
+-rw-r--r--   0 dima      (1000) dima      (1000)       20 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     4860 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/flat.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)    10394 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/hierarchical.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     8701 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/infer.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     1008 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/likelihoods.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6139 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/mixed.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     8109 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/pyro/nonparametric.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     6575 2023-04-21 16:18:01.000000 pybefit-0.1.21/src/pybefit/inference/regression.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     2916 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/simulate.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.784801 pybefit-0.1.21/src/pybefit/tasks/
+-rwxr-xr-x   0 dima      (1000) dima      (1000)       59 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/__init__.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     4136 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/bandits.py
+-rwxr-xr-x   0 dima      (1000) dima      (1000)     2650 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/rev_learning.py
+-rw-r--r--   0 dima      (1000) dima      (1000)     3716 2023-01-22 14:03:59.000000 pybefit-0.1.21/src/pybefit/tasks/sat.py
+drwxr-xr-x   0 dima      (1000) dima      (1000)        0 2023-05-09 14:24:09.781467 pybefit-0.1.21/src/pybefit.egg-info/
+-rw-r--r--   0 dima      (1000) dima      (1000)      461 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/PKG-INFO
+-rw-r--r--   0 dima      (1000) dima      (1000)     1380 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/SOURCES.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        1 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/dependency_links.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)      104 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/requires.txt
+-rw-r--r--   0 dima      (1000) dima      (1000)        8 2023-05-09 14:24:09.000000 pybefit-0.1.21/src/pybefit.egg-info/top_level.txt
```

### Comparing `pybefit-0.1.2/LICENSE.md` & `pybefit-0.1.21/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/README.md` & `pybefit-0.1.21/README.md`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/setup.py` & `pybefit-0.1.21/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 packages = \
 ['pybefit',
  'pybefit.agents',
  'pybefit.agents.jax',
  'pybefit.agents.torch',
  'pybefit.inference',
+ 'pybefit.inference.pyro',
+ 'pybefit.inference.numpyro',
  'pybefit.tasks']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['jax',
@@ -38,15 +40,15 @@
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.10'
 ]
 
 setup_kwargs = {
     'name': 'pybefit',
-    'version': '0.1.2',
+    'version': '0.1.21',
     'description': 'Probabilistic inference for models of behaviour',
     'long_description': 'PyBefit is a Python library for Bayesian analysis of behavioral data. It is based on Pyro/Numpyro a probabilistic programing language, PyTorch, and Jax machine learning libraries.',
     'author': 'Dimitrije Marković',
     'author_email': 'dimitrije.markovic@tu-dresden.de',
     'url': 'https://github.com/dimarkov/pybefit',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pybefit-0.1.2/src/pybefit/agents/base.py` & `pybefit-0.1.21/src/pybefit/agents/base.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/agents/jax/hsmm_ai.py` & `pybefit-0.1.21/src/pybefit/agents/jax/hsmm_ai.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/agents/torch/active_inference.py` & `pybefit-0.1.21/src/pybefit/agents/torch/active_inference.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/agents/torch/bayesian.py` & `pybefit-0.1.21/src/pybefit/agents/torch/bayesian.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/agents/torch/dynamic_programming.py` & `pybefit-0.1.21/src/pybefit/agents/torch/dynamic_programming.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/agents/torch/random.py` & `pybefit-0.1.21/src/pybefit/agents/torch/random.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/agents/torch/rl.py` & `pybefit-0.1.21/src/pybefit/agents/torch/rl.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/inference/methods.py` & `pybefit-0.1.21/src/pybefit/inference/methods.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/inference/models.py` & `pybefit-0.1.21/src/pybefit/inference/models.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/inference/posteriors.py` & `pybefit-0.1.21/src/pybefit/inference/posteriors.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/inference/priors.py` & `pybefit-0.1.21/src/pybefit/inference/priors.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/inference/regression.py` & `pybefit-0.1.21/src/pybefit/inference/regression.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/simulate.py` & `pybefit-0.1.21/src/pybefit/simulate.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/tasks/bandits.py` & `pybefit-0.1.21/src/pybefit/tasks/bandits.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/tasks/rev_learning.py` & `pybefit-0.1.21/src/pybefit/tasks/rev_learning.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit/tasks/sat.py` & `pybefit-0.1.21/src/pybefit/tasks/sat.py`

 * *Files identical despite different names*

### Comparing `pybefit-0.1.2/src/pybefit.egg-info/SOURCES.txt` & `pybefit-0.1.21/src/pybefit.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -22,11 +22,21 @@
 src/pybefit/agents/torch/rl.py
 src/pybefit/inference/__init__.py
 src/pybefit/inference/methods.py
 src/pybefit/inference/models.py
 src/pybefit/inference/posteriors.py
 src/pybefit/inference/priors.py
 src/pybefit/inference/regression.py
+src/pybefit/inference/numpyro/__init__.py
+src/pybefit/inference/numpyro/likelihoods.py
+src/pybefit/inference/numpyro/regression.py
+src/pybefit/inference/pyro/__init__.py
+src/pybefit/inference/pyro/flat.py
+src/pybefit/inference/pyro/hierarchical.py
+src/pybefit/inference/pyro/infer.py
+src/pybefit/inference/pyro/likelihoods.py
+src/pybefit/inference/pyro/mixed.py
+src/pybefit/inference/pyro/nonparametric.py
 src/pybefit/tasks/__init__.py
 src/pybefit/tasks/bandits.py
 src/pybefit/tasks/rev_learning.py
 src/pybefit/tasks/sat.py
```

