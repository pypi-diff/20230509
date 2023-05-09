# Comparing `tmp/certbot-dns-rfc2136-2.5.0.tar.gz` & `tmp/certbot-dns-rfc2136-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-dns-rfc2136-2.5.0.tar", last modified: Tue Apr  4 15:07:22 2023, max compression
+gzip compressed data, was "certbot-dns-rfc2136-2.6.0.tar", last modified: Tue May  9 19:44:59 2023, max compression
```

## Comparing `certbot-dns-rfc2136-2.5.0.tar` & `certbot-dns-rfc2136-2.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      153 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1189 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       46 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/
--rw-r--r--   0 bmw        (501) staff       (20)     7240 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       76 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     9746 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/dns_rfc2136.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       32 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     8557 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/tests/dns_rfc2136_test.py
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1189 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)      640 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)       88 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      116 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       20 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/top_level.txt
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/docs/
--rw-r--r--   0 bmw        (501) staff       (20)        9 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/docs/.gitignore
--rw-r--r--   0 bmw        (501) staff       (20)      619 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/docs/Makefile
--rw-r--r--   0 bmw        (501) staff       (20)      149 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/docs/api.rst
--rw-r--r--   0 bmw        (501) staff       (20)     5816 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/docs/conf.py
--rw-r--r--   0 bmw        (501) staff       (20)      561 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/docs/index.rst
--rw-r--r--   0 bmw        (501) staff       (20)      822 2023-04-04 15:06:41.000000 certbot-dns-rfc2136-2.5.0/docs/make.bat
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:22.000000 certbot-dns-rfc2136-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     2394 2023-04-04 15:06:42.000000 certbot-dns-rfc2136-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      153 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1189 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8347 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       76 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10043 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/dns_rfc2136.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       32 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9782 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/tests/dns_rfc2136_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1189 2023-05-09 19:44:59.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      640 2023-05-09 19:44:59.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:59.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       88 2023-05-09 19:44:59.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      116 2023-05-09 19:44:59.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       20 2023-05-09 19:44:59.000000 certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      619 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5816 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      561 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      822 2023-05-09 19:44:36.000000 certbot-dns-rfc2136-2.6.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:59.850839 certbot-dns-rfc2136-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2394 2023-05-09 19:44:37.000000 certbot-dns-rfc2136-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-dns-rfc2136-2.5.0/LICENSE.txt` & `certbot-dns-rfc2136-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-rfc2136-2.5.0/PKG-INFO` & `certbot-dns-rfc2136-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-rfc2136
-Version: 2.5.0
+Version: 2.6.0
 Summary: RFC 2136 DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/__init__.py` & `certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 
 Credentials
 -----------
 
 Use of this plugin requires a configuration file containing the target DNS
 server and optional port that supports RFC 2136 Dynamic Updates, the name
-of the TSIG key, the TSIG key secret itself and the algorithm used if it's
-different to HMAC-MD5.
+of the TSIG key, the TSIG key secret itself, the algorithm used if it's
+different to HMAC-MD5, and optionally whether to sign the initial SOA query.
 
 .. code-block:: ini
    :name: credentials.ini
    :caption: Example credentials file:
 
    # Target DNS server (IPv4 or IPv6 address, not a hostname)
    dns_rfc2136_server = 192.0.2.1
@@ -40,14 +40,17 @@
    # TSIG key name
    dns_rfc2136_name = keyname.
    # TSIG key secret
    dns_rfc2136_secret = 4q4wM/2I180UXoMyN4INVhJNi8V9BCV+jMw2mXgZw/CSuxUT8C7NKKFs \
 AmKd7ak51vWKgSl12ib86oQRPkpDjg==
    # TSIG key algorithm
    dns_rfc2136_algorithm = HMAC-SHA512
+   # TSIG sign SOA query (optional, default: false)
+   dns_rfc2136_sign_query = false
+
 
 The path to this file can be provided interactively or using the
 ``--dns-rfc2136-credentials`` command-line argument. Certbot records the
 path to this file for use during renewal, but does not store the file's contents.
 
 .. caution::
    You should protect this TSIG key material as it can be used to potentially
@@ -190,8 +193,38 @@
 
    view "internal" {
      zone "example.com." IN {
        in-view external;
      };
    };
 
+Another solution is to add `dns_rfc2136_sign_query = true` to the configuration file and then
+add the key to the `match-clients` list within the external zone view. All queries signed with
+this key should then be directed to this view, regardless of source IP.
+
+.. code-block:: none
+   :caption: Split-view BIND configuration with key-based ACLs
+
+   key "keyname." {
+     algorithm hmac-sha512;
+     secret "4q4wM/2I180UXoMyN4INVhJNi8V9BCV+jMw2mXgZw/CSuxUT8C7NKKFs \
+AmKd7ak51vWKgSl12ib86oQRPkpDjg==";
+   };
+
+   // adjust internal-addresses to suit your needs
+   acl internal-address { 127.0.0.0/8; 10.0.0.0/8; 192.168.0.0/16; 172.16.0.0/12; };
+
+   acl certbot-keys { key keyname.; }
+
+   view "external" {
+     match-clients { acl certbot-keys; !internal-addresses; any; };
+
+     zone "example.com." IN {
+       type master;
+       file "named.example.com";
+       update-policy {
+         grant keyname. name _acme-challenge.example.com. txt;
+       };
+     };
+   };
+
 """
```

### Comparing `certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/dns_rfc2136.py` & `certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/dns_rfc2136.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """DNS Authenticator using RFC 2136 Dynamic Updates."""
 import logging
 from typing import Any
 from typing import Callable
+from typing import cast
 from typing import Optional
 
 import dns.flags
 import dns.message
 import dns.name
 import dns.query
 import dns.rdataclass
@@ -55,15 +56,15 @@
         add('credentials', help='RFC 2136 credentials INI file.')
 
     def more_info(self) -> str:
         return 'This plugin configures a DNS TXT record to respond to a dns-01 challenge using ' + \
                'RFC 2136 Dynamic Updates.'
 
     def _validate_credentials(self, credentials: CredentialsConfiguration) -> None:
-        server = credentials.conf('server')
+        server = cast(str, credentials.conf('server'))
         if not is_ipaddress(server):
             raise errors.PluginError("The configured target DNS server ({0}) is not a valid IPv4 "
                                      "or IPv6 address. A hostname is not allowed.".format(server))
         algorithm = credentials.conf('algorithm')
         if algorithm:
             if not self.ALGORITHMS.get(algorithm.upper()):
                 raise errors.PluginError("Unknown algorithm: {0}.".format(algorithm))
@@ -85,34 +86,38 @@
 
     def _cleanup(self, _domain: str, validation_name: str, validation: str) -> None:
         self._get_rfc2136_client().del_txt_record(validation_name, validation)
 
     def _get_rfc2136_client(self) -> "_RFC2136Client":
         if not self.credentials:  # pragma: no cover
             raise errors.Error("Plugin has not been prepared.")
-        return _RFC2136Client(self.credentials.conf('server'),
-                              int(self.credentials.conf('port') or self.PORT),
-                              self.credentials.conf('name'),
-                              self.credentials.conf('secret'),
-                              self.ALGORITHMS.get(self.credentials.conf('algorithm'),
-                                                  dns.tsig.HMAC_MD5))
+
+        return _RFC2136Client(cast(str, self.credentials.conf('server')),
+                              int(cast(str, self.credentials.conf('port')) or self.PORT),
+                              cast(str, self.credentials.conf('name')),
+                              cast(str, self.credentials.conf('secret')),
+                              self.ALGORITHMS.get(self.credentials.conf('algorithm') or '',
+                                                  dns.tsig.HMAC_MD5),
+                              (self.credentials.conf('sign_query') or '').upper() == "TRUE")
 
 
 class _RFC2136Client:
     """
     Encapsulates all communication with the target DNS server.
     """
     def __init__(self, server: str, port: int, key_name: str, key_secret: str,
-                 key_algorithm: dns.name.Name, timeout: int = DEFAULT_NETWORK_TIMEOUT) -> None:
+                 key_algorithm: dns.name.Name, sign_query: bool,
+                 timeout: int = DEFAULT_NETWORK_TIMEOUT) -> None:
         self.server = server
         self.port = port
         self.keyring = dns.tsigkeyring.from_text({
             key_name: key_secret
         })
         self.algorithm = key_algorithm
+        self.sign_query = sign_query
         self._default_timeout = timeout
 
     def add_txt_record(self, record_name: str, record_content: str, record_ttl: int) -> None:
         """
         Add a TXT record using the supplied information.
 
         :param str record_name: The record name (typically beginning with '_acme-challenge.').
@@ -212,16 +217,17 @@
         """
 
         domain = dns.name.from_text(domain_name)
 
         request = dns.message.make_query(domain, dns.rdatatype.SOA, dns.rdataclass.IN)
         # Turn off Recursion Desired bit in query
         request.flags ^= dns.flags.RD
-        # Use our TSIG keyring
-        request.use_tsig(self.keyring, algorithm=self.algorithm)
+        # Use our TSIG keyring if configured
+        if self.sign_query:
+            request.use_tsig(self.keyring, algorithm=self.algorithm)
 
         try:
             try:
                 response = dns.query.tcp(request, self.server, self._default_timeout, self.port)
             except (OSError, dns.exception.Timeout) as e:
                 logger.debug('TCP query failed, fallback to UDP: %s', e)
                 response = dns.query.udp(request, self.server, self._default_timeout, self.port)
```

### Comparing `certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136/_internal/tests/dns_rfc2136_test.py` & `certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136/_internal/tests/dns_rfc2136_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,27 @@
         self.config = mock.MagicMock(rfc2136_credentials=path,
                                      rfc2136_propagation_seconds=0)  # don't wait during tests
 
         self.auth = Authenticator(self.config, "rfc2136")
 
         self.mock_client = mock.MagicMock()
         # _get_rfc2136_client | pylint: disable=protected-access
+        self.orig_get_client = self.auth._get_rfc2136_client
         self.auth._get_rfc2136_client = mock.MagicMock(return_value=self.mock_client)
 
+    def test_get_client_default_conf_values(self):
+        # algorithm and sign_query are intentionally absent to test that the default (None)
+        # value does not crash Certbot.
+        creds = { "server": SERVER, "port": PORT, "name": NAME, "secret": SECRET }
+        self.auth.credentials = mock.MagicMock()
+        self.auth.credentials.conf = lambda key: creds.get(key, None)
+        client = self.orig_get_client()
+        assert client.algorithm == self.auth.ALGORITHMS["HMAC-MD5"]
+        assert client.sign_query == False
+
     @test_util.patch_display_util()
     def test_perform(self, unused_mock_get_utility):
         self.auth.perform([self.achall])
 
         expected = [mock.call.add_txt_record('_acme-challenge.'+DOMAIN, mock.ANY, mock.ANY)]
         assert expected == self.mock_client.mock_calls
 
@@ -96,15 +107,15 @@
 
 class RFC2136ClientTest(unittest.TestCase):
 
     def setUp(self):
         from certbot_dns_rfc2136._internal.dns_rfc2136 import _RFC2136Client
 
         self.rfc2136_client = _RFC2136Client(SERVER, PORT, NAME, SECRET, dns.tsig.HMAC_MD5,
-        TIMEOUT)
+        False, TIMEOUT)
 
     @mock.patch("dns.query.tcp")
     def test_add_txt_record(self, query_mock):
         query_mock.return_value.rcode.return_value = dns.rcode.NOERROR
         # _find_domain | pylint: disable=protected-access
         self.rfc2136_client._find_domain = mock.MagicMock(return_value="example.com")
 
@@ -173,22 +184,25 @@
         # _query_soa | pylint: disable=protected-access
         self.rfc2136_client._query_soa = mock.MagicMock(return_value=False)
 
         with pytest.raises(errors.PluginError):
             self.rfc2136_client._find_domain('foo.bar.'+DOMAIN)
 
     @mock.patch("dns.query.tcp")
-    def test_query_soa_found(self, query_mock):
+    @mock.patch("dns.message.make_query")
+    def test_query_soa_found(self, mock_make_query, query_mock):
         query_mock.return_value = mock.MagicMock(answer=[mock.MagicMock()], flags=dns.flags.AA)
         query_mock.return_value.rcode.return_value = dns.rcode.NOERROR
+        mock_make_query.return_value = mock.MagicMock()
 
         # _query_soa | pylint: disable=protected-access
         result = self.rfc2136_client._query_soa(DOMAIN)
 
         query_mock.assert_called_with(mock.ANY, SERVER, TIMEOUT, PORT)
+        mock_make_query.return_value.use_tsig.assert_not_called()
         assert result
 
     @mock.patch("dns.query.tcp")
     def test_query_soa_not_found(self, query_mock):
         query_mock.return_value.rcode.return_value = dns.rcode.NXDOMAIN
 
         # _query_soa | pylint: disable=protected-access
@@ -214,10 +228,21 @@
         # _query_soa | pylint: disable=protected-access
         result = self.rfc2136_client._query_soa(DOMAIN)
 
         tcp_mock.assert_called_with(mock.ANY, SERVER, TIMEOUT, PORT)
         udp_mock.assert_called_with(mock.ANY, SERVER, TIMEOUT, PORT)
         assert result
 
+    @mock.patch("dns.query.tcp")
+    @mock.patch("dns.message.make_query")
+    def test_query_soa_signed(self, mock_make_query, unused_mock_query):
+        mock_make_query.return_value = mock.MagicMock()
+        self.rfc2136_client.sign_query = True
+        self.rfc2136_client.algorithm = "alg0"
+
+        self.rfc2136_client._query_soa(DOMAIN)
+
+        mock_make_query.return_value.use_tsig.assert_called_with(mock.ANY, algorithm="alg0")
+
 
 if __name__ == "__main__":
     sys.exit(pytest.main(sys.argv[1:] + [__file__]))  # pragma: no cover
```

### Comparing `certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/PKG-INFO` & `certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-rfc2136
-Version: 2.5.0
+Version: 2.6.0
 Summary: RFC 2136 DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-rfc2136-2.5.0/certbot_dns_rfc2136.egg-info/SOURCES.txt` & `certbot-dns-rfc2136-2.6.0/certbot_dns_rfc2136.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-rfc2136-2.5.0/docs/Makefile` & `certbot-dns-rfc2136-2.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-rfc2136-2.5.0/docs/conf.py` & `certbot-dns-rfc2136-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-rfc2136-2.5.0/docs/index.rst` & `certbot-dns-rfc2136-2.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-rfc2136-2.5.0/docs/make.bat` & `certbot-dns-rfc2136-2.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-rfc2136-2.5.0/setup.py` & `certbot-dns-rfc2136-2.6.0/setup.py`

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
     'dnspython>=1.15.0',
     'setuptools>=41.6.0',
 ]
 
 if not os.environ.get('SNAP_BUILD'):
```

