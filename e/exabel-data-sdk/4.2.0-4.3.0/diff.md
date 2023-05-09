# Comparing `tmp/exabel-data-sdk-4.2.0.tar.gz` & `tmp/exabel-data-sdk-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exabel-data-sdk-4.2.0.tar", last modified: Thu May  4 11:24:22 2023, max compression
+gzip compressed data, was "dist/exabel-data-sdk-4.3.0.tar", last modified: Tue May  9 08:08:15 2023, max compression
```

## Comparing `exabel-data-sdk-4.2.0.tar` & `exabel-data-sdk-4.3.0.tar`

### file list

```diff
@@ -1,411 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/library_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/user_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_insert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/paging_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_set_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/derived_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/library_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/namespace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/pageable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/prediction_model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/resource_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/search_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25471 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/time_series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/exabel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/client/user_login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/create_time_series_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/examples/get_company_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/query/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/base_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/command_line_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folder_accessors.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folders.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationship_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_entities_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_time_series_from_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/move_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/search_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/share_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_athena.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/sql_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/unshare_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_relationship_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_loading_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_relationship_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/entity_mapping_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    34075 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_writer_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_resource_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_namespace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_relationship_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_signal_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_time_series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/exabel_mock_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_exabel_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_command_line_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_excel_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_loading_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_writer_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/test_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_parse_property_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_type_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/case_insensitive_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/deprecate_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/handle_missing_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/parse_property_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/resource_name_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/exabel_data_sdk/util/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:24:22.000000 exabel-data-sdk-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-04 11:22:15.000000 exabel-data-sdk-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/entity_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/library_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/namespace_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/prediction_model_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/signal_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/tag_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/user_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/bulk_insert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/paging_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_set_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/derived_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/library_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/namespace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/pageable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/prediction_model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16290 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/resource_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/search_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/time_series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/exabel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/client/user_login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/examples/create_time_series_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/examples/get_company_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/query/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/base_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/command_line_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/csv_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_folder_accessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_relationship_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/load_entities_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/load_relationships_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/load_time_series_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/load_time_series_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/move_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/search_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/share_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/read_athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/read_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/read_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/sql_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/unshare_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/update_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/update_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/update_relationship_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_loading_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_relationship_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/entity_mapping_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_loading_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34306 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_time_series_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_writer_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/athena_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/sql_reader_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14383 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21787 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18779 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11807 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/math/all_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/time/all_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_resource_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_namespace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_relationship_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_signal_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_time_series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/exabel_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/query/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/test_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/test_exabel_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/test_user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_command_line_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35797 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23337 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27281 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_excel_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_loading_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_writer_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_parse_property_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_type_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/batcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/case_insensitive_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/deprecate_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/handle_missing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/parse_property_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/resource_name_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/exabel_data_sdk/util/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-09 08:08:14.000000 exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:08:14.000000 exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-09 08:08:14.000000 exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 08:08:14.000000 exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:08:15.000000 exabel-data-sdk-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-09 08:05:50.000000 exabel-data-sdk-4.3.0/setup.py
```

### Comparing `exabel-data-sdk-4.2.0/LICENSE` & `exabel-data-sdk-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/PKG-INFO` & `exabel-data-sdk-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 4.2.0
+Version: 4.3.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-4.2.0/README.md` & `exabel-data-sdk-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/data_set_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/derived_signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/entity_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/entity_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/exabel_api_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/base_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/data_set_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/derived_signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/entity_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/library_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/namespace_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/prediction_model_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/relationship_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/signal_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/tag_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/time_series_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/grpc/user_grpc_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/library_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/library_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/relationship_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/signal_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/signal_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/tag_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/tag_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/time_series_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/api_client/user_api_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/api_client/user_api_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_import.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/bulk_import.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/bulk_insert.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/bulk_insert.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/data_set.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/data_set.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/derived_signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/folder_accessor.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/folder_item.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/folder_item.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/group.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/namespace.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/namespace.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/paging_result.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/paging_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/request_error.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/request_error.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/tag.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/tag.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/time_series.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_classes/user.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/data_set_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/data_set_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/derived_signal_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/derived_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/entity_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/error_handler.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/error_handler.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/export_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/export_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         )
         if response.status_code == 200:
             return response.content
         error_message = response.content.decode()
         if error_message.startswith('"') and error_message.endswith('"'):
             error_message = error_message[1:-1]
         error_message = f"{response.status_code}: {error_message}"
-        raise Exception(error_message)
+        raise ValueError(error_message)
 
     def run_query(self, query: Union[str, Query]) -> pd.DataFrame:
         """
         Run an export data query, and returns a DataFrame with the results.
         Raises an exception if the status code is not 200.
         """
         content = self.run_query_bytes(query, file_format="pickle")
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/library_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/library_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/namespace_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/namespace_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/pageable_resource.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/pageable_resource.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/prediction_model_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/prediction_model_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/proto_utils.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/proto_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/relationship_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/resource_creation_result.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/resource_creation_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/search_service.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/search_service.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/signal_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/tag_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/time_series_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/time_series_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,14 @@
                             upload to be aborted; if it is `None`, the upload is never aborted.
 
         Returns:
             ResourceCreationResults containing the status for each time series that was imported.
         """
 
         def import_func(ts_sequence: Sequence[pd.Series]) -> Sequence[ResourceCreationResult]:
-
             result = self.import_time_series(
                 parent="signals/-",
                 series=ts_sequence,
                 default_known_time=default_known_time,
                 allow_missing=True,
                 create_tag=create_tag,
                 status_in_response=True,
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/api/user_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/client_config.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/client_config.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/exabel_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/exabel_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/client/user_login.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/client/user_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                 server_address = ("localhost", port)
                 handler = partial(TokenHandler, self)
                 httpd = HTTPServer(server_address, handler)
             except OSError as error:
                 if error.errno != errno.EADDRINUSE:
                     raise error
         if httpd is None:
-            raise Exception("Cannot start a local HTTP server to receive the login token.")
+            raise ValueError("Cannot start a local HTTP server to receive the login token.")
 
         thread = threading.Thread(target=httpd.serve_forever, daemon=True)
         thread.start()
         return httpd
 
     def read_refresh_token(self) -> None:
         """Read the refresh token from the user’s home directory."""
@@ -284,15 +284,15 @@
     def auth_headers(self) -> Dict[str, str]:
         """The authentication headers for HTTPS requests to the Exabel API."""
         return {"Authorization": f"Bearer {self.access_token}"}
 
     def get_auth_headers(self) -> Dict[str, str]:
         """Log in and get the authentication headers for HTTPS requests to the Exabel API."""
         if not self.log_in():
-            raise Exception("Failed to log in.")
+            raise ValueError("Failed to log in.")
         return self.auth_headers
 
 
 class TokenHandler(BaseHTTPRequestHandler):
     """HTTP reponse handler for Auth0 callbacks."""
 
     def __init__(self, login: UserLogin, *args: Any, **kwargs: Any):
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/examples/create_time_series_example.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/examples/create_time_series_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/examples/get_company_example.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/examples/get_company_example.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/query/column.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/query/column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/query/dashboard.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/query/dashboard.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/query/literal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/query/literal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/query/predicate.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/query/predicate.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/query/query.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/query/query.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/query/signals.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/query/signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/actions.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/actions.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/base_script.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/base_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/check_company_identifiers_in_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/command_line_script.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/command_line_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_derived_signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_entity_mapping_from_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
             default="entityTypes/company",
             help="The entity type to search for in the mapping",
         )
 
     def get_entity_mapping(
         self, client: ExabelClient, args: argparse.Namespace, mapping_input: pd.DataFrame
     ) -> pd.DataFrame:
-
         """
         Find the entity type we are creating mapping for.
 
         Check what type of mapping we are creating and call the relevant method.
 
         Args:
               client:        ExabelClient instance
@@ -218,15 +217,14 @@
         if market == "US":
             markets = ["XNAS", "XNYS", "XASE"]
         else:
             markets = [market]
         return markets
 
     def run_script(self, client: ExabelClient, args: argparse.Namespace) -> None:
-
         mapping_input = CsvReader.read_file(
             args.filename_input, separator=args.sep, string_columns=[0], keep_default_na=True
         )
         mapping_input = mapping_input.loc[0:, mapping_input.columns].drop_duplicates()
 
         try:
             mapping_output = self.get_entity_mapping(client, args, mapping_input)
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_prediction_model_run.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/create_signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/create_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/csv_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/csv_script_with_entity_mapping.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entities.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/delete_signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/delete_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/export_data.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/export_data.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_entity.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/get_time_series.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/get_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entities.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_entity_types.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_entity_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folder_accessors.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_folder_accessors.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_folders.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_folders.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_items.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationship_types.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_relationship_types.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_relationships.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_relationships.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_signals.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_signals.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/list_time_series.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/list_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_entities_from_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/load_entities_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_relationships_from_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/load_relationships_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/load_time_series_from_file.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/load_time_series_from_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,14 +115,24 @@
         self.parser.add_argument(
             "--skip-validation",
             required=False,
             action="store_true",
             default=False,
             help="If set, the time series are not validated before uploading.",
         )
+        self.parser.add_argument(
+            "--case-sensitive-signals",
+            required=False,
+            action="store_true",
+            default=False,
+            help="If set, signal names are treated case sensitive. Note that this will disable "
+            "lowercasing of other column headers as well, as entities, 'date', and "
+            "'known_time'. Take care to maintain correct casing in the file when using this "
+            "option.",
+        )
 
     def run_script(self, client: ExabelClient, args: argparse.Namespace) -> None:
         try:
             FileTimeSeriesLoader(client).load_time_series(
                 filename=args.filename,
                 entity_mapping_filename=args.entity_mapping_filename,
                 separator=args.sep,
@@ -134,14 +144,15 @@
                 create_tag=args.create_tag,
                 create_library_signal=args.create_library_signal,
                 threads=args.threads,
                 dry_run=args.dry_run,
                 retries=args.retries,
                 batch_size=args.batch_size,
                 skip_validation=args.skip_validation,
+                case_sensitive_signals=args.case_sensitive_signals,
             )
         except FileLoadingException as e:
             print(e)
             sys.exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/login.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/move_items.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/move_items.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/search_entities.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/search_entities.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/share_folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/share_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_athena.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/read_athena.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_bigquery.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/read_bigquery.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/read_snowflake.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/read_snowflake.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/sql/sql_script.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/sql/sql_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/unshare_folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/unshare_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/update_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/update_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/scripts/update_relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/scripts/update_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_entity_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_entity_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_reader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_relationship_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_relationship_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_time_series_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_time_series_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         global_time_series: Optional[bool] = None,
         threads: int = DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         skip_validation: bool = False,
+        case_sensitive_signals: bool = False,
         # Deprecated arguments
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> FileLoadingResult:
         """
         Load a CSV file and upload the time series to the Exabel Data API
 
         Args:
@@ -65,14 +66,15 @@
             dry_run: if True, the file is processed, but no time series are actually uploaded
             error_on_any_failure: if True, an  exception is raised if any time series failed to be
                 created
             retries: the maximum number of retries to make for each failed request
             abort_threshold: the threshold for the proportion of failed requests that will cause the
                  upload to be aborted; if it is `None`, the upload is never aborted
             skip_validation: if True, the time series are not validated before uploading
+            case_sensitive_signals: if True, signals are case sensitive
         """
         results = FileTimeSeriesLoader(self._client).load_time_series(
             filename=filename,
             entity_mapping_filename=entity_mapping_filename,
             separator=separator,
             pit_current_time=pit_current_time,
             pit_offset=pit_offset,
@@ -82,11 +84,12 @@
             global_time_series=global_time_series,
             threads=threads,
             dry_run=dry_run,
             error_on_any_failure=error_on_any_failure,
             retries=retries,
             abort_threshold=abort_threshold,
             skip_validation=skip_validation,
+            case_sensitive_signals=case_sensitive_signals,
         )
         if len(results) != 1:
             raise ValueError("Unexpected number of results from time series loading.")
         return results[0]
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/csv_writer.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/csv_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/entity_mapping_file_reader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/entity_mapping_file_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_exception.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_loading_exception.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_loading_result.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_loading_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_time_series_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         threads: int = DEFAULT_NUMBER_OF_THREADS_FOR_IMPORT,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         batch_size: Optional[int] = None,
         skip_validation: bool = False,
+        case_sensitive_signals: bool = False,
         return_results: bool = True,
         # Deprecated arguments
         namespace: Optional[str] = None,  # pylint: disable=unused-argument
     ) -> Sequence[TimeSeriesFileLoadingResult]:
         """
         Load a file and upload the time series to the Exabel Data API
 
@@ -100,14 +101,15 @@
                 created
             retries: the maximum number of retries to make for each failed request
             abort_threshold: the threshold for the proportion of failed requests that will cause the
                  upload to be aborted; if it is `None`, the upload is never aborted
             batch_size: the number of rows to read and upload in each batch; if not specified, the
                 entire file will be read into memory and uploaded in a single batch
             skip_validation: if True, the time series are not validated before uploading
+            case_sensitive_signals: if True, signals are case sensitive
         """
         if batch_size is not None:
             logger.info(
                 "Reading input data in batches of %d rows. File format with entities in columns is "
                 "not supported. Duplicate detection is best effort.",
                 batch_size,
             )
@@ -135,14 +137,15 @@
                 global_time_series=global_time_series,
                 threads=threads,
                 dry_run=dry_run,
                 error_on_any_failure=error_on_any_failure,
                 retries=retries,
                 abort_threshold=abort_threshold,
                 skip_validation=skip_validation,
+                case_sensitive_signals=case_sensitive_signals,
             )
             if return_results:
                 results.append(result)
         return results
 
     def _load_time_series(
         self,
@@ -159,14 +162,15 @@
         global_time_series: Optional[bool] = None,
         threads: int = DEFAULT_NUMBER_OF_THREADS,
         dry_run: bool = False,
         error_on_any_failure: bool = False,
         retries: int = DEFAULT_NUMBER_OF_RETRIES,
         abort_threshold: Optional[float] = 0.5,
         skip_validation: bool = False,
+        case_sensitive_signals: bool = False,
     ) -> TimeSeriesFileLoadingResult:
         """
         Load time series from a parser.
         """
         if dry_run:
             logger.info("Running dry-run...")
         if identifier_type and not entity_type:
@@ -200,14 +204,15 @@
             if candidate_class.can_parse(parser):
                 parsed_file = candidate_class.from_file(
                     parser,
                     self._client.entity_api,
                     self._client.namespace,
                     entity_mapping,
                     entity_type=identifier_type or entity_type,
+                    case_sensitive_signals=case_sensitive_signals,
                 )
                 break
         if parsed_file is None:
             parser.check_columns()
             raise FileLoadingException("Column and row setup not recognized.")
 
         if parsed_file.has_known_time():
@@ -260,30 +265,34 @@
         prefix = "signals/"
         if self._client.namespace:
             prefix += self._client.namespace + "."
 
         # Signals are reversed because we want to match the first signal returned by the API
         # lexicographically.
         all_signals = {
-            signal.name.lower(): signal
+            signal.name if case_sensitive_signals else signal.name.lower(): signal
             for signal in reversed(list(self._client.signal_api.get_signal_iterator()))
         }
 
         missing_signals = []
         signals_to_rename = {}
         for signal in signals:
-            lowered_signal_name = prefix + signal.lower()
-            if lowered_signal_name not in all_signals:
-                missing_signals.append(lowered_signal_name)
-                if isinstance(parsed_file, SignalNamesInRows) and signal != signal.lower():
+            signal_name = prefix + signal if case_sensitive_signals else prefix + signal.lower()
+            if signal_name not in all_signals:
+                missing_signals.append(signal_name)
+                if (
+                    not case_sensitive_signals
+                    and isinstance(parsed_file, SignalNamesInRows)
+                    and signal != signal.lower()
+                ):
                     signals_to_rename[signal] = signal.lower()
             else:
-                signal_match = all_signals[lowered_signal_name]
+                signal_match = all_signals[signal_name]
                 signal_name = signal_match.name.split(".")[-1]
-                if lowered_signal_name != signal_match.name or (
+                if signal_name != signal_match.name or (
                     isinstance(parsed_file, SignalNamesInRows) and signal != signal_name
                 ):
                     signals_to_rename[signal] = signal_name
 
         if missing_signals:
             logger.info("The following signals are missing:\n%s", missing_signals)
             if create_missing_signals:
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_time_series_parser.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_time_series_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,18 @@
         return self._preview
 
     def sheet_name(self) -> Optional[str]:
         """Return the name of the worksheet, when applicable."""
         return str(self.worksheet) if self.worksheet is not None else None
 
     def parse_file(
-        self, nrows: Optional[int] = None, header: Optional[Sequence[int]] = None
+        self,
+        nrows: Optional[int] = None,
+        header: Optional[Sequence[int]] = None,
+        case_sensitive_signals: bool = False,
     ) -> pd.DataFrame:
         """Parse the file as a Pandas data frame."""
         extension = Path(self.filename).suffix.lower()
         if self.data_frame is not None:
             if header is not None:
                 raise ValueError("Cannot specify header when uploading in batches.")
             if nrows is not None:
@@ -132,15 +135,15 @@
                 keep_default_na=True,
                 sheet_name=self.worksheet,
                 dtype={0: str},
                 engine="openpyxl",
             )
         else:
             raise FileLoadingException(f"Unknown file extension '{extension}'")
-        if not df.empty:
+        if not df.empty and not case_sensitive_signals:
             df = df.rename(lambda n: n.lower(), axis="columns", level=0)
         return df
 
     def check_columns(self) -> None:
         """
         Checks that the columns of the file are valid.
 
@@ -212,17 +215,18 @@
     def from_file(
         cls,
         file_parser: TimeSeriesFileParser,
         entity_api: EntityApi,
         namespace: str,
         entity_mapping: Optional[Mapping[str, Mapping[str, str]]] = None,
         entity_type: Optional[str] = None,
+        case_sensitive_signals: bool = False,
     ) -> "ParsedTimeSeriesFile":
         """Read a file and construct a parsed file from the contents."""
-        data = file_parser.parse_file()
+        data = file_parser.parse_file(case_sensitive_signals=case_sensitive_signals)
         return cls.from_data_frame(data, entity_api, namespace, entity_mapping, entity_type)
 
     @classmethod
     def from_data_frame(
         cls,
         data: pd.DataFrame,
         entity_api: EntityApi,
@@ -706,14 +710,15 @@
     def from_file(
         cls,
         file_parser: TimeSeriesFileParser,
         entity_api: EntityApi,
         namespace: str,
         entity_mapping: Optional[Mapping[str, Mapping[str, str]]] = None,
         entity_type: Optional[str] = None,
+        case_sensitive_signals: bool = False,
     ) -> "ParsedTimeSeriesFile":
         """Read a file and construct a new parser from the contents of that file."""
         if entity_type is not None:
             raise FileLoadingException("entity_type is not supported with this format")
         data = file_parser.parse_file(header=[0, 1])
         entity_type = data.columns.get_level_values(1)[0]
         data = cls._set_index(data)
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/file_writer_provider.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/file_writer_provider.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/athena_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/athena_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/bigquery_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/snowflake_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/sql_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/services/sql/sql_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/services/sql/sql_reader_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import abc
 import argparse
+from dataclasses import dataclass
 from typing import Any, Mapping, NamedTuple, NewType
 
 ConnectionString = NewType("ConnectionString", str)
 
 
 class EngineArgs(NamedTuple):
     """Arguments for creating a SQLAlchemy engine."""
 
     connection_string: ConnectionString
     kwargs: Mapping[str, Any]
 
 
+@dataclass
 class SqlReaderConfiguration(abc.ABC):
     """Base class for SQL reader configurations."""
 
     @classmethod
     @abc.abstractmethod
     def from_args(cls, args: argparse.Namespace) -> "SqlReaderConfiguration":
         """Construct a SQL reader configuration from the given command-line arguments."""
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/derived_signal_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/item_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/prediction_model_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/analytics/v1/tag_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/all_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/data_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/import_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/namespaces_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/relationship_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/search_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/signal_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/data/v1/time_series_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/folder_messages_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 _sym_db = _symbol_database.Default()
 from .....exabel.api.management.v1 import user_messages_pb2 as exabel_dot_api_dot_management_dot_v1_dot_user__messages__pb2
 from google.api import field_behavior_pb2 as google_dot_api_dot_field__behavior__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from .....protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/folder_messages.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xf3\x01\n\x06Folder\x120\n\x04name\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x120\n\x0cdisplay_name\x18\x02 \x01(\tB\x1a\xe0A\x02\x92A\x14J\x12"My shared folder"\x12\x12\n\x05write\x18\x03 \x01(\x08B\x03\xe0A\x03\x12;\n\x05items\x18\x04 \x03(\x0b2$.exabel.api.management.v1.FolderItemB\x06\xe0A\x06\xe0A\x03\x124\n\x0bdescription\x18\x05 \x01(\tB\x1f\x92A\x1cJ\x1a"This is my shared folder""\xf0\x02\n\nFolderItem\x122\n\x06parent\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12*\n\x04name\x18\x02 \x01(\tB\x1c\xe0A\x03\x92A\x16J\x14"derivedSignals/123"\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"my_signal"\x12\x13\n\x0bdescription\x18\t \x01(\t\x12;\n\titem_type\x18\x04 \x01(\x0e2(.exabel.api.management.v1.FolderItemType\x12/\n\x0bcreate_time\x18\x05 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\x06 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12\x12\n\nupdated_by\x18\x08 \x01(\t"O\n\x0eFolderAccessor\x12.\n\x05group\x18\x01 \x01(\x0b2\x1f.exabel.api.management.v1.Group\x12\r\n\x05write\x18\x02 \x01(\x08"B\n\x0cSearchResult\x122\n\x04item\x18\x01 \x01(\x0b2$.exabel.api.management.v1.FolderItem*\xc4\x01\n\x0eFolderItemType\x12\x1c\n\x18FOLDER_ITEM_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x14\n\x10PREDICTION_MODEL\x10\x02\x12\x16\n\x12PORTFOLIO_STRATEGY\x10\x03\x12\r\n\tDASHBOARD\x10\x04\x12\x0e\n\nDRILL_DOWN\x10\x05\x12\x07\n\x03TAG\x10\x06\x12\n\n\x06SCREEN\x10\x07\x12\x13\n\x0fFINANCIAL_MODEL\x10\x08\x12\t\n\x05CHART\x10\tBS\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.exabel/api/management/v1/folder_messages.proto\x12\x18exabel.api.management.v1\x1a,exabel/api/management/v1/user_messages.proto\x1a\x1fgoogle/api/field_behavior.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc_gen_openapiv2/options/annotations.proto"\xf3\x01\n\x06Folder\x120\n\x04name\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x120\n\x0cdisplay_name\x18\x02 \x01(\tB\x1a\xe0A\x02\x92A\x14J\x12"My shared folder"\x124\n\x0bdescription\x18\x05 \x01(\tB\x1f\x92A\x1cJ\x1a"This is my shared folder"\x12\x12\n\x05write\x18\x03 \x01(\x08B\x03\xe0A\x03\x12;\n\x05items\x18\x04 \x03(\x0b2$.exabel.api.management.v1.FolderItemB\x06\xe0A\x06\xe0A\x03"\xf0\x02\n\nFolderItem\x122\n\x06parent\x18\x01 \x01(\tB"\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName\x12*\n\x04name\x18\x02 \x01(\tB\x1c\xe0A\x03\x92A\x16J\x14"derivedSignals/123"\x12&\n\x0cdisplay_name\x18\x03 \x01(\tB\x10\x92A\rJ\x0b"my_signal"\x12\x13\n\x0bdescription\x18\t \x01(\t\x12;\n\titem_type\x18\x04 \x01(\x0e2(.exabel.api.management.v1.FolderItemType\x12/\n\x0bcreate_time\x18\x05 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12/\n\x0bupdate_time\x18\x06 \x01(\x0b2\x1a.google.protobuf.Timestamp\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12\x12\n\nupdated_by\x18\x08 \x01(\t"O\n\x0eFolderAccessor\x12.\n\x05group\x18\x01 \x01(\x0b2\x1f.exabel.api.management.v1.Group\x12\r\n\x05write\x18\x02 \x01(\x08"B\n\x0cSearchResult\x122\n\x04item\x18\x01 \x01(\x0b2$.exabel.api.management.v1.FolderItem*\xc4\x01\n\x0eFolderItemType\x12\x1c\n\x18FOLDER_ITEM_TYPE_INVALID\x10\x00\x12\x12\n\x0eDERIVED_SIGNAL\x10\x01\x12\x14\n\x10PREDICTION_MODEL\x10\x02\x12\x16\n\x12PORTFOLIO_STRATEGY\x10\x03\x12\r\n\tDASHBOARD\x10\x04\x12\x0e\n\nDRILL_DOWN\x10\x05\x12\x07\n\x03TAG\x10\x06\x12\n\n\x06SCREEN\x10\x07\x12\x13\n\x0fFINANCIAL_MODEL\x10\x08\x12\t\n\x05CHART\x10\tBS\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1b\x06proto3')
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'exabel.api.management.v1.folder_messages_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
     DESCRIPTOR._serialized_options = b'\n\x1ccom.exabel.api.management.v1B\x13FolderMessagesProtoP\x01Z\x1cexabel.com/api/management/v1'
     _FOLDER.fields_by_name['name']._options = None
     _FOLDER.fields_by_name['name']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _FOLDER.fields_by_name['display_name']._options = None
     _FOLDER.fields_by_name['display_name']._serialized_options = b'\xe0A\x02\x92A\x14J\x12"My shared folder"'
+    _FOLDER.fields_by_name['description']._options = None
+    _FOLDER.fields_by_name['description']._serialized_options = b'\x92A\x1cJ\x1a"This is my shared folder"'
     _FOLDER.fields_by_name['write']._options = None
     _FOLDER.fields_by_name['write']._serialized_options = b'\xe0A\x03'
     _FOLDER.fields_by_name['items']._options = None
     _FOLDER.fields_by_name['items']._serialized_options = b'\xe0A\x06\xe0A\x03'
-    _FOLDER.fields_by_name['description']._options = None
-    _FOLDER.fields_by_name['description']._serialized_options = b'\x92A\x1cJ\x1a"This is my shared folder"'
     _FOLDERITEM.fields_by_name['parent']._options = None
     _FOLDERITEM.fields_by_name['parent']._serialized_options = b'\x92A\x1fJ\r"folders/123"\xca>\r\xfa\x02\nfolderName'
     _FOLDERITEM.fields_by_name['name']._options = None
     _FOLDERITEM.fields_by_name['name']._serialized_options = b'\xe0A\x03\x92A\x16J\x14"derivedSignals/123"'
     _FOLDERITEM.fields_by_name['display_name']._options = None
     _FOLDERITEM.fields_by_name['display_name']._serialized_options = b'\x92A\rJ\x0b"my_signal"'
     _FOLDERITEMTYPE._serialized_start = 1003
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/library_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/management/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/math/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/exabel/api/time/time_range_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/stubs/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/api_client/test_exabel_api_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_data_set.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_derived_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_folder.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_accessor.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_folder_item.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_group.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_prediction_model_run.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_request_error.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_signal.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_tag.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_time_series.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/data_classes/test_user.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_entity_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_resource_store.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_resource_store.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/mock_signal_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/mock_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_bulk_insert_import.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_entity_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_entity_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_error_handler.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_export_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_export_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_namespace_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_namespace_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_pageable_resource.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_relationship_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_relationship_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_resource_creation_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_signal_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_signal_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/api/test_time_series_api.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/api/test_time_series_api.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/exabel_mock_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/exabel_mock_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/query/test_query.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/query/test_query.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_client_config.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/test_client_config.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_exabel_client.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/test_exabel_client.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/client/test_user_login.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/client/test_user_login.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/decorators.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/common_utils.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/common_utils.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/sql/test_read_snowflake.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/sql/test_sql_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_actions.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_actions.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_command_line_script.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_command_line_script.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_create_entity_mapping_from_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
         self.client.entity_api = mock.create_autospec(EntityApi)
         self.temp_file = tempfile.NamedTemporaryFile()  # pylint: disable=consider-using-with
 
     def tearDown(self):
         self.temp_file.close()
 
     def test_create_mapping_ticker(self):
-
         args = [
             "script-name",
             "--filename-input",
             "./exabel_data_sdk/tests/resources/data/mapping_ticker.csv",
             "--filename-output",
             self.temp_file.name,
             "--api-key",
@@ -73,15 +72,14 @@
         self.assertEqual(
             {"entity_type": "entityTypes/company", "mic": "XHKG", "ticker": "001"},
             kwargs,
             "Arguments not as expected",
         )
 
     def test_create_mapping_isin(self):
-
         args = [
             "script-name",
             "--filename-input",
             "./exabel_data_sdk/tests/resources/data/mapping_isin.csv",
             "--filename-output",
             self.temp_file.name,
             "--api-key",
@@ -97,15 +95,14 @@
         self.assertEqual(
             {"entity_type": "entityTypes/company", "isin": "NO0010096985"},
             kwargs,
             "Arguments not as expected",
         )
 
     def test_create_mapping_factset_identifier(self):
-
         args = [
             "script-name",
             "--filename-input",
             "./exabel_data_sdk/tests/resources/data/mapping_factset_identifier.csv",
             "--filename-output",
             self.temp_file.name,
             "--api-key",
@@ -130,15 +127,14 @@
         self.assertEqual(
             {"entity_type": "entityTypes/company", "factset_identifier": "DT699H-S"},
             kwargs,
             "Arguments not as expected",
         )
 
     def test_create_mapping_bloomberg_ticker(self):
-
         args = [
             "script-name",
             "--filename-input",
             "./exabel_data_sdk/tests/resources/data/mapping_bloomberg_ticker.csv",
             "--filename-output",
             self.temp_file.name,
             "--api-key",
@@ -163,15 +159,14 @@
         self.assertEqual(
             {"entity_type": "entityTypes/company", "bloomberg_ticker": "AMZN US"},
             kwargs,
             "Arguments not as expected",
         )
 
     def test_create_mapping_figi(self):
-
         args = [
             "script-name",
             "--filename-input",
             "./exabel_data_sdk/tests/resources/data/mapping_figi.csv",
             "--filename-output",
             self.temp_file.name,
             "--api-key",
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_create_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_create_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_delete_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_export_data.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_export_data.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_entities_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_relationships_from_csv.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_scripts.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_scripts.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -694,25 +694,178 @@
                 ),
                 name="entityTypes/brand/entities/ns.A_brand/signals/ns.SIGNAL1",
             ),
             series[0],
             check_freq=False,
         )
 
+    def test_load_time_series_with_uppercase_signals_not_existing_case_sensitive(self):
+        args = common_args + [
+            "--filename",
+            "./exabel_data_sdk/tests/resources/data/timeseries_with_mixedcase_columns.csv",
+            "--create-missing-signals",
+            "--case-sensitive-signals",
+        ]
+        script = LoadTimeSeriesFromFile(args)
+        self.client.signal_api.get_signal.return_value = None
+        self.client.signal_api.get_signal_iterator.side_effect = lambda *_: PagingResult([], "", 0)
+        self.client.entity_api.get_entity_type_iterator.side_effect = (
+            self._list_entity_types_uppercase
+        )
+
+        script.run_script(self.client, script.parse_arguments())
+
+        call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
+        self.assertEqual(1, len(call_args_list))
+        series = call_args_list[0][0][0]
+        self.assertEqual(1, len(series))
+        call_args_list_create_signal = self.client.signal_api.create_signal.call_args_list
+        self.assertEqual(1, len(call_args_list_create_signal))
+        signal = call_args_list_create_signal[0][0][0]
+        self.assertEqual("signals/ns.Signal1", signal.name)
+
+        pd.testing.assert_series_equal(
+            pd.Series(
+                [1, 2, 3, 4, 5],
+                pd.MultiIndex.from_arrays(
+                    [
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                    ]
+                ),
+                name="entityTypes/BRAND/entities/ns.A_brand/signals/ns.Signal1",
+            ),
+            series[0],
+            check_freq=False,
+        )
+
+    def test_load_time_series_with_uppercase_signals_and_lower_case_existing_case_sensitive(self):
+        args = common_args + [
+            "--filename",
+            "./exabel_data_sdk/tests/resources/data/timeseries_with_mixedcase_columns.csv",
+            "--create-missing-signals",
+            "--case-sensitive-signals",
+        ]
+        script = LoadTimeSeriesFromFile(args)
+        self.client.signal_api.get_signal_iterator.side_effect = self._list_signal
+        self.client.signal_api.get_signal.return_value = None
+        self.client.signal_api.get_signal_iterator.side_effect = lambda *_: PagingResult([], "", 0)
+        self.client.entity_api.get_entity_type_iterator.side_effect = (
+            self._list_entity_types_uppercase
+        )
+
+        script.run_script(self.client, script.parse_arguments())
+
+        call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
+        self.assertEqual(1, len(call_args_list))
+        series = call_args_list[0][0][0]
+        self.assertEqual(1, len(series))
+        call_args_list_create_signal = self.client.signal_api.create_signal.call_args_list
+        self.assertEqual(1, len(call_args_list_create_signal))
+        signal = call_args_list_create_signal[0][0][0]
+        self.assertEqual("signals/ns.Signal1", signal.name)
+
+        pd.testing.assert_series_equal(
+            pd.Series(
+                [1, 2, 3, 4, 5],
+                pd.MultiIndex.from_arrays(
+                    [
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                    ]
+                ),
+                name="entityTypes/BRAND/entities/ns.A_brand/signals/ns.Signal1",
+            ),
+            series[0],
+            check_freq=False,
+        )
+
+    def test_load_time_series_with_uppercase_signals_existing_case_sensitive(self):
+        args = common_args + [
+            "--filename",
+            "./exabel_data_sdk/tests/resources/data/timeseries_with_mixedcase_columns.csv",
+            "--create-missing-signals",
+            "--case-sensitive-signals",
+        ]
+        script = LoadTimeSeriesFromFile(args)
+        self.client.signal_api.get_signal_iterator.side_effect = self._list_signal_mixedcase
+        self.client.entity_api.get_entity_type_iterator.side_effect = self._list_entity_types
+        script.run_script(self.client, script.parse_arguments())
+
+        call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
+        self.assertEqual(1, len(call_args_list))
+        self.assertEqual(0, len(self.client.signal_api.create_signal.call_args_list))
+        series = call_args_list[0][0][0]
+        self.assertEqual(1, len(series))
+
+        pd.testing.assert_series_equal(
+            pd.Series(
+                [1, 2, 3, 4, 5],
+                pd.MultiIndex.from_arrays(
+                    [
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                    ]
+                ),
+                name="entityTypes/brand/entities/ns.A_brand/signals/ns.Signal1",
+            ),
+            series[0],
+            check_freq=False,
+        )
+
+    def test_load_time_series_with_mixedcase_signals_existing_and_entity_type_nonexisting_cs(
+        self,
+    ):
+        args = common_args + [
+            "--filename",
+            "./exabel_data_sdk/tests/resources/data/timeseries_with_mixedcase_columns.csv",
+            "--create-missing-signals",
+            "--case-sensitive",
+        ]
+        script = LoadTimeSeriesFromFile(args)
+        self.client.signal_api.get_signal_iterator.side_effect = self._list_signal_mixedcase
+        self.client.entity_api.get_entity_type_iterator.side_effect = self._list_entity_types
+
+        script.run_script(self.client, script.parse_arguments())
+
+        call_args_list = self.client.time_series_api.bulk_upsert_time_series.call_args_list
+        self.assertEqual(1, len(call_args_list))
+        self.assertEqual(0, len(self.client.signal_api.create_signal.call_args_list))
+        series = call_args_list[0][0][0]
+        self.assertEqual(1, len(series))
+
+        pd.testing.assert_series_equal(
+            pd.Series(
+                [1, 2, 3, 4, 5],
+                pd.MultiIndex.from_arrays(
+                    [
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                        pd.date_range("2021-01-01", periods=5, tz=tz.tzutc()),
+                    ]
+                ),
+                name="entityTypes/brand/entities/ns.A_brand/signals/ns.Signal1",
+            ),
+            series[0],
+            check_freq=False,
+        )
+
     def _list_signal(self):
         return iter(
             [
                 Signal("signals/ns.signal1", "The Signal", "A description of the signal"),
                 Signal("signals/ns.signal2", "The Other Signal", "A description of the signal"),
             ]
         )
 
     def _list_signal_uppercase(self):
         return iter([Signal("signals/ns.SIGNAL1", "The Signal", "A description of the signal")])
 
+    def _list_signal_mixedcase(self):
+        return iter([Signal("signals/ns.Signal1", "The Signal", "A description of the signal")])
+
     def _list_entity_types(self):
         return iter([EntityType("entityTypes/brand", "", "", False)])
 
     def _list_entity_types_uppercase(self):
         return iter([EntityType("entityTypes/BRAND", "", "", False)])
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_load_time_series_from_excel.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_update_entity_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/scripts/test_update_relationship_type.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_athena_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_bigquery_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_snowflake_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_sql_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/sql/test_sql_reader_configuration.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_entity_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_reader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_relationship_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_csv_writer.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_entity_mapping_file_reader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_excel_writer.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_excel_writer.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_loading_result.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_loading_result.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_time_series_loader.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_time_series_parser.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/services/test_file_writer_provider.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/services/test_file_writer_provider.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/test_decorators.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_batcher.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_batcher.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_deprecate_arguments.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_handle_missing_imports.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_parse_property_columns.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_parse_property_columns.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_resource_name_normalization.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/tests/util/test_type_converter.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/tests/util/test_type_converter.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/util/case_insensitive_column.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/util/case_insensitive_column.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/util/deprecate_arguments.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/util/deprecate_arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import warnings
 from typing import Any, Callable, Optional, TypeVar, overload
 
 from exabel_data_sdk.util.warnings import ExabelDeprecationWarning
 
 FunctionT = TypeVar("FunctionT", bound=Callable[..., Any])
 
+
 # Pylint flags '__func' as an invalid argument name, but we want the '__' prefix to make Mypy
 # interpret it as a positional-only argument. Therefore, we disable the check for this argument.
 @overload
 def deprecate_arguments(
     **deprecation_replacements: Optional[str],
 ) -> Callable[[FunctionT], FunctionT]:
     ...
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/util/handle_missing_imports.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/util/handle_missing_imports.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/util/import_.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/util/import_.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/util/parse_property_columns.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/util/parse_property_columns.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/util/resource_name_normalization.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/util/resource_name_normalization.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk/util/type_converter.py` & `exabel-data-sdk-4.3.0/exabel_data_sdk/util/type_converter.py`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/PKG-INFO` & `exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exabel-data-sdk
-Version: 4.2.0
+Version: 4.3.0
 Summary: Python SDK for the Exabel Data API
 Home-page: https://github.com/Exabel/python-sdk
 Author: Exabel
 Author-email: support@exabel.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `exabel-data-sdk-4.2.0/exabel_data_sdk.egg-info/SOURCES.txt` & `exabel-data-sdk-4.3.0/exabel_data_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/pyproject.toml` & `exabel-data-sdk-4.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exabel-data-sdk-4.2.0/setup.py` & `exabel-data-sdk-4.3.0/setup.py`

 * *Files identical despite different names*

