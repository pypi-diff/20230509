# Comparing `tmp/wsiserver-1.0.3.tar.gz` & `tmp/wsiserver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsiserver-1.0.3.tar", last modified: Mon May  1 00:44:59 2023, max compression
+gzip compressed data, was "wsiserver-1.0.4.tar", last modified: Tue May  9 02:43:42 2023, max compression
```

## Comparing `wsiserver-1.0.3.tar` & `wsiserver-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.181815 wsiserver-1.0.3/
--rw-r--r--   0 takumi     (501) staff       (20)    11357 2023-04-19 13:54:50.000000 wsiserver-1.0.3/LICENSE
--rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-05-01 00:44:59.180962 wsiserver-1.0.3/PKG-INFO
--rw-r--r--   0 takumi     (501) staff       (20)      326 2023-04-22 01:08:13.000000 wsiserver-1.0.3/README.md
--rw-r--r--   0 takumi     (501) staff       (20)      677 2023-04-22 01:03:50.000000 wsiserver-1.0.3/pyproject.toml
--rw-r--r--   0 takumi     (501) staff       (20)       38 2023-05-01 00:44:59.181905 wsiserver-1.0.3/setup.cfg
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.176277 wsiserver-1.0.3/src/
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.178164 wsiserver-1.0.3/src/wsiserver/
--rw-r--r--   0 takumi     (501) staff       (20)       22 2023-05-01 00:44:29.000000 wsiserver-1.0.3/src/wsiserver/__init__.py
--rw-r--r--   0 takumi     (501) staff       (20)     2498 2023-05-01 00:43:06.000000 wsiserver-1.0.3/src/wsiserver/app.py
-drwxr-xr-x   0 takumi     (501) staff       (20)        0 2023-05-01 00:44:59.180490 wsiserver-1.0.3/src/wsiserver.egg-info/
--rw-r--r--   0 takumi     (501) staff       (20)    13576 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/PKG-INFO
--rw-r--r--   0 takumi     (501) staff       (20)      303 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/SOURCES.txt
--rw-r--r--   0 takumi     (501) staff       (20)        1 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/dependency_links.txt
--rw-r--r--   0 takumi     (501) staff       (20)       49 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/entry_points.txt
--rw-r--r--   0 takumi     (501) staff       (20)       40 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/requires.txt
--rw-r--r--   0 takumi     (501) staff       (20)       10 2023-05-01 00:44:59.000000 wsiserver-1.0.3/src/wsiserver.egg-info/top_level.txt
+drwxrwxr-x   0 ngpin     (1000) ngpin     (1000)        0 2023-05-09 02:43:42.666563 wsiserver-1.0.4/
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)    11357 2023-05-09 02:40:54.000000 wsiserver-1.0.4/LICENSE
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)    13576 2023-05-09 02:43:42.666563 wsiserver-1.0.4/PKG-INFO
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)      326 2023-05-09 02:40:54.000000 wsiserver-1.0.4/README.md
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)      677 2023-05-09 02:40:54.000000 wsiserver-1.0.4/pyproject.toml
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)       38 2023-05-09 02:43:42.666563 wsiserver-1.0.4/setup.cfg
+drwxrwxr-x   0 ngpin     (1000) ngpin     (1000)        0 2023-05-09 02:43:42.666563 wsiserver-1.0.4/src/
+drwxrwxr-x   0 ngpin     (1000) ngpin     (1000)        0 2023-05-09 02:43:42.666563 wsiserver-1.0.4/src/wsiserver/
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)       22 2023-05-09 02:41:54.000000 wsiserver-1.0.4/src/wsiserver/__init__.py
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)     2498 2023-05-09 02:40:54.000000 wsiserver-1.0.4/src/wsiserver/app.py
+drwxrwxr-x   0 ngpin     (1000) ngpin     (1000)        0 2023-05-09 02:43:42.666563 wsiserver-1.0.4/src/wsiserver.egg-info/
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)    13576 2023-05-09 02:43:42.000000 wsiserver-1.0.4/src/wsiserver.egg-info/PKG-INFO
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)      303 2023-05-09 02:43:42.000000 wsiserver-1.0.4/src/wsiserver.egg-info/SOURCES.txt
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)        1 2023-05-09 02:43:42.000000 wsiserver-1.0.4/src/wsiserver.egg-info/dependency_links.txt
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)       49 2023-05-09 02:43:42.000000 wsiserver-1.0.4/src/wsiserver.egg-info/entry_points.txt
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)       40 2023-05-09 02:43:42.000000 wsiserver-1.0.4/src/wsiserver.egg-info/requires.txt
+-rw-rw-r--   0 ngpin     (1000) ngpin     (1000)       10 2023-05-09 02:43:42.000000 wsiserver-1.0.4/src/wsiserver.egg-info/top_level.txt
```

### Comparing `wsiserver-1.0.3/LICENSE` & `wsiserver-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wsiserver-1.0.3/PKG-INFO` & `wsiserver-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsiserver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Very simple wsi server
 Author-email: Takumi Ando <takumi.ando826@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `wsiserver-1.0.3/pyproject.toml` & `wsiserver-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wsiserver-1.0.3/src/wsiserver/app.py` & `wsiserver-1.0.4/src/wsiserver/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument("wsi", type=str, help="path to the WSI to load")
 parser.add_argument("--host", type=str, default="0.0.0.0", help="host to listen on")
 parser.add_argument("--port", type=int, default=31791, help="port to listen on")
 parser.add_argument("--tile_size", type=int, default=256, help="tile size")
-parser.add_argument("--version", "-v", action="version" ,versino=wsiserver.__version__)
+parser.add_argument("--version", "-v", action="version", version=wsiserver.__version__)
 args = parser.parse_args()
 
 app = FastAPI()
 app.add_middleware(
     CORSMiddleware,
     allow_origins=["*"],
     allow_credentials=True,
```

### Comparing `wsiserver-1.0.3/src/wsiserver.egg-info/PKG-INFO` & `wsiserver-1.0.4/src/wsiserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsiserver
-Version: 1.0.3
+Version: 1.0.4
 Summary: Very simple wsi server
 Author-email: Takumi Ando <takumi.ando826@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

