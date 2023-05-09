# Comparing `tmp/xdatasets-0.2.3.tar.gz` & `tmp/xdatasets-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdatasets-0.2.3.tar", last modified: Tue May  2 00:30:53 2023, max compression
+gzip compressed data, was "xdatasets-0.2.6.tar", last modified: Tue May  9 16:35:56 2023, max compression
```

## Comparing `xdatasets-0.2.3.tar` & `xdatasets-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:30:53.562669 xdatasets-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-02 00:30:49.000000 xdatasets-0.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-02 00:30:49.000000 xdatasets-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 00:30:49.000000 xdatasets-0.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-02 00:30:49.000000 xdatasets-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 00:30:49.000000 xdatasets-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-02 00:30:53.562669 xdatasets-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-02 00:30:49.000000 xdatasets-0.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-02 00:30:53.562669 xdatasets-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-02 00:30:49.000000 xdatasets-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:30:53.558669 xdatasets-0.2.3/xdatasets/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-02 00:30:49.000000 xdatasets-0.2.3/xdatasets/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 00:30:53.562669 xdatasets-0.2.3/xdatasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 00:30:53.000000 xdatasets-0.2.3/xdatasets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:35:56.370160 xdatasets-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-09 16:35:49.000000 xdatasets-0.2.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-09 16:35:49.000000 xdatasets-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-09 16:35:49.000000 xdatasets-0.2.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-09 16:35:49.000000 xdatasets-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 16:35:49.000000 xdatasets-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 16:35:56.370160 xdatasets-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-09 16:35:49.000000 xdatasets-0.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-09 16:35:56.370160 xdatasets-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-09 16:35:49.000000 xdatasets-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:35:56.370160 xdatasets-0.2.6/xdatasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-09 16:35:49.000000 xdatasets-0.2.6/xdatasets/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:35:56.370160 xdatasets-0.2.6/xdatasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 16:35:56.000000 xdatasets-0.2.6/xdatasets.egg-info/top_level.txt
```

### Comparing `xdatasets-0.2.3/CONTRIBUTING.rst` & `xdatasets-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/LICENSE` & `xdatasets-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/PKG-INFO` & `xdatasets-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.3
+Version: 0.2.6
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.3/README.rst` & `xdatasets-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/setup.py` & `xdatasets-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,10 +72,10 @@
     long_description_content_type="text/x-rst",
     include_package_data=True,
     keywords=KEYWORDS,
     name=NAME,
     packages=find_packages(),
     extras_require={"dev": dev_requirements},
     url=URL,
-    version='0.2.3',
+    version='0.2.6',
     zip_safe=False,
 )
```

### Comparing `xdatasets-0.2.3/xdatasets/core.py` & `xdatasets-0.2.6/xdatasets/core.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/xdatasets/scripting.py` & `xdatasets-0.2.6/xdatasets/scripting.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/xdatasets/spatial.py` & `xdatasets-0.2.6/xdatasets/spatial.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 
 
 
 def clip_by_polygon(ds,
                     space,
                     dataset_name
                     ):
+    # We are not using clisops for weighted averages because it is too unstable for now and requires conda environment.
+    # We use a modified version of the xagg package from which we have removed the xesmf/esmpy dependency
+
+
     indexer = shape_bbox_indexer(ds, space['geometry'])
     ds_copy = ds.isel(indexer).copy()
     
     arrays = []
     pbar = tqdm(space['geometry'].iterrows())
     for idx, row in pbar:
         item = row[space['unique_id']] if space['unique_id'] != None and space['unique_id'] in row else idx
```

### Comparing `xdatasets-0.2.3/xdatasets/temporal.py` & `xdatasets-0.2.6/xdatasets/temporal.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/xdatasets/tutorial.py` & `xdatasets-0.2.6/xdatasets/tutorial.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/xdatasets/utils.py` & `xdatasets-0.2.6/xdatasets/utils.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/xdatasets/validations.py` & `xdatasets-0.2.6/xdatasets/validations.py`

 * *Files identical despite different names*

### Comparing `xdatasets-0.2.3/xdatasets/workflows.py` & `xdatasets-0.2.6/xdatasets/workflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,19 +151,14 @@
     #     ds = clip_by_bbox(ds, space, dataset_name).load()
         
     if time["timestep"] != None and time['aggregation'] != None:
         if pd.Timedelta(1, unit=time["timestep"]) > pd.Timedelta(1, unit=xr.infer_freq(ds.time)):
             ds = temporal_aggregation(ds,
                                     time,
                                     dataset_name)
-    # Add source name to dataset
-    #np.warnings.filterwarnings('ignore', category=np.VisibleDeprecationWarning)
-    ds = ds.assign_coords(source=("source", [dataset_name]))
-    for var in ds.keys():
-        ds[var] = ds[var].expand_dims("source", axis=-1)
 
     return ds
 
 
 def user_provided_dataset(dataset_name,
                           variables,
                           space,
```

### Comparing `xdatasets-0.2.3/xdatasets.egg-info/PKG-INFO` & `xdatasets-0.2.6/xdatasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdatasets
-Version: 0.2.3
+Version: 0.2.6
 Summary: Easy acess to earth observation datasets with xarray.
 Home-page: https://github.com/hydrologie/xdatasets'
 Author: Sebastien Langlois
 Author-email: sebastien.langlois62@gmail.com
 License: MIT license
 Keywords: xdatasets hydrology meteorology climate climatology netcdf gridded analysis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xdatasets-0.2.3/xdatasets.egg-info/requires.txt` & `xdatasets-0.2.6/xdatasets.egg-info/requires.txt`

 * *Files identical despite different names*

