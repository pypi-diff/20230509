# Comparing `tmp/Pulse3D-0.33.2.tar.gz` & `tmp/Pulse3D-0.33.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pulse3D-0.33.2.tar", last modified: Fri May  5 18:01:07 2023, max compression
+gzip compressed data, was "Pulse3D-0.33.3.tar", last modified: Mon May  8 21:56:35 2023, max compression
```

## Comparing `Pulse3D-0.33.2.tar` & `Pulse3D-0.33.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.345611 Pulse3D-0.33.2/mantarray-magnet-finding/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.341611 Pulse3D-0.33.2/mantarray-magnet-finding/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.345611 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-05 18:00:03.000000 Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 18:01:07.353612 Pulse3D-0.33.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.341611 Pulse3D-0.33.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/src/Pulse3D.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-05 18:01:07.000000 Pulse3D-0.33.2/src/Pulse3D.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-05 18:01:07.000000 Pulse3D-0.33.2/src/Pulse3D.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:00:52.000000 Pulse3D-0.33.2/src/Pulse3D.egg-info/not-zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.345611 Pulse3D-0.33.2/src/mantarray_magnet_finding/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-05 18:00:31.000000 Pulse3D-0.33.2/src/mantarray_magnet_finding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:01:07.349611 Pulse3D-0.33.2/src/pulse3D/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/compression_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    46415 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/magnet_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/nb_peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/peak_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    33482 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/plate_recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/stimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-05 17:59:59.000000 Pulse3D-0.33.2/src/pulse3D/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.907337 Pulse3D-0.33.3/mantarray-magnet-finding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.907337 Pulse3D-0.33.3/mantarray-magnet-finding/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-08 21:55:17.000000 Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 21:56:35.915337 Pulse3D-0.33.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.907337 Pulse3D-0.33.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/src/Pulse3D.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-08 21:56:35.000000 Pulse3D-0.33.3/src/Pulse3D.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-08 21:56:35.000000 Pulse3D-0.33.3/src/Pulse3D.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:56:18.000000 Pulse3D-0.33.3/src/Pulse3D.egg-info/not-zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/src/mantarray_magnet_finding/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-08 21:55:52.000000 Pulse3D-0.33.3/src/mantarray_magnet_finding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:35.911337 Pulse3D-0.33.3/src/pulse3D/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/compression_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46415 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/magnet_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34854 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/nb_peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/peak_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33482 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/plate_recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/stimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-08 21:55:09.000000 Pulse3D-0.33.3/src/pulse3D/utils.py
```

### Comparing `Pulse3D-0.33.2/LICENSE` & `Pulse3D-0.33.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/PKG-INFO` & `Pulse3D-0.33.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.2
+Version: 0.33.3
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.2/mantarray-magnet-finding/setup.py` & `Pulse3D-0.33.3/mantarray-magnet-finding/setup.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.3/mantarray-magnet-finding/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/setup.py` & `Pulse3D-0.33.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extensions = [Extension("pulse3D.compression_cy", [os.path.join("src", "pulse3D", "compression_cy") + ext])]
 if USE_CYTHON:
     # cythonizing compression_cy.pyx with kwarg annotate=True will help when optimizing the code by enabling generation of the html annotation file
     extensions = cythonize(extensions, annotate=False)
 
 setup(
     name="Pulse3D",
-    version="0.33.2",
+    version="0.33.3",
     description="Pulse3D Analysis Platform",
     url="https://github.com/CuriBio/Pulse3D",
     project_urls={"Documentation": "https://pulse3D.readthedocs.io/en/latest/"},
     author="Curi Bio",
     author_email="contact@curibio.com",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `Pulse3D-0.33.2/src/Pulse3D.egg-info/PKG-INFO` & `Pulse3D-0.33.3/src/Pulse3D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pulse3D
-Version: 0.33.2
+Version: 0.33.3
 Summary: Pulse3D Analysis Platform
 Home-page: https://github.com/CuriBio/Pulse3D
 Author: Curi Bio
 Author-email: contact@curibio.com
 License: MIT
 Project-URL: Documentation, https://pulse3D.readthedocs.io/en/latest/
 Classifier: Development Status :: 1 - Planning
```

### Comparing `Pulse3D-0.33.2/src/Pulse3D.egg-info/SOURCES.txt` & `Pulse3D-0.33.3/src/Pulse3D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/mantarray_magnet_finding/magnet_finding.py` & `Pulse3D-0.33.3/src/mantarray_magnet_finding/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/mantarray_magnet_finding/utils.py` & `Pulse3D-0.33.3/src/mantarray_magnet_finding/utils.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/compression_cy.pyx` & `Pulse3D-0.33.3/src/pulse3D/compression_cy.pyx`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/constants.py` & `Pulse3D-0.33.3/src/pulse3D/constants.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/excel_writer.py` & `Pulse3D-0.33.3/src/pulse3D/excel_writer.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/exceptions.py` & `Pulse3D-0.33.3/src/pulse3D/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/magnet_finding.py` & `Pulse3D-0.33.3/src/pulse3D/magnet_finding.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/metrics.py` & `Pulse3D-0.33.3/src/pulse3D/metrics.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/nb_peak_detection.py` & `Pulse3D-0.33.3/src/pulse3D/nb_peak_detection.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Optional
 from typing import Tuple
 
 from nptyping import NDArray
 import numpy as np
 from pulse3D.exceptions import InvalidValleySearchDurationError
 from pulse3D.exceptions import TooFewPeaksDetectedError
+from pulse3D.transforms import get_time_window_indices
 from scipy import signal
 from scipy.optimize import curve_fit
 
 from .constants import DEFAULT_NB_HEIGHT_FACTOR
 from .constants import DEFAULT_NB_NOISE_PROMINENCE_FACTOR
 from .constants import DEFAULT_NB_RELATIVE_PROMINENCE_FACTOR
 from .constants import DEFAULT_NB_UPSLOPE_DUR
@@ -25,26 +26,30 @@
 def quadratic(x, a, b, c):
     return a * (x**2) + b * x + c
 
 
 # TODO ? prefix args with peak_ or valley_ so it's more clear which they affect
 def noise_based_peak_finding(
     tissue_data: NDArray[(2, Any), float],
+    start_time: float = 0,
+    end_time: float = np.inf,
     noise_prominence_factor: float = DEFAULT_NB_NOISE_PROMINENCE_FACTOR,
     relative_prominence_factor: Optional[float] = DEFAULT_NB_RELATIVE_PROMINENCE_FACTOR,
     width_factors: Tuple[float, float] = DEFAULT_NB_WIDTH_FACTORS,
     height_factor: float = DEFAULT_NB_HEIGHT_FACTOR,
     max_frequency: Optional[float] = None,
     valley_search_duration: float = DEFAULT_NB_VALLEY_SEARCH_DUR,
     upslope_duration: float = DEFAULT_NB_UPSLOPE_DUR,
     upslope_noise_allowance_duration: float = DEFAULT_NB_UPSLOPE_NOISE_ALLOWANCE_DUR,
 ):
     """
     Args:
         tissue_data: Waveform Amplitude (force/displacement/etc.) v. Time array. Time values should be in seconds. Data should be interpolated and normalized
+        start_time: The earliest timepoint to consider
+        end_time: The greatest timepoint to consider
         noise_prominence_factor: The minimum required SNR of a peak
         relative_prominence_factor: If specified, the prominence of each peak relative to the tallest peak will be taken into consideration.
             If this falls below the noise-based prominence threshold determined by `noise_prominence_factor`, that will be used instead.
         width_factor: The minimum and maximum width in seconds of a peak required to be considered
         height_factor: The minimum height of a peak required to be considered. This should be given in the unit of measure as the Waveform Amplitude values in `tissue_data`
         max_frequency: The maximum frequency (Hz) at which a peak can occur. Specifically, this is used to calculate the minimum required distance between adjacent peaks.
             For example, if the value given is 1, then at most peaks will occur at 1Hz. In other words, the peaks will be no closer than 1 second.
@@ -54,15 +59,16 @@
             If this window includes a previous peak then for that peak the window will automatically be shortened
         upslope_duration: The min duration of time in seconds through which the waveform values must continuously rise in order to be considered an upslope.
         upslope_noise_allowance_duration: The max duration of time in seconds in the upslope in which there is an amplitude decrease which can be tolerated within a single upslope.
 
     Returns:
         A tuple containing an of the indices of the peaks and an array of the indices of valleys
     """
-    time_axis, waveform = tissue_data
+    window_indices = get_time_window_indices(tissue_data[0], start_time, end_time)
+    time_axis, waveform = tissue_data[:, window_indices]
 
     # TODO split into subfunctions, one for finding peaks and the other for finding valleys
 
     # extract sample frequency from time_axis (assumes sampling freq is constant)
     sample_freq = 1 / (time_axis[1] - time_axis[0])
 
     if max_frequency:
@@ -202,8 +208,12 @@
 
         valley_indices.append(valley_index)
 
     valleys = np.array(
         [peak - (window - index) for peak, index, window in zip(peaks, valley_indices, search_windows)]
     )
 
+    # indices are only valid with the given window, so adjust to match original signal
+    peaks += window_indices[0]
+    valleys += window_indices[0]
+
     return peaks, valleys
```

### Comparing `Pulse3D-0.33.2/src/pulse3D/peak_detection.py` & `Pulse3D-0.33.3/src/pulse3D/peak_detection.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/plate_recording.py` & `Pulse3D-0.33.3/src/pulse3D/plate_recording.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/plotting.py` & `Pulse3D-0.33.3/src/pulse3D/plotting.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/stimulation.py` & `Pulse3D-0.33.3/src/pulse3D/stimulation.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/transforms.py` & `Pulse3D-0.33.3/src/pulse3D/transforms.py`

 * *Files identical despite different names*

### Comparing `Pulse3D-0.33.2/src/pulse3D/utils.py` & `Pulse3D-0.33.3/src/pulse3D/utils.py`

 * *Files identical despite different names*

