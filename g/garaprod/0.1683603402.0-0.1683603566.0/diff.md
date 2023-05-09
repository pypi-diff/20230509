# Comparing `tmp/garaprod-0.1683603402.0.tar.gz` & `tmp/garaprod-0.1683603566.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garaprod-0.1683603402.0.tar", last modified: Tue May  9 03:36:42 2023, max compression
+gzip compressed data, was "garaprod-0.1683603566.0.tar", last modified: Tue May  9 03:39:26 2023, max compression
```

## Comparing `garaprod-0.1683603402.0.tar` & `garaprod-0.1683603566.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:36:42.729286 garaprod-0.1683603402.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:36:42.728891 garaprod-0.1683603402.0/PKG-INFO
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:36:42.726149 garaprod-0.1683603402.0/garaprod.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:36:42.000000 garaprod-0.1683603402.0/garaprod.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      254 2023-05-09 03:36:42.000000 garaprod-0.1683603402.0/garaprod.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 03:36:42.000000 garaprod-0.1683603402.0/garaprod.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       42 2023-05-09 03:36:42.000000 garaprod-0.1683603402.0/garaprod.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 03:36:42.000000 garaprod-0.1683603402.0/garaprod.egg-info/top_level.txt
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:36:42.728383 garaprod-0.1683603402.0/garastem/
--rw-r--r--   0 curlyz     (501) staff       (20)     8864 2023-05-09 03:35:00.000000 garaprod-0.1683603402.0/garastem/__init__ copy.py
--rw-r--r--   0 curlyz     (501) staff       (20)     9600 2023-05-09 03:35:00.000000 garaprod-0.1683603402.0/garastem/__init__.py
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683603402.0/garastem/modules.py
--rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 03:36:42.000000 garaprod-0.1683603402.0/garastem/version.py
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 03:36:42.729421 garaprod-0.1683603402.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1119 2023-05-09 03:36:29.000000 garaprod-0.1683603402.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:39:26.491639 garaprod-0.1683603566.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:39:26.491334 garaprod-0.1683603566.0/PKG-INFO
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:39:26.488023 garaprod-0.1683603566.0/garaprod/
+-rw-r--r--   0 curlyz     (501) staff       (20)      915 2023-05-09 03:37:42.000000 garaprod-0.1683603566.0/garaprod/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 03:35:00.000000 garaprod-0.1683603566.0/garaprod/modules.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       26 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod/version.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 03:39:26.490782 garaprod-0.1683603566.0/garaprod.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      293 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      228 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       42 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 03:39:26.000000 garaprod-0.1683603566.0/garaprod.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 03:39:26.491765 garaprod-0.1683603566.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1119 2023-05-09 03:39:24.000000 garaprod-0.1683603566.0/setup.py
```

### Comparing `garaprod-0.1683603402.0/setup.py` & `garaprod-0.1683603566.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 import time
-with open('garastem/README.md') as readme_file:
+with open('garaprod/README.md') as readme_file:
     README = readme_file.read()
 
-with open('garastem/HISTORY.md') as history_file:
+with open('garaprod/HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 version_string = '0.{}.0'.format(int(time.time()))
-with open('garastem/version.py', 'w') as f:
+with open('garaprod/version.py', 'w') as f:
     f.write(f'version = "{version_string}"')
 
 import time
 setup_args = dict(
     name='garaprod',
     version=version_string,
     description='GaraSTEM Production Library',
     # long_description_content_type="text/markdown",
     # long_description=README + '\n\n' + HISTORY,
     license='MIT',
-    packages=['garastem'],
+    packages=['garaprod'],
     author='Curly Nguyen',
     author_email='curly.saigonese@gmail.com',
     keywords=['GaraSTEM', 'GRobot'],
-    url='https://github.com/curlyz/garastem',
-    download_url='https://pypi.org/project/garastem/'
+    url='https://github.com/curlyz/garaprod',
+    download_url='https://pypi.org/project/garaprod/'
 )
 
 install_requires = [
     'bleak',
     'termcolor',
     'requests',
     'umsgpack',
```

