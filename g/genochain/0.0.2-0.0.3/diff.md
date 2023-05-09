# Comparing `tmp/genochain-0.0.2.tar.gz` & `tmp/genochain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genochain-0.0.2.tar", last modified: Tue May  9 17:10:17 2023, max compression
+gzip compressed data, was "genochain-0.0.3.tar", last modified: Tue May  9 17:17:08 2023, max compression
```

## Comparing `genochain-0.0.2.tar` & `genochain-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:10:17.069451 genochain-0.0.2/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:10:17.068980 genochain-0.0.2/PKG-INFO
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:10:17.064308 genochain-0.0.2/genochain/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      581 2023-05-09 13:51:15.000000 genochain-0.0.2/genochain/Block.py
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       33 2023-05-09 16:20:34.000000 genochain-0.0.2/genochain/__init__.py
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)     3661 2023-05-09 13:50:25.000000 genochain-0.0.2/genochain/genochain.py
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:10:17.067909 genochain-0.0.2/genochain.egg-info/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:10:16.000000 genochain-0.0.2/genochain.egg-info/PKG-INFO
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      204 2023-05-09 17:10:17.000000 genochain-0.0.2/genochain.egg-info/SOURCES.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)        1 2023-05-09 17:10:16.000000 genochain-0.0.2/genochain.egg-info/dependency_links.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       10 2023-05-09 17:10:16.000000 genochain-0.0.2/genochain.egg-info/top_level.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       38 2023-05-09 17:10:17.069662 genochain-0.0.2/setup.cfg
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)     1154 2023-05-09 17:08:57.000000 genochain-0.0.2/setup.py
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:17:08.292374 genochain-0.0.3/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:17:08.291940 genochain-0.0.3/PKG-INFO
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:17:08.286016 genochain-0.0.3/genochain/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      581 2023-05-09 13:51:15.000000 genochain-0.0.3/genochain/Block.py
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       51 2023-05-09 17:16:29.000000 genochain-0.0.3/genochain/__init__.py
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)     3661 2023-05-09 13:50:25.000000 genochain-0.0.3/genochain/genochain.py
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:17:08.290848 genochain-0.0.3/genochain.egg-info/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:17:08.000000 genochain-0.0.3/genochain.egg-info/PKG-INFO
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      204 2023-05-09 17:17:08.000000 genochain-0.0.3/genochain.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)        1 2023-05-09 17:17:08.000000 genochain-0.0.3/genochain.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       10 2023-05-09 17:17:08.000000 genochain-0.0.3/genochain.egg-info/top_level.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       38 2023-05-09 17:17:08.292527 genochain-0.0.3/setup.cfg
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)     1154 2023-05-09 17:14:23.000000 genochain-0.0.3/setup.py
```

### Comparing `genochain-0.0.2/PKG-INFO` & `genochain-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genochain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Storing and versioning genomics data on a blockchain
 Author: GenoChain(Sanjana Sharma)
 Author-email: <sharmasanjana1947@gmail.com>
 Keywords: python,blockchain,genomics,fasta,block,biology
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genochain-0.0.2/genochain/Block.py` & `genochain-0.0.3/genochain/Block.py`

 * *Files identical despite different names*

### Comparing `genochain-0.0.2/genochain/genochain.py` & `genochain-0.0.3/genochain/genochain.py`

 * *Files identical despite different names*

### Comparing `genochain-0.0.2/genochain.egg-info/PKG-INFO` & `genochain-0.0.3/genochain.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genochain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Storing and versioning genomics data on a blockchain
 Author: GenoChain(Sanjana Sharma)
 Author-email: <sharmasanjana1947@gmail.com>
 Keywords: python,blockchain,genomics,fasta,block,biology
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genochain-0.0.2/setup.py` & `genochain-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Storing and versioning genomics data on a blockchain'
 LONG_DESCRIPTION = 'The provided code is a Python implementation of a simple blockchain. It allows for the creation of a genesis block with a given FASTA sequence, addition of new blocks with a given FASTA sequence and associated ID, and versioning of FASTA sequences. The blockchain can also be checked and printed. This code is licensed under the MIT License.'
 
 # Setting up
 setup(
     name="genochain",
     version=VERSION,
```

