# Comparing `tmp/labnas-0.1.2.tar.gz` & `tmp/labnas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labnas-0.1.2.tar", max compression
+gzip compressed data, was "labnas-0.1.3.tar", max compression
```

## Comparing `labnas-0.1.2.tar` & `labnas-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       22 2023-03-17 12:34:50.451746 labnas-0.1.2/labnas/__init__.py
--rw-r--r--   0        0        0     5747 2023-03-21 17:28:52.494073 labnas-0.1.2/labnas/base.py
--rw-r--r--   0        0        0     2330 2023-03-21 17:27:30.674073 labnas-0.1.2/labnas/imaging.py
--rw-r--r--   0        0        0     3018 2023-03-21 17:27:30.674073 labnas-0.1.2/labnas/local.py
--rw-r--r--   0        0        0      379 2023-03-21 17:29:13.666073 labnas-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 labnas-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-02-23 15:12:09.060507 labnas-0.1.3/labnas/__init__.py
+-rw-r--r--   0        0        0     5747 2023-03-28 10:52:04.309993 labnas-0.1.3/labnas/connection.py
+-rw-r--r--   0        0        0     2334 2023-03-28 10:52:25.469761 labnas-0.1.3/labnas/imaging.py
+-rw-r--r--   0        0        0     3119 2023-05-09 11:43:37.154399 labnas-0.1.3/labnas/local.py
+-rw-r--r--   0        0        0      379 2023-05-09 11:36:32.685690 labnas-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 labnas-0.1.3/PKG-INFO
```

### Comparing `labnas-0.1.2/labnas/base.py` & `labnas-0.1.3/labnas/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 
 import pysftp
 from tqdm import tqdm
 
 from labnas.local import list_files_and_folders
 
-class SftpConnection:
+
+class NasConnection:
     """Basic SFTP connection (wrapper around pysftp)"""
 
     def __init__(self, host_name: str, user_name: str, pwd: str) -> None:
         self.connection: pysftp.Connection = pysftp.Connection(
             host=host_name,
             username=user_name,
             password=pwd,
```

### Comparing `labnas-0.1.2/labnas/imaging.py` & `labnas-0.1.3/labnas/imaging.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import os
 from pathlib import Path
 
 import pandas as pd
 from tqdm import tqdm
 
-from labnas.base import SftpConnection
+from labnas.connection import NasConnection
 from labnas.local import convert_tif_folder_into_file
 
 
-class ImagingConnection(SftpConnection):
+class ImagingConnection(NasConnection):
     def scan(self, remote_folder: Path) -> pd.DataFrame:
         rows = []
 
         files, subject_folders = self.list_files_and_folder(remote_folder)
         for subject_folder in subject_folders:
             sessions_folder = subject_folder / "sessions"
             if self.connection.isdir(str(sessions_folder)):
```

### Comparing `labnas-0.1.2/labnas/local.py` & `labnas-0.1.3/labnas/local.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,34 +27,37 @@
     tif_files = []
     for file in files:
         if file.suffix == ".tif":
             tif_files.append(file)
     return tif_files
 
 
-def convert_tif_folder_into_file(source_folder: Path, target_parent: Path) -> Path:
+def convert_tif_folder_into_file(source_folder: Path, output_file: Path | None = None) -> Path:
     """Convert a folder full of single frame tifs into a single multi-frame tif file."""
     if not source_folder.is_dir():
         raise FileNotFoundError(f"{source_folder} does not exist.")
-    if not target_parent.is_dir():
-        raise FileNotFoundError(f"{target_parent} does not exist.")
 
-    target_file = target_parent / f"{source_folder.name}.tif"
-    if target_file.is_file():
-        raise FileExistsError(f"{target_file} already exists.")
+    if output_file is None:
+        target_parent = source_folder.parent
+        output_file = target_parent / f"{source_folder.name}.tif"
+        print(f"No output file given - using {output_file}")
+    else:
+        assert output_file.suffix == ".tif"
+    if output_file.is_file():
+        raise FileExistsError(f"{output_file} already exists.")
 
     tifs = list_tifs(source_folder)
     print(f"{len(tifs)} found in {source_folder}.")
     sorted_tifs = sort_tifs(tifs)
     print(f"Loading {sorted_tifs.size} tifs.")
     movie = load_tifs(sorted_tifs)
     print(f"Tifs loaded into movie with shape {movie.shape}.")
-    print(f"Saving movie to {target_file}.")
-    write_movie_to_tif(movie, target_file)
-    return target_file
+    print(f"Saving movie to {output_file}.")
+    write_movie_to_tif(movie, output_file)
+    return output_file
 
 
 def list_tifs(local_folder: Path) -> list:
     """List all .tif files in a folder."""
     files, _ = list_files_and_folders(local_folder)
     tif_files = identify_tifs(files)
     return tif_files
```

