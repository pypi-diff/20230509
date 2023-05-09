# Comparing `tmp/s3autocp-0.0.3.tar.gz` & `tmp/s3autocp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3autocp-0.0.3.tar", last modified: Tue May  9 12:52:08 2023, max compression
+gzip compressed data, was "s3autocp-0.0.4.tar", last modified: Tue May  9 14:12:45 2023, max compression
```

## Comparing `s3autocp-0.0.3.tar` & `s3autocp-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 12:52:08.404298 s3autocp-0.0.3/
--rw-r--r--   0 jouni     (1000) jouni     (1000)    11357 2023-05-09 11:22:16.000000 s3autocp-0.0.3/LICENSE
--rw-r--r--   0 jouni     (1000) jouni     (1000)      521 2023-05-09 12:52:08.403298 s3autocp-0.0.3/PKG-INFO
--rw-r--r--   0 jouni     (1000) jouni     (1000)       10 2023-05-09 11:22:16.000000 s3autocp-0.0.3/README.md
--rw-r--r--   0 jouni     (1000) jouni     (1000)      621 2023-05-09 12:51:39.000000 s3autocp-0.0.3/pyproject.toml
--rw-r--r--   0 jouni     (1000) jouni     (1000)       38 2023-05-09 12:52:08.404298 s3autocp-0.0.3/setup.cfg
--rw-r--r--   0 jouni     (1000) jouni     (1000)      131 2023-05-09 12:07:20.000000 s3autocp-0.0.3/setup.py
-drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 12:52:08.399298 s3autocp-0.0.3/src/
-drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 12:52:08.401298 s3autocp-0.0.3/src/s3autocp/
--rw-r--r--   0 jouni     (1000) jouni     (1000)       68 2023-05-09 12:08:21.000000 s3autocp-0.0.3/src/s3autocp/__init__.py
--rw-r--r--   0 jouni     (1000) jouni     (1000)     6238 2023-05-09 12:50:01.000000 s3autocp-0.0.3/src/s3autocp/s3autocp.py
-drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 12:52:08.403298 s3autocp-0.0.3/src/s3autocp.egg-info/
--rw-r--r--   0 jouni     (1000) jouni     (1000)      521 2023-05-09 12:52:08.000000 s3autocp-0.0.3/src/s3autocp.egg-info/PKG-INFO
--rw-r--r--   0 jouni     (1000) jouni     (1000)      309 2023-05-09 12:52:08.000000 s3autocp-0.0.3/src/s3autocp.egg-info/SOURCES.txt
--rw-r--r--   0 jouni     (1000) jouni     (1000)        1 2023-05-09 12:52:08.000000 s3autocp-0.0.3/src/s3autocp.egg-info/dependency_links.txt
--rw-r--r--   0 jouni     (1000) jouni     (1000)       43 2023-05-09 12:52:08.000000 s3autocp-0.0.3/src/s3autocp.egg-info/entry_points.txt
--rw-r--r--   0 jouni     (1000) jouni     (1000)        6 2023-05-09 12:52:08.000000 s3autocp-0.0.3/src/s3autocp.egg-info/requires.txt
--rw-r--r--   0 jouni     (1000) jouni     (1000)        9 2023-05-09 12:52:08.000000 s3autocp-0.0.3/src/s3autocp.egg-info/top_level.txt
+drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 14:12:45.273945 s3autocp-0.0.4/
+-rw-r--r--   0 jouni     (1000) jouni     (1000)    11357 2023-05-09 11:22:16.000000 s3autocp-0.0.4/LICENSE
+-rw-r--r--   0 jouni     (1000) jouni     (1000)      521 2023-05-09 14:12:45.272945 s3autocp-0.0.4/PKG-INFO
+-rw-r--r--   0 jouni     (1000) jouni     (1000)       10 2023-05-09 11:22:16.000000 s3autocp-0.0.4/README.md
+-rw-r--r--   0 jouni     (1000) jouni     (1000)      621 2023-05-09 14:11:54.000000 s3autocp-0.0.4/pyproject.toml
+-rw-r--r--   0 jouni     (1000) jouni     (1000)       38 2023-05-09 14:12:45.273945 s3autocp-0.0.4/setup.cfg
+-rw-r--r--   0 jouni     (1000) jouni     (1000)      131 2023-05-09 12:07:20.000000 s3autocp-0.0.4/setup.py
+drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 14:12:45.270945 s3autocp-0.0.4/src/
+drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 14:12:45.271945 s3autocp-0.0.4/src/s3autocp/
+-rw-r--r--   0 jouni     (1000) jouni     (1000)       68 2023-05-09 12:08:21.000000 s3autocp-0.0.4/src/s3autocp/__init__.py
+-rw-r--r--   0 jouni     (1000) jouni     (1000)     6069 2023-05-09 14:12:21.000000 s3autocp-0.0.4/src/s3autocp/s3autocp.py
+drwxr-xr-x   0 jouni     (1000) jouni     (1000)        0 2023-05-09 14:12:45.272945 s3autocp-0.0.4/src/s3autocp.egg-info/
+-rw-r--r--   0 jouni     (1000) jouni     (1000)      521 2023-05-09 14:12:45.000000 s3autocp-0.0.4/src/s3autocp.egg-info/PKG-INFO
+-rw-r--r--   0 jouni     (1000) jouni     (1000)      309 2023-05-09 14:12:45.000000 s3autocp-0.0.4/src/s3autocp.egg-info/SOURCES.txt
+-rw-r--r--   0 jouni     (1000) jouni     (1000)        1 2023-05-09 14:12:45.000000 s3autocp-0.0.4/src/s3autocp.egg-info/dependency_links.txt
+-rw-r--r--   0 jouni     (1000) jouni     (1000)       43 2023-05-09 14:12:45.000000 s3autocp-0.0.4/src/s3autocp.egg-info/entry_points.txt
+-rw-r--r--   0 jouni     (1000) jouni     (1000)        6 2023-05-09 14:12:45.000000 s3autocp-0.0.4/src/s3autocp.egg-info/requires.txt
+-rw-r--r--   0 jouni     (1000) jouni     (1000)        9 2023-05-09 14:12:45.000000 s3autocp-0.0.4/src/s3autocp.egg-info/top_level.txt
```

### Comparing `s3autocp-0.0.3/LICENSE` & `s3autocp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `s3autocp-0.0.3/PKG-INFO` & `s3autocp-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3autocp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool for copying build folders to S3 with guessed Content-Type and Cache-Control
 Author-email: Jouni Tenhunen <jouni.tenhunen@nitor.com>
 Project-URL: Homepage, https://github.com/NitorCreations/s3autocp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `s3autocp-0.0.3/pyproject.toml` & `s3autocp-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "s3autocp"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jouni Tenhunen", email="jouni.tenhunen@nitor.com" },
 ]
 description = "A tool for copying build folders to S3 with guessed Content-Type and Cache-Control"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `s3autocp-0.0.3/src/s3autocp/s3autocp.py` & `s3autocp-0.0.4/src/s3autocp/s3autocp.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,21 +113,15 @@
         "destination",
         metavar="destination",
         type=str,
         nargs=1,
         help="destination s3 url",
     )
     args = parser.parse_args()
-    source = args.source[0]
-    destination = args.destination[0]
-    if source.endswith("/"):
-        source = source[:-1]
-    if destination.endswith("/"):
-        destination = destination[:-1]
-    return source, destination
+    return args.source[0], args.destination[0]
 
 
 def _get_filenames(source_dir: str) -> Iterator[str]:
     if source_dir[-1] != "/":
         source_dir += "/"
     path = source_dir + "/**/*"
     return (f for f in iglob(path, recursive=True) if not os.path.isdir(f))
@@ -135,17 +129,17 @@
 
 def _filename_contains_hash(filename: str) -> bool:
     return bool(HASH_IN_FILENAME_REGEX.match(filename))
 
 
 def _get_cache_control(filename: str) -> str:
     if _filename_contains_hash(filename=filename):
-        return "infinite"
+        return "max-age=31536000, immutable"
     else:
-        return "must-revalidate"
+        return "no-cache"
 
 
 def _get_bucket_name_and_path(destination: str, source: str) -> Tuple[str, str]:
     if destination.startswith("s3://"):
         destination = destination[5:]
     parts = destination.split("/")
     bucket_name = parts[0]
```

### Comparing `s3autocp-0.0.3/src/s3autocp.egg-info/PKG-INFO` & `s3autocp-0.0.4/src/s3autocp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3autocp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool for copying build folders to S3 with guessed Content-Type and Cache-Control
 Author-email: Jouni Tenhunen <jouni.tenhunen@nitor.com>
 Project-URL: Homepage, https://github.com/NitorCreations/s3autocp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

