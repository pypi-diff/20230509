# Comparing `tmp/BTS_dji-0.1.5.tar.gz` & `tmp/BTS_dji-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BTS_dji-0.1.5.tar", last modified: Tue May  9 04:02:29 2023, max compression
+gzip compressed data, was "BTS_dji-0.1.6.tar", last modified: Tue May  9 04:12:12 2023, max compression
```

## Comparing `BTS_dji-0.1.5.tar` & `BTS_dji-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:29.515040 BTS_dji-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:29.511040 BTS_dji-0.1.5/BTS_dji/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-09 04:02:17.000000 BTS_dji-0.1.5/BTS_dji/Robomaster.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:17.000000 BTS_dji-0.1.5/BTS_dji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-05-09 04:02:17.000000 BTS_dji-0.1.5/BTS_dji/controler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-09 04:02:17.000000 BTS_dji-0.1.5/BTS_dji/kbd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:02:29.511040 BTS_dji-0.1.5/BTS_dji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 04:02:29.000000 BTS_dji-0.1.5/BTS_dji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 04:02:29.000000 BTS_dji-0.1.5/BTS_dji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:02:29.000000 BTS_dji-0.1.5/BTS_dji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 04:02:29.000000 BTS_dji-0.1.5/BTS_dji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 04:02:29.000000 BTS_dji-0.1.5/BTS_dji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 04:02:29.511040 BTS_dji-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 04:02:17.000000 BTS_dji-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 04:02:29.515040 BTS_dji-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-09 04:02:17.000000 BTS_dji-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:12:12.660359 BTS_dji-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:12:12.660359 BTS_dji-0.1.6/BTS_dji/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-09 04:12:01.000000 BTS_dji-0.1.6/BTS_dji/Robomaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:12:01.000000 BTS_dji-0.1.6/BTS_dji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26123 2023-05-09 04:12:01.000000 BTS_dji-0.1.6/BTS_dji/controler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-09 04:12:01.000000 BTS_dji-0.1.6/BTS_dji/kbd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:12:12.660359 BTS_dji-0.1.6/BTS_dji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 04:12:12.000000 BTS_dji-0.1.6/BTS_dji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-09 04:12:12.000000 BTS_dji-0.1.6/BTS_dji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:12:12.000000 BTS_dji-0.1.6/BTS_dji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 04:12:12.000000 BTS_dji-0.1.6/BTS_dji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-09 04:12:12.000000 BTS_dji-0.1.6/BTS_dji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-09 04:12:12.660359 BTS_dji-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 04:12:01.000000 BTS_dji-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 04:12:12.660359 BTS_dji-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-09 04:12:01.000000 BTS_dji-0.1.6/setup.py
```

### Comparing `BTS_dji-0.1.5/BTS_dji/Robomaster.py` & `BTS_dji-0.1.6/BTS_dji/Robomaster.py`

 * *Files identical despite different names*

### Comparing `BTS_dji-0.1.5/BTS_dji/controler.py` & `BTS_dji-0.1.6/BTS_dji/controler.py`

 * *Files identical despite different names*

### Comparing `BTS_dji-0.1.5/BTS_dji/kbd.py` & `BTS_dji-0.1.6/BTS_dji/kbd.py`

 * *Files identical despite different names*

### Comparing `BTS_dji-0.1.5/setup.py` & `BTS_dji-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="BTS_dji",
-    version="0.1.5",
+    version="0.1.6",
     description="A simplified version of the dji robomaster library with some addons. Made for the bendigo tech school.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Bevan Matsacos",
     author_email="B.Matsacos@latrobe.edu.au",
     license="MIT",
@@ -27,9 +27,17 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["BTS_dji"],
     include_package_data=True,
-    install_requires=["pynput", "robomaster"]
+    install_requires=[
+        'numpy >= 1.18',
+        'opencv-python >= 4.2',
+        'netaddr >= 0.8',
+        'netifaces >= 0.10',
+        'myqr >= 2.3',
+        'pynput==1.7.6',
+        'robomaster==0.1.1.68',
+    ]
 )
```

