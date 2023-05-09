# Comparing `tmp/ipfskvs-0.1.6.tar.gz` & `tmp/ipfskvs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.1.6.tar", max compression
+gzip compressed data, was "ipfskvs-0.1.7.tar", max compression
```

## Comparing `ipfskvs-0.1.6.tar` & `ipfskvs-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.6/LICENSE
--rw-r--r--   0        0        0     2051 2023-05-09 00:58:37.701559 ipfskvs-0.1.6/README.md
--rw-r--r--   0        0        0      114 2023-05-09 01:00:10.495777 ipfskvs-0.1.6/ipfskvs/__init__.py
--rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.6/ipfskvs/index.py
--rw-r--r--   0        0        0     9407 2023-05-09 00:56:41.654228 ipfskvs-0.1.6/ipfskvs/store.py
--rw-r--r--   0        0        0      434 2023-05-09 01:00:06.730083 ipfskvs-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 ipfskvs-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2051 2023-05-09 00:58:37.701559 ipfskvs-0.1.7/README.md
+-rw-r--r--   0        0        0      114 2023-05-09 01:22:58.534774 ipfskvs-0.1.7/ipfskvs/__init__.py
+-rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.7/ipfskvs/index.py
+-rw-r--r--   0        0        0     9624 2023-05-09 01:22:43.997617 ipfskvs-0.1.7/ipfskvs/store.py
+-rw-r--r--   0        0        0      434 2023-05-09 01:22:55.441124 ipfskvs-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 ipfskvs-0.1.7/PKG-INFO
```

### Comparing `ipfskvs-0.1.6/LICENSE` & `ipfskvs-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.6/README.md` & `ipfskvs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.6/ipfskvs/index.py` & `ipfskvs-0.1.7/ipfskvs/index.py`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.6/ipfskvs/store.py` & `ipfskvs-0.1.7/ipfskvs/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -202,15 +202,19 @@
             metadata = store.index.get_metadata()
             LOG.debug(f"Found metadata: {metadata}")
             for key in metadata:
                 if key not in pandas_input:
                     LOG.debug(f"Found key: {key}")
                     pandas_input[key] = []
 
-                pandas_input[key].append(metadata[key])
+                # Check if the metadata is a list and extend pandas_input[key]
+                if isinstance(metadata[key], list):
+                    pandas_input[key].extend(metadata[key])
+                else:
+                    pandas_input[key].append(metadata[key])
 
             # add top level data from the reader
             for key in protobuf_parsers:
                 if key not in pandas_input:
                     pandas_input[key] = []
 
                 parsed_data = protobuf_parsers[key](store)
```

### Comparing `ipfskvs-0.1.6/PKG-INFO` & `ipfskvs-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.1.6
+Version: 0.1.7
 Summary: IPFS Key Value Store
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (>=0.0.7,<0.0.8)
```

