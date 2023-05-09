# Comparing `tmp/basal_and_bark-0.0.7.tar.gz` & `tmp/basal_and_bark-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basal_and_bark-0.0.7.tar", last modified: Sun May  7 03:33:17 2023, max compression
+gzip compressed data, was "basal_and_bark-0.0.8.tar", last modified: Tue May  9 18:51:13 2023, max compression
```

## Comparing `basal_and_bark-0.0.7.tar` & `basal_and_bark-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/basal_and_bark/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/basal_and_bark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/basal_and_bark/basal_and_bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/basal_and_bark/basal_and_bark_folium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/basal_and_bark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:51:13.572009 basal_and_bark-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-09 18:51:13.572009 basal_and_bark-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:51:13.572009 basal_and_bark-0.0.8/basal_and_bark/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/basal_and_bark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/basal_and_bark/basal_and_bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/basal_and_bark/basal_and_bark_folium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:51:13.572009 basal_and_bark-0.0.8/basal_and_bark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-09 18:51:13.000000 basal_and_bark-0.0.8/basal_and_bark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-09 18:51:13.000000 basal_and_bark-0.0.8/basal_and_bark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 18:51:13.000000 basal_and_bark-0.0.8/basal_and_bark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:51:13.000000 basal_and_bark-0.0.8/basal_and_bark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 18:51:13.000000 basal_and_bark-0.0.8/basal_and_bark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 18:51:13.000000 basal_and_bark-0.0.8/basal_and_bark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-09 18:51:13.576009 basal_and_bark-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-09 18:50:59.000000 basal_and_bark-0.0.8/setup.py
```

### Comparing `basal_and_bark-0.0.7/LICENSE` & `basal_and_bark-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.7/PKG-INFO` & `basal_and_bark-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal_and_bark
-Version: 0.0.7
+Version: 0.0.8
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.7/README.md` & `basal_and_bark-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.7/basal_and_bark/basal_and_bark.py` & `basal_and_bark-0.0.8/basal_and_bark/basal_and_bark.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,16 +451,19 @@
 
         Args:
             state (string): State of inventory
             year (string): Year of inventory
         """        
         states = self.statesDict()
         state_name=state
-        url = f"https://apps.fs.usda.gov/fiadb-api/fullreport?rselected=Land%20Use%20-%20Major&cselected=Land%20use&snum=79&wc={states[str(state)]}{year}&outputFormat=NJSON"    
 
+        if state in states:
+            url = f"https://apps.fs.usda.gov/fiadb-api/fullreport?rselected=Land%20Use%20-%20Major&cselected=Land%20use&snum=79&wc={states[str(state)]}{year}&outputFormat=NJSON"    
+        else:
+            return "This is not a state in the USFS Southern Research Station."
 
         resp = requests.get(url)
         data = resp.json()
  # create output dictionary and populate it with estimate data frames
         outDict = {}
     # append estimates
         outDict['estimates'] = pandas.DataFrame(data['estimates'])
```

### Comparing `basal_and_bark-0.0.7/basal_and_bark/basal_and_bark_folium.py` & `basal_and_bark-0.0.8/basal_and_bark/basal_and_bark_folium.py`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.7/basal_and_bark.egg-info/PKG-INFO` & `basal_and_bark-0.0.8/basal_and_bark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal-and-bark
-Version: 0.0.7
+Version: 0.0.8
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.7/setup.py` & `basal_and_bark-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='basal_and_bark',
     name='basal_and_bark',
     packages=find_packages(include=['basal_and_bark', 'basal_and_bark.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZachDorm/basal_and_bark',
-    version='0.0.7',
+    version='0.0.8',
     zip_safe=False,
 )
```

