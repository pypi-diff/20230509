# Comparing `tmp/TCLR-1.7.0.tar.gz` & `tmp/TCLR-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCLR-1.7.0.tar", last modified: Mon May  8 04:12:29 2023, max compression
+gzip compressed data, was "TCLR-1.8.0.tar", last modified: Tue May  9 03:03:46 2023, max compression
```

## Comparing `TCLR-1.7.0.tar` & `TCLR-1.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:12:29.833837 TCLR-1.7.0/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:12:29.833691 TCLR-1.7.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.7.0/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:12:29.832704 TCLR-1.7.0/TCLR/
--rw-r-----   0 jacob      (501) staff       (20)    34868 2023-05-08 04:12:08.000000 TCLR-1.7.0/TCLR/TCLRalgorithm.py
--rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.7.0/TCLR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-08 04:12:29.833507 TCLR-1.7.0/TCLR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-08 04:12:29.000000 TCLR-1.7.0/TCLR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-08 04:12:29.833879 TCLR-1.7.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-08 04:12:23.000000 TCLR-1.7.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 03:03:46.174685 TCLR-1.8.0/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 03:03:46.174567 TCLR-1.8.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.8.0/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 03:03:46.173807 TCLR-1.8.0/TCLR/
+-rw-r-----   0 jacob      (501) staff       (20)    37461 2023-05-09 03:02:55.000000 TCLR-1.8.0/TCLR/TCLRalgorithm.py
+-rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.8.0/TCLR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 03:03:46.174405 TCLR-1.8.0/TCLR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-09 03:03:46.000000 TCLR-1.8.0/TCLR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-09 03:03:46.174722 TCLR-1.8.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-09 03:03:27.000000 TCLR-1.8.0/setup.py
```

### Comparing `TCLR-1.7.0/PKG-INFO` & `TCLR-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.7.0
+Version: 1.8.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.7.0/README.md` & `TCLR-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `TCLR-1.7.0/TCLR/TCLRalgorithm.py` & `TCLR-1.8.0/TCLR/TCLRalgorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import re
 from tabnanny import check
 from textwrap import indent
 import time
 import copy
 import os
 import warnings
+import random
+from typing import List
 import numpy as np
 import pandas as pd
 from graphviz import Digraph
 from scipy import stats
 from gplearn import genetic
 from minepy import MINE
 
@@ -25,15 +27,15 @@
         self.size = data.shape[0]
         self.R = 0
         self.bestFeature = 0
         self.bestValue = 0
         self.leaf_no = -1
 
 
-def start(filePath, correlation='PearsonR(+)', minsize=3, threshold=0.95, mininc=0.01, split_tol = 0.8,tolerance_list = None , weight=True,
+def start(filePath, correlation='PearsonR(+)', minsize=3, threshold=0.95, mininc=0.01, split_tol = 0.8, epochs = 5,random_seed=42, Generate_Features = True, tolerance_list = None , weight=True,
          gplearn = False, gpl_dummyfea = None, population_size = 500, generations = 100, verbose = 1, 
          metric = 'mean absolute error',
          function_set = ['add', 'sub', 'mul', 'div', 'log', 'sqrt', 'abs', 'neg','inv','sin','cos','tan',]):
     
     """
     Tree Classifier for Linear Regression (TCLR) 
 
@@ -72,15 +74,15 @@
             3>
             R2:
             In statistics, the coefficient of determination, denoted R2 or r2 and pronounced "R squared", 
             is the proportion of the variation in the dependent variable that is predictable from the independent variable(s).
             t is a statistic used in the context of statistical models whose main purpose is either the prediction of future 
             outcomes or the testing of hypotheses, on the basis of other related information. It provides a measure of how well
             observed outcomes are replicated by the model, based on the proportion of total variation of outcomes explained by the model.
-            Definition from Wikipedia ：https://en.wikipedia.org/wiki/Coefficient_of_determination
+            Definition from Wikipedia : https://en.wikipedia.org/wiki/Coefficient_of_determination
             R2 = 1 - SSres / SStot. Its value may be a negative one for poor correlation.
  
   
     :param minsize : 
             a int number (default=3), minimum unique values for linear features of data on each leaf.
     
     :param threshold : 
@@ -88,14 +90,23 @@
             In the process of dividing the dataset, the smallest relevant index allowed in the you research.
             To avoid overfitting, threshold = 0.5 is suggested for MIC 0.5.
     
     :param mininc : Minimum expected gain of objective function (default=0.01)
 
     :param split_tol : a float (default=0.8), constrained features value shound be narrowed in a minmimu ratio of split_tol on split path
 
+    :param epochs : an integer (default=5), see parameter Generate_Features (below)
+
+    :param random_seed :  an integer (default=42), see parameter Generate_Features (below)
+
+    :param Generate_Features : boole (default=True). When Generate_Features = True, TCLR will generate new features by operating  
+        the ['+','-','*'] on original features. Iterating [param : epoachs] times, and each time generating 3 new features.  [param : random_seed]
+        is used to control the randomness.
+        When Generate_Features = False, TCLR will apply the original features
+
     :param tolerance_list: 
             constraints imposed on features, default is null
             list shape in two dimensions, viz., [['feature_name1',tol_1],['feature_name2',tol_2]...]
             'feature_name1', 'feature_name2' (string) are names of input features;
             tol_1, tol_2 (float, between 0 to 1) are feature's tolerance ratios;
             the variations of feature values on each leaf must be in the tolerance;
             if tol_1 = 0, the value of feature 'feature_name1' must be a constant on each leaf,
@@ -105,16 +116,14 @@
     :param weight:
             The weight of the gain function, default is True.
             When weight is True: linear_gain = R(father node) - ( W_l * R(left child node) + W_r * R(right child node)) / 2
             Where W_l is the ratio of the number of samples in the left child node to the total number of samples ;
                   W_r is the ratio of the number of samples in the right child node to the total number of samples.
             When weight is False: linear_gain = R(father node) - ( R(left child node) + R(right child node)) / 2
 
-
-
     :param gplearn : Whether to call the embedded gplearn package of TCLR to regress formula (default=False).
     
     :param gpl_dummyfea: 
             dummy features in gpleran regression, default is null
             list shape in one dimension, viz., ['feature_name1','feature_name2',...]
             dummy features : 'feature_name1','feature_name2',... are not used anymore in gpleran regression 
 
@@ -176,15 +185,36 @@
     os.makedirs('Segmented', exist_ok=True)
     # global var. for statisticaling  results
     global record
     record = 0
     timename = time.localtime(time.time())
     namey, nameM, named, nameh, namem = timename.tm_year, timename.tm_mon, timename.tm_mday, timename.tm_hour, timename.tm_min
 
-    csvData = pd.read_csv(filePath)
+    read_csvData = pd.read_csv(filePath)
+
+    input_csvData = read_csvData.iloc[:,:-2]
+    if Generate_Features == True:
+        # cal an appropriate value of batch
+        if len(input_csvData) - 1 <= 3:
+            batch = 1
+        else:
+            batch = 3
+        # generate new dataset
+        for epoch in range(epochs):
+            # for increasing the randomness
+            random_seed += 1
+            input_csvData = generate_random_features(input_csvData,[column for column in input_csvData],batch,random_seed)
+           
+        input_csvData = input_csvData.assign(linear_X=read_csvData.iloc[:,-2])
+        csvData = input_csvData.assign(linear_Y=read_csvData.iloc[:,-1])
+
+    else:
+        csvData = read_csvData
+    
+    
     copy_csvData = copy.deepcopy(csvData)
     copy_csvData['slope'] = None
     copy_csvData['intercept'] = None
     copy_csvData[correlation] = None
     copy_csvData.to_csv('Segmented/all_dataset.csv', index=False)
 
     feats = [column for column in csvData]
@@ -768,7 +798,43 @@
     elif weight == True:
         weightRa = len(subDataSetA[:, -1]) / (len(subDataSetA[:, -1]) + len(subDataSetB[:, -1]))
         weightRb = len(subDataSetB[:, -1]) / (len(subDataSetA[:, -1]) + len(subDataSetB[:, -1]))
         R = weightRa * newRa + weightRb * newRb
         return R
     else:
         print('Parameter error | weight')
+
+
+# code on 22023 May 9, Bin Cao
+def generate_random_features(df: pd.DataFrame, 
+                            feature_list: List[str],
+                            num_combinations: int,
+                             random_seed:int) -> pd.DataFrame:
+    """
+    randomly generates new feature combinations.
+
+    :param df: DataFrame containing the original features.
+    :param feature_list: List of original features.
+    :param num_combinations: Number of combination features to generate.
+    :return: DataFrame containing the new features.
+    """
+    new_features = []
+    random.seed(random_seed)
+    # randomly generates combination features
+    for i in range(num_combinations):
+        # randomly chooses two features
+        f1 = random.choice(feature_list)
+        f2 = random.choice(feature_list)
+        
+        # choose a operator
+        op = random.choice(['+', '-', '*'])
+        
+        # new feature name
+        new_feature = f'({f1} {op} {f2})'
+        
+        new_features.append(new_feature)
+        
+        # cal new features
+        df[new_feature] = eval(f'df["{f1}"] {op} df["{f2}"]')
+    
+    # reture DataFrame 
+    return df
```

### Comparing `TCLR-1.7.0/TCLR/__init__.py` & `TCLR-1.8.0/TCLR/__init__.py`

 * *Files identical despite different names*

### Comparing `TCLR-1.7.0/TCLR.egg-info/PKG-INFO` & `TCLR-1.8.0/TCLR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.7.0
+Version: 1.8.0
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.7.0/setup.py` & `TCLR-1.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='TCLR',  # 包名
-    version='1.7.0',  # 版本
+    version='1.8.0',  # 版本
     description="Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

