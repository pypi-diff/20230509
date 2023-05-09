# Comparing `tmp/treelite-3.4.0.tar.gz` & `tmp/treelite-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treelite-3.4.0.tar", last modified: Tue May  2 03:53:10 2023, max compression
+gzip compressed data, was "treelite-3.9.0.tar", last modified: Tue May  9 05:02:09 2023, max compression
```

## Comparing `treelite-3.4.0.tar` & `treelite-3.9.0.tar`

### file list

```diff
@@ -1,155 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-02 03:52:46.000000 treelite-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 03:53:10.835741 treelite-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 03:53:10.835741 treelite-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-02 03:52:46.000000 treelite-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.823741 treelite-3.4.0/treelite/
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/annotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.823741 treelite-3.4.0/treelite/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Doxygen.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/ExternalLibs.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/FetchContentMakeAvailable.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Python_version.in
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/TreeliteConfig.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/Version.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/cmake/version.h.in
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/gcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/msvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/contrib/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gallery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/gallery/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gallery/sklearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/gtil/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gtil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/gtil/gtil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.819741 treelite-3.4.0/treelite/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/include/treelite/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/annotator.h
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/base.h
--rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api.h
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api_common.h
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api_error.h
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/c_api_runtime.h
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/compiler_param.h
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/data.h
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/frontend.h
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/frontend_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/gtil.h
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/math.h
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/omp.h
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/omp_exception.h
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/optional.h
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/predictor.h
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/thread_local.h
--rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/tree_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/include/treelite/typeinfo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/libpath.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.827741 treelite-3.4.0/treelite/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/serialize/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/gbm_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/gbm_multi_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/gbm_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/rf_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/rf_multi_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/sklearn/rf_regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/annotator.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/c_api/
--rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api_common.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api_error.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/c_api/c_api_runtime.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/ast/
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/ast.h
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/build.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/builder.h
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/dump.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/fold_code.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/is_categorical_array.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/load_data_counts.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/quantize.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast/split.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast_native.cc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/ast_native.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/common/categorical_bitmap.h
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/common/code_folding_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/common/format_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/compiler.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.831741 treelite-3.4.0/treelite/src/compiler/elf/
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.h
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/failsafe.cc
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/failsafe.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/compiler/native/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/code_folder_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/header_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/main_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/qnode_template.h
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/native/typeinfo_ctypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/compiler/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/data.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/filesystem.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/builder.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/json_importer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/lightgbm.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/sklearn.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/frontend/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost/xgboost.h
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost/xgboost_json.h
--rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost.cc
--rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost_json.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/frontend/xgboost_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/gtil/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/config.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/pred_transform.cc
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/pred_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/gtil/predict.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/json_serializer.cc
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/model_concat.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/predictor/
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/predictor/predictor.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/predictor/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/predictor/thread_pool/spsc_queue.h
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/predictor/thread_pool/thread_pool.h
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/serializer.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.835741 treelite-3.4.0/treelite/src/threading_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/threading_utils/parallel_for.h
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/src/typeinfo.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 03:52:46.000000 treelite-3.4.0/treelite/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 03:53:10.823741 treelite-3.4.0/treelite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 03:53:10.000000 treelite-3.4.0/treelite.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 05:01:51.000000 treelite-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 05:02:09.217137 treelite-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:02:09.217137 treelite-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-09 05:01:51.000000 treelite-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.205137 treelite-3.9.0/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/annotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.205137 treelite-3.9.0/treelite/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/Doxygen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/ExternalLibs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/FetchContentMakeAvailable.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/Python_version.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/Sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/TreeliteConfig.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/Version.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/cmake/version.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.205137 treelite-3.9.0/treelite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/contrib/gcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/contrib/msvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/contrib/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45591 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.205137 treelite-3.9.0/treelite/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/gallery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.205137 treelite-3.9.0/treelite/gallery/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/gallery/sklearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.205137 treelite-3.9.0/treelite/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/gtil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/gtil/gtil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.201137 treelite-3.9.0/treelite/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.209137 treelite-3.9.0/treelite/include/treelite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/annotator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/base.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44721 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/c_api.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/c_api_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/c_api_error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/c_api_runtime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/compiler_param.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/data.h
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28276 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/frontend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/frontend_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/gtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/math.h
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/omp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/omp_exception.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/optional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/predictor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/thread_local.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34430 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/tree_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/include/treelite/typeinfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/libpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.209137 treelite-3.9.0/treelite/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/serialize/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.209137 treelite-3.9.0/treelite/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/gbm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/gbm_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/gbm_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/rf_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/rf_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/sklearn/rf_regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.213137 treelite-3.9.0/treelite/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/annotator.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.213137 treelite-3.9.0/treelite/src/c_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    26843 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/c_api/c_api.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/c_api/c_api_common.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/c_api/c_api_error.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/c_api/c_api_runtime.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.213137 treelite-3.9.0/treelite/src/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.213137 treelite-3.9.0/treelite/src/compiler/ast/
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/ast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/build.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/builder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/dump.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/fold_code.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/is_categorical_array.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/load_data_counts.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/quantize.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast/split.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30563 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast_native.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/ast_native.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.213137 treelite-3.9.0/treelite/src/compiler/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/common/categorical_bitmap.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/common/code_folding_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/common/format_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/compiler.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.213137 treelite-3.9.0/treelite/src/compiler/elf/
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/elf/elf_formatter.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/elf/elf_formatter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/failsafe.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/failsafe.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/treelite/src/compiler/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/native/code_folder_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/native/header_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/native/main_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/native/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/native/qnode_template.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/native/typeinfo_ctypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/compiler/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/data.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/filesystem.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/treelite/src/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/json_importer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21059 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/lightgbm.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22631 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/sklearn.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/treelite/src/frontend/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/xgboost/xgboost.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/xgboost/xgboost_json.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/xgboost.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/xgboost_json.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/frontend/xgboost_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/treelite/src/gtil/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/gtil/config.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/gtil/pred_transform.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/gtil/pred_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34278 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/gtil/predict.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/json_serializer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/model_concat.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/treelite/src/predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/predictor/predictor.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/treelite/src/predictor/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/predictor/thread_pool/spsc_queue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/predictor/thread_pool/thread_pool.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/serializer.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.217137 treelite-3.9.0/treelite/src/threading_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/threading_utils/parallel_for.h
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/src/typeinfo.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 05:01:51.000000 treelite-3.9.0/treelite/warn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:02:09.205137 treelite-3.9.0/treelite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 05:02:09.000000 treelite-3.9.0/treelite.egg-info/top_level.txt
```

### Comparing `treelite-3.4.0/PKG-INFO` & `treelite-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite
-Version: 3.4.0
+Version: 3.9.0
 Summary: Treelite: model compiler for decision trees
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite-3.4.0/setup.py` & `treelite-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/CMakeLists.txt` & `treelite-3.9.0/treelite/CMakeLists.txt`

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

### Comparing `treelite-3.4.0/treelite/LICENSE` & `treelite-3.9.0/treelite/LICENSE`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/__init__.py` & `treelite-3.9.0/treelite/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/annotator.py` & `treelite-3.9.0/treelite/annotator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 """branch annotator module"""
 
 import ctypes
 from treelite_runtime import DMatrix
 from .util import c_str, TreeliteError
 from .core import _LIB, _check_call
 from .frontend import Model
+from .warn import deprecate
 
 
 class Annotator():
     """
     Branch annotator class: annotate branches in a given model using frequency
     patterns in the training data
     """
 
     def __init__(self):
+        deprecate("class Annotator")
         self.handle = None
 
     def annotate_branch(self, model, dmat, nthread=None, verbose=False):
         """
         Annotate branches in a given model using frequency patterns in the
         training data. Each node gets the count of the instances that belong to it.
         Any prior annotation information stored in the annotator will be replaced
```

### Comparing `treelite-3.4.0/treelite/cmake/ExternalLibs.cmake` & `treelite-3.9.0/treelite/cmake/ExternalLibs.cmake`

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

### Comparing `treelite-3.4.0/treelite/cmake/Sanitizer.cmake` & `treelite-3.9.0/treelite/cmake/Sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/cmake/Utils.cmake` & `treelite-3.9.0/treelite/cmake/Utils.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/cmake/Version.cmake` & `treelite-3.9.0/treelite/cmake/Version.cmake`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/contrib/__init__.py` & `treelite-3.9.0/treelite/contrib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import sys
 import os
 import json
 import time
 import ctypes
 from ..util import TreeliteError, lineno, log_info
+from ..warn import deprecate
 from .util import _libext, _toolchain_exist_check
 
 
 def expand_windows_path(dirpath):
     """
     Expand a short path to full path (only applicable for Windows)
 
@@ -56,14 +57,15 @@
     toolchain : :py:class:`str <python:str>`
         which toolchain to use. You may choose one of 'msvc', 'clang', and 'gcc'.
         You may also specify a specific variation of clang or gcc (e.g. 'gcc-7')
     options : :py:class:`list <python:list>` of :py:class:`str <python:str>`, \
               optional
         Additional options to pass to toolchain
     """
+    deprecate("Function treelite.generate_makefile()")
     if not os.path.isdir(dirpath):
         raise TreeliteError('Directory {} does not exist'.format(dirpath))
     try:
         with open(os.path.join(dirpath, 'recipe.json'), 'r', encoding='UTF-8') as f:
             recipe = json.load(f)
     except IOError as e:
         raise TreeliteError('Failed to open recipe.json') from e
@@ -128,14 +130,15 @@
         directory containing the header and source files previously generated
         by :py:meth:`Model.compile`. The directory must contain recipe.json
         which specifies build dependencies.
     options : :py:class:`list <python:list>` of :py:class:`str <python:str>`, \
               optional
         Additional options to pass to toolchain
     """
+    deprecate("Function treelite.generate_cmakelists()")
     if not os.path.isdir(dirpath):
         raise TreeliteError(f'Directory {dirpath} does not exist')
     try:
         with open(os.path.join(dirpath, 'recipe.json'), 'r', encoding='UTF-8') as f:
             recipe = json.load(f)
     except IOError as e:
         raise TreeliteError('Failed to open recipe.json') from e
@@ -227,17 +230,18 @@
 
     Alternatively, one may specify the library down to its file name:
 
     .. code-block:: python
 
        predictor = Predictor(libpath='./my/model/model.dll', verbose=True)
     """
-
     # pylint: disable=R0912
 
+    deprecate("Function treelite.create_shared()")
+
     if nthread is not None and nthread <= 0:
         raise TreeliteError('nthread must be positive integer')
     dirpath = expand_windows_path(dirpath)
     if not os.path.isdir(dirpath):
         raise TreeliteError('Directory {} does not exist'.format(dirpath))
     try:
         with open(os.path.join(dirpath, 'recipe.json'), 'r', encoding='UTF-8') as f:
```

### Comparing `treelite-3.4.0/treelite/contrib/gcc.py` & `treelite-3.9.0/treelite/contrib/gcc.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/contrib/msvc.py` & `treelite-3.9.0/treelite/contrib/msvc.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/contrib/util.py` & `treelite-3.9.0/treelite/contrib/util.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/core.py` & `treelite-3.9.0/treelite/core.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/frontend.py` & `treelite-3.9.0/treelite/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from packaging.version import parse as parse_version
 
 import numpy as np
 
 from .util import c_str, py_str, TreeliteError, type_info_to_ctypes_type, type_info_to_numpy_type
 from .core import _LIB, c_array, _check_call
 from .contrib import create_shared, generate_makefile, generate_cmakelists, _toolchain_exist_check
+from .warn import deprecate
 
 
 def _isascii(string):
     """Tests if a given string is pure ASCII; works for both Python 2 and 3"""
     try:
         return len(string) == len(string.encode())
     except UnicodeDecodeError:
@@ -246,14 +247,15 @@
 
            model.compile(dirpath='/temporary/directory', params={}, verbose=True)
            treelite.create_shared(toolchain='msvc', dirpath='/temporary/directory',
                                   verbose=True)
            # move the library out of the temporary directory
            shutil.move('/temporary/directory/mymodel.dll', './mymodel.dll')
         """
+        deprecate("Method treelite.Model.export_lib()")
         _toolchain_exist_check(toolchain)
 
         _params = dict(params) if isinstance(params, list) else params
         long_build_time_warning = not (_params and 'parallel_comp' in _params)
 
         with TemporaryDirectory(dir=os.path.dirname(libpath)) as temp_dir:
             self.compile(temp_dir, params, compiler, verbose)
@@ -317,14 +319,15 @@
            generate_makefile(dirpath='/temporary/directory/mymodel',
                              platform='unix', toolchain='gcc')
            # zip the directory containing C code and Makefile
            shutil.make_archive(base_name=pkgpath, format='zip',
                                root_dir='/temporary/directory',
                                base_dir='mymodel/')
         """
+        deprecate("Method treelite.Model.export_srcpkg()")
         # check for file extension
         fileext = os.path.splitext(pkgpath)[1]
         if fileext != '.zip':
             raise ValueError('Source package file should have .zip extension')
         libname = os.path.basename(libname)
         if toolchain != 'cmake':
             _toolchain_exist_check(toolchain)
@@ -378,14 +381,15 @@
 
         If parallel compilation is enabled (parameter ``parallel_comp``), the files
         are in the form of ``./my/model/header.h``, ``./my/model/main.c``,
         ``./my/model/tu0.c``, ``./my/model/tu1.c`` and so forth, depending on
         the value of ``parallel_comp``. Otherwise, there will be exactly two files:
         ``./model/header.h``, ``./my/model/main.c``
         """
+        deprecate("Method treelite.Model.compile()")
         compiler_handle = ctypes.c_void_p()
         _params = dict(params) if isinstance(params, list) else params
         if verbose and _params:
             _params['verbose'] = 1
         params_json_str = json.dumps(_params) if _params else '{}'
         _check_call(_LIB.TreeliteCompilerCreateV2(c_str(compiler),
                                                   c_str(params_json_str),
```

### Comparing `treelite-3.4.0/treelite/gtil/gtil.py` & `treelite-3.9.0/treelite/gtil/gtil.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/annotator.h` & `treelite-3.9.0/treelite/include/treelite/annotator.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/base.h` & `treelite-3.9.0/treelite/include/treelite/base.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/c_api.h` & `treelite-3.9.0/treelite/include/treelite/c_api.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/c_api_common.h` & `treelite-3.9.0/treelite/include/treelite/c_api_common.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/c_api_error.h` & `treelite-3.9.0/treelite/include/treelite/c_api_error.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/c_api_runtime.h` & `treelite-3.9.0/treelite/include/treelite/c_api_runtime.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/compiler.h` & `treelite-3.9.0/treelite/include/treelite/compiler.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/compiler_param.h` & `treelite-3.9.0/treelite/include/treelite/compiler_param.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/data.h` & `treelite-3.9.0/treelite/include/treelite/data.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/filesystem.h` & `treelite-3.9.0/treelite/include/treelite/filesystem.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/frontend.h` & `treelite-3.9.0/treelite/include/treelite/frontend.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/frontend_impl.h` & `treelite-3.9.0/treelite/include/treelite/frontend_impl.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/gtil.h` & `treelite-3.9.0/treelite/include/treelite/gtil.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/logging.h` & `treelite-3.9.0/treelite/include/treelite/logging.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/math.h` & `treelite-3.9.0/treelite/include/treelite/math.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/omp.h` & `treelite-3.9.0/treelite/include/treelite/omp.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/omp_exception.h` & `treelite-3.9.0/treelite/include/treelite/omp_exception.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/optional.h` & `treelite-3.9.0/treelite/include/treelite/optional.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/predictor.h` & `treelite-3.9.0/treelite/include/treelite/predictor.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/thread_local.h` & `treelite-3.9.0/treelite/include/treelite/thread_local.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/tree.h` & `treelite-3.9.0/treelite/include/treelite/tree.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/tree_impl.h` & `treelite-3.9.0/treelite/include/treelite/tree_impl.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/include/treelite/typeinfo.h` & `treelite-3.9.0/treelite/include/treelite/typeinfo.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/libpath.py` & `treelite-3.9.0/treelite/libpath.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/serialize/__main__.py` & `treelite-3.9.0/treelite/serialize/__main__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/__init__.py` & `treelite-3.9.0/treelite/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/common.py` & `treelite-3.9.0/treelite/sklearn/common.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/gbm_classifier.py` & `treelite-3.9.0/treelite/sklearn/gbm_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/gbm_multi_classifier.py` & `treelite-3.9.0/treelite/sklearn/gbm_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/gbm_regressor.py` & `treelite-3.9.0/treelite/sklearn/gbm_regressor.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/importer.py` & `treelite-3.9.0/treelite/sklearn/importer.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/rf_classifier.py` & `treelite-3.9.0/treelite/sklearn/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/rf_multi_classifier.py` & `treelite-3.9.0/treelite/sklearn/rf_multi_classifier.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/sklearn/rf_regressor.py` & `treelite-3.9.0/treelite/sklearn/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/CMakeLists.txt` & `treelite-3.9.0/treelite/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/annotator.cc` & `treelite-3.9.0/treelite/src/annotator.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/c_api/c_api.cc` & `treelite-3.9.0/treelite/src/c_api/c_api.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/c_api/c_api_common.cc` & `treelite-3.9.0/treelite/src/c_api/c_api_common.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/c_api/c_api_error.cc` & `treelite-3.9.0/treelite/src/c_api/c_api_error.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/c_api/c_api_runtime.cc` & `treelite-3.9.0/treelite/src/c_api/c_api_runtime.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/ast.h` & `treelite-3.9.0/treelite/src/compiler/ast/ast.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/build.cc` & `treelite-3.9.0/treelite/src/compiler/ast/build.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/builder.h` & `treelite-3.9.0/treelite/src/compiler/ast/builder.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/dump.cc` & `treelite-3.9.0/treelite/src/compiler/ast/dump.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/fold_code.cc` & `treelite-3.9.0/treelite/src/compiler/ast/fold_code.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/is_categorical_array.cc` & `treelite-3.9.0/treelite/src/compiler/ast/is_categorical_array.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/load_data_counts.cc` & `treelite-3.9.0/treelite/src/compiler/ast/load_data_counts.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/quantize.cc` & `treelite-3.9.0/treelite/src/compiler/ast/quantize.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast/split.cc` & `treelite-3.9.0/treelite/src/compiler/ast/split.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast_native.cc` & `treelite-3.9.0/treelite/src/compiler/ast_native.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/ast_native.h` & `treelite-3.9.0/treelite/src/compiler/ast_native.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/common/categorical_bitmap.h` & `treelite-3.9.0/treelite/src/compiler/common/categorical_bitmap.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/common/code_folding_util.h` & `treelite-3.9.0/treelite/src/compiler/common/code_folding_util.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/common/format_util.h` & `treelite-3.9.0/treelite/src/compiler/common/format_util.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/compiler.cc` & `treelite-3.9.0/treelite/src/compiler/compiler.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.cc` & `treelite-3.9.0/treelite/src/compiler/elf/elf_formatter.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/elf/elf_formatter.h` & `treelite-3.9.0/treelite/src/compiler/elf/elf_formatter.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/failsafe.cc` & `treelite-3.9.0/treelite/src/compiler/failsafe.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/failsafe.h` & `treelite-3.9.0/treelite/src/compiler/failsafe.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/native/code_folder_template.h` & `treelite-3.9.0/treelite/src/compiler/native/code_folder_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/native/header_template.h` & `treelite-3.9.0/treelite/src/compiler/native/header_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/native/main_template.h` & `treelite-3.9.0/treelite/src/compiler/native/main_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/native/pred_transform.h` & `treelite-3.9.0/treelite/src/compiler/native/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/native/qnode_template.h` & `treelite-3.9.0/treelite/src/compiler/native/qnode_template.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/native/typeinfo_ctypes.h` & `treelite-3.9.0/treelite/src/compiler/native/typeinfo_ctypes.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/pred_transform.cc` & `treelite-3.9.0/treelite/src/compiler/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/compiler/pred_transform.h` & `treelite-3.9.0/treelite/src/compiler/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/data.cc` & `treelite-3.9.0/treelite/src/data.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/filesystem.cc` & `treelite-3.9.0/treelite/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/builder.cc` & `treelite-3.9.0/treelite/src/frontend/builder.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/json_importer.cc` & `treelite-3.9.0/treelite/src/frontend/json_importer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/lightgbm.cc` & `treelite-3.9.0/treelite/src/frontend/lightgbm.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/sklearn.cc` & `treelite-3.9.0/treelite/src/frontend/sklearn.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/xgboost/xgboost.h` & `treelite-3.9.0/treelite/src/frontend/xgboost/xgboost.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/xgboost/xgboost_json.h` & `treelite-3.9.0/treelite/src/frontend/xgboost/xgboost_json.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/xgboost.cc` & `treelite-3.9.0/treelite/src/frontend/xgboost.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/xgboost_json.cc` & `treelite-3.9.0/treelite/src/frontend/xgboost_json.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/frontend/xgboost_util.cc` & `treelite-3.9.0/treelite/src/frontend/xgboost_util.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/gtil/config.cc` & `treelite-3.9.0/treelite/src/gtil/config.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/gtil/pred_transform.cc` & `treelite-3.9.0/treelite/src/gtil/pred_transform.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/gtil/pred_transform.h` & `treelite-3.9.0/treelite/src/gtil/pred_transform.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/gtil/predict.cc` & `treelite-3.9.0/treelite/src/gtil/predict.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/json_serializer.cc` & `treelite-3.9.0/treelite/src/json_serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/logging.cc` & `treelite-3.9.0/treelite/src/logging.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/model_concat.cc` & `treelite-3.9.0/treelite/src/model_concat.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/predictor/predictor.cc` & `treelite-3.9.0/treelite/src/predictor/predictor.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/predictor/thread_pool/spsc_queue.h` & `treelite-3.9.0/treelite/src/predictor/thread_pool/spsc_queue.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/predictor/thread_pool/thread_pool.h` & `treelite-3.9.0/treelite/src/predictor/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/serializer.cc` & `treelite-3.9.0/treelite/src/serializer.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/threading_utils/parallel_for.h` & `treelite-3.9.0/treelite/src/threading_utils/parallel_for.h`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/src/typeinfo.cc` & `treelite-3.9.0/treelite/src/typeinfo.cc`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite/util.py` & `treelite-3.9.0/treelite/util.py`

 * *Files identical despite different names*

### Comparing `treelite-3.4.0/treelite.egg-info/PKG-INFO` & `treelite-3.9.0/treelite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treelite
-Version: 3.4.0
+Version: 3.9.0
 Summary: Treelite: model compiler for decision trees
 Home-page: https://github.com/dmlc/treelite
 Author: DMLC
 Maintainer: Hyunsu Cho
 Maintainer-email: chohyu01@cs.washington.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `treelite-3.4.0/treelite.egg-info/SOURCES.txt` & `treelite-3.9.0/treelite.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 treelite/annotator.py
 treelite/compat.py
 treelite/core.py
 treelite/frontend.py
 treelite/libpath.py
 treelite/py.typed
 treelite/util.py
+treelite/warn.py
 treelite.egg-info/PKG-INFO
 treelite.egg-info/SOURCES.txt
 treelite.egg-info/dependency_links.txt
 treelite.egg-info/not-zip-safe
 treelite.egg-info/requires.txt
 treelite.egg-info/top_level.txt
 treelite/cmake/Doxygen.cmake
```

