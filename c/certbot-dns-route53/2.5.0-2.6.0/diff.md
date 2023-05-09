# Comparing `tmp/certbot-dns-route53-2.5.0.tar.gz` & `tmp/certbot-dns-route53-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-route53-2.5.0.tar", last modified: Tue Apr  4 15:07:23 2023, max compression
+gzip compressed data, was "certbot-dns-route53-2.6.0.tar", last modified: Tue May  9 19:45:01 2023, max compression
```

## Comparing `certbot-dns-route53-2.5.0.tar` & `certbot-dns-route53-2.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    11357 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      153 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1218 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       66 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/
--rw-r--r--   0 bmw        (501) staff       (20)     3845 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       76 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     6645 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/dns_route53.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       32 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     9508 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/tests/dns_route53_test.py
--rw-r--r--   0 bmw        (501) staff       (20)      594 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/authenticator.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/certbot_dns_route53/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1218 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      677 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)      159 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      113 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       20 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      616 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5816 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      561 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      828 2023-04-04 15:06:41.000000 certbot-dns-route53-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:23.000000 certbot-dns-route53-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2518 2023-04-04 15:06:42.000000 certbot-dns-route53-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:01.334482 certbot-dns-route53-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11357 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      153 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1218 2023-05-09 19:45:01.334482 certbot-dns-route53-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       66 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:01.326484 certbot-dns-route53-2.6.0/certbot_dns_route53/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3845 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/certbot_dns_route53/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:01.326484 certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       76 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6645 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/dns_route53.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:01.326484 certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       32 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9508 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/tests/dns_route53_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      594 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/certbot_dns_route53/authenticator.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/certbot_dns_route53/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:01.326484 certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1218 2023-05-09 19:45:01.000000 certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      677 2023-05-09 19:45:01.000000 certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:45:01.000000 certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      159 2023-05-09 19:45:01.000000 certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      113 2023-05-09 19:45:01.000000 certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       20 2023-05-09 19:45:01.000000 certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:01.330483 certbot-dns-route53-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      616 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5816 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      561 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      828 2023-05-09 19:44:36.000000 certbot-dns-route53-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:45:01.334482 certbot-dns-route53-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2518 2023-05-09 19:44:37.000000 certbot-dns-route53-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-route53-2.5.0/LICENSE.txt` & `certbot-dns-route53-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/PKG-INFO` & `certbot-dns-route53-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-route53
-Version: 2.5.0
+Version: 2.6.0
 Summary: Route53 DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Keywords: certbot,route53,aws
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `certbot-dns-route53-2.5.0/certbot_dns_route53/__init__.py` & `certbot-dns-route53-2.6.0/certbot_dns_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/dns_route53.py` & `certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/dns_route53.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/certbot_dns_route53/_internal/tests/dns_route53_test.py` & `certbot-dns-route53-2.6.0/certbot_dns_route53/_internal/tests/dns_route53_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/certbot_dns_route53/authenticator.py` & `certbot-dns-route53-2.6.0/certbot_dns_route53/authenticator.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/PKG-INFO` & `certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-route53
-Version: 2.5.0
+Version: 2.6.0
 Summary: Route53 DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Keywords: certbot,route53,aws
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `certbot-dns-route53-2.5.0/certbot_dns_route53.egg-info/SOURCES.txt` & `certbot-dns-route53-2.6.0/certbot_dns_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/docs/Makefile` & `certbot-dns-route53-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/docs/conf.py` & `certbot-dns-route53-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/docs/index.rst` & `certbot-dns-route53-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/docs/make.bat` & `certbot-dns-route53-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-route53-2.5.0/setup.py` & `certbot-dns-route53-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.5.0'
+version = '2.6.0'
 
 install_requires = [
     'boto3>=1.15.15',
     'setuptools>=41.6.0',
 ]
 
 if not os.environ.get('SNAP_BUILD'):
```

