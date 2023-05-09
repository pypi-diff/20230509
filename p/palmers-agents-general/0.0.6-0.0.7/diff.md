# Comparing `tmp/palmers_agents_general-0.0.6.tar.gz` & `tmp/palmers_agents_general-0.0.7.tar.gz`

## Comparing `palmers_agents_general-0.0.6.tar` & `palmers_agents_general-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/__init__.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/base_mq_consumer.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/blobs_handler.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/models_handler.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/__init__.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/base_mq_consumer.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/blobs_handler.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/palmers_agents_general/models_handler.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.7/PKG-INFO
```

### Comparing `palmers_agents_general-0.0.6/palmers_agents_general/base_mq_consumer.py` & `palmers_agents_general-0.0.7/palmers_agents_general/base_mq_consumer.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.6/palmers_agents_general/blobs_handler.py` & `palmers_agents_general-0.0.7/palmers_agents_general/blobs_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 from io import BytesIO
 
 import pandas as pd
 from azure.storage.blob import BlobServiceClient
 
 
-def read_df_from_blob(connection_string, container_name, blob_name, local_file_name=None):
-    if local_file_name is None:
-        local_file_name = blob_name
-
+def read_df_from_blob(connection_string, container_name, blob_name):
     blob_service_client = BlobServiceClient.from_connection_string(connection_string)
     blob_client = blob_service_client.get_blob_client(container=container_name, blob=blob_name, snapshot=None)
 
-    # old method, save csv to file and then read it.
-    # with open(blob_name, "wb") as my_blob:
-    #     blob_data = blob_client.download_blob()
-    #     blob_data.readinto(my_blob)
-    #
-    # df = pd.read_csv(local_file_name)
-    # delete file at local_file_name
-    # should we???
-
-
     download_stream = blob_client.download_blob()
     csv_file = download_stream.content_as_text(encoding='utf-8-sig')
     file = BytesIO(csv_file.encode())
     df = pd.read_csv(file)
 
 
     return df
```

### Comparing `palmers_agents_general-0.0.6/palmers_agents_general/models_handler.py` & `palmers_agents_general-0.0.7/palmers_agents_general/models_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.6/LICENSE` & `palmers_agents_general-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.6/pyproject.toml` & `palmers_agents_general-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_agents_general"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_agents_general-0.0.6/PKG-INFO` & `palmers_agents_general-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_agents_general
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Assaf <assafm@sdatta.ai>, Roy  <roy@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

