# Comparing `tmp/garaprod-0.1683603566.0.tar.gz` & `tmp/garaprod-0.1683603820.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683603566.0.tar", last modified: Tue May  9 03:39:26 2023, max compression
+gzip compressed data, was "garaprod-0.1683603820.0.tar", last modified: Tue May  9 03:43:40 2023, max compression
```

## Comparing `garaprod-0.1683603566.0.tar` & `garaprod-0.1683603820.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:39:26.491639 garaprod-0.1683603566.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:39:26.491334 garaprod-0.1683603566.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:39:26.488023 garaprod-0.1683603566.0/garaprod/
--rw-r--r--   0 curlyz     (501) staff       (20)      915 2023-05-09 03:37:42.000000 garaprod-0.1683603566.0/garaprod/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683603566.0/garaprod/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod/version.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:39:26.490782 garaprod-0.1683603566.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       42 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 03:39:26.491765 garaprod-0.1683603566.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1119 2023-05-09 03:39:24.000000 garaprod-0.1683603566.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:43:40.340776 garaprod-0.1683603820.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:43:40.340435 garaprod-0.1683603820.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:43:40.333199 garaprod-0.1683603820.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)      578 2023-05-09 03:43:30.000000 garaprod-0.1683603820.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683603820.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:43:40.339760 garaprod-0.1683603820.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       36 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 03:43:40.000000 garaprod-0.1683603820.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 03:43:40.340923 garaprod-0.1683603820.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1106 2023-05-09 03:43:37.000000 garaprod-0.1683603820.0/setup.py
```

### Comparing `garaprod-0.1683603566.0/setup.py` & `garaprod-0.1683603820.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     author_email='curly.saigonese@gmail.com',
     keywords=['GaraSTEM', 'GRobot'],
     url='https://github.com/curlyz/garaprod',
     download_url='https://pypi.org/project/garaprod/'
 )
 
 install_requires = [
-    'bleak',
     'termcolor',
     'requests',
     'umsgpack',
     'esptool'
 ]
 
 print("find_packages()", find_packages())
```

