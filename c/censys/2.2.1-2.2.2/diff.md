# Comparing `tmp/censys-2.2.1.tar.gz` & `tmp/censys-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censys-2.2.1.tar", max compression
+gzip compressed data, was "censys-2.2.2.tar", max compression
```

## Comparing `censys-2.2.1.tar` & `censys-2.2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    10174 2023-05-08 20:59:03.417712 censys-2.2.1/LICENSE
--rw-r--r--   0        0        0     4466 2023-05-08 20:59:03.417712 censys-2.2.1/README.md
--rw-r--r--   0        0        0       91 2023-05-08 20:59:03.417712 censys-2.2.1/censys/__main__.py
--rw-r--r--   0        0        0      633 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/__init__.py
--rw-r--r--   0        0        0     3474 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/api.py
--rw-r--r--   0        0        0      410 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/__init__.py
--rw-r--r--   0        0        0     5900 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/assets.py
--rw-r--r--   0        0        0      424 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/certificates.py
--rw-r--r--   0        0        0     1118 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/domains.py
--rw-r--r--   0        0        0      389 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/hosts.py
--rw-r--r--   0        0        0     2075 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/subdomains.py
--rw-r--r--   0        0        0     1775 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/assets/web_entities.py
--rw-r--r--   0        0        0     1598 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/client.py
--rw-r--r--   0        0        0     2380 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/clouds.py
--rw-r--r--   0        0        0     2519 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/events.py
--rw-r--r--   0        0        0     2482 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/inventory.py
--rw-r--r--   0        0        0     3981 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/risks.py
--rw-r--r--   0        0        0     2784 2023-05-08 20:59:03.417712 censys-2.2.1/censys/asm/seeds.py
--rw-r--r--   0        0        0      675 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/__init__.py
--rw-r--r--   0        0        0     1901 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/args.py
--rw-r--r--   0        0        0      174 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/__init__.py
--rw-r--r--   0        0        0     2045 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/account.py
--rw-r--r--   0        0        0     6793 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/asm.py
--rw-r--r--   0        0        0     3171 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/config.py
--rw-r--r--   0        0        0     5526 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/hnri.py
--rw-r--r--   0        0        0     6603 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/search.py
--rw-r--r--   0        0        0     3492 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/subdomains.py
--rw-r--r--   0        0        0     3760 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/commands/view.py
--rw-r--r--   0        0        0   233252 2023-05-08 20:59:03.417712 censys-2.2.1/censys/cli/data/certificates_autocomplete.json
--rw-r--r--   0        0        0   324545 2023-05-08 20:59:03.421712 censys-2.2.1/censys/cli/data/hosts_autocomplete.json
--rw-r--r--   0        0        0     3279 2023-05-08 20:59:03.421712 censys-2.2.1/censys/cli/utils.py
--rw-r--r--   0        0        0      105 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/__init__.py
--rw-r--r--   0        0        0     8552 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/base.py
--rw-r--r--   0        0        0     1690 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/config.py
--rw-r--r--   0        0        0     1106 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/deprecation.py
--rw-r--r--   0        0        0    12446 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/exceptions.py
--rw-r--r--   0        0        0      144 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/types.py
--rw-r--r--   0        0        0      453 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/utils.py
--rw-r--r--   0        0        0      242 2023-05-08 20:59:03.421712 censys-2.2.1/censys/common/version.py
--rw-r--r--   0        0        0        0 2023-05-08 20:59:03.421712 censys-2.2.1/censys/py.typed
--rw-r--r--   0        0        0      375 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/__init__.py
--rw-r--r--   0        0        0     2133 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/client.py
--rw-r--r--   0        0        0      169 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/__init__.py
--rw-r--r--   0        0        0     5805 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/api.py
--rw-r--r--   0        0        0     1830 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/certificates.py
--rw-r--r--   0        0        0     1224 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v1/data.py
--rw-r--r--   0        0        0      151 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/__init__.py
--rw-r--r--   0        0        0    17200 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/api.py
--rw-r--r--   0        0        0    12823 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/certs.py
--rw-r--r--   0        0        0    10570 2023-05-08 20:59:03.421712 censys-2.2.1/censys/search/v2/hosts.py
--rw-r--r--   0        0        0     3365 2023-05-08 20:59:03.425712 censys-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     7080 1970-01-01 00:00:00.000000 censys-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-05-09 14:00:31.082041 censys-2.2.2/LICENSE
+-rw-r--r--   0        0        0     4466 2023-05-09 14:00:31.082041 censys-2.2.2/README.md
+-rw-r--r--   0        0        0       91 2023-05-09 14:00:31.082041 censys-2.2.2/censys/__main__.py
+-rw-r--r--   0        0        0      633 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/__init__.py
+-rw-r--r--   0        0        0     3474 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/api.py
+-rw-r--r--   0        0        0      410 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/__init__.py
+-rw-r--r--   0        0        0     5900 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/assets.py
+-rw-r--r--   0        0        0      424 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/certificates.py
+-rw-r--r--   0        0        0     1118 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/domains.py
+-rw-r--r--   0        0        0      389 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/hosts.py
+-rw-r--r--   0        0        0     2075 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/subdomains.py
+-rw-r--r--   0        0        0     1775 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/assets/web_entities.py
+-rw-r--r--   0        0        0     1598 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/client.py
+-rw-r--r--   0        0        0     2380 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/clouds.py
+-rw-r--r--   0        0        0     2519 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/events.py
+-rw-r--r--   0        0        0     2482 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/inventory.py
+-rw-r--r--   0        0        0     3981 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/risks.py
+-rw-r--r--   0        0        0     2784 2023-05-09 14:00:31.082041 censys-2.2.2/censys/asm/seeds.py
+-rw-r--r--   0        0        0      675 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/__init__.py
+-rw-r--r--   0        0        0     1901 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/args.py
+-rw-r--r--   0        0        0      174 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2045 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/account.py
+-rw-r--r--   0        0        0     6793 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/asm.py
+-rw-r--r--   0        0        0     3171 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/config.py
+-rw-r--r--   0        0        0     5526 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/hnri.py
+-rw-r--r--   0        0        0     6603 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/search.py
+-rw-r--r--   0        0        0     3492 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/subdomains.py
+-rw-r--r--   0        0        0     3760 2023-05-09 14:00:31.082041 censys-2.2.2/censys/cli/commands/view.py
+-rw-r--r--   0        0        0   233252 2023-05-09 14:00:31.086041 censys-2.2.2/censys/cli/data/certificates_autocomplete.json
+-rw-r--r--   0        0        0   324545 2023-05-09 14:00:31.086041 censys-2.2.2/censys/cli/data/hosts_autocomplete.json
+-rw-r--r--   0        0        0     3279 2023-05-09 14:00:31.086041 censys-2.2.2/censys/cli/utils.py
+-rw-r--r--   0        0        0      105 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/__init__.py
+-rw-r--r--   0        0        0     8552 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/base.py
+-rw-r--r--   0        0        0     1690 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/config.py
+-rw-r--r--   0        0        0     1106 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/deprecation.py
+-rw-r--r--   0        0        0    12446 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/exceptions.py
+-rw-r--r--   0        0        0      144 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/types.py
+-rw-r--r--   0        0        0      453 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/utils.py
+-rw-r--r--   0        0        0      242 2023-05-09 14:00:31.086041 censys-2.2.2/censys/common/version.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:00:31.086041 censys-2.2.2/censys/py.typed
+-rw-r--r--   0        0        0      375 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/__init__.py
+-rw-r--r--   0        0        0     2133 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/client.py
+-rw-r--r--   0        0        0      169 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/__init__.py
+-rw-r--r--   0        0        0     5805 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/api.py
+-rw-r--r--   0        0        0     1830 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/certificates.py
+-rw-r--r--   0        0        0     1224 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v1/data.py
+-rw-r--r--   0        0        0      151 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/__init__.py
+-rw-r--r--   0        0        0    17200 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/api.py
+-rw-r--r--   0        0        0    12823 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/certs.py
+-rw-r--r--   0        0        0    10570 2023-05-09 14:00:31.086041 censys-2.2.2/censys/search/v2/hosts.py
+-rw-r--r--   0        0        0     3449 2023-05-09 14:00:31.090041 censys-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7112 1970-01-01 00:00:00.000000 censys-2.2.2/PKG-INFO
```

### Comparing `censys-2.2.1/LICENSE` & `censys-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/README.md` & `censys-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/__init__.py` & `censys-2.2.2/censys/asm/__init__.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/api.py` & `censys-2.2.2/censys/asm/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/assets/assets.py` & `censys-2.2.2/censys/asm/assets/assets.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/assets/domains.py` & `censys-2.2.2/censys/asm/assets/domains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/assets/subdomains.py` & `censys-2.2.2/censys/asm/assets/subdomains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/assets/web_entities.py` & `censys-2.2.2/censys/asm/assets/web_entities.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/client.py` & `censys-2.2.2/censys/asm/client.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/clouds.py` & `censys-2.2.2/censys/asm/clouds.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/events.py` & `censys-2.2.2/censys/asm/events.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/inventory.py` & `censys-2.2.2/censys/asm/inventory.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/risks.py` & `censys-2.2.2/censys/asm/risks.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/asm/seeds.py` & `censys-2.2.2/censys/asm/seeds.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/__init__.py` & `censys-2.2.2/censys/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/args.py` & `censys-2.2.2/censys/cli/args.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/commands/account.py` & `censys-2.2.2/censys/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/commands/asm.py` & `censys-2.2.2/censys/cli/commands/asm.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/commands/config.py` & `censys-2.2.2/censys/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/commands/hnri.py` & `censys-2.2.2/censys/cli/commands/hnri.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/commands/search.py` & `censys-2.2.2/censys/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/commands/subdomains.py` & `censys-2.2.2/censys/cli/commands/subdomains.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/commands/view.py` & `censys-2.2.2/censys/cli/commands/view.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/data/certificates_autocomplete.json` & `censys-2.2.2/censys/cli/data/certificates_autocomplete.json`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/data/hosts_autocomplete.json` & `censys-2.2.2/censys/cli/data/hosts_autocomplete.json`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/cli/utils.py` & `censys-2.2.2/censys/cli/utils.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/common/base.py` & `censys-2.2.2/censys/common/base.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/common/config.py` & `censys-2.2.2/censys/common/config.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/common/deprecation.py` & `censys-2.2.2/censys/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/common/exceptions.py` & `censys-2.2.2/censys/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/search/client.py` & `censys-2.2.2/censys/search/client.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/search/v1/api.py` & `censys-2.2.2/censys/search/v1/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/search/v1/certificates.py` & `censys-2.2.2/censys/search/v1/certificates.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/search/v1/data.py` & `censys-2.2.2/censys/search/v1/data.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/search/v2/api.py` & `censys-2.2.2/censys/search/v2/api.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/search/v2/certs.py` & `censys-2.2.2/censys/search/v2/certs.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/censys/search/v2/hosts.py` & `censys-2.2.2/censys/search/v2/hosts.py`

 * *Files identical despite different names*

### Comparing `censys-2.2.1/pyproject.toml` & `censys-2.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censys"
-version = "2.2.1"
+version = "2.2.2"
 description = "An easy-to-use and lightweight API wrapper for Censys APIs (censys.io)."
 authors = ["Censys, Inc. <support@censys.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = ["censys/py.typed"]
 keywords = ["censys", "api", "search", "attack surface management"]
 classifiers = [
@@ -49,18 +49,19 @@
 
 [tool.poetry.scripts]
 censys = "censys.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4.0.0"
 requests = ">=2.29.0"
-backoff = "^2.0.1"
+urllib3 = "<2.0.0" # Waiting until requests supports urllib3>=2.0.0
+backoff = ">=2.0.0,<3.0.0"
 rich = ">=10.16.2"
 importlib-metadata = { version = "*", python = "<3.8" }
-argcomplete = "^3.0.8"
+argcomplete = ">=2.0.0,<4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 # Lint
 black = "^23.3.0"
 blacken-docs = "^1.13.0"
 darglint = "^1.8.1"
 flake8 = "^5.0.4"
```

### Comparing `censys-2.2.1/PKG-INFO` & `censys-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censys
-Version: 2.2.1
+Version: 2.2.2
 Summary: An easy-to-use and lightweight API wrapper for Censys APIs (censys.io).
 License: Apache-2.0
 Keywords: censys,api,search,attack surface management
 Author: Censys, Inc.
 Author-email: support@censys.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -36,19 +36,20 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: argcomplete (>=3.0.8,<4.0.0)
-Requires-Dist: backoff (>=2.0.1,<3.0.0)
+Requires-Dist: argcomplete (>=2.0.0,<4.0.0)
+Requires-Dist: backoff (>=2.0.0,<3.0.0)
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: requests (>=2.29.0)
 Requires-Dist: rich (>=10.16.2)
+Requires-Dist: urllib3 (<2.0.0)
 Project-URL: Censys Homepage, https://censys.io/
 Project-URL: Censys Search, https://search.censys.io/
 Project-URL: Changelog, https://github.com/censys/censys-python/releases
 Project-URL: Discussions, https://github.com/censys/censys-python/discussions
 Project-URL: Documentation, https://censys-python.rtfd.io
 Project-URL: Source, https://github.com/censys/censys-python
 Project-URL: Tracker, https://github.com/censys/censys-python/issues
```

