# Comparing `tmp/bitsrun-3.5.1.tar.gz` & `tmp/bitsrun-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitsrun-3.5.1.tar", last modified: Tue Apr  4 03:25:53 2023, max compression
+gzip compressed data, was "bitsrun-3.5.2.tar", last modified: Tue May  9 10:13:24 2023, max compression
```

## Comparing `bitsrun-3.5.1.tar` & `bitsrun-3.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      496 2023-04-04 03:25:29.668641 bitsrun-3.5.1/LICENSE
--rw-r--r--   0        0        0     3445 2023-04-04 03:25:29.668641 bitsrun-3.5.1/README.md
--rw-r--r--   0        0        0        0 2023-04-04 03:25:29.668641 bitsrun-3.5.1/bitsrun/__init__.py
--rw-r--r--   0        0        0     4571 2023-04-04 03:25:29.668641 bitsrun-3.5.1/bitsrun/cli.py
--rw-r--r--   0        0        0     2332 2023-04-04 03:25:29.668641 bitsrun-3.5.1/bitsrun/config.py
--rw-r--r--   0        0        0      891 2023-04-04 03:25:29.668641 bitsrun-3.5.1/bitsrun/models.py
--rw-r--r--   0        0        0     4634 2023-04-04 03:25:29.668641 bitsrun-3.5.1/bitsrun/user.py
--rw-r--r--   0        0        0     4193 2023-04-04 03:25:29.668641 bitsrun-3.5.1/bitsrun/utils.py
--rw-r--r--   0        0        0     1739 2023-04-04 03:25:29.668641 bitsrun-3.5.1/pyproject.toml
--rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 bitsrun-3.5.1/PKG-INFO
+-rw-r--r--   0        0        0      496 2023-05-09 10:12:57.953702 bitsrun-3.5.2/LICENSE
+-rw-r--r--   0        0        0     3445 2023-05-09 10:12:57.953702 bitsrun-3.5.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/__init__.py
+-rw-r--r--   0        0        0     4811 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/cli.py
+-rw-r--r--   0        0        0     2332 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/config.py
+-rw-r--r--   0        0        0      891 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/models.py
+-rw-r--r--   0        0        0     4921 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/user.py
+-rw-r--r--   0        0        0     4193 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/utils.py
+-rw-r--r--   0        0        0     1739 2023-05-09 10:12:57.953702 bitsrun-3.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 bitsrun-3.5.2/PKG-INFO
```

### Comparing `bitsrun-3.5.1/README.md` & `bitsrun-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.1/bitsrun/cli.py` & `bitsrun-3.5.2/bitsrun/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+import warnings
 from getpass import getpass
 from json import dumps
 
 import click
 from rich import print_json
 
 from bitsrun.config import get_config_paths, read_config
@@ -14,14 +15,22 @@
 _options = [
     click.option("-u", "--username", help="Your username.", required=False),
     click.option("-p", "--password", help="Your password.", required=False),
     click.option("-v", "--verbose", is_flag=True, help="Verbosely echo API response."),
 ]
 
 
+# Replace the default implementation
+warnings.showwarning = (
+    lambda message, category, filename, lineno, file=None, line=None: click.echo(
+        f"{click.style('warning:', fg='yellow')} {message}", err=True
+    )
+)
+
+
 # Decorator to add options to a click command (used w/ the hack above)
 def add_options(options):
     def _add_options(func):
         for option in reversed(options):
             func = option(func)
         return func
```

### Comparing `bitsrun-3.5.1/bitsrun/config.py` & `bitsrun-3.5.2/bitsrun/config.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.1/bitsrun/models.py` & `bitsrun-3.5.2/bitsrun/models.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.1/bitsrun/user.py` & `bitsrun-3.5.2/bitsrun/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hmac
 import json
 from hashlib import sha1
 from typing import Optional
+from warnings import warn
 
 import httpx
 
 from bitsrun.models import LoginStatusRespType, UserResponseType
 from bitsrun.utils import fkbase64, xencode
 
 _API_BASE = "http://10.0.0.55"
@@ -51,17 +52,20 @@
         # Check current login status and get device `online_ip`
         login_status = get_login_status(client=self.client)
         self.ip = login_status.get("online_ip")
         self.logged_in_user = login_status.get("user_name")
 
         # Validate if current logged in user matches the provided username
         if self.logged_in_user and self.logged_in_user != self.username:
-            raise Exception(
+            warn(
                 f"Current logged in user ({self.logged_in_user}) and "
-                f"yours ({self.username}) does not match"
+                f"yours ({self.username}) does not match. "
+                "Most likely bitsrun will work fine, "
+                "but that may differ from what you really want.",
+                stacklevel=1,
             )
 
     def login(self) -> UserResponseType:
         # Raise exception if device is already logged in
         if self.logged_in_user == self.username:
             raise Exception(f"{self.logged_in_user}, you are already online")
 
@@ -117,15 +121,17 @@
 
         # Logout params contain only the following fields
         params = {
             "callback": "jsonp",
             "action": "logout",
             "ac_id": self.acid,
             "ip": self.ip,
-            "username": self.username,
+            "username": self.logged_in_user,
+            # `logged_in_user` may differ from `username`.
+            # Anyway, we can logout without password.
         }
         response = self.client.get("/cgi-bin/srun_portal", params=params)
         return json.loads(response.text[6:-1])
 
     def _get_token(self) -> str:
         """Get challenge token for login authentication."""
         params = {"callback": "jsonp", "username": self.username, "ip": self.ip}
```

### Comparing `bitsrun-3.5.1/bitsrun/utils.py` & `bitsrun-3.5.2/bitsrun/utils.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.1/pyproject.toml` & `bitsrun-3.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "bitsrun"
-version = "3.5.1"
+version = "3.5.2"
 description = "A headless login / logout script for 10.0.0.55"
 authors = [
     { name = "spencerwooo", email = "spencer.woo@outlook.com" },
 ]
 dependencies = [
-    "httpx>=0.23.3",
-    "rich>=13.3.1",
+    "httpx>=0.24.0",
+    "rich>=13.3.5",
     "humanize>=4.5.0",
     "click>=8.1.3",
     "platformdirs>=2.6.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
@@ -46,17 +46,17 @@
 
 [project.scripts]
 bitsrun = "bitsrun.cli:cli"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=23.3.0",
-    "ruff>=0.0.260",
-    "mypy>=1.1.1",
-    "pre-commit>=3.2.2",
+    "ruff>=0.0.265",
+    "mypy>=1.2.0",
+    "pre-commit>=3.3.1",
 ]
 
 [tool.pdm.build]
 includes = []
 
 [tool.pdm.scripts]
 lint = "pre-commit run --all-files"
```

### Comparing `bitsrun-3.5.1/PKG-INFO` & `bitsrun-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitsrun
-Version: 3.5.1
+Version: 3.5.2
 Summary: A headless login / logout script for 10.0.0.55
 License: WTFPL
 Keywords: bit,srun,srun-login,srun-client,beijing-institute-of-technology
 Author-email: spencerwooo <spencer.woo@outlook.com>
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

