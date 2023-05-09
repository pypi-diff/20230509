# Comparing `tmp/bcirisktools-0.2.9.tar.gz` & `tmp/bcirisktools-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.2.9.tar", last modified: Tue May  9 13:15:04 2023, max compression
+gzip compressed data, was "bcirisktools-0.3.tar", last modified: Tue May  9 16:20:46 2023, max compression
```

## Comparing `bcirisktools-0.2.9.tar` & `bcirisktools-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-09 13:15:04.931000 bcirisktools-0.2.9/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.2.9/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-05-09 13:15:04.924000 bcirisktools-0.2.9/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.2.9/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-09 13:15:04.789000 bcirisktools-0.2.9/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.2.9/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-03-02 03:11:23.000000 bcirisktools-0.2.9/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.2.9/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.2.9/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    10025 2023-03-23 00:01:50.000000 bcirisktools-0.2.9/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5852 2023-05-09 13:14:22.000000 bcirisktools-0.2.9/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    19187 2023-05-09 13:13:17.000000 bcirisktools-0.2.9/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-09 13:15:04.903000 bcirisktools-0.2.9/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-05-09 13:15:04.000000 bcirisktools-0.2.9/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-05-09 13:15:04.000000 bcirisktools-0.2.9/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-05-09 13:15:04.000000 bcirisktools-0.2.9/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-05-09 13:15:04.000000 bcirisktools-0.2.9/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-05-09 13:15:04.000000 bcirisktools-0.2.9/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.2.9/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-05-09 13:15:04.936000 bcirisktools-0.2.9/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1018 2023-05-09 13:14:47.000000 bcirisktools-0.2.9/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-09 16:20:46.131000 bcirisktools-0.3/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2022-10-12 10:00:20.000000 bcirisktools-0.3/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-05-09 16:20:46.124000 bcirisktools-0.3/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2022-12-02 15:48:25.000000 bcirisktools-0.3/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-09 16:20:45.992000 bcirisktools-0.3/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-03-02 03:02:45.000000 bcirisktools-0.3/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-03-02 03:11:23.000000 bcirisktools-0.3/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-03-02 03:02:45.000000 bcirisktools-0.3/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-03-02 03:02:45.000000 bcirisktools-0.3/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    10025 2023-03-23 00:01:50.000000 bcirisktools-0.3/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5783 2023-05-09 16:19:37.000000 bcirisktools-0.3/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    19187 2023-05-09 13:13:17.000000 bcirisktools-0.3/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-05-09 16:20:46.106000 bcirisktools-0.3/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-05-09 16:20:45.000000 bcirisktools-0.3/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      410 2023-05-09 16:20:45.000000 bcirisktools-0.3/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-05-09 16:20:45.000000 bcirisktools-0.3/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-05-09 16:20:45.000000 bcirisktools-0.3/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-05-09 16:20:45.000000 bcirisktools-0.3/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-03-02 03:02:45.000000 bcirisktools-0.3/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-05-09 16:20:46.135000 bcirisktools-0.3/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1016 2023-05-09 16:19:48.000000 bcirisktools-0.3/setup.py
```

### Comparing `bcirisktools-0.2.9/LICENCE` & `bcirisktools-0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.9/PKG-INFO` & `bcirisktools-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.2.9
+Version: 0.3
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.2.9/README.md` & `bcirisktools-0.3/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.9/bcirisktools/input_filters.py` & `bcirisktools-0.3/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.9/bcirisktools/metrics_bci.py` & `bcirisktools-0.3/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.9/bcirisktools/modeling.py` & `bcirisktools-0.3/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.9/bcirisktools/shapley_report.py` & `bcirisktools-0.3/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.9/bcirisktools/stability.py` & `bcirisktools-0.3/bcirisktools/stability.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             expected = df_feat.iloc[:, i] + 10e-20
             df_out.iloc[:, i + 1] = (actual - expected) * np.log(actual / expected)
 
         # Preparamos salida y append
         df_out = df_out.drop(columns=df_feat.columns[0])
         df_out = pd.DataFrame(df_out.sum()).rename(columns={0: a_variable}).T
         df_out["cuantil"] = quantiles
-        df_append = pd.concat([df_append, df_out], axis=0).reset_index(drop=True)
+        df_append = pd.concat([df_append, df_out], axis=0)
 
     # Semaforo de estabilidad
     df_append["status"] = "🟢"
     df_append["status_2"] = "low"
 
     cond1 = (df_append.iloc[:, :-3] >= 0.1) & (df_append.iloc[:, :-3] < 0.2)
     cond1 = cond1.any(axis=1)
@@ -136,23 +136,25 @@
         # Preparamos salida y append para la mean
         df_feat_mean = (
             df_feat_mean.dropna()[["period", "diff_%"]]
             .rename(columns={"diff_%": a_variable})
             .set_index("period")
             .T
         )
-        df_append_mean = pd.concat([df_append_mean, df_feat_mean], axis=0).reset_index(drop=True)
+        df_append_mean = pd.concat([df_append_mean, df_feat_mean], axis=0)
 
         # Preparamos salida y append para la std
         df_feat_std = df_feat_std.set_index("period").T
-        df_append_std = pd.concat([df_append_std, df_feat_std], axis=0).reset_index(drop=True)
+        df_append_std = pd.concat([df_append_std, df_feat_std], axis=0)
 
         # generamos info de nulls
         a = df_feat_nulls.groupby("period").agg({"bool": "count"})
         b = df_feat_nulls.groupby("period").agg({"bool": "sum"})
         df_feat_nulls = (b * 100 / a).rename(columns={"bool": a_variable})
 
         # Preparamos salida de nulos
         df_feat_nulls = df_feat_nulls.T
-        df_append_nulls = pd.concat([df_append_nulls,df_feat_nulls], axis=0).reset_index(drop=True)
+        df_append_nulls = pd.concat(
+            [df_append_nulls, df_feat_nulls], axis=0
+        )
 
     return df_append_mean, df_append_std, df_append_nulls
```

### Comparing `bcirisktools-0.2.9/bcirisktools/tree_crt.py` & `bcirisktools-0.3/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.2.9/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.3/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.2.9
+Version: 0.3
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.2.9/setup.py` & `bcirisktools-0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.2.9"
+VERSION = "0.3"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

