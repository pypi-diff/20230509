# Comparing `tmp/captcha6-0.6.tar.gz` & `tmp/captcha6-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captcha6-0.6.tar", last modified: Tue May  9 15:52:06 2023, max compression
+gzip compressed data, was "captcha6-0.7.tar", last modified: Tue May  9 16:11:13 2023, max compression
```

## Comparing `captcha6-0.6.tar` & `captcha6-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:52:06.200917 captcha6-0.6/
--rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 captcha6-0.6/LICENSE
--rw-rw-rw-   0        0        0     2114 2023-05-09 15:52:06.199917 captcha6-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1557 2023-05-09 15:47:30.000000 captcha6-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 15:52:06.148915 captcha6-0.6/captcha6/
--rw-rw-rw-   0        0        0     1348 2023-05-09 15:48:07.000000 captcha6-0.6/captcha6/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:52:06.196919 captcha6-0.6/captcha6.egg-info/
--rw-rw-rw-   0        0        0     2114 2023-05-09 15:52:05.000000 captcha6-0.6/captcha6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-09 15:52:05.000000 captcha6-0.6/captcha6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:52:05.000000 captcha6-0.6/captcha6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-09 15:52:05.000000 captcha6-0.6/captcha6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 15:52:05.000000 captcha6-0.6/captcha6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 15:52:06.201917 captcha6-0.6/setup.cfg
--rw-rw-rw-   0        0        0      875 2023-05-09 15:48:29.000000 captcha6-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:11:13.044850 captcha6-0.7/
+-rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 captcha6-0.7/LICENSE
+-rw-rw-rw-   0        0        0     2149 2023-05-09 16:11:13.042850 captcha6-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1592 2023-05-09 16:10:45.000000 captcha6-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 16:11:12.986847 captcha6-0.7/captcha6/
+-rw-rw-rw-   0        0        0     1348 2023-05-09 15:48:07.000000 captcha6-0.7/captcha6/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:11:13.040850 captcha6-0.7/captcha6.egg-info/
+-rw-rw-rw-   0        0        0     2149 2023-05-09 16:11:12.000000 captcha6-0.7/captcha6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-09 16:11:12.000000 captcha6-0.7/captcha6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:11:12.000000 captcha6-0.7/captcha6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-09 16:11:12.000000 captcha6-0.7/captcha6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 16:11:12.000000 captcha6-0.7/captcha6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:11:13.044850 captcha6-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      875 2023-05-09 16:11:06.000000 captcha6-0.7/setup.py
```

### Comparing `captcha6-0.6/PKG-INFO` & `captcha6-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captcha6
-Version: 0.6
+Version: 0.7
 Summary: 2captcha.io
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: 2captcha.io
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -52,14 +52,16 @@
 # B3 = CAPTCHAv.CAPTCHAv3(api,websiteKey,websiteURL)
 # print(B3)
 ```
 ---
 ### 2 Here is an example that explains more
 
 ```python 
+from captcha6  import CAPTCHAv 
+
 api = ""
 websiteKey = "6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
 websiteURL = "https://google.com/recaptcha/api2/demo"
 
 
 A2 = CAPTCHAv.CAPTCHAv2(api,websiteKey,websiteURL)
 if "False" == A2:
```

### Comparing `captcha6-0.6/README.md` & `captcha6-0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 # B3 = CAPTCHAv.CAPTCHAv3(api,websiteKey,websiteURL)
 # print(B3)
 ```
 ---
 ### 2 Here is an example that explains more
 
 ```python 
+from captcha6  import CAPTCHAv 
+
 api = ""
 websiteKey = "6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
 websiteURL = "https://google.com/recaptcha/api2/demo"
 
 
 A2 = CAPTCHAv.CAPTCHAv2(api,websiteKey,websiteURL)
 if "False" == A2:
```

### Comparing `captcha6-0.6/captcha6/__init__.py` & `captcha6-0.7/captcha6/__init__.py`

 * *Files identical despite different names*

### Comparing `captcha6-0.6/captcha6.egg-info/PKG-INFO` & `captcha6-0.7/captcha6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captcha6
-Version: 0.6
+Version: 0.7
 Summary: 2captcha.io
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: 2captcha.io
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -52,14 +52,16 @@
 # B3 = CAPTCHAv.CAPTCHAv3(api,websiteKey,websiteURL)
 # print(B3)
 ```
 ---
 ### 2 Here is an example that explains more
 
 ```python 
+from captcha6  import CAPTCHAv 
+
 api = ""
 websiteKey = "6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
 websiteURL = "https://google.com/recaptcha/api2/demo"
 
 
 A2 = CAPTCHAv.CAPTCHAv2(api,websiteKey,websiteURL)
 if "False" == A2:
```

### Comparing `captcha6-0.6/setup.py` & `captcha6-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 # with open('requirements.txt','r') as fr:
 #     requires = fr.read().split('\n')
 
 setuptools.setup(
     name='captcha6',
-    version="0.6",
+    version="0.7",
     author='2captcha.io',
     author_email='omarllStyle@gmail.com',
     description='2captcha.io',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Omarail1/omarpoop.git',
     packages=['captcha6'],
```

