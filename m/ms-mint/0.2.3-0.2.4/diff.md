# Comparing `tmp/ms-mint-0.2.3.tar.gz` & `tmp/ms-mint-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-0.2.3.tar", last modified: Thu Apr 27 15:30:19 2023, max compression
+gzip compressed data, was "ms-mint-0.2.4.tar", last modified: Tue May  9 16:42:49 2023, max compression
```

## Comparing `ms-mint-0.2.3.tar` & `ms-mint-0.2.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:30:19.840465 ms-mint-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-04-27 15:29:56.000000 ms-mint-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 15:29:56.000000 ms-mint-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-27 15:30:19.840465 ms-mint-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-04-27 15:29:56.000000 ms-mint-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:30:19.840465 ms-mint-0.2.3/ms_mint/
--rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 15:30:19.840465 ms-mint-0.2.3/ms_mint/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/matplotlib_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/plotly_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-27 15:29:56.000000 ms-mint-0.2.3/ms_mint/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:30:19.840465 ms-mint-0.2.3/ms_mint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 15:30:19.000000 ms-mint-0.2.3/ms_mint.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-04-27 15:30:19.840465 ms-mint-0.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1248 2023-04-27 15:29:56.000000 ms-mint-0.2.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-04-27 15:29:56.000000 ms-mint-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-05-09 16:42:32.000000 ms-mint-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-09 16:42:32.000000 ms-mint-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-09 16:42:49.036971 ms-mint-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-05-09 16:42:32.000000 ms-mint-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/ms_mint/
+-rw-r--r--   0 runner    (1001) docker     (123)    15871 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 16:42:49.036971 ms-mint-0.2.4/ms_mint/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11653 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/matplotlib_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/plotly_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-09 16:42:32.000000 ms-mint-0.2.4/ms_mint/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/ms_mint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-09 16:42:49.000000 ms-mint-0.2.4/ms_mint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 16:42:48.000000 ms-mint-0.2.4/ms_mint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:42:49.036971 ms-mint-0.2.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 16:42:32.000000 ms-mint-0.2.4/scripts/ms-mint-convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      450 2023-05-09 16:42:49.036971 ms-mint-0.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-05-09 16:42:32.000000 ms-mint-0.2.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-05-09 16:42:33.000000 ms-mint-0.2.4/versioneer.py
```

### Comparing `ms-mint-0.2.3/LICENSE` & `ms-mint-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/PKG-INFO` & `ms-mint-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.3
+Version: 0.2.4
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-0.2.3/README.md` & `ms-mint-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/Mint.py` & `ms-mint-0.2.4/ms_mint/Mint.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/chromatogram.py` & `ms-mint-0.2.4/ms_mint/chromatogram.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/filelock.py` & `ms-mint-0.2.4/ms_mint/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/filters.py` & `ms-mint-0.2.4/ms_mint/filters.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/io.py` & `ms-mint-0.2.4/ms_mint/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 
 from pathlib import Path as P
 from datetime import date
 from pyteomics import mzxml, mzml
 
 try:
     from pyteomics import mzmlb
-
     MZMLB_AVAILABLE = True
-except ImportError:
-    logging.warning("Cound not import pyteomics.mzmlb")
+except ImportError as e:
+    logging.warning(f"Cound not import pyteomics.mzmlb:\n{e}")
     MZMLB_AVAILABLE = False
 
 
 MS_FILE_COLUMNS = [
     "scan_id",
     "ms_level",
     "polarity",
@@ -296,15 +295,15 @@
 
     if read_only:
         return None
 
     data = list(extract_mzmlb(data))
     df = (
         pd.DataFrame.from_dict(data)
-        .set_index(["index", "retentionTime"])
+        .set_index(["index", "retentionTime", "polarity"])
         .apply(pd.Series.explode)
         .reset_index()
         .rename(
             columns={
                 "index": "scan_id",
                 "retentionTime": "scan_time",
                 "m/z array": "mz",
@@ -312,22 +311,28 @@
                 "intensity array": "intensity",
             }
         )
     )
 
     # mzMLb starts scan index with 0
     df["scan_id"] = df["scan_id"] + 1
-    df["polarity"] = None
+    
     df = df[MS_FILE_COLUMNS]
     return df
 
 
 def _extract_mzmlb(data):
-    cols = ["index", "ms level", "retentionTime", "m/z array", "intensity array"]
+    cols = ["index", "ms level", "polarity", "retentionTime", "m/z array", "intensity array"]
     data["retentionTime"] = data["scanList"]["scan"][0]["scan start time"] * 60
+    if 'positive scan' in data.keys():
+        data["polarity"] = '+'
+    elif 'negative scan' in data.keys():
+        data["polarity"] = '-'
+    else:
+        data["polarity"] = None
     return {c: data[c] for c in cols}
 
 
 extract_mzmlb = np.vectorize(_extract_mzmlb)
 
 
 def df_to_numeric(df):
```

### Comparing `ms-mint-0.2.3/ms_mint/matplotlib_tools.py` & `ms-mint-0.2.4/ms_mint/matplotlib_tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/notebook.py` & `ms-mint-0.2.4/ms_mint/notebook.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/pca.py` & `ms-mint-0.2.4/ms_mint/pca.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/plotly_tools.py` & `ms-mint-0.2.4/ms_mint/plotly_tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/plotting.py` & `ms-mint-0.2.4/ms_mint/plotting.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/processing.py` & `ms-mint-0.2.4/ms_mint/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,14 @@
 
     try:
         results = process_ms1_file(filename=filename, targets=targets)
     except Exception as e:
         logging.error(f"process_ms1_files_in_parallel(): {e}")
         results = pd.DataFrame()
 
-    print(len(results))
-
     if (output_fn is not None) and (len(results) > 0):
         append_results(results, output_fn)
         return None
 
     return results
 
 
@@ -86,15 +84,14 @@
     df = ms_file_to_df(filename)
     results = process_ms1(df, targets)
     results["total_intensity"] = df["intensity"].sum()
     results["ms_file"] = os.path.basename(filename)
     results["ms_path"] = os.path.dirname(filename)
     results["ms_file_size"] = os.path.getsize(filename) / 1024 / 1024
     results["peak_score"] = score_peaks(results)
-    print(results)
     return results[MINT_RESULTS_COLUMNS]
 
 
 def process_ms1(df, targets):
     """
     Process MS-1 data with a target list.
 
@@ -187,22 +184,14 @@
     """
 
     float_list_to_comma_sep_str = lambda x: ",".join([str(np.round(i, 4)) for i in x])
     int_list_to_comma_sep_str = lambda x: ",".join([str(int(i)) for i in x])
 
     projection = pd.DataFrame(array[:, [0, 2]], columns=["rt", "int"])
 
-    print("DEBUG extract_ms1_properties")
-    print(array)
-    print(array.dtype)
-    print(array.shape)
-    print(len(projection))
-    print(projection)
-    print(projection.dtypes)
-
     projection["rt"] = projection["rt"].round(2)
     projection["int"] = projection["int"].astype(int)
     projection = projection.groupby("rt").max().reset_index().values
 
     times = array[:, 0]
     masses = array[:, 1]
     intensities = array[:, 2]
```

### Comparing `ms-mint-0.2.3/ms_mint/standards.py` & `ms-mint-0.2.4/ms_mint/standards.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/targets.py` & `ms-mint-0.2.4/ms_mint/targets.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint/tools.py` & `ms-mint-0.2.4/ms_mint/tools.py`

 * *Files identical despite different names*

### Comparing `ms-mint-0.2.3/ms_mint.egg-info/PKG-INFO` & `ms-mint-0.2.4/ms_mint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint
-Version: 0.2.3
+Version: 0.2.4
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-0.2.3/ms_mint.egg-info/SOURCES.txt` & `ms-mint-0.2.4/ms_mint.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 ms_mint/standards.py
 ms_mint/targets.py
 ms_mint/tools.py
 ms_mint.egg-info/PKG-INFO
 ms_mint.egg-info/SOURCES.txt
 ms_mint.egg-info/dependency_links.txt
 ms_mint.egg-info/requires.txt
-ms_mint.egg-info/top_level.txt
+ms_mint.egg-info/top_level.txt
+scripts/ms-mint-convert.py
```

### Comparing `ms-mint-0.2.3/setup.py` & `ms-mint-0.2.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,17 +27,23 @@
     "colorlover",
     "tqdm",
     "ipywidgets",
     "ipyfilechooser",
     "openpyxl",
     "pyarrow",
     "tables",
+    "h5py",
+    "hdf5plugin"
 ]
 
 
+scripts = [
+    "scripts/ms-mint-convert.py"
+]
+
 config = {
     "name": "ms-mint",
     "version": versioneer.get_version(),
     "cmdclass": versioneer.get_cmdclass(),
     "description": "Metabolomics Integrator (Mint)",
     "long_description": long_description,
     "long_description_content_type": "text/markdown",
@@ -49,11 +55,12 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     "python_requires": ">=3.8",
     "install_requires": install_reqs,
     "include_package_data": True,
+    "scripts": scripts
 }
 
 
 setup(**config)
```

### Comparing `ms-mint-0.2.3/versioneer.py` & `ms-mint-0.2.4/versioneer.py`

 * *Files identical despite different names*

