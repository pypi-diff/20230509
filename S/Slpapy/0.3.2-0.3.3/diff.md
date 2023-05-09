# Comparing `tmp/Slpapy-0.3.2.tar.gz` & `tmp/Slpapy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.3.2.tar", last modified: Tue May  9 06:54:02 2023, max compression
+gzip compressed data, was "Slpapy-0.3.3.tar", last modified: Tue May  9 08:15:08 2023, max compression
```

## Comparing `Slpapy-0.3.2.tar` & `Slpapy-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.973240 Slpapy-0.3.2/
--rw-rw-rw-   0        0        0      159 2023-05-09 06:54:02.973240 Slpapy-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.931424 Slpapy-0.3.2/Slpapy/
--rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.2/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.2/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.970248 Slpapy-0.3.2/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.3.2/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.3.2/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.2/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.2/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.2/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.3.2/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.3.2/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5812 2023-05-09 06:48:17.000000 Slpapy-0.3.2/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.941398 Slpapy-0.3.2/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 06:54:02.974237 Slpapy-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      484 2023-05-09 06:53:57.000000 Slpapy-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:08.178050 Slpapy-0.3.3/
+-rw-rw-rw-   0        0        0      159 2023-05-09 08:15:08.178050 Slpapy-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:08.141149 Slpapy-0.3.3/Slpapy/
+-rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.3/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.3/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:08.176056 Slpapy-0.3.3/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      662 2023-05-09 08:14:40.000000 Slpapy-0.3.3/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.3.3/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.3/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.3/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.3/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.3/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.3/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.3/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.3/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.3/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.3/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.3/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43450 2023-05-09 08:14:40.000000 Slpapy-0.3.3/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.3.3/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5812 2023-05-09 06:48:17.000000 Slpapy-0.3.3/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:15:08.150128 Slpapy-0.3.3/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-09 08:15:07.000000 Slpapy-0.3.3/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-09 08:15:08.000000 Slpapy-0.3.3/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 08:15:07.000000 Slpapy-0.3.3/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-09 08:15:07.000000 Slpapy-0.3.3/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 08:15:07.000000 Slpapy-0.3.3/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 08:15:08.178050 Slpapy-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-05-09 08:14:57.000000 Slpapy-0.3.3/setup.py
```

### Comparing `Slpapy-0.3.2/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.3/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.3/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/beats.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/logging.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.3.3/Slpapy/Spatial_map/scatterplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1355,7 +1355,18 @@
     lens = [len(arg) for arg in args]
     longest = max(lens)
     if not (set(lens) == {1, longest} or set(lens) == {longest}):
         raise ValueError(f"Could not broadast together arguments with shapes: {lens}.")
     return list(
         [[arg[0] for _ in range(longest)] if len(arg) == 1 else arg for arg in args]
     )
+
+def Spatial_class(adata, cls, n):
+    cls = str(cls)
+
+    for j in adata.obs_names:
+        if adata.obs.loc[j, f'{cls}'] == str(n):
+            adata.obs.loc[j, 'leidens'] = str(n)
+        else:
+            adata.obs.loc[j, 'leidens'] = 'bg'
+    embedding(adata, basis='X_spacial', color='leidens', frameon=False, save=f'_spacial_{cls}_{n}.png')
+    del adata.obs['leidens']
```

### Comparing `Slpapy-0.3.2/Slpapy/processing_analyze.py` & `Slpapy-0.3.3/Slpapy/processing_analyze.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.3.2/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.3/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

