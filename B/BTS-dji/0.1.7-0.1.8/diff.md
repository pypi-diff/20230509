# Comparing `tmp/BTS_dji-0.1.7.tar.gz` & `tmp/BTS_dji-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/BTS-dji/BTS-dji/dist/.tmp-b_esxidg/BTS_dji-0.1.7.tar", last modified: Tue May  9 04:21:16 2023, max compression
+gzip compressed data, was "/home/runner/work/BTS-dji/BTS-dji/dist/.tmp-4ulv5p8n/BTS_dji-0.1.8.tar", last modified: Tue May  9 05:53:52 2023, max compression
```

## Comparing `BTS_dji-0.1.7.tar` & `BTS_dji-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/BTS_dji/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-09 04:21:05.000000 BTS_dji-0.1.7/BTS_dji/Robomaster.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:21:05.000000 BTS_dji-0.1.7/BTS_dji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-05-09 04:21:05.000000 BTS_dji-0.1.7/BTS_dji/controler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-09 04:21:05.000000 BTS_dji-0.1.7/BTS_dji/kbd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/BTS_dji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/BTS_dji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/BTS_dji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/BTS_dji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/BTS_dji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/BTS_dji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 04:21:05.000000 BTS_dji-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 04:21:16.000000 BTS_dji-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 04:21:05.000000 BTS_dji-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/BTS_dji/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-09 05:53:38.000000 BTS_dji-0.1.8/BTS_dji/Robomaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 05:53:38.000000 BTS_dji-0.1.8/BTS_dji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-05-09 05:53:38.000000 BTS_dji-0.1.8/BTS_dji/controler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-09 05:53:38.000000 BTS_dji-0.1.8/BTS_dji/kbd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/BTS_dji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/BTS_dji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/BTS_dji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/BTS_dji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/BTS_dji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/BTS_dji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-09 05:53:38.000000 BTS_dji-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:53:52.000000 BTS_dji-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-09 05:53:38.000000 BTS_dji-0.1.8/setup.py
```

### Comparing `BTS_dji-0.1.7/BTS_dji/Robomaster.py` & `BTS_dji-0.1.8/BTS_dji/Robomaster.py`

 * *Files identical despite different names*

### Comparing `BTS_dji-0.1.7/BTS_dji/controler.py` & `BTS_dji-0.1.8/BTS_dji/controler.py`

 * *Files identical despite different names*

### Comparing `BTS_dji-0.1.7/BTS_dji/kbd.py` & `BTS_dji-0.1.8/BTS_dji/kbd.py`

 * *Files identical despite different names*

### Comparing `BTS_dji-0.1.7/setup.py` & `BTS_dji-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="BTS_dji",
-    version="0.1.7",
+    version="0.1.8",
     description="A simplified version of the dji robomaster library with some addons. Made for the bendigo tech school.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="",
+    url="https://github.com/bendigo-tech-school/BTS-dji",
     author="Bevan Matsacos",
     author_email="B.Matsacos@latrobe.edu.au",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```

