# Comparing `tmp/pytorch_mppi-0.6.0.tar.gz` & `tmp/pytorch_mppi-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_mppi-0.6.0.tar", last modified: Fri Feb 24 23:09:56 2023, max compression
+gzip compressed data, was "pytorch_mppi-0.7.0.tar", last modified: Tue May  9 01:40:03 2023, max compression
```

## Comparing `pytorch_mppi-0.6.0.tar` & `pytorch_mppi-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-02-24 23:09:56.172549 pytorch_mppi-0.6.0/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 pytorch_mppi-0.6.0/LICENSE.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    13554 2023-02-24 23:09:56.172549 pytorch_mppi-0.6.0/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    11482 2023-02-24 23:09:24.000000 pytorch_mppi-0.6.0/README.md
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4321 2023-02-24 23:09:24.000000 pytorch_mppi-0.6.0/pyproject.toml
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-02-24 23:09:56.172549 pytorch_mppi-0.6.0/setup.cfg
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-02-24 23:09:56.172549 pytorch_mppi-0.6.0/src/
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-02-24 23:09:56.172549 pytorch_mppi-0.6.0/src/pytorch_mppi/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       35 2023-02-10 05:03:49.000000 pytorch_mppi-0.6.0/src/pytorch_mppi/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     7817 2023-02-24 19:31:03.000000 pytorch_mppi-0.6.0/src/pytorch_mppi/autotune.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4938 2023-02-24 23:06:20.000000 pytorch_mppi-0.6.0/src/pytorch_mppi/autotune_global.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3676 2023-02-24 23:06:20.000000 pytorch_mppi-0.6.0/src/pytorch_mppi/autotune_qd.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    16379 2023-02-24 02:47:25.000000 pytorch_mppi-0.6.0/src/pytorch_mppi/mppi.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-02-24 23:09:56.172549 pytorch_mppi-0.6.0/src/pytorch_mppi.egg-info/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    13554 2023-02-24 23:09:56.000000 pytorch_mppi-0.6.0/src/pytorch_mppi.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      414 2023-02-24 23:09:56.000000 pytorch_mppi-0.6.0/src/pytorch_mppi.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-02-24 23:09:56.000000 pytorch_mppi-0.6.0/src/pytorch_mppi.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      173 2023-02-24 23:09:56.000000 pytorch_mppi-0.6.0/src/pytorch_mppi.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       13 2023-02-24 23:09:56.000000 pytorch_mppi-0.6.0/src/pytorch_mppi.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-02-24 23:09:56.172549 pytorch_mppi-0.6.0/tests/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1491 2023-02-10 04:59:55.000000 pytorch_mppi-0.6.0/tests/test_batch_wrapper.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 01:40:03.951557 pytorch_mppi-0.7.0/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 pytorch_mppi-0.7.0/LICENSE.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    14034 2023-05-09 01:40:03.951557 pytorch_mppi-0.7.0/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    11962 2023-05-09 01:39:01.000000 pytorch_mppi-0.7.0/README.md
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4321 2023-05-09 01:38:41.000000 pytorch_mppi-0.7.0/pyproject.toml
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-05-09 01:40:03.951557 pytorch_mppi-0.7.0/setup.cfg
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 01:40:03.947557 pytorch_mppi-0.7.0/src/
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 01:40:03.951557 pytorch_mppi-0.7.0/src/pytorch_mppi/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       35 2023-02-10 05:03:49.000000 pytorch_mppi-0.7.0/src/pytorch_mppi/__init__.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    10236 2023-05-09 01:30:00.000000 pytorch_mppi-0.7.0/src/pytorch_mppi/autotune.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5646 2023-05-09 01:30:00.000000 pytorch_mppi-0.7.0/src/pytorch_mppi/autotune_global.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3664 2023-05-09 01:30:00.000000 pytorch_mppi-0.7.0/src/pytorch_mppi/autotune_qd.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    16444 2023-04-19 01:21:43.000000 pytorch_mppi-0.7.0/src/pytorch_mppi/mppi.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 01:40:03.951557 pytorch_mppi-0.7.0/src/pytorch_mppi.egg-info/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    14034 2023-05-09 01:40:03.000000 pytorch_mppi-0.7.0/src/pytorch_mppi.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      414 2023-05-09 01:40:03.000000 pytorch_mppi-0.7.0/src/pytorch_mppi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-05-09 01:40:03.000000 pytorch_mppi-0.7.0/src/pytorch_mppi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      173 2023-05-09 01:40:03.000000 pytorch_mppi-0.7.0/src/pytorch_mppi.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       13 2023-05-09 01:40:03.000000 pytorch_mppi-0.7.0/src/pytorch_mppi.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 01:40:03.951557 pytorch_mppi-0.7.0/tests/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1491 2023-02-10 04:59:55.000000 pytorch_mppi-0.7.0/tests/test_batch_wrapper.py
```

### Comparing `pytorch_mppi-0.6.0/LICENSE.txt` & `pytorch_mppi-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch_mppi-0.6.0/PKG-INFO` & `pytorch_mppi-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch_mppi
-Version: 0.6.0
+Version: 0.7.0
 Summary: Model Predictive Path Integral (MPPI) implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -124,14 +124,17 @@
 from version 0.5.0 onwards, you can automatically tune the hyperparameters.
 A convenient tuner compatible with the popular [ray tune](https://docs.ray.io/en/latest/tune/index.html) library
 is implemented. You can select from a variety of cutting edge black-box optimizers such as 
 [CMA-ES](https://github.com/CMA-ES/pycma), [HyperOpt](http://hyperopt.github.io/hyperopt/),
 [fmfn/BayesianOptimization](https://github.com/fmfn/BayesianOptimization), and so on.
 See `tests/auto_tune_parameters.py` for an example. A tutorial based on it follows.
 
+The tuner can be used for other controllers as well, but you will need to define the appropriate
+`TunableParameter` subclasses.
+
 First we create a toy 2D environment to do controls on and create the controller with some
 default parameters.
 ```python
 import torch
 from pytorch_mppi import MPPI
 
 device = "cpu"
@@ -193,49 +196,55 @@
         rollouts.append(rollout)
         costs.append(this_cost)
     # can return None for rollouts if they do not need to be calculated
     return autotune.EvaluationResult(torch.stack(costs), torch.stack(rollouts))
 ```
 
 With this we have enough to start tuning. For example, we can tune iteratively with the CMA-ES optimizer
+
 ```python
-  # choose from autotune.AutotuneMPPI.TUNABLE_PARAMS
-params_to_tune = ['sigma', 'horizon', 'lambda']
+# these are subclass of TunableParameter (specifically MPPIParameter) that we want to tune
+params_to_tune = [autotune.SigmaParameter(mppi), autotune.HorizonParameter(mppi), autotune.LambdaParameter(mppi)]
 # create a tuner with a CMA-ES optimizer
-tuner = autotune.AutotuneMPPI(mppi, params_to_tune, evaluate_fn=evaluate, optimizer=autotune.CMAESOpt(sigma=1.0))
+tuner = autotune.Autotune(mppi, params_to_tune, evaluate_fn=evaluate, optimizer=autotune.CMAESOpt(sigma=1.0))
 # tune parameters for a number of iterations
 iterations = 30
 for i in range(iterations):
-    # results of this optimization step are returned
-    res = tuner.optimize_step()
-    # we can render the rollouts in the environment
-    env.draw_rollouts(res.rollouts)
+  # results of this optimization step are returned
+  res = tuner.optimize_step()
+  # we can render the rollouts in the environment
+  env.draw_rollouts(res.rollouts)
 # get best results and apply it to the controller
 # (by default the controller will take on the latest tuned parameter, which may not be best)
 res = tuner.get_best_result()
-tuner.apply_parameters(res.params)
+tuner.apply_parameters(res.param_values)
 ```
 This is a local search method that optimizes starting from the initially defined parameters.
 For global searching, we use ray tune compatible searching algorithms. Note that you can modify the
 search space of each parameter, but default reasonable ones are provided.
 
 ```python
 # can also use a Ray Tune optimizer, see
 # https://docs.ray.io/en/latest/tune/api_docs/suggestion.html#search-algorithms-tune-search
 # rather than adapting the current parameters, these optimizers allow you to define a search space for each
 # and will search on that space
 from pytorch_mppi import autotune_global
 from ray.tune.search.hyperopt import HyperOptSearch
 from ray.tune.search.bayesopt import BayesOptSearch
 
+# the global version of the parameters define a reasonable search space for each parameter
+params_to_tune = [autotune_global.SigmaGlobalParameter(mppi),
+                  autotune_global.HorizonGlobalParameter(mppi),
+                  autotune_global.LambdaGlobalParameter(mppi)]
+
 # be sure to close any figures before ray tune optimization or they will be duplicated
 env.visualize = False
 plt.close('all')
-tuner = autotune_global.AutotuneMPPIGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
-                                           optimizer=autotune_global.RayOptimizer(HyperOptSearch))
+tuner = autotune_global.AutotuneGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
+                                       optimizer=autotune_global.RayOptimizer(HyperOptSearch))
 # ray tuners cannot be tuned iteratively, but you can specify how many iterations to tune for
 res = tuner.optimize_all(100)
 res = tuner.get_best_result()
 tuner.apply_parameters(res.params)
 ```
 
 For example tuning hyperparameters (with CMA-ES) only on the toy problem (the nominal trajectory is reset each time so they are sampling from noise):
@@ -263,29 +272,30 @@
 for top results while checking for diversity.
 To use it, you need to install
 ```python
 pip install ribs
 ```
 
 You then use it as
+
 ```python
 import pytorch_mppi.autotune_qd
 
 optim = pytorch_mppi.autotune_qd.CMAMEOpt()
-tuner = autotune_global.AutotuneMPPIGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
-                                           optimizer=optim)
+tuner = autotune_global.AutotuneGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
+                                       optimizer=optim)
 
 iterations = 10
 for i in range(iterations):
-    # results of this optimization step are returned
-    res = tuner.optimize_step()
-    # we can render the rollouts in the environment
-    best_params = optim.get_diverse_top_parameters(5)
-    for res in best_params:
-        print(res)
+  # results of this optimization step are returned
+  res = tuner.optimize_step()
+  # we can render the rollouts in the environment
+  best_params = optim.get_diverse_top_parameters(5)
+  for res in best_params:
+    print(res)
 ```
 
 # Tests
 You'll need to install `gym<=0.20` to run the tests (for the `Pendulum-v0` environment).
 The easy way to install this and other testing dependencies is running `python setup.py test`.
 Note that `gym` past `0.20` deprecated `Pendulum-v0` for `Pendulum-v1` with incompatible dynamics.
```

### Comparing `pytorch_mppi-0.6.0/README.md` & `pytorch_mppi-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 from version 0.5.0 onwards, you can automatically tune the hyperparameters.
 A convenient tuner compatible with the popular [ray tune](https://docs.ray.io/en/latest/tune/index.html) library
 is implemented. You can select from a variety of cutting edge black-box optimizers such as 
 [CMA-ES](https://github.com/CMA-ES/pycma), [HyperOpt](http://hyperopt.github.io/hyperopt/),
 [fmfn/BayesianOptimization](https://github.com/fmfn/BayesianOptimization), and so on.
 See `tests/auto_tune_parameters.py` for an example. A tutorial based on it follows.
 
+The tuner can be used for other controllers as well, but you will need to define the appropriate
+`TunableParameter` subclasses.
+
 First we create a toy 2D environment to do controls on and create the controller with some
 default parameters.
 ```python
 import torch
 from pytorch_mppi import MPPI
 
 device = "cpu"
@@ -151,49 +154,55 @@
         rollouts.append(rollout)
         costs.append(this_cost)
     # can return None for rollouts if they do not need to be calculated
     return autotune.EvaluationResult(torch.stack(costs), torch.stack(rollouts))
 ```
 
 With this we have enough to start tuning. For example, we can tune iteratively with the CMA-ES optimizer
+
 ```python
-  # choose from autotune.AutotuneMPPI.TUNABLE_PARAMS
-params_to_tune = ['sigma', 'horizon', 'lambda']
+# these are subclass of TunableParameter (specifically MPPIParameter) that we want to tune
+params_to_tune = [autotune.SigmaParameter(mppi), autotune.HorizonParameter(mppi), autotune.LambdaParameter(mppi)]
 # create a tuner with a CMA-ES optimizer
-tuner = autotune.AutotuneMPPI(mppi, params_to_tune, evaluate_fn=evaluate, optimizer=autotune.CMAESOpt(sigma=1.0))
+tuner = autotune.Autotune(mppi, params_to_tune, evaluate_fn=evaluate, optimizer=autotune.CMAESOpt(sigma=1.0))
 # tune parameters for a number of iterations
 iterations = 30
 for i in range(iterations):
-    # results of this optimization step are returned
-    res = tuner.optimize_step()
-    # we can render the rollouts in the environment
-    env.draw_rollouts(res.rollouts)
+  # results of this optimization step are returned
+  res = tuner.optimize_step()
+  # we can render the rollouts in the environment
+  env.draw_rollouts(res.rollouts)
 # get best results and apply it to the controller
 # (by default the controller will take on the latest tuned parameter, which may not be best)
 res = tuner.get_best_result()
-tuner.apply_parameters(res.params)
+tuner.apply_parameters(res.param_values)
 ```
 This is a local search method that optimizes starting from the initially defined parameters.
 For global searching, we use ray tune compatible searching algorithms. Note that you can modify the
 search space of each parameter, but default reasonable ones are provided.
 
 ```python
 # can also use a Ray Tune optimizer, see
 # https://docs.ray.io/en/latest/tune/api_docs/suggestion.html#search-algorithms-tune-search
 # rather than adapting the current parameters, these optimizers allow you to define a search space for each
 # and will search on that space
 from pytorch_mppi import autotune_global
 from ray.tune.search.hyperopt import HyperOptSearch
 from ray.tune.search.bayesopt import BayesOptSearch
 
+# the global version of the parameters define a reasonable search space for each parameter
+params_to_tune = [autotune_global.SigmaGlobalParameter(mppi),
+                  autotune_global.HorizonGlobalParameter(mppi),
+                  autotune_global.LambdaGlobalParameter(mppi)]
+
 # be sure to close any figures before ray tune optimization or they will be duplicated
 env.visualize = False
 plt.close('all')
-tuner = autotune_global.AutotuneMPPIGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
-                                           optimizer=autotune_global.RayOptimizer(HyperOptSearch))
+tuner = autotune_global.AutotuneGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
+                                       optimizer=autotune_global.RayOptimizer(HyperOptSearch))
 # ray tuners cannot be tuned iteratively, but you can specify how many iterations to tune for
 res = tuner.optimize_all(100)
 res = tuner.get_best_result()
 tuner.apply_parameters(res.params)
 ```
 
 For example tuning hyperparameters (with CMA-ES) only on the toy problem (the nominal trajectory is reset each time so they are sampling from noise):
@@ -221,29 +230,30 @@
 for top results while checking for diversity.
 To use it, you need to install
 ```python
 pip install ribs
 ```
 
 You then use it as
+
 ```python
 import pytorch_mppi.autotune_qd
 
 optim = pytorch_mppi.autotune_qd.CMAMEOpt()
-tuner = autotune_global.AutotuneMPPIGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
-                                           optimizer=optim)
+tuner = autotune_global.AutotuneGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
+                                       optimizer=optim)
 
 iterations = 10
 for i in range(iterations):
-    # results of this optimization step are returned
-    res = tuner.optimize_step()
-    # we can render the rollouts in the environment
-    best_params = optim.get_diverse_top_parameters(5)
-    for res in best_params:
-        print(res)
+  # results of this optimization step are returned
+  res = tuner.optimize_step()
+  # we can render the rollouts in the environment
+  best_params = optim.get_diverse_top_parameters(5)
+  for res in best_params:
+    print(res)
 ```
 
 # Tests
 You'll need to install `gym<=0.20` to run the tests (for the `Pendulum-v0` environment).
 The easy way to install this and other testing dependencies is running `python setup.py test`.
 Note that `gym` past `0.20` deprecated `Pendulum-v0` for `Pendulum-v1` with incompatible dynamics.
```

### Comparing `pytorch_mppi-0.6.0/pyproject.toml` & `pytorch_mppi-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytorch_mppi"
-version = "0.6.0"
+version = "0.7.0"
 description = "Model Predictive Path Integral (MPPI) implemented in pytorch"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `pytorch_mppi-0.6.0/src/pytorch_mppi/autotune.py` & `pytorch_mppi-0.7.0/src/pytorch_mppi/autotune.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     params: dict = None
     # iteration number populated by the tuner after evaluation returns
     iteration: int = None
 
 
 class Optimizer:
     def __init__(self):
-        self.tuner: typing.Optional[AutotuneMPPI] = None
+        self.tuner: typing.Optional[Autotune] = None
         self.optim = None
 
     @abc.abstractmethod
     def setup_optimization(self) -> None:
         """Create backend optim object with optimization parameters and MPPI parameters from the tuner"""
 
     @abc.abstractmethod
@@ -80,37 +80,178 @@
 
         best_param = self.optim.best.x
         self.tuner.unflatten_params(best_param)
         res = self.tuner.evaluate_fn()
         return res
 
 
-class AutotuneMPPI:
-    """Tune selected MPPI hyperparameters using state-of-the-art optimizers on an evaluation function.
-    Subclass to define other parameters to optimize over such as terminal cost scaling. An example
-    evaluate_fn:
+class TunableParameter(abc.ABC):
+    """A parameter that can be tuned by the autotuner. Holds references to the object that defines its actual value."""
+
+    @staticmethod
+    @abc.abstractmethod
+    def name():
+        """Get the name of the parameter"""
+
+    @abc.abstractmethod
+    def dim(self):
+        """Get the dimension of the parameter"""
+
+    @abc.abstractmethod
+    def get_current_parameter_value(self):
+        """Get the current underlying value of the parameter"""
+
+    @abc.abstractmethod
+    def ensure_valid_value(self, value):
+        """Return a validated parameter value as close in intent as the input value as possible"""
+
+    @abc.abstractmethod
+    def apply_parameter_value(self, value):
+        """Apply the parameter value to the underlying object"""
+
+    def get_parameter_value_from_config(self, config):
+        """Get the serialized value of the parameter from a config dictionary, where each name is a scalar"""
+        return config[self.name()]
+
+    def get_config_from_parameter_value(self, value):
+        """Reverse of the above method, get a config dictionary from a parameter value"""
+        return {self.name(): value}
+
+
+class MPPIParameter(TunableParameter, abc.ABC):
+    def __init__(self, mppi: MPPI):
+        self.mppi = mppi
+        self.d = mppi.d
+        self.dtype = mppi.dtype
+
+
+class SigmaParameter(MPPIParameter):
+    eps = 0.0001
+
+    @staticmethod
+    def name():
+        return 'sigma'
+
+    def dim(self):
+        return self.mppi.nu
+
+    def get_current_parameter_value(self):
+        return torch.cat([self.mppi.noise_sigma[i][i].view(1) for i in range(self.mppi.nu)])
+
+    def ensure_valid_value(self, value):
+        sigma = ensure_tensor(self.d, self.dtype, value)
+        sigma[sigma < self.eps] = self.eps
+        return sigma
+
+    def apply_parameter_value(self, value):
+        sigma = self.ensure_valid_value(value)
+        self.mppi.noise_dist = MultivariateNormal(self.mppi.noise_mu, covariance_matrix=torch.diag(sigma))
+        self.mppi.noise_sigma_inv = torch.inverse(self.mppi.noise_sigma.detach())
+
+    def get_parameter_value_from_config(self, config):
+        return torch.tensor([config[f'{self.name()}{i}'] for i in range(self.mppi.nu)], dtype=self.dtype, device=self.d)
+
+    def get_config_from_parameter_value(self, value):
+        return {f'{self.name()}{i}': value[i].item() for i in range(self.mppi.nu)}
 
 
+class MuParameter(MPPIParameter):
+    @staticmethod
+    def name():
+        return 'mu'
+
+    def dim(self):
+        return self.mppi.nu
+
+    def get_current_parameter_value(self):
+        return self.mppi.noise_mu.clone()
+
+    def ensure_valid_value(self, value):
+        mu = ensure_tensor(self.d, self.dtype, value)
+        return mu
+
+    def apply_parameter_value(self, value):
+        mu = self.ensure_valid_value(value)
+        self.mppi.noise_dist = MultivariateNormal(mu, covariance_matrix=self.mppi.noise_sigma)
+        self.mppi.noise_sigma_inv = torch.inverse(self.mppi.noise_sigma.detach())
+
+    def get_parameter_value_from_config(self, config):
+        return torch.tensor([config[f'{self.name()}{i}'] for i in range(self.mppi.nu)], dtype=self.dtype, device=self.d)
+
+    def get_config_from_parameter_value(self, value):
+        return {f'{self.name()}{i}': value[i].item() for i in range(self.mppi.nu)}
+
+
+class LambdaParameter(MPPIParameter):
+    eps = 0.0001
+
+    @staticmethod
+    def name():
+        return 'lambda'
+
+    def dim(self):
+        return 1
+
+    def get_current_parameter_value(self):
+        return self.mppi.lambda_
+
+    def ensure_valid_value(self, value):
+        if torch.is_tensor(value) or isinstance(value, np.ndarray):
+            value = value[0]
+        v = max(value, self.eps)
+        return v
+
+    def apply_parameter_value(self, value):
+        v = self.ensure_valid_value(value)
+        self.mppi.lambda_ = v
+
+
+class HorizonParameter(MPPIParameter):
+    @staticmethod
+    def name():
+        return 'horizon'
+
+    def dim(self):
+        return 1
+
+    def get_current_parameter_value(self):
+        return self.mppi.T
+
+    def ensure_valid_value(self, value):
+        if torch.is_tensor(value) or isinstance(value, np.ndarray):
+            value = value[0]
+        v = max(round(value), 1)
+        return v
+
+    def apply_parameter_value(self, value):
+        v = self.ensure_valid_value(value)
+        self.mppi.change_horizon(v)
+
+
+class Autotune:
+    """Tune selected hyperparameters using state-of-the-art optimizers on an evaluation function.
+    Subclass to define other parameters to optimize over such as terminal cost scaling. 
+    See tests/auto_tune_parameters.py for an example evaluate_fn
     """
-    TUNABLE_PARAMS = ['sigma', 'mu', 'lambda', 'horizon']
     eps = 0.0001
 
-    def __init__(self, mppi: MPPI, params_to_tune: typing.Sequence[str],
+    def __init__(self, mppi: MPPI, params_to_tune: typing.Sequence[TunableParameter],
                  evaluate_fn: typing.Callable[[], EvaluationResult], optimizer=CMAESOpt()):
         self.mppi = mppi
         self.evaluate_fn = evaluate_fn
         self.d = mppi.d
         self.dtype = mppi.dtype
 
-        self.params = None
+        self.params = params_to_tune
+        self.param_values = None
         self.optim = optimizer
         self.optim.tuner = self
         self.results = []
 
-        self.define_parameters(params_to_tune)
+        self.get_parameter_values(self.params)
         self.optim.setup_optimization()
 
     def optimize_step(self) -> EvaluationResult:
         res = self.optim.optimize_step()
         res = self.log_current_result(res)
         return res
 
@@ -123,97 +264,47 @@
         return min(self.results, key=lambda res: res.costs.mean().item())
 
     def log_current_result(self, res: EvaluationResult):
         with torch.no_grad():
             iteration = len(self.results)
             res = res._replace(iteration=iteration,
                                params={k: v.detach().clone() if torch.is_tensor(v) else v for k, v in
-                                       self.params.items()})
-            logger.info(f"i:{iteration} cost: {res.costs.mean().item()} params:{self.params}")
+                                       self.param_values.items()})
+            logger.info(f"i:{iteration} cost: {res.costs.mean().item()} params:{self.param_values}")
             self.results.append(res)
         return res
 
-    def define_parameters(self, params_to_tune: typing.Sequence[str]):
-        pm = {}
+    def get_parameter_values(self, params_to_tune: typing.Sequence[TunableParameter]):
         # take on the assigned values to the MPPI
-        if 'sigma' in params_to_tune:
-            # we're going to require that sigma be diagonal of positive values to enforce positive definiteness
-            pm['sigma'] = torch.cat([self.mppi.noise_sigma[i][i].view(1) for i in range(self.mppi.nu)])
-        if 'mu' in params_to_tune:
-            pm['mu'] = self.mppi.noise_mu.clone()
-        if 'lambda' in params_to_tune:
-            pm['lambda'] = self.mppi.lambda_
-        if 'horizon' in params_to_tune:
-            pm['horizon'] = self.mppi.T
-        self.params = pm
+        self.param_values = {p.name(): p.get_current_parameter_value() for p in params_to_tune}
 
     def flatten_params(self):
         x = []
-        if 'sigma' in self.params:
-            x.append(self.params['sigma'].detach().cpu().numpy())
-        if 'mu' in self.params:
-            x.append(self.params['mu'].detach().cpu().numpy())
-        if 'lambda' in self.params:
-            x.append([self.params['lambda']])
-        if 'horizon' in self.params:
-            x.append([self.params['horizon']])
+        # TODO ensure this is the same order as define and unflatten
+        for k, v in self.param_values.items():
+            if torch.is_tensor(v):
+                x.append(v.detach().cpu().numpy())
+            else:
+                x.append([v])
         x = np.concatenate(x)
         return x
 
     def unflatten_params(self, x, apply=True):
         # have to be in the same order as the flattening
         params = {}
-        nu = self.mppi.nu
         i = 0
-        if 'sigma' in self.params:
-            sigma = ensure_tensor(self.d, self.dtype, x[i:i + nu])
-            sigma[sigma < self.eps] = self.eps
-            params['sigma'] = sigma
-            i += nu
-        if 'mu' in self.params:
-            mu = ensure_tensor(self.d, self.dtype, x[i:i + nu])
-            params['mu'] = mu
-            i += nu
-        if 'lambda' in self.params:
-            v = max(x[i], self.eps)
-            params['lambda'] = v
-            i += 1
-        if 'horizon' in self.params:
-            v = max(round(x[i]), 1)
-            params['horizon'] = v
-            i += 1
+        for p in self.params:
+            raw_value = x[i:i + p.dim()]
+            params[p.name()] = p.ensure_valid_value(raw_value)
+            i += p.dim()
         if apply:
             self.apply_parameters(params)
         return params
 
     def apply_parameters(self, params):
-        if 'sigma' in params:
-            # to remain positive definite
-            self.mppi.noise_dist = MultivariateNormal(self.mppi.noise_mu, covariance_matrix=torch.diag(params['sigma']))
-            self.mppi.noise_sigma_inv = torch.inverse(self.mppi.noise_sigma.detach())
-        if 'mu' in params:
-            # to remain positive definite
-            self.mppi.noise_dist = MultivariateNormal(params['mu'], covariance_matrix=self.mppi.noise_sigma)
-            self.mppi.noise_sigma_inv = torch.inverse(self.mppi.noise_sigma.detach())
-        if 'lambda' in params:
-            self.mppi.lambda_ = params['lambda']
-        if 'horizon' in params:
-            self.mppi.change_horizon(params['horizon'])
-        self.params = params
+        for p in self.params:
+            p.apply_parameter_value(params[p.name()])
+        self.param_values = params
 
     def config_to_params(self, config):
         """Configs are param dictionaries where each must be a scalar"""
-        nu = self.mppi.nu
-        p = self.params
-
-        dtype = self.dtype
-        device = self.d
-
-        params = {}
-        for name in ['sigma', 'mu']:
-            if name in p:
-                params[name] = torch.tensor([config[f'{name}{i}'] for i in range(nu)], dtype=dtype, device=device)
-        for name in ['lambda', 'horizon']:
-            if name in p:
-                params[name] = config[name]
-
-        return params
+        return {p.name(): p.get_parameter_value_from_config(config) for p in self.params}
```

### Comparing `pytorch_mppi-0.6.0/src/pytorch_mppi/autotune_qd.py` & `pytorch_mppi-0.7.0/src/pytorch_mppi/autotune_qd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 # pip install ribs
 import ribs
 
 from pytorch_mppi import autotune
-from pytorch_mppi.autotune_global import AutotuneMPPIGlobal
+from pytorch_mppi.autotune_global import AutotuneGlobal
 
 
 class CMAMEOpt(autotune.Optimizer):
     """Quality Diversity optimize using CMA-ME to find a set of good and diverse hyperparameters"""
 
     def __init__(self, population=10, sigma=1.0, bins=15):
         """
@@ -23,15 +23,15 @@
         self.archive = None
         self.qd_score_offset = -3000
         self.num_emitters = 1
         self.bins = bins
         super().__init__()
 
     def setup_optimization(self):
-        if not isinstance(self.tuner, AutotuneMPPIGlobal):
+        if not isinstance(self.tuner, AutotuneGlobal):
             raise RuntimeError(f"Quality diversity optimizers require global search space information provided "
                                f"by AutotuneMPPIGlobal")
 
         x = self.tuner.flatten_params()
         ranges = self.tuner.linearized_search_space()
         ranges = list(ranges.values())
 
@@ -47,15 +47,15 @@
             ribs.emitters.EvolutionStrategyEmitter(self.archive, x0=x, sigma0=self.sigma, batch_size=self.population,
                                                    seed=np.random.randint(0, 10000)) for i in
             range(self.num_emitters)
         ]
         self.optim = ribs.schedulers.Scheduler(self.archive, emitters)
 
     def optimize_step(self):
-        if not isinstance(self.tuner, AutotuneMPPIGlobal):
+        if not isinstance(self.tuner, AutotuneGlobal):
             raise RuntimeError(f"Quality diversity optimizers require global search space information provided "
                                f"by AutotuneMPPIGlobal")
 
         params = self.optim.ask()
         # measure is the whole hyperparameter set - we want to diverse along each dimension
 
         cost_per_param = []
```

### Comparing `pytorch_mppi-0.6.0/src/pytorch_mppi/mppi.py` & `pytorch_mppi-0.7.0/src/pytorch_mppi/mppi.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,16 +196,16 @@
         self.actions = None
 
     @handle_batch_input(n=2)
     def _dynamics(self, state, u, t):
         return self.F(state, u, t) if self.step_dependency else self.F(state, u)
 
     @handle_batch_input(n=2)
-    def _running_cost(self, state, u):
-        return self.running_cost(state, u)
+    def _running_cost(self, state, u, t):
+        return self.running_cost(state, u, t) if self.step_dependency else self.running_cost(state, u)
 
     def command(self, state, shift_nominal_trajectory=True):
         """
         :param state: (nx) or (K x nx) current state, or samples of states (for propagating a distribution of states)
         :param shift_nominal_trajectory: Whether to roll the nominal trajectory forward one step. This should be True
         if the command is to be executed. If the nominal trajectory is to be refined then it should be False.
         :returns action: (nu) best action
@@ -270,15 +270,15 @@
         state = state.repeat(self.M, 1, 1)
 
         states = []
         actions = []
         for t in range(T):
             u = self.u_scale * perturbed_actions[:, t].repeat(self.M, 1, 1)
             state = self._dynamics(state, u, t)
-            c = self._running_cost(state, u)
+            c = self._running_cost(state, u, t)
             cost_samples = cost_samples + c
             if self.M > 1:
                 cost_var += c.var(dim=0) * (self.rollout_var_discount ** t)
 
             # Save total states/actions
             states.append(state)
             actions.append(u)
@@ -348,15 +348,15 @@
             state = state.repeat(num_rollouts, 1)
 
         T = self.U.shape[0]
         states = torch.zeros((num_rollouts, T + 1, self.nx), dtype=self.U.dtype, device=self.U.device)
         states[:, 0] = state
         for t in range(T):
             states[:, t + 1] = self._dynamics(states[:, t].view(num_rollouts, -1),
-                                              self.u_scale * self.U[t].view(num_rollouts, -1), t)
+                                              self.u_scale * self.U[t].tile(num_rollouts, 1), t)
         return states[:, 1:]
 
 
 def run_mppi(mppi, env, retrain_dynamics, retrain_after_iter=50, iter=1000, render=True):
     dataset = torch.zeros((retrain_after_iter, mppi.nx + mppi.nu), dtype=mppi.U.dtype, device=mppi.d)
     total_reward = 0
     for i in range(iter):
```

### Comparing `pytorch_mppi-0.6.0/src/pytorch_mppi.egg-info/PKG-INFO` & `pytorch_mppi-0.7.0/src/pytorch_mppi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-mppi
-Version: 0.6.0
+Version: 0.7.0
 Summary: Model Predictive Path Integral (MPPI) implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -124,14 +124,17 @@
 from version 0.5.0 onwards, you can automatically tune the hyperparameters.
 A convenient tuner compatible with the popular [ray tune](https://docs.ray.io/en/latest/tune/index.html) library
 is implemented. You can select from a variety of cutting edge black-box optimizers such as 
 [CMA-ES](https://github.com/CMA-ES/pycma), [HyperOpt](http://hyperopt.github.io/hyperopt/),
 [fmfn/BayesianOptimization](https://github.com/fmfn/BayesianOptimization), and so on.
 See `tests/auto_tune_parameters.py` for an example. A tutorial based on it follows.
 
+The tuner can be used for other controllers as well, but you will need to define the appropriate
+`TunableParameter` subclasses.
+
 First we create a toy 2D environment to do controls on and create the controller with some
 default parameters.
 ```python
 import torch
 from pytorch_mppi import MPPI
 
 device = "cpu"
@@ -193,49 +196,55 @@
         rollouts.append(rollout)
         costs.append(this_cost)
     # can return None for rollouts if they do not need to be calculated
     return autotune.EvaluationResult(torch.stack(costs), torch.stack(rollouts))
 ```
 
 With this we have enough to start tuning. For example, we can tune iteratively with the CMA-ES optimizer
+
 ```python
-  # choose from autotune.AutotuneMPPI.TUNABLE_PARAMS
-params_to_tune = ['sigma', 'horizon', 'lambda']
+# these are subclass of TunableParameter (specifically MPPIParameter) that we want to tune
+params_to_tune = [autotune.SigmaParameter(mppi), autotune.HorizonParameter(mppi), autotune.LambdaParameter(mppi)]
 # create a tuner with a CMA-ES optimizer
-tuner = autotune.AutotuneMPPI(mppi, params_to_tune, evaluate_fn=evaluate, optimizer=autotune.CMAESOpt(sigma=1.0))
+tuner = autotune.Autotune(mppi, params_to_tune, evaluate_fn=evaluate, optimizer=autotune.CMAESOpt(sigma=1.0))
 # tune parameters for a number of iterations
 iterations = 30
 for i in range(iterations):
-    # results of this optimization step are returned
-    res = tuner.optimize_step()
-    # we can render the rollouts in the environment
-    env.draw_rollouts(res.rollouts)
+  # results of this optimization step are returned
+  res = tuner.optimize_step()
+  # we can render the rollouts in the environment
+  env.draw_rollouts(res.rollouts)
 # get best results and apply it to the controller
 # (by default the controller will take on the latest tuned parameter, which may not be best)
 res = tuner.get_best_result()
-tuner.apply_parameters(res.params)
+tuner.apply_parameters(res.param_values)
 ```
 This is a local search method that optimizes starting from the initially defined parameters.
 For global searching, we use ray tune compatible searching algorithms. Note that you can modify the
 search space of each parameter, but default reasonable ones are provided.
 
 ```python
 # can also use a Ray Tune optimizer, see
 # https://docs.ray.io/en/latest/tune/api_docs/suggestion.html#search-algorithms-tune-search
 # rather than adapting the current parameters, these optimizers allow you to define a search space for each
 # and will search on that space
 from pytorch_mppi import autotune_global
 from ray.tune.search.hyperopt import HyperOptSearch
 from ray.tune.search.bayesopt import BayesOptSearch
 
+# the global version of the parameters define a reasonable search space for each parameter
+params_to_tune = [autotune_global.SigmaGlobalParameter(mppi),
+                  autotune_global.HorizonGlobalParameter(mppi),
+                  autotune_global.LambdaGlobalParameter(mppi)]
+
 # be sure to close any figures before ray tune optimization or they will be duplicated
 env.visualize = False
 plt.close('all')
-tuner = autotune_global.AutotuneMPPIGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
-                                           optimizer=autotune_global.RayOptimizer(HyperOptSearch))
+tuner = autotune_global.AutotuneGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
+                                       optimizer=autotune_global.RayOptimizer(HyperOptSearch))
 # ray tuners cannot be tuned iteratively, but you can specify how many iterations to tune for
 res = tuner.optimize_all(100)
 res = tuner.get_best_result()
 tuner.apply_parameters(res.params)
 ```
 
 For example tuning hyperparameters (with CMA-ES) only on the toy problem (the nominal trajectory is reset each time so they are sampling from noise):
@@ -263,29 +272,30 @@
 for top results while checking for diversity.
 To use it, you need to install
 ```python
 pip install ribs
 ```
 
 You then use it as
+
 ```python
 import pytorch_mppi.autotune_qd
 
 optim = pytorch_mppi.autotune_qd.CMAMEOpt()
-tuner = autotune_global.AutotuneMPPIGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
-                                           optimizer=optim)
+tuner = autotune_global.AutotuneGlobal(mppi, params_to_tune, evaluate_fn=evaluate,
+                                       optimizer=optim)
 
 iterations = 10
 for i in range(iterations):
-    # results of this optimization step are returned
-    res = tuner.optimize_step()
-    # we can render the rollouts in the environment
-    best_params = optim.get_diverse_top_parameters(5)
-    for res in best_params:
-        print(res)
+  # results of this optimization step are returned
+  res = tuner.optimize_step()
+  # we can render the rollouts in the environment
+  best_params = optim.get_diverse_top_parameters(5)
+  for res in best_params:
+    print(res)
 ```
 
 # Tests
 You'll need to install `gym<=0.20` to run the tests (for the `Pendulum-v0` environment).
 The easy way to install this and other testing dependencies is running `python setup.py test`.
 Note that `gym` past `0.20` deprecated `Pendulum-v0` for `Pendulum-v1` with incompatible dynamics.
```

### Comparing `pytorch_mppi-0.6.0/tests/test_batch_wrapper.py` & `pytorch_mppi-0.7.0/tests/test_batch_wrapper.py`

 * *Files identical despite different names*

