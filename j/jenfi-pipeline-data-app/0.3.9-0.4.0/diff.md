# Comparing `tmp/jenfi_pipeline_data_app-0.3.9.tar.gz` & `tmp/jenfi_pipeline_data_app-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenfi_pipeline_data_app-0.3.9.tar", max compression
+gzip compressed data, was "jenfi_pipeline_data_app-0.4.0.tar", max compression
```

## Comparing `jenfi_pipeline_data_app-0.3.9.tar` & `jenfi_pipeline_data_app-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      506 2022-09-28 01:48:11.362394 jenfi_pipeline_data_app-0.3.9/README.md
--rw-r--r--   0        0        0     1313 2022-09-28 02:32:06.697627 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/API.md
--rw-r--r--   0        0        0      699 2022-11-01 07:55:16.205711 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/__init__.py
--rw-r--r--   0        0        0      352 2022-09-27 12:01:11.538904 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/_pdoc.py
--rw-r--r--   0        0        0     2159 2022-09-28 05:35:29.110840 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app.py
--rw-r--r--   0        0        0      290 2022-11-01 06:52:43.710759 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_constants.py
--rw-r--r--   0        0        0     1171 2022-11-01 04:25:15.307222 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_db_handler.py
--rw-r--r--   0        0        0      644 2022-09-28 03:11:48.896815 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_exit_program.py
--rw-r--r--   0        0        0     1071 2022-09-26 02:09:40.339139 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_models_s3.py
--rw-r--r--   0        0        0     1229 2022-09-26 02:09:40.339356 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_parameters.py
--rw-r--r--   0        0        0     1152 2022-09-28 01:29:43.344757 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_query.py
--rw-r--r--   0        0        0     2937 2022-09-28 07:27:48.368864 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_result.py
--rw-r--r--   0        0        0      543 2022-09-23 02:13:28.814271 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
--rw-r--r--   0        0        0     1414 2022-11-01 04:23:14.674255 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/config/db.py
--rw-r--r--   0        0        0      403 2022-09-26 02:09:40.340068 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/config/s3.py
--rw-r--r--   0        0        0       30 2022-09-26 02:09:40.340419 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/__init__.py
--rw-r--r--   0        0        0     3846 2022-09-26 02:09:40.340623 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/cacher.py
--rw-r--r--   0        0        0     1610 2022-09-26 04:22:14.607584 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/db_cache.py
--rw-r--r--   0        0        0     2199 2022-11-01 07:44:20.436236 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_models.py
--rw-r--r--   0        0        0      862 2022-11-01 07:55:16.050538 jenfi_pipeline_data_app-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     1621 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.3.9/setup.py
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      510 2023-01-20 08:43:07.713833 jenfi_pipeline_data_app-0.4.0/README.md
+-rw-r--r--   0        0        0     1313 2022-09-28 02:32:06.697627 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/API.md
+-rw-r--r--   0        0        0     1526 2023-05-09 02:21:49.104886 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/__init__.py
+-rw-r--r--   0        0        0      354 2023-05-09 01:55:02.513098 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/_pdoc.py
+-rw-r--r--   0        0        0     2222 2023-05-09 01:55:30.035561 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app.py
+-rw-r--r--   0        0        0      345 2023-05-09 01:55:01.490867 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_constants.py
+-rw-r--r--   0        0        0     1107 2023-05-09 01:56:23.563197 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_db_handler.py
+-rw-r--r--   0        0        0     1066 2022-11-02 00:33:49.627056 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_exit_program.py
+-rw-r--r--   0        0        0     1074 2023-05-09 01:55:02.723840 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_models_s3.py
+-rw-r--r--   0        0        0     1323 2023-05-09 02:13:40.620671 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_parameters.py
+-rw-r--r--   0        0        0     1282 2023-05-09 02:21:49.112873 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_query.py
+-rw-r--r--   0        0        0     2896 2023-05-09 01:57:09.624035 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_result.py
+-rw-r--r--   0        0        0      569 2023-05-09 01:58:34.501284 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
+-rw-r--r--   0        0        0     1419 2023-05-09 01:58:06.146777 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/config/db.py
+-rw-r--r--   0        0        0      395 2023-05-09 01:55:01.562329 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/config/s3.py
+-rw-r--r--   0        0        0       43 2023-05-09 01:58:34.496937 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/__init__.py
+-rw-r--r--   0        0        0     3838 2023-05-09 01:55:02.728505 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/cacher.py
+-rw-r--r--   0        0        0     1771 2023-05-09 02:14:47.825830 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/db_cache.py
+-rw-r--r--   0        0        0     2050 2023-05-09 01:58:45.726647 jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_models.py
+-rw-r--r--   0        0        0      941 2023-05-09 02:16:15.078822 jenfi_pipeline_data_app-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.4.0/PKG-INFO
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/API.md` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/API.md`

 * *Files identical despite different names*

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import sys
 import os
 import platform
+import sys
 import tempfile
 from pathlib import Path
 
-import sklearn
 
-class Application(object):
+class Application:
     """
     .. include:: API.md
 
     """
 
     from .app_funcs._constants import (
-        ROOT_DIR,
-        RESULT_FILENAME,
         PYTHON_ENV,
-        STATUS_NOT_APPLICABLE,
+        RESULT_FILENAME,
+        ROOT_DIR,
         STATUS_INSUFFICIENT_DATA,
-        STATUS_SUCCESS,
         STATUS_NO_RESULT,
+        STATUS_NOT_APPLICABLE,
+        STATUS_NOTEBOOK_NOT_FOUND_S3,
+        STATUS_SUCCESS,
     )
-
-    from .app_funcs._db_handler import _init_db, _close_db, _db_config
-    from .app_funcs._query import df_query, query_one, query_all, _db_cache
-    from .app_funcs._parameters import load_test_parameters, get_parameter, _run_data
-    from .app_funcs._result import (
-        write_result_to_db,
-        write_result,
-        load_result,
-        _add_run_metadata,
-        _remove_result_file,
-        _write_result,
+    from .app_funcs._db_handler import _close_db, _db_config, _init_db
+    from .app_funcs._exit_program import (
+        exit_insufficient_data,
+        exit_not_applicable,
+        notebook_not_found_s3,
     )
     from .app_funcs._models_s3 import (
-        push_model_to_s3,
-        load_model_from_s3,
         _init_config_s3,
+        load_model_from_s3,
+        push_model_to_s3,
     )
-    from .app_funcs._exit_program import (
-        exit_not_applicable,
-        exit_insufficient_data,
+    from .app_funcs._parameters import _run_data, get_parameter, load_test_parameters
+    from .app_funcs._query import _db_cache, df_query, query_all, query_one
+    from .app_funcs._result import (
+        _add_run_metadata,
+        _remove_results_tmpfile,
+        _results_to_tmpfile,
+        load_result,
+        write_result,
+        write_result_to_db,
     )
 
     def boot(self):
         """Sets up configs, db connections. It is run as part of the module import."""
         self._init_db()
         self._init_config_s3()
-        self._remove_result_file()  # Any lingering files
+        self._remove_results_tmpfile()  # Any lingering files
 
     def cleanup(self):
         """Closes connections and cleans up any lingering items."""
         self._close_db()
-        self._remove_result_file()
+        self._remove_results_tmpfile()
 
     def tmp_dir(self) -> Path:
         if self.PYTHON_ENV == "production":
             tmp_path = "/tmp"
         elif self.PYTHON_ENV == "staging":
             tmp_path = "/tmp"
         else:
@@ -72,11 +72,11 @@
         return Path(os.path.join(tmp_path, rel_filepath))
 
     def __repr__(self):
         return self.__dict__
 
     if "pytest" in sys.modules:
         from .app_funcs._test_funcs import (
-            _test_direct_module,
             _test_access_global_var,
+            _test_direct_module,
             _test_set_global_var,
         )
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_db_handler.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_db_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from sqlalchemy import create_engine, MetaData, or_
-from sqlalchemy.orm import sessionmaker, scoped_session
-from sqlalchemy.ext.automap import automap_base
-
 from dotenv import load_dotenv
+from sqlalchemy import create_engine
+from sqlalchemy.orm import scoped_session, sessionmaker
 
 
 def _init_db(self):
     db_config = self._db_config()
 
     self.db_engine = create_engine(db_config.SQL_ALCHEMY_CONN, echo=False)
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_exit_program.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_exit_program.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,23 +5,37 @@
 def exit_not_applicable(self, message: str) -> None:
     """Exits the program early and puts status `not_applicable`"""
 
     result_with_metadata = self._add_run_metadata(
         self.STATUS_NOT_APPLICABLE, message=message
     )
 
-    self._write_result(result_with_metadata)
+    self._results_to_tmpfile(result_with_metadata)
 
     sys.exit(0)
 
 
 def exit_insufficient_data(self, message: str) -> None:
     """Exits the program early and puts status `insufficient_data`"""
     # Write output
 
     result_with_metadata = self._add_run_metadata(
         self.STATUS_INSUFFICIENT_DATA, message=message
     )
 
-    self._write_result(result_with_metadata)
+    self._results_to_tmpfile(result_with_metadata)
 
     sys.exit(0)
+
+
+def notebook_not_found_s3(self) -> None:
+    """Notebook could not be found/downloaded from S3. Not designed to be run from inside a notebook."""
+
+    message = "Notebook could not be found/downloaded from S3. Check keys, file."
+
+    result_with_metadata = self._add_run_metadata(
+        self.STATUS_NOTEBOOK_NOT_FOUND_S3, message=message
+    )
+
+    self._results_to_tmpfile(result_with_metadata)
+
+    pass
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_models_s3.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_models_s3.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-import boto3
 import pickle
 
+import boto3
+
+
 def _init_config_s3(self):
     if self.PYTHON_ENV == "production":
         from ..config.s3 import ProductionConfig
 
         self.s3_config = ProductionConfig()
     elif self.PYTHON_ENV == "staging":
         from ..config.s3 import StagingConfig
@@ -13,27 +15,28 @@
     else:
         from ..config.s3 import DevelopmentConfig
 
         self.s3_config = DevelopmentConfig()
 
     pass
 
+
 def push_model_to_s3(self, model, model_key):
     pickle_byte_obj = pickle.dumps(model)
 
     _s3_model_obj(self, model_key).put(Body=pickle_byte_obj)
 
     pass
 
 
 def load_model_from_s3(self, model_key):
     # Model => S3 => Download Model
     obj = _s3_model_obj(self, model_key)
 
-    return pickle.loads(obj.get()['Body'].read())
+    return pickle.loads(obj.get()["Body"].read())
 
 
 def _s3_model_obj(self, model_key):
     bucket_name = self.s3_config.S3_TRAINED_MODELS_BUCKET
     fileprefix = self.get_parameter("logical_step_name")  # Supposed to be step_name
     filepath = f"{fileprefix}/{model_key}.pickle"
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_parameters.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 
+
 # This is built specifically to handle loading test variables for papermill.
 # EXTREMELY brittle.
 def load_test_parameters(self, params_dict):
     mod = _get_notebook_module()
 
     for var_name, var_val in params_dict.items():
         try:
@@ -11,15 +12,15 @@
             eval(f"mod.{var_name}")
         except (NameError, AttributeError):
             # Papermill nor anyone else defined this variable, let's set it ourselves!
             setattr(mod, var_name, var_val)
 
 
 def get_parameter(self, var_name, default=None):
-    mod = _get_notebook_module()
+    mod = _get_notebook_module()  # noqa F841
 
     if default:
         try:
             return eval(f"mod.{var_name}")
         except (NameError, AttributeError):
             return default
     else:
@@ -30,12 +31,14 @@
     mod = sys.modules["__main__"]
 
     if mod:
         return mod
     else:
         raise ModuleNotFoundError("__main__ not found, is this called from a Notebook?")
 
+
 def _run_data(self):
     logical_step_name = self.get_parameter("logical_step_name")
     state_machine_run_id = self.get_parameter("state_machine_run_id")
+    disable_cache = self.get_parameter("disable_cache", False)
 
-    return logical_step_name, state_machine_run_id
+    return logical_step_name, state_machine_run_id, disable_cache
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_query.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,52 @@
-from ..db_cache import DbCache
 from pandas import DataFrame
 
+from ..db_cache import DbCache
+
+
 # Primary use point for Credit
 # Should be able to help take snapshot of data and return the cache as necessary.
-def df_query(self, query_str: str, rebuild_cache: bool=False) -> DataFrame:
+def df_query(self, query_str: str, rebuild_cache: bool = False) -> DataFrame:
     """
     Provide a valid psql query_str and returns a Pandas DataFrame. Has caching.
     """
     db_cache = self._db_cache()
 
     return db_cache.df_query(query_str, rebuild_cache)
 
 
-def query_one(self, query_str: str, rebuild_cache: bool=False):
+# Alias for df_query
+query_df = df_query
+
+
+def query_one(self, query_str: str, rebuild_cache: bool = False):
     """
     Direct sqlalchmey fetchone(). Returns None or a dict. Has caching.
     """
     db_cache = self._db_cache()
 
     return db_cache.query_one(query_str, rebuild_cache)
 
 
-def query_all(self, query_str: str, rebuild_cache: bool=False):
+def query_all(self, query_str: str, rebuild_cache: bool = False):
     """
     Direct sqlalchmey fetchall(). Returns an Array. Has caching.
     """
 
     db_cache = self._db_cache()
 
     return db_cache.query_all(query_str, rebuild_cache)
 
 
 def _db_cache(self) -> None:
-    (step_name, run_id) = self._run_data()
+    (step_name, run_id, disable_cache) = self._run_data()
     bucket_name = self.s3_config.S3_DB_QUERY_CACHE_BUCKET
 
     return DbCache(
-        self.db, self.db_engine, step_name, run_id, self.tmp_dir(), bucket_name
+        self.db,
+        self.db_engine,
+        step_name,
+        run_id,
+        self.tmp_dir(),
+        bucket_name,
+        disable_cache,
     )
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_result.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,70 @@
-import os
 import json
-import numpy as np
-import pandas as pd
-
-from decimal import Decimal
+import os
 from datetime import date, datetime
+from decimal import Decimal
 from pathlib import Path
 
+import numpy as np
+
 
 class NpEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         if isinstance(obj, np.floating):
             return float(obj)
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         if isinstance(obj, Decimal):
             return float(obj)
         if isinstance(obj, (datetime, date)):
             return obj.isoformat()
 
-        return super(NpEncoder, self).default(obj)
+        return super().default(obj)
 
     def _preprocess_nan(self, obj):
         if isinstance(obj, float) and np.isnan(obj):
             return None
         elif isinstance(obj, dict):
             return {
                 self._preprocess_nan(k): self._preprocess_nan(v) for k, v in obj.items()
             }
         elif isinstance(obj, list):
             return [self._preprocess_nan(i) for i in obj]
         return obj
 
     def iterencode(self, obj):
-        return super(NpEncoder, self).iterencode(self._preprocess_nan(obj))
+        return super().iterencode(self._preprocess_nan(obj))
 
 
-def write_result_to_db(self, logical_step_name, state_machine_run_id):
+def write_result_to_db(self, logical_step_name, state_machine_run_id, results):
     from ..db_models import state_machine_run_model
 
     StateMachineRun = state_machine_run_model(self)
     return StateMachineRun().result_to_db(
-        logical_step_name, state_machine_run_id, self.load_result()
+        logical_step_name, state_machine_run_id, results
     )
 
 
 def write_result(self, result: dict) -> Path:
     """
     Use after whole notebook is finished to return the final result with a status of `success`
     """
 
     result_with_metadata = self._add_run_metadata(self.STATUS_SUCCESS, result)
 
-    return self._write_result(result_with_metadata)
+    return self._results_to_tmpfile(result_with_metadata)
 
 
 def load_result(self):
     result_filepath = self.tmp_filepath(self.RESULT_FILENAME)
 
     if result_filepath.is_file():
-        with open(result_filepath, "r") as result:
+        with open(result_filepath) as result:
             output_data = json.load(result)
 
         return output_data
     else:
         return self._add_run_metadata(
             self.STATUS_NO_RESULT,
             message="There was no result directly returned from this notebook. Is this expected?",
@@ -82,23 +81,23 @@
 
     if message is not None:
         result_with_metadata["run_metadata"]["message"] = message
 
     return result_with_metadata
 
 
-def _write_result(self, result: dict) -> Path:
+def _results_to_tmpfile(self, result: dict) -> Path:
     result_filepath = self.tmp_filepath(self.RESULT_FILENAME)
 
     with open(result_filepath, "w") as f:
         json.dump(result, f, cls=NpEncoder)
 
     return result_filepath
 
 
-def _remove_result_file(self) -> None:
+def _remove_results_tmpfile(self) -> None:
     result_filepath = self.tmp_filepath(self.RESULT_FILENAME)
 
     if result_filepath.is_file():
         os.remove(result_filepath)
 
     pass
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_test_funcs.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/app_funcs/_test_funcs.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 def _test_direct_module(self, mod):
     return eval("mod.var_defined_globally")
 
 
 # Most of these methods below don't work because of how jupyter runs code.
 def _test_access_global_var(self):
     # https://stackoverflow.com/questions/1095543/get-name-of-calling-functions-module-in-python
-    mod = inspect.getmodule(inspect.stack()[1][0])
+    mod = inspect.getmodule(inspect.stack()[1][0])  # noqa F841
 
     return eval("mod.var_defined_globally")
 
 
 def _test_set_global_var(self):
-    mod = inspect.getmodule(inspect.stack()[1][0])
+    mod = inspect.getmodule(inspect.stack()[1][0])  # noqa F841
 
     exec("mod.var_defined_globally = 'bar'")
 
     pass
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/config/db.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/config/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 
-class Config(object):
+class Config:
     DEBUG = False
     TESTING = False
 
     @property
     def SQL_ALCHEMY_CONN(self):
-        return f"postgresql+psycopg2://{self.PG_USERNAME}:{self.PG_PASSWORD}@{self.PG_HOST}:{self.DB_PORT}/{self.DB_NAME}"
+        return f"postgresql+psycopg2://{self.PG_USERNAME}:{self.PG_PASSWORD}@{self.PG_HOST}:{self.DB_PORT}/{self.DB_NAME}"  # noqa E501
 
 
 class ProductionConfig(Config):
     DEBUG = False
     PG_USERNAME = os.getenv("PG_USERNAME")
     PG_PASSWORD = os.getenv("PG_PASSWORD")
     PG_HOST = os.getenv("PG_HOST")
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/cacher.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/cacher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import boto3
-import pickle
 import hashlib
 import logging
-import sqlparse
-
-from pathlib import Path
+import pickle
 from functools import lru_cache
+from pathlib import Path
+
+import boto3
+import sqlparse
 
 
-class Cacher(object):
+class Cacher:
     MAX_NORMALIZE_QUERY_LENGTH = 40000
     LOGGER = logging.getLogger(__name__)
 
     def __init__(
         self,
         logical_step_name: str,
         state_machine_run_id: str,
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/db_cache.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_cache/db_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from sqlalchemy.engine import Engine
 from pathlib import Path
+
 import pandas as pd
+from sqlalchemy.engine import Engine
 
 from .cacher import Cacher
 
 
-class DbCache(object):
+class DbCache:
     def __init__(
         self,
         db,
         db_engine: Engine,
         logical_step_name: str,
         state_machine_run_id: str,
         local_cache_dir: Path,
         s3_bucket_name: str,
+        disable_cache: bool,
     ) -> None:
         self.db = db
         self.db_engine = db_engine
+        self.disable_cache = disable_cache
         self.cacher = Cacher(
             logical_step_name, state_machine_run_id, local_cache_dir, s3_bucket_name
         )
 
         pass
 
     def df_query(self, query_str: str, rebuild_cache: bool) -> pd.DataFrame:
@@ -38,15 +41,17 @@
     def query_all(self, query_str: str, rebuild_cache: bool):
         return self._with_cacher(self._query_all, query_str, rebuild_cache)
 
     def _query_all(self, query_str: str):
         return self.db.execute(query_str).fetchall()
 
     def _with_cacher(self, query_func, query_str: str, rebuild_cache: bool):
-        if self.cacher.exists(query_str) and not rebuild_cache:
+        if self.disable_cache and not rebuild_cache:
+            return query_func(query_str)
+        elif self.cacher.exists(query_str) and not rebuild_cache:
             return self.cacher.from_cache(query_str)
         else:
             result = query_func(query_str)
 
             self.cacher.to_cache(query_str, result)
 
             return result
```

### Comparing `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_models.py` & `jenfi_pipeline_data_app-0.4.0/jenfi_pipeline_data_app/db_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-from sqlalchemy import ForeignKey, Table, MetaData, Column, JSON
-from sqlalchemy.ext.mutable import MutableDict
-from sqlalchemy.ext.automap import automap_base
-from sqlalchemy.ext.declarative import declarative_base
-
-from sqlalchemy.orm.attributes import flag_modified
-
 import datetime
 
-from sqlalchemy import Table, Column, Integer, DateTime
+from sqlalchemy import JSON, Column, DateTime, Integer, MetaData, Table
+from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.ext.mutable import MutableDict
+
 
 # This shouldn't be a function, but I can't figure out how to pass a db_engine before the class creation on import.
 # ATM, all classes will have to be loaded via function =\
 #
 # https://stackoverflow.com/questions/4215920/how-to-bind-engine-when-i-want-when-using-declarative-base-in-sqlalchemy
 # The above is the same problem. It recommends using a DeferredRefelection, but that didn't work for me.
 def state_machine_run_model(app):
@@ -20,16 +16,16 @@
 
     class StateMachineRun(Base):
         __table__ = Table(
             "pipeline_state_machine_runs",
             metadata,
             Column("id", Integer, primary_key=True),
             Column("result", MutableDict.as_mutable(JSON)),
-            Column('created_at', DateTime, default=datetime.datetime.now),
-            Column('updated_at', DateTime, default=datetime.datetime.now),
+            Column("created_at", DateTime, default=datetime.datetime.now),
+            Column("updated_at", DateTime, default=datetime.datetime.now),
             autoload=True,
         )
 
         def result_to_db(self, logical_step_name, state_machine_run_id, results):
             sm_run = (
                 app.db.query(StateMachineRun)
                 .populate_existing()
@@ -38,22 +34,23 @@
             )
             sm_run.result[logical_step_name] = results
 
             return app.db.commit()
 
     return StateMachineRun
 
+
 def state_machine_model(app):
     Base = declarative_base()
     metadata = MetaData(bind=app.db_engine)
 
     class StateMachine(Base):
         __table__ = Table(
             "pipeline_state_machines",
             metadata,
             Column("id", Integer, primary_key=True),
-            Column('created_at', DateTime, default=datetime.datetime.now),
-            Column('updated_at', DateTime, default=datetime.datetime.now),
+            Column("created_at", DateTime, default=datetime.datetime.now),
+            Column("updated_at", DateTime, default=datetime.datetime.now),
             autoload=True,
         )
 
     return StateMachine
```

### Comparing `jenfi_pipeline_data_app-0.3.9/pyproject.toml` & `jenfi_pipeline_data_app-0.4.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [tool.poetry]
 name = "jenfi-pipeline-data-app"
-version = "0.3.9"
+version = "0.4.0"
 description = ""
 readme = "README.md"
 authors = ["Justin Louie <224840+nitsujri@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 SQLAlchemy = "^1.4.40"
 numpy = "^1.23.2"
 python-dotenv = "^0.20.0"
 psycopg2 = "^2.9.3"
 pandas = "^1.4.3"
 boto3 = "^1.24.78"
 sqlparse = "^0.4.2"
-sklearn = "^0.0"
 scikit-learn = "^1.1.2"
+sagemaker = "^2.150.0"
+statsmodels = "^0.13.5"
+jupyterlab-git = "^0.41.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 pytest = "^7.1.3"
 pdoc3 = "^0.10.0"
 papermill = "^2.4.0"
 jupyterlab = "^3.4.7"
 
 [tool.poetry.scripts]
 pipeline-data-app = 'pipeline_data_app:main'
 
 [tool.poetry.group.dev.dependencies]
 pytest-env = "^0.8.1"
+pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 env = [
```

### Comparing `jenfi_pipeline_data_app-0.3.9/PKG-INFO` & `jenfi_pipeline_data_app-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: jenfi-pipeline-data-app
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Author: Justin Louie
 Author-email: 224840+nitsujri@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0)
 Requires-Dist: boto3 (>=1.24.78,<2.0.0)
+Requires-Dist: jupyterlab-git (>=0.41.0,<0.42.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: psycopg2 (>=2.9.3,<3.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: sagemaker (>=2.150.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
-Requires-Dist: sklearn (>=0.0,<0.1)
 Requires-Dist: sqlparse (>=0.4.2,<0.5.0)
+Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
 Description-Content-Type: text/markdown
 
 # Jenfi Pipeline Data App
 
 Designed to allow teams to access Jenfi's data sources in a Jupyter Notebook.
 
 ## Docs
 
-[View public API doc](https://jenfi-eng.github.io/pipeline-data) for using in Jupyter notebook.
+[View public API doc](https://jenfi-eng.github.io/pipeline-data-app) for using in Jupyter notebook.
 
 ## Basic Usage
 
 ```python
 from jenfi_pipeline_data_app import PipelineDataApp as Jenfi
 
 Jenfi.ROOT_DIR # => /Your/app/root/dir
```

