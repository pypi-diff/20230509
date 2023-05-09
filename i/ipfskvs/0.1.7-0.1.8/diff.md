# Comparing `tmp/ipfskvs-0.1.7.tar.gz` & `tmp/ipfskvs-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfskvs-0.1.7.tar", max compression
+gzip compressed data, was "ipfskvs-0.1.8.tar", max compression
```

## Comparing `ipfskvs-0.1.7.tar` & `ipfskvs-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.7/LICENSE
--rw-r--r--   0        0        0     2051 2023-05-09 00:58:37.701559 ipfskvs-0.1.7/README.md
--rw-r--r--   0        0        0      114 2023-05-09 01:22:58.534774 ipfskvs-0.1.7/ipfskvs/__init__.py
--rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.7/ipfskvs/index.py
--rw-r--r--   0        0        0     9624 2023-05-09 01:22:43.997617 ipfskvs-0.1.7/ipfskvs/store.py
--rw-r--r--   0        0        0      434 2023-05-09 01:22:55.441124 ipfskvs-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 ipfskvs-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-12 01:55:42.945987 ipfskvs-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2051 2023-05-09 00:58:37.701559 ipfskvs-0.1.8/README.md
+-rw-r--r--   0        0        0      114 2023-05-09 01:51:08.829795 ipfskvs-0.1.8/ipfskvs/__init__.py
+-rw-r--r--   0        0        0     6386 2023-04-21 01:22:01.481387 ipfskvs-0.1.8/ipfskvs/index.py
+-rw-r--r--   0        0        0     9449 2023-05-09 01:50:06.841147 ipfskvs-0.1.8/ipfskvs/store.py
+-rw-r--r--   0        0        0      434 2023-05-09 01:51:12.427091 ipfskvs-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 ipfskvs-0.1.8/PKG-INFO
```

### Comparing `ipfskvs-0.1.7/LICENSE` & `ipfskvs-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.7/README.md` & `ipfskvs-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.7/ipfskvs/index.py` & `ipfskvs-0.1.8/ipfskvs/index.py`

 * *Files identical despite different names*

### Comparing `ipfskvs-0.1.7/ipfskvs/store.py` & `ipfskvs-0.1.8/ipfskvs/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,14 +147,15 @@
             raise FileNotFoundError(
                 errno.ENOENT,
                 os.strerror(errno.ENOENT),
                 filename
             )
 
         LOG.debug(result)
+        self.reader = type(self.reader)()
         self.reader.ParseFromString(result)
 
     def write(self: Self) -> None:
         """Write the protobuf data from `self.writer` to IPFS."""
         raise NotImplementedError("For now, just use `add` and `delete`")
         self.ipfs.write(
             self.index.get_filename(),
@@ -202,19 +203,15 @@
             metadata = store.index.get_metadata()
             LOG.debug(f"Found metadata: {metadata}")
             for key in metadata:
                 if key not in pandas_input:
                     LOG.debug(f"Found key: {key}")
                     pandas_input[key] = []
 
-                # Check if the metadata is a list and extend pandas_input[key]
-                if isinstance(metadata[key], list):
-                    pandas_input[key].extend(metadata[key])
-                else:
-                    pandas_input[key].append(metadata[key])
+                pandas_input[key].append(metadata[key])
 
             # add top level data from the reader
             for key in protobuf_parsers:
                 if key not in pandas_input:
                     pandas_input[key] = []
 
                 parsed_data = protobuf_parsers[key](store)
```

### Comparing `ipfskvs-0.1.7/PKG-INFO` & `ipfskvs-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfskvs
-Version: 0.1.7
+Version: 0.1.8
 Summary: IPFS Key Value Store
 Author: Nate Schultz
 Author-email: nate.schultz@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipfsclient (>=0.0.7,<0.0.8)
```

