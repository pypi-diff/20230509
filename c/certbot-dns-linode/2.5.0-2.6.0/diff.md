# Comparing `tmp/certbot-dns-linode-2.5.0.tar.gz` & `tmp/certbot-dns-linode-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-linode-2.5.0.tar", last modified: Tue Apr  4 15:07:16 2023, max compression
+gzip compressed data, was "certbot-dns-linode-2.6.0.tar", last modified: Tue May  9 19:44:54 2023, max compression
```

## Comparing `certbot-dns-linode-2.5.0.tar` & `certbot-dns-linode-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      152 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1186 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       44 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/
--rw-r--r--   0 bmw        (501) staff       (20)     4055 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       74 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     4089 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/dns_linode.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       31 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     5763 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/tests/dns_linode_test.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/certbot_dns_linode/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1186 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      626 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)       85 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      117 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       19 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      616 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5806 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      563 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      827 2023-04-04 15:06:41.000000 certbot-dns-linode-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:16.000000 certbot-dns-linode-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2389 2023-04-04 15:06:42.000000 certbot-dns-linode-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:54.252226 certbot-dns-linode-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      152 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1186 2023-05-09 19:44:54.252226 certbot-dns-linode-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       44 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:54.248227 certbot-dns-linode-2.6.0/certbot_dns_linode/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4055 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/certbot_dns_linode/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:54.248227 certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       74 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4124 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/dns_linode.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:54.252226 certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       31 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5763 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/tests/dns_linode_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/certbot_dns_linode/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:54.248227 certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1186 2023-05-09 19:44:54.000000 certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      626 2023-05-09 19:44:54.000000 certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:54.000000 certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       85 2023-05-09 19:44:54.000000 certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      117 2023-05-09 19:44:54.000000 certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       19 2023-05-09 19:44:54.000000 certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:54.252226 certbot-dns-linode-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      616 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5806 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      563 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      827 2023-05-09 19:44:36.000000 certbot-dns-linode-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:54.252226 certbot-dns-linode-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2389 2023-05-09 19:44:37.000000 certbot-dns-linode-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-linode-2.5.0/LICENSE.txt` & `certbot-dns-linode-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/PKG-INFO` & `certbot-dns-linode-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-linode
-Version: 2.5.0
+Version: 2.6.0
 Summary: Linode DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-linode-2.5.0/certbot_dns_linode/__init__.py` & `certbot-dns-linode-2.6.0/certbot_dns_linode/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/dns_linode.py` & `certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/dns_linode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """DNS Authenticator for Linode."""
 import logging
 import re
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Optional
 from typing import Union
 
 from lexicon.providers import linode
 from lexicon.providers import linode4
 
 from certbot import errors
@@ -57,15 +58,15 @@
 
     def _cleanup(self, domain: str, validation_name: str, validation: str) -> None:
         self._get_linode_client().del_txt_record(domain, validation_name, validation)
 
     def _get_linode_client(self) -> '_LinodeLexiconClient':
         if not self.credentials:  # pragma: no cover
             raise errors.Error("Plugin has not been prepared.")
-        api_key = self.credentials.conf('key')
+        api_key = cast(str, self.credentials.conf('key'))
         api_version: Optional[Union[str, int]] = self.credentials.conf('version')
         if api_version == '':
             api_version = None
 
         if not api_version:
             api_version = 3
```

### Comparing `certbot-dns-linode-2.5.0/certbot_dns_linode/_internal/tests/dns_linode_test.py` & `certbot-dns-linode-2.6.0/certbot_dns_linode/_internal/tests/dns_linode_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/PKG-INFO` & `certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-linode
-Version: 2.5.0
+Version: 2.6.0
 Summary: Linode DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-linode-2.5.0/certbot_dns_linode.egg-info/SOURCES.txt` & `certbot-dns-linode-2.6.0/certbot_dns_linode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/docs/Makefile` & `certbot-dns-linode-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/docs/conf.py` & `certbot-dns-linode-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/docs/index.rst` & `certbot-dns-linode-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/docs/make.bat` & `certbot-dns-linode-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-linode-2.5.0/setup.py` & `certbot-dns-linode-2.6.0/setup.py`

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
     'dns-lexicon>=3.2.1',
     'setuptools>=41.6.0',
 ]
 
 if not os.environ.get('SNAP_BUILD'):
```

