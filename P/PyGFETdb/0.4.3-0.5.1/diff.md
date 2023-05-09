# Comparing `tmp/PyGFETdb-0.4.3.tar.gz` & `tmp/PyGFETdb-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyGFETdb-0.4.3.tar", last modified: Wed Jun  1 09:56:13 2022, max compression
+gzip compressed data, was "PyGFETdb-0.5.1.tar", last modified: Tue May  9 17:35:40 2023, max compression
```

## Comparing `PyGFETdb-0.4.3.tar` & `PyGFETdb-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2022-06-01 09:56:13.000000 PyGFETdb-0.4.3/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       56 2022-06-01 09:44:33.000000 PyGFETdb-0.4.3/MANIFEST.in
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1140 2022-06-01 09:56:13.000000 PyGFETdb-0.4.3/PKG-INFO
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2022-06-01 09:56:13.000000 PyGFETdb-0.4.3/PyGFETdb/
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     7054 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/AnalyzeData.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    11612 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/BiosensAnalysis.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      312 2022-05-17 17:34:24.000000 PyGFETdb-0.4.3/PyGFETdb/Connection.bin
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)      306 2022-02-18 13:00:16.000000 PyGFETdb-0.4.3/PyGFETdb/DB.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    18058 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/DBAnalyze.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    21757 2022-05-26 22:10:22.000000 PyGFETdb-0.4.3/PyGFETdb/DBCore.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    24169 2022-06-01 09:46:28.000000 PyGFETdb-0.4.3/PyGFETdb/DBCore2.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    10422 2022-05-30 22:33:17.000000 PyGFETdb-0.4.3/PyGFETdb/DBInterface.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    10572 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/DBSearch.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    62531 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/DBXlsReport.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    36817 2022-06-01 09:09:06.000000 PyGFETdb-0.4.3/PyGFETdb/DataClass.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     7091 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/DataStructures.py
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2022-06-01 09:56:13.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    29113 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    34902 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView.ui
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    26147 2022-06-01 07:49:58.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView_v2.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    22290 2022-05-26 18:28:55.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView_v2.ui
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    26961 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDataExplorer.ui
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     8938 2022-06-01 07:49:58.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDataExplorer_v2.ui
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    13544 2022-05-26 18:28:55.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/UpdateDialogs.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)       88 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/GuiDBView/__init__.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     2457 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/NoiseModel.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    25350 2022-02-18 13:00:16.000000 PyGFETdb-0.4.3/PyGFETdb/PlotDataClass.py
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)       88 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/PyGFETdb/__init__.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     5773 2022-05-17 17:34:24.000000 PyGFETdb-0.4.3/PyGFETdb/ws_json_class.py
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2022-06-01 09:56:13.000000 PyGFETdb-0.4.3/PyGFETdb.egg-info/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1140 2022-06-01 09:56:12.000000 PyGFETdb-0.4.3/PyGFETdb.egg-info/PKG-INFO
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      839 2022-06-01 09:56:12.000000 PyGFETdb-0.4.3/PyGFETdb.egg-info/SOURCES.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        1 2022-06-01 09:56:12.000000 PyGFETdb-0.4.3/PyGFETdb.egg-info/dependency_links.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       71 2022-06-01 09:56:12.000000 PyGFETdb-0.4.3/PyGFETdb.egg-info/entry_points.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        9 2022-06-01 09:56:12.000000 PyGFETdb-0.4.3/PyGFETdb.egg-info/top_level.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       18 2022-02-18 12:59:57.000000 PyGFETdb-0.4.3/README.md
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       38 2022-06-01 09:56:13.000000 PyGFETdb-0.4.3/setup.cfg
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     2591 2022-06-01 09:55:34.000000 PyGFETdb-0.4.3/setup.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-09 17:35:40.560397 PyGFETdb-0.5.1/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       56 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/MANIFEST.in
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1121 2023-05-09 17:35:40.556397 PyGFETdb-0.5.1/PKG-INFO
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-09 17:35:40.552397 PyGFETdb-0.5.1/PyGFETdb/
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     7054 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/AnalyzeData.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    11612 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/BiosensAnalysis.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      312 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/Connection.bin
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    18058 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/DBAnalyze.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    24612 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/DBCore2.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    12426 2023-05-09 17:10:52.000000 PyGFETdb-0.5.1/PyGFETdb/DBInterface.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    10572 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/DBSearch.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    62531 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/DBXlsReport.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    38362 2023-05-08 13:20:38.000000 PyGFETdb-0.5.1/PyGFETdb/DataClass.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     7091 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/DataStructures.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-09 17:35:40.556397 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    29113 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    34902 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView.ui
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     7329 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBViewDataExplorer.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    18580 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView_v2.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    22846 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView_v2.ui
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    26961 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDataExplorer.ui
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    14209 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDataExplorer_v2.ui
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    15231 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiHelpers.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     3395 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiNormalization.ui
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     3728 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/NormGui.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    30242 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/UpdateDialogs.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)       88 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/GuiDBView/__init__.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     2457 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/PyGFETdb/NoiseModel.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)    25350 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/PlotDataClass.py
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)      110 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/__init__.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     5773 2023-05-09 16:51:28.000000 PyGFETdb-0.5.1/PyGFETdb/ws_json_class.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-09 17:35:40.552397 PyGFETdb-0.5.1/PyGFETdb.egg-info/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1121 2023-05-09 17:35:40.000000 PyGFETdb-0.5.1/PyGFETdb.egg-info/PKG-INFO
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      951 2023-05-09 17:35:40.000000 PyGFETdb-0.5.1/PyGFETdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        1 2023-05-09 17:35:40.000000 PyGFETdb-0.5.1/PyGFETdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       71 2023-05-09 17:35:40.000000 PyGFETdb-0.5.1/PyGFETdb.egg-info/entry_points.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        9 2023-05-09 17:35:40.000000 PyGFETdb-0.5.1/PyGFETdb.egg-info/top_level.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       18 2023-05-09 16:50:55.000000 PyGFETdb-0.5.1/README.md
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       38 2023-05-09 17:35:40.560397 PyGFETdb-0.5.1/setup.cfg
+-rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     2591 2023-05-09 17:34:02.000000 PyGFETdb-0.5.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyGFETdb-0.4.3/PKG-INFO` & `PyGFETdb-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: PyGFETdb
-Version: 0.4.3
+Version: 0.5.1
 Summary: GFET Analysis tools
 Home-page: https://github.com/aguimera/PyGFETdb
 Download-URL: https://github.com/aguimera/PyGFETdb
 Author: Anton Guimera-Brunet
 Author-email: anton.guimera@csic.es
 Maintainer: Anton Guimera-Brunet
 Maintainer-email: anton.guimera@csic.es
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: Microsoft :: Windows
@@ -25,8 +24,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: User Interfaces
 
 
                    Library for GFET analysis tools
                    
-
```

### Comparing `PyGFETdb-0.4.3/PyGFETdb/AnalyzeData.py` & `PyGFETdb-0.5.1/PyGFETdb/AnalyzeData.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/BiosensAnalysis.py` & `PyGFETdb-0.5.1/PyGFETdb/BiosensAnalysis.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/DBAnalyze.py` & `PyGFETdb-0.5.1/PyGFETdb/DBAnalyze.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/DBCore2.py` & `PyGFETdb-0.5.1/PyGFETdb/DBCore2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,33 +13,36 @@
 import sys
 import pandas as pd
 import numpy as np
 import traceback
 import base64
 from cryptography.fernet import Fernet
 import importlib
+from multiprocessing import Pool
 
 
 def WS_Types(name):
     if name.endswith('id'):
         return 'int'
     elif name == 'Data':
         return 'bin'
     else:
         return 'str'
 
 
 class PyFETdb():
+    Threads = 8
 
-    def __init__(self, connection):
+    def __init__(self, connection, Multiprocess=True):
         f = Fernet(connection)
         # da = f.decrypt(open('./Connection', 'rb').read())
         da = f.decrypt(importlib.resources.read_binary('PyGFETdb', 'Connection.bin'))
         self.connection = pickle.loads(da)
         self._DEBUG = False
+        self.Multiprocess = Multiprocess
 
     def CreateQueryConditions(self, Conditions):
         Cond = []
         values = []
         for c in Conditions:
             cc = " %s OR ".join([c] * len(Conditions[c]))
             Cond.append("({} %s)".format(cc))
@@ -260,44 +263,44 @@
             fp = f.split('_')
             if fp[0] == Table:
                 fn = Dat.get('Info', {})
                 fn[fp[1]] = Res[f]
                 Dat['Info'] = fn
             elif fp[0] == 'Users':
                 fn = Dat.get('Info', {})
-                fn['User'+fp[1]] = Res[f]
+                fn['User' + fp[1]] = Res[f]
                 Dat['Info'] = fn
             else:
                 fn = Dat.get(fp[0], {})
                 fn[fp[1]] = Res[f]
                 Dat[fp[0]] = fn
 
         Dat['Name'] = Res['Trts_Name']
 
         if GetGate:
-            if Table == 'DCcharacts':                
+            if Table == 'DCcharacts':
                 Dat['Gate'] = self.GetGateFromId(Res['DCcharacts_Gate_id'])
             elif Table == 'ACcharacts':
-                cond = {'idDCcharacts = ': (Res['ACcharacts_DC_id'], )}
+                cond = {'idDCcharacts = ': (Res['ACcharacts_DC_id'],)}
                 Res = self.MultiSelect(Table='DCcharacts',
-                                        Conditions=cond,
-                                        Output=('Gate_id', ))
+                                       Conditions=cond,
+                                       Output=('Gate_id',))
 
-                Dat['Gate'] = self.GetGateFromId(Res[0]['Gate_id'])             
+                Dat['Gate'] = self.GetGateFromId(Res[0]['Gate_id'])
 
         return Dat
 
     def GetGateFromId(self, idg):
         Rows = self.MultiSelect(Table='Gcharacts',
-                                Conditions={'idGcharacts=': (idg, )},
-                                Output=('Data', ))
+                                Conditions={'idGcharacts=': (idg,)},
+                                Output=('Data',))
         if len(Rows):
             GateData = pickle.loads(Rows[0]['Data'], encoding='latin')
             Res = self.GetCharactInfo(Table='DCcharacts',
-                                      Conditions={'DCcharacts.Gate_id = ': (idg, )},
+                                      Conditions={'DCcharacts.Gate_id = ': (idg,)},
                                       Output=('Trts.Name',))
             Trts = []
             for re in Res:
                 Trts.append(re['Trts_Name'])
 
             GateData['GateTrts'] = Trts
             return GateData
@@ -330,20 +333,28 @@
             ids = []
             for TrtName, dt in gn:
                 dt.sort_values(by='MeasDate', ascending=False, inplace=True)
                 ids.append(dt.iloc[0]['id{}'.format(Table)])
         else:
             ids = list(dfr['id{}'.format(Table)])
 
-        Data = []
-        for ic, Id in enumerate(ids):
-            print("Downloading {} of {}".format(ic, len(ids)))
-            Data.append(self.GetCharactFromId(Table=Table,
-                                              Id=Id,
-                                              GetGate=GetGate))
+        if self.Multiprocess:
+            Args = []
+            for Id in ids:
+                Args.append((Table, Id, GetGate))
+            print("Downloading {} Records".format(len(ids)))
+            with Pool(self.Threads) as p:
+                Data = p.starmap(self.GetCharactFromId, Args)
+        else:
+            Data = []
+            for ic, Id in enumerate(ids):
+                print("Downloading {} of {}".format(ic, len(ids)))
+                Data.append(self.GetCharactFromId(Table=Table,
+                                                  Id=Id,
+                                                  GetGate=GetGate))
 
         return Data
 
     def InsertCharact(self, DCVals, Fields, ACVals=None, OptFields=None,
                       TrtTypeFields=None, OverWrite=True):
 
         Author = Fields['User']
@@ -418,16 +429,16 @@
             NewData['IsOK'] = DCVals['IsOK']
         if OptFields:
             NewData.update(OptFields)
 
         # Check if exists
         sMeasDate = DCVals['DateTime'].strftime("%Y-%m-%d %H:%M:%S")
         Rows = self.MultiSelect(Table='DCcharacts',
-                                Conditions={'Trt_id=': (Trt_id, ),
-                                            'MeasDate=': (sMeasDate, )},
+                                Conditions={'Trt_id=': (Trt_id,),
+                                            'MeasDate=': (sMeasDate,)},
                                 Output=('Trt_id', 'idDCcharacts'))
 
         if len(Rows) == 0:  # New Record
             DCchatact_id = self.NewRow(Table='DCcharacts', Fields=NewData)
         else:
             print('WARNING EXISTS', Rows)
             if OverWrite:  # OverWrite
@@ -467,115 +478,123 @@
                 print('WARNING EXISTS', Rows)
                 if OverWrite:  # OverWrite
                     ACchatact_id = Rows[0]['idACcharacts']
                     print('Overwrite Record id ', ACchatact_id)
                     scond = 'idACcharacts = {}'.format(ACchatact_id)
                     self.UpdateRow(Table='ACcharacts',
                                    Fields=NewData,
-                                   Condition= scond)
-                    
+                                   Condition=scond)
 
     def InsertGateCharact(self, GateData, Fields, OverWrite=True):
         # Set Get information in other tables
         Author = Fields['User']
         Author_id = self.GetId(Table='Users',
                                Value=Author,
                                NewVals={'Name': Author})
         Fields.pop('User')
 
         # Check if exists
         sMeasDate = GateData['DateTime'].strftime("%Y-%m-%d %H:%M:%S")
         Rows = self.MultiSelect(Table='Gcharacts',
                                 Conditions={'Name=': (Fields['Name'],),
-                                            'MeasDate=': (sMeasDate, )},
-                                Output=('idGcharacts', ))
+                                            'MeasDate=': (sMeasDate,)},
+                                Output=('idGcharacts',))
 
         NewData = {'Data': pickle.dumps(GateData),
                    'User_id': Author_id,
                    'MeasDate': str(GateData['DateTime']),
                    'UpdateDate': str(datetime.datetime.now())}
         NewData.update(Fields)
 
         if len(Rows) == 0:  # New Record
             Gate_id = self.NewRow(Table='Gcharacts', Fields=NewData)
-        else:                        
+        else:
             Gate_id = Rows[0]['idGcharacts']
-            print ('Gate id foung {}'. format(Gate_id))
+            print('Gate id foung {}, Overwriting'.format(Gate_id))
             if OverWrite:  # OverWrite                
-                print ('WARNING EXISTS', Rows)
-                print ('Overwrite Record id ', Gate_id)
+                # print ('WARNING EXISTS', Rows)
+                # print ('Overwrite Record id ', Gate_id)
                 scond = 'idGcharacts = {}'.format(Gate_id)
                 self.UpdateRow(Table='Gcharacts',
                                Fields=NewData,
                                Condition=scond)
         return Gate_id
-    
-    def InsertDataFrame(self, dfUpload):        
+
+    def InsertDataFrame(self, dfUpload):
         FieldsCols = ('User',
                       'Wafer',
                       'Device',
                       'TrtType',
                       'Trt')
 
         DataFields = ('DCVals', 'ACVals', 'GateData', 'TrtTypeFields')
         NonOptFields = list(FieldsCols) + list(DataFields)
 
         for ir, r in dfUpload.iterrows():
             print("Upload {} of {}  {}".format(ir, dfUpload.shape[0], r.Trt))
-            
+
             GateId = None
             if r.GateData is not None:
-                GateFields= {'User': r.User,
-                             'Name': '{}-Gate'.format(r.Device),
-                             'FileName': r.FileName}
+                GateFields = {'User': r.User,
+                              'Name': '{}-Gate'.format(r.Device),
+                              'FileName': r.FileName}
                 GateId = self.InsertGateCharact(GateData=r.GateData,
                                                 Fields=GateFields)
-                    
+
             Fields = r[list(FieldsCols)].to_dict()
             Fields['Gate_id'] = GateId
-            
+
             self.InsertCharact(DCVals=r.DCVals,
                                Fields=Fields,
                                ACVals=r.ACVals,
                                OptFields=r.drop(NonOptFields).to_dict(),
                                TrtTypeFields=r.TrtTypeFields)
-        
 
 
-def Data2Pandas(Data):
-    pdSeries = []
-    for ic, dd in enumerate(Data):
-        print("Converting {} of {}".format(ic, len(Data)))
-        pdser = {}
-        d = DataCharAC(dd)
-        pdser['Name'] = d.Name
-        pdser['CharCl'] = d
-        pdser['IsOk'] = d.IsOK
-        pdser['ChName'] = d.ChName
-        pdser['Date'] = d.GetDateTime()
-        for k, v in d['Wafers'].items():
-            if k == 'Name':
-                pdser['Wafer'] = v
-            else:
-                pdser['Waf' + k] = v
-        for k, v in d['Devices'].items():
-            if k == 'Name':
-                pdser['Device'] = v
-            else:
-                pdser['Dev' + k] = v
-        for k, v in d['TrtTypes'].items():
-            if k == 'Name':
-                pdser['TrtType'] = v
-            else:
-                pdser[k] = v
-        for k, v in d['Info'].items():
-            if k == 'Gate_id':
-                continue
+def GetSerie(Data):
+    pdser = {}
+    d = DataCharAC(Data)
+    pdser['Name'] = d.Name
+    pdser['CharCl'] = d
+    pdser['IsOk'] = d.IsOK
+    pdser['ChName'] = d.ChName
+    pdser['Date'] = d.GetDateTime()
+    for k, v in d['Wafers'].items():
+        if k == 'Name':
+            pdser['Wafer'] = v
+        else:
+            pdser['Waf' + k] = v
+    for k, v in d['Devices'].items():
+        if k == 'Name':
+            pdser['Device'] = v
+        else:
+            pdser['Dev' + k] = v
+    for k, v in d['TrtTypes'].items():
+        if k == 'Name':
+            pdser['TrtType'] = v
+        else:
             pdser[k] = v
-        pdSeries.append(pd.Series(pdser))
+    for k, v in d['Info'].items():
+        if k == 'Gate_id':
+            continue
+        pdser[k] = v
+
+    return pd.Series(pdser)
+
+
+def Data2Pandas(Data, Threads=True):
+    if Threads:
+        print("Converting {} Records".format(len(Data)))
+        with Pool() as p:
+            pdSeries = p.map(GetSerie, Data)
+    else:
+        pdSeries = []
+        for ic, dd in enumerate(Data):
+            print("Converting {} of {}".format(ic, len(Data)))
+            pdSeries.append(GetSerie(Data=dd))
 
     dfRaw = pd.concat(pdSeries, axis=1).transpose()
     DataTypes = {}
     for col in dfRaw.keys():
         if col in ('Width', 'Length', 'Pass', 'Area', 'Ph', 'IonStrength', 'AnalyteCon'):
             dfRaw[col] = pd.to_numeric(dfRaw[col], errors='coerce')
             DataTypes[col] = float
@@ -584,15 +603,14 @@
 
     DataTypes['CharCl'] = object
     DataTypes['IsOk'] = bool
     DataTypes['Date'] = 'datetime64[ns]'
 
     return dfRaw.astype(DataTypes, errors='ignore')
 
-
 # if __name__ == '__main__':
 #     # f = Fernet(open('key.key', 'rb').read())
 #     # da = f.decrypt(open('Connection', 'rb').read())
 #     # connection = pickle.loads(da)
 #     MyDb = PyFETdb(open('key.key', 'rb').read())
 
 # %% Test insert bin data
```

### Comparing `PyGFETdb-0.4.3/PyGFETdb/DBInterface.py` & `PyGFETdb-0.5.1/PyGFETdb/DBInterface.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 """
 Created on Fri Jan 12 13:12:37 2018
 
 @author: aguimera
 """
 
 from PyGFETdb.DataClass import DataCharAC, DataCharDC
-import PyGFETdb.DBCore as PyFETdb
+import PyGFETdb.DBCore2 as PyFETdb
 import numpy as np
 import pandas as pd
 import quantities as pq
 import pickle
+from multiprocessing import Pool
 
 # Array values on measured Vgs range
 OutUnits = {'Ids': 'uA',
             'GM': 'mS',
             'GMV': 'mS/V',
             'Irms': 'uA',
             'Vrms': 'uV',
@@ -24,164 +25,227 @@
             }
 
 ########################################################################################################################
 ## Define default scalar parameters
 ########################################################################################################################
 ScalarParamsDC = ['Ids', 'GM', 'GMV']
 ScalarParamsAC = ['Irms', 'Vrms', 'NoA', 'NoB', 'NoC']
-VgsScalar = -0.1*pq.V
+VgsScalar = -0.1 * pq.V
 ScalarQueriesDC = {'CNP': {'Param': 'Ud0',
-                            'Units': 'mV'},
+                           'Units': 'mV'},
                    'IgMax': {'Param': 'IgMax',
-                              'Units': 'nA'
-                              },
+                             'Units': 'nA'
+                             },
                    'IdsV01': {'Param': 'Ids',
-                              'Vgs': 0.1*pq.V,
+                              'Vgs': 0.1 * pq.V,
                               'Ud0Norm': False,
                               'Units': 'uA'
                               },
                    'RdsCNP': {'Param': 'Rds',
-                              'Vgs': 0*pq.V,
+                              'Vgs': 0 * pq.V,
                               'Ud0Norm': True,
                               'Units': 'kOhm'
                               },
                    'IdsCNP': {'Param': 'Ids',
-                              'Vgs': 0*pq.V,
+                              'Vgs': 0 * pq.V,
                               'Ud0Norm': True,
                               'Units': 'uA'
-                              } ,
+                              },
                    }
 
 for par in ScalarParamsDC:
     d = {'Param': par,
          'Vgs': VgsScalar,
          'Ud0Norm': True}
     if par in OutUnits:
         d['Units'] = OutUnits[par]
-    ScalarQueriesDC[par+'01'] = d
+    ScalarQueriesDC[par + '01'] = d
 
 ScalarQueries = ScalarQueriesDC.copy()
 for par in ScalarParamsAC:
     d = {'Param': par,
          'Vgs': VgsScalar,
          'Ud0Norm': True}
     if par in OutUnits:
         d['Units'] = OutUnits[par]
-    ScalarQueries[par+'01'] = d
+    ScalarQueries[par + '01'] = d
 
 ########################################################################################################################
 ## Define default Array parameters
 ########################################################################################################################
 Vgs = np.linspace(-0.1, 0.6, 100) * pq.V
 VgsNorm = np.linspace(-0.4, 0.4, 100) * pq.V
 ArrayParamsDC = ['Ids', 'GM', 'GMV', 'Ig']
 ArrayParamsAC = ['Irms', 'Vrms', 'NoA', 'NoB', 'NoC']
 ArrayQueriesDC = {}
+ArrayQueriesNormDC = {}
 for par in ArrayParamsDC:
     d = {'Param': par,
          'Vgs': Vgs,
          'Ud0Norm': False}
     if par in OutUnits:
         d['Units'] = OutUnits[par]
     ArrayQueriesDC[par] = d
 
     d = {'Param': par,
          'Vgs': VgsNorm,
          'Ud0Norm': True}
     if par in OutUnits:
         d['Units'] = OutUnits[par]
-    ArrayQueriesDC[par+'Norm']=d
+    ArrayQueriesNormDC[par + 'Norm'] = d
 
 ArrayQueries = ArrayQueriesDC.copy()
+ArrayQueriesNorm = ArrayQueriesNormDC.copy()
 for par in ArrayParamsAC:
     d = {'Param': par,
          'Vgs': Vgs,
          'Ud0Norm': False}
     if par in OutUnits:
         d['Units'] = OutUnits[par]
     ArrayQueries[par] = d
 
     d = {'Param': par,
          'Vgs': VgsNorm,
          'Ud0Norm': True}
     if par in OutUnits:
         d['Units'] = OutUnits[par]
-    ArrayQueries[par+'Norm']=d
+    ArrayQueriesNorm[par + 'Norm'] = d
 
 ########################################################################################################################
 ## Define default Array parameters
 ########################################################################################################################
 
 ClassQueries = ScalarQueries.copy()
 ClassQueries.update(ArrayQueries)
+ClassQueries.update(ArrayQueriesNorm)
 pdAttr = {'Vgs': Vgs,
           'VgsNorm': VgsNorm,
           'ScalarCols': list(ScalarQueries.keys()),
-          'ArrayCols': list(ArrayQueries.keys()),
+          'ArrayCols': list(ArrayQueries.keys()) + list(ArrayQueriesNorm.keys()),
+          'ArrayColsNorm': list(ArrayQueriesNorm.keys())
           }
 
 ClassQueriesDC = ScalarQueriesDC.copy()
 ClassQueriesDC.update(ArrayQueriesDC)
+ClassQueriesDC.update(ArrayQueriesNormDC)
 pdAttrDC = {'Vgs': Vgs,
             'VgsNorm': VgsNorm,
             'ScalarCols': list(ScalarQueriesDC.keys()),
-            'ArrayCols': list(ArrayQueriesDC.keys()),
+            'ArrayCols': list(ArrayQueriesDC.keys()) + list(ArrayQueriesNormDC.keys()),
+            'ArrayColsNorm': list(ArrayQueriesNormDC.keys())
             }
 
 
-def CalcElectricalParams(dbRaw, ClsQueries, dfAttr, pErrors=False):
-    PdSeries = []
+def CalcElect(ClsQueries, char, vds, row, pErrors):
+    vals = {'Vds': vds.flatten()}
+    for parn, park in ClsQueries.items():
+        park['Vds'] = vds
+        try:
+            val = char.Get(**park)
+        except:
+            if pErrors:
+                print('Error', parn, char.Name)
+            continue
+        if val is None:
+            continue
+        if val.size > 1:
+            vals[parn] = val
+        else:
+            vals[parn] = val.flatten()
+    return pd.concat((row, pd.Series(vals)))
+
+
+def CalcElectricalParams(dbRaw, ClsQueries, dfAttr, pErrors=False, Threads=True):
+    Args = []
     for index, row in dbRaw.iterrows():
-        print("Calculating {} of {}".format(index, dbRaw.shape[0]))
         char = row['CharCl']
         Vds = char.GetVds()
         for vds in Vds:
-            vals = {}
-            vals['Vds'] = vds.flatten()
-            for parn, park in ClsQueries.items():
-                park['Vds'] = vds
-                try:
-                    val = char.Get(**park)
-                except:
-                    if pErrors:
-                        print('Error', parn, char.Name)
-                    continue
-                if val is None:
-                    continue
-                if val.size > 1:
-                    vals[parn] = val
-                else:
-                    vals[parn] = val.flatten()
-            PdSeries.append(pd.concat((row, pd.Series(vals))))
-    
-    dfDat = pd.concat(PdSeries, axis=1).transpose()       
-    
+            Args.append((ClsQueries, char, vds, row, pErrors))
+
+    if Threads:
+        print("Calculating {} rows ".format(len(Args)))
+        with Pool() as p:
+            PdSeries = p.starmap(CalcElect, Args)
+    else:
+        PdSeries = []
+        for ia, a in enumerate(Args):
+            print("Calculating {} of {}".format(ia, len(Args)))
+            PdSeries.append(CalcElect(*a))
+
+    dfDat = pd.concat(PdSeries, axis=1).transpose()
+
     DataTypes = dbRaw.dtypes
-    DataTypes['Vds'] = np.float
+    DataTypes['Vds'] = float
+    sCols = []
     for col in dfAttr['ScalarCols']:
         if col in dfDat.columns:
-            DataTypes[col] = np.float
+            DataTypes[col] = float
+            sCols.append(col)
+    aCols = []
     for col in dfAttr['ArrayCols']:
         if col in dfDat.columns:
             DataTypes[col] = object
+            aCols.append(col)
     dfDat = dfDat.astype(DataTypes)
-    
+
+    dfAttr['ArrayCols'] = aCols
+    dfAttr['ScalarCols'] = sCols
+
     ColUnits = {}
     for col, p in ClsQueries.items():
         if 'Units' in p:
             ColUnits[col] = p['Units']
         else:
             ColUnits[col] = ''
-    
+
     dfAttr['ColUnits'] = ColUnits
-    
+
     dfDat.attrs.update(dfAttr)
 
     return dfDat
 
+FilePaser = {'FS': {'Field': 'FuncStep',
+                    'Type': str,
+                    'Fconvert': str, },
+             'CO': {'Field': 'Comments',
+                    'Type': str,
+                    'Fconvert': str, },
+             'SO': {'Field': 'Solution',
+                    'Type': str,
+                    'Fconvert': str, },
+             'PH': {'Field': 'Ph',
+                    'Type': float,
+                    'Fconvert': float, },
+             'IS': {'Field': 'IonStrength',
+                    'Type': float,
+                    'Fconvert': float, },
+             'IC': {'Field': 'IsCmp',
+                    'Type': int,
+                    'Fconvert': int, },
+             'AN': {'Field': 'AnalyteCon',
+                    'Type': float,
+                    'Fconvert': float, },
+             }
+
+def FileParser(FileName, Fields):
+    fName = FileName.replace('\\', '/').split('/')[-1]
+    fNameP = fName.split('--')
+    
+    Fields['Wafer'] = fNameP[0]
+    Fields['Device'] = '{}-{}'.format(Fields['Wafer'], fNameP[1])
+    Fields['FileName'] = fName
+    
+    for f in fNameP[2:]:
+        ff = f.split('_')
+        ffi = ff[0].upper()
+        if ffi in FilePaser:
+            Fields[FilePaser[ffi]['Field']] = FilePaser[ffi]['Fconvert'](ff[1].replace('p','.'))
+
+
 def LoadPickleData(FileIn):
     DataIn = pickle.load(open(FileIn, 'rb'), encoding='latin')
     DevDCVals = DataIn['DevDC']
     DevACVals = DataIn['DevAC']
 
     DictClDC = {}
     if DevACVals is not None:
@@ -202,24 +266,24 @@
 
         acDat = DCclass.__dict__.copy()
         acDat.update(DevACVals[chn])
         acDat.pop('Ids')
         acDat['Vgs'] = acDat.pop('VgsAC')
         acDat['Vds'] = acDat.pop('VdsAC')
         DictClAC[chn] = DataCharAC(acDat)
-    
+
     return DictClDC, DictClAC, GateDict
 
 
 def CheckConditionsCharTable(Conditions, Table):
     for k in list(Conditions.keys()):
         if k.startswith('CharTable'):
             nk = k.replace('CharTable', Table)
             Conditions.update({nk: Conditions[k]})
-            del(Conditions[k])
+            del (Conditions[k])
     return Conditions
 
 
 def GetFromDB(Conditions, Table='ACcharacts', Last=True, GetGate=True):
     """
     Get data from data base
 
@@ -264,30 +328,30 @@
     MyDb = PyFETdb.PyFETdb()
 
     DataD, Trts = MyDb.GetData2(Conditions=Conditions,
                                 Table=Table,
                                 Last=Last,
                                 GetGate=GetGate)
 
-    del(MyDb)
+    del (MyDb)
     Trts = list(Trts)
 
     Data = {}
     for Trtn, Cys in DataD.items():
         Chars = []
         for Cyn, Dat in sorted(Cys.items()):
             try:
                 Char = DataCharAC(Dat)
                 Chars.append(Char)
             except:
                 print('Failed loading', Trtn)
                 print(Dat)
         Data[Trtn] = Chars
 
-    print ('Trts Found ->', len(Trts))
+    print('Trts Found ->', len(Trts))
     return Data, Trts
 
 
 def Data2Pandas(DictData):
     pdSeries = []
     for tn, dats in DictData.items():
         for dd in dats:
@@ -313,23 +377,21 @@
                 else:
                     pdser[k] = v
             for k, v in dd['Info'].items():
                 if k == 'Gate_id':
                     continue
                 pdser[k] = v
             pdSeries.append(pd.Series(pdser))
-        
+
     dfRaw = pd.concat(pdSeries, axis=1).transpose()
     DataTypes = {}
-    for col in dfRaw.keys():    
+    for col in dfRaw.keys():
         if col in ('Width', 'Length', 'Pass', 'Area', 'Ph', 'IonStrength', 'AnalyteCon'):
             DataTypes[col] = np.float
         else:
             DataTypes[col] = 'category'
-    
+
     DataTypes['CharCl'] = object
     DataTypes['IsOk'] = bool
     DataTypes['Date'] = 'datetime64[ns]'
-    
-    return dfRaw.astype(DataTypes)
-
 
+    return dfRaw.astype(DataTypes)
```

### Comparing `PyGFETdb-0.4.3/PyGFETdb/DBSearch.py` & `PyGFETdb-0.5.1/PyGFETdb/DBSearch.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/DBXlsReport.py` & `PyGFETdb-0.5.1/PyGFETdb/DBXlsReport.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/DataClass.py` & `PyGFETdb-0.5.1/PyGFETdb/DataClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,30 @@
 import copy
 
 from PyGFETdb import PlotDataClass
 import sys
 
 DebugPrint = True
 
+ParametersList = ['GM',
+                  'GMV',
+                  'Ig',
+                  'Ids',
+                  'Irms',
+                  'Vrms',
+                  'Rds',
+                  'NoA',
+                  'NoB',
+                  'NoC',
+                  'FEMmu',
+                  'FEMn',
+                  'FEMmuGm',
+                  'Ud0',
+                  'IgMax'
+                  ]
 
 class DataCharDC(object):
     """
     Class to manage the DC characteristics of GFET characteristics.
 
     """
 
@@ -73,23 +89,36 @@
     def _CalcIsOK(self, RdsRange=(400, 10e3)):
         Rds = self.GetRds()
         if np.any([Rds < RdsRange[0], Rds > RdsRange[1]]):
             self.IsOK = False
         else:
             self.IsOK = True
 
+    def __CheckData(self, Data):
+        if 'Ids' in Data:
+            nanidsInds = np.where(np.isnan(Data['Ids']))[0]
+            if len(nanidsInds):
+                print('Detected NaN values', Data['Vgs'][nanidsInds])
+                Data['Ids'] = np.delete(Data['Ids'], nanidsInds, axis=0)
+                Data['Vgs'] = np.delete(Data['Vgs'], nanidsInds)
+                Data['Slope'] = np.delete(Data['Slope'], nanidsInds, axis=0)
+            
+        return Data
+
     def __init__(self, Data):
         """
         Create a class to manage the GFET characteristics.
 
         Parameters
         ----------
         Data: Dictionary from DB
 
         """
+        
+        Data = self.__CheckData(Data)
 
         for k, v in Data.items():
             if k == 'Gate':
                 if v is None:
                     if DebugPrint:
                         print('No gate values')
                 elif np.isnan(v['Ig']).any():
@@ -899,37 +928,54 @@
     def GetFitPSD(self, Vgs=None, Vds=None, Ud0Norm=False, **kwargs):
         SiVds, VgsInd = self._GetFreqVgsInd(Vgs, Vds, Ud0Norm)
         if VgsInd is None:
             return None
         return self.FitPSD[SiVds[0]][VgsInd, :].transpose()
 
     def GetPSD(self, Vgs=None, Vds=None, Ud0Norm=False, **kwargs):
+        if 'PSD' not in self.__dict__:
+            print('PSD is not a valid parameter ', self.Name)
+            return None
         SiVds, VgsInd = self._GetFreqVgsInd(Vgs, Vds, Ud0Norm)
         if VgsInd is None:
             return None
         return self.PSD[SiVds[0]][VgsInd, :].transpose()
 
     def GetGmMag(self, Vgs=None, Vds=None, Ud0Norm=False, **kwargs):
+        if 'gm' not in self.__dict__:
+            print('gm is not a valid parameter ', self.Name)
+            return None
+
         SiVds, VgsInd = self._GetFreqVgsInd(Vgs, Vds, Ud0Norm)
         if VgsInd is None:
             return None
 
         return np.abs(self.gm[SiVds[0]][VgsInd, :].transpose())
 
     def GetGmPh(self, Vgs=None, Vds=None, Ud0Norm=False, **kwargs):
+        if 'gm' not in self.__dict__:
+            print('gm is not a valid parameter ', self.Name)
+            return None
+
         SiVds, VgsInd = self._GetFreqVgsInd(Vgs, Vds, Ud0Norm)
         if VgsInd is None:
             return None
 
         return np.angle(self.gm[SiVds[0]][VgsInd, :].transpose(), deg=True)
 
     def GetFpsd(self, **kwargs):
+        if 'Fpsd' not in self.__dict__:
+            print('Fpsd is not a valid parameter ', self.Name)
+            return None
         return self.Fpsd
 
     def GetFgm(self, **kwargs):
+        if 'Fgm' not in self.__dict__:
+            print('Fgm is not a valid parameter ', self.Name)
+            return None
         return self.Fgm
 
     def _CheckRMS(self, NFmin, NFmax):
         if NFmin is not None or NFmax is not None:
             if self.NFmin != NFmin or self.NFmax != NFmax:
                 # print ('Calc IRMS')
                 self.NFmin = NFmin
```

### Comparing `PyGFETdb-0.4.3/PyGFETdb/DataStructures.py` & `PyGFETdb-0.5.1/PyGFETdb/DataStructures.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView.py` & `PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView.ui` & `PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView.ui`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView_v2.ui` & `PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView_v2.ui`

 * *Files 1% similar despite different names*

#### Comparing `PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDBView_v2.ui` & `PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDBView_v2.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>PyFETdbViewer</class>
   <widget class="QMainWindow" name="PyFETdbViewer">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>994</width>
-        <height>728</height>
+        <width>1055</width>
+        <height>784</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>MainWindow</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QVBoxLayout" name="verticalLayout_5">
@@ -427,205 +427,220 @@
                     </widget>
                   </widget>
                 </item>
               </layout>
             </widget>
             <widget class="QTabWidget" name="tabWidget">
               <property name="currentIndex">
-                <number>1</number>
+                <number>0</number>
               </property>
-              <widget class="QWidget" name="DC">
+              <widget class="QWidget" name="AC">
                 <attribute name="title">
-                  <string>DC Data</string>
+                  <string>AC Data</string>
                 </attribute>
-                <layout class="QGridLayout" name="gridLayout_4">
+                <layout class="QGridLayout" name="gridLayout_5">
                   <item row="0" column="0">
-                    <widget class="QFrame" name="frame_6">
+                    <widget class="QFrame" name="frame_7">
                       <property name="frameShape">
                         <enum>QFrame::StyledPanel</enum>
                       </property>
                       <property name="frameShadow">
                         <enum>QFrame::Raised</enum>
                       </property>
-                      <layout class="QGridLayout" name="gridLayout_3">
-                        <item row="0" column="1">
-                          <widget class="QPushButton" name="ButDeleteDC">
-                            <property name="minimumSize">
+                      <layout class="QGridLayout" name="gridLayout_2">
+                        <item row="0" column="6">
+                          <widget class="QPushButton" name="ButViewAC">
+                            <property name="maximumSize">
                               <size>
                                 <width>50</width>
-                                <height>0</height>
+                                <height>16777215</height>
                               </size>
                             </property>
                             <property name="text">
-                              <string>Delete</string>
-                            </property>
-                          </widget>
-                        </item>
-                        <item row="1" column="0" colspan="5">
-                          <widget class="QTableView" name="TblDC">
-                            <property name="font">
-                              <font>
-                                <pointsize>6</pointsize>
-                              </font>
-                            </property>
-                            <property name="sortingEnabled">
-                              <bool>true</bool>
+                              <string>View</string>
                             </property>
                           </widget>
                         </item>
-                        <item row="0" column="3">
-                          <spacer name="horizontalSpacer_2">
+                        <item row="0" column="4">
+                          <spacer name="horizontalSpacer">
                             <property name="orientation">
                               <enum>Qt::Horizontal</enum>
                             </property>
                             <property name="sizeHint" stdset="0">
                               <size>
-                                <width>16</width>
+                                <width>28</width>
                                 <height>20</height>
                               </size>
                             </property>
                           </spacer>
                         </item>
-                        <item row="0" column="4">
-                          <widget class="QPushButton" name="ButViewDC">
-                            <property name="sizePolicy">
-                              <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
-                                <horstretch>0</horstretch>
-                                <verstretch>0</verstretch>
-                              </sizepolicy>
-                            </property>
+                        <item row="0" column="1">
+                          <widget class="QPushButton" name="ButDeleteAC">
                             <property name="minimumSize">
                               <size>
-                                <width>25</width>
+                                <width>50</width>
                                 <height>0</height>
                               </size>
                             </property>
                             <property name="maximumSize">
                               <size>
-                                <width>16777215</width>
+                                <width>0</width>
                                 <height>16777215</height>
                               </size>
                             </property>
                             <property name="text">
-                              <string>View</string>
+                              <string>Delete</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item row="1" column="0" colspan="8">
+                          <widget class="QTableView" name="TblAC">
+                            <property name="font">
+                              <font>
+                                <pointsize>6</pointsize>
+                              </font>
+                            </property>
+                            <property name="sortingEnabled">
+                              <bool>true</bool>
                             </property>
                           </widget>
                         </item>
                         <item row="0" column="2">
-                          <widget class="QPushButton" name="ButEditDC">
+                          <widget class="QPushButton" name="ButEditAC">
                             <property name="text">
                               <string>Edit</string>
                             </property>
                           </widget>
                         </item>
+                        <item row="0" column="3">
+                          <widget class="QPushButton" name="ButEditElecParsAC">
+                            <property name="text">
+                              <string>Edit Calcs</string>
+                            </property>
+                          </widget>
+                        </item>
                       </layout>
-                      <zorder>TblDC</zorder>
-                      <zorder>ButViewDC</zorder>
-                      <zorder>horizontalSpacer_2</zorder>
-                      <zorder>ButDeleteDC</zorder>
-                      <zorder>ButEditDC</zorder>
                     </widget>
                   </item>
                 </layout>
               </widget>
-              <widget class="QWidget" name="AC">
+              <widget class="QWidget" name="DC">
                 <attribute name="title">
-                  <string>AC Data</string>
+                  <string>DC Data</string>
                 </attribute>
-                <layout class="QGridLayout" name="gridLayout_5">
+                <layout class="QGridLayout" name="gridLayout_4">
                   <item row="0" column="0">
-                    <widget class="QFrame" name="frame_7">
+                    <widget class="QFrame" name="frame_6">
                       <property name="frameShape">
                         <enum>QFrame::StyledPanel</enum>
                       </property>
                       <property name="frameShadow">
                         <enum>QFrame::Raised</enum>
                       </property>
-                      <layout class="QGridLayout" name="gridLayout_2">
+                      <layout class="QGridLayout" name="gridLayout_3">
+                        <item row="0" column="4">
+                          <spacer name="horizontalSpacer_2">
+                            <property name="orientation">
+                              <enum>Qt::Horizontal</enum>
+                            </property>
+                            <property name="sizeHint" stdset="0">
+                              <size>
+                                <width>16</width>
+                                <height>20</height>
+                              </size>
+                            </property>
+                          </spacer>
+                        </item>
                         <item row="0" column="1">
-                          <widget class="QPushButton" name="ButDeleteAC">
+                          <widget class="QPushButton" name="ButDeleteDC">
                             <property name="minimumSize">
                               <size>
                                 <width>50</width>
                                 <height>0</height>
                               </size>
                             </property>
+                            <property name="text">
+                              <string>Delete</string>
+                            </property>
+                          </widget>
+                        </item>
+                        <item row="0" column="5">
+                          <widget class="QPushButton" name="ButViewDC">
+                            <property name="sizePolicy">
+                              <sizepolicy hsizetype="Minimum" vsizetype="Fixed">
+                                <horstretch>0</horstretch>
+                                <verstretch>0</verstretch>
+                              </sizepolicy>
+                            </property>
+                            <property name="minimumSize">
+                              <size>
+                                <width>25</width>
+                                <height>0</height>
+                              </size>
+                            </property>
                             <property name="maximumSize">
                               <size>
-                                <width>0</width>
+                                <width>16777215</width>
                                 <height>16777215</height>
                               </size>
                             </property>
                             <property name="text">
-                              <string>Delete</string>
+                              <string>View</string>
                             </property>
                           </widget>
                         </item>
-                        <item row="1" column="0" colspan="7">
-                          <widget class="QTableView" name="TblAC">
+                        <item row="1" column="0" colspan="6">
+                          <widget class="QTableView" name="TblDC">
                             <property name="font">
                               <font>
                                 <pointsize>6</pointsize>
                               </font>
                             </property>
                             <property name="sortingEnabled">
                               <bool>true</bool>
                             </property>
                           </widget>
                         </item>
-                        <item row="0" column="3">
-                          <spacer name="horizontalSpacer">
-                            <property name="orientation">
-                              <enum>Qt::Horizontal</enum>
-                            </property>
-                            <property name="sizeHint" stdset="0">
-                              <size>
-                                <width>28</width>
-                                <height>20</height>
-                              </size>
-                            </property>
-                          </spacer>
-                        </item>
-                        <item row="0" column="5">
-                          <widget class="QPushButton" name="ButViewAC">
-                            <property name="maximumSize">
-                              <size>
-                                <width>50</width>
-                                <height>16777215</height>
-                              </size>
-                            </property>
+                        <item row="0" column="2">
+                          <widget class="QPushButton" name="ButEditDC">
                             <property name="text">
-                              <string>View</string>
+                              <string>Edit</string>
                             </property>
                           </widget>
                         </item>
-                        <item row="0" column="2">
-                          <widget class="QPushButton" name="ButEditAC">
+                        <item row="0" column="3">
+                          <widget class="QPushButton" name="ButEditElecParsDC">
                             <property name="text">
-                              <string>Edit</string>
+                              <string>Edit Calcs</string>
                             </property>
                           </widget>
                         </item>
                       </layout>
+                      <zorder>TblDC</zorder>
+                      <zorder>ButViewDC</zorder>
+                      <zorder>horizontalSpacer_2</zorder>
+                      <zorder>ButDeleteDC</zorder>
+                      <zorder>ButEditDC</zorder>
+                      <zorder>ButEditElecParsDC</zorder>
                     </widget>
                   </item>
                 </layout>
               </widget>
             </widget>
           </widget>
         </item>
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
-          <width>994</width>
-          <height>19</height>
+          <width>1055</width>
+          <height>22</height>
         </rect>
       </property>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
   </widget>
   <resources/>
   <connections/>
```

### Comparing `PyGFETdb-0.4.3/PyGFETdb/GuiDBView/GuiDataExplorer.ui` & `PyGFETdb-0.5.1/PyGFETdb/GuiDBView/GuiDataExplorer.ui`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/NoiseModel.py` & `PyGFETdb-0.5.1/PyGFETdb/NoiseModel.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/PlotDataClass.py` & `PyGFETdb-0.5.1/PyGFETdb/PlotDataClass.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb/ws_json_class.py` & `PyGFETdb-0.5.1/PyGFETdb/ws_json_class.py`

 * *Files identical despite different names*

### Comparing `PyGFETdb-0.4.3/PyGFETdb.egg-info/PKG-INFO` & `PyGFETdb-0.5.1/PyGFETdb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: PyGFETdb
-Version: 0.4.3
+Version: 0.5.1
 Summary: GFET Analysis tools
 Home-page: https://github.com/aguimera/PyGFETdb
 Download-URL: https://github.com/aguimera/PyGFETdb
 Author: Anton Guimera-Brunet
 Author-email: anton.guimera@csic.es
 Maintainer: Anton Guimera-Brunet
 Maintainer-email: anton.guimera@csic.es
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: Microsoft :: Windows
@@ -25,8 +24,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: User Interfaces
 
 
                    Library for GFET analysis tools
                    
-
```

### Comparing `PyGFETdb-0.4.3/PyGFETdb.egg-info/SOURCES.txt` & `PyGFETdb-0.5.1/PyGFETdb.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 MANIFEST.in
 README.md
 setup.py
 PyGFETdb/AnalyzeData.py
 PyGFETdb/BiosensAnalysis.py
 PyGFETdb/Connection.bin
-PyGFETdb/DB.py
 PyGFETdb/DBAnalyze.py
-PyGFETdb/DBCore.py
 PyGFETdb/DBCore2.py
 PyGFETdb/DBInterface.py
 PyGFETdb/DBSearch.py
 PyGFETdb/DBXlsReport.py
 PyGFETdb/DataClass.py
 PyGFETdb/DataStructures.py
 PyGFETdb/NoiseModel.py
@@ -20,13 +18,17 @@
 PyGFETdb.egg-info/PKG-INFO
 PyGFETdb.egg-info/SOURCES.txt
 PyGFETdb.egg-info/dependency_links.txt
 PyGFETdb.egg-info/entry_points.txt
 PyGFETdb.egg-info/top_level.txt
 PyGFETdb/GuiDBView/GuiDBView.py
 PyGFETdb/GuiDBView/GuiDBView.ui
+PyGFETdb/GuiDBView/GuiDBViewDataExplorer.py
 PyGFETdb/GuiDBView/GuiDBView_v2.py
 PyGFETdb/GuiDBView/GuiDBView_v2.ui
 PyGFETdb/GuiDBView/GuiDataExplorer.ui
 PyGFETdb/GuiDBView/GuiDataExplorer_v2.ui
+PyGFETdb/GuiDBView/GuiHelpers.py
+PyGFETdb/GuiDBView/GuiNormalization.ui
+PyGFETdb/GuiDBView/NormGui.py
 PyGFETdb/GuiDBView/UpdateDialogs.py
 PyGFETdb/GuiDBView/__init__.py
```

### Comparing `PyGFETdb-0.4.3/setup.py` & `PyGFETdb-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Foobar.  If not, see <http://www.gnu.org/licenses/>.
 
 
 from setuptools import setup, find_packages
 
-_version = '0.4.3'
+_version = '0.5.1'
 
 long_description = """
                    Library for GFET analysis tools
                    """
 
 install_requires = [ ]
```

