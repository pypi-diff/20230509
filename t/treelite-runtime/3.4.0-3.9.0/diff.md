# Comparing `tmp/treelite_runtime-3.4.0.tar.gz` & `tmp/treelite_runtime-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treelite_runtime-3.4.0.tar", last modified: Tue May  2 03:53:11 2023, max compression
+gzip compressed data, was "treelite_runtime-3.9.0.tar", last modified: Tue May  9 05:02:09 2023, max compression
```

## Comparing `treelite_runtime-3.4.0.tar` & `treelite_runtime-3.9.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.227741 treelite_runtime-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 03:53:11.227741 treelite_runtime-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 03:53:11.227741 treelite_runtime-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.215741 treelite_runtime-3.4.0/treelite_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.215741 treelite_runtime-3.4.0/treelite_runtime/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Doxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/ExternalLibs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/FetchContentMakeAvailable.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Python_version.in
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/TreeliteConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/Version.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/cmake/version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.211741 treelite_runtime-3.4.0/treelite_runtime/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/include/treelite/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/annotator.h
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/base.h
--rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_error.h
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_runtime.h
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler_param.h
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/data.h
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend.h
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/gtil.h
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/math.h
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp_exception.h
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/optional.h
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/predictor.h
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/thread_local.h
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/include/treelite/typeinfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/libpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/annotator.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/src/c_api/
--rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_common.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_error.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_runtime.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.219740 treelite_runtime-3.4.0/treelite_runtime/src/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/ast.h
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/build.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/dump.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/fold_code.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/load_data_counts.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/quantize.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/split.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.cc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/categorical_bitmap.h
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/code_folding_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/format_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/compiler.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.cc
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/code_folder_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/header_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/main_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/qnode_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/data.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/filesystem.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/json_importer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/lightgbm.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/sklearn.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost.h
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h
--rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost.cc
--rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/gtil/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/config.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/gtil/predict.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/json_serializer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/model_concat.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/predictor/predictor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/serializer.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.223741 treelite_runtime-3.4.0/treelite_runtime/src/threading_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/threading_utils/parallel_for.h
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/src/typeinfo.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-02 03:52:46.000000 treelite_runtime-3.4.0/treelite_runtime/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:11.215741 treelite_runtime-3.4.0/treelite_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-02 03:53:11.000000 treelite_runtime-3.4.0/treelite_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.593135 treelite_runtime-3.9.0/treelite_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.597135 treelite_runtime-3.9.0/treelite_runtime/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/Doxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/ExternalLibs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/FetchContentMakeAvailable.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/Python_version.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/Sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/TreeliteConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/Version.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/cmake/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.593135 treelite_runtime-3.9.0/treelite_runtime/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.597135 treelite_runtime-3.9.0/treelite_runtime/include/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/annotator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api_error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api_runtime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/compiler_param.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/frontend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/frontend_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/gtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/omp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/omp_exception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/optional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/predictor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/thread_local.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/tree_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/include/treelite/typeinfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/libpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.601135 treelite_runtime-3.9.0/treelite_runtime/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/annotator.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.601135 treelite_runtime-3.9.0/treelite_runtime/src/c_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api_common.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api_error.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api_runtime.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.601135 treelite_runtime-3.9.0/treelite_runtime/src/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.601135 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/build.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/dump.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/fold_code.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/load_data_counts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/quantize.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/split.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast_native.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast_native.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.601135 treelite_runtime-3.9.0/treelite_runtime/src/compiler/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/common/categorical_bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/common/code_folding_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/common/format_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/compiler.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.601135 treelite_runtime-3.9.0/treelite_runtime/src/compiler/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/elf/elf_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/elf/elf_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/failsafe.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/failsafe.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.601135 treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/code_folder_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/header_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/main_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/qnode_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/compiler/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/filesystem.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/treelite_runtime/src/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/json_importer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/lightgbm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/sklearn.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost/xgboost.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/treelite_runtime/src/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/gtil/config.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/gtil/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/gtil/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/gtil/predict.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/json_serializer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/model_concat.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/treelite_runtime/src/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/predictor/predictor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/treelite_runtime/src/predictor/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/serializer.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.605135 treelite_runtime-3.9.0/treelite_runtime/src/threading_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/threading_utils/parallel_for.h
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/src/typeinfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 05:01:51.000000 treelite_runtime-3.9.0/treelite_runtime/warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.593135 treelite_runtime-3.9.0/treelite_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-09 05:02:09.000000 treelite_runtime-3.9.0/treelite_runtime.egg-info/top_level.txt
```

### Comparing `treelite_runtime-3.4.0/PKG-INFO` & `treelite_runtime-3.9.0/treelite_runtime.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: treelite_runtime
-Version: 3.4.0
+Name: treelite-runtime
+Version: 3.9.0
 Summary: Treelite runtime
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite_runtime-3.4.0/setup.py` & `treelite_runtime-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/CMakeLists.txt` & `treelite_runtime-3.9.0/treelite_runtime/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmake_policy(SET CMP0091 NEW)
 set(CMAKE_FIND_NO_INSTALL_PREFIX TRUE FORCE)
 cmake_minimum_required (VERSION 3.16)
-project(treelite LANGUAGES CXX C VERSION 3.4.0)
+project(treelite LANGUAGES CXX C VERSION 3.9.0)
 
 # check MSVC version
 if(MSVC)
   if(MSVC_VERSION LESS 1920)
     message(FATAL_ERROR "Need Visual Studio 2019 or newer to compile Treelite")
   endif()
 endif()
@@ -97,14 +97,18 @@
 endif()
 
 foreach(lib ${TREELITE_TARGETS})
   set_output_directory(${lib} ${PROJECT_BINARY_DIR})
 endforeach()
 
 # Export install targets
+if(CMAKE_SOURCE_DIR STREQUAL CMAKE_CURRENT_SOURCE_DIR)
+  # Include CPack only if the current project is top level.
+  include(CPack)
+endif()
 include(GNUInstallDirs)
 include(CMakePackageConfigHelpers)
 set(INSTALL_TARGETS ${TREELITE_TARGETS}
                     objtreelite objtreelite_common objtreelite_runtime rapidjson)
 if(NOT FMTLIB_FROM_SYSTEM_ROOT)
   list(APPEND INSTALL_TARGETS fmt-header-only)
 endif()
```

### Comparing `treelite_runtime-3.4.0/treelite_runtime/LICENSE` & `treelite_runtime-3.9.0/treelite_runtime/LICENSE`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/cmake/ExternalLibs.cmake` & `treelite_runtime-3.9.0/treelite_runtime/cmake/ExternalLibs.cmake`

 * *Files 14% similar despite different names*

```diff
@@ -46,9 +46,13 @@
       googletest
       GIT_REPOSITORY https://github.com/google/googletest.git
       GIT_TAG        release-1.11.0
     )
     FetchContent_MakeAvailable(googletest)
     add_library(GTest::GTest ALIAS gtest)
     add_library(GTest::gmock ALIAS gmock)
+    if(IS_DIRECTORY "${googletest_SOURCE_DIR}")
+      # Do not install gtest
+      set_property(DIRECTORY ${googletest_SOURCE_DIR} PROPERTY EXCLUDE_FROM_ALL YES)
+    endif()
   endif()
 endif()
```

### Comparing `treelite_runtime-3.4.0/treelite_runtime/cmake/Sanitizer.cmake` & `treelite_runtime-3.9.0/treelite_runtime/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/cmake/Utils.cmake` & `treelite_runtime-3.9.0/treelite_runtime/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/cmake/Version.cmake` & `treelite_runtime-3.9.0/treelite_runtime/cmake/Version.cmake`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/annotator.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/annotator.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/base.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/base.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_common.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api_common.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_error.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api_error.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/c_api_runtime.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/c_api_runtime.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/compiler.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/compiler_param.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/compiler_param.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/data.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/data.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/filesystem.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/filesystem.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/frontend.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/frontend_impl.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/frontend_impl.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/gtil.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/gtil.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/logging.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/logging.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/math.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/math.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/omp.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/omp_exception.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/omp_exception.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/optional.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/optional.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/predictor.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/predictor.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/thread_local.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/thread_local.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/tree.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/tree_impl.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/tree_impl.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/include/treelite/typeinfo.h` & `treelite_runtime-3.9.0/treelite_runtime/include/treelite/typeinfo.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/libpath.py` & `treelite_runtime-3.9.0/treelite_runtime/libpath.py`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/predictor.py` & `treelite_runtime-3.9.0/treelite_runtime/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pathlib
 import numpy as np
 import scipy.sparse
 from .util import c_str, py_str, _log_callback, TreeliteRuntimeError, lineno, log_info, \
     lib_extension_current_platform, type_info_to_ctypes_type, type_info_to_numpy_type, \
     numpy_type_to_type_info
 from .libpath import TreeliteRuntimeLibraryNotFound, find_lib_path
+from .warn import deprecate
 
 
 def _load_runtime_lib():
     """Load Treelite runtime"""
     lib_path = find_lib_path()
     if sys.version_info >= (3, 8) and sys.platform == 'win32':
         # pylint: disable=no-member
@@ -74,14 +75,15 @@
     verbose : :py:class:`bool <python:bool>`, optional
         Whether to print extra messages during construction
     """
 
     # pylint: disable=R0903
 
     def __init__(self, libpath, nthread=None, verbose=False):
+        deprecate("class treelite_runtime.Predictor")
         if os.path.isdir(libpath):  # libpath is a directory
             # directory is given; locate shared library inside it
             lib_found = False
             dir = pathlib.Path(libpath)
             ext = lib_extension_current_platform()
             for candidate in dir.glob(f'*{ext}'):
                 try:
@@ -276,14 +278,15 @@
     """
 
     # pylint: disable=R0902,R0903,R0913
 
     def __init__(self, data, data_format=None, dtype=None, missing=None,
                  feature_names=None, feature_types=None,
                  verbose=False, nthread=None):
+        deprecate("class treelite_runtime.DMatrix")
         if data is None:
             raise TreeliteRuntimeError("'data' argument cannot be None")
 
         self.handle = ctypes.c_void_p()
 
         if isinstance(data, (str,)):
             raise TreeliteRuntimeError(
```

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/CMakeLists.txt` & `treelite_runtime-3.9.0/treelite_runtime/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/annotator.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/annotator.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_common.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api_common.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_error.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/c_api/c_api_runtime.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/c_api/c_api_runtime.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/ast.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/ast.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/build.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/build.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/builder.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/builder.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/dump.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/dump.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/fold_code.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/fold_code.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/is_categorical_array.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/load_data_counts.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/load_data_counts.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/quantize.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/quantize.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast/split.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast/split.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast_native.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/ast_native.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/ast_native.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/categorical_bitmap.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/common/categorical_bitmap.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/code_folding_util.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/common/code_folding_util.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/common/format_util.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/common/format_util.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/compiler.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/compiler.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/elf/elf_formatter.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/elf/elf_formatter.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/elf/elf_formatter.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/failsafe.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/failsafe.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/failsafe.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/code_folder_template.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/code_folder_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/header_template.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/header_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/main_template.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/main_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/pred_transform.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/qnode_template.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/qnode_template.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/native/typeinfo_ctypes.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/compiler/pred_transform.h` & `treelite_runtime-3.9.0/treelite_runtime/src/compiler/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/data.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/data.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/filesystem.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/builder.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/builder.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/json_importer.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/json_importer.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/lightgbm.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/lightgbm.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/sklearn.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost.h` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost/xgboost.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost/xgboost_json.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_json.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost_json.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/frontend/xgboost_util.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/frontend/xgboost_util.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/gtil/config.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/gtil/config.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/gtil/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/gtil/pred_transform.h` & `treelite_runtime-3.9.0/treelite_runtime/src/gtil/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/gtil/predict.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/gtil/predict.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/json_serializer.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/json_serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/logging.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/model_concat.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/model_concat.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/predictor/predictor.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/predictor/predictor.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h` & `treelite_runtime-3.9.0/treelite_runtime/src/predictor/thread_pool/spsc_queue.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h` & `treelite_runtime-3.9.0/treelite_runtime/src/predictor/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/serializer.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/threading_utils/parallel_for.h` & `treelite_runtime-3.9.0/treelite_runtime/src/threading_utils/parallel_for.h`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/src/typeinfo.cc` & `treelite_runtime-3.9.0/treelite_runtime/src/typeinfo.cc`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime/util.py` & `treelite_runtime-3.9.0/treelite_runtime/util.py`

 * *Files identical despite different names*

### Comparing `treelite_runtime-3.4.0/treelite_runtime.egg-info/SOURCES.txt` & `treelite_runtime-3.9.0/treelite_runtime.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 treelite_runtime/CMakeLists.txt
 treelite_runtime/LICENSE
 treelite_runtime/VERSION
 treelite_runtime/__init__.py
 treelite_runtime/libpath.py
 treelite_runtime/predictor.py
 treelite_runtime/util.py
+treelite_runtime/warn.py
 treelite_runtime.egg-info/PKG-INFO
 treelite_runtime.egg-info/SOURCES.txt
 treelite_runtime.egg-info/dependency_links.txt
 treelite_runtime.egg-info/not-zip-safe
 treelite_runtime.egg-info/requires.txt
 treelite_runtime.egg-info/top_level.txt
 treelite_runtime/cmake/Doxygen.cmake
```

