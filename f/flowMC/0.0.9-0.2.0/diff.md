# Comparing `tmp/flowMC-0.0.9.tar.gz` & `tmp/flowMC-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowMC-0.0.9.tar", last modified: Thu Nov 17 07:06:46 2022, max compression
+gzip compressed data, was "flowMC-0.2.0.tar", last modified: Tue May  9 18:58:39 2023, max compression
```

## Comparing `flowMC-0.0.9.tar` & `flowMC-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,34 @@
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     1080 2022-11-02 23:17:49.000000 flowMC-0.0.9/LICENSE
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      351 2022-11-17 07:06:46.882324 flowMC-0.0.9/PKG-INFO
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2448 2022-11-10 08:16:30.000000 flowMC-0.0.9/README.md
--rw-rw-r--   0 kaze      (1001) kaze      (1001)       88 2022-11-02 23:17:49.000000 flowMC-0.0.9/pyproject.toml
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      510 2022-11-17 07:06:46.882324 flowMC-0.0.9/setup.cfg
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.874323 flowMC-0.0.9/src/
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.878323 flowMC-0.0.9/src/flowMC/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/__init__.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/src/flowMC/nfmodel/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/nfmodel/__init__.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5429 2022-11-15 08:25:19.000000 flowMC-0.0.9/src/flowMC/nfmodel/realNVP.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5230 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/nfmodel/rqSpline.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     3009 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/nfmodel/utils.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/src/flowMC/sampler/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2695 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/Gaussian_random_walk.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     6256 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/HMC.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      558 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/LocalSampler_Base.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5302 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/MALA.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     8150 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/sampler/NF_proposal.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)    15627 2022-11-15 14:15:36.000000 flowMC-0.0.9/src/flowMC/sampler/Sampler.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/sampler/__init__.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     5996 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/sampler/mMALA.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/src/flowMC/utils/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      988 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/PRNG_keys.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     3910 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/PythonFunctionWrap.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        0 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/__init__.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2700 2022-11-02 23:17:49.000000 flowMC-0.0.9/src/flowMC/utils/progressBar.py
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.878323 flowMC-0.0.9/src/flowMC.egg-info/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      351 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/PKG-INFO
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      851 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/SOURCES.txt
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        1 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/dependency_links.txt
--rw-rw-r--   0 kaze      (1001) kaze      (1001)       29 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/requires.txt
--rw-rw-r--   0 kaze      (1001) kaze      (1001)        7 2022-11-17 07:06:46.000000 flowMC-0.0.9/src/flowMC.egg-info/top_level.txt
-drwxrwxr-x   0 kaze      (1001) kaze      (1001)        0 2022-11-17 07:06:46.882324 flowMC-0.0.9/test/
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2367 2022-11-15 14:15:36.000000 flowMC-0.0.9/test/test_HMC.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2433 2022-11-15 14:15:36.000000 flowMC-0.0.9/test/test_MALA.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2244 2022-11-15 14:15:36.000000 flowMC-0.0.9/test/test_RWMCMC.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)     2626 2022-11-02 23:17:49.000000 flowMC-0.0.9/test/test_normalizingFlow.py
--rw-rw-r--   0 kaze      (1001) kaze      (1001)      804 2022-11-02 23:17:49.000000 flowMC-0.0.9/test/test_quickstart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 18:58:28.000000 flowMC-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-09 18:58:39.528934 flowMC-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-09 18:58:28.000000 flowMC-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 18:58:28.000000 flowMC-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-09 18:58:39.528934 flowMC-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.524934 flowMC-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.524934 flowMC-0.2.0/src/flowMC/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC/nfmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/realNVP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/rqSpline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/Gaussian_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/HMC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/LocalSampler_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/MALA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/NF_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16931 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/mMALA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/utils/PRNG_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/utils/PythonFunctionWrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/top_level.txt
```

### Comparing `flowMC-0.0.9/LICENSE` & `flowMC-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.9/README.md` & `flowMC-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# FlowMC
+# flowMC
 
 **Normalizing-flow enhanced sampling package for probabilistic inference**
 
 <a href="https://flowmc.readthedocs.io/en/latest/">
 <img src="https://badgen.net/badge/Read/the doc/blue" alt="doc"/>
 </a>
 <a href="https://github.com/kazewong/FlowMC/blob/Packaging/LICENSE">
 <img src="https://badgen.net/badge/License/MIT/blue" alt="doc"/>
 </a>
 
 ![flowMC_logo](./docs//source/logo_0810.png)
 
-FlowMC is a Jax-based python package for normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling.
+flowMC is a Jax-based python package for normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling.
 The code is open source under MIT license, and it is under active development.
 
 - Just-in-time compilation is supported.
 - Native support for GPU acceleration.
 - Suit for problems with multi-modality.
 - Minimal tuning.
 
@@ -57,15 +57,15 @@
 
 To visualize the inference results in the examples, we requrie the following packages in addtion to the above:
 
     * matplotlib
     * corner
     * arviz
 
-
+The test suite is based on pytest. To run the tests, one needs to install `pytest` and run `pytest` at the root directory of this repo.
 
 # Attribution
 
 A Jax implementation of methods described in: 
 > *Efficient Bayesian Sampling Using Normalizing Flows to Assist Markov Chain Monte Carlo Methods* Gabrié M., Rotskoff G. M., Vanden-Eijnden E. - ICML INNF+ workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx)
 
 > *Adaptive Monte Carlo augmented with normalizing flows.*
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-# FlowMC **Normalizing-flow enhanced sampling package for probabilistic
-inference** [doc] [doc] ![flowMC_logo](./docs//source/logo_0810.png) FlowMC is
+# flowMC **Normalizing-flow enhanced sampling package for probabilistic
+inference** [doc] [doc] ![flowMC_logo](./docs//source/logo_0810.png) flowMC is
 a Jax-based python package for normalizing-flow enhanced Markov chain Monte
 Carlo (MCMC) sampling. The code is open source under MIT license, and it is
 under active development. - Just-in-time compilation is supported. - Native
 support for GPU acceleration. - Suit for problems with multi-modality. -
 Minimal tuning. # Installation The simplest way to install the package is to do
 it through pip ``` pip install flowMC ``` This will install the latest stable
 release and its dependencies. flowMC is based on [Jax](https://github.com/
@@ -15,14 +15,16 @@
 Jax with GPU support: ``` pip install --upgrade "jax[cuda]" -f https://
 storage.googleapis.com/jax-releases/jax_cuda_releases.html ``` If you want to
 install the latest version of flowMC, you can clone this repo and install it
 locally: ``` git clone https://github.com/kazewong/flowMC.git cd flowMC pip
 install -e . ``` ## Requirements Here is a list of packages we use in the main
 library * Python 3.8+ * Jax * Jaxlib * Flax To visualize the inference results
 in the examples, we requrie the following packages in addtion to the above: *
-matplotlib * corner * arviz # Attribution A Jax implementation of methods
-described in: > *Efficient Bayesian Sampling Using Normalizing Flows to Assist
-Markov Chain Monte Carlo Methods* GabriÃ© M., Rotskoff G. M., Vanden-Eijnden E.
-- ICML INNF+ workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx) >
-*Adaptive Monte Carlo augmented with normalizing flows.* GabriÃ© M., Rotskoff
-G. M., Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/
+matplotlib * corner * arviz The test suite is based on pytest. To run the
+tests, one needs to install `pytest` and run `pytest` at the root directory of
+this repo. # Attribution A Jax implementation of methods described in: >
+*Efficient Bayesian Sampling Using Normalizing Flows to Assist Markov Chain
+Monte Carlo Methods* GabriÃ© M., Rotskoff G. M., Vanden-Eijnden E. - ICML INNF+
+workshop 2021 - [pdf](https://openreview.net/pdf?id=mvtooHbjOwx) > *Adaptive
+Monte Carlo augmented with normalizing flows.* GabriÃ© M., Rotskoff G. M.,
+Vanden-Eijnden E. - PNAS 2022 - [doi](https://www.pnas.org/doi/10.1073/
 pnas.2109420119), [arxiv](https://arxiv.org/abs/2105.12603)
```

### Comparing `flowMC-0.0.9/src/flowMC/nfmodel/realNVP.py` & `flowMC-0.2.0/src/flowMC/nfmodel/realNVP.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,25 @@
 from typing import Sequence, Callable
 import jax
 import jax.numpy as jnp
 from flax import linen as nn
 import numpy as np
-
-
-class MLP(nn.Module):
-
-    """
-    Multi-layer perceptron in Flax.
-
-    Parameters
-    ----------
-    features : list of int
-        The number of features in each layer.
-    activation : callable
-        The activation function at each level
-    use_bias : bool
-        Whether to use bias in the layers.
-    init_weight_scale : float
-        The initial weight scale for the layers.
-    kernel_init : callable
-        The kernel initializer for the layers.
-        We use a gaussian kernel with a standard deviation of `init_weight_scale` by default.
-    """
-
-    features: Sequence[int]
-    activation: Callable = nn.relu
-    use_bias: bool = True
-    init_weight_scale: float = 1e-4
-    kernel_i: Callable = jax.nn.initializers.variance_scaling
-
-    def setup(self):
-        self.layers = [
-            nn.Dense(
-                feat,
-                use_bias=self.use_bias,
-                kernel_init=self.kernel_i(self.init_weight_scale, "fan_in", "normal"),
-            )
-            for feat in self.features
-        ]
-
-    def __call__(self, x):
-        for l, layer in enumerate(self.layers[:-1]):
-            x = self.activation(layer(x))
-        x = self.layers[-1](x)
-        return x
-
+from flowMC.nfmodel.mlp import MLP
 
 class AffineCoupling(nn.Module):
-
     """
-    Affine coupling layer. (Defined in the RealNVP paper https://arxiv.org/abs/1605.08803)
+    Affine coupling layer. 
+    (Defined in the RealNVP paper https://arxiv.org/abs/1605.08803)
     We use tanh as the default activation function.
 
-    Parameters
-    ----------
-    n_features : int
-        The number of features in the input.
-    n_hidden : int
-        The number of hidden units in the MLP.
-    mask : ndarray
-        Alternating mask for the affine coupling layer.
-    dt : float
-        Scaling factor for the affine coupling layer.
+    Args:
+        n_features: (int) The number of features in the input.
+        n_hidden: (int) The number of hidden units in the MLP.
+        mask: (ndarray) Alternating mask for the affine coupling layer.
+        dt: (float) Scaling factor for the affine coupling layer.
     """
 
     n_features: int
     n_hidden: int
     mask: jnp.array
     dt: float = 1
 
@@ -93,46 +45,39 @@
         t = self.dt * t
         log_det = -s.reshape(s.shape[0], -1).sum(axis=-1)
         outputs = x * jnp.exp(-s) - t
         return outputs, log_det
 
 
 class RealNVP(nn.Module):
-
     """
-
     RealNVP mode defined in the paper https://arxiv.org/abs/1605.08803.
     MLP is needed to make sure the scaling between layers are more or less the same.
 
-    Parameters
-    ----------
-    n_layer : int
-        The number of affine coupling layers.
-    n_features : int
-        The number of features in the input.
-    n_hidden : int
-        The number of hidden units in the MLP.
-    dt : float
-        Scaling factor for the affine coupling layer.
-    base_mean : ndarray
-        Mean of Gaussian base distribution
-    base_cov : ndarray
-        Covariance of Gaussian base distribution
+    Args:
+        n_layer: (int) The number of affine coupling layers.
+        n_features: (int) The number of features in the input.
+        n_hidden: (int) The number of hidden units in the MLP.
+        dt: (float) Scaling factor for the affine coupling layer.
+
+    Properties:
+        base_mean: (ndarray) Mean of Gaussian base distribution
+        base_cov: (ndarray) Covariance of Gaussian base distribution
     """
 
     n_layer: int
     n_features: int
     n_hidden: int
     dt: float = 1
 
     def setup(self):
         affine_coupling = []
         for i in range(self.n_layer):
             mask = np.ones(self.n_features)
-            mask[int(self.n_features / 2) :] = 0
+            mask[int(self.n_features / 2):] = 0
             if i % 2 == 0:
                 mask = 1 - mask
             mask = jnp.array(mask)
             affine_coupling.append(
                 AffineCoupling(self.n_features, self.n_hidden, mask, dt=self.dt)
             )
         self.affine_coupling = affine_coupling
```

### Comparing `flowMC-0.0.9/src/flowMC/nfmodel/rqSpline.py` & `flowMC-0.2.0/src/flowMC/nfmodel/rqSpline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,15 @@
-from typing import Sequence, Callable, List
+from typing import Sequence, Callable
 import numpy as np
 import jax
 import jax.numpy as jnp
 import distrax
 
 from flax import linen as nn  # The Linen API
-
-
-class MLP(nn.Module):
-    features: Sequence[int]
-    activation: Callable = nn.tanh
-    use_bias: bool = True
-    init_weight_scale: float = 1e-2
-    kernel_i: Callable = jax.nn.initializers.variance_scaling
-
-    def setup(self):
-        self.layers = [
-            nn.Dense(
-                feat,
-                use_bias=self.use_bias,
-                kernel_init=self.kernel_i(self.init_weight_scale, "fan_in", "normal"),
-            )
-            for feat in self.features
-        ]
-
-    def __call__(self, x):
-        for l, layer in enumerate(self.layers[:-1]):
-            x = self.activation(layer(x))
-        x = self.layers[-1](x)
-        return x
+from flowMC.nfmodel.mlp import MLP
 
 
 class Reshape(nn.Module):
     shape: Sequence[int]
 
     def __call__(self, x):
         return jnp.reshape(x.T, self.shape)
@@ -42,16 +19,17 @@
     n_features: int
     hidden_size: Sequence[int]
     num_bijector_params: int
 
     def setup(self):
         self.conditioner = nn.Sequential(
             [
-                MLP([self.n_features] + list(self.hidden_size)),
+                MLP([self.n_features] + list(self.hidden_size),
                 nn.tanh,
+                init_weight_scale=1e-2),
                 nn.Dense(
                     self.n_features * self.num_bijector_params,
                     kernel_init=jax.nn.initializers.zeros,
                     bias_init=jax.nn.initializers.zeros,
                 ),
                 Reshape((self.n_features, self.num_bijector_params)),
             ]
@@ -77,30 +55,27 @@
 
 
 def scalar_affine(params: jnp.ndarray):
     return distrax.ScalarAffine(scale=params[0], shift=params[1])
 
 
 class RQSpline(nn.Module):
-
     """
     Rational quadratic spline normalizing flow model using distrax.
 
-    Parameters
-    ----------
-    n_features : int
-        Number of features in the data.
-    num_layers : int
-        Number of layers in the flow.
-    num_bins : int
-        Number of bins in the spline.
-    hidden_size : Sequence[int]
-        Size of the hidden layers in the conditioner.
-    spline_range : Sequence[float]
-        Range of the spline.
+    Args:
+        n_features : (int) Number of features in the data.
+        num_layers : (int) Number of layers in the flow.
+        num_bins : (int) Number of bins in the spline.
+        hidden_size : (Sequence[int]) Size of the hidden layers in the conditioner.
+        spline_range : (Sequence[float]) Range of the spline.
+    
+    Properties:
+        base_mean: (ndarray) Mean of Gaussian base distribution
+        base_cov: (ndarray) Covariance of Gaussian base distribution
     """
 
     n_features: int
     num_layers: int
     hidden_size: Sequence[int]
     num_bins: int
     spline_range: Sequence[float] = (-10.0, 10.0)
@@ -164,14 +139,17 @@
 
     def __call__(self, x: jnp.array) -> jnp.array:
         x = (x-self.base_mean.value)/jnp.sqrt(jnp.diag(self.base_cov.value))
         base_dist, flow = self.make_flow()
         return distrax.Transformed(base_dist, flow).log_prob(x)
 
     def sample(self, rng: jax.random.PRNGKey, num_samples: int) -> jnp.array:
+        """"
+        Sample from the flow.
+        """
         base_dist, flow = self.make_flow()
         samples = distrax.Transformed(base_dist, flow).sample(
             seed=rng, sample_shape=(num_samples)
         )
         return samples * jnp.sqrt(jnp.diag(self.base_cov.value)) + self.base_mean.value
 
     def log_prob(self, x: jnp.array) -> jnp.array:
```

### Comparing `flowMC-0.0.9/src/flowMC/sampler/HMC.py` & `flowMC-0.2.0/src/flowMC/sampler/HMC.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,28 @@
 import jax
 import jax.numpy as jnp
 from jax.scipy.stats import multivariate_normal
 from tqdm import tqdm
 from flowMC.sampler.LocalSampler_Base import LocalSamplerBase
 
 class HMC(LocalSamplerBase):
+    """
+    Hamiltonian Monte Carlo sampler class builiding the hmc_sampler method
+    from target logpdf.
+
+    Args:
+        logpdf: target logpdf function 
+        jit: whether to jit the sampler
+        params: dictionary of parameters for the sampler
+    """
     
-    def __init__(self, logpdf: Callable, jit: bool, params: dict) -> Callable:
+    def __init__(self, logpdf: Callable, jit: bool, params: dict, verbose: bool = False) -> Callable:
         super().__init__(logpdf, jit, params)
 
-        self.potential = lambda x: -self.logpdf(x)
+        self.potential = lambda x, data: -logpdf(x, data)
         self.grad_potential = jax.grad(self.potential)
         
         self.params = params
         if "condition_matrix" in params:
             self.inverse_metric = params["condition_matrix"]
         else:
             self.inverse_metric = 1
@@ -25,108 +34,121 @@
         if "n_leapfrog" in params:
             self.n_leapfrog = params["n_leapfrog"]
         else:
             raise NotImplementedError
 
         self.kinetic = lambda p, params: 0.5*(p**2 * params['inverse_metric']).sum()
         self.grad_kinetic = jax.grad(self.kinetic)
-
-    def get_initial_hamiltonian(self, rng_key: jax.random.PRNGKey, position: jnp.array, params: dict):
-        momentum = jax.random.normal(rng_key, shape=position.shape) * params['inverse_metric']
-        return self.potential(position) + self.kinetic(momentum, params)
+        self.logpdf = self.potential
+        self.logpdf_vmap = jax.vmap(self.logpdf, in_axes=(0, None))
+        self.verbose = verbose
+        self.kernel = None
+        self.kernel_vmap = None
+        self.update = None
+        self.update_vmap = None
+        self.sampler = None
+
+    def get_initial_hamiltonian(self, rng_key: jax.random.PRNGKey, position: jnp.array,
+                                data: jnp.array,
+                                params: dict):
+        """
+        Compute the value of the Hamiltonian from positions with initial momentum draw
+        at random from the standard normal distribution.
+        """
+        
+        momentum = jax.random.normal(rng_key, shape=position.shape) * params['inverse_metric'] **-0.5
+        return self.potential(position, data) + self.kinetic(momentum, params)
 
     def make_kernel(self, return_aux = False) -> Callable:
         """
-
         Making HMC kernel for a single step
-
         """
 
-        def leapfrog_kernal(carry, data):
-            position, momentum, params = carry
+        def leapfrog_kernel(carry, extras):
+            position, momentum, params, data = carry
             position = position + params['step_size'] * self.grad_kinetic(momentum, params)
-            momentum = momentum - params['step_size'] * self.grad_potential(position)
-            return (position, momentum, params), data
+            momentum = momentum - params['step_size'] * self.grad_potential(position, data)
+            return (position, momentum, params, data), extras
 
 
-        def leapfrog_step(position, momentum, params: dict):
-            momentum = momentum - 0.5 * params['step_size'] * self.grad_potential(position)
-            (position, momentum, params), _ = jax.lax.scan(leapfrog_kernal, (position, momentum, params), jnp.arange(self.n_leapfrog-1))
+        def leapfrog_step(position, momentum, data, params: dict):
+            momentum = momentum - 0.5 * params['step_size'] * self.grad_potential(position, data)
+            (position, momentum, params, data), _ = jax.lax.scan(leapfrog_kernel, (position, momentum, params, data), jnp.arange(self.n_leapfrog-1))
             position = position + params['step_size'] * self.grad_kinetic(momentum, params)
-            momentum = momentum - 0.5*params['step_size'] * self.grad_potential(position)
+            momentum = momentum - 0.5*params['step_size'] * self.grad_potential(position, data)
             return position, momentum
 
-        def hmc_kernel(rng_key, position, H, params: dict):
+        def hmc_kernel(rng_key, position, PE, data, params: dict):
             """
-
-            Note that since the potential function is the negative log likelihood, hamiltonian is going down, but the likelihood value should go up.
+            Note that since the potential function is the negative log likelihood, 
+            hamiltonian is going down, but the likelihood value should go up.
 
             Args:
-            rng_key (n_chains, 2): random key
-            position (n_chains, n_dim): current position
-            H (n_chains, ): Hamiltonian of the current position
+                rng_key (n_chains, 2): random key
+                position (n_chains, n_dim): current position
+                PE (n_chains, ): Potential energy of the current position
             """
             key1, key2 = jax.random.split(rng_key)
 
-            momentum = jax.random.normal(key1, shape=position.shape) * params['inverse_metric']
-            proposed_position, proposed_momentum = leapfrog_step(position, momentum, params)
-            proposed_ham = self.potential(proposed_position) + self.kinetic(proposed_momentum, params)
+            momentum = jax.random.normal(key1, shape=position.shape) * params['inverse_metric']**-0.5
+            H = PE + self.kinetic(momentum, params)
+            proposed_position, proposed_momentum = leapfrog_step(position, momentum, data, params)
+            proposed_PE = self.potential(proposed_position, data)
+            proposed_ham = proposed_PE + self.kinetic(proposed_momentum, params)
             log_acc = H - proposed_ham
             log_uniform = jnp.log(jax.random.uniform(key2))
 
             do_accept = log_uniform < log_acc
 
             position = jnp.where(do_accept, proposed_position, position)
-            log_prob = jnp.where(do_accept, proposed_ham, H)
+            log_prob = jnp.where(do_accept, proposed_PE, PE)
 
             return position, log_prob, do_accept
         
         if return_aux == False:
             return hmc_kernel
         else:
-            return hmc_kernel, leapfrog_kernal, leapfrog_step
+            return hmc_kernel, leapfrog_kernel, leapfrog_step
             
 
     def make_update(self) -> Callable:
         """
-        
         Making HMC update function for multiple steps
-
         """
 
-        hmc_kernel = self.make_kernel()
+        if self.kernel is None:
+            raise ValueError("Kernel not defined. Please run make_kernel first.")
 
         def hmc_update(i, state):
-            key, positions, log_Ham, acceptance, params = state
+            key, positions, PE, acceptance, data, params = state
             _, key = jax.random.split(key)
-            new_position, new_log_Ham, do_accept = hmc_kernel(
-                key, positions[i - 1], log_Ham[i - 1], params
+            new_position, new_PE, do_accept = self.kernel(
+                key, positions[i - 1], PE[i - 1], data, params
             )
             positions = positions.at[i].set(new_position)
-            log_Ham = log_Ham.at[i].set(new_log_Ham)
+            PE = PE.at[i].set(new_PE)
             acceptance = acceptance.at[i].set(do_accept)
-            return (key, positions, log_Ham, acceptance, params)
+            return (key, positions, PE, acceptance, data, params)
 
         return hmc_update
 
     def make_sampler(self) -> Callable:
-        hmc_update = self.make_update()
-
-        if self.jit:
-            hmc_update = jax.jit(hmc_update)
+        """
+        Making HMC sampler function for multiple chains from initial positions
+        """
 
-        hmc_update = jax.vmap(hmc_update, in_axes = (None, (0, 0, 0, 0, None)), out_axes=(0, 0, 0, 0, None))
-        lh = jax.vmap(self.get_initial_hamiltonian, in_axes=(0, 0, None))
+        if self.update is None:
+            raise ValueError("Update function not defined. Please run make_update first.")
 
-        def hmc_sampler(rng_key, n_steps, initial_position):
+        def hmc_sampler(rng_key, n_steps, initial_position, data):
             
             keys = jax.vmap(jax.random.split)(rng_key)
             rng_key = keys[:, 0]
             rng_init = keys[:, 1]
-            logp = lh(rng_init,initial_position, self.params)
+            logp = self.logpdf_vmap(initial_position, data)
             n_chains = rng_key.shape[0]
             acceptance = jnp.zeros(
                 (
                     n_chains,
                     n_steps
                 )
             )
@@ -145,30 +167,29 @@
                     (
                         n_chains,
                         n_steps,
                     )
                 )
                 + logp[:, None]
             )
-            state = (rng_key, all_positions, all_logp, acceptance, self.params)
-            for i in tqdm(
-                range(1, n_steps), desc="Sampling Locally", miniters=int(n_steps / 10)
-            ):
-                state = hmc_update(i, state)
-            return state[:-1]
+            state = (rng_key, all_positions, all_logp, acceptance, data, self.params)
+
+            if self.verbose:
+                iterator_loop = tqdm(range(1, n_steps), desc="Sampling Locally", miniters=int(n_steps / 10))
+            else:
+                iterator_loop = range(1, n_steps)
+
+            for i in iterator_loop:
+                state = self.update_vmap(i, state)
+
+            state = (state[0], state[1], -state[2], state[3])
+            return state
 
         return hmc_sampler
 
     def make_leapforg_kernel(self):
-        def leapfrog_kernal(carry, data):
-            position, momentum, params = carry
+        def leapfrog_kernel(carry, extras):
+            position, momentum, params, data = carry
             position = position + self.step_size * self.grad_kinetic(momentum, params)
-            momentum = momentum - self.step_size * self.grad_potential(position)
+            momentum = momentum - self.step_size * self.grad_potential(position, data)
             return position, momentum
-        return leapfrog_kernal
-
-
-
-
-
-from tqdm import tqdm
-from functools import partialmethod
+        return leapfrog_kernel
```

### Comparing `flowMC-0.0.9/src/flowMC/sampler/MALA.py` & `flowMC-0.2.0/src/flowMC/sampler/mMALA.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,142 +1,169 @@
-from typing import Callable
 import jax
 import jax.numpy as jnp
 from jax.scipy.stats import multivariate_normal
 from tqdm import tqdm
-from flowMC.sampler.LocalSampler_Base import LocalSamplerBase
 
 
-class MALA(LocalSamplerBase):
+def make_mMALA_kernel(logpdf, d_logpdf, d2_logpdf, dt):
+    def mMALA_kernel(rng_key, position, log_prob):
 
-    def __init__(self, logpdf: Callable, jit: bool, params: dict) -> Callable:
-        super().__init__(logpdf, jit, params)
-        self.params = params
-        self.logpdf = logpdf
-
-    def make_kernel(self, return_aux = False) -> Callable:
         """
-        Make a MALA kernel for a given logpdf.
+        Metropolis-adjusted Langevin algorithm kernel.
+        This function make a proposal and accept/reject it.
 
-        Parameters
-        ----------
-        logpdf : Callable
-            The logpdf of the target distribution.
-
-        Returns
-        -------
-        Callable
-            A MALA kernel.
+        Args:
+            rng_key (n_chains, 2): random key
+            logpdf (function) : log-density function
+            d_logpdf (function): gradient of log-density function
+            position (n_chains, n_dim): current position
+            log_prob (n_chains, ): log-probability of the current position
+            dt (float): step size of the MALA step
+
+        Returns:
+            position (n_chains, n_dim): the new poisiton of the chain
+            log_prob (n_chains, ): the log-probability of the new position
+            do_accept (n_chains, ): whether to accept the new position
 
         """
-        def body(carry, this_key):
-            this_position, dt = carry
-            dt2 = dt*dt
-            this_log_prob, this_d_log = jax.value_and_grad(self.logpdf)(this_position)
-            proposal = this_position + jnp.dot(dt2, this_d_log) / 2
-            proposal += jnp.dot(dt, jax.random.normal(this_key, shape=this_position.shape))
-            return (proposal,dt), (proposal, this_log_prob, this_d_log)
-
-        def mala_kernel(rng_key, position, log_prob, params = {"step_size": 0.1}):
-
-            """
-            Metropolis-adjusted Langevin algorithm kernel.
-            This function make a proposal and accept/reject it.
-
-            Args:
-                rng_key (n_chains, 2): random key
-                position (n_chains, n_dim): current position
-                log_prob (n_chains, ): log-probability of the current position
-
-            Returns:
-                position (n_chains, n_dim): the new poisiton of the chain
-                log_prob (n_chains, ): the log-probability of the new position
-                do_accept (n_chains, ): whether to accept the new position
+        key1, key2 = jax.random.split(rng_key)
 
-            """
-            key1, key2 = jax.random.split(rng_key)
+        n_dim = position.shape[-1]
+        d_log_current = d_logpdf(position)
+        d2_current = d2_logpdf(position)
+        d2_current = jax.lax.cond(
+            jnp.any(jnp.isnan(d2_current)), lambda: jnp.eye(n_dim), lambda: d2_current
+        )
+        d2_current = jnp.linalg.inv(d2_current)
+
+        dt_current_sqrt = dt * jnp.sqrt(d2_current)
+
+        proposal = position + jnp.dot((dt * d2_current) ** 2, d_log_current) / 2
+        proposal += jnp.dot(
+            dt_current_sqrt, jax.random.normal(key1, shape=position.shape)
+        )
+        proposal_log_prob = logpdf(proposal)
+        d2_proposal = d2_logpdf(proposal)
+        d2_proposal = jax.lax.cond(
+            jnp.any(jnp.isnan(d2_proposal)), lambda: jnp.eye(n_dim), lambda: d2_proposal
+        )
+        d2_proposal = jnp.linalg.inv(d2_proposal)
+
+        ratio = proposal_log_prob - logpdf(position)
+        ratio -= multivariate_normal.logpdf(
+            position,
+            proposal + jnp.dot(d2_proposal * dt * dt, d_logpdf(proposal)) / 2,
+            d2_proposal * dt * dt,
+        )
+        ratio += multivariate_normal.logpdf(
+            proposal,
+            position + jnp.dot(d2_current * dt * dt, d_log_current) / 2,
+            d2_current * dt * dt,
+        )
+
+        log_uniform = jnp.log(jax.random.uniform(key2))
+        do_accept = log_uniform < ratio
+
+        position = jnp.where(do_accept, proposal, position)
+        log_prob = jnp.where(do_accept, proposal_log_prob, log_prob)
+        return position, log_prob, do_accept
+
+    return mMALA_kernel
+
+
+def make_mMALA_update(logpdf, d_logpdf, d2_logpdf, dt):
+    mMALA_kernel = make_mMALA_kernel(logpdf, d_logpdf, d2_logpdf, dt)
+
+    def mMALA_update(i, state):
+        key, positions, log_prob, acceptance = state
+        _, key = jax.random.split(key)
+        new_position, new_log_prob, do_accept = mMALA_kernel(
+            key, positions[i - 1], log_prob[i - 1]
+        )
+        positions = positions.at[i].set(new_position)
+        log_prob = log_prob.at[i].set(new_log_prob)
+        acceptance = acceptance.at[i].set(do_accept)
+        return (key, positions, log_prob, acceptance)
+
+    mMALA_update = jax.vmap(mMALA_update, in_axes=(None, (0, 0, 0, 0)))
+    mMALA_kernel_vec = jax.vmap(mMALA_kernel, in_axes=(0, 0, 0))
+    logpdf = jax.vmap(logpdf)
+    d_logpdf = jax.vmap(d_logpdf)
+
+    # Apperantly jitting after vmap will make compilation much slower.
+    # Output the kernel, logpdf, and dlogpdf for warmup jitting.
+    # Apperantly passing in a warmed up function will still trigger recompilation.
+    # so the warmup need to be done with the output function
+
+    return mMALA_update, mMALA_kernel_vec, logpdf, d_logpdf
+
+
+def make_MALA_sampler(logpdf, dt=1e-5, jit=False):
+
+    d_logpdf = jax.grad(logpdf)
+    d2_logpdf = jax.hessian(logpdf)
+    mMALA_update, mk, lp, dlp = make_mMALA_update(logpdf, d_logpdf, d2_logpdf, dt)
+    # Somehow if I define the function inside the other function,
+    # I think it doesn't use the cache and recompile everytime.
+    if jit:
+        mMALA_update = jax.jit(mMALA_update)
+        mk = jax.jit(mk)
+        lp = jax.jit(lp)
+        dlp = jax.jit(dlp)
+        d2lp = jax.jit(d2lp)
 
-            dt = params['step_size']
-            dt2 = dt * dt
+    def mMALA_sampler(rng_key, n_steps, initial_position):
 
-            _, (proposal, logprob, d_logprob) = jax.lax.scan(
-                body, (position, dt), jnp.array([key1, key1])
-            )
+        """
+        Metropolis-adjusted Langevin algorithm sampler.
+        This function do n step with the mMALA kernel.
 
-            ratio = logprob[1] - logprob[0]
-            ratio -= multivariate_normal.logpdf(
-                proposal[0], position + jnp.dot(dt2, d_logprob[0]) / 2, dt2
+        Args:
+            rng_key (n_chains, 2): random key for the sampler
+            n_steps (int): number of local steps
+            logpdf (function): log-density function
+            d_logpdf (function): gradient of log-density function
+            initial_position (n_chains, n_dim): initial position of the chain
+            dt (float): step size of the mMALA step
+
+        Returns:
+            rng_key (n_chains, 2): random key for the sampler after the sampling
+            all_positions (n_chains, n_steps, n_dim): all the positions of the chain
+            log_probs (n_chains, ): log probability at the end of the chain
+            acceptance: acceptance rate of the chain
+        """
+
+        logp = lp(initial_position)
+        n_chains = rng_key.shape[0]
+        acceptance = jnp.zeros(
+            (
+                n_chains,
+                n_steps,
             )
-            ratio += multivariate_normal.logpdf(
-                position, proposal[0] + jnp.dot(dt2, d_logprob[1]) / 2, dt2
+        )
+        all_positions = (
+            jnp.zeros(
+                (
+                    n_chains,
+                    n_steps,
+                )
+                + initial_position.shape[-1:]
             )
+            + initial_position[:, None]
+        )
+        all_logp = (
+            jnp.zeros(
+                (
+                    n_chains,
+                    n_steps,
+                )
+            )
+            + logp[:, None]
+        )
+        state = (rng_key, all_positions, all_logp, acceptance)
+        for i in tqdm(
+            range(1, n_steps), desc="Sampling Locally", miniters=int(n_steps / 10)
+        ):
+            state = mMALA_update(i, state)
+        return state
 
-            log_uniform = jnp.log(jax.random.uniform(key2))
-            do_accept = log_uniform < ratio
-
-            position = jnp.where(do_accept, proposal[0], position)
-            log_prob = jnp.where(do_accept, logprob[1], logprob[0])
-            return position, log_prob, do_accept
-
-        return mala_kernel
-
-    def make_update(self) -> Callable:
-
-        mala_kernel = self.make_kernel()
-
-        def mala_update(i, state):
-            key, positions, log_p, acceptance, params = state
-            _, key = jax.random.split(key)
-            new_position, new_log_p, do_accept = mala_kernel(key, positions[i-1], log_p[i-1], params)
-            positions = positions.at[i].set(new_position)
-            log_p = log_p.at[i].set(new_log_p)
-            acceptance = acceptance.at[i].set(do_accept)
-            return (key, positions, log_p, acceptance, params)
-        
-        return mala_update
-
-    def make_sampler(self) -> Callable:
-        mala_update = self.make_update()
-        lp = self.logpdf
-
-        if self.jit:
-            mala_update = jax.jit(mala_update)
-            lp = jax.jit(self.logpdf)
-
-        mala_update = jax.vmap(mala_update, in_axes = (None, (0, 0, 0, 0, None)), out_axes=(0, 0, 0, 0, None))
-        lp = jax.vmap(lp)
-
-        def mala_sampler(rng_key, n_steps, initial_position):
-            logp = lp(initial_position)
-            n_chains = rng_key.shape[0]
-            acceptance = jnp.zeros((n_chains, n_steps))
-            all_positions = (jnp.zeros((n_chains, n_steps) + initial_position.shape[-1:])) + initial_position[:, None]
-            all_logp = (jnp.zeros((n_chains, n_steps)) + logp[:, None])
-            state = (rng_key, all_positions, all_logp, acceptance, self.params)
-            for i in tqdm(range(1, n_steps)):
-                state = mala_update(i, state)
-            return state[:-1]
-
-        return mala_sampler 
-
-from tqdm import tqdm
-from functools import partialmethod
-
-def mala_sampler_autotune(mala_kernel_vmap, rng_key, initial_position, log_prob, params, max_iter = 30):
-    tqdm.__init__ = partialmethod(tqdm.__init__, disable=True)
-
-    counter = 0
-    position, log_prob, do_accept = mala_kernel_vmap(rng_key, initial_position, log_prob, params)
-    acceptance_rate = jnp.mean(do_accept)
-    while (acceptance_rate < 0.3) or (acceptance_rate > 0.5):
-        if counter > max_iter:
-            print("Maximal number of iterations reached. Existing tuning with current parameters.")
-            break
-        if acceptance_rate < 0.3:
-            params['step_size'] *= 0.8
-        elif acceptance_rate > 0.5:
-            params['step_size'] *= 1.25
-        counter += 1
-        position, log_prob, do_accept = mala_kernel_vmap(rng_key, initial_position, log_prob, params)
-        acceptance_rate = jnp.mean(do_accept)
-    tqdm.__init__ = partialmethod(tqdm.__init__, disable=False)
-    return params
+    return mMALA_sampler, mMALA_update, mk, lp, dlp
```

### Comparing `flowMC-0.0.9/src/flowMC/sampler/NF_proposal.py` & `flowMC-0.2.0/src/flowMC/sampler/NF_proposal.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,60 +7,59 @@
 n_sample_max = 100000
 
 
 def nf_metropolis_kernel(
     rng_key: jax.random.PRNGKey,
     proposal_position: jnp.ndarray,
     initial_position: jnp.ndarray,
-    proposal_pdf: jnp.ndarray,
-    proposal_nf_pdf: jnp.ndarray,
-    initial_pdf: jnp.ndarray,
-    initial_nf_pdf: jnp.ndarray,
+    log_proposal_pdf: jnp.ndarray,
+    log_proposal_nf_pdf: jnp.ndarray,
+    log_initial_pdf: jnp.ndarray,
+    log_initial_nf_pdf: jnp.ndarray,
 ):
 
     """
     A one-step global sampling kernel for a given normalizing flow model.
 
     Args:
         rng_key: Jax PRNGKey.
         proposal_position: Proposed positions, shape (Ndim).
         initial_position: Initial positions, shape (Ndim).
-        proposal_pdf: Pdf value evaluate using the target function at the proposal position, shape (Ndim).
-        proposal_nf_pdf: Pdf value evaluate using the normalizing flow model at the proposal position, shape (Ndim).
-        initial_pdf: Pdf value evaluate using the target function at the initial position, shape (Ndim).
-        initial_nf_pdf: Pdf value evaluate using the normalizing flow model at the initial position, shape (Ndim).
+        log_proposal_pdf: Log-pdf value evaluate using the target function at the proposal position, shape (Ndim).
+        log_proposal_nf_pdf: Log-pdf value evaluate using the normalizing flow model at the proposal position, shape (Ndim).
+        log_initial_pdf: Log-pdf value evaluate using the target function at the initial position, shape (Ndim).
+        log_initial_nf_pdf: Log-pdf value evaluate using the normalizing flow model at the initial position, shape (Ndim).
 
     Returns:
         position: New positions, shape (Ndim).
         log_prob: Pdf value evaluate using the target function at the new position, shape (Ndim).
         log_prob_nf: Pdf value evaluate using the normalizing flow model at the new position, shape (Ndim).
         do_accept: Acceptance boolean, shape (Ndim).
     """
 
     rng_key, subkeys = random.split(rng_key, 2)
-    ratio = (proposal_pdf - initial_pdf) - (proposal_nf_pdf - initial_nf_pdf)
+    ratio = (log_proposal_pdf - log_initial_pdf) - (log_proposal_nf_pdf - log_initial_nf_pdf)
     u = jnp.log(jax.random.uniform(subkeys, ratio.shape))
     do_accept = u < ratio
     position = jnp.where(do_accept, proposal_position, initial_position)
-    log_prob = jnp.where(do_accept, proposal_pdf, initial_pdf)
-    log_prob_nf = jnp.where(do_accept, proposal_nf_pdf, initial_nf_pdf)
+    log_prob = jnp.where(do_accept, log_proposal_pdf, log_initial_pdf)
+    log_prob_nf = jnp.where(do_accept, log_proposal_nf_pdf, log_initial_nf_pdf)
     return position, log_prob, log_prob_nf, do_accept
 
 
 nf_metropolis_kernel = vmap(nf_metropolis_kernel)
 
 
 @jax.jit
 def nf_metropolis_update(i: int, state: Tuple):
-
     """
     A multistep global sampling kernel for a given normalizing flow model.
 
     Args:
-        i: Number of iteration.
+        i: Number of current iteration.
         state: A tuple containing the current state of the sampler.
 
     """
 
     (
         key,
         positions,
@@ -97,31 +96,32 @@
         log_prob_proposal,
         log_prob_nf_proposal,
         acceptance,
     )
 
 
 def make_nf_metropolis_sampler(nf_model):
-
     """
-    A function make the normalizing flow sampler for a given normalizing flow model.
+    Make the normalizing flow sampler for a given normalizing flow model 
+    for multiple steps and from multiple initial positions.
 
     Args:
         nf_model: A normalizing flow model.
         
     Returns:
         nf_metropolis_sampler: A normalizing flow sampler that has the following signature:
 
             Args:
                 rng_key: Jax PRNGKey.
                 n_steps: Number of steps.
                 nf_param: Normalizing flow parameters.
                 nf_variables: Normalizing flow variables.
                 target_pdf: Target pdf.
                 initial_position: Initial position.
+                data: Data.
 
             Returns:
                 rng_key: Current state of random key
                 all_positions: All positions of the chain
                 all_logp: Log probability of the target function at all positions
                 all_logp_nf: Log probability of the normalizing flow model at all positions
                 acceptance: Acceptance boolean
@@ -143,24 +143,24 @@
             n_samples,
             method=nf_model.sample,
         )
 
     sample_nf = jax.jit(sample_nf, static_argnums=(1))
 
     def nf_metropolis_sampler(
-        rng_key, n_steps, nf_param, nf_variables, target_pdf, initial_position
+        rng_key, n_steps, nf_param, nf_variables, target_pdf, initial_position, data
     ):
         rng_key, *subkeys = random.split(rng_key, 3)
 
         total_sample = initial_position.shape[0] * n_steps
 
         log_pdf_nf_initial = eval_nf_logprob(
             initial_position, nf_param, nf_variables
         )
-        log_pdf_initial = target_pdf(initial_position)
+        log_pdf_initial = target_pdf(initial_position, data)
 
         if total_sample > n_sample_max:
             proposal_position = jnp.zeros((total_sample, initial_position.shape[-1]))
             log_pdf_nf_proposal = jnp.zeros((total_sample,))
             log_pdf_proposal = jnp.zeros((total_sample,))
             local_key, subkey = random.split(subkeys[0], 2)
             for i in tqdm(
@@ -173,25 +173,25 @@
                     i * n_sample_max : (i + 1) * n_sample_max
                 ].set(local_samples)
                 log_pdf_nf_proposal = log_pdf_nf_proposal.at[
                     i * n_sample_max : (i + 1) * n_sample_max
                 ].set(eval_nf_logprob(local_samples, nf_param, nf_variables))
                 log_pdf_proposal = log_pdf_proposal.at[
                     i * n_sample_max : (i + 1) * n_sample_max
-                ].set(target_pdf(local_samples))
+                ].set(target_pdf(local_samples, data))
                 local_key, subkey = random.split(local_key, 2)
 
         else:
             proposal_position = sample_nf(
                 subkeys[0], total_sample, nf_param, nf_variables
             )
             log_pdf_nf_proposal = eval_nf_logprob(
                 proposal_position, nf_param, nf_variables
             )
-            log_pdf_proposal = target_pdf(proposal_position)
+            log_pdf_proposal = target_pdf(proposal_position, data)
 
         proposal_position = proposal_position.reshape(
             n_steps, initial_position.shape[0], initial_position.shape[1]
         )
         log_pdf_nf_proposal = log_pdf_nf_proposal.reshape(
             n_steps, initial_position.shape[0]
         )
```

### Comparing `flowMC-0.0.9/src/flowMC/sampler/Sampler.py` & `flowMC-0.2.0/src/flowMC/sampler/Sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from logging import lastResort
 from typing import Callable, Tuple
 import jax
 import jax.numpy as jnp
 import numpy as np
-from flowMC.nfmodel.utils import sample_nf, make_training_loop
+from flowMC.nfmodel.utils import sample_nf, make_training_loop, eval_nf
 from flowMC.sampler.NF_proposal import make_nf_metropolis_sampler
 from flax.training import train_state  # Useful dataclass to keep train state
 import flax
 import optax
 from flowMC.sampler.LocalSampler_Base import LocalSamplerBase
+from tqdm import tqdm
 
 
 class Sampler():
     """
     Sampler class that host configuration parameters, NF model, and local sampler
 
     Args:
@@ -34,23 +35,23 @@
         batch_size (int, optional): Batch size for the NF model. Defaults to 10.
         use_global (bool, optional): Whether to use global sampler. Defaults to True.
         logging (bool, optional): Whether to log the training process. Defaults to True.
         nf_variable (None, optional): Mean and variance variables for the NF model. Defaults to None.
         keep_quantile (float, optional): Quantile of chains to keep when training the normalizing flow model. Defaults to 0..
         local_autotune (None, optional): Auto-tune function for the local sampler. Defaults to None.
         train_thinning (int, optional): Thinning for the data used to train the normalizing flow. Defaults to 1.
-
+        model_init (dic, optional): Dictionary with keys "params" and "variables" for the NF model. Defaults to None.
     """
 
     def __init__(
         self,
         n_dim: int,
         rng_key_set: Tuple,
+        data: jnp.ndarray,
         local_sampler: LocalSamplerBase,
-        likelihood: Callable,
         nf_model: Callable,
         n_loop_training: int = 3,
         n_loop_production: int = 3,
         n_local_steps: int = 50,
         n_global_steps: int = 50,
         n_chains: int = 20,
         n_epochs: int = 30,
@@ -60,22 +61,19 @@
         batch_size: int = 10000,
         use_global: bool = True,
         logging: bool = True,
         nf_variable=None,
         keep_quantile=0,
         local_autotune=None,
         train_thinning = 1,
+        model_init = None,
     ):
         rng_key_init, rng_keys_mcmc, rng_keys_nf, init_rng_keys_nf = rng_key_set
 
-        self.likelihood = likelihood
-        self.likelihood_vec = jax.jit(jax.vmap(self.likelihood))
-        self.local_sampler_class = local_sampler
-        self.local_sampler = local_sampler.make_sampler()
-        self.local_autotune = local_autotune
+        # Copying input into the model
 
         self.rng_keys_nf = rng_keys_nf
         self.rng_keys_mcmc = rng_keys_mcmc
         self.n_dim = n_dim
         self.n_loop_training = n_loop_training
         self.n_loop_production = n_loop_production
         self.n_local_steps = n_local_steps
@@ -84,39 +82,43 @@
         self.n_epochs = n_epochs
         self.learning_rate = learning_rate
         self.max_samples = max_samples
         self.momentum = momentum
         self.batch_size = batch_size
         self.use_global = use_global
         self.logging = logging
+        self.keep_quantile = keep_quantile
+        self.train_thinning = train_thinning
+
+        # Initialized local and global samplers
 
+        self.local_sampler_class = local_sampler
+        self.local_sampler_class.precompilation(n_chains=n_chains, n_dims=n_dim, n_step=n_local_steps, data=data)
+        self.local_sampler = self.local_sampler_class.sampler
 
+        self.local_autotune = local_autotune
+        self.likelihood_vec = self.local_sampler_class.logpdf_vmap
         self.nf_model = nf_model
-        model_init = nf_model.init(init_rng_keys_nf, jnp.ones((1, self.n_dim)))
+        if model_init is None:
+            model_init = nf_model.init(init_rng_keys_nf, jnp.ones((1, self.n_dim)))
         params = model_init["params"]
         self.variables = model_init["variables"]
         if nf_variable is not None:
             self.variables = self.variables
-
-        self.keep_quantile = keep_quantile
-        self.train_thinning = train_thinning
+        self.global_sampler = make_nf_metropolis_sampler(self.nf_model)
+        
         self.nf_training_loop, train_epoch, train_step = make_training_loop(
             self.nf_model
         )
-        self.global_sampler = make_nf_metropolis_sampler(self.nf_model)
-
         tx = optax.adam(self.learning_rate, self.momentum)
-        # tx = optax.chain(
-        #     optax.adaptive_grad_clip(1, eps=0.001),
-        #     optax.adam(self.learning_rate, self.momentum)
-        # )
         self.state = train_state.TrainState.create(
             apply_fn=nf_model.apply, params=params, tx=tx
         )
 
+        # Initialized result dictionary
         training = {}
         training["chains"] = jnp.empty((self.n_chains, 0, self.n_dim))
         training["log_prob"] = jnp.empty((self.n_chains, 0))
         training["local_accs"] = jnp.empty((self.n_chains, 0))
         training["global_accs"] = jnp.empty((self.n_chains, 0))
         training["loss_vals"] = jnp.empty((0, self.n_epochs))
 
@@ -126,15 +128,15 @@
         production["local_accs"] = jnp.empty((self.n_chains, 0))
         production["global_accs"] = jnp.empty((self.n_chains, 0))
 
         self.summary = {}
         self.summary['training'] = training
         self.summary['production'] = production
 
-    def sample(self, initial_position):
+    def sample(self, initial_position, data):
         """
         Sample from the posterior using the local sampler.
 
         Args:
             initial_position (Device Array): Initial position.
 
         Returns:
@@ -144,42 +146,41 @@
             global_accs (Device Array): (n_chains, n_global_steps * n_loop)
             loss_vals (Device Array): (n_epoch * n_loop,)
         """
 
         # Note that auto-tune function needs to have the same number of steps
         # as the actual sampling loop to avoid recompilation.
 
-        self.local_sampler_tuning(initial_position)
+        self.local_sampler_tuning(initial_position, data)
         last_step = initial_position
         if self.use_global == True:
-            last_step = self.global_sampler_tuning(last_step)
+            last_step = self.global_sampler_tuning(last_step, data)
 
-        last_step = self.production_run(last_step)
+        last_step = self.production_run(last_step, data)
 
-    def sampling_loop(self, initial_position: jnp.array, training=False) -> jnp.array:
+    def sampling_loop(self, initial_position: jnp.array, data: jnp.array, training=False) -> jnp.array:
         """
         One sampling loop that iterate through the local sampler and potentially the global sampler.
         If training is set to True, the loop will also train the normalizing flow model.
 
         Args:
             initial_position (jnp.array): Initial position. Shape (n_chains, n_dim)
             training (bool, optional): Whether to train the normalizing flow model. Defaults to False.
 
         Returns:
             chains (jnp.array): Samples from the posterior. Shape (n_chains, n_local_steps + n_global_steps, n_dim)
-
         """
 
         if training == True:
             summary_mode = 'training'
         else:
             summary_mode = 'production'
 
         self.rng_keys_mcmc, positions, log_prob, local_acceptance = self.local_sampler(
-            self.rng_keys_mcmc, self.n_local_steps, initial_position
+            self.rng_keys_mcmc, self.n_local_steps, initial_position, data
         )
 
         self.summary[summary_mode]['chains'] = jnp.append(
             self.summary[summary_mode]['chains'], positions, axis=1
         )
         self.summary[summary_mode]['log_prob'] = jnp.append(
             self.summary[summary_mode]['log_prob'], log_prob, axis=1
@@ -239,14 +240,15 @@
             ) = self.global_sampler(
                 self.rng_keys_nf,
                 self.n_global_steps,
                 self.state.params,
                 self.variables,
                 self.likelihood_vec,
                 positions[:, -1],
+                data,
             )
 
             self.summary[summary_mode]['chains'] = jnp.append(
                 self.summary[summary_mode]['chains'], nf_chain, axis=1
             )
             self.summary[summary_mode]['log_prob'] = jnp.append(
                 self.summary[summary_mode]['log_prob'], log_prob, axis=1
@@ -256,65 +258,75 @@
                 self.summary[summary_mode]['global_accs'], global_acceptance[:,1:], axis=1
             )
 
         last_step = self.summary[summary_mode]['chains'][:, -1]
 
         return last_step
 
-    def local_sampler_tuning(self, initial_position: jnp.array, max_iter: int = 100):
+    def local_sampler_tuning(self, initial_position: jnp.array, data: jnp.array, max_iter: int = 100):
         """
         Tuning the local sampler. This runs a number of iterations of the local sampler,
         and then uses the acceptance rate to adjust the local sampler parameters.
         Since this is mostly for a fast adaptation, we do not carry the sample state forward.
         Instead, we only adapt the sampler parameters using the initial position.
 
         Args:
             n_steps (int): Number of steps to run the local sampler.
             initial_position (Device Array): Initial position for the local sampler.
             max_iter (int): Number of iterations to run the local sampler.
         """
         if self.local_autotune is not None:
             print("Autotune found, start tuning sampler_params")
-            kernel_vmap = jax.vmap(self.local_sampler_class.make_kernel(), in_axes = (0, 0, 0,  None), out_axes=(0, 0, 0))
-            self.local_sampler_class.params = self.local_autotune(
-                kernel_vmap, self.rng_keys_mcmc, initial_position, self.likelihood_vec(initial_position), self.local_sampler_class.params, max_iter)
-            self.local_sampler = self.local_sampler_class.make_sampler()
+            kernel_vmap = self.local_sampler.kernel_vmap
+            self.local_sampler.params = self.local_autotune(
+                kernel_vmap, self.rng_keys_mcmc, initial_position, self.likelihood_vec(initial_position), data, self.local_sampler.params, max_iter)
+            self.local_sampler = self.local_sampler.make_sampler()
 
         else:
             print("No autotune found, use input sampler_params")
 
-    def global_sampler_tuning(self, initial_position: jnp.ndarray) -> jnp.array:
+    def global_sampler_tuning(self, initial_position: jnp.ndarray, data: jnp.array) -> jnp.array:
         """
         Tuning the global sampler. This runs both the local sampler and the global sampler,
         and train the normalizing flow on the run.
         To adapt the normalizing flow, we need to keep certain amount of the data generated during the sampling.
-        The data is stored in the summary dictionary.
+        The data is stored in the summary dictionary and can be accessed through the `get_sampler_state` method.
+        This tuning run is meant to be followed by a production run as defined below.
 
         Args:
             initial_position (Device Array): Initial position for the sampler, shape (n_chains, n_dim)
 
         """
         print("Training normalizing flow")
         last_step = initial_position
-        for _ in range(self.n_loop_training):
-            last_step = self.sampling_loop(last_step, training=True)
+        for _ in tqdm(
+                range(self.n_loop_training),
+                desc="Tuning global sampler",
+                ):
+            last_step = self.sampling_loop(last_step, data, training=True)
         return last_step
 
-    def production_run(self, initial_position: jnp.ndarray) -> jnp.array:
+    def production_run(self, initial_position: jnp.ndarray, data: jnp.array) -> jnp.array:
         """
         Sampling procedure that produce the final set of samples.
         The main difference between this and the global tuning step is
-        we do not train the normalizing flow in order to main detail balance.
-        The data is stored in the summary dictionary.
+        we do not train the normalizing flow, omitting training allows to maintain detail balance.
+        The data is stored in the summary dictionary and can be accessed through the `get_sampler_state` method.
+
+        Args:
+            initial_position (Device Array): Initial position for the sampler, shape (n_chains, n_dim)
         
         """
         print("Starting Production run")
         last_step = initial_position
-        for _ in range(self.n_loop_production):
-            last_step = self.sampling_loop(last_step)
+        for _ in tqdm(
+                range(self.n_loop_production),
+                desc="Production run",
+                ):
+            last_step = self.sampling_loop(last_step, data)
         return last_step
 
     def get_sampler_state(self, training: bool=False) -> dict:
         """
         Get the sampler state. There are two sets of sampler outputs one can get,
         the training set and the production set.
         The training set is produced during the global tuning step, and the production set
@@ -329,15 +341,14 @@
         if training == True:
             return self.summary['training']
         else:
             return self.summary['production']
 
     def sample_flow(self, n_samples: int) -> jnp.ndarray:
         """
-
         Sample from the normalizing flow.
 
         Args:
             n_samples (int): Number of samples to generate.
 
         Returns:
             Device Array: Samples generated using the normalizing flow.
@@ -348,14 +359,32 @@
             self.state.params,
             self.rng_keys_nf,
             n_samples,
             self.variables,
         )
         return nf_samples
 
+    def evalulate_flow(self, samples: jnp.ndarray) -> jnp.ndarray:
+        """
+        Evaluate the log probability of the normalizing flow.
+
+        Args:
+            samples (Device Array): Samples to evaluate.
+
+        Returns:
+            Device Array: Log probability of the samples.
+        """
+        log_prob = eval_nf(
+            self.nf_model,
+            self.state.params,
+            samples,
+            self.variables,
+        )
+        return log_prob
+
     def reset(self):
         """
         Reset the sampler state.
 
         """
         training = {}
         training["chains"] = jnp.empty((self.n_chains, 0, self.n_dim))
```

### Comparing `flowMC-0.0.9/src/flowMC/utils/PRNG_keys.py` & `flowMC-0.2.0/src/flowMC/utils/PRNG_keys.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.9/src/flowMC/utils/PythonFunctionWrap.py` & `flowMC-0.2.0/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.0.9/src/flowMC.egg-info/SOURCES.txt` & `flowMC-0.2.0/src/flowMC.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,27 +5,22 @@
 src/flowMC/__init__.py
 src/flowMC.egg-info/PKG-INFO
 src/flowMC.egg-info/SOURCES.txt
 src/flowMC.egg-info/dependency_links.txt
 src/flowMC.egg-info/requires.txt
 src/flowMC.egg-info/top_level.txt
 src/flowMC/nfmodel/__init__.py
+src/flowMC/nfmodel/mlp.py
 src/flowMC/nfmodel/realNVP.py
 src/flowMC/nfmodel/rqSpline.py
 src/flowMC/nfmodel/utils.py
 src/flowMC/sampler/Gaussian_random_walk.py
 src/flowMC/sampler/HMC.py
 src/flowMC/sampler/LocalSampler_Base.py
 src/flowMC/sampler/MALA.py
 src/flowMC/sampler/NF_proposal.py
 src/flowMC/sampler/Sampler.py
 src/flowMC/sampler/__init__.py
 src/flowMC/sampler/mMALA.py
 src/flowMC/utils/PRNG_keys.py
 src/flowMC/utils/PythonFunctionWrap.py
-src/flowMC/utils/__init__.py
-src/flowMC/utils/progressBar.py
-test/test_HMC.py
-test/test_MALA.py
-test/test_RWMCMC.py
-test/test_normalizingFlow.py
-test/test_quickstart.py
+src/flowMC/utils/__init__.py
```

