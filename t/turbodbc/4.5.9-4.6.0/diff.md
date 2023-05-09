# Comparing `tmp/turbodbc-4.5.9.tar.gz` & `tmp/turbodbc-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbodbc-4.5.9.tar", last modified: Tue Feb 21 12:39:22 2023, max compression
+gzip compressed data, was "turbodbc-4.6.0.tar", last modified: Tue May  9 09:50:37 2023, max compression
```

## Comparing `turbodbc-4.5.9.tar` & `turbodbc-4.6.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.773481 turbodbc-4.5.9/
--rw-r--r--   0 root         (0) root         (0)    20393 2020-04-16 12:00:00.000000 turbodbc-4.5.9/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     1087 2020-04-16 12:00:00.000000 turbodbc-4.5.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       96 2020-04-16 12:00:00.000000 turbodbc-4.5.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3481 2023-02-21 12:39:22.773481 turbodbc-4.5.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2523 2020-04-16 12:00:00.000000 turbodbc-4.5.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.729480 turbodbc-4.5.9/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.733480 turbodbc-4.5.9/include/cpp_odbc/
--rw-r--r--   0 root         (0) root         (0)      957 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/column_description.h
--rw-r--r--   0 root         (0) root         (0)     2554 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/connection.h
--rw-r--r--   0 root         (0) root         (0)      893 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/cpp_odbc.h
--rw-r--r--   0 root         (0) root         (0)      512 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/credentials.h
--rw-r--r--   0 root         (0) root         (0)     1377 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/environment.h
--rw-r--r--   0 root         (0) root         (0)      551 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/error.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.737480 turbodbc-4.5.9/include/cpp_odbc/level1/
--rw-r--r--   0 root         (0) root         (0)    11658 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level1/api.h
--rw-r--r--   0 root         (0) root         (0)      506 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level1/level1.h
--rw-r--r--   0 root         (0) root         (0)     4792 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level1/unixodbc_backend.h
--rw-r--r--   0 root         (0) root         (0)     4810 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level1/unixodbc_backend_debug.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.737480 turbodbc-4.5.9/include/cpp_odbc/level2/
--rw-r--r--   0 root         (0) root         (0)    19100 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/api.h
--rw-r--r--   0 root         (0) root         (0)      636 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/diagnostic_record.h
--rw-r--r--   0 root         (0) root         (0)     1286 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/fixed_length_string_buffer.h
--rw-r--r--   0 root         (0) root         (0)     2498 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/handles.h
--rw-r--r--   0 root         (0) root         (0)      838 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/input_string_buffer.h
--rw-r--r--   0 root         (0) root         (0)      855 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/input_u16string_buffer.h
--rw-r--r--   0 root         (0) root         (0)     4565 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/level1_connector.h
--rw-r--r--   0 root         (0) root         (0)      736 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/level2.h
--rw-r--r--   0 root         (0) root         (0)     1435 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/string_buffer.h
--rw-r--r--   0 root         (0) root         (0)     1513 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level2/u16string_buffer.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.737480 turbodbc-4.5.9/include/cpp_odbc/level3/
--rw-r--r--   0 root         (0) root         (0)      588 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level3/level3.h
--rw-r--r--   0 root         (0) root         (0)     1909 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level3/raii_connection.h
--rw-r--r--   0 root         (0) root         (0)     1323 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level3/raii_environment.h
--rw-r--r--   0 root         (0) root         (0)     2606 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/level3/raii_statement.h
--rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/make_environment.h
--rw-r--r--   0 root         (0) root         (0)     3045 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/multi_value_buffer.h
--rw-r--r--   0 root         (0) root         (0)     7841 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/cpp_odbc/statement.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.741480 turbodbc-4.5.9/include/turbodbc/
--rw-r--r--   0 root         (0) root         (0)     1443 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/buffer_size.h
--rw-r--r--   0 root         (0) root         (0)     1241 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/column.h
--rw-r--r--   0 root         (0) root         (0)      217 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/column_info.h
--rw-r--r--   0 root         (0) root         (0)     1602 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/command.h
--rw-r--r--   0 root         (0) root         (0)      842 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/configuration.h
--rw-r--r--   0 root         (0) root         (0)      486 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/connect.h
--rw-r--r--   0 root         (0) root         (0)     1427 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/connection.h
--rw-r--r--   0 root         (0) root         (0)     1093 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/cursor.h
--rw-r--r--   0 root         (0) root         (0)     1640 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/description.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.741480 turbodbc-4.5.9/include/turbodbc/descriptions/
--rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions/boolean_description.h
--rw-r--r--   0 root         (0) root         (0)      537 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions/date_description.h
--rw-r--r--   0 root         (0) root         (0)      615 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions/floating_point_description.h
--rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions/integer_description.h
--rw-r--r--   0 root         (0) root         (0)      693 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions/string_description.h
--rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions/timestamp_description.h
--rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions/unicode_description.h
--rw-r--r--   0 root         (0) root         (0)      404 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/descriptions.h
--rw-r--r--   0 root         (0) root         (0)      230 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/errors.h
--rw-r--r--   0 root         (0) root         (0)      746 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field.h
--rw-r--r--   0 root         (0) root         (0)      711 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translator.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.745480 turbodbc-4.5.9/include/turbodbc/field_translators/
--rw-r--r--   0 root         (0) root         (0)      372 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translators/boolean_translator.h
--rw-r--r--   0 root         (0) root         (0)      354 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translators/date_translator.h
--rw-r--r--   0 root         (0) root         (0)      386 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translators/float64_translator.h
--rw-r--r--   0 root         (0) root         (0)      373 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translators/int64_translator.h
--rw-r--r--   0 root         (0) root         (0)      368 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translators/string_translator.h
--rw-r--r--   0 root         (0) root         (0)      374 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translators/timestamp_translator.h
--rw-r--r--   0 root         (0) root         (0)      364 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/field_translators.h
--rw-r--r--   0 root         (0) root         (0)     1019 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/make_description.h
--rw-r--r--   0 root         (0) root         (0)      316 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/make_field_translator.h
--rw-r--r--   0 root         (0) root         (0)     1761 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/parameter.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.745480 turbodbc-4.5.9/include/turbodbc/parameter_sets/
--rw-r--r--   0 root         (0) root         (0)     2469 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/parameter_sets/bound_parameter_set.h
--rw-r--r--   0 root         (0) root         (0)      745 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/parameter_sets/field_parameter_set.h
--rw-r--r--   0 root         (0) root         (0)      704 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/parameter_sets/set_field.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.745480 turbodbc-4.5.9/include/turbodbc/result_sets/
--rw-r--r--   0 root         (0) root         (0)     1254 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/result_sets/bound_result_set.h
--rw-r--r--   0 root         (0) root         (0)     2327 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/result_sets/double_buffered_result_set.h
--rw-r--r--   0 root         (0) root         (0)      971 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/result_sets/field_result_set.h
--rw-r--r--   0 root         (0) root         (0)     1256 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/result_sets/result_set.h
--rw-r--r--   0 root         (0) root         (0)     1028 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/result_sets/row_based_result_set.h
--rw-r--r--   0 root         (0) root         (0)      157 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/string_helpers.h
--rw-r--r--   0 root         (0) root         (0)     1190 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/time_helpers.h
--rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc/type_code.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.745480 turbodbc-4.5.9/include/turbodbc_arrow/
--rw-r--r--   0 root         (0) root         (0)     1674 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_arrow/arrow_result_set.h
--rw-r--r--   0 root         (0) root         (0)      297 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_arrow/set_arrow_parameters.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.749481 turbodbc-4.5.9/include/turbodbc_numpy/
--rw-r--r--   0 root         (0) root         (0)      556 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/binary_column.h
--rw-r--r--   0 root         (0) root         (0)      683 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/datetime_column.h
--rw-r--r--   0 root         (0) root         (0)      378 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/make_numpy_array.h
--rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/masked_column.h
--rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/ndarrayobject.h
--rw-r--r--   0 root         (0) root         (0)      756 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/numpy_result_set.h
--rw-r--r--   0 root         (0) root         (0)      260 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/numpy_type.h
--rw-r--r--   0 root         (0) root         (0)      299 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/set_numpy_parameters.h
--rw-r--r--   0 root         (0) root         (0)      508 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/string_column.h
--rw-r--r--   0 root         (0) root         (0)      511 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_numpy/unicode_column.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.749481 turbodbc-4.5.9/include/turbodbc_python/
--rw-r--r--   0 root         (0) root         (0)      454 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_python/determine_parameter_type.h
--rw-r--r--   0 root         (0) root         (0)      685 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_python/python_parameter_set.h
--rw-r--r--   0 root         (0) root         (0)      885 2020-04-16 12:00:00.000000 turbodbc-4.5.9/include/turbodbc_python/python_result_set.h
--rw-r--r--   0 root         (0) root         (0)      155 2023-02-21 12:39:22.777481 turbodbc-4.5.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    10145 2020-04-16 12:00:00.000000 turbodbc-4.5.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.733480 turbodbc-4.5.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.753481 turbodbc-4.5.9/src/cpp_odbc/
--rw-r--r--   0 root         (0) root         (0)     2694 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/column_description.cpp
--rw-r--r--   0 root         (0) root         (0)      802 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/connection.cpp
--rw-r--r--   0 root         (0) root         (0)      190 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/cpp_odbc.cpp
--rw-r--r--   0 root         (0) root         (0)      411 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/environment.cpp
--rw-r--r--   0 root         (0) root         (0)      744 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/error.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.753481 turbodbc-4.5.9/src/cpp_odbc/level1/
--rw-r--r--   0 root         (0) root         (0)     7405 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level1/api.cpp
--rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level1/level1.cpp
--rw-r--r--   0 root         (0) root         (0)     7663 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level1/unixodbc_backend.cpp
--rw-r--r--   0 root         (0) root         (0)    12404 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level1/unixodbc_backend_debug.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.753481 turbodbc-4.5.9/src/cpp_odbc/level2/
--rw-r--r--   0 root         (0) root         (0)     5853 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/api.cpp
--rw-r--r--   0 root         (0) root         (0)     1265 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/handles.cpp
--rw-r--r--   0 root         (0) root         (0)      419 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/input_string_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)      457 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/input_u16string_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)    16753 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/level1_connector.cpp
--rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/level2.cpp
--rw-r--r--   0 root         (0) root         (0)      595 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/string_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)      621 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level2/u16string_buffer.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.753481 turbodbc-4.5.9/src/cpp_odbc/level3/
--rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level3/level3.cpp
--rw-r--r--   0 root         (0) root         (0)     3649 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level3/raii_connection.cpp
--rw-r--r--   0 root         (0) root         (0)     1623 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level3/raii_environment.cpp
--rw-r--r--   0 root         (0) root         (0)     3845 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/level3/raii_statement.cpp
--rw-r--r--   0 root         (0) root         (0)      949 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/make_environment.cpp
--rw-r--r--   0 root         (0) root         (0)     1816 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/multi_value_buffer.cpp
--rw-r--r--   0 root         (0) root         (0)     2787 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/cpp_odbc/statement.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.757481 turbodbc-4.5.9/src/turbodbc/
--rw-r--r--   0 root         (0) root         (0)     1218 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/buffer_size.cpp
--rw-r--r--   0 root         (0) root         (0)      963 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/column.cpp
--rw-r--r--   0 root         (0) root         (0)     1805 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/command.cpp
--rw-r--r--   0 root         (0) root         (0)      901 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/configuration.cpp
--rw-r--r--   0 root         (0) root         (0)      298 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/connect.cpp
--rw-r--r--   0 root         (0) root         (0)     1136 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/connection.cpp
--rw-r--r--   0 root         (0) root         (0)     1941 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/cursor.cpp
--rw-r--r--   0 root         (0) root         (0)      830 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/description.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.761481 turbodbc-4.5.9/src/turbodbc/descriptions/
--rw-r--r--   0 root         (0) root         (0)      783 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/descriptions/boolean_description.cpp
--rw-r--r--   0 root         (0) root         (0)      784 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/descriptions/date_description.cpp
--rw-r--r--   0 root         (0) root         (0)      899 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/descriptions/floating_point_description.cpp
--rw-r--r--   0 root         (0) root         (0)      810 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/descriptions/integer_description.cpp
--rw-r--r--   0 root         (0) root         (0)      915 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/descriptions/string_description.cpp
--rw-r--r--   0 root         (0) root         (0)      864 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/descriptions/timestamp_description.cpp
--rw-r--r--   0 root         (0) root         (0)      993 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/descriptions/unicode_description.cpp
--rw-r--r--   0 root         (0) root         (0)      211 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/errors.cpp
--rw-r--r--   0 root         (0) root         (0)      393 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/field_translator.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.761481 turbodbc-4.5.9/src/turbodbc/field_translators/
--rw-r--r--   0 root         (0) root         (0)      380 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/field_translators/boolean_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      483 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/field_translators/date_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      414 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/field_translators/float64_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      403 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/field_translators/int64_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      389 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/field_translators/string_translator.cpp
--rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/field_translators/timestamp_translator.cpp
--rw-r--r--   0 root         (0) root         (0)     7166 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/make_description.cpp
--rw-r--r--   0 root         (0) root         (0)      972 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/make_field_translator.cpp
--rw-r--r--   0 root         (0) root         (0)     1820 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/parameter.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.761481 turbodbc-4.5.9/src/turbodbc/parameter_sets/
--rw-r--r--   0 root         (0) root         (0)     4834 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/parameter_sets/bound_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)     2680 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/parameter_sets/field_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)     3552 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/parameter_sets/set_field.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.761481 turbodbc-4.5.9/src/turbodbc/result_sets/
--rw-r--r--   0 root         (0) root         (0)     3054 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/result_sets/bound_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)     2929 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/result_sets/double_buffered_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      856 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/result_sets/field_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      481 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/result_sets/result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      985 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/result_sets/row_based_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      436 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/string_helpers.cpp
--rw-r--r--   0 root         (0) root         (0)     3200 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc/time_helpers.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.765481 turbodbc-4.5.9/src/turbodbc_arrow/
--rw-r--r--   0 root         (0) root         (0)    15431 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_arrow/arrow_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)     1113 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_arrow/python_bindings.cpp
--rw-r--r--   0 root         (0) root         (0)    19064 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_arrow/set_arrow_parameters.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.765481 turbodbc-4.5.9/src/turbodbc_numpy/
--rw-r--r--   0 root         (0) root         (0)     1907 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/binary_column.cpp
--rw-r--r--   0 root         (0) root         (0)     2492 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/datetime_column.cpp
--rw-r--r--   0 root         (0) root         (0)     2304 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/make_numpy_array.cpp
--rw-r--r--   0 root         (0) root         (0)      431 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/masked_column.cpp
--rw-r--r--   0 root         (0) root         (0)     2434 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/numpy_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)      327 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/numpy_type.cpp
--rw-r--r--   0 root         (0) root         (0)     1396 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/python_bindings.cpp
--rw-r--r--   0 root         (0) root         (0)    15127 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/set_numpy_parameters.cpp
--rw-r--r--   0 root         (0) root         (0)     1077 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/string_column.cpp
--rw-r--r--   0 root         (0) root         (0)     1092 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_numpy/unicode_column.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.765481 turbodbc-4.5.9/src/turbodbc_python/
--rw-r--r--   0 root         (0) root         (0)     4027 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/determine_parameter_type.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.769481 turbodbc-4.5.9/src/turbodbc_python/python_bindings/
--rw-r--r--   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/buffer_size.cpp
--rw-r--r--   0 root         (0) root         (0)      505 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/column_info.cpp
--rw-r--r--   0 root         (0) root         (0)      205 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/connect.cpp
--rw-r--r--   0 root         (0) root         (0)      560 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/connection.cpp
--rw-r--r--   0 root         (0) root         (0)      701 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/cursor.cpp
--rw-r--r--   0 root         (0) root         (0)      340 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/error.cpp
--rw-r--r--   0 root         (0) root         (0)     1155 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/module.cpp
--rw-r--r--   0 root         (0) root         (0)     2786 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/options.cpp
--rw-r--r--   0 root         (0) root         (0)      568 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/python_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)      913 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_bindings/python_result_set.cpp
--rw-r--r--   0 root         (0) root         (0)     3004 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_parameter_set.cpp
--rw-r--r--   0 root         (0) root         (0)     3469 2020-04-16 12:00:00.000000 turbodbc-4.5.9/src/turbodbc_python/python_result_set.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.773481 turbodbc-4.5.9/turbodbc/
--rw-r--r--   0 root         (0) root         (0)      826 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      154 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/api_constants.py
--rw-r--r--   0 root         (0) root         (0)      247 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/arrow_support.py
--rw-r--r--   0 root         (0) root         (0)     1949 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/connect.py
--rw-r--r--   0 root         (0) root         (0)     1871 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/connection.py
--rw-r--r--   0 root         (0) root         (0)      286 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/constructors.py
--rw-r--r--   0 root         (0) root         (0)    15873 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/cursor.py
--rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/data_types.py
--rw-r--r--   0 root         (0) root         (0)      990 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6269 2020-04-16 12:00:00.000000 turbodbc-4.5.9/turbodbc/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-21 12:39:22.773481 turbodbc-4.5.9/turbodbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3481 2023-02-21 12:39:22.000000 turbodbc-4.5.9/turbodbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7302 2023-02-21 12:39:22.000000 turbodbc-4.5.9/turbodbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-21 12:39:22.000000 turbodbc-4.5.9/turbodbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-02-21 12:39:22.000000 turbodbc-4.5.9/turbodbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-02-21 12:39:22.000000 turbodbc-4.5.9/turbodbc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.542194 turbodbc-4.6.0/
+-rw-r--r--   0 root         (0) root         (0)    20707 2020-04-16 12:00:00.000000 turbodbc-4.6.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     1087 2020-04-16 12:00:00.000000 turbodbc-4.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       96 2020-04-16 12:00:00.000000 turbodbc-4.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-05-09 09:50:37.542194 turbodbc-4.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2523 2020-04-16 12:00:00.000000 turbodbc-4.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.494193 turbodbc-4.6.0/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.502193 turbodbc-4.6.0/include/cpp_odbc/
+-rw-r--r--   0 root         (0) root         (0)      957 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/column_description.h
+-rw-r--r--   0 root         (0) root         (0)     2554 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/connection.h
+-rw-r--r--   0 root         (0) root         (0)      893 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/cpp_odbc.h
+-rw-r--r--   0 root         (0) root         (0)      512 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/credentials.h
+-rw-r--r--   0 root         (0) root         (0)     1377 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/environment.h
+-rw-r--r--   0 root         (0) root         (0)      551 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/error.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.502193 turbodbc-4.6.0/include/cpp_odbc/level1/
+-rw-r--r--   0 root         (0) root         (0)    11658 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level1/api.h
+-rw-r--r--   0 root         (0) root         (0)      506 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level1/level1.h
+-rw-r--r--   0 root         (0) root         (0)     4792 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level1/unixodbc_backend.h
+-rw-r--r--   0 root         (0) root         (0)     4810 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level1/unixodbc_backend_debug.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.502193 turbodbc-4.6.0/include/cpp_odbc/level2/
+-rw-r--r--   0 root         (0) root         (0)    19100 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/api.h
+-rw-r--r--   0 root         (0) root         (0)      636 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/diagnostic_record.h
+-rw-r--r--   0 root         (0) root         (0)     1286 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/fixed_length_string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     2498 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/handles.h
+-rw-r--r--   0 root         (0) root         (0)      838 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/input_string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)      855 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/input_u16string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     4565 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/level1_connector.h
+-rw-r--r--   0 root         (0) root         (0)      736 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/level2.h
+-rw-r--r--   0 root         (0) root         (0)     1435 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/string_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     1513 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level2/u16string_buffer.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.506193 turbodbc-4.6.0/include/cpp_odbc/level3/
+-rw-r--r--   0 root         (0) root         (0)      588 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level3/level3.h
+-rw-r--r--   0 root         (0) root         (0)     1909 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level3/raii_connection.h
+-rw-r--r--   0 root         (0) root         (0)     1323 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level3/raii_environment.h
+-rw-r--r--   0 root         (0) root         (0)     2606 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/level3/raii_statement.h
+-rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/make_environment.h
+-rw-r--r--   0 root         (0) root         (0)     3045 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/multi_value_buffer.h
+-rw-r--r--   0 root         (0) root         (0)     7841 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/cpp_odbc/statement.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.506193 turbodbc-4.6.0/include/turbodbc/
+-rw-r--r--   0 root         (0) root         (0)     1443 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/buffer_size.h
+-rw-r--r--   0 root         (0) root         (0)     1241 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/column.h
+-rw-r--r--   0 root         (0) root         (0)      217 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/column_info.h
+-rw-r--r--   0 root         (0) root         (0)     1602 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/command.h
+-rw-r--r--   0 root         (0) root         (0)      842 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/configuration.h
+-rw-r--r--   0 root         (0) root         (0)      486 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/connect.h
+-rw-r--r--   0 root         (0) root         (0)     1427 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/connection.h
+-rw-r--r--   0 root         (0) root         (0)     1093 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/cursor.h
+-rw-r--r--   0 root         (0) root         (0)     1640 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/description.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.510193 turbodbc-4.6.0/include/turbodbc/descriptions/
+-rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions/boolean_description.h
+-rw-r--r--   0 root         (0) root         (0)      537 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions/date_description.h
+-rw-r--r--   0 root         (0) root         (0)      615 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions/floating_point_description.h
+-rw-r--r--   0 root         (0) root         (0)      552 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions/integer_description.h
+-rw-r--r--   0 root         (0) root         (0)      693 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions/string_description.h
+-rw-r--r--   0 root         (0) root         (0)      562 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions/timestamp_description.h
+-rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions/unicode_description.h
+-rw-r--r--   0 root         (0) root         (0)      404 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/descriptions.h
+-rw-r--r--   0 root         (0) root         (0)      230 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/errors.h
+-rw-r--r--   0 root         (0) root         (0)      746 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field.h
+-rw-r--r--   0 root         (0) root         (0)      711 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translator.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.510193 turbodbc-4.6.0/include/turbodbc/field_translators/
+-rw-r--r--   0 root         (0) root         (0)      372 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translators/boolean_translator.h
+-rw-r--r--   0 root         (0) root         (0)      354 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translators/date_translator.h
+-rw-r--r--   0 root         (0) root         (0)      386 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translators/float64_translator.h
+-rw-r--r--   0 root         (0) root         (0)      373 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translators/int64_translator.h
+-rw-r--r--   0 root         (0) root         (0)      368 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translators/string_translator.h
+-rw-r--r--   0 root         (0) root         (0)      374 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translators/timestamp_translator.h
+-rw-r--r--   0 root         (0) root         (0)      364 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/field_translators.h
+-rw-r--r--   0 root         (0) root         (0)     1019 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/make_description.h
+-rw-r--r--   0 root         (0) root         (0)      316 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/make_field_translator.h
+-rw-r--r--   0 root         (0) root         (0)     1761 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/parameter.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.510193 turbodbc-4.6.0/include/turbodbc/parameter_sets/
+-rw-r--r--   0 root         (0) root         (0)     2469 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/parameter_sets/bound_parameter_set.h
+-rw-r--r--   0 root         (0) root         (0)      745 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/parameter_sets/field_parameter_set.h
+-rw-r--r--   0 root         (0) root         (0)      704 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/parameter_sets/set_field.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.510193 turbodbc-4.6.0/include/turbodbc/result_sets/
+-rw-r--r--   0 root         (0) root         (0)     1254 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/result_sets/bound_result_set.h
+-rw-r--r--   0 root         (0) root         (0)     2327 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/result_sets/double_buffered_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      971 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/result_sets/field_result_set.h
+-rw-r--r--   0 root         (0) root         (0)     1256 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/result_sets/result_set.h
+-rw-r--r--   0 root         (0) root         (0)     1028 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/result_sets/row_based_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      157 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/string_helpers.h
+-rw-r--r--   0 root         (0) root         (0)     1190 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/time_helpers.h
+-rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc/type_code.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.510193 turbodbc-4.6.0/include/turbodbc_arrow/
+-rw-r--r--   0 root         (0) root         (0)     1674 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_arrow/arrow_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      297 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_arrow/set_arrow_parameters.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.514193 turbodbc-4.6.0/include/turbodbc_numpy/
+-rw-r--r--   0 root         (0) root         (0)      556 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/binary_column.h
+-rw-r--r--   0 root         (0) root         (0)      683 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/datetime_column.h
+-rw-r--r--   0 root         (0) root         (0)      378 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/make_numpy_array.h
+-rw-r--r--   0 root         (0) root         (0)      698 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/masked_column.h
+-rw-r--r--   0 root         (0) root         (0)      459 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/ndarrayobject.h
+-rw-r--r--   0 root         (0) root         (0)      756 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/numpy_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      260 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/numpy_type.h
+-rw-r--r--   0 root         (0) root         (0)      299 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/set_numpy_parameters.h
+-rw-r--r--   0 root         (0) root         (0)      508 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/string_column.h
+-rw-r--r--   0 root         (0) root         (0)      511 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_numpy/unicode_column.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.514193 turbodbc-4.6.0/include/turbodbc_python/
+-rw-r--r--   0 root         (0) root         (0)      454 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_python/determine_parameter_type.h
+-rw-r--r--   0 root         (0) root         (0)      685 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_python/python_parameter_set.h
+-rw-r--r--   0 root         (0) root         (0)      885 2020-04-16 12:00:00.000000 turbodbc-4.6.0/include/turbodbc_python/python_result_set.h
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-09 09:50:37.546193 turbodbc-4.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    10193 2020-04-16 12:00:00.000000 turbodbc-4.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.498193 turbodbc-4.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.514193 turbodbc-4.6.0/src/cpp_odbc/
+-rw-r--r--   0 root         (0) root         (0)     2694 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/column_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      802 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/connection.cpp
+-rw-r--r--   0 root         (0) root         (0)      190 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/cpp_odbc.cpp
+-rw-r--r--   0 root         (0) root         (0)      411 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/environment.cpp
+-rw-r--r--   0 root         (0) root         (0)      744 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/error.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.514193 turbodbc-4.6.0/src/cpp_odbc/level1/
+-rw-r--r--   0 root         (0) root         (0)     7405 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level1/api.cpp
+-rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level1/level1.cpp
+-rw-r--r--   0 root         (0) root         (0)     7663 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level1/unixodbc_backend.cpp
+-rw-r--r--   0 root         (0) root         (0)    12404 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level1/unixodbc_backend_debug.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.518193 turbodbc-4.6.0/src/cpp_odbc/level2/
+-rw-r--r--   0 root         (0) root         (0)     5853 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/api.cpp
+-rw-r--r--   0 root         (0) root         (0)     1265 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/handles.cpp
+-rw-r--r--   0 root         (0) root         (0)      419 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/input_string_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)      457 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/input_u16string_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)    16753 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/level1_connector.cpp
+-rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/level2.cpp
+-rw-r--r--   0 root         (0) root         (0)      595 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/string_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)      621 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level2/u16string_buffer.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.518193 turbodbc-4.6.0/src/cpp_odbc/level3/
+-rw-r--r--   0 root         (0) root         (0)      193 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level3/level3.cpp
+-rw-r--r--   0 root         (0) root         (0)     3649 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level3/raii_connection.cpp
+-rw-r--r--   0 root         (0) root         (0)     1623 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level3/raii_environment.cpp
+-rw-r--r--   0 root         (0) root         (0)     3845 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/level3/raii_statement.cpp
+-rw-r--r--   0 root         (0) root         (0)      949 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/make_environment.cpp
+-rw-r--r--   0 root         (0) root         (0)     1816 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/multi_value_buffer.cpp
+-rw-r--r--   0 root         (0) root         (0)     2787 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/cpp_odbc/statement.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.526193 turbodbc-4.6.0/src/turbodbc/
+-rw-r--r--   0 root         (0) root         (0)     1218 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/buffer_size.cpp
+-rw-r--r--   0 root         (0) root         (0)      963 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/column.cpp
+-rw-r--r--   0 root         (0) root         (0)     1805 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/command.cpp
+-rw-r--r--   0 root         (0) root         (0)      901 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/configuration.cpp
+-rw-r--r--   0 root         (0) root         (0)      298 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/connect.cpp
+-rw-r--r--   0 root         (0) root         (0)     1136 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/connection.cpp
+-rw-r--r--   0 root         (0) root         (0)     1941 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/cursor.cpp
+-rw-r--r--   0 root         (0) root         (0)      830 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/description.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.526193 turbodbc-4.6.0/src/turbodbc/descriptions/
+-rw-r--r--   0 root         (0) root         (0)      783 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/descriptions/boolean_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      784 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/descriptions/date_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      899 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/descriptions/floating_point_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      810 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/descriptions/integer_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      915 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/descriptions/string_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      864 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/descriptions/timestamp_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      993 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/descriptions/unicode_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      211 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/errors.cpp
+-rw-r--r--   0 root         (0) root         (0)      393 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/field_translator.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.530193 turbodbc-4.6.0/src/turbodbc/field_translators/
+-rw-r--r--   0 root         (0) root         (0)      380 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/field_translators/boolean_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      483 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/field_translators/date_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      414 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/field_translators/float64_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      403 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/field_translators/int64_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      389 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/field_translators/string_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/field_translators/timestamp_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)     7166 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/make_description.cpp
+-rw-r--r--   0 root         (0) root         (0)      972 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/make_field_translator.cpp
+-rw-r--r--   0 root         (0) root         (0)     1820 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/parameter.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.530193 turbodbc-4.6.0/src/turbodbc/parameter_sets/
+-rw-r--r--   0 root         (0) root         (0)     4834 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/parameter_sets/bound_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     2680 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/parameter_sets/field_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     3552 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/parameter_sets/set_field.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.534193 turbodbc-4.6.0/src/turbodbc/result_sets/
+-rw-r--r--   0 root         (0) root         (0)     3054 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/result_sets/bound_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     2929 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/result_sets/double_buffered_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      856 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/result_sets/field_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      481 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/result_sets/result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      985 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/result_sets/row_based_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      436 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/string_helpers.cpp
+-rw-r--r--   0 root         (0) root         (0)     3200 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc/time_helpers.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.534193 turbodbc-4.6.0/src/turbodbc_arrow/
+-rw-r--r--   0 root         (0) root         (0)    15431 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_arrow/arrow_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     1113 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_arrow/python_bindings.cpp
+-rw-r--r--   0 root         (0) root         (0)    19064 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_arrow/set_arrow_parameters.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.534193 turbodbc-4.6.0/src/turbodbc_numpy/
+-rw-r--r--   0 root         (0) root         (0)     1907 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/binary_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     2492 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/datetime_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     2304 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/make_numpy_array.cpp
+-rw-r--r--   0 root         (0) root         (0)      431 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/masked_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     2434 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/numpy_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      327 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/numpy_type.cpp
+-rw-r--r--   0 root         (0) root         (0)     1396 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/python_bindings.cpp
+-rw-r--r--   0 root         (0) root         (0)    15127 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/set_numpy_parameters.cpp
+-rw-r--r--   0 root         (0) root         (0)     1077 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/string_column.cpp
+-rw-r--r--   0 root         (0) root         (0)     1092 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_numpy/unicode_column.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.538193 turbodbc-4.6.0/src/turbodbc_python/
+-rw-r--r--   0 root         (0) root         (0)     4027 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/determine_parameter_type.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.538193 turbodbc-4.6.0/src/turbodbc_python/python_bindings/
+-rw-r--r--   0 root         (0) root         (0)      675 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/buffer_size.cpp
+-rw-r--r--   0 root         (0) root         (0)      505 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/column_info.cpp
+-rw-r--r--   0 root         (0) root         (0)      259 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/connect.cpp
+-rw-r--r--   0 root         (0) root         (0)      776 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/connection.cpp
+-rw-r--r--   0 root         (0) root         (0)      757 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/cursor.cpp
+-rw-r--r--   0 root         (0) root         (0)      340 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/error.cpp
+-rw-r--r--   0 root         (0) root         (0)     1155 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/module.cpp
+-rw-r--r--   0 root         (0) root         (0)     2786 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/options.cpp
+-rw-r--r--   0 root         (0) root         (0)      568 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/python_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)      913 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_bindings/python_result_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     3004 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_parameter_set.cpp
+-rw-r--r--   0 root         (0) root         (0)     3469 2020-04-16 12:00:00.000000 turbodbc-4.6.0/src/turbodbc_python/python_result_set.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.542194 turbodbc-4.6.0/turbodbc/
+-rw-r--r--   0 root         (0) root         (0)      826 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      154 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/api_constants.py
+-rw-r--r--   0 root         (0) root         (0)      247 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/arrow_support.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/connect.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/connection.py
+-rw-r--r--   0 root         (0) root         (0)      286 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/constructors.py
+-rw-r--r--   0 root         (0) root         (0)    15873 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/cursor.py
+-rw-r--r--   0 root         (0) root         (0)      761 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/data_types.py
+-rw-r--r--   0 root         (0) root         (0)      990 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6269 2020-04-16 12:00:00.000000 turbodbc-4.6.0/turbodbc/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 09:50:37.542194 turbodbc-4.6.0/turbodbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-05-09 09:50:37.000000 turbodbc-4.6.0/turbodbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7302 2023-05-09 09:50:37.000000 turbodbc-4.6.0/turbodbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 09:50:37.000000 turbodbc-4.6.0/turbodbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-09 09:50:37.000000 turbodbc-4.6.0/turbodbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-09 09:50:37.000000 turbodbc-4.6.0/turbodbc.egg-info/top_level.txt
```

### Comparing `turbodbc-4.5.9/CHANGELOG.rst` & `turbodbc-4.6.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,29 @@
 Version history / changelog
 ===========================
 
 From version 2.0.0, turbodbc adapts semantic versioning.
 
+Version 4.6.0
+--------------
+
+* Drop python 3.8 support
+* Add python 3.11 support
+* Require ``numpy>=1.20.0``
+* Require ``pyarrow>=7``
+* Support ``pyarrow=12``
+* Bump pybind11 version to 2.10.4
+* Update GitHub Actions
+* Update pre-commit hooks and linting
+
+Version 4.5.10
+--------------
+
+* Support ``pyarrow=11``
+
 Version 4.5.9
 -------------
 
 * Check for ``_GLIBCXX_USE_CXX11_ABI`` setting of ``pyarrow``.
 
 Version 4.5.8
 -------------
```

### Comparing `turbodbc-4.5.9/LICENSE` & `turbodbc-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/PKG-INFO` & `turbodbc-4.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: turbodbc
-Version: 4.5.9
+Version: 4.6.0
 Summary: turbodbc is a Python DB API 2.0 compatible ODBC driver
 Home-page: https://github.com/blue-yonder/turbodbc
 Author: Michael Koenig
 Author-email: michael.koenig@blue-yonder.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: arrow
 Provides-Extra: numpy
 License-File: LICENSE
 
 ![turbodbc logo](/page/logo.png?raw=true "turbodbc logo")
 
@@ -44,15 +44,15 @@
 For maximum performance, turbodbc offers built-in [NumPy](http://www.numpy.org) and
 [Apache Arrow](https://arrow.apache.org) support
 and internally relies on batched data transfer instead of single-record communication as
 other popular ODBC modules do.
 
 Turbodbc is free to use ([MIT license](https://github.com/blue-yonder/turbodbc/blob/master/LICENSE)),
 open source ([GitHub](https://github.com/blue-yonder/turbodbc)),
-works with Python 3.8+, and is available for Linux, macOS, and Windows.
+works with Python 3.9+, and is available for Linux, macOS, and Windows.
 
 Turbodbc is routinely tested with [MySQL](https://www.mysql.com),
 [PostgreSQL](https://www.postgresql.org), [EXASOL](http://www.exasol.com),
 and [MSSQL](http://microsoft.com/sql), but probably also works with your database.
 
 
 Nice! Where can I find documentation?
```

### Comparing `turbodbc-4.5.9/README.md` & `turbodbc-4.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 For maximum performance, turbodbc offers built-in [NumPy](http://www.numpy.org) and
 [Apache Arrow](https://arrow.apache.org) support
 and internally relies on batched data transfer instead of single-record communication as
 other popular ODBC modules do.
 
 Turbodbc is free to use ([MIT license](https://github.com/blue-yonder/turbodbc/blob/master/LICENSE)),
 open source ([GitHub](https://github.com/blue-yonder/turbodbc)),
-works with Python 3.8+, and is available for Linux, macOS, and Windows.
+works with Python 3.9+, and is available for Linux, macOS, and Windows.
 
 Turbodbc is routinely tested with [MySQL](https://www.mysql.com),
 [PostgreSQL](https://www.postgresql.org), [EXASOL](http://www.exasol.com),
 and [MSSQL](http://microsoft.com/sql), but probably also works with your database.
 
 
 Nice! Where can I find documentation?
```

### Comparing `turbodbc-4.5.9/include/cpp_odbc/column_description.h` & `turbodbc-4.6.0/include/cpp_odbc/column_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/connection.h` & `turbodbc-4.6.0/include/cpp_odbc/connection.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/cpp_odbc.h` & `turbodbc-4.6.0/include/cpp_odbc/cpp_odbc.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/credentials.h` & `turbodbc-4.6.0/include/cpp_odbc/credentials.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/environment.h` & `turbodbc-4.6.0/include/cpp_odbc/environment.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/error.h` & `turbodbc-4.6.0/include/cpp_odbc/error.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level1/api.h` & `turbodbc-4.6.0/include/cpp_odbc/level1/api.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level1/unixodbc_backend.h` & `turbodbc-4.6.0/include/cpp_odbc/level1/unixodbc_backend.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level1/unixodbc_backend_debug.h` & `turbodbc-4.6.0/include/cpp_odbc/level1/unixodbc_backend_debug.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/api.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/api.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/diagnostic_record.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/diagnostic_record.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/fixed_length_string_buffer.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/fixed_length_string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/handles.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/handles.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/input_string_buffer.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/input_string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/input_u16string_buffer.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/input_u16string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/level1_connector.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/level1_connector.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/level2.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/level2.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/string_buffer.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level2/u16string_buffer.h` & `turbodbc-4.6.0/include/cpp_odbc/level2/u16string_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level3/level3.h` & `turbodbc-4.6.0/include/cpp_odbc/level3/level3.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level3/raii_connection.h` & `turbodbc-4.6.0/include/cpp_odbc/level3/raii_connection.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level3/raii_environment.h` & `turbodbc-4.6.0/include/cpp_odbc/level3/raii_environment.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/level3/raii_statement.h` & `turbodbc-4.6.0/include/cpp_odbc/level3/raii_statement.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/make_environment.h` & `turbodbc-4.6.0/include/cpp_odbc/make_environment.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/multi_value_buffer.h` & `turbodbc-4.6.0/include/cpp_odbc/multi_value_buffer.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/cpp_odbc/statement.h` & `turbodbc-4.6.0/include/cpp_odbc/statement.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/buffer_size.h` & `turbodbc-4.6.0/include/turbodbc/buffer_size.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/column.h` & `turbodbc-4.6.0/include/turbodbc/column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/command.h` & `turbodbc-4.6.0/include/turbodbc/command.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/configuration.h` & `turbodbc-4.6.0/include/turbodbc/configuration.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/connection.h` & `turbodbc-4.6.0/include/turbodbc/connection.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/cursor.h` & `turbodbc-4.6.0/include/turbodbc/cursor.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/description.h` & `turbodbc-4.6.0/include/turbodbc/description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/descriptions/boolean_description.h` & `turbodbc-4.6.0/include/turbodbc/descriptions/boolean_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/descriptions/date_description.h` & `turbodbc-4.6.0/include/turbodbc/descriptions/date_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/descriptions/floating_point_description.h` & `turbodbc-4.6.0/include/turbodbc/descriptions/floating_point_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/descriptions/integer_description.h` & `turbodbc-4.6.0/include/turbodbc/descriptions/integer_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/descriptions/string_description.h` & `turbodbc-4.6.0/include/turbodbc/descriptions/string_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/descriptions/timestamp_description.h` & `turbodbc-4.6.0/include/turbodbc/descriptions/timestamp_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/descriptions/unicode_description.h` & `turbodbc-4.6.0/include/turbodbc/descriptions/unicode_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/field.h` & `turbodbc-4.6.0/include/turbodbc/field.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/field_translator.h` & `turbodbc-4.6.0/include/turbodbc/field_translator.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/make_description.h` & `turbodbc-4.6.0/include/turbodbc/make_description.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/parameter.h` & `turbodbc-4.6.0/include/turbodbc/parameter.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/parameter_sets/bound_parameter_set.h` & `turbodbc-4.6.0/include/turbodbc/parameter_sets/bound_parameter_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/parameter_sets/field_parameter_set.h` & `turbodbc-4.6.0/include/turbodbc/parameter_sets/field_parameter_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/parameter_sets/set_field.h` & `turbodbc-4.6.0/include/turbodbc/parameter_sets/set_field.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/result_sets/bound_result_set.h` & `turbodbc-4.6.0/include/turbodbc/result_sets/bound_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/result_sets/double_buffered_result_set.h` & `turbodbc-4.6.0/include/turbodbc/result_sets/double_buffered_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/result_sets/field_result_set.h` & `turbodbc-4.6.0/include/turbodbc/result_sets/field_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/result_sets/result_set.h` & `turbodbc-4.6.0/include/turbodbc/result_sets/result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/result_sets/row_based_result_set.h` & `turbodbc-4.6.0/include/turbodbc/result_sets/row_based_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc/time_helpers.h` & `turbodbc-4.6.0/include/turbodbc/time_helpers.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc_arrow/arrow_result_set.h` & `turbodbc-4.6.0/include/turbodbc_arrow/arrow_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc_numpy/binary_column.h` & `turbodbc-4.6.0/include/turbodbc_numpy/binary_column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc_numpy/datetime_column.h` & `turbodbc-4.6.0/include/turbodbc_numpy/datetime_column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc_numpy/masked_column.h` & `turbodbc-4.6.0/include/turbodbc_numpy/masked_column.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc_numpy/numpy_result_set.h` & `turbodbc-4.6.0/include/turbodbc_numpy/numpy_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc_python/python_parameter_set.h` & `turbodbc-4.6.0/include/turbodbc_python/python_parameter_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/include/turbodbc_python/python_result_set.h` & `turbodbc-4.6.0/include/turbodbc_python/python_result_set.h`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/setup.py` & `turbodbc-4.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import distutils.ccompiler
 import distutils.sysconfig
 import itertools
 import os
 import os.path
 import sys
 from glob import iglob
-from typing import List
 
 import setuptools.command.build_ext
 from setuptools import Distribution, Extension, setup
 from setuptools.command.build_ext import build_ext
 
 
 class TurbodbcExtensionBuilder(build_ext):
@@ -72,19 +71,19 @@
         import pybind11
 
         return pybind11.get_include()
 
 
 extra_compile_args = []
 hidden_visibility_args = []
-include_dirs = ["include/", _deferred_pybind11_include()]
+include_dirs: list[str] = ["include/", str(_deferred_pybind11_include())]
 
-library_dirs = []
+library_dirs: list[str] = []
 python_module_link_args = []
-base_library_link_args: List[str] = []
+base_library_link_args: list[str] = []
 
 if sys.platform == "darwin":
     extra_compile_args.append("--std=c++17")
     extra_compile_args.append("--stdlib=libc++")
     extra_compile_args.append("-mmacosx-version-min=10.9")
     # See https://conda-forge.org/docs/maintainer/knowledge_base.html#newer-c-features-with-old-sdk
     extra_compile_args.append("-D_LIBCPP_DISABLE_AVAILABILITY")
@@ -99,33 +98,35 @@
     full_name = builder.get_ext_filename("libturbodbc")
     base_library_link_args.append(f"-Wl,-dylib_install_name,@loader_path/{full_name}")
     base_library_link_args.append("-dynamiclib")
     odbclib = "odbc"
 elif sys.platform == "win32":
     extra_compile_args.append("-DNOMINMAX")
     extra_compile_args.append("/std:c++17")
-    if "BOOST_ROOT" in os.environ:
-        include_dirs.append(os.getenv("BOOST_ROOT"))
-        library_dirs.append(os.path.join(os.getenv("BOOST_ROOT"), "stage", "lib"))
-        library_dirs.append(os.path.join(os.getenv("BOOST_ROOT"), "lib64-msvc-14.0"))
+    boost_root = os.getenv("BOOST_ROOT")
+    if boost_root:
+        include_dirs.append(boost_root)
+        library_dirs.append(os.path.join(boost_root, "stage", "lib"))
+        library_dirs.append(os.path.join(boost_root, "lib64-msvc-14.0"))
     else:
         print("warning: BOOST_ROOT enviroment variable not set")
     odbclib = "odbc32"
-    if "CONDA_PREFIX" in os.environ:
-        include_dirs.append(
-            os.path.join(os.environ["CONDA_PREFIX"], "Library", "include")
-        )
+    conda_prefix = os.getenv("CONDA_PREFIX")
+    if conda_prefix:
+        include_dirs.append(os.path.join(conda_prefix, "Library", "include"))
 else:
     extra_compile_args.append("--std=c++17")
     hidden_visibility_args.append("-fvisibility=hidden")
     python_module_link_args.append("-Wl,-rpath,$ORIGIN")
-    if "UNIXODBC_INCLUDE_DIR" in os.environ:
-        include_dirs.append(os.getenv("UNIXODBC_INCLUDE_DIR"))
-    if "UNIXODBC_LIBRARY_DIR" in os.environ:
-        library_dirs.append(os.getenv("UNIXODBC_LIBRARY_DIR"))
+    unixodbc_include_dir = os.getenv("UNIXODBC_INCLUDE_DIR")
+    if unixodbc_include_dir:
+        include_dirs.append(unixodbc_include_dir)
+    unixodbc_library_dir = os.getenv("UNIXODBC_LIBRARY_DIR")
+    if unixodbc_library_dir:
+        library_dirs.append(unixodbc_library_dir)
     odbclib = "odbc"
 
 
 def _get_cxx_compiler():
     cc = distutils.ccompiler.new_compiler()
     distutils.sysconfig.customize_compiler(cc)
     return cc.compiler_cxx[0]  # type: ignore
@@ -250,41 +251,41 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
     name="turbodbc",
-    version="4.5.9",
+    version="4.6.0",
     description="turbodbc is a Python DB API 2.0 compatible ODBC driver",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/blue-yonder/turbodbc",
     author="Michael Koenig",
     author_email="michael.koenig@blue-yonder.com",
     packages=["turbodbc"],
     setup_requires=[
-        "pybind11>=2.2.0",
-        "pyarrow>=1,<11",
-        "numpy>=1.18",
+        "pybind11>=2.10.4",
+        "pyarrow>=7,<13",
+        "numpy>=1.20",
     ],
     install_requires=[],
-    extras_require={"arrow": ["pyarrow>=1.0,<11"], "numpy": "numpy>=1.19.0"},
-    python_requires=">=3.8",
+    extras_require={"arrow": ["pyarrow>=7.0,<13"], "numpy": "numpy>=1.20.0"},
+    python_requires=">=3.9",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: C++",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Database",
     ],
     cmdclass=dict(build_ext=TurbodbcExtensionBuilder),
     ext_modules=get_extension_modules(),
 )
```

### Comparing `turbodbc-4.5.9/src/cpp_odbc/column_description.cpp` & `turbodbc-4.6.0/src/cpp_odbc/column_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/connection.cpp` & `turbodbc-4.6.0/src/cpp_odbc/connection.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/error.cpp` & `turbodbc-4.6.0/src/cpp_odbc/error.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level1/api.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level1/api.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level1/unixodbc_backend.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level1/unixodbc_backend.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level1/unixodbc_backend_debug.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level1/unixodbc_backend_debug.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level2/api.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level2/api.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level2/handles.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level2/handles.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level2/level1_connector.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level2/level1_connector.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level2/string_buffer.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level2/string_buffer.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level2/u16string_buffer.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level2/u16string_buffer.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level3/raii_connection.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level3/raii_connection.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level3/raii_environment.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level3/raii_environment.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/level3/raii_statement.cpp` & `turbodbc-4.6.0/src/cpp_odbc/level3/raii_statement.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/make_environment.cpp` & `turbodbc-4.6.0/src/cpp_odbc/make_environment.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/multi_value_buffer.cpp` & `turbodbc-4.6.0/src/cpp_odbc/multi_value_buffer.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/cpp_odbc/statement.cpp` & `turbodbc-4.6.0/src/cpp_odbc/statement.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/buffer_size.cpp` & `turbodbc-4.6.0/src/turbodbc/buffer_size.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/column.cpp` & `turbodbc-4.6.0/src/turbodbc/column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/command.cpp` & `turbodbc-4.6.0/src/turbodbc/command.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/configuration.cpp` & `turbodbc-4.6.0/src/turbodbc/configuration.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/connection.cpp` & `turbodbc-4.6.0/src/turbodbc/connection.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/cursor.cpp` & `turbodbc-4.6.0/src/turbodbc/cursor.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/description.cpp` & `turbodbc-4.6.0/src/turbodbc/description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/descriptions/boolean_description.cpp` & `turbodbc-4.6.0/src/turbodbc/descriptions/boolean_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/descriptions/date_description.cpp` & `turbodbc-4.6.0/src/turbodbc/descriptions/date_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/descriptions/floating_point_description.cpp` & `turbodbc-4.6.0/src/turbodbc/descriptions/floating_point_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/descriptions/integer_description.cpp` & `turbodbc-4.6.0/src/turbodbc/descriptions/integer_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/descriptions/string_description.cpp` & `turbodbc-4.6.0/src/turbodbc/descriptions/string_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/descriptions/timestamp_description.cpp` & `turbodbc-4.6.0/src/turbodbc/descriptions/timestamp_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/descriptions/unicode_description.cpp` & `turbodbc-4.6.0/src/turbodbc/descriptions/unicode_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/field_translators/timestamp_translator.cpp` & `turbodbc-4.6.0/src/turbodbc/field_translators/timestamp_translator.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/make_description.cpp` & `turbodbc-4.6.0/src/turbodbc/make_description.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/make_field_translator.cpp` & `turbodbc-4.6.0/src/turbodbc/make_field_translator.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/parameter.cpp` & `turbodbc-4.6.0/src/turbodbc/parameter.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/parameter_sets/bound_parameter_set.cpp` & `turbodbc-4.6.0/src/turbodbc/parameter_sets/bound_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/parameter_sets/field_parameter_set.cpp` & `turbodbc-4.6.0/src/turbodbc/parameter_sets/field_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/parameter_sets/set_field.cpp` & `turbodbc-4.6.0/src/turbodbc/parameter_sets/set_field.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/result_sets/bound_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc/result_sets/bound_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/result_sets/double_buffered_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc/result_sets/double_buffered_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/result_sets/field_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc/result_sets/field_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/result_sets/row_based_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc/result_sets/row_based_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc/time_helpers.cpp` & `turbodbc-4.6.0/src/turbodbc/time_helpers.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_arrow/arrow_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc_arrow/arrow_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_arrow/python_bindings.cpp` & `turbodbc-4.6.0/src/turbodbc_arrow/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_arrow/set_arrow_parameters.cpp` & `turbodbc-4.6.0/src/turbodbc_arrow/set_arrow_parameters.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/binary_column.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/binary_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/datetime_column.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/datetime_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/make_numpy_array.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/make_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/numpy_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/numpy_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/python_bindings.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/set_numpy_parameters.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/set_numpy_parameters.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/string_column.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/string_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_numpy/unicode_column.cpp` & `turbodbc-4.6.0/src/turbodbc_numpy/unicode_column.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/determine_parameter_type.cpp` & `turbodbc-4.6.0/src/turbodbc_python/determine_parameter_type.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_bindings/buffer_size.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_bindings/buffer_size.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_bindings/connection.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_bindings/connection.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 #include <pybind11/pybind11.h>
 
 
 namespace turbodbc { namespace bindings {
 
 void for_connection(pybind11::module &module) {
     pybind11::class_<turbodbc::connection>(module, "Connection")
-        .def("commit", &turbodbc::connection::commit)
-        .def("rollback", &turbodbc::connection::rollback)
-        .def("cursor", &turbodbc::connection::make_cursor)
-        .def("set_autocommit", &turbodbc::connection::set_autocommit)
+        .def("commit", &turbodbc::connection::commit, pybind11::call_guard<pybind11::gil_scoped_release>())
+        .def("rollback", &turbodbc::connection::rollback, pybind11::call_guard<pybind11::gil_scoped_release>())
+        .def("cursor", &turbodbc::connection::make_cursor, pybind11::call_guard<pybind11::gil_scoped_release>())
+        .def("set_autocommit", &turbodbc::connection::set_autocommit, pybind11::call_guard<pybind11::gil_scoped_release>())
         .def("autocommit_enabled", &turbodbc::connection::autocommit_enabled)
         ;
 
 }
 
 } }
```

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_bindings/cursor.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_bindings/cursor.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 
 
 namespace turbodbc { namespace bindings {
 
 void for_cursor(pybind11::module & module)
 {
     pybind11::class_<turbodbc::cursor>(module, "Cursor")
-            .def("prepare", &turbodbc::cursor::prepare)
-            .def("execute", [](turbodbc::cursor& cursor) {
-                pybind11::gil_scoped_release release;
-                cursor.execute();
-            })
-            .def("_reset",  &turbodbc::cursor::reset)
+            .def("prepare", &turbodbc::cursor::prepare, pybind11::call_guard<pybind11::gil_scoped_release>())
+            .def("execute", &turbodbc::cursor::execute, pybind11::call_guard<pybind11::gil_scoped_release>())
+            .def("_reset",  &turbodbc::cursor::reset, pybind11::call_guard<pybind11::gil_scoped_release>())
             .def("get_row_count", &turbodbc::cursor::get_row_count)
             .def("get_result_set", &turbodbc::cursor::get_result_set)
             .def("more_results", &turbodbc::cursor::more_results)
         ;
 }
 
 } }
```

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_bindings/module.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_bindings/module.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_bindings/options.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_bindings/options.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_bindings/python_parameter_set.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_bindings/python_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_bindings/python_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_bindings/python_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_parameter_set.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/src/turbodbc_python/python_result_set.cpp` & `turbodbc-4.6.0/src/turbodbc_python/python_result_set.cpp`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc/__init__.py` & `turbodbc-4.6.0/turbodbc/__init__.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc/connect.py` & `turbodbc-4.6.0/turbodbc/connect.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc/connection.py` & `turbodbc-4.6.0/turbodbc/connection.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc/cursor.py` & `turbodbc-4.6.0/turbodbc/cursor.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc/data_types.py` & `turbodbc-4.6.0/turbodbc/data_types.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc/exceptions.py` & `turbodbc-4.6.0/turbodbc/exceptions.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc/options.py` & `turbodbc-4.6.0/turbodbc/options.py`

 * *Files identical despite different names*

### Comparing `turbodbc-4.5.9/turbodbc.egg-info/PKG-INFO` & `turbodbc-4.6.0/turbodbc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: turbodbc
-Version: 4.5.9
+Version: 4.6.0
 Summary: turbodbc is a Python DB API 2.0 compatible ODBC driver
 Home-page: https://github.com/blue-yonder/turbodbc
 Author: Michael Koenig
 Author-email: michael.koenig@blue-yonder.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: arrow
 Provides-Extra: numpy
 License-File: LICENSE
 
 ![turbodbc logo](/page/logo.png?raw=true "turbodbc logo")
 
@@ -44,15 +44,15 @@
 For maximum performance, turbodbc offers built-in [NumPy](http://www.numpy.org) and
 [Apache Arrow](https://arrow.apache.org) support
 and internally relies on batched data transfer instead of single-record communication as
 other popular ODBC modules do.
 
 Turbodbc is free to use ([MIT license](https://github.com/blue-yonder/turbodbc/blob/master/LICENSE)),
 open source ([GitHub](https://github.com/blue-yonder/turbodbc)),
-works with Python 3.8+, and is available for Linux, macOS, and Windows.
+works with Python 3.9+, and is available for Linux, macOS, and Windows.
 
 Turbodbc is routinely tested with [MySQL](https://www.mysql.com),
 [PostgreSQL](https://www.postgresql.org), [EXASOL](http://www.exasol.com),
 and [MSSQL](http://microsoft.com/sql), but probably also works with your database.
 
 
 Nice! Where can I find documentation?
```

### Comparing `turbodbc-4.5.9/turbodbc.egg-info/SOURCES.txt` & `turbodbc-4.6.0/turbodbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

