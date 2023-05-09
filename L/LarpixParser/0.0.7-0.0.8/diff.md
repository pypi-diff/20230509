# Comparing `tmp/LarpixParser-0.0.7.tar.gz` & `tmp/LarpixParser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LarpixParser-0.0.7.tar", last modified: Mon Apr 24 23:01:34 2023, max compression
+gzip compressed data, was "LarpixParser-0.0.8.tar", last modified: Tue May  9 03:49:36 2023, max compression
```

## Comparing `LarpixParser-0.0.7.tar` & `LarpixParser-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.410316 LarpixParser-0.0.7/
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1061 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/LICENSE
--rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-24 23:01:34.407021 LarpixParser-0.0.7/PKG-INFO
--rw-r--r--   0 cyifan   (18025) nu        (1123)     5354 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/README.md
--rw-r--r--   0 cyifan   (18025) nu        (1123)       38 2023-04-24 23:01:34.408553 LarpixParser-0.0.7/setup.cfg
--rw-r--r--   0 cyifan   (18025) nu        (1123)      983 2023-04-24 22:59:56.000000 LarpixParser-0.0.7/setup.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.090033 LarpixParser-0.0.7/src/
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.116098 LarpixParser-0.0.7/src/LarpixParser/
--rw-r--r--   0 cyifan   (18025) nu        (1123)       31 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/__init__.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)      685 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/charge_calibration.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.245092 LarpixParser-0.0.7/src/LarpixParser/config_repo/
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1682 2023-04-24 21:06:45.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/2x2.yaml
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.267162 LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/
--rw-r--r--   0 cyifan   (18025) nu        (1123)  5282199 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl
--rw-r--r--   0 cyifan   (18025) nu        (1123) 27857539 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1567 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/module0.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)   134242 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)   330018 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3880 2023-04-24 21:07:29.000000 LarpixParser-0.0.7/src/LarpixParser/config_repo/ndlar-module.yaml
--rw-r--r--   0 cyifan   (18025) nu        (1123)      117 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/coord_transform.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1847 2023-04-24 21:05:25.000000 LarpixParser-0.0.7/src/LarpixParser/event_parser.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     4000 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/geom_to_dict.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1400 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/get_charge.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1963 2023-04-24 21:44:16.000000 LarpixParser-0.0.7/src/LarpixParser/get_raw_coord.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3443 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/get_vdrift.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     2240 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/hit_parser.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     1287 2023-04-20 22:47:21.000000 LarpixParser-0.0.7/src/LarpixParser/units.py
--rw-r--r--   0 cyifan   (18025) nu        (1123)     3729 2023-04-24 21:06:21.000000 LarpixParser-0.0.7/src/LarpixParser/util.py
-drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-04-24 23:01:34.130975 LarpixParser-0.0.7/src/LarpixParser.egg-info/
--rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/PKG-INFO
--rw-r--r--   0 cyifan   (18025) nu        (1123)      954 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/SOURCES.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)        1 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/dependency_links.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)       16 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/requires.txt
--rw-r--r--   0 cyifan   (18025) nu        (1123)       13 2023-04-24 23:01:33.000000 LarpixParser-0.0.7/src/LarpixParser.egg-info/top_level.txt
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-05-09 03:49:36.720340 LarpixParser-0.0.8/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1061 2023-05-09 03:13:06.000000 LarpixParser-0.0.8/LICENSE
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-05-09 03:49:36.717140 LarpixParser-0.0.8/PKG-INFO
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     5354 2023-05-09 03:13:06.000000 LarpixParser-0.0.8/README.md
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       38 2023-05-09 03:49:36.718404 LarpixParser-0.0.8/setup.cfg
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      983 2023-05-09 03:45:30.000000 LarpixParser-0.0.8/setup.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-05-09 03:49:36.413534 LarpixParser-0.0.8/src/
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-05-09 03:49:36.546411 LarpixParser-0.0.8/src/LarpixParser/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       31 2023-05-09 03:13:06.000000 LarpixParser-0.0.8/src/LarpixParser/__init__.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      685 2023-05-09 03:13:06.000000 LarpixParser-0.0.8/src/LarpixParser/charge_calibration.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-05-09 03:49:36.672129 LarpixParser-0.0.8/src/LarpixParser/config_repo/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1682 2023-05-09 03:13:06.000000 LarpixParser-0.0.8/src/LarpixParser/config_repo/2x2.yaml
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-05-09 03:49:36.685315 LarpixParser-0.0.8/src/LarpixParser/config_repo/dict_repo/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)  5282199 2023-05-09 03:13:06.000000 LarpixParser-0.0.8/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl
+-rw-r--r--   0 cyifan   (18025) nu        (1123) 27857539 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1567 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/config_repo/module0.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)   134242 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)   330018 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3880 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/config_repo/ndlar-module.yaml
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      117 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/coord_transform.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     2082 2023-05-09 03:45:03.000000 LarpixParser-0.0.8/src/LarpixParser/event_parser.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     4000 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/geom_to_dict.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1400 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/get_charge.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1963 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/get_raw_coord.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3443 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/get_vdrift.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     2240 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/hit_parser.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     1287 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/units.py
+-rw-r--r--   0 cyifan   (18025) nu        (1123)     3729 2023-05-09 03:13:07.000000 LarpixParser-0.0.8/src/LarpixParser/util.py
+drwxr-sr-x   0 cyifan   (18025) nu        (1123)        0 2023-05-09 03:49:36.661001 LarpixParser-0.0.8/src/LarpixParser.egg-info/
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      578 2023-05-09 03:49:36.000000 LarpixParser-0.0.8/src/LarpixParser.egg-info/PKG-INFO
+-rw-r--r--   0 cyifan   (18025) nu        (1123)      954 2023-05-09 03:49:36.000000 LarpixParser-0.0.8/src/LarpixParser.egg-info/SOURCES.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)        1 2023-05-09 03:49:36.000000 LarpixParser-0.0.8/src/LarpixParser.egg-info/dependency_links.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       16 2023-05-09 03:49:36.000000 LarpixParser-0.0.8/src/LarpixParser.egg-info/requires.txt
+-rw-r--r--   0 cyifan   (18025) nu        (1123)       13 2023-05-09 03:49:36.000000 LarpixParser-0.0.8/src/LarpixParser.egg-info/top_level.txt
```

### Comparing `LarpixParser-0.0.7/LICENSE` & `LarpixParser-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/PKG-INFO` & `LarpixParser-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LarpixParser
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package parsing the larpix output to hit-level
 Home-page: https://github.com/YifanC/larpix_readout_parser
 Author: Yifan C. and others
 Author-email: cyifan@slac.stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LarpixParser-0.0.7/README.md` & `LarpixParser-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/setup.py` & `LarpixParser-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 import setuptools
 
-VER = "0.0.7"
+VER = "0.0.8"
 
 setuptools.setup(
     name="LarpixParser",
     version=VER,
     author="Yifan C. and others",
     author_email="cyifan@slac.stanford.edu",
     description="A package parsing the larpix output to hit-level",
```

### Comparing `LarpixParser-0.0.7/src/LarpixParser/charge_calibration.py` & `LarpixParser-0.0.8/src/LarpixParser/charge_calibration.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/config_repo/2x2.yaml` & `LarpixParser-0.0.8/src/LarpixParser/config_repo/2x2.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl` & `LarpixParser-0.0.8/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-2.3.16.pkl`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl` & `LarpixParser-0.0.8/src/LarpixParser/config_repo/dict_repo/multi_tile_layout-3.0.40.pkl`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/config_repo/module0.yaml` & `LarpixParser-0.0.8/src/LarpixParser/config_repo/module0.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml` & `LarpixParser-0.0.8/src/LarpixParser/config_repo/multi_tile_layout-2.3.16.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml` & `LarpixParser-0.0.8/src/LarpixParser/config_repo/multi_tile_layout-3.0.40.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/config_repo/ndlar-module.yaml` & `LarpixParser-0.0.8/src/LarpixParser/config_repo/ndlar-module.yaml`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/event_parser.py` & `LarpixParser-0.0.8/src/LarpixParser/event_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,28 +18,33 @@
     t0 = np.array(t0)
 
     threshold = 40 #us
     t0_ev = np.delete(t0, np.argwhere(np.ediff1d(t0) <= threshold) + 1)
 
     return t0_ev
 
-def get_t0_event(vertices, run_config, time_parser='t_event'):
+def get_t0_event(vertices, run_config, event_parser='eventID', time_parser='t_event'):
     try:
         dt_window = run_config['beam_duration']
     except:
         dt_window = 0
         print("Found no 'beam_duration' in the configuration file")
 
     if time_parser in vertices.dtype.names and not (np.all(vertices[time_parser]) == 0):
-        t0_ev = (np.unique(vertices[time_parser]) + dt_window *0.5)
+        uniq_ev, counts = np.unique(vertices['eventID'], return_counts=True)
+        idx = np.cumsum(counts) - 1
+        t0_ev = np.take(vertices[time_parser], idx) + dt_window *0.5
     else:
         raise ValueError("True event time is not given!")
 
     return t0_ev
 
+def get_eventid(vertices, event_parser='eventID'):
+    return np.unique(vertices[event_parser])
+
 def packet_to_eventid(assn, tracks, event_parser='eventID'):
     '''
     Assoiciate packet to eventID.
     
     Arguments
     ---------
     assn : array_like
```

### Comparing `LarpixParser-0.0.7/src/LarpixParser/geom_to_dict.py` & `LarpixParser-0.0.8/src/LarpixParser/geom_to_dict.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/get_charge.py` & `LarpixParser-0.0.8/src/LarpixParser/get_charge.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/get_raw_coord.py` & `LarpixParser-0.0.8/src/LarpixParser/get_raw_coord.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/get_vdrift.py` & `LarpixParser-0.0.8/src/LarpixParser/get_vdrift.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/hit_parser.py` & `LarpixParser-0.0.8/src/LarpixParser/hit_parser.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/units.py` & `LarpixParser-0.0.8/src/LarpixParser/units.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser/util.py` & `LarpixParser-0.0.8/src/LarpixParser/util.py`

 * *Files identical despite different names*

### Comparing `LarpixParser-0.0.7/src/LarpixParser.egg-info/PKG-INFO` & `LarpixParser-0.0.8/src/LarpixParser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LarpixParser
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package parsing the larpix output to hit-level
 Home-page: https://github.com/YifanC/larpix_readout_parser
 Author: Yifan C. and others
 Author-email: cyifan@slac.stanford.edu
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `LarpixParser-0.0.7/src/LarpixParser.egg-info/SOURCES.txt` & `LarpixParser-0.0.8/src/LarpixParser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

