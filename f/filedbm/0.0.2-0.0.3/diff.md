# Comparing `tmp/filedbm-0.0.2.tar.gz` & `tmp/filedbm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filedbm-0.0.2.tar", last modified: Mon May  8 06:23:12 2023, max compression
+gzip compressed data, was "filedbm-0.0.3.tar", last modified: Mon May  8 22:14:59 2023, max compression
```

## Comparing `filedbm-0.0.2.tar` & `filedbm-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.078271 filedbm-0.0.2/
--rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.2/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 06:23:12.078271 filedbm-0.0.2/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.2/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.074271 filedbm-0.0.2/filedbm/
--rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.2/filedbm/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     6560 2023-05-08 05:09:06.000000 filedbm-0.0.2/filedbm/main.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.078271 filedbm-0.0.2/filedbm/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.2/filedbm/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     5043 2023-05-08 06:16:54.000000 filedbm-0.0.2/filedbm/utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 06:23:12.078271 filedbm-0.0.2/filedbm.egg-info/
--rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-08 06:23:12.000000 filedbm-0.0.2/filedbm.egg-info/top_level.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.2/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 06:23:12.078271 filedbm-0.0.2/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-08 06:23:05.000000 filedbm-0.0.2/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    11357 2023-05-08 01:46:02.000000 filedbm-0.0.3/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 22:14:59.440277 filedbm-0.0.3/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      152 2023-05-08 01:50:12.000000 filedbm-0.0.3/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/filedbm/
+-rw-rw-r--   0 mike      (1000) mike      (1000)       70 2023-05-08 05:12:10.000000 filedbm-0.0.3/filedbm/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7265 2023-05-08 22:09:12.000000 filedbm-0.0.3/filedbm/main.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/filedbm/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      208 2023-05-08 01:48:21.000000 filedbm-0.0.3/filedbm/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4963 2023-05-08 21:36:23.000000 filedbm-0.0.3/filedbm/utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-05-08 22:14:59.440277 filedbm-0.0.3/filedbm.egg-info/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      663 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)      255 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        8 2023-05-08 22:14:59.000000 filedbm-0.0.3/filedbm.egg-info/top_level.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      104 2023-05-08 01:48:21.000000 filedbm-0.0.3/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)       67 2023-05-08 22:14:59.440277 filedbm-0.0.3/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7116 2023-05-08 22:12:45.000000 filedbm-0.0.3/setup.py
```

### Comparing `filedbm-0.0.2/LICENSE` & `filedbm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `filedbm-0.0.2/PKG-INFO` & `filedbm-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.2/filedbm/main.py` & `filedbm-0.0.3/filedbm/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 """
 # import os
 import io
 import pathlib
 from collections.abc import Mapping, MutableMapping
-from typing import Any, Generic, Iterator, Union, Dict
+from typing import Any, Generic, Iterator, Union, Dict, List
 import shutil
 # from hashlib import blake2b
 
 # import utils
 from . import utils
 
 
@@ -19,15 +19,15 @@
 ### Classes
 
 
 class FileDBM(MutableMapping):
     """
 
     """
-    def __init__(self, db_path: str, flag: str = "r", n_bytes_key=2, n_bytes_value=4):
+    def __init__(self, db_path: str, flag: str = "r", buffer_size: int=512000, n_bytes_key=2, n_bytes_value=4):
         """
 
         """
         fp = pathlib.Path(db_path)
         fp_exists = fp.exists()
 
         if flag == "r":  # Open existing database for reading only (default)
@@ -45,35 +45,46 @@
             if fp_exists:
                 shutil.rmtree(fp, ignore_errors=True)
             fp_exists = False
         else:
             raise ValueError("Invalid flag")
 
         self._write = write
+        self._buffer_size = buffer_size
         self._n_bytes_key = n_bytes_key
         self._n_bytes_value = n_bytes_value
 
         ## Load or assign encodings and attributes
         if not fp_exists:
             fp.mkdir(parents=True)
 
         self.db_path = fp
 
 
     def keys(self):
         for key in utils.iter_keys_values(self.db_path, True, False, self._n_bytes_key, self._n_bytes_value):
             yield key
 
-    def items(self):
-        for key, value in utils.iter_keys_values(self.db_path, True, True, self._n_bytes_key, self._n_bytes_value):
-            yield key, value
-
-    def values(self):
-        for value in utils.iter_keys_values(self.db_path, False, True, self._n_bytes_key, self._n_bytes_value):
-            yield value
+    def items(self, keys: List[str]=None):
+        if keys is None:
+            for key, value in utils.iter_keys_values(self.db_path, True, True, self._n_bytes_key, self._n_bytes_value):
+                yield key, value
+        else:
+            for key in keys:
+                value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value)
+                yield key, value
+
+    def values(self, keys: List[str]=None):
+        if keys is None:
+            for value in utils.iter_keys_values(self.db_path, False, True, self._n_bytes_key, self._n_bytes_value):
+                yield value
+        else:
+            for key in keys:
+                value = utils.get_value(self.db_path, key.encode(), self._n_bytes_key, self._n_bytes_value)
+                yield value
 
     def __iter__(self):
         return self.keys()
 
     def __len__(self):
         return len([file for file in self.db_path.iterdir() if file.is_file()])
 
@@ -108,15 +119,15 @@
             raise KeyError(key)
         else:
             return value
 
 
     def __setitem__(self, key: str, value: Union[bytes, io.IOBase]):
         if self._write:
-            utils.write_data_block(self.db_path, key.encode(), value, self._n_bytes_key, self._n_bytes_value)
+            utils.write_data_block(self.db_path, key.encode(), value, self._n_bytes_key, self._n_bytes_value, self._buffer_size)
         else:
             raise ValueError('File is open for read only.')
 
     def __delitem__(self, key: str):
         if self._write:
             key_hash = utils.hash_key(key.encode())
             file_path = self.db_path.joinpath(key_hash.hex())
@@ -157,26 +168,29 @@
     #         self._mm.write(utils.int_to_bytes(self._n_keys, 4))
     #         self._mm.flush()
     #         self._file.flush()
 
 
 
 def open(
-    db_path: str, flag: str = "r", n_bytes_key=2, n_bytes_value=4):
+    db_path: str, flag: str = "r", buffer_size: int=512000, n_bytes_key=2, n_bytes_value=4):
     """
     Open a persistent dictionary for reading and writing. All keys and values are stored in individual files within the db_path. Keys must be strings and values must be either bytes or file-objects.
 
     Parameters
     -----------
     db_path : str or pathlib.Path
         It must be a path to a folder. If the folder doesn't exist, it will be created if flags 'c' or 'n' are passed.
 
     flag : str
         Flag associated with how the file is opened according to the dbm style. See below for details.
 
+    buffer_size : int
+        The buffer memory size used for reading and writing. Defaults to 512000.
+
     n_bytes_key : int
         The number of bytes to represent an integer of the max length of each key.
 
     n_bytes_value : int
         The number of bytes to represent an integer of the max length of each value.
 
     Returns
@@ -197,8 +211,8 @@
     | ``'c'`` | Open database for reading and writing,    |
     |         | creating it if it doesn't exist           |
     +---------+-------------------------------------------+
     | ``'n'`` | Always create a new, empty database, open |
     |         | for reading and writing                   |
     +---------+-------------------------------------------+
     """
-    return FileDBM(db_path, flag, n_bytes_key, n_bytes_value)
+    return FileDBM(db_path, flag, buffer_size, n_bytes_key, n_bytes_value)
```

### Comparing `filedbm-0.0.2/filedbm/utils.py` & `filedbm-0.0.3/filedbm/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from typing import Any, Generic, Iterator, Union
 import mmap
 
 ############################################
 ### Parameters
 
 key_hash_len = 13
-default_write_buffer_size = 512000
 
 
 ############################################
 ### Classes
 
 
 class FileObjectSlice(io.IOBase):
@@ -153,15 +152,15 @@
     for file_path in db_path.iterdir():
         file = io.open(file_path, 'rb')
         mm = mmap.mmap(file.fileno(), 0, access=mmap.ACCESS_READ)
 
         yield get_data_block(mm, key, value, n_bytes_key, n_bytes_value)
 
 
-def write_data_block(db_path, key, value, n_bytes_key, n_bytes_value):
+def write_data_block(db_path, key, value, n_bytes_key, n_bytes_value, buffer_size):
     """
 
     """
     key_bytes_len = len(key)
     key_hash = hash_key(key)
 
     if isinstance(value, bytes):
@@ -174,16 +173,14 @@
     file_path = db_path.joinpath(key_hash.hex())
 
     file = io.open(file_path, 'w+b')
     _ = file.write(write_init_bytes)
 
     if hasattr(value, '_buffer_size'):
         buffer_size = value._buffer_size
-    else:
-        buffer_size = default_write_buffer_size
 
     chunk = value.read(buffer_size)
     while chunk:
         file.write(chunk)
         chunk = value.read(buffer_size)
 
     file.close()
```

### Comparing `filedbm-0.0.2/filedbm.egg-info/PKG-INFO` & `filedbm-0.0.3/filedbm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filedbm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A persistent key-value database
 Home-page: https://github.com/mullenkamp/filedbm
 Author: Mike Kittridge
 Author-email: mullenkamp1@gmail.com
 License: Apache
 Keywords: shelve dbm
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `filedbm-0.0.2/setup.py` & `filedbm-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # General parameters
 name = 'filedbm'
 main_package = 'filedbm'
-version = '0.0.2'
+version = '0.0.3'
 descrip = 'A persistent key-value database'
 
 # The below code is for readthedocs. To have sphinx/readthedocs interact with
 # the contained package, readthedocs needs to build the package. But the dependencies
 # should be installed via the conda yml env file rather than during the package build.
 if os.environ.get('READTHEDOCS', False) == 'True':
     INSTALL_REQUIRES = []
```

