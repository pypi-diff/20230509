# Comparing `tmp/pawflim-1.0.0.tar.gz` & `tmp/pawflim-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pawflim-1.0.0.tar", last modified: Tue May  9 19:10:39 2023, max compression
+gzip compressed data, was "pawflim-1.0.1.tar", last modified: Tue May  9 19:18:00 2023, max compression
```

## Comparing `pawflim-1.0.0.tar` & `pawflim-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 maurosilber   (501) staff       (20)        0 2023-05-09 19:10:39.113216 pawflim-1.0.0/
-drwxr-xr-x   0 maurosilber   (501) staff       (20)        0 2023-05-09 19:10:39.110739 pawflim-1.0.0/.github/
-drwxr-xr-x   0 maurosilber   (501) staff       (20)        0 2023-05-09 19:10:39.111765 pawflim-1.0.0/.github/workflows/
--rw-r--r--   0 maurosilber   (501) staff       (20)      501 2023-05-09 19:09:54.000000 pawflim-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 maurosilber   (501) staff       (20)      572 2023-05-09 19:09:54.000000 pawflim-1.0.0/.github/workflows/test.yml
--rw-r--r--   0 maurosilber   (501) staff       (20)     1073 2023-05-09 19:09:54.000000 pawflim-1.0.0/LICENSE
--rw-r--r--   0 maurosilber   (501) staff       (20)     2660 2023-05-09 19:10:39.113064 pawflim-1.0.0/PKG-INFO
--rw-r--r--   0 maurosilber   (501) staff       (20)      605 2023-05-09 19:09:54.000000 pawflim-1.0.0/README.md
-drwxr-xr-x   0 maurosilber   (501) staff       (20)        0 2023-05-09 19:10:39.111879 pawflim-1.0.0/examples/
--rw-r--r--   0 maurosilber   (501) staff       (20)   153455 2023-05-09 19:09:54.000000 pawflim-1.0.0/examples/simulated_data.ipynb
--rw-r--r--   0 maurosilber   (501) staff       (20)     1359 2023-05-09 19:09:54.000000 pawflim-1.0.0/pyproject.toml
--rw-r--r--   0 maurosilber   (501) staff       (20)       18 2023-05-09 19:09:54.000000 pawflim-1.0.0/requirements.test.txt
--rw-r--r--   0 maurosilber   (501) staff       (20)       25 2023-05-09 19:09:54.000000 pawflim-1.0.0/requirements.txt
--rw-r--r--   0 maurosilber   (501) staff       (20)       38 2023-05-09 19:10:39.113258 pawflim-1.0.0/setup.cfg
-drwxr-xr-x   0 maurosilber   (501) staff       (20)        0 2023-05-09 19:10:39.112200 pawflim-1.0.0/src/
-drwxr-xr-x   0 maurosilber   (501) staff       (20)        0 2023-05-09 19:10:39.112855 pawflim-1.0.0/src/pawflim.egg-info/
--rw-r--r--   0 maurosilber   (501) staff       (20)     2660 2023-05-09 19:10:39.000000 pawflim-1.0.0/src/pawflim.egg-info/PKG-INFO
--rw-r--r--   0 maurosilber   (501) staff       (20)      367 2023-05-09 19:10:39.000000 pawflim-1.0.0/src/pawflim.egg-info/SOURCES.txt
--rw-r--r--   0 maurosilber   (501) staff       (20)        1 2023-05-09 19:10:39.000000 pawflim-1.0.0/src/pawflim.egg-info/dependency_links.txt
--rw-r--r--   0 maurosilber   (501) staff       (20)       49 2023-05-09 19:10:39.000000 pawflim-1.0.0/src/pawflim.egg-info/requires.txt
--rw-r--r--   0 maurosilber   (501) staff       (20)        1 2023-05-09 19:10:39.000000 pawflim-1.0.0/src/pawflim.egg-info/top_level.txt
--rw-r--r--   0 maurosilber   (501) staff       (20)     3795 2023-05-09 19:09:54.000000 pawflim-1.0.0/src/pawflim.py
--rw-r--r--   0 maurosilber   (501) staff       (20)      666 2023-05-09 19:09:54.000000 pawflim-1.0.0/src/test_pawflim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.273449 pawflim-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.265449 pawflim-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.269449 pawflim-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-09 19:17:47.000000 pawflim-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 19:17:47.000000 pawflim-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-09 19:17:47.000000 pawflim-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-09 19:18:00.273449 pawflim-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-09 19:17:47.000000 pawflim-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.269449 pawflim-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   153455 2023-05-09 19:17:47.000000 pawflim-1.0.1/examples/simulated_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-09 19:17:47.000000 pawflim-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 19:17:47.000000 pawflim-1.0.1/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 19:17:47.000000 pawflim-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:18:00.273449 pawflim-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.273449 pawflim-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:18:00.273449 pawflim-1.0.1/src/pawflim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:18:00.000000 pawflim-1.0.1/src/pawflim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-09 19:17:47.000000 pawflim-1.0.1/src/pawflim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-09 19:17:47.000000 pawflim-1.0.1/src/test_pawflim.py
```

### Comparing `pawflim-1.0.0/.github/workflows/test.yml` & `pawflim-1.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.0/LICENSE` & `pawflim-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.0/PKG-INFO` & `pawflim-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawflim
-Version: 1.0.0
+Version: 1.0.1
 Summary: Denoising via adaptive binning for FLIM datasets.
 Author-email: Mauro Silberberg <maurosilber@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mauro Silberberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,9 +63,9 @@
 
 denoised = pawflim(data, n_sigmas=2)
 
 phasor = denoised[1] / denoised[0]
 ```
 
 See the notebook in
-[examples](https://github.com/maurosilber/binlets-paper/blob/main/examples/simulated_data.ipynb)
+[examples](https://github.com/maurosilber/pawflim/blob/main/examples/simulated_data.ipynb)
 for an example with simulated data.
```

### Comparing `pawflim-1.0.0/README.md` & `pawflim-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,9 +21,9 @@
 
 denoised = pawflim(data, n_sigmas=2)
 
 phasor = denoised[1] / denoised[0]
 ```
 
 See the notebook in
-[examples](https://github.com/maurosilber/binlets-paper/blob/main/examples/simulated_data.ipynb)
+[examples](https://github.com/maurosilber/pawflim/blob/main/examples/simulated_data.ipynb)
 for an example with simulated data.
```

### Comparing `pawflim-1.0.0/examples/simulated_data.ipynb` & `pawflim-1.0.1/examples/simulated_data.ipynb`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.0/pyproject.toml` & `pawflim-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawflim-1.0.0/src/pawflim.egg-info/PKG-INFO` & `pawflim-1.0.1/src/pawflim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawflim
-Version: 1.0.0
+Version: 1.0.1
 Summary: Denoising via adaptive binning for FLIM datasets.
 Author-email: Mauro Silberberg <maurosilber@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mauro Silberberg
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,9 +63,9 @@
 
 denoised = pawflim(data, n_sigmas=2)
 
 phasor = denoised[1] / denoised[0]
 ```
 
 See the notebook in
-[examples](https://github.com/maurosilber/binlets-paper/blob/main/examples/simulated_data.ipynb)
+[examples](https://github.com/maurosilber/pawflim/blob/main/examples/simulated_data.ipynb)
 for an example with simulated data.
```

### Comparing `pawflim-1.0.0/src/pawflim.py` & `pawflim-1.0.1/src/pawflim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 from binlets import binlets
 from scipy import stats
 
 
 def phasor(R0, Rn, *, mask=None):
     """Compute phasor by normalizing with zeroth harmonic.
```

### Comparing `pawflim-1.0.0/src/test_pawflim.py` & `pawflim-1.0.1/src/test_pawflim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import hypothesis
 import hypothesis.extra.numpy as st_np
 import hypothesis.strategies as st
 import numpy as np
 
 from .pawflim import _inverse
```

