# Comparing `tmp/ansys-tools-path-0.2.0.tar.gz` & `tmp/ansys-tools-path-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-tools-path-0.2.0.tar", last modified: Fri May  5 11:29:55 2023, max compression
+gzip compressed data, was "ansys-tools-path-0.2.1.tar", last modified: Tue May  9 15:14:34 2023, max compression
```

## Comparing `ansys-tools-path-0.2.0.tar` & `ansys-tools-path-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-05-05 11:29:42.712175 ansys-tools-path-0.2.0/LICENSE
--rw-r--r--   0        0        0     4701 2023-05-05 11:29:42.712175 ansys-tools-path-0.2.0/README.rst
--rw-r--r--   0        0        0     1849 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      919 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      648 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    25880 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4701 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/README.rst
+-rw-r--r--   0        0        0     1849 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      919 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      648 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    25892 2023-05-09 15:14:18.238790 ansys-tools-path-0.2.1/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.2.1/PKG-INFO
```

### Comparing `ansys-tools-path-0.2.0/LICENSE` & `ansys-tools-path-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.0/README.rst` & `ansys-tools-path-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.0/pyproject.toml` & `ansys-tools-path-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys-tools-path-0.2.0/src/ansys/tools/path/__init__.py` & `ansys-tools-path-0.2.1/src/ansys/tools/path/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.0/src/ansys/tools/path/misc.py` & `ansys-tools-path-0.2.1/src/ansys/tools/path/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.2.0/src/ansys/tools/path/path.py` & `ansys-tools-path-0.2.1/src/ansys/tools/path/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -672,15 +672,15 @@
     old_settings_dir = appdirs.user_data_dir(f"ansys_{product_name}_core")
     old_config_file = os.path.join(old_settings_dir, old_config_file_name)
     if os.path.isfile(old_config_file):
         with open(old_config_file) as f:
             exe_loc = f.read()
 
         if os.path.isfile(CONFIG_FILE):
-            new_config_data = _read_config_file()
+            new_config_data = _read_config_file(product_name)
         else:
             new_config_data = {}
         new_config_data[product_name] = exe_loc
         _write_config_file(new_config_data)
         os.remove(old_config_file)
```

### Comparing `ansys-tools-path-0.2.0/PKG-INFO` & `ansys-tools-path-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

