# Comparing `tmp/genochain-0.0.4.tar.gz` & `tmp/genochain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genochain-0.0.4.tar", last modified: Tue May  9 17:24:07 2023, max compression
+gzip compressed data, was "genochain-0.0.5.tar", last modified: Tue May  9 17:34:49 2023, max compression
```

## Comparing `genochain-0.0.4.tar` & `genochain-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:24:07.145028 genochain-0.0.4/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:24:07.144673 genochain-0.0.4/PKG-INFO
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:24:07.139996 genochain-0.0.4/genochain/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      581 2023-05-09 13:51:15.000000 genochain-0.0.4/genochain/Block.py
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       52 2023-05-09 17:22:40.000000 genochain-0.0.4/genochain/__init__.py
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)     3661 2023-05-09 13:50:25.000000 genochain-0.0.4/genochain/genochain.py
-drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:24:07.143874 genochain-0.0.4/genochain.egg-info/
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:24:07.000000 genochain-0.0.4/genochain.egg-info/PKG-INFO
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)      204 2023-05-09 17:24:07.000000 genochain-0.0.4/genochain.egg-info/SOURCES.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)        1 2023-05-09 17:24:07.000000 genochain-0.0.4/genochain.egg-info/dependency_links.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       10 2023-05-09 17:24:07.000000 genochain-0.0.4/genochain.egg-info/top_level.txt
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)       38 2023-05-09 17:24:07.145168 genochain-0.0.4/setup.cfg
--rw-r--r--   0 sanjana.sharma   (502) staff       (20)     1154 2023-05-09 17:23:45.000000 genochain-0.0.4/setup.py
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:34:49.620398 genochain-0.0.5/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:34:49.619966 genochain-0.0.5/PKG-INFO
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:34:49.615217 genochain-0.0.5/genochain/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       35 2023-05-09 17:34:02.000000 genochain-0.0.5/genochain/__init__.py
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)     4201 2023-05-09 17:33:17.000000 genochain-0.0.5/genochain/genochain.py
+drwxr-xr-x   0 sanjana.sharma   (502) staff       (20)        0 2023-05-09 17:34:49.619148 genochain-0.0.5/genochain.egg-info/
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      871 2023-05-09 17:34:49.000000 genochain-0.0.5/genochain.egg-info/PKG-INFO
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)      185 2023-05-09 17:34:49.000000 genochain-0.0.5/genochain.egg-info/SOURCES.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)        1 2023-05-09 17:34:49.000000 genochain-0.0.5/genochain.egg-info/dependency_links.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       10 2023-05-09 17:34:49.000000 genochain-0.0.5/genochain.egg-info/top_level.txt
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)       38 2023-05-09 17:34:49.620657 genochain-0.0.5/setup.cfg
+-rw-r--r--   0 sanjana.sharma   (502) staff       (20)     1154 2023-05-09 17:33:29.000000 genochain-0.0.5/setup.py
```

### Comparing `genochain-0.0.4/PKG-INFO` & `genochain-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genochain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Storing and versioning genomics data on a blockchain
 Author: GenoChain(Sanjana Sharma)
 Author-email: <sharmasanjana1947@gmail.com>
 Keywords: python,blockchain,genomics,fasta,block,biology
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genochain-0.0.4/genochain/genochain.py` & `genochain-0.0.5/genochain/genochain.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 import json
 import hashlib
 import time
 
+class Block:
+    def __init__(self, index, timestamp, data, previous_hash, version_changes):
+        self.index = index
+        self.timestamp = timestamp
+        self.data = data
+        self.previous_hash = previous_hash
+        self.version_changes = version_changes
+        self.hash = self.calculate_hash()
+
+    def calculate_hash(self):
+        return hashlib.sha256(str(self.index).encode() + str(self.timestamp).encode() + str(self.data).encode() + str(self.previous_hash).encode() + str(self.version_changes).encode()).hexdigest()
 
 class BlockChain:
     def __init__(self, genesis_fasta):
         self.chain = [self.create_genesis_block(genesis_fasta)]
 
     def create_genesis_block(self, genesis_fasta):
         return Block(0, time.time(), {"id": "Genesis Block", "fasta": genesis_fasta}, "0", {"version-1": "Initial version"})
```

### Comparing `genochain-0.0.4/genochain.egg-info/PKG-INFO` & `genochain-0.0.5/genochain.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genochain
-Version: 0.0.4
+Version: 0.0.5
 Summary: Storing and versioning genomics data on a blockchain
 Author: GenoChain(Sanjana Sharma)
 Author-email: <sharmasanjana1947@gmail.com>
 Keywords: python,blockchain,genomics,fasta,block,biology
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `genochain-0.0.4/setup.py` & `genochain-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Storing and versioning genomics data on a blockchain'
 LONG_DESCRIPTION = 'The provided code is a Python implementation of a simple blockchain. It allows for the creation of a genesis block with a given FASTA sequence, addition of new blocks with a given FASTA sequence and associated ID, and versioning of FASTA sequences. The blockchain can also be checked and printed. This code is licensed under the MIT License.'
 
 # Setting up
 setup(
     name="genochain",
     version=VERSION,
```

