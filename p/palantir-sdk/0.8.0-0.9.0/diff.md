# Comparing `tmp/palantir-sdk-0.8.0.tar.gz` & `tmp/palantir-sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palantir-sdk-0.8.0.tar", max compression
+gzip compressed data, was "palantir-sdk-0.9.0.tar", max compression
```

## Comparing `palantir-sdk-0.8.0.tar` & `palantir-sdk-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11358 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/LICENSE
--rw-r--r--   0        0        0      728 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/__init__.py
--rw-r--r--   0        0        0       22 2022-04-25 18:34:36.920199 palantir-sdk-0.8.0/palantir/_version.py
--rw-r--r--   0        0        0      657 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/core/__init__.py
--rw-r--r--   0        0        0     7169 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/core/config.py
--rw-r--r--   0        0        0     2096 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/core/functions.py
--rw-r--r--   0        0        0     1408 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/core/rpc.py
--rw-r--r--   0        0        0     2922 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/core/types.py
--rw-r--r--   0        0        0     1942 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/core/util.py
--rw-r--r--   0        0        0      657 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/datasets/__init__.py
--rw-r--r--   0        0        0    20335 2022-04-25 18:34:36.624195 palantir-sdk-0.8.0/palantir/datasets/client.py
--rw-r--r--   0        0        0    11230 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/core.py
--rw-r--r--   0        0        0     1257 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/errors.py
--rw-r--r--   0        0        0     2842 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/functions.py
--rw-r--r--   0        0        0      625 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/rpc/__init__.py
--rw-r--r--   0        0        0    29412 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/rpc/catalog.py
--rw-r--r--   0        0        0    12754 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/rpc/data_proxy.py
--rw-r--r--   0        0        0     2150 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/rpc/path.py
--rw-r--r--   0        0        0    12229 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/rpc/schema.py
--rw-r--r--   0        0        0    11196 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/rpc/sql.py
--rw-r--r--   0        0        0     3660 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/schema.py
--rw-r--r--   0        0        0    10286 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/datasets/types.py
--rw-r--r--   0        0        0        0 2022-04-25 18:34:36.628195 palantir-sdk-0.8.0/palantir/py.typed
--rw-r--r--   0        0        0      820 2022-04-25 18:34:37.412205 palantir-sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      758 2022-04-25 18:34:38.343374 palantir-sdk-0.8.0/setup.py
--rw-r--r--   0        0        0      605 2022-04-25 18:34:38.343603 palantir-sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/LICENSE
+-rw-r--r--   0        0        0      728 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/__init__.py
+-rw-r--r--   0        0        0       22 2022-08-15 14:48:26.700909 palantir-sdk-0.9.0/palantir/_version.py
+-rw-r--r--   0        0        0      657 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/core/__init__.py
+-rw-r--r--   0        0        0     7169 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/core/config.py
+-rw-r--r--   0        0        0     2096 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/core/functions.py
+-rw-r--r--   0        0        0     1408 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/core/rpc.py
+-rw-r--r--   0        0        0     2922 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/core/types.py
+-rw-r--r--   0        0        0     1942 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/core/util.py
+-rw-r--r--   0        0        0      657 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/__init__.py
+-rw-r--r--   0        0        0    20335 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/client.py
+-rw-r--r--   0        0        0    11235 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/core.py
+-rw-r--r--   0        0        0     1257 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/errors.py
+-rw-r--r--   0        0        0     2842 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/functions.py
+-rw-r--r--   0        0        0      625 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/rpc/__init__.py
+-rw-r--r--   0        0        0    29582 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/rpc/catalog.py
+-rw-r--r--   0        0        0    12860 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/rpc/data_proxy.py
+-rw-r--r--   0        0        0     2208 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/rpc/path.py
+-rw-r--r--   0        0        0    12637 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/rpc/schema.py
+-rw-r--r--   0        0        0    11286 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/rpc/sql.py
+-rw-r--r--   0        0        0      848 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/rpc/util.py
+-rw-r--r--   0        0        0     3660 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/schema.py
+-rw-r--r--   0        0        0    10286 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/datasets/types.py
+-rw-r--r--   0        0        0        0 2022-08-15 14:48:26.452908 palantir-sdk-0.9.0/palantir/py.typed
+-rw-r--r--   0        0        0      820 2022-08-15 14:48:27.224909 palantir-sdk-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      758 2022-08-15 14:48:28.252101 palantir-sdk-0.9.0/setup.py
+-rw-r--r--   0        0        0      605 2022-08-15 14:48:28.252449 palantir-sdk-0.9.0/PKG-INFO
```

### Comparing `palantir-sdk-0.8.0/LICENSE` & `palantir-sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/__init__.py` & `palantir-sdk-0.9.0/palantir/__init__.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/core/__init__.py` & `palantir-sdk-0.9.0/palantir/core/__init__.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/core/config.py` & `palantir-sdk-0.9.0/palantir/core/config.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/core/functions.py` & `palantir-sdk-0.9.0/palantir/core/functions.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/core/rpc.py` & `palantir-sdk-0.9.0/palantir/core/rpc.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/core/types.py` & `palantir-sdk-0.9.0/palantir/core/types.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/core/util.py` & `palantir-sdk-0.9.0/palantir/core/util.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/datasets/__init__.py` & `palantir-sdk-0.9.0/palantir/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/datasets/client.py` & `palantir-sdk-0.9.0/palantir/datasets/client.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/datasets/core.py` & `palantir-sdk-0.9.0/palantir/datasets/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,21 +127,20 @@
 
         Returns:
             A :class:`Transaction` object that can be used to manage the lifecyle of the Transaction.
 
         Examples:
             >>> from palantir.datasets import dataset
             >>> ds = dataset("/path/to/dataset")
-            ... with ds.start_transaction():
-            ...     ds.file("file.txt").write(b"file content")
-
+            ... with ds.start_transaction() as txn:
+            ...     txn.write("file.txt", b"file content")
 
             >>> ds = dataset("/path/to/dataset")
-            ... with ds.start_transaction('SNAPSHOT'):
-            ...     ds.file("file.txt").write(b"file content")
+            ... with ds.start_transaction('SNAPSHOT') as txn:
+            ...     txn.write("file.txt", b"file content")
         """
         _txn_type = (
             txn_type
             if isinstance(txn_type, TransactionType)
             else (
                 TransactionType(txn_type)
                 if txn_type is not None
```

### Comparing `palantir-sdk-0.8.0/palantir/datasets/errors.py` & `palantir-sdk-0.9.0/palantir/datasets/errors.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/datasets/functions.py` & `palantir-sdk-0.9.0/palantir/datasets/functions.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/datasets/rpc/__init__.py` & `palantir-sdk-0.9.0/palantir/datasets/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/datasets/rpc/catalog.py` & `palantir-sdk-0.9.0/palantir/datasets/rpc/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ConjureEncoder,
     ConjureBeanType,
     ConjureFieldDefinition,
     DictType,
     ConjureEnumType,
     OptionalTypeWrapper,
 )
+from .util import format_path_with_params
 
 
 class CatalogService(Service):
     def create_dataset(
         self, auth_header: str, request: "CreateDatasetRequest"
     ) -> "Dataset":
         _headers: Dict[str, Any] = {
@@ -39,15 +40,15 @@
         _params: Dict[str, Any] = {}
 
         _path_params: Dict[str, Any] = {}
 
         _json: Any = ConjureEncoder().default(request)
 
         _path = "/catalog/datasets"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), Dataset)
@@ -71,15 +72,15 @@
             "datasetRid": dataset_rid,
             "branchId": branch_id,
         }
 
         _json: Any = ConjureEncoder().default(request)
 
         _path = "/catalog/datasets/{datasetRid}/branchesUnrestricted2/{branchId}"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), Branch)
@@ -106,15 +107,15 @@
             "datasetRid": dataset_rid,
             "endRef": end_ref,
         }
 
         _json = None
 
         _path = "/catalog/datasets/{datasetRid}/views2/{endRef}/range"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "GET", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return (
@@ -157,15 +158,15 @@
             "datasetRid": dataset_rid,
             "endRef": end_ref,
         }
 
         _json = None
 
         _path = "/catalog/datasets/{datasetRid}/views2/{endRef}/files"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "GET", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), FileResourcesPage)
@@ -185,15 +186,15 @@
         _path_params: Dict[str, Any] = {
             "datasetRid": dataset_rid,
         }
 
         _json: Any = ConjureEncoder().default(request)
 
         _path = "/catalog/datasets/{datasetRid}/transactions"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), Transaction)
@@ -217,15 +218,15 @@
             "datasetRid": dataset_rid,
             "transactionRid": transaction_rid,
         }
 
         _json: Any = ConjureEncoder().default(txn_type)
 
         _path = "/catalog/datasets/{datasetRid}/transactions/{transactionRid}"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), Transaction)
@@ -249,15 +250,15 @@
             "datasetRid": dataset_rid,
             "transactionRid": transaction_rid,
         }
 
         _json: Any = ConjureEncoder().default(request)
 
         _path = "/catalog/datasets/{datasetRid}/transactions/{transactionRid}/commit"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
     def abort_transaction(
         self,
@@ -278,15 +279,15 @@
             "datasetRid": dataset_rid,
             "transactionRid": transaction_rid,
         }
 
         _json: Any = ConjureEncoder().default(request)
 
         _path = "/catalog/datasets/{datasetRid}/transactions/{transactionRid}/abortWithMetadata"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
 
 class StartTransactionRequest(ConjureBeanType):
```

### Comparing `palantir-sdk-0.8.0/palantir/datasets/rpc/data_proxy.py` & `palantir-sdk-0.9.0/palantir/datasets/rpc/data_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     ConjureBeanType,
     ConjureFieldDefinition,
     ConjureUnionType,
     ConjureDecoder,
     ConjureEncoder,
 )
 from requests import Response
+from .util import format_path_with_params
 
 
 class DataProxyService(Service):
     def get_file_in_view(
         self,
         auth_header: str,
         dataset_rid: str,
@@ -51,15 +52,15 @@
             "endRef": end_ref,
             "logicalPath": logical_path,
         }
 
         _json = None
 
         _path = "/dataproxy/datasets/{datasetRid}/views/{endRef}/{logicalPath}"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response: Response = self._request(
             "GET",
             self._uri + _path,
             params=_params,
             headers=_headers,
             stream=True,
@@ -91,15 +92,15 @@
         }
 
         _path_params: Dict[str, Any] = {
             "datasetRid": dataset_rid,
             "transactionRid": transaction_rid,
         }
         _path = "/dataproxy/datasets/{datasetRid}/transactions/{transactionRid}/putFile"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, data=file_data
         )
 
 
 class DataProxyConcatenationService(Service):
@@ -127,15 +128,15 @@
             "datasetRid": dataset_rid,
             "transactionRid": transaction_rid,
         }
 
         _json: Any = ConjureEncoder().default(request)
 
         _path = "/concatenation-tasks/datasets/{datasetRid}/transactions/{transactionRid}/start"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), StartConcatenationTaskResponse)
@@ -154,15 +155,15 @@
         _path_params: Dict[str, Any] = {
             "concatenationTaskId": concatenation_task_id,
         }
 
         _json: Any = None
 
         _path = "/concatenation-tasks/tasks/{concatenationTaskId}/status-report"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "GET", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), ConcatenationTaskStatusReport)
```

### Comparing `palantir-sdk-0.8.0/palantir/datasets/rpc/path.py` & `palantir-sdk-0.9.0/palantir/datasets/rpc/path.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from conjure_python_client import (
     Service,
     ConjureDecoder,
     ConjureBeanType,
     ConjureFieldDefinition,
     OptionalTypeWrapper,
 )
+from .util import format_path_with_params
 
 
 class PathService(Service):
     def get_resource_by_path(
         self, auth_header: str, path: Optional[str] = None
     ) -> "Optional[DecoratedResource]":
         _headers: Dict[str, Any] = {
@@ -38,15 +39,15 @@
         }
 
         _path_params: Dict[str, Any] = {}
 
         _json = None
 
         _path = "/resources"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "GET", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return (
```

### Comparing `palantir-sdk-0.8.0/palantir/datasets/rpc/schema.py` & `palantir-sdk-0.9.0/palantir/datasets/rpc/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     ConjureBeanType,
     ConjureFieldDefinition,
     DictType,
     ConjureEnumType,
     OptionalTypeWrapper,
 )
 from requests import Response
+from .util import format_path_with_params
 
 
 class SchemaService(Service):
     def put_schema(
         self,
         auth_header: str,
         dataset_rid: str,
@@ -41,15 +42,20 @@
             "Authorization": auth_header,
         }
 
         _params: Mapping[str, Any] = {"endTransactionRid": end_transaction_rid}
 
         _json: Any = ConjureEncoder.do_encode(schema)
 
-        _path = f"/schemas/datasets/{dataset_rid}/branches/{branch_id}"
+        _path_params: Dict[str, Any] = {
+            "datasetRid": dataset_rid,
+            "branchId": branch_id,
+        }
+        _path = "/schemas/datasets/{datasetRid}/branches/{branchId}"
+        _path = format_path_with_params(_path, _path_params)
 
         _response: Response = self._request(
             "POST",
             self._uri + _path,
             params=_params,
             headers=_headers,
             json=_json,
@@ -69,15 +75,20 @@
         }
 
         _params: Mapping[str, Any] = {
             "endTransactionRid": end_transaction_rid,
             "versionId": version_rid,
         }
 
-        _path = f"/schemas/datasets/{dataset_rid}/branches/{branch_id}"
+        _path_params: Dict[str, Any] = {
+            "datasetRid": dataset_rid,
+            "branchId": branch_id,
+        }
+        _path = "/schemas/datasets/{datasetRid}/branches/{branchId}"
+        _path = format_path_with_params(_path, _path_params)
 
         _response: Response = self._request(
             "GET", self._uri + _path, params=_params, headers=_headers
         )
 
         _decoder = ConjureDecoder()
         return (
```

### Comparing `palantir-sdk-0.8.0/palantir/datasets/rpc/sql.py` & `palantir-sdk-0.9.0/palantir/datasets/rpc/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     ConjureDecoder,
     ConjureBeanType,
     ConjureFieldDefinition,
     ConjureEnumType,
     ConjureUnionType,
     OptionalTypeWrapper,
 )
+from .util import format_path_with_params
 
 
 class SqlQueryService(Service):
     def execute(
         self, auth_header: str, request: "SqlExecuteRequest"
     ) -> "SqlExecuteResponse":
         _headers: Dict[str, Any] = {
@@ -41,15 +42,15 @@
         _params: Dict[str, Any] = {}
 
         _path_params: Dict[str, Any] = {}
 
         _json = ConjureEncoder().default(request)
 
         _path = "/queries/execute"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(
             "POST", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), SqlExecuteResponse)
@@ -65,15 +66,15 @@
         _path_params: Dict[str, Any] = {
             "queryId": query_id,
         }
 
         _json: Any = None
 
         _path = "/queries/{queryId}/status"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(  # type: ignore
             "GET", self._uri + _path, params=_params, headers=_headers, json=_json
         )
 
         _decoder = ConjureDecoder()
         return _decoder.decode(_response.json(), SqlGetStatusResponse)
@@ -89,15 +90,15 @@
         _path_params: Dict[str, Any] = {
             "queryId": query_id,
         }
 
         _json: Any = None
 
         _path = "/queries/{queryId}/results"
-        _path = _path.format(**_path_params)
+        _path = format_path_with_params(_path, _path_params)
 
         _response = self._request(  # type: ignore
             "GET",
             self._uri + _path,
             params=_params,
             headers=_headers,
             stream=True,
```

### Comparing `palantir-sdk-0.8.0/palantir/datasets/schema.py` & `palantir-sdk-0.9.0/palantir/datasets/schema.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/palantir/datasets/types.py` & `palantir-sdk-0.9.0/palantir/datasets/types.py`

 * *Files identical despite different names*

### Comparing `palantir-sdk-0.8.0/pyproject.toml` & `palantir-sdk-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "palantir-sdk"
-version = "0.8.0"  # placeholder, updated by git describe during publish
+version = "0.9.0"  # placeholder, updated by git describe during publish
 description = "Palantir Python SDK"
 license = "Apache-2.0"
 authors = ["Andrew Higgins <ahiggins@palantir.com>"]
 packages = [{include = "palantir"}]
 include = ["palantir/_version.py"]
 homepage = "https://github.com/palantir/palantir-python-sdk"
```

### Comparing `palantir-sdk-0.8.0/setup.py` & `palantir-sdk-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['conjure-python-client>=2.1.0,<3.0.0', 'tomli>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'palantir-sdk',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Palantir Python SDK',
     'long_description': None,
     'author': 'Andrew Higgins',
     'author_email': 'ahiggins@palantir.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/palantir/palantir-python-sdk',
```

### Comparing `palantir-sdk-0.8.0/PKG-INFO` & `palantir-sdk-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palantir-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Palantir Python SDK
 Home-page: https://github.com/palantir/palantir-python-sdk
 License: Apache-2.0
 Author: Andrew Higgins
 Author-email: ahiggins@palantir.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

