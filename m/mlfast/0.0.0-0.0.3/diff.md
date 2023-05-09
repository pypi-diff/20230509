# Comparing `tmp/mlfast-0.0.0.tar.gz` & `tmp/mlfast-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfast-0.0.0.tar", last modified: Tue May  9 05:30:24 2023, max compression
+gzip compressed data, was "mlfast-0.0.3.tar", last modified: Tue May  9 17:55:47 2023, max compression
```

## Comparing `mlfast-0.0.0.tar` & `mlfast-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:30:24.767910 mlfast-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 05:29:29.000000 mlfast-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-09 05:30:24.767910 mlfast-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 05:29:29.000000 mlfast-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 05:29:29.000000 mlfast-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-09 05:30:24.767910 mlfast-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-09 05:29:29.000000 mlfast-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:30:24.763910 mlfast-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:30:24.763910 mlfast-0.0.0/src/mlfast/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-09 05:29:29.000000 mlfast-0.0.0/src/mlfast/Classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-09 05:29:29.000000 mlfast-0.0.0/src/mlfast/Regression.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-09 05:29:29.000000 mlfast-0.0.0/src/mlfast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-09 05:29:29.000000 mlfast-0.0.0/src/mlfast/custom_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 05:29:29.000000 mlfast-0.0.0/src/mlfast/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:30:24.763910 mlfast-0.0.0/src/mlfast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-09 05:30:24.000000 mlfast-0.0.0/src/mlfast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-09 05:30:24.000000 mlfast-0.0.0/src/mlfast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:30:24.000000 mlfast-0.0.0/src/mlfast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 05:30:24.000000 mlfast-0.0.0/src/mlfast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 05:30:24.000000 mlfast-0.0.0/src/mlfast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 17:54:47.000000 mlfast-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 17:55:47.053438 mlfast-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 17:54:47.000000 mlfast-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 17:54:47.000000 mlfast-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-09 17:55:47.053438 mlfast-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-09 17:54:47.000000 mlfast-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/src/mlfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/Classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/Regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/custom_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-09 17:54:47.000000 mlfast-0.0.3/src/mlfast/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:55:47.053438 mlfast-0.0.3/src/mlfast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 17:55:47.000000 mlfast-0.0.3/src/mlfast.egg-info/top_level.txt
```

### Comparing `mlfast-0.0.0/LICENSE` & `mlfast-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.0/setup.cfg` & `mlfast-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.0/setup.py` & `mlfast-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
-    
-__version__="0.0.0"
+
+__version__ = "0.0.3"
 
 REPO_NAME = "mlfast"
 AUTHOR_USER_NAME = "Abdul-Jaweed"
-AUTHOR_EMAIL = "jdgaming7320@gmail.com"
 SRC_REPO = "mlfast"
-DESCRIPTION = "its a python machine learning package"
+AUTHOR_EMAIL = "jdgaming7320@gmail.com"
 
 setuptools.setup(
     name=SRC_REPO,
     version=__version__,
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    description=DESCRIPTION,
+    description="its a python machine learning package",
     long_description=long_description,
-    long_description_content = "text/markdown",
-    url = f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
+    long_description_content="text/markdown",
+    url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src")
-)
+)
```

### Comparing `mlfast-0.0.0/src/mlfast/Classification.py` & `mlfast-0.0.3/src/mlfast/Regression.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,106 @@
 # importing Libraries
-
 import os
 import sys
+import numpy as np
+import pandas as pd
 from sklearn.model_selection import train_test_split
-from sklearn.linear_model import LogisticRegression
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.ensemble import RandomForestClassifier, GradientBoostingClassifier, AdaBoostClassifier
-from sklearn.svm import SVC
-from sklearn.neighbors import KNeighborsClassifier
+from sklearn.linear_model import LinearRegression, Ridge, Lasso, ElasticNet
+from sklearn.tree import DecisionTreeRegressor
+from sklearn.ensemble import (
+    RandomForestRegressor,
+    GradientBoostingRegressor,
+    AdaBoostRegressor,
+)
+from sklearn.svm import SVR
+from sklearn.neighbors import KNeighborsRegressor
 import xgboost as xgb
-from sklearn.metrics import accuracy_score, classification_report
-from sklearn.preprocessing import StandardScaler, RobustScaler, OneHotEncoder, LabelEncoder
+from sklearn.metrics import mean_absolute_error, mean_squared_error, r2_score
+from sklearn.preprocessing import StandardScaler, RobustScaler, OneHotEncoder
 from sklearn.compose import ColumnTransformer
 import pickle
 import warnings
-warnings.filterwarnings("ignore") 
-
 
+warnings.filterwarnings("ignore")
 
 
+def Regression(X, y, model="lr", scaler=None, cat=False):
+    import warnings
 
-def Classification(X, y, model='lr', scaler=None, cat=False):
-    
+    warnings.filterwarnings("ignore")
 
-    
     # Train test split
-    X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=52)
-    
-    
+    X_train, X_test, y_train, y_test = train_test_split(
+        X, y, test_size=0.2, random_state=52
+    )
+
     # One-hot encoding
     if cat:
-        categorical_cols = X.select_dtypes(include=['object']).columns.tolist()
+        categorical_cols = X.select_dtypes(include=["O"]).columns.tolist()
         if categorical_cols:
-            transformer = ColumnTransformer(transformers=[('ohe', OneHotEncoder(), categorical_cols)], remainder='passthrough')
+            transformer = ColumnTransformer(
+                transformers=[("ohe", OneHotEncoder(), categorical_cols)],
+                remainder="passthrough",
+            )
             X_train = transformer.fit_transform(X_train)
             X_test = transformer.transform(X_test)
-    
-    
-    
-    # Encoding the target variable if it is categorical
-    if y_train.dtype == 'O':
-        le = LabelEncoder()
-        y_train = le.fit_transform(y_train)
-        y_test = le.transform(y_test)
-    
-    
+
     # Scaling the data
-    if scaler == 'standard':
+    if scaler == "standard":
         scaler = StandardScaler()
-    elif scaler == 'robust':
+    elif scaler == "robust":
         scaler = RobustScaler()
     else:
         scaler = None
-    
+
     if scaler is not None:
         X_train = scaler.fit_transform(X_train)
         X_test = scaler.transform(X_test)
-    
-    
-    
+
     # Selecting the Model
-    if model == 'lr':
-        clf = LogisticRegression()
-    elif model == 'dt':
-        clf = DecisionTreeClassifier()
-    elif model == 'rf':
-        clf = RandomForestClassifier()
-    elif model == 'svm':
-        clf = SVC()
-    elif model == 'knn':
-        clf = KNeighborsClassifier()
-    elif model == 'gb':
-        clf = GradientBoostingClassifier()
-    elif model == 'ada':
-        clf = AdaBoostClassifier()
-    elif model == 'xbg':
-        clf = xgb.XGBClassifier(n_estimators=100, learning_rate=0.05, random_state=42)
+    if model == "lr":
+        reg = LinearRegression()
+    elif model == "ridge":
+        reg = Ridge()
+    elif model == "lasso":
+        reg = Lasso()
+    elif model == "enet":
+        reg = ElasticNet()
+    elif model == "dt":
+        reg = DecisionTreeRegressor()
+    elif model == "rf":
+        reg = RandomForestRegressor()
+    elif model == "svm":
+        reg = SVR()
+    elif model == "knn":
+        reg = KNeighborsRegressor()
+    elif model == "gb":
+        reg = GradientBoostingRegressor()
+    elif model == "ada":
+        reg = AdaBoostRegressor()
+    elif model == "xbg":
+        reg = xgb.XGBRegressor(n_estimators=100, learning_rate=0.05, random_state=42)
     else:
         return print("Invalid model name")
-    
+
     # Fitting the Model
-    clf.fit(X_train, y_train)
-    y_pred = clf.predict(X_test)
-    
+    reg.fit(X_train, y_train)
+    y_pred = reg.predict(X_test)
+
     # Printing Metrics
-    print(f"Accuracy Score :{accuracy_score(y_test, y_pred)}, \
-    \n \n Classification Report  \n {classification_report(y_test, y_pred)} ")
-    
+    print(
+        f" Mean Absolute Error :{mean_absolute_error(y_test, y_pred)},\
+    \n \n Mean Squared Error :{mean_squared_error(y_test, y_pred)},\
+    \n \n Root Mean Squared Error :{np.sqrt(mean_squared_error(y_test, y_pred))},\
+    \n \n R2 Score :{r2_score(y_test, y_pred)}"
+    )
+
     # Saving the Model
-    model_dir = 'model'
+    model_dir = "model"
     if not os.path.exists(model_dir):
         os.mkdir(model_dir)
-    
-    filename = os.path.join(model_dir, f'{model}.pkl')
-    with open(filename, 'wb') as file:
-        pickle.dump(clf, file)
-    
-    print(f" \n Model saved successfully in {filename}")
+
+    filename = os.path.join(model_dir, f"{model}.pkl")
+    with open(filename, "wb") as file:
+        pickle.dump(reg, file)
+
+    print(f" \n Model saved successfully in {filename}")
```

