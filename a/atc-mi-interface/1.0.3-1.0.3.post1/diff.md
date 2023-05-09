# Comparing `tmp/atc-mi-interface-1.0.3.tar.gz` & `tmp/atc-mi-interface-1.0.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atc-mi-interface-1.0.3.tar", last modified: Tue May  9 12:45:57 2023, max compression
+gzip compressed data, was "atc-mi-interface-1.0.3.post1.tar", last modified: Tue May  9 12:49:58 2023, max compression
```

## Comparing `atc-mi-interface-1.0.3.tar` & `atc-mi-interface-1.0.3.post1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 12:45:57.331586 atc-mi-interface-1.0.3/
--rw-rw-rw-   0        0        0     2121 2023-05-09 12:45:57.331586 atc-mi-interface-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    43303 2023-05-09 11:41:20.000000 atc-mi-interface-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 12:45:57.315960 atc-mi-interface-1.0.3/atc_mi_interface/
--rw-rw-rw-   0        0        0      327 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3/atc_mi_interface/__init__.py
--rw-rw-rw-   0        0        0     1904 2023-05-09 11:37:14.000000 atc-mi-interface-1.0.3/atc_mi_interface/__main__.py
--rw-rw-rw-   0        0        0     1900 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_adv_format.py
--rw-rw-rw-   0        0        0     4335 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_advertising.py
--rw-rw-rw-   0        0        0    29742 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_config.py
--rw-rw-rw-   0        0        0    28561 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_construct.py
--rw-rw-rw-   0        0        0     6740 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_construct_adapters.py
--rw-rw-rw-   0        0        0     7127 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_format_test.py
--rw-rw-rw-   0        0        0     1918 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3/atc_mi_interface/construct_module.py
-drwxrwxrwx   0        0        0        0 2023-05-09 12:45:57.331586 atc-mi-interface-1.0.3/atc_mi_interface.egg-info/
--rw-rw-rw-   0        0        0     2121 2023-05-09 12:45:57.000000 atc-mi-interface-1.0.3/atc_mi_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2023-05-09 12:45:57.000000 atc-mi-interface-1.0.3/atc_mi_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 12:45:57.000000 atc-mi-interface-1.0.3/atc_mi_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      194 2023-05-09 12:45:57.000000 atc-mi-interface-1.0.3/atc_mi_interface.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       93 2023-05-09 12:45:57.000000 atc-mi-interface-1.0.3/atc_mi_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-09 12:45:57.000000 atc-mi-interface-1.0.3/atc_mi_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 12:45:57.331586 atc-mi-interface-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3444 2023-05-09 12:34:23.000000 atc-mi-interface-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:49:58.591784 atc-mi-interface-1.0.3.post1/
+-rw-rw-rw-   0        0        0     2381 2023-05-09 12:49:58.591784 atc-mi-interface-1.0.3.post1/PKG-INFO
+-rw-rw-rw-   0        0        0    43303 2023-05-09 11:41:20.000000 atc-mi-interface-1.0.3.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 12:49:58.560529 atc-mi-interface-1.0.3.post1/atc_mi_interface/
+-rw-rw-rw-   0        0        0      327 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/__init__.py
+-rw-rw-rw-   0        0        0     1904 2023-05-09 11:37:14.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/__main__.py
+-rw-rw-rw-   0        0        0     1900 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_adv_format.py
+-rw-rw-rw-   0        0        0     4335 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_advertising.py
+-rw-rw-rw-   0        0        0    29742 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_config.py
+-rw-rw-rw-   0        0        0    28561 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_construct.py
+-rw-rw-rw-   0        0        0     6740 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_construct_adapters.py
+-rw-rw-rw-   0        0        0     7127 2023-05-08 22:18:17.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_format_test.py
+-rw-rw-rw-   0        0        0     1918 2023-05-08 07:40:04.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface/construct_module.py
+drwxrwxrwx   0        0        0        0 2023-05-09 12:49:58.576151 atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/
+-rw-rw-rw-   0        0        0     2381 2023-05-09 12:49:58.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2023-05-09 12:49:58.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 12:49:58.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-05-09 12:49:58.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       93 2023-05-09 12:49:58.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-09 12:49:58.000000 atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 12:49:58.591784 atc-mi-interface-1.0.3.post1/setup.cfg
+-rw-rw-rw-   0        0        0     3704 2023-05-09 12:49:13.000000 atc-mi-interface-1.0.3.post1/setup.py
```

### Comparing `atc-mi-interface-1.0.3/PKG-INFO` & `atc-mi-interface-1.0.3.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atc-mi-interface
-Version: 1.0.3
+Version: 1.0.3.post1
 Summary: Python tools and API of the "atc1441" and "pvvx" Xiaomi Mijia Thermometer custom firmware (ATC_MiThermometer)
 Home-page: https://github.com/pvvx/ATC_MiThermometer/tree/master/python-interface
 Author: Ircama
 License: https://unlicense.org
 Keywords: atc-mi-interface,Xiaomi,Mijia,Thermometer,firmware,wxpython,editor,construct,bleak,BLE,bluetooth
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -43,7 +43,11 @@
 
 ```
 pip install [ -i https://test.pypi.org/simple/ ] atc-mi-interface[gui]
 ```
 
 Full information, installation notes, API reference and usage details at the
 [pvvx/ATC_MiThermometer/python-interface repository](https://github.com/pvvx/ATC_MiThermometer/tree/master/python-interface#python-interfacing-methods-and-data-representation-model).
+
+Notice that the above document has not yet updated. Use this URL for the documentation of this pre-release:
+
+https://github.com/Ircama/ATC_MiThermometer/tree/atc-mi-intercace/python-interface#python-interfacing-methods-and-data-representation-model
```

### Comparing `atc-mi-interface-1.0.3/README.md` & `atc-mi-interface-1.0.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/__main__.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/__main__.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_adv_format.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_adv_format.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_advertising.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_advertising.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_config.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_config.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_construct.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_construct.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_construct_adapters.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_construct_adapters.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/atc_mi_format_test.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/atc_mi_format_test.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface/construct_module.py` & `atc-mi-interface-1.0.3.post1/atc_mi_interface/construct_module.py`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface.egg-info/PKG-INFO` & `atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atc-mi-interface
-Version: 1.0.3
+Version: 1.0.3.post1
 Summary: Python tools and API of the "atc1441" and "pvvx" Xiaomi Mijia Thermometer custom firmware (ATC_MiThermometer)
 Home-page: https://github.com/pvvx/ATC_MiThermometer/tree/master/python-interface
 Author: Ircama
 License: https://unlicense.org
 Keywords: atc-mi-interface,Xiaomi,Mijia,Thermometer,firmware,wxpython,editor,construct,bleak,BLE,bluetooth
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -43,7 +43,11 @@
 
 ```
 pip install [ -i https://test.pypi.org/simple/ ] atc-mi-interface[gui]
 ```
 
 Full information, installation notes, API reference and usage details at the
 [pvvx/ATC_MiThermometer/python-interface repository](https://github.com/pvvx/ATC_MiThermometer/tree/master/python-interface#python-interfacing-methods-and-data-representation-model).
+
+Notice that the above document has not yet updated. Use this URL for the documentation of this pre-release:
+
+https://github.com/Ircama/ATC_MiThermometer/tree/atc-mi-intercace/python-interface#python-interfacing-methods-and-data-representation-model
```

### Comparing `atc-mi-interface-1.0.3/atc_mi_interface.egg-info/SOURCES.txt` & `atc-mi-interface-1.0.3.post1/atc_mi_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atc-mi-interface-1.0.3/setup.py` & `atc-mi-interface-1.0.3.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,21 +37,25 @@
 
 ```
 pip install [ -i https://test.pypi.org/simple/ ] atc-mi-interface[gui]
 ```
 
 Full information, installation notes, API reference and usage details at the
 [pvvx/ATC_MiThermometer/python-interface repository](https://github.com/pvvx/ATC_MiThermometer/tree/master/python-interface#python-interfacing-methods-and-data-representation-model).
+
+Notice that the above document has not yet updated. Use this URL for the documentation of this pre-release:
+
+https://github.com/Ircama/ATC_MiThermometer/tree/atc-mi-intercace/python-interface#python-interfacing-methods-and-data-representation-model
 '''
 
 ###########################################################################
 
 setup(
     name="atc-mi-interface",
-    version="1.0.3",  # Format: A.B.C.postN
+    version="1.0.3.post1",  # Format: A.B.C.postN
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Topic :: Software Development :: Libraries :: Python Modules",
         'Programming Language :: Python :: 3 :: Only',
```

