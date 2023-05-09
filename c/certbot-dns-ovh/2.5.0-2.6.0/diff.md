# Comparing `tmp/certbot-dns-ovh-2.5.0.tar.gz` & `tmp/certbot-dns-ovh-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-ovh-2.5.0.tar", last modified: Tue Apr  4 15:07:20 2023, max compression
+gzip compressed data, was "certbot-dns-ovh-2.6.0.tar", last modified: Tue May  9 19:44:58 2023, max compression
```

## Comparing `certbot-dns-ovh-2.5.0.tar` & `certbot-dns-ovh-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1180 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       41 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/
--rw-r--r--   0 bmw        (501) staff       (20)     4036 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       68 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     4287 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/dns_ovh.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       28 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     2080 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/tests/dns_ovh_test.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1180 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      584 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)       76 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      117 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       16 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      612 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5776 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      545 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      824 2023-04-04 15:06:41.000000 certbot-dns-ovh-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:20.000000 certbot-dns-ovh-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2374 2023-04-04 15:06:42.000000 certbot-dns-ovh-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:58.475174 certbot-dns-ovh-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1180 2023-05-09 19:44:58.475174 certbot-dns-ovh-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       41 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:58.471175 certbot-dns-ovh-2.6.0/certbot_dns_ovh/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4036 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:58.471175 certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       68 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4355 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/dns_ovh.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:58.471175 certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       28 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2080 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/tests/dns_ovh_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:58.471175 certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1180 2023-05-09 19:44:58.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      584 2023-05-09 19:44:58.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:58.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       76 2023-05-09 19:44:58.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      117 2023-05-09 19:44:58.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       16 2023-05-09 19:44:58.000000 certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:58.471175 certbot-dns-ovh-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      612 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5776 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      545 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      824 2023-05-09 19:44:36.000000 certbot-dns-ovh-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:58.475174 certbot-dns-ovh-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2374 2023-05-09 19:44:37.000000 certbot-dns-ovh-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-ovh-2.5.0/LICENSE.txt` & `certbot-dns-ovh-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/PKG-INFO` & `certbot-dns-ovh-2.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-ovh
-Version: 2.5.0
+Version: 2.6.0
 Summary: OVH DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-ovh-2.5.0/certbot_dns_ovh/__init__.py` & `certbot-dns-ovh-2.6.0/certbot_dns_ovh/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/dns_ovh.py` & `certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/dns_ovh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """DNS Authenticator for OVH DNS."""
 import logging
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Optional
 
 from lexicon.providers import ovh
 from requests import HTTPError
 
 from certbot import errors
 from certbot.plugins import dns_common
@@ -61,18 +62,18 @@
     def _cleanup(self, domain: str, validation_name: str, validation: str) -> None:
         self._get_ovh_client().del_txt_record(domain, validation_name, validation)
 
     def _get_ovh_client(self) -> "_OVHLexiconClient":
         if not self.credentials:  # pragma: no cover
             raise errors.Error("Plugin has not been prepared.")
         return _OVHLexiconClient(
-            self.credentials.conf('endpoint'),
-            self.credentials.conf('application-key'),
-            self.credentials.conf('application-secret'),
-            self.credentials.conf('consumer-key'),
+            cast(str, self.credentials.conf('endpoint')),
+            cast(str, self.credentials.conf('application-key')),
+            cast(str, self.credentials.conf('application-secret')),
+            cast(str, self.credentials.conf('consumer-key')),
             self.ttl
         )
 
 
 class _OVHLexiconClient(dns_common_lexicon.LexiconClient):
     """
     Encapsulates all communication with the OVH API via Lexicon.
```

### Comparing `certbot-dns-ovh-2.5.0/certbot_dns_ovh/_internal/tests/dns_ovh_test.py` & `certbot-dns-ovh-2.6.0/certbot_dns_ovh/_internal/tests/dns_ovh_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/PKG-INFO` & `certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-ovh
-Version: 2.5.0
+Version: 2.6.0
 Summary: OVH DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-ovh-2.5.0/certbot_dns_ovh.egg-info/SOURCES.txt` & `certbot-dns-ovh-2.6.0/certbot_dns_ovh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/docs/Makefile` & `certbot-dns-ovh-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/docs/conf.py` & `certbot-dns-ovh-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/docs/index.rst` & `certbot-dns-ovh-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/docs/make.bat` & `certbot-dns-ovh-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-ovh-2.5.0/setup.py` & `certbot-dns-ovh-2.6.0/setup.py`

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

