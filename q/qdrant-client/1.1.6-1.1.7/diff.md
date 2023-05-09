# Comparing `tmp/qdrant_client-1.1.6.tar.gz` & `tmp/qdrant_client-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.1.6.tar", max compression
+gzip compressed data, was "qdrant_client-1.1.7.tar", max compression
```

## Comparing `qdrant_client-1.1.6.tar` & `qdrant_client-1.1.7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    11357 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/LICENSE
--rw-r--r--   0        0        0     6250 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/README.md
--rw-r--r--   0        0        0     1304 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/pyproject.toml
--rw-r--r--   0        0        0       56 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/__init__.py
--rw-r--r--   0        0        0    25845 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/client_base.py
--rw-r--r--   0        0        0     9363 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3231 2023-04-25 22:06:31.201146 qdrant_client-1.1.6/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    62445 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    28633 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     1794 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    13456 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    44493 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2502 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    23694 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    30407 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    30820 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    18850 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    60032 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    21902 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     5888 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2922 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     2237 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    18939 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0       40 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-04-25 22:06:31.209145 qdrant_client-1.1.6/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    10979 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1168 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1936 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    14566 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2196 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/py.typed
--rw-r--r--   0        0        0    55103 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    90192 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2865 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2537 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-04-25 22:06:31.213146 qdrant_client-1.1.6/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     7309 1970-01-01 00:00:00.000000 qdrant_client-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 15:43:22.771894 qdrant_client-1.1.7/LICENSE
+-rw-r--r--   0        0        0     6250 2023-05-09 15:43:22.771894 qdrant_client-1.1.7/README.md
+-rw-r--r--   0        0        0     1327 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/__init__.py
+-rw-r--r--   0        0        0    25845 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     9363 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3231 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    62445 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    28633 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     1794 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    13456 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    44493 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2502 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    23694 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      505 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:43:22.775894 qdrant_client-1.1.7/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10437 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    30407 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    30820 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9499 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    18850 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    60032 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2962 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    21902 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     5888 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     4388 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    19858 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0       40 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    10979 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1168 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    14566 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2196 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/py.typed
+-rw-r--r--   0        0        0    55103 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    90192 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2865 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2537 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3200 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-09 15:43:22.779894 qdrant_client-1.1.7/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     7353 1970-01-01 00:00:00.000000 qdrant_client-1.1.7/PKG-INFO
```

### Comparing `qdrant_client-1.1.6/LICENSE` & `qdrant_client-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/README.md` & `qdrant_client-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/pyproject.toml` & `qdrant_client-1.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.1.6"
+version = "1.1.7"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 readme = "README.md"
@@ -20,14 +20,15 @@
     { version = ">=1.21", python = ">=3.8" }
 ]
 pydantic = "^1.8"
 typing-extensions = "^4.0.0"
 grpcio = { version = ">=1.41.0", allow-prereleases = true }
 grpcio-tools = ">=1.41.0"
 urllib3 = "^1.26.14"
+portalocker = "^2.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
 grpcio-tools = "^1.46.0"
 sphinx = "^4.4.0"
 qdrant-sphinx-theme = { git = "https://github.com/qdrant/qdrant_sphinx_theme.git", branch = "master" }
 coverage = "^6.3.3"
```

### Comparing `qdrant_client-1.1.6/qdrant_client/client_base.py` & `qdrant_client-1.1.7/qdrant_client/client_base.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/connection.py` & `qdrant_client-1.1.7/qdrant_client/connection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/conversions/common_types.py` & `qdrant_client-1.1.7/qdrant_client/conversions/common_types.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/conversions/conversion.py` & `qdrant_client-1.1.7/qdrant_client/conversions/conversion.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.1.7/qdrant_client/grpc/collections_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.1.7/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.1.7/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.1.7/qdrant_client/grpc/points_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.1.7/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.1.7/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.1.7/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.1.7/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.1.7/qdrant_client/http/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/api/points_api.py` & `qdrant_client-1.1.7/qdrant_client/http/api/points_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/api/service_api.py` & `qdrant_client-1.1.7/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.1.7/qdrant_client/http/api/snapshots_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/api_client.py` & `qdrant_client-1.1.7/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/exceptions.py` & `qdrant_client-1.1.7/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/http/models/models.py` & `qdrant_client-1.1.7/qdrant_client/http/models/models.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/local/distances.py` & `qdrant_client-1.1.7/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/local/geo.py` & `qdrant_client-1.1.7/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/local/local_collection.py` & `qdrant_client-1.1.7/qdrant_client/local/local_collection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/local/payload_filters.py` & `qdrant_client-1.1.7/qdrant_client/local/payload_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.1.7/qdrant_client/local/payload_value_extractor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.1.7/qdrant_client/local/qdrant_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 import logging
 import os
 import shutil
-import numpy as np
+from io import TextIOWrapper
 from itertools import zip_longest
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
+import numpy as np
+import portalocker
+
 from qdrant_client.client_base import QdrantBase
 from qdrant_client.conversions import common_types as types
 from qdrant_client.http import models as rest_models
 from qdrant_client.local.local_collection import LocalCollection
 
 META_INFO_FILENAME = "meta.json"
 
@@ -32,14 +35,16 @@
         Args:
             location: Where to store data. Can be a path to a directory or `:memory:` for in-memory storage.
         """
         self.location = location
         self.persistent = location != ":memory:"
         self.collections: Dict[str, LocalCollection] = {}
         self.aliases: Dict[str, str] = {}
+        self._lock = None
+        self._flock_file: Optional[TextIOWrapper] = None
         self._load()
 
     def _load(self) -> None:
         if not self.persistent:
             return
         meta_path = os.path.join(self.location, META_INFO_FILENAME)
         if not os.path.exists(meta_path):
@@ -51,14 +56,31 @@
                 meta = json.load(f)
                 for collection_name, config_json in meta["collections"].items():
                     config = rest_models.CreateCollection(**config_json)
                     collection_path = self._collection_path(collection_name)
                     self.collections[collection_name] = LocalCollection(config, collection_path)
                 self.aliases = meta["aliases"]
 
+        lock_file_path = os.path.join(self.location, ".lock")
+        if not os.path.exists(lock_file_path):
+            os.makedirs(self.location, exist_ok=True)
+            with open(lock_file_path, "w") as f:
+                f.write("tmp lock file")
+        self._flock_file = open(lock_file_path, "r+")
+        try:
+            self._flock = portalocker.lock(
+                self._flock_file,
+                portalocker.LockFlags.EXCLUSIVE | portalocker.LockFlags.NON_BLOCKING,
+            )
+        except portalocker.exceptions.LockException:
+            raise RuntimeError(
+                f"Storage folder {self.location} is already accessed by another instance of Qdrant client."
+                f" If you require concurrent access, use Qdrant server instead."
+            )
+
     def _save(self) -> None:
         if not self.persistent:
             return
         meta_path = os.path.join(self.location, META_INFO_FILENAME)
         with open(meta_path, "w") as f:
             f.write(
                 json.dumps(
```

### Comparing `qdrant_client-1.1.6/qdrant_client/parallel_processor.py` & `qdrant_client-1.1.7/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/proto/collections.proto` & `qdrant_client-1.1.7/qdrant_client/proto/collections.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.1.7/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.1.7/qdrant_client/proto/json_with_int.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/proto/points.proto` & `qdrant_client-1.1.7/qdrant_client/proto/points.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/proto/points_service.proto` & `qdrant_client-1.1.7/qdrant_client/proto/points_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.1.7/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/qdrant_client.py` & `qdrant_client-1.1.7/qdrant_client/qdrant_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/qdrant_remote.py` & `qdrant_client-1.1.7/qdrant_client/qdrant_remote.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.1.7/qdrant_client/uploader/grpc_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.1.7/qdrant_client/uploader/rest_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/qdrant_client/uploader/uploader.py` & `qdrant_client-1.1.7/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.6/PKG-INFO` & `qdrant_client-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.1.6
+Version: 1.1.7
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.41.0)
 Requires-Dist: grpcio-tools (>=1.41.0)
 Requires-Dist: httpx[http2] (>=0.14.0)
 Requires-Dist: numpy (<1.21) ; python_version < "3.8"
 Requires-Dist: numpy (>=1.21) ; python_version >= "3.8"
+Requires-Dist: portalocker (>=2.7.0,<3.0.0)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
 Project-URL: Repository, https://github.com/qdrant/qdrant-client
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.6 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.7 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client Keywords: vector,search,neural,matching,client Author:
 Andrey Vasnetsov Author-email: andrey@qdrant.tech Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.41.0) Requires-Dist: grpcio-tools (>=1.41.0)
 Requires-Dist: httpx[http2] (>=0.14.0) Requires-Dist: numpy (<1.21) ;
 python_version < "3.8" Requires-Dist: numpy (>=1.21) ; python_version >= "3.8"
-Requires-Dist: pydantic (>=1.8,<2.0) Requires-Dist: typing-extensions
-(>=4.0.0,<5.0.0) Requires-Dist: urllib3 (>=1.26.14,<2.0.0) Project-URL:
-Repository, https://github.com/qdrant/qdrant-client Description-Content-Type:
-text/markdown
+Requires-Dist: portalocker (>=2.7.0,<3.0.0) Requires-Dist: pydantic
+(>=1.8,<2.0) Requires-Dist: typing-extensions (>=4.0.0,<5.0.0) Requires-Dist:
+urllib3 (>=1.26.14,<2.0.0) Project-URL: Repository, https://github.com/qdrant/
+qdrant-client Description-Content-Type: text/markdown
                                    [Qdrant]
           Python Client library for the Qdrant vector search engine.
   [PyPI_version] [OpenAPI_Docs] [Apache_2.0_License] [Discord] [Roadmap_2023]
 # Python Qdrant Client Client library and SDK for the [Qdrant](https://
 github.com/qdrant/qdrant) vector search engine. Library contains type
 definitions for all Qdrant API and allows to make both Sync and Async requests.
 Client allows calls for all [Qdrant API methods](https://qdrant.github.io/
```

