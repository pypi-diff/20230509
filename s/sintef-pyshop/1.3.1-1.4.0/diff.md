# Comparing `tmp/sintef-pyshop-1.3.1.tar.gz` & `tmp/sintef-pyshop-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sintef-pyshop-1.3.1.tar", last modified: Wed Nov  2 12:17:45 2022, max compression
+gzip compressed data, was "sintef-pyshop-1.4.0.tar", last modified: Tue May  9 12:54:10 2023, max compression
```

## Comparing `sintef-pyshop-1.3.1.tar` & `sintef-pyshop-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 12:17:45.127521 sintef-pyshop-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5293 2022-11-02 12:17:45.127521 sintef-pyshop-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4239 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 12:17:45.123520 sintef-pyshop-1.3.1/pyshop/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 12:17:45.123520 sintef-pyshop-1.3.1/pyshop/helpers/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/helpers/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     5035 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/helpers/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/helpers/typing_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 12:17:45.123520 sintef-pyshop-1.3.1/pyshop/lp_model/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/lp_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1996 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/lp_model/index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/lp_model/lp_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    10661 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/lp_model/row.py
--rw-r--r--   0 runner    (1001) docker     (121)     9366 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/lp_model/var.py
--rw-r--r--   0 runner    (1001) docker     (121)    12653 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/shop_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 12:17:45.123520 sintef-pyshop-1.3.1/pyshop/shopcore/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/shopcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/shopcore/command_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    24008 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/shopcore/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    13096 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/shopcore/script_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    14831 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/shopcore/shop_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/pyshop/shopcore/shop_rest.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-02 12:17:45.127521 sintef-pyshop-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-11-02 12:17:32.000000 sintef-pyshop-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 12:17:45.127521 sintef-pyshop-1.3.1/sintef_pyshop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5293 2022-11-02 12:17:45.000000 sintef-pyshop-1.3.1/sintef_pyshop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-02 12:17:45.000000 sintef-pyshop-1.3.1/sintef_pyshop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 12:17:45.000000 sintef-pyshop-1.3.1/sintef_pyshop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-11-02 12:17:45.000000 sintef-pyshop-1.3.1/sintef_pyshop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-02 12:17:45.000000 sintef-pyshop-1.3.1/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1078 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4239 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.408684 sintef-pyshop-1.4.0/pyshop/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/pyshop/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1564 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/helpers/typing_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/pyshop/lp_model/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2195 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2555 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/lp_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10661 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/row.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9366 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/lp_model/var.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13496 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shop_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/pyshop/shopcore/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/command_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24862 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12969 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/script_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14831 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/shop_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/pyshop/shopcore/shop_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5293 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-09 12:54:10.000000 sintef-pyshop-1.4.0/sintef_pyshop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 12:54:10.412684 sintef-pyshop-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/tests/test_helpers_command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/tests/test_helpers_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7580 2023-05-09 12:53:59.000000 sintef-pyshop-1.4.0/tests/test_shop_api.py
```

### Comparing `sintef-pyshop-1.3.1/LICENSE` & `sintef-pyshop-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/PKG-INFO` & `sintef-pyshop-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://github.com/sintef-energy/pyshop
```

### Comparing `sintef-pyshop-1.3.1/README.md` & `sintef-pyshop-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/helpers/commands.py` & `sintef-pyshop-1.4.0/pyshop/helpers/commands.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/helpers/time.py` & `sintef-pyshop-1.4.0/pyshop/helpers/time.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/helpers/timeseries.py` & `sintef-pyshop-1.4.0/pyshop/helpers/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Compress timeseries by only keeping the first row of consecutive duplicates. This is done by comparing a copied
     DataFrame/Series that has been shifted by one, with the original, and only keeping the rows in which at least one
     one column value is different from the previous row. The first row will always be kept. NaN values must be replaced
     with a proper number before comparing since NaN != NaN. Undo the change before returning the compressed DataFrame/Series
     """
     df = df.replace(np.nan, 1e40)
     if isinstance(df, pd.DataFrame):
-        df = df.loc[(df.shift() != df).any(1)]
+        df = df.loc[(df.shift() != df).any(axis=1)]
     else:
         df = df.loc[df.shift() != df]
     df = df.replace(1e40, np.nan)
     return df
 
 
 def get_timestamp_indexed_series(starttime:pd.Timestamp, time_unit:str, t:Sequence[Union[int,float]], y:Sequence[float], column_name:str='data') -> DataFrameOrSeries:
```

### Comparing `sintef-pyshop-1.3.1/pyshop/helpers/typing_annotations.py` & `sintef-pyshop-1.4.0/pyshop/helpers/typing_annotations.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/lp_model/index.py` & `sintef-pyshop-1.4.0/pyshop/lp_model/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from typing import List, Optional, Sequence, Union
+from typing import List, Optional, Sequence, Union, Dict
 import numpy as np
 from . import lp_model
 
 
 class IndexType(object):
 
     lp_model:'lp_model.LpModelBuilder'
     id:int
 
     def __init__(self, lp_model:'lp_model.LpModelBuilder', id:int) -> None:
         self.lp_model = lp_model
         self.id = id
 
-    def __getattr__(self, attr:str) -> Union[int, str, Sequence[str]]:
+    def __getattr__(self, attr:str) -> Union[int, str, Sequence[str], Dict[int, str]]:
         if attr == 'id':
             return self.id
         elif attr == 'name':
             return self.lp_model._lp_model['index_type_names'][self.id]
         elif attr == 'description':
             id_start = self.lp_model._lp_model['index_type_desc_beg'][self.id]
             id_count = self.lp_model._lp_model['index_type_desc_cnt'][self.id]
-            return self.lp_model._lp_model['index_type_desc_val'][id_start:id_start+id_count]
+            desc_vals = self.lp_model._lp_model['index_type_desc_val'][id_start:id_start+id_count]
+            desc_indices = self.lp_model._lp_model['index_type_desc_index'][id_start:id_start+id_count]
+            return {i: v for (i,v) in zip(desc_indices, desc_vals)}
 
     def __dir__(self) -> List[str]:
         return ['id', 'name', 'description']
 
 
 class IndexTypeBuilder(object):
```

### Comparing `sintef-pyshop-1.3.1/pyshop/lp_model/lp_model.py` & `sintef-pyshop-1.4.0/pyshop/lp_model/lp_model.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/lp_model/row.py` & `sintef-pyshop-1.4.0/pyshop/lp_model/row.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/lp_model/var.py` & `sintef-pyshop-1.4.0/pyshop/lp_model/var.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/shop_runner.py` & `sintef-pyshop-1.4.0/pyshop/shop_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 import sys
-from typing import Dict, List, Optional, Callable
+from typing import Dict, List, Optional, Callable, Union
 import pandas as pd
 import numpy as np
 import requests
 
 from .helpers.commands import get_commands_from_file
 from .helpers.time import get_shop_timestring
 from .helpers.typing_annotations import CommandOptions, CommandValues, DataFrameOrSeries, Message, ShopApi
@@ -236,18 +236,18 @@
             #Stop before optimization begins if requested
             if break_before_opt and command_text == "start sim":
                 break
             
             #Reading input files should be done with proper API calls instead
             if command_text in ["read model", "add model"]:
                 if not skip_reading_input:
-                    self.read_ascii_file(os.path.join(folder, values[0]))
+                    self.read_ascii_file(os.path.join(folder, values[0].replace('"','')))
             elif command_text == "read yaml":
                 if not skip_reading_input:
-                    self.load_yaml(folder,values[0])
+                    self.load_yaml(folder,values[0].replace('"',''))
             else:            
                 #Directly execute all other commands
                 self.shop_api.ExecuteCommand(command_text, options, values)
 
     def run_command_file_progress(self, folder:str, command_file:str) -> None:
         with open(os.path.join(folder, command_file), 'r', encoding='iso-8859-1') as run_file:
             file_string = run_file.read()
@@ -284,8 +284,35 @@
             info = l[1]
 
             if info not in license_dict.keys():
                 license_dict[info] = [name]
             else:
                 license_dict[info].append(name)
 
-        return license_dict
+        return license_dict
+    
+    def get_message_definitions(self) -> Dict[str, List[Union[str, int]]]:
+        try:
+            messageVector = self.shop_api.GetAllMessages()
+        except AttributeError:
+            print("Function get_message_definitions can only be used for SHOP 15.1.1.0 and newer")
+            return {}
+        
+        allCodes = []
+        allTexts = []
+        allTypes = []
+        allCallCounts = []
+
+        for i in messageVector:
+            allCodes.append(int(i[0]))
+            allTypes.append(i[1])
+            allTexts.append(i[2])
+            allCallCounts.append(int(i[3]))
+        
+        messageDefinitions = {
+            "code": allCodes,
+            "type": allTypes,
+            "text": allTexts,
+            "callCount": allCallCounts
+        }
+
+        return messageDefinitions
```

### Comparing `sintef-pyshop-1.3.1/pyshop/shopcore/command_builder.py` & `sintef-pyshop-1.4.0/pyshop/shopcore/command_builder.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/shopcore/model_builder.py` & `sintef-pyshop-1.4.0/pyshop/shopcore/model_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -221,14 +221,16 @@
             return AttributeObject(self._shop_api, self._type, self._name, attr_name, self.datatype_dict[attr_name])
         elif attr_name == 'generators' and self._type == 'plant':
             return self._get_generators()
         elif attr_name == 'pumps' and self._type == 'plant':
             return self._get_pumps()            
         elif attr_name == 'unit_combinations' and self._type == 'plant':
             return self._get_unit_combinations()
+        elif attr_name == 'needle_combinations' and self._type == 'generator':
+            return self._get_needle_combinations()        
         else:
             raise ValueError(f'Unknown attribute: "{attr_name}" for "{self._name}" ({self._type})')
 
     def __dir__(self) -> List[str]:
         dirs = [x for x in super().__dir__() if x[0] != '_'] + self._attr_names
         if self._type == 'plant':
             return dirs + ['generators','pumps','unit_combinations']
@@ -266,14 +268,25 @@
         connected_indices = self._shop_api.GetRelations(self._type, self._name, 'connection_standard')
         comb_names = [object_names[i] for i in connected_indices if object_types[i] == 'unit_combination']
         comb_objects = []
         for comb_name in comb_names:
             new_comb = AttributeBuilderObject(self._shop_api, 'unit_combination', comb_name)
             comb_objects.append(new_comb)
         return comb_objects
+    
+    def _get_needle_combinations(self) -> List['AttributeBuilderObject']:
+        object_names = self._shop_api.GetObjectNamesInSystem()
+        object_types = self._shop_api.GetObjectTypesInSystem()
+        connected_indices = self._shop_api.GetRelations(self._type, self._name, 'connection_standard')
+        needle_comb_names = [object_names[i] for i in connected_indices if object_types[i] == 'needle_combination']
+        needle_comb_objects = []
+        for needle_comb_name in needle_comb_names:
+            new_needle_comb = AttributeBuilderObject(self._shop_api, 'needle_combination', needle_comb_name)
+            needle_comb_objects.append(new_needle_comb)
+        return needle_comb_objects        
 
     def get_relations(self, direction:str="both", relation_type:str="all", relation_category:str='both') -> List['AttributeBuilderObject']:
         direction = direction.lower()
         relation_type = relation_type.lower()
         relation_category = relation_category.lower()
         if direction not in ["both", "input", "output"]:
             raise ValueError('Unknown direction, valid values are "both", "input" and "output"')
```

### Comparing `sintef-pyshop-1.3.1/pyshop/shopcore/script_generator.py` & `sintef-pyshop-1.4.0/pyshop/shopcore/script_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,259 +1,270 @@
 from ..helpers.typing_annotations import ShopApi
 from ..helpers.timeseries import remove_consecutive_duplicates
 from .shop_api import get_time_resolution, get_attribute_value
 
+import unicodedata
+
 def write_pyshop_model_file(file_path:str, shop_api:ShopApi, static_data_only:bool) -> None:
 
     #Write a pyshop script file to recreate the current input model definition
+    with open(file_path,"w",encoding="utf-8") as f:
+        #Basic imports
+        f.write("from pyshop import ShopSession\n")
+        f.write("import pandas as pd\n")
+
+        #Manually import Timestamp from pandas so that Timestamp objects can be written directly to the file as strings
+        f.write("from pandas import Timestamp\n")
+        #Manually import nan from numpy so that nan values in TXYs can be written directly to the file as strings
+        f.write("from numpy import nan\n")
+        f.write("\n")
+
+        #Init ShopSession
+        f.write("def get_model() -> ShopSession:\n\n")
+        f.write("    #Initialize a new ShopSession\n")
+        f.write("    shop = ShopSession()\n\n")
+
+        #Set time resolution
+        time_res = get_time_resolution(shop_api)
+        f.write("    #Set the time resolution of the optimization\n")
+        f.write(f"    start_time = Timestamp('{time_res['starttime']}')\n")
+        f.write(f"    end_time = Timestamp('{time_res['endtime']}')\n")
+        step_length = remove_consecutive_duplicates(time_res['timeresolution'])
+        t = list(step_length.index)
+        y = list(step_length.values)
+        f.write(f"    t = {t}\n")
+        f.write(f"    y = {y}\n")
+        f.write(f"    step_length = pd.Series(y,index=t)\n")
+        f.write(f"    shop.set_time_resolution(start_time, end_time, '{time_res['timeunit']}', step_length)\n")
+        f.write("\n")
+
+        all_types = shop_api.GetObjectTypesInSystem()
+        all_names = shop_api.GetObjectNamesInSystem()
+
+        #Save the objects in the same order every time
+        unique_types = list(set(all_types))
+        unique_types.sort(reverse=True)
+
+        #Save a list of all 'active' objects with attributes to write
+        objects = []
+        for obj_type in unique_types:
+            
+            #Always skip the scenario object if there is only one of them
+            if obj_type == "scenario" and all_types.count("scenario") == 1:
+                continue
+            
+            attributes = shop_api.GetObjectTypeAttributeNames(obj_type)
+            datatypes = shop_api.GetObjectTypeAttributeDatatypes(obj_type)
 
-        with open(file_path,"w",encoding="utf-8") as f:
-            #Basic imports
-            f.write("from pyshop import ShopSession\n")
-            f.write("import pandas as pd\n")
-
-            #Manually import Timestamp from pandas so that Timestamp objects can be written directly to the file as strings
-            f.write("from pandas import Timestamp\n")
-            #Manually import nan from numpy so that nan values in TXYs can be written directly to the file as strings
-            f.write("from numpy import nan\n")
-            f.write("\n")
-
-            #Init ShopSession
-            f.write("def get_model() -> ShopSession:\n\n")
-            f.write("    #Initialize a new ShopSession\n")
-            f.write("    shop = ShopSession()\n\n")
-
-            #Set time resolution
-            time_res = get_time_resolution(shop_api)
-            f.write("    #Set the time resolution of the optimization\n")
-            f.write(f"    start_time = Timestamp('{time_res['starttime']}')\n")
-            f.write(f"    end_time = Timestamp('{time_res['endtime']}')\n")
-            step_length = remove_consecutive_duplicates(time_res['timeresolution'])
-            t = list(step_length.index)
-            y = list(step_length.values)
-            f.write(f"    t = {t}\n")
-            f.write(f"    y = {y}\n")
-            f.write(f"    step_length = pd.Series(y,index=t)\n")
-            f.write(f"    shop.set_time_resolution(start_time, end_time, '{time_res['timeunit']}', step_length)\n")
-            f.write("\n")
-
-            all_types = shop_api.GetObjectTypesInSystem()
-            all_names = shop_api.GetObjectNamesInSystem()
-
-            #Save the objects in the same order every time
-            unique_types = list(set(all_types))
-            unique_types.sort(reverse=True)
-
-            #Save a list of all 'active' objects with attributes to write
-            objects = []
-            for obj_type in unique_types:
+            input_attributes = []
+            input_datatypes = []
+            for attr,dtype in zip(attributes,datatypes):
                 
-                #Always skip the scenario object if there is only one of them
-                if obj_type == "scenario" and all_types.count("scenario") == 1:
+                #Don't include time dependent data if specified
+                if static_data_only and (dtype == "txy" or dtype == "xyt"):
                     continue
-                
-                attributes = shop_api.GetObjectTypeAttributeNames(obj_type)
-                datatypes = shop_api.GetObjectTypeAttributeDatatypes(obj_type)
 
-                input_attributes = []
-                input_datatypes = []
-                for attr,dtype in zip(attributes,datatypes):
-                    
-                    #Don't include time dependent data if specified
-                    if static_data_only and (dtype == "txy" or dtype == "xyt"):
-                        continue
+                #Don't include output attributes
+                if shop_api.GetAttributeInfo(obj_type, attr, "isInput") == "False":
+                    continue
 
-                    #Don't include output attributes
-                    if shop_api.GetAttributeInfo(obj_type, attr, "isInput") == "False":
-                        continue
+                #Don't include internal attributes
+                if "INTERNAL" in shop_api.GetAttributeInfo(obj_type, attr, "licenseName"):
+                    continue
 
-                    #Don't include internal attributes
-                    if "INTERNAL" in shop_api.GetAttributeInfo(obj_type, attr, "licenseName"):
-                        continue
+                input_attributes.append(attr)
+                input_datatypes.append(dtype)
 
-                    input_attributes.append(attr)
-                    input_datatypes.append(dtype)
+            obj_names = [name for name,other_type in zip(all_names,all_types) if other_type==obj_type]
 
-                obj_names = [name for name,other_type in zip(all_names,all_types) if other_type==obj_type]
+            for i,name in enumerate(obj_names):
 
-                for i,name in enumerate(obj_names):
+                active_attributes = []
+                active_attribute_names = []
+                active_attribute_datatypes = []
+                for attr,dtype in zip(input_attributes,input_datatypes):
+                    
+                    #Skip attributes that are default for the object
+                    if shop_api.AttributeIsDefault(obj_type,name,attr):
+                        continue             
 
-                    active_attributes = []
-                    active_attribute_names = []
-                    active_attribute_datatypes = []
-                    for attr,dtype in zip(input_attributes,input_datatypes):
+                    val = get_attribute_value(shop_api,name,obj_type,attr,dtype)
+                    
+                    #Skip attributes that were actually not active
+                    if val is None:
+                        continue
+                    
+                    active_attributes.append(val)
+                    active_attribute_names.append(attr)
+                    active_attribute_datatypes.append(dtype)
+
+                #Add another active object if there is at least one active input attribute OR the object is an (empty) input object
+                if len(active_attributes) > 0 or shop_api.GetObjectInfo(obj_type,"isInput") == "True":
+                    obj = {}
+                    obj["type"] = obj_type
+                    obj["name"] = name
+
+                    if obj_type == "global_settings":
+                        obj["code_name"] = "global_settings"
+                    else:
+                        clean_name = name.lower()
+                        #Manually convert nordic characters
+                        clean_name = clean_name.replace("æ","ae")
+                        clean_name = clean_name.replace("ø","oe")
+                        clean_name = clean_name.replace("å","aa")                         
+
+                        #Normalize and convert/ignore other strange characters in the name
+                        clean_name = unicodedata.normalize("NFKD", clean_name).encode("ascii", "ignore").decode()
+
+                        #Replace space and remove all special characters that can't be used for variable names in Python
+                        clean_name = clean_name.replace(" ","_")
+                        illegal_characters = '''~`!@#$%^&*-+={}[]|\/:;"'<>,.?()'''                           
+                        clean_name = clean_name.translate({ord(i): None for i in illegal_characters})
                         
-                        #Skip attributes that are default for the object
-                        if shop_api.AttributeIsDefault(obj_type,name,attr):
-                            continue             
+                        obj["code_name"] = f"{obj_type}_{clean_name}".replace("__","_")
 
-                        val = get_attribute_value(shop_api,name,obj_type,attr,dtype)
-                        
-                        #Skip attributes that were actually not active
-                        if val is None:
-                            continue
+                    obj["attributes"] = active_attributes
+                    obj["attribute_names"] = active_attribute_names
+                    obj["attribute_datatypes"] = active_attribute_datatypes                     
+                    objects.append(obj)
+                    
+        #Write the active input attributes of each object to the file
+        f.write("    #Add all objects and set all attributes\n")
+        for obj in objects:
                         
-                        active_attributes.append(val)
-                        active_attribute_names.append(attr)
-                        active_attribute_datatypes.append(dtype)
-
-                    #Add another active object if there is at least one active input attribute OR the object is an (empty) input object
-                    if len(active_attributes) > 0 or shop_api.GetObjectInfo(obj_type,"isInput") == "True":
-                        obj = {}
-                        obj["type"] = obj_type
-                        obj["name"] = name
+            var_name = obj["code_name"]
+            obj_type = obj["type"]
+            name = obj["name"]
+            
+            #Create or retrieve the object depending on if it is an input type or not
+            if shop_api.GetObjectInfo(obj_type,"isInput") == "True":
+                f.write(f"    {var_name} = shop.model.{obj_type}.add_object('{name}')\n")
+            else:
+                f.write(f"    {var_name} = shop.model.{obj_type}['{name}']\n")
 
-                        if obj_type == "global_settings":
-                            obj["code_name"] = "global_settings"
-                        else:
-                            clean_name = name.lower()
-                            clean_name = clean_name.replace("æ","ae")
-                            clean_name = clean_name.replace("ø","oe")
-                            clean_name = clean_name.replace("å","aa")
-                            obj["code_name"] = f"{obj_type}_{clean_name}"
-
-                        obj["attributes"] = active_attributes
-                        obj["attribute_names"] = active_attribute_names
-                        obj["attribute_datatypes"] = active_attribute_datatypes                     
-                        objects.append(obj)
-                        
-            #Write the active input attributes of each object to the file
-            f.write("    #Add all objects and set all attributes\n")
-            for obj in objects:
-                           
-                var_name = obj["code_name"]
-                obj_type = obj["type"]
-                name = obj["name"]
-                
-                #Create or retrieve the object depending on if it is an input type or not
-                if shop_api.GetObjectInfo(obj_type,"isInput") == "True":
-                    f.write(f"    {var_name} = shop.model.{obj_type}.add_object('{name}')\n")
-                else:
-                    f.write(f"    {var_name} = shop.model.{obj_type}['{name}']\n")
-
-                #Set all active attributes
-                for val,attr,dtype in zip(obj["attributes"],obj["attribute_names"],obj["attribute_datatypes"]):
-
-                    if dtype in ["int", "double", "int_array", "double_array"]:
-                        f.write(f"    {var_name}.{attr}.set({val})\n")
-                    elif dtype == "string":
-                        f.write(f"    {var_name}.{attr}.set('{val}')\n")
-                    elif dtype == "string_array":
-                        input_list = f"['{val[0]}'"
-                        for v in val[1:]:
-                            input_list += f", '{v}'"
-                        input_list += "]"
-                        f.write(f"    {var_name}.{attr}.set({input_list})\n")           
-                    elif dtype == "sy":
-                        f.write(f"    s = {list(val.index)}\n")
-                        f.write(f"    y = {list(val.values)}\n")
-                        f.write(f"    {var_name}.{attr}.set(pd.Series(y,index=s))\n")                                
-                    elif dtype == "xy":
-                        f.write(f"    x = {list(val.index)}\n")
-                        f.write(f"    y = {list(val.values)}\n")
-                        f.write(f"    {var_name}.{attr}.set(pd.Series(y,index=x,name={val.name}))\n")    
-                    elif dtype == "xy_array":
-                        f.write("    xy_curves = []\n")
-                        for xy in val:
-                            f.write(f"    x = {list(xy.index)}\n")
-                            f.write(f"    y = {list(xy.values)}\n")
-                            f.write(f"    xy_curves.append(pd.Series(y,index=x,name={xy.name}))\n")
-                        f.write(f"    {var_name}.{attr}.set(xy_curves)\n") 
-                    elif dtype == "xyt":
-                        f.write("    xyt = []\n")
-                        for xy in val:               
-                            f.write(f"    x = {list(xy.index)}\n")
-                            f.write(f"    y = {list(xy.values)}\n")
-                            f.write(f"    xyt.append(pd.Series(y,index=x,name=Timestamp('{str(xy.name)}')))\n")
-                        f.write(f"    {var_name}.{attr}.set(xyt)\n")                                                                   
-                    elif dtype == "txy":
-                        val = remove_consecutive_duplicates(val)
-                        if len(val.values) > 1:
-                            f.write(f"    t = {list(val.index)}\n")
-                            f.write(f"    {attr} = {list(val.values)}\n")
-                            f.write(f"    {var_name}.{attr}.set(pd.Series({attr},index=t))\n")                  
-                        #Use simple syntax if there is only one value in the txy
-                        else:
-                            f.write(f"    {var_name}.{attr}.set({val.values[0]})\n")                                                                   
-                
-                f.write("\n")
+            #Set all active attributes
+            for val,attr,dtype in zip(obj["attributes"],obj["attribute_names"],obj["attribute_datatypes"]):
 
-            #Find and write all connections
-            connections = []
-            connection_types = ["standard","bypass","spill"]
+                if dtype in ["int", "double", "int_array", "double_array"]:
+                    f.write(f"    {var_name}.{attr}.set({val})\n")
+                elif dtype == "string":
+                    f.write(f"    {var_name}.{attr}.set('{val}')\n")
+                elif dtype == "string_array":
+                    input_list = f"['{val[0]}'"
+                    for v in val[1:]:
+                        input_list += f", '{v}'"
+                    input_list += "]"
+                    f.write(f"    {var_name}.{attr}.set({input_list})\n")           
+                elif dtype == "sy":
+                    f.write(f"    s = {list(val.index)}\n")
+                    f.write(f"    y = {list(val.values)}\n")
+                    f.write(f"    {var_name}.{attr}.set(pd.Series(y,index=s))\n")                                
+                elif dtype == "xy":
+                    f.write(f"    x = {list(val.index)}\n")
+                    f.write(f"    y = {list(val.values)}\n")
+                    f.write(f"    {var_name}.{attr}.set(pd.Series(y,index=x,name={val.name}))\n")    
+                elif dtype == "xy_array":
+                    f.write("    xy_curves = []\n")
+                    for xy in val:
+                        f.write(f"    x = {list(xy.index)}\n")
+                        f.write(f"    y = {list(xy.values)}\n")
+                        f.write(f"    xy_curves.append(pd.Series(y,index=x,name={xy.name}))\n")
+                    f.write(f"    {var_name}.{attr}.set(xy_curves)\n") 
+                elif dtype == "xyt":
+                    f.write("    xyt = []\n")
+                    for xy in val:               
+                        f.write(f"    x = {list(xy.index)}\n")
+                        f.write(f"    y = {list(xy.values)}\n")
+                        f.write(f"    xyt.append(pd.Series(y,index=x,name=Timestamp('{str(xy.name)}')))\n")
+                    f.write(f"    {var_name}.{attr}.set(xyt)\n")                                                                   
+                elif dtype == "txy":
+                    val = remove_consecutive_duplicates(val)
+                    if len(val.values) > 1:
+                        f.write(f"    t = {list(val.index)}\n")
+                        f.write(f"    {attr} = {list(val.values)}\n")
+                        f.write(f"    {var_name}.{attr}.set(pd.Series({attr},index=t))\n")                  
+                    #Use simple syntax if there is only one value in the txy
+                    else:
+                        f.write(f"    {var_name}.{attr}.set({val.values[0]})\n")                                                                   
             
-            f.write("\n    #Connect all objects\n")
-            for obj in objects:
-                
-                up_name = obj["code_name"]
-                obj_type = obj["type"]
-                name = obj["name"]
+            f.write("\n")
+
+        #Find and write all connections
+        connections = []
+        connection_types = ["standard","bypass","spill"]
+        
+        f.write("\n    #Connect all objects\n")
+        for obj in objects:
+            
+            up_name = obj["code_name"]
+            obj_type = obj["type"]
+            name = obj["name"]
+            
+            wrote_connection = False
+
+            for ctype in connection_types:
                 
-                wrote_connection = False
+                #Get connected objects for the connection type
+                related_indices = shop_api.GetRelations(obj_type, name, f"connection_{ctype}")
+            
+                for i in related_indices:   
 
-                for ctype in connection_types:
+                    rel_name = all_names[i]
+                    rel_type = all_types[i]
+
+                    #Find the related object in the active object list
+                    rel_obj = None
+                    for o in objects:
+                        if o["name"] == rel_name and o["type"] == rel_type:
+                            rel_obj = o
+                            break
+
+                    if rel_obj is None:
+                        print(f"Object {rel_type} {rel_name} related to {obj} not found!")
+                        raise RuntimeError
+
+                    #Check if the connection (or its reverse) has already been added
+                    connection_exists = False
+                    for c in connections:
+
+                        identical = c["from"] == obj and c["to"] == rel_obj
+                        reversed = c["from"] == rel_obj and c["to"] == obj
+
+                        if identical or reversed:
+                            connection_exists = True
+                            break
                     
-                    #Get connected objects for the connection type
-                    related_indices = shop_api.GetRelations(obj_type, name, f"connection_{ctype}")
-                
-                    for i in related_indices:   
+                    #Add the connection to the list and write the line to connect the two objects
+                    if not connection_exists:                            
 
-                        rel_name = all_names[i]
-                        rel_type = all_types[i]
+                        connections.append({"from":obj,"to":rel_obj,"connection_type":ctype})
+                        down_name = rel_obj["code_name"]
+                        if ctype == "standard":
+                            f.write(f"    {up_name}.connect_to({down_name})\n")
+                        else:
+                            f.write(f"    {up_name}.connect_to({down_name},connection_type='{ctype}')\n")
+                        wrote_connection = True
+            
+            #Add a new line when we are done writing connections for an object
+            if wrote_connection:
+                f.write("\n")
 
-                        #Find the related object in the active object list
-                        rel_obj = None
-                        for o in objects:
-                            if o["name"] == rel_name and o["type"] == rel_type:
-                                rel_obj = o
-                                break
-
-                        if rel_obj is None:
-                            print(f"Object {rel_type} {rel_name} related to {obj} not found!")
-                            raise RuntimeError
-
-                        #Check if the connection (or its reverse) has already been added
-                        connection_exists = False
-                        for c in connections:
-
-                            identical = c["from"] == obj and c["to"] == rel_obj
-                            reversed = c["from"] == rel_obj and c["to"] == obj
-
-                            if identical or reversed:
-                                connection_exists = True
-                                break
-                        
-                        #Add the connection to the list and write the line to connect the two objects
-                        if not connection_exists:                            
+        f.write("    return shop\n\n")
 
-                            connections.append({"from":obj,"to":rel_obj,"connection_type":ctype})
-                            down_name = rel_obj["code_name"]
-                            if ctype == "standard":
-                                f.write(f"    {up_name}.connect_to({down_name})\n")
-                            else:
-                                f.write(f"    {up_name}.connect_to({down_name},connection_type='{ctype}')\n")
-                            wrote_connection = True
-                
-                #Add a new line when we are done writing connections for an object
-                if wrote_connection:
-                    f.write("\n")
-
-            f.write("    return shop\n\n")
-
-            #Create a function to run all the executed commands in this session
-            #There will probably be overlap with the values directly set on the global_settings object, this should not matter
-            commands = shop_api.GetExecutedCommands()
-            f.write("def run_commands(shop:ShopSession) -> None:\n\n")
-            if len(commands) == 0:
-                f.write("    #No commands to execute\n")
-                f.write("    pass\n")
-            else:
-                f.write("    #Commands to execute\n")
-                for c in commands:
-                    #Skip reading input commands since the model is already defined
-                    if "read model" in c or "add model" in c or "read yaml" in c:
-                        continue
-                    f.write(f"    shop.execute_full_command('{c}')\n")
+        #Create a function to run all the executed commands in this session
+        #There will probably be overlap with the values directly set on the global_settings object, this should not matter
+        commands = shop_api.GetExecutedCommands()
+        f.write("def run_commands(shop:ShopSession) -> None:\n\n")
+        if len(commands) == 0:
+            f.write("    #No commands to execute\n")
+            f.write("    pass\n")
+        else:
+            f.write("    #Commands to execute\n")
+            for c in commands:
+                #Skip reading input commands since the model is already defined
+                if "read model" in c or "add model" in c or "read yaml" in c:
+                    continue
+                f.write(f"    shop.execute_full_command('{c}')\n")
 
-            f.write("\n")
-            f.write("shop = get_model()\n")
-            f.write("run_commands(shop)\n")
+        f.write("\n")
+        f.write("shop = get_model()\n")
+        f.write("run_commands(shop)\n")
```

### Comparing `sintef-pyshop-1.3.1/pyshop/shopcore/shop_api.py` & `sintef-pyshop-1.4.0/pyshop/shopcore/shop_api.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/pyshop/shopcore/shop_rest.py` & `sintef-pyshop-1.4.0/pyshop/shopcore/shop_rest.py`

 * *Files identical despite different names*

### Comparing `sintef-pyshop-1.3.1/setup.py` & `sintef-pyshop-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(name='sintef-pyshop',
-      version='1.3.1',
+      version='1.4.0',
       author='SINTEF Energy Research',
       description='Python interface to SHOP',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['pyshop',
                 'pyshop.helpers',
                 'pyshop.shopcore',
```

### Comparing `sintef-pyshop-1.3.1/sintef_pyshop.egg-info/PKG-INFO` & `sintef-pyshop-1.4.0/sintef_pyshop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sintef-pyshop
-Version: 1.3.1
+Version: 1.4.0
 Summary: Python interface to SHOP
 Home-page: http://www.sintef.no/programvare/SHOP
 Author: SINTEF Energy Research
 Author-email: support.energy@sintef.no
 License: MIT
 Project-URL: Documentation, https://shop.sintef.energy/documentation/tutorials/pyshop/
 Project-URL: Source, https://github.com/sintef-energy/pyshop
```

### Comparing `sintef-pyshop-1.3.1/sintef_pyshop.egg-info/SOURCES.txt` & `sintef-pyshop-1.4.0/sintef_pyshop.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 pyshop/shopcore/script_generator.py
 pyshop/shopcore/shop_api.py
 pyshop/shopcore/shop_rest.py
 sintef_pyshop.egg-info/PKG-INFO
 sintef_pyshop.egg-info/SOURCES.txt
 sintef_pyshop.egg-info/dependency_links.txt
 sintef_pyshop.egg-info/requires.txt
-sintef_pyshop.egg-info/top_level.txt
+sintef_pyshop.egg-info/top_level.txt
+tests/test_helpers_command.py
+tests/test_helpers_time.py
+tests/test_shop_api.py
```

