# Comparing `tmp/certbot-dns-digitalocean-2.5.0.tar.gz` & `tmp/certbot-dns-digitalocean-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-digitalocean-2.5.0.tar", last modified: Tue Apr  4 15:07:08 2023, max compression
+gzip compressed data, was "certbot-dns-digitalocean-2.6.0.tar", last modified: Tue May  9 19:44:47 2023, max compression
```

## Comparing `certbot-dns-digitalocean-2.5.0.tar` & `certbot-dns-digitalocean-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      158 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1198 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       50 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/
--rw-r--r--   0 bmw        (501) staff       (20)     3892 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       86 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     7611 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/dns_digitalocean.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       37 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     6698 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/tests/dns_digitalocean_test.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1198 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      710 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)      103 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      124 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       25 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      621 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5866 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      581 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      833 2023-04-04 15:06:41.000000 certbot-dns-digitalocean-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:08.000000 certbot-dns-digitalocean-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2475 2023-04-04 15:06:42.000000 certbot-dns-digitalocean-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      158 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1198 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       50 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3892 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       86 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7646 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/dns_digitalocean.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       37 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6698 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/tests/dns_digitalocean_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1198 2023-05-09 19:44:47.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      710 2023-05-09 19:44:47.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:47.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      103 2023-05-09 19:44:47.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      124 2023-05-09 19:44:47.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       25 2023-05-09 19:44:47.000000 certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      621 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5866 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      581 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      833 2023-05-09 19:44:36.000000 certbot-dns-digitalocean-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:47.242066 certbot-dns-digitalocean-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2475 2023-05-09 19:44:37.000000 certbot-dns-digitalocean-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-digitalocean-2.5.0/LICENSE.txt` & `certbot-dns-digitalocean-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/PKG-INFO` & `certbot-dns-digitalocean-2.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-digitalocean
-Version: 2.5.0
+Version: 2.6.0
 Summary: DigitalOcean DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/__init__.py` & `certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/dns_digitalocean.py` & `certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/dns_digitalocean.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """DNS Authenticator for DigitalOcean."""
 import logging
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Optional
 
 import digitalocean
 
 from certbot import errors
 from certbot.plugins import dns_common
 from certbot.plugins.dns_common import CredentialsConfiguration
@@ -52,15 +53,15 @@
 
     def _cleanup(self, domain: str, validation_name: str, validation: str) -> None:
         self._get_digitalocean_client().del_txt_record(domain, validation_name, validation)
 
     def _get_digitalocean_client(self) -> "_DigitalOceanClient":
         if not self.credentials:  # pragma: no cover
             raise errors.Error("Plugin has not been prepared.")
-        return _DigitalOceanClient(self.credentials.conf('token'))
+        return _DigitalOceanClient(cast(str, self.credentials.conf('token')))
 
 
 class _DigitalOceanClient:
     """
     Encapsulates all communication with the DigitalOcean API.
     """
```

### Comparing `certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean/_internal/tests/dns_digitalocean_test.py` & `certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean/_internal/tests/dns_digitalocean_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/PKG-INFO` & `certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-digitalocean
-Version: 2.5.0
+Version: 2.6.0
 Summary: DigitalOcean DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-digitalocean-2.5.0/certbot_dns_digitalocean.egg-info/SOURCES.txt` & `certbot-dns-digitalocean-2.6.0/certbot_dns_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/docs/Makefile` & `certbot-dns-digitalocean-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/docs/conf.py` & `certbot-dns-digitalocean-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/docs/index.rst` & `certbot-dns-digitalocean-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/docs/make.bat` & `certbot-dns-digitalocean-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-digitalocean-2.5.0/setup.py` & `certbot-dns-digitalocean-2.6.0/setup.py`

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
     'python-digitalocean>=1.11', # 1.15.0 or newer is recommended for TTL support
     'setuptools>=41.6.0',
 ]
 
 if not os.environ.get('SNAP_BUILD'):
```

