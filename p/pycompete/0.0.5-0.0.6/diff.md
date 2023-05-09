# Comparing `tmp/pycompete-0.0.5.tar.gz` & `tmp/pycompete-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycompete-0.0.5.tar", last modified: Tue May  9 08:37:50 2023, max compression
+gzip compressed data, was "pycompete-0.0.6.tar", last modified: Tue May  9 08:41:30 2023, max compression
```

## Comparing `pycompete-0.0.5.tar` & `pycompete-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 08:37:37.000000 pycompete-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-09 08:37:37.000000 pycompete-0.0.5/.github/workflows/syntax.yml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-09 08:37:37.000000 pycompete-0.0.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-09 08:37:37.000000 pycompete-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 08:37:37.000000 pycompete-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 08:37:37.000000 pycompete-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-09 08:37:37.000000 pycompete-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 08:37:50.101942 pycompete-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 08:37:37.000000 pycompete-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-09 08:37:37.000000 pycompete-0.0.5/notebooks/Untitled.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/pycompete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 08:37:49.000000 pycompete-0.0.5/pycompete/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/pycompete/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/pycompete/features/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/features/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/pycompete/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-09 08:37:37.000000 pycompete-0.0.5/pycompete/model_selection/cv_splitters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/pycompete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 08:37:50.000000 pycompete-0.0.5/pycompete.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-09 08:37:37.000000 pycompete-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 08:37:37.000000 pycompete-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:37:50.101942 pycompete-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:37:37.000000 pycompete-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.097942 pycompete-0.0.5/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:37:50.101942 pycompete-0.0.5/tests/unit/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-09 08:37:37.000000 pycompete-0.0.5/tests/unit/evaluation/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.850945 pycompete-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.846945 pycompete-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.846945 pycompete-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 08:41:22.000000 pycompete-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-09 08:41:22.000000 pycompete-0.0.6/.github/workflows/syntax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-09 08:41:22.000000 pycompete-0.0.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-09 08:41:22.000000 pycompete-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 08:41:22.000000 pycompete-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 08:41:22.000000 pycompete-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-09 08:41:22.000000 pycompete-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 08:41:30.850945 pycompete-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 08:41:22.000000 pycompete-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.846945 pycompete-0.0.6/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-09 08:41:22.000000 pycompete-0.0.6/notebooks/Untitled.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.846945 pycompete-0.0.6/pycompete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:22.000000 pycompete-0.0.6/pycompete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 08:41:30.000000 pycompete-0.0.6/pycompete/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.850945 pycompete-0.0.6/pycompete/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-09 08:41:22.000000 pycompete-0.0.6/pycompete/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.850945 pycompete-0.0.6/pycompete/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-09 08:41:22.000000 pycompete-0.0.6/pycompete/features/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.850945 pycompete-0.0.6/pycompete/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-09 08:41:22.000000 pycompete-0.0.6/pycompete/model_selection/cv_splitters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.850945 pycompete-0.0.6/pycompete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 08:41:30.000000 pycompete-0.0.6/pycompete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-09 08:41:30.000000 pycompete-0.0.6/pycompete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:41:30.000000 pycompete-0.0.6/pycompete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 08:41:30.000000 pycompete-0.0.6/pycompete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 08:41:30.000000 pycompete-0.0.6/pycompete.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-09 08:41:22.000000 pycompete-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 08:41:22.000000 pycompete-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:41:30.850945 pycompete-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:41:22.000000 pycompete-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.846945 pycompete-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.846945 pycompete-0.0.6/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.850945 pycompete-0.0.6/tests/unit/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-09 08:41:22.000000 pycompete-0.0.6/tests/unit/evaluation/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:41:30.850945 pycompete-0.0.6/tests/unit/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-09 08:41:22.000000 pycompete-0.0.6/tests/unit/features/test_transformers.py
```

### Comparing `pycompete-0.0.5/.github/workflows/tests.yml` & `pycompete-0.0.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/.gitignore` & `pycompete-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/CONTRIBUTING.md` & `pycompete-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/LICENSE.txt` & `pycompete-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/PKG-INFO` & `pycompete-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompete
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools to support the training and evalaution of models for the CrunchDAO project.
 Author: Francis P Chmiel
 License: MIT license
 Keywords: crunchdao
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pycompete-0.0.5/README.md` & `pycompete-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/notebooks/Untitled.ipynb` & `pycompete-0.0.6/notebooks/Untitled.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9458333333333333%*

 * *Differences: {"'cells'": "{0: {'execution_count': 4, 'source': ['import numpy as np\\n', 'import pandas as "*

 * *            "pd']}, 7: {'execution_count': 2, 'outputs': [], 'source': ['X = "*

 * *            "np.array([[0,0.1,0.04], [0.4,0.45,-1], [0.78,0.81,2]])']}, 14: {'id': "*

 * *            "'34aa4763-8122-4c48-85a0-05bb062f022f'}, insert: [(8, OrderedDict([('cell_type', "*

 * *            "'code'), ('execution_count', 8), ('id', 'e282ab86-f8dd-4fb6-8b90-3b613f585663'), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ( […]*

```diff
@@ -1,17 +1,18 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 4,
             "id": "efff084a-f4cb-4cff-9805-9c6081ec0cc7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numpy as np"
+                "import numpy as np\n",
+                "import pandas as pd"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 15,
             "id": "c76eb5cd-a20c-4ba2-897e-d215b654eea5",
             "metadata": {},
@@ -127,37 +128,133 @@
             ],
             "source": [
                 "moons_large[np.argwhere(np.isin(moons_large, groups_in_fold))]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 43,
+            "execution_count": 2,
             "id": "96d29f7e-6dfe-4e54-ac9c-31d229a47d9b",
             "metadata": {},
+            "outputs": [],
+            "source": [
+                "X = np.array([[0,0.1,0.04], [0.4,0.45,-1], [0.78,0.81,2]])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "e282ab86-f8dd-4fb6-8b90-3b613f585663",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "upper = np.triu(pd.DataFrame(X).corr().values, k=1)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "1b3aed41-1b55-4d11-906e-b792e0259a41",
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "2"
+                            "array([[0.        , 0.99973702, 0.63192464],\n",
+                            "       [0.        , 0.        , 0.64953166],\n",
+                            "       [0.        , 0.        , 0.        ]])"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "upper"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "dcd6de75-864c-4b55-9b96-58320886a52b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "\n",
+                "corr_cols = np.argwhere(upper>0.95)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "f9691003-2ed2-4dbd-a040-7f9b55d930f0",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([[0, 1]], dtype=int64)"
+                        ]
+                    },
+                    "execution_count": 10,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "corr_cols"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 38,
+            "id": "336c384d-b210-4fde-bbb7-d2e9b390302d",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([0.  , 0.4 , 0.78])"
+                        ]
+                    },
+                    "execution_count": 38,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "X[:,0]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 39,
+            "id": "407eae23-840e-482b-b203-e0e93f9b4227",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "array([0.1 , 0.45, 0.81])"
                         ]
                     },
-                    "execution_count": 43,
+                    "execution_count": 39,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "10//5"
+                "X[:,1]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e282ab86-f8dd-4fb6-8b90-3b613f585663",
+            "id": "34aa4763-8122-4c48-85a0-05bb062f022f",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `pycompete-0.0.5/pycompete/evaluation/metrics.py` & `pycompete-0.0.6/pycompete/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/pycompete/features/transformers.py` & `pycompete-0.0.6/pycompete/features/transformers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn._typing import ArrayLike, MatrixLike
+from numpy.typing import ArrayLike
 from typing import Optional
 import numpy as np
 import pandas as pd
 
 
 class RemoveCorrelated(BaseEstimator, TransformerMixin):
     def __init__(self, max_correlation: int = 0.95):
         """
         A transformer which removes highly correlated features.
 
+        This is a naive implementation which removes correlated features, it is
+        not stable for cases with groups of correlated features. This
+        implementation keeps the features with the lowest column index.
+
         Parameters:
         -----------
         max_correlation : float,
             The maximum correlation between features before they are removed.
 
         Attributes:
         -----------
         self.c_mat_ : np.array,
             The correlation matrix of X.
         """
         self.max_correlation = max_correlation
 
-    def fit(self, X: MatrixLike, y: Optional[ArrayLike] = None):
+    def fit(self, X: ArrayLike, y: Optional[ArrayLike] = None):
         """
         Fit the transformer according to the given training data.
 
         Calculates the correlation matrix (c_mat_) of X and calculates
         indexes of columns which display more than 'max_correlation'
         to another column.
 
@@ -38,22 +42,21 @@
 
         y : array-like of shape (n_samples,),
             Target vector relative to X. Not used, included for API
             compatability.
         """
         if isinstance(X, pd.DataFrame):
             X = X.to_numpy()
-        # TO DO: check all entries are float
-        self.c_mat_ = np.corrcoef(X)
-        correlated_mask = (self.c_mat_ > self.max_correlation) & (self.c_mat_ != 1)
-        corr_cols = np.argwhere(correlated_mask)
-        self.cols_to_drop = np.unique((np.sort(corr_cols, axis=1)), axis=0)[:, 0]
+        self.c_mat_ = np.absolute(np.corrcoef(X, rowvar=False))
+        upper = np.triu(self.c_mat_, k=1)
+        corr_cols = np.argwhere(upper > self.max_correlation)
+        self.cols_to_drop = np.unique(corr_cols[:, 1])
         return self
 
-    def transform(self, X: MatrixLike, y: Optional[ArrayLike] = None):
+    def transform(self, X: ArrayLike, y: Optional[ArrayLike] = None):
         """
         Transform X by removing the columns which are highly correlated.
 
         Parameters:
         -----------
         X : {array-like, sparse matrix}
             Training vector of shape (n_samples, n_features), where 'n_samples'
```

### Comparing `pycompete-0.0.5/pycompete/model_selection/cv_splitters.py` & `pycompete-0.0.6/pycompete/model_selection/cv_splitters.py`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/pycompete.egg-info/PKG-INFO` & `pycompete-0.0.6/pycompete.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycompete
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools to support the training and evalaution of models for the CrunchDAO project.
 Author: Francis P Chmiel
 License: MIT license
 Keywords: crunchdao
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pycompete-0.0.5/pycompete.egg-info/SOURCES.txt` & `pycompete-0.0.6/pycompete.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 pycompete.egg-info/SOURCES.txt
 pycompete.egg-info/dependency_links.txt
 pycompete.egg-info/requires.txt
 pycompete.egg-info/top_level.txt
 pycompete/evaluation/metrics.py
 pycompete/features/transformers.py
 pycompete/model_selection/cv_splitters.py
-tests/unit/evaluation/test_metric.py
+tests/unit/evaluation/test_metric.py
+tests/unit/features/test_transformers.py
```

### Comparing `pycompete-0.0.5/pyproject.toml` & `pycompete-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycompete-0.0.5/tests/unit/evaluation/test_metric.py` & `pycompete-0.0.6/tests/unit/evaluation/test_metric.py`

 * *Files identical despite different names*

