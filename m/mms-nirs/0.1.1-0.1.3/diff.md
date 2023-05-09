# Comparing `tmp/mms_nirs-0.1.1.tar.gz` & `tmp/mms_nirs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_nirs-0.1.1.tar", max compression
+gzip compressed data, was "mms_nirs-0.1.3.tar", max compression
```

## Comparing `mms_nirs-0.1.1.tar` & `mms_nirs-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.1.1/README.md
--rw-r--r--   0        0        0      611 2023-05-09 15:01:31.364702 mms_nirs-0.1.1/mms_nirs/UCLN/DefaultValues.py
--rw-r--r--   0        0        0     3341 2023-05-09 15:01:31.364702 mms_nirs-0.1.1/mms_nirs/UCLN/UCLN.py
--rw-r--r--   0        0        0      132 2023-05-09 15:01:31.364702 mms_nirs-0.1.1/mms_nirs/UCLN/__init__.py
--rw-r--r--   0        0        0     3875 2023-05-09 15:01:31.364702 mms_nirs-0.1.1/mms_nirs/UCLN/defaults.csv
--rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.1.1/mms_nirs/__init__.py
--rw-r--r--   0        0        0      892 2023-05-09 15:18:32.124293 mms_nirs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 mms_nirs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.1.3/README.md
+-rw-r--r--   0        0        0      662 2023-05-09 17:15:42.681482 mms_nirs-0.1.3/mms_nirs/UCLN/DefaultValues.py
+-rw-r--r--   0        0        0     3304 2023-05-09 17:15:42.681482 mms_nirs-0.1.3/mms_nirs/UCLN/UCLN.py
+-rw-r--r--   0        0        0      132 2023-05-09 15:01:31.364702 mms_nirs-0.1.3/mms_nirs/UCLN/__init__.py
+-rw-r--r--   0        0        0     3876 2023-05-09 17:15:42.681482 mms_nirs-0.1.3/mms_nirs/UCLN/defaults.csv
+-rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.1.3/mms_nirs/__init__.py
+-rw-r--r--   0        0        0      892 2023-05-09 17:17:07.741448 mms_nirs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 mms_nirs-0.1.3/PKG-INFO
```

### Comparing `mms_nirs-0.1.1/mms_nirs/UCLN/DefaultValues.py` & `mms_nirs-0.1.3/mms_nirs/UCLN/DefaultValues.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,7 +16,8 @@
             engine="pyarrow",
             index_col="wavelength",
         )
 
         self.extinction_coefficients = df[species].values
         self.wavelength_dependency = np.array(df["wl_dep"].values)
         self.spectra_wavelengths = np.array(df.index.values)
+        self.spectra_wavelengths = df.index.values
```

### Comparing `mms_nirs-0.1.1/mms_nirs/UCLN/UCLN.py` & `mms_nirs-0.1.3/mms_nirs/UCLN/UCLN.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,16 +83,14 @@
 
         # Note: The inverse of the matrix isn't unique meaning these differ
         # from the MATLAB equivalents
         ext_coeffs_inv: np.ndarray = linalg.pinv(
             self.constants.extinction_coefficients
         )
 
-        print(ext_coeffs_inv.shape)
-
         optode_dist = self.constants.optode_dist
         dpf = self.constants.dpf
 
         if self.attenuation_interp_wavelength_dependency is not None:
             return np.transpose(
                 np.matmul(
                     ext_coeffs_inv,
```

### Comparing `mms_nirs-0.1.1/mms_nirs/UCLN/defaults.csv` & `mms_nirs-0.1.3/mms_nirs/UCLN/defaults.csv`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 790,0.8005,0.9264,2.1506,0.9945
 791,0.807, 0.9143,2.1572,0.9937
 792,0.8134,0.9034,2.1638,0.9929
 793,0.8197,0.8939,2.1763,0.9922
 794,0.8264,0.8844,2.1887,0.9914
 795,0.833, 0.8752,2.2015,0.9906
 796,0.8392,0.8676,2.2142,0.9883
-797,0.8458,0.8600,.2279,0.9859
+797,0.8458,0.8600,2.2279,0.9859
 798,0.8524,0.8524,2.2416,0.9835
 799,0.8588,0.8461,2.2518,0.9812
 800,0.8653,0.8399,2.2619,0.9788
 801,0.8716,0.8338,2.2666,0.9779
 802,0.878, 0.8285,2.2713,0.977
 803,0.8845,0.8237,2.2762,0.976
 804,0.8909,0.819, 2.2812,0.9751
```

### Comparing `mms_nirs-0.1.1/pyproject.toml` & `mms_nirs-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms-nirs"
-version = "0.1.1"
+version = "0.1.3"
 description = "Algorithms used in the multimodal spectroscopy group to process NIRS data"
 authors = ["Josh Buckland, <joshua.russell-buckland@ucl.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "mms_nirs" }]
 
 [tool.poetry.dependencies]
```

### Comparing `mms_nirs-0.1.1/PKG-INFO` & `mms_nirs-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-nirs
-Version: 0.1.1
+Version: 0.1.3
 Summary: Algorithms used in the multimodal spectroscopy group to process NIRS data
 License: MIT
 Author: Josh Buckland,
 Author-email: joshua.russell-buckland@ucl.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

