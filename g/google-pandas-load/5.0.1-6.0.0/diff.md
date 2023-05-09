# Comparing `tmp/google_pandas_load-5.0.1-py3-none-any.whl.zip` & `tmp/google_pandas_load-6.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 13691 bytes, number of entries: 11
--rw-rw-r--  2.0 unx      166 b- defN 20-Dec-30 10:49 google_pandas_load/__init__.py
--rw-rw-r--  2.0 unx      550 b- defN 22-Apr-08 16:33 google_pandas_load/constants.py
--rw-rw-r--  2.0 unx     9214 b- defN 22-Apr-15 14:00 google_pandas_load/load_config.py
--rw-rw-r--  2.0 unx    27023 b- defN 22-Apr-15 14:00 google_pandas_load/loader.py
--rw-rw-r--  2.0 unx     3833 b- defN 22-Apr-15 14:00 google_pandas_load/loader_quick_setup.py
--rw-rw-r--  2.0 unx     1131 b- defN 22-Apr-08 16:33 google_pandas_load/utils.py
--rw-rw-r--  2.0 unx     1074 b- defN 22-Apr-15 14:11 google_pandas_load-5.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1882 b- defN 22-Apr-15 14:11 google_pandas_load-5.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Apr-15 14:11 google_pandas_load-5.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       19 b- defN 22-Apr-15 14:11 google_pandas_load-5.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      971 b- defN 22-Apr-15 14:11 google_pandas_load-5.0.1.dist-info/RECORD
-11 files, 45955 bytes uncompressed, 12027 bytes compressed:  73.8%
+Zip file size: 13898 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx      166 b- defN 22-Nov-21 13:08 google_pandas_load/__init__.py
+-rw-rw-r--  2.0 unx      550 b- defN 22-Nov-16 09:00 google_pandas_load/constants.py
+-rw-rw-r--  2.0 unx     9358 b- defN 23-May-05 09:38 google_pandas_load/load_config.py
+-rw-rw-r--  2.0 unx    27317 b- defN 23-May-09 14:22 google_pandas_load/loader.py
+-rw-rw-r--  2.0 unx     4077 b- defN 23-Jan-06 10:34 google_pandas_load/loader_quick_setup.py
+-rw-rw-r--  2.0 unx     1141 b- defN 22-Nov-26 13:47 google_pandas_load/utils.py
+-rw-rw-r--  2.0 unx     1074 b- defN 23-May-09 14:38 google_pandas_load-6.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1953 b- defN 23-May-09 14:38 google_pandas_load-6.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-09 14:38 google_pandas_load-6.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       19 b- defN 23-May-09 14:38 google_pandas_load-6.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      971 b- defN 23-May-09 14:38 google_pandas_load-6.0.0.dist-info/RECORD
+11 files, 46718 bytes uncompressed, 12234 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: google_pandas_load/loader_quick_setup.py
 Comment: 
 
 Filename: google_pandas_load/utils.py
 Comment: 
 
-Filename: google_pandas_load-5.0.1.dist-info/LICENSE
+Filename: google_pandas_load-6.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: google_pandas_load-5.0.1.dist-info/METADATA
+Filename: google_pandas_load-6.0.0.dist-info/METADATA
 Comment: 
 
-Filename: google_pandas_load-5.0.1.dist-info/WHEEL
+Filename: google_pandas_load-6.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: google_pandas_load-5.0.1.dist-info/top_level.txt
+Filename: google_pandas_load-6.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: google_pandas_load-5.0.1.dist-info/RECORD
+Filename: google_pandas_load-6.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## google_pandas_load/load_config.py

```diff
@@ -1,33 +1,30 @@
 import pandas
 from argparse import Namespace
-from typing import List, Dict, Any, Optional
+from typing import Literal, List, Dict, Any, Optional
 from google.cloud import bigquery
-from pandas.api.types import infer_dtype
-from google_pandas_load import utils
-from google_pandas_load.constants import LOCATIONS, SOURCE_LOCATIONS, \
-    DESTINATION_LOCATIONS, REVERSED_LOCATIONS, MIDDLE_LOCATIONS
+from google_pandas_load import constants, utils
 
 
 class LoadConfig:
     """Configuration for a load job.
 
     This class has the same parameters as
     :meth:`google_pandas_load.loader.Loader.load`. It is used to launch
     simultaneously load jobs as follows:
 
     - A list of LoadConfig is built.
     - The list is passed
       to :meth:`google_pandas_load.loader.Loader.multi_load`.
     """
-
     def __init__(
             self,
-            source: str,
-            destination: str,
+            source: Literal[
+                'query', 'dataset', 'bucket', 'local', 'dataframe'],
+            destination: Literal['dataset', 'bucket', 'local', 'dataframe'],
 
             data_name: Optional[str] = None,
             query: Optional[str] = None,
             dataframe: Optional[pandas.DataFrame] = None,
 
             write_disposition: Optional[str] =
             bigquery.WriteDisposition.WRITE_TRUNCATE,
@@ -71,33 +68,33 @@
             raise ValueError(msg)
 
     def _check_data_name_not_contain_slash(self):
         assert self.data_name is not None
         utils.check_data_name_not_contain_slash(self.data_name)
 
     def _check_source_value(self):
-        if self.source not in SOURCE_LOCATIONS:
+        if self.source not in constants.SOURCE_LOCATIONS:
             msg = ("source must be one of 'query' or 'dataset' "
                    "or 'bucket' or 'local' or 'dataframe")
             raise ValueError(msg)
 
     def _check_destination_value(self):
-        if self.destination not in DESTINATION_LOCATIONS:
+        if self.destination not in constants.DESTINATION_LOCATIONS:
             msg = ("destination must be one of 'dataset' "
                    "or 'bucket' or 'local' or 'dataframe'")
             raise ValueError(msg)
 
     def _check_source_different_from_destination(self):
         if self.source == self.destination:
             raise ValueError('source must be different from destination')
 
     def _check_if_data_name_missing(self):
         c1 = self.data_name is None
-        c2 = self.source in MIDDLE_LOCATIONS
-        c3 = self.destination in MIDDLE_LOCATIONS
+        c2 = self.source in constants.MIDDLE_LOCATIONS
+        c3 = self.destination in constants.MIDDLE_LOCATIONS
         if c1 and (c2 or c3):
             msg = ("data_name must be provided if source or destination is "
                    "one of 'dataset' or 'bucket' or 'local'")
             raise ValueError(msg)
 
     def _check_if_query_missing(self):
         if self.source == 'query' and self._query is None:
@@ -150,28 +147,28 @@
             raise ValueError(msg)
         if timestamp_cols is None:
             timestamp_cols = []
         if date_cols is None:
             date_cols = []
         bq_schema = []
         for col in dataframe.columns:
-            dtype_description = infer_dtype(dataframe[col])
+            dtype_description = pandas.api.types.infer_dtype(dataframe[col])
             if col in date_cols:
                 bq_schema.append(bigquery.SchemaField(name=col,
                                                       field_type='DATE'))
             elif col in timestamp_cols:
                 bq_schema.append(bigquery.SchemaField(name=col,
                                                       field_type='TIMESTAMP'))
             elif dtype_description == 'boolean':
                 bq_schema.append(bigquery.SchemaField(name=col,
                                                       field_type='BOOLEAN'))
             elif dtype_description == 'integer':
                 bq_schema.append(bigquery.SchemaField(name=col,
                                                       field_type='INTEGER'))
-            elif dtype_description == 'floating':
+            elif dtype_description in ('floating', 'mixed-integer-float'):
                 bq_schema.append(bigquery.SchemaField(name=col,
                                                       field_type='FLOAT'))
             else:
                 bq_schema.append(bigquery.SchemaField(name=col,
                                                       field_type='STRING'))
         return bq_schema
 
@@ -179,24 +176,26 @@
         self._bq_schema = self.bq_schema_inferred_from_dataframe(
             dataframe=self._dataframe,
             timestamp_cols=self._timestamp_cols,
             date_cols=self._date_cols)
 
     @property
     def _names_atomic_functions_to_call(self):
-        index_source = LOCATIONS.index(self.source)
-        index_destination = LOCATIONS.index(self.destination)
-        rindex_source = REVERSED_LOCATIONS.index(self.source)
-        rindex_destination = REVERSED_LOCATIONS.index(self.destination)
+        index_source = constants.LOCATIONS.index(self.source)
+        index_destination = constants.LOCATIONS.index(self.destination)
+        rindex_source = constants.REVERSED_LOCATIONS.index(self.source)
+        rindex_destination = constants.REVERSED_LOCATIONS.index(
+            self.destination)
         if index_source < index_destination:
             return utils.build_atomic_function_names(
-                LOCATIONS[index_source: index_destination + 1])
+                constants.LOCATIONS[index_source: index_destination + 1])
         else:
             return utils.build_atomic_function_names(
-                REVERSED_LOCATIONS[rindex_source: rindex_destination + 1])
+                constants.REVERSED_LOCATIONS
+                [rindex_source: rindex_destination + 1])
 
     def _query_to_dataset_config(self):
         return Namespace(
             query=self._query,
             write_disposition=self._write_disposition)
 
     def _local_to_dataframe_config(self):
@@ -221,10 +220,10 @@
                 res[n] = getattr(self, atomic_config_name)()
             else:
                 res[n] = Namespace()
             res[n].data_name = self.data_name
             source, destination = n.split('_to_')
             res[n].source = source
             res[n].destination = destination
-            if res[n].source in MIDDLE_LOCATIONS:
+            if res[n].source in constants.MIDDLE_LOCATIONS:
                 res[n].clear_source = (i != 0)
         return res
```

## google_pandas_load/loader.py

```diff
@@ -1,33 +1,31 @@
 import os
 import logging
 import pandas
-from typing import List, Dict, Any, Optional
+from typing import Literal, List, Dict, Any, Optional
 from datetime import datetime
 from copy import deepcopy
 from google.cloud import bigquery, storage
-from google_pandas_load.load_config import LoadConfig
-from google_pandas_load import utils
-from google_pandas_load.constants import \
-    MIDDLE_LOCATIONS, \
-    DESTINATIONS_TO_ALWAYS_CLEAR, \
-    ATOMIC_FUNCTION_NAMES, \
-    BQ_CLIENT_ATOMIC_FUNCTION_NAMES
-
+from google_pandas_load import constants, load_config, utils
 logger = logging.getLogger(name=__name__)
 
 
 class Loader:
     """Wrapper for transferring data between A and B where A and B are
     distinct and chosen between a BigQuery dataset, a Storage bucket directory,
     a local directory and the RAM (with type pandas.DataFrame).
 
     The Loader bundles all the parameters that do not change often when
     executing load jobs during a workflow.
 
+    Note:
+        If the optional argument bucket_dir_path is not given, data will be
+        stored at the root of the bucket. It is a good practice to specify this
+        argument so that data is stored in a defined bucket directory.
+
     Args:
         bq_client (google.cloud.bigquery.client.Client, optional): Client to
             manage connections to the BigQuery API.
         dataset_id (str, optional): The dataset id.
         gs_client (google.cloud.storage.client.Client, optional): Client for
             interacting with the Storage API.
         bucket_name (str, optional): The bucket name.
@@ -39,27 +37,25 @@
             when data is uploaded. See
             `here <https://googleapis.dev/python/storage/latest/blobs.html>`_
             for more information. Defaults to 2**28.
         timeout (int, optional): The amount of time, in seconds, to wait
             for the server response when uploading a Storage blob.
             Defaults to 60.
     """
-
     def __init__(
             self,
             bq_client: Optional[bigquery.Client] = None,
             dataset_id: Optional[str] = None,
             gs_client: Optional[storage.Client] = None,
             bucket_name: Optional[str] = None,
             bucket_dir_path: Optional[str] = None,
             local_dir_path: Optional[str] = None,
             separator: Optional[str] = '|',
             chunk_size: Optional[int] = 2**28,
             timeout: Optional[int] = 60):
-
         self._bq_client = bq_client
         self._dataset_id = dataset_id
         self._gs_client = gs_client
         self._bucket_name = bucket_name
         self._bucket_dir_path = bucket_dir_path
         self._local_dir_path = local_dir_path
         self._separator = separator
@@ -310,15 +306,14 @@
     def _local_file_to_dataframe(
             self, local_file_path, dtype, parse_dates):
         return pandas.read_csv(
             filepath_or_buffer=local_file_path,
             sep=self._separator,
             dtype=dtype,
             parse_dates=parse_dates,
-            infer_datetime_format=True,
             skip_blank_lines=False)
 
     def _dataframe_to_local_file(self, dataframe, local_file_path):
         dataframe.to_csv(
             path_or_buf=local_file_path,
             sep=self._separator,
             index=False,
@@ -429,46 +424,48 @@
         source = configs[0].source
         destination = configs[0].destination
         assert all([c.source == source and c.destination == destination
                     for c in configs])
         atomic_function_name = f'{source}_to_{destination}'
         self._log(f'Starting {source} to {destination}...')
         start_timestamp = datetime.now()
-        if source in MIDDLE_LOCATIONS:
+        if source in constants.MIDDLE_LOCATIONS:
             for c in configs:
                 self._check_if_data_in_source(c)
-        if destination in DESTINATIONS_TO_ALWAYS_CLEAR:
+        if destination in constants.DESTINATIONS_TO_ALWAYS_CLEAR:
             for c in configs:
                 self._clear_destination(c)
         try:
-            if atomic_function_name in BQ_CLIENT_ATOMIC_FUNCTION_NAMES:
+            if atomic_function_name in \
+                    constants.BQ_CLIENT_ATOMIC_FUNCTION_NAMES:
                 res = self._execute_bq_client_loads(configs)
             else:
                 res = self._execute_local_loads(configs)
         finally:
-            if source in MIDDLE_LOCATIONS:
+            if source in constants.MIDDLE_LOCATIONS:
                 for c in configs:
                     if c.clear_source:
                         self._clear_source(c)
         end_timestamp = datetime.now()
-        duration = (end_timestamp - start_timestamp).seconds
+        duration = round((end_timestamp - start_timestamp).total_seconds())
         if atomic_function_name != 'query_to_dataset':
             msg = f'Ended {source} to {destination} [{duration}s]'
             self._log(msg)
         else:
             jobs = res
-            total_bytes_billed_list = [j.total_bytes_billed for j in jobs]
-            costs = [round(tbb / 10 ** 12 * 5, 5)
-                     for tbb in total_bytes_billed_list]
-            cost = sum(costs)
-            msg = f'Ended query to dataset [{duration}s, {cost}$]'
+            total_bytes_processed_list = [
+                j.total_bytes_processed for j in jobs]
+            gb_processed_list = [
+                round(tbb / 10 ** 9, 2) for tbb in total_bytes_processed_list]
+            gb_processed = sum(gb_processed_list)
+            msg = f'Ended query to dataset [{duration}s, {gb_processed}GB]'
             self._log(msg)
         return res
 
-    def multi_load(self, configs: List[LoadConfig]):
+    def multi_load(self, configs: List[load_config.LoadConfig]):
         """Execute several load jobs specified by the configurations.
 
         The BigQuery Client executes simultaneously the query_to_dataset parts
         (resp. the dataset_to_bucket and bucket_to_dataset parts) from the
         configurations.
 
         Args:
@@ -493,15 +490,15 @@
         names_atomic_functions_to_call = utils.union_keys(sliced_configs)
 
         self._check_if_bq_client_missing(names_atomic_functions_to_call)
         self._check_if_gs_client_missing(names_atomic_functions_to_call)
         self._check_if_local_dir_path_missing(names_atomic_functions_to_call)
 
         res = dict()
-        for n in ATOMIC_FUNCTION_NAMES:
+        for n in constants.ATOMIC_FUNCTION_NAMES:
             indexed_atomic_configs = [
                 (i, s[n]) for i, s in enumerate(sliced_configs) if n in s]
             if len(indexed_atomic_configs) == 0:
                 continue
             atomic_configs = [iac[1] for iac in indexed_atomic_configs]
             n_res = self._execute_same_type_loads(atomic_configs)
             if n == 'local_to_dataframe':
@@ -509,16 +506,17 @@
                 for i in indexes:
                     res[i] = n_res.pop(0)
         res = [res.get(i) for i in range(nb_configs)]
         return res
 
     def load(
             self,
-            source: str,
-            destination: str,
+            source: Literal[
+                'query', 'dataset', 'bucket', 'local', 'dataframe'],
+            destination: Literal['dataset', 'bucket', 'local', 'dataframe'],
 
             data_name: Optional[str] = None,
             query: Optional[str] = None,
             dataframe: Optional[pandas.DataFrame] = None,
 
             write_disposition: Optional[str] =
             bigquery.WriteDisposition.WRITE_TRUNCATE,
@@ -633,16 +631,15 @@
         Returns:
             pandas.DataFrame or NoneType: The result of the load job:
 
             - When destination = 'dataframe', it returns a pandas dataframe
               populated with the data specified by the arguments.
             - In all other cases, it returns None.
         """
-
-        config = LoadConfig(
+        config = load_config.LoadConfig(
             source=source,
             destination=destination,
 
             data_name=data_name,
             query=query,
             dataframe=dataframe,
```

## google_pandas_load/loader_quick_setup.py

```diff
@@ -31,14 +31,19 @@
             project=project_id,
             credentials=credentials)
         dataset_id = project_id + '.' + dataset_name
         gs_client = google.cloud.storage.Client(
             project=project_id,
             credentials=credentials)
 
+    Note:
+        If the optional argument bucket_dir_path is not given, data will be
+        stored at the root of the bucket. It is a good practice to specify this
+        argument so that data is stored in a defined bucket directory.
+
     Args:
         project_id (str, optional): The project id.
         dataset_name (str, optional): The dataset name.
         bucket_name (str, optional): The bucket name.
         bucket_dir_path (str, optional): See base class.
         credentials (google.auth.credentials.Credentials): Credentials used to
             build the bq_client and the gs_client. If not passed, falls back to
@@ -96,12 +101,12 @@
         c2 = dataset_name is None
         c3 = bucket_name is None
         if not c1 and c2 and c3:
             msg = ('At least one of dataset_name or bucket_name '
                    'must be provided if project_id is provided')
             raise ValueError(msg)
         if not c2 and c1:
-            msg = 'project_id must provided if dataset_name is provided'
+            msg = 'project_id must be provided if dataset_name is provided'
             raise ValueError(msg)
         if not c3 and c1:
-            msg = 'project_id must provided if bucket_name is provided'
+            msg = 'project_id must be provided if bucket_name is provided'
             raise ValueError(msg)
```

## google_pandas_load/utils.py

```diff
@@ -1,17 +1,17 @@
 import uuid
+import google.cloud.exceptions
 from datetime import datetime
-from google.cloud.exceptions import NotFound
 
 
 def table_exists(bq_client, table_id):
     try:
         bq_client.get_table(table_id)
         return True
-    except NotFound:
+    except google.cloud.exceptions.NotFound:
         return False
 
 
 def wait_for_jobs(jobs):
     for job in jobs:
         job.result()
```

## Comparing `google_pandas_load-5.0.1.dist-info/LICENSE` & `google_pandas_load-6.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `google_pandas_load-5.0.1.dist-info/METADATA` & `google_pandas_load-6.0.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: google-pandas-load
-Version: 5.0.1
+Version: 6.0.0
 Summary: Wrapper for transferring data from A to B, where A and B are distinct and chosen between BigQuery, Storage, a local directory and pandas.
 Home-page: UNKNOWN
 Author: Augustin Barillec
 Author-email: augustin.barillec@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://google-pandas-load.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/augustin-barillec/google-pandas-load
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
+License-File: LICENSE
 Requires-Dist: google-cloud-bigquery (==3.*)
 Requires-Dist: google-cloud-storage (==2.*)
-Requires-Dist: pandas (==1.*)
+Requires-Dist: pandas (==2.*)
 
 google-pandas-load
 ==================
 
 .. image:: https://img.shields.io/pypi/v/google-pandas-load
     :target: https://pypi.org/project/google-pandas-load/
 
 .. image:: https://img.shields.io/pypi/l/google-pandas-load.svg
     :target: https://pypi.org/project/google-pandas-load/
 
 .. image:: https://img.shields.io/pypi/pyversions/google-pandas-load.svg
     :target: https://pypi.org/project/google-pandas-load/
 
-.. image:: https://codecov.io/gh/augustin-barillec/google-pandas-load/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/augustin-barillec/google-pandas-load/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/augustin-barillec/google-pandas-load
 
 .. image:: https://pepy.tech/badge/google-pandas-load
     :target: https://pepy.tech/project/google-pandas-load
 
 Wrapper for transferring data from A to B, where A and B are distinct
 and chosen between BigQuery, Storage, a local directory and pandas.
```

