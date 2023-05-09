# Comparing `tmp/certbot-dns-google-2.5.0.tar.gz` & `tmp/certbot-dns-google-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-google-2.5.0.tar", last modified: Tue Apr  4 15:07:14 2023, max compression
+gzip compressed data, was "certbot-dns-google-2.6.0.tar", last modified: Tue May  9 19:44:52 2023, max compression
```

## Comparing `certbot-dns-google-2.5.0.tar` & `certbot-dns-google-2.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      216 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1192 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       50 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google/
--rw-r--r--   0 bmw        (501) staff       (20)     5190 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/certbot_dns_google/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       74 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)    13492 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/dns_google.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       31 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)    21024 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/tests/dns_google_test.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/tests/testdata/
--rw-r--r--   0 bmw        (501) staff       (20)    47584 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/certbot_dns_google/_internal/tests/testdata/discovery.json
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/certbot_dns_google/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1192 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      685 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)       85 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      157 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       19 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/certbot_dns_google.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      615 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5805 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      557 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      827 2023-04-04 15:06:41.000000 certbot-dns-google-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:14.000000 certbot-dns-google-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2530 2023-04-04 15:06:42.000000 certbot-dns-google-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:52.872578 certbot-dns-google-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      216 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1192 2023-05-09 19:44:52.872578 certbot-dns-google-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       50 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:52.868579 certbot-dns-google-2.6.0/certbot_dns_google/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10225 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/certbot_dns_google/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:52.868579 certbot-dns-google-2.6.0/certbot_dns_google/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       74 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/certbot_dns_google/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13426 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/certbot_dns_google/_internal/dns_google.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:52.868579 certbot-dns-google-2.6.0/certbot_dns_google/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       31 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/certbot_dns_google/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22735 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/certbot_dns_google/_internal/tests/dns_google_test.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:52.868579 certbot-dns-google-2.6.0/certbot_dns_google/_internal/tests/testdata/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    47584 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/certbot_dns_google/_internal/tests/testdata/discovery.json
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/certbot_dns_google/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:52.868579 certbot-dns-google-2.6.0/certbot_dns_google.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1192 2023-05-09 19:44:52.000000 certbot-dns-google-2.6.0/certbot_dns_google.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      685 2023-05-09 19:44:52.000000 certbot-dns-google-2.6.0/certbot_dns_google.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:52.000000 certbot-dns-google-2.6.0/certbot_dns_google.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       85 2023-05-09 19:44:52.000000 certbot-dns-google-2.6.0/certbot_dns_google.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      150 2023-05-09 19:44:52.000000 certbot-dns-google-2.6.0/certbot_dns_google.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       19 2023-05-09 19:44:52.000000 certbot-dns-google-2.6.0/certbot_dns_google.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:52.872578 certbot-dns-google-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      615 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5805 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      557 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      827 2023-05-09 19:44:36.000000 certbot-dns-google-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:52.872578 certbot-dns-google-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2435 2023-05-09 19:44:37.000000 certbot-dns-google-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-google-2.5.0/LICENSE.txt` & `certbot-dns-google-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.5.0/PKG-INFO` & `certbot-dns-google-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-google
-Version: 2.5.0
+Version: 2.6.0
 Summary: Google Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-google-2.5.0/certbot_dns_google/_internal/dns_google.py` & `certbot-dns-google-2.6.0/certbot_dns_google/_internal/dns_google.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """DNS Authenticator for Google Cloud DNS."""
-import json
 import logging
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Optional
 
+import google.auth
+
+from google.auth import exceptions as googleauth_exceptions
 from googleapiclient import discovery
 from googleapiclient import errors as googleapiclient_errors
-import httplib2
-from oauth2client.service_account import ServiceAccountCredentials
 
 from certbot import errors
 from certbot.plugins import dns_common
 
 logger = logging.getLogger(__name__)
 
+ADC_URL = 'https://cloud.google.com/docs/authentication/application-default-credentials'
 ACCT_URL = 'https://developers.google.com/identity/protocols/OAuth2ServiceAccount#creatinganaccount'
 PERMISSIONS_URL = 'https://cloud.google.com/dns/access-control#permissions_and_roles'
 METADATA_URL = 'http://metadata.google.internal/computeMetadata/v1/'
 METADATA_HEADERS = {'Metadata-Flavor': 'Google'}
 
 
 class Authenticator(dns_common.DNSAuthenticator):
@@ -27,76 +28,95 @@
 
     This Authenticator uses the Google Cloud DNS API to fulfill a dns-01 challenge.
     """
 
     description = ('Obtain certificates using a DNS TXT record (if you are using Google Cloud DNS '
                    'for DNS).')
     ttl = 60
+    google_client = None
 
     @classmethod
     def add_parser_arguments(cls, add: Callable[..., None],
                              default_propagation_seconds: int = 60) -> None:
         super().add_parser_arguments(add, default_propagation_seconds=60)
         add('credentials',
-            help=('Path to Google Cloud DNS service account JSON file. (See {0} for' +
-                  'information about creating a service account and {1} for information about the' +
-                  'required permissions.)').format(ACCT_URL, PERMISSIONS_URL),
+            help=('Path to Google Cloud DNS service account JSON file to use instead of relying on'
+                  ' Application Default Credentials (ADC). (See {0} for information about ADC, {1}'
+                  ' for information about creating a service account, and {2} for information about'
+                  ' the permissions required to modify Cloud DNS records.)')
+                  .format(ADC_URL, ACCT_URL, PERMISSIONS_URL),
+            default=None)
+
+        add('project',
+            help=('The ID of the Google Cloud project that the Google Cloud DNS managed zone(s)' +
+                  ' reside in. This will be determined automatically if not specified.'),
             default=None)
 
     def more_info(self) -> str:
         return 'This plugin configures a DNS TXT record to respond to a dns-01 challenge using ' + \
                'the Google Cloud DNS API.'
 
     def _setup_credentials(self) -> None:
-        if self.conf('credentials') is None:
-            try:
-                # use project_id query to check for availability of google metadata server
-                # we won't use the result but know we're not on GCP when an exception is thrown
-                _GoogleClient.get_project_id()
-            except (ValueError, httplib2.ServerNotFoundError):
-                raise errors.PluginError('Unable to get Google Cloud Metadata and no credentials'
-                                         ' specified. Automatic credential lookup is only '
-                                         'available on Google Cloud Platform. Please configure'
-                                         ' credentials using --dns-google-credentials <file>')
-        else:
+        if self.conf('credentials') is not None:
             self._configure_file('credentials',
                                  'path to Google Cloud DNS service account JSON file')
 
             dns_common.validate_file_permissions(self.conf('credentials'))
 
+        try:
+            self._get_google_client()
+        except googleauth_exceptions.DefaultCredentialsError as e:
+            raise errors.PluginError('Authentication using Google Application Default Credentials '
+                                     'failed ({}). Please configure credentials using'
+                                     ' --dns-google-credentials <file>'.format(e))
+
     def _perform(self, domain: str, validation_name: str, validation: str) -> None:
         self._get_google_client().add_txt_record(domain, validation_name, validation, self.ttl)
 
     def _cleanup(self, domain: str, validation_name: str, validation: str) -> None:
         self._get_google_client().del_txt_record(domain, validation_name, validation, self.ttl)
 
     def _get_google_client(self) -> '_GoogleClient':
-        return _GoogleClient(self.conf('credentials'))
+        if self.google_client is None:
+            self.google_client = _GoogleClient(self.conf('credentials'), self.conf('project'))
+        return self.google_client
+
 
 
 class _GoogleClient:
     """
     Encapsulates all communication with the Google Cloud DNS API.
     """
 
     def __init__(self, account_json: Optional[str] = None,
+                 dns_project_id: Optional[str] = None,
                  dns_api: Optional[discovery.Resource] = None) -> None:
 
         scopes = ['https://www.googleapis.com/auth/ndev.clouddns.readwrite']
+        credentials = None
+        project_id = None
+
         if account_json is not None:
             try:
-                credentials = ServiceAccountCredentials.from_json_keyfile_name(account_json, scopes)
-                with open(account_json) as account:
-                    self.project_id = json.load(account)['project_id']
-            except Exception as e:
+                credentials, project_id = google.auth.load_credentials_from_file(
+                    account_json, scopes=scopes)
+            except googleauth_exceptions.GoogleAuthError as e:
                 raise errors.PluginError(
-                    "Error parsing credentials file '{}': {}".format(account_json, e))
+                    "Error loading credentials file '{}': {}".format(account_json, e))
         else:
-            credentials = None
-            self.project_id = self.get_project_id()
+            credentials, project_id = google.auth.default(scopes=scopes)
+
+        if dns_project_id is not None:
+            project_id = dns_project_id
+
+        if not project_id:
+            raise errors.PluginError('The Google Cloud project could not be automatically '
+                                     'determined. Please configure it using --dns-google-project'
+                                     ' <project>.')
+        self.project_id = project_id
 
         if not dns_api:
             self.dns = discovery.build('dns', 'v1',
                                        credentials=credentials,
                                        cache_discovery=False)
         else:
             self.dns = dns_api
@@ -288,30 +308,7 @@
                 zone_id = zone['id']
                 if 'privateVisibilityConfig' not in zone:
                     logger.debug('Found id of %s for %s using name %s', zone_id, domain, zone_name)
                     return zone_id
 
         raise errors.PluginError('Unable to determine managed zone for {0} using zone names: {1}.'
                                  .format(domain, zone_dns_name_guesses))
-
-    @staticmethod
-    def get_project_id() -> str:
-        """
-        Query the google metadata service for the current project ID
-
-        This only works on Google Cloud Platform
-
-        :raises ServerNotFoundError: Not running on Google Compute or DNS not available
-        :raises ValueError: Server is found, but response code is not 200
-        :returns: project id
-        """
-        url = '{0}project/project-id'.format(METADATA_URL)
-
-        # Request an access token from the metadata server.
-        http = httplib2.Http()
-        r, content = http.request(url, headers=METADATA_HEADERS)
-        if r.status != 200:
-            raise ValueError("Invalid status code: {0}".format(r))
-
-        if isinstance(content, bytes):
-            return content.decode()
-        return content
```

### Comparing `certbot-dns-google-2.5.0/certbot_dns_google/_internal/tests/testdata/discovery.json` & `certbot-dns-google-2.6.0/certbot_dns_google/_internal/tests/testdata/discovery.json`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.5.0/certbot_dns_google.egg-info/PKG-INFO` & `certbot-dns-google-2.6.0/certbot_dns_google.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-google
-Version: 2.5.0
+Version: 2.6.0
 Summary: Google Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-google-2.5.0/certbot_dns_google.egg-info/SOURCES.txt` & `certbot-dns-google-2.6.0/certbot_dns_google.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.5.0/docs/Makefile` & `certbot-dns-google-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.5.0/docs/conf.py` & `certbot-dns-google-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.5.0/docs/index.rst` & `certbot-dns-google-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.5.0/docs/make.bat` & `certbot-dns-google-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.5.0/setup.py` & `certbot-dns-google-2.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.5.0'
+version = '2.6.0'
 
 install_requires = [
-    'google-api-python-client>=1.5.5',
-    'oauth2client>=4.0',
+    'google-api-python-client>=1.6.5',
+    'google-auth>=2.16.0',
     'setuptools>=41.6.0',
-    # already a dependency of google-api-python-client, but added for consistency
-    'httplib2'
 ]
 
 if not os.environ.get('SNAP_BUILD'):
     install_requires.extend([
         # We specify the minimum acme and certbot version as the current plugin
         # version for simplicity. See
         # https://github.com/certbot/certbot/issues/8761 for more info.
```

