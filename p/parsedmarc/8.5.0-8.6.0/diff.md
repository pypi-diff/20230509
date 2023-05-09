# Comparing `tmp/parsedmarc-8.5.0.tar.gz` & `tmp/parsedmarc-8.6.0.tar.gz`

## Comparing `parsedmarc-8.5.0.tar` & `parsedmarc-8.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    61170 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/__init__.py
--rw-r--r--   0        0        0    48948 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/cli.py
--rw-r--r--   0        0        0    20853 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/elastic.py
--rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/kafkaclient.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/log.py
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/loganalytics.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/s3.py
--rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/splunk.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/syslog.py
--rw-r--r--   0        0        0    17841 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/utils.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/__init__.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/gmail.py
--rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/graph.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/imap.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/mail/mailbox_connection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/resources/__init__.py
--rwxr-xr-x   0        0        0  7028733 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/parsedmarc/resources/dbip-country-lite.mmdb
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/LICENSE
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/README.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/pyproject.toml
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 parsedmarc-8.5.0/PKG-INFO
+-rw-r--r--   0        0        0    61170 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/__init__.py
+-rw-r--r--   0        0        0    48948 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/cli.py
+-rw-r--r--   0        0        0    20853 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/elastic.py
+-rw-r--r--   0        0        0     6160 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/kafkaclient.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/log.py
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/loganalytics.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/s3.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/splunk.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/syslog.py
+-rw-r--r--   0        0        0    16553 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/utils.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/__init__.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/gmail.py
+-rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/graph.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/imap.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/mail/mailbox_connection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/resources/__init__.py
+-rwxr-xr-x   0        0        0  7028733 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/parsedmarc/resources/dbip-country-lite.mmdb
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/LICENSE
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/README.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 parsedmarc-8.6.0/PKG-INFO
```

### Comparing `parsedmarc-8.5.0/parsedmarc/__init__.py` & `parsedmarc-8.6.0/parsedmarc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from parsedmarc.log import logger
 from parsedmarc.mail import MailboxConnection
 from parsedmarc.utils import get_base_domain, get_ip_address_info
 from parsedmarc.utils import is_outlook_msg, convert_outlook_msg
 from parsedmarc.utils import parse_email
 from parsedmarc.utils import timestamp_to_human, human_timestamp_to_datetime
 
-__version__ = "8.5.0"
+__version__ = "8.6.0"
 
 logger.debug("parsedmarc v{0}".format(__version__))
 
 feedback_report_regex = re.compile(r"^([\w\-]+): (.+)$", re.MULTILINE)
 xml_header_regex = re.compile(r"^<\?xml .*?>", re.MULTILINE)
 xml_schema_regex = re.compile(r"</??xs:schema.*>", re.MULTILINE)
 text_report_regex = re.compile(r"\s*([a-zA-Z\s]+):\s(.+)", re.MULTILINE)
```

### Comparing `parsedmarc-8.5.0/parsedmarc/cli.py` & `parsedmarc-8.6.0/parsedmarc/cli.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/elastic.py` & `parsedmarc-8.6.0/parsedmarc/elastic.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/kafkaclient.py` & `parsedmarc-8.6.0/parsedmarc/kafkaclient.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/loganalytics.py` & `parsedmarc-8.6.0/parsedmarc/loganalytics.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/s3.py` & `parsedmarc-8.6.0/parsedmarc/s3.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/splunk.py` & `parsedmarc-8.6.0/parsedmarc/splunk.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/syslog.py` & `parsedmarc-8.6.0/parsedmarc/syslog.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/utils.py` & `parsedmarc-8.6.0/parsedmarc/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import tempfile
 import subprocess
 import shutil
 import mailparser
 import json
 import hashlib
 import base64
-import platform
 import atexit
 import mailbox
 import re
 try:
     import importlib.resources as pkg_resources
 except ImportError:
     # Try backported to PY<37 `importlib_resources`
@@ -25,24 +24,19 @@
 
 from dateutil.parser import parse as parse_date
 import dns.reversename
 import dns.resolver
 import dns.exception
 import geoip2.database
 import geoip2.errors
-import requests
-import publicsuffix2
+import publicsuffixlist
 
 from parsedmarc.log import logger
 import parsedmarc.resources
 
-USER_AGENT = "Mozilla/5.0 (({0} {1})) parsedmarc".format(
-            platform.system(),
-            platform.release(),
-        )
 
 parenthesis_regex = re.compile(r'\s*\(.*\)\s*')
 
 null_file = open(os.devnull, "w")
 mailparser_logger = logging.getLogger("mailparser")
 mailparser_logger.setLevel(logging.CRITICAL)
 
@@ -79,59 +73,31 @@
     data = bytes(data, encoding="ascii")
     missing_padding = len(data) % 4
     if missing_padding != 0:
         data += b'=' * (4 - missing_padding)
     return base64.b64decode(data)
 
 
-def get_base_domain(domain, use_fresh_psl=False):
+def get_base_domain(domain):
     """
     Gets the base domain name for the given domain
 
     .. note::
         Results are based on a list of public domain suffixes at
         https://publicsuffix.org/list/public_suffix_list.dat.
 
     Args:
         domain (str): A domain or subdomain
-        use_fresh_psl (bool): Download a fresh Public Suffix List
 
     Returns:
         str: The base domain of the given domain
 
     """
-    psl_path = os.path.join(tempdir, "public_suffix_list.dat")
-
-    def download_psl():
-        url = "https://publicsuffix.org/list/public_suffix_list.dat"
-        # Use a browser-like user agent string to bypass some proxy blocks
-        headers = {"User-Agent": USER_AGENT}
-        try:
-            fresh_psl = requests.get(url, headers=headers).text
-            with open(psl_path, "w", encoding="utf-8") as fresh_psl_file:
-                fresh_psl_file.write(fresh_psl)
-        except Exception as error:
-            raise DownloadError(
-                "Failed to download an updated PSL {0}".format(error))
-
-    if use_fresh_psl:
-        if not os.path.exists(psl_path):
-            download_psl()
-        else:
-            psl_age = datetime.now() - datetime.fromtimestamp(
-                os.stat(psl_path).st_mtime)
-            if psl_age > timedelta(hours=24):
-                download_psl()
-
-        with open(psl_path, encoding="utf-8") as psl_file:
-            psl = publicsuffix2.PublicSuffixList(psl_file)
-
-        return psl.get_public_suffix(domain)
-    else:
-        return publicsuffix2.get_sld(domain)
+    psl = publicsuffixlist.PublicSuffixList()
+    return psl.privatesuffix(domain)
 
 
 def query_dns(domain, record_type, cache=None, nameservers=None, timeout=2.0):
     """
     Queries DNS
 
     Args:
```

### Comparing `parsedmarc-8.5.0/parsedmarc/mail/gmail.py` & `parsedmarc-8.6.0/parsedmarc/mail/gmail.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/mail/graph.py` & `parsedmarc-8.6.0/parsedmarc/mail/graph.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/mail/imap.py` & `parsedmarc-8.6.0/parsedmarc/mail/imap.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/mail/mailbox_connection.py` & `parsedmarc-8.6.0/parsedmarc/mail/mailbox_connection.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/parsedmarc/resources/dbip-country-lite.mmdb` & `parsedmarc-8.6.0/parsedmarc/resources/dbip-country-lite.mmdb`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/.gitignore` & `parsedmarc-8.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/LICENSE` & `parsedmarc-8.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/README.md` & `parsedmarc-8.6.0/README.md`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.5.0/pyproject.toml` & `parsedmarc-8.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "google-auth-oauthlib>=0.4.6",
     "google-auth>=2.3.3",
     "imapclient>=2.1.0",
     "kafka-python>=1.4.4",
     "lxml>=4.4.0",
     "mailsuite>=1.6.1",
     "msgraph-core>=0.2.2",
-    "publicsuffix2>=2.20190812",
+    "publicsuffixlist>=0.10.0",
     "requests>=2.22.0",
     "tqdm>=4.31.1",
     "urllib3>=1.25.7",
     "xmltodict>=0.12.0",
 ]
 
 [project.scripts]
```

### Comparing `parsedmarc-8.5.0/PKG-INFO` & `parsedmarc-8.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsedmarc
-Version: 8.5.0
+Version: 8.6.0
 Summary: A Python package and CLI for parsing aggregate and forensic DMARC reports
 Project-URL: Homepage, https://domainaware.github.io/parsedmarc
 Author-email: Sean Whalen <whalenster@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: DMARC,parser,reporting
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 Requires-Dist: google-auth-oauthlib>=0.4.6
 Requires-Dist: google-auth>=2.3.3
 Requires-Dist: imapclient>=2.1.0
 Requires-Dist: kafka-python>=1.4.4
 Requires-Dist: lxml>=4.4.0
 Requires-Dist: mailsuite>=1.6.1
 Requires-Dist: msgraph-core>=0.2.2
-Requires-Dist: publicsuffix2>=2.20190812
+Requires-Dist: publicsuffixlist>=0.10.0
 Requires-Dist: requests>=2.22.0
 Requires-Dist: tqdm>=4.31.1
 Requires-Dist: urllib3>=1.25.7
 Requires-Dist: xmltodict>=0.12.0
 Description-Content-Type: text/markdown
 
 # parsedmarc
```

