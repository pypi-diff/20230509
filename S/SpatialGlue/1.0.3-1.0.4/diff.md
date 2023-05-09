# Comparing `tmp/SpatialGlue-1.0.3.tar.gz` & `tmp/SpatialGlue-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpatialGlue-1.0.3.tar", last modified: Tue May  9 01:57:26 2023, max compression
+gzip compressed data, was "dist/SpatialGlue-1.0.4.tar", last modified: Tue May  9 02:21:35 2023, max compression
```

## Comparing `SpatialGlue-1.0.3.tar` & `SpatialGlue-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:57:26.782359 SpatialGlue-1.0.3/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)    34523 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/LICENSE.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 01:57:26.778358 SpatialGlue-1.0.3/PKG-INFO
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1671 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/README.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/README.rst
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:57:26.778358 SpatialGlue-1.0.3/SpatialGlue/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     6845 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/SpatialGlue/SpatialGlue.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     7620 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/SpatialGlue/model.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)    12330 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/SpatialGlue/preprocess.py
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/SpatialGlue/readme.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     6019 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/SpatialGlue/utils.py
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:57:26.778358 SpatialGlue-1.0.3/SpatialGlue.egg-info/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 01:57:26.000000 SpatialGlue-1.0.3/SpatialGlue.egg-info/PKG-INFO
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      409 2023-05-09 01:57:26.000000 SpatialGlue-1.0.3/SpatialGlue.egg-info/SOURCES.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:57:26.000000 SpatialGlue-1.0.3/SpatialGlue.egg-info/dependency_links.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 01:57:26.000000 SpatialGlue-1.0.3/SpatialGlue.egg-info/not-zip-safe
--rw-rw-r--   0 yahui     (9019) yahui     (1023)        9 2023-05-09 01:57:26.000000 SpatialGlue-1.0.3/SpatialGlue.egg-info/requires.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)       12 2023-05-09 01:57:26.000000 SpatialGlue-1.0.3/SpatialGlue.egg-info/top_level.txt
--rw-rw-r--   0 yahui     (9019) yahui     (1023)   653466 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/SpatialGlue.png
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      330 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/__init__.py
-drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 01:57:26.778358 SpatialGlue-1.0.3/data/
--rw-rw-r--   0 yahui     (9019) yahui     (1023)      628 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/data/readme.md
--rw-rw-r--   0 yahui     (9019) yahui     (1023)       38 2023-05-09 01:57:26.782359 SpatialGlue-1.0.3/setup.cfg
--rw-rw-r--   0 yahui     (9019) yahui     (1023)     1685 2023-05-09 01:56:35.000000 SpatialGlue-1.0.3/setup.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)    34523 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/LICENSE.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/PKG-INFO
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1671 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/README.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/README.rst
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/SpatialGlue/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     6845 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/SpatialGlue.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     7620 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/model.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)    12330 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/preprocess.py
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/readme.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     5974 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue/utils.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/SpatialGlue.egg-info/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1006 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/PKG-INFO
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      409 2023-05-09 02:21:35.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/SOURCES.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/dependency_links.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        1 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/not-zip-safe
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)        9 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/requires.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)       12 2023-05-09 02:21:34.000000 SpatialGlue-1.0.4/SpatialGlue.egg-info/top_level.txt
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)   653466 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/SpatialGlue.png
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      330 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/__init__.py
+drwxrwxr-x   0 yahui     (9019) yahui     (1023)        0 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/data/
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)      628 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/data/readme.md
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)       38 2023-05-09 02:21:35.061217 SpatialGlue-1.0.4/setup.cfg
+-rw-rw-r--   0 yahui     (9019) yahui     (1023)     1685 2023-05-09 02:20:42.000000 SpatialGlue-1.0.4/setup.py
```

### Comparing `SpatialGlue-1.0.3/LICENSE.md` & `SpatialGlue-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.3/PKG-INFO` & `SpatialGlue-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialGlue
-Version: 1.0.3
+Version: 1.0.4
 Summary: Integrated analysis of spatial multi-omics with SpatialGlue
 Home-page: https://github.com/JinmiaoChenLab/SpatialGlue
 Author: Yahui Long
 Author-email: longyh@immunol.a-star.edu.sg
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `SpatialGlue-1.0.3/README.md` & `SpatialGlue-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.3/SpatialGlue/SpatialGlue.py` & `SpatialGlue-1.0.4/SpatialGlue/SpatialGlue.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.3/SpatialGlue/model.py` & `SpatialGlue-1.0.4/SpatialGlue/model.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.3/SpatialGlue/preprocess.py` & `SpatialGlue-1.0.4/SpatialGlue/preprocess.py`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.3/SpatialGlue/utils.py` & `SpatialGlue-1.0.4/SpatialGlue/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,19 +134,19 @@
 
 def plot_weight_value(alpha, label, modality1='mRNA', modality2='protein'):
   """\
   Plotting weight values
   
   """  
   import pandas as pd  
-  for i, val in enumerate(alpha):
-    df = pd.DataFrame(columns=[modality1, modality2, 'label'])  
-    df[modality1], df[modality2] = val[:, 0], val[:, 1]
-    df['label'] = label
-    df = df.set_index('label').stack().reset_index()
-    df.columns = ['label_SpatialGlue', 'Modality', 'Weight value']
-    ax = sns.violinplot(data=df, x='label_SpatialGlue', y='Weight value', hue="Modality",
+  
+  df = pd.DataFrame(columns=[modality1, modality2, 'label'])  
+  df[modality1], df[modality2] = alpha[:, 0], alpha[:, 1]
+  df['label'] = label
+  df = df.set_index('label').stack().reset_index()
+  df.columns = ['label_SpatialGlue', 'Modality', 'Weight value']
+  ax = sns.violinplot(data=df, x='label_SpatialGlue', y='Weight value', hue="Modality",
                 split=True, inner="quart", linewidth=1, show=False)
-    ax.set_title(modality1 + ' vs ' + modality2) 
+  ax.set_title(modality1 + ' vs ' + modality2) 
 
-    plt.tight_layout(w_pad=0.05)
-    plt.show()     
+  plt.tight_layout(w_pad=0.05)
+  plt.show()
```

### Comparing `SpatialGlue-1.0.3/SpatialGlue.egg-info/PKG-INFO` & `SpatialGlue-1.0.4/SpatialGlue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialGlue
-Version: 1.0.3
+Version: 1.0.4
 Summary: Integrated analysis of spatial multi-omics with SpatialGlue
 Home-page: https://github.com/JinmiaoChenLab/SpatialGlue
 Author: Yahui Long
 Author-email: longyh@immunol.a-star.edu.sg
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `SpatialGlue-1.0.3/SpatialGlue.png` & `SpatialGlue-1.0.4/SpatialGlue.png`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.3/data/readme.md` & `SpatialGlue-1.0.4/data/readme.md`

 * *Files identical despite different names*

### Comparing `SpatialGlue-1.0.3/setup.py` & `SpatialGlue-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import Command, find_packages, setup
 
 __lib_name__ = "SpatialGlue"
-__lib_version__ = "1.0.3"
+__lib_version__ = "1.0.4"
 __description__ = "Integrated analysis of spatial multi-omics with SpatialGlue"
 __url__ = "https://github.com/JinmiaoChenLab/SpatialGlue"
 __author__ = "Yahui Long"
 __author_email__ = "longyh@immunol.a-star.edu.sg"
 __license__ = "MIT"
 __keywords__ = ["Spatial multi-omics", "Cross-omics integration", "Deep learning", "Graph neural networks", "Dual attention"]
 __requires__ = ["requests",]
```

