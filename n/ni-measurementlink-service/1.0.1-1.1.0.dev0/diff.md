# Comparing `tmp/ni_measurementlink_service-1.0.1.tar.gz` & `tmp/ni_measurementlink_service-1.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ni_measurementlink_service-1.0.1.tar", max compression
+gzip compressed data, was "ni_measurementlink_service-1.1.0.dev0.tar", max compression
```

## Comparing `ni_measurementlink_service-1.0.1.tar` & `ni_measurementlink_service-1.1.0.dev0.tar`

### file list

```diff
@@ -1,55 +1,61 @@
--rw-r--r--   0        0        0     1071 2023-03-24 16:33:23.187670 ni_measurementlink_service-1.0.1/LICENSE
--rw-r--r--   0        0        0    15792 2023-03-24 16:33:23.187670 ni_measurementlink_service-1.0.1/README.md
--rw-r--r--   0        0        0      517 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/__init__.py
--rw-r--r--   0        0        0       62 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/__init__.py
--rw-r--r--   0        0        0    10333 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/discovery_client.py
--rw-r--r--   0        0        0     8872 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/grpc_servicer.py
--rw-r--r--   0        0        0       58 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/parameter/__init__.py
--rw-r--r--   0        0        0     2236 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/parameter/metadata.py
--rw-r--r--   0        0        0     9062 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
--rw-r--r--   0        0        0     6197 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/parameter/serializer.py
--rw-r--r--   0        0        0     3371 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/service_manager.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/__init__.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/__init__.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
--rw-r--r--   0        0        0     4348 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
--rw-r--r--   0        0        0     9392 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
--rw-r--r--   0        0        0    11001 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
--rw-r--r--   0        0        0     5454 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
--rw-r--r--   0        0        0    14601 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
--rw-r--r--   0        0        0     5629 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
--rw-r--r--   0        0        0     1554 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
--rw-r--r--   0        0        0     1343 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
--rw-r--r--   0        0        0      158 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
--rw-r--r--   0        0        0     6337 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
--rw-r--r--   0        0        0    19326 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
--rw-r--r--   0        0        0    14348 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
--rw-r--r--   0        0        0       33 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
--rw-r--r--   0        0        0     6072 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
--rw-r--r--   0        0        0    13959 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
--rw-r--r--   0        0        0    14097 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
--rw-r--r--   0        0        0      709 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/README.md
--rw-r--r--   0        0        0     6052 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
--rw-r--r--   0        0        0     6650 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
--rw-r--r--   0        0        0      712 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
--rw-r--r--   0        0        0     9622 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
--rw-r--r--   0        0        0     8468 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
--rw-r--r--   0        0        0     2426 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/session.proto
--rw-r--r--   0        0        0     4320 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/session_pb2.py
--rw-r--r--   0        0        0     9200 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
--rw-r--r--   0        0        0     9142 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
--rw-r--r--   0        0        0       35 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/utilities/__init__.py
--rw-r--r--   0        0        0       37 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/measurement/__init__.py
--rw-r--r--   0        0        0     3021 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/measurement/info.py
--rw-r--r--   0        0        0    13261 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/measurement/service.py
--rw-r--r--   0        0        0    14466 2023-03-24 16:33:23.231670 ni_measurementlink_service-1.0.1/ni_measurementlink_service/session_management.py
--rw-r--r--   0        0        0     2357 2023-03-24 16:34:55.772174 ni_measurementlink_service-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    18476 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.0.1/setup.py
--rw-r--r--   0        0        0    17006 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 22:25:40.024292 ni_measurementlink_service-1.1.0.dev0/LICENSE
+-rw-r--r--   0        0        0    15792 2023-05-08 22:25:40.024292 ni_measurementlink_service-1.1.0.dev0/README.md
+-rw-r--r--   0        0        0      513 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/__init__.py
+-rw-r--r--   0        0        0    10404 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/discovery_client.py
+-rw-r--r--   0        0        0    16735 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/grpc_servicer.py
+-rw-r--r--   0        0        0       58 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/__init__.py
+-rw-r--r--   0        0        0     2236 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py
+-rw-r--r--   0        0        0     9062 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py
+-rw-r--r--   0        0        0     6182 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py
+-rw-r--r--   0        0        0     3933 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/service_manager.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/__init__.py
+-rw-r--r--   0        0        0     4264 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py
+-rw-r--r--   0        0        0     8921 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi
+-rw-r--r--   0        0        0    10817 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/__init__.py
+-rw-r--r--   0        0        0     5345 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py
+-rw-r--r--   0        0        0    13593 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5546 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/__init__.py
+-rw-r--r--   0        0        0     5777 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py
+-rw-r--r--   0        0        0    15001 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi
+-rw-r--r--   0        0        0     5549 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1532 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py
+-rw-r--r--   0        0        0     1314 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/__init__.py
+-rw-r--r--   0        0        0     6202 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py
+-rw-r--r--   0        0        0    18188 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi
+-rw-r--r--   0        0        0    14078 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/__init__.py
+-rw-r--r--   0        0        0     5955 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py
+-rw-r--r--   0        0        0    13237 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13882 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0      709 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md
+-rw-r--r--   0        0        0     6052 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto
+-rw-r--r--   0        0        0     6650 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto
+-rw-r--r--   0        0        0     7228 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v2/measurement_service.proto
+-rw-r--r--   0        0        0      712 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto
+-rw-r--r--   0        0        0     9622 2023-05-08 22:25:40.068291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto
+-rw-r--r--   0        0        0     8468 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto
+-rw-r--r--   0        0        0     2426 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto
+-rw-r--r--   0        0        0     4196 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py
+-rw-r--r--   0        0        0     8735 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi
+-rw-r--r--   0        0        0     8948 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py
+-rw-r--r--   0        0        0       35 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/utilities/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/__init__.py
+-rw-r--r--   0        0        0     3021 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/info.py
+-rw-r--r--   0        0        0    13261 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/service.py
+-rw-r--r--   0        0        0        0 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/py.typed
+-rw-r--r--   0        0        0    14466 2023-05-08 22:25:40.072291 ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/session_management.py
+-rw-r--r--   0        0        0     2650 2023-05-08 22:27:14.811198 ni_measurementlink_service-1.1.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    18650 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev0/setup.py
+-rw-r--r--   0        0        0    17006 1970-01-01 00:00:00.000000 ni_measurementlink_service-1.1.0.dev0/PKG-INFO
```

### Comparing `ni_measurementlink_service-1.0.1/LICENSE` & `ni_measurementlink_service-1.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/README.md` & `ni_measurementlink_service-1.1.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/discovery_client.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/discovery_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,18 @@
     import msvcrt
 
     import win32con
     import win32file
     import winerror
 
 
-_PROVIDED_MEASUREMENT_SERVICE = "ni.measurementlink.measurement.v1.MeasurementService"
+_PROVIDED_MEASUREMENT_SERVICES = [
+    "ni.measurementlink.measurement.v1.MeasurementService",
+    "ni.measurementlink.measurement.v2.MeasurementService",
+]
 
 _logger = logging.getLogger(__name__)
 
 
 class ServiceLocation(typing.NamedTuple):
     """Represents the location of a service."""
 
@@ -104,15 +107,15 @@
             service_location.location = "localhost"
             service_location.insecure_port = service_port
             # Service Descriptor
             service_descriptor = discovery_service_pb2.ServiceDescriptor()
             service_descriptor.display_name = measurement_info.display_name
             service_descriptor.service_class = service_info.service_class
             service_descriptor.description_url = service_info.description_url
-            service_descriptor.provided_interfaces.append(_PROVIDED_MEASUREMENT_SERVICE)
+            service_descriptor.provided_interfaces.extend(_PROVIDED_MEASUREMENT_SERVICES)
 
             # Registration Request Creation
             request = discovery_service_pb2.RegisterServiceRequest(
                 location=service_location, service_description=service_descriptor
             )
             # Registration RPC Call
             register_response = self.stub.RegisterService(request)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/parameter/metadata.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/metadata.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/parameter/serialization_strategy.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serialization_strategy.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/parameter/serializer.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/parameter/serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """Parameter Serializer."""
 
-from ast import Bytes
 from io import BytesIO
-from typing import Any, Dict, List
+from typing import Any, Dict, Sequence
 
 from google.protobuf.internal import encoder
 
 from ni_measurementlink_service._internal.parameter import serialization_strategy
 from ni_measurementlink_service._internal.parameter.metadata import ParameterMetadata
 
-
 _GRPC_WIRE_TYPE_BIT_WIDTH = 3
 
 
 def deserialize_parameters(
-    parameter_metadata_dict: Dict[int, ParameterMetadata], parameter_bytes: Bytes
+    parameter_metadata_dict: Dict[int, ParameterMetadata], parameter_bytes: bytes
 ) -> Dict[int, Any]:
     """Deserialize the bytes of the parameter based on the metadata.
 
     Args
     ----
         parameter_metadata_dict (Dict[int, ParameterMetadata]): Parameter metadata by ID.
 
-        parameter_bytes (bytes): Bytes of Parameter that need to be deserialized.
+        parameter_bytes (bytes): Byte string to deserialize.
 
     Returns
     -------
         Dict[int, Any]: Deserialized parameters by ID
 
     """
     # Getting overlapping parameters
@@ -38,31 +36,32 @@
         parameter_metadata_dict, overlapping_parameter_by_id
     )
     overlapping_parameter_by_id.update(missing_parameters)
     return overlapping_parameter_by_id
 
 
 def serialize_parameters(
-    parameter_metadata_dict: Dict[int, ParameterMetadata], parameter_value: List[Any]
+    parameter_metadata_dict: Dict[int, ParameterMetadata],
+    parameter_values: Sequence[Any],
 ) -> bytes:
     """Serialize the parameter values in same order based on the metadata_dict.
 
     Args
     ----
         parameter_metadata_dict (Dict[int, ParameterMetadata]): Parameter metadata by ID.
 
-        parameter_value (List[Any]): List of Parameter values that need to be serialized.
+        parameter_value (Sequence[Any]): Parameter values to serialize.
 
     Returns
     -------
-        Bytes: Serialized Bytes of Parameter Values.
+        bytes: Serialized byte string containing parameter values.
 
     """
     serialize_buffer = BytesIO()  # inner_encoder updates the serialize_buffer
-    for i, parameter in enumerate(parameter_value):
+    for i, parameter in enumerate(parameter_values):
         parameter_metadata = parameter_metadata_dict[i + 1]
         encoder = serialization_strategy.Context.get_encoder(
             parameter_metadata.type,
             parameter_metadata.repeated,
         )
         type_default_value = serialization_strategy.Context.get_type_default(
             parameter_metadata.type,
@@ -80,66 +79,65 @@
 
     Args
     -----
         parameter_metadata_dict (Dict[int, ParameterMetadata]): Configuration metadata.
 
     Returns
     -------
-        bytes: Serialized Bytes of default value.
+        bytes: Serialized byte string containing default values.
 
     """
     default_value_parameter_array = list()
     default_value_parameter_array = [
         parameter.default_value for parameter in parameter_metadata_dict.values()
     ]
     return serialize_parameters(parameter_metadata_dict, default_value_parameter_array)
 
 
-def _get_field_index(parameter_bytes, tag_position: int):
+def _get_field_index(parameter_bytes: bytes, tag_position: int):
     """Get the Filed Index based on the tag's position.
 
     The tag Position should be the index of the TagValue in the ByteArray for valid field index.
 
     Args
     ----
-        parameter_bytes (Bytes): Serialized Bytes
+        parameter_bytes (bytes): Serialized bytes
 
         tag_position (int): Tag position
 
     Returns
     -------
         int: Filed index of the Tag Position
 
     """
     return parameter_bytes[tag_position] >> _GRPC_WIRE_TYPE_BIT_WIDTH
 
 
 def _get_overlapping_parameters(
-    parameter_metadata_dict: Dict[int, ParameterMetadata], parameter_bytes
+    parameter_metadata_dict: Dict[int, ParameterMetadata], parameter_bytes: bytes
 ) -> Dict[int, Any]:
     """Get the parameters present in both `parameter_metadata_dict` and `parameter_bytes`.
 
     Args
     ----
         parameter_metadata_dict (Dict[int, ParameterMetadata]): Parameter metadata by ID.
 
-        parameter_bytes (bytes): Bytes of Parameter that need to be deserialized.
+        parameter_bytes (bytes): bytes of Parameter that need to be deserialized.
 
     Raises
     ------
         Exception: If the protobuf filed index is invalid.
 
     Returns
     -------
         Dict[int, Any]: Overlapping Parameters by ID.
 
     """
-    overlapping_parameters_by_id: Dict[
-        int, Any
-    ] = {}  # inner_decoder update the overlapping_parameters
+    # inner_decoder update the overlapping_parameters
+    overlapping_parameters_by_id: Dict[int, Any] = {}
     position = 0
     while position < len(parameter_bytes):
         field_index = _get_field_index(parameter_bytes, position)
         if field_index not in parameter_metadata_dict:
             raise Exception(
                 f"Error occurred while reading the parameter - given protobuf index '{field_index}' is invalid."
             )
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/service_manager.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/service_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 from typing import Callable, List, Optional
 
 import grpc
 from grpc.framework.foundation import logging_pool
 
 from ni_measurementlink_service._internal.discovery_client import DiscoveryClient
 from ni_measurementlink_service._internal.grpc_servicer import (
-    MeasurementServiceServicer,
+    MeasurementServiceServicerV1,
+    MeasurementServiceServicerV2,
 )
 from ni_measurementlink_service._internal.parameter.metadata import ParameterMetadata
 from ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v1 import (
-    measurement_service_pb2_grpc,
+    measurement_service_pb2_grpc as v1_measurement_service_pb2_grpc,
+)
+from ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v2 import (
+    measurement_service_pb2_grpc as v2_measurement_service_pb2_grpc,
 )
 from ni_measurementlink_service.measurement.info import MeasurementInfo, ServiceInfo
 
 _logger = logging.getLogger(__name__)
 
 
 class GrpcService:
@@ -72,22 +76,31 @@
         self.server = grpc.server(
             logging_pool.pool(max_workers=10),
             options=[
                 ("grpc.max_receive_message_length", -1),
                 ("grpc.max_send_message_length", -1),
             ],
         )
-        self.servicer = MeasurementServiceServicer(
+        servicer_v1 = MeasurementServiceServicerV1(
+            measurement_info,
+            configuration_parameter_list,
+            output_parameter_list,
+            measure_function,
+        )
+        v1_measurement_service_pb2_grpc.add_MeasurementServiceServicer_to_server(
+            servicer_v1, self.server
+        )
+        servicer_v2 = MeasurementServiceServicerV2(
             measurement_info,
             configuration_parameter_list,
             output_parameter_list,
             measure_function,
         )
-        measurement_service_pb2_grpc.add_MeasurementServiceServicer_to_server(
-            self.servicer, self.server
+        v2_measurement_service_pb2_grpc.add_MeasurementServiceServicer_to_server(
+            servicer_v2, self.server
         )
         port = str(self.server.add_insecure_port("[::]:0"))
         self.server.start()
         _logger.info("Measurement service hosted on port: %s", port)
         self.discovery_client.register_measurement_service(port, service_info, measurement_info)
 
         self.port = port
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,46 +2,43 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ni/measurementlink/discovery/v1/discovery_service.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n7ni/measurementlink/discovery/v1/discovery_service.proto\x12\x1fni.measurementlink.discovery.v1"v\n\x11ServiceDescriptor\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x65scription_url\x18\x02 \x01(\t\x12\x1b\n\x13provided_interfaces\x18\x03 \x03(\t\x12\x15\n\rservice_class\x18\x04 \x01(\t"Z\n\x0fServiceLocation\x12\x10\n\x08location\x18\x01 \x01(\t\x12\x15\n\rinsecure_port\x18\x02 \x01(\t\x12\x1e\n\x16ssl_authenticated_port\x18\x03 \x01(\t"\xad\x01\n\x16RegisterServiceRequest\x12O\n\x13service_description\x18\x01 \x01(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor\x12\x42\n\x08location\x18\x02 \x01(\x0b\x32\x30.ni.measurementlink.discovery.v1.ServiceLocation"2\n\x17RegisterServiceResponse\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t"3\n\x18UnregisterServiceRequest\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t"\x1b\n\x19UnregisterServiceResponse"6\n\x18\x45numerateServicesRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t"k\n\x19\x45numerateServicesResponse\x12N\n\x12\x61vailable_services\x18\x01 \x03(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor"J\n\x15ResolveServiceRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t\x12\x15\n\rservice_class\x18\x02 \x01(\t2\xaf\x04\n\x10\x44iscoveryService\x12\x84\x01\n\x0fRegisterService\x12\x37.ni.measurementlink.discovery.v1.RegisterServiceRequest\x1a\x38.ni.measurementlink.discovery.v1.RegisterServiceResponse\x12\x8a\x01\n\x11UnregisterService\x12\x39.ni.measurementlink.discovery.v1.UnregisterServiceRequest\x1a:.ni.measurementlink.discovery.v1.UnregisterServiceResponse\x12\x8a\x01\n\x11\x45numerateServices\x12\x39.ni.measurementlink.discovery.v1.EnumerateServicesRequest\x1a:.ni.measurementlink.discovery.v1.EnumerateServicesResponse\x12z\n\x0eResolveService\x12\x36.ni.measurementlink.discovery.v1.ResolveServiceRequest\x1a\x30.ni.measurementlink.discovery.v1.ServiceLocationB\xcc\x01\n#com.ni.measurementlink.discovery.v1B\x15\x44iscoveryServiceProtoP\x01Z\x0b\x64iscoveryv1\xa2\x02\x04NIMD\xaa\x02\x30NationalInstruments.MeasurementLink.Discovery.V1\xca\x02\x1fNI\\MeasurementLink\\Discovery\\V1\xea\x02"NI::MeasurementLink::Discovery::V1b\x06proto3'
-)
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7ni/measurementlink/discovery/v1/discovery_service.proto\x12\x1fni.measurementlink.discovery.v1\"v\n\x11ServiceDescriptor\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x17\n\x0f\x64\x65scription_url\x18\x02 \x01(\t\x12\x1b\n\x13provided_interfaces\x18\x03 \x03(\t\x12\x15\n\rservice_class\x18\x04 \x01(\t\"Z\n\x0fServiceLocation\x12\x10\n\x08location\x18\x01 \x01(\t\x12\x15\n\rinsecure_port\x18\x02 \x01(\t\x12\x1e\n\x16ssl_authenticated_port\x18\x03 \x01(\t\"\xad\x01\n\x16RegisterServiceRequest\x12O\n\x13service_description\x18\x01 \x01(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor\x12\x42\n\x08location\x18\x02 \x01(\x0b\x32\x30.ni.measurementlink.discovery.v1.ServiceLocation\"2\n\x17RegisterServiceResponse\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t\"3\n\x18UnregisterServiceRequest\x12\x17\n\x0fregistration_id\x18\x01 \x01(\t\"\x1b\n\x19UnregisterServiceResponse\"6\n\x18\x45numerateServicesRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t\"k\n\x19\x45numerateServicesResponse\x12N\n\x12\x61vailable_services\x18\x01 \x03(\x0b\x32\x32.ni.measurementlink.discovery.v1.ServiceDescriptor\"J\n\x15ResolveServiceRequest\x12\x1a\n\x12provided_interface\x18\x01 \x01(\t\x12\x15\n\rservice_class\x18\x02 \x01(\t2\xaf\x04\n\x10\x44iscoveryService\x12\x84\x01\n\x0fRegisterService\x12\x37.ni.measurementlink.discovery.v1.RegisterServiceRequest\x1a\x38.ni.measurementlink.discovery.v1.RegisterServiceResponse\x12\x8a\x01\n\x11UnregisterService\x12\x39.ni.measurementlink.discovery.v1.UnregisterServiceRequest\x1a:.ni.measurementlink.discovery.v1.UnregisterServiceResponse\x12\x8a\x01\n\x11\x45numerateServices\x12\x39.ni.measurementlink.discovery.v1.EnumerateServicesRequest\x1a:.ni.measurementlink.discovery.v1.EnumerateServicesResponse\x12z\n\x0eResolveService\x12\x36.ni.measurementlink.discovery.v1.ResolveServiceRequest\x1a\x30.ni.measurementlink.discovery.v1.ServiceLocationB\xcc\x01\n#com.ni.measurementlink.discovery.v1B\x15\x44iscoveryServiceProtoP\x01Z\x0b\x64iscoveryv1\xa2\x02\x04NIMD\xaa\x02\x30NationalInstruments.MeasurementLink.Discovery.V1\xca\x02\x1fNI\\MeasurementLink\\Discovery\\V1\xea\x02\"NI::MeasurementLink::Discovery::V1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "ni.measurementlink.discovery.v1.discovery_service_pb2", globals()
-)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ni.measurementlink.discovery.v1.discovery_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b'\n#com.ni.measurementlink.discovery.v1B\025DiscoveryServiceProtoP\001Z\013discoveryv1\242\002\004NIMD\252\0020NationalInstruments.MeasurementLink.Discovery.V1\312\002\037NI\\MeasurementLink\\Discovery\\V1\352\002"NI::MeasurementLink::Discovery::V1'
-    _SERVICEDESCRIPTOR._serialized_start = 92
-    _SERVICEDESCRIPTOR._serialized_end = 210
-    _SERVICELOCATION._serialized_start = 212
-    _SERVICELOCATION._serialized_end = 302
-    _REGISTERSERVICEREQUEST._serialized_start = 305
-    _REGISTERSERVICEREQUEST._serialized_end = 478
-    _REGISTERSERVICERESPONSE._serialized_start = 480
-    _REGISTERSERVICERESPONSE._serialized_end = 530
-    _UNREGISTERSERVICEREQUEST._serialized_start = 532
-    _UNREGISTERSERVICEREQUEST._serialized_end = 583
-    _UNREGISTERSERVICERESPONSE._serialized_start = 585
-    _UNREGISTERSERVICERESPONSE._serialized_end = 612
-    _ENUMERATESERVICESREQUEST._serialized_start = 614
-    _ENUMERATESERVICESREQUEST._serialized_end = 668
-    _ENUMERATESERVICESRESPONSE._serialized_start = 670
-    _ENUMERATESERVICESRESPONSE._serialized_end = 777
-    _RESOLVESERVICEREQUEST._serialized_start = 779
-    _RESOLVESERVICEREQUEST._serialized_end = 853
-    _DISCOVERYSERVICE._serialized_start = 856
-    _DISCOVERYSERVICE._serialized_end = 1415
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n#com.ni.measurementlink.discovery.v1B\025DiscoveryServiceProtoP\001Z\013discoveryv1\242\002\004NIMD\252\0020NationalInstruments.MeasurementLink.Discovery.V1\312\002\037NI\\MeasurementLink\\Discovery\\V1\352\002\"NI::MeasurementLink::Discovery::V1'
+  _SERVICEDESCRIPTOR._serialized_start=92
+  _SERVICEDESCRIPTOR._serialized_end=210
+  _SERVICELOCATION._serialized_start=212
+  _SERVICELOCATION._serialized_end=302
+  _REGISTERSERVICEREQUEST._serialized_start=305
+  _REGISTERSERVICEREQUEST._serialized_end=478
+  _REGISTERSERVICERESPONSE._serialized_start=480
+  _REGISTERSERVICERESPONSE._serialized_end=530
+  _UNREGISTERSERVICEREQUEST._serialized_start=532
+  _UNREGISTERSERVICEREQUEST._serialized_end=583
+  _UNREGISTERSERVICERESPONSE._serialized_start=585
+  _UNREGISTERSERVICERESPONSE._serialized_end=612
+  _ENUMERATESERVICESREQUEST._serialized_start=614
+  _ENUMERATESERVICESREQUEST._serialized_end=668
+  _ENUMERATESERVICESRESPONSE._serialized_start=670
+  _ENUMERATESERVICESRESPONSE._serialized_end=777
+  _RESOLVESERVICEREQUEST._serialized_start=779
+  _RESOLVESERVICEREQUEST._serialized_end=853
+  _DISCOVERYSERVICE._serialized_start=856
+  _DISCOVERYSERVICE._serialized_end=1415
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -31,17 +31,15 @@
     PROVIDED_INTERFACES_FIELD_NUMBER: builtins.int
     SERVICE_CLASS_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Required. The user visible name of the service."""
     description_url: builtins.str
     """Optional. Url which provides descriptive information about the service"""
     @property
-    def provided_interfaces(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+    def provided_interfaces(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Required. The service interfaces provided by the service. This is the gRPC Full Name of the service.
         Registration can use the gRPC metadata to provide these names.
         """
     service_class: builtins.str
     """Required. The "class" of a service. The value of this field should be unique for a given interface in provided_interfaces.
     In effect, the .proto service declaration defines the interface, and this field defines a class or concrete type of the interface.
     """
@@ -49,27 +47,15 @@
         self,
         *,
         display_name: builtins.str = ...,
         description_url: builtins.str = ...,
         provided_interfaces: collections.abc.Iterable[builtins.str] | None = ...,
         service_class: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "description_url",
-            b"description_url",
-            "display_name",
-            b"display_name",
-            "provided_interfaces",
-            b"provided_interfaces",
-            "service_class",
-            b"service_class",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description_url", b"description_url", "display_name", b"display_name", "provided_interfaces", b"provided_interfaces", "service_class", b"service_class"]) -> None: ...
 
 global___ServiceDescriptor = ServiceDescriptor
 
 @typing_extensions.final
 class ServiceLocation(google.protobuf.message.Message):
     """Represents the location of a service. The location generally includes the IP address and port number for the service
     which can be used to establish communication with the service.
@@ -93,25 +79,15 @@
     def __init__(
         self,
         *,
         location: builtins.str = ...,
         insecure_port: builtins.str = ...,
         ssl_authenticated_port: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "insecure_port",
-            b"insecure_port",
-            "location",
-            b"location",
-            "ssl_authenticated_port",
-            b"ssl_authenticated_port",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["insecure_port", b"insecure_port", "location", b"location", "ssl_authenticated_port", b"ssl_authenticated_port"]) -> None: ...
 
 global___ServiceLocation = ServiceLocation
 
 @typing_extensions.final
 class RegisterServiceRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -125,26 +101,16 @@
         """Required. The canonical location information for the service."""
     def __init__(
         self,
         *,
         service_description: global___ServiceDescriptor | None = ...,
         location: global___ServiceLocation | None = ...,
     ) -> None: ...
-    def HasField(
-        self,
-        field_name: typing_extensions.Literal[
-            "location", b"location", "service_description", b"service_description"
-        ],
-    ) -> builtins.bool: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "location", b"location", "service_description", b"service_description"
-        ],
-    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["location", b"location", "service_description", b"service_description"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["location", b"location", "service_description", b"service_description"]) -> None: ...
 
 global___RegisterServiceRequest = RegisterServiceRequest
 
 @typing_extensions.final
 class RegisterServiceResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -152,17 +118,15 @@
     registration_id: builtins.str
     """ID that can be used to unregister the service."""
     def __init__(
         self,
         *,
         registration_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["registration_id", b"registration_id"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["registration_id", b"registration_id"]) -> None: ...
 
 global___RegisterServiceResponse = RegisterServiceResponse
 
 @typing_extensions.final
 class UnregisterServiceRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -170,17 +134,15 @@
     registration_id: builtins.str
     """Required. The registration ID of the service that should be unregistered."""
     def __init__(
         self,
         *,
         registration_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["registration_id", b"registration_id"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["registration_id", b"registration_id"]) -> None: ...
 
 global___UnregisterServiceRequest = UnregisterServiceRequest
 
 @typing_extensions.final
 class UnregisterServiceResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -200,40 +162,32 @@
     information for all services registered with the discovery service will be returned.
     """
     def __init__(
         self,
         *,
         provided_interface: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["provided_interface", b"provided_interface"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["provided_interface", b"provided_interface"]) -> None: ...
 
 global___EnumerateServicesRequest = EnumerateServicesRequest
 
 @typing_extensions.final
 class EnumerateServicesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AVAILABLE_SERVICES_FIELD_NUMBER: builtins.int
     @property
-    def available_services(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___ServiceDescriptor
-    ]:
+    def available_services(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceDescriptor]:
         """The list of available services which implement the specified service interface."""
     def __init__(
         self,
         *,
         available_services: collections.abc.Iterable[global___ServiceDescriptor] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["available_services", b"available_services"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["available_services", b"available_services"]) -> None: ...
 
 global___EnumerateServicesResponse = EnumerateServicesResponse
 
 @typing_extensions.final
 class ResolveServiceRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -249,15 +203,10 @@
     """
     def __init__(
         self,
         *,
         provided_interface: builtins.str = ...,
         service_class: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "provided_interface", b"provided_interface", "service_class", b"service_class"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["provided_interface", b"provided_interface", "service_class", b"service_class"]) -> None: ...
 
 global___ResolveServiceRequest = ResolveServiceRequest
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/discovery/v1/discovery_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery.v1 import (
-    discovery_service_pb2 as ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2,
-)
+from ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery.v1 import discovery_service_pb2 as ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2
 
 
 class DiscoveryServiceStub(object):
     """The service used as a registry for other services. This service can be used to discover
     and activate other services present in the system.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.RegisterService = channel.unary_unary(
-            "/ni.measurementlink.discovery.v1.DiscoveryService/RegisterService",
-            request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceResponse.FromString,
-        )
+                '/ni.measurementlink.discovery.v1.DiscoveryService/RegisterService',
+                request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceResponse.FromString,
+                )
         self.UnregisterService = channel.unary_unary(
-            "/ni.measurementlink.discovery.v1.DiscoveryService/UnregisterService",
-            request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceResponse.FromString,
-        )
+                '/ni.measurementlink.discovery.v1.DiscoveryService/UnregisterService',
+                request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceResponse.FromString,
+                )
         self.EnumerateServices = channel.unary_unary(
-            "/ni.measurementlink.discovery.v1.DiscoveryService/EnumerateServices",
-            request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesResponse.FromString,
-        )
+                '/ni.measurementlink.discovery.v1.DiscoveryService/EnumerateServices',
+                request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesResponse.FromString,
+                )
         self.ResolveService = channel.unary_unary(
-            "/ni.measurementlink.discovery.v1.DiscoveryService/ResolveService",
-            request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ResolveServiceRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ServiceLocation.FromString,
-        )
+                '/ni.measurementlink.discovery.v1.DiscoveryService/ResolveService',
+                request_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ResolveServiceRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ServiceLocation.FromString,
+                )
 
 
 class DiscoveryServiceServicer(object):
     """The service used as a registry for other services. This service can be used to discover
     and activate other services present in the system.
     """
 
@@ -53,191 +51,143 @@
         - ServiceDescriptor.provided_interfaces is empty
         - ServiceDescriptor.service_class is empty
         - ServiceLocation.location is empty
         - Both ServiceLocation.insecure_port and ServiceLocation.ssl_authenticated_port are empty
         - Either ServiceLocation.insecure_port or ServiceLocation.ssl_authenticated_port contain an invalid port number
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def UnregisterService(self, request, context):
-        """Unregisters a service instance with the discovery service."""
+        """Unregisters a service instance with the discovery service.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def EnumerateServices(self, request, context):
         """Enumerate all services which implement a specific service interface.
         This is useful for plugin type systems where the possible services are not known ahead of time.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ResolveService(self, request, context):
         """Given a description of a service, returns information that can be used to establish communication
         with that service. If necessary, the service will be started by the discovery service if it has not
         already been started. Activation of the service is accomplished through use of a .serviceconfig file
         which includes information describing the service. Services that register a .serviceconfig file must
         call RegisterService when their service is started or this call will never complete successfully when
         the discovery service attempts to start it.
         Status Codes for errors:
         - INVALID_ARGUMENT: provided_interfaces is empty
         - NOT_FOUND: No service matching the resolve request was found
         - FAILED_PRECONDITION: More than one service matching the resolve request was found
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_DiscoveryServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "RegisterService": grpc.unary_unary_rpc_method_handler(
-            servicer.RegisterService,
-            request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceResponse.SerializeToString,
-        ),
-        "UnregisterService": grpc.unary_unary_rpc_method_handler(
-            servicer.UnregisterService,
-            request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceResponse.SerializeToString,
-        ),
-        "EnumerateServices": grpc.unary_unary_rpc_method_handler(
-            servicer.EnumerateServices,
-            request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesResponse.SerializeToString,
-        ),
-        "ResolveService": grpc.unary_unary_rpc_method_handler(
-            servicer.ResolveService,
-            request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ResolveServiceRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ServiceLocation.SerializeToString,
-        ),
+            'RegisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterService,
+                    request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceResponse.SerializeToString,
+            ),
+            'UnregisterService': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterService,
+                    request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceResponse.SerializeToString,
+            ),
+            'EnumerateServices': grpc.unary_unary_rpc_method_handler(
+                    servicer.EnumerateServices,
+                    request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesResponse.SerializeToString,
+            ),
+            'ResolveService': grpc.unary_unary_rpc_method_handler(
+                    servicer.ResolveService,
+                    request_deserializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ResolveServiceRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ServiceLocation.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "ni.measurementlink.discovery.v1.DiscoveryService", rpc_method_handlers
-    )
+            'ni.measurementlink.discovery.v1.DiscoveryService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class DiscoveryService(object):
     """The service used as a registry for other services. This service can be used to discover
     and activate other services present in the system.
     """
 
     @staticmethod
-    def RegisterService(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def RegisterService(request,
             target,
-            "/ni.measurementlink.discovery.v1.DiscoveryService/RegisterService",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.discovery.v1.DiscoveryService/RegisterService',
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceRequest.SerializeToString,
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.RegisterServiceResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UnregisterService(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def UnregisterService(request,
             target,
-            "/ni.measurementlink.discovery.v1.DiscoveryService/UnregisterService",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.discovery.v1.DiscoveryService/UnregisterService',
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceRequest.SerializeToString,
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.UnregisterServiceResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def EnumerateServices(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def EnumerateServices(request,
             target,
-            "/ni.measurementlink.discovery.v1.DiscoveryService/EnumerateServices",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.discovery.v1.DiscoveryService/EnumerateServices',
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesRequest.SerializeToString,
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.EnumerateServicesResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ResolveService(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def ResolveService(request,
             target,
-            "/ni.measurementlink.discovery.v1.DiscoveryService/ResolveService",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.discovery.v1.DiscoveryService/ResolveService',
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ResolveServiceRequest.SerializeToString,
             ni_dot_measurementlink_dot_discovery_dot_v1_dot_discovery__service__pb2.ServiceLocation.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: ni/measurementlink/measurement/v1/measurement_service.proto
+# source: ni/measurementlink/measurement/v2/measurement_service.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import type_pb2 as google_dot_protobuf_dot_type__pb2
-from ni_measurementlink_service._internal.stubs.ni.measurementlink import (
-    pin_map_context_pb2 as ni_dot_measurementlink_dot_pin__map__context__pb2,
-)
+from ni_measurementlink_service._internal.stubs.ni.measurementlink import pin_map_context_pb2 as ni_dot_measurementlink_dot_pin__map__context__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n;ni/measurementlink/measurement/v1/measurement_service.proto\x12!ni.measurementlink.measurement.v1\x1a\x19google/protobuf/any.proto\x1a\x1agoogle/protobuf/type.proto\x1a(ni/measurementlink/pin_map_context.proto"\x14\n\x12GetMetadataRequest"\x9a\x02\n\x13GetMetadataResponse\x12R\n\x13measurement_details\x18\x01 \x01(\x0b\x32\x35.ni.measurementlink.measurement.v1.MeasurementDetails\x12V\n\x15measurement_signature\x18\x02 \x01(\x0b\x32\x37.ni.measurementlink.measurement.v1.MeasurementSignature\x12W\n\x16user_interface_details\x18\x03 \x03(\x0b\x32\x37.ni.measurementlink.measurement.v1.UserInterfaceDetails"\x84\x01\n\x0eMeasureRequest\x12\x36\n\x18\x63onfiguration_parameters\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12:\n\x0fpin_map_context\x18\x02 \x01(\x0b\x32!.ni.measurementlink.PinMapContext"8\n\x0fMeasureResponse\x12%\n\x07outputs\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any";\n\x12MeasurementDetails\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t"\xb2\x02\n\x14MeasurementSignature\x12-\n%configuration_parameters_message_type\x18\x01 \x01(\t\x12[\n\x18\x63onfiguration_parameters\x18\x02 \x03(\x0b\x32\x39.ni.measurementlink.measurement.v1.ConfigurationParameter\x12\x34\n\x16\x63onfiguration_defaults\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x1c\n\x14outputs_message_type\x18\x04 \x01(\t\x12:\n\x07outputs\x18\x05 \x03(\x0b\x32).ni.measurementlink.measurement.v1.Output"(\n\x14UserInterfaceDetails\x12\x10\n\x08\x66ile_url\x18\x01 \x01(\t"\x8e\x02\n\x16\x43onfigurationParameter\x12\x14\n\x0c\x66ield_number\x18\x01 \x01(\x05\x12)\n\x04type\x18\x02 \x01(\x0e\x32\x1b.google.protobuf.Field.Kind\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08repeated\x18\x04 \x01(\x08\x12_\n\x0b\x61nnotations\x18\x05 \x03(\x0b\x32J.ni.measurementlink.measurement.v1.ConfigurationParameter.AnnotationsEntry\x1a\x32\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01"i\n\x06Output\x12\x14\n\x0c\x66ield_number\x18\x01 \x01(\x05\x12)\n\x04type\x18\x02 \x01(\x0e\x32\x1b.google.protobuf.Field.Kind\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08repeated\x18\x04 \x01(\x08\x32\x84\x02\n\x12MeasurementService\x12|\n\x0bGetMetadata\x12\x35.ni.measurementlink.measurement.v1.GetMetadataRequest\x1a\x36.ni.measurementlink.measurement.v1.GetMetadataResponse\x12p\n\x07Measure\x12\x31.ni.measurementlink.measurement.v1.MeasureRequest\x1a\x32.ni.measurementlink.measurement.v1.MeasureResponseB\xd8\x01\n%com.ni.measurementlink.measurement.v1B\x17MeasurementServiceProtoP\x01Z\rmeasurementv1\xa2\x02\x04NIMM\xaa\x02\x32NationalInstruments.MeasurementLink.Measurement.V1\xca\x02!NI\\MeasurementLink\\Measurement\\V1\xea\x02$NI::MeasurementLink::Measurement::V1b\x06proto3'
-)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;ni/measurementlink/measurement/v2/measurement_service.proto\x12!ni.measurementlink.measurement.v2\x1a\x19google/protobuf/any.proto\x1a\x1agoogle/protobuf/type.proto\x1a(ni/measurementlink/pin_map_context.proto\"\x14\n\x12GetMetadataRequest\"\x9a\x02\n\x13GetMetadataResponse\x12R\n\x13measurement_details\x18\x01 \x01(\x0b\x32\x35.ni.measurementlink.measurement.v2.MeasurementDetails\x12V\n\x15measurement_signature\x18\x02 \x01(\x0b\x32\x37.ni.measurementlink.measurement.v2.MeasurementSignature\x12W\n\x16user_interface_details\x18\x03 \x03(\x0b\x32\x37.ni.measurementlink.measurement.v2.UserInterfaceDetails\"\x84\x01\n\x0eMeasureRequest\x12\x36\n\x18\x63onfiguration_parameters\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12:\n\x0fpin_map_context\x18\x02 \x01(\x0b\x32!.ni.measurementlink.PinMapContext\"8\n\x0fMeasureResponse\x12%\n\x07outputs\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\";\n\x12MeasurementDetails\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\xb2\x02\n\x14MeasurementSignature\x12-\n%configuration_parameters_message_type\x18\x01 \x01(\t\x12[\n\x18\x63onfiguration_parameters\x18\x02 \x03(\x0b\x32\x39.ni.measurementlink.measurement.v2.ConfigurationParameter\x12\x34\n\x16\x63onfiguration_defaults\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x1c\n\x14outputs_message_type\x18\x04 \x01(\t\x12:\n\x07outputs\x18\x05 \x03(\x0b\x32).ni.measurementlink.measurement.v2.Output\"(\n\x14UserInterfaceDetails\x12\x10\n\x08\x66ile_url\x18\x01 \x01(\t\"\x8e\x02\n\x16\x43onfigurationParameter\x12\x14\n\x0c\x66ield_number\x18\x01 \x01(\x05\x12)\n\x04type\x18\x02 \x01(\x0e\x32\x1b.google.protobuf.Field.Kind\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08repeated\x18\x04 \x01(\x08\x12_\n\x0b\x61nnotations\x18\x05 \x03(\x0b\x32J.ni.measurementlink.measurement.v2.ConfigurationParameter.AnnotationsEntry\x1a\x32\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xee\x01\n\x06Output\x12\x14\n\x0c\x66ield_number\x18\x01 \x01(\x05\x12)\n\x04type\x18\x02 \x01(\x0e\x32\x1b.google.protobuf.Field.Kind\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x10\n\x08repeated\x18\x04 \x01(\x08\x12O\n\x0b\x61nnotations\x18\x05 \x03(\x0b\x32:.ni.measurementlink.measurement.v2.Output.AnnotationsEntry\x1a\x32\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x32\x86\x02\n\x12MeasurementService\x12|\n\x0bGetMetadata\x12\x35.ni.measurementlink.measurement.v2.GetMetadataRequest\x1a\x36.ni.measurementlink.measurement.v2.GetMetadataResponse\x12r\n\x07Measure\x12\x31.ni.measurementlink.measurement.v2.MeasureRequest\x1a\x32.ni.measurementlink.measurement.v2.MeasureResponse0\x01\x42\xd8\x01\n%com.ni.measurementlink.measurement.v2B\x17MeasurementServiceProtoP\x01Z\rmeasurementv2\xa2\x02\x04NIMM\xaa\x02\x32NationalInstruments.MeasurementLink.Measurement.V2\xca\x02!NI\\MeasurementLink\\Measurement\\V2\xea\x02$NI::MeasurementLink::Measurement::V2b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "ni.measurementlink.measurement.v1.measurement_service_pb2", globals()
-)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ni.measurementlink.measurement.v2.measurement_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"\n%com.ni.measurementlink.measurement.v1B\027MeasurementServiceProtoP\001Z\rmeasurementv1\242\002\004NIMM\252\0022NationalInstruments.MeasurementLink.Measurement.V1\312\002!NI\\MeasurementLink\\Measurement\\V1\352\002$NI::MeasurementLink::Measurement::V1"
-    _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._options = None
-    _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._serialized_options = b"8\001"
-    _GETMETADATAREQUEST._serialized_start = 195
-    _GETMETADATAREQUEST._serialized_end = 215
-    _GETMETADATARESPONSE._serialized_start = 218
-    _GETMETADATARESPONSE._serialized_end = 500
-    _MEASUREREQUEST._serialized_start = 503
-    _MEASUREREQUEST._serialized_end = 635
-    _MEASURERESPONSE._serialized_start = 637
-    _MEASURERESPONSE._serialized_end = 693
-    _MEASUREMENTDETAILS._serialized_start = 695
-    _MEASUREMENTDETAILS._serialized_end = 754
-    _MEASUREMENTSIGNATURE._serialized_start = 757
-    _MEASUREMENTSIGNATURE._serialized_end = 1063
-    _USERINTERFACEDETAILS._serialized_start = 1065
-    _USERINTERFACEDETAILS._serialized_end = 1105
-    _CONFIGURATIONPARAMETER._serialized_start = 1108
-    _CONFIGURATIONPARAMETER._serialized_end = 1378
-    _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._serialized_start = 1328
-    _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._serialized_end = 1378
-    _OUTPUT._serialized_start = 1380
-    _OUTPUT._serialized_end = 1485
-    _MEASUREMENTSERVICE._serialized_start = 1488
-    _MEASUREMENTSERVICE._serialized_end = 1748
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n%com.ni.measurementlink.measurement.v2B\027MeasurementServiceProtoP\001Z\rmeasurementv2\242\002\004NIMM\252\0022NationalInstruments.MeasurementLink.Measurement.V2\312\002!NI\\MeasurementLink\\Measurement\\V2\352\002$NI::MeasurementLink::Measurement::V2'
+  _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._options = None
+  _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._serialized_options = b'8\001'
+  _OUTPUT_ANNOTATIONSENTRY._options = None
+  _OUTPUT_ANNOTATIONSENTRY._serialized_options = b'8\001'
+  _GETMETADATAREQUEST._serialized_start=195
+  _GETMETADATAREQUEST._serialized_end=215
+  _GETMETADATARESPONSE._serialized_start=218
+  _GETMETADATARESPONSE._serialized_end=500
+  _MEASUREREQUEST._serialized_start=503
+  _MEASUREREQUEST._serialized_end=635
+  _MEASURERESPONSE._serialized_start=637
+  _MEASURERESPONSE._serialized_end=693
+  _MEASUREMENTDETAILS._serialized_start=695
+  _MEASUREMENTDETAILS._serialized_end=754
+  _MEASUREMENTSIGNATURE._serialized_start=757
+  _MEASUREMENTSIGNATURE._serialized_end=1063
+  _USERINTERFACEDETAILS._serialized_start=1065
+  _USERINTERFACEDETAILS._serialized_end=1105
+  _CONFIGURATIONPARAMETER._serialized_start=1108
+  _CONFIGURATIONPARAMETER._serialized_end=1378
+  _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._serialized_start=1328
+  _CONFIGURATIONPARAMETER_ANNOTATIONSENTRY._serialized_end=1378
+  _OUTPUT._serialized_start=1381
+  _OUTPUT._serialized_end=1619
+  _OUTPUT_ANNOTATIONSENTRY._serialized_start=1328
+  _OUTPUT_ANNOTATIONSENTRY._serialized_end=1378
+  _MEASUREMENTSERVICE._serialized_start=1622
+  _MEASUREMENTSERVICE._serialized_end=1884
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -41,48 +41,25 @@
     @property
     def measurement_details(self) -> global___MeasurementDetails:
         """Required. Specifies basic information about the measurement."""
     @property
     def measurement_signature(self) -> global___MeasurementSignature:
         """Required. Specifies the signature of the measurement."""
     @property
-    def user_interface_details(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___UserInterfaceDetails
-    ]:
+    def user_interface_details(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UserInterfaceDetails]:
         """Optional. Specifies the user interfaces available for use with the measurement, if any."""
     def __init__(
         self,
         *,
         measurement_details: global___MeasurementDetails | None = ...,
         measurement_signature: global___MeasurementSignature | None = ...,
-        user_interface_details: collections.abc.Iterable[global___UserInterfaceDetails]
-        | None = ...,
-    ) -> None: ...
-    def HasField(
-        self,
-        field_name: typing_extensions.Literal[
-            "measurement_details",
-            b"measurement_details",
-            "measurement_signature",
-            b"measurement_signature",
-        ],
-    ) -> builtins.bool: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "measurement_details",
-            b"measurement_details",
-            "measurement_signature",
-            b"measurement_signature",
-            "user_interface_details",
-            b"user_interface_details",
-        ],
+        user_interface_details: collections.abc.Iterable[global___UserInterfaceDetails] | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["measurement_details", b"measurement_details", "measurement_signature", b"measurement_signature", "user_interface_details", b"user_interface_details"]) -> None: ...
 
 global___GetMetadataResponse = GetMetadataResponse
 
 @typing_extensions.final
 class MeasureRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -102,32 +79,16 @@
         """
     def __init__(
         self,
         *,
         configuration_parameters: google.protobuf.any_pb2.Any | None = ...,
         pin_map_context: ni.measurementlink.pin_map_context_pb2.PinMapContext | None = ...,
     ) -> None: ...
-    def HasField(
-        self,
-        field_name: typing_extensions.Literal[
-            "configuration_parameters",
-            b"configuration_parameters",
-            "pin_map_context",
-            b"pin_map_context",
-        ],
-    ) -> builtins.bool: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "configuration_parameters",
-            b"configuration_parameters",
-            "pin_map_context",
-            b"pin_map_context",
-        ],
-    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["configuration_parameters", b"configuration_parameters", "pin_map_context", b"pin_map_context"]) -> None: ...
 
 global___MeasureRequest = MeasureRequest
 
 @typing_extensions.final
 class MeasureResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -139,17 +100,15 @@
         which of its output fields are required and which are optional based on the configuration for the measurement.
         """
     def __init__(
         self,
         *,
         outputs: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
-    def HasField(
-        self, field_name: typing_extensions.Literal["outputs", b"outputs"]
-    ) -> builtins.bool: ...
+    def HasField(self, field_name: typing_extensions.Literal["outputs", b"outputs"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["outputs", b"outputs"]) -> None: ...
 
 global___MeasureResponse = MeasureResponse
 
 @typing_extensions.final
 class MeasurementDetails(google.protobuf.message.Message):
     """Message that contains standard information reported by a measurement."""
@@ -164,20 +123,15 @@
     """Optional. The current version of the measurement."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         version: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "display_name", b"display_name", "version", b"version"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "version", b"version"]) -> None: ...
 
 global___MeasurementDetails = MeasurementDetails
 
 @typing_extensions.final
 class MeasurementSignature(google.protobuf.message.Message):
     """Message that defines the signature of a measurement."""
 
@@ -189,64 +143,40 @@
     OUTPUTS_MESSAGE_TYPE_FIELD_NUMBER: builtins.int
     OUTPUTS_FIELD_NUMBER: builtins.int
     configuration_parameters_message_type: builtins.str
     """Required. The type name of the message used to define the measurement's configuration.
     This is the gRPC full name for the message.
     """
     @property
-    def configuration_parameters(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___ConfigurationParameter
-    ]:
+    def configuration_parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ConfigurationParameter]:
         """Required. Defines the configuration parameters for the measurement."""
     @property
     def configuration_defaults(self) -> google.protobuf.any_pb2.Any:
         """Optional. The default values to use for the configuration parameters. Caller can use these default values
         rather than specifying their own. These values should be supplied using the message type defined by
         configuration_parameters_message_type.
         """
     outputs_message_type: builtins.str
     """Required. The type name of the message used to define the measurement's outputs.
     This is the gRPC full name for the message.
     """
     @property
-    def outputs(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Output]:
+    def outputs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Output]:
         """Required. Defines the outputs for the measurement."""
     def __init__(
         self,
         *,
         configuration_parameters_message_type: builtins.str = ...,
-        configuration_parameters: collections.abc.Iterable[global___ConfigurationParameter]
-        | None = ...,
+        configuration_parameters: collections.abc.Iterable[global___ConfigurationParameter] | None = ...,
         configuration_defaults: google.protobuf.any_pb2.Any | None = ...,
         outputs_message_type: builtins.str = ...,
         outputs: collections.abc.Iterable[global___Output] | None = ...,
     ) -> None: ...
-    def HasField(
-        self,
-        field_name: typing_extensions.Literal["configuration_defaults", b"configuration_defaults"],
-    ) -> builtins.bool: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "configuration_defaults",
-            b"configuration_defaults",
-            "configuration_parameters",
-            b"configuration_parameters",
-            "configuration_parameters_message_type",
-            b"configuration_parameters_message_type",
-            "outputs",
-            b"outputs",
-            "outputs_message_type",
-            b"outputs_message_type",
-        ],
-    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["configuration_defaults", b"configuration_defaults"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["configuration_defaults", b"configuration_defaults", "configuration_parameters", b"configuration_parameters", "configuration_parameters_message_type", b"configuration_parameters_message_type", "outputs", b"outputs", "outputs_message_type", b"outputs_message_type"]) -> None: ...
 
 global___MeasurementSignature = MeasurementSignature
 
 @typing_extensions.final
 class UserInterfaceDetails(google.protobuf.message.Message):
     """Contains measurement User Interface details."""
 
@@ -256,17 +186,15 @@
     file_url: builtins.str
     """Optional. The URL to the file (such as .measui or .vi) providing a user interface for the measurement."""
     def __init__(
         self,
         *,
         file_url: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["file_url", b"file_url"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["file_url", b"file_url"]) -> None: ...
 
 global___UserInterfaceDetails = UserInterfaceDetails
 
 @typing_extensions.final
 class ConfigurationParameter(google.protobuf.message.Message):
     """Message that defines a configuration parameter for the measurement."""
 
@@ -282,17 +210,15 @@
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
-        def ClearField(
-            self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]
-        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELD_NUMBER_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     REPEATED_FIELD_NUMBER: builtins.int
     ANNOTATIONS_FIELD_NUMBER: builtins.int
     field_number: builtins.int
@@ -304,91 +230,92 @@
     name: builtins.str
     """Required. The name of the configuration parameter. When defining a user interface for the measurement, a control
     that matches this name will be used to supply a value to this configuration parameter.
     """
     repeated: builtins.bool
     """Required. True if this configuration parameter represents repeated data and False if it represents a scalar value."""
     @property
-    def annotations(
-        self,
-    ) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
+    def annotations(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Optional. Represents a set of annotations on the type.
         Well-known annotations:
         - Type specialization. The keys to other annotations will be read based on the value of `ni/type_specialization` annotation.
           - Key: "ni/type_specialization"
-          - Common Values: "pin" ...
+          - Common Values: "pin", "path", "enum", ...
+          - "pin" and "path" parameters require the type field to be TYPE_STRING.
+          - "enum" parameters requires the type field to be TYPE_ENUM.
         - For string parameter with ni/type_specialization annotation equals "pin"
           - Key: "ni/pin.instrument_type"
           - Common Values: "niDCPower", "niScope"...
+        - For enum parameter with ni/type_specialization annotation equals "enum"
+          - Key: "ni/enum.values"
+          - Expected format: JSON dictionary string"
+          - Example: "{\\"RED\\":0, \\"GREEN\\":25, \\"BLUE\\":5}"
         """
     def __init__(
         self,
         *,
         field_number: builtins.int = ...,
         type: google.protobuf.type_pb2.Field.Kind.ValueType = ...,
         name: builtins.str = ...,
         repeated: builtins.bool = ...,
         annotations: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "annotations",
-            b"annotations",
-            "field_number",
-            b"field_number",
-            "name",
-            b"name",
-            "repeated",
-            b"repeated",
-            "type",
-            b"type",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["annotations", b"annotations", "field_number", b"field_number", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
 
 global___ConfigurationParameter = ConfigurationParameter
 
 @typing_extensions.final
 class Output(google.protobuf.message.Message):
     """Message that defines an output of the measurement."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
+    class AnnotationsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
     FIELD_NUMBER_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     REPEATED_FIELD_NUMBER: builtins.int
+    ANNOTATIONS_FIELD_NUMBER: builtins.int
     field_number: builtins.int
     """Required. The field number for the output as defined by the message indicated by
     MethodSignature.outputs_message_type.
     """
     type: google.protobuf.type_pb2.Field.Kind.ValueType
     """Required. The data type for the output."""
     name: builtins.str
     """Required. The name of the output. When defining a user interface for the measurement, an indicator
     that matches this name will be used to display the value for this output.
     """
     repeated: builtins.bool
     """Required. True if this output represents repeated data and False if it represents a scalar value."""
+    @property
+    def annotations(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
+        """Optional. Represents a set of annotations on the type.
+        See documentation for ConfigurationParameter annotations for more details and examples.
+        """
     def __init__(
         self,
         *,
         field_number: builtins.int = ...,
         type: google.protobuf.type_pb2.Field.Kind.ValueType = ...,
         name: builtins.str = ...,
         repeated: builtins.bool = ...,
+        annotations: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "field_number",
-            b"field_number",
-            "name",
-            b"name",
-            "repeated",
-            b"repeated",
-            "type",
-            b"type",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["annotations", b"annotations", "field_number", b"field_number", "name", b"name", "repeated", b"repeated", "type", b"type"]) -> None: ...
 
 global___Output = Output
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v1/measurement_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/measurement/v2/measurement_service_pb2_grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,132 +1,107 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v1 import (
-    measurement_service_pb2 as ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2,
-)
+from ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v2 import measurement_service_pb2 as ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2
 
 
 class MeasurementServiceStub(object):
     """Service that implements a measurement. Unlike other services, a MeasurementService is designed to be a plugin
     where there can be multiple implementations of the service that provide different measurement capabilities.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetMetadata = channel.unary_unary(
-            "/ni.measurementlink.measurement.v1.MeasurementService/GetMetadata",
-            request_serializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.GetMetadataRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.GetMetadataResponse.FromString,
-        )
-        self.Measure = channel.unary_unary(
-            "/ni.measurementlink.measurement.v1.MeasurementService/Measure",
-            request_serializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.MeasureRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.MeasureResponse.FromString,
-        )
+                '/ni.measurementlink.measurement.v2.MeasurementService/GetMetadata',
+                request_serializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.GetMetadataRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.GetMetadataResponse.FromString,
+                )
+        self.Measure = channel.unary_stream(
+                '/ni.measurementlink.measurement.v2.MeasurementService/Measure',
+                request_serializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.MeasureRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.MeasureResponse.FromString,
+                )
 
 
 class MeasurementServiceServicer(object):
     """Service that implements a measurement. Unlike other services, a MeasurementService is designed to be a plugin
     where there can be multiple implementations of the service that provide different measurement capabilities.
     """
 
     def GetMetadata(self, request, context):
-        """Returns information that describes the measurement."""
+        """Returns information that describes the measurement.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def Measure(self, request, context):
-        """API used to perform a measurement."""
+        """API used to perform a measurement.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_MeasurementServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "GetMetadata": grpc.unary_unary_rpc_method_handler(
-            servicer.GetMetadata,
-            request_deserializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.GetMetadataRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.GetMetadataResponse.SerializeToString,
-        ),
-        "Measure": grpc.unary_unary_rpc_method_handler(
-            servicer.Measure,
-            request_deserializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.MeasureRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.MeasureResponse.SerializeToString,
-        ),
+            'GetMetadata': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetMetadata,
+                    request_deserializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.GetMetadataRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.GetMetadataResponse.SerializeToString,
+            ),
+            'Measure': grpc.unary_stream_rpc_method_handler(
+                    servicer.Measure,
+                    request_deserializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.MeasureRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.MeasureResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "ni.measurementlink.measurement.v1.MeasurementService", rpc_method_handlers
-    )
+            'ni.measurementlink.measurement.v2.MeasurementService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class MeasurementService(object):
     """Service that implements a measurement. Unlike other services, a MeasurementService is designed to be a plugin
     where there can be multiple implementations of the service that provide different measurement capabilities.
     """
 
     @staticmethod
-    def GetMetadata(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def GetMetadata(request,
             target,
-            "/ni.measurementlink.measurement.v1.MeasurementService/GetMetadata",
-            ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.GetMetadataRequest.SerializeToString,
-            ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.GetMetadataResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.measurement.v2.MeasurementService/GetMetadata',
+            ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.GetMetadataRequest.SerializeToString,
+            ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.GetMetadataResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Measure(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def Measure(request,
             target,
-            "/ni.measurementlink.measurement.v1.MeasurementService/Measure",
-            ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.MeasureRequest.SerializeToString,
-            ni_dot_measurementlink_dot_measurement_dot_v1_dot_measurement__service__pb2.MeasureResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/ni.measurementlink.measurement.v2.MeasurementService/Measure',
+            ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.MeasureRequest.SerializeToString,
+            ni_dot_measurementlink_dot_measurement_dot_v2_dot_measurement__service__pb2.MeasureResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,25 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ni/measurementlink/pin_map_context.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n(ni/measurementlink/pin_map_context.proto\x12\x12ni.measurementlink"2\n\rPinMapContext\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x03(\x05\x42\x96\x01\n\x16\x63om.ni.measurementlinkB\x12PinMapContextProtoP\x01Z\x0fpinmapcontextv1\xa2\x02\x03NIM\xaa\x02#NationalInstruments.MeasurementLink\xca\x02\x12NI\\MeasurementLink\xea\x02\x13NI::MeasurementLinkb\x06proto3'
-)
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(ni/measurementlink/pin_map_context.proto\x12\x12ni.measurementlink\"2\n\rPinMapContext\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x03(\x05\x42\x96\x01\n\x16\x63om.ni.measurementlinkB\x12PinMapContextProtoP\x01Z\x0fpinmapcontextv1\xa2\x02\x03NIM\xaa\x02#NationalInstruments.MeasurementLink\xca\x02\x12NI\\MeasurementLink\xea\x02\x13NI::MeasurementLinkb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "ni.measurementlink.pin_map_context_pb2", globals()
-)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ni.measurementlink.pin_map_context_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"\n\026com.ni.measurementlinkB\022PinMapContextProtoP\001Z\017pinmapcontextv1\242\002\003NIM\252\002#NationalInstruments.MeasurementLink\312\002\022NI\\MeasurementLink\352\002\023NI::MeasurementLink"
-    _PINMAPCONTEXT._serialized_start = 64
-    _PINMAPCONTEXT._serialized_end = 114
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\026com.ni.measurementlinkB\022PinMapContextProtoP\001Z\017pinmapcontextv1\242\002\003NIM\252\002#NationalInstruments.MeasurementLink\312\002\022NI\\MeasurementLink\352\002\023NI::MeasurementLink'
+  _PINMAPCONTEXT._serialized_start=64
+  _PINMAPCONTEXT._serialized_end=114
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pin_map_context_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,18 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     SITES_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the pin map in the Pin Map service that should be used for the call."""
     @property
-    def sites(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+    def sites(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Optional. List of site numbers being used for the call. If unspecified, use all sites in the pin map."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         sites: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id", "sites", b"sites"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id", "sites", b"sites"]) -> None: ...
 
 global___PinMapContext = PinMapContext
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,60 +2,57 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ni/measurementlink/pinmap/v1/pin_map_service.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n2ni/measurementlink/pinmap/v1/pin_map_service.proto\x12\x1cni.measurementlink.pinmap.v1"\x1c\n\x06PinMap\x12\x12\n\npin_map_id\x18\x01 \x01(\t"E\n\x1a\x43reatePinMapFromXmlRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\x13\n\x0bpin_map_xml\x18\x02 \x01(\t"E\n\x1aUpdatePinMapFromXmlRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\x13\n\x0bpin_map_xml\x18\x02 \x01(\t"&\n\x10GetPinMapRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t"B\n\x10QueryPinsRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\x1a\n\x12instrument_type_id\x18\x02 \x01(\t"\x94\x01\n\x11QueryPinsResponse\x12\x39\n\x04pins\x18\x01 \x03(\x0b\x32+.ni.measurementlink.pinmap.v1.PinDefinition\x12\x44\n\npin_groups\x18\x02 \x03(\x0b\x32\x30.ni.measurementlink.pinmap.v1.PinGroupDefinition"<\n\rPinDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x15\n\ris_system_pin\x18\x02 \x01(\x08"b\n\x12PinGroupDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x1f\n\x17pin_or_group_references\x18\x02 \x03(\t\x12\x15\n\rresolved_pins\x18\x03 \x03(\t"(\n\x12QueryRelaysRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t"\x9e\x01\n\x13QueryRelaysResponse\x12=\n\x06relays\x18\x01 \x03(\x0b\x32-.ni.measurementlink.pinmap.v1.RelayDefinition\x12H\n\x0crelay_groups\x18\x02 \x03(\x0b\x32\x32.ni.measurementlink.pinmap.v1.RelayGroupDefinition"@\n\x0fRelayDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x17\n\x0fis_system_relay\x18\x02 \x01(\x08"h\n\x14RelayGroupDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12!\n\x19relay_or_group_references\x18\x02 \x03(\t\x12\x17\n\x0fresolved_relays\x18\x03 \x03(\t"\x82\x01\n%QueryResourceAccessInformationRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x03(\x05\x12\x1a\n\x12pin_or_relay_names\x18\x03 \x03(\t\x12\x1a\n\x12instrument_type_id\x18\x04 \x01(\t"\x86\x01\n&QueryResourceAccessInformationResponse\x12\\\n\x1bresource_access_information\x18\x01 \x03(\x0b\x32\x37.ni.measurementlink.pinmap.v1.ResourceAccessInformation"\xac\x01\n\x19ResourceAccessInformation\x12\x15\n\rresource_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x1a\n\x12instrument_type_id\x18\x03 \x01(\t\x12\x46\n\x10\x63hannel_mappings\x18\x04 \x03(\x0b\x32,.ni.measurementlink.pinmap.v1.ChannelMapping"J\n\x0e\x43hannelMapping\x12\x19\n\x11pin_or_relay_name\x18\x01 \x01(\t\x12\x0c\n\x04site\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\t2\xf0\x05\n\rPinMapService\x12u\n\x13\x43reatePinMapFromXml\x12\x38.ni.measurementlink.pinmap.v1.CreatePinMapFromXmlRequest\x1a$.ni.measurementlink.pinmap.v1.PinMap\x12u\n\x13UpdatePinMapFromXml\x12\x38.ni.measurementlink.pinmap.v1.UpdatePinMapFromXmlRequest\x1a$.ni.measurementlink.pinmap.v1.PinMap\x12\x61\n\tGetPinMap\x12..ni.measurementlink.pinmap.v1.GetPinMapRequest\x1a$.ni.measurementlink.pinmap.v1.PinMap\x12l\n\tQueryPins\x12..ni.measurementlink.pinmap.v1.QueryPinsRequest\x1a/.ni.measurementlink.pinmap.v1.QueryPinsResponse\x12r\n\x0bQueryRelays\x12\x30.ni.measurementlink.pinmap.v1.QueryRelaysRequest\x1a\x31.ni.measurementlink.pinmap.v1.QueryRelaysResponse\x12\xab\x01\n\x1eQueryResourceAccessInformation\x12\x43.ni.measurementlink.pinmap.v1.QueryResourceAccessInformationRequest\x1a\x44.ni.measurementlink.pinmap.v1.QueryResourceAccessInformationResponseB\xba\x01\n com.ni.measurementlink.pinmap.v1B\x12PinMapServiceProtoP\x01Z\x08pinmapv1\xa2\x02\x04NIMP\xaa\x02-NationalInstruments.MeasurementLink.PinMap.V1\xca\x02\x1cNI\\MeasurementLink\\PinMap\\V1\xea\x02\x1fNI::MeasurementLink::PinMap::V1b\x06proto3'
-)
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2ni/measurementlink/pinmap/v1/pin_map_service.proto\x12\x1cni.measurementlink.pinmap.v1\"\x1c\n\x06PinMap\x12\x12\n\npin_map_id\x18\x01 \x01(\t\"E\n\x1a\x43reatePinMapFromXmlRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\x13\n\x0bpin_map_xml\x18\x02 \x01(\t\"E\n\x1aUpdatePinMapFromXmlRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\x13\n\x0bpin_map_xml\x18\x02 \x01(\t\"&\n\x10GetPinMapRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\"B\n\x10QueryPinsRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\x1a\n\x12instrument_type_id\x18\x02 \x01(\t\"\x94\x01\n\x11QueryPinsResponse\x12\x39\n\x04pins\x18\x01 \x03(\x0b\x32+.ni.measurementlink.pinmap.v1.PinDefinition\x12\x44\n\npin_groups\x18\x02 \x03(\x0b\x32\x30.ni.measurementlink.pinmap.v1.PinGroupDefinition\"<\n\rPinDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x15\n\ris_system_pin\x18\x02 \x01(\x08\"b\n\x12PinGroupDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x1f\n\x17pin_or_group_references\x18\x02 \x03(\t\x12\x15\n\rresolved_pins\x18\x03 \x03(\t\"(\n\x12QueryRelaysRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\"\x9e\x01\n\x13QueryRelaysResponse\x12=\n\x06relays\x18\x01 \x03(\x0b\x32-.ni.measurementlink.pinmap.v1.RelayDefinition\x12H\n\x0crelay_groups\x18\x02 \x03(\x0b\x32\x32.ni.measurementlink.pinmap.v1.RelayGroupDefinition\"@\n\x0fRelayDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x17\n\x0fis_system_relay\x18\x02 \x01(\x08\"h\n\x14RelayGroupDefinition\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12!\n\x19relay_or_group_references\x18\x02 \x03(\t\x12\x17\n\x0fresolved_relays\x18\x03 \x03(\t\"\x82\x01\n%QueryResourceAccessInformationRequest\x12\x12\n\npin_map_id\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x03(\x05\x12\x1a\n\x12pin_or_relay_names\x18\x03 \x03(\t\x12\x1a\n\x12instrument_type_id\x18\x04 \x01(\t\"\x86\x01\n&QueryResourceAccessInformationResponse\x12\\\n\x1bresource_access_information\x18\x01 \x03(\x0b\x32\x37.ni.measurementlink.pinmap.v1.ResourceAccessInformation\"\xac\x01\n\x19ResourceAccessInformation\x12\x15\n\rresource_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63hannel_list\x18\x02 \x01(\t\x12\x1a\n\x12instrument_type_id\x18\x03 \x01(\t\x12\x46\n\x10\x63hannel_mappings\x18\x04 \x03(\x0b\x32,.ni.measurementlink.pinmap.v1.ChannelMapping\"J\n\x0e\x43hannelMapping\x12\x19\n\x11pin_or_relay_name\x18\x01 \x01(\t\x12\x0c\n\x04site\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\t2\xf0\x05\n\rPinMapService\x12u\n\x13\x43reatePinMapFromXml\x12\x38.ni.measurementlink.pinmap.v1.CreatePinMapFromXmlRequest\x1a$.ni.measurementlink.pinmap.v1.PinMap\x12u\n\x13UpdatePinMapFromXml\x12\x38.ni.measurementlink.pinmap.v1.UpdatePinMapFromXmlRequest\x1a$.ni.measurementlink.pinmap.v1.PinMap\x12\x61\n\tGetPinMap\x12..ni.measurementlink.pinmap.v1.GetPinMapRequest\x1a$.ni.measurementlink.pinmap.v1.PinMap\x12l\n\tQueryPins\x12..ni.measurementlink.pinmap.v1.QueryPinsRequest\x1a/.ni.measurementlink.pinmap.v1.QueryPinsResponse\x12r\n\x0bQueryRelays\x12\x30.ni.measurementlink.pinmap.v1.QueryRelaysRequest\x1a\x31.ni.measurementlink.pinmap.v1.QueryRelaysResponse\x12\xab\x01\n\x1eQueryResourceAccessInformation\x12\x43.ni.measurementlink.pinmap.v1.QueryResourceAccessInformationRequest\x1a\x44.ni.measurementlink.pinmap.v1.QueryResourceAccessInformationResponseB\xba\x01\n com.ni.measurementlink.pinmap.v1B\x12PinMapServiceProtoP\x01Z\x08pinmapv1\xa2\x02\x04NIMP\xaa\x02-NationalInstruments.MeasurementLink.PinMap.V1\xca\x02\x1cNI\\MeasurementLink\\PinMap\\V1\xea\x02\x1fNI::MeasurementLink::PinMap::V1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "ni.measurementlink.pinmap.v1.pin_map_service_pb2", globals()
-)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ni.measurementlink.pinmap.v1.pin_map_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"\n com.ni.measurementlink.pinmap.v1B\022PinMapServiceProtoP\001Z\010pinmapv1\242\002\004NIMP\252\002-NationalInstruments.MeasurementLink.PinMap.V1\312\002\034NI\\MeasurementLink\\PinMap\\V1\352\002\037NI::MeasurementLink::PinMap::V1"
-    _PINMAP._serialized_start = 84
-    _PINMAP._serialized_end = 112
-    _CREATEPINMAPFROMXMLREQUEST._serialized_start = 114
-    _CREATEPINMAPFROMXMLREQUEST._serialized_end = 183
-    _UPDATEPINMAPFROMXMLREQUEST._serialized_start = 185
-    _UPDATEPINMAPFROMXMLREQUEST._serialized_end = 254
-    _GETPINMAPREQUEST._serialized_start = 256
-    _GETPINMAPREQUEST._serialized_end = 294
-    _QUERYPINSREQUEST._serialized_start = 296
-    _QUERYPINSREQUEST._serialized_end = 362
-    _QUERYPINSRESPONSE._serialized_start = 365
-    _QUERYPINSRESPONSE._serialized_end = 513
-    _PINDEFINITION._serialized_start = 515
-    _PINDEFINITION._serialized_end = 575
-    _PINGROUPDEFINITION._serialized_start = 577
-    _PINGROUPDEFINITION._serialized_end = 675
-    _QUERYRELAYSREQUEST._serialized_start = 677
-    _QUERYRELAYSREQUEST._serialized_end = 717
-    _QUERYRELAYSRESPONSE._serialized_start = 720
-    _QUERYRELAYSRESPONSE._serialized_end = 878
-    _RELAYDEFINITION._serialized_start = 880
-    _RELAYDEFINITION._serialized_end = 944
-    _RELAYGROUPDEFINITION._serialized_start = 946
-    _RELAYGROUPDEFINITION._serialized_end = 1050
-    _QUERYRESOURCEACCESSINFORMATIONREQUEST._serialized_start = 1053
-    _QUERYRESOURCEACCESSINFORMATIONREQUEST._serialized_end = 1183
-    _QUERYRESOURCEACCESSINFORMATIONRESPONSE._serialized_start = 1186
-    _QUERYRESOURCEACCESSINFORMATIONRESPONSE._serialized_end = 1320
-    _RESOURCEACCESSINFORMATION._serialized_start = 1323
-    _RESOURCEACCESSINFORMATION._serialized_end = 1495
-    _CHANNELMAPPING._serialized_start = 1497
-    _CHANNELMAPPING._serialized_end = 1571
-    _PINMAPSERVICE._serialized_start = 1574
-    _PINMAPSERVICE._serialized_end = 2326
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n com.ni.measurementlink.pinmap.v1B\022PinMapServiceProtoP\001Z\010pinmapv1\242\002\004NIMP\252\002-NationalInstruments.MeasurementLink.PinMap.V1\312\002\034NI\\MeasurementLink\\PinMap\\V1\352\002\037NI::MeasurementLink::PinMap::V1'
+  _PINMAP._serialized_start=84
+  _PINMAP._serialized_end=112
+  _CREATEPINMAPFROMXMLREQUEST._serialized_start=114
+  _CREATEPINMAPFROMXMLREQUEST._serialized_end=183
+  _UPDATEPINMAPFROMXMLREQUEST._serialized_start=185
+  _UPDATEPINMAPFROMXMLREQUEST._serialized_end=254
+  _GETPINMAPREQUEST._serialized_start=256
+  _GETPINMAPREQUEST._serialized_end=294
+  _QUERYPINSREQUEST._serialized_start=296
+  _QUERYPINSREQUEST._serialized_end=362
+  _QUERYPINSRESPONSE._serialized_start=365
+  _QUERYPINSRESPONSE._serialized_end=513
+  _PINDEFINITION._serialized_start=515
+  _PINDEFINITION._serialized_end=575
+  _PINGROUPDEFINITION._serialized_start=577
+  _PINGROUPDEFINITION._serialized_end=675
+  _QUERYRELAYSREQUEST._serialized_start=677
+  _QUERYRELAYSREQUEST._serialized_end=717
+  _QUERYRELAYSRESPONSE._serialized_start=720
+  _QUERYRELAYSRESPONSE._serialized_end=878
+  _RELAYDEFINITION._serialized_start=880
+  _RELAYDEFINITION._serialized_end=944
+  _RELAYGROUPDEFINITION._serialized_start=946
+  _RELAYGROUPDEFINITION._serialized_end=1050
+  _QUERYRESOURCEACCESSINFORMATIONREQUEST._serialized_start=1053
+  _QUERYRESOURCEACCESSINFORMATIONREQUEST._serialized_end=1183
+  _QUERYRESOURCEACCESSINFORMATIONRESPONSE._serialized_start=1186
+  _QUERYRESOURCEACCESSINFORMATIONRESPONSE._serialized_end=1320
+  _RESOURCEACCESSINFORMATION._serialized_start=1323
+  _RESOURCEACCESSINFORMATION._serialized_end=1495
+  _CHANNELMAPPING._serialized_start=1497
+  _CHANNELMAPPING._serialized_end=1571
+  _PINMAPSERVICE._serialized_start=1574
+  _PINMAPSERVICE._serialized_end=2326
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     pin_map_id: builtins.str
     """Output only. The resource id of the registered pin map resource."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___PinMap = PinMap
 
 @typing_extensions.final
 class CreatePinMapFromXmlRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -48,20 +46,15 @@
     """Required. A string representing contents of a pin map file."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         pin_map_xml: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"]) -> None: ...
 
 global___CreatePinMapFromXmlRequest = CreatePinMapFromXmlRequest
 
 @typing_extensions.final
 class UpdatePinMapFromXmlRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -73,20 +66,15 @@
     """Required. New pin map file content."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         pin_map_xml: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id", "pin_map_xml", b"pin_map_xml"]) -> None: ...
 
 global___UpdatePinMapFromXmlRequest = UpdatePinMapFromXmlRequest
 
 @typing_extensions.final
 class GetPinMapRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -94,17 +82,15 @@
     pin_map_id: builtins.str
     """Required. The resource id of the registered pin map resource."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___GetPinMapRequest = GetPinMapRequest
 
 @typing_extensions.final
 class QueryPinsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -125,55 +111,40 @@
     """
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
         instrument_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "instrument_type_id", b"instrument_type_id", "pin_map_id", b"pin_map_id"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___QueryPinsRequest = QueryPinsRequest
 
 @typing_extensions.final
 class QueryPinsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PINS_FIELD_NUMBER: builtins.int
     PIN_GROUPS_FIELD_NUMBER: builtins.int
     @property
-    def pins(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___PinDefinition
-    ]:
+    def pins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PinDefinition]:
         """List of pins on the registered pin map resource. This list includes both DUT and System pins."""
     @property
-    def pin_groups(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___PinGroupDefinition
-    ]:
+    def pin_groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PinGroupDefinition]:
         """List of pin groups on the registered pin map resource.
         When an instrument type id filter is specified, a pin group will only be included
         in the response if all pins in the pin group match the instrument type.
         """
     def __init__(
         self,
         *,
         pins: collections.abc.Iterable[global___PinDefinition] | None = ...,
         pin_groups: collections.abc.Iterable[global___PinGroupDefinition] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["pin_groups", b"pin_groups", "pins", b"pins"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pin_groups", b"pin_groups", "pins", b"pins"]) -> None: ...
 
 global___QueryPinsResponse = QueryPinsResponse
 
 @typing_extensions.final
 class PinDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -185,60 +156,41 @@
     """A boolean that indicates a System pin when 'true', or DUT pin when 'false'."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         is_system_pin: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "display_name", b"display_name", "is_system_pin", b"is_system_pin"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "is_system_pin", b"is_system_pin"]) -> None: ...
 
 global___PinDefinition = PinDefinition
 
 @typing_extensions.final
 class PinGroupDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     PIN_OR_GROUP_REFERENCES_FIELD_NUMBER: builtins.int
     RESOLVED_PINS_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Name of the pin group."""
     @property
-    def pin_or_group_references(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+    def pin_or_group_references(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of other pins or pin groups within this pin group."""
     @property
-    def resolved_pins(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+    def resolved_pins(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Distinct union of pins within this pin group, including those within nested pin groups."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         pin_or_group_references: collections.abc.Iterable[builtins.str] | None = ...,
         resolved_pins: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "display_name",
-            b"display_name",
-            "pin_or_group_references",
-            b"pin_or_group_references",
-            "resolved_pins",
-            b"resolved_pins",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "pin_or_group_references", b"pin_or_group_references", "resolved_pins", b"resolved_pins"]) -> None: ...
 
 global___PinGroupDefinition = PinGroupDefinition
 
 @typing_extensions.final
 class QueryRelaysRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -246,50 +198,37 @@
     pin_map_id: builtins.str
     """Required. The resource id of the registered pin map resource."""
     def __init__(
         self,
         *,
         pin_map_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["pin_map_id", b"pin_map_id"]) -> None: ...
 
 global___QueryRelaysRequest = QueryRelaysRequest
 
 @typing_extensions.final
 class QueryRelaysResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RELAYS_FIELD_NUMBER: builtins.int
     RELAY_GROUPS_FIELD_NUMBER: builtins.int
     @property
-    def relays(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___RelayDefinition
-    ]:
+    def relays(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RelayDefinition]:
         """List of relays on the registered pin map resource. This list includes both Site relays and System relays."""
     @property
-    def relay_groups(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___RelayGroupDefinition
-    ]:
+    def relay_groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RelayGroupDefinition]:
         """List of relay groups on the registered pin map resource."""
     def __init__(
         self,
         *,
         relays: collections.abc.Iterable[global___RelayDefinition] | None = ...,
         relay_groups: collections.abc.Iterable[global___RelayGroupDefinition] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal["relay_groups", b"relay_groups", "relays", b"relays"],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["relay_groups", b"relay_groups", "relays", b"relays"]) -> None: ...
 
 global___QueryRelaysResponse = QueryRelaysResponse
 
 @typing_extensions.final
 class RelayDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -301,82 +240,59 @@
     """A boolean that indicates a System relay when 'true', or Site relay when 'false'."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         is_system_relay: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "display_name", b"display_name", "is_system_relay", b"is_system_relay"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "is_system_relay", b"is_system_relay"]) -> None: ...
 
 global___RelayDefinition = RelayDefinition
 
 @typing_extensions.final
 class RelayGroupDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     RELAY_OR_GROUP_REFERENCES_FIELD_NUMBER: builtins.int
     RESOLVED_RELAYS_FIELD_NUMBER: builtins.int
     display_name: builtins.str
     """Name of the relay group."""
     @property
-    def relay_or_group_references(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+    def relay_or_group_references(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of other relays or relay groups within this relay group."""
     @property
-    def resolved_relays(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+    def resolved_relays(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Distinct union of relays within this relay group, including those within nested relay groups."""
     def __init__(
         self,
         *,
         display_name: builtins.str = ...,
         relay_or_group_references: collections.abc.Iterable[builtins.str] | None = ...,
         resolved_relays: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "display_name",
-            b"display_name",
-            "relay_or_group_references",
-            b"relay_or_group_references",
-            "resolved_relays",
-            b"resolved_relays",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "relay_or_group_references", b"relay_or_group_references", "resolved_relays", b"resolved_relays"]) -> None: ...
 
 global___RelayGroupDefinition = RelayGroupDefinition
 
 @typing_extensions.final
 class QueryResourceAccessInformationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PIN_MAP_ID_FIELD_NUMBER: builtins.int
     SITES_FIELD_NUMBER: builtins.int
     PIN_OR_RELAY_NAMES_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     pin_map_id: builtins.str
     """Required. The resource id of the registered pin map resource."""
     @property
-    def sites(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+    def sites(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Optional. The list of sites for which to get instrument resource access information. If unspecified, get instrument resource information for all sites in the registered pin map resource."""
     @property
-    def pin_or_relay_names(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+    def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Optional. The list of pins, pin groups, relays, or relay groups for which to get instrument resource access information. If unspecified, get instrument resource information for all pins and relays in the registered pin map resource."""
     instrument_type_id: builtins.str
     """Optional. The instrument type for which to get instrument resource access information. If unspecified, get instrument resource information for all instrument types connected in the registered pin map resource.
     Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
          "niDCPower"
          "niDigitalPattern"
          "niScope"
@@ -390,54 +306,32 @@
         self,
         *,
         pin_map_id: builtins.str = ...,
         sites: collections.abc.Iterable[builtins.int] | None = ...,
         pin_or_relay_names: collections.abc.Iterable[builtins.str] | None = ...,
         instrument_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "instrument_type_id",
-            b"instrument_type_id",
-            "pin_map_id",
-            b"pin_map_id",
-            "pin_or_relay_names",
-            b"pin_or_relay_names",
-            "sites",
-            b"sites",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "pin_map_id", b"pin_map_id", "pin_or_relay_names", b"pin_or_relay_names", "sites", b"sites"]) -> None: ...
 
 global___QueryResourceAccessInformationRequest = QueryResourceAccessInformationRequest
 
 @typing_extensions.final
 class QueryResourceAccessInformationResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     RESOURCE_ACCESS_INFORMATION_FIELD_NUMBER: builtins.int
     @property
-    def resource_access_information(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___ResourceAccessInformation
-    ]:
+    def resource_access_information(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceAccessInformation]:
         """List of ResourceAccessInformation objects with instrument resource names and channels."""
     def __init__(
         self,
         *,
-        resource_access_information: collections.abc.Iterable[global___ResourceAccessInformation]
-        | None = ...,
-    ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "resource_access_information", b"resource_access_information"
-        ],
+        resource_access_information: collections.abc.Iterable[global___ResourceAccessInformation] | None = ...,
     ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["resource_access_information", b"resource_access_information"]) -> None: ...
 
 global___QueryResourceAccessInformationResponse = QueryResourceAccessInformationResponse
 
 @typing_extensions.final
 class ResourceAccessInformation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -466,43 +360,27 @@
          "niDMM"
          "niDAQmx"
          "niFGen"
          "niRelayDriver"
     For custom instruments the user defined instrument type id is defined in the pin map file.
     """
     @property
-    def channel_mappings(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___ChannelMapping
-    ]:
+    def channel_mappings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ChannelMapping]:
         """List of site and pin/relay mappings that correspond to each channel in the channel_list.
         Each item contains a mapping corresponding to a channel in this instrument resource, in the order of the channel_list.
         """
     def __init__(
         self,
         *,
         resource_name: builtins.str = ...,
         channel_list: builtins.str = ...,
         instrument_type_id: builtins.str = ...,
         channel_mappings: collections.abc.Iterable[global___ChannelMapping] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "channel_list",
-            b"channel_list",
-            "channel_mappings",
-            b"channel_mappings",
-            "instrument_type_id",
-            b"instrument_type_id",
-            "resource_name",
-            b"resource_name",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel_list", b"channel_list", "channel_mappings", b"channel_mappings", "instrument_type_id", b"instrument_type_id", "resource_name", b"resource_name"]) -> None: ...
 
 global___ResourceAccessInformation = ResourceAccessInformation
 
 @typing_extensions.final
 class ChannelMapping(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -520,15 +398,10 @@
     def __init__(
         self,
         *,
         pin_or_relay_name: builtins.str = ...,
         site: builtins.int = ...,
         channel: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "channel", b"channel", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel", b"channel", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"]) -> None: ...
 
 global___ChannelMapping = ChannelMapping
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/pinmap/v1/pin_map_service_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,331 +1,259 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap.v1 import (
-    pin_map_service_pb2 as ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2,
-)
+from ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap.v1 import pin_map_service_pb2 as ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2
 
 
 class PinMapServiceStub(object):
-    """Service to keep track of pin map resources."""
+    """Service to keep track of pin map resources.
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.CreatePinMapFromXml = channel.unary_unary(
-            "/ni.measurementlink.pinmap.v1.PinMapService/CreatePinMapFromXml",
-            request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.CreatePinMapFromXmlRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
-        )
+                '/ni.measurementlink.pinmap.v1.PinMapService/CreatePinMapFromXml',
+                request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.CreatePinMapFromXmlRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
+                )
         self.UpdatePinMapFromXml = channel.unary_unary(
-            "/ni.measurementlink.pinmap.v1.PinMapService/UpdatePinMapFromXml",
-            request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.UpdatePinMapFromXmlRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
-        )
+                '/ni.measurementlink.pinmap.v1.PinMapService/UpdatePinMapFromXml',
+                request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.UpdatePinMapFromXmlRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
+                )
         self.GetPinMap = channel.unary_unary(
-            "/ni.measurementlink.pinmap.v1.PinMapService/GetPinMap",
-            request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.GetPinMapRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
-        )
+                '/ni.measurementlink.pinmap.v1.PinMapService/GetPinMap',
+                request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.GetPinMapRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
+                )
         self.QueryPins = channel.unary_unary(
-            "/ni.measurementlink.pinmap.v1.PinMapService/QueryPins",
-            request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsResponse.FromString,
-        )
+                '/ni.measurementlink.pinmap.v1.PinMapService/QueryPins',
+                request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsResponse.FromString,
+                )
         self.QueryRelays = channel.unary_unary(
-            "/ni.measurementlink.pinmap.v1.PinMapService/QueryRelays",
-            request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysResponse.FromString,
-        )
+                '/ni.measurementlink.pinmap.v1.PinMapService/QueryRelays',
+                request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysResponse.FromString,
+                )
         self.QueryResourceAccessInformation = channel.unary_unary(
-            "/ni.measurementlink.pinmap.v1.PinMapService/QueryResourceAccessInformation",
-            request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationResponse.FromString,
-        )
+                '/ni.measurementlink.pinmap.v1.PinMapService/QueryResourceAccessInformation',
+                request_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationResponse.FromString,
+                )
 
 
 class PinMapServiceServicer(object):
-    """Service to keep track of pin map resources."""
+    """Service to keep track of pin map resources.
+    """
 
     def CreatePinMapFromXml(self, request, context):
         """Registers pin map with the PinMapService and returns a pin map resource.
         Status Codes for errors:
         - INVALID_ARGUMENT: Pin map id is empty or has whitespace, or pin map xml string is not valid
         - ALREADY_EXISTS: Pin map resource with the specified pin map id already exists
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def UpdatePinMapFromXml(self, request, context):
         """Updates registered pin map contents and returns it.
         Creates and registers a pin map if a pin map resource for the specified pin map id is not found.
         Status Codes for errors:
         - INVALID_ARGUMENT: Pin map xml string is not valid
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def GetPinMap(self, request, context):
         """Get registered pin map resource.
         Status Codes for errors:
         - NOT_FOUND: Pin map resource for the specified pin map id is not found
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def QueryPins(self, request, context):
         """Returns list of pins from the registered pin map resource.
         Status Codes for errors:
         - NOT_FOUND: Pin map resource for the specified pin map id is not found
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def QueryRelays(self, request, context):
         """Returns list of relays from the registered pin map resource.
         Status Codes for errors:
         - NOT_FOUND: Pin map resource for the specified pin map id is not found
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def QueryResourceAccessInformation(self, request, context):
         """Get instrument resource names, channels, and instrument type for the specified sites, pins or pin groups, relays or relay groups, instrument type in the registered pin map resource.
         Status Codes for errors:
         - NOT_FOUND:
         - Pin map resource for the specified pin map id is not found.
         - Specified site number is not in the valid range for the registered pin map.
         - INVALID_ARGUMENT:
         - Specified pin or relay is not present in the registered pin map resource.
         - Empty string specified for a pin or relay name.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_PinMapServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "CreatePinMapFromXml": grpc.unary_unary_rpc_method_handler(
-            servicer.CreatePinMapFromXml,
-            request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.CreatePinMapFromXmlRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.SerializeToString,
-        ),
-        "UpdatePinMapFromXml": grpc.unary_unary_rpc_method_handler(
-            servicer.UpdatePinMapFromXml,
-            request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.UpdatePinMapFromXmlRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.SerializeToString,
-        ),
-        "GetPinMap": grpc.unary_unary_rpc_method_handler(
-            servicer.GetPinMap,
-            request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.GetPinMapRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.SerializeToString,
-        ),
-        "QueryPins": grpc.unary_unary_rpc_method_handler(
-            servicer.QueryPins,
-            request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsResponse.SerializeToString,
-        ),
-        "QueryRelays": grpc.unary_unary_rpc_method_handler(
-            servicer.QueryRelays,
-            request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysResponse.SerializeToString,
-        ),
-        "QueryResourceAccessInformation": grpc.unary_unary_rpc_method_handler(
-            servicer.QueryResourceAccessInformation,
-            request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationResponse.SerializeToString,
-        ),
+            'CreatePinMapFromXml': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreatePinMapFromXml,
+                    request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.CreatePinMapFromXmlRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.SerializeToString,
+            ),
+            'UpdatePinMapFromXml': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdatePinMapFromXml,
+                    request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.UpdatePinMapFromXmlRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.SerializeToString,
+            ),
+            'GetPinMap': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPinMap,
+                    request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.GetPinMapRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.SerializeToString,
+            ),
+            'QueryPins': grpc.unary_unary_rpc_method_handler(
+                    servicer.QueryPins,
+                    request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsResponse.SerializeToString,
+            ),
+            'QueryRelays': grpc.unary_unary_rpc_method_handler(
+                    servicer.QueryRelays,
+                    request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysResponse.SerializeToString,
+            ),
+            'QueryResourceAccessInformation': grpc.unary_unary_rpc_method_handler(
+                    servicer.QueryResourceAccessInformation,
+                    request_deserializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "ni.measurementlink.pinmap.v1.PinMapService", rpc_method_handlers
-    )
+            'ni.measurementlink.pinmap.v1.PinMapService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class PinMapService(object):
-    """Service to keep track of pin map resources."""
+    """Service to keep track of pin map resources.
+    """
 
     @staticmethod
-    def CreatePinMapFromXml(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def CreatePinMapFromXml(request,
             target,
-            "/ni.measurementlink.pinmap.v1.PinMapService/CreatePinMapFromXml",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.pinmap.v1.PinMapService/CreatePinMapFromXml',
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.CreatePinMapFromXmlRequest.SerializeToString,
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UpdatePinMapFromXml(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def UpdatePinMapFromXml(request,
             target,
-            "/ni.measurementlink.pinmap.v1.PinMapService/UpdatePinMapFromXml",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.pinmap.v1.PinMapService/UpdatePinMapFromXml',
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.UpdatePinMapFromXmlRequest.SerializeToString,
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetPinMap(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def GetPinMap(request,
             target,
-            "/ni.measurementlink.pinmap.v1.PinMapService/GetPinMap",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.pinmap.v1.PinMapService/GetPinMap',
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.GetPinMapRequest.SerializeToString,
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.PinMap.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def QueryPins(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def QueryPins(request,
             target,
-            "/ni.measurementlink.pinmap.v1.PinMapService/QueryPins",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.pinmap.v1.PinMapService/QueryPins',
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsRequest.SerializeToString,
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryPinsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def QueryRelays(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def QueryRelays(request,
             target,
-            "/ni.measurementlink.pinmap.v1.PinMapService/QueryRelays",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.pinmap.v1.PinMapService/QueryRelays',
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysRequest.SerializeToString,
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryRelaysResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def QueryResourceAccessInformation(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def QueryResourceAccessInformation(request,
             target,
-            "/ni.measurementlink.pinmap.v1.PinMapService/QueryResourceAccessInformation",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.pinmap.v1.PinMapService/QueryResourceAccessInformation',
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationRequest.SerializeToString,
             ni_dot_measurementlink_dot_pinmap_dot_v1_dot_pin__map__service__pb2.QueryResourceAccessInformationResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,58 +2,51 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ni/measurementlink/sessionmanagement/v1/session_management_service.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from ni_measurementlink_service._internal.stubs.ni.measurementlink import (
-    pin_map_context_pb2 as ni_dot_measurementlink_dot_pin__map__context__pb2,
-)
+from ni_measurementlink_service._internal.stubs.ni.measurementlink import pin_map_context_pb2 as ni_dot_measurementlink_dot_pin__map__context__pb2
 from ni_measurementlink_service._internal.stubs import session_pb2 as session__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\nHni/measurementlink/sessionmanagement/v1/session_management_service.proto\x12\'ni.measurementlink.sessionmanagement.v1\x1a(ni/measurementlink/pin_map_context.proto\x1a\rsession.proto"\xf1\x01\n\x12SessionInformation\x12\'\n\x07session\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x14\n\x0c\x63hannel_list\x18\x03 \x01(\t\x12\x1a\n\x12instrument_type_id\x18\x04 \x01(\t\x12\x16\n\x0esession_exists\x18\x05 \x01(\x08\x12Q\n\x10\x63hannel_mappings\x18\x06 \x03(\x0b\x32\x37.ni.measurementlink.sessionmanagement.v1.ChannelMapping"J\n\x0e\x43hannelMapping\x12\x19\n\x11pin_or_relay_name\x18\x01 \x01(\t\x12\x0c\n\x04site\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\t"\xad\x01\n\x16ReserveSessionsRequest\x12:\n\x0fpin_map_context\x18\x01 \x01(\x0b\x32!.ni.measurementlink.PinMapContext\x12\x1a\n\x12pin_or_relay_names\x18\x02 \x03(\t\x12\x1a\n\x12instrument_type_id\x18\x03 \x01(\t\x12\x1f\n\x17timeout_in_milliseconds\x18\x04 \x01(\x05"h\n\x17ReserveSessionsResponse\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation"i\n\x18UnreserveSessionsRequest\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation"\x1b\n\x19UnreserveSessionsResponse"h\n\x17RegisterSessionsRequest\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation"\x1a\n\x18RegisterSessionsResponse"j\n\x19UnregisterSessionsRequest\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation"\x1c\n\x1aUnregisterSessionsResponse"b\n#ReserveAllRegisteredSessionsRequest\x12\x1f\n\x17timeout_in_milliseconds\x18\x01 \x01(\x05\x12\x1a\n\x12instrument_type_id\x18\x02 \x01(\t"u\n$ReserveAllRegisteredSessionsResponse\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation2\xc6\x06\n\x18SessionManagementService\x12\x94\x01\n\x0fReserveSessions\x12?.ni.measurementlink.sessionmanagement.v1.ReserveSessionsRequest\x1a@.ni.measurementlink.sessionmanagement.v1.ReserveSessionsResponse\x12\x9a\x01\n\x11UnreserveSessions\x12\x41.ni.measurementlink.sessionmanagement.v1.UnreserveSessionsRequest\x1a\x42.ni.measurementlink.sessionmanagement.v1.UnreserveSessionsResponse\x12\x97\x01\n\x10RegisterSessions\x12@.ni.measurementlink.sessionmanagement.v1.RegisterSessionsRequest\x1a\x41.ni.measurementlink.sessionmanagement.v1.RegisterSessionsResponse\x12\x9d\x01\n\x12UnregisterSessions\x12\x42.ni.measurementlink.sessionmanagement.v1.UnregisterSessionsRequest\x1a\x43.ni.measurementlink.sessionmanagement.v1.UnregisterSessionsResponse\x12\xbb\x01\n\x1cReserveAllRegisteredSessions\x12L.ni.measurementlink.sessionmanagement.v1.ReserveAllRegisteredSessionsRequest\x1aM.ni.measurementlink.sessionmanagement.v1.ReserveAllRegisteredSessionsResponseB\xf5\x01\n+com.ni.measurementlink.sessionmanagement.v1B\x16SessionManagementProtoP\x01Z\x13sessionmanagementv1\xa2\x02\x04NIMS\xaa\x02\x38NationalInstruments.MeasurementLink.SessionManagement.V1\xca\x02\'NI\\MeasurementLink\\SessionManagement\\V1\xea\x02*NI::MeasurementLink::SessionManagement::V1b\x06proto3'
-)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHni/measurementlink/sessionmanagement/v1/session_management_service.proto\x12\'ni.measurementlink.sessionmanagement.v1\x1a(ni/measurementlink/pin_map_context.proto\x1a\rsession.proto\"\xf1\x01\n\x12SessionInformation\x12\'\n\x07session\x18\x01 \x01(\x0b\x32\x16.nidevice_grpc.Session\x12\x15\n\rresource_name\x18\x02 \x01(\t\x12\x14\n\x0c\x63hannel_list\x18\x03 \x01(\t\x12\x1a\n\x12instrument_type_id\x18\x04 \x01(\t\x12\x16\n\x0esession_exists\x18\x05 \x01(\x08\x12Q\n\x10\x63hannel_mappings\x18\x06 \x03(\x0b\x32\x37.ni.measurementlink.sessionmanagement.v1.ChannelMapping\"J\n\x0e\x43hannelMapping\x12\x19\n\x11pin_or_relay_name\x18\x01 \x01(\t\x12\x0c\n\x04site\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\t\"\xad\x01\n\x16ReserveSessionsRequest\x12:\n\x0fpin_map_context\x18\x01 \x01(\x0b\x32!.ni.measurementlink.PinMapContext\x12\x1a\n\x12pin_or_relay_names\x18\x02 \x03(\t\x12\x1a\n\x12instrument_type_id\x18\x03 \x01(\t\x12\x1f\n\x17timeout_in_milliseconds\x18\x04 \x01(\x05\"h\n\x17ReserveSessionsResponse\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation\"i\n\x18UnreserveSessionsRequest\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation\"\x1b\n\x19UnreserveSessionsResponse\"h\n\x17RegisterSessionsRequest\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation\"\x1a\n\x18RegisterSessionsResponse\"j\n\x19UnregisterSessionsRequest\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation\"\x1c\n\x1aUnregisterSessionsResponse\"b\n#ReserveAllRegisteredSessionsRequest\x12\x1f\n\x17timeout_in_milliseconds\x18\x01 \x01(\x05\x12\x1a\n\x12instrument_type_id\x18\x02 \x01(\t\"u\n$ReserveAllRegisteredSessionsResponse\x12M\n\x08sessions\x18\x01 \x03(\x0b\x32;.ni.measurementlink.sessionmanagement.v1.SessionInformation2\xc6\x06\n\x18SessionManagementService\x12\x94\x01\n\x0fReserveSessions\x12?.ni.measurementlink.sessionmanagement.v1.ReserveSessionsRequest\x1a@.ni.measurementlink.sessionmanagement.v1.ReserveSessionsResponse\x12\x9a\x01\n\x11UnreserveSessions\x12\x41.ni.measurementlink.sessionmanagement.v1.UnreserveSessionsRequest\x1a\x42.ni.measurementlink.sessionmanagement.v1.UnreserveSessionsResponse\x12\x97\x01\n\x10RegisterSessions\x12@.ni.measurementlink.sessionmanagement.v1.RegisterSessionsRequest\x1a\x41.ni.measurementlink.sessionmanagement.v1.RegisterSessionsResponse\x12\x9d\x01\n\x12UnregisterSessions\x12\x42.ni.measurementlink.sessionmanagement.v1.UnregisterSessionsRequest\x1a\x43.ni.measurementlink.sessionmanagement.v1.UnregisterSessionsResponse\x12\xbb\x01\n\x1cReserveAllRegisteredSessions\x12L.ni.measurementlink.sessionmanagement.v1.ReserveAllRegisteredSessionsRequest\x1aM.ni.measurementlink.sessionmanagement.v1.ReserveAllRegisteredSessionsResponseB\xf5\x01\n+com.ni.measurementlink.sessionmanagement.v1B\x16SessionManagementProtoP\x01Z\x13sessionmanagementv1\xa2\x02\x04NIMS\xaa\x02\x38NationalInstruments.MeasurementLink.SessionManagement.V1\xca\x02\'NI\\MeasurementLink\\SessionManagement\\V1\xea\x02*NI::MeasurementLink::SessionManagement::V1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "ni.measurementlink.sessionmanagement.v1.session_management_service_pb2", globals()
-)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ni.measurementlink.sessionmanagement.v1.session_management_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = b"\n+com.ni.measurementlink.sessionmanagement.v1B\026SessionManagementProtoP\001Z\023sessionmanagementv1\242\002\004NIMS\252\0028NationalInstruments.MeasurementLink.SessionManagement.V1\312\002'NI\\MeasurementLink\\SessionManagement\\V1\352\002*NI::MeasurementLink::SessionManagement::V1"
-    _SESSIONINFORMATION._serialized_start = 175
-    _SESSIONINFORMATION._serialized_end = 416
-    _CHANNELMAPPING._serialized_start = 418
-    _CHANNELMAPPING._serialized_end = 492
-    _RESERVESESSIONSREQUEST._serialized_start = 495
-    _RESERVESESSIONSREQUEST._serialized_end = 668
-    _RESERVESESSIONSRESPONSE._serialized_start = 670
-    _RESERVESESSIONSRESPONSE._serialized_end = 774
-    _UNRESERVESESSIONSREQUEST._serialized_start = 776
-    _UNRESERVESESSIONSREQUEST._serialized_end = 881
-    _UNRESERVESESSIONSRESPONSE._serialized_start = 883
-    _UNRESERVESESSIONSRESPONSE._serialized_end = 910
-    _REGISTERSESSIONSREQUEST._serialized_start = 912
-    _REGISTERSESSIONSREQUEST._serialized_end = 1016
-    _REGISTERSESSIONSRESPONSE._serialized_start = 1018
-    _REGISTERSESSIONSRESPONSE._serialized_end = 1044
-    _UNREGISTERSESSIONSREQUEST._serialized_start = 1046
-    _UNREGISTERSESSIONSREQUEST._serialized_end = 1152
-    _UNREGISTERSESSIONSRESPONSE._serialized_start = 1154
-    _UNREGISTERSESSIONSRESPONSE._serialized_end = 1182
-    _RESERVEALLREGISTEREDSESSIONSREQUEST._serialized_start = 1184
-    _RESERVEALLREGISTEREDSESSIONSREQUEST._serialized_end = 1282
-    _RESERVEALLREGISTEREDSESSIONSRESPONSE._serialized_start = 1284
-    _RESERVEALLREGISTEREDSESSIONSRESPONSE._serialized_end = 1401
-    _SESSIONMANAGEMENTSERVICE._serialized_start = 1404
-    _SESSIONMANAGEMENTSERVICE._serialized_end = 2242
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n+com.ni.measurementlink.sessionmanagement.v1B\026SessionManagementProtoP\001Z\023sessionmanagementv1\242\002\004NIMS\252\0028NationalInstruments.MeasurementLink.SessionManagement.V1\312\002\'NI\\MeasurementLink\\SessionManagement\\V1\352\002*NI::MeasurementLink::SessionManagement::V1'
+  _SESSIONINFORMATION._serialized_start=175
+  _SESSIONINFORMATION._serialized_end=416
+  _CHANNELMAPPING._serialized_start=418
+  _CHANNELMAPPING._serialized_end=492
+  _RESERVESESSIONSREQUEST._serialized_start=495
+  _RESERVESESSIONSREQUEST._serialized_end=668
+  _RESERVESESSIONSRESPONSE._serialized_start=670
+  _RESERVESESSIONSRESPONSE._serialized_end=774
+  _UNRESERVESESSIONSREQUEST._serialized_start=776
+  _UNRESERVESESSIONSREQUEST._serialized_end=881
+  _UNRESERVESESSIONSRESPONSE._serialized_start=883
+  _UNRESERVESESSIONSRESPONSE._serialized_end=910
+  _REGISTERSESSIONSREQUEST._serialized_start=912
+  _REGISTERSESSIONSREQUEST._serialized_end=1016
+  _REGISTERSESSIONSRESPONSE._serialized_start=1018
+  _REGISTERSESSIONSRESPONSE._serialized_end=1044
+  _UNREGISTERSESSIONSREQUEST._serialized_start=1046
+  _UNREGISTERSESSIONSREQUEST._serialized_end=1152
+  _UNREGISTERSESSIONSRESPONSE._serialized_start=1154
+  _UNREGISTERSESSIONSRESPONSE._serialized_end=1182
+  _RESERVEALLREGISTEREDSESSIONSREQUEST._serialized_start=1184
+  _RESERVEALLREGISTEREDSESSIONSREQUEST._serialized_end=1282
+  _RESERVEALLREGISTEREDSESSIONSRESPONSE._serialized_start=1284
+  _RESERVEALLREGISTEREDSESSIONSRESPONSE._serialized_end=1401
+  _SESSIONMANAGEMENTSERVICE._serialized_start=1404
+  _SESSIONMANAGEMENTSERVICE._serialized_end=2242
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -56,19 +56,15 @@
     This field is readonly.
     """
     session_exists: builtins.bool
     """Indicates whether the session exists in the Session Manager. This indicates whether the session has been created.
     This field is readonly.
     """
     @property
-    def channel_mappings(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___ChannelMapping
-    ]:
+    def channel_mappings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ChannelMapping]:
         """List of site and pin/relay mappings that correspond to each channel in the channel_list.
         Each item contains a mapping corresponding to a channel in this instrument resource, in the order of the channel_list.
         This field is empty for any SessionInformation returned from ReserveAllRegisteredSessions.
         This field is readonly.
         """
     def __init__(
         self,
@@ -76,34 +72,16 @@
         session: session_pb2.Session | None = ...,
         resource_name: builtins.str = ...,
         channel_list: builtins.str = ...,
         instrument_type_id: builtins.str = ...,
         session_exists: builtins.bool = ...,
         channel_mappings: collections.abc.Iterable[global___ChannelMapping] | None = ...,
     ) -> None: ...
-    def HasField(
-        self, field_name: typing_extensions.Literal["session", b"session"]
-    ) -> builtins.bool: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "channel_list",
-            b"channel_list",
-            "channel_mappings",
-            b"channel_mappings",
-            "instrument_type_id",
-            b"instrument_type_id",
-            "resource_name",
-            b"resource_name",
-            "session",
-            b"session",
-            "session_exists",
-            b"session_exists",
-        ],
-    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["session", b"session"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel_list", b"channel_list", "channel_mappings", b"channel_mappings", "instrument_type_id", b"instrument_type_id", "resource_name", b"resource_name", "session", b"session", "session_exists", b"session_exists"]) -> None: ...
 
 global___SessionInformation = SessionInformation
 
 @typing_extensions.final
 class ChannelMapping(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -121,20 +99,15 @@
     def __init__(
         self,
         *,
         pin_or_relay_name: builtins.str = ...,
         site: builtins.int = ...,
         channel: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "channel", b"channel", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["channel", b"channel", "pin_or_relay_name", b"pin_or_relay_name", "site", b"site"]) -> None: ...
 
 global___ChannelMapping = ChannelMapping
 
 @typing_extensions.final
 class ReserveSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -142,17 +115,15 @@
     PIN_OR_RELAY_NAMES_FIELD_NUMBER: builtins.int
     INSTRUMENT_TYPE_ID_FIELD_NUMBER: builtins.int
     TIMEOUT_IN_MILLISECONDS_FIELD_NUMBER: builtins.int
     @property
     def pin_map_context(self) -> ni.measurementlink.pin_map_context_pb2.PinMapContext:
         """Required. Includes the pin map ID for the pin map in the Pin Map Service, as well as the list of sites for the measurement."""
     @property
-    def pin_or_relay_names(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+    def pin_or_relay_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Optional. List of pins, pin groups, relays, or relay groups to use for the measurement. If unspecified, reserve sessions for all pins and relays in the registered pin map resource."""
     instrument_type_id: builtins.str
     """Optional. Instrument type ID for the measurement. If unspecified, reserve sessions for all instrument types connected in the registered pin map resource.
     Pin maps have built in instrument definitions using the following NI driver based instrument type ids:
          "niDCPower"
          "niDigitalPattern"
          "niScope"
@@ -170,78 +141,52 @@
         self,
         *,
         pin_map_context: ni.measurementlink.pin_map_context_pb2.PinMapContext | None = ...,
         pin_or_relay_names: collections.abc.Iterable[builtins.str] | None = ...,
         instrument_type_id: builtins.str = ...,
         timeout_in_milliseconds: builtins.int = ...,
     ) -> None: ...
-    def HasField(
-        self, field_name: typing_extensions.Literal["pin_map_context", b"pin_map_context"]
-    ) -> builtins.bool: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "instrument_type_id",
-            b"instrument_type_id",
-            "pin_map_context",
-            b"pin_map_context",
-            "pin_or_relay_names",
-            b"pin_or_relay_names",
-            "timeout_in_milliseconds",
-            b"timeout_in_milliseconds",
-        ],
-    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["pin_map_context", b"pin_map_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "pin_map_context", b"pin_map_context", "pin_or_relay_names", b"pin_or_relay_names", "timeout_in_milliseconds", b"timeout_in_milliseconds"]) -> None: ...
 
 global___ReserveSessionsRequest = ReserveSessionsRequest
 
 @typing_extensions.final
 class ReserveSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
-    def sessions(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___SessionInformation
-    ]:
+    def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """List of information needed to create or use each session for the given pin, site, and instrument type ID.
         This field is readonly.
         """
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["sessions", b"sessions"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
 
 global___ReserveSessionsResponse = ReserveSessionsResponse
 
 @typing_extensions.final
 class UnreserveSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
-    def sessions(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___SessionInformation
-    ]:
+    def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Required. List of information of sessions to be unreserved in the session management service."""
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["sessions", b"sessions"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
 
 global___UnreserveSessionsRequest = UnreserveSessionsRequest
 
 @typing_extensions.final
 class UnreserveSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -253,28 +198,22 @@
 
 @typing_extensions.final
 class RegisterSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
-    def sessions(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___SessionInformation
-    ]:
+    def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Required. List of sessions to register with the session management service to track as the sessions are open."""
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["sessions", b"sessions"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
 
 global___RegisterSessionsRequest = RegisterSessionsRequest
 
 @typing_extensions.final
 class RegisterSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -286,28 +225,22 @@
 
 @typing_extensions.final
 class UnregisterSessionsRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
-    def sessions(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___SessionInformation
-    ]:
+    def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Required. List of sessions to unregister with the session management service to mark them as sessions were closed."""
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["sessions", b"sessions"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
 
 global___UnregisterSessionsRequest = UnregisterSessionsRequest
 
 @typing_extensions.final
 class UnregisterSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -341,41 +274,27 @@
     """
     def __init__(
         self,
         *,
         timeout_in_milliseconds: builtins.int = ...,
         instrument_type_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "instrument_type_id",
-            b"instrument_type_id",
-            "timeout_in_milliseconds",
-            b"timeout_in_milliseconds",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instrument_type_id", b"instrument_type_id", "timeout_in_milliseconds", b"timeout_in_milliseconds"]) -> None: ...
 
 global___ReserveAllRegisteredSessionsRequest = ReserveAllRegisteredSessionsRequest
 
 @typing_extensions.final
 class ReserveAllRegisteredSessionsResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SESSIONS_FIELD_NUMBER: builtins.int
     @property
-    def sessions(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___SessionInformation
-    ]:
+    def sessions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SessionInformation]:
         """Sessions currently registered in the session management service."""
     def __init__(
         self,
         *,
         sessions: collections.abc.Iterable[global___SessionInformation] | None = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["sessions", b"sessions"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["sessions", b"sessions"]) -> None: ...
 
 global___ReserveAllRegisteredSessionsResponse = ReserveAllRegisteredSessionsResponse
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/ni/measurementlink/sessionmanagement/v1/session_management_service_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1 import (
-    session_management_service_pb2 as ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2,
-)
+from ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1 import session_management_service_pb2 as ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2
 
 
 class SessionManagementServiceStub(object):
-    """Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site."""
+    """Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site.
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.ReserveSessions = channel.unary_unary(
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveSessions",
-            request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsResponse.FromString,
-        )
+                '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveSessions',
+                request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsResponse.FromString,
+                )
         self.UnreserveSessions = channel.unary_unary(
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnreserveSessions",
-            request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsResponse.FromString,
-        )
+                '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnreserveSessions',
+                request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsResponse.FromString,
+                )
         self.RegisterSessions = channel.unary_unary(
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/RegisterSessions",
-            request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsResponse.FromString,
-        )
+                '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/RegisterSessions',
+                request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsResponse.FromString,
+                )
         self.UnregisterSessions = channel.unary_unary(
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnregisterSessions",
-            request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsResponse.FromString,
-        )
+                '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnregisterSessions',
+                request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsResponse.FromString,
+                )
         self.ReserveAllRegisteredSessions = channel.unary_unary(
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveAllRegisteredSessions",
-            request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsRequest.SerializeToString,
-            response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsResponse.FromString,
-        )
+                '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveAllRegisteredSessions',
+                request_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsRequest.SerializeToString,
+                response_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsResponse.FromString,
+                )
 
 
 class SessionManagementServiceServicer(object):
-    """Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site."""
+    """Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site.
+    """
 
     def ReserveSessions(self, request, context):
         """Reserve session(s) for the given pins or relays, sites, and instrument type ID and returns the information needed to create or access the session.
         (Will be implemented in AB#2046548) Also reserves the session so other processes cannot access it with a ReserveSessions() call.
         Status Codes for errors:
         - INVALID_ARGUMENT:
         - Pin Map Context references a site number that is not defined in the pin map
@@ -56,231 +56,172 @@
         - Timeout specified is less than -1.
         - NOT_FOUND:
         - Pin Map Context has a pin map ID that does not match any pin maps registered with the Pin Map Service.
         - UNAVAILABLE:
         - Session(s) were already reserved and didn't become available before the specified timeout expired.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def UnreserveSessions(self, request, context):
         """Unreserves sessions so they can be accessed by other clients.
         - RESOURCE_EXHAUSTED:
         - Error occurred while unreserving sessions.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def RegisterSessions(self, request, context):
         """Registers the sessions with this service. Indicates that the sessions are open and will need to be closed later.
         Status Codes for errors:
         - ALREADY_EXISTS:
         - Session by the same name is already registered.
         - INVALID_ARGUMENT:
         - Session names list has an empty string.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def UnregisterSessions(self, request, context):
-        """Unregisters the sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again."""
+        """Unregisters the sessions with this service. Indicates that the sessions have been closed and will need to be reopened before they can be used again.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ReserveAllRegisteredSessions(self, request, context):
         """Reserves and gets all sessions currently registered with this service.
         - INVALID_ARGUMENT:
         - Timeout specified is less than -1.
         - UNAVAILABLE:
         - Session(s) were already reserved and didn't become available before the specified timeout expired.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_SessionManagementServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "ReserveSessions": grpc.unary_unary_rpc_method_handler(
-            servicer.ReserveSessions,
-            request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsResponse.SerializeToString,
-        ),
-        "UnreserveSessions": grpc.unary_unary_rpc_method_handler(
-            servicer.UnreserveSessions,
-            request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsResponse.SerializeToString,
-        ),
-        "RegisterSessions": grpc.unary_unary_rpc_method_handler(
-            servicer.RegisterSessions,
-            request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsResponse.SerializeToString,
-        ),
-        "UnregisterSessions": grpc.unary_unary_rpc_method_handler(
-            servicer.UnregisterSessions,
-            request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsResponse.SerializeToString,
-        ),
-        "ReserveAllRegisteredSessions": grpc.unary_unary_rpc_method_handler(
-            servicer.ReserveAllRegisteredSessions,
-            request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsRequest.FromString,
-            response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsResponse.SerializeToString,
-        ),
+            'ReserveSessions': grpc.unary_unary_rpc_method_handler(
+                    servicer.ReserveSessions,
+                    request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsResponse.SerializeToString,
+            ),
+            'UnreserveSessions': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnreserveSessions,
+                    request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsResponse.SerializeToString,
+            ),
+            'RegisterSessions': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterSessions,
+                    request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsResponse.SerializeToString,
+            ),
+            'UnregisterSessions': grpc.unary_unary_rpc_method_handler(
+                    servicer.UnregisterSessions,
+                    request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsResponse.SerializeToString,
+            ),
+            'ReserveAllRegisteredSessions': grpc.unary_unary_rpc_method_handler(
+                    servicer.ReserveAllRegisteredSessions,
+                    request_deserializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsRequest.FromString,
+                    response_serializer=ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "ni.measurementlink.sessionmanagement.v1.SessionManagementService", rpc_method_handlers
-    )
+            'ni.measurementlink.sessionmanagement.v1.SessionManagementService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class SessionManagementService(object):
-    """Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site."""
+    """Service to keep track of open sessions used by measurement services, and to allow measurement services to access sessions by pin and site.
+    """
 
     @staticmethod
-    def ReserveSessions(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def ReserveSessions(request,
             target,
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveSessions",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveSessions',
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsRequest.SerializeToString,
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveSessionsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UnreserveSessions(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def UnreserveSessions(request,
             target,
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnreserveSessions",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnreserveSessions',
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsRequest.SerializeToString,
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnreserveSessionsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def RegisterSessions(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def RegisterSessions(request,
             target,
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/RegisterSessions",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/RegisterSessions',
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsRequest.SerializeToString,
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.RegisterSessionsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def UnregisterSessions(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def UnregisterSessions(request,
             target,
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnregisterSessions",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/UnregisterSessions',
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsRequest.SerializeToString,
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.UnregisterSessionsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ReserveAllRegisteredSessions(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def ReserveAllRegisteredSessions(request,
             target,
-            "/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveAllRegisteredSessions",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ni.measurementlink.sessionmanagement.v1.SessionManagementService/ReserveAllRegisteredSessions',
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsRequest.SerializeToString,
             ni_dot_measurementlink_dot_sessionmanagement_dot_v1_dot_session__management__service__pb2.ReserveAllRegisteredSessionsResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/README.md` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/README.md`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/discovery/v1/discovery_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/measurement/v1/measurement_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pin_map_context.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/pinmap/v1/pin_map_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/ni/measurementlink/sessionmanagement/v1/session_management_service.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/proto/session.proto` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/proto/session.proto`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/session_pb2.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,54 +2,51 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: session.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\rsession.proto\x12\rnidevice_grpc"2\n\x07Session\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x12\x0c\n\x02id\x18\x02 \x01(\rH\x00\x42\t\n\x07session"j\n\x10\x44\x65viceProperties\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05model\x18\x02 \x01(\t\x12\x0e\n\x06vendor\x18\x03 \x01(\t\x12\x15\n\rserial_number\x18\x04 \x01(\t\x12\x12\n\nproduct_id\x18\x05 \x01(\r"\x19\n\x17\x45numerateDevicesRequest"L\n\x18\x45numerateDevicesResponse\x12\x30\n\x07\x64\x65vices\x18\x01 \x03(\x0b\x32\x1f.nidevice_grpc.DeviceProperties";\n\x0eReserveRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t"&\n\x0fReserveResponse\x12\x13\n\x0bis_reserved\x18\x01 \x01(\x08"F\n\x19IsReservedByClientRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t"1\n\x1aIsReservedByClientResponse\x12\x13\n\x0bis_reserved\x18\x01 \x01(\x08"=\n\x10UnreserveRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t"*\n\x11UnreserveResponse\x12\x15\n\ris_unreserved\x18\x01 \x01(\x08"\x14\n\x12ResetServerRequest".\n\x13ResetServerResponse\x12\x17\n\x0fis_server_reset\x18\x01 \x01(\x08*\xbc\x01\n\x1dSessionInitializationBehavior\x12/\n+SESSION_INITIALIZATION_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x32\n.SESSION_INITIALIZATION_BEHAVIOR_INITIALIZE_NEW\x10\x01\x12\x36\n2SESSION_INITIALIZATION_BEHAVIOR_ATTACH_TO_EXISTING\x10\x02\x32\xd2\x03\n\x10SessionUtilities\x12\x63\n\x10\x45numerateDevices\x12&.nidevice_grpc.EnumerateDevicesRequest\x1a\'.nidevice_grpc.EnumerateDevicesResponse\x12H\n\x07Reserve\x12\x1d.nidevice_grpc.ReserveRequest\x1a\x1e.nidevice_grpc.ReserveResponse\x12i\n\x12IsReservedByClient\x12(.nidevice_grpc.IsReservedByClientRequest\x1a).nidevice_grpc.IsReservedByClientResponse\x12N\n\tUnreserve\x12\x1f.nidevice_grpc.UnreserveRequest\x1a .nidevice_grpc.UnreserveResponse\x12T\n\x0bResetServer\x12!.nidevice_grpc.ResetServerRequest\x1a".nidevice_grpc.ResetServerResponseBB\n\x12\x63om.ni.grpc.deviceB\x08NiDeviceP\x01\xaa\x02\x1fNationalInstruments.Grpc.Deviceb\x06proto3'
-)
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rsession.proto\x12\rnidevice_grpc\"2\n\x07Session\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x12\x0c\n\x02id\x18\x02 \x01(\rH\x00\x42\t\n\x07session\"j\n\x10\x44\x65viceProperties\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05model\x18\x02 \x01(\t\x12\x0e\n\x06vendor\x18\x03 \x01(\t\x12\x15\n\rserial_number\x18\x04 \x01(\t\x12\x12\n\nproduct_id\x18\x05 \x01(\r\"\x19\n\x17\x45numerateDevicesRequest\"L\n\x18\x45numerateDevicesResponse\x12\x30\n\x07\x64\x65vices\x18\x01 \x03(\x0b\x32\x1f.nidevice_grpc.DeviceProperties\";\n\x0eReserveRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\"&\n\x0fReserveResponse\x12\x13\n\x0bis_reserved\x18\x01 \x01(\x08\"F\n\x19IsReservedByClientRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\"1\n\x1aIsReservedByClientResponse\x12\x13\n\x0bis_reserved\x18\x01 \x01(\x08\"=\n\x10UnreserveRequest\x12\x16\n\x0ereservation_id\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\"*\n\x11UnreserveResponse\x12\x15\n\ris_unreserved\x18\x01 \x01(\x08\"\x14\n\x12ResetServerRequest\".\n\x13ResetServerResponse\x12\x17\n\x0fis_server_reset\x18\x01 \x01(\x08*\xbc\x01\n\x1dSessionInitializationBehavior\x12/\n+SESSION_INITIALIZATION_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x32\n.SESSION_INITIALIZATION_BEHAVIOR_INITIALIZE_NEW\x10\x01\x12\x36\n2SESSION_INITIALIZATION_BEHAVIOR_ATTACH_TO_EXISTING\x10\x02\x32\xd2\x03\n\x10SessionUtilities\x12\x63\n\x10\x45numerateDevices\x12&.nidevice_grpc.EnumerateDevicesRequest\x1a\'.nidevice_grpc.EnumerateDevicesResponse\x12H\n\x07Reserve\x12\x1d.nidevice_grpc.ReserveRequest\x1a\x1e.nidevice_grpc.ReserveResponse\x12i\n\x12IsReservedByClient\x12(.nidevice_grpc.IsReservedByClientRequest\x1a).nidevice_grpc.IsReservedByClientResponse\x12N\n\tUnreserve\x12\x1f.nidevice_grpc.UnreserveRequest\x1a .nidevice_grpc.UnreserveResponse\x12T\n\x0bResetServer\x12!.nidevice_grpc.ResetServerRequest\x1a\".nidevice_grpc.ResetServerResponseBB\n\x12\x63om.ni.grpc.deviceB\x08NiDeviceP\x01\xaa\x02\x1fNationalInstruments.Grpc.Deviceb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "session_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'session_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
-    DESCRIPTOR._options = None
-    DESCRIPTOR._serialized_options = (
-        b"\n\022com.ni.grpc.deviceB\010NiDeviceP\001\252\002\037NationalInstruments.Grpc.Device"
-    )
-    _SESSIONINITIALIZATIONBEHAVIOR._serialized_start = 699
-    _SESSIONINITIALIZATIONBEHAVIOR._serialized_end = 887
-    _SESSION._serialized_start = 32
-    _SESSION._serialized_end = 82
-    _DEVICEPROPERTIES._serialized_start = 84
-    _DEVICEPROPERTIES._serialized_end = 190
-    _ENUMERATEDEVICESREQUEST._serialized_start = 192
-    _ENUMERATEDEVICESREQUEST._serialized_end = 217
-    _ENUMERATEDEVICESRESPONSE._serialized_start = 219
-    _ENUMERATEDEVICESRESPONSE._serialized_end = 295
-    _RESERVEREQUEST._serialized_start = 297
-    _RESERVEREQUEST._serialized_end = 356
-    _RESERVERESPONSE._serialized_start = 358
-    _RESERVERESPONSE._serialized_end = 396
-    _ISRESERVEDBYCLIENTREQUEST._serialized_start = 398
-    _ISRESERVEDBYCLIENTREQUEST._serialized_end = 468
-    _ISRESERVEDBYCLIENTRESPONSE._serialized_start = 470
-    _ISRESERVEDBYCLIENTRESPONSE._serialized_end = 519
-    _UNRESERVEREQUEST._serialized_start = 521
-    _UNRESERVEREQUEST._serialized_end = 582
-    _UNRESERVERESPONSE._serialized_start = 584
-    _UNRESERVERESPONSE._serialized_end = 626
-    _RESETSERVERREQUEST._serialized_start = 628
-    _RESETSERVERREQUEST._serialized_end = 648
-    _RESETSERVERRESPONSE._serialized_start = 650
-    _RESETSERVERRESPONSE._serialized_end = 696
-    _SESSIONUTILITIES._serialized_start = 890
-    _SESSIONUTILITIES._serialized_end = 1356
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\022com.ni.grpc.deviceB\010NiDeviceP\001\252\002\037NationalInstruments.Grpc.Device'
+  _SESSIONINITIALIZATIONBEHAVIOR._serialized_start=699
+  _SESSIONINITIALIZATIONBEHAVIOR._serialized_end=887
+  _SESSION._serialized_start=32
+  _SESSION._serialized_end=82
+  _DEVICEPROPERTIES._serialized_start=84
+  _DEVICEPROPERTIES._serialized_end=190
+  _ENUMERATEDEVICESREQUEST._serialized_start=192
+  _ENUMERATEDEVICESREQUEST._serialized_end=217
+  _ENUMERATEDEVICESRESPONSE._serialized_start=219
+  _ENUMERATEDEVICESRESPONSE._serialized_end=295
+  _RESERVEREQUEST._serialized_start=297
+  _RESERVEREQUEST._serialized_end=356
+  _RESERVERESPONSE._serialized_start=358
+  _RESERVERESPONSE._serialized_end=396
+  _ISRESERVEDBYCLIENTREQUEST._serialized_start=398
+  _ISRESERVEDBYCLIENTREQUEST._serialized_end=468
+  _ISRESERVEDBYCLIENTRESPONSE._serialized_start=470
+  _ISRESERVEDBYCLIENTRESPONSE._serialized_end=519
+  _UNRESERVEREQUEST._serialized_start=521
+  _UNRESERVEREQUEST._serialized_end=582
+  _UNRESERVERESPONSE._serialized_start=584
+  _UNRESERVERESPONSE._serialized_end=626
+  _RESETSERVERREQUEST._serialized_start=628
+  _RESETSERVERREQUEST._serialized_end=648
+  _RESETSERVERRESPONSE._serialized_start=650
+  _RESETSERVERRESPONSE._serialized_end=696
+  _SESSIONUTILITIES._serialized_start=890
+  _SESSIONUTILITIES._serialized_end=1356
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/session_pb2.pyi` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -18,28 +18,21 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _SessionInitializationBehavior:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _SessionInitializationBehaviorEnumTypeWrapper(
-    google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[
-        _SessionInitializationBehavior.ValueType
-    ],
-    builtins.type,
-):
+class _SessionInitializationBehaviorEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_SessionInitializationBehavior.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SESSION_INITIALIZATION_BEHAVIOR_UNSPECIFIED: _SessionInitializationBehavior.ValueType  # 0
     SESSION_INITIALIZATION_BEHAVIOR_INITIALIZE_NEW: _SessionInitializationBehavior.ValueType  # 1
     SESSION_INITIALIZATION_BEHAVIOR_ATTACH_TO_EXISTING: _SessionInitializationBehavior.ValueType  # 2
 
-class SessionInitializationBehavior(
-    _SessionInitializationBehavior, metaclass=_SessionInitializationBehaviorEnumTypeWrapper
-): ...
+class SessionInitializationBehavior(_SessionInitializationBehavior, metaclass=_SessionInitializationBehaviorEnumTypeWrapper): ...
 
 SESSION_INITIALIZATION_BEHAVIOR_UNSPECIFIED: SessionInitializationBehavior.ValueType  # 0
 SESSION_INITIALIZATION_BEHAVIOR_INITIALIZE_NEW: SessionInitializationBehavior.ValueType  # 1
 SESSION_INITIALIZATION_BEHAVIOR_ATTACH_TO_EXISTING: SessionInitializationBehavior.ValueType  # 2
 global___SessionInitializationBehavior = SessionInitializationBehavior
 
 @typing_extensions.final
@@ -52,25 +45,17 @@
     id: builtins.int
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         id: builtins.int = ...,
     ) -> None: ...
-    def HasField(
-        self,
-        field_name: typing_extensions.Literal["id", b"id", "name", b"name", "session", b"session"],
-    ) -> builtins.bool: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal["id", b"id", "name", b"name", "session", b"session"],
-    ) -> None: ...
-    def WhichOneof(
-        self, oneof_group: typing_extensions.Literal["session", b"session"]
-    ) -> typing_extensions.Literal["name", "id"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["id", b"id", "name", b"name", "session", b"session"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "name", b"name", "session", b"session"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["session", b"session"]) -> typing_extensions.Literal["name", "id"] | None: ...
 
 global___Session = Session
 
 @typing_extensions.final
 class DeviceProperties(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -89,29 +74,15 @@
         *,
         name: builtins.str = ...,
         model: builtins.str = ...,
         vendor: builtins.str = ...,
         serial_number: builtins.str = ...,
         product_id: builtins.int = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "model",
-            b"model",
-            "name",
-            b"name",
-            "product_id",
-            b"product_id",
-            "serial_number",
-            b"serial_number",
-            "vendor",
-            b"vendor",
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["model", b"model", "name", b"name", "product_id", b"product_id", "serial_number", b"serial_number", "vendor", b"vendor"]) -> None: ...
 
 global___DeviceProperties = DeviceProperties
 
 @typing_extensions.final
 class EnumerateDevicesRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -123,19 +94,15 @@
 
 @typing_extensions.final
 class EnumerateDevicesResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEVICES_FIELD_NUMBER: builtins.int
     @property
-    def devices(
-        self,
-    ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[
-        global___DeviceProperties
-    ]: ...
+    def devices(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeviceProperties]: ...
     def __init__(
         self,
         *,
         devices: collections.abc.Iterable[global___DeviceProperties] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["devices", b"devices"]) -> None: ...
 
@@ -153,37 +120,30 @@
     """client defined identifier for a specific client"""
     def __init__(
         self,
         *,
         reservation_id: builtins.str = ...,
         client_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "client_id", b"client_id", "reservation_id", b"reservation_id"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
 
 global___ReserveRequest = ReserveRequest
 
 @typing_extensions.final
 class ReserveResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_RESERVED_FIELD_NUMBER: builtins.int
     is_reserved: builtins.bool
     def __init__(
         self,
         *,
         is_reserved: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["is_reserved", b"is_reserved"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["is_reserved", b"is_reserved"]) -> None: ...
 
 global___ReserveResponse = ReserveResponse
 
 @typing_extensions.final
 class IsReservedByClientRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -195,37 +155,30 @@
     """client defined identifier for a specific client"""
     def __init__(
         self,
         *,
         reservation_id: builtins.str = ...,
         client_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "client_id", b"client_id", "reservation_id", b"reservation_id"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
 
 global___IsReservedByClientRequest = IsReservedByClientRequest
 
 @typing_extensions.final
 class IsReservedByClientResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_RESERVED_FIELD_NUMBER: builtins.int
     is_reserved: builtins.bool
     def __init__(
         self,
         *,
         is_reserved: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["is_reserved", b"is_reserved"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["is_reserved", b"is_reserved"]) -> None: ...
 
 global___IsReservedByClientResponse = IsReservedByClientResponse
 
 @typing_extensions.final
 class UnreserveRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -237,37 +190,30 @@
     """client defined identifier for a specific client"""
     def __init__(
         self,
         *,
         reservation_id: builtins.str = ...,
         client_id: builtins.str = ...,
     ) -> None: ...
-    def ClearField(
-        self,
-        field_name: typing_extensions.Literal[
-            "client_id", b"client_id", "reservation_id", b"reservation_id"
-        ],
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["client_id", b"client_id", "reservation_id", b"reservation_id"]) -> None: ...
 
 global___UnreserveRequest = UnreserveRequest
 
 @typing_extensions.final
 class UnreserveResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IS_UNRESERVED_FIELD_NUMBER: builtins.int
     is_unreserved: builtins.bool
     def __init__(
         self,
         *,
         is_unreserved: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["is_unreserved", b"is_unreserved"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["is_unreserved", b"is_unreserved"]) -> None: ...
 
 global___UnreserveResponse = UnreserveResponse
 
 @typing_extensions.final
 class ResetServerRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -284,12 +230,10 @@
     IS_SERVER_RESET_FIELD_NUMBER: builtins.int
     is_server_reset: builtins.bool
     def __init__(
         self,
         *,
         is_server_reset: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(
-        self, field_name: typing_extensions.Literal["is_server_reset", b"is_server_reset"]
-    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["is_server_reset", b"is_server_reset"]) -> None: ...
 
 global___ResetServerResponse = ResetServerResponse
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/_internal/stubs/session_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,251 +11,194 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.EnumerateDevices = channel.unary_unary(
-            "/nidevice_grpc.SessionUtilities/EnumerateDevices",
-            request_serializer=session__pb2.EnumerateDevicesRequest.SerializeToString,
-            response_deserializer=session__pb2.EnumerateDevicesResponse.FromString,
-        )
+                '/nidevice_grpc.SessionUtilities/EnumerateDevices',
+                request_serializer=session__pb2.EnumerateDevicesRequest.SerializeToString,
+                response_deserializer=session__pb2.EnumerateDevicesResponse.FromString,
+                )
         self.Reserve = channel.unary_unary(
-            "/nidevice_grpc.SessionUtilities/Reserve",
-            request_serializer=session__pb2.ReserveRequest.SerializeToString,
-            response_deserializer=session__pb2.ReserveResponse.FromString,
-        )
+                '/nidevice_grpc.SessionUtilities/Reserve',
+                request_serializer=session__pb2.ReserveRequest.SerializeToString,
+                response_deserializer=session__pb2.ReserveResponse.FromString,
+                )
         self.IsReservedByClient = channel.unary_unary(
-            "/nidevice_grpc.SessionUtilities/IsReservedByClient",
-            request_serializer=session__pb2.IsReservedByClientRequest.SerializeToString,
-            response_deserializer=session__pb2.IsReservedByClientResponse.FromString,
-        )
+                '/nidevice_grpc.SessionUtilities/IsReservedByClient',
+                request_serializer=session__pb2.IsReservedByClientRequest.SerializeToString,
+                response_deserializer=session__pb2.IsReservedByClientResponse.FromString,
+                )
         self.Unreserve = channel.unary_unary(
-            "/nidevice_grpc.SessionUtilities/Unreserve",
-            request_serializer=session__pb2.UnreserveRequest.SerializeToString,
-            response_deserializer=session__pb2.UnreserveResponse.FromString,
-        )
+                '/nidevice_grpc.SessionUtilities/Unreserve',
+                request_serializer=session__pb2.UnreserveRequest.SerializeToString,
+                response_deserializer=session__pb2.UnreserveResponse.FromString,
+                )
         self.ResetServer = channel.unary_unary(
-            "/nidevice_grpc.SessionUtilities/ResetServer",
-            request_serializer=session__pb2.ResetServerRequest.SerializeToString,
-            response_deserializer=session__pb2.ResetServerResponse.FromString,
-        )
+                '/nidevice_grpc.SessionUtilities/ResetServer',
+                request_serializer=session__pb2.ResetServerRequest.SerializeToString,
+                response_deserializer=session__pb2.ResetServerResponse.FromString,
+                )
 
 
 class SessionUtilitiesServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def EnumerateDevices(self, request, context):
-        """Provides a list of devices or chassis connected to server under localhost"""
+        """Provides a list of devices or chassis connected to server under localhost
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def Reserve(self, request, context):
-        """Reserve a set of client defined resources for exclusive use"""
+        """Reserve a set of client defined resources for exclusive use
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def IsReservedByClient(self, request, context):
         """Determines if a set of client defined resources is currently reserved by a
         specific client
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def Unreserve(self, request, context):
-        """Unreserves a previously reserved resource"""
+        """Unreserves a previously reserved resource
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
     def ResetServer(self, request, context):
-        """Resets the server to a default state with no open sessions"""
+        """Resets the server to a default state with no open sessions
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details("Method not implemented!")
-        raise NotImplementedError("Method not implemented!")
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
 
 
 def add_SessionUtilitiesServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        "EnumerateDevices": grpc.unary_unary_rpc_method_handler(
-            servicer.EnumerateDevices,
-            request_deserializer=session__pb2.EnumerateDevicesRequest.FromString,
-            response_serializer=session__pb2.EnumerateDevicesResponse.SerializeToString,
-        ),
-        "Reserve": grpc.unary_unary_rpc_method_handler(
-            servicer.Reserve,
-            request_deserializer=session__pb2.ReserveRequest.FromString,
-            response_serializer=session__pb2.ReserveResponse.SerializeToString,
-        ),
-        "IsReservedByClient": grpc.unary_unary_rpc_method_handler(
-            servicer.IsReservedByClient,
-            request_deserializer=session__pb2.IsReservedByClientRequest.FromString,
-            response_serializer=session__pb2.IsReservedByClientResponse.SerializeToString,
-        ),
-        "Unreserve": grpc.unary_unary_rpc_method_handler(
-            servicer.Unreserve,
-            request_deserializer=session__pb2.UnreserveRequest.FromString,
-            response_serializer=session__pb2.UnreserveResponse.SerializeToString,
-        ),
-        "ResetServer": grpc.unary_unary_rpc_method_handler(
-            servicer.ResetServer,
-            request_deserializer=session__pb2.ResetServerRequest.FromString,
-            response_serializer=session__pb2.ResetServerResponse.SerializeToString,
-        ),
+            'EnumerateDevices': grpc.unary_unary_rpc_method_handler(
+                    servicer.EnumerateDevices,
+                    request_deserializer=session__pb2.EnumerateDevicesRequest.FromString,
+                    response_serializer=session__pb2.EnumerateDevicesResponse.SerializeToString,
+            ),
+            'Reserve': grpc.unary_unary_rpc_method_handler(
+                    servicer.Reserve,
+                    request_deserializer=session__pb2.ReserveRequest.FromString,
+                    response_serializer=session__pb2.ReserveResponse.SerializeToString,
+            ),
+            'IsReservedByClient': grpc.unary_unary_rpc_method_handler(
+                    servicer.IsReservedByClient,
+                    request_deserializer=session__pb2.IsReservedByClientRequest.FromString,
+                    response_serializer=session__pb2.IsReservedByClientResponse.SerializeToString,
+            ),
+            'Unreserve': grpc.unary_unary_rpc_method_handler(
+                    servicer.Unreserve,
+                    request_deserializer=session__pb2.UnreserveRequest.FromString,
+                    response_serializer=session__pb2.UnreserveResponse.SerializeToString,
+            ),
+            'ResetServer': grpc.unary_unary_rpc_method_handler(
+                    servicer.ResetServer,
+                    request_deserializer=session__pb2.ResetServerRequest.FromString,
+                    response_serializer=session__pb2.ResetServerResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        "nidevice_grpc.SessionUtilities", rpc_method_handlers
-    )
+            'nidevice_grpc.SessionUtilities', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
-# This class is part of an EXPERIMENTAL API.
+ # This class is part of an EXPERIMENTAL API.
 class SessionUtilities(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def EnumerateDevices(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def EnumerateDevices(request,
             target,
-            "/nidevice_grpc.SessionUtilities/EnumerateDevices",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nidevice_grpc.SessionUtilities/EnumerateDevices',
             session__pb2.EnumerateDevicesRequest.SerializeToString,
             session__pb2.EnumerateDevicesResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Reserve(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def Reserve(request,
             target,
-            "/nidevice_grpc.SessionUtilities/Reserve",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nidevice_grpc.SessionUtilities/Reserve',
             session__pb2.ReserveRequest.SerializeToString,
             session__pb2.ReserveResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def IsReservedByClient(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def IsReservedByClient(request,
             target,
-            "/nidevice_grpc.SessionUtilities/IsReservedByClient",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nidevice_grpc.SessionUtilities/IsReservedByClient',
             session__pb2.IsReservedByClientRequest.SerializeToString,
             session__pb2.IsReservedByClientResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Unreserve(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def Unreserve(request,
             target,
-            "/nidevice_grpc.SessionUtilities/Unreserve",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nidevice_grpc.SessionUtilities/Unreserve',
             session__pb2.UnreserveRequest.SerializeToString,
             session__pb2.UnreserveResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ResetServer(
-        request,
-        target,
-        options=(),
-        channel_credentials=None,
-        call_credentials=None,
-        insecure=False,
-        compression=None,
-        wait_for_ready=None,
-        timeout=None,
-        metadata=None,
-    ):
-        return grpc.experimental.unary_unary(
-            request,
+    def ResetServer(request,
             target,
-            "/nidevice_grpc.SessionUtilities/ResetServer",
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/nidevice_grpc.SessionUtilities/ResetServer',
             session__pb2.ResetServerRequest.SerializeToString,
             session__pb2.ResetServerResponse.FromString,
-            options,
-            channel_credentials,
-            insecure,
-            call_credentials,
-            compression,
-            wait_for_ready,
-            timeout,
-            metadata,
-        )
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/measurement/info.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/info.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/measurement/service.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/measurement/service.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/ni_measurementlink_service/session_management.py` & `ni_measurementlink_service-1.1.0.dev0/ni_measurementlink_service/session_management.py`

 * *Files identical despite different names*

### Comparing `ni_measurementlink_service-1.0.1/pyproject.toml` & `ni_measurementlink_service-1.1.0.dev0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 | \.venv
 | venv
 )
 '''
 
 [tool.poetry]
 name = "ni_measurementlink_service"
-version = "1.0.1"
+version = "1.1.0-dev0"
 description = "MeasurementLink Support for Python"
 authors = ["NI <opensource@ni.com>"]
 readme = "README.md" # apply the repo readme to the package as well
 repository = "https://github.com/ni/measurementlink-python/"
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -32,49 +32,57 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 # This package includes gRPC stubs that were generated with the version of grpcio-tools specified
 # below. Please keep the minimum grpcio version in sync with the grpcio-tools version. Otherwise,
 # the generated gRPC stubs may not work with the minimum grpcio version.
 grpcio = "^1.49.1"
 protobuf = "^4.21"
-pywin32 = {version = "^303", platform = "win32"}
+pywin32 = {version = ">=303", platform = "win32"}
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
-ni-python-styleguide = ">=0.4.0"
+ni-python-styleguide = ">=0.4.1"
 # When you update the grpcio-tools version, you should update the minimum grpcio version
 # and regenerate gRPC stubs.
 grpcio-tools = "1.49.1"
+pytest-cov = ">=3.0.0"
+mypy = ">=1.0"
+mypy-protobuf = ">=3.4"
+types-protobuf = "^4.21"
+types-pkg-resources = "*"
+types-pywin32 = {version = ">=304", platform = "win32"}
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
 Sphinx = "^5.0.1"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-autoapi = "^1.8.4"
 m2r2 = "^0.3.2"
 toml = "^0.10.2"
 tomlkit = "^0.11.0"
 sphinx-click = "^4.1.0"
-pytest-cov = ">=3.0.0"
-mypy = ">=1.0"
-mypy-protobuf = ">=3.4"
-types-protobuf = "^4.21"
-types-pkg-resources = "*"
-mako = "*"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ni-python-styleguide]
 extend_exclude = "*_pb2_grpc.py,*_pb2.py,venv,ni_measurementlink_generator/*"
 
 [tool.pytest.ini_options]
-testpaths = [
-    "tests"
-]
+addopts = "--doctest-modules --strict-markers"
+filterwarnings = ["always::ImportWarning", "always::ResourceWarning"]
+testpaths = ["tests"]
 
 [tool.mypy]
 exclude = ["stubs"]
 warn_unused_configs = true
 namespace_packages = true
 check_untyped_defs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
-ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "grpc.*"
+ignore_missing_imports = true
```

### Comparing `ni_measurementlink_service-1.0.1/setup.py` & `ni_measurementlink_service-1.1.0.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,39 +8,41 @@
  'ni_measurementlink_service._internal.stubs',
  'ni_measurementlink_service._internal.stubs.ni',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.discovery.v1',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v1',
+ 'ni_measurementlink_service._internal.stubs.ni.measurementlink.measurement.v2',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.pinmap.v1',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement',
  'ni_measurementlink_service._internal.stubs.ni.measurementlink.sessionmanagement.v1',
  'ni_measurementlink_service._internal.utilities',
  'ni_measurementlink_service.measurement']
 
 package_data = \
 {'': ['*'],
  'ni_measurementlink_service._internal.stubs': ['proto/*',
                                                 'proto/ni/measurementlink/*',
                                                 'proto/ni/measurementlink/discovery/v1/*',
                                                 'proto/ni/measurementlink/measurement/v1/*',
+                                                'proto/ni/measurementlink/measurement/v2/*',
                                                 'proto/ni/measurementlink/pinmap/v1/*',
                                                 'proto/ni/measurementlink/sessionmanagement/v1/*']}
 
 install_requires = \
 ['grpcio>=1.49.1,<2.0.0', 'protobuf>=4.21,<5.0']
 
 extras_require = \
-{':sys_platform == "win32"': ['pywin32>=303,<304']}
+{':sys_platform == "win32"': ['pywin32>=303']}
 
 setup_kwargs = {
     'name': 'ni-measurementlink-service',
-    'version': '1.0.1',
+    'version': '1.1.0.dev0',
     'description': 'MeasurementLink Support for Python',
     'long_description': '# MeasurementLink™ Support for Python\n\n- [MeasurementLink™ Support for Python](#measurementlink--support-for-python)\n  - [Introduction](#introduction)\n  - [Dependencies](#dependencies)\n  - [Documentation](#documentation)\n  - [Examples](#examples)\n  - [Developing Measurements: Quick Start](#developing-measurements-quick-start)\n    - [Installation](#installation)\n    - [Developing a minimal python measurement](#developing-a-minimal-python-measurement)\n  - [Steps to run/debug the measurement service](#steps-to-rundebug-the-measurement-service)\n  - [Static Registration of Python Measurements](#static-registration-of-python-measurements)\n    - [Create a batch file that runs a python measurement](#create-a-batch-file-that-runs-a-python-measurement)\n    - [Create Executable for Python Scripts](#create-executable-for-python-scripts)\n  - [Appendix: Managing Measurement as Python Package (Project)](#appendix-managing-measurement-as-python-package-project)\n    - [Create and Manage Python Measurement Package using Poetry](#create-and-manage-python-measurement-package-using-poetry)\n    - [Create and Manage Python Measurement Package using `venv`](#create-and-manage-python-measurement-package-using-venv)\n    - [Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package](#create-and-manage-python-measurement-package-by-directly-installing-ni-measurementlink-service-as-a-system-level-package)\n\n---\n\n## Introduction\n\nMeasurementLink Support for Python (`ni-measurementlink-service`) is a Python framework that enables measurement developers to quickly create Python measurements and run them as a service (gRPC).\n\n---\n\n## Dependencies\n\n- Python >= 3.8 [(3.9 recommended)](https://www.python.org/downloads/release/python-3913/)\n- [grpcio >= 1.49.1, < 2.x](https://pypi.org/project/grpcio/1.49.1/)\n- [protobuf >= 4.21, < 5.x](https://pypi.org/project/protobuf/4.21.0/)\n- [pywin32 >= 303 (Only for Windows)](https://pypi.org/project/pywin32/303/)\n\n---\n\n## Documentation\n\n- [MeasurementLink Manual](https://www.ni.com/docs/en-US/bundle/measurementlink)\n- [API Reference](https://ni.github.io/measurementlink-python/)\n\n---\n\n## System Configuration\n\n### Enable Win32 Long Paths\n\nBy default, Windows has a path length limit of 260 characters. NI recommends enabling support for long paths when developing and deploying Python measurement services. \n\nThere are three ways to do this:\n- When installing Python using the Python for Windows installer, click `Disable path length limit` at the end of the installation.\n- Set the `Enable Win32 long paths` group policy:\n  - Run `gpedit.msc`.\n  - Expand `Computer Configuration` » `Administrative Templates` » `All Settings`.\n  - Find `Enable Win32 long paths` in the list, double-click it, and set it to `Enabled`.\n- In the Windows registry, set `HKEY_LOCAL_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\FileSystem\\LongPathsEnabled` (type: `REG_DWORD`) to 1. For more details, see [Maximum Path Length Limitation](https://learn.microsoft.com/en-us/windows/win32/fileio/maximum-file-path-limitation).\n\n---\n\n## Examples\n\nThe [`examples`](https://github.com/ni/measurementlink-python/tree/main/examples/) directory contains example measurement services. See the [README.md](https://github.com/ni/measurementlink-python/tree/main/examples/README.md) file for more information.\n\n---\n\n## Developing Measurements: Quick Start\n\nThis section provides instructions to develop custom measurement services in Python using MeasurementLink Support for Python.\n\n### Installation\n\nMake sure the system has the recommended Python version is installed. Install MeasurementLink Support for Python using [pip](https://pip.pypa.io/).\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-service\n```\n\nCheck if you have installed the expected version of MeasurementLink Support for Python installed by running the below command:\n\n```cmd\npip show ni-measurementlink-service\n```\n\n### Developing a minimal Python measurement\n\n1. Install the `ni-measurementlink-generator` package.\n\n``` cmd\nREM Activate the required virtual environment if any.\npip install ni-measurementlink-generator\n```\n\n2. Run the `ni-measurementlink-generator` tool. Use command line arguments to specify the `display-name` and optionally the `version`, `measurement-type`, and `product-type`.\n\n    1. Running `ni-measurementlink-generator` without optional arguments:\n\n    `ni-measurementlink-generator SampleMeasurement`\n\n    \'SampleMeasurement\' is the display name of your measurement service. Without the optional arguments,\n    the other arguments are generated for you based on the display name.\n\n    2. Running `ni-measurementlink-generator` with optional arguments for `measurement-version`, `ui-file`,\n    `service-class`, and `description-url`:\n\n    `ni-measurementlink-generator SampleMeasurement --measurement-version 0.1.0.0 --ui-file MeasurementUI.measui --service-class SampleMeasurement_Python --description-url https://www.example.com/SampleMeasurement.html`\n\n    3. Running `ni-measurementlink-generator` with optional argument for `directory-out`\n\n    `ni-measurementlink-generator SampleMeasurement --directory-out <new_path_for_created_files>`\n\n    If no output directory is specified, the files will\n    be placed in a new folder under the current directory\n    named after the display name without spaces.\n\n3. To customize the created measurement, provide metadata of the measurement\'s configuration (input parameters) and outputs (output parameters) in `measurement.py`.\n    1. Use the `configuration()` decorator to provide metadata about the configurations.**The order of the configuration decorator must match with the order of the parameters defined in the function signature.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        #Display Names can not contains backslash or front slash.\n        @foo_measurement_service.configuration("DisplayNameForInput1", DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", DataType.String, "DefaultValueForInput2")\n        def measure(input_1, input_2):\n            \'\'\' A simple Measurement method\'\'\'\n            return ["foo", "bar"]\n        ```\n\n    2. Use the `output()` decorator to provide metadata about the output.**The order of the output decorators from top to bottom must match the order of the values of the list returned by the function.**\n\n        ``` python\n        @foo_measurement_service.register_measurement\n        @foo_measurement_service.configuration("DisplayNameForInput1", nims.DataType.String, "DefaultValueForInput1")\n        @foo_measurement_service.configuration("DisplayNameForInput2", nims.DataType.String, "DefaultValueForInput2")\n        @foo_measurement_service.output("DisplayNameForOutput1", nims.DataType.String)\n        @foo_measurement_service.output("DisplayNameForOutput2", nims.DataType.String)\n        def measure(input_1, input_2):\n            return ["foo", "bar"]\n        ```\n\n4. Run/Debug the created measurement by following the steps discussed in the section ["Steps to run/debug the measurement service".](#steps-to-rundebug-the-measurement-service)\n\n---\n\n## Steps to run/debug the measurement service\n\n1. Start the discovery service if not already started.\n\n2. (Optional) Activate related virtual environments. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    .venv\\scripts\\activate\n    ```\n\n    - After successful activation, you can see the name of the environment, `(.venv)` is added to the command prompt.\n    - If you face an access issue when trying to activate, retry after allowing scripts to run as Administrator by executing the below command in Windows PowerShell:\n\n        ```cmd\n        Set-ExecutionPolicy RemoteSigned \n        ```\n\n3. [Run](https://code.visualstudio.com/docs/python/python-tutorial#_run-hello-world)/[Debug](https://code.visualstudio.com/docs/python/debugging#_basic-debugging) the measurement Python file.\n\n4. To stop the running measurement service, press `Enter` in the terminal to properly close the service.\n\n5. (Optional) After the usage of measurement, deactivate the virtual environment. Measurement developers can skip this step if they are not using any [virtual environments](#create-and-manage-python-measurement-package-using-venv) or [poetry-based projects.](#create-and-manage-python-measurement-package-using-poetry)\n\n    ```cmd\n    deactivate\n    ```\n\n---\n\n## Static Registration of Python Measurements\n\nThe MeasurementLink discovery service provides a registry of other services, and can discover and activate other services on the system. These features allow the discovery service to distinguish, manage, and describe measurement services on the system.\n\nTo statically register a measurement service with the MeasurementLink discovery service, do the following:\n\n1. Create a [startup batch file](#create-a-batch-file-that-runs-a-python-measurement) or [executable](#create-executable-for-python-scripts) for the measurement service.\n\n2. Edit the measurement service\'s `.serviceconfig` file and set the `path` value to the filename of the startup batch file or executable.\n\n3. Copy the measurement service\'s directory (including the `.venv` subdirectory if present, `.serviceconfig` file, and startup batch file) to a subdirectory of `C:\\ProgramData\\National Instruments\\MeasurementLink\\Services`. \n\nOnce your measurement service is statically registered, the MeasurementLink discovery service makes it visible in supported NI applications.\n\n### Create a batch file that runs a Python measurement\n\nThe batch file used for static registration is responsible for starting the Python Scripts.\n\nTypical Batch File:\n\n``` cmd\n"<path_to_python_exe>" "<path_to_measurement_file>"\n```\n\nExamples to start the fictitious file named `foo_measurement.py`:\n\n1. Using the Python system distribution\n\n    ```cmd\n    python foo_measurement.py\n    ```\n\n2. Using the virtual environment\n\n    ```cmd\n    REM Windows\n    .\\.venv\\Scripts\\python.exe foo_measurement.py\n\n    REM Linux \n    .venv/bin/python foo_measurement.py\n    ```\n\n### Create Executable for Python Scripts\n\nTo create an executable from a measurement, measurement authors can use the [pyinstaller](https://www.pyinstaller.org/) tooling. During the executable creation, the user can also embed the User Interface file using the `--add-data "<path_of_the_UI_File>;."`.\n\nTypical Pyinstaller command to build executable.\n\n```cmd\npyinstaller --onefile --console --add-data "<path_of_the_UI_File>;." --paths .venv\\Lib\\site-packages\\ <path_of_the_measurement_script>\n```\n\n## Troubleshooting\n\n### "File not found" or "No such file or directory" errors when copying or running a measurement service\n\nIf copying or running a measurement service produces "File not found" or "No such file or directory" errors, make sure to [enable Win32 long paths](#enable-win32-long-paths). If you are unable to enable Win32 long paths, consider deploying the measurement service to a directory with a shorter path.\n\n## Appendix: Managing Measurement as Python Package (Project)\n\nMeasurement and its related files can be maintained as a Python package. The basic components of any Python measurement package are:\n\n1. Measurement Python module (`.py` file)\n    - This file contains all the details related to the measurement and also contains the logic for the measurement execution.\n    - This file is run to start the measurement as a service.\n\n2. UI File\n    - UI file for the measurement. Types of supported UI files are:\n        - Measurement UI (`.measui`): created using the **MeasurementLink UI Editor** application.\n        - LabVIEW UI (`.vi`)\n    - The path of this file is configured by `ui_file_path` in `measurement_info` variable definition in measurement Python module (`.py`).\n\nPython communities have different ways of managing Python packages and their dependencies. It is up to the measurement developer to decide how to maintain the package and dependencies. Measurement developers can choose from a few common approaches discussed below based on their requirements.\n\n### Create and Manage Python Measurement Package using Poetry\n\n1. Install `poetry` (one-time setup)\n\n    1. Make sure the system has the recommended Python version installed.\n\n    2. Install `poetry` using the installation steps given in <https://python-poetry.org/docs/#installation>.\n\n2. Create a new Python project and add `ni-measurementlink-service` as a dependency to the project.\n\n    1. Open a command prompt, and change the working directory to the directory of your choice where you want to create the project.\n\n        ``` cmd\n        cd <path_of_directory_of_your_choice>\n        ```\n\n    2. Create a Python package (project) using the `poetry new` command. Poetry will create boilerplate files and folders that are commonly needed for a Python project.\n\n        ``` cmd\n        poetry new <name_of_the_project>\n        ```\n\n    3. Add the `ni-measurementlink-service` package as a dependency using the [`poetry add`](https://python-poetry.org/docs/cli/#add) command.\n\n        ``` cmd\n        cd <name_of_the_project>\n        poetry add ni-measurementlink-service\n        ```\n\n    4. The virtual environment will be auto-created by poetry.\n\n    5. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n        - Any additional dependencies required by measurement can be added using [add command](https://python-poetry.org/docs/cli/#add).\n\n            ``` cmd\n            poetry add <dependency_package_name>\n            ```\n\nFor detailed info on managing projects using poetry [refer to the official documentation](https://python-poetry.org/docs/cli/).\n\n### Create and Manage Python Measurement Package using `venv`\n\n1. Make sure the system has the recommended Python version installed.\n\n2. Open a command prompt, and change the working directory to the directory of your choice where you want to create a project.\n\n    ``` cmd\n    cd <path_of_directory_of_your_choice>\n    ```\n\n3. Create a virtual environment.\n\n    ``` cmd\n    REM This creates a virtual environment named .venv\n    python -m venv .venv\n    ```\n\n4. Activate the virtual environment. After successful activation\n\n    ``` cmd\n    .venv\\scripts\\activate\n    REM Optionally upgrade the pip within the venv by executing the command\n    python -m pip install -U pip\n    ```\n\n5. Install the `ni-measurementlink-service` package into the virtual environment.\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n6. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n    - Any additional dependencies required by measurement can be added pip install.\n\n        ``` cmd\n        pip install <dependency_package_name>\n        ```\n\nFor detailed info on managing projects with a virtual environment, refer to the [official documentation](https://docs.python.org/3/tutorial/venv.html).\n\n### Create and Manage Python Measurement Package by directly installing `ni-measurementlink-service` as a system-level package\n\nMeasurement developers can also install `ni-measurementlink-service` as a system package if necessary.\n\n1. Install the `ni-measurementlink-service` package from the command prompt\n\n    ``` cmd\n    pip install ni-measurementlink-service\n    ```\n\n2. Create measurement modules as described in ["Developing a minimal Python measurement"](#developing-a-minimal-python-measurement)\n\n---\n',
     'author': 'NI',
     'author_email': 'opensource@ni.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ni/measurementlink-python/',
```

### Comparing `ni_measurementlink_service-1.0.1/PKG-INFO` & `ni_measurementlink_service-1.1.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ni-measurementlink-service
-Version: 1.0.1
+Version: 1.1.0.dev0
 Summary: MeasurementLink Support for Python
 Home-page: https://github.com/ni/measurementlink-python/
 License: MIT
 Author: NI
 Author-email: opensource@ni.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Hardware
 Requires-Dist: grpcio (>=1.49.1,<2.0.0)
 Requires-Dist: protobuf (>=4.21,<5.0)
-Requires-Dist: pywin32 (>=303,<304); sys_platform == "win32"
+Requires-Dist: pywin32 (>=303); sys_platform == "win32"
 Project-URL: Repository, https://github.com/ni/measurementlink-python/
 Description-Content-Type: text/markdown
 
 # MeasurementLink™ Support for Python
 
 - [MeasurementLink™ Support for Python](#measurementlink--support-for-python)
   - [Introduction](#introduction)
```

