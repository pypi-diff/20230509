# Comparing `tmp/certbot-dns-gehirn-2.5.0.tar.gz` & `tmp/certbot-dns-gehirn-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-gehirn-2.5.0.tar", last modified: Tue Apr  4 15:07:13 2023, max compression
+gzip compressed data, was "certbot-dns-gehirn-2.6.0.tar", last modified: Tue May  9 19:44:51 2023, max compression
```

## Comparing `certbot-dns-gehirn-2.5.0.tar` & `certbot-dns-gehirn-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      152 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1209 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       67 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/
--rw-r--r--   0 bmw        (501) staff       (20)     3626 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       74 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     3605 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/dns_gehirn.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       31 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     2005 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/tests/dns_gehirn_test.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1209 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      626 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)       85 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      117 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       19 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      615 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5806 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      557 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      827 2023-04-04 15:06:41.000000 certbot-dns-gehirn-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:13.000000 certbot-dns-gehirn-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2412 2023-04-04 15:06:42.000000 certbot-dns-gehirn-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:51.488937 certbot-dns-gehirn-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      152 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1209 2023-05-09 19:44:51.488937 certbot-dns-gehirn-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       67 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:51.484938 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3626 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:51.484938 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       74 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3651 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/dns_gehirn.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:51.484938 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       31 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2005 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/tests/dns_gehirn_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:51.484938 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1209 2023-05-09 19:44:51.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      626 2023-05-09 19:44:51.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:51.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       85 2023-05-09 19:44:51.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      117 2023-05-09 19:44:51.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       19 2023-05-09 19:44:51.000000 certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:51.484938 certbot-dns-gehirn-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      615 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5806 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      557 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      827 2023-05-09 19:44:36.000000 certbot-dns-gehirn-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:51.488937 certbot-dns-gehirn-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2412 2023-05-09 19:44:37.000000 certbot-dns-gehirn-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-gehirn-2.5.0/LICENSE.txt` & `certbot-dns-gehirn-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/PKG-INFO` & `certbot-dns-gehirn-2.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-gehirn
-Version: 2.5.0
+Version: 2.6.0
 Summary: Gehirn Infrastructure Service DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/__init__.py` & `certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/dns_gehirn.py` & `certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/dns_gehirn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """DNS Authenticator for Gehirn Infrastructure Service DNS."""
 import logging
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Optional
 
 from lexicon.providers import gehirn
 from requests import HTTPError
 
 from certbot import errors
 from certbot.plugins import dns_common
@@ -60,16 +61,16 @@
     def _cleanup(self, domain: str, validation_name: str, validation: str) -> None:
         self._get_gehirn_client().del_txt_record(domain, validation_name, validation)
 
     def _get_gehirn_client(self) -> "_GehirnLexiconClient":
         if not self.credentials:  # pragma: no cover
             raise errors.Error("Plugin has not been prepared.")
         return _GehirnLexiconClient(
-            self.credentials.conf('api-token'),
-            self.credentials.conf('api-secret'),
+            cast(str, self.credentials.conf('api-token')),
+            cast(str, self.credentials.conf('api-secret')),
             self.ttl
         )
 
 
 class _GehirnLexiconClient(dns_common_lexicon.LexiconClient):
     """
     Encapsulates all communication with the Gehirn Infrastructure Service via Lexicon.
```

### Comparing `certbot-dns-gehirn-2.5.0/certbot_dns_gehirn/_internal/tests/dns_gehirn_test.py` & `certbot-dns-gehirn-2.6.0/certbot_dns_gehirn/_internal/tests/dns_gehirn_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/PKG-INFO` & `certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-gehirn
-Version: 2.5.0
+Version: 2.6.0
 Summary: Gehirn Infrastructure Service DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-gehirn-2.5.0/certbot_dns_gehirn.egg-info/SOURCES.txt` & `certbot-dns-gehirn-2.6.0/certbot_dns_gehirn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/docs/Makefile` & `certbot-dns-gehirn-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/docs/conf.py` & `certbot-dns-gehirn-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/docs/index.rst` & `certbot-dns-gehirn-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/docs/make.bat` & `certbot-dns-gehirn-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-gehirn-2.5.0/setup.py` & `certbot-dns-gehirn-2.6.0/setup.py`

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

