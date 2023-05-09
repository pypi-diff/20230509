# Comparing `tmp/latch_config-0.1.2.tar.gz` & `tmp/latch_config-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_config-0.1.2.tar", max compression
+gzip compressed data, was "latch_config-0.1.3.tar", max compression
```

## Comparing `latch_config-0.1.2.tar` & `latch_config-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.2/LICENSE
--rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.2/README.md
--rw-r--r--   0        0        0     2238 2023-04-28 21:10:22.580571 latch_config-0.1.2/latch_config/config.py
--rw-r--r--   0        0        0      782 2023-04-28 21:10:40.091123 latch_config-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.2/setup.py
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     7052 2023-04-27 16:58:00.656170 latch_config-0.1.3/LICENSE
+-rw-r--r--   0        0        0       16 2023-04-27 16:43:12.678337 latch_config-0.1.3/README.md
+-rw-r--r--   0        0        0     2238 2023-04-28 21:10:22.580571 latch_config-0.1.3/latch_config/config.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:28:54.229755 latch_config-0.1.3/latch_config/py.typed
+-rw-r--r--   0        0        0      782 2023-05-09 16:29:26.173618 latch_config-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 latch_config-0.1.3/setup.py
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 latch_config-0.1.3/PKG-INFO
```

### Comparing `latch_config-0.1.2/LICENSE` & `latch_config-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latch_config-0.1.2/latch_config/config.py` & `latch_config-0.1.3/latch_config/config.py`

 * *Files identical despite different names*

### Comparing `latch_config-0.1.2/pyproject.toml` & `latch_config-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-config"
-version = "0.1.2"
+version = "0.1.3"
 description = "Shared config for latch python backend services"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_config"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_config-0.1.2/setup.py` & `latch_config-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['latch_config']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'latch-config',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Shared config for latch python backend services',
     'long_description': '# python-config\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

