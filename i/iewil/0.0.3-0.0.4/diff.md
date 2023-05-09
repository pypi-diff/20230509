# Comparing `tmp/iewil-0.0.3.tar.gz` & `tmp/iewil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iewil-0.0.3.tar", last modified: Tue May  9 14:41:46 2023, max compression
+gzip compressed data, was "iewil-0.0.4.tar", last modified: Tue May  9 15:00:03 2023, max compression
```

## Comparing `iewil-0.0.3.tar` & `iewil-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 14:41:46.228738 iewil-0.0.3/
--rw-rw-rw-   0        0        0      436 2023-05-09 14:41:46.227745 iewil-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 14:41:46.209979 iewil-0.0.3/iewil/
--rw-rw-rw-   0        0        0     4321 2023-05-09 14:41:17.000000 iewil-0.0.3/iewil/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 14:41:46.225792 iewil-0.0.3/iewil.egg-info/
--rw-rw-rw-   0        0        0      436 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-09 14:41:45.000000 iewil-0.0.3/iewil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 14:41:46.228738 iewil-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      650 2023-05-09 14:40:35.000000 iewil-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:00:03.201168 iewil-0.0.4/
+-rw-rw-rw-   0        0        0      436 2023-05-09 15:00:03.200192 iewil-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 15:00:03.186528 iewil-0.0.4/iewil/
+-rw-rw-rw-   0        0        0     4267 2023-05-09 14:57:39.000000 iewil-0.0.4/iewil/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:00:03.199216 iewil-0.0.4/iewil.egg-info/
+-rw-rw-rw-   0        0        0      436 2023-05-09 15:00:03.000000 iewil-0.0.4/iewil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-05-09 15:00:03.000000 iewil-0.0.4/iewil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 15:00:03.000000 iewil-0.0.4/iewil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-09 15:00:03.000000 iewil-0.0.4/iewil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 15:00:03.201168 iewil-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      650 2023-05-09 14:59:49.000000 iewil-0.0.4/setup.py
```

### Comparing `iewil-0.0.3/iewil/__init__.py` & `iewil-0.0.4/iewil/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,9 +95,8 @@
         a += 1
         x = random.choice(col)
         nic = auth(x)
         res = timr - time.time()
         if res < 1:
             break
         print("         " + x + sym[a % 4] + p + str(int(res / 3600)) + x + ":" + p + str(int((res % 3600) / 60)) + x + ":" + p + str(int(res % 60)) + nic[a % 18], end="\r")
-        time.sleep(0.1)
-    print("\r                                   \r")
+        time.sleep(0.1)
```

### Comparing `iewil-0.0.3/setup.py` & `iewil-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'modul pribadi ygy'
 
 # Setting up
 setup(
     name="iewil",
     version=VERSION,
     author="iewilmaestro",
```

