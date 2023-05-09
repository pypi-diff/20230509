# Comparing `tmp/flask-securelogin-0.1.0.tar.gz` & `tmp/flask-securelogin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask-securelogin-0.1.0.tar", last modified: Mon May  8 05:50:31 2023, max compression
+gzip compressed data, was "dist/flask-securelogin-0.1.1.tar", last modified: Tue May  9 01:49:07 2023, max compression
```

## Comparing `flask-securelogin-0.1.0.tar` & `flask-securelogin-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/
--rw-r--r--   0 qianguanghui   (501) staff       (20)      772 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/PKG-INFO
--rw-r--r--   0 qianguanghui   (501) staff       (20)    26526 2023-05-06 20:49:31.000000 flask-securelogin-0.1.0/LICENSE
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin.egg-info/
--rw-r--r--   0 qianguanghui   (501) staff       (20)      772 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin.egg-info/PKG-INFO
--rw-r--r--   0 qianguanghui   (501) staff       (20)      807 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin.egg-info/SOURCES.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)      599 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin.egg-info/requires.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)       18 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin.egg-info/top_level.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)        1 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin.egg-info/dependency_links.txt
--rw-r--r--   0 qianguanghui   (501) staff       (20)       16 2023-05-07 01:00:18.000000 flask-securelogin-0.1.0/MANIFEST.in
--rw-r--r--   0 qianguanghui   (501) staff       (20)     2265 2023-05-08 05:24:17.000000 flask-securelogin-0.1.0/setup.py
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin/
--rw-r--r--   0 qianguanghui   (501) staff       (20)      175 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/exception.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      432 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/SecureAuth.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1969 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/models.py
-drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/flask_securelogin/sms/
--rw-r--r--   0 qianguanghui   (501) staff       (20)      223 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/models.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)        0 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/__init__.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      921 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/SMSBaseSender.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      306 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/SMSCall.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      767 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/TwilioClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     2495 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/TencentAPIClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1580 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/OTPGenerator.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1025 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/SMSFactory.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     1262 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/sms/UniSMSClient.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)       63 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/__init__.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     5497 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/tokens.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)      661 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/errors.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     3846 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/account.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)     7962 2023-05-07 22:47:18.000000 flask-securelogin-0.1.0/flask_securelogin/routes.py
--rw-r--r--   0 qianguanghui   (501) staff       (20)       38 2023-05-08 05:50:31.000000 flask-securelogin-0.1.0/setup.cfg
--rw-r--r--   0 qianguanghui   (501) staff       (20)       99 2023-05-07 00:31:50.000000 flask-securelogin-0.1.0/README.rst
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)    26526 2023-05-06 20:49:31.000000 flask-securelogin-0.1.1/LICENSE
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       16 2023-05-07 01:00:18.000000 flask-securelogin-0.1.1/MANIFEST.in
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      769 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/PKG-INFO
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       99 2023-05-07 00:31:50.000000 flask-securelogin-0.1.1/README.rst
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      432 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/SecureAuth.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       63 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/__init__.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     3846 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/account.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      661 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/errors.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      175 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/exception.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1969 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/models.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     7962 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/routes.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin/sms/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1580 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/OTPGenerator.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      921 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/SMSBaseSender.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      306 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/SMSCall.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1025 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/SMSFactory.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     2495 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/TencentAPIClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      767 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/TwilioClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     1262 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/UniSMSClient.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)        0 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/__init__.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      223 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/sms/models.py
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     5497 2023-05-07 22:47:18.000000 flask-securelogin-0.1.1/flask_securelogin/tokens.py
+drwxr-xr-x   0 qianguanghui   (501) staff       (20)        0 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      769 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/PKG-INFO
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      807 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)        1 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)      599 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/requires.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       18 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/flask_securelogin.egg-info/top_level.txt
+-rw-r--r--   0 qianguanghui   (501) staff       (20)       38 2023-05-09 01:49:07.000000 flask-securelogin-0.1.1/setup.cfg
+-rw-r--r--   0 qianguanghui   (501) staff       (20)     2264 2023-05-09 01:48:52.000000 flask-securelogin-0.1.1/setup.py
```

### Comparing `flask-securelogin-0.1.0/PKG-INFO` & `flask-securelogin-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: flask-securelogin
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.
 Home-page: https://github.com/brilliance-qian/flask-securelogin
 Author: Brilliance Qian
 License: UNKNOWN
-Description: flask_securelogin
-        -----------------
-        To use the library, just type
-        >>> import flask_securelogin
-        >>>
+Description: # flask-securelogin
+        A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flask-securelogin-0.1.0/LICENSE` & `flask-securelogin-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin.egg-info/PKG-INFO` & `flask-securelogin-0.1.1/flask_securelogin.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: flask-securelogin
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.
 Home-page: https://github.com/brilliance-qian/flask-securelogin
 Author: Brilliance Qian
 License: UNKNOWN
-Description: flask_securelogin
-        -----------------
-        To use the library, just type
-        >>> import flask_securelogin
-        >>>
+Description: # flask-securelogin
+        A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flask-securelogin-0.1.0/flask_securelogin.egg-info/SOURCES.txt` & `flask-securelogin-0.1.1/flask_securelogin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin.egg-info/requires.txt` & `flask-securelogin-0.1.1/flask_securelogin.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/setup.py` & `flask-securelogin-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
     with open(file_path, "r") as fh:
         file_contents = fh.read()
     return file_contents
 
 
 setup(
     name='flask-securelogin',
-    version='0.1.0',
+    version='0.1.1',
     description='A Flask-based installable library that provides secure login capabilities with SMS and auth tokens.',
-    long_description=read_content("README.rst"),
+    long_description=read_content("README.md"),
     long_description_content_type="text/markdown",
     url='https://github.com/brilliance-qian/flask-securelogin',
     author='Brilliance Qian',
     license_files=('LICENSE.txt',),
     packages=setuptools.find_packages(),
     install_requires=[
         'aiohttp',
```

### Comparing `flask-securelogin-0.1.0/flask_securelogin/models.py` & `flask-securelogin-0.1.1/flask_securelogin/models.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/sms/SMSBaseSender.py` & `flask-securelogin-0.1.1/flask_securelogin/sms/SMSBaseSender.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/sms/TwilioClient.py` & `flask-securelogin-0.1.1/flask_securelogin/sms/TwilioClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/sms/TencentAPIClient.py` & `flask-securelogin-0.1.1/flask_securelogin/sms/TencentAPIClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/sms/OTPGenerator.py` & `flask-securelogin-0.1.1/flask_securelogin/sms/OTPGenerator.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/sms/SMSFactory.py` & `flask-securelogin-0.1.1/flask_securelogin/sms/SMSFactory.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/sms/UniSMSClient.py` & `flask-securelogin-0.1.1/flask_securelogin/sms/UniSMSClient.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/tokens.py` & `flask-securelogin-0.1.1/flask_securelogin/tokens.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/errors.py` & `flask-securelogin-0.1.1/flask_securelogin/errors.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/account.py` & `flask-securelogin-0.1.1/flask_securelogin/account.py`

 * *Files identical despite different names*

### Comparing `flask-securelogin-0.1.0/flask_securelogin/routes.py` & `flask-securelogin-0.1.1/flask_securelogin/routes.py`

 * *Files identical despite different names*

