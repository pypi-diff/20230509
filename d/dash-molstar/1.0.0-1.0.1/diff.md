# Comparing `tmp/dash_molstar-1.0.0.tar.gz` & `tmp/dash_molstar-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_molstar-1.0.0.tar", last modified: Thu May  4 07:10:41 2023, max compression
+gzip compressed data, was "dash_molstar-1.0.1.tar", last modified: Tue May  9 01:05:50 2023, max compression
```

## Comparing `dash_molstar-1.0.0.tar` & `dash_molstar-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 07:10:41.380555 dash_molstar-1.0.0/
--rw-r--r--   0 simon      (501) staff       (20)    26526 2023-02-27 01:41:14.000000 dash_molstar-1.0.0/LICENSE
--rw-r--r--   0 simon      (501) staff       (20)      353 2023-02-15 14:31:58.000000 dash_molstar-1.0.0/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)      223 2023-05-04 07:10:41.378897 dash_molstar-1.0.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    13617 2023-05-04 03:52:14.000000 dash_molstar-1.0.0/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 07:10:41.372597 dash_molstar-1.0.0/dash_molstar/
--rw-r--r--   0 simon      (501) staff       (20)     1986 2023-04-24 08:48:00.000000 dash_molstar-1.0.0/dash_molstar/MolstarViewer.py
--rw-r--r--   0 simon      (501) staff       (20)     2373 2023-02-23 05:26:42.000000 dash_molstar-1.0.0/dash_molstar/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)       75 2023-04-24 08:48:00.000000 dash_molstar-1.0.0/dash_molstar/_imports_.py
--rw-r--r--   0 simon      (501) staff       (20)    82526 2023-04-24 08:47:58.000000 dash_molstar-1.0.0/dash_molstar/dash_molstar.min.js
--rw-r--r--   0 simon      (501) staff       (20)       96 2023-04-24 08:47:58.000000 dash_molstar-1.0.0/dash_molstar/dash_molstar.min.js.map
--rw-r--r--   0 simon      (501) staff       (20)     3523 2023-04-24 08:48:00.000000 dash_molstar-1.0.0/dash_molstar/metadata.json
--rw-r--r--   0 simon      (501) staff       (20)     2077 2023-05-04 03:57:40.000000 dash_molstar-1.0.0/dash_molstar/package-info.json
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 07:10:41.376995 dash_molstar-1.0.0/dash_molstar/utils/
--rw-r--r--   0 simon      (501) staff       (20)       28 2023-02-27 04:32:33.000000 dash_molstar-1.0.0/dash_molstar/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6526 2023-04-24 06:36:09.000000 dash_molstar-1.0.0/dash_molstar/utils/molstar_helper.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-04 07:10:41.375756 dash_molstar-1.0.0/dash_molstar.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)      223 2023-05-04 07:10:41.000000 dash_molstar-1.0.0/dash_molstar.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      472 2023-05-04 07:10:41.000000 dash_molstar-1.0.0/dash_molstar.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-04 07:10:41.000000 dash_molstar-1.0.0/dash_molstar.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       13 2023-05-04 07:10:41.000000 dash_molstar-1.0.0/dash_molstar.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)     2077 2023-05-04 03:56:31.000000 dash_molstar-1.0.0/package.json
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-04 07:10:41.381034 dash_molstar-1.0.0/setup.cfg
--rw-r--r--   0 simon      (501) staff       (20)      556 2023-05-04 05:12:31.000000 dash_molstar-1.0.0/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 01:05:50.141266 dash_molstar-1.0.1/
+-rw-r--r--   0 simon      (501) staff       (20)    26526 2023-02-27 01:41:14.000000 dash_molstar-1.0.1/LICENSE
+-rw-r--r--   0 simon      (501) staff       (20)      353 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)      223 2023-05-09 01:05:50.140816 dash_molstar-1.0.1/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    13735 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 01:05:50.125503 dash_molstar-1.0.1/dash_molstar/
+-rw-r--r--   0 simon      (501) staff       (20)     1986 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/MolstarViewer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2373 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)       75 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/_imports_.py
+-rw-r--r--   0 simon      (501) staff       (20)    82526 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/dash_molstar.min.js
+-rw-r--r--   0 simon      (501) staff       (20)       96 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/dash_molstar.min.js.map
+-rw-r--r--   0 simon      (501) staff       (20)     3523 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/metadata.json
+-rw-r--r--   0 simon      (501) staff       (20)     2077 2023-05-09 01:02:12.000000 dash_molstar-1.0.1/dash_molstar/package-info.json
+-rw-r--r--   0 simon      (501) staff       (20)  5791504 2023-05-09 01:02:39.000000 dash_molstar-1.0.1/dash_molstar/rcsb-molstar.js
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 01:05:50.139782 dash_molstar-1.0.1/dash_molstar/utils/
+-rw-r--r--   0 simon      (501) staff       (20)       28 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6526 2023-05-04 07:28:17.000000 dash_molstar-1.0.1/dash_molstar/utils/molstar_helper.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-09 01:05:50.138840 dash_molstar-1.0.1/dash_molstar.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)      223 2023-05-09 01:05:50.000000 dash_molstar-1.0.1/dash_molstar.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      501 2023-05-09 01:05:50.000000 dash_molstar-1.0.1/dash_molstar.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-09 01:05:50.000000 dash_molstar-1.0.1/dash_molstar.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       13 2023-05-09 01:05:50.000000 dash_molstar-1.0.1/dash_molstar.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)     2077 2023-05-09 01:00:55.000000 dash_molstar-1.0.1/package.json
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-09 01:05:50.141372 dash_molstar-1.0.1/setup.cfg
+-rw-r--r--   0 simon      (501) staff       (20)      575 2023-05-09 00:57:30.000000 dash_molstar-1.0.1/setup.py
```

### Comparing `dash_molstar-1.0.0/LICENSE` & `dash_molstar-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_molstar-1.0.0/README.md` & `dash_molstar-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,20 @@
     ),
 )
 
 if __name__ == '__main__':
     app.run_server(debug=True)
 ```
 
+Clone the repository to your local directory and run the following command to see the demo:
+
+```
+python usage.py
+```
+
 ## Parameters
 
 Parameters for `MolstarViewer` include `id`, `data`, `focus`, `layout`, `selection` and `style`.
 
 - `id` is the id for the html container of molstar, and should be unique in `app.layout`.
 
 - `data` is the molecule to be loaded into molstar viewer. It is a `dict` or list of dicts, each containing a molecule to be loaded. With helper function `parse_molecule`, one can easily generate correct data for this parameter. `data` can include additional components to be shown in the viewer. The component data should be generated by the helper function `create_component`.
```

### Comparing `dash_molstar-1.0.0/dash_molstar/MolstarViewer.py` & `dash_molstar-1.0.1/dash_molstar/MolstarViewer.py`

 * *Files identical despite different names*

### Comparing `dash_molstar-1.0.0/dash_molstar/__init__.py` & `dash_molstar-1.0.1/dash_molstar/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_molstar-1.0.0/dash_molstar/dash_molstar.min.js` & `dash_molstar-1.0.1/dash_molstar/dash_molstar.min.js`

 * *Files identical despite different names*

### Comparing `dash_molstar-1.0.0/dash_molstar/metadata.json` & `dash_molstar-1.0.1/dash_molstar/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_molstar-1.0.0/dash_molstar/package-info.json` & `dash_molstar-1.0.1/dash_molstar/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -52,9 +52,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_molstar -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `dash_molstar-1.0.0/dash_molstar/utils/molstar_helper.py` & `dash_molstar-1.0.1/dash_molstar/utils/molstar_helper.py`

 * *Files identical despite different names*

### Comparing `dash_molstar-1.0.0/package.json` & `dash_molstar-1.0.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -52,9 +52,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_molstar -p package-info.json --r-prefix '' --jl-prefix '' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `dash_molstar-1.0.0/setup.py` & `dash_molstar-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 package_name = package["name"].replace(" ", "_").replace("-", "_")
 
 setup(
     name=package_name,
     version=package["version"],
     author=package['author'],
     packages=[package_name],
-    package_data={package_name: ['utils/*']},
+    package_data={package_name: ['utils/*', 'rcsb-molstar.js']},
     include_package_data=True,
     license=package['license'],
     description=package.get('description', package_name),
     install_requires=[],
     classifiers = [
         'Framework :: Dash',
     ],
```

