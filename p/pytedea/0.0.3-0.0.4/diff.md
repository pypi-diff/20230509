# Comparing `tmp/pytedea-0.0.3.tar.gz` & `tmp/pytedea-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytedea-0.0.3.tar", last modified: Thu May  4 14:31:56 2023, max compression
+gzip compressed data, was "pytedea-0.0.4.tar", last modified: Tue May  9 14:01:28 2023, max compression
```

## Comparing `pytedea-0.0.3.tar` & `pytedea-0.0.4.tar`

### file list

```diff
@@ -1,79 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.983391 pytedea-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-04 14:31:38.000000 pytedea-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 14:31:38.000000 pytedea-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-04 14:31:56.983391 pytedea-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-04 14:31:38.000000 pytedea-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.975391 pytedea-0.0.3/pytedea/
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DDF.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DDFt.py
--rw-r--r--   0 runner    (1001) docker     (123)    23332 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DEA.py
--rw-r--r--   0 runner    (1001) docker     (123)   138273 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/DEAt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/HYPER.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/HYPERt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/NDDF.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/pytedea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.983391 pytedea-0.0.3/pytedea/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CNLSZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/CQERZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/sweet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28389 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSbZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCNLSxZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERDDFZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERbZG2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxG2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxZG1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-04 14:31:38.000000 pytedea-0.0.3/pytedea/utils/weakCQERxZG2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:31:56.975391 pytedea-0.0.3/pytedea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 14:31:56.000000 pytedea-0.0.3/pytedea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 14:31:38.000000 pytedea-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 14:31:56.983391 pytedea-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-04 14:31:38.000000 pytedea-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:28.074285 pytedea-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-09 14:01:10.000000 pytedea-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 14:01:10.000000 pytedea-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-09 14:01:28.074285 pytedea-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 14:01:10.000000 pytedea-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:28.070285 pytedea-0.0.4/pytedea/
+-rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/DDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/DDFt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/DEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138792 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/DEAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/HYPER.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/HYPERt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/MQDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/MQDDFt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/MQDEA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/MQDEAt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/MQNDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/NDDF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/pytedea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:28.074285 pytedea-0.0.4/pytedea/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/CQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/sweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9053 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCNLSxZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERDDFG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERDDFG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERDDFZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERDDFZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERbG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERbG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERbZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERbZG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERxG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERxG2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERxZG1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-09 14:01:10.000000 pytedea-0.0.4/pytedea/utils/weakCQERxZG2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 14:01:28.070285 pytedea-0.0.4/pytedea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-09 14:01:27.000000 pytedea-0.0.4/pytedea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-09 14:01:28.000000 pytedea-0.0.4/pytedea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 14:01:27.000000 pytedea-0.0.4/pytedea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 14:01:27.000000 pytedea-0.0.4/pytedea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 14:01:27.000000 pytedea-0.0.4/pytedea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 14:01:27.000000 pytedea-0.0.4/pytedea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 14:01:10.000000 pytedea-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-09 14:01:28.078286 pytedea-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-09 14:01:10.000000 pytedea-0.0.4/setup.py
```

### Comparing `pytedea-0.0.3/LICENSE` & `pytedea-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/PKG-INFO` & `pytedea-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedea
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data envelopment analysis using Python.
 Home-page: https://github.com/advancehs/pytedea
 Author: advancehs
 Author-email: 1019753743@qq.com
 License: GNU General Public License v3
 Keywords: pytedea
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedea-0.0.3/pytedea/DDF.py` & `pytedea-0.0.4/pytedea/DDF.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,21 +48,21 @@
             self.__model__.I2 = Set(initialize= self.xref.index)                     ## I2 是 参考决策单元的数量
             self.__model__.K = Set(initialize=range(len(self.x.iloc[0])))   ## K 是投入个数
             self.__model__.L = Set(initialize=range(len(self.y.iloc[0])))   ## L 是产出个数 被评价单元和参考单元的K，L一样
             self.__model__.J = Set(initialize=range(len(self.b.iloc[0])))   ## J 是非期望产出个数
 
 
             # Initialize variable
-            self.__model__.beta = Var(Set(initialize=range(1)),bounds=(0.0, None), \
+            self.__model__.beta = Var(Set(initialize=range(1)),bounds=(0.0, 1), \
                                       within=Reals,doc='directional distance')
             self.__model__.lamda = Var(self.__model__.I2, bounds=(0.0, None),within=Reals, doc='intensity variables')
             if self.rts == RTS_VRS:
                 if self.emf == EMF_SAME:
                     if abs(np.asarray(self.gx).sum())>=1:
-                        self.__model__.beta2 = Var(Set(initialize=range(1)), bounds=(0.0, None), \
+                        self.__model__.beta2 = Var(Set(initialize=range(1)), bounds=(0.0, 1), \
                                                   within=Reals, doc='beta*theta')
                     self.__model__.theta = Var(Set(initialize=range(1)), bounds=(0.0, 1.0), \
                                               within=Reals, doc='theta')
                 elif self.emf == EMF_DIFFERENT:
                     self.__model__.phi = Var(self.__model__.I2, bounds=(0.0, None), within=Reals, doc='phi_i')
                     self.__model__.mu = Var(self.__model__.I2, bounds=(0.0, None),within=Reals, doc='mu_i')
                 else:
```

### Comparing `pytedea-0.0.3/pytedea/DDFt.py` & `pytedea-0.0.4/pytedea/DDFt.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import pandas as pd
 from .constant import CET_ADDI, ORIENT_IO, ORIENT_OO,ORIENT_HYPERYB, RTS_VRS, RTS_CRS, OPT_DEFAULT, OPT_LOCAL
 from .utils import tools
 from .DEAt import DEAt
 import ast
 
 class DDFt(DEAt):
-    def __init__(self, data,sent = "inputvar=outputvar",  gy=[1], gx=[1],rts=RTS_VRS, baseindex=None,refindex=None):
+    def __init__(self, data,sent = "inputvar=outputvar",  \
+                 gy=[1], gx=[1],rts=RTS_VRS, baseindex=None,refindex=None):
         """DEA: Directional distance function
 
         Args:
             data (pandas.DataFrame): input pandas.
             sent (str): inputvars=outputvars[: unoutputvars]. e.g.: "K L CO2= Y"
             gy (list, optional): output directional vector. Defaults to [1].
             gx (list, optional): input directional vector. Defaults to [1].
@@ -52,15 +53,15 @@
             # Initialize sets
             self.__model__.I2 = Set(initialize= self.xref.index)                     ## I2 是 参考决策单元的数量
             self.__model__.K = Set(initialize=range(len(self.x.iloc[0])))          ## K 是投入个数
             self.__model__.L = Set(initialize=range(len(self.y.iloc[0])))          ## L 是产出个数 被评价单元和参考单元的K，L一样
 
 
             # Initialize variable
-            self.__model__.theta = Var(Set(initialize=range(1)),bounds=(0.0, None), within=Reals,doc='directional distance')
+            self.__model__.beta = Var(Set(initialize=range(1)),bounds=(0.0, None), within=Reals,doc='directional distance')
             self.__model__.lamda = Var(self.__model__.I2, bounds=(0.0, None),within=Reals, doc='intensity variables')
 
             # Setup the objective function and constraints
             self.__model__.objective = Objective(rule=self.__objective_rule(), sense=maximize, doc='objective function')
             self.__model__.input = Constraint(self.__model__.K,  rule=self.__input_rule(), doc='input constraint')
             self.__model__.output = Constraint(self.__model__.L,  rule=self.__output_rule(), doc='output constraint')
 
@@ -70,29 +71,29 @@
 
             self.__modeldict[i] = self.__model__
 
         # Optimize model
     def __objective_rule(self):
         """Return the proper objective function"""
         def objective_rule(model):
-            return model.theta[0]*1
+            return model.beta[0]*1
         return objective_rule
 
     def __input_rule(self):
         """Return the proper input constraint"""
         def input_rule(model, k):
             return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2
-                    ) - model.theta[0]*self.gx[k]*self.x.loc[self.I0,self.xcol[k]] <= self.x.loc[self.I0,self.xcol[k]]
+                    ) - model.beta[0]*self.gx[k]*self.x.loc[self.I0,self.xcol[k]] <= self.x.loc[self.I0,self.xcol[k]]
         return input_rule
 
     def __output_rule(self):
         """Return the proper output constraint"""
         def output_rule(model, l):
             return -sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2
-                    ) + model.theta[0]*self.gy[l] *self.y.loc[self.I0,self.ycol[l]]<= -self.y.loc[self.I0,self.ycol[l]]
+                    ) + model.beta[0]*self.gy[l] *self.y.loc[self.I0,self.ycol[l]]<= -self.y.loc[self.I0,self.ycol[l]]
         return output_rule
 
     def __vrs_rule(self):
 
         def vrs_rule(model):
             return sum(model.lamda[ i2] for i2 in model.I2) == 1
 
@@ -103,24 +104,22 @@
         """Optimize the function by requested method
 
         Args:
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
         """
         # TODO(error/warning handling): Check problem status after optimization
 
-        data2,theta,lamda,= pd.DataFrame(),{},{}
+        data2,beta,lamda,= pd.DataFrame(),{},{}
         for ind, problem in self.__modeldict.items():
             _, data2.loc[ind,"optimization_status"]= tools.optimize_model2(problem, ind, solver)
-            theta[ind],= np.asarray(list(problem.theta[:].value))
-            # lamda[ind] =  np.asarray(list(problem.lamda[:].value))
-        # print(theta)
-        theta = pd.DataFrame(theta,index=["theta"]).T
+            beta[ind],= np.asarray(list(problem.beta[:].value))
+        beta = pd.DataFrame(beta,index=["beta"]).T
         # lamda2 = pd.DataFrame(lamda).T
         # lamda2.columns = map(lambda x: "lamda"+str(x) ,lamda2.columns)
-        data3 = pd.concat([data2,theta],axis=1)
+        data3 = pd.concat([data2,beta],axis=1)
         return data3
 
     def info(self, dmu = "all"):
         """Show the infomation of the lp model
 
         Args:
             dmu (string): The solver chosen for optimization. Default is "all".
```

### Comparing `pytedea-0.0.3/pytedea/DEA.py` & `pytedea-0.0.4/pytedea/DEA.py`

 * *Files 2% similar despite different names*

```diff
@@ -388,35 +388,35 @@
                     data2.loc[ind, "theta"] = np.asarray(list(problem.theta[:].value))
 
                     if (self.orient == ORIENT_IO) | (type(self.xindexs)!=type(None) ):
                         data2.loc[ind,"beta2"] = np.asarray(list(problem.beta2[:].value))
                         data2["beta"] = data2["beta2"] / data2["theta"]
                     else:
                         data2.loc[ind,"beta"] = np.asarray(list(problem.beta[:].value))
-                if self.orient == ORIENT_OO:
+                if (self.orient == ORIENT_OO)  | (type(self.yindexs) != type(None)):
                     data2["te"] = 1 / data2["beta"]
                 else:
                     data2["te"] = data2["beta"]
             elif self.emf==EMF_DIFFERENT:
                 data2 = pd.DataFrame()
                 for ind, problem in self.__modeldict.items():
                     _, data2.loc[ind, "optimization_status"] = tools.optimize_model2(problem, ind, solver)
                     data2.loc[ind, "beta"] = np.asarray(list(problem.beta[:].value))
-                if self.orient == ORIENT_OO:
+                if (self.orient == ORIENT_OO)  | (type(self.yindexs) != type(None)):
                     data2["te"] = 1 / data2["beta"]
                 else:
                     data2["te"] = data2["beta"]
             else:
                 raise ValueError("Undefined model parameters.")
         elif self.rts == RTS_CRS:
             data2 = pd.DataFrame()
             for ind, problem in self.__modeldict.items():
                 _, data2.loc[ind,"optimization_status"] = tools.optimize_model2(problem, ind, solver)
                 data2.loc[ind,"beta"] = np.asarray(list(problem.beta[:].value))
-            if self.orient == ORIENT_OO:
+            if (self.orient == ORIENT_OO) | (type(self.yindexs) != type(None)):
                 data2["te"] = 1 / data2["beta"]
             else:
                 data2["te"] = data2["beta"]
         else:
             raise ValueError("Undefined model parameters.")
         return data2
```

### Comparing `pytedea-0.0.3/pytedea/DEAt.py` & `pytedea-0.0.4/pytedea/DEAt.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,23 @@
 
             self.__model__.I2 = Set(initialize=  self.xref.index)       ## I2 是 参考决策单元的数量
 
             self.__model__.K = Set(initialize=range(len(self.x.iloc[0])))          ## K 是投入个数
             self.__model__.L = Set(initialize=range(len(self.y.iloc[0])))           ## L 是产出个数 被评价单元和参考单元的K，L一样
 
             # Initialize variable
-            self.__model__.theta = Var(Set(initialize=range(1)),bounds=(None, None), doc='efficiency')
-            if self.orient == ORIENT_HYPERYX:
-                self.__model__.delta = Var(Set(initialize=range(1)),bounds=(None, None), doc='efficiency**2')
+            if self.orient == ORIENT_IO:
+                self.__model__.beta = Var(Set(initialize=range(1)),bounds=(0, 1), doc='efficiency')
+            elif self.orient == ORIENT_OO:
+                self.__model__.beta = Var(Set(initialize=range(1)),bounds=(1, None), doc='efficiency')
+            else:
+                if type(self.xindexs)!=type(None):
+                    self.__model__.beta = Var(Set(initialize=range(1)), bounds=(0, 1), doc='efficiency')
+                else:
+                    self.__model__.beta = Var(Set(initialize=range(1)), bounds=(1, None), doc='efficiency')
 
             self.__model__.lamda = Var(self.__model__.I2, bounds=(0.0, None), doc='intensity variables')
 
             # Setup the objective function and constraints
             if self.orient == ORIENT_IO:
                 self.__model__.objective = Objective(
                     rule=self.__objective_rule(), sense=minimize, doc='objective function')
@@ -98,62 +104,62 @@
 
         # # Optimize model
 
 
     def __objective_rule(self):
         """Return the proper objective function"""
         def objective_rule(model):
-            return model.theta[0]*1  + sum(model.lamda[i2] *0 for i2 in model.I2)
+            return model.beta[0]*1  + sum(model.lamda[i2] *0 for i2 in model.I2)
         return objective_rule
 
 
     def __input_rule(self):
         """Return the proper input constraint"""
         if self.orient == ORIENT_OO:
             def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
                     self.x.loc[self.I0,self.xcol[k]]
         elif self.orient == ORIENT_IO:
             def input_rule(model, k):
                 return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
-                    model.theta * self.x.loc[self.I0,self.xcol[k]]
+                    model.beta * self.x.loc[self.I0,self.xcol[k]]
 
         else:
             if type(self.xindexs)!=type(None):
                 def input_rule(model, k):
                     if k != self.xindexs:
                         return Constraint.Skip
                     return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= \
-                        model.theta * self.x.loc[self.I0,self.xcol[k]]
+                        model.beta * self.x.loc[self.I0,self.xcol[k]]
             else:
                 def input_rule(model, k):
                     return sum(model.lamda[i2] * self.xref.loc[i2,self.xcol[k]] for i2 in model.I2) <= self.x.loc[self.I0,self.xcol[k]]
 
         return input_rule
 
 
 
     def __output_rule(self):
         """Return the proper output constraint"""
         if self.orient == ORIENT_OO:
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
-                    >=model.theta * self.y.loc[self.I0,self.ycol[l]]
+                    >=model.beta * self.y.loc[self.I0,self.ycol[l]]
         elif self.orient == ORIENT_IO:
             def output_rule(model, l):
                 return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                     >= self.y.loc[self.I0,self.ycol[l]]
 
         else:
             if type(self.yindexs)!=type(None):
                 def output_rule(model, l):
                     if l != self.yindexs:
                         return Constraint.Skip
                     return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
-                        >= model.theta * self.y.loc[self.I0,self.ycol[l]]
+                        >= model.beta * self.y.loc[self.I0,self.ycol[l]]
             else:
                 def output_rule(model, l):
                     return sum(model.lamda[i2] * self.yref.loc[i2,self.ycol[l]] for i2 in model.I2) \
                         >= self.y.loc[self.I0,self.ycol[l]]
 
         return output_rule
 
@@ -169,20 +175,25 @@
             solver (string): The solver chosen for optimization. It will optimize with default solver if OPT_DEFAULT is given.
         """
         # TODO(error/warning handling): Check problem status after optimization
 
         data2,lamda = pd.DataFrame(),{}
         for ind, problem in self.__modeldict.items():
             _, data2.loc[ind,"optimization_status"] = tools.optimize_model2(problem, ind, solver)
-            data2.loc[ind,"theta"] = np.asarray(list(problem.theta[:].value))
+            data2.loc[ind,"beta"] = np.asarray(list(problem.beta[:].value))
 
         if self.orient==ORIENT_OO:
-            data2["te"] = 1/  data2["theta"]
+            data2["te"] = 1/  data2["beta"]
+        elif self.orient == ORIENT_IO:
+            data2["te"] = data2["beta"]
         else:
-            data2["te"] = data2["theta"]
+            if type(self.xindexs)!=type(None):
+                data2["te"] = data2["beta"]
+            else:
+                data2["te"] = 1 / data2["beta"]
         return data2
 
     def info(self, dmu = "all"):
         """Show the infomation of the lp model
 
         Args:
             dmu (string): The solver chosen for optimization. Default is "all".
```

### Comparing `pytedea-0.0.3/pytedea/HYPER.py` & `pytedea-0.0.4/pytedea/HYPER.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/HYPERt.py` & `pytedea-0.0.4/pytedea/HYPERt.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/NDDF.py` & `pytedea-0.0.4/pytedea/NDDF.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/__init__.py` & `pytedea-0.0.4/pytedea/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = """advancehs"""
 __email__ = '1019753743@qq.com'
-__version__ = '0.0.3'
+__version__ = '0.0.4'
 
 from . import DEAt
 from . import DDFt
 from . import DEA
 from . import DDF
 from . import HYPER
 # from . import CQER
```

### Comparing `pytedea-0.0.3/pytedea/constant.py` & `pytedea-0.0.4/pytedea/constant.py`

 * *Files 26% similar despite different names*

```diff
@@ -94,14 +94,48 @@
     ORIENT_IO: "Input orientation",
     ORIENT_OO: "Output orientation",
     ORIENT_UO: "Undesirable Output orientation",
     ORIENT_HYPERYB: "Hyperbolic orientation for desirable outputs and undesirable outputs",
     ORIENT_HYPERYX: "Hyperbolic orientation for desirable outputs and inputs"
 }
 
+
+# technology
+TOTAL = "Global production technology"
+"""
+    window(#)                   use window production technology with the #-period bandwidth
+    biennial                    use biennial production technology
+    sequential                  use sequential production technology
+    TOTAL:  Global production technology.
+"""
+CONTEMPORARY = "Contemporary production technolog"
+"""
+CONTEMPORARY:  Contemporary production technology.
+"""
+
+TECH_Categories = {
+    TOTAL: "Global production technology",
+    CONTEMPORARY:"Contemporary production technology"
+}
+
+# dynamic productivity index
+MAL = " malquist prodcutivity index or malquist-luenberger prodcutivity index"
+
+"""
+    MAL              malquist prodcutivity index or malquist-luenberger prodcutivity index
+"""
+LUE = "luenberger prodcutivity index"
+"""
+    LUE              luenberger prodcutivity index
+"""
+DYNAMIC_Categories = {
+    MAL : " malquist prodcutivity index or malquist-luenberger prodcutivity index",
+    LUE : "luenberger prodcutivity index"
+}
+
 # left-hand or right-hand Derivative
 LEFT = "left-hand Derivative"
 """
 LEFT: left-hand Derivative.
 """
 
 RIGHT = "right-hand Derivative"
```

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSDDFG1.py` & `pytedea-0.0.4/pytedea/utils/CNLSDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSDDFG2.py` & `pytedea-0.0.4/pytedea/utils/CNLSDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSDDFZG1.py` & `pytedea-0.0.4/pytedea/utils/CNLSDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSDDFZG2.py` & `pytedea-0.0.4/pytedea/utils/CNLSDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSG1.py` & `pytedea-0.0.4/pytedea/utils/CNLSG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSG2.py` & `pytedea-0.0.4/pytedea/utils/CNLSG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSZG1.py` & `pytedea-0.0.4/pytedea/utils/CNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CNLSZG2.py` & `pytedea-0.0.4/pytedea/utils/CNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERDDFG1.py` & `pytedea-0.0.4/pytedea/utils/CQERDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERDDFG2.py` & `pytedea-0.0.4/pytedea/utils/CQERDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERDDFZG1.py` & `pytedea-0.0.4/pytedea/utils/CQERDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERDDFZG2.py` & `pytedea-0.0.4/pytedea/utils/CQERDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERG1.py` & `pytedea-0.0.4/pytedea/utils/CQERG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERG2.py` & `pytedea-0.0.4/pytedea/utils/CQERG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERZG1.py` & `pytedea-0.0.4/pytedea/utils/CQERZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/CQERZG2.py` & `pytedea-0.0.4/pytedea/utils/CQERZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/interpolation.py` & `pytedea-0.0.4/pytedea/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/sweet.py` & `pytedea-0.0.4/pytedea/utils/sweet.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/tools.py` & `pytedea-0.0.4/pytedea/utils/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -193,14 +193,15 @@
                                   ], data.loc[:, unoutputvars]
 
     if x.shape[0] != y.shape[0]:
         raise ValueError(
             "Number of DMUs must be the same in x and y.")
     return outputvars,inputvars, unoutputvars,y, x,b ,yref, xref,bref
 
+
 def assert_valid_ddf(sent,gy,gx,gb):
     inputvars = sent.split('=')[0].strip(' ').split(' ')
     try:
         outputvars = sent.split('=')[1].split(':')[0].strip(' ').split(' ')
         unoutputvars = sent.split('=')[1].split(':')[1].strip(' ').split(' ')
     except:
         outputvars = sent.split('=')[1].strip(' ').split(' ')
@@ -245,16 +246,28 @@
                                   ], data.loc[:, unoutputvars]
 
     if x.shape[0] != y.shape[0]:
         raise ValueError(
             "Number of DMUs must be the same in x and y.")
     return y, x,b ,yref, xref,bref
 
+def assert_valid_mqdea(sent):
+    inputvars = sent.split('=')[0].strip(' ').split(' ')
+    try:
+        outputvars = sent.split('=')[1].split(':')[0].strip(' ').split(' ')
+        unoutputvars = sent.split('=')[1].split(':')[1].strip(' ').split(' ')
+    except:
+        outputvars = sent.split('=')[1].strip(' ').split(' ')
+        unoutputvars = None
+    return inputvars,outputvars,unoutputvars
 
-
+def assert_valid_mqdeat(sent):
+    inputvars = sent.split('=')[0].strip(' ').split(' ')
+    outputvars = sent.split('=')[1].strip(' ').split(' ')
+    return inputvars,outputvars
 
 def assert_valid_basic_data(y, x, z=None):
     y = trans_list(y)
     x = trans_list(x)
 
     y = to_1d_list(y)
     x = to_2d_list(x)
```

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSDDFG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSDDFG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSDDFZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSbG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSbG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSbG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSbG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSbZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSbZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSbZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSbZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSxG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSxG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSxG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSxG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSxZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSxZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCNLSxZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCNLSxZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERDDFG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERDDFG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERDDFG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERDDFG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERDDFZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERDDFZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERDDFZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERDDFZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERbG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERbG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERbG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERbG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERbZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERbZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERbZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERbZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERxG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERxG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERxG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERxG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERxZG1.py` & `pytedea-0.0.4/pytedea/utils/weakCQERxZG1.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea/utils/weakCQERxZG2.py` & `pytedea-0.0.4/pytedea/utils/weakCQERxZG2.py`

 * *Files identical despite different names*

### Comparing `pytedea-0.0.3/pytedea.egg-info/PKG-INFO` & `pytedea-0.0.4/pytedea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytedea
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data envelopment analysis using Python.
 Home-page: https://github.com/advancehs/pytedea
 Author: advancehs
 Author-email: 1019753743@qq.com
 License: GNU General Public License v3
 Keywords: pytedea
 Classifier: Intended Audience :: Developers
```

### Comparing `pytedea-0.0.3/pytedea.egg-info/SOURCES.txt` & `pytedea-0.0.4/pytedea.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 setup.py
 pytedea/DDF.py
 pytedea/DDFt.py
 pytedea/DEA.py
 pytedea/DEAt.py
 pytedea/HYPER.py
 pytedea/HYPERt.py
+pytedea/MQDDF.py
+pytedea/MQDDFt.py
+pytedea/MQDEA.py
+pytedea/MQDEAt.py
+pytedea/MQNDDF.py
 pytedea/NDDF.py
 pytedea/__init__.py
 pytedea/constant.py
 pytedea/pytedea.py
 pytedea.egg-info/PKG-INFO
 pytedea.egg-info/SOURCES.txt
 pytedea.egg-info/dependency_links.txt
```

### Comparing `pytedea-0.0.3/setup.py` & `pytedea-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='pytedea',
     name='pytedea',
     packages=find_packages(include=['pytedea', 'pytedea.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/advancehs/pytedea',
-    version='0.0.3',
+    version='0.0.4',
     zip_safe=False,
 )
```

