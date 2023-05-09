# Comparing `tmp/garatool-0.1683653555.0.tar.gz` & `tmp/garatool-0.1683653830.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683653555.0.tar", last modified: Tue May  9 17:32:36 2023, max compression
+gzip compressed data, was "garatool-0.1683653830.0.tar", last modified: Tue May  9 17:37:10 2023, max compression
```

## Comparing `garatool-0.1683653555.0.tar` & `garatool-0.1683653830.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:32:36.062021 garatool-0.1683653555.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:32:36.061648 garatool-0.1683653555.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683653555.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:32:36.058179 garatool-0.1683653555.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5747 2023-05-09 17:32:09.000000 garatool-0.1683653555.0/garatool/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683653555.0/garatool/__main__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:32:36.061042 garatool-0.1683653555.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:32:36.000000 garatool-0.1683653555.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:32:36.062162 garatool-0.1683653555.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683653555.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:37:10.878089 garatool-0.1683653830.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:37:10.877781 garatool-0.1683653830.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683653830.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:37:10.875215 garatool-0.1683653830.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5749 2023-05-09 17:37:09.000000 garatool-0.1683653830.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683653830.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 17:37:10.877380 garatool-0.1683653830.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 17:37:10.000000 garatool-0.1683653830.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 17:37:10.000000 garatool-0.1683653830.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 17:37:10.000000 garatool-0.1683653830.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 17:37:10.000000 garatool-0.1683653830.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 17:37:10.000000 garatool-0.1683653830.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 17:37:10.878179 garatool-0.1683653830.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683653830.0/setup.py
```

### Comparing `garatool-0.1683653555.0/garatool/__init__.py` & `garatool-0.1683653830.0/garatool/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 
 
 def program_device(br: BuildRequest):
     # for parti in br.partitions:
     for i in range(len(br.partitions)):
         parti = br.partitions[i]
-        parti['file'] = tempfile.mkstemp()[1]
+        # parti['file'] = tempfile.mkstemp()[1]
         print(parti['file'], parti['offset'], len(parti['data']))
         with open(parti['file'], 'wb') as f:
             f.write(parti['data'])
 
 
 
     partition_params = ' '.join([
```

### Comparing `garatool-0.1683653555.0/setup.py` & `garatool-0.1683653830.0/setup.py`

 * *Files identical despite different names*

