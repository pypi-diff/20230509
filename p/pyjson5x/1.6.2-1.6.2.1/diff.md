# Comparing `tmp/pyjson5x-1.6.2.tar.gz` & `tmp/pyjson5x-1.6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjson5x-1.6.2.tar", last modified: Tue May  9 06:16:10 2023, max compression
+gzip compressed data, was "pyjson5x-1.6.2.1.tar", last modified: Tue May  9 17:18:47 2023, max compression
```

## Comparing `pyjson5x-1.6.2.tar` & `pyjson5x-1.6.2.1.tar`

### file list

```diff
@@ -1,68 +1,73 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.461874 pyjson5x-1.6.2/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-05-09 04:34:36.000000 pyjson5x-1.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      295 2023-05-09 04:34:30.000000 pyjson5x-1.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1638 2023-05-09 04:34:30.000000 pyjson5x-1.6.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     2604 2023-05-09 06:16:10.461874 pyjson5x-1.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1375 2023-05-09 04:55:50.000000 pyjson5x-1.6.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.453874 pyjson5x-1.6.2/docs/
--rw-r--r--   0 root         (0) root         (0)     2196 2023-05-09 04:34:36.000000 pyjson5x-1.6.2/docs/changelog.md
--rw-r--r--   0 root         (0) root         (0)     1766 2023-05-09 04:41:53.000000 pyjson5x-1.6.2/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     1739 2023-05-09 04:41:53.000000 pyjson5x-1.6.2/docs/decoder.rst
--rw-r--r--   0 root         (0) root         (0)     1604 2023-05-09 04:41:53.000000 pyjson5x-1.6.2/docs/encoder.rst
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-09 04:41:53.000000 pyjson5x-1.6.2/docs/exceptions.rst
--rw-r--r--   0 root         (0) root         (0)     1607 2023-05-09 04:41:53.000000 pyjson5x-1.6.2/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     7732 2023-05-09 04:41:53.000000 pyjson5x-1.6.2/docs/performance.rst
--rwxr-xr-x   0 root         (0) root         (0)     2076 2023-05-09 04:34:36.000000 pyjson5x-1.6.2/make_decoder_recursive_select.py
--rwxr-xr-x   0 root         (0) root         (0)     1648 2023-05-09 04:34:36.000000 pyjson5x-1.6.2/make_escape_dct.py
--rwxr-xr-x   0 root         (0) root         (0)     4581 2023-05-09 04:34:36.000000 pyjson5x-1.6.2/make_unicode_categories.py
--rw-r--r--   0 root         (0) root         (0)  2244433 2023-05-09 04:34:30.000000 pyjson5x-1.6.2/pyjson5x.cpp
--rw-r--r--   0 root         (0) root         (0)     1402 2023-05-09 04:34:30.000000 pyjson5x-1.6.2/pyjson5x.pyx
--rw-r--r--   0 root         (0) root         (0)      115 2023-05-09 04:34:36.000000 pyjson5x-1.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-09 06:16:10.465874 pyjson5x-1.6.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      453 2023-05-09 04:34:36.000000 pyjson5x-1.6.2/setup.py
--rwxr-xr-x   0 root         (0) root         (0)     1039 2023-05-09 04:34:30.000000 pyjson5x-1.6.2/sha512sum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.461874 pyjson5x-1.6.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.461874 pyjson5x-1.6.2/src/.ipynb_checkpoints/
--rw-r--r--   0 root         (0) root         (0)     1852 2023-05-09 04:52:13.000000 pyjson5x-1.6.2/src/.ipynb_checkpoints/_decoder_recursive_select-checkpoint.hpp
--rw-r--r--   0 root         (0) root         (0)      717 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/DESCRIPTION.inc
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/VERSION.inc
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_constants.pyx
--rw-r--r--   0 root         (0) root         (0)    24579 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_decoder.pyx
--rw-r--r--   0 root         (0) root         (0)     1852 2023-05-09 04:52:13.000000 pyjson5x-1.6.2/src/_decoder_recursive_select.hpp
--rw-r--r--   0 root         (0) root         (0)    13753 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_encoder.pyx
--rw-r--r--   0 root         (0) root         (0)     5516 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_encoder_options.pyx
--rw-r--r--   0 root         (0) root         (0)    15851 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_escape_dct.hpp
--rw-r--r--   0 root         (0) root         (0)      324 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_exceptions.pyx
--rw-r--r--   0 root         (0) root         (0)     2153 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_exceptions_decoder.pyx
--rw-r--r--   0 root         (0) root         (0)      598 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_exceptions_encoder.pyx
--rw-r--r--   0 root         (0) root         (0)    17265 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_exports.pyx
--rw-r--r--   0 root         (0) root         (0)     6734 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_imports.pyx
--rw-r--r--   0 root         (0) root         (0)     2039 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_legacy.pyx
--rw-r--r--   0 root         (0) root         (0)     2384 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_raise_decoder.pyx
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_raise_encoder.pyx
--rw-r--r--   0 root         (0) root         (0)     1084 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_reader_callback.pyx
--rw-r--r--   0 root         (0) root         (0)     1891 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_reader_ucs.pyx
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_readers.pyx
--rw-r--r--   0 root         (0) root         (0)     2434 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_stack_heap_string.hpp
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_unicode.pyx
--rw-r--r--   0 root         (0) root         (0)   620667 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_unicode_cat_of.hpp
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_writer_callback.pyx
--rw-r--r--   0 root         (0) root         (0)      385 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_writer_noop.pyx
--rw-r--r--   0 root         (0) root         (0)     1630 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_writer_reallocatable.pyx
--rw-r--r--   0 root         (0) root         (0)      290 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/_writers.pyx
--rw-r--r--   0 root         (0) root         (0)    58461 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/dragonbox.cc
--rw-r--r--   0 root         (0) root         (0)     5183 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/native.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.461874 pyjson5x-1.6.2/src/pyjson5x/
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/pyjson5x/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8430 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/pyjson5x/__init__.pyi
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/pyjson5x/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.461874 pyjson5x-1.6.2/src/pyjson5x.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2604 2023-05-09 06:16:10.000000 pyjson5x-1.6.2/src/pyjson5x.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1283 2023-05-09 06:16:10.000000 pyjson5x-1.6.2/src/pyjson5x.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 06:16:10.000000 pyjson5x-1.6.2/src/pyjson5x.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 04:41:45.000000 pyjson5x-1.6.2/src/pyjson5x.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-09 06:16:10.000000 pyjson5x-1.6.2/src/pyjson5x.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.445874 pyjson5x-1.6.2/third-party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.445874 pyjson5x-1.6.2/third-party/fast_double_parser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 06:16:10.461874 pyjson5x-1.6.2/third-party/fast_double_parser/include/
--rw-r--r--   0 root         (0) root         (0)    49886 2023-05-09 04:40:29.000000 pyjson5x-1.6.2/third-party/fast_double_parser/include/fast_double_parser.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.118491 pyjson5x-1.6.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-09 17:18:47.118491 pyjson5x-1.6.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-09 16:57:44.000000 pyjson5x-1.6.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.106491 pyjson5x-1.6.2.1/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.110491 pyjson5x-1.6.2.1/docs/.ipynb_checkpoints/
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/.ipynb_checkpoints/decoder-checkpoint.rst
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/.ipynb_checkpoints/index-checkpoint.rst
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/changelog.md
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/decoder.rst
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/encoder.rst
+-rw-r--r--   0 root         (0) root         (0)      410 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/exceptions.rst
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     7732 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/docs/performance.rst
+-rwxr-xr-x   0 root         (0) root         (0)     2076 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/make_decoder_recursive_select.py
+-rwxr-xr-x   0 root         (0) root         (0)     1648 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/make_escape_dct.py
+-rwxr-xr-x   0 root         (0) root         (0)     4581 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/make_unicode_categories.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/pyjson5x.pyx
+-rw-r--r--   0 root         (0) root         (0)      115 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-05-09 17:18:47.118491 pyjson5x-1.6.2.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      453 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)     1039 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/sha512sum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.114491 pyjson5x-1.6.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.118491 pyjson5x-1.6.2.1/src/.ipynb_checkpoints/
+-rw-r--r--   0 root         (0) root         (0)    24951 2023-05-09 16:54:24.000000 pyjson5x-1.6.2.1/src/.ipynb_checkpoints/_decoder-checkpoint.pyx
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/.ipynb_checkpoints/_exceptions-checkpoint.pyx
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/.ipynb_checkpoints/_exceptions_decoder-checkpoint.pyx
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/.ipynb_checkpoints/_raise_decoder-checkpoint.pyx
+-rw-r--r--   0 root         (0) root         (0)      717 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/DESCRIPTION.inc
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/VERSION.inc
+-rw-r--r--   0 root         (0) root         (0)      642 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_constants.pyx
+-rw-r--r--   0 root         (0) root         (0)    24951 2023-05-09 16:54:24.000000 pyjson5x-1.6.2.1/src/_decoder.pyx
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_decoder_recursive_select.hpp
+-rw-r--r--   0 root         (0) root         (0)    13753 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_encoder.pyx
+-rw-r--r--   0 root         (0) root         (0)     5516 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_encoder_options.pyx
+-rw-r--r--   0 root         (0) root         (0)    15851 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_escape_dct.hpp
+-rw-r--r--   0 root         (0) root         (0)      324 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_exceptions.pyx
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_exceptions_decoder.pyx
+-rw-r--r--   0 root         (0) root         (0)      598 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_exceptions_encoder.pyx
+-rw-r--r--   0 root         (0) root         (0)    17265 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_exports.pyx
+-rw-r--r--   0 root         (0) root         (0)     6734 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_imports.pyx
+-rw-r--r--   0 root         (0) root         (0)     2039 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_legacy.pyx
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_raise_decoder.pyx
+-rw-r--r--   0 root         (0) root         (0)      303 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_raise_encoder.pyx
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_reader_callback.pyx
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_reader_ucs.pyx
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_readers.pyx
+-rw-r--r--   0 root         (0) root         (0)     2434 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_stack_heap_string.hpp
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_unicode.pyx
+-rw-r--r--   0 root         (0) root         (0)   620667 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_unicode_cat_of.hpp
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_writer_callback.pyx
+-rw-r--r--   0 root         (0) root         (0)      385 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_writer_noop.pyx
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_writer_reallocatable.pyx
+-rw-r--r--   0 root         (0) root         (0)      290 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/_writers.pyx
+-rw-r--r--   0 root         (0) root         (0)    58461 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/dragonbox.cc
+-rw-r--r--   0 root         (0) root         (0)     5183 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/native.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.118491 pyjson5x-1.6.2.1/src/pyjson5x/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/pyjson5x/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8430 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/pyjson5x/__init__.pyi
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 08:14:54.000000 pyjson5x-1.6.2.1/src/pyjson5x/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.118491 pyjson5x-1.6.2.1/src/pyjson5x.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2699 2023-05-09 17:18:47.000000 pyjson5x-1.6.2.1/src/pyjson5x.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-05-09 17:18:47.000000 pyjson5x-1.6.2.1/src/pyjson5x.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:18:47.000000 pyjson5x-1.6.2.1/src/pyjson5x.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:18:47.000000 pyjson5x-1.6.2.1/src/pyjson5x.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-09 17:18:47.000000 pyjson5x-1.6.2.1/src/pyjson5x.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.102491 pyjson5x-1.6.2.1/third-party/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.102491 pyjson5x-1.6.2.1/third-party/fast_double_parser/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:18:47.118491 pyjson5x-1.6.2.1/third-party/fast_double_parser/include/
+-rw-r--r--   0 root         (0) root         (0)    49886 2023-05-09 08:15:03.000000 pyjson5x-1.6.2.1/third-party/fast_double_parser/include/fast_double_parser.h
```

### Comparing `pyjson5x-1.6.2/LICENSE` & `pyjson5x-1.6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/Makefile` & `pyjson5x-1.6.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/PKG-INFO` & `pyjson5x-1.6.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjson5x
-Version: 1.6.2
+Version: 1.6.2.1
 Summary: JSON5 rough serializer and parser for Python 3 written in Cython.
 Home-page: https://github.com/caffeinism/pyjson5x
 Author: Kim Minjong
 Author-email: make.dirty.code@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,23 +19,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Text Processing :: General
-Requires-Python: ~=3.5
+Requires-Python: ~=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 PyJSON5x
 ==========
 
 
-This package is the same as pyjson5, but interprets True and False as booleans. For more information, see the source repository. https://github.com/Kijewski/pyjson5
+This package is the same as pyjson5, but this library does some crude decoding. 
+
+- interprets True and False as booleans.
+
+- strive to properly handle unclosed brackets.
+
+
+For more information, see the source repository. https://github.com/Kijewski/pyjson5
 
 
 A JSON5 serializer and parser library for Python 3 written in
 `Cython <http://cython.org/>`_.
 
 
 Serializer
```

### Comparing `pyjson5x-1.6.2/README.rst` & `pyjson5x-1.6.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 PyJSON5x
 ==========
 
 
-This package is the same as pyjson5, but interprets True and False as booleans. For more information, see the source repository. https://github.com/Kijewski/pyjson5
+This package is the same as pyjson5, but this library does some crude decoding. 
+
+- interprets True and False as booleans.
+
+- strive to properly handle unclosed brackets.
+
+
+For more information, see the source repository. https://github.com/Kijewski/pyjson5
 
 
 A JSON5 serializer and parser library for Python 3 written in
 `Cython <http://cython.org/>`_.
 
 
 Serializer
```

### Comparing `pyjson5x-1.6.2/docs/changelog.md` & `pyjson5x-1.6.2.1/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/docs/conf.py` & `pyjson5x-1.6.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/docs/decoder.rst` & `pyjson5x-1.6.2.1/docs/.ipynb_checkpoints/decoder-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/docs/encoder.rst` & `pyjson5x-1.6.2.1/docs/encoder.rst`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/docs/index.rst` & `pyjson5x-1.6.2.1/docs/.ipynb_checkpoints/index-checkpoint.rst`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/docs/performance.rst` & `pyjson5x-1.6.2.1/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/make_decoder_recursive_select.py` & `pyjson5x-1.6.2.1/make_decoder_recursive_select.py`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/make_escape_dct.py` & `pyjson5x-1.6.2.1/make_escape_dct.py`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/make_unicode_categories.py` & `pyjson5x-1.6.2.1/make_unicode_categories.py`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/pyjson5x.pyx` & `pyjson5x-1.6.2.1/pyjson5x.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/setup.cfg` & `pyjson5x-1.6.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.6.2
+version = 1.6.2.1
 name = pyjson5x
 description = JSON5 rough serializer and parser for Python 3 written in Cython.
 url = https://github.com/caffeinism/pyjson5x
 author = Kim Minjong
 author_email = make.dirty.code@gmail.com
 long_description = file: README.rst
 long_description_content_type = text/x-rst
@@ -26,15 +26,15 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Text Processing :: General
 
 [options]
 zip_safe = False
-python_requires = ~= 3.5
+python_requires = ~= 3.6
 setup_requires = 
 	Cython
 	setuptools
 	wheel
 include_package_data = True
 packages = pyjson5x
 package_dir =
```

### Comparing `pyjson5x-1.6.2/sha512sum.py` & `pyjson5x-1.6.2.1/sha512sum.py`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/.ipynb_checkpoints/_decoder_recursive_select-checkpoint.hpp` & `pyjson5x-1.6.2.1/src/_decoder_recursive_select.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/DESCRIPTION.inc` & `pyjson5x-1.6.2.1/src/DESCRIPTION.inc`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_constants.pyx` & `pyjson5x-1.6.2.1/src/_constants.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_decoder.pyx` & `pyjson5x-1.6.2.1/src/.ipynb_checkpoints/_decoder-checkpoint.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -162,17 +162,14 @@
         return 0x0000
     elif c0 == b'x':
         return _get_hex_character(reader, 2)
     elif c0 == b'u':
         return _get_escaped_unicode_maybe_surrogate(reader, start)
     elif c0 == b'U':
         return _get_hex_character(reader, 8)
-    elif expect(b'1' <= c0 <= b'9', False):
-        _raise_expected_s('escape sequence', start, c0)
-        return -2
     elif _is_line_terminator(c0):
         if c0 != 0x000D:
             return -1
 
         c0 = _reader_get(reader)
         if c0 == 0x000A:
             return -1
@@ -365,15 +362,15 @@
             buf.push_back(<char> <unsigned char> c0)
         elif not was_point:
             was_point = True
         else:
             _raise_unclosed('NumericLiteral', start)
 
         if not _reader_good(reader):
-            c1 = -1
+            c1 = NO_EXTRA_DATA
             break
 
         c0 = _reader_get(reader)
 
     c_in_out[0] = c1
 
     if leading_point and buf.size() == 1:  # single '.'
@@ -437,34 +434,39 @@
         return _decode_number_any(reader, buf, c_in_out, start)
 
 
 #  1: done
 #  0: data found
 # -1: exception (exhausted)
 cdef uint32_t _skip_comma(ReaderRef reader, Py_ssize_t start,
-                          uint32_t terminator, const char *what,
-                          int32_t *c_in_out) except -1:
+                          uint32_t terminator, uint32_t counter_terminator, 
+                          const char *what, int32_t *c_in_out) except -1:
     cdef int32_t c0
     cdef uint32_t c1
     cdef boolean needs_comma
     cdef uint32_t done
 
     c0 = c_in_out[0]
     c1 = cast_to_uint32(c0)
 
     needs_comma = True
     while True:
         c0 = _skip_to_data_sub(reader, c1)
         if c0 < 0:
-            break
+            c_in_out[0] = NO_EXTRA_DATA
+            return 1
 
         c1 = cast_to_uint32(c0)
         if c1 == terminator:
             c_in_out[0] = NO_EXTRA_DATA
             return 1
+        
+        if c1 == counter_terminator:
+            c_in_out[0] = c0
+            return 1
 
         if c1 != b',':
             if expect(needs_comma, False):
                 _raise_expected_sc(
                     'comma', terminator, _reader_tell(reader), c1,
                 )
             c_in_out[0] = c0
@@ -523,29 +525,32 @@
 
     c_in_out[0] = c0
     return PyUnicode_FromKindAndData(
         PyUnicode_4BYTE_KIND, buf.data(), buf.size(),
     )
 
 
-cdef boolean _decode_object(ReaderRef reader, object result) except False:
+cdef boolean _decode_object(
+    ReaderRef reader, object result, int32_t *c_in_out
+) except False:
     cdef int32_t c0
     cdef uint32_t c1
     cdef Py_ssize_t start
     cdef boolean done
     cdef object key
     cdef object value
     cdef object ex
 
     start = _reader_tell(reader)
 
     c0 = _skip_to_data(reader)
     if expect(c0 >= 0, True):
         c1 = cast_to_uint32(c0)
         if c1 == b'}':
+            c_in_out[0] = NO_EXTRA_DATA
             return True
 
         while True:
             if c1 in b'"\'':
                 key = _decode_string(reader, &c0)
             else:
                 key = _decode_identifier_name(reader, &c0)
@@ -576,57 +581,64 @@
 
             if expect(c0 < 0, False):
                 break
 
             PyDict_SetItem(result, key, value)
 
             done = _skip_comma(
-                reader, start, <unsigned char>b'}', b'object', &c0,
+                reader, start, <unsigned char>b'}',
+                <unsigned char>b']', b'object', &c0,
             )
             if done:
+                c_in_out[0] = c0
                 return True
 
             c1 = cast_to_uint32(c0)
 
     _raise_unclosed(b'object', start)
-    return False
 
 
-cdef boolean _decode_array(ReaderRef reader, object result) except False:
+cdef boolean _decode_array(
+    ReaderRef reader, object result, int32_t *c_in_out
+) except False:
     cdef int32_t c0
     cdef uint32_t c1
     cdef Py_ssize_t start
     cdef boolean done
     cdef object value
     cdef object ex
 
     start = _reader_tell(reader)
 
     c0 = _skip_to_data(reader)
     if expect(c0 >= 0, True):
         c1 = cast_to_uint32(c0)
         if c1 == b']':
+            c_in_out[0] = NO_EXTRA_DATA
             return True
 
         while True:
             try:
                 value = _decode_recursive(reader, &c0)
             except _DecoderException as ex:
                 PyList_Append(result, (<_DecoderException> ex).result)
                 raise
 
             if expect(c0 < 0, False):
+                c_in_out[0] = NO_EXTRA_DATA
                 break
 
             PyList_Append(result, value)
 
             done = _skip_comma(
-                reader, start, <unsigned char>b']', b'array', &c0,
+                reader, start, <unsigned char>b']',
+                <unsigned char>b'}', b'array', &c0,
             )
             if done:
+                c_in_out[0] = c0
                 return True
 
     _raise_unclosed(b'array', start)
 
 
 cdef boolean _accept_string(ReaderRef reader, const char *string) except False:
     cdef uint32_t c0
@@ -682,15 +694,15 @@
     #                       N
     _accept_string(reader, b'aN')
     c_in_out[0] = NO_EXTRA_DATA
     return CONST_POS_NAN
 
 
 cdef object _decode_recursive_enter(ReaderRef reader, int32_t *c_in_out):
-    cdef boolean (*fn)(ReaderRef reader, object result) except False
+    cdef boolean (*fn)(ReaderRef reader, object result, int32_t *c_in_out) except False
     cdef object result
     cdef int32_t c0
     cdef uint32_t c1
     cdef object ex
 
     c0 = c_in_out[0]
     c1 = cast_to_uint32(c0)
@@ -700,24 +712,24 @@
         fn = _decode_object
     else:
         result = []
         fn = _decode_array
 
     _reader_enter(reader)
     try:
-        fn(reader, result)
+        fn(reader, result, &c0)
     except RecursionError:
         _raise_nesting(_reader_tell(reader), result)
     except _DecoderException as ex:
         (<_DecoderException> ex).result = result
         raise
     finally:
         _reader_leave(reader)
 
-    c_in_out[0] = NO_EXTRA_DATA
+    c_in_out[0] = c0
     return result
 
 
 cdef object _decoder_unknown(ReaderRef reader, int32_t *c_in_out):
     cdef int32_t c0
     cdef uint32_t c1
     cdef Py_ssize_t start
```

### Comparing `pyjson5x-1.6.2/src/_encoder.pyx` & `pyjson5x-1.6.2.1/src/_encoder.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_encoder_options.pyx` & `pyjson5x-1.6.2.1/src/_encoder_options.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_escape_dct.hpp` & `pyjson5x-1.6.2.1/src/_escape_dct.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_exceptions_decoder.pyx` & `pyjson5x-1.6.2.1/src/.ipynb_checkpoints/_exceptions_decoder-checkpoint.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_exceptions_encoder.pyx` & `pyjson5x-1.6.2.1/src/_exceptions_encoder.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_exports.pyx` & `pyjson5x-1.6.2.1/src/_exports.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_imports.pyx` & `pyjson5x-1.6.2.1/src/_imports.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_legacy.pyx` & `pyjson5x-1.6.2.1/src/_legacy.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_raise_decoder.pyx` & `pyjson5x-1.6.2.1/src/.ipynb_checkpoints/_raise_decoder-checkpoint.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_reader_callback.pyx` & `pyjson5x-1.6.2.1/src/_reader_callback.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_reader_ucs.pyx` & `pyjson5x-1.6.2.1/src/_reader_ucs.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_readers.pyx` & `pyjson5x-1.6.2.1/src/_readers.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_stack_heap_string.hpp` & `pyjson5x-1.6.2.1/src/_stack_heap_string.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_unicode.pyx` & `pyjson5x-1.6.2.1/src/_unicode.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_unicode_cat_of.hpp` & `pyjson5x-1.6.2.1/src/_unicode_cat_of.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_writer_callback.pyx` & `pyjson5x-1.6.2.1/src/_writer_callback.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/_writer_reallocatable.pyx` & `pyjson5x-1.6.2.1/src/_writer_reallocatable.pyx`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/dragonbox.cc` & `pyjson5x-1.6.2.1/src/dragonbox.cc`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/native.hpp` & `pyjson5x-1.6.2.1/src/native.hpp`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/pyjson5x/__init__.pyi` & `pyjson5x-1.6.2.1/src/pyjson5x/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyjson5x-1.6.2/src/pyjson5x.egg-info/PKG-INFO` & `pyjson5x-1.6.2.1/src/pyjson5x.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjson5x
-Version: 1.6.2
+Version: 1.6.2.1
 Summary: JSON5 rough serializer and parser for Python 3 written in Cython.
 Home-page: https://github.com/caffeinism/pyjson5x
 Author: Kim Minjong
 Author-email: make.dirty.code@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,23 +19,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Text Processing :: General
-Requires-Python: ~=3.5
+Requires-Python: ~=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 PyJSON5x
 ==========
 
 
-This package is the same as pyjson5, but interprets True and False as booleans. For more information, see the source repository. https://github.com/Kijewski/pyjson5
+This package is the same as pyjson5, but this library does some crude decoding. 
+
+- interprets True and False as booleans.
+
+- strive to properly handle unclosed brackets.
+
+
+For more information, see the source repository. https://github.com/Kijewski/pyjson5
 
 
 A JSON5 serializer and parser library for Python 3 written in
 `Cython <http://cython.org/>`_.
 
 
 Serializer
```

### Comparing `pyjson5x-1.6.2/src/pyjson5x.egg-info/SOURCES.txt` & `pyjson5x-1.6.2.1/src/pyjson5x.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 make_decoder_recursive_select.py
 make_escape_dct.py
 make_unicode_categories.py
-pyjson5x.cpp
 pyjson5x.pyx
 pyproject.toml
 setup.cfg
 setup.py
 sha512sum.py
 docs/changelog.md
 docs/conf.py
 docs/decoder.rst
 docs/encoder.rst
 docs/exceptions.rst
 docs/index.rst
 docs/performance.rst
+docs/.ipynb_checkpoints/decoder-checkpoint.rst
+docs/.ipynb_checkpoints/index-checkpoint.rst
 src/DESCRIPTION.inc
 src/VERSION.inc
 src/_constants.pyx
 src/_decoder.pyx
 src/_decoder_recursive_select.hpp
 src/_encoder.pyx
 src/_encoder_options.pyx
@@ -42,15 +43,18 @@
 src/_unicode_cat_of.hpp
 src/_writer_callback.pyx
 src/_writer_noop.pyx
 src/_writer_reallocatable.pyx
 src/_writers.pyx
 src/dragonbox.cc
 src/native.hpp
-src/.ipynb_checkpoints/_decoder_recursive_select-checkpoint.hpp
+src/.ipynb_checkpoints/_decoder-checkpoint.pyx
+src/.ipynb_checkpoints/_exceptions-checkpoint.pyx
+src/.ipynb_checkpoints/_exceptions_decoder-checkpoint.pyx
+src/.ipynb_checkpoints/_raise_decoder-checkpoint.pyx
 src/pyjson5x/__init__.py
 src/pyjson5x/__init__.pyi
 src/pyjson5x/py.typed
 src/pyjson5x.egg-info/PKG-INFO
 src/pyjson5x.egg-info/SOURCES.txt
 src/pyjson5x.egg-info/dependency_links.txt
 src/pyjson5x.egg-info/not-zip-safe
```

### Comparing `pyjson5x-1.6.2/third-party/fast_double_parser/include/fast_double_parser.h` & `pyjson5x-1.6.2.1/third-party/fast_double_parser/include/fast_double_parser.h`

 * *Files identical despite different names*

