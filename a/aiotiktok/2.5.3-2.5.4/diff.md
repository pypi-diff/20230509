# Comparing `tmp/aiotiktok-2.5.3.tar.gz` & `tmp/aiotiktok-2.5.4.tar.gz`

## Comparing `aiotiktok-2.5.3.tar` & `aiotiktok-2.5.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/__init__.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/client.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/exceptions.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/aiotiktok/types.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/LICENSE
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/README.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiotiktok-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/__init__.py
+-rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/client.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/exceptions.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/extractors.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/aiotiktok/types.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/LICENSE
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/README.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiotiktok-2.5.4/PKG-INFO
```

### Comparing `aiotiktok-2.5.3/aiotiktok/types.py` & `aiotiktok-2.5.4/aiotiktok/types.py`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.5.3/.gitignore` & `aiotiktok-2.5.4/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 main.py
+.idea
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
```

### Comparing `aiotiktok-2.5.3/LICENSE` & `aiotiktok-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.5.3/README.md` & `aiotiktok-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.5.3/pyproject.toml` & `aiotiktok-2.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiotiktok-2.5.3/PKG-INFO` & `aiotiktok-2.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotiktok
-Version: 2.5.3
+Version: 2.5.4
 Summary: Tool for parse tiktok data
 Project-URL: Homepage, https://github.com/sheldygg/aiotiktok
 Author: sheldy
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

