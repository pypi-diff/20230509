# Comparing `tmp/steam-pysigma-2023.5.2.tar.gz` & `tmp/steam-pysigma-2023.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.5.2.tar", last modified: Fri May  5 13:50:28 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.5.4.tar", last modified: Tue May  9 14:28:20 2023, max compression
```

## Comparing `steam-pysigma-2023.5.2.tar` & `steam-pysigma-2023.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 13:50:28.700742 steam-pysigma-2023.5.2/
--rw-rw-rw-   0        0        0     1030 2023-05-05 13:50:28.699741 steam-pysigma-2023.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 13:50:28.701741 steam-pysigma-2023.5.2/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-05-05 13:49:36.000000 steam-pysigma-2023.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:50:28.687478 steam-pysigma-2023.5.2/steam_pysigma/
--rw-rw-rw-   0        0        0     2484 2023-05-05 08:55:14.000000 steam-pysigma-2023.5.2/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.2/steam_pysigma/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.2/steam_pysigma/helpers.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.2/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-05-05 13:50:28.697728 steam-pysigma-2023.5.2/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 13:50:24.000000 steam-pysigma-2023.5.2/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 14:28:20.783859 steam-pysigma-2023.5.4/
+-rw-rw-rw-   0        0        0     1030 2023-05-09 14:28:20.782859 steam-pysigma-2023.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:28:20.783859 steam-pysigma-2023.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-05-09 14:27:36.000000 steam-pysigma-2023.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:28:20.763860 steam-pysigma-2023.5.4/steam_pysigma/
+-rw-rw-rw-   0        0        0     2252 2023-05-09 08:07:19.000000 steam-pysigma-2023.5.4/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.5.4/steam_pysigma/__init__.py
+-rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.5.4/steam_pysigma/helpers.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.5.4/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:28:20.780859 steam-pysigma-2023.5.4/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-05-09 14:28:15.000000 steam-pysigma-2023.5.4/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-09 14:28:15.000000 steam-pysigma-2023.5.4/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:28:15.000000 steam-pysigma-2023.5.4/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-05-09 14:28:15.000000 steam-pysigma-2023.5.4/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 14:28:15.000000 steam-pysigma-2023.5.4/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.5.2/PKG-INFO` & `steam-pysigma-2023.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.2
+Version: 2023.5.4
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,SIGMA
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.5.2/README.md` & `steam-pysigma-2023.5.4/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.2/setup.py` & `steam-pysigma-2023.5.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.5.2",
+    version="2023.5.4",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.5.2/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.5.4/steam_pysigma/MainSIGMA.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from pathlib import Path
 
 from steam_pysigma.comsol.BuildComsolModel import BuildComsolModel
 from steam_pysigma.data import DataSIGMA as dS
 import yaml
 from steam_pysigma.utils import Util
-import steam_pysigma.pysigma as ps
 import logging
 
 
 class MainSIGMA:
     """
         Class to generate SIGMA models
     """
@@ -19,35 +18,30 @@
         """
               Main class for working with FiQuS simulations
               :param input_file_path: input file full path
               :param verbose: if True, more info is printed in the console
               """
         self.start_folder = os.getcwd()
         self.wrk_folder = model_folder
-        self.g = ps.GatewaySIGMA()
 
         logger = logging.getLogger()
         if verbose:
             logger.setLevel(logging.INFO)
         else:
             logger.setLevel(logging.DEBUG)
 
-        #if Path.exists(system_settings_path):
-           # with open(system_settings_path, 'r') as stream:
-                #self.settings = yaml.safe_load(stream)
         self.settings = system_settings
         # Load yaml input file
         if not dm:
             self.dm = Util.FilesAndFolders.read_data_from_yaml(input_file_path, dS.DataSIGMA)
         else:
             self.dm = dm
-        self.sdm = Util.FilesAndFolders.read_data_from_yaml(f'{input_file_path[:-5]}.set', dS.MultipoleSettings)
-        self.roxie_data = Util.FilesAndFolders.read_data_from_yaml(f'{input_file_path[:-5]}.geom', dS.SIGMAGeometry)
-
-        # domains = self.build_domains()
+        base_file_name = os.path.splitext(input_file_path)[0]
+        self.sdm = Util.FilesAndFolders.read_data_from_yaml(f'{base_file_name}.set', dS.MultipoleSettings)
+        self.roxie_data = Util.FilesAndFolders.read_data_from_yaml(f'{base_file_name}.geom', dS.SIGMAGeometry)
 
         BuildComsolModel(self.dm, self.sdm, self.settings, self.wrk_folder, self.roxie_data)
 
 
 if __name__ == "__main__":
     # if len(sys.argv) < 4:
     #     mp = MainFiQuS(sys.argv[1], sys.argv[2])
```

### Comparing `steam-pysigma-2023.5.2/steam_pysigma/helpers.py` & `steam-pysigma-2023.5.4/steam_pysigma/helpers.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.2/steam_pysigma/pysigma.py` & `steam-pysigma-2023.5.4/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.5.2/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.5.4/steam_pysigma.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.5.2
+Version: 2023.5.4
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,SIGMA
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

