# Comparing `tmp/conda_pip_minimal-0.2.0.tar.gz` & `tmp/conda_pip_minimal-0.2.1.tar.gz`

## Comparing `conda_pip_minimal-0.2.0.tar` & `conda_pip_minimal-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/__main__.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/cli.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/cmd.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/conda_env.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/deps.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/export.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/logging.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/min.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/result_capture.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/conda_pip_minimal/version.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/.gitignore
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/README.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/__main__.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/cli.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/cmd.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/conda_env.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/deps.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/export.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/logging.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/min.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/result_capture.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/conda_pip_minimal/version.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/.gitignore
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/README.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 conda_pip_minimal-0.2.1/PKG-INFO
```

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/cli.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/cli.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/cmd.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/cmd.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/conda_env.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/conda_env.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/deps.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     cmd: Cmd, args: List[str], min_version: Version
 ) -> Version:
     try:
         version = extract_semver(await cmd(args))
     except subprocess.CalledProcessError:
         raise EnsureCmdError(f"Could not ensure {cmd=} {args=}")
 
-    if not version.is_compatible(min_version):
+    if not min_version.is_compatible(version):
         raise EnsureCmdError(
             f"Could not ensure {cmd=}, {min_version=}, found {version=}"
         )
 
     return version
```

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/export.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/export.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/logging.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/logging.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/min.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/min.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/result_capture.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/result_capture.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/conda_pip_minimal/version.py` & `conda_pip_minimal-0.2.1/conda_pip_minimal/version.py`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/README.md` & `conda_pip_minimal-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/pyproject.toml` & `conda_pip_minimal-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conda_pip_minimal-0.2.0/PKG-INFO` & `conda_pip_minimal-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-pip-minimal
-Version: 0.2.0
+Version: 0.2.1
 Summary: Conda+Pip minimal env exports
 Project-URL: Homepage, https://github.com/indigoviolet/conda-pip-minimal
 Author-email: Venky Iyer <indigoviolet@gmail.com>
 License-Expression: MIT
 Keywords: conda,environment.yaml,packaging,pip
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

