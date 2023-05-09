# Comparing `tmp/pysfa-0.2.tar.gz` & `tmp/pysfa-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysfa-0.2.tar", last modified: Fri May  5 10:46:26 2023, max compression
+gzip compressed data, was "pysfa-0.3.tar", last modified: Tue May  9 17:01:43 2023, max compression
```

## Comparing `pysfa-0.2.tar` & `pysfa-0.3.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:46:26.458160 pysfa-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 10:46:12.000000 pysfa-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-05 10:46:26.458160 pysfa-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-05 10:46:12.000000 pysfa-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:46:26.458160 pysfa-0.2/pysfa/
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-05 10:46:12.000000 pysfa-0.2/pysfa/SFA.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 10:46:12.000000 pysfa-0.2/pysfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 10:46:12.000000 pysfa-0.2/pysfa/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:46:26.458160 pysfa-0.2/pysfa/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-05 10:46:12.000000 pysfa-0.2/pysfa/data/41Firm.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:46:26.458160 pysfa-0.2/pysfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-05 10:46:26.000000 pysfa-0.2/pysfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 10:46:26.000000 pysfa-0.2/pysfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:46:26.000000 pysfa-0.2/pysfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:46:26.000000 pysfa-0.2/pysfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 10:46:26.000000 pysfa-0.2/pysfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 10:46:26.000000 pysfa-0.2/pysfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:46:26.458160 pysfa-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-05 10:46:12.000000 pysfa-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 17:01:28.000000 pysfa-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-09 17:01:43.772496 pysfa-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-09 17:01:28.000000 pysfa-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/SFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/data/41Firm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/data/electricityFirms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:01:43.772496 pysfa-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-09 17:01:28.000000 pysfa-0.3/setup.py
```

### Comparing `pysfa-0.2/LICENSE` & `pysfa-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysfa-0.2/PKG-INFO` & `pysfa-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,68 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.2
+Version: 0.3
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
-Author: Sheng Dai
+Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Stochastic Frontier Analysis (SFA)
 
-
 ## Installation
 
 The [`pySFA`](https://pypi.org/project/pysfa/) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`pySFA`](https://github.com/gEAPA/pySFA). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI [![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/pysfa/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/pysfa)
 
     pip install pysfa
 
 #### GitHub
 
     pip install -U git+https://github.com/gEAPA/pySFA
+
+
+## Authors
+
+- [Sheng Dai](https://daisheng.io), PhD, Turku School of Economics, University of Turku, Finland.
+- [Zhiqiang Liao](https://liaozhiqiang.com), Doctoral Researcher, Aalto University School of Business, Finland.
+
+
+## Demo: Estimating a production function by `pySFA`
+
+```python
+import numpy as np
+import pandas as pd
+from pysfa import SFA
+from pysfa.dataset import load_Tim_Coelli_frontier
+
+
+# import the data from Tim Coelli Frontier 4.1
+df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
+                              y_select=['output'])
+y = np.log(df.y)
+x = np.log(df.x)
+
+# Estimate SFA model
+res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
+
+# print estimates
+print(res.get_beta())
+print(res.get_lambda())
+print(res.get_sigma2())
+print(res.get_sigmau2())
+print(res.get_sigmav2())
+
+# print TE
+print(res.get_technical_efficiency())
+```
+
```

### Comparing `pysfa-0.2/pysfa/SFA.py` & `pysfa-0.3/pysfa/SFA.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import numpy as np
 from sklearn.linear_model import LinearRegression
 from math import sqrt, pi, log
 from scipy.stats import norm
 import scipy.optimize as opt
 from .constant import FUN_PROD, FUN_COST, TE_teJ, TE_te, TE_teMod
+from .utils import tools
 
 
 class SFA:
     """Stochastic frontier analysis (SFA) 
     """
 
     def __init__(self, y, x, fun=FUN_PROD, lamda0=1, method=TE_teJ):
         """SFA model
 
           Args:
-              y (float): output variable. 
-              x (float): input variables.
+              y (float) of shape (n,): output variable. 
+              x (float) of shape (n, d): input variables.
               fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
           """
-        self.x, self.y, self.fun, self.lamda0, self.method = x, y, fun, lamda0, method
+        self.y, self.x = tools.assert_valid_basic_data(y, x, fun)
+        self.fun, self.lamda0, self.method = fun, lamda0, method
 
     def __mle(self):
 
         # initial OLS regression
         reg = LinearRegression().fit(X=self.x, y=self.y)
         beta0 = np.concatenate(([reg.intercept_], reg.coef_), axis=0)
         parm = np.concatenate((beta0, [self.lamda0]), axis=0)
 
         # Maximum Likelihood Estimation
         def __loglik(parm):
             ''' Log-likelihood function'''
-            N, K = self.x.shape[0], self.x.shape[1] + 1
+            N, K = len(self.x), len(self.x[0]) + 1
             beta0, lamda0 = parm[0:K], parm[K]
             e = self.__resfun(beta0)
             s = np.sum(e**2)/N
             z = -lamda0*e/sqrt(s)
             pz = np.maximum(norm.cdf(z), 1e-323)
             return N/2*log(pi/2) + N/2*log(s) - np.sum(np.log(pz)) + N/2.0
 
-        fit = opt.minimize(__loglik, parm, method='L-BFGS-B').x
+        fit = opt.minimize(__loglik, parm, method='BFGS').x
 
         # beta, residuals, lambda, sigma^2
-        K = self.x.shape[1] + 1
+        K = len(self.x[0]) + 1
         self.beta = fit[0:K]
         self.residuals = self.__resfun(self.beta)
         self.lamda = fit[K]
         self.sigma2 = np.sum(self.residuals ** 2)/self.residuals.shape[0]
 
         # sigma_u^2, sigma_v^2
         self.s2u = self.lamda**2 / (1+self.lamda**2) * self.sigma2
@@ -54,38 +56,47 @@
     def __resfun(self, beta):
         return self.y - beta[0] - np.dot(self.x, beta[1:])
 
     def __teJ(self):
         '''Efficiencies estimates using the conditional mean approach 
             Jondrow et al. (1982, 235)'''
 
-        self.sign = 1
+        if self.fun == FUN_COST:
+            self.sign == -1
+        else:
+            self.sign = 1
         self.ustar = - self.sign * self.residuals * \
             self.lamda**2/(1+self.lamda**2)
         self.sstar = self.lamda/(1+self.lamda**2)*sqrt(self.sigma2)
         return np.exp(-self.ustar - self.sstar *
                       (norm.pdf(self.ustar/self.sstar)/norm.cdf(self.ustar/self.sstar)))
 
     def __te(self):
         '''Efficiencies estimated by minimizing the mean square error; 
             Eq. (7.21) in Bogetoft and Otto (2011, 219) and Battese and Coelli (1988, 392)'''
 
-        self.sign = 1
+        if self.fun == FUN_COST:
+            self.sign == -1
+        else:
+            self.sign = 1
         self.ustar = - self.sign * self.residuals * \
             self.lamda**2/(1+self.lamda**2)
         self.sstar = self.lamda/(1+self.lamda**2)*sqrt(self.sigma2)
         return norm.cdf(self.ustar/self.sstar - self.sstar) / \
             norm.cdf(self.ustar/self.sstar) * \
             np.exp(self.sstar**2/2 - self.ustar)
 
     def __teMod(self):
         '''Efficiencies estimates using the conditional mode approach;
             Bogetoft and Otto (2011, 219), Jondrow et al. (1982, 235)'''
 
-        self.sign = 1
+        if self.fun == FUN_COST:
+            self.sign == -1
+        else:
+            self.sign = 1
         self.ustar = - self.sign * self.residuals * \
             self.lamda**2/(1+self.lamda**2)
         return np.exp(np.minimum(0, -self.ustar))
 
     def get_technical_efficiency(self):
         """
         Args:
@@ -97,15 +108,15 @@
         if self.method == TE_teJ:
             return self.__teJ()
         elif self.method == TE_te:
             return self.__te()
         elif self.method == TE_teMod:
             return self.__teMod()
         else:
-            raise ValueError("Undefined estimation technique.")
+            raise ValueError("Undefined decomposition technique.")
 
     def get_beta(self):
         '''Return the estimated coefficients'''
         return self.beta
 
     def get_residuals(self):
         '''Return the residuals'''
```

### Comparing `pysfa-0.2/pysfa/constant.py` & `pysfa-0.3/pysfa/constant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# Frontier
+# function
 FUN_PROD = "prod"
 """
-FUN_PROD: Production frontier.
+FUN_PROD: Production function.
 """
 
 FUN_COST = "cost"
 """
-FUN_COST: Cost frontier.
+FUN_COST: Cost function.
 """
 
 FUN_Categories = {
-    FUN_PROD: "Production frontier",
-    FUN_COST: "Cost frontier"
+    FUN_PROD: "Production function",
+    FUN_COST: "Cost function"
 }
 
 
 # Technical inefficiency
 TE_teJ = "teJ"
 """
-RED_MOM: Method of moments.
+TE_teJ: Using conditional mean approach.
 """
 
 TE_te = "te"
 """
-RED_QLE: Quassi-likelihood estimation.
+TE_te: Minimizing the mean square error.
 """
 
 TE_teMod = "teMod"
 """
-RED_KDE: Kernel deconvolution estimation.
+TE_teMod: Using conditional mode approach.
 """
 
 RED_Categories = {
-    TE_teJ: "Method of moments",
-    TE_te: "Quassi-likelihood estimation",
-    TE_teMod: "Kernel deconvolution estimation"
+    TE_teJ: "Conditional mean",
+    TE_te: "Mean square error",
+    TE_teMod: "Conditional mode"
 }
-
```

### Comparing `pysfa-0.2/pysfa/data/41Firm.csv` & `pysfa-0.3/pysfa/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.2/pysfa.egg-info/PKG-INFO` & `pysfa-0.3/pysfa.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,68 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.2
+Version: 0.3
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
-Author: Sheng Dai
+Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Stochastic Frontier Analysis (SFA)
 
-
 ## Installation
 
 The [`pySFA`](https://pypi.org/project/pysfa/) package is now avaiable on PyPI and the latest development version can be installed from the Github repository [`pySFA`](https://github.com/gEAPA/pySFA). Please feel free to download and test it. We welcome any bug reports and feedback.
 
 #### PyPI [![PyPI version](https://img.shields.io/pypi/v/pysfa.svg?maxAge=3600)](https://pypi.org/project/pysfa/)[![PyPI downloads](https://img.shields.io/pypi/dm/pysfa.svg?maxAge=21600)](https://pypistats.org/packages/pysfa)
 
     pip install pysfa
 
 #### GitHub
 
     pip install -U git+https://github.com/gEAPA/pySFA
+
+
+## Authors
+
+- [Sheng Dai](https://daisheng.io), PhD, Turku School of Economics, University of Turku, Finland.
+- [Zhiqiang Liao](https://liaozhiqiang.com), Doctoral Researcher, Aalto University School of Business, Finland.
+
+
+## Demo: Estimating a production function by `pySFA`
+
+```python
+import numpy as np
+import pandas as pd
+from pysfa import SFA
+from pysfa.dataset import load_Tim_Coelli_frontier
+
+
+# import the data from Tim Coelli Frontier 4.1
+df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
+                              y_select=['output'])
+y = np.log(df.y)
+x = np.log(df.x)
+
+# Estimate SFA model
+res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
+
+# print estimates
+print(res.get_beta())
+print(res.get_lambda())
+print(res.get_sigma2())
+print(res.get_sigmau2())
+print(res.get_sigmav2())
+
+# print TE
+print(res.get_technical_efficiency())
+```
+
```

### Comparing `pysfa-0.2/setup.py` & `pysfa-0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pysfa',
-    version='0.2',
+    version='0.3',
     description='A Python Package for Stochastic Frontier Analysis',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
-    author='Sheng Dai',
+    author='Sheng Dai, Zhiqiang Liao',
     author_email='sheng.dai@utu.fi',
     keywords=['SFA', 'MLE', 'TE'],
     url='https://github.com/gEAPA/pySFA',
     download_url='https://pypi.org/project/pysfa/',
     include_package_data=True,
     zip_safe=False,
     classifiers=[
@@ -26,13 +26,14 @@
         'Operating System :: OS Independent',
     ],
     package_data={'pysfa': ['data/*.csv']},
 )
 
 install_requires = [
     'numpy>=1.19.2',
+    'pandas>=1.1.3',
     'scipy>=1.5.2',
     'scikit-learn>=1.2.2',
 ]
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

