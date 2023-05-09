# Comparing `tmp/garatool-0.1683651958.0.tar.gz` & `tmp/garatool-0.1683652121.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683651958.0.tar", last modified: Tue May  9 17:05:58 2023, max compression
+gzip compressed data, was "garatool-0.1683652121.0.tar", last modified: Tue May  9 17:08:41 2023, max compression
```

## Comparing `garatool-0.1683651958.0.tar` & `garatool-0.1683652121.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:05:58.436349 garatool-0.1683651958.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:05:58.430236 garatool-0.1683651958.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683651958.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:05:58.420718 garatool-0.1683651958.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5732 2023-05-09 17:05:56.000000 garatool-0.1683651958.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683651958.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:05:58.429384 garatool-0.1683651958.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:05:58.000000 garatool-0.1683651958.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:05:58.000000 garatool-0.1683651958.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:05:58.000000 garatool-0.1683651958.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:05:58.000000 garatool-0.1683651958.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:05:58.000000 garatool-0.1683651958.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:05:58.436486 garatool-0.1683651958.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683651958.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:08:41.294398 garatool-0.1683652121.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:08:41.293968 garatool-0.1683652121.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683652121.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:08:41.290611 garatool-0.1683652121.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5732 2023-05-09 17:08:38.000000 garatool-0.1683652121.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683652121.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:08:41.293322 garatool-0.1683652121.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:08:41.000000 garatool-0.1683652121.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:08:41.000000 garatool-0.1683652121.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:08:41.000000 garatool-0.1683652121.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:08:41.000000 garatool-0.1683652121.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:08:41.000000 garatool-0.1683652121.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:08:41.294522 garatool-0.1683652121.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683652121.0/setup.py
```

### Comparing `garatool-0.1683651958.0/garatool/__init__.py` & `garatool-0.1683652121.0/garatool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         print(parti['file'], parti['offset'], len(parti['data']))
         with open(parti['file'], 'wb') as f:
             f.write(parti['data'])
 
 
 
     partition_params = ' '.join([
-        f"{p['offset']} \'{p['file']}\'" for p in br.partitions
+        f'{p["offset"]} \"{p["file"]}\"' for p in br.partitions
     ])
 
     os.system(cmd(' '.join([
         ESPTOOL,
         '-p', parsed.port,
         '-b', '460800',
         '--no-stub' if br.nostub else ' '
```

### Comparing `garatool-0.1683651958.0/setup.py` & `garatool-0.1683652121.0/setup.py`

 * *Files identical despite different names*

