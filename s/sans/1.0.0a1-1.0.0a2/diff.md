# Comparing `tmp/sans-1.0.0a1.tar.gz` & `tmp/sans-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sans-1.0.0a1.tar", last modified: Tue May  9 02:57:07 2023, max compression
+gzip compressed data, was "sans-1.0.0a2.tar", last modified: Tue May  9 04:44:04 2023, max compression
```

## Comparing `sans-1.0.0a1.tar` & `sans-1.0.0a2.tar`

### file list

```diff
@@ -1,48 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.457871 sans-1.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.453871 sans-1.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.453871 sans-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-09 02:56:56.000000 sans-1.0.0a1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-09 02:56:56.000000 sans-1.0.0a1/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-09 02:56:56.000000 sans-1.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-09 02:56:56.000000 sans-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-09 02:56:56.000000 sans-1.0.0a1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-09 02:56:56.000000 sans-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 02:56:56.000000 sans-1.0.0a1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-09 02:57:07.457871 sans-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-09 02:56:56.000000 sans-1.0.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.453871 sans-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/__init__.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/objects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 02:56:56.000000 sans-1.0.0a1/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-09 02:56:56.000000 sans-1.0.0a1/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-09 02:56:56.000000 sans-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 02:56:56.000000 sans-1.0.0a1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.457871 sans-1.0.0a1/sans/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-09 02:56:56.000000 sans-1.0.0a1/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 02:57:07.457871 sans-1.0.0a1/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 02:57:07.000000 sans-1.0.0a1/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 02:57:07.457871 sans-1.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 02:56:56.000000 sans-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:04.554112 sans-1.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:04.550111 sans-1.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:04.550111 sans-1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-09 04:43:52.000000 sans-1.0.0a2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-09 04:43:52.000000 sans-1.0.0a2/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-09 04:43:52.000000 sans-1.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-09 04:43:52.000000 sans-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-09 04:43:52.000000 sans-1.0.0a2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-09 04:43:52.000000 sans-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-09 04:44:04.554112 sans-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-09 04:43:52.000000 sans-1.0.0a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:04.550111 sans-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/objects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 04:43:52.000000 sans-1.0.0a2/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-09 04:43:52.000000 sans-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-09 04:43:52.000000 sans-1.0.0a2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:04.554112 sans-1.0.0a2/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23030 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-09 04:43:52.000000 sans-1.0.0a2/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:04.554112 sans-1.0.0a2/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-09 04:44:04.000000 sans-1.0.0a2/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-09 04:44:04.000000 sans-1.0.0a2/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:44:04.000000 sans-1.0.0a2/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 04:44:04.000000 sans-1.0.0a2/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-09 04:44:04.000000 sans-1.0.0a2/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 04:44:04.000000 sans-1.0.0a2/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 04:44:04.554112 sans-1.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 04:43:52.000000 sans-1.0.0a2/setup.py
```

### Comparing `sans-1.0.0a1/.github/workflows/codeql-analysis.yml` & `sans-1.0.0a2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/.github/workflows/pythonpublish.yml` & `sans-1.0.0a2/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/.gitignore` & `sans-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/.pre-commit-config.yaml` & `sans-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/LICENSE` & `sans-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/PKG-INFO` & `sans-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sans-1.0.0a1/README.rst` & `sans-1.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/docs/Makefile` & `sans-1.0.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/docs/conf.py` & `sans-1.0.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/docs/make.bat` & `sans-1.0.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/pyproject.toml` & `sans-1.0.0a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/__init__.py` & `sans-1.0.0a2/sans/__init__.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/__main__.py` & `sans-1.0.0a2/sans/__main__.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/_state.py` & `sans-1.0.0a2/sans/_state.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/client.py` & `sans-1.0.0a2/sans/client.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/client.pyi` & `sans-1.0.0a2/sans/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -718,43 +718,43 @@
 ) -> Iterator[Response]: ...
 def get(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes = ...,
+    auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 def options(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes = ...,
+    auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
 def head(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes = ...,
+    auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
@@ -814,15 +814,15 @@
 ) -> Response: ...
 def delete(
     url: URLTypes,
     *,
     params: QueryParamTypes = ...,
     headers: HeaderTypes = ...,
     cookies: CookieTypes = ...,
-    auth: AuthTypes = ...,
+    auth: RateLimiter = ...,
     proxies: ProxiesTypes = ...,
     follow_redirects: bool = ...,
     cert: CertTypes = ...,
     verify: VerifyTypes = ...,
     timeout: TimeoutTypes = ...,
     trust_env: bool = ...,
 ) -> Response: ...
```

### Comparing `sans-1.0.0a1/sans/decoder.py` & `sans-1.0.0a2/sans/decoder.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/errors.py` & `sans-1.0.0a2/sans/errors.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/limiter.py` & `sans-1.0.0a2/sans/limiter.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/lock.py` & `sans-1.0.0a2/sans/lock.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/request.py` & `sans-1.0.0a2/sans/request.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/response.py` & `sans-1.0.0a2/sans/response.py`

 * *Files identical despite different names*

### Comparing `sans-1.0.0a1/sans/utils.py` & `sans-1.0.0a2/sans/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     response = await client.send(request)
     token: str = response.xml.find("TOKEN").text  # type: ignore
     request = Request(*shards, **parameters, mode="execute", token=token)
     return await client.send(request)
 
 
 if sys.version_info < (3, 9):
-
+    # from: https://stackoverflow.com/a/4590052
     def indent(
         tree: etree.Element | etree.ElementTree,
         space: str = "  ",
         level: int = 0,
         *,
         _parent: etree.Element | None = None,
         _index: int = -1,
```

### Comparing `sans-1.0.0a1/sans.egg-info/PKG-INFO` & `sans-1.0.0a2/sans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sans-1.0.0a1/sans.egg-info/SOURCES.txt` & `sans-1.0.0a2/sans.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
 LICENSE
-Makefile
 README.rst
-make.bat
 pyproject.toml
 requirements.txt
 setup.py
 .github/workflows/codeql-analysis.yml
 .github/workflows/pythonpublish.yml
 docs/Makefile
 docs/__init__.rst
```

