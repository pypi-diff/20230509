# Comparing `tmp/pysfa-0.3.tar.gz` & `tmp/pysfa-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysfa-0.3.tar", last modified: Tue May  9 17:01:43 2023, max compression
+gzip compressed data, was "pysfa-0.4.tar", last modified: Tue May  9 17:31:05 2023, max compression
```

## Comparing `pysfa-0.3.tar` & `pysfa-0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 17:01:28.000000 pysfa-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-09 17:01:43.772496 pysfa-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-09 17:01:28.000000 pysfa-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa/
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/SFA.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/data/41Firm.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/data/electricityFirms.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-09 17:01:28.000000 pysfa-0.3/pysfa/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:01:43.772496 pysfa-0.3/pysfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 17:01:43.000000 pysfa-0.3/pysfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:01:43.772496 pysfa-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-09 17:01:28.000000 pysfa-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 17:30:54.000000 pysfa-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-09 17:31:05.849717 pysfa-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-09 17:30:54.000000 pysfa-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/SFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/data/41Firm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/data/electricityFirms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:31:05.849717 pysfa-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-09 17:30:54.000000 pysfa-0.4/setup.py
```

### Comparing `pysfa-0.3/LICENSE` & `pysfa-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysfa-0.3/PKG-INFO` & `pysfa-0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.3
+Version: 0.4
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
@@ -26,21 +26,19 @@
 
     pip install pysfa
 
 #### GitHub
 
     pip install -U git+https://github.com/gEAPA/pySFA
 
-
 ## Authors
 
 - [Sheng Dai](https://daisheng.io), PhD, Turku School of Economics, University of Turku, Finland.
 - [Zhiqiang Liao](https://liaozhiqiang.com), Doctoral Researcher, Aalto University School of Business, Finland.
 
-
 ## Demo: Estimating a production function by `pySFA`
 
 ```python
 import numpy as np
 import pandas as pd
 from pysfa import SFA
 from pysfa.dataset import load_Tim_Coelli_frontier
@@ -53,16 +51,18 @@
 x = np.log(df.x)
 
 # Estimate SFA model
 res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
 
 # print estimates
 print(res.get_beta())
+print(res.get_residuals())
+
+# print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
 print(res.get_sigmau2())
 print(res.get_sigmav2())
 
 # print TE
 print(res.get_technical_efficiency())
 ```
-
```

### Comparing `pysfa-0.3/README.md` & `pysfa-0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 
     pip install pysfa
 
 #### GitHub
 
     pip install -U git+https://github.com/gEAPA/pySFA
 
-
 ## Authors
 
 - [Sheng Dai](https://daisheng.io), PhD, Turku School of Economics, University of Turku, Finland.
 - [Zhiqiang Liao](https://liaozhiqiang.com), Doctoral Researcher, Aalto University School of Business, Finland.
 
-
 ## Demo: Estimating a production function by `pySFA`
 
 ```python
 import numpy as np
 import pandas as pd
 from pysfa import SFA
 from pysfa.dataset import load_Tim_Coelli_frontier
@@ -35,16 +33,18 @@
 x = np.log(df.x)
 
 # Estimate SFA model
 res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
 
 # print estimates
 print(res.get_beta())
+print(res.get_residuals())
+
+# print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
 print(res.get_sigmau2())
 print(res.get_sigmav2())
 
 # print TE
 print(res.get_technical_efficiency())
 ```
-
```

### Comparing `pysfa-0.3/pysfa/SFA.py` & `pysfa-0.4/pysfa/SFA.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     """Stochastic frontier analysis (SFA) 
     """
 
     def __init__(self, y, x, fun=FUN_PROD, lamda0=1, method=TE_teJ):
         """SFA model
 
           Args:
-              y (float) of shape (n,): output variable. 
-              x (float) of shape (n, d): input variables.
-              fun (String, optional): FUN_PROD (production frontier) or FUN_COST (cost frontier). Defaults to FUN_PROD.
+              y (float) : output variable. 
+              x (float) : input variables.
+              fun (String, optional): FUN_PROD (production function) or FUN_COST (cost function). Defaults to FUN_PROD.
           """
         self.y, self.x = tools.assert_valid_basic_data(y, x, fun)
         self.fun, self.lamda0, self.method = fun, lamda0, method
 
     def __mle(self):
 
         # initial OLS regression
@@ -49,14 +49,16 @@
         self.lamda = fit[K]
         self.sigma2 = np.sum(self.residuals ** 2)/self.residuals.shape[0]
 
         # sigma_u^2, sigma_v^2
         self.s2u = self.lamda**2 / (1+self.lamda**2) * self.sigma2
         self.s2v = self.sigma2 / (1+self.lamda**2)
 
+        return self.beta, self.residuals, self.lamda, self.sigma2, self.s2u, self.s2v
+
     def __resfun(self, beta):
         return self.y - beta[0] - np.dot(self.x, beta[1:])
 
     def __teJ(self):
         '''Efficiencies estimates using the conditional mean approach 
             Jondrow et al. (1982, 235)'''
 
@@ -112,28 +114,28 @@
         elif self.method == TE_teMod:
             return self.__teMod()
         else:
             raise ValueError("Undefined decomposition technique.")
 
     def get_beta(self):
         '''Return the estimated coefficients'''
-        return self.beta
+        return self.__mle()[0]
 
     def get_residuals(self):
         '''Return the residuals'''
-        return self.residuals
+        return self.__mle()[1]
+
+    def get_lambda(self):
+        '''Return the lambda'''
+        return self.__mle()[2]
 
     def get_sigma2(self):
         '''Return the sigma2'''
-        return self.sigma2
+        return self.__mle()[3]
 
     def get_sigmau2(self):
         '''Return the sigma_u**2'''
-        return self.s2u
+        return self.__mle()[4]
 
     def get_sigmav2(self):
         '''Return the sigma_v**2'''
-        return self.s2v
-
-    def get_lambda(self):
-        '''Return the lambda'''
-        return self.lamda
+        return self.__mle()[5]
```

### Comparing `pysfa-0.3/pysfa/constant.py` & `pysfa-0.4/pysfa/constant.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.3/pysfa/data/41Firm.csv` & `pysfa-0.4/pysfa/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.3/pysfa/data/electricityFirms.csv` & `pysfa-0.4/pysfa/data/electricityFirms.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.3/pysfa/dataset.py` & `pysfa-0.4/pysfa/dataset.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.3/pysfa/utils/tools.py` & `pysfa-0.4/pysfa/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.3/pysfa.egg-info/PKG-INFO` & `pysfa-0.4/pysfa.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.3
+Version: 0.4
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
@@ -26,21 +26,19 @@
 
     pip install pysfa
 
 #### GitHub
 
     pip install -U git+https://github.com/gEAPA/pySFA
 
-
 ## Authors
 
 - [Sheng Dai](https://daisheng.io), PhD, Turku School of Economics, University of Turku, Finland.
 - [Zhiqiang Liao](https://liaozhiqiang.com), Doctoral Researcher, Aalto University School of Business, Finland.
 
-
 ## Demo: Estimating a production function by `pySFA`
 
 ```python
 import numpy as np
 import pandas as pd
 from pysfa import SFA
 from pysfa.dataset import load_Tim_Coelli_frontier
@@ -53,16 +51,18 @@
 x = np.log(df.x)
 
 # Estimate SFA model
 res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
 
 # print estimates
 print(res.get_beta())
+print(res.get_residuals())
+
+# print estimated parameters
 print(res.get_lambda())
 print(res.get_sigma2())
 print(res.get_sigmau2())
 print(res.get_sigmav2())
 
 # print TE
 print(res.get_technical_efficiency())
 ```
-
```

### Comparing `pysfa-0.3/setup.py` & `pysfa-0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pysfa',
-    version='0.3',
+    version='0.4',
     description='A Python Package for Stochastic Frontier Analysis',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Sheng Dai, Zhiqiang Liao',
     author_email='sheng.dai@utu.fi',
```

