# Comparing `tmp/certbot-dns-sakuracloud-2.5.0.tar.gz` & `tmp/certbot-dns-sakuracloud-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-sakuracloud-2.5.0.tar", last modified: Tue Apr  4 15:07:25 2023, max compression
+gzip compressed data, was "certbot-dns-sakuracloud-2.6.0.tar", last modified: Tue May  9 19:45:02 2023, max compression
```

## Comparing `certbot-dns-sakuracloud-2.5.0.tar` & `certbot-dns-sakuracloud-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      157 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1197 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       50 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/
--rw-r--r--   0 bmw        (501) staff       (20)     3607 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       84 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     3444 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/dns_sakuracloud.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       36 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     2120 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/tests/dns_sakuracloud_test.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1197 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      696 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)      100 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      117 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       24 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      620 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5856 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      577 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      832 2023-04-04 15:06:41.000000 certbot-dns-sakuracloud-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:25.000000 certbot-dns-sakuracloud-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2415 2023-04-04 15:06:42.000000 certbot-dns-sakuracloud-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:02.818129 certbot-dns-sakuracloud-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      157 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1197 2023-05-09 19:45:02.818129 certbot-dns-sakuracloud-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       50 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:02.814130 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3607 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:02.818129 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       84 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3490 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/dns_sakuracloud.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:02.818129 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       36 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2120 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/tests/dns_sakuracloud_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:02.814130 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1197 2023-05-09 19:45:02.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      696 2023-05-09 19:45:02.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:45:02.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      100 2023-05-09 19:45:02.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      117 2023-05-09 19:45:02.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       24 2023-05-09 19:45:02.000000 certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:45:02.818129 certbot-dns-sakuracloud-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      620 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5856 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      577 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      832 2023-05-09 19:44:36.000000 certbot-dns-sakuracloud-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:45:02.818129 certbot-dns-sakuracloud-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2415 2023-05-09 19:44:37.000000 certbot-dns-sakuracloud-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-sakuracloud-2.5.0/LICENSE.txt` & `certbot-dns-sakuracloud-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/PKG-INFO` & `certbot-dns-sakuracloud-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-sakuracloud
-Version: 2.5.0
+Version: 2.6.0
 Summary: Sakura Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/__init__.py` & `certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/dns_sakuracloud.py` & `certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/dns_sakuracloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """DNS Authenticator for Sakura Cloud DNS."""
 import logging
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Optional
 
 from lexicon.providers import sakuracloud
 from requests import HTTPError
 
 from certbot import errors
 from certbot.plugins import dns_common
@@ -60,16 +61,16 @@
         self._get_sakuracloud_client().del_txt_record(
             domain, validation_name, validation)
 
     def _get_sakuracloud_client(self) -> "_SakuraCloudLexiconClient":
         if not self.credentials:  # pragma: no cover
             raise errors.Error("Plugin has not been prepared.")
         return _SakuraCloudLexiconClient(
-            self.credentials.conf('api-token'),
-            self.credentials.conf('api-secret'),
+            cast(str, self.credentials.conf('api-token')),
+            cast(str, self.credentials.conf('api-secret')),
             self.ttl
         )
 
 
 class _SakuraCloudLexiconClient(dns_common_lexicon.LexiconClient):
     """
     Encapsulates all communication with the Sakura Cloud via Lexicon.
```

### Comparing `certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud/_internal/tests/dns_sakuracloud_test.py` & `certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud/_internal/tests/dns_sakuracloud_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/PKG-INFO` & `certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-sakuracloud
-Version: 2.5.0
+Version: 2.6.0
 Summary: Sakura Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-sakuracloud-2.5.0/certbot_dns_sakuracloud.egg-info/SOURCES.txt` & `certbot-dns-sakuracloud-2.6.0/certbot_dns_sakuracloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/docs/Makefile` & `certbot-dns-sakuracloud-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/docs/conf.py` & `certbot-dns-sakuracloud-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/docs/index.rst` & `certbot-dns-sakuracloud-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/docs/make.bat` & `certbot-dns-sakuracloud-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-sakuracloud-2.5.0/setup.py` & `certbot-dns-sakuracloud-2.6.0/setup.py`

 * *Files 4% similar despite different names*

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

