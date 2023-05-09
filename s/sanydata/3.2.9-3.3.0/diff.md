# Comparing `tmp/sanydata-3.2.9.tar.gz` & `tmp/sanydata-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanydata-3.2.9.tar", last modified: Mon May  8 11:33:13 2023, max compression
+gzip compressed data, was "sanydata-3.3.0.tar", last modified: Tue May  9 02:31:34 2023, max compression
```

## Comparing `sanydata-3.2.9.tar` & `sanydata-3.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.902794 sanydata-3.2.9/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-08 11:33:13.902558 sanydata-3.2.9/PKG-INFO
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.898800 sanydata-3.2.9/sanydata/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.2.9/sanydata/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)   114403 2023-05-08 11:32:13.000000 sanydata-3.2.9/sanydata/datatools.py
--rw-r--r--   0 thao       (501) staff       (20)    20291 2022-08-29 10:08:03.000000 sanydata-3.2.9/sanydata/model_data_message_pb2.py
--rw-r--r--   0 thao       (501) staff       (20)    20370 2022-08-29 10:08:03.000000 sanydata-3.2.9/sanydata/model_data_message_pb2_grpc.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.900299 sanydata-3.2.9/sanydata.egg-info/
--rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/PKG-INFO
--rw-r--r--   0 thao       (501) staff       (20)      371 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/SOURCES.txt
--rw-r--r--   0 thao       (501) staff       (20)        1 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/dependency_links.txt
--rw-r--r--   0 thao       (501) staff       (20)      130 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/requires.txt
--rw-r--r--   0 thao       (501) staff       (20)       15 2023-05-08 11:33:13.000000 sanydata-3.2.9/sanydata.egg-info/top_level.txt
--rw-r--r--   0 thao       (501) staff       (20)       38 2023-05-08 11:33:13.902897 sanydata-3.2.9/setup.cfg
--rw-r--r--   0 thao       (501) staff       (20)      999 2023-05-08 11:31:50.000000 sanydata-3.2.9/setup.py
-drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-08 11:33:13.901966 sanydata-3.2.9/utils/
--rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.2.9/utils/__init__.py
--rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.2.9/utils/cos_handler.py
--rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.2.9/utils/file_operation.py
--rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.2.9/utils/local_handler.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.550407 sanydata-3.3.0/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-09 02:31:34.550186 sanydata-3.3.0/PKG-INFO
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.545909 sanydata-3.3.0/sanydata/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.0/sanydata/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)   114500 2023-05-09 02:31:01.000000 sanydata-3.3.0/sanydata/datatools.py
+-rw-r--r--   0 thao       (501) staff       (20)    20291 2022-08-29 10:08:03.000000 sanydata-3.3.0/sanydata/model_data_message_pb2.py
+-rw-r--r--   0 thao       (501) staff       (20)    20370 2022-08-29 10:08:03.000000 sanydata-3.3.0/sanydata/model_data_message_pb2_grpc.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.547408 sanydata-3.3.0/sanydata.egg-info/
+-rw-r--r--   0 thao       (501) staff       (20)      302 2023-05-09 02:31:33.000000 sanydata-3.3.0/sanydata.egg-info/PKG-INFO
+-rw-r--r--   0 thao       (501) staff       (20)      371 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/SOURCES.txt
+-rw-r--r--   0 thao       (501) staff       (20)        1 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/dependency_links.txt
+-rw-r--r--   0 thao       (501) staff       (20)      130 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/requires.txt
+-rw-r--r--   0 thao       (501) staff       (20)       15 2023-05-09 02:31:34.000000 sanydata-3.3.0/sanydata.egg-info/top_level.txt
+-rw-r--r--   0 thao       (501) staff       (20)       38 2023-05-09 02:31:34.550486 sanydata-3.3.0/setup.cfg
+-rw-r--r--   0 thao       (501) staff       (20)      999 2023-05-09 02:31:14.000000 sanydata-3.3.0/setup.py
+drwxr-xr-x   0 thao       (501) staff       (20)        0 2023-05-09 02:31:34.549447 sanydata-3.3.0/utils/
+-rw-r--r--   0 thao       (501) staff       (20)      103 2022-04-09 07:48:22.000000 sanydata-3.3.0/utils/__init__.py
+-rw-r--r--   0 thao       (501) staff       (20)     1328 2022-04-14 01:33:04.000000 sanydata-3.3.0/utils/cos_handler.py
+-rw-r--r--   0 thao       (501) staff       (20)     1080 2022-04-13 10:48:13.000000 sanydata-3.3.0/utils/file_operation.py
+-rw-r--r--   0 thao       (501) staff       (20)      667 2022-04-14 01:24:56.000000 sanydata-3.3.0/utils/local_handler.py
```

### Comparing `sanydata-3.2.9/sanydata/datatools.py` & `sanydata-3.3.0/sanydata/datatools.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 
     return wrapper
 
 
 class DataTools(object):
     # This programme is to get data.
     PROGRAMME = 'DataTools'
-    VERSION = '3.2.9'
+    VERSION = '3.3.0'
 
     def __init__(self, stub=None, es_hosts='http://es.sanywind.net:9200/'):
         self.es = Elasticsearch(hosts=es_hosts)
 
         if stub:
             with grpc.insecure_channel(stub, options=options) as channel:
                 stub = model_data_message_pb2_grpc.ModelDataMessageStub(channel)
@@ -412,15 +412,15 @@
         elif check_result == 2:
             df = map_fc(data=df, map_v=map_v)
         else:
             pass
         return df
 
     def pd_read_csv(self, file_data, columns, header, names, map_fc, map_v, check_result, turbine_num=None,
-                    file_type='csv', sheet_name=0):
+                    file_type='csv', sheet_name=0, file_name=None, use_filename=None):
         try:
             if file_type == 'csv':
                 df = pd.read_csv(io.BytesIO(file_data), header=header, names=names, encoding='utf-8', usecols=columns)
             elif file_type == 'excel':
                 df = pd.read_excel(io.BytesIO(file_data), header=header, names=names,
                                    usecols=columns, sheet_name=sheet_name)
         except Exception as e:
@@ -428,14 +428,16 @@
                 df = pd.read_csv(io.BytesIO(file_data), header=header, names=names, encoding='gbk', usecols=columns)
             else:
                 print(e)
         if columns:
             df = df.reindex(columns=columns)
         if turbine_num:
             df['turbine_num'] = turbine_num
+        if use_filename:
+            df['sanydata_file_name'] = file_name
         df = self.map_data(df, check_result, map_fc, map_v)
         return df
 
     def pd_read_parquet(self, file_data, columns, map_fc, map_v, check_result):
         data = io.BytesIO(file_data)
         if columns:
             schem_columns = pq.read_schema(data)
@@ -640,17 +642,16 @@
                         df = self.map_data(df, check_result, map_fc, map_v)
                         df_all.append(df)
                     else:
                         turbine_num = file_name.split('_')[1]
                         if 'cmsadaptor' in file_list[0].split('/'):
                             header = None
                             names = ['振动幅值']
-                        if use_filename:
-                            df['sanydata_file_name'] = file_name
-                        df = self.pd_read_csv(file_data, columns, header, names, map_fc, map_v, check_result, turbine_num)
+                        df = self.pd_read_csv(file_data, columns, header, names, map_fc, map_v, check_result,
+                                              turbine_num, file_name=file_name, use_filename=use_filename)
                         df_all.append(df)
                 except Exception as e:
                     print(file_name)
                     print(e)
         if len(df_all) > 0:
             df_all = pd.concat(df_all)
             df_all = df_all.reset_index(drop=True)
```

### Comparing `sanydata-3.2.9/sanydata/model_data_message_pb2.py` & `sanydata-3.3.0/sanydata/model_data_message_pb2.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.9/sanydata/model_data_message_pb2_grpc.py` & `sanydata-3.3.0/sanydata/model_data_message_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.9/setup.py` & `sanydata-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import sys
 import importlib
 
 importlib.reload(sys)
 
 setup(
     name="sanydata",
-    version="3.2.9",
+    version="3.3.0",
     keywords=["pip", "sanydata", "thao"],
     description="get data and get wind farm information",
     long_description="get data and get wind farm information",
     license="MIT Licence",
 
     url="http://gitlab.sanywind.net/sanydata/sanydata",
     author="thao",
```

### Comparing `sanydata-3.2.9/utils/cos_handler.py` & `sanydata-3.3.0/utils/cos_handler.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.9/utils/file_operation.py` & `sanydata-3.3.0/utils/file_operation.py`

 * *Files identical despite different names*

### Comparing `sanydata-3.2.9/utils/local_handler.py` & `sanydata-3.3.0/utils/local_handler.py`

 * *Files identical despite different names*

