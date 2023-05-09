# Comparing `tmp/sybil-5.0.0.tar.gz` & `tmp/sybil-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-5.0.0.tar", last modified: Sun Mar 26 11:38:55 2023, max compression
+gzip compressed data, was "sybil-5.0.1.tar", last modified: Tue May  9 06:59:47 2023, max compression
```

## Comparing `sybil-5.0.0.tar` & `sybil-5.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.243051 sybil-5.0.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-03-26 11:38:42.000000 sybil-5.0.0/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-03-26 11:38:55.243051 sybil-5.0.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-03-26 11:38:42.000000 sybil-5.0.0/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-03-26 11:38:55.243051 sybil-5.0.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-03-26 11:38:42.000000 sybil-5.0.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.239051 sybil-5.0.0/sybil/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8523 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/document.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.239051 sybil-5.0.0/sybil/evaluators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/evaluators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/evaluators/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1600 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/evaluators/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/evaluators/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1775 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/evaluators/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/example.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.239051 sybil-5.0.0/sybil/integration/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/integration/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3911 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/integration/pytest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/integration/unittest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.239051 sybil-5.0.0/sybil/parsers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.243051 sybil-5.0.0/sybil/parsers/abstract/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/abstract/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/abstract/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/abstract/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2145 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/abstract/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/abstract/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/abstract/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/doctest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.243051 sybil-5.0.0/sybil/parsers/myst/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/myst/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/myst/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2784 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/myst/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      989 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/myst/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5747 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/myst/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/myst/skip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.243051 sybil-5.0.0/sybil/parsers/rest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/rest/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/rest/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/rest/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/rest/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/rest/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2688 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/rest/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/rest/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/parsers/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3288 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/region.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6439 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/sybil.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-03-26 11:38:42.000000 sybil-5.0.0/sybil/typing.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 11:38:55.239051 sybil-5.0.0/sybil.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-03-26 11:38:55.000000 sybil-5.0.0/sybil.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-03-26 11:38:55.000000 sybil-5.0.0/sybil.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-26 11:38:55.000000 sybil-5.0.0/sybil.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-03-26 11:38:55.000000 sybil-5.0.0/sybil.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-03-26 11:38:55.000000 sybil-5.0.0/sybil.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2023-05-09 06:59:35.000000 sybil-5.0.1/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-09 06:59:47.863063 sybil-5.0.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2023-05-09 06:59:35.000000 sybil-5.0.1/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-05-09 06:59:47.867063 sybil-5.0.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1002 2023-05-09 06:59:35.000000 sybil-5.0.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8523 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/document.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil/evaluators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1600 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1775 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/evaluators/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/example.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil/integration/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/integration/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3911 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/integration/pytest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1428 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/integration/unittest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/abstract/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      173 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1915 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2145 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3208 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/abstract/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/doctest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/myst/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      175 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      387 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2784 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      989 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      277 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/myst/skip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.863063 sybil-5.0.1/sybil/parsers/rest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2862 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      368 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1465 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2688 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/rest/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/parsers/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3288 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/region.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6439 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/sybil.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      466 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-09 06:59:35.000000 sybil-5.0.1/sybil/typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-09 06:59:47.859063 sybil-5.0.1/sybil.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-09 06:59:47.000000 sybil-5.0.1/sybil.egg-info/top_level.txt
```

### Comparing `sybil-5.0.0/LICENSE.txt` & `sybil-5.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/PKG-INFO` & `sybil-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 5.0.0
+Version: 5.0.1
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `sybil-5.0.0/README.rst` & `sybil-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/setup.py` & `sybil-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 
 setup(
     name='sybil',
-    version='5.0.0',
+    version='5.0.1',
     author='Chris Withers',
     author_email='chris@withers.org',
     license='MIT',
     description="Automated testing for the examples in your code and documentation.",
     long_description=open('README.rst').read(),
     url='https://github.com/simplistix/sybil',
     classifiers=[
```

### Comparing `sybil-5.0.0/sybil/document.py` & `sybil-5.0.1/sybil/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             source_start = start_match.end()
             end_match = end_pattern.search(self.text, source_start)
             source_end = end_match.start()
             source = self.text[source_start:source_end]
             yield start_match, end_match, source
 
 
-DOCSTRING_PUNCTUATION = re.compile('["\']{3}|["\']')
+DOCSTRING_PUNCTUATION = re.compile('[rf]?(["\']{3}|["\'])')
 
 
 class PythonDocument(Document):
     """
     A :class:`~sybil.Document` type that imports the document's source
     file as a Python module, making names within it available in the document's
     :attr:`~sybil.Document.namespace`.
@@ -176,15 +176,15 @@
                     isinstance(docstring, Str) or
                     isinstance(docstring, Constant) and isinstance(docstring.value, str)
             ):
                 continue
             node_start = line_offsets.get(docstring.lineno-1, docstring.col_offset)
             node_end = line_offsets.get(docstring.end_lineno-1, docstring.end_col_offset)
             punc = DOCSTRING_PUNCTUATION.match(python_source_code, node_start, node_end)
-            punc_size = punc.end() - punc.start()
+            punc_size = len(punc.group(1))
             start = punc.end()
             end = node_end - punc_size
             yield start, end, python_source_code[start:end]
 
     @classmethod
     def parse(cls, path: str, *parsers: Parser, encoding: str = 'utf-8') -> 'Document':
         """
```

### Comparing `sybil-5.0.0/sybil/evaluators/doctest.py` & `sybil-5.0.1/sybil/evaluators/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/evaluators/python.py` & `sybil-5.0.1/sybil/evaluators/python.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/evaluators/skip.py` & `sybil-5.0.1/sybil/evaluators/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/example.py` & `sybil-5.0.1/sybil/example.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/integration/pytest.py` & `sybil-5.0.1/sybil/integration/pytest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/integration/unittest.py` & `sybil-5.0.1/sybil/integration/unittest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/abstract/clear.py` & `sybil-5.0.1/sybil/parsers/abstract/clear.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/abstract/codeblock.py` & `sybil-5.0.1/sybil/parsers/abstract/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/abstract/doctest.py` & `sybil-5.0.1/sybil/parsers/abstract/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/abstract/lexers.py` & `sybil-5.0.1/sybil/parsers/abstract/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/abstract/skip.py` & `sybil-5.0.1/sybil/parsers/abstract/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/myst/codeblock.py` & `sybil-5.0.1/sybil/parsers/myst/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/myst/doctest.py` & `sybil-5.0.1/sybil/parsers/myst/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/myst/lexers.py` & `sybil-5.0.1/sybil/parsers/myst/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/rest/capture.py` & `sybil-5.0.1/sybil/parsers/rest/capture.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/rest/codeblock.py` & `sybil-5.0.1/sybil/parsers/rest/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/rest/doctest.py` & `sybil-5.0.1/sybil/parsers/rest/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/parsers/rest/lexers.py` & `sybil-5.0.1/sybil/parsers/rest/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/python.py` & `sybil-5.0.1/sybil/python.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/region.py` & `sybil-5.0.1/sybil/region.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil/sybil.py` & `sybil-5.0.1/sybil/sybil.py`

 * *Files identical despite different names*

### Comparing `sybil-5.0.0/sybil.egg-info/PKG-INFO` & `sybil-5.0.1/sybil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 5.0.0
+Version: 5.0.1
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `sybil-5.0.0/sybil.egg-info/SOURCES.txt` & `sybil-5.0.1/sybil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

