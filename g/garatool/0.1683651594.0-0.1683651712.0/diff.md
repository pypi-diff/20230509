# Comparing `tmp/garatool-0.1683651594.0.tar.gz` & `tmp/garatool-0.1683651712.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683651594.0.tar", last modified: Tue May  9 16:59:54 2023, max compression
+gzip compressed data, was "garatool-0.1683651712.0.tar", last modified: Tue May  9 17:01:52 2023, max compression
```

## Comparing `garatool-0.1683651594.0.tar` & `garatool-0.1683651712.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:59:54.235278 garatool-0.1683651594.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:59:54.234971 garatool-0.1683651594.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683651594.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:59:54.231702 garatool-0.1683651594.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5725 2023-05-09 16:59:17.000000 garatool-0.1683651594.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683651594.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:59:54.234471 garatool-0.1683651594.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:59:54.000000 garatool-0.1683651594.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 16:59:54.000000 garatool-0.1683651594.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:59:54.000000 garatool-0.1683651594.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:59:54.000000 garatool-0.1683651594.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:59:54.000000 garatool-0.1683651594.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:59:54.235367 garatool-0.1683651594.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683651594.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:01:52.653772 garatool-0.1683651712.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:01:52.653328 garatool-0.1683651712.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683651712.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:01:52.650684 garatool-0.1683651712.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5728 2023-05-09 17:01:50.000000 garatool-0.1683651712.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683651712.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:01:52.652781 garatool-0.1683651712.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:01:52.000000 garatool-0.1683651712.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:01:52.000000 garatool-0.1683651712.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:01:52.000000 garatool-0.1683651712.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:01:52.000000 garatool-0.1683651712.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:01:52.000000 garatool-0.1683651712.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:01:52.653913 garatool-0.1683651712.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683651712.0/setup.py
```

### Comparing `garatool-0.1683651594.0/garatool/__init__.py` & `garatool-0.1683651712.0/garatool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 
 
 def program_device(br: BuildRequest):
     # for parti in br.partitions:
     for i in range(len(br.partitions)):
         parti = br.partitions[i]
-        parti['file'] = tempfile.mkstemp()
+        parti['file'] = tempfile.mkstemp()[1]
         print(parti['file'], parti['offset'], len(parti['data']))
         with open(parti['file'], 'wb') as f:
             f.write(parti['data'])
 
 
 
     partition_params = ' '.join([
```

### Comparing `garatool-0.1683651594.0/setup.py` & `garatool-0.1683651712.0/setup.py`

 * *Files identical despite different names*

