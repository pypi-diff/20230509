# Comparing `tmp/certbot-dns-cloudflare-2.5.0.tar.gz` & `tmp/certbot-dns-cloudflare-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-cloudflare-2.5.0.tar", last modified: Tue Apr  4 15:07:07 2023, max compression
+gzip compressed data, was "certbot-dns-cloudflare-2.6.0.tar", last modified: Tue May  9 19:44:45 2023, max compression
```

## Comparing `certbot-dns-cloudflare-2.5.0.tar` & `certbot-dns-cloudflare-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      156 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1194 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       48 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/
--rw-r--r--   0 bmw        (501) staff       (20)     5309 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       82 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)    12911 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       35 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     9767 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1194 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      682 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)       97 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      116 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       23 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      620 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5846 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      572 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      831 2023-04-04 15:06:41.000000 certbot-dns-cloudflare-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:07.000000 certbot-dns-cloudflare-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2408 2023-04-04 15:06:42.000000 certbot-dns-cloudflare-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:45.862443 certbot-dns-cloudflare-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      156 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1194 2023-05-09 19:44:45.862443 certbot-dns-cloudflare-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       48 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:45.858444 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5309 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:45.858444 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       82 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    12911 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:45.858444 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       35 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9767 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:45.858444 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1194 2023-05-09 19:44:45.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      682 2023-05-09 19:44:45.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:45.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2023-05-09 19:44:45.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      116 2023-05-09 19:44:45.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       23 2023-05-09 19:44:45.000000 certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:45.862443 certbot-dns-cloudflare-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      620 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5846 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      572 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      831 2023-05-09 19:44:36.000000 certbot-dns-cloudflare-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:45.862443 certbot-dns-cloudflare-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2408 2023-05-09 19:44:37.000000 certbot-dns-cloudflare-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-cloudflare-2.5.0/LICENSE.txt` & `certbot-dns-cloudflare-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/PKG-INFO` & `certbot-dns-cloudflare-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-cloudflare
-Version: 2.5.0
+Version: 2.6.0
 Summary: Cloudflare DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/__init__.py` & `certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py` & `certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py` & `certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/PKG-INFO` & `certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-cloudflare
-Version: 2.5.0
+Version: 2.6.0
 Summary: Cloudflare DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-cloudflare-2.5.0/certbot_dns_cloudflare.egg-info/SOURCES.txt` & `certbot-dns-cloudflare-2.6.0/certbot_dns_cloudflare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/docs/Makefile` & `certbot-dns-cloudflare-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/docs/conf.py` & `certbot-dns-cloudflare-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/docs/index.rst` & `certbot-dns-cloudflare-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/docs/make.bat` & `certbot-dns-cloudflare-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.5.0/setup.py` & `certbot-dns-cloudflare-2.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.5.0'
+version = '2.6.0'
 
 install_requires = [
     'cloudflare>=1.5.1',
     'setuptools>=41.6.0',
 ]
 
 if not os.environ.get('SNAP_BUILD'):
```

