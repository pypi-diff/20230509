# Comparing `tmp/checkdmarc-4.5.2.tar.gz` & `tmp/checkdmarc-4.6.0.tar.gz`

## Comparing `checkdmarc-4.5.2.tar` & `checkdmarc-4.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0   117844 2020-02-02 00:00:00.000000 checkdmarc-4.5.2/checkdmarc.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 checkdmarc-4.5.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 checkdmarc-4.5.2/LICENSE
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 checkdmarc-4.5.2/README.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 checkdmarc-4.5.2/pyproject.toml
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 checkdmarc-4.5.2/PKG-INFO
+-rw-r--r--   0        0        0   116311 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/checkdmarc.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/LICENSE
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/README.md
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 checkdmarc-4.6.0/PKG-INFO
```

### Comparing `checkdmarc-4.5.2/checkdmarc.py` & `checkdmarc-4.6.0/checkdmarc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 from collections import OrderedDict
 from re import compile, IGNORECASE
 import json
 from csv import DictWriter
 from argparse import ArgumentParser
 import os
 from time import sleep
-from datetime import datetime, timedelta
 import socket
 import smtplib
 import tempfile
 import platform
 import shutil
 import atexit
-import requests
 from ssl import SSLError, CertificateError, create_default_context
 
 from io import StringIO
 from expiringdict import ExpiringDict
 
-import publicsuffix2
+import publicsuffixlist
 import dns
 import dns.resolver
 import dns.exception
 import timeout_decorator
 from pyleri import (Grammar,
                     Regex,
                     Sequence,
@@ -47,15 +45,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License."""
 
-__version__ = "4.5.2"
+__version__ = "4.6.0"
 
 DMARC_VERSION_REGEX_STRING = r"v *= *DMARC1;"
 BIMI_VERSION_REGEX_STRING = r"v=BIMI1;"
 DMARC_TAG_VALUE_REGEX_STRING = r"([a-z]{1,5}) *= *([\w.:@/+!,_\- ]+)"
 BIMI_TAG_VALUE_REGEX_STRING = r"([a-z]{1}) *= *(.*)"
 MAILTO_REGEX_STRING = r"^(mailto):" \
                       r"([\w\-!#$%&'*+-/=?^_`{|}~]" \
@@ -576,67 +574,32 @@
                               'the entire retrieved '
                               'record MUST be ignored. '
                               'It MUST be the first '
                               'tag in the list.')
 )
 
 
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
-    psl_path = os.path.join(TMPDIR, "public_suffix_list.dat")
 
-    def download_psl():
-        url = "https://publicsuffix.org/list/public_suffix_list.dat"
-        # Use a browser-like user agent string to bypass some proxy blocks
-        headers = {"User-Agent": USER_AGENT}
-        fresh_psl = requests.get(url, headers=headers).text
-        with open(psl_path, "w", encoding="utf-8") as fresh_psl_file:
-            fresh_psl_file.write(fresh_psl)
-
-    domain = domain.lower()
-    if domain.endswith(".test") or domain.endswith(
-        ".example") or domain.endswith(".invalid") or domain.endswith(
-            ".localhost"):
-        parts = domain.strip(".").split(".")
-        if len(parts) == 1:
-            return parts[0]
-        else:
-            return ".".join(parts[-2::])
-    if use_fresh_psl:
-        if not os.path.exists(psl_path):
-            download_psl()
-        else:
-            psl_age = datetime.now() - datetime.fromtimestamp(
-                os.stat(psl_path).st_mtime)
-            if psl_age > timedelta(hours=24):
-                try:
-                    download_psl()
-                except Exception as error:
-                    logging.warning(
-                        "Failed to download an updated PSL {0}".format(error))
-        with open(psl_path, encoding="utf-8") as psl_file:
-            psl = publicsuffix2.PublicSuffixList(psl_file)
-
-        return psl.get_public_suffix(domain)
-    else:
-        return publicsuffix2.get_sld(domain)
+    psl = publicsuffixlist.PublicSuffixList()
+    return psl.privatesuffix(domain)
 
 
 def _query_dns(domain, record_type, nameservers=None, resolver=None,
                timeout=2.0, cache=None):
     """
     Queries DNS
```

### Comparing `checkdmarc-4.5.2/.gitignore` & `checkdmarc-4.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `checkdmarc-4.5.2/LICENSE` & `checkdmarc-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `checkdmarc-4.5.2/README.md` & `checkdmarc-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `checkdmarc-4.5.2/pyproject.toml` & `checkdmarc-4.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Security",
     "Topic :: Communications :: Email",
 ]
 dependencies = [
     "dnspython>=2.0.0",
     "expiringdict>=1.1.4",
-    "publicsuffix2>=2.20191221",
+    "publicsuffixlist>=0.10.0",
     "pyleri>=1.3.2",
     "requests>=2.25.0",
     "timeout-decorator>=0.4.1",
 ]
 
 [project.scripts]
 checkdmarc = "checkdmarc:_main"
```

### Comparing `checkdmarc-4.5.2/PKG-INFO` & `checkdmarc-4.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: checkdmarc
-Version: 4.5.2
+Version: 4.6.0
 Summary: A Python module and command line parser for SPF and DMARC records
 Project-URL: Homepage, https://github.com/domainaware/checkdmarc
 Project-URL: Documentation, https://domainaware.github.io/checkdmarc/
 Project-URL: Issues, https://github.com/domainaware/checkdmarc/issues
 Project-URL: Changelog, https://github.com/domainaware/checkdmarc/blob/master/CHANGELOG.md
 Author-email: Sean Whalen <whalenster@gmail.com>
+License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: DMARC,DNS,SPF
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Security
 Requires-Dist: dnspython>=2.0.0
 Requires-Dist: expiringdict>=1.1.4
-Requires-Dist: publicsuffix2>=2.20191221
+Requires-Dist: publicsuffixlist>=0.10.0
 Requires-Dist: pyleri>=1.3.2
 Requires-Dist: requests>=2.25.0
 Requires-Dist: timeout-decorator>=0.4.1
 Description-Content-Type: text/markdown
 
 # checkdmarc
```

