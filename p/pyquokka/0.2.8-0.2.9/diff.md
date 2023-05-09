# Comparing `tmp/pyquokka-0.2.8-py3-none-any.whl.zip` & `tmp/pyquokka-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 288013 bytes, number of entries: 39
--rw-rw-r--  2.0 unx      309 b- defN 23-May-09 16:09 pyquokka/__init__.py
+Zip file size: 288009 bytes, number of entries: 39
+-rw-rw-r--  2.0 unx      309 b- defN 23-May-09 16:28 pyquokka/__init__.py
 -rw-rw-r--  2.0 unx     4291 b- defN 23-Apr-21 22:04 pyquokka/catalog.py
 -rw-rw-r--  2.0 unx      372 b- defN 23-Apr-21 22:04 pyquokka/common_startup.sh
 -rw-rw-r--  2.0 unx    28239 b- defN 23-Apr-21 22:04 pyquokka/coordinator.py
 -rw-rw-r--  2.0 unx    48179 b- defN 23-May-09 05:45 pyquokka/core.py
 -rw-rw-r--  2.0 unx    48426 b- defN 23-Apr-21 22:04 pyquokka/dataset.py
 -rw-rw-r--  2.0 unx    98944 b- defN 23-May-09 05:06 pyquokka/datastream.py
 -rw-rw-r--  2.0 unx     1438 b- defN 23-Apr-21 22:04 pyquokka/debugger.py
--rw-rw-r--  2.0 unx    76129 b- defN 23-May-09 15:51 pyquokka/df.py
+-rw-rw-r--  2.0 unx    76119 b- defN 23-May-09 16:27 pyquokka/df.py
 -rw-rw-r--  2.0 unx    37360 b- defN 23-Apr-21 22:04 pyquokka/executors.py
 -rw-rw-r--  2.0 unx    12657 b- defN 23-Apr-21 22:04 pyquokka/expression.py
 -rw-rw-r--  2.0 unx    17483 b- defN 23-Apr-21 22:04 pyquokka/flight.py
 -rw-rw-r--  2.0 unx     3098 b- defN 23-May-09 03:48 pyquokka/hbq.py
 -rwxrwxr-x  2.0 unx   368480 b- defN 23-Apr-21 22:04 pyquokka/ldb.so
 -rw-rw-r--  2.0 unx      274 b- defN 23-Apr-21 22:04 pyquokka/leader_start_ray.sh
 -rw-rw-r--  2.0 unx      619 b- defN 23-Apr-21 22:04 pyquokka/leader_startup.sh
@@ -29,13 +29,13 @@
 -rw-rw-r--  2.0 unx    39151 b- defN 23-May-09 15:31 pyquokka/utils.py
 -rw-rw-r--  2.0 unx     4081 b- defN 23-Apr-21 22:04 pyquokka/windowtypes.py
 -rw-rw-r--  2.0 unx      146 b- defN 23-May-09 04:03 pyquokka/executors/__init__.py
 -rw-rw-r--  2.0 unx      811 b- defN 23-May-08 15:34 pyquokka/executors/base_executor.py
 -rw-rw-r--  2.0 unx    17511 b- defN 23-May-09 04:03 pyquokka/executors/sql_executors.py
 -rw-rw-r--  2.0 unx    17185 b- defN 23-May-09 04:03 pyquokka/executors/ts_executors.py
 -rw-rw-r--  2.0 unx     2870 b- defN 23-May-09 05:34 pyquokka/executors/vector_executors.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-May-09 16:15 pyquokka-0.2.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1020 b- defN 23-May-09 16:15 pyquokka-0.2.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-09 16:15 pyquokka-0.2.8.dist-info/WHEEL
--rwxrwxr-x  2.0 unx        9 b- defN 23-May-09 16:15 pyquokka-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3116 b- defN 23-May-09 16:15 pyquokka-0.2.8.dist-info/RECORD
-39 files, 1038826 bytes uncompressed, 283147 bytes compressed:  72.7%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-May-09 16:30 pyquokka-0.2.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1020 b- defN 23-May-09 16:30 pyquokka-0.2.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-09 16:30 pyquokka-0.2.9.dist-info/WHEEL
+-rwxrwxr-x  2.0 unx        9 b- defN 23-May-09 16:30 pyquokka-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3116 b- defN 23-May-09 16:30 pyquokka-0.2.9.dist-info/RECORD
+39 files, 1038816 bytes uncompressed, 283143 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -96,23 +96,23 @@
 
 Filename: pyquokka/executors/ts_executors.py
 Comment: 
 
 Filename: pyquokka/executors/vector_executors.py
 Comment: 
 
-Filename: pyquokka-0.2.8.dist-info/LICENSE
+Filename: pyquokka-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: pyquokka-0.2.8.dist-info/METADATA
+Filename: pyquokka-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: pyquokka-0.2.8.dist-info/WHEEL
+Filename: pyquokka-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyquokka-0.2.8.dist-info/top_level.txt
+Filename: pyquokka-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyquokka-0.2.8.dist-info/RECORD
+Filename: pyquokka-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyquokka/__init__.py

```diff
@@ -8,8 +8,8 @@
 from . import orderedstream
 from . import tables
 from . import task
 from . import hbq
 
 from .df import QuokkaContext
 
-__version__ = '0.2.8'
+__version__ = '0.2.9'
```

## pyquokka/df.py

```diff
@@ -764,19 +764,19 @@
                                  0: PassThroughPartitioner()}, node=DataSetNode(schema), schema=schema)
         return DataSet(self, schema, stream.source_node_id)
 
     def optimize(self, node_id):
         self.__push_ann__()
         self.__push_filter__(node_id)
         self.__early_projection__(node_id)
-        # self.__fold_map__(node_id)
-        # if self.sql_config["optimize_joins"]:
-        #     self.__merge_joins__(node_id)
-        # self.__propagate_cardinality__(node_id)
-        # self.__determine_stages__(node_id)
+        self.__fold_map__(node_id)
+        if self.sql_config["optimize_joins"]:
+            self.__merge_joins__(node_id)
+        self.__propagate_cardinality__(node_id)
+        self.__determine_stages__(node_id)
         
         assert len(self.execution_nodes[node_id].parents) == 1
         parent_idx = list(self.execution_nodes[node_id].parents)[0]
         parent_id = self.execution_nodes[node_id].parents[parent_idx]
 
         if issubclass(type(self.execution_nodes[parent_id]), SourceNode):
             self.execution_nodes[node_id].blocking = True
```

## Comparing `pyquokka-0.2.8.dist-info/LICENSE` & `pyquokka-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyquokka-0.2.8.dist-info/METADATA` & `pyquokka-0.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquokka
-Version: 0.2.8
+Version: 0.2.9
 Summary: Quokka
 Author: Tony Wang
 Author-email: zihengw@stanford.edu
 License: http://www.apache.org/licenses/LICENSE-2.0
 Keywords: python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyquokka-0.2.8.dist-info/RECORD` & `pyquokka-0.2.9.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pyquokka/__init__.py,sha256=dCpFpXk81q0aL2Umoye0o4Ad4wsDzYnmvXmavLcJGeU,309
+pyquokka/__init__.py,sha256=wDw5IDuVPjlYJ2iMpyYDOZRhteJtZsDQSbpyb9B_qdg,309
 pyquokka/catalog.py,sha256=XczH9nRAjYE0eWvPdoI_sQE1N85vflPouzjpIe0lqOA,4291
 pyquokka/common_startup.sh,sha256=Rst9lyiO_Fx34swl6_-Z8w7lRHQM-8GDhsUFCbS_kP8,372
 pyquokka/coordinator.py,sha256=s7yjNB_F6bEoWoko_5cTfN0BAyH9AcYm2PKIbqJexhI,28239
 pyquokka/core.py,sha256=BQoZLOBXUpI2peE8rIgp1a0gC-Pk0nMCzlz8V1dkq6s,48179
 pyquokka/dataset.py,sha256=vgKT07HkV_P0LVu5JHijEHvYUkeQZElbgLnMC8yw_jg,48426
 pyquokka/datastream.py,sha256=X34J074YncZqikKloV4wHGdpTB5kGoBv6TluPSVv1nY,98944
 pyquokka/debugger.py,sha256=Yi1CqGHbV2y2bszUhKuxcQ561vugc6hs6xfnpJ8HIjU,1438
-pyquokka/df.py,sha256=ZbHcGUdHeD2ZvnTspqhfBCvB6G7Yi63ALW1u5qixZEw,76129
+pyquokka/df.py,sha256=C3vAduJYuMW-bM8uPl6UGpiuM8hslQ7unGeMfKx9ji8,76119
 pyquokka/executors.py,sha256=dVzy3_WbsMtbAWay2UlEgE1GmxEVbT6Fz1X9i2elboY,37360
 pyquokka/expression.py,sha256=SmJxvGrSgW3ra8EU5SLGbQ8AxbJ2bPxKHLvbXpQ-8WY,12657
 pyquokka/flight.py,sha256=ri1aEXtn4s2_ACD8PfU5EIy_fA7FlNrM61WuUjQ9Pl8,17483
 pyquokka/hbq.py,sha256=V3nE2IcIIclxxdDyXRdzuV7_y_DRa90B_aVaa6aU9tg,3098
 pyquokka/ldb.so,sha256=SO70uhXN219Ns5RNIEePv1fs0qRSksc6yq2eN0tucw8,368480
 pyquokka/leader_start_ray.sh,sha256=vyZi-Utmj7r8Qr43YmOQq3uIuAN5Nn4F61MIszzdit4,274
 pyquokka/leader_startup.sh,sha256=yOP5vjuLS9D2WtcozcFewXQB84p8jm8IcyltYcuWNss,619
@@ -28,12 +28,12 @@
 pyquokka/utils.py,sha256=sn_Rs0BIGfkmtN8rNfWGOSKJ_1btLTDk8-SW9SazJQ0,39151
 pyquokka/windowtypes.py,sha256=zPh9QgwSQ3E00eNQM8jk2iQZNMuzAQ3eoaFDm1H5NGk,4081
 pyquokka/executors/__init__.py,sha256=48lCF53HMa4Od5yyQfV8T2X0aLL5q9LZ0XVO_0-_MtA,146
 pyquokka/executors/base_executor.py,sha256=clVkP0wf03OMG7x9vMdzRPTviT5DE6rQv3n6E81bZM4,811
 pyquokka/executors/sql_executors.py,sha256=35xL26SqKQQCwqmCVyWxHKtdkHpWCbGoSjvoufJqHFk,17511
 pyquokka/executors/ts_executors.py,sha256=KPRjeMap_PogESYfqYpCBrLyVgRKVrGxWQYICQRehEo,17185
 pyquokka/executors/vector_executors.py,sha256=hs7mrwyXf3Dcvn0pvG9p_IFaJgX0xbCfxUaFj7-WCGQ,2870
-pyquokka-0.2.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pyquokka-0.2.8.dist-info/METADATA,sha256=TFvrGARo30jYPMHNo6hvmcAVBWDlzez4OV6FyENhEME,1020
-pyquokka-0.2.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pyquokka-0.2.8.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
-pyquokka-0.2.8.dist-info/RECORD,,
+pyquokka-0.2.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pyquokka-0.2.9.dist-info/METADATA,sha256=D9BHEUARLypwBwZ2Nfi21vXS-uv5ieTWIv-z8AdPb9U,1020
+pyquokka-0.2.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pyquokka-0.2.9.dist-info/top_level.txt,sha256=u5sX_ng3imCHha6-wOUpEO0V2TufF_OHADKxb38hwHg,9
+pyquokka-0.2.9.dist-info/RECORD,,
```

